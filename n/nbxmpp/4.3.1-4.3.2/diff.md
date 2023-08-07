# Comparing `tmp/nbxmpp-4.3.1.tar.gz` & `tmp/nbxmpp-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbxmpp-4.3.1.tar", last modified: Sun May 28 21:20:13 2023, max compression
+gzip compressed data, was "nbxmpp-4.3.2.tar", last modified: Mon Aug  7 21:00:18 2023, max compression
```

## Comparing `nbxmpp-4.3.1.tar` & `nbxmpp-4.3.2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/
--rw-rw-rw-   0 worker    (1000) worker    (1000)    35147 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/COPYING
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8302 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/ChangeLog
--rw-rw-rw-   0 worker    (1000) worker    (1000)       91 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/MANIFEST.in
--rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/PKG-INFO
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1135 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/README.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.251864 nbxmpp-4.3.1/nbxmpp/
--rw-rw-rw-   0 worker    (1000) worker    (1000)      138 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/nbxmpp/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8454 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/addresses.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1961 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/c14n.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    29929 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/client.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4447 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/connection.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14689 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/const.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    19830 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/dispatcher.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4962 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/errors.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      820 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/exceptions.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    19012 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/nbxmpp/http.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    18504 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/idlequeue.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.271866 nbxmpp-4.3.1/nbxmpp/modules/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3692 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/activity.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6961 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/adhoc.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3618 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/annotations.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1706 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/attention.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1469 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/base.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2496 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bits_of_binary.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5103 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/blocking.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.275866 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4130 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/native_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3379 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/pep_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1990 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/private_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5394 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1945 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/captcha.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1984 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/chat_markers.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2009 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/chatstates.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1847 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/correction.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    20214 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/dataforms.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6166 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/date_and_time.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4020 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/delay.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1980 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/delimiter.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4612 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/discovery.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1740 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/eme.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3837 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/entity_caps.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3983 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/entity_time.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2011 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/http_auth.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2899 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/http_upload.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5934 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/ibb.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1875 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/idle.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2101 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/iq.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3286 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/last_activity.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2888 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/location.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6373 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/mam.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4265 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/message.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4348 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/misc.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3099 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/mood.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.275866 nbxmpp-4.3.1/nbxmpp/modules/muc/
--rw-rw-rw-   0 worker    (1000) worker    (1000)       21 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3478 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/moderation.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    20848 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/muc.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5726 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7370 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muclumbus.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4308 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/nickname.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    15721 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/modules/omemo.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1669 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/oob.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    13348 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/openpgp.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2180 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/pgplegacy.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1916 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/ping.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5368 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/presence.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14592 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/pubsub.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2275 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/reactions.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2986 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/receipts.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/nbxmpp/modules/register/
--rw-rw-rw-   0 worker    (1000) worker    (1000)       31 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/register/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3456 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/register/register.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4233 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/register/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3210 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/modules/replies.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5512 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/roster.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1846 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/rsm.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4789 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/security_labels.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3829 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/software_version.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2965 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/tune.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    10856 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/user_avatar.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2558 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    31943 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/vcard4.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2214 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/vcard_avatar.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4366 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/vcard_temp.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8820 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/namespaces.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    28667 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/old_dispatcher.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3549 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/plugin.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      499 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/precis.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    76385 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/protocol.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/py.typed
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14968 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/sasl.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    27907 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/simplexml.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    11907 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/smacks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8157 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/stringprep.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    34441 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/structs.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    11501 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/task.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14807 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/tcp.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/nbxmpp/third_party/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/third_party/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8903 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/third_party/hsluv.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      118 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/types.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    15519 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6873 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/nbxmpp/websocket.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1691 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/xmppiri.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.255864 nbxmpp-4.3.1/nbxmpp.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     3241 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       69 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        7 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/top_level.txt
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1120 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)       38 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/setup.cfg
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/test/
--rw-rw-rw-   0 worker    (1000) worker    (1000)      116 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/__init__.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/test/lib/
--rw-rw-rw-   0 worker    (1000) worker    (1000)      837 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/lib/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      104 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/lib/const.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1322 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/test/lib/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2706 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/lib/xmpp_mocks.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/test/unit/
--rw-rw-rw-   0 worker    (1000) worker    (1000)       54 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1975 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_activity.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2375 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_avatar.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4471 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4209 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_datetime_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1013 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_delay_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8758 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_entity_caps.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1411 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_error_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8433 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/test/unit/test_http.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7296 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/test/unit/test_jid_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4360 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_location.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1724 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_mood.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1241 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_muclumbus.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3159 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_pubsub.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4555 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_reactions.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1177 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_sasl_scram.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7729 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/test/unit/test_stringprep.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2279 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_tune.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2389 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_xml_vulnerability.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.902733 nbxmpp-4.3.2/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    35147 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/COPYING
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8701 2023-08-07 20:57:37.000000 nbxmpp-4.3.2/ChangeLog
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       91 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/MANIFEST.in
+-rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-08-07 21:00:18.902733 nbxmpp-4.3.2/PKG-INFO
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1135 2023-01-23 23:24:27.000000 nbxmpp-4.3.2/README.md
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.874731 nbxmpp-4.3.2/nbxmpp/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      138 2023-08-07 20:57:37.000000 nbxmpp-4.3.2/nbxmpp/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8454 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/addresses.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1961 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/c14n.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    29934 2023-06-30 13:30:57.000000 nbxmpp-4.3.2/nbxmpp/client.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4447 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/connection.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14689 2023-05-21 07:37:52.000000 nbxmpp-4.3.2/nbxmpp/const.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    19830 2023-02-03 15:54:25.000000 nbxmpp-4.3.2/nbxmpp/dispatcher.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4962 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/errors.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      820 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/exceptions.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    19306 2023-07-04 19:42:46.000000 nbxmpp-4.3.2/nbxmpp/http.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    18504 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/idlequeue.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.886732 nbxmpp-4.3.2/nbxmpp/modules/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3692 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/activity.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6961 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/adhoc.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3618 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/annotations.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1706 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/attention.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1469 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/base.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2496 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/bits_of_binary.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5103 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/blocking.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.890732 nbxmpp-4.3.2/nbxmpp/modules/bookmarks/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/bookmarks/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4130 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/bookmarks/native_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3379 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/bookmarks/pep_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1990 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/bookmarks/private_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5394 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/bookmarks/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1945 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/captcha.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1984 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/chat_markers.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2009 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/chatstates.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1847 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/correction.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    20214 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/dataforms.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6178 2023-06-18 20:26:26.000000 nbxmpp-4.3.2/nbxmpp/modules/date_and_time.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4020 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/delay.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1980 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/delimiter.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4612 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/discovery.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1740 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/eme.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3837 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/entity_caps.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3983 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/entity_time.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2011 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/http_auth.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2899 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/http_upload.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5934 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/ibb.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1875 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/idle.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2101 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/iq.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3286 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/last_activity.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2888 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/location.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6373 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/mam.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4944 2023-07-02 07:10:22.000000 nbxmpp-4.3.2/nbxmpp/modules/message.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4360 2023-06-18 20:26:26.000000 nbxmpp-4.3.2/nbxmpp/modules/misc.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3099 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/mood.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.890732 nbxmpp-4.3.2/nbxmpp/modules/muc/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       21 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/muc/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6282 2023-06-18 20:26:26.000000 nbxmpp-4.3.2/nbxmpp/modules/muc/moderation.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    20619 2023-06-18 20:26:26.000000 nbxmpp-4.3.2/nbxmpp/modules/muc/muc.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5726 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/muc/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     7370 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/muclumbus.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4308 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/nickname.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    15721 2023-05-10 18:13:15.000000 nbxmpp-4.3.2/nbxmpp/modules/omemo.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1669 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/oob.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    13348 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/openpgp.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2180 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/pgplegacy.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1916 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/ping.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5368 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/presence.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14592 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/pubsub.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2275 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/reactions.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2986 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/receipts.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.890732 nbxmpp-4.3.2/nbxmpp/modules/register/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       31 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/register/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3456 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/register/register.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4233 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/register/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3210 2023-02-03 15:54:25.000000 nbxmpp-4.3.2/nbxmpp/modules/replies.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5512 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/roster.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1846 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/rsm.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4948 2023-06-20 22:50:26.000000 nbxmpp-4.3.2/nbxmpp/modules/security_labels.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3829 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/software_version.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2965 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/tune.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    10856 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/user_avatar.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2558 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    31943 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/vcard4.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2214 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/vcard_avatar.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4366 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/modules/vcard_temp.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8820 2023-02-03 15:54:25.000000 nbxmpp-4.3.2/nbxmpp/namespaces.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    28667 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/old_dispatcher.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3549 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/plugin.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      499 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/precis.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    76565 2023-06-18 20:26:26.000000 nbxmpp-4.3.2/nbxmpp/protocol.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/py.typed
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14968 2023-04-23 13:45:46.000000 nbxmpp-4.3.2/nbxmpp/sasl.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    27907 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/simplexml.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    11907 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/smacks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8157 2023-02-05 14:55:00.000000 nbxmpp-4.3.2/nbxmpp/stringprep.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    34809 2023-06-20 22:50:26.000000 nbxmpp-4.3.2/nbxmpp/structs.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    11501 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/task.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14807 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/tcp.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.890732 nbxmpp-4.3.2/nbxmpp/third_party/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/third_party/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8903 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/third_party/hsluv.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      118 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/types.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    15519 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/nbxmpp/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6873 2023-05-26 20:22:05.000000 nbxmpp-4.3.2/nbxmpp/websocket.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1691 2023-04-21 14:56:16.000000 nbxmpp-4.3.2/nbxmpp/xmppiri.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.878731 nbxmpp-4.3.2/nbxmpp.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-08-07 21:00:18.000000 nbxmpp-4.3.2/nbxmpp.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     3241 2023-08-07 21:00:18.000000 nbxmpp-4.3.2/nbxmpp.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-08-07 21:00:18.000000 nbxmpp-4.3.2/nbxmpp.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       69 2023-08-07 21:00:18.000000 nbxmpp-4.3.2/nbxmpp.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        7 2023-08-07 21:00:18.000000 nbxmpp-4.3.2/nbxmpp.egg-info/top_level.txt
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1120 2023-01-23 23:24:27.000000 nbxmpp-4.3.2/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)       38 2023-08-07 21:00:18.902733 nbxmpp-4.3.2/setup.cfg
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.890732 nbxmpp-4.3.2/test/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      116 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/__init__.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.890732 nbxmpp-4.3.2/test/lib/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      837 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/lib/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      104 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/lib/const.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1322 2023-05-28 19:56:15.000000 nbxmpp-4.3.2/test/lib/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2706 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/lib/xmpp_mocks.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-08-07 21:00:18.902733 nbxmpp-4.3.2/test/unit/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       54 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1975 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_activity.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2375 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_avatar.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4471 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4209 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_datetime_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1013 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_delay_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8758 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_entity_caps.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1411 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_error_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8433 2023-05-28 19:56:15.000000 nbxmpp-4.3.2/test/unit/test_http.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     7296 2023-04-21 14:56:16.000000 nbxmpp-4.3.2/test/unit/test_jid_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4360 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_location.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1724 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_mood.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1241 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_muclumbus.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3159 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_pubsub.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4555 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_reactions.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1177 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_sasl_scram.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     7729 2023-02-05 14:55:00.000000 nbxmpp-4.3.2/test/unit/test_stringprep.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2279 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_tune.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2389 2022-12-31 20:57:12.000000 nbxmpp-4.3.2/test/unit/test_xml_vulnerability.py
```

### Comparing `nbxmpp-4.3.1/COPYING` & `nbxmpp-4.3.2/COPYING`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/ChangeLog` & `nbxmpp-4.3.2/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+nbxmpp 4.3.2 (04 Jul 2023)
+
+  New
+
+  * SecurityLabels: Add get_label_hash()
+  * JID: Add sqlite3 adapter magic method
+  * MessageProperties: Add origin_id attribute
+  * MessageProperties: Add remote_jid attribute
+
+  Improvements
+
+  * Client: Return only copy of ignored errors
+  * CommonError: Add 'by' attribute
+  * Moderation: Parse more data
+
+  Bug Fixes
+
+  * HTTP: Add set_accept_certificate()
+
 nbxmpp 4.3.1 (28 May 2023)
 
   Bug Fixes
 
   * HTTP: Abort correctly on content overflow
   * Websocket: Always set peer certificate
```

### Comparing `nbxmpp-4.3.1/PKG-INFO` & `nbxmpp-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbxmpp
-Version: 4.3.1
+Version: 4.3.2
 Summary: XMPP Library
 Author-email: Philipp Hörist <philipp@hoerist.com>, Yann Leboulanger <yann@leboulanger.org>
 License: GPL-3.0-or-later
 Project-URL: repository, https://dev.gajim.org/gajim/python-nbxmpp
 Keywords: chat,messaging,im,xmpp
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `nbxmpp-4.3.1/README.md` & `nbxmpp-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/addresses.py` & `nbxmpp-4.3.2/nbxmpp/addresses.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/c14n.py` & `nbxmpp-4.3.2/nbxmpp/c14n.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/client.py` & `nbxmpp-4.3.2/nbxmpp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         self._custom_host = (host_or_uri, protocol, type_)
 
     def set_accepted_certificates(self, certificates):
         self._accepted_certificates = certificates
 
     @property
     def ignored_tls_errors(self):
-        return self._ignored_tls_errors
+        return set(self._ignored_tls_errors)
 
     def set_ignored_tls_errors(self, errors):
         if errors is None:
             errors = set()
         self._ignored_tls_errors = errors
 
     @property
```

### Comparing `nbxmpp-4.3.1/nbxmpp/connection.py` & `nbxmpp-4.3.2/nbxmpp/connection.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/const.py` & `nbxmpp-4.3.2/nbxmpp/const.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/dispatcher.py` & `nbxmpp-4.3.2/nbxmpp/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/errors.py` & `nbxmpp-4.3.2/nbxmpp/errors.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/exceptions.py` & `nbxmpp-4.3.2/nbxmpp/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/http.py` & `nbxmpp-4.3.2/nbxmpp/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         self._input_stream: Optional[Gio.InputStream] = None
         self._output_stream: Optional[Gio.OutputStream] = None
         self._is_finished = False
         self._error: Optional[HTTPRequestError] = None
         self._is_complete = False
         self._timeout_reached = False
         self._timeout_id = None
+        self._accept_certificate_func = None
 
         self._response_body_file: Optional[Gio.File] = None
         self._response_body_data = b''
         self._body_received = False
 
         self._request_body_file: Optional[Gio.File] = None
         self._request_body_data: Optional[bytes] = None
@@ -179,14 +180,17 @@
     def cancel(self) -> None:
         if self._is_finished:
             raise ValueError('Session already finished')
 
         self._log.info('Cancel requested')
         self._cancellable.cancel()
 
+    def set_accept_certificate_func(self, func: Any) -> None:
+        self._accept_certificate_func = func
+
     def set_request_body_from_path(self, content_type: str, path: Path) -> None:
         if not path.exists():
             raise ValueError('%s does not exist' % path)
 
         if not path.is_file():
             raise ValueError('%s is not a file' % path)
 
@@ -281,14 +285,16 @@
                                       self._on_request_body_progress)
 
         self._message.connect('content-sniffed', self._on_content_sniffed)
         self._message.connect('got-body', self._on_got_body)
         self._message.connect('restarted', self._on_restarted)
         self._message.connect('finished', self._on_finished)
         self._message.connect('got-headers', self._on_got_headers)
+        if self._accept_certificate_func is not None:
+            self._message.connect('accept-certificate', self._accept_certificate_func)
 
         soup_session = self._session.get_soup_session()
         soup_session.send_async(self._message,
                                 GLib.PRIORITY_DEFAULT,
                                 self._cancellable,
                                 self._on_response)
```

### Comparing `nbxmpp-4.3.1/nbxmpp/idlequeue.py` & `nbxmpp-4.3.2/nbxmpp/idlequeue.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/activity.py` & `nbxmpp-4.3.2/nbxmpp/modules/activity.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/adhoc.py` & `nbxmpp-4.3.2/nbxmpp/modules/adhoc.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/annotations.py` & `nbxmpp-4.3.2/nbxmpp/modules/annotations.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/attention.py` & `nbxmpp-4.3.2/nbxmpp/modules/attention.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/base.py` & `nbxmpp-4.3.2/nbxmpp/modules/base.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/bits_of_binary.py` & `nbxmpp-4.3.2/nbxmpp/modules/bits_of_binary.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/blocking.py` & `nbxmpp-4.3.2/nbxmpp/modules/blocking.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/native_bookmarks.py` & `nbxmpp-4.3.2/nbxmpp/modules/bookmarks/native_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/pep_bookmarks.py` & `nbxmpp-4.3.2/nbxmpp/modules/bookmarks/pep_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/private_bookmarks.py` & `nbxmpp-4.3.2/nbxmpp/modules/bookmarks/private_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/util.py` & `nbxmpp-4.3.2/nbxmpp/modules/bookmarks/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/captcha.py` & `nbxmpp-4.3.2/nbxmpp/modules/captcha.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/chat_markers.py` & `nbxmpp-4.3.2/nbxmpp/modules/chat_markers.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/chatstates.py` & `nbxmpp-4.3.2/nbxmpp/modules/chatstates.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/correction.py` & `nbxmpp-4.3.2/nbxmpp/modules/correction.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/dataforms.py` & `nbxmpp-4.3.2/nbxmpp/modules/dataforms.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/date_and_time.py` & `nbxmpp-4.3.2/nbxmpp/modules/date_and_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     if hours in (24, -24) and minutes != 0:
         log.warning('Wrong tz string: %s', tz_string)
         return None
     return timezone(timedelta(hours=hours, minutes=minutes))
 
 
-def parse_datetime(timestring, check_utc=False,
+def parse_datetime(timestring: str | None, check_utc=False,
                    convert='utc', epoch=False):
     '''
     Parse a XEP-0082 DateTime Profile String
 
     :param timestring: a XEP-0082 DateTime profile formated string
 
     :param check_utc:  if True, returns None if timestring is not
```

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/delay.py` & `nbxmpp-4.3.2/nbxmpp/modules/delay.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/delimiter.py` & `nbxmpp-4.3.2/nbxmpp/modules/delimiter.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/discovery.py` & `nbxmpp-4.3.2/nbxmpp/modules/discovery.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/eme.py` & `nbxmpp-4.3.2/nbxmpp/modules/eme.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/entity_caps.py` & `nbxmpp-4.3.2/nbxmpp/modules/entity_caps.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/entity_time.py` & `nbxmpp-4.3.2/nbxmpp/modules/entity_time.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/http_auth.py` & `nbxmpp-4.3.2/nbxmpp/modules/http_auth.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/http_upload.py` & `nbxmpp-4.3.2/nbxmpp/modules/http_upload.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/ibb.py` & `nbxmpp-4.3.2/nbxmpp/modules/ibb.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/idle.py` & `nbxmpp-4.3.2/nbxmpp/modules/idle.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/iq.py` & `nbxmpp-4.3.2/nbxmpp/modules/iq.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/last_activity.py` & `nbxmpp-4.3.2/nbxmpp/modules/last_activity.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/location.py` & `nbxmpp-4.3.2/nbxmpp/modules/location.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/mam.py` & `nbxmpp-4.3.2/nbxmpp/modules/mam.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/message.py` & `nbxmpp-4.3.2/nbxmpp/modules/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,38 +38,56 @@
                           callback=self._process_message_after_base,
                           priority=10),
         ]
 
     def _process_message_base(self, _client, stanza, properties):
         properties.type = self._parse_type(stanza)
 
-        # Determine remote JID
         if properties.is_carbon_message and properties.carbon.is_sent:
             properties.jid = stanza.getTo()
 
         elif properties.is_mam_message and not properties.type.is_groupchat:
             own_jid = self._client.get_bound_jid()
             if own_jid.bare_match(stanza.getFrom()):
                 properties.jid = stanza.getTo()
             else:
                 properties.jid = stanza.getFrom()
 
         else:
             properties.jid = stanza.getFrom()
 
+        self._parse_if_private_message(stanza, properties)
+
+        properties.remote_jid = self._determine_remote_jid(properties)
         properties.from_ = stanza.getFrom()
         properties.to = stanza.getTo()
         properties.id = stanza.getID()
         properties.self_message = self._parse_self_message(stanza, properties)
 
+        properties.origin_id = stanza.getOriginID()
         properties.stanza_ids = self._parse_stanza_ids(stanza)
 
         if properties.type.is_error:
             properties.error = error_factory(stanza)
 
+    def _determine_remote_jid(self, properties):
+        if properties.is_muc_pm:
+            return properties.jid
+        return properties.jid.new_as_bare()
+
+    def _parse_if_private_message(self, stanza, properties) -> None:
+        muc_user = stanza.getTag('x', namespace=Namespace.MUC_USER)
+        if muc_user is None:
+            return
+
+        if (properties.type.is_chat or
+                properties.type.is_error and
+                not muc_user.getChildren()):
+            properties.muc_private_message = True
+
     def _process_message_after_base(self, _client, stanza, properties):
         # This handler runs after decryption handlers had the chance
         # to decrypt the body
         properties.body = stanza.getBody()
         properties.thread = stanza.getThread()
         properties.subject = stanza.getSubject()
         forms = stanza.getTags('x', namespace=Namespace.DATA)
```

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/misc.py` & `nbxmpp-4.3.2/nbxmpp/modules/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     frm = message.getFrom()
     if frm is None:
         message.setFrom(own_jid.bare)
 
     # Timestamp parsing
     # Most servers dont set the 'from' attr, so we cant check for it
-    delay_timestamp = parse_delay(forwarded)
+    delay_timestamp = parse_delay(forwarded, epoch=True)
     if delay_timestamp is None:
         log.warning('No timestamp on MAM message')
         log.warning(stanza)
         raise InvalidStanza
 
     return message, MAMData(id=id_,
                             query_id=query_id,
```

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/mood.py` & `nbxmpp-4.3.2/nbxmpp/modules/mood.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/muc/muc.py` & `nbxmpp-4.3.2/nbxmpp/modules/muc/muc.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,21 +241,14 @@
 
         occupant_id = stanza.getTagAttr('occupant-id',
                                         'id',
                                         namespace=Namespace.OCCUPANT_ID)
 
         properties.occupant_id = occupant_id
 
-        # MUC Private message
-        if (properties.type.is_chat or
-                properties.type.is_error and
-                not muc_user.getChildren()):
-            properties.muc_private_message = True
-            return
-
         if properties.is_muc_invite_or_decline:
             return
 
         properties.from_muc = True
         properties.muc_jid = properties.jid.new_as_bare()
 
         if not properties.jid.is_bare:
```

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/muc/util.py` & `nbxmpp-4.3.2/nbxmpp/modules/muc/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/muclumbus.py` & `nbxmpp-4.3.2/nbxmpp/modules/muclumbus.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/nickname.py` & `nbxmpp-4.3.2/nbxmpp/modules/nickname.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/omemo.py` & `nbxmpp-4.3.2/nbxmpp/modules/omemo.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/oob.py` & `nbxmpp-4.3.2/nbxmpp/modules/oob.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/openpgp.py` & `nbxmpp-4.3.2/nbxmpp/modules/openpgp.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/pgplegacy.py` & `nbxmpp-4.3.2/nbxmpp/modules/pgplegacy.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/ping.py` & `nbxmpp-4.3.2/nbxmpp/modules/ping.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/presence.py` & `nbxmpp-4.3.2/nbxmpp/modules/presence.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/pubsub.py` & `nbxmpp-4.3.2/nbxmpp/modules/pubsub.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/reactions.py` & `nbxmpp-4.3.2/nbxmpp/modules/reactions.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/receipts.py` & `nbxmpp-4.3.2/nbxmpp/modules/receipts.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/register/register.py` & `nbxmpp-4.3.2/nbxmpp/modules/register/register.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/register/util.py` & `nbxmpp-4.3.2/nbxmpp/modules/register/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/replies.py` & `nbxmpp-4.3.2/nbxmpp/modules/replies.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/roster.py` & `nbxmpp-4.3.2/nbxmpp/modules/roster.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/rsm.py` & `nbxmpp-4.3.2/nbxmpp/modules/rsm.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/security_labels.py` & `nbxmpp-4.3.2/nbxmpp/modules/security_labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Dict
 
 from dataclasses import dataclass
+import hashlib
 
 from nbxmpp.protocol import Iq
 from nbxmpp.simplexml import Node
 from nbxmpp.namespaces import Namespace
 from nbxmpp.structs import StanzaHandler
 from nbxmpp.errors import StanzaError
 from nbxmpp.task import iq_request_task
@@ -146,14 +147,18 @@
 
         label = security.getTag('label')
         if label is None:
             raise ValueError('label node missing')
 
         return cls(displaymarking=displaymarking, label=label)
 
+    def get_label_hash(self) -> str:
+        sha = hashlib.sha512()
+        sha.update(str(self.label).encode())
+        return sha.hexdigest()
 
 @dataclass
 class Catalog:
     labels: Dict[str, SecurityLabel]
     default: str
 
     def get_label_names(self):
```

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/software_version.py` & `nbxmpp-4.3.2/nbxmpp/modules/software_version.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/tune.py` & `nbxmpp-4.3.2/nbxmpp/modules/tune.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/user_avatar.py` & `nbxmpp-4.3.2/nbxmpp/modules/user_avatar.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/util.py` & `nbxmpp-4.3.2/nbxmpp/modules/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/vcard4.py` & `nbxmpp-4.3.2/nbxmpp/modules/vcard4.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/vcard_avatar.py` & `nbxmpp-4.3.2/nbxmpp/modules/vcard_avatar.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/modules/vcard_temp.py` & `nbxmpp-4.3.2/nbxmpp/modules/vcard_temp.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/namespaces.py` & `nbxmpp-4.3.2/nbxmpp/namespaces.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/old_dispatcher.py` & `nbxmpp-4.3.2/nbxmpp/old_dispatcher.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/plugin.py` & `nbxmpp-4.3.2/nbxmpp/plugin.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/protocol.py` & `nbxmpp-4.3.2/nbxmpp/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,4720 +56,4731 @@
 00000370: 2055 6e69 6f6e 0a66 726f 6d20 7479 7069   Union.from typi
 00000380: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
 00000390: 616c 0a66 726f 6d20 7479 7069 6e67 2069  al.from typing i
 000003a0: 6d70 6f72 7420 6361 7374 0a0a 696d 706f  mport cast..impo
 000003b0: 7274 206f 730a 696d 706f 7274 2074 696d  rt os.import tim
 000003c0: 650a 696d 706f 7274 2068 6173 686c 6962  e.import hashlib
 000003d0: 0a69 6d70 6f72 7420 6675 6e63 746f 6f6c  .import functool
-000003e0: 730a 696d 706f 7274 2077 6172 6e69 6e67  s.import warning
-000003f0: 730a 6672 6f6d 2062 6173 6536 3420 696d  s.from base64 im
-00000400: 706f 7274 2062 3634 656e 636f 6465 0a66  port b64encode.f
-00000410: 726f 6d20 6461 7461 636c 6173 7365 7320  rom dataclasses 
-00000420: 696d 706f 7274 2064 6174 6163 6c61 7373  import dataclass
-00000430: 0a66 726f 6d20 6461 7461 636c 6173 7365  .from dataclasse
-00000440: 7320 696d 706f 7274 2061 7364 6963 740a  s import asdict.
-00000450: 0a66 726f 6d20 6769 2e72 6570 6f73 6974  .from gi.reposit
-00000460: 6f72 7920 696d 706f 7274 2047 4c69 620a  ory import GLib.
-00000470: 0a69 6d70 6f72 7420 6964 6e61 0a66 726f  .import idna.fro
-00000480: 6d20 6e62 786d 7070 2e78 6d70 7069 7269  m nbxmpp.xmppiri
-00000490: 2069 6d70 6f72 7420 6573 6361 7065 5f69   import escape_i
-000004a0: 6672 6167 6d65 6e74 0a66 726f 6d20 6e62  fragment.from nb
-000004b0: 786d 7070 2e78 6d70 7069 7269 2069 6d70  xmpp.xmppiri imp
-000004c0: 6f72 7420 6573 6361 7065 5f69 6e6f 6465  ort escape_inode
-000004d0: 0a66 726f 6d20 6e62 786d 7070 2e78 6d70  .from nbxmpp.xmp
-000004e0: 7069 7269 2069 6d70 6f72 7420 6573 6361  piri import esca
-000004f0: 7065 5f69 7265 730a 6672 6f6d 206e 6278  pe_ires.from nbx
-00000500: 6d70 702e 786d 7070 6972 6920 696d 706f  mpp.xmppiri impo
-00000510: 7274 2065 7363 6170 655f 6976 616c 7565  rt escape_ivalue
-00000520: 0a66 726f 6d20 6e62 786d 7070 2e78 6d70  .from nbxmpp.xmp
-00000530: 7069 7269 2069 6d70 6f72 7420 7661 6c69  piri import vali
-00000540: 6461 7465 5f69 6b65 790a 6672 6f6d 206e  date_ikey.from n
-00000550: 6278 6d70 702e 786d 7070 6972 6920 696d  bxmpp.xmppiri im
-00000560: 706f 7274 2076 616c 6964 6174 655f 7175  port validate_qu
-00000570: 6572 7974 7970 650a 6672 6f6d 206e 6278  erytype.from nbx
-00000580: 6d70 702e 7369 6d70 6c65 786d 6c20 696d  mpp.simplexml im
-00000590: 706f 7274 204e 6f64 650a 6672 6f6d 206e  port Node.from n
-000005a0: 6278 6d70 702e 6e61 6d65 7370 6163 6573  bxmpp.namespaces
-000005b0: 2069 6d70 6f72 7420 4e61 6d65 7370 6163   import Namespac
-000005c0: 650a 6672 6f6d 206e 6278 6d70 702e 7374  e.from nbxmpp.st
-000005d0: 7269 6e67 7072 6570 2069 6d70 6f72 7420  ringprep import 
-000005e0: 6e6f 6465 7072 6570 0a66 726f 6d20 6e62  nodeprep.from nb
-000005f0: 786d 7070 2e73 7472 696e 6770 7265 7020  xmpp.stringprep 
-00000600: 696d 706f 7274 2072 6573 6f75 7263 6570  import resourcep
-00000610: 7265 700a 6672 6f6d 206e 6278 6d70 702e  rep.from nbxmpp.
-00000620: 7072 6563 6973 2069 6d70 6f72 7420 656e  precis import en
-00000630: 666f 7263 655f 7072 6563 6973 5f75 7365  force_precis_use
-00000640: 726e 616d 650a 6672 6f6d 206e 6278 6d70  rname.from nbxmp
-00000650: 702e 7072 6563 6973 2069 6d70 6f72 7420  p.precis import 
-00000660: 656e 666f 7263 655f 7072 6563 6973 5f6f  enforce_precis_o
-00000670: 7061 7175 650a 0a0a 6465 6620 6173 6369  paque...def asci
-00000680: 695f 7570 7065 7228 7329 3a0a 2020 2020  i_upper(s):.    
-00000690: 7265 7475 726e 2073 2e75 7070 6572 2829  return s.upper()
-000006a0: 0a0a 0a53 4153 4c5f 4155 5448 5f4d 4543  ...SASL_AUTH_MEC
-000006b0: 4853 203d 205b 0a20 2020 2027 5343 5241  HS = [.    'SCRA
-000006c0: 4d2d 5348 412d 3531 322d 504c 5553 272c  M-SHA-512-PLUS',
-000006d0: 0a20 2020 2027 5343 5241 4d2d 5348 412d  .    'SCRAM-SHA-
-000006e0: 3531 3227 2c0a 2020 2020 2753 4352 414d  512',.    'SCRAM
-000006f0: 2d53 4841 2d32 3536 2d50 4c55 5327 2c0a  -SHA-256-PLUS',.
-00000700: 2020 2020 2753 4352 414d 2d53 4841 2d32      'SCRAM-SHA-2
-00000710: 3536 272c 0a20 2020 2027 5343 5241 4d2d  56',.    'SCRAM-
-00000720: 5348 412d 312d 504c 5553 272c 0a20 2020  SHA-1-PLUS',.   
-00000730: 2027 5343 5241 4d2d 5348 412d 3127 2c0a   'SCRAM-SHA-1',.
-00000740: 2020 2020 2747 5353 4150 4927 2c0a 2020      'GSSAPI',.  
-00000750: 2020 2750 4c41 494e 272c 0a20 2020 2027    'PLAIN',.    '
-00000760: 4558 5445 524e 414c 272c 0a20 2020 2027  EXTERNAL',.    '
-00000770: 414e 4f4e 594d 4f55 5327 2c0a 5d0a 0a53  ANONYMOUS',.]..S
-00000780: 4153 4c5f 4552 524f 525f 434f 4e44 4954  ASL_ERROR_CONDIT
-00000790: 494f 4e53 203d 205b 0a20 2020 2027 6162  IONS = [.    'ab
-000007a0: 6f72 7465 6427 2c0a 2020 2020 2761 6363  orted',.    'acc
-000007b0: 6f75 6e74 2d64 6973 6162 6c65 6427 2c0a  ount-disabled',.
-000007c0: 2020 2020 2763 7265 6465 6e74 6961 6c73      'credentials
-000007d0: 2d65 7870 6972 6564 272c 0a20 2020 2027  -expired',.    '
-000007e0: 656e 6372 7970 7469 6f6e 2d72 6571 7569  encryption-requi
-000007f0: 7265 6427 2c0a 2020 2020 2769 6e63 6f72  red',.    'incor
-00000800: 7265 6374 2d65 6e63 6f64 696e 6727 2c0a  rect-encoding',.
-00000810: 2020 2020 2769 6e76 616c 6964 2d61 7574      'invalid-aut
-00000820: 687a 6964 272c 0a20 2020 2027 696e 7661  hzid',.    'inva
-00000830: 6c69 642d 6d65 6368 616e 6973 6d27 2c0a  lid-mechanism',.
-00000840: 2020 2020 276d 6563 6861 6e69 736d 2d74      'mechanism-t
-00000850: 6f6f 2d77 6561 6b27 2c0a 2020 2020 276d  oo-weak',.    'm
-00000860: 616c 666f 726d 6564 2d72 6571 7565 7374  alformed-request
-00000870: 272c 0a20 2020 2027 6e6f 742d 6175 7468  ',.    'not-auth
-00000880: 6f72 697a 6564 272c 0a20 2020 2027 7465  orized',.    'te
-00000890: 6d70 6f72 6172 792d 6175 7468 2d66 6169  mporary-auth-fai
-000008a0: 6c75 7265 272c 0a5d 0a0a 4552 524f 5253  lure',.]..ERRORS
-000008b0: 203d 207b 0a20 2020 2027 7572 6e3a 6965   = {.    'urn:ie
-000008c0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-000008d0: 3a78 6d70 702d 7361 736c 2061 626f 7274  :xmpp-sasl abort
-000008e0: 6564 273a 205b 2727 2c0a 2020 2020 2020  ed': ['',.      
-000008f0: 2020 2727 2c0a 2020 2020 2020 2020 2754    '',.        'T
-00000900: 6865 2072 6563 6569 7669 6e67 2065 6e74  he receiving ent
-00000910: 6974 7920 6163 6b6e 6f77 6c65 6467 6573  ity acknowledges
-00000920: 2061 6e20 3c61 626f 7274 2f3e 2065 6c65   an <abort/> ele
-00000930: 6d65 6e74 2073 656e 7420 6279 2074 6865  ment sent by the
-00000940: 2069 6e69 7469 6174 696e 6720 656e 7469   initiating enti
-00000950: 7479 3b20 7365 6e74 2069 6e20 7265 706c  ty; sent in repl
-00000960: 7920 746f 2074 6865 203c 6162 6f72 742f  y to the <abort/
-00000970: 3e20 656c 656d 656e 742e 275d 2c0a 2020  > element.'],.  
-00000980: 2020 2775 726e 3a69 6574 663a 7061 7261    'urn:ietf:para
-00000990: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
-000009a0: 6173 6c20 696e 636f 7272 6563 742d 656e  asl incorrect-en
-000009b0: 636f 6469 6e67 273a 205b 2727 2c0a 2020  coding': ['',.  
-000009c0: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
-000009d0: 2020 2754 6865 2064 6174 6120 7072 6f76    'The data prov
-000009e0: 6964 6564 2062 7920 7468 6520 696e 6974  ided by the init
-000009f0: 6961 7469 6e67 2065 6e74 6974 7920 636f  iating entity co
-00000a00: 756c 6420 6e6f 7420 6265 2070 726f 6365  uld not be proce
-00000a10: 7373 6564 2062 6563 6175 7365 2074 6865  ssed because the
-00000a20: 205b 4241 5345 3634 5d4a 6f73 6566 7373   [BASE64]Josefss
-00000a30: 6f6e 2c20 532e 2c20 5468 6520 4261 7365  on, S., The Base
-00000a40: 3136 2c20 4261 7365 3332 2c20 616e 6420  16, Base32, and 
-00000a50: 4261 7365 3634 2044 6174 6120 456e 636f  Base64 Data Enco
-00000a60: 6469 6e67 732c 204a 756c 7920 3230 3033  dings, July 2003
-00000a70: 2e20 656e 636f 6469 6e67 2069 7320 696e  . encoding is in
-00000a80: 636f 7272 6563 7420 2865 2e67 2e2c 2062  correct (e.g., b
-00000a90: 6563 6175 7365 2074 6865 2065 6e63 6f64  ecause the encod
-00000aa0: 696e 6720 646f 6573 206e 6f74 2061 6468  ing does not adh
-00000ab0: 6572 6520 746f 2074 6865 2064 6566 696e  ere to the defin
-00000ac0: 6974 696f 6e20 696e 2053 6563 7469 6f6e  ition in Section
-00000ad0: 2033 206f 6620 5b42 4153 4536 345d 4a6f   3 of [BASE64]Jo
-00000ae0: 7365 6673 736f 6e2c 2053 2e2c 2054 6865  sefsson, S., The
-00000af0: 2042 6173 6531 362c 2042 6173 6533 322c   Base16, Base32,
-00000b00: 2061 6e64 2042 6173 6536 3420 4461 7461   and Base64 Data
-00000b10: 2045 6e63 6f64 696e 6773 2c20 4a75 6c79   Encodings, July
-00000b20: 2032 3030 332e 293b 2073 656e 7420 696e   2003.); sent in
-00000b30: 2072 6570 6c79 2074 6f20 6120 3c72 6573   reply to a <res
-00000b40: 706f 6e73 652f 3e20 656c 656d 656e 7420  ponse/> element 
-00000b50: 6f72 2061 6e20 3c61 7574 682f 3e20 656c  or an <auth/> el
-00000b60: 656d 656e 7420 7769 7468 2069 6e69 7469  ement with initi
-00000b70: 616c 2072 6573 706f 6e73 6520 6461 7461  al response data
-00000b80: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-00000b90: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-00000ba0: 3a78 6d70 702d 7361 736c 2069 6e76 616c  :xmpp-sasl inval
-00000bb0: 6964 2d61 7574 687a 6964 273a 205b 2727  id-authzid': [''
-00000bc0: 2c0a 2020 2020 2020 2020 2727 2c0a 2020  ,.        '',.  
-00000bd0: 2020 2020 2020 2754 6865 2061 7574 687a        'The authz
-00000be0: 6964 2070 726f 7669 6465 6420 6279 2074  id provided by t
-00000bf0: 6865 2069 6e69 7469 6174 696e 6720 656e  he initiating en
-00000c00: 7469 7479 2069 7320 696e 7661 6c69 642c  tity is invalid,
-00000c10: 2065 6974 6865 7220 6265 6361 7573 6520   either because 
-00000c20: 6974 2069 7320 696e 636f 7272 6563 746c  it is incorrectl
-00000c30: 7920 666f 726d 6174 7465 6420 6f72 2062  y formatted or b
-00000c40: 6563 6175 7365 2074 6865 2069 6e69 7469  ecause the initi
-00000c50: 6174 696e 6720 656e 7469 7479 2064 6f65  ating entity doe
-00000c60: 7320 6e6f 7420 6861 7665 2070 6572 6d69  s not have permi
-00000c70: 7373 696f 6e73 2074 6f20 6175 7468 6f72  ssions to author
-00000c80: 697a 6520 7468 6174 2049 443b 2073 656e  ize that ID; sen
-00000c90: 7420 696e 2072 6570 6c79 2074 6f20 6120  t in reply to a 
-00000ca0: 3c72 6573 706f 6e73 652f 3e20 656c 656d  <response/> elem
-00000cb0: 656e 7420 6f72 2061 6e20 3c61 7574 682f  ent or an <auth/
-00000cc0: 3e20 656c 656d 656e 7420 7769 7468 2069  > element with i
-00000cd0: 6e69 7469 616c 2072 6573 706f 6e73 6520  nitial response 
-00000ce0: 6461 7461 2e27 5d2c 0a20 2020 2027 7572  data.'],.    'ur
-00000cf0: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
-00000d00: 6c3a 6e73 3a78 6d70 702d 7361 736c 2069  l:ns:xmpp-sasl i
-00000d10: 6e76 616c 6964 2d6d 6563 6861 6e69 736d  nvalid-mechanism
-00000d20: 273a 205b 2727 2c0a 2020 2020 2020 2020  ': ['',.        
-00000d30: 2727 2c0a 2020 2020 2020 2020 2754 6865  '',.        'The
-00000d40: 2069 6e69 7469 6174 696e 6720 656e 7469   initiating enti
-00000d50: 7479 2064 6964 206e 6f74 2070 726f 7669  ty did not provi
-00000d60: 6465 2061 206d 6563 6861 6e69 736d 206f  de a mechanism o
-00000d70: 7220 7265 7175 6573 7465 6420 6120 6d65  r requested a me
-00000d80: 6368 616e 6973 6d20 7468 6174 2069 7320  chanism that is 
-00000d90: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
-00000da0: 2074 6865 2072 6563 6569 7669 6e67 2065   the receiving e
-00000db0: 6e74 6974 793b 2073 656e 7420 696e 2072  ntity; sent in r
-00000dc0: 6570 6c79 2074 6f20 616e 203c 6175 7468  eply to an <auth
-00000dd0: 2f3e 2065 6c65 6d65 6e74 2e27 5d2c 0a20  /> element.'],. 
-00000de0: 2020 2027 7572 6e3a 6965 7466 3a70 6172     'urn:ietf:par
-00000df0: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00000e00: 7361 736c 206d 6563 6861 6e69 736d 2d74  sasl mechanism-t
-00000e10: 6f6f 2d77 6561 6b27 3a20 5b27 272c 0a20  oo-weak': ['',. 
-00000e20: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
-00000e30: 2020 2027 5468 6520 6d65 6368 616e 6973     'The mechanis
-00000e40: 6d20 7265 7175 6573 7465 6420 6279 2074  m requested by t
-00000e50: 6865 2069 6e69 7469 6174 696e 6720 656e  he initiating en
-00000e60: 7469 7479 2069 7320 7765 616b 6572 2074  tity is weaker t
-00000e70: 6861 6e20 7365 7276 6572 2070 6f6c 6963  han server polic
-00000e80: 7920 7065 726d 6974 7320 666f 7220 7468  y permits for th
-00000e90: 6174 2069 6e69 7469 6174 696e 6720 656e  at initiating en
-00000ea0: 7469 7479 3b20 7365 6e74 2069 6e20 7265  tity; sent in re
-00000eb0: 706c 7920 746f 2061 203c 7265 7370 6f6e  ply to a <respon
-00000ec0: 7365 2f3e 2065 6c65 6d65 6e74 206f 7220  se/> element or 
-00000ed0: 616e 203c 6175 7468 2f3e 2065 6c65 6d65  an <auth/> eleme
-00000ee0: 6e74 2077 6974 6820 696e 6974 6961 6c20  nt with initial 
-00000ef0: 7265 7370 6f6e 7365 2064 6174 612e 275d  response data.']
-00000f00: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
-00000f10: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00000f20: 7070 2d73 6173 6c20 6e6f 742d 6175 7468  pp-sasl not-auth
-00000f30: 6f72 697a 6564 273a 205b 2727 2c0a 2020  orized': ['',.  
-00000f40: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
-00000f50: 2020 2754 6865 2061 7574 6865 6e74 6963    'The authentic
-00000f60: 6174 696f 6e20 6661 696c 6564 2062 6563  ation failed bec
-00000f70: 6175 7365 2074 6865 2069 6e69 7469 6174  ause the initiat
-00000f80: 696e 6720 656e 7469 7479 2064 6964 206e  ing entity did n
-00000f90: 6f74 2070 726f 7669 6465 2076 616c 6964  ot provide valid
-00000fa0: 2063 7265 6465 6e74 6961 6c73 2028 7468   credentials (th
-00000fb0: 6973 2069 6e63 6c75 6465 7320 6275 7420  is includes but 
-00000fc0: 6973 206e 6f74 206c 696d 6974 6564 2074  is not limited t
-00000fd0: 6f20 7468 6520 6361 7365 206f 6620 616e  o the case of an
-00000fe0: 2075 6e6b 6e6f 776e 2075 7365 726e 616d   unknown usernam
-00000ff0: 6529 3b20 7365 6e74 2069 6e20 7265 706c  e); sent in repl
-00001000: 7920 746f 2061 203c 7265 7370 6f6e 7365  y to a <response
-00001010: 2f3e 2065 6c65 6d65 6e74 206f 7220 616e  /> element or an
-00001020: 203c 6175 7468 2f3e 2065 6c65 6d65 6e74   <auth/> element
-00001030: 2077 6974 6820 696e 6974 6961 6c20 7265   with initial re
-00001040: 7370 6f6e 7365 2064 6174 612e 275d 2c0a  sponse data.'],.
-00001050: 2020 2020 2775 726e 3a69 6574 663a 7061      'urn:ietf:pa
-00001060: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
-00001070: 2d73 6173 6c20 7465 6d70 6f72 6172 792d  -sasl temporary-
-00001080: 6175 7468 2d66 6169 6c75 7265 273a 205b  auth-failure': [
-00001090: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
-000010a0: 2020 2020 2020 2020 2754 6865 2061 7574          'The aut
-000010b0: 6865 6e74 6963 6174 696f 6e20 6661 696c  hentication fail
-000010c0: 6564 2062 6563 6175 7365 206f 6620 6120  ed because of a 
-000010d0: 7465 6d70 6f72 6172 7920 6572 726f 7220  temporary error 
-000010e0: 636f 6e64 6974 696f 6e20 7769 7468 696e  condition within
-000010f0: 2074 6865 2072 6563 6569 7669 6e67 2065   the receiving e
-00001100: 6e74 6974 793b 2073 656e 7420 696e 2072  ntity; sent in r
-00001110: 6570 6c79 2074 6f20 616e 203c 6175 7468  eply to an <auth
-00001120: 2f3e 2065 6c65 6d65 6e74 206f 7220 3c72  /> element or <r
-00001130: 6573 706f 6e73 652f 3e20 656c 656d 656e  esponse/> elemen
-00001140: 742e 275d 2c0a 2020 2020 2775 726e 3a69  t.'],.    'urn:i
-00001150: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
-00001160: 733a 786d 7070 2d73 7461 6e7a 6173 2062  s:xmpp-stanzas b
-00001170: 6164 2d72 6571 7565 7374 273a 205b 2734  ad-request': ['4
-00001180: 3030 272c 0a20 2020 2020 2020 2027 6d6f  00',.        'mo
-00001190: 6469 6679 272c 0a20 2020 2020 2020 2027  dify',.        '
-000011a0: 5468 6520 7365 6e64 6572 2068 6173 2073  The sender has s
-000011b0: 656e 7420 584d 4c20 7468 6174 2069 7320  ent XML that is 
-000011c0: 6d61 6c66 6f72 6d65 6420 6f72 2074 6861  malformed or tha
-000011d0: 7420 6361 6e6e 6f74 2062 6520 7072 6f63  t cannot be proc
-000011e0: 6573 7365 642e 275d 2c0a 2020 2020 2775  essed.'],.    'u
-000011f0: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
-00001200: 6d6c 3a6e 733a 786d 7070 2d73 7461 6e7a  ml:ns:xmpp-stanz
-00001210: 6173 2063 6f6e 666c 6963 7427 3a20 5b27  as conflict': ['
-00001220: 3430 3927 2c0a 2020 2020 2020 2020 2763  409',.        'c
-00001230: 616e 6365 6c27 2c0a 2020 2020 2020 2020  ancel',.        
-00001240: 2741 6363 6573 7320 6361 6e6e 6f74 2062  'Access cannot b
-00001250: 6520 6772 616e 7465 6420 6265 6361 7573  e granted becaus
-00001260: 6520 616e 2065 7869 7374 696e 6720 7265  e an existing re
-00001270: 736f 7572 6365 206f 7220 7365 7373 696f  source or sessio
-00001280: 6e20 6578 6973 7473 2077 6974 6820 7468  n exists with th
-00001290: 6520 7361 6d65 206e 616d 6520 6f72 2061  e same name or a
-000012a0: 6464 7265 7373 2e27 5d2c 0a20 2020 2027  ddress.'],.    '
-000012b0: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-000012c0: 786d 6c3a 6e73 3a78 6d70 702d 7374 616e  xml:ns:xmpp-stan
-000012d0: 7a61 7320 6665 6174 7572 652d 6e6f 742d  zas feature-not-
-000012e0: 696d 706c 656d 656e 7465 6427 3a20 5b27  implemented': ['
-000012f0: 3530 3127 2c0a 2020 2020 2020 2020 2763  501',.        'c
-00001300: 616e 6365 6c27 2c0a 2020 2020 2020 2020  ancel',.        
-00001310: 2754 6865 2066 6561 7475 7265 2072 6571  'The feature req
-00001320: 7565 7374 6564 2069 7320 6e6f 7420 696d  uested is not im
-00001330: 706c 656d 656e 7465 6420 6279 2074 6865  plemented by the
-00001340: 2072 6563 6970 6965 6e74 206f 7220 7365   recipient or se
-00001350: 7276 6572 2061 6e64 2074 6865 7265 666f  rver and therefo
-00001360: 7265 2063 616e 6e6f 7420 6265 2070 726f  re cannot be pro
-00001370: 6365 7373 6564 2e27 5d2c 0a20 2020 2027  cessed.'],.    '
-00001380: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00001390: 786d 6c3a 6e73 3a78 6d70 702d 7374 616e  xml:ns:xmpp-stan
-000013a0: 7a61 7320 666f 7262 6964 6465 6e27 3a20  zas forbidden': 
-000013b0: 5b27 3430 3327 2c0a 2020 2020 2020 2020  ['403',.        
-000013c0: 2761 7574 6827 2c0a 2020 2020 2020 2020  'auth',.        
-000013d0: 2754 6865 2072 6571 7565 7374 696e 6720  'The requesting 
-000013e0: 656e 7469 7479 2064 6f65 7320 6e6f 7420  entity does not 
-000013f0: 706f 7373 6573 7320 7468 6520 7265 7175  possess the requ
-00001400: 6972 6564 2070 6572 6d69 7373 696f 6e73  ired permissions
-00001410: 2074 6f20 7065 7266 6f72 6d20 7468 6520   to perform the 
-00001420: 6163 7469 6f6e 2e27 5d2c 0a20 2020 2027  action.'],.    '
-00001430: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00001440: 786d 6c3a 6e73 3a78 6d70 702d 7374 616e  xml:ns:xmpp-stan
-00001450: 7a61 7320 676f 6e65 273a 205b 2733 3032  zas gone': ['302
-00001460: 272c 0a20 2020 2020 2020 2027 6d6f 6469  ',.        'modi
-00001470: 6679 272c 0a20 2020 2020 2020 2027 5468  fy',.        'Th
-00001480: 6520 7265 6369 7069 656e 7420 6f72 2073  e recipient or s
-00001490: 6572 7665 7220 6361 6e20 6e6f 206c 6f6e  erver can no lon
-000014a0: 6765 7220 6265 2063 6f6e 7461 6374 6564  ger be contacted
-000014b0: 2061 7420 7468 6973 2061 6464 7265 7373   at this address
-000014c0: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-000014d0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-000014e0: 3a78 6d70 702d 7374 616e 7a61 7320 696e  :xmpp-stanzas in
-000014f0: 7465 726e 616c 2d73 6572 7665 722d 6572  ternal-server-er
-00001500: 726f 7227 3a20 5b27 3530 3027 2c0a 2020  ror': ['500',.  
-00001510: 2020 2020 2020 2777 6169 7427 2c0a 2020        'wait',.  
-00001520: 2020 2020 2020 2754 6865 2073 6572 7665        'The serve
-00001530: 7220 636f 756c 6420 6e6f 7420 7072 6f63  r could not proc
-00001540: 6573 7320 7468 6520 7374 616e 7a61 2062  ess the stanza b
-00001550: 6563 6175 7365 206f 6620 6120 6d69 7363  ecause of a misc
-00001560: 6f6e 6669 6775 7261 7469 6f6e 206f 7220  onfiguration or 
-00001570: 616e 206f 7468 6572 7769 7365 2d75 6e64  an otherwise-und
-00001580: 6566 696e 6564 2069 6e74 6572 6e61 6c20  efined internal 
-00001590: 7365 7276 6572 2065 7272 6f72 2e27 5d2c  server error.'],
-000015a0: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
-000015b0: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
-000015c0: 702d 7374 616e 7a61 7320 6974 656d 2d6e  p-stanzas item-n
-000015d0: 6f74 2d66 6f75 6e64 273a 205b 2734 3034  ot-found': ['404
-000015e0: 272c 0a20 2020 2020 2020 2027 6361 6e63  ',.        'canc
-000015f0: 656c 272c 0a20 2020 2020 2020 2027 5468  el',.        'Th
-00001600: 6520 6164 6472 6573 7365 6420 4a49 4420  e addressed JID 
-00001610: 6f72 2069 7465 6d20 7265 7175 6573 7465  or item requeste
-00001620: 6420 6361 6e6e 6f74 2062 6520 666f 756e  d cannot be foun
-00001630: 642e 275d 2c0a 2020 2020 2775 726e 3a69  d.'],.    'urn:i
-00001640: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
-00001650: 733a 786d 7070 2d73 7461 6e7a 6173 206a  s:xmpp-stanzas j
-00001660: 6964 2d6d 616c 666f 726d 6564 273a 205b  id-malformed': [
-00001670: 2734 3030 272c 0a20 2020 2020 2020 2027  '400',.        '
-00001680: 6d6f 6469 6679 272c 0a20 2020 2020 2020  modify',.       
-00001690: 2022 5468 6520 7661 6c75 6520 6f66 2074   "The value of t
-000016a0: 6865 2020 2020 2020 2020 2774 6f27 2061  he        'to' a
-000016b0: 7474 7269 6275 7465 2069 6e20 7468 6520  ttribute in the 
-000016c0: 7365 6e64 6572 2773 2073 7461 6e7a 6120  sender's stanza 
-000016d0: 646f 6573 206e 6f74 2061 6468 6572 6520  does not adhere 
-000016e0: 746f 2074 6865 2073 796e 7461 7820 6465  to the syntax de
-000016f0: 6669 6e65 6420 696e 2041 6464 7265 7373  fined in Address
-00001700: 696e 6720 5363 6865 6d65 2e22 5d2c 0a20  ing Scheme."],. 
-00001710: 2020 2027 7572 6e3a 6965 7466 3a70 6172     'urn:ietf:par
-00001720: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00001730: 7374 616e 7a61 7320 6e6f 742d 6163 6365  stanzas not-acce
-00001740: 7074 6162 6c65 273a 205b 2734 3036 272c  ptable': ['406',
-00001750: 0a20 2020 2020 2020 2027 6361 6e63 656c  .        'cancel
-00001760: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
-00001770: 7265 6369 7069 656e 7420 6f72 2073 6572  recipient or ser
-00001780: 7665 7220 756e 6465 7273 7461 6e64 7320  ver understands 
-00001790: 7468 6520 7265 7175 6573 7420 6275 7420  the request but 
-000017a0: 6973 2072 6566 7573 696e 6720 746f 2070  is refusing to p
-000017b0: 726f 6365 7373 2069 7420 6265 6361 7573  rocess it becaus
-000017c0: 6520 6974 2064 6f65 7320 6e6f 7420 6d65  e it does not me
-000017d0: 6574 2063 7269 7465 7269 6120 6465 6669  et criteria defi
-000017e0: 6e65 6420 6279 2074 6865 2072 6563 6970  ned by the recip
-000017f0: 6965 6e74 206f 7220 7365 7276 6572 2e27  ient or server.'
-00001800: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
-00001810: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00001820: 6d70 702d 7374 616e 7a61 7320 6e6f 742d  mpp-stanzas not-
-00001830: 616c 6c6f 7765 6427 3a20 5b27 3430 3527  allowed': ['405'
-00001840: 2c0a 2020 2020 2020 2020 2763 616e 6365  ,.        'cance
-00001850: 6c27 2c0a 2020 2020 2020 2020 2754 6865  l',.        'The
-00001860: 2072 6563 6970 6965 6e74 206f 7220 7365   recipient or se
-00001870: 7276 6572 2064 6f65 7320 6e6f 7420 616c  rver does not al
-00001880: 6c6f 7720 616e 7920 656e 7469 7479 2074  low any entity t
-00001890: 6f20 7065 7266 6f72 6d20 7468 6520 6163  o perform the ac
-000018a0: 7469 6f6e 2e27 5d2c 0a20 2020 2027 7572  tion.'],.    'ur
-000018b0: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
-000018c0: 6c3a 6e73 3a78 6d70 702d 7374 616e 7a61  l:ns:xmpp-stanza
-000018d0: 7320 6e6f 742d 6175 7468 6f72 697a 6564  s not-authorized
-000018e0: 273a 205b 2734 3031 272c 0a20 2020 2020  ': ['401',.     
-000018f0: 2020 2027 6175 7468 272c 0a20 2020 2020     'auth',.     
-00001900: 2020 2027 5468 6520 7365 6e64 6572 206d     'The sender m
-00001910: 7573 7420 7072 6f76 6964 6520 7072 6f70  ust provide prop
-00001920: 6572 2063 7265 6465 6e74 6961 6c73 2062  er credentials b
-00001930: 6566 6f72 6520 6265 696e 6720 616c 6c6f  efore being allo
-00001940: 7765 6420 746f 2070 6572 666f 726d 2074  wed to perform t
-00001950: 6865 2061 6374 696f 6e2c 206f 7220 6861  he action, or ha
-00001960: 7320 7072 6f76 6964 6564 2069 6d70 726f  s provided impro
-00001970: 7065 7220 6372 6564 656e 7469 616c 732e  per credentials.
-00001980: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
-00001990: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-000019a0: 786d 7070 2d73 7461 6e7a 6173 2070 6179  xmpp-stanzas pay
-000019b0: 6d65 6e74 2d72 6571 7569 7265 6427 3a20  ment-required': 
-000019c0: 5b27 3430 3227 2c0a 2020 2020 2020 2020  ['402',.        
-000019d0: 2761 7574 6827 2c0a 2020 2020 2020 2020  'auth',.        
-000019e0: 2754 6865 2072 6571 7565 7374 696e 6720  'The requesting 
-000019f0: 656e 7469 7479 2069 7320 6e6f 7420 6175  entity is not au
-00001a00: 7468 6f72 697a 6564 2074 6f20 6163 6365  thorized to acce
-00001a10: 7373 2074 6865 2072 6571 7565 7374 6564  ss the requested
-00001a20: 2073 6572 7669 6365 2062 6563 6175 7365   service because
-00001a30: 2070 6179 6d65 6e74 2069 7320 7265 7175   payment is requ
-00001a40: 6972 6564 2e27 5d2c 0a20 2020 2027 7572  ired.'],.    'ur
-00001a50: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
-00001a60: 6c3a 6e73 3a78 6d70 702d 7374 616e 7a61  l:ns:xmpp-stanza
-00001a70: 7320 7265 6369 7069 656e 742d 756e 6176  s recipient-unav
-00001a80: 6169 6c61 626c 6527 3a20 5b27 3430 3427  ailable': ['404'
-00001a90: 2c0a 2020 2020 2020 2020 2777 6169 7427  ,.        'wait'
-00001aa0: 2c0a 2020 2020 2020 2020 2754 6865 2069  ,.        'The i
-00001ab0: 6e74 656e 6465 6420 7265 6369 7069 656e  ntended recipien
-00001ac0: 7420 6973 2074 656d 706f 7261 7269 6c79  t is temporarily
-00001ad0: 2075 6e61 7661 696c 6162 6c65 2e27 5d2c   unavailable.'],
-00001ae0: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
-00001af0: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
-00001b00: 702d 7374 616e 7a61 7320 7265 6469 7265  p-stanzas redire
-00001b10: 6374 273a 205b 2733 3032 272c 0a20 2020  ct': ['302',.   
-00001b20: 2020 2020 2027 6d6f 6469 6679 272c 0a20       'modify',. 
-00001b30: 2020 2020 2020 2027 5468 6520 7265 6369         'The reci
-00001b40: 7069 656e 7420 6f72 2073 6572 7665 7220  pient or server 
-00001b50: 6973 2072 6564 6972 6563 7469 6e67 2072  is redirecting r
-00001b60: 6571 7565 7374 7320 666f 7220 7468 6973  equests for this
-00001b70: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
-00001b80: 616e 6f74 6865 7220 656e 7469 7479 2e27  another entity.'
-00001b90: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
-00001ba0: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00001bb0: 6d70 702d 7374 616e 7a61 7320 7265 6769  mpp-stanzas regi
-00001bc0: 7374 7261 7469 6f6e 2d72 6571 7569 7265  stration-require
-00001bd0: 6427 3a20 5b27 3430 3727 2c0a 2020 2020  d': ['407',.    
-00001be0: 2020 2020 2761 7574 6827 2c0a 2020 2020      'auth',.    
-00001bf0: 2020 2020 2754 6865 2072 6571 7565 7374      'The request
-00001c00: 696e 6720 656e 7469 7479 2069 7320 6e6f  ing entity is no
-00001c10: 7420 6175 7468 6f72 697a 6564 2074 6f20  t authorized to 
-00001c20: 6163 6365 7373 2074 6865 2072 6571 7565  access the reque
-00001c30: 7374 6564 2073 6572 7669 6365 2062 6563  sted service bec
-00001c40: 6175 7365 2072 6567 6973 7472 6174 696f  ause registratio
-00001c50: 6e20 6973 2072 6571 7569 7265 642e 275d  n is required.']
-00001c60: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
-00001c70: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00001c80: 7070 2d73 7461 6e7a 6173 2072 656d 6f74  pp-stanzas remot
-00001c90: 652d 7365 7276 6572 2d6e 6f74 2d66 6f75  e-server-not-fou
-00001ca0: 6e64 273a 205b 2734 3034 272c 0a20 2020  nd': ['404',.   
-00001cb0: 2020 2020 2027 6361 6e63 656c 272c 0a20       'cancel',. 
-00001cc0: 2020 2020 2020 2027 4120 7265 6d6f 7465         'A remote
-00001cd0: 2073 6572 7665 7220 6f72 2073 6572 7669   server or servi
-00001ce0: 6365 2073 7065 6369 6669 6564 2061 7320  ce specified as 
-00001cf0: 7061 7274 206f 7220 616c 6c20 6f66 2074  part or all of t
-00001d00: 6865 204a 4944 206f 6620 7468 6520 696e  he JID of the in
-00001d10: 7465 6e64 6564 2072 6563 6970 6965 6e74  tended recipient
-00001d20: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
-00001d30: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
-00001d40: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-00001d50: 786d 7070 2d73 7461 6e7a 6173 2072 656d  xmpp-stanzas rem
-00001d60: 6f74 652d 7365 7276 6572 2d74 696d 656f  ote-server-timeo
-00001d70: 7574 273a 205b 2735 3034 272c 0a20 2020  ut': ['504',.   
-00001d80: 2020 2020 2027 7761 6974 272c 0a20 2020       'wait',.   
-00001d90: 2020 2020 2027 4120 7265 6d6f 7465 2073       'A remote s
-00001da0: 6572 7665 7220 6f72 2073 6572 7669 6365  erver or service
-00001db0: 2073 7065 6369 6669 6564 2061 7320 7061   specified as pa
-00001dc0: 7274 206f 7220 616c 6c20 6f66 2074 6865  rt or all of the
-00001dd0: 204a 4944 206f 6620 7468 6520 696e 7465   JID of the inte
-00001de0: 6e64 6564 2072 6563 6970 6965 6e74 2063  nded recipient c
-00001df0: 6f75 6c64 206e 6f74 2062 6520 636f 6e74  ould not be cont
-00001e00: 6163 7465 6420 7769 7468 696e 2061 2072  acted within a r
-00001e10: 6561 736f 6e61 626c 6520 616d 6f75 6e74  easonable amount
-00001e20: 206f 6620 7469 6d65 2e27 5d2c 0a20 2020   of time.'],.   
-00001e30: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
-00001e40: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
-00001e50: 616e 7a61 7320 7265 736f 7572 6365 2d63  anzas resource-c
-00001e60: 6f6e 7374 7261 696e 7427 3a20 5b27 3530  onstraint': ['50
-00001e70: 3027 2c0a 2020 2020 2020 2020 2777 6169  0',.        'wai
-00001e80: 7427 2c0a 2020 2020 2020 2020 2754 6865  t',.        'The
-00001e90: 2073 6572 7665 7220 6f72 2072 6563 6970   server or recip
-00001ea0: 6965 6e74 206c 6163 6b73 2074 6865 2073  ient lacks the s
-00001eb0: 7973 7465 6d20 7265 736f 7572 6365 7320  ystem resources 
-00001ec0: 6e65 6365 7373 6172 7920 746f 2073 6572  necessary to ser
-00001ed0: 7669 6365 2074 6865 2072 6571 7565 7374  vice the request
-00001ee0: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-00001ef0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-00001f00: 3a78 6d70 702d 7374 616e 7a61 7320 7365  :xmpp-stanzas se
-00001f10: 7276 6963 652d 756e 6176 6169 6c61 626c  rvice-unavailabl
-00001f20: 6527 3a20 5b27 3530 3327 2c0a 2020 2020  e': ['503',.    
-00001f30: 2020 2020 2763 616e 6365 6c27 2c0a 2020      'cancel',.  
-00001f40: 2020 2020 2020 2754 6865 2073 6572 7665        'The serve
-00001f50: 7220 6f72 2072 6563 6970 6965 6e74 2064  r or recipient d
-00001f60: 6f65 7320 6e6f 7420 6375 7272 656e 746c  oes not currentl
-00001f70: 7920 7072 6f76 6964 6520 7468 6520 7265  y provide the re
-00001f80: 7175 6573 7465 6420 7365 7276 6963 652e  quested service.
-00001f90: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
-00001fa0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-00001fb0: 786d 7070 2d73 7461 6e7a 6173 2073 7562  xmpp-stanzas sub
-00001fc0: 7363 7269 7074 696f 6e2d 7265 7175 6972  scription-requir
-00001fd0: 6564 273a 205b 2734 3037 272c 0a20 2020  ed': ['407',.   
-00001fe0: 2020 2020 2027 6175 7468 272c 0a20 2020       'auth',.   
-00001ff0: 2020 2020 2027 5468 6520 7265 7175 6573       'The reques
-00002000: 7469 6e67 2065 6e74 6974 7920 6973 206e  ting entity is n
-00002010: 6f74 2061 7574 686f 7269 7a65 6420 746f  ot authorized to
-00002020: 2061 6363 6573 7320 7468 6520 7265 7175   access the requ
-00002030: 6573 7465 6420 7365 7276 6963 6520 6265  ested service be
-00002040: 6361 7573 6520 6120 7375 6273 6372 6970  cause a subscrip
-00002050: 7469 6f6e 2069 7320 7265 7175 6972 6564  tion is required
-00002060: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-00002070: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-00002080: 3a78 6d70 702d 7374 616e 7a61 7320 756e  :xmpp-stanzas un
-00002090: 6465 6669 6e65 642d 636f 6e64 6974 696f  defined-conditio
-000020a0: 6e27 3a20 5b27 3530 3027 2c0a 2020 2020  n': ['500',.    
-000020b0: 2020 2020 2727 2c0a 2020 2020 2020 2020      '',.        
-000020c0: 2755 6e64 6566 696e 6564 2043 6f6e 6469  'Undefined Condi
-000020d0: 7469 6f6e 275d 2c0a 2020 2020 2775 726e  tion'],.    'urn
-000020e0: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
-000020f0: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
-00002100: 2075 6e65 7870 6563 7465 642d 7265 7175   unexpected-requ
-00002110: 6573 7427 3a20 5b27 3430 3027 2c0a 2020  est': ['400',.  
-00002120: 2020 2020 2020 2777 6169 7427 2c0a 2020        'wait',.  
-00002130: 2020 2020 2020 2754 6865 2072 6563 6970        'The recip
-00002140: 6965 6e74 206f 7220 7365 7276 6572 2075  ient or server u
-00002150: 6e64 6572 7374 6f6f 6420 7468 6520 7265  nderstood the re
-00002160: 7175 6573 7420 6275 7420 7761 7320 6e6f  quest but was no
-00002170: 7420 6578 7065 6374 696e 6720 6974 2061  t expecting it a
-00002180: 7420 7468 6973 2074 696d 6520 2865 2e67  t this time (e.g
-00002190: 2e2c 2074 6865 2072 6571 7565 7374 2077  ., the request w
-000021a0: 6173 206f 7574 206f 6620 6f72 6465 7229  as out of order)
-000021b0: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-000021c0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-000021d0: 3a78 6d70 702d 7374 7265 616d 7320 6261  :xmpp-streams ba
-000021e0: 642d 666f 726d 6174 273a 205b 2727 2c0a  d-format': ['',.
-000021f0: 2020 2020 2020 2020 2727 2c0a 2020 2020          '',.    
-00002200: 2020 2020 2754 6865 2065 6e74 6974 7920      'The entity 
-00002210: 6861 7320 7365 6e74 2058 4d4c 2074 6861  has sent XML tha
-00002220: 7420 6361 6e6e 6f74 2062 6520 7072 6f63  t cannot be proc
-00002230: 6573 7365 642e 275d 2c0a 2020 2020 2775  essed.'],.    'u
-00002240: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
-00002250: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
-00002260: 6d73 2062 6164 2d6e 616d 6573 7061 6365  ms bad-namespace
-00002270: 2d70 7265 6669 7827 3a20 5b27 272c 0a20  -prefix': ['',. 
-00002280: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
-00002290: 2020 2027 5468 6520 656e 7469 7479 2068     'The entity h
-000022a0: 6173 2073 656e 7420 6120 6e61 6d65 7370  as sent a namesp
-000022b0: 6163 6520 7072 6566 6978 2074 6861 7420  ace prefix that 
-000022c0: 6973 2075 6e73 7570 706f 7274 6564 2c20  is unsupported, 
-000022d0: 6f72 2068 6173 2073 656e 7420 6e6f 206e  or has sent no n
-000022e0: 616d 6573 7061 6365 2070 7265 6669 7820  amespace prefix 
-000022f0: 6f6e 2061 6e20 656c 656d 656e 7420 7468  on an element th
-00002300: 6174 2072 6571 7569 7265 7320 7375 6368  at requires such
-00002310: 2061 2070 7265 6669 782e 275d 2c0a 2020   a prefix.'],.  
-00002320: 2020 2775 726e 3a69 6574 663a 7061 7261    'urn:ietf:para
-00002330: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
-00002340: 7472 6561 6d73 2063 6f6e 666c 6963 7427  treams conflict'
-00002350: 3a20 5b27 272c 0a20 2020 2020 2020 2027  : ['',.        '
-00002360: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
-00002370: 7365 7276 6572 2069 7320 636c 6f73 696e  server is closin
-00002380: 6720 7468 6520 6163 7469 7665 2073 7472  g the active str
-00002390: 6561 6d20 666f 7220 7468 6973 2065 6e74  eam for this ent
-000023a0: 6974 7920 6265 6361 7573 6520 6120 6e65  ity because a ne
-000023b0: 7720 7374 7265 616d 2068 6173 2062 6565  w stream has bee
-000023c0: 6e20 696e 6974 6961 7465 6420 7468 6174  n initiated that
-000023d0: 2063 6f6e 666c 6963 7473 2077 6974 6820   conflicts with 
-000023e0: 7468 6520 6578 6973 7469 6e67 2073 7472  the existing str
-000023f0: 6561 6d2e 275d 2c0a 2020 2020 2775 726e  eam.'],.    'urn
-00002400: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
-00002410: 3a6e 733a 786d 7070 2d73 7472 6561 6d73  :ns:xmpp-streams
-00002420: 2063 6f6e 6e65 6374 696f 6e2d 7469 6d65   connection-time
-00002430: 6f75 7427 3a20 5b27 272c 0a20 2020 2020  out': ['',.     
-00002440: 2020 2027 272c 0a20 2020 2020 2020 2027     '',.        '
-00002450: 5468 6520 656e 7469 7479 2068 6173 206e  The entity has n
-00002460: 6f74 2067 656e 6572 6174 6564 2061 6e79  ot generated any
-00002470: 2074 7261 6666 6963 206f 7665 7220 7468   traffic over th
-00002480: 6520 7374 7265 616d 2066 6f72 2073 6f6d  e stream for som
-00002490: 6520 7065 7269 6f64 206f 6620 7469 6d65  e period of time
-000024a0: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-000024b0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-000024c0: 3a78 6d70 702d 7374 7265 616d 7320 686f  :xmpp-streams ho
-000024d0: 7374 2d67 6f6e 6527 3a20 5b27 272c 0a20  st-gone': ['',. 
-000024e0: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
-000024f0: 2020 2022 5468 6520 7661 6c75 6520 6f66     "The value of
-00002500: 2074 6865 2020 2020 2020 2020 2774 6f27   the        'to'
-00002510: 2061 7474 7269 6275 7465 2070 726f 7669   attribute provi
-00002520: 6465 6420 6279 2074 6865 2069 6e69 7469  ded by the initi
-00002530: 6174 696e 6720 656e 7469 7479 2069 6e20  ating entity in 
-00002540: 7468 6520 7374 7265 616d 2068 6561 6465  the stream heade
-00002550: 7220 636f 7272 6573 706f 6e64 7320 746f  r corresponds to
-00002560: 2061 2068 6f73 746e 616d 6520 7468 6174   a hostname that
-00002570: 2069 7320 6e6f 206c 6f6e 6765 7220 686f   is no longer ho
-00002580: 7374 6564 2062 7920 7468 6520 7365 7276  sted by the serv
-00002590: 6572 2e22 5d2c 0a20 2020 2027 7572 6e3a  er."],.    'urn:
-000025a0: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
-000025b0: 6e73 3a78 6d70 702d 7374 7265 616d 7320  ns:xmpp-streams 
-000025c0: 686f 7374 2d75 6e6b 6e6f 776e 273a 205b  host-unknown': [
-000025d0: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
-000025e0: 2020 2020 2020 2020 2254 6865 2076 616c          "The val
-000025f0: 7565 206f 6620 7468 6520 2020 2020 2020  ue of the       
-00002600: 2027 746f 2720 6174 7472 6962 7574 6520   'to' attribute 
-00002610: 7072 6f76 6964 6564 2062 7920 7468 6520  provided by the 
-00002620: 696e 6974 6961 7469 6e67 2065 6e74 6974  initiating entit
-00002630: 7920 696e 2074 6865 2073 7472 6561 6d20  y in the stream 
-00002640: 6865 6164 6572 2064 6f65 7320 6e6f 7420  header does not 
-00002650: 636f 7272 6573 706f 6e64 2074 6f20 6120  correspond to a 
-00002660: 686f 7374 6e61 6d65 2074 6861 7420 6973  hostname that is
-00002670: 2068 6f73 7465 6420 6279 2074 6865 2073   hosted by the s
-00002680: 6572 7665 722e 225d 2c0a 2020 2020 2775  erver."],.    'u
-00002690: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
-000026a0: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
-000026b0: 6d73 2069 6d70 726f 7065 722d 6164 6472  ms improper-addr
-000026c0: 6573 7369 6e67 273a 205b 2727 2c0a 2020  essing': ['',.  
-000026d0: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
-000026e0: 2020 2241 2073 7461 6e7a 6120 7365 6e74    "A stanza sent
-000026f0: 2062 6574 7765 656e 2074 776f 2073 6572   between two ser
-00002700: 7665 7273 206c 6163 6b73 2061 2020 2020  vers lacks a    
-00002710: 2020 2020 2774 6f27 206f 7220 2766 726f      'to' or 'fro
-00002720: 6d27 2061 7474 7269 6275 7465 2028 6f72  m' attribute (or
-00002730: 2074 6865 2061 7474 7269 6275 7465 2068   the attribute h
-00002740: 6173 206e 6f20 7661 6c75 6529 2e22 5d2c  as no value)."],
-00002750: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
-00002760: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
-00002770: 702d 7374 7265 616d 7320 696e 7465 726e  p-streams intern
-00002780: 616c 2d73 6572 7665 722d 6572 726f 7227  al-server-error'
-00002790: 3a20 5b27 272c 0a20 2020 2020 2020 2027  : ['',.        '
-000027a0: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
-000027b0: 7365 7276 6572 2068 6173 2065 7870 6572  server has exper
-000027c0: 6965 6e63 6564 2061 206d 6973 636f 6e66  ienced a misconf
-000027d0: 6967 7572 6174 696f 6e20 6f72 2061 6e20  iguration or an 
-000027e0: 6f74 6865 7277 6973 652d 756e 6465 6669  otherwise-undefi
-000027f0: 6e65 6420 696e 7465 726e 616c 2065 7272  ned internal err
-00002800: 6f72 2074 6861 7420 7072 6576 656e 7473  or that prevents
-00002810: 2069 7420 6672 6f6d 2073 6572 7669 6369   it from servici
-00002820: 6e67 2074 6865 2073 7472 6561 6d2e 275d  ng the stream.']
-00002830: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
-00002840: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00002850: 7070 2d73 7472 6561 6d73 2069 6e76 616c  pp-streams inval
-00002860: 6964 2d66 726f 6d27 3a20 5b27 6361 6e63  id-from': ['canc
-00002870: 656c 272c 0a20 2020 2020 2020 2027 272c  el',.        '',
-00002880: 0a20 2020 2020 2020 2022 5468 6520 4a49  .        "The JI
-00002890: 4420 6f72 2068 6f73 746e 616d 6520 7072  D or hostname pr
-000028a0: 6f76 6964 6564 2069 6e20 6120 2020 2020  ovided in a     
-000028b0: 2020 2027 6672 6f6d 2720 6164 6472 6573     'from' addres
-000028c0: 7320 646f 6573 206e 6f74 206d 6174 6368  s does not match
-000028d0: 2061 6e20 6175 7468 6f72 697a 6564 204a   an authorized J
-000028e0: 4944 206f 7220 7661 6c69 6461 7465 6420  ID or validated 
-000028f0: 646f 6d61 696e 206e 6567 6f74 6961 7465  domain negotiate
-00002900: 6420 6265 7477 6565 6e20 7365 7276 6572  d between server
-00002910: 7320 7669 6120 5341 534c 206f 7220 6469  s via SASL or di
-00002920: 616c 6261 636b 2c20 6f72 2062 6574 7765  alback, or betwe
-00002930: 656e 2061 2063 6c69 656e 7420 616e 6420  en a client and 
-00002940: 6120 7365 7276 6572 2076 6961 2061 7574  a server via aut
-00002950: 6865 6e74 6963 6174 696f 6e20 616e 6420  hentication and 
-00002960: 7265 736f 7572 6365 2061 7574 686f 7269  resource authori
-00002970: 7a61 7469 6f6e 2e22 5d2c 0a20 2020 2027  zation."],.    '
-00002980: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00002990: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
-000029a0: 616d 7320 696e 7661 6c69 642d 6964 273a  ams invalid-id':
-000029b0: 205b 2727 2c0a 2020 2020 2020 2020 2727   ['',.        ''
-000029c0: 2c0a 2020 2020 2020 2020 2754 6865 2073  ,.        'The s
-000029d0: 7472 6561 6d20 4944 206f 7220 6469 616c  tream ID or dial
-000029e0: 6261 636b 2049 4420 6973 2069 6e76 616c  back ID is inval
-000029f0: 6964 206f 7220 646f 6573 206e 6f74 206d  id or does not m
-00002a00: 6174 6368 2061 6e20 4944 2070 7265 7669  atch an ID previ
-00002a10: 6f75 736c 7920 7072 6f76 6964 6564 2e27  ously provided.'
-00002a20: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
-00002a30: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00002a40: 6d70 702d 7374 7265 616d 7320 696e 7661  mpp-streams inva
-00002a50: 6c69 642d 6e61 6d65 7370 6163 6527 3a20  lid-namespace': 
-00002a60: 5b27 272c 0a20 2020 2020 2020 2027 272c  ['',.        '',
-00002a70: 0a20 2020 2020 2020 2027 5468 6520 7374  .        'The st
-00002a80: 7265 616d 7320 6e61 6d65 7370 6163 6520  reams namespace 
-00002a90: 6e61 6d65 2069 7320 736f 6d65 7468 696e  name is somethin
-00002aa0: 6720 6f74 6865 7220 7468 616e 2020 2020  g other than    
-00002ab0: 2020 2020 2268 7474 703a 2f2f 6574 6865      "http://ethe
-00002ac0: 7278 2e6a 6162 6265 722e 6f72 672f 7374  rx.jabber.org/st
-00002ad0: 7265 616d 7322 206f 7220 7468 6520 6469  reams" or the di
-00002ae0: 616c 6261 636b 206e 616d 6573 7061 6365  alback namespace
-00002af0: 206e 616d 6520 6973 2073 6f6d 6574 6869   name is somethi
-00002b00: 6e67 206f 7468 6572 2074 6861 6e20 226a  ng other than "j
-00002b10: 6162 6265 723a 7365 7276 6572 3a64 6961  abber:server:dia
-00002b20: 6c62 6163 6b22 2e27 5d2c 0a20 2020 2027  lback".'],.    '
-00002b30: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00002b40: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
-00002b50: 616d 7320 696e 7661 6c69 642d 786d 6c27  ams invalid-xml'
-00002b60: 3a20 5b27 272c 0a20 2020 2020 2020 2027  : ['',.        '
-00002b70: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
-00002b80: 656e 7469 7479 2068 6173 2073 656e 7420  entity has sent 
-00002b90: 696e 7661 6c69 6420 584d 4c20 6f76 6572  invalid XML over
-00002ba0: 2074 6865 2073 7472 6561 6d20 746f 2061   the stream to a
-00002bb0: 2073 6572 7665 7220 7468 6174 2070 6572   server that per
-00002bc0: 666f 726d 7320 7661 6c69 6461 7469 6f6e  forms validation
-00002bd0: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
-00002be0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-00002bf0: 3a78 6d70 702d 7374 7265 616d 7320 6e6f  :xmpp-streams no
-00002c00: 742d 6175 7468 6f72 697a 6564 273a 205b  t-authorized': [
-00002c10: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
-00002c20: 2020 2020 2020 2020 2754 6865 2065 6e74          'The ent
-00002c30: 6974 7920 6861 7320 6174 7465 6d70 7465  ity has attempte
-00002c40: 6420 746f 2073 656e 6420 6461 7461 2062  d to send data b
-00002c50: 6566 6f72 6520 7468 6520 7374 7265 616d  efore the stream
-00002c60: 2068 6173 2062 6565 6e20 6175 7468 656e   has been authen
-00002c70: 7469 6361 7465 642c 206f 7220 6f74 6865  ticated, or othe
-00002c80: 7277 6973 6520 6973 206e 6f74 2061 7574  rwise is not aut
-00002c90: 686f 7269 7a65 6420 746f 2070 6572 666f  horized to perfo
-00002ca0: 726d 2061 6e20 6163 7469 6f6e 2072 656c  rm an action rel
-00002cb0: 6174 6564 2074 6f20 7374 7265 616d 206e  ated to stream n
-00002cc0: 6567 6f74 6961 7469 6f6e 2e27 5d2c 0a20  egotiation.'],. 
-00002cd0: 2020 2027 7572 6e3a 6965 7466 3a70 6172     'urn:ietf:par
-00002ce0: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00002cf0: 7374 7265 616d 7320 706f 6c69 6379 2d76  streams policy-v
-00002d00: 696f 6c61 7469 6f6e 273a 205b 2727 2c0a  iolation': ['',.
-00002d10: 2020 2020 2020 2020 2727 2c0a 2020 2020          '',.    
-00002d20: 2020 2020 2754 6865 2065 6e74 6974 7920      'The entity 
-00002d30: 6861 7320 7669 6f6c 6174 6564 2073 6f6d  has violated som
-00002d40: 6520 6c6f 6361 6c20 7365 7276 6963 6520  e local service 
-00002d50: 706f 6c69 6379 2e27 5d2c 0a20 2020 2027  policy.'],.    '
-00002d60: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00002d70: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
-00002d80: 616d 7320 7265 6d6f 7465 2d63 6f6e 6e65  ams remote-conne
-00002d90: 6374 696f 6e2d 6661 696c 6564 273a 205b  ction-failed': [
-00002da0: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
-00002db0: 2020 2020 2020 2020 2754 6865 2073 6572          'The ser
-00002dc0: 7665 7220 6973 2075 6e61 626c 6520 746f  ver is unable to
-00002dd0: 2070 726f 7065 726c 7920 636f 6e6e 6563   properly connec
-00002de0: 7420 746f 2061 2072 656d 6f74 6520 7265  t to a remote re
-00002df0: 736f 7572 6365 2074 6861 7420 6973 2072  source that is r
-00002e00: 6571 7569 7265 6420 666f 7220 6175 7468  equired for auth
-00002e10: 656e 7469 6361 7469 6f6e 206f 7220 6175  entication or au
-00002e20: 7468 6f72 697a 6174 696f 6e2e 275d 2c0a  thorization.'],.
-00002e30: 2020 2020 2775 726e 3a69 6574 663a 7061      'urn:ietf:pa
-00002e40: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
-00002e50: 2d73 7472 6561 6d73 2072 6573 6f75 7263  -streams resourc
-00002e60: 652d 636f 6e73 7472 6169 6e74 273a 205b  e-constraint': [
-00002e70: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
-00002e80: 2020 2020 2020 2020 2754 6865 2073 6572          'The ser
-00002e90: 7665 7220 6c61 636b 7320 7468 6520 7379  ver lacks the sy
-00002ea0: 7374 656d 2072 6573 6f75 7263 6573 206e  stem resources n
-00002eb0: 6563 6573 7361 7279 2074 6f20 7365 7276  ecessary to serv
-00002ec0: 6963 6520 7468 6520 7374 7265 616d 2e27  ice the stream.'
-00002ed0: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
-00002ee0: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00002ef0: 6d70 702d 7374 7265 616d 7320 7265 7374  mpp-streams rest
-00002f00: 7269 6374 6564 2d78 6d6c 273a 205b 2727  ricted-xml': [''
-00002f10: 2c0a 2020 2020 2020 2020 2727 2c0a 2020  ,.        '',.  
-00002f20: 2020 2020 2020 2754 6865 2065 6e74 6974        'The entit
-00002f30: 7920 6861 7320 6174 7465 6d70 7465 6420  y has attempted 
-00002f40: 746f 2073 656e 6420 7265 7374 7269 6374  to send restrict
-00002f50: 6564 2058 4d4c 2066 6561 7475 7265 7320  ed XML features 
-00002f60: 7375 6368 2061 7320 6120 636f 6d6d 656e  such as a commen
-00002f70: 742c 2070 726f 6365 7373 696e 6720 696e  t, processing in
-00002f80: 7374 7275 6374 696f 6e2c 2044 5444 2c20  struction, DTD, 
-00002f90: 656e 7469 7479 2072 6566 6572 656e 6365  entity reference
-00002fa0: 2c20 6f72 2075 6e65 7363 6170 6564 2063  , or unescaped c
-00002fb0: 6861 7261 6374 6572 2e27 5d2c 0a20 2020  haracter.'],.   
-00002fc0: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
-00002fd0: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
-00002fe0: 7265 616d 7320 7365 652d 6f74 6865 722d  reams see-other-
-00002ff0: 686f 7374 273a 205b 2727 2c0a 2020 2020  host': ['',.    
-00003000: 2020 2020 2727 2c0a 2020 2020 2020 2020      '',.        
-00003010: 2754 6865 2073 6572 7665 7220 7769 6c6c  'The server will
-00003020: 206e 6f74 2070 726f 7669 6465 2073 6572   not provide ser
-00003030: 7669 6365 2074 6f20 7468 6520 696e 6974  vice to the init
-00003040: 6961 7469 6e67 2065 6e74 6974 7920 6275  iating entity bu
-00003050: 7420 6973 2072 6564 6972 6563 7469 6e67  t is redirecting
-00003060: 2074 7261 6666 6963 2074 6f20 616e 6f74   traffic to anot
-00003070: 6865 7220 686f 7374 2e27 5d2c 0a20 2020  her host.'],.   
-00003080: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
-00003090: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
-000030a0: 7265 616d 7320 7379 7374 656d 2d73 6875  reams system-shu
-000030b0: 7464 6f77 6e27 3a20 5b27 272c 0a20 2020  tdown': ['',.   
-000030c0: 2020 2020 2027 272c 0a20 2020 2020 2020       '',.       
-000030d0: 2027 5468 6520 7365 7276 6572 2069 7320   'The server is 
-000030e0: 6265 696e 6720 7368 7574 2064 6f77 6e20  being shut down 
-000030f0: 616e 6420 616c 6c20 6163 7469 7665 2073  and all active s
-00003100: 7472 6561 6d73 2061 7265 2062 6569 6e67  treams are being
-00003110: 2063 6c6f 7365 642e 275d 2c0a 2020 2020   closed.'],.    
-00003120: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
-00003130: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
-00003140: 6561 6d73 2075 6e64 6566 696e 6564 2d63  eams undefined-c
-00003150: 6f6e 6469 7469 6f6e 273a 205b 2727 2c0a  ondition': ['',.
-00003160: 2020 2020 2020 2020 2727 2c0a 2020 2020          '',.    
-00003170: 2020 2020 2754 6865 2065 7272 6f72 2063      'The error c
-00003180: 6f6e 6469 7469 6f6e 2069 7320 6e6f 7420  ondition is not 
-00003190: 6f6e 6520 6f66 2074 686f 7365 2064 6566  one of those def
-000031a0: 696e 6564 2062 7920 7468 6520 6f74 6865  ined by the othe
-000031b0: 7220 636f 6e64 6974 696f 6e73 2069 6e20  r conditions in 
-000031c0: 7468 6973 206c 6973 742e 275d 2c0a 2020  this list.'],.  
-000031d0: 2020 2775 726e 3a69 6574 663a 7061 7261    'urn:ietf:para
-000031e0: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
-000031f0: 7472 6561 6d73 2075 6e73 7570 706f 7274  treams unsupport
-00003200: 6564 2d65 6e63 6f64 696e 6727 3a20 5b27  ed-encoding': ['
-00003210: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
-00003220: 2020 2020 2020 2027 5468 6520 696e 6974         'The init
-00003230: 6961 7469 6e67 2065 6e74 6974 7920 6861  iating entity ha
-00003240: 7320 656e 636f 6465 6420 7468 6520 7374  s encoded the st
-00003250: 7265 616d 2069 6e20 616e 2065 6e63 6f64  ream in an encod
-00003260: 696e 6720 7468 6174 2069 7320 6e6f 7420  ing that is not 
-00003270: 7375 7070 6f72 7465 6420 6279 2074 6865  supported by the
-00003280: 2073 6572 7665 722e 275d 2c0a 2020 2020   server.'],.    
-00003290: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
-000032a0: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
-000032b0: 6561 6d73 2075 6e73 7570 706f 7274 6564  eams unsupported
-000032c0: 2d73 7461 6e7a 612d 7479 7065 273a 205b  -stanza-type': [
-000032d0: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
-000032e0: 2020 2020 2020 2020 2754 6865 2069 6e69          'The ini
-000032f0: 7469 6174 696e 6720 656e 7469 7479 2068  tiating entity h
-00003300: 6173 2073 656e 7420 6120 6669 7273 742d  as sent a first-
-00003310: 6c65 7665 6c20 6368 696c 6420 6f66 2074  level child of t
-00003320: 6865 2073 7472 6561 6d20 7468 6174 2069  he stream that i
-00003330: 7320 6e6f 7420 7375 7070 6f72 7465 6420  s not supported 
-00003340: 6279 2074 6865 2073 6572 7665 722e 275d  by the server.']
-00003350: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
-00003360: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00003370: 7070 2d73 7472 6561 6d73 2075 6e73 7570  pp-streams unsup
-00003380: 706f 7274 6564 2d76 6572 7369 6f6e 273a  ported-version':
-00003390: 205b 2727 2c0a 2020 2020 2020 2020 2727   ['',.        ''
-000033a0: 2c0a 2020 2020 2020 2020 2254 6865 2076  ,.        "The v
-000033b0: 616c 7565 206f 6620 7468 6520 2020 2020  alue of the     
-000033c0: 2020 2027 7665 7273 696f 6e27 2061 7474     'version' att
-000033d0: 7269 6275 7465 2070 726f 7669 6465 6420  ribute provided 
-000033e0: 6279 2074 6865 2069 6e69 7469 6174 696e  by the initiatin
-000033f0: 6720 656e 7469 7479 2069 6e20 7468 6520  g entity in the 
-00003400: 7374 7265 616d 2068 6561 6465 7220 7370  stream header sp
-00003410: 6563 6966 6965 7320 6120 7665 7273 696f  ecifies a versio
-00003420: 6e20 6f66 2058 4d50 5020 7468 6174 2069  n of XMPP that i
-00003430: 7320 6e6f 7420 7375 7070 6f72 7465 6420  s not supported 
-00003440: 6279 2074 6865 2073 6572 7665 722e 225d  by the server."]
-00003450: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
-00003460: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00003470: 7070 2d73 7472 6561 6d73 2078 6d6c 2d6e  pp-streams xml-n
-00003480: 6f74 2d77 656c 6c2d 666f 726d 6564 273a  ot-well-formed':
-00003490: 205b 2727 2c0a 2020 2020 2020 2020 2727   ['',.        ''
-000034a0: 2c0a 2020 2020 2020 2020 2754 6865 2069  ,.        'The i
-000034b0: 6e69 7469 6174 696e 6720 656e 7469 7479  nitiating entity
-000034c0: 2068 6173 2073 656e 7420 584d 4c20 7468   has sent XML th
-000034d0: 6174 2069 7320 6e6f 7420 7765 6c6c 2d66  at is not well-f
-000034e0: 6f72 6d65 642e 275d 0a7d 0a0a 5f65 7272  ormed.'].}.._err
-000034f0: 6f72 636f 6465 7320 3d20 7b0a 2020 2020  orcodes = {.    
-00003500: 2733 3032 273a 2027 7265 6469 7265 6374  '302': 'redirect
-00003510: 272c 0a20 2020 2027 3430 3027 3a20 2775  ',.    '400': 'u
-00003520: 6e65 7870 6563 7465 642d 7265 7175 6573  nexpected-reques
-00003530: 7427 2c0a 2020 2020 2734 3031 273a 2027  t',.    '401': '
-00003540: 6e6f 742d 6175 7468 6f72 697a 6564 272c  not-authorized',
-00003550: 0a20 2020 2027 3430 3227 3a20 2770 6179  .    '402': 'pay
-00003560: 6d65 6e74 2d72 6571 7569 7265 6427 2c0a  ment-required',.
-00003570: 2020 2020 2734 3033 273a 2027 666f 7262      '403': 'forb
-00003580: 6964 6465 6e27 2c0a 2020 2020 2734 3034  idden',.    '404
-00003590: 273a 2027 7265 6d6f 7465 2d73 6572 7665  ': 'remote-serve
-000035a0: 722d 6e6f 742d 666f 756e 6427 2c0a 2020  r-not-found',.  
-000035b0: 2020 2734 3035 273a 2027 6e6f 742d 616c    '405': 'not-al
-000035c0: 6c6f 7765 6427 2c0a 2020 2020 2734 3036  lowed',.    '406
-000035d0: 273a 2027 6e6f 742d 6163 6365 7074 6162  ': 'not-acceptab
-000035e0: 6c65 272c 0a20 2020 2027 3430 3727 3a20  le',.    '407': 
-000035f0: 2773 7562 7363 7269 7074 696f 6e2d 7265  'subscription-re
-00003600: 7175 6972 6564 272c 0a20 2020 2027 3430  quired',.    '40
-00003610: 3927 3a20 2763 6f6e 666c 6963 7427 2c0a  9': 'conflict',.
-00003620: 2020 2020 2735 3030 273a 2027 756e 6465      '500': 'unde
-00003630: 6669 6e65 642d 636f 6e64 6974 696f 6e27  fined-condition'
-00003640: 2c0a 2020 2020 2735 3031 273a 2027 6665  ,.    '501': 'fe
-00003650: 6174 7572 652d 6e6f 742d 696d 706c 656d  ature-not-implem
-00003660: 656e 7465 6427 2c0a 2020 2020 2735 3033  ented',.    '503
-00003670: 273a 2027 7365 7276 6963 652d 756e 6176  ': 'service-unav
-00003680: 6169 6c61 626c 6527 2c0a 2020 2020 2735  ailable',.    '5
-00003690: 3034 273a 2027 7265 6d6f 7465 2d73 6572  04': 'remote-ser
-000036a0: 7665 722d 7469 6d65 6f75 7427 2c0a 2020  ver-timeout',.  
-000036b0: 2020 2763 616e 6365 6c27 3a20 2769 6e76    'cancel': 'inv
-000036c0: 616c 6964 2d66 726f 6d27 0a7d 0a0a 0a5f  alid-from'.}..._
-000036d0: 6c6f 6361 6c70 6172 745f 6573 6361 7065  localpart_escape
-000036e0: 5f63 6861 7273 203d 2027 2022 265c 272f  _chars = ' "&\'/
-000036f0: 3a3c 3e40 270a 0a0a 5354 5245 414d 5f4e  :<>@'...STREAM_N
-00003700: 4f54 5f41 5554 484f 5249 5a45 4420 3d20  OT_AUTHORIZED = 
-00003710: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
-00003720: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
-00003730: 6561 6d73 206e 6f74 2d61 7574 686f 7269  eams not-authori
-00003740: 7a65 6427 0a53 5452 4541 4d5f 5245 4d4f  zed'.STREAM_REMO
-00003750: 5445 5f43 4f4e 4e45 4354 494f 4e5f 4641  TE_CONNECTION_FA
-00003760: 494c 4544 203d 2027 7572 6e3a 6965 7466  ILED = 'urn:ietf
-00003770: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00003780: 6d70 702d 7374 7265 616d 7320 7265 6d6f  mpp-streams remo
-00003790: 7465 2d63 6f6e 6e65 6374 696f 6e2d 6661  te-connection-fa
-000037a0: 696c 6564 270a 5341 534c 5f4d 4543 4841  iled'.SASL_MECHA
-000037b0: 4e49 534d 5f54 4f4f 5f57 4541 4b20 3d20  NISM_TOO_WEAK = 
-000037c0: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
-000037d0: 3a78 6d6c 3a6e 733a 786d 7070 2d73 6173  :xml:ns:xmpp-sas
-000037e0: 6c20 6d65 6368 616e 6973 6d2d 746f 6f2d  l mechanism-too-
-000037f0: 7765 616b 270a 5354 5245 414d 5f58 4d4c  weak'.STREAM_XML
-00003800: 5f4e 4f54 5f57 454c 4c5f 464f 524d 4544  _NOT_WELL_FORMED
-00003810: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
-00003820: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00003830: 7374 7265 616d 7320 786d 6c2d 6e6f 742d  streams xml-not-
-00003840: 7765 6c6c 2d66 6f72 6d65 6427 0a45 5252  well-formed'.ERR
-00003850: 5f4a 4944 5f4d 414c 464f 524d 4544 203d  _JID_MALFORMED =
-00003860: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
-00003870: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
-00003880: 616e 7a61 7320 6a69 642d 6d61 6c66 6f72  anzas jid-malfor
-00003890: 6d65 6427 0a53 5452 4541 4d5f 5345 455f  med'.STREAM_SEE_
-000038a0: 4f54 4845 525f 484f 5354 203d 2027 7572  OTHER_HOST = 'ur
-000038b0: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
-000038c0: 6c3a 6e73 3a78 6d70 702d 7374 7265 616d  l:ns:xmpp-stream
-000038d0: 7320 7365 652d 6f74 6865 722d 686f 7374  s see-other-host
-000038e0: 270a 5354 5245 414d 5f42 4144 5f4e 414d  '.STREAM_BAD_NAM
-000038f0: 4553 5041 4345 5f50 5245 4649 5820 3d20  ESPACE_PREFIX = 
-00003900: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
-00003910: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
-00003920: 6561 6d73 2062 6164 2d6e 616d 6573 7061  eams bad-namespa
-00003930: 6365 2d70 7265 6669 7827 0a45 5252 5f53  ce-prefix'.ERR_S
-00003940: 4552 5649 4345 5f55 4e41 5641 494c 4142  ERVICE_UNAVAILAB
-00003950: 4c45 203d 2027 7572 6e3a 6965 7466 3a70  LE = 'urn:ietf:p
-00003960: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
-00003970: 702d 7374 616e 7a61 7320 7365 7276 6963  p-stanzas servic
-00003980: 652d 756e 6176 6169 6c61 626c 6527 0a53  e-unavailable'.S
-00003990: 5452 4541 4d5f 434f 4e4e 4543 5449 4f4e  TREAM_CONNECTION
-000039a0: 5f54 494d 454f 5554 203d 2027 7572 6e3a  _TIMEOUT = 'urn:
-000039b0: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
-000039c0: 6e73 3a78 6d70 702d 7374 7265 616d 7320  ns:xmpp-streams 
-000039d0: 636f 6e6e 6563 7469 6f6e 2d74 696d 656f  connection-timeo
-000039e0: 7574 270a 5354 5245 414d 5f55 4e53 5550  ut'.STREAM_UNSUP
-000039f0: 504f 5254 4544 5f56 4552 5349 4f4e 203d  PORTED_VERSION =
-00003a00: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
-00003a10: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
-00003a20: 7265 616d 7320 756e 7375 7070 6f72 7465  reams unsupporte
-00003a30: 642d 7665 7273 696f 6e27 0a53 5452 4541  d-version'.STREA
-00003a40: 4d5f 494d 5052 4f50 4552 5f41 4444 5245  M_IMPROPER_ADDRE
-00003a50: 5353 494e 4720 3d20 2775 726e 3a69 6574  SSING = 'urn:iet
-00003a60: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-00003a70: 786d 7070 2d73 7472 6561 6d73 2069 6d70  xmpp-streams imp
-00003a80: 726f 7065 722d 6164 6472 6573 7369 6e67  roper-addressing
-00003a90: 270a 5354 5245 414d 5f55 4e44 4546 494e  '.STREAM_UNDEFIN
-00003aa0: 4544 5f43 4f4e 4449 5449 4f4e 203d 2027  ED_CONDITION = '
-00003ab0: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00003ac0: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
-00003ad0: 616d 7320 756e 6465 6669 6e65 642d 636f  ams undefined-co
-00003ae0: 6e64 6974 696f 6e27 0a53 4153 4c5f 4e4f  ndition'.SASL_NO
-00003af0: 545f 4155 5448 4f52 495a 4544 203d 2027  T_AUTHORIZED = '
-00003b00: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00003b10: 786d 6c3a 6e73 3a78 6d70 702d 7361 736c  xml:ns:xmpp-sasl
-00003b20: 206e 6f74 2d61 7574 686f 7269 7a65 6427   not-authorized'
-00003b30: 0a45 5252 5f47 4f4e 4520 3d20 2775 726e  .ERR_GONE = 'urn
-00003b40: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
-00003b50: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
-00003b60: 2067 6f6e 6527 0a53 4153 4c5f 5445 4d50   gone'.SASL_TEMP
-00003b70: 4f52 4152 595f 4155 5448 5f46 4149 4c55  ORARY_AUTH_FAILU
-00003b80: 5245 203d 2027 7572 6e3a 6965 7466 3a70  RE = 'urn:ietf:p
-00003b90: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
-00003ba0: 702d 7361 736c 2074 656d 706f 7261 7279  p-sasl temporary
-00003bb0: 2d61 7574 682d 6661 696c 7572 6527 0a45  -auth-failure'.E
-00003bc0: 5252 5f52 454d 4f54 455f 5345 5256 4552  RR_REMOTE_SERVER
-00003bd0: 5f4e 4f54 5f46 4f55 4e44 203d 2027 7572  _NOT_FOUND = 'ur
-00003be0: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
-00003bf0: 6c3a 6e73 3a78 6d70 702d 7374 616e 7a61  l:ns:xmpp-stanza
-00003c00: 7320 7265 6d6f 7465 2d73 6572 7665 722d  s remote-server-
-00003c10: 6e6f 742d 666f 756e 6427 0a45 5252 5f55  not-found'.ERR_U
-00003c20: 4e45 5850 4543 5445 445f 5245 5155 4553  NEXPECTED_REQUES
-00003c30: 5420 3d20 2775 726e 3a69 6574 663a 7061  T = 'urn:ietf:pa
-00003c40: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
-00003c50: 2d73 7461 6e7a 6173 2075 6e65 7870 6563  -stanzas unexpec
-00003c60: 7465 642d 7265 7175 6573 7427 0a45 5252  ted-request'.ERR
-00003c70: 5f52 4543 4950 4945 4e54 5f55 4e41 5641  _RECIPIENT_UNAVA
-00003c80: 494c 4142 4c45 203d 2027 7572 6e3a 6965  ILABLE = 'urn:ie
-00003c90: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-00003ca0: 3a78 6d70 702d 7374 616e 7a61 7320 7265  :xmpp-stanzas re
-00003cb0: 6369 7069 656e 742d 756e 6176 6169 6c61  cipient-unavaila
-00003cc0: 626c 6527 0a45 5252 5f43 4f4e 464c 4943  ble'.ERR_CONFLIC
-00003cd0: 5420 3d20 2775 726e 3a69 6574 663a 7061  T = 'urn:ietf:pa
-00003ce0: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
-00003cf0: 2d73 7461 6e7a 6173 2063 6f6e 666c 6963  -stanzas conflic
-00003d00: 7427 0a53 5452 4541 4d5f 5359 5354 454d  t'.STREAM_SYSTEM
-00003d10: 5f53 4855 5444 4f57 4e20 3d20 2775 726e  _SHUTDOWN = 'urn
-00003d20: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
-00003d30: 3a6e 733a 786d 7070 2d73 7472 6561 6d73  :ns:xmpp-streams
-00003d40: 2073 7973 7465 6d2d 7368 7574 646f 776e   system-shutdown
-00003d50: 270a 5354 5245 414d 5f42 4144 5f46 4f52  '.STREAM_BAD_FOR
-00003d60: 4d41 5420 3d20 2775 726e 3a69 6574 663a  MAT = 'urn:ietf:
-00003d70: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00003d80: 7070 2d73 7472 6561 6d73 2062 6164 2d66  pp-streams bad-f
-00003d90: 6f72 6d61 7427 0a45 5252 5f53 5542 5343  ormat'.ERR_SUBSC
-00003da0: 5249 5054 494f 4e5f 5245 5155 4952 4544  RIPTION_REQUIRED
-00003db0: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
-00003dc0: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00003dd0: 7374 616e 7a61 7320 7375 6273 6372 6970  stanzas subscrip
-00003de0: 7469 6f6e 2d72 6571 7569 7265 6427 0a53  tion-required'.S
-00003df0: 5452 4541 4d5f 494e 5445 524e 414c 5f53  TREAM_INTERNAL_S
-00003e00: 4552 5645 525f 4552 524f 5220 3d20 2775  ERVER_ERROR = 'u
-00003e10: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
-00003e20: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
-00003e30: 6d73 2069 6e74 6572 6e61 6c2d 7365 7276  ms internal-serv
-00003e40: 6572 2d65 7272 6f72 270a 4552 525f 4e4f  er-error'.ERR_NO
-00003e50: 545f 4155 5448 4f52 495a 4544 203d 2027  T_AUTHORIZED = '
-00003e60: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00003e70: 786d 6c3a 6e73 3a78 6d70 702d 7374 616e  xml:ns:xmpp-stan
-00003e80: 7a61 7320 6e6f 742d 6175 7468 6f72 697a  zas not-authoriz
-00003e90: 6564 270a 5341 534c 5f41 424f 5254 4544  ed'.SASL_ABORTED
-00003ea0: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
-00003eb0: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00003ec0: 7361 736c 2061 626f 7274 6564 270a 4552  sasl aborted'.ER
-00003ed0: 525f 5245 4749 5354 5241 5449 4f4e 5f52  R_REGISTRATION_R
-00003ee0: 4551 5549 5245 4420 3d20 2775 726e 3a69  EQUIRED = 'urn:i
-00003ef0: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
-00003f00: 733a 786d 7070 2d73 7461 6e7a 6173 2072  s:xmpp-stanzas r
-00003f10: 6567 6973 7472 6174 696f 6e2d 7265 7175  egistration-requ
-00003f20: 6972 6564 270a 4552 525f 494e 5445 524e  ired'.ERR_INTERN
-00003f30: 414c 5f53 4552 5645 525f 4552 524f 5220  AL_SERVER_ERROR 
-00003f40: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
-00003f50: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
-00003f60: 7461 6e7a 6173 2069 6e74 6572 6e61 6c2d  tanzas internal-
-00003f70: 7365 7276 6572 2d65 7272 6f72 270a 5341  server-error'.SA
-00003f80: 534c 5f49 4e43 4f52 5245 4354 5f45 4e43  SL_INCORRECT_ENC
-00003f90: 4f44 494e 4720 3d20 2775 726e 3a69 6574  ODING = 'urn:iet
-00003fa0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-00003fb0: 786d 7070 2d73 6173 6c20 696e 636f 7272  xmpp-sasl incorr
-00003fc0: 6563 742d 656e 636f 6469 6e67 270a 5354  ect-encoding'.ST
-00003fd0: 5245 414d 5f48 4f53 545f 474f 4e45 203d  REAM_HOST_GONE =
-00003fe0: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
-00003ff0: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
-00004000: 7265 616d 7320 686f 7374 2d67 6f6e 6527  reams host-gone'
-00004010: 0a53 5452 4541 4d5f 504f 4c49 4359 5f56  .STREAM_POLICY_V
-00004020: 494f 4c41 5449 4f4e 203d 2027 7572 6e3a  IOLATION = 'urn:
-00004030: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
-00004040: 6e73 3a78 6d70 702d 7374 7265 616d 7320  ns:xmpp-streams 
-00004050: 706f 6c69 6379 2d76 696f 6c61 7469 6f6e  policy-violation
-00004060: 270a 5354 5245 414d 5f49 4e56 414c 4944  '.STREAM_INVALID
-00004070: 5f58 4d4c 203d 2027 7572 6e3a 6965 7466  _XML = 'urn:ietf
-00004080: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00004090: 6d70 702d 7374 7265 616d 7320 696e 7661  mpp-streams inva
-000040a0: 6c69 642d 786d 6c27 0a53 5452 4541 4d5f  lid-xml'.STREAM_
-000040b0: 434f 4e46 4c49 4354 203d 2027 7572 6e3a  CONFLICT = 'urn:
-000040c0: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
-000040d0: 6e73 3a78 6d70 702d 7374 7265 616d 7320  ns:xmpp-streams 
-000040e0: 636f 6e66 6c69 6374 270a 5354 5245 414d  conflict'.STREAM
-000040f0: 5f52 4553 4f55 5243 455f 434f 4e53 5452  _RESOURCE_CONSTR
-00004100: 4149 4e54 203d 2027 7572 6e3a 6965 7466  AINT = 'urn:ietf
-00004110: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00004120: 6d70 702d 7374 7265 616d 7320 7265 736f  mpp-streams reso
-00004130: 7572 6365 2d63 6f6e 7374 7261 696e 7427  urce-constraint'
-00004140: 0a53 5452 4541 4d5f 554e 5355 5050 4f52  .STREAM_UNSUPPOR
-00004150: 5445 445f 454e 434f 4449 4e47 203d 2027  TED_ENCODING = '
-00004160: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00004170: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
-00004180: 616d 7320 756e 7375 7070 6f72 7465 642d  ams unsupported-
-00004190: 656e 636f 6469 6e67 270a 4552 525f 4e4f  encoding'.ERR_NO
-000041a0: 545f 414c 4c4f 5745 4420 3d20 2775 726e  T_ALLOWED = 'urn
-000041b0: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
-000041c0: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
-000041d0: 206e 6f74 2d61 6c6c 6f77 6564 270a 4552   not-allowed'.ER
-000041e0: 525f 4954 454d 5f4e 4f54 5f46 4f55 4e44  R_ITEM_NOT_FOUND
-000041f0: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
-00004200: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00004210: 7374 616e 7a61 7320 6974 656d 2d6e 6f74  stanzas item-not
-00004220: 2d66 6f75 6e64 270a 4552 525f 4e4f 545f  -found'.ERR_NOT_
-00004230: 4143 4345 5054 4142 4c45 203d 2027 7572  ACCEPTABLE = 'ur
-00004240: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
-00004250: 6c3a 6e73 3a78 6d70 702d 7374 616e 7a61  l:ns:xmpp-stanza
-00004260: 7320 6e6f 742d 6163 6365 7074 6162 6c65  s not-acceptable
-00004270: 270a 5354 5245 414d 5f49 4e56 414c 4944  '.STREAM_INVALID
-00004280: 5f46 524f 4d20 3d20 2775 726e 3a69 6574  _FROM = 'urn:iet
-00004290: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-000042a0: 786d 7070 2d73 7472 6561 6d73 2069 6e76  xmpp-streams inv
-000042b0: 616c 6964 2d66 726f 6d27 0a45 5252 5f46  alid-from'.ERR_F
-000042c0: 4541 5455 5245 5f4e 4f54 5f49 4d50 4c45  EATURE_NOT_IMPLE
-000042d0: 4d45 4e54 4544 203d 2027 7572 6e3a 6965  MENTED = 'urn:ie
-000042e0: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-000042f0: 3a78 6d70 702d 7374 616e 7a61 7320 6665  :xmpp-stanzas fe
-00004300: 6174 7572 652d 6e6f 742d 696d 706c 656d  ature-not-implem
-00004310: 656e 7465 6427 0a45 5252 5f42 4144 5f52  ented'.ERR_BAD_R
-00004320: 4551 5545 5354 203d 2027 7572 6e3a 6965  EQUEST = 'urn:ie
-00004330: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
-00004340: 3a78 6d70 702d 7374 616e 7a61 7320 6261  :xmpp-stanzas ba
-00004350: 642d 7265 7175 6573 7427 0a53 5452 4541  d-request'.STREA
-00004360: 4d5f 494e 5641 4c49 445f 4944 203d 2027  M_INVALID_ID = '
-00004370: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
-00004380: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
-00004390: 616d 7320 696e 7661 6c69 642d 6964 270a  ams invalid-id'.
-000043a0: 5354 5245 414d 5f48 4f53 545f 554e 4b4e  STREAM_HOST_UNKN
-000043b0: 4f57 4e20 3d20 2775 726e 3a69 6574 663a  OWN = 'urn:ietf:
-000043c0: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-000043d0: 7070 2d73 7472 6561 6d73 2068 6f73 742d  pp-streams host-
-000043e0: 756e 6b6e 6f77 6e27 0a45 5252 5f55 4e44  unknown'.ERR_UND
-000043f0: 4546 494e 4544 5f43 4f4e 4449 5449 4f4e  EFINED_CONDITION
-00004400: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
-00004410: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-00004420: 7374 616e 7a61 7320 756e 6465 6669 6e65  stanzas undefine
-00004430: 642d 636f 6e64 6974 696f 6e27 0a53 4153  d-condition'.SAS
-00004440: 4c5f 494e 5641 4c49 445f 4d45 4348 414e  L_INVALID_MECHAN
-00004450: 4953 4d20 3d20 2775 726e 3a69 6574 663a  ISM = 'urn:ietf:
-00004460: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
-00004470: 7070 2d73 6173 6c20 696e 7661 6c69 642d  pp-sasl invalid-
-00004480: 6d65 6368 616e 6973 6d27 0a53 5452 4541  mechanism'.STREA
-00004490: 4d5f 5245 5354 5249 4354 4544 5f58 4d4c  M_RESTRICTED_XML
-000044a0: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
-000044b0: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
-000044c0: 7374 7265 616d 7320 7265 7374 7269 6374  streams restrict
-000044d0: 6564 2d78 6d6c 270a 4552 525f 5245 534f  ed-xml'.ERR_RESO
-000044e0: 5552 4345 5f43 4f4e 5354 5241 494e 5420  URCE_CONSTRAINT 
-000044f0: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
-00004500: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
-00004510: 7461 6e7a 6173 2072 6573 6f75 7263 652d  tanzas resource-
-00004520: 636f 6e73 7472 6169 6e74 270a 4552 525f  constraint'.ERR_
-00004530: 5245 4d4f 5445 5f53 4552 5645 525f 5449  REMOTE_SERVER_TI
-00004540: 4d45 4f55 5420 3d20 2775 726e 3a69 6574  MEOUT = 'urn:iet
-00004550: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
-00004560: 786d 7070 2d73 7461 6e7a 6173 2072 656d  xmpp-stanzas rem
-00004570: 6f74 652d 7365 7276 6572 2d74 696d 656f  ote-server-timeo
-00004580: 7574 270a 5341 534c 5f49 4e56 414c 4944  ut'.SASL_INVALID
-00004590: 5f41 5554 485a 4944 203d 2027 7572 6e3a  _AUTHZID = 'urn:
-000045a0: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
-000045b0: 6e73 3a78 6d70 702d 7361 736c 2069 6e76  ns:xmpp-sasl inv
-000045c0: 616c 6964 2d61 7574 687a 6964 270a 4552  alid-authzid'.ER
-000045d0: 525f 5041 594d 454e 545f 5245 5155 4952  R_PAYMENT_REQUIR
-000045e0: 4544 203d 2027 7572 6e3a 6965 7466 3a70  ED = 'urn:ietf:p
-000045f0: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
-00004600: 702d 7374 616e 7a61 7320 7061 796d 656e  p-stanzas paymen
-00004610: 742d 7265 7175 6972 6564 270a 5354 5245  t-required'.STRE
-00004620: 414d 5f49 4e56 414c 4944 5f4e 414d 4553  AM_INVALID_NAMES
-00004630: 5041 4345 203d 2027 7572 6e3a 6965 7466  PACE = 'urn:ietf
-00004640: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
-00004650: 6d70 702d 7374 7265 616d 7320 696e 7661  mpp-streams inva
-00004660: 6c69 642d 6e61 6d65 7370 6163 6527 0a45  lid-namespace'.E
-00004670: 5252 5f52 4544 4952 4543 5420 3d20 2775  RR_REDIRECT = 'u
-00004680: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
-00004690: 6d6c 3a6e 733a 786d 7070 2d73 7461 6e7a  ml:ns:xmpp-stanz
-000046a0: 6173 2072 6564 6972 6563 7427 0a53 5452  as redirect'.STR
-000046b0: 4541 4d5f 554e 5355 5050 4f52 5445 445f  EAM_UNSUPPORTED_
-000046c0: 5354 414e 5a41 5f54 5950 4520 3d20 2775  STANZA_TYPE = 'u
-000046d0: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
-000046e0: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
-000046f0: 6d73 2075 6e73 7570 706f 7274 6564 2d73  ms unsupported-s
-00004700: 7461 6e7a 612d 7479 7065 270a 4552 525f  tanza-type'.ERR_
-00004710: 464f 5242 4944 4445 4e20 3d20 2775 726e  FORBIDDEN = 'urn
-00004720: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
-00004730: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
-00004740: 2066 6f72 6269 6464 656e 270a 0a0a 6465   forbidden'...de
-00004750: 6620 6973 5265 7375 6c74 4e6f 6465 286e  f isResultNode(n
-00004760: 6f64 6529 3a0a 2020 2020 2222 220a 2020  ode):.    """.  
-00004770: 2020 5265 7475 726e 2074 7275 6520 6966    Return true if
-00004780: 2074 6865 206e 6f64 6520 6973 2061 2070   the node is a p
-00004790: 6f73 6974 6976 6520 7265 706c 790a 2020  ositive reply.  
-000047a0: 2020 2222 220a 2020 2020 7265 7475 726e    """.    return
-000047b0: 206e 6f64 6520 616e 6420 6e6f 6465 2e67   node and node.g
-000047c0: 6574 5479 7065 2829 203d 3d20 2772 6573  etType() == 'res
-000047d0: 756c 7427 0a0a 6465 6620 6973 4572 726f  ult'..def isErro
-000047e0: 724e 6f64 6528 6e6f 6465 293a 0a20 2020  rNode(node):.   
-000047f0: 2022 2222 0a20 2020 2052 6574 7572 6e20   """.    Return 
-00004800: 7472 7565 2069 6620 7468 6520 6e6f 6465  true if the node
-00004810: 2069 7320 6120 6e65 6761 7469 7665 2072   is a negative r
-00004820: 6570 6c79 0a20 2020 2022 2222 0a20 2020  eply.    """.   
-00004830: 2072 6574 7572 6e20 6e6f 6465 2061 6e64   return node and
-00004840: 206e 6f64 652e 6765 7454 7970 6528 2920   node.getType() 
-00004850: 3d3d 2027 6572 726f 7227 0a0a 6465 6620  == 'error'..def 
-00004860: 6973 4d75 6350 4d28 6d65 7373 6167 6529  isMucPM(message)
-00004870: 3a0a 2020 2020 6d75 635f 7573 6572 203d  :.    muc_user =
-00004880: 206d 6573 7361 6765 2e67 6574 5461 6728   message.getTag(
-00004890: 2778 272c 206e 616d 6573 7061 6365 3d4e  'x', namespace=N
-000048a0: 616d 6573 7061 6365 2e4d 5543 5f55 5345  amespace.MUC_USE
-000048b0: 5229 0a20 2020 2072 6574 7572 6e20 286d  R).    return (m
-000048c0: 6573 7361 6765 2e67 6574 5479 7065 2829  essage.getType()
-000048d0: 2069 6e20 2827 6368 6174 272c 2027 6572   in ('chat', 'er
-000048e0: 726f 7227 2920 616e 640a 2020 2020 2020  ror') and.      
-000048f0: 2020 2020 2020 6d75 635f 7573 6572 2069        muc_user i
-00004900: 7320 6e6f 7420 4e6f 6e65 2061 6e64 0a20  s not None and. 
-00004910: 2020 2020 2020 2020 2020 206e 6f74 206d             not m
-00004920: 7563 5f75 7365 722e 6765 7443 6869 6c64  uc_user.getChild
-00004930: 7265 6e28 2929 0a0a 636c 6173 7320 4e6f  ren())..class No
-00004940: 6465 5072 6f63 6573 7365 6428 4578 6365  deProcessed(Exce
-00004950: 7074 696f 6e29 3a0a 2020 2020 2222 220a  ption):.    """.
-00004960: 2020 2020 4578 6365 7074 696f 6e20 7468      Exception th
-00004970: 6174 2073 686f 756c 6420 6265 2072 6169  at should be rai
-00004980: 7365 6420 6279 2068 616e 646c 6572 2077  sed by handler w
-00004990: 6865 6e20 7468 6520 6861 6e64 6c69 6e67  hen the handling
-000049a0: 2073 686f 756c 6420 6265 0a20 2020 2073   should be.    s
-000049b0: 746f 7070 6564 0a20 2020 2022 2222 0a0a  topped.    """..
-000049c0: 636c 6173 7320 5374 7265 616d 4572 726f  class StreamErro
-000049d0: 7228 4578 6365 7074 696f 6e29 3a0a 2020  r(Exception):.  
-000049e0: 2020 2222 220a 2020 2020 4261 7365 2065    """.    Base e
-000049f0: 7863 6570 7469 6f6e 2063 6c61 7373 2066  xception class f
-00004a00: 6f72 2073 7472 6561 6d20 6572 726f 7273  or stream errors
-00004a10: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-00004a20: 4261 6446 6f72 6d61 7428 5374 7265 616d  BadFormat(Stream
-00004a30: 4572 726f 7229 3a0a 2020 2020 7061 7373  Error):.    pass
-00004a40: 0a0a 636c 6173 7320 4261 644e 616d 6573  ..class BadNames
-00004a50: 7061 6365 5072 6566 6978 2853 7472 6561  pacePrefix(Strea
-00004a60: 6d45 7272 6f72 293a 0a20 2020 2070 6173  mError):.    pas
-00004a70: 730a 0a63 6c61 7373 2043 6f6e 666c 6963  s..class Conflic
-00004a80: 7428 5374 7265 616d 4572 726f 7229 3a0a  t(StreamError):.
-00004a90: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
-00004aa0: 436f 6e6e 6563 7469 6f6e 5469 6d65 6f75  ConnectionTimeou
-00004ab0: 7428 5374 7265 616d 4572 726f 7229 3a0a  t(StreamError):.
-00004ac0: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
-00004ad0: 486f 7374 476f 6e65 2853 7472 6561 6d45  HostGone(StreamE
-00004ae0: 7272 6f72 293a 0a20 2020 2070 6173 730a  rror):.    pass.
-00004af0: 0a63 6c61 7373 2048 6f73 7455 6e6b 6e6f  .class HostUnkno
-00004b00: 776e 2853 7472 6561 6d45 7272 6f72 293a  wn(StreamError):
-00004b10: 0a20 2020 2070 6173 730a 0a63 6c61 7373  .    pass..class
-00004b20: 2049 6d70 726f 7065 7241 6464 7265 7373   ImproperAddress
-00004b30: 696e 6728 5374 7265 616d 4572 726f 7229  ing(StreamError)
-00004b40: 3a0a 2020 2020 7061 7373 0a0a 636c 6173  :.    pass..clas
-00004b50: 7320 496e 7465 726e 616c 5365 7276 6572  s InternalServer
-00004b60: 4572 726f 7228 5374 7265 616d 4572 726f  Error(StreamErro
-00004b70: 7229 3a0a 2020 2020 7061 7373 0a0a 636c  r):.    pass..cl
-00004b80: 6173 7320 496e 7661 6c69 6446 726f 6d28  ass InvalidFrom(
-00004b90: 5374 7265 616d 4572 726f 7229 3a0a 2020  StreamError):.  
-00004ba0: 2020 7061 7373 0a0a 636c 6173 7320 496e    pass..class In
-00004bb0: 7661 6c69 6449 4428 5374 7265 616d 4572  validID(StreamEr
-00004bc0: 726f 7229 3a0a 2020 2020 7061 7373 0a0a  ror):.    pass..
-00004bd0: 636c 6173 7320 496e 7661 6c69 644e 616d  class InvalidNam
-00004be0: 6573 7061 6365 2853 7472 6561 6d45 7272  espace(StreamErr
-00004bf0: 6f72 293a 0a20 2020 2070 6173 730a 0a63  or):.    pass..c
-00004c00: 6c61 7373 2049 6e76 616c 6964 584d 4c28  lass InvalidXML(
-00004c10: 5374 7265 616d 4572 726f 7229 3a0a 2020  StreamError):.  
-00004c20: 2020 7061 7373 0a0a 636c 6173 7320 4e6f    pass..class No
-00004c30: 7441 7574 686f 7269 7a65 6428 5374 7265  tAuthorized(Stre
-00004c40: 616d 4572 726f 7229 3a0a 2020 2020 7061  amError):.    pa
-00004c50: 7373 0a0a 636c 6173 7320 506f 6c69 6379  ss..class Policy
-00004c60: 5669 6f6c 6174 696f 6e28 5374 7265 616d  Violation(Stream
-00004c70: 4572 726f 7229 3a0a 2020 2020 7061 7373  Error):.    pass
-00004c80: 0a0a 636c 6173 7320 5265 6d6f 7465 436f  ..class RemoteCo
-00004c90: 6e6e 6563 7469 6f6e 4661 696c 6564 2853  nnectionFailed(S
-00004ca0: 7472 6561 6d45 7272 6f72 293a 0a20 2020  treamError):.   
-00004cb0: 2070 6173 730a 0a63 6c61 7373 2052 6573   pass..class Res
-00004cc0: 6f75 7263 6543 6f6e 7374 7261 696e 7428  ourceConstraint(
-00004cd0: 5374 7265 616d 4572 726f 7229 3a0a 2020  StreamError):.  
-00004ce0: 2020 7061 7373 0a0a 636c 6173 7320 5265    pass..class Re
-00004cf0: 7374 7269 6374 6564 584d 4c28 5374 7265  strictedXML(Stre
-00004d00: 616d 4572 726f 7229 3a0a 2020 2020 7061  amError):.    pa
-00004d10: 7373 0a0a 636c 6173 7320 5365 654f 7468  ss..class SeeOth
-00004d20: 6572 486f 7374 2853 7472 6561 6d45 7272  erHost(StreamErr
-00004d30: 6f72 293a 0a20 2020 2070 6173 730a 0a63  or):.    pass..c
-00004d40: 6c61 7373 2053 7973 7465 6d53 6875 7464  lass SystemShutd
-00004d50: 6f77 6e28 5374 7265 616d 4572 726f 7229  own(StreamError)
-00004d60: 3a0a 2020 2020 7061 7373 0a0a 636c 6173  :.    pass..clas
-00004d70: 7320 556e 6465 6669 6e65 6443 6f6e 6469  s UndefinedCondi
-00004d80: 7469 6f6e 2853 7472 6561 6d45 7272 6f72  tion(StreamError
-00004d90: 293a 0a20 2020 2070 6173 730a 0a63 6c61  ):.    pass..cla
-00004da0: 7373 2055 6e73 7570 706f 7274 6564 456e  ss UnsupportedEn
-00004db0: 636f 6469 6e67 2853 7472 6561 6d45 7272  coding(StreamErr
-00004dc0: 6f72 293a 0a20 2020 2070 6173 730a 0a63  or):.    pass..c
-00004dd0: 6c61 7373 2055 6e73 7570 706f 7274 6564  lass Unsupported
-00004de0: 5374 616e 7a61 5479 7065 2853 7472 6561  StanzaType(Strea
-00004df0: 6d45 7272 6f72 293a 0a20 2020 2070 6173  mError):.    pas
-00004e00: 730a 0a63 6c61 7373 2055 6e73 7570 706f  s..class Unsuppo
-00004e10: 7274 6564 5665 7273 696f 6e28 5374 7265  rtedVersion(Stre
-00004e20: 616d 4572 726f 7229 3a0a 2020 2020 7061  amError):.    pa
-00004e30: 7373 0a0a 636c 6173 7320 584d 4c4e 6f74  ss..class XMLNot
-00004e40: 5765 6c6c 466f 726d 6564 2853 7472 6561  WellFormed(Strea
-00004e50: 6d45 7272 6f72 293a 0a20 2020 2070 6173  mError):.    pas
-00004e60: 730a 0a63 6c61 7373 2049 6e76 616c 6964  s..class Invalid
-00004e70: 5374 616e 7a61 2845 7863 6570 7469 6f6e  Stanza(Exception
-00004e80: 293a 0a20 2020 2070 6173 730a 0a63 6c61  ):.    pass..cla
-00004e90: 7373 2049 6e76 616c 6964 4a69 6428 4578  ss InvalidJid(Ex
-00004ea0: 6365 7074 696f 6e29 3a0a 2020 2020 7061  ception):.    pa
-00004eb0: 7373 0a0a 636c 6173 7320 4c6f 6361 6c70  ss..class Localp
-00004ec0: 6172 7442 7974 654c 696d 6974 2849 6e76  artByteLimit(Inv
-00004ed0: 616c 6964 4a69 6429 3a0a 2020 2020 6465  alidJid):.    de
-00004ee0: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-00004ef0: 3a0a 2020 2020 2020 2020 496e 7661 6c69  :.        Invali
-00004f00: 644a 6964 2e5f 5f69 6e69 745f 5f28 7365  dJid.__init__(se
-00004f10: 6c66 2c20 274c 6f63 616c 7061 7274 206d  lf, 'Localpart m
-00004f20: 7573 7420 6265 2062 6574 7765 656e 2031  ust be between 1
-00004f30: 2061 6e64 2031 3032 3320 6279 7465 7327   and 1023 bytes'
-00004f40: 290a 0a63 6c61 7373 204c 6f63 616c 7061  )..class Localpa
-00004f50: 7274 4e6f 7441 6c6c 6f77 6564 4368 6172  rtNotAllowedChar
-00004f60: 2849 6e76 616c 6964 4a69 6429 3a0a 2020  (InvalidJid):.  
-00004f70: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00004f80: 656c 6629 3a0a 2020 2020 2020 2020 496e  elf):.        In
-00004f90: 7661 6c69 644a 6964 2e5f 5f69 6e69 745f  validJid.__init_
-00004fa0: 5f28 7365 6c66 2c20 274e 6f74 2061 6c6c  _(self, 'Not all
-00004fb0: 6f77 6564 2063 6861 7261 6374 6572 2069  owed character i
-00004fc0: 6e20 6c6f 6361 6c70 6172 7427 290a 0a63  n localpart')..c
-00004fd0: 6c61 7373 2052 6573 6f75 7263 6570 6172  lass Resourcepar
-00004fe0: 7442 7974 654c 696d 6974 2849 6e76 616c  tByteLimit(Inval
-00004ff0: 6964 4a69 6429 3a0a 2020 2020 6465 6620  idJid):.    def 
-00005000: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0a  __init__(self):.
-00005010: 2020 2020 2020 2020 496e 7661 6c69 644a          InvalidJ
-00005020: 6964 2e5f 5f69 6e69 745f 5f28 7365 6c66  id.__init__(self
-00005030: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005040: 2020 2020 2020 2020 2020 2020 2020 2752                'R
-00005050: 6573 6f75 7263 6570 6172 7420 6d75 7374  esourcepart must
-00005060: 2062 6520 6265 7477 6565 6e20 3120 616e   be between 1 an
-00005070: 6420 3130 3233 2062 7974 6573 2729 0a0a  d 1023 bytes')..
-00005080: 636c 6173 7320 5265 736f 7572 6365 7061  class Resourcepa
-00005090: 7274 4e6f 7441 6c6c 6f77 6564 4368 6172  rtNotAllowedChar
-000050a0: 2849 6e76 616c 6964 4a69 6429 3a0a 2020  (InvalidJid):.  
-000050b0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-000050c0: 656c 6629 3a0a 2020 2020 2020 2020 496e  elf):.        In
-000050d0: 7661 6c69 644a 6964 2e5f 5f69 6e69 745f  validJid.__init_
-000050e0: 5f28 7365 6c66 2c20 274e 6f74 2061 6c6c  _(self, 'Not all
-000050f0: 6f77 6564 2063 6861 7261 6374 6572 2069  owed character i
-00005100: 6e20 7265 736f 7572 6365 7061 7274 2729  n resourcepart')
-00005110: 0a0a 636c 6173 7320 446f 6d61 696e 7061  ..class Domainpa
-00005120: 7274 4279 7465 4c69 6d69 7428 496e 7661  rtByteLimit(Inva
-00005130: 6c69 644a 6964 293a 0a20 2020 2064 6566  lidJid):.    def
-00005140: 205f 5f69 6e69 745f 5f28 7365 6c66 293a   __init__(self):
-00005150: 0a20 2020 2020 2020 2049 6e76 616c 6964  .        Invalid
-00005160: 4a69 642e 5f5f 696e 6974 5f5f 2873 656c  Jid.__init__(sel
-00005170: 662c 2027 446f 6d61 696e 7061 7274 206d  f, 'Domainpart m
-00005180: 7573 7420 6265 2062 6574 7765 656e 2031  ust be between 1
-00005190: 2061 6e64 2031 3032 3320 6279 7465 7327   and 1023 bytes'
-000051a0: 290a 0a63 6c61 7373 2044 6f6d 6169 6e70  )..class Domainp
-000051b0: 6172 744e 6f74 416c 6c6f 7765 6443 6861  artNotAllowedCha
-000051c0: 7228 496e 7661 6c69 644a 6964 293a 0a20  r(InvalidJid):. 
-000051d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000051e0: 7365 6c66 293a 0a20 2020 2020 2020 2049  self):.        I
-000051f0: 6e76 616c 6964 4a69 642e 5f5f 696e 6974  nvalidJid.__init
-00005200: 5f5f 2873 656c 662c 2027 4e6f 7420 616c  __(self, 'Not al
-00005210: 6c6f 7765 6420 6368 6172 6163 7465 7220  lowed character 
-00005220: 696e 2064 6f6d 6169 6e70 6172 7427 290a  in domainpart').
-00005230: 0a63 6c61 7373 2053 7461 6e7a 614d 616c  .class StanzaMal
-00005240: 666f 726d 6564 2845 7863 6570 7469 6f6e  formed(Exception
-00005250: 293a 0a20 2020 2070 6173 730a 0a63 6c61  ):.    pass..cla
-00005260: 7373 2044 6973 636f 496e 666f 4d61 6c66  ss DiscoInfoMalf
-00005270: 6f72 6d65 6428 4578 6365 7074 696f 6e29  ormed(Exception)
-00005280: 3a0a 2020 2020 7061 7373 0a0a 7374 7265  :.    pass..stre
-00005290: 616d 5f65 7863 6570 7469 6f6e 7320 3d20  am_exceptions = 
-000052a0: 7b27 6261 642d 666f 726d 6174 273a 2042  {'bad-format': B
-000052b0: 6164 466f 726d 6174 2c0a 2020 2020 2020  adFormat,.      
-000052c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000052d0: 6261 642d 6e61 6d65 7370 6163 652d 7072  bad-namespace-pr
-000052e0: 6566 6978 273a 2042 6164 4e61 6d65 7370  efix': BadNamesp
-000052f0: 6163 6550 7265 6669 782c 0a20 2020 2020  acePrefix,.     
-00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005310: 2763 6f6e 666c 6963 7427 3a20 436f 6e66  'conflict': Conf
-00005320: 6c69 6374 2c0a 2020 2020 2020 2020 2020  lict,.          
-00005330: 2020 2020 2020 2020 2020 2027 636f 6e6e             'conn
-00005340: 6563 7469 6f6e 2d74 696d 656f 7574 273a  ection-timeout':
-00005350: 2043 6f6e 6e65 6374 696f 6e54 696d 656f   ConnectionTimeo
-00005360: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
-00005370: 2020 2020 2020 2020 2027 686f 7374 2d67           'host-g
-00005380: 6f6e 6527 3a20 486f 7374 476f 6e65 2c0a  one': HostGone,.
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2020 2020 2027 686f 7374 2d75 6e6b 6e6f       'host-unkno
-000053b0: 776e 273a 2048 6f73 7455 6e6b 6e6f 776e  wn': HostUnknown
-000053c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000053d0: 2020 2020 2020 2027 696d 7072 6f70 6572         'improper
-000053e0: 2d61 6464 7265 7373 696e 6727 3a20 496d  -addressing': Im
-000053f0: 7072 6f70 6572 4164 6472 6573 7369 6e67  properAddressing
-00005400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005410: 2020 2020 2020 2027 696e 7465 726e 616c         'internal
-00005420: 2d73 6572 7665 722d 6572 726f 7227 3a20  -server-error': 
-00005430: 496e 7465 726e 616c 5365 7276 6572 4572  InternalServerEr
-00005440: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-00005450: 2020 2020 2020 2020 2020 2769 6e76 616c            'inval
-00005460: 6964 2d66 726f 6d27 3a20 496e 7661 6c69  id-from': Invali
-00005470: 6446 726f 6d2c 0a20 2020 2020 2020 2020  dFrom,.         
-00005480: 2020 2020 2020 2020 2020 2020 2769 6e76              'inv
-00005490: 616c 6964 2d69 6427 3a20 496e 7661 6c69  alid-id': Invali
-000054a0: 6449 442c 0a20 2020 2020 2020 2020 2020  dID,.           
-000054b0: 2020 2020 2020 2020 2020 2769 6e76 616c            'inval
-000054c0: 6964 2d6e 616d 6573 7061 6365 273a 2049  id-namespace': I
-000054d0: 6e76 616c 6964 4e61 6d65 7370 6163 652c  nvalidNamespace,
-000054e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000054f0: 2020 2020 2020 2769 6e76 616c 6964 2d78        'invalid-x
-00005500: 6d6c 273a 2049 6e76 616c 6964 584d 4c2c  ml': InvalidXML,
-00005510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005520: 2020 2020 2020 276e 6f74 2d61 7574 686f        'not-autho
-00005530: 7269 7a65 6427 3a20 4e6f 7441 7574 686f  rized': NotAutho
-00005540: 7269 7a65 642c 0a20 2020 2020 2020 2020  rized,.         
-00005550: 2020 2020 2020 2020 2020 2020 2770 6f6c              'pol
-00005560: 6963 792d 7669 6f6c 6174 696f 6e27 3a20  icy-violation': 
-00005570: 506f 6c69 6379 5669 6f6c 6174 696f 6e2c  PolicyViolation,
-00005580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005590: 2020 2020 2020 2772 656d 6f74 652d 636f        'remote-co
-000055a0: 6e6e 6563 7469 6f6e 2d66 6169 6c65 6427  nnection-failed'
-000055b0: 3a20 5265 6d6f 7465 436f 6e6e 6563 7469  : RemoteConnecti
-000055c0: 6f6e 4661 696c 6564 2c0a 2020 2020 2020  onFailed,.      
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000055e0: 7265 736f 7572 6365 2d63 6f6e 7374 7261  resource-constra
-000055f0: 696e 7427 3a20 5265 736f 7572 6365 436f  int': ResourceCo
-00005600: 6e73 7472 6169 6e74 2c0a 2020 2020 2020  nstraint,.      
-00005610: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005620: 7265 7374 7269 6374 6564 2d78 6d6c 273a  restricted-xml':
-00005630: 2052 6573 7472 6963 7465 6458 4d4c 2c0a   RestrictedXML,.
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005650: 2020 2020 2027 7365 652d 6f74 6865 722d       'see-other-
-00005660: 686f 7374 273a 2053 6565 4f74 6865 7248  host': SeeOtherH
-00005670: 6f73 742c 0a20 2020 2020 2020 2020 2020  ost,.           
-00005680: 2020 2020 2020 2020 2020 2773 7973 7465            'syste
-00005690: 6d2d 7368 7574 646f 776e 273a 2053 7973  m-shutdown': Sys
-000056a0: 7465 6d53 6875 7464 6f77 6e2c 0a20 2020  temShutdown,.   
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2775 6e64 6566 696e 6564 2d63 6f6e    'undefined-con
-000056d0: 6469 7469 6f6e 273a 2055 6e64 6566 696e  dition': Undefin
-000056e0: 6564 436f 6e64 6974 696f 6e2c 0a20 2020  edCondition,.   
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2775 6e73 7570 706f 7274 6564 2d65    'unsupported-e
-00005710: 6e63 6f64 696e 6727 3a20 556e 7375 7070  ncoding': Unsupp
-00005720: 6f72 7465 6445 6e63 6f64 696e 672c 0a20  ortedEncoding,. 
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2775 6e73 7570 706f 7274 6564      'unsupported
-00005750: 2d73 7461 6e7a 612d 7479 7065 273a 2055  -stanza-type': U
-00005760: 6e73 7570 706f 7274 6564 5374 616e 7a61  nsupportedStanza
-00005770: 5479 7065 2c0a 2020 2020 2020 2020 2020  Type,.          
-00005780: 2020 2020 2020 2020 2020 2027 756e 7375             'unsu
-00005790: 7070 6f72 7465 642d 7665 7273 696f 6e27  pported-version'
-000057a0: 3a20 556e 7375 7070 6f72 7465 6456 6572  : UnsupportedVer
-000057b0: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
-000057c0: 2020 2020 2020 2020 2020 2027 786d 6c2d             'xml-
-000057d0: 6e6f 742d 7765 6c6c 2d66 6f72 6d65 6427  not-well-formed'
-000057e0: 3a20 584d 4c4e 6f74 5765 6c6c 466f 726d  : XMLNotWellForm
-000057f0: 6564 7d0a 0a0a 6465 6620 6465 7072 6563  ed}...def deprec
-00005800: 6174 696f 6e5f 7761 726e 696e 6728 6d65  ation_warning(me
-00005810: 7373 6167 6529 3a0a 2020 2020 7761 726e  ssage):.    warn
-00005820: 696e 6773 2e77 6172 6e28 6d65 7373 6167  ings.warn(messag
-00005830: 652c 2044 6570 7265 6361 7469 6f6e 5761  e, DeprecationWa
-00005840: 726e 696e 6729 0a0a 0a40 6675 6e63 746f  rning)...@functo
-00005850: 6f6c 732e 6c72 755f 6361 6368 6528 6d61  ols.lru_cache(ma
-00005860: 7873 697a 653d 4e6f 6e65 290a 6465 6620  xsize=None).def 
-00005870: 7661 6c69 6461 7465 5f6c 6f63 616c 7061  validate_localpa
-00005880: 7274 286c 6f63 616c 7061 7274 3a20 7374  rt(localpart: st
-00005890: 7229 202d 3e20 7374 723a 0a20 2020 2069  r) -> str:.    i
-000058a0: 6620 6e6f 7420 6c6f 6361 6c70 6172 7420  f not localpart 
-000058b0: 6f72 206c 656e 286c 6f63 616c 7061 7274  or len(localpart
-000058c0: 2e65 6e63 6f64 6528 2929 203e 2031 3032  .encode()) > 102
-000058d0: 333a 0a20 2020 2020 2020 2072 6169 7365  3:.        raise
-000058e0: 204c 6f63 616c 7061 7274 4279 7465 4c69   LocalpartByteLi
-000058f0: 6d69 740a 0a20 2020 2069 6620 6f73 2e65  mit..    if os.e
-00005900: 6e76 6972 6f6e 2e67 6574 2827 4e42 584d  nviron.get('NBXM
-00005910: 5050 5f45 4e46 4f52 4345 5f50 5245 4349  PP_ENFORCE_PRECI
-00005920: 5327 2920 6973 204e 6f6e 653a 0a20 2020  S') is None:.   
-00005930: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00005940: 2020 2020 2020 7265 7475 726e 206e 6f64        return nod
-00005950: 6570 7265 7028 6c6f 6361 6c70 6172 7429  eprep(localpart)
-00005960: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00005970: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
-00005980: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00005990: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000059a0: 726e 2065 6e66 6f72 6365 5f70 7265 6369  rn enforce_preci
-000059b0: 735f 7573 6572 6e61 6d65 286c 6f63 616c  s_username(local
-000059c0: 7061 7274 290a 2020 2020 2020 2020 2020  part).          
-000059d0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000059e0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000059f0: 2020 2020 7261 6973 6520 4c6f 6361 6c70      raise Localp
-00005a00: 6172 744e 6f74 416c 6c6f 7765 6443 6861  artNotAllowedCha
-00005a10: 720a 0a20 2020 2074 7279 3a0a 2020 2020  r..    try:.    
-00005a20: 2020 2020 7265 7475 726e 2065 6e66 6f72      return enfor
-00005a30: 6365 5f70 7265 6369 735f 7573 6572 6e61  ce_precis_userna
-00005a40: 6d65 286c 6f63 616c 7061 7274 290a 2020  me(localpart).  
-00005a50: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00005a60: 6f6e 3a0a 2020 2020 2020 2020 7261 6973  on:.        rais
-00005a70: 6520 4c6f 6361 6c70 6172 744e 6f74 416c  e LocalpartNotAl
-00005a80: 6c6f 7765 6443 6861 720a 0a0a 4066 756e  lowedChar...@fun
-00005a90: 6374 6f6f 6c73 2e6c 7275 5f63 6163 6865  ctools.lru_cache
-00005aa0: 286d 6178 7369 7a65 3d4e 6f6e 6529 0a64  (maxsize=None).d
-00005ab0: 6566 2076 616c 6964 6174 655f 7265 736f  ef validate_reso
-00005ac0: 7572 6365 7061 7274 2872 6573 6f75 7263  urcepart(resourc
-00005ad0: 6570 6172 743a 2073 7472 2920 2d3e 2073  epart: str) -> s
-00005ae0: 7472 3a0a 2020 2020 6966 206e 6f74 2072  tr:.    if not r
-00005af0: 6573 6f75 7263 6570 6172 7420 6f72 206c  esourcepart or l
-00005b00: 656e 2872 6573 6f75 7263 6570 6172 742e  en(resourcepart.
-00005b10: 656e 636f 6465 2829 2920 3e20 3130 3233  encode()) > 1023
-00005b20: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00005b30: 5265 736f 7572 6365 7061 7274 4279 7465  ResourcepartByte
-00005b40: 4c69 6d69 740a 0a20 2020 2069 6620 6f73  Limit..    if os
-00005b50: 2e65 6e76 6972 6f6e 2e67 6574 2827 4e42  .environ.get('NB
-00005b60: 584d 5050 5f45 4e46 4f52 4345 5f50 5245  XMPP_ENFORCE_PRE
-00005b70: 4349 5327 2920 6973 204e 6f6e 653a 0a20  CIS') is None:. 
-00005b80: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00005b90: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00005ba0: 6573 6f75 7263 6570 7265 7028 7265 736f  esourceprep(reso
-00005bb0: 7572 6365 7061 7274 290a 2020 2020 2020  urcepart).      
-00005bc0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00005bd0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00005be0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00005bf0: 2020 2020 2072 6574 7572 6e20 656e 666f       return enfo
-00005c00: 7263 655f 7072 6563 6973 5f6f 7061 7175  rce_precis_opaqu
-00005c10: 6528 7265 736f 7572 6365 7061 7274 290a  e(resourcepart).
-00005c20: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00005c30: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
-00005c40: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00005c50: 6973 6520 5265 736f 7572 6365 7061 7274  ise Resourcepart
-00005c60: 4e6f 7441 6c6c 6f77 6564 4368 6172 0a0a  NotAllowedChar..
-00005c70: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00005c80: 2072 6574 7572 6e20 656e 666f 7263 655f   return enforce_
-00005c90: 7072 6563 6973 5f6f 7061 7175 6528 7265  precis_opaque(re
-00005ca0: 736f 7572 6365 7061 7274 290a 2020 2020  sourcepart).    
-00005cb0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00005cc0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00005cd0: 5265 736f 7572 6365 7061 7274 4e6f 7441  ResourcepartNotA
-00005ce0: 6c6c 6f77 6564 4368 6172 0a0a 0a40 6675  llowedChar...@fu
-00005cf0: 6e63 746f 6f6c 732e 6c72 755f 6361 6368  nctools.lru_cach
-00005d00: 6528 6d61 7873 697a 653d 4e6f 6e65 290a  e(maxsize=None).
-00005d10: 6465 6620 7661 6c69 6461 7465 5f64 6f6d  def validate_dom
-00005d20: 6169 6e70 6172 7428 646f 6d61 696e 7061  ainpart(domainpa
-00005d30: 7274 3a20 7374 7229 202d 3e20 7374 723a  rt: str) -> str:
-00005d40: 0a20 2020 2069 6620 6e6f 7420 646f 6d61  .    if not doma
-00005d50: 696e 7061 7274 3a0a 2020 2020 2020 2020  inpart:.        
-00005d60: 7261 6973 6520 446f 6d61 696e 7061 7274  raise Domainpart
-00005d70: 4279 7465 4c69 6d69 740a 0a20 2020 2069  ByteLimit..    i
-00005d80: 705f 6164 6472 6573 7320 3d20 646f 6d61  p_address = doma
-00005d90: 696e 7061 7274 2e73 7472 6970 2827 5b5d  inpart.strip('[]
-00005da0: 2729 0a20 2020 2069 6620 474c 6962 2e68  ').    if GLib.h
-00005db0: 6f73 746e 616d 655f 6973 5f69 705f 6164  ostname_is_ip_ad
-00005dc0: 6472 6573 7328 6970 5f61 6464 7265 7373  dress(ip_address
-00005dd0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00005de0: 6e20 6970 5f61 6464 7265 7373 0a0a 2020  n ip_address..  
-00005df0: 2020 6c65 6e67 7468 203d 206c 656e 2864    length = len(d
-00005e00: 6f6d 6169 6e70 6172 742e 656e 636f 6465  omainpart.encode
-00005e10: 2829 290a 2020 2020 6966 206c 656e 6774  ()).    if lengt
-00005e20: 6820 3d3d 2030 206f 7220 6c65 6e67 7468  h == 0 or length
-00005e30: 203e 2031 3032 333a 0a20 2020 2020 2020   > 1023:.       
-00005e40: 2072 6169 7365 2044 6f6d 6169 6e70 6172   raise Domainpar
-00005e50: 7442 7974 654c 696d 6974 0a0a 2020 2020  tByteLimit..    
-00005e60: 6966 2064 6f6d 6169 6e70 6172 742e 656e  if domainpart.en
-00005e70: 6473 7769 7468 2827 2e27 293a 2020 2320  dswith('.'):  # 
-00005e80: 5246 4337 3632 322c 2033 2e32 0a20 2020  RFC7622, 3.2.   
-00005e90: 2020 2020 2064 6f6d 6169 6e70 6172 7420       domainpart 
-00005ea0: 3d20 646f 6d61 696e 7061 7274 5b3a 2d31  = domainpart[:-1
-00005eb0: 5d0a 0a20 2020 2074 7279 3a0a 2020 2020  ]..    try:.    
-00005ec0: 2020 2020 646f 6d61 696e 7061 7274 203d      domainpart =
-00005ed0: 2069 646e 6132 3030 385f 7072 6570 2864   idna2008_prep(d
-00005ee0: 6f6d 6169 6e70 6172 7429 0a20 2020 2065  omainpart).    e
-00005ef0: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
-00005f00: 0a20 2020 2020 2020 2072 6169 7365 2044  .        raise D
-00005f10: 6f6d 6169 6e70 6172 744e 6f74 416c 6c6f  omainpartNotAllo
-00005f20: 7765 6443 6861 720a 0a20 2020 2072 6574  wedChar..    ret
-00005f30: 7572 6e20 646f 6d61 696e 7061 7274 0a0a  urn domainpart..
-00005f40: 0a40 6675 6e63 746f 6f6c 732e 6c72 755f  .@functools.lru_
-00005f50: 6361 6368 6528 6d61 7873 697a 653d 4e6f  cache(maxsize=No
-00005f60: 6e65 290a 6465 6620 6964 6e61 3230 3038  ne).def idna2008
-00005f70: 5f70 7265 7028 646f 6d61 696e 3a20 7374  _prep(domain: st
-00005f80: 722c 2074 6f5f 6173 6369 693a 2062 6f6f  r, to_ascii: boo
-00005f90: 6c20 3d20 4661 6c73 6529 202d 3e20 7374  l = False) -> st
-00005fa0: 723a 0a20 2020 2027 2727 0a20 2020 2050  r:.    '''.    P
-00005fb0: 7265 7061 7265 2077 6974 6820 5554 5334  repare with UTS4
-00005fc0: 3620 6361 7365 206d 6170 7069 6e67 2074  6 case mapping t
-00005fd0: 6f20 7374 6179 2063 6f6d 7061 7469 6265  o stay compatibe
-00005fe0: 6c20 7769 7468 2074 6865 2049 444e 4132  l with the IDNA2
-00005ff0: 3030 330a 2020 2020 6d61 7070 696e 672e  003.    mapping.
-00006000: 2046 7572 7468 6572 2074 7279 2074 6f20   Further try to 
-00006010: 656e 636f 6465 2074 6865 2064 6f6d 6169  encode the domai
-00006020: 6e20 746f 2063 6174 6368 2069 6c6c 6567  n to catch illeg
-00006030: 616c 2064 6f6d 6169 6e73 2e0a 2020 2020  al domains..    
-00006040: 4f6e 6c79 2072 6574 7572 6e20 7468 6520  Only return the 
-00006050: 6361 7365 206d 6170 7065 6420 646f 6d61  case mapped doma
-00006060: 696e 2062 6563 6175 7365 206f 6e20 7468  in because on th
-00006070: 6520 584d 5050 2077 6972 652c 5554 4638  e XMPP wire,UTF8
-00006080: 2064 6f6d 6169 6e73 0a20 2020 2061 7265   domains.    are
-00006090: 2066 696e 652e 0a20 2020 2027 2727 0a20   fine..    '''. 
-000060a0: 2020 2064 6f6d 6169 6e20 3d20 6964 6e61     domain = idna
-000060b0: 2e75 7473 3436 5f72 656d 6170 2864 6f6d  .uts46_remap(dom
-000060c0: 6169 6e29 0a20 2020 2065 6e63 6f64 6564  ain).    encoded
-000060d0: 5f64 6f6d 6169 6e20 3d20 6964 6e61 2e65  _domain = idna.e
-000060e0: 6e63 6f64 6528 646f 6d61 696e 290a 2020  ncode(domain).  
-000060f0: 2020 6966 2074 6f5f 6173 6369 693a 0a20    if to_ascii:. 
-00006100: 2020 2020 2020 2072 6574 7572 6e20 656e         return en
-00006110: 636f 6465 645f 646f 6d61 696e 2e64 6563  coded_domain.dec
-00006120: 6f64 6528 290a 2020 2020 7265 7475 726e  ode().    return
-00006130: 2064 6f6d 6169 6e0a 0a0a 4066 756e 6374   domain...@funct
-00006140: 6f6f 6c73 2e6c 7275 5f63 6163 6865 286d  ools.lru_cache(m
-00006150: 6178 7369 7a65 3d4e 6f6e 6529 0a64 6566  axsize=None).def
-00006160: 2065 7363 6170 655f 6c6f 6361 6c70 6172   escape_localpar
-00006170: 7428 6c6f 6361 6c70 6172 743a 2073 7472  t(localpart: str
-00006180: 2920 2d3e 2073 7472 3a0a 2020 2020 2320  ) -> str:.    # 
-00006190: 6874 7470 733a 2f2f 786d 7070 2e6f 7267  https://xmpp.org
-000061a0: 2f65 7874 656e 7369 6f6e 732f 7865 702d  /extensions/xep-
-000061b0: 3031 3036 2e68 746d 6c23 6269 7a72 756c  0106.html#bizrul
-000061c0: 6573 2d61 6c67 6f72 6974 686d 0a20 2020  es-algorithm.   
-000061d0: 2023 0a20 2020 2023 2049 6620 7468 6572   #.    # If ther
-000061e0: 6520 6172 6520 616e 7920 696e 7374 616e  e are any instan
-000061f0: 6365 7320 6f66 2063 6861 7261 6374 6572  ces of character
-00006200: 2073 6571 7565 6e63 6573 2074 6861 7420   sequences that 
-00006210: 636f 7272 6573 706f 6e64 0a20 2020 2023  correspond.    #
-00006220: 2074 6f20 6573 6361 7069 6e67 7320 6f66   to escapings of
-00006230: 2074 6865 2064 6973 616c 6c6f 7765 6420   the disallowed 
-00006240: 6368 6172 6163 7465 7273 0a20 2020 2023  characters.    #
-00006250: 2028 652e 672e 2c20 7468 6520 6368 6172   (e.g., the char
-00006260: 6163 7465 7220 7365 7175 656e 6365 2022  acter sequence "
-00006270: 5c32 3722 2920 6f72 2074 6865 2065 7363  \27") or the esc
-00006280: 6170 696e 6720 6368 6172 6163 7465 720a  aping character.
-00006290: 2020 2020 2320 2869 2e65 2e2c 2074 6865      # (i.e., the
-000062a0: 2063 6861 7261 6374 6572 2073 6571 7565   character seque
-000062b0: 6e63 6520 225c 3563 2229 2069 6e20 7468  nce "\5c") in th
-000062c0: 6520 736f 7572 6365 2061 6464 7265 7373  e source address
-000062d0: 2c0a 2020 2020 2320 7468 6520 6c65 6164  ,.    # the lead
-000062e0: 696e 6720 6261 636b 736c 6173 6820 6368  ing backslash ch
-000062f0: 6172 6163 7465 7220 4d55 5354 2062 6520  aracter MUST be 
-00006300: 6573 6361 7065 6420 746f 2074 6865 2063  escaped to the c
-00006310: 6861 7261 6374 6572 0a20 2020 2023 2073  haracter.    # s
-00006320: 6571 7565 6e63 6520 225c 3563 220a 0a20  equence "\5c".. 
-00006330: 2020 2066 6f72 2063 6861 7220 696e 2027     for char in '
-00006340: 5c5c 2720 2b20 5f6c 6f63 616c 7061 7274  \\' + _localpart
-00006350: 5f65 7363 6170 655f 6368 6172 733a 0a20  _escape_chars:. 
-00006360: 2020 2020 2020 2073 6571 203d 2022 5c5c         seq = "\\
-00006370: 7b3a 3032 787d 222e 666f 726d 6174 286f  {:02x}".format(o
-00006380: 7264 2863 6861 7229 290a 2020 2020 2020  rd(char)).      
-00006390: 2020 6c6f 6361 6c70 6172 7420 3d20 6c6f    localpart = lo
-000063a0: 6361 6c70 6172 742e 7265 706c 6163 6528  calpart.replace(
-000063b0: 7365 712c 2022 5c5c 3563 7b3a 3032 787d  seq, "\\5c{:02x}
-000063c0: 222e 666f 726d 6174 286f 7264 2863 6861  ".format(ord(cha
-000063d0: 7229 2929 0a0a 2020 2020 2320 4573 6361  r)))..    # Esca
-000063e0: 7065 2061 6c6c 206f 7468 6572 2063 6861  pe all other cha
-000063f0: 7273 0a20 2020 2066 6f72 2063 6861 7220  rs.    for char 
-00006400: 696e 205f 6c6f 6361 6c70 6172 745f 6573  in _localpart_es
-00006410: 6361 7065 5f63 6861 7273 3a0a 2020 2020  cape_chars:.    
-00006420: 2020 2020 6c6f 6361 6c70 6172 7420 3d20      localpart = 
-00006430: 6c6f 6361 6c70 6172 742e 7265 706c 6163  localpart.replac
-00006440: 6528 6368 6172 2c20 225c 5c7b 3a30 3278  e(char, "\\{:02x
-00006450: 7d22 2e66 6f72 6d61 7428 6f72 6428 6368  }".format(ord(ch
-00006460: 6172 2929 290a 0a20 2020 2072 6574 7572  ar)))..    retur
-00006470: 6e20 6c6f 6361 6c70 6172 740a 0a0a 4066  n localpart...@f
-00006480: 756e 6374 6f6f 6c73 2e6c 7275 5f63 6163  unctools.lru_cac
-00006490: 6865 286d 6178 7369 7a65 3d4e 6f6e 6529  he(maxsize=None)
-000064a0: 0a64 6566 2075 6e65 7363 6170 655f 6c6f  .def unescape_lo
-000064b0: 6361 6c70 6172 7428 6c6f 6361 6c70 6172  calpart(localpar
-000064c0: 743a 2073 7472 2920 2d3e 2073 7472 3a0a  t: str) -> str:.
-000064d0: 2020 2020 6966 206c 6f63 616c 7061 7274      if localpart
-000064e0: 2e73 7461 7274 7377 6974 6828 275c 5c32  .startswith('\\2
-000064f0: 3027 2920 6f72 206c 6f63 616c 7061 7274  0') or localpart
-00006500: 2e65 6e64 7377 6974 6828 275c 5c32 3027  .endswith('\\20'
-00006510: 293a 0a20 2020 2020 2020 2023 2045 7363  ):.        # Esc
-00006520: 6170 6564 204a 4944 7320 6172 6520 6e6f  aped JIDs are no
-00006530: 7420 616c 6c6f 7765 6420 746f 2073 7461  t allowed to sta
-00006540: 7274 206f 7220 656e 6420 7769 7468 205c  rt or end with \
-00006550: 3230 0a20 2020 2020 2020 2023 2073 6f20  20.        # so 
-00006560: 7468 6973 206c 6f63 616c 7061 7274 206d  this localpart m
-00006570: 7573 7420 6265 2061 6c72 6561 6479 2075  ust be already u
-00006580: 6e65 7363 6170 6564 0a20 2020 2020 2020  nescaped.       
-00006590: 2072 6574 7572 6e20 6c6f 6361 6c70 6172   return localpar
-000065a0: 740a 0a20 2020 2066 6f72 2063 6861 7220  t..    for char 
-000065b0: 696e 205f 6c6f 6361 6c70 6172 745f 6573  in _localpart_es
-000065c0: 6361 7065 5f63 6861 7273 3a0a 2020 2020  cape_chars:.    
-000065d0: 2020 2020 7365 7120 3d20 225c 5c7b 3a30      seq = "\\{:0
-000065e0: 3278 7d22 2e66 6f72 6d61 7428 6f72 6428  2x}".format(ord(
-000065f0: 6368 6172 2929 0a20 2020 2020 2020 206c  char)).        l
-00006600: 6f63 616c 7061 7274 203d 206c 6f63 616c  ocalpart = local
-00006610: 7061 7274 2e72 6570 6c61 6365 2873 6571  part.replace(seq
-00006620: 2c20 6368 6172 290a 0a20 2020 2066 6f72  , char)..    for
-00006630: 2063 6861 7220 696e 205f 6c6f 6361 6c70   char in _localp
-00006640: 6172 745f 6573 6361 7065 5f63 6861 7273  art_escape_chars
-00006650: 202b 2022 5c5c 223a 0a20 2020 2020 2020   + "\\":.       
-00006660: 2073 6571 203d 2022 5c5c 3563 7b3a 3032   seq = "\\5c{:02
-00006670: 787d 222e 666f 726d 6174 286f 7264 2863  x}".format(ord(c
-00006680: 6861 7229 290a 2020 2020 2020 2020 6c6f  har)).        lo
-00006690: 6361 6c70 6172 7420 3d20 6c6f 6361 6c70  calpart = localp
-000066a0: 6172 742e 7265 706c 6163 6528 7365 712c  art.replace(seq,
-000066b0: 2022 5c5c 7b3a 3032 787d 222e 666f 726d   "\\{:02x}".form
-000066c0: 6174 286f 7264 2863 6861 7229 2929 0a0a  at(ord(char)))..
-000066d0: 2020 2020 7265 7475 726e 206c 6f63 616c      return local
-000066e0: 7061 7274 0a0a 0a40 6461 7461 636c 6173  part...@dataclas
-000066f0: 7328 6672 6f7a 656e 3d54 7275 6529 0a63  s(frozen=True).c
-00006700: 6c61 7373 204a 4944 3a0a 2020 2020 6c6f  lass JID:.    lo
-00006710: 6361 6c70 6172 743a 204f 7074 696f 6e61  calpart: Optiona
-00006720: 6c5b 7374 725d 203d 204e 6f6e 650a 2020  l[str] = None.  
-00006730: 2020 646f 6d61 696e 3a20 4f70 7469 6f6e    domain: Option
-00006740: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
-00006750: 2020 2072 6573 6f75 7263 653a 204f 7074     resource: Opt
-00006760: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00006770: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
-00006780: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
-00006790: 2020 2020 2020 2020 2020 206c 6f63 616c             local
-000067a0: 7061 7274 3a20 4f70 7469 6f6e 616c 5b73  part: Optional[s
-000067b0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-000067c0: 2020 2020 2020 2020 2020 2020 2064 6f6d               dom
-000067d0: 6169 6e3a 204f 7074 696f 6e61 6c5b 7374  ain: Optional[st
-000067e0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-000067f0: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-00006800: 7572 6365 3a20 4f70 7469 6f6e 616c 5b73  urce: Optional[s
-00006810: 7472 5d20 3d20 4e6f 6e65 293a 0a0a 2020  tr] = None):..  
-00006820: 2020 2020 2020 6966 206c 6f63 616c 7061        if localpa
-00006830: 7274 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rt is not None:.
-00006840: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00006850: 6c70 6172 7420 3d20 7661 6c69 6461 7465  lpart = validate
-00006860: 5f6c 6f63 616c 7061 7274 286c 6f63 616c  _localpart(local
-00006870: 7061 7274 290a 2020 2020 2020 2020 2020  part).          
-00006880: 2020 6f62 6a65 6374 2e5f 5f73 6574 6174    object.__setat
-00006890: 7472 5f5f 2873 656c 662c 2022 6c6f 6361  tr__(self, "loca
-000068a0: 6c70 6172 7422 2c20 6c6f 6361 6c70 6172  lpart", localpar
-000068b0: 7429 0a0a 2020 2020 2020 2020 646f 6d61  t)..        doma
-000068c0: 696e 203d 2076 616c 6964 6174 655f 646f  in = validate_do
-000068d0: 6d61 696e 7061 7274 2864 6f6d 6169 6e29  mainpart(domain)
-000068e0: 0a20 2020 2020 2020 206f 626a 6563 742e  .        object.
-000068f0: 5f5f 7365 7461 7474 725f 5f28 7365 6c66  __setattr__(self
-00006900: 2c20 2264 6f6d 6169 6e22 2c20 646f 6d61  , "domain", doma
-00006910: 696e 290a 0a20 2020 2020 2020 2069 6620  in)..        if 
-00006920: 7265 736f 7572 6365 2069 7320 6e6f 7420  resource is not 
-00006930: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006940: 2020 7265 736f 7572 6365 203d 2076 616c    resource = val
-00006950: 6964 6174 655f 7265 736f 7572 6365 7061  idate_resourcepa
-00006960: 7274 2872 6573 6f75 7263 6529 0a20 2020  rt(resource).   
-00006970: 2020 2020 2020 2020 206f 626a 6563 742e           object.
-00006980: 5f5f 7365 7461 7474 725f 5f28 7365 6c66  __setattr__(self
-00006990: 2c20 2272 6573 6f75 7263 6522 2c20 7265  , "resource", re
-000069a0: 736f 7572 6365 290a 0a20 2020 2040 636c  source)..    @cl
-000069b0: 6173 736d 6574 686f 640a 2020 2020 4066  assmethod.    @f
-000069c0: 756e 6374 6f6f 6c73 2e6c 7275 5f63 6163  unctools.lru_cac
-000069d0: 6865 286d 6178 7369 7a65 3d4e 6f6e 6529  he(maxsize=None)
-000069e0: 0a20 2020 2064 6566 2066 726f 6d5f 7374  .    def from_st
-000069f0: 7269 6e67 2863 6c73 2c20 6a69 645f 7374  ring(cls, jid_st
-00006a00: 7269 6e67 3a20 7374 722c 2066 6f72 6365  ring: str, force
-00006a10: 5f62 6172 653a 2062 6f6f 6c20 3d20 4661  _bare: bool = Fa
-00006a20: 6c73 6529 202d 3e20 4a49 443a 0a20 2020  lse) -> JID:.   
-00006a30: 2020 2020 2023 2068 7474 7073 3a2f 2f74       # https://t
-00006a40: 6f6f 6c73 2e69 6574 662e 6f72 672f 6874  ools.ietf.org/ht
-00006a50: 6d6c 2f72 6663 3736 3232 2373 6563 7469  ml/rfc7622#secti
-00006a60: 6f6e 2d33 2e32 0a0a 2020 2020 2020 2020  on-3.2..        
-00006a70: 2320 5265 6d6f 7665 2061 6e79 2070 6f72  # Remove any por
-00006a80: 7469 6f6e 2066 726f 6d20 7468 6520 6669  tion from the fi
-00006a90: 7273 7420 272f 2720 6368 6172 6163 7465  rst '/' characte
-00006aa0: 7220 746f 2074 6865 2065 6e64 206f 6620  r to the end of 
-00006ab0: 7468 650a 2020 2020 2020 2020 2320 7374  the.        # st
-00006ac0: 7269 6e67 2028 6966 2074 6865 7265 2069  ring (if there i
-00006ad0: 7320 6120 272f 2720 6368 6172 6163 7465  s a '/' characte
-00006ae0: 7220 7072 6573 656e 7429 2e0a 0a20 2020  r present)...   
-00006af0: 2020 2020 2023 2052 656d 6f76 6520 616e       # Remove an
-00006b00: 7920 706f 7274 696f 6e20 6672 6f6d 2074  y portion from t
-00006b10: 6865 2062 6567 696e 6e69 6e67 206f 6620  he beginning of 
-00006b20: 7468 6520 7374 7269 6e67 2074 6f20 7468  the string to th
-00006b30: 6520 6669 7273 740a 2020 2020 2020 2020  e first.        
-00006b40: 2320 2740 2720 6368 6172 6163 7465 7220  # '@' character 
-00006b50: 2869 6620 7468 6572 6520 6973 2061 6e20  (if there is an 
-00006b60: 2740 2720 6368 6172 6163 7465 7220 7072  '@' character pr
-00006b70: 6573 656e 7429 2e0a 0a20 2020 2020 2020  esent)...       
-00006b80: 2069 6620 6a69 645f 7374 7269 6e67 2e66   if jid_string.f
-00006b90: 696e 6428 272f 2729 2021 3d20 2d31 3a0a  ind('/') != -1:.
-00006ba0: 2020 2020 2020 2020 2020 2020 7265 7374              rest
-00006bb0: 2c20 7265 736f 7572 6365 7061 7274 203d  , resourcepart =
-00006bc0: 206a 6964 5f73 7472 696e 672e 7370 6c69   jid_string.spli
-00006bd0: 7428 272f 272c 2031 290a 2020 2020 2020  t('/', 1).      
-00006be0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00006bf0: 2020 2020 7265 7374 2c20 7265 736f 7572      rest, resour
-00006c00: 6365 7061 7274 203d 206a 6964 5f73 7472  cepart = jid_str
-00006c10: 696e 672c 204e 6f6e 650a 0a20 2020 2020  ing, None..     
-00006c20: 2020 2069 6620 7265 7374 2e66 696e 6428     if rest.find(
-00006c30: 2740 2729 2021 3d20 2d31 3a0a 2020 2020  '@') != -1:.    
-00006c40: 2020 2020 2020 2020 6c6f 6361 6c70 6172          localpar
-00006c50: 742c 2064 6f6d 6169 6e70 6172 7420 3d20  t, domainpart = 
-00006c60: 7265 7374 2e73 706c 6974 2827 4027 2c20  rest.split('@', 
-00006c70: 3129 0a20 2020 2020 2020 2065 6c73 653a  1).        else:
-00006c80: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-00006c90: 616c 7061 7274 2c20 646f 6d61 696e 7061  alpart, domainpa
-00006ca0: 7274 203d 204e 6f6e 652c 2072 6573 740a  rt = None, rest.
-00006cb0: 0a20 2020 2020 2020 2069 6620 666f 7263  .        if forc
-00006cc0: 655f 6261 7265 3a0a 2020 2020 2020 2020  e_bare:.        
-00006cd0: 2020 2020 6966 206c 6f63 616c 7061 7274      if localpart
-00006ce0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006cf0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006d00: 4c6f 6361 6c70 6172 7442 7974 654c 696d  LocalpartByteLim
-00006d10: 6974 0a20 2020 2020 2020 2020 2020 2072  it.            r
-00006d20: 6573 6f75 7263 6570 6172 7420 3d20 4e6f  esourcepart = No
-00006d30: 6e65 0a0a 2020 2020 2020 2020 7265 7475  ne..        retu
-00006d40: 726e 2063 6c73 286c 6f63 616c 7061 7274  rn cls(localpart
-00006d50: 3d6c 6f63 616c 7061 7274 2c0a 2020 2020  =localpart,.    
-00006d60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006d70: 6f6d 6169 6e3d 646f 6d61 696e 7061 7274  omain=domainpart
-00006d80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006d90: 2020 2020 2072 6573 6f75 7263 653d 7265       resource=re
-00006da0: 736f 7572 6365 7061 7274 290a 0a20 2020  sourcepart)..   
-00006db0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00006dc0: 2020 4066 756e 6374 6f6f 6c73 2e6c 7275    @functools.lru
-00006dd0: 5f63 6163 6865 286d 6178 7369 7a65 3d4e  _cache(maxsize=N
-00006de0: 6f6e 6529 0a20 2020 2064 6566 2066 726f  one).    def fro
-00006df0: 6d5f 7573 6572 5f69 6e70 7574 2863 6c73  m_user_input(cls
-00006e00: 2c20 7573 6572 5f69 6e70 7574 3a20 7374  , user_input: st
-00006e10: 722c 2065 7363 6170 6564 3a20 626f 6f6c  r, escaped: bool
-00006e20: 203d 2046 616c 7365 2920 2d3e 204a 4944   = False) -> JID
-00006e30: 3a0a 2020 2020 2020 2020 2320 5573 6520  :.        # Use 
-00006e40: 7468 6973 2069 6620 7765 2077 616e 7420  this if we want 
-00006e50: 4a49 4473 2074 6f20 6265 2065 7363 6170  JIDs to be escap
-00006e60: 6564 2061 6363 6f72 6469 6e67 2074 6f20  ed according to 
-00006e70: 5845 502d 3031 3036 0a20 2020 2020 2020  XEP-0106.       
-00006e80: 2023 2054 6865 2073 7461 6e64 6172 6420   # The standard 
-00006e90: 4a49 4420 7061 7273 696e 6720 6361 6e6e  JID parsing cann
-00006ea0: 6f74 2062 6520 6170 706c 6965 6420 6265  ot be applied be
-00006eb0: 6361 7573 6520 7573 6572 5f69 6e70 7574  cause user_input
-00006ec0: 2069 730a 2020 2020 2020 2020 2320 6e6f   is.        # no
-00006ed0: 7420 6120 7661 6c69 6420 4a49 442e 0a0a  t a valid JID...
-00006ee0: 2020 2020 2020 2020 2320 4f6e 6c79 2075          # Only u
-00006ef0: 7365 725f 696e 7075 7420 7768 6963 6820  ser_input which 
-00006f00: 6166 7465 7220 6573 6361 7069 6e67 2072  after escaping r
-00006f10: 6573 756c 7420 696e 2061 2062 6172 6520  esult in a bare 
-00006f20: 4a49 4420 6361 6e20 6265 0a20 2020 2020  JID can be.     
-00006f30: 2020 2023 2073 7563 6365 7373 6675 6c6c     # successfull
-00006f40: 7920 7061 7273 6564 2e0a 0a20 2020 2020  y parsed...     
-00006f50: 2020 2023 2054 6865 2061 7373 756d 7075     # The assumpu
-00006f60: 7469 6f6e 2069 7320 7573 6572 5f69 6e70  tion is user_inp
-00006f70: 7574 2069 7320 6120 6261 7265 204a 4944  ut is a bare JID
-00006f80: 2073 6f20 7765 2073 7461 7274 2077 6974   so we start wit
-00006f90: 6820 616e 0a20 2020 2020 2020 2023 2072  h an.        # r
-00006fa0: 7370 6c69 7420 6f6e 2040 2062 6563 6175  split on @ becau
-00006fb0: 7365 2077 6520 6173 7375 6d65 2074 6865  se we assume the
-00006fc0: 7265 2069 7320 6e6f 2072 6573 6f75 7263  re is no resourc
-00006fd0: 652c 2073 6f20 7468 6520 6368 6172 2040  e, so the char @
-00006fe0: 0a20 2020 2020 2020 2023 2069 6e20 7468  .        # in th
-00006ff0: 6520 6c6f 6361 6c70 6172 7420 6361 6e20  e localpart can 
-00007000: 6c61 7465 7220 6265 2065 7363 6170 6564  later be escaped
-00007010: 2e0a 0a20 2020 2020 2020 2069 6620 6573  ...        if es
-00007020: 6361 7065 643a 0a20 2020 2020 2020 2020  caped:.         
-00007030: 2020 2023 2066 6f72 2063 6f6e 7665 6e69     # for conveni
-00007040: 656e 6365 0a20 2020 2020 2020 2020 2020  ence.           
-00007050: 2072 6574 7572 6e20 636c 732e 6672 6f6d   return cls.from
-00007060: 5f73 7472 696e 6728 7573 6572 5f69 6e70  _string(user_inp
-00007070: 7574 290a 0a20 2020 2020 2020 2069 6620  ut)..        if 
-00007080: 2740 2720 696e 2075 7365 725f 696e 7075  '@' in user_inpu
-00007090: 743a 0a20 2020 2020 2020 2020 2020 206c  t:.            l
-000070a0: 6f63 616c 7061 7274 2c20 646f 6d61 696e  ocalpart, domain
-000070b0: 7061 7274 203d 2075 7365 725f 696e 7075  part = user_inpu
-000070c0: 742e 7273 706c 6974 2827 4027 2c20 3129  t.rsplit('@', 1)
-000070d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000070e0: 6c6f 6361 6c70 6172 742e 7374 6172 7473  localpart.starts
-000070f0: 7769 7468 2827 2027 2920 6f72 206c 6f63  with(' ') or loc
-00007100: 616c 7061 7274 2e65 6e64 7377 6974 6828  alpart.endswith(
-00007110: 2720 2729 3a0a 2020 2020 2020 2020 2020  ' '):.          
-00007120: 2020 2020 2020 7261 6973 6520 4c6f 6361        raise Loca
-00007130: 6c70 6172 744e 6f74 416c 6c6f 7765 6443  lpartNotAllowedC
-00007140: 6861 720a 0a20 2020 2020 2020 2020 2020  har..           
-00007150: 206c 6f63 616c 7061 7274 203d 2065 7363   localpart = esc
-00007160: 6170 655f 6c6f 6361 6c70 6172 7428 6c6f  ape_localpart(lo
-00007170: 6361 6c70 6172 7429 0a0a 2020 2020 2020  calpart)..      
-00007180: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007190: 2020 2020 6c6f 6361 6c70 6172 7420 3d20      localpart = 
-000071a0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000071b0: 2064 6f6d 6169 6e70 6172 7420 3d20 7573   domainpart = us
-000071c0: 6572 5f69 6e70 7574 0a0a 2020 2020 2020  er_input..      
-000071d0: 2020 7265 7475 726e 2063 6c73 286c 6f63    return cls(loc
-000071e0: 616c 7061 7274 3d6c 6f63 616c 7061 7274  alpart=localpart
-000071f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007200: 2020 2020 2064 6f6d 6169 6e3d 646f 6d61       domain=doma
-00007210: 696e 7061 7274 2c0a 2020 2020 2020 2020  inpart,.        
-00007220: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-00007230: 7263 653d 4e6f 6e65 290a 0a20 2020 2064  rce=None)..    d
-00007240: 6566 205f 5f73 7472 5f5f 2873 656c 6629  ef __str__(self)
-00007250: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00007260: 2069 6620 7365 6c66 2e6c 6f63 616c 7061   if self.localpa
-00007270: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
-00007280: 6a69 6420 3d20 6627 7b73 656c 662e 6c6f  jid = f'{self.lo
-00007290: 6361 6c70 6172 747d 407b 7365 6c66 2e64  calpart}@{self.d
-000072a0: 6f6d 6169 6e7d 270a 2020 2020 2020 2020  omain}'.        
-000072b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000072c0: 2020 6a69 6420 3d20 6361 7374 2873 7472    jid = cast(str
-000072d0: 2c20 7365 6c66 2e64 6f6d 6169 6e29 0a0a  , self.domain)..
-000072e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000072f0: 7265 736f 7572 6365 2069 7320 6e6f 7420  resource is not 
-00007300: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00007310: 2020 7265 7475 726e 2066 277b 6a69 647d    return f'{jid}
-00007320: 2f7b 7365 6c66 2e72 6573 6f75 7263 657d  /{self.resource}
-00007330: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-00007340: 206a 6964 0a0a 2020 2020 6465 6620 5f5f   jid..    def __
-00007350: 6861 7368 5f5f 2873 656c 6629 3a0a 2020  hash__(self):.  
-00007360: 2020 2020 2020 7265 7475 726e 2068 6173        return has
-00007370: 6828 7374 7228 7365 6c66 2929 0a0a 2020  h(str(self))..  
-00007380: 2020 6465 6620 5f5f 6571 5f5f 2873 656c    def __eq__(sel
-00007390: 662c 206f 7468 6572 3a20 556e 696f 6e5b  f, other: Union[
-000073a0: 7374 722c 204a 4944 5d29 202d 3e20 626f  str, JID]) -> bo
-000073b0: 6f6c 3a0a 2020 2020 2020 2020 6966 2069  ol:.        if i
-000073c0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-000073d0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-000073e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000073f0: 2020 2020 2020 2020 7265 7475 726e 204a          return J
-00007400: 4944 2e66 726f 6d5f 7374 7269 6e67 286f  ID.from_string(o
-00007410: 7468 6572 2920 3d3d 2073 656c 660a 2020  ther) == self.  
-00007420: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00007430: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
-00007440: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00007450: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-00007460: 2020 7265 7475 726e 2028 7365 6c66 2e6c    return (self.l
-00007470: 6f63 616c 7061 7274 203d 3d20 6f74 6865  ocalpart == othe
-00007480: 722e 6c6f 6361 6c70 6172 7420 616e 640a  r.localpart and.
-00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074a0: 7365 6c66 2e64 6f6d 6169 6e20 3d3d 206f  self.domain == o
-000074b0: 7468 6572 2e64 6f6d 6169 6e20 616e 640a  ther.domain and.
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 7365 6c66 2e72 6573 6f75 7263 6520 3d3d  self.resource ==
-000074e0: 206f 7468 6572 2e72 6573 6f75 7263 6529   other.resource)
-000074f0: 0a0a 2020 2020 6465 6620 5f5f 6e65 5f5f  ..    def __ne__
-00007500: 2873 656c 662c 206f 7468 6572 3a20 556e  (self, other: Un
-00007510: 696f 6e5b 7374 722c 204a 4944 5d29 202d  ion[str, JID]) -
-00007520: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00007530: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
-00007540: 5f5f 6571 5f5f 286f 7468 6572 290a 0a20  __eq__(other).. 
-00007550: 2020 2064 6566 2064 6f6d 6169 6e5f 746f     def domain_to
-00007560: 5f61 7363 6969 2873 656c 6629 202d 3e20  _ascii(self) -> 
-00007570: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
-00007580: 7572 6e20 6964 6e61 3230 3038 5f70 7265  urn idna2008_pre
-00007590: 7028 7365 6c66 2e64 6f6d 6169 6e2c 2074  p(self.domain, t
-000075a0: 6f5f 6173 6369 693d 5472 7565 290a 0a20  o_ascii=True).. 
-000075b0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000075c0: 2064 6566 2062 6172 6528 7365 6c66 2920   def bare(self) 
-000075d0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-000075e0: 6966 2073 656c 662e 6c6f 6361 6c70 6172  if self.localpar
-000075f0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-00007600: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007610: 6e20 6627 7b73 656c 662e 6c6f 6361 6c70  n f'{self.localp
-00007620: 6172 747d 407b 7365 6c66 2e64 6f6d 6169  art}@{self.domai
-00007630: 6e7d 270a 2020 2020 2020 2020 7265 7475  n}'.        retu
-00007640: 726e 2073 656c 662e 646f 6d61 696e 0a0a  rn self.domain..
-00007650: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00007660: 2020 6465 6620 6973 5f62 6172 6528 7365    def is_bare(se
-00007670: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00007680: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00007690: 2e72 6573 6f75 7263 6520 6973 204e 6f6e  .resource is Non
-000076a0: 650a 0a20 2020 2064 6566 206e 6577 5f61  e..    def new_a
-000076b0: 735f 6261 7265 2873 656c 6629 202d 3e20  s_bare(self) -> 
-000076c0: 4a49 443a 0a20 2020 2020 2020 2069 6620  JID:.        if 
-000076d0: 7365 6c66 2e72 6573 6f75 7263 6520 6973  self.resource is
-000076e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000076f0: 2020 2072 6574 7572 6e20 7365 6c66 0a20     return self. 
-00007700: 2020 2020 2020 2072 6574 7572 6e20 4a49         return JI
-00007710: 442e 6672 6f6d 5f73 7472 696e 6728 7365  D.from_string(se
-00007720: 6c66 2e62 6172 6529 0a0a 2020 2020 6465  lf.bare)..    de
-00007730: 6620 6261 7265 5f6d 6174 6368 2873 656c  f bare_match(sel
-00007740: 662c 206f 7468 6572 3a20 556e 696f 6e5b  f, other: Union[
-00007750: 7374 722c 204a 4944 5d29 202d 3e20 626f  str, JID]) -> bo
-00007760: 6f6c 3a0a 2020 2020 2020 2020 6966 2069  ol:.        if i
-00007770: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-00007780: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00007790: 2020 206f 7468 6572 203d 204a 4944 2e66     other = JID.f
-000077a0: 726f 6d5f 7374 7269 6e67 286f 7468 6572  rom_string(other
-000077b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000077c0: 2073 656c 662e 6261 7265 203d 3d20 6f74   self.bare == ot
-000077d0: 6865 722e 6261 7265 0a0a 2020 2020 4070  her.bare..    @p
-000077e0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000077f0: 6973 5f64 6f6d 6169 6e28 7365 6c66 2920  is_domain(self) 
-00007800: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00007810: 2072 6574 7572 6e20 7365 6c66 2e6c 6f63   return self.loc
-00007820: 616c 7061 7274 2069 7320 4e6f 6e65 2061  alpart is None a
-00007830: 6e64 2073 656c 662e 7265 736f 7572 6365  nd self.resource
-00007840: 2069 7320 4e6f 6e65 0a0a 2020 2020 4070   is None..    @p
-00007850: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00007860: 6973 5f66 756c 6c28 7365 6c66 2920 2d3e  is_full(self) ->
-00007870: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
-00007880: 6574 7572 6e20 2873 656c 662e 6c6f 6361  eturn (self.loca
-00007890: 6c70 6172 7420 6973 206e 6f74 204e 6f6e  lpart is not Non
-000078a0: 6520 616e 640a 2020 2020 2020 2020 2020  e and.          
-000078b0: 2020 2020 2020 7365 6c66 2e64 6f6d 6169        self.domai
-000078c0: 6e20 6973 206e 6f74 204e 6f6e 6520 616e  n is not None an
-000078d0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-000078e0: 2020 7365 6c66 2e72 6573 6f75 7263 6520    self.resource 
-000078f0: 6973 206e 6f74 204e 6f6e 6529 0a0a 2020  is not None)..  
-00007900: 2020 6465 6620 6e65 775f 7769 7468 2873    def new_with(s
-00007910: 656c 662c 202a 2a6b 7761 7267 733a 2064  elf, **kwargs: d
-00007920: 6963 745b 7374 722c 2073 7472 5d29 202d  ict[str, str]) -
-00007930: 3e20 4a49 443a 0a20 2020 2020 2020 206e  > JID:.        n
-00007940: 6577 203d 2061 7364 6963 7428 7365 6c66  ew = asdict(self
-00007950: 290a 2020 2020 2020 2020 6e65 772e 7570  ).        new.up
-00007960: 6461 7465 286b 7761 7267 7329 0a20 2020  date(kwargs).   
-00007970: 2020 2020 2072 6574 7572 6e20 4a49 4428       return JID(
-00007980: 2a2a 6e65 7729 0a0a 2020 2020 6465 6620  **new)..    def 
-00007990: 746f 5f75 7365 725f 7374 7269 6e67 2873  to_user_string(s
-000079a0: 656c 662c 2073 686f 775f 7075 6e79 636f  elf, show_punyco
-000079b0: 6465 3a20 626f 6f6c 203d 2054 7275 6529  de: bool = True)
-000079c0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-000079d0: 2064 6f6d 6169 6e20 3d20 7365 6c66 2e64   domain = self.d
-000079e0: 6f6d 6169 6e5f 746f 5f61 7363 6969 2829  omain_to_ascii()
-000079f0: 0a20 2020 2020 2020 2069 6620 646f 6d61  .        if doma
-00007a00: 696e 2e73 7461 7274 7377 6974 6828 2778  in.startswith('x
-00007a10: 6e2d 2d27 2920 616e 6420 7368 6f77 5f70  n--') and show_p
-00007a20: 756e 7963 6f64 653a 0a20 2020 2020 2020  unycode:.       
-00007a30: 2020 2020 2064 6f6d 6169 6e5f 656e 636f       domain_enco
-00007a40: 6465 6420 3d20 6627 2028 7b64 6f6d 6169  ded = f' ({domai
-00007a50: 6e7d 2927 0a20 2020 2020 2020 2065 6c73  n})'.        els
-00007a60: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-00007a70: 6f6d 6169 6e5f 656e 636f 6465 6420 3d20  omain_encoded = 
-00007a80: 2727 0a0a 2020 2020 2020 2020 6966 2073  ''..        if s
-00007a90: 656c 662e 6c6f 6361 6c70 6172 7420 6973  elf.localpart is
-00007aa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007ab0: 2020 2072 6574 7572 6e20 6627 7b73 656c     return f'{sel
-00007ac0: 667d 7b64 6f6d 6169 6e5f 656e 636f 6465  f}{domain_encode
-00007ad0: 647d 270a 0a20 2020 2020 2020 206c 6f63  d}'..        loc
-00007ae0: 616c 7061 7274 203d 2075 6e65 7363 6170  alpart = unescap
-00007af0: 655f 6c6f 6361 6c70 6172 7428 7365 6c66  e_localpart(self
-00007b00: 2e6c 6f63 616c 7061 7274 290a 0a20 2020  .localpart)..   
-00007b10: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-00007b20: 6f75 7263 6520 6973 204e 6f6e 653a 0a20  ource is None:. 
-00007b30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007b40: 6e20 6627 7b6c 6f63 616c 7061 7274 7d40  n f'{localpart}@
-00007b50: 7b73 656c 662e 646f 6d61 696e 7d7b 646f  {self.domain}{do
-00007b60: 6d61 696e 5f65 6e63 6f64 6564 7d27 0a20  main_encoded}'. 
-00007b70: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-00007b80: 7b6c 6f63 616c 7061 7274 7d40 7b73 656c  {localpart}@{sel
-00007b90: 662e 646f 6d61 696e 7d2f 7b73 656c 662e  f.domain}/{self.
-00007ba0: 7265 736f 7572 6365 7d7b 646f 6d61 696e  resource}{domain
-00007bb0: 5f65 6e63 6f64 6564 7d27 0a0a 2020 2020  _encoded}'..    
-00007bc0: 6465 6620 746f 5f69 7269 2873 656c 662c  def to_iri(self,
-00007bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007be0: 7175 6572 793a 204f 7074 696f 6e61 6c5b  query: Optional[
-00007bf0: 7374 7220 7c20 7475 706c 655b 7374 722c  str | tuple[str,
-00007c00: 206c 6973 745b 7475 706c 655b 7374 722c   list[tuple[str,
-00007c10: 2073 7472 5d5d 5d5d 203d 204e 6f6e 652c   str]]]] = None,
-00007c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c30: 6672 6167 6d65 6e74 3a20 4f70 7469 6f6e  fragment: Option
-00007c40: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
-00007c60: 2d3e 2073 7472 3a0a 0a20 2020 2020 2020  -> str:..       
-00007c70: 2069 6620 7365 6c66 2e6c 6f63 616c 7061   if self.localpa
-00007c80: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
-00007c90: 696e 6f64 6520 3d20 6573 6361 7065 5f69  inode = escape_i
-00007ca0: 6e6f 6465 2873 656c 662e 6c6f 6361 6c70  node(self.localp
-00007cb0: 6172 7429 0a20 2020 2020 2020 2020 2020  art).           
-00007cc0: 2069 7061 7468 786d 7070 203d 2066 277b   ipathxmpp = f'{
-00007cd0: 696e 6f64 657d 407b 7365 6c66 2e64 6f6d  inode}@{self.dom
-00007ce0: 6169 6e7d 270a 2020 2020 2020 2020 656c  ain}'.        el
-00007cf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007d00: 6970 6174 6878 6d70 7020 3d20 6627 7b73  ipathxmpp = f'{s
-00007d10: 656c 662e 646f 6d61 696e 7d27 0a0a 2020  elf.domain}'..  
-00007d20: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00007d30: 736f 7572 6365 2069 7320 6e6f 7420 4e6f  source is not No
-00007d40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007d50: 6972 6573 203d 2065 7363 6170 655f 6972  ires = escape_ir
-00007d60: 6573 2873 656c 662e 7265 736f 7572 6365  es(self.resource
-00007d70: 290a 2020 2020 2020 2020 2020 2020 6970  ).            ip
-00007d80: 6174 6878 6d70 7020 3d20 6627 7b69 7061  athxmpp = f'{ipa
-00007d90: 7468 786d 7070 7d2f 7b69 7265 737d 270a  thxmpp}/{ires}'.
-00007da0: 0a20 2020 2020 2020 2069 7269 203d 2066  .        iri = f
-00007db0: 2778 6d70 703a 7b69 7061 7468 786d 7070  'xmpp:{ipathxmpp
-00007dc0: 7d27 0a0a 2020 2020 2020 2020 6966 2071  }'..        if q
-00007dd0: 7565 7279 2069 7320 6e6f 7420 4e6f 6e65  uery is not None
-00007de0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00007df0: 2069 7369 6e73 7461 6e63 6528 7175 6572   isinstance(quer
-00007e00: 792c 2073 7472 293a 0a20 2020 2020 2020  y, str):.       
-00007e10: 2020 2020 2020 2020 2071 7565 7279 7479           queryty
-00007e20: 7065 203d 2071 7565 7279 0a20 2020 2020  pe = query.     
-00007e30: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00007e40: 7061 7261 6d73 203d 204e 6f6e 650a 2020  params = None.  
-00007e50: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 7175 6572 7974 7970 652c 2071 7565 7279  querytype, query
-00007e80: 7061 7261 6d73 203d 2071 7565 7279 0a0a  params = query..
-00007e90: 2020 2020 2020 2020 2020 2020 6971 7565              ique
-00007ea0: 7279 7479 7065 203d 2076 616c 6964 6174  rytype = validat
-00007eb0: 655f 7175 6572 7974 7970 6528 7175 6572  e_querytype(quer
-00007ec0: 7974 7970 6529 0a20 2020 2020 2020 2020  ytype).         
-00007ed0: 2020 2069 7269 202b 3d20 6627 3f7b 6971     iri += f'?{iq
-00007ee0: 7565 7279 7479 7065 7d27 0a0a 2020 2020  uerytype}'..    
-00007ef0: 2020 2020 2020 2020 6966 2071 7565 7279          if query
-00007f00: 7061 7261 6d73 2069 7320 6e6f 7420 4e6f  params is not No
-00007f10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007f20: 2020 2020 666f 7220 696b 6579 2c20 6976      for ikey, iv
-00007f30: 616c 7565 2069 6e20 7175 6572 7970 6172  alue in querypar
-00007f40: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
-00007f50: 2020 2020 2020 2020 2069 7661 6c75 6520           ivalue 
-00007f60: 3d20 6573 6361 7065 5f69 7661 6c75 6528  = escape_ivalue(
-00007f70: 6976 616c 7565 290a 2020 2020 2020 2020  ivalue).        
-00007f80: 2020 2020 2020 2020 2020 2020 696b 6579              ikey
-00007f90: 203d 2076 616c 6964 6174 655f 696b 6579   = validate_ikey
-00007fa0: 2869 6b65 7929 0a20 2020 2020 2020 2020  (ikey).         
-00007fb0: 2020 2020 2020 2020 2020 2069 7269 202b             iri +
-00007fc0: 3d20 6627 3b7b 696b 6579 7d3d 7b69 7661  = f';{ikey}={iva
-00007fd0: 6c75 657d 270a 0a20 2020 2020 2020 2069  lue}'..        i
-00007fe0: 6620 6672 6167 6d65 6e74 2069 7320 6e6f  f fragment is no
-00007ff0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00008000: 2020 2020 6966 7261 676d 656e 7420 3d20      ifragment = 
-00008010: 6573 6361 7065 5f69 6672 6167 6d65 6e74  escape_ifragment
-00008020: 2866 7261 676d 656e 7429 0a20 2020 2020  (fragment).     
-00008030: 2020 2020 2020 2069 7269 202b 3d20 6627         iri += f'
-00008040: 237b 6966 7261 676d 656e 747d 270a 0a20  #{ifragment}'.. 
-00008050: 2020 2020 2020 2072 6574 7572 6e20 6972         return ir
-00008060: 690a 0a20 2020 2064 6566 2063 6f70 7928  i..    def copy(
-00008070: 7365 6c66 2920 2d3e 204a 4944 3a0a 2020  self) -> JID:.  
-00008080: 2020 2020 2020 6465 7072 6563 6174 696f        deprecatio
-00008090: 6e5f 7761 726e 696e 6728 2763 6f70 7928  n_warning('copy(
-000080a0: 2920 6973 206e 6f74 206e 6565 6465 642c  ) is not needed,
-000080b0: 204a 4944 2069 7320 696d 6d75 7461 626c   JID is immutabl
-000080c0: 6527 290a 2020 2020 2020 2020 7265 7475  e').        retu
-000080d0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000080e0: 5374 7265 616d 4572 726f 724e 6f64 6528  StreamErrorNode(
-000080f0: 4e6f 6465 293a 0a20 2020 2064 6566 205f  Node):.    def _
-00008100: 5f69 6e69 745f 5f28 7365 6c66 2c20 6e6f  _init__(self, no
-00008110: 6465 293a 0a20 2020 2020 2020 204e 6f64  de):.        Nod
-00008120: 652e 5f5f 696e 6974 5f5f 2873 656c 662c  e.__init__(self,
-00008130: 206e 6f64 653d 6e6f 6465 290a 0a20 2020   node=node)..   
-00008140: 2020 2020 2073 656c 662e 5f74 6578 743a       self._text:
-00008150: 2064 6963 745b 4f70 7469 6f6e 616c 5b73   dict[Optional[s
-00008160: 7472 5d2c 2073 7472 5d20 3d20 7b7d 0a0a  tr], str] = {}..
-00008170: 2020 2020 2020 2020 7465 7874 5f65 6c65          text_ele
-00008180: 6d65 6e74 7320 3d20 7365 6c66 2e67 6574  ments = self.get
-00008190: 5461 6773 2827 7465 7874 272c 206e 616d  Tags('text', nam
-000081a0: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
-000081b0: 2e58 4d50 505f 5354 5245 414d 5329 0a20  .XMPP_STREAMS). 
-000081c0: 2020 2020 2020 2066 6f72 2065 6c65 6d65         for eleme
-000081d0: 6e74 2069 6e20 7465 7874 5f65 6c65 6d65  nt in text_eleme
-000081e0: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
-000081f0: 206c 616e 6720 3d20 656c 656d 656e 742e   lang = element.
-00008200: 6765 7458 6d6c 4c61 6e67 2829 0a20 2020  getXmlLang().   
-00008210: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00008220: 656c 656d 656e 742e 6765 7444 6174 6128  element.getData(
-00008230: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00008240: 6c66 2e5f 7465 7874 5b6c 616e 675d 203d  lf._text[lang] =
-00008250: 2074 6578 740a 0a20 2020 2064 6566 2067   text..    def g
-00008260: 6574 5f63 6f6e 6469 7469 6f6e 2873 656c  et_condition(sel
-00008270: 6629 202d 3e20 4f70 7469 6f6e 616c 5b73  f) -> Optional[s
-00008280: 7472 5d3a 0a20 2020 2020 2020 2066 6f72  tr]:.        for
-00008290: 2074 6167 2069 6e20 7365 6c66 2e67 6574   tag in self.get
-000082a0: 4368 696c 6472 656e 2829 3a0a 2020 2020  Children():.    
-000082b0: 2020 2020 2020 2020 6966 2028 7461 672e          if (tag.
-000082c0: 6765 744e 616d 6528 2920 213d 2027 7465  getName() != 'te
-000082d0: 7874 2720 616e 640a 2020 2020 2020 2020  xt' and.        
-000082e0: 2020 2020 2020 2020 2020 2020 7461 672e              tag.
-000082f0: 6765 744e 616d 6573 7061 6365 2829 203d  getNamespace() =
-00008300: 3d20 4e61 6d65 7370 6163 652e 584d 5050  = Namespace.XMPP
-00008310: 5f53 5452 4541 4d53 293a 0a20 2020 2020  _STREAMS):.     
-00008320: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008330: 6e20 7461 672e 6765 744e 616d 6528 290a  n tag.getName().
-00008340: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00008350: 6f6e 650a 0a20 2020 2064 6566 2067 6574  one..    def get
-00008360: 5f74 6578 7428 7365 6c66 2c20 7072 6566  _text(self, pref
-00008370: 5f6c 616e 673a 204f 7074 696f 6e61 6c5b  _lang: Optional[
-00008380: 7374 725d 203d 204e 6f6e 6529 202d 3e20  str] = None) -> 
-00008390: 7374 723a 0a20 2020 2020 2020 2069 6620  str:.        if 
-000083a0: 7072 6566 5f6c 616e 6720 6973 206e 6f74  pref_lang is not
-000083b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000083c0: 2020 2074 6578 7420 3d20 7365 6c66 2e5f     text = self._
-000083d0: 7465 7874 2e67 6574 2870 7265 665f 6c61  text.get(pref_la
-000083e0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
-000083f0: 6966 2074 6578 7420 6973 206e 6f74 204e  if text is not N
-00008400: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00008410: 2020 2020 2072 6574 7572 6e20 7465 7874       return text
-00008420: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00008430: 662e 5f74 6578 743a 0a20 2020 2020 2020  f._text:.       
-00008440: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
-00008450: 2e5f 7465 7874 2e67 6574 2827 656e 2729  ._text.get('en')
-00008460: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00008470: 7465 7874 2069 7320 6e6f 7420 4e6f 6e65  text is not None
-00008480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008490: 2020 7265 7475 726e 2074 6578 740a 0a20    return text.. 
-000084a0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-000084b0: 3d20 7365 6c66 2e5f 7465 7874 2e67 6574  = self._text.get
-000084c0: 284e 6f6e 6529 0a20 2020 2020 2020 2020  (None).         
-000084d0: 2020 2069 6620 7465 7874 2069 7320 6e6f     if text is no
-000084e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000084f0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00008500: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-00008510: 7265 7475 726e 2073 656c 662e 5f74 6578  return self._tex
-00008520: 742e 706f 7069 7465 6d28 295b 315d 0a20  t.popitem()[1]. 
-00008530: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
-00008540: 0a0a 0a63 6c61 7373 2050 726f 746f 636f  ...class Protoco
-00008550: 6c28 4e6f 6465 293a 0a20 2020 2022 2222  l(Node):.    """
-00008560: 0a20 2020 2041 2022 7374 616e 7a61 2220  .    A "stanza" 
-00008570: 6f62 6a65 6374 2063 6c61 7373 2e20 436f  object class. Co
-00008580: 6e74 6169 6e73 206d 6574 686f 6473 2074  ntains methods t
-00008590: 6861 7420 6172 6520 636f 6d6d 6f6e 2066  hat are common f
-000085a0: 6f72 2070 7265 7365 6e63 6573 2c20 6971  or presences, iq
-000085b0: 730a 2020 2020 616e 6420 6d65 7373 6167  s.    and messag
-000085c0: 6573 0a20 2020 2022 2222 0a0a 2020 2020  es.    """..    
-000085d0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000085e0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-000085f0: 2020 2020 6e61 6d65 3d4e 6f6e 652c 0a20      name=None,. 
-00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008610: 746f 3d4e 6f6e 652c 0a20 2020 2020 2020  to=None,.       
-00008620: 2020 2020 2020 2020 2020 7479 703d 4e6f            typ=No
-00008630: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00008640: 2020 2020 2066 726d 3d4e 6f6e 652c 0a20       frm=None,. 
-00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008660: 6174 7472 733d 4e6f 6e65 2c0a 2020 2020  attrs=None,.    
-00008670: 2020 2020 2020 2020 2020 2020 2070 6179               pay
-00008680: 6c6f 6164 3d4e 6f6e 652c 0a20 2020 2020  load=None,.     
-00008690: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-000086a0: 7374 616d 703d 4e6f 6e65 2c0a 2020 2020  stamp=None,.    
-000086b0: 2020 2020 2020 2020 2020 2020 2078 6d6c               xml
-000086c0: 6e73 3d4e 6f6e 652c 0a20 2020 2020 2020  ns=None,.       
-000086d0: 2020 2020 2020 2020 2020 6e6f 6465 3d4e            node=N
-000086e0: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-000086f0: 220a 2020 2020 2020 2020 436f 6e73 7472  ".        Constr
-00008700: 7563 746f 722c 206e 616d 6520 6973 2074  uctor, name is t
-00008710: 6865 206e 616d 6520 6f66 2074 6865 2073  he name of the s
-00008720: 7461 6e7a 610a 2020 2020 2020 2020 692e  tanza.        i.
-00008730: 652e 2027 6d65 7373 6167 6527 206f 7220  e. 'message' or 
-00008740: 2770 7265 7365 6e63 6527 6f72 2027 6971  'presence'or 'iq
-00008750: 270a 0a20 2020 2020 2020 2074 6f20 6973  '..        to is
-00008760: 2074 6865 2076 616c 7565 206f 6620 2774   the value of 't
-00008770: 6f27 2061 7474 7269 6275 7265 2c20 2774  o' attribure, 't
-00008780: 7970 2720 2d20 2774 7970 6527 2061 7474  yp' - 'type' att
-00008790: 7269 6275 7465 0a20 2020 2020 2020 2066  ribute.        f
-000087a0: 726e 202d 2066 726f 6d20 6174 7472 6962  rn - from attrib
-000087b0: 7572 652c 2061 7474 7273 202d 206f 7468  ure, attrs - oth
-000087c0: 6572 2061 7474 7269 6275 7465 7320 6d61  er attributes ma
-000087d0: 7070 696e 672c 0a20 2020 2020 2020 2070  pping,.        p
-000087e0: 6179 6c6f 6164 202d 2073 616d 6520 6d65  ayload - same me
-000087f0: 616e 696e 6720 6173 2066 6f72 2073 696d  aning as for sim
-00008800: 706c 6578 6d6c 2070 6179 6c6f 6164 2064  plexml payload d
-00008810: 6566 696e 6974 696f 6e0a 2020 2020 2020  efinition.      
-00008820: 2020 7469 6d65 7374 616d 7020 2d20 7468    timestamp - th
-00008830: 6520 7469 6d65 2076 616c 7565 2074 6861  e time value tha
-00008840: 7420 6e65 6564 7320 746f 2062 6520 7374  t needs to be st
-00008850: 616d 7065 6420 6f76 6572 2073 7461 6e7a  amped over stanz
-00008860: 610a 2020 2020 2020 2020 786d 6c6e 7320  a.        xmlns 
-00008870: 2d20 6e61 6d65 7370 6163 6520 6f66 2074  - namespace of t
-00008880: 6f70 2073 7461 6e7a 6120 6e6f 6465 0a20  op stanza node. 
-00008890: 2020 2020 2020 206e 6f64 6520 2d20 7061         node - pa
-000088a0: 7273 6564 206f 7220 756e 7061 7273 6564  rsed or unparsed
-000088b0: 2073 7461 6e61 2074 6f20 6265 2074 616b   stana to be tak
-000088c0: 656e 2061 7320 7072 6f74 6f74 7970 652e  en as prototype.
-000088d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000088e0: 2020 2020 2069 6620 6e6f 7420 6174 7472       if not attr
-000088f0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00008900: 7474 7273 203d 207b 7d0a 2020 2020 2020  ttrs = {}.      
-00008910: 2020 6966 2074 6f3a 0a20 2020 2020 2020    if to:.       
-00008920: 2020 2020 2061 7474 7273 5b27 746f 275d       attrs['to']
-00008930: 203d 2074 6f0a 2020 2020 2020 2020 6966   = to.        if
-00008940: 2066 726d 3a0a 2020 2020 2020 2020 2020   frm:.          
-00008950: 2020 6174 7472 735b 2766 726f 6d27 5d20    attrs['from'] 
-00008960: 3d20 6672 6d0a 2020 2020 2020 2020 6966  = frm.        if
-00008970: 2074 7970 3a0a 2020 2020 2020 2020 2020   typ:.          
-00008980: 2020 6174 7472 735b 2774 7970 6527 5d20    attrs['type'] 
-00008990: 3d20 7479 700a 2020 2020 2020 2020 4e6f  = typ.        No
-000089a0: 6465 2e5f 5f69 6e69 745f 5f28 7365 6c66  de.__init__(self
-000089b0: 2c20 7461 673d 6e61 6d65 2c20 6174 7472  , tag=name, attr
-000089c0: 733d 6174 7472 732c 2070 6179 6c6f 6164  s=attrs, payload
-000089d0: 3d70 6179 6c6f 6164 2c20 6e6f 6465 3d6e  =payload, node=n
-000089e0: 6f64 6529 0a20 2020 2020 2020 2069 6620  ode).        if 
-000089f0: 6e6f 7420 6e6f 6465 2061 6e64 2078 6d6c  not node and xml
-00008a00: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00008a10: 7365 6c66 2e73 6574 4e61 6d65 7370 6163  self.setNamespac
-00008a20: 6528 786d 6c6e 7329 0a20 2020 2020 2020  e(xmlns).       
-00008a30: 2069 6620 7365 6c66 5b27 746f 275d 3a0a   if self['to']:.
-00008a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008a50: 2e73 6574 546f 2873 656c 665b 2774 6f27  .setTo(self['to'
-00008a60: 5d29 0a20 2020 2020 2020 2069 6620 7365  ]).        if se
-00008a70: 6c66 5b27 6672 6f6d 275d 3a0a 2020 2020  lf['from']:.    
-00008a80: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00008a90: 4672 6f6d 2873 656c 665b 2766 726f 6d27  From(self['from'
-00008aa0: 5d29 0a20 2020 2020 2020 2069 6620 286e  ]).        if (n
-00008ab0: 6f64 6520 616e 640a 2020 2020 2020 2020  ode and.        
-00008ac0: 2020 2020 2020 2020 6973 696e 7374 616e          isinstan
-00008ad0: 6365 286e 6f64 652c 2050 726f 746f 636f  ce(node, Protoco
-00008ae0: 6c29 2061 6e64 0a20 2020 2020 2020 2020  l) and.         
-00008af0: 2020 2020 2020 2073 656c 662e 5f5f 636c         self.__cl
-00008b00: 6173 735f 5f20 3d3d 206e 6f64 652e 5f5f  ass__ == node.__
-00008b10: 636c 6173 735f 5f0a 2020 2020 2020 2020  class__.        
-00008b20: 2020 2020 2020 2020 616e 6420 2769 6427          and 'id'
-00008b30: 2069 6e20 7365 6c66 2e61 7474 7273 293a   in self.attrs):
-00008b40: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-00008b50: 2073 656c 662e 6174 7472 735b 2769 6427   self.attrs['id'
-00008b60: 5d0a 2020 2020 2020 2020 7365 6c66 2e74  ].        self.t
-00008b70: 696d 6573 7461 6d70 203d 204e 6f6e 650a  imestamp = None.
-00008b80: 2020 2020 2020 2020 666f 7220 6420 696e          for d in
-00008b90: 2073 656c 662e 6765 7454 6167 7328 2764   self.getTags('d
-00008ba0: 656c 6179 272c 206e 616d 6573 7061 6365  elay', namespace
-00008bb0: 3d4e 616d 6573 7061 6365 2e44 454c 4159  =Namespace.DELAY
-00008bc0: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
-00008bd0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00008be0: 2020 2020 2069 6620 642e 6765 7441 7474       if d.getAtt
-00008bf0: 7228 2773 7461 6d70 2729 203c 2073 656c  r('stamp') < sel
-00008c00: 662e 6765 7454 696d 6573 7461 6d70 3228  f.getTimestamp2(
-00008c10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008c20: 2020 2020 2020 2073 656c 662e 7365 7454         self.setT
-00008c30: 696d 6573 7461 6d70 2864 2e67 6574 4174  imestamp(d.getAt
-00008c40: 7472 2827 7374 616d 7027 2929 0a20 2020  tr('stamp')).   
-00008c50: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00008c60: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
-00008c70: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00008c80: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00008c90: 656c 662e 7469 6d65 7374 616d 703a 0a20  elf.timestamp:. 
-00008ca0: 2020 2020 2020 2020 2020 2066 6f72 2078             for x
-00008cb0: 2069 6e20 7365 6c66 2e67 6574 5461 6773   in self.getTags
-00008cc0: 2827 7827 2c20 6e61 6d65 7370 6163 653d  ('x', namespace=
-00008cd0: 4e61 6d65 7370 6163 652e 4445 4c41 5929  Namespace.DELAY)
-00008ce0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008cf0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00008d00: 2020 2020 2020 2020 2020 2069 6620 782e             if x.
-00008d10: 6765 7441 7474 7228 2773 7461 6d70 2729  getAttr('stamp')
-00008d20: 203c 2073 656c 662e 6765 7454 696d 6573   < self.getTimes
-00008d30: 7461 6d70 2829 3a0a 2020 2020 2020 2020  tamp():.        
-00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 7365 6c66 2e73 6574 5469 6d65 7374 616d  self.setTimestam
-00008d60: 7028 782e 6765 7441 7474 7228 2773 7461  p(x.getAttr('sta
-00008d70: 6d70 2729 290a 2020 2020 2020 2020 2020  mp')).          
-00008d80: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00008d90: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
-00008da0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00008db0: 0a20 2020 2020 2020 2069 6620 7469 6d65  .        if time
-00008dc0: 7374 616d 7020 6973 206e 6f74 204e 6f6e  stamp is not Non
-00008dd0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00008de0: 656c 662e 7365 7454 696d 6573 7461 6d70  elf.setTimestamp
-00008df0: 2874 696d 6573 7461 6d70 290a 0a20 2020  (timestamp)..   
-00008e00: 2064 6566 2069 7345 7272 6f72 2873 656c   def isError(sel
-00008e10: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00008e20: 726e 2073 656c 662e 6765 7441 7474 7228  rn self.getAttr(
-00008e30: 2774 7970 6527 2920 3d3d 2027 6572 726f  'type') == 'erro
-00008e40: 7227 0a0a 2020 2020 6465 6620 6973 5265  r'..    def isRe
-00008e50: 7375 6c74 2873 656c 6629 3a0a 2020 2020  sult(self):.    
-00008e60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00008e70: 6765 7441 7474 7228 2774 7970 6527 2920  getAttr('type') 
-00008e80: 3d3d 2027 7265 7375 6c74 270a 0a20 2020  == 'result'..   
-00008e90: 2064 6566 2067 6574 546f 2873 656c 6629   def getTo(self)
-00008ea0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00008eb0: 2020 2020 2020 5265 7475 726e 2076 616c        Return val
-00008ec0: 7565 206f 6620 7468 6520 2774 6f27 2061  ue of the 'to' a
-00008ed0: 7474 7269 6275 7465 0a20 2020 2020 2020  ttribute.       
-00008ee0: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
-00008ef0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00008f00: 7475 726e 2073 656c 665b 2774 6f27 5d0a  turn self['to'].
-00008f10: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00008f20: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00008f30: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00008f40: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00008f50: 2020 2020 6465 6620 6765 7446 726f 6d28      def getFrom(
-00008f60: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00008f70: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00008f80: 6e20 7661 6c75 6520 6f66 2074 6865 2027  n value of the '
-00008f90: 6672 6f6d 2720 6174 7472 6962 7574 650a  from' attribute.
-00008fa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008fb0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00008fc0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008fd0: 5b27 6672 6f6d 275d 0a20 2020 2020 2020  ['from'].       
-00008fe0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00008ff0: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
-00009000: 6173 730a 2020 2020 2020 2020 7265 7475  ass.        retu
-00009010: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
-00009020: 2067 6574 5469 6d65 7374 616d 7028 7365   getTimestamp(se
-00009030: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00009040: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-00009050: 7468 6520 7469 6d65 7374 616d 7020 696e  the timestamp in
-00009060: 2074 6865 2027 7979 7979 6d6d 6464 5468   the 'yyyymmddTh
-00009070: 686d 6d73 7327 2066 6f72 6d61 740a 2020  hmmss' format.  
-00009080: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00009090: 2020 6966 2073 656c 662e 7469 6d65 7374    if self.timest
-000090a0: 616d 703a 0a20 2020 2020 2020 2020 2020  amp:.           
-000090b0: 2072 6574 7572 6e20 7365 6c66 2e74 696d   return self.tim
-000090c0: 6573 7461 6d70 0a20 2020 2020 2020 2072  estamp.        r
-000090d0: 6574 7572 6e20 7469 6d65 2e73 7472 6674  eturn time.strft
-000090e0: 696d 6528 2725 5925 6d25 6454 2548 3a25  ime('%Y%m%dT%H:%
-000090f0: 4d3a 2553 272c 2074 696d 652e 676d 7469  M:%S', time.gmti
-00009100: 6d65 2829 290a 0a20 2020 2064 6566 2067  me())..    def g
-00009110: 6574 5469 6d65 7374 616d 7032 2873 656c  etTimestamp2(sel
-00009120: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00009130: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-00009140: 6865 2074 696d 6573 7461 6d70 2069 6e20  he timestamp in 
-00009150: 7468 6520 2779 7979 796d 6d64 6454 6868  the 'yyyymmddThh
-00009160: 6d6d 7373 2720 666f 726d 6174 0a20 2020  mmss' format.   
-00009170: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009180: 2069 6620 7365 6c66 2e74 696d 6573 7461   if self.timesta
-00009190: 6d70 3a0a 2020 2020 2020 2020 2020 2020  mp:.            
-000091a0: 7265 7475 726e 2073 656c 662e 7469 6d65  return self.time
-000091b0: 7374 616d 700a 2020 2020 2020 2020 7265  stamp.        re
-000091c0: 7475 726e 2074 696d 652e 7374 7266 7469  turn time.strfti
-000091d0: 6d65 2827 2559 2d25 6d2d 2564 5425 483a  me('%Y-%m-%dT%H:
-000091e0: 254d 3a25 535a 272c 2074 696d 652e 676d  %M:%SZ', time.gm
-000091f0: 7469 6d65 2829 290a 0a20 2020 2064 6566  time())..    def
-00009200: 2067 6574 4a69 6428 7365 6c66 293a 0a20   getJid(self):. 
-00009210: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009220: 2020 2052 6574 7572 6e20 7468 6520 7661     Return the va
-00009230: 6c75 6520 6f66 2074 6865 2027 6a69 6427  lue of the 'jid'
-00009240: 2061 7474 7269 6275 7465 0a20 2020 2020   attribute.     
-00009250: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-00009260: 7474 7220 3d20 7365 6c66 2e67 6574 4174  ttr = self.getAt
-00009270: 7472 2827 6a69 6427 290a 2020 2020 2020  tr('jid').      
-00009280: 2020 6966 2061 7474 723a 0a20 2020 2020    if attr:.     
-00009290: 2020 2020 2020 2072 6574 7572 6e20 4a49         return JI
-000092a0: 442e 6672 6f6d 5f73 7472 696e 6728 6174  D.from_string(at
-000092b0: 7472 290a 2020 2020 2020 2020 7265 7475  tr).        retu
-000092c0: 726e 2061 7474 720a 0a20 2020 2064 6566  rn attr..    def
-000092d0: 2067 6574 4944 2873 656c 6629 202d 3e20   getID(self) -> 
-000092e0: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
-000092f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009300: 2020 2052 6574 7572 6e20 7468 6520 7661     Return the va
-00009310: 6c75 6520 6f66 2074 6865 2027 6964 2720  lue of the 'id' 
-00009320: 6174 7472 6962 7574 650a 2020 2020 2020  attribute.      
-00009330: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00009340: 7475 726e 2073 656c 662e 6765 7441 7474  turn self.getAtt
-00009350: 7228 2769 6427 290a 0a20 2020 2064 6566  r('id')..    def
-00009360: 2073 6574 546f 2873 656c 662c 2076 616c   setTo(self, val
-00009370: 3a20 556e 696f 6e5b 7374 722c 204a 4944  : Union[str, JID
-00009380: 5d29 3a0a 2020 2020 2020 2020 2222 220a  ]):.        """.
-00009390: 2020 2020 2020 2020 5365 7420 7468 6520          Set the 
-000093a0: 7661 6c75 6520 6f66 2074 6865 2027 746f  value of the 'to
-000093b0: 2720 6174 7472 6962 7574 650a 2020 2020  ' attribute.    
-000093c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000093d0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-000093e0: 6528 7661 6c2c 204a 4944 293a 0a20 2020  e(val, JID):.   
-000093f0: 2020 2020 2020 2020 2076 616c 203d 204a           val = J
-00009400: 4944 2e66 726f 6d5f 7374 7269 6e67 2876  ID.from_string(v
-00009410: 616c 290a 2020 2020 2020 2020 7365 6c66  al).        self
-00009420: 2e73 6574 4174 7472 2827 746f 272c 2076  .setAttr('to', v
-00009430: 616c 290a 0a20 2020 2064 6566 2067 6574  al)..    def get
-00009440: 5479 7065 2873 656c 6629 202d 3e20 4f70  Type(self) -> Op
-00009450: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
-00009460: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009470: 2052 6574 7572 6e20 7468 6520 7661 6c75   Return the valu
-00009480: 6520 6f66 2074 6865 2027 7479 7065 2720  e of the 'type' 
-00009490: 6174 7472 6962 7574 650a 2020 2020 2020  attribute.      
-000094a0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-000094b0: 7475 726e 2073 656c 662e 6765 7441 7474  turn self.getAtt
-000094c0: 7228 2774 7970 6527 290a 0a20 2020 2064  r('type')..    d
-000094d0: 6566 2073 6574 4672 6f6d 2873 656c 662c  ef setFrom(self,
-000094e0: 2076 616c 3a20 556e 696f 6e5b 7374 722c   val: Union[str,
-000094f0: 204a 4944 5d29 3a0a 2020 2020 2020 2020   JID]):.        
-00009500: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
-00009510: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
-00009520: 2027 6672 6f6d 2720 6174 7472 6962 7574   'from' attribut
-00009530: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00009540: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-00009550: 6e73 7461 6e63 6528 7661 6c2c 204a 4944  nstance(val, JID
-00009560: 293a 0a20 2020 2020 2020 2020 2020 2076  ):.            v
-00009570: 616c 203d 204a 4944 2e66 726f 6d5f 7374  al = JID.from_st
-00009580: 7269 6e67 2876 616c 290a 2020 2020 2020  ring(val).      
-00009590: 2020 7365 6c66 2e73 6574 4174 7472 2827    self.setAttr('
-000095a0: 6672 6f6d 272c 2076 616c 290a 0a20 2020  from', val)..   
-000095b0: 2064 6566 2073 6574 5479 7065 2873 656c   def setType(sel
-000095c0: 662c 2076 616c 3a20 7374 7229 3a0a 2020  f, val: str):.  
-000095d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000095e0: 2020 5365 7420 7468 6520 7661 6c75 6520    Set the value 
-000095f0: 6f66 2074 6865 2027 7479 7065 2720 6174  of the 'type' at
-00009600: 7472 6962 7574 650a 2020 2020 2020 2020  tribute.        
-00009610: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00009620: 2e73 6574 4174 7472 2827 7479 7065 272c  .setAttr('type',
-00009630: 2076 616c 290a 0a20 2020 2064 6566 2073   val)..    def s
-00009640: 6574 4944 2873 656c 662c 2076 616c 3a20  etID(self, val: 
-00009650: 7374 7229 3a0a 2020 2020 2020 2020 2222  str):.        ""
-00009660: 220a 2020 2020 2020 2020 5365 7420 7468  ".        Set th
-00009670: 6520 7661 6c75 6520 6f66 2074 6865 2027  e value of the '
-00009680: 6964 2720 6174 7472 6962 7574 650a 2020  id' attribute.  
-00009690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000096a0: 2020 7365 6c66 2e73 6574 4174 7472 2827    self.setAttr('
-000096b0: 6964 272c 2076 616c 290a 0a20 2020 2064  id', val)..    d
-000096c0: 6566 2067 6574 4572 726f 7228 7365 6c66  ef getError(self
-000096d0: 2920 2d3e 204f 7074 696f 6e61 6c5b 7374  ) -> Optional[st
-000096e0: 725d 3a0a 2020 2020 2020 2020 2222 220a  r]:.        """.
-000096f0: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-00009700: 6865 2065 7272 6f72 2d63 6f6e 6469 7469  he error-conditi
-00009710: 6f6e 2028 6966 2070 7265 7365 6e74 2920  on (if present) 
-00009720: 6f72 2074 6865 2074 6578 7475 616c 2064  or the textual d
-00009730: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
-00009740: 2020 206f 6620 7468 6520 6572 726f 7220     of the error 
-00009750: 286f 7468 6572 7769 7365 290a 2020 2020  (otherwise).    
-00009760: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009770: 6572 7274 6167 203d 2073 656c 662e 6765  errtag = self.ge
-00009780: 7454 6167 2827 6572 726f 7227 290a 2020  tTag('error').  
-00009790: 2020 2020 2020 6966 2065 7272 7461 6720        if errtag 
-000097a0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000097b0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-000097c0: 0a20 2020 2020 2020 2066 6f72 2074 6167  .        for tag
-000097d0: 2069 6e20 6572 7274 6167 2e67 6574 4368   in errtag.getCh
-000097e0: 696c 6472 656e 2829 3a0a 2020 2020 2020  ildren():.      
-000097f0: 2020 2020 2020 6966 2028 7461 672e 6765        if (tag.ge
-00009800: 744e 616d 6528 2920 213d 2027 7465 7874  tName() != 'text
-00009810: 2720 616e 640a 2020 2020 2020 2020 2020  ' and.          
-00009820: 2020 2020 2020 2020 2020 7461 672e 6765            tag.ge
-00009830: 744e 616d 6573 7061 6365 2829 203d 3d20  tNamespace() == 
-00009840: 4e61 6d65 7370 6163 652e 5354 414e 5a41  Namespace.STANZA
-00009850: 5329 3a0a 2020 2020 2020 2020 2020 2020  S):.            
-00009860: 2020 2020 7265 7475 726e 2074 6167 2e67      return tag.g
-00009870: 6574 4e61 6d65 2829 0a20 2020 2020 2020  etName().       
-00009880: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00009890: 2020 6465 6620 6765 7441 7070 4572 726f    def getAppErro
-000098a0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-000098b0: 2065 7272 7461 6720 3d20 7365 6c66 2e67   errtag = self.g
-000098c0: 6574 5461 6728 2765 7272 6f72 2729 0a20  etTag('error'). 
-000098d0: 2020 2020 2020 2069 6620 6572 7274 6167         if errtag
-000098e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000098f0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00009900: 650a 2020 2020 2020 2020 666f 7220 7461  e.        for ta
-00009910: 6720 696e 2065 7272 7461 672e 6765 7443  g in errtag.getC
-00009920: 6869 6c64 7265 6e28 293a 0a20 2020 2020  hildren():.     
-00009930: 2020 2020 2020 2069 6620 2874 6167 2e67         if (tag.g
-00009940: 6574 4e61 6d65 2829 2021 3d20 2774 6578  etName() != 'tex
-00009950: 7427 2061 6e64 0a20 2020 2020 2020 2020  t' and.         
-00009960: 2020 2020 2020 2020 2020 2074 6167 2e67             tag.g
-00009970: 6574 4e61 6d65 7370 6163 6528 2920 213d  etNamespace() !=
-00009980: 204e 616d 6573 7061 6365 2e53 5441 4e5a   Namespace.STANZ
-00009990: 4153 293a 0a20 2020 2020 2020 2020 2020  AS):.           
-000099a0: 2020 2020 2072 6574 7572 6e20 7461 672e       return tag.
-000099b0: 6765 744e 616d 6528 290a 2020 2020 2020  getName().      
-000099c0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-000099d0: 2020 2064 6566 2067 6574 4170 7045 7272     def getAppErr
-000099e0: 6f72 4e61 6d65 7370 6163 6528 7365 6c66  orNamespace(self
-000099f0: 293a 0a20 2020 2020 2020 2065 7272 7461  ):.        errta
-00009a00: 6720 3d20 7365 6c66 2e67 6574 5461 6728  g = self.getTag(
-00009a10: 2765 7272 6f72 2729 0a20 2020 2020 2020  'error').       
-00009a20: 2069 6620 6572 7274 6167 2069 7320 4e6f   if errtag is No
-00009a30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00009a40: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00009a50: 2020 2020 666f 7220 7461 6720 696e 2065      for tag in e
-00009a60: 7272 7461 672e 6765 7443 6869 6c64 7265  rrtag.getChildre
-00009a70: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-00009a80: 2069 6620 2874 6167 2e67 6574 4e61 6d65   if (tag.getName
-00009a90: 2829 2021 3d20 2774 6578 7427 2061 6e64  () != 'text' and
-00009aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ab0: 2020 2020 2074 6167 2e67 6574 4e61 6d65       tag.getName
-00009ac0: 7370 6163 6528 2920 213d 204e 616d 6573  space() != Names
-00009ad0: 7061 6365 2e53 5441 4e5a 4153 293a 0a20  pace.STANZAS):. 
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009af0: 6574 7572 6e20 7461 672e 6765 744e 616d  eturn tag.getNam
-00009b00: 6573 7061 6365 2829 0a20 2020 2020 2020  espace().       
-00009b10: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00009b20: 2020 6465 6620 6765 7445 7272 6f72 4d73    def getErrorMs
-00009b30: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-00009b40: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-00009b50: 7572 6e20 7468 6520 7465 7874 7561 6c20  urn the textual 
-00009b60: 6465 7363 7269 7074 696f 6e20 6f66 2074  description of t
-00009b70: 6865 2065 7272 6f72 2028 6966 2070 7265  he error (if pre
-00009b80: 7365 6e74 290a 2020 2020 2020 2020 6f72  sent).        or
-00009b90: 2074 6865 2065 7272 6f72 2063 6f6e 6469   the error condi
-00009ba0: 7469 6f6e 0a20 2020 2020 2020 2022 2222  tion.        """
-00009bb0: 0a20 2020 2020 2020 2065 7272 7461 6720  .        errtag 
-00009bc0: 3d20 7365 6c66 2e67 6574 5461 6728 2765  = self.getTag('e
-00009bd0: 7272 6f72 2729 0a20 2020 2020 2020 2069  rror').        i
-00009be0: 6620 6572 7274 6167 3a0a 2020 2020 2020  f errtag:.      
-00009bf0: 2020 2020 2020 666f 7220 7461 6720 696e        for tag in
-00009c00: 2065 7272 7461 672e 6765 7443 6869 6c64   errtag.getChild
-00009c10: 7265 6e28 293a 0a20 2020 2020 2020 2020  ren():.         
-00009c20: 2020 2020 2020 2069 6620 7461 672e 6765         if tag.ge
-00009c30: 744e 616d 6528 2920 3d3d 2027 7465 7874  tName() == 'text
-00009c40: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00009c50: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
-00009c60: 672e 6765 7444 6174 6128 290a 2020 2020  g.getData().    
-00009c70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00009c80: 656c 662e 6765 7445 7272 6f72 2829 0a20  elf.getError(). 
-00009c90: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00009ca0: 6e65 0a0a 2020 2020 6465 6620 6765 7445  ne..    def getE
-00009cb0: 7272 6f72 436f 6465 2873 656c 6629 3a0a  rrorCode(self):.
-00009cc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009cd0: 2020 2020 5265 7475 726e 2074 6865 2065      Return the e
-00009ce0: 7272 6f72 2063 6f64 652e 204f 6273 6f6c  rror code. Obsol
-00009cf0: 6574 652e 0a20 2020 2020 2020 2022 2222  ete..        """
-00009d00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009d10: 7365 6c66 2e67 6574 5461 6741 7474 7228  self.getTagAttr(
-00009d20: 2765 7272 6f72 272c 2027 636f 6465 2729  'error', 'code')
-00009d30: 0a0a 2020 2020 6465 6620 6765 7445 7272  ..    def getErr
-00009d40: 6f72 5479 7065 2873 656c 6629 3a0a 2020  orType(self):.  
-00009d50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00009d60: 2020 5265 7475 726e 2074 6865 2065 7272    Return the err
-00009d70: 6f72 2063 6f64 652e 204f 6273 6f6c 6574  or code. Obsolet
-00009d80: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00009d90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009da0: 6c66 2e67 6574 5461 6741 7474 7228 2765  lf.getTagAttr('e
-00009db0: 7272 6f72 272c 2027 7479 7065 2729 0a0a  rror', 'type')..
-00009dc0: 2020 2020 6465 6620 6765 7453 7461 7475      def getStatu
-00009dd0: 7343 6f6e 6469 7469 6f6e 7328 7365 6c66  sConditions(self
-00009de0: 2c20 6173 5f63 6f64 653d 4661 6c73 6529  , as_code=False)
-00009df0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00009e00: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
-00009e10: 2073 7461 7475 7320 636f 6e64 6974 696f   status conditio
-00009e20: 6e73 206c 6973 7420 6173 2064 6566 696e  ns list as defin
-00009e30: 6564 2069 6e20 5845 502d 3033 3036 2e0a  ed in XEP-0306..
-00009e40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009e50: 2020 2020 7265 7375 6c74 203d 2073 6574      result = set
-00009e60: 2829 0a20 2020 2020 2020 2073 7461 7475  ().        statu
-00009e70: 735f 7461 6773 203d 2073 656c 662e 6765  s_tags = self.ge
-00009e80: 7454 6167 7328 2773 7461 7475 7327 290a  tTags('status').
-00009e90: 2020 2020 2020 2020 666f 7220 7374 6174          for stat
-00009ea0: 7573 2069 6e20 7374 6174 7573 5f74 6167  us in status_tag
-00009eb0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00009ec0: 6620 6173 5f63 6f64 653a 0a20 2020 2020  f as_code:.     
-00009ed0: 2020 2020 2020 2020 2020 2063 6f64 6520             code 
-00009ee0: 3d20 7374 6174 7573 2e67 6574 4174 7472  = status.getAttr
-00009ef0: 2827 636f 6465 2729 0a20 2020 2020 2020  ('code').       
-00009f00: 2020 2020 2020 2020 2069 6620 636f 6465           if code
-00009f10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f30: 2020 7265 7375 6c74 2e61 6464 2863 6f64    result.add(cod
-00009f40: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
-00009f50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009f60: 2020 2020 2066 6f72 2063 6f6e 6469 7469       for conditi
-00009f70: 6f6e 2069 6e20 7374 6174 7573 2e67 6574  on in status.get
-00009f80: 4368 696c 6472 656e 2829 3a0a 2020 2020  Children():.    
-00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fa0: 7265 7375 6c74 2e61 6464 2863 6f6e 6469  result.add(condi
-00009fb0: 7469 6f6e 2e67 6574 4e61 6d65 2829 290a  tion.getName()).
-00009fc0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00009fd0: 6973 7428 7265 7375 6c74 290a 0a20 2020  ist(result)..   
-00009fe0: 2064 6566 2073 6574 4572 726f 7228 7365   def setError(se
-00009ff0: 6c66 2c20 6572 726f 722c 2063 6f64 653d  lf, error, code=
-0000a000: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-0000a010: 2222 0a20 2020 2020 2020 2053 6574 2074  "".        Set t
-0000a020: 6865 2065 7272 6f72 2063 6f64 652e 204f  he error code. O
-0000a030: 6273 6f6c 6574 652e 2055 7365 2065 7272  bsolete. Use err
-0000a040: 6f72 2d63 6f6e 6469 7469 6f6e 7320 696e  or-conditions in
-0000a050: 7374 6561 640a 2020 2020 2020 2020 2222  stead.        ""
-0000a060: 220a 2020 2020 2020 2020 6966 2063 6f64  ".        if cod
-0000a070: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0000a080: 6620 7374 7228 636f 6465 2920 696e 205f  f str(code) in _
-0000a090: 6572 726f 7263 6f64 6573 2e6b 6579 7328  errorcodes.keys(
-0000a0a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000a0b0: 2020 2065 7272 6f72 203d 2045 7272 6f72     error = Error
-0000a0c0: 4e6f 6465 285f 6572 726f 7263 6f64 6573  Node(_errorcodes
-0000a0d0: 5b73 7472 2863 6f64 6529 5d2c 2074 6578  [str(code)], tex
-0000a0e0: 743d 6572 726f 7229 0a20 2020 2020 2020  t=error).       
-0000a0f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a100: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-0000a110: 203d 2045 7272 6f72 4e6f 6465 2845 5252   = ErrorNode(ERR
-0000a120: 5f55 4e44 4546 494e 4544 5f43 4f4e 4449  _UNDEFINED_CONDI
-0000a130: 5449 4f4e 2c20 636f 6465 3d63 6f64 652c  TION, code=code,
-0000a140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a160: 2020 2074 7970 3d27 6361 6e63 656c 272c     typ='cancel',
-0000a170: 2074 6578 743d 6572 726f 7229 0a20 2020   text=error).   
-0000a180: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000a190: 616e 6365 2865 7272 6f72 2c20 7374 7229  ance(error, str)
-0000a1a0: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
-0000a1b0: 726f 7220 3d20 4572 726f 724e 6f64 6528  ror = ErrorNode(
-0000a1c0: 6572 726f 7229 0a20 2020 2020 2020 2073  error).        s
-0000a1d0: 656c 662e 7365 7454 7970 6528 2765 7272  elf.setType('err
-0000a1e0: 6f72 2729 0a20 2020 2020 2020 2073 656c  or').        sel
-0000a1f0: 662e 6164 6443 6869 6c64 286e 6f64 653d  f.addChild(node=
-0000a200: 6572 726f 7229 0a0a 2020 2020 6465 6620  error)..    def 
-0000a210: 7365 7454 696d 6573 7461 6d70 2873 656c  setTimestamp(sel
-0000a220: 662c 2076 616c 3d4e 6f6e 6529 3a0a 2020  f, val=None):.  
-0000a230: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000a240: 2020 5365 7420 7468 6520 7469 6d65 7374    Set the timest
-0000a250: 616d 702e 2074 696d 6573 7461 6d70 2073  amp. timestamp s
-0000a260: 686f 756c 6420 6265 2074 6865 2079 7979  hould be the yyy
-0000a270: 796d 6d64 6454 6868 6d6d 7373 2073 7472  ymmddThhmmss str
-0000a280: 696e 670a 2020 2020 2020 2020 2222 220a  ing.        """.
-0000a290: 2020 2020 2020 2020 6966 206e 6f74 2076          if not v
-0000a2a0: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
-0000a2b0: 7661 6c20 3d20 7469 6d65 2e73 7472 6674  val = time.strft
-0000a2c0: 696d 6528 2725 5925 6d25 6454 2548 3a25  ime('%Y%m%dT%H:%
-0000a2d0: 4d3a 2553 272c 2074 696d 652e 676d 7469  M:%S', time.gmti
-0000a2e0: 6d65 2829 290a 2020 2020 2020 2020 7365  me()).        se
-0000a2f0: 6c66 2e74 696d 6573 7461 6d70 3d76 616c  lf.timestamp=val
-0000a300: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a310: 7454 6167 2827 7827 2c20 7b27 7374 616d  tTag('x', {'stam
-0000a320: 7027 3a20 7365 6c66 2e74 696d 6573 7461  p': self.timesta
-0000a330: 6d70 7d2c 206e 616d 6573 7061 6365 3d4e  mp}, namespace=N
-0000a340: 616d 6573 7061 6365 2e44 454c 4159 290a  amespace.DELAY).
-0000a350: 0a20 2020 2064 6566 2067 6574 5072 6f70  .    def getProp
-0000a360: 6572 7469 6573 2873 656c 6629 3a0a 2020  erties(self):.  
-0000a370: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000a380: 2020 5265 7475 726e 2074 6865 206c 6973    Return the lis
-0000a390: 7420 6f66 206e 616d 6573 7061 6365 7320  t of namespaces 
-0000a3a0: 746f 2077 6869 6368 2062 656c 6f6e 6773  to which belongs
-0000a3b0: 2074 6865 0a20 2020 2020 2020 2064 6972   the.        dir
-0000a3c0: 6563 7420 6368 696c 6473 206f 6620 656c  ect childs of el
-0000a3d0: 656d 656e 740a 2020 2020 2020 2020 2222  ement.        ""
-0000a3e0: 220a 2020 2020 2020 2020 7072 6f70 7320  ".        props 
-0000a3f0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-0000a400: 2063 6869 6c64 2069 6e20 7365 6c66 2e67   child in self.g
-0000a410: 6574 4368 696c 6472 656e 2829 3a0a 2020  etChildren():.  
-0000a420: 2020 2020 2020 2020 2020 7072 6f70 203d            prop =
-0000a430: 2063 6869 6c64 2e67 6574 4e61 6d65 7370   child.getNamesp
-0000a440: 6163 6528 290a 2020 2020 2020 2020 2020  ace().          
-0000a450: 2020 6966 2070 726f 7020 6e6f 7420 696e    if prop not in
-0000a460: 2070 726f 7073 3a0a 2020 2020 2020 2020   props:.        
-0000a470: 2020 2020 2020 2020 7072 6f70 732e 6170          props.ap
-0000a480: 7065 6e64 2870 726f 7029 0a20 2020 2020  pend(prop).     
-0000a490: 2020 2072 6574 7572 6e20 7072 6f70 730a     return props.
-0000a4a0: 0a20 2020 2064 6566 2067 6574 5461 6728  .    def getTag(
-0000a4b0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000a4c0: 2020 2020 206e 616d 653a 2073 7472 2c0a       name: str,.
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000a4e0: 7474 7273 3a20 4f70 7469 6f6e 616c 5b64  ttrs: Optional[d
-0000a4f0: 6963 745b 7374 722c 2041 6e79 5d5d 203d  ict[str, Any]] =
-0000a500: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0000a510: 2020 2020 2020 6e61 6d65 7370 6163 653a        namespace:
-0000a520: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000a530: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0000a540: 2020 2020 2020 7072 6f74 6f63 6f6c 3a20        protocol: 
-0000a550: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
-0000a560: 204f 7074 696f 6e61 6c5b 4e6f 6465 5d3a   Optional[Node]:
-0000a570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a580: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
-0000a590: 4e6f 6465 2069 6e73 7461 6e63 6520 666f  Node instance fo
-0000a5a0: 7220 7468 6520 7461 672e 0a20 2020 2020  r the tag..     
-0000a5b0: 2020 2049 6620 7072 6f74 6f63 6f6c 2069     If protocol i
-0000a5c0: 7320 5472 7565 2063 6f6e 7665 7274 2074  s True convert t
-0000a5d0: 6f20 6120 6e65 7720 5072 6f74 6f63 6f6c  o a new Protocol
-0000a5e0: 2f4d 6573 7361 6765 2069 6e73 7461 6e63  /Message instanc
-0000a5f0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-0000a600: 2020 2020 2020 2074 6167 203d 204e 6f64         tag = Nod
-0000a610: 652e 6765 7454 6167 2873 656c 662c 206e  e.getTag(self, n
-0000a620: 616d 652c 2061 7474 7273 2c20 6e61 6d65  ame, attrs, name
-0000a630: 7370 6163 6529 0a20 2020 2020 2020 2069  space).        i
-0000a640: 6620 7072 6f74 6f63 6f6c 2061 6e64 2074  f protocol and t
-0000a650: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
-0000a660: 6966 206e 616d 6520 3d3d 2027 6d65 7373  if name == 'mess
-0000a670: 6167 6527 3a0a 2020 2020 2020 2020 2020  age':.          
-0000a680: 2020 2020 2020 7265 7475 726e 204d 6573        return Mes
-0000a690: 7361 6765 286e 6f64 653d 7461 6729 0a20  sage(node=tag). 
-0000a6a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a6b0: 6e20 5072 6f74 6f63 6f6c 286e 6f64 653d  n Protocol(node=
-0000a6c0: 7461 6729 0a20 2020 2020 2020 2072 6574  tag).        ret
-0000a6d0: 7572 6e20 7461 670a 0a20 2020 2064 6566  urn tag..    def
-0000a6e0: 205f 5f73 6574 6974 656d 5f5f 2873 656c   __setitem__(sel
-0000a6f0: 662c 2069 7465 6d3a 2073 7472 2c20 7661  f, item: str, va
-0000a700: 6c3a 2055 6e69 6f6e 5b73 7472 2c20 4a49  l: Union[str, JI
-0000a710: 445d 293a 0a20 2020 2020 2020 2022 2222  D]):.        """
-0000a720: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
-0000a730: 2069 7465 6d20 2769 7465 6d27 2074 6f20   item 'item' to 
-0000a740: 7468 6520 7661 6c75 6520 2776 616c 270a  the value 'val'.
-0000a750: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000a760: 2020 2020 6966 2069 7465 6d20 696e 205b      if item in [
-0000a770: 2774 6f27 2c20 2766 726f 6d27 5d3a 0a20  'to', 'from']:. 
-0000a780: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000a790: 7420 6973 696e 7374 616e 6365 2876 616c  t isinstance(val
-0000a7a0: 2c20 4a49 4429 3a0a 2020 2020 2020 2020  , JID):.        
-0000a7b0: 2020 2020 2020 2020 7661 6c20 3d20 4a49          val = JI
-0000a7c0: 442e 6672 6f6d 5f73 7472 696e 6728 7661  D.from_string(va
-0000a7d0: 6c29 0a20 2020 2020 2020 2073 656c 662e  l).        self.
-0000a7e0: 7365 7441 7474 7228 6974 656d 2c20 7661  setAttr(item, va
-0000a7f0: 6c29 0a0a 0a63 6c61 7373 204d 6573 7361  l)...class Messa
-0000a800: 6765 2850 726f 746f 636f 6c29 3a0a 2020  ge(Protocol):.  
-0000a810: 2020 2222 220a 2020 2020 584d 5050 204d    """.    XMPP M
-0000a820: 6573 7361 6765 2073 7461 6e7a 6120 2d20  essage stanza - 
-0000a830: 2270 7573 6822 206d 6563 6861 6e69 736d  "push" mechanism
-0000a840: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-0000a850: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0000a860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a870: 2020 746f 3d4e 6f6e 652c 0a20 2020 2020    to=None,.     
-0000a880: 2020 2020 2020 2020 2020 2020 626f 6479              body
-0000a890: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-0000a8a0: 2020 2020 2020 2020 7868 746d 6c3d 4e6f          xhtml=No
-0000a8b0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000a8c0: 2020 2020 2074 7970 3d4e 6f6e 652c 0a20       typ=None,. 
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 7375 626a 6563 743d 4e6f 6e65 2c0a 2020  subject=None,.  
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000a900: 7474 7273 3d4e 6f6e 652c 0a20 2020 2020  ttrs=None,.     
-0000a910: 2020 2020 2020 2020 2020 2020 6672 6d3d              frm=
-0000a920: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000a930: 2020 2020 2020 2070 6179 6c6f 6164 3d4e         payload=N
-0000a940: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000a950: 2020 2020 2020 7469 6d65 7374 616d 703d        timestamp=
-0000a960: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000a970: 2020 2020 2020 2078 6d6c 6e73 3d4e 616d         xmlns=Nam
-0000a980: 6573 7061 6365 2e43 4c49 454e 542c 0a20  espace.CLIENT,. 
-0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9a0: 6e6f 6465 3d4e 6f6e 6529 3a0a 2020 2020  node=None):.    
-0000a9b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a9c0: 596f 7520 6361 6e20 7370 6563 6966 7920  You can specify 
-0000a9d0: 7265 6369 7069 656e 742c 2074 6578 7420  recipient, text 
-0000a9e0: 6f66 206d 6573 7361 6765 2c20 7479 7065  of message, type
-0000a9f0: 206f 6620 6d65 7373 6167 6520 616e 790a   of message any.
-0000aa00: 2020 2020 2020 2020 6164 6469 7469 6f6e          addition
-0000aa10: 616c 2061 7474 7269 6275 7465 732c 2073  al attributes, s
-0000aa20: 656e 6465 7220 6f66 2074 6865 206d 6573  ender of the mes
-0000aa30: 7361 6765 2c20 616e 7920 6164 6469 7469  sage, any additi
-0000aa40: 6f6e 616c 2070 6179 6c6f 6164 0a20 2020  onal payload.   
-0000aa50: 2020 2020 2028 662e 652e 206a 6162 6265       (f.e. jabbe
-0000aa60: 723a 783a 6465 6c61 7920 656c 656d 656e  r:x:delay elemen
-0000aa70: 7429 2061 6e64 206e 616d 6573 7061 6365  t) and namespace
-0000aa80: 2069 6e20 6f6e 6520 676f 2e0a 0a20 2020   in one go...   
-0000aa90: 2020 2020 2041 6c74 6572 6e61 7469 7665       Alternative
-0000aaa0: 6c79 2079 6f75 2063 616e 2070 6173 7320  ly you can pass 
-0000aab0: 696e 2074 6865 206f 7468 6572 2058 4d4c  in the other XML
-0000aac0: 206f 626a 6563 7420 6173 2074 6865 2027   object as the '
-0000aad0: 6e6f 6465 270a 2020 2020 2020 2020 7061  node'.        pa
-0000aae0: 7261 6d65 7465 6420 746f 2072 6570 6c69  rameted to repli
-0000aaf0: 6361 7465 2069 7420 6173 206d 6573 7361  cate it as messa
-0000ab00: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
-0000ab10: 2020 2020 2020 2050 726f 746f 636f 6c2e         Protocol.
-0000ab20: 5f5f 696e 6974 5f5f 2873 656c 662c 0a20  __init__(self,. 
-0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2020 2020 2020 2027 6d65 7373 6167           'messag
-0000ab50: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-0000ab60: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000ab70: 3d74 6f2c 0a20 2020 2020 2020 2020 2020  =to,.           
-0000ab80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ab90: 7970 3d74 7970 2c0a 2020 2020 2020 2020  yp=typ,.        
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 6174 7472 733d 6174 7472 732c 0a20    attrs=attrs,. 
-0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 2020 2066 726d 3d66 726d           frm=frm
-0000abe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000abf0: 2020 2020 2020 2020 2020 2020 7061 796c              payl
-0000ac00: 6f61 643d 7061 796c 6f61 642c 0a20 2020  oad=payload,.   
+000003e0: 730a 696d 706f 7274 2073 716c 6974 6533  s.import sqlite3
+000003f0: 0a69 6d70 6f72 7420 7761 726e 696e 6773  .import warnings
+00000400: 0a66 726f 6d20 6261 7365 3634 2069 6d70  .from base64 imp
+00000410: 6f72 7420 6236 3465 6e63 6f64 650a 6672  ort b64encode.fr
+00000420: 6f6d 2064 6174 6163 6c61 7373 6573 2069  om dataclasses i
+00000430: 6d70 6f72 7420 6461 7461 636c 6173 730a  mport dataclass.
+00000440: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
+00000450: 2069 6d70 6f72 7420 6173 6469 6374 0a0a   import asdict..
+00000460: 6672 6f6d 2067 692e 7265 706f 7369 746f  from gi.reposito
+00000470: 7279 2069 6d70 6f72 7420 474c 6962 0a0a  ry import GLib..
+00000480: 696d 706f 7274 2069 646e 610a 6672 6f6d  import idna.from
+00000490: 206e 6278 6d70 702e 786d 7070 6972 6920   nbxmpp.xmppiri 
+000004a0: 696d 706f 7274 2065 7363 6170 655f 6966  import escape_if
+000004b0: 7261 676d 656e 740a 6672 6f6d 206e 6278  ragment.from nbx
+000004c0: 6d70 702e 786d 7070 6972 6920 696d 706f  mpp.xmppiri impo
+000004d0: 7274 2065 7363 6170 655f 696e 6f64 650a  rt escape_inode.
+000004e0: 6672 6f6d 206e 6278 6d70 702e 786d 7070  from nbxmpp.xmpp
+000004f0: 6972 6920 696d 706f 7274 2065 7363 6170  iri import escap
+00000500: 655f 6972 6573 0a66 726f 6d20 6e62 786d  e_ires.from nbxm
+00000510: 7070 2e78 6d70 7069 7269 2069 6d70 6f72  pp.xmppiri impor
+00000520: 7420 6573 6361 7065 5f69 7661 6c75 650a  t escape_ivalue.
+00000530: 6672 6f6d 206e 6278 6d70 702e 786d 7070  from nbxmpp.xmpp
+00000540: 6972 6920 696d 706f 7274 2076 616c 6964  iri import valid
+00000550: 6174 655f 696b 6579 0a66 726f 6d20 6e62  ate_ikey.from nb
+00000560: 786d 7070 2e78 6d70 7069 7269 2069 6d70  xmpp.xmppiri imp
+00000570: 6f72 7420 7661 6c69 6461 7465 5f71 7565  ort validate_que
+00000580: 7279 7479 7065 0a66 726f 6d20 6e62 786d  rytype.from nbxm
+00000590: 7070 2e73 696d 706c 6578 6d6c 2069 6d70  pp.simplexml imp
+000005a0: 6f72 7420 4e6f 6465 0a66 726f 6d20 6e62  ort Node.from nb
+000005b0: 786d 7070 2e6e 616d 6573 7061 6365 7320  xmpp.namespaces 
+000005c0: 696d 706f 7274 204e 616d 6573 7061 6365  import Namespace
+000005d0: 0a66 726f 6d20 6e62 786d 7070 2e73 7472  .from nbxmpp.str
+000005e0: 696e 6770 7265 7020 696d 706f 7274 206e  ingprep import n
+000005f0: 6f64 6570 7265 700a 6672 6f6d 206e 6278  odeprep.from nbx
+00000600: 6d70 702e 7374 7269 6e67 7072 6570 2069  mpp.stringprep i
+00000610: 6d70 6f72 7420 7265 736f 7572 6365 7072  mport resourcepr
+00000620: 6570 0a66 726f 6d20 6e62 786d 7070 2e70  ep.from nbxmpp.p
+00000630: 7265 6369 7320 696d 706f 7274 2065 6e66  recis import enf
+00000640: 6f72 6365 5f70 7265 6369 735f 7573 6572  orce_precis_user
+00000650: 6e61 6d65 0a66 726f 6d20 6e62 786d 7070  name.from nbxmpp
+00000660: 2e70 7265 6369 7320 696d 706f 7274 2065  .precis import e
+00000670: 6e66 6f72 6365 5f70 7265 6369 735f 6f70  nforce_precis_op
+00000680: 6171 7565 0a0a 0a64 6566 2061 7363 6969  aque...def ascii
+00000690: 5f75 7070 6572 2873 293a 0a20 2020 2072  _upper(s):.    r
+000006a0: 6574 7572 6e20 732e 7570 7065 7228 290a  eturn s.upper().
+000006b0: 0a0a 5341 534c 5f41 5554 485f 4d45 4348  ..SASL_AUTH_MECH
+000006c0: 5320 3d20 5b0a 2020 2020 2753 4352 414d  S = [.    'SCRAM
+000006d0: 2d53 4841 2d35 3132 2d50 4c55 5327 2c0a  -SHA-512-PLUS',.
+000006e0: 2020 2020 2753 4352 414d 2d53 4841 2d35      'SCRAM-SHA-5
+000006f0: 3132 272c 0a20 2020 2027 5343 5241 4d2d  12',.    'SCRAM-
+00000700: 5348 412d 3235 362d 504c 5553 272c 0a20  SHA-256-PLUS',. 
+00000710: 2020 2027 5343 5241 4d2d 5348 412d 3235     'SCRAM-SHA-25
+00000720: 3627 2c0a 2020 2020 2753 4352 414d 2d53  6',.    'SCRAM-S
+00000730: 4841 2d31 2d50 4c55 5327 2c0a 2020 2020  HA-1-PLUS',.    
+00000740: 2753 4352 414d 2d53 4841 2d31 272c 0a20  'SCRAM-SHA-1',. 
+00000750: 2020 2027 4753 5341 5049 272c 0a20 2020     'GSSAPI',.   
+00000760: 2027 504c 4149 4e27 2c0a 2020 2020 2745   'PLAIN',.    'E
+00000770: 5854 4552 4e41 4c27 2c0a 2020 2020 2741  XTERNAL',.    'A
+00000780: 4e4f 4e59 4d4f 5553 272c 0a5d 0a0a 5341  NONYMOUS',.]..SA
+00000790: 534c 5f45 5252 4f52 5f43 4f4e 4449 5449  SL_ERROR_CONDITI
+000007a0: 4f4e 5320 3d20 5b0a 2020 2020 2761 626f  ONS = [.    'abo
+000007b0: 7274 6564 272c 0a20 2020 2027 6163 636f  rted',.    'acco
+000007c0: 756e 742d 6469 7361 626c 6564 272c 0a20  unt-disabled',. 
+000007d0: 2020 2027 6372 6564 656e 7469 616c 732d     'credentials-
+000007e0: 6578 7069 7265 6427 2c0a 2020 2020 2765  expired',.    'e
+000007f0: 6e63 7279 7074 696f 6e2d 7265 7175 6972  ncryption-requir
+00000800: 6564 272c 0a20 2020 2027 696e 636f 7272  ed',.    'incorr
+00000810: 6563 742d 656e 636f 6469 6e67 272c 0a20  ect-encoding',. 
+00000820: 2020 2027 696e 7661 6c69 642d 6175 7468     'invalid-auth
+00000830: 7a69 6427 2c0a 2020 2020 2769 6e76 616c  zid',.    'inval
+00000840: 6964 2d6d 6563 6861 6e69 736d 272c 0a20  id-mechanism',. 
+00000850: 2020 2027 6d65 6368 616e 6973 6d2d 746f     'mechanism-to
+00000860: 6f2d 7765 616b 272c 0a20 2020 2027 6d61  o-weak',.    'ma
+00000870: 6c66 6f72 6d65 642d 7265 7175 6573 7427  lformed-request'
+00000880: 2c0a 2020 2020 276e 6f74 2d61 7574 686f  ,.    'not-autho
+00000890: 7269 7a65 6427 2c0a 2020 2020 2774 656d  rized',.    'tem
+000008a0: 706f 7261 7279 2d61 7574 682d 6661 696c  porary-auth-fail
+000008b0: 7572 6527 2c0a 5d0a 0a45 5252 4f52 5320  ure',.]..ERRORS 
+000008c0: 3d20 7b0a 2020 2020 2775 726e 3a69 6574  = {.    'urn:iet
+000008d0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+000008e0: 786d 7070 2d73 6173 6c20 6162 6f72 7465  xmpp-sasl aborte
+000008f0: 6427 3a20 5b27 272c 0a20 2020 2020 2020  d': ['',.       
+00000900: 2027 272c 0a20 2020 2020 2020 2027 5468   '',.        'Th
+00000910: 6520 7265 6365 6976 696e 6720 656e 7469  e receiving enti
+00000920: 7479 2061 636b 6e6f 776c 6564 6765 7320  ty acknowledges 
+00000930: 616e 203c 6162 6f72 742f 3e20 656c 656d  an <abort/> elem
+00000940: 656e 7420 7365 6e74 2062 7920 7468 6520  ent sent by the 
+00000950: 696e 6974 6961 7469 6e67 2065 6e74 6974  initiating entit
+00000960: 793b 2073 656e 7420 696e 2072 6570 6c79  y; sent in reply
+00000970: 2074 6f20 7468 6520 3c61 626f 7274 2f3e   to the <abort/>
+00000980: 2065 6c65 6d65 6e74 2e27 5d2c 0a20 2020   element.'],.   
+00000990: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
+000009a0: 733a 786d 6c3a 6e73 3a78 6d70 702d 7361  s:xml:ns:xmpp-sa
+000009b0: 736c 2069 6e63 6f72 7265 6374 2d65 6e63  sl incorrect-enc
+000009c0: 6f64 696e 6727 3a20 5b27 272c 0a20 2020  oding': ['',.   
+000009d0: 2020 2020 2027 272c 0a20 2020 2020 2020       '',.       
+000009e0: 2027 5468 6520 6461 7461 2070 726f 7669   'The data provi
+000009f0: 6465 6420 6279 2074 6865 2069 6e69 7469  ded by the initi
+00000a00: 6174 696e 6720 656e 7469 7479 2063 6f75  ating entity cou
+00000a10: 6c64 206e 6f74 2062 6520 7072 6f63 6573  ld not be proces
+00000a20: 7365 6420 6265 6361 7573 6520 7468 6520  sed because the 
+00000a30: 5b42 4153 4536 345d 4a6f 7365 6673 736f  [BASE64]Josefsso
+00000a40: 6e2c 2053 2e2c 2054 6865 2042 6173 6531  n, S., The Base1
+00000a50: 362c 2042 6173 6533 322c 2061 6e64 2042  6, Base32, and B
+00000a60: 6173 6536 3420 4461 7461 2045 6e63 6f64  ase64 Data Encod
+00000a70: 696e 6773 2c20 4a75 6c79 2032 3030 332e  ings, July 2003.
+00000a80: 2065 6e63 6f64 696e 6720 6973 2069 6e63   encoding is inc
+00000a90: 6f72 7265 6374 2028 652e 672e 2c20 6265  orrect (e.g., be
+00000aa0: 6361 7573 6520 7468 6520 656e 636f 6469  cause the encodi
+00000ab0: 6e67 2064 6f65 7320 6e6f 7420 6164 6865  ng does not adhe
+00000ac0: 7265 2074 6f20 7468 6520 6465 6669 6e69  re to the defini
+00000ad0: 7469 6f6e 2069 6e20 5365 6374 696f 6e20  tion in Section 
+00000ae0: 3320 6f66 205b 4241 5345 3634 5d4a 6f73  3 of [BASE64]Jos
+00000af0: 6566 7373 6f6e 2c20 532e 2c20 5468 6520  efsson, S., The 
+00000b00: 4261 7365 3136 2c20 4261 7365 3332 2c20  Base16, Base32, 
+00000b10: 616e 6420 4261 7365 3634 2044 6174 6120  and Base64 Data 
+00000b20: 456e 636f 6469 6e67 732c 204a 756c 7920  Encodings, July 
+00000b30: 3230 3033 2e29 3b20 7365 6e74 2069 6e20  2003.); sent in 
+00000b40: 7265 706c 7920 746f 2061 203c 7265 7370  reply to a <resp
+00000b50: 6f6e 7365 2f3e 2065 6c65 6d65 6e74 206f  onse/> element o
+00000b60: 7220 616e 203c 6175 7468 2f3e 2065 6c65  r an <auth/> ele
+00000b70: 6d65 6e74 2077 6974 6820 696e 6974 6961  ment with initia
+00000b80: 6c20 7265 7370 6f6e 7365 2064 6174 612e  l response data.
+00000b90: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+00000ba0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00000bb0: 786d 7070 2d73 6173 6c20 696e 7661 6c69  xmpp-sasl invali
+00000bc0: 642d 6175 7468 7a69 6427 3a20 5b27 272c  d-authzid': ['',
+00000bd0: 0a20 2020 2020 2020 2027 272c 0a20 2020  .        '',.   
+00000be0: 2020 2020 2027 5468 6520 6175 7468 7a69       'The authzi
+00000bf0: 6420 7072 6f76 6964 6564 2062 7920 7468  d provided by th
+00000c00: 6520 696e 6974 6961 7469 6e67 2065 6e74  e initiating ent
+00000c10: 6974 7920 6973 2069 6e76 616c 6964 2c20  ity is invalid, 
+00000c20: 6569 7468 6572 2062 6563 6175 7365 2069  either because i
+00000c30: 7420 6973 2069 6e63 6f72 7265 6374 6c79  t is incorrectly
+00000c40: 2066 6f72 6d61 7474 6564 206f 7220 6265   formatted or be
+00000c50: 6361 7573 6520 7468 6520 696e 6974 6961  cause the initia
+00000c60: 7469 6e67 2065 6e74 6974 7920 646f 6573  ting entity does
+00000c70: 206e 6f74 2068 6176 6520 7065 726d 6973   not have permis
+00000c80: 7369 6f6e 7320 746f 2061 7574 686f 7269  sions to authori
+00000c90: 7a65 2074 6861 7420 4944 3b20 7365 6e74  ze that ID; sent
+00000ca0: 2069 6e20 7265 706c 7920 746f 2061 203c   in reply to a <
+00000cb0: 7265 7370 6f6e 7365 2f3e 2065 6c65 6d65  response/> eleme
+00000cc0: 6e74 206f 7220 616e 203c 6175 7468 2f3e  nt or an <auth/>
+00000cd0: 2065 6c65 6d65 6e74 2077 6974 6820 696e   element with in
+00000ce0: 6974 6961 6c20 7265 7370 6f6e 7365 2064  itial response d
+00000cf0: 6174 612e 275d 2c0a 2020 2020 2775 726e  ata.'],.    'urn
+00000d00: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
+00000d10: 3a6e 733a 786d 7070 2d73 6173 6c20 696e  :ns:xmpp-sasl in
+00000d20: 7661 6c69 642d 6d65 6368 616e 6973 6d27  valid-mechanism'
+00000d30: 3a20 5b27 272c 0a20 2020 2020 2020 2027  : ['',.        '
+00000d40: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
+00000d50: 696e 6974 6961 7469 6e67 2065 6e74 6974  initiating entit
+00000d60: 7920 6469 6420 6e6f 7420 7072 6f76 6964  y did not provid
+00000d70: 6520 6120 6d65 6368 616e 6973 6d20 6f72  e a mechanism or
+00000d80: 2072 6571 7565 7374 6564 2061 206d 6563   requested a mec
+00000d90: 6861 6e69 736d 2074 6861 7420 6973 206e  hanism that is n
+00000da0: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
+00000db0: 7468 6520 7265 6365 6976 696e 6720 656e  the receiving en
+00000dc0: 7469 7479 3b20 7365 6e74 2069 6e20 7265  tity; sent in re
+00000dd0: 706c 7920 746f 2061 6e20 3c61 7574 682f  ply to an <auth/
+00000de0: 3e20 656c 656d 656e 742e 275d 2c0a 2020  > element.'],.  
+00000df0: 2020 2775 726e 3a69 6574 663a 7061 7261    'urn:ietf:para
+00000e00: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00000e10: 6173 6c20 6d65 6368 616e 6973 6d2d 746f  asl mechanism-to
+00000e20: 6f2d 7765 616b 273a 205b 2727 2c0a 2020  o-weak': ['',.  
+00000e30: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
+00000e40: 2020 2754 6865 206d 6563 6861 6e69 736d    'The mechanism
+00000e50: 2072 6571 7565 7374 6564 2062 7920 7468   requested by th
+00000e60: 6520 696e 6974 6961 7469 6e67 2065 6e74  e initiating ent
+00000e70: 6974 7920 6973 2077 6561 6b65 7220 7468  ity is weaker th
+00000e80: 616e 2073 6572 7665 7220 706f 6c69 6379  an server policy
+00000e90: 2070 6572 6d69 7473 2066 6f72 2074 6861   permits for tha
+00000ea0: 7420 696e 6974 6961 7469 6e67 2065 6e74  t initiating ent
+00000eb0: 6974 793b 2073 656e 7420 696e 2072 6570  ity; sent in rep
+00000ec0: 6c79 2074 6f20 6120 3c72 6573 706f 6e73  ly to a <respons
+00000ed0: 652f 3e20 656c 656d 656e 7420 6f72 2061  e/> element or a
+00000ee0: 6e20 3c61 7574 682f 3e20 656c 656d 656e  n <auth/> elemen
+00000ef0: 7420 7769 7468 2069 6e69 7469 616c 2072  t with initial r
+00000f00: 6573 706f 6e73 6520 6461 7461 2e27 5d2c  esponse data.'],
+00000f10: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
+00000f20: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00000f30: 702d 7361 736c 206e 6f74 2d61 7574 686f  p-sasl not-autho
+00000f40: 7269 7a65 6427 3a20 5b27 272c 0a20 2020  rized': ['',.   
+00000f50: 2020 2020 2027 272c 0a20 2020 2020 2020       '',.       
+00000f60: 2027 5468 6520 6175 7468 656e 7469 6361   'The authentica
+00000f70: 7469 6f6e 2066 6169 6c65 6420 6265 6361  tion failed beca
+00000f80: 7573 6520 7468 6520 696e 6974 6961 7469  use the initiati
+00000f90: 6e67 2065 6e74 6974 7920 6469 6420 6e6f  ng entity did no
+00000fa0: 7420 7072 6f76 6964 6520 7661 6c69 6420  t provide valid 
+00000fb0: 6372 6564 656e 7469 616c 7320 2874 6869  credentials (thi
+00000fc0: 7320 696e 636c 7564 6573 2062 7574 2069  s includes but i
+00000fd0: 7320 6e6f 7420 6c69 6d69 7465 6420 746f  s not limited to
+00000fe0: 2074 6865 2063 6173 6520 6f66 2061 6e20   the case of an 
+00000ff0: 756e 6b6e 6f77 6e20 7573 6572 6e61 6d65  unknown username
+00001000: 293b 2073 656e 7420 696e 2072 6570 6c79  ); sent in reply
+00001010: 2074 6f20 6120 3c72 6573 706f 6e73 652f   to a <response/
+00001020: 3e20 656c 656d 656e 7420 6f72 2061 6e20  > element or an 
+00001030: 3c61 7574 682f 3e20 656c 656d 656e 7420  <auth/> element 
+00001040: 7769 7468 2069 6e69 7469 616c 2072 6573  with initial res
+00001050: 706f 6e73 6520 6461 7461 2e27 5d2c 0a20  ponse data.'],. 
+00001060: 2020 2027 7572 6e3a 6965 7466 3a70 6172     'urn:ietf:par
+00001070: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
+00001080: 7361 736c 2074 656d 706f 7261 7279 2d61  sasl temporary-a
+00001090: 7574 682d 6661 696c 7572 6527 3a20 5b27  uth-failure': ['
+000010a0: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
+000010b0: 2020 2020 2020 2027 5468 6520 6175 7468         'The auth
+000010c0: 656e 7469 6361 7469 6f6e 2066 6169 6c65  entication faile
+000010d0: 6420 6265 6361 7573 6520 6f66 2061 2074  d because of a t
+000010e0: 656d 706f 7261 7279 2065 7272 6f72 2063  emporary error c
+000010f0: 6f6e 6469 7469 6f6e 2077 6974 6869 6e20  ondition within 
+00001100: 7468 6520 7265 6365 6976 696e 6720 656e  the receiving en
+00001110: 7469 7479 3b20 7365 6e74 2069 6e20 7265  tity; sent in re
+00001120: 706c 7920 746f 2061 6e20 3c61 7574 682f  ply to an <auth/
+00001130: 3e20 656c 656d 656e 7420 6f72 203c 7265  > element or <re
+00001140: 7370 6f6e 7365 2f3e 2065 6c65 6d65 6e74  sponse/> element
+00001150: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
+00001160: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
+00001170: 3a78 6d70 702d 7374 616e 7a61 7320 6261  :xmpp-stanzas ba
+00001180: 642d 7265 7175 6573 7427 3a20 5b27 3430  d-request': ['40
+00001190: 3027 2c0a 2020 2020 2020 2020 276d 6f64  0',.        'mod
+000011a0: 6966 7927 2c0a 2020 2020 2020 2020 2754  ify',.        'T
+000011b0: 6865 2073 656e 6465 7220 6861 7320 7365  he sender has se
+000011c0: 6e74 2058 4d4c 2074 6861 7420 6973 206d  nt XML that is m
+000011d0: 616c 666f 726d 6564 206f 7220 7468 6174  alformed or that
+000011e0: 2063 616e 6e6f 7420 6265 2070 726f 6365   cannot be proce
+000011f0: 7373 6564 2e27 5d2c 0a20 2020 2027 7572  ssed.'],.    'ur
+00001200: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
+00001210: 6c3a 6e73 3a78 6d70 702d 7374 616e 7a61  l:ns:xmpp-stanza
+00001220: 7320 636f 6e66 6c69 6374 273a 205b 2734  s conflict': ['4
+00001230: 3039 272c 0a20 2020 2020 2020 2027 6361  09',.        'ca
+00001240: 6e63 656c 272c 0a20 2020 2020 2020 2027  ncel',.        '
+00001250: 4163 6365 7373 2063 616e 6e6f 7420 6265  Access cannot be
+00001260: 2067 7261 6e74 6564 2062 6563 6175 7365   granted because
+00001270: 2061 6e20 6578 6973 7469 6e67 2072 6573   an existing res
+00001280: 6f75 7263 6520 6f72 2073 6573 7369 6f6e  ource or session
+00001290: 2065 7869 7374 7320 7769 7468 2074 6865   exists with the
+000012a0: 2073 616d 6520 6e61 6d65 206f 7220 6164   same name or ad
+000012b0: 6472 6573 732e 275d 2c0a 2020 2020 2775  dress.'],.    'u
+000012c0: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+000012d0: 6d6c 3a6e 733a 786d 7070 2d73 7461 6e7a  ml:ns:xmpp-stanz
+000012e0: 6173 2066 6561 7475 7265 2d6e 6f74 2d69  as feature-not-i
+000012f0: 6d70 6c65 6d65 6e74 6564 273a 205b 2735  mplemented': ['5
+00001300: 3031 272c 0a20 2020 2020 2020 2027 6361  01',.        'ca
+00001310: 6e63 656c 272c 0a20 2020 2020 2020 2027  ncel',.        '
+00001320: 5468 6520 6665 6174 7572 6520 7265 7175  The feature requ
+00001330: 6573 7465 6420 6973 206e 6f74 2069 6d70  ested is not imp
+00001340: 6c65 6d65 6e74 6564 2062 7920 7468 6520  lemented by the 
+00001350: 7265 6369 7069 656e 7420 6f72 2073 6572  recipient or ser
+00001360: 7665 7220 616e 6420 7468 6572 6566 6f72  ver and therefor
+00001370: 6520 6361 6e6e 6f74 2062 6520 7072 6f63  e cannot be proc
+00001380: 6573 7365 642e 275d 2c0a 2020 2020 2775  essed.'],.    'u
+00001390: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+000013a0: 6d6c 3a6e 733a 786d 7070 2d73 7461 6e7a  ml:ns:xmpp-stanz
+000013b0: 6173 2066 6f72 6269 6464 656e 273a 205b  as forbidden': [
+000013c0: 2734 3033 272c 0a20 2020 2020 2020 2027  '403',.        '
+000013d0: 6175 7468 272c 0a20 2020 2020 2020 2027  auth',.        '
+000013e0: 5468 6520 7265 7175 6573 7469 6e67 2065  The requesting e
+000013f0: 6e74 6974 7920 646f 6573 206e 6f74 2070  ntity does not p
+00001400: 6f73 7365 7373 2074 6865 2072 6571 7569  ossess the requi
+00001410: 7265 6420 7065 726d 6973 7369 6f6e 7320  red permissions 
+00001420: 746f 2070 6572 666f 726d 2074 6865 2061  to perform the a
+00001430: 6374 696f 6e2e 275d 2c0a 2020 2020 2775  ction.'],.    'u
+00001440: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00001450: 6d6c 3a6e 733a 786d 7070 2d73 7461 6e7a  ml:ns:xmpp-stanz
+00001460: 6173 2067 6f6e 6527 3a20 5b27 3330 3227  as gone': ['302'
+00001470: 2c0a 2020 2020 2020 2020 276d 6f64 6966  ,.        'modif
+00001480: 7927 2c0a 2020 2020 2020 2020 2754 6865  y',.        'The
+00001490: 2072 6563 6970 6965 6e74 206f 7220 7365   recipient or se
+000014a0: 7276 6572 2063 616e 206e 6f20 6c6f 6e67  rver can no long
+000014b0: 6572 2062 6520 636f 6e74 6163 7465 6420  er be contacted 
+000014c0: 6174 2074 6869 7320 6164 6472 6573 732e  at this address.
+000014d0: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+000014e0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+000014f0: 786d 7070 2d73 7461 6e7a 6173 2069 6e74  xmpp-stanzas int
+00001500: 6572 6e61 6c2d 7365 7276 6572 2d65 7272  ernal-server-err
+00001510: 6f72 273a 205b 2735 3030 272c 0a20 2020  or': ['500',.   
+00001520: 2020 2020 2027 7761 6974 272c 0a20 2020       'wait',.   
+00001530: 2020 2020 2027 5468 6520 7365 7276 6572       'The server
+00001540: 2063 6f75 6c64 206e 6f74 2070 726f 6365   could not proce
+00001550: 7373 2074 6865 2073 7461 6e7a 6120 6265  ss the stanza be
+00001560: 6361 7573 6520 6f66 2061 206d 6973 636f  cause of a misco
+00001570: 6e66 6967 7572 6174 696f 6e20 6f72 2061  nfiguration or a
+00001580: 6e20 6f74 6865 7277 6973 652d 756e 6465  n otherwise-unde
+00001590: 6669 6e65 6420 696e 7465 726e 616c 2073  fined internal s
+000015a0: 6572 7665 7220 6572 726f 722e 275d 2c0a  erver error.'],.
+000015b0: 2020 2020 2775 726e 3a69 6574 663a 7061      'urn:ietf:pa
+000015c0: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
+000015d0: 2d73 7461 6e7a 6173 2069 7465 6d2d 6e6f  -stanzas item-no
+000015e0: 742d 666f 756e 6427 3a20 5b27 3430 3427  t-found': ['404'
+000015f0: 2c0a 2020 2020 2020 2020 2763 616e 6365  ,.        'cance
+00001600: 6c27 2c0a 2020 2020 2020 2020 2754 6865  l',.        'The
+00001610: 2061 6464 7265 7373 6564 204a 4944 206f   addressed JID o
+00001620: 7220 6974 656d 2072 6571 7565 7374 6564  r item requested
+00001630: 2063 616e 6e6f 7420 6265 2066 6f75 6e64   cannot be found
+00001640: 2e27 5d2c 0a20 2020 2027 7572 6e3a 6965  .'],.    'urn:ie
+00001650: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
+00001660: 3a78 6d70 702d 7374 616e 7a61 7320 6a69  :xmpp-stanzas ji
+00001670: 642d 6d61 6c66 6f72 6d65 6427 3a20 5b27  d-malformed': ['
+00001680: 3430 3027 2c0a 2020 2020 2020 2020 276d  400',.        'm
+00001690: 6f64 6966 7927 2c0a 2020 2020 2020 2020  odify',.        
+000016a0: 2254 6865 2076 616c 7565 206f 6620 7468  "The value of th
+000016b0: 6520 2020 2020 2020 2027 746f 2720 6174  e        'to' at
+000016c0: 7472 6962 7574 6520 696e 2074 6865 2073  tribute in the s
+000016d0: 656e 6465 7227 7320 7374 616e 7a61 2064  ender's stanza d
+000016e0: 6f65 7320 6e6f 7420 6164 6865 7265 2074  oes not adhere t
+000016f0: 6f20 7468 6520 7379 6e74 6178 2064 6566  o the syntax def
+00001700: 696e 6564 2069 6e20 4164 6472 6573 7369  ined in Addressi
+00001710: 6e67 2053 6368 656d 652e 225d 2c0a 2020  ng Scheme."],.  
+00001720: 2020 2775 726e 3a69 6574 663a 7061 7261    'urn:ietf:para
+00001730: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00001740: 7461 6e7a 6173 206e 6f74 2d61 6363 6570  tanzas not-accep
+00001750: 7461 626c 6527 3a20 5b27 3430 3627 2c0a  table': ['406',.
+00001760: 2020 2020 2020 2020 2763 616e 6365 6c27          'cancel'
+00001770: 2c0a 2020 2020 2020 2020 2754 6865 2072  ,.        'The r
+00001780: 6563 6970 6965 6e74 206f 7220 7365 7276  ecipient or serv
+00001790: 6572 2075 6e64 6572 7374 616e 6473 2074  er understands t
+000017a0: 6865 2072 6571 7565 7374 2062 7574 2069  he request but i
+000017b0: 7320 7265 6675 7369 6e67 2074 6f20 7072  s refusing to pr
+000017c0: 6f63 6573 7320 6974 2062 6563 6175 7365  ocess it because
+000017d0: 2069 7420 646f 6573 206e 6f74 206d 6565   it does not mee
+000017e0: 7420 6372 6974 6572 6961 2064 6566 696e  t criteria defin
+000017f0: 6564 2062 7920 7468 6520 7265 6369 7069  ed by the recipi
+00001800: 656e 7420 6f72 2073 6572 7665 722e 275d  ent or server.']
+00001810: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
+00001820: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00001830: 7070 2d73 7461 6e7a 6173 206e 6f74 2d61  pp-stanzas not-a
+00001840: 6c6c 6f77 6564 273a 205b 2734 3035 272c  llowed': ['405',
+00001850: 0a20 2020 2020 2020 2027 6361 6e63 656c  .        'cancel
+00001860: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
+00001870: 7265 6369 7069 656e 7420 6f72 2073 6572  recipient or ser
+00001880: 7665 7220 646f 6573 206e 6f74 2061 6c6c  ver does not all
+00001890: 6f77 2061 6e79 2065 6e74 6974 7920 746f  ow any entity to
+000018a0: 2070 6572 666f 726d 2074 6865 2061 6374   perform the act
+000018b0: 696f 6e2e 275d 2c0a 2020 2020 2775 726e  ion.'],.    'urn
+000018c0: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
+000018d0: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
+000018e0: 206e 6f74 2d61 7574 686f 7269 7a65 6427   not-authorized'
+000018f0: 3a20 5b27 3430 3127 2c0a 2020 2020 2020  : ['401',.      
+00001900: 2020 2761 7574 6827 2c0a 2020 2020 2020    'auth',.      
+00001910: 2020 2754 6865 2073 656e 6465 7220 6d75    'The sender mu
+00001920: 7374 2070 726f 7669 6465 2070 726f 7065  st provide prope
+00001930: 7220 6372 6564 656e 7469 616c 7320 6265  r credentials be
+00001940: 666f 7265 2062 6569 6e67 2061 6c6c 6f77  fore being allow
+00001950: 6564 2074 6f20 7065 7266 6f72 6d20 7468  ed to perform th
+00001960: 6520 6163 7469 6f6e 2c20 6f72 2068 6173  e action, or has
+00001970: 2070 726f 7669 6465 6420 696d 7072 6f70   provided improp
+00001980: 6572 2063 7265 6465 6e74 6961 6c73 2e27  er credentials.'
+00001990: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
+000019a0: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+000019b0: 6d70 702d 7374 616e 7a61 7320 7061 796d  mpp-stanzas paym
+000019c0: 656e 742d 7265 7175 6972 6564 273a 205b  ent-required': [
+000019d0: 2734 3032 272c 0a20 2020 2020 2020 2027  '402',.        '
+000019e0: 6175 7468 272c 0a20 2020 2020 2020 2027  auth',.        '
+000019f0: 5468 6520 7265 7175 6573 7469 6e67 2065  The requesting e
+00001a00: 6e74 6974 7920 6973 206e 6f74 2061 7574  ntity is not aut
+00001a10: 686f 7269 7a65 6420 746f 2061 6363 6573  horized to acces
+00001a20: 7320 7468 6520 7265 7175 6573 7465 6420  s the requested 
+00001a30: 7365 7276 6963 6520 6265 6361 7573 6520  service because 
+00001a40: 7061 796d 656e 7420 6973 2072 6571 7569  payment is requi
+00001a50: 7265 642e 275d 2c0a 2020 2020 2775 726e  red.'],.    'urn
+00001a60: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
+00001a70: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
+00001a80: 2072 6563 6970 6965 6e74 2d75 6e61 7661   recipient-unava
+00001a90: 696c 6162 6c65 273a 205b 2734 3034 272c  ilable': ['404',
+00001aa0: 0a20 2020 2020 2020 2027 7761 6974 272c  .        'wait',
+00001ab0: 0a20 2020 2020 2020 2027 5468 6520 696e  .        'The in
+00001ac0: 7465 6e64 6564 2072 6563 6970 6965 6e74  tended recipient
+00001ad0: 2069 7320 7465 6d70 6f72 6172 696c 7920   is temporarily 
+00001ae0: 756e 6176 6169 6c61 626c 652e 275d 2c0a  unavailable.'],.
+00001af0: 2020 2020 2775 726e 3a69 6574 663a 7061      'urn:ietf:pa
+00001b00: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
+00001b10: 2d73 7461 6e7a 6173 2072 6564 6972 6563  -stanzas redirec
+00001b20: 7427 3a20 5b27 3330 3227 2c0a 2020 2020  t': ['302',.    
+00001b30: 2020 2020 276d 6f64 6966 7927 2c0a 2020      'modify',.  
+00001b40: 2020 2020 2020 2754 6865 2072 6563 6970        'The recip
+00001b50: 6965 6e74 206f 7220 7365 7276 6572 2069  ient or server i
+00001b60: 7320 7265 6469 7265 6374 696e 6720 7265  s redirecting re
+00001b70: 7175 6573 7473 2066 6f72 2074 6869 7320  quests for this 
+00001b80: 696e 666f 726d 6174 696f 6e20 746f 2061  information to a
+00001b90: 6e6f 7468 6572 2065 6e74 6974 792e 275d  nother entity.']
+00001ba0: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
+00001bb0: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00001bc0: 7070 2d73 7461 6e7a 6173 2072 6567 6973  pp-stanzas regis
+00001bd0: 7472 6174 696f 6e2d 7265 7175 6972 6564  tration-required
+00001be0: 273a 205b 2734 3037 272c 0a20 2020 2020  ': ['407',.     
+00001bf0: 2020 2027 6175 7468 272c 0a20 2020 2020     'auth',.     
+00001c00: 2020 2027 5468 6520 7265 7175 6573 7469     'The requesti
+00001c10: 6e67 2065 6e74 6974 7920 6973 206e 6f74  ng entity is not
+00001c20: 2061 7574 686f 7269 7a65 6420 746f 2061   authorized to a
+00001c30: 6363 6573 7320 7468 6520 7265 7175 6573  ccess the reques
+00001c40: 7465 6420 7365 7276 6963 6520 6265 6361  ted service beca
+00001c50: 7573 6520 7265 6769 7374 7261 7469 6f6e  use registration
+00001c60: 2069 7320 7265 7175 6972 6564 2e27 5d2c   is required.'],
+00001c70: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
+00001c80: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00001c90: 702d 7374 616e 7a61 7320 7265 6d6f 7465  p-stanzas remote
+00001ca0: 2d73 6572 7665 722d 6e6f 742d 666f 756e  -server-not-foun
+00001cb0: 6427 3a20 5b27 3430 3427 2c0a 2020 2020  d': ['404',.    
+00001cc0: 2020 2020 2763 616e 6365 6c27 2c0a 2020      'cancel',.  
+00001cd0: 2020 2020 2020 2741 2072 656d 6f74 6520        'A remote 
+00001ce0: 7365 7276 6572 206f 7220 7365 7276 6963  server or servic
+00001cf0: 6520 7370 6563 6966 6965 6420 6173 2070  e specified as p
+00001d00: 6172 7420 6f72 2061 6c6c 206f 6620 7468  art or all of th
+00001d10: 6520 4a49 4420 6f66 2074 6865 2069 6e74  e JID of the int
+00001d20: 656e 6465 6420 7265 6369 7069 656e 7420  ended recipient 
+00001d30: 646f 6573 206e 6f74 2065 7869 7374 2e27  does not exist.'
+00001d40: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
+00001d50: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+00001d60: 6d70 702d 7374 616e 7a61 7320 7265 6d6f  mpp-stanzas remo
+00001d70: 7465 2d73 6572 7665 722d 7469 6d65 6f75  te-server-timeou
+00001d80: 7427 3a20 5b27 3530 3427 2c0a 2020 2020  t': ['504',.    
+00001d90: 2020 2020 2777 6169 7427 2c0a 2020 2020      'wait',.    
+00001da0: 2020 2020 2741 2072 656d 6f74 6520 7365      'A remote se
+00001db0: 7276 6572 206f 7220 7365 7276 6963 6520  rver or service 
+00001dc0: 7370 6563 6966 6965 6420 6173 2070 6172  specified as par
+00001dd0: 7420 6f72 2061 6c6c 206f 6620 7468 6520  t or all of the 
+00001de0: 4a49 4420 6f66 2074 6865 2069 6e74 656e  JID of the inten
+00001df0: 6465 6420 7265 6369 7069 656e 7420 636f  ded recipient co
+00001e00: 756c 6420 6e6f 7420 6265 2063 6f6e 7461  uld not be conta
+00001e10: 6374 6564 2077 6974 6869 6e20 6120 7265  cted within a re
+00001e20: 6173 6f6e 6162 6c65 2061 6d6f 756e 7420  asonable amount 
+00001e30: 6f66 2074 696d 652e 275d 2c0a 2020 2020  of time.'],.    
+00001e40: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
+00001e50: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7461  :xml:ns:xmpp-sta
+00001e60: 6e7a 6173 2072 6573 6f75 7263 652d 636f  nzas resource-co
+00001e70: 6e73 7472 6169 6e74 273a 205b 2735 3030  nstraint': ['500
+00001e80: 272c 0a20 2020 2020 2020 2027 7761 6974  ',.        'wait
+00001e90: 272c 0a20 2020 2020 2020 2027 5468 6520  ',.        'The 
+00001ea0: 7365 7276 6572 206f 7220 7265 6369 7069  server or recipi
+00001eb0: 656e 7420 6c61 636b 7320 7468 6520 7379  ent lacks the sy
+00001ec0: 7374 656d 2072 6573 6f75 7263 6573 206e  stem resources n
+00001ed0: 6563 6573 7361 7279 2074 6f20 7365 7276  ecessary to serv
+00001ee0: 6963 6520 7468 6520 7265 7175 6573 742e  ice the request.
+00001ef0: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+00001f00: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00001f10: 786d 7070 2d73 7461 6e7a 6173 2073 6572  xmpp-stanzas ser
+00001f20: 7669 6365 2d75 6e61 7661 696c 6162 6c65  vice-unavailable
+00001f30: 273a 205b 2735 3033 272c 0a20 2020 2020  ': ['503',.     
+00001f40: 2020 2027 6361 6e63 656c 272c 0a20 2020     'cancel',.   
+00001f50: 2020 2020 2027 5468 6520 7365 7276 6572       'The server
+00001f60: 206f 7220 7265 6369 7069 656e 7420 646f   or recipient do
+00001f70: 6573 206e 6f74 2063 7572 7265 6e74 6c79  es not currently
+00001f80: 2070 726f 7669 6465 2074 6865 2072 6571   provide the req
+00001f90: 7565 7374 6564 2073 6572 7669 6365 2e27  uested service.'
+00001fa0: 5d2c 0a20 2020 2027 7572 6e3a 6965 7466  ],.    'urn:ietf
+00001fb0: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+00001fc0: 6d70 702d 7374 616e 7a61 7320 7375 6273  mpp-stanzas subs
+00001fd0: 6372 6970 7469 6f6e 2d72 6571 7569 7265  cription-require
+00001fe0: 6427 3a20 5b27 3430 3727 2c0a 2020 2020  d': ['407',.    
+00001ff0: 2020 2020 2761 7574 6827 2c0a 2020 2020      'auth',.    
+00002000: 2020 2020 2754 6865 2072 6571 7565 7374      'The request
+00002010: 696e 6720 656e 7469 7479 2069 7320 6e6f  ing entity is no
+00002020: 7420 6175 7468 6f72 697a 6564 2074 6f20  t authorized to 
+00002030: 6163 6365 7373 2074 6865 2072 6571 7565  access the reque
+00002040: 7374 6564 2073 6572 7669 6365 2062 6563  sted service bec
+00002050: 6175 7365 2061 2073 7562 7363 7269 7074  ause a subscript
+00002060: 696f 6e20 6973 2072 6571 7569 7265 642e  ion is required.
+00002070: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+00002080: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00002090: 786d 7070 2d73 7461 6e7a 6173 2075 6e64  xmpp-stanzas und
+000020a0: 6566 696e 6564 2d63 6f6e 6469 7469 6f6e  efined-condition
+000020b0: 273a 205b 2735 3030 272c 0a20 2020 2020  ': ['500',.     
+000020c0: 2020 2027 272c 0a20 2020 2020 2020 2027     '',.        '
+000020d0: 556e 6465 6669 6e65 6420 436f 6e64 6974  Undefined Condit
+000020e0: 696f 6e27 5d2c 0a20 2020 2027 7572 6e3a  ion'],.    'urn:
+000020f0: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
+00002100: 6e73 3a78 6d70 702d 7374 616e 7a61 7320  ns:xmpp-stanzas 
+00002110: 756e 6578 7065 6374 6564 2d72 6571 7565  unexpected-reque
+00002120: 7374 273a 205b 2734 3030 272c 0a20 2020  st': ['400',.   
+00002130: 2020 2020 2027 7761 6974 272c 0a20 2020       'wait',.   
+00002140: 2020 2020 2027 5468 6520 7265 6369 7069       'The recipi
+00002150: 656e 7420 6f72 2073 6572 7665 7220 756e  ent or server un
+00002160: 6465 7273 746f 6f64 2074 6865 2072 6571  derstood the req
+00002170: 7565 7374 2062 7574 2077 6173 206e 6f74  uest but was not
+00002180: 2065 7870 6563 7469 6e67 2069 7420 6174   expecting it at
+00002190: 2074 6869 7320 7469 6d65 2028 652e 672e   this time (e.g.
+000021a0: 2c20 7468 6520 7265 7175 6573 7420 7761  , the request wa
+000021b0: 7320 6f75 7420 6f66 206f 7264 6572 292e  s out of order).
+000021c0: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+000021d0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+000021e0: 786d 7070 2d73 7472 6561 6d73 2062 6164  xmpp-streams bad
+000021f0: 2d66 6f72 6d61 7427 3a20 5b27 272c 0a20  -format': ['',. 
+00002200: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
+00002210: 2020 2027 5468 6520 656e 7469 7479 2068     'The entity h
+00002220: 6173 2073 656e 7420 584d 4c20 7468 6174  as sent XML that
+00002230: 2063 616e 6e6f 7420 6265 2070 726f 6365   cannot be proce
+00002240: 7373 6564 2e27 5d2c 0a20 2020 2027 7572  ssed.'],.    'ur
+00002250: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
+00002260: 6c3a 6e73 3a78 6d70 702d 7374 7265 616d  l:ns:xmpp-stream
+00002270: 7320 6261 642d 6e61 6d65 7370 6163 652d  s bad-namespace-
+00002280: 7072 6566 6978 273a 205b 2727 2c0a 2020  prefix': ['',.  
+00002290: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
+000022a0: 2020 2754 6865 2065 6e74 6974 7920 6861    'The entity ha
+000022b0: 7320 7365 6e74 2061 206e 616d 6573 7061  s sent a namespa
+000022c0: 6365 2070 7265 6669 7820 7468 6174 2069  ce prefix that i
+000022d0: 7320 756e 7375 7070 6f72 7465 642c 206f  s unsupported, o
+000022e0: 7220 6861 7320 7365 6e74 206e 6f20 6e61  r has sent no na
+000022f0: 6d65 7370 6163 6520 7072 6566 6978 206f  mespace prefix o
+00002300: 6e20 616e 2065 6c65 6d65 6e74 2074 6861  n an element tha
+00002310: 7420 7265 7175 6972 6573 2073 7563 6820  t requires such 
+00002320: 6120 7072 6566 6978 2e27 5d2c 0a20 2020  a prefix.'],.   
+00002330: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
+00002340: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
+00002350: 7265 616d 7320 636f 6e66 6c69 6374 273a  reams conflict':
+00002360: 205b 2727 2c0a 2020 2020 2020 2020 2727   ['',.        ''
+00002370: 2c0a 2020 2020 2020 2020 2754 6865 2073  ,.        'The s
+00002380: 6572 7665 7220 6973 2063 6c6f 7369 6e67  erver is closing
+00002390: 2074 6865 2061 6374 6976 6520 7374 7265   the active stre
+000023a0: 616d 2066 6f72 2074 6869 7320 656e 7469  am for this enti
+000023b0: 7479 2062 6563 6175 7365 2061 206e 6577  ty because a new
+000023c0: 2073 7472 6561 6d20 6861 7320 6265 656e   stream has been
+000023d0: 2069 6e69 7469 6174 6564 2074 6861 7420   initiated that 
+000023e0: 636f 6e66 6c69 6374 7320 7769 7468 2074  conflicts with t
+000023f0: 6865 2065 7869 7374 696e 6720 7374 7265  he existing stre
+00002400: 616d 2e27 5d2c 0a20 2020 2027 7572 6e3a  am.'],.    'urn:
+00002410: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
+00002420: 6e73 3a78 6d70 702d 7374 7265 616d 7320  ns:xmpp-streams 
+00002430: 636f 6e6e 6563 7469 6f6e 2d74 696d 656f  connection-timeo
+00002440: 7574 273a 205b 2727 2c0a 2020 2020 2020  ut': ['',.      
+00002450: 2020 2727 2c0a 2020 2020 2020 2020 2754    '',.        'T
+00002460: 6865 2065 6e74 6974 7920 6861 7320 6e6f  he entity has no
+00002470: 7420 6765 6e65 7261 7465 6420 616e 7920  t generated any 
+00002480: 7472 6166 6669 6320 6f76 6572 2074 6865  traffic over the
+00002490: 2073 7472 6561 6d20 666f 7220 736f 6d65   stream for some
+000024a0: 2070 6572 696f 6420 6f66 2074 696d 652e   period of time.
+000024b0: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+000024c0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+000024d0: 786d 7070 2d73 7472 6561 6d73 2068 6f73  xmpp-streams hos
+000024e0: 742d 676f 6e65 273a 205b 2727 2c0a 2020  t-gone': ['',.  
+000024f0: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
+00002500: 2020 2254 6865 2076 616c 7565 206f 6620    "The value of 
+00002510: 7468 6520 2020 2020 2020 2027 746f 2720  the        'to' 
+00002520: 6174 7472 6962 7574 6520 7072 6f76 6964  attribute provid
+00002530: 6564 2062 7920 7468 6520 696e 6974 6961  ed by the initia
+00002540: 7469 6e67 2065 6e74 6974 7920 696e 2074  ting entity in t
+00002550: 6865 2073 7472 6561 6d20 6865 6164 6572  he stream header
+00002560: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+00002570: 6120 686f 7374 6e61 6d65 2074 6861 7420  a hostname that 
+00002580: 6973 206e 6f20 6c6f 6e67 6572 2068 6f73  is no longer hos
+00002590: 7465 6420 6279 2074 6865 2073 6572 7665  ted by the serve
+000025a0: 722e 225d 2c0a 2020 2020 2775 726e 3a69  r."],.    'urn:i
+000025b0: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
+000025c0: 733a 786d 7070 2d73 7472 6561 6d73 2068  s:xmpp-streams h
+000025d0: 6f73 742d 756e 6b6e 6f77 6e27 3a20 5b27  ost-unknown': ['
+000025e0: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
+000025f0: 2020 2020 2020 2022 5468 6520 7661 6c75         "The valu
+00002600: 6520 6f66 2074 6865 2020 2020 2020 2020  e of the        
+00002610: 2774 6f27 2061 7474 7269 6275 7465 2070  'to' attribute p
+00002620: 726f 7669 6465 6420 6279 2074 6865 2069  rovided by the i
+00002630: 6e69 7469 6174 696e 6720 656e 7469 7479  nitiating entity
+00002640: 2069 6e20 7468 6520 7374 7265 616d 2068   in the stream h
+00002650: 6561 6465 7220 646f 6573 206e 6f74 2063  eader does not c
+00002660: 6f72 7265 7370 6f6e 6420 746f 2061 2068  orrespond to a h
+00002670: 6f73 746e 616d 6520 7468 6174 2069 7320  ostname that is 
+00002680: 686f 7374 6564 2062 7920 7468 6520 7365  hosted by the se
+00002690: 7276 6572 2e22 5d2c 0a20 2020 2027 7572  rver."],.    'ur
+000026a0: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
+000026b0: 6c3a 6e73 3a78 6d70 702d 7374 7265 616d  l:ns:xmpp-stream
+000026c0: 7320 696d 7072 6f70 6572 2d61 6464 7265  s improper-addre
+000026d0: 7373 696e 6727 3a20 5b27 272c 0a20 2020  ssing': ['',.   
+000026e0: 2020 2020 2027 272c 0a20 2020 2020 2020       '',.       
+000026f0: 2022 4120 7374 616e 7a61 2073 656e 7420   "A stanza sent 
+00002700: 6265 7477 6565 6e20 7477 6f20 7365 7276  between two serv
+00002710: 6572 7320 6c61 636b 7320 6120 2020 2020  ers lacks a     
+00002720: 2020 2027 746f 2720 6f72 2027 6672 6f6d     'to' or 'from
+00002730: 2720 6174 7472 6962 7574 6520 286f 7220  ' attribute (or 
+00002740: 7468 6520 6174 7472 6962 7574 6520 6861  the attribute ha
+00002750: 7320 6e6f 2076 616c 7565 292e 225d 2c0a  s no value)."],.
+00002760: 2020 2020 2775 726e 3a69 6574 663a 7061      'urn:ietf:pa
+00002770: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
+00002780: 2d73 7472 6561 6d73 2069 6e74 6572 6e61  -streams interna
+00002790: 6c2d 7365 7276 6572 2d65 7272 6f72 273a  l-server-error':
+000027a0: 205b 2727 2c0a 2020 2020 2020 2020 2727   ['',.        ''
+000027b0: 2c0a 2020 2020 2020 2020 2754 6865 2073  ,.        'The s
+000027c0: 6572 7665 7220 6861 7320 6578 7065 7269  erver has experi
+000027d0: 656e 6365 6420 6120 6d69 7363 6f6e 6669  enced a misconfi
+000027e0: 6775 7261 7469 6f6e 206f 7220 616e 206f  guration or an o
+000027f0: 7468 6572 7769 7365 2d75 6e64 6566 696e  therwise-undefin
+00002800: 6564 2069 6e74 6572 6e61 6c20 6572 726f  ed internal erro
+00002810: 7220 7468 6174 2070 7265 7665 6e74 7320  r that prevents 
+00002820: 6974 2066 726f 6d20 7365 7276 6963 696e  it from servicin
+00002830: 6720 7468 6520 7374 7265 616d 2e27 5d2c  g the stream.'],
+00002840: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
+00002850: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00002860: 702d 7374 7265 616d 7320 696e 7661 6c69  p-streams invali
+00002870: 642d 6672 6f6d 273a 205b 2763 616e 6365  d-from': ['cance
+00002880: 6c27 2c0a 2020 2020 2020 2020 2727 2c0a  l',.        '',.
+00002890: 2020 2020 2020 2020 2254 6865 204a 4944          "The JID
+000028a0: 206f 7220 686f 7374 6e61 6d65 2070 726f   or hostname pro
+000028b0: 7669 6465 6420 696e 2061 2020 2020 2020  vided in a      
+000028c0: 2020 2766 726f 6d27 2061 6464 7265 7373    'from' address
+000028d0: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
+000028e0: 616e 2061 7574 686f 7269 7a65 6420 4a49  an authorized JI
+000028f0: 4420 6f72 2076 616c 6964 6174 6564 2064  D or validated d
+00002900: 6f6d 6169 6e20 6e65 676f 7469 6174 6564  omain negotiated
+00002910: 2062 6574 7765 656e 2073 6572 7665 7273   between servers
+00002920: 2076 6961 2053 4153 4c20 6f72 2064 6961   via SASL or dia
+00002930: 6c62 6163 6b2c 206f 7220 6265 7477 6565  lback, or betwee
+00002940: 6e20 6120 636c 6965 6e74 2061 6e64 2061  n a client and a
+00002950: 2073 6572 7665 7220 7669 6120 6175 7468   server via auth
+00002960: 656e 7469 6361 7469 6f6e 2061 6e64 2072  entication and r
+00002970: 6573 6f75 7263 6520 6175 7468 6f72 697a  esource authoriz
+00002980: 6174 696f 6e2e 225d 2c0a 2020 2020 2775  ation."],.    'u
+00002990: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+000029a0: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
+000029b0: 6d73 2069 6e76 616c 6964 2d69 6427 3a20  ms invalid-id': 
+000029c0: 5b27 272c 0a20 2020 2020 2020 2027 272c  ['',.        '',
+000029d0: 0a20 2020 2020 2020 2027 5468 6520 7374  .        'The st
+000029e0: 7265 616d 2049 4420 6f72 2064 6961 6c62  ream ID or dialb
+000029f0: 6163 6b20 4944 2069 7320 696e 7661 6c69  ack ID is invali
+00002a00: 6420 6f72 2064 6f65 7320 6e6f 7420 6d61  d or does not ma
+00002a10: 7463 6820 616e 2049 4420 7072 6576 696f  tch an ID previo
+00002a20: 7573 6c79 2070 726f 7669 6465 642e 275d  usly provided.']
+00002a30: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
+00002a40: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00002a50: 7070 2d73 7472 6561 6d73 2069 6e76 616c  pp-streams inval
+00002a60: 6964 2d6e 616d 6573 7061 6365 273a 205b  id-namespace': [
+00002a70: 2727 2c0a 2020 2020 2020 2020 2727 2c0a  '',.        '',.
+00002a80: 2020 2020 2020 2020 2754 6865 2073 7472          'The str
+00002a90: 6561 6d73 206e 616d 6573 7061 6365 206e  eams namespace n
+00002aa0: 616d 6520 6973 2073 6f6d 6574 6869 6e67  ame is something
+00002ab0: 206f 7468 6572 2074 6861 6e20 2020 2020   other than     
+00002ac0: 2020 2022 6874 7470 3a2f 2f65 7468 6572     "http://ether
+00002ad0: 782e 6a61 6262 6572 2e6f 7267 2f73 7472  x.jabber.org/str
+00002ae0: 6561 6d73 2220 6f72 2074 6865 2064 6961  eams" or the dia
+00002af0: 6c62 6163 6b20 6e61 6d65 7370 6163 6520  lback namespace 
+00002b00: 6e61 6d65 2069 7320 736f 6d65 7468 696e  name is somethin
+00002b10: 6720 6f74 6865 7220 7468 616e 2022 6a61  g other than "ja
+00002b20: 6262 6572 3a73 6572 7665 723a 6469 616c  bber:server:dial
+00002b30: 6261 636b 222e 275d 2c0a 2020 2020 2775  back".'],.    'u
+00002b40: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00002b50: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
+00002b60: 6d73 2069 6e76 616c 6964 2d78 6d6c 273a  ms invalid-xml':
+00002b70: 205b 2727 2c0a 2020 2020 2020 2020 2727   ['',.        ''
+00002b80: 2c0a 2020 2020 2020 2020 2754 6865 2065  ,.        'The e
+00002b90: 6e74 6974 7920 6861 7320 7365 6e74 2069  ntity has sent i
+00002ba0: 6e76 616c 6964 2058 4d4c 206f 7665 7220  nvalid XML over 
+00002bb0: 7468 6520 7374 7265 616d 2074 6f20 6120  the stream to a 
+00002bc0: 7365 7276 6572 2074 6861 7420 7065 7266  server that perf
+00002bd0: 6f72 6d73 2076 616c 6964 6174 696f 6e2e  orms validation.
+00002be0: 275d 2c0a 2020 2020 2775 726e 3a69 6574  '],.    'urn:iet
+00002bf0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00002c00: 786d 7070 2d73 7472 6561 6d73 206e 6f74  xmpp-streams not
+00002c10: 2d61 7574 686f 7269 7a65 6427 3a20 5b27  -authorized': ['
+00002c20: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
+00002c30: 2020 2020 2020 2027 5468 6520 656e 7469         'The enti
+00002c40: 7479 2068 6173 2061 7474 656d 7074 6564  ty has attempted
+00002c50: 2074 6f20 7365 6e64 2064 6174 6120 6265   to send data be
+00002c60: 666f 7265 2074 6865 2073 7472 6561 6d20  fore the stream 
+00002c70: 6861 7320 6265 656e 2061 7574 6865 6e74  has been authent
+00002c80: 6963 6174 6564 2c20 6f72 206f 7468 6572  icated, or other
+00002c90: 7769 7365 2069 7320 6e6f 7420 6175 7468  wise is not auth
+00002ca0: 6f72 697a 6564 2074 6f20 7065 7266 6f72  orized to perfor
+00002cb0: 6d20 616e 2061 6374 696f 6e20 7265 6c61  m an action rela
+00002cc0: 7465 6420 746f 2073 7472 6561 6d20 6e65  ted to stream ne
+00002cd0: 676f 7469 6174 696f 6e2e 275d 2c0a 2020  gotiation.'],.  
+00002ce0: 2020 2775 726e 3a69 6574 663a 7061 7261    'urn:ietf:para
+00002cf0: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00002d00: 7472 6561 6d73 2070 6f6c 6963 792d 7669  treams policy-vi
+00002d10: 6f6c 6174 696f 6e27 3a20 5b27 272c 0a20  olation': ['',. 
+00002d20: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
+00002d30: 2020 2027 5468 6520 656e 7469 7479 2068     'The entity h
+00002d40: 6173 2076 696f 6c61 7465 6420 736f 6d65  as violated some
+00002d50: 206c 6f63 616c 2073 6572 7669 6365 2070   local service p
+00002d60: 6f6c 6963 792e 275d 2c0a 2020 2020 2775  olicy.'],.    'u
+00002d70: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00002d80: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
+00002d90: 6d73 2072 656d 6f74 652d 636f 6e6e 6563  ms remote-connec
+00002da0: 7469 6f6e 2d66 6169 6c65 6427 3a20 5b27  tion-failed': ['
+00002db0: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
+00002dc0: 2020 2020 2020 2027 5468 6520 7365 7276         'The serv
+00002dd0: 6572 2069 7320 756e 6162 6c65 2074 6f20  er is unable to 
+00002de0: 7072 6f70 6572 6c79 2063 6f6e 6e65 6374  properly connect
+00002df0: 2074 6f20 6120 7265 6d6f 7465 2072 6573   to a remote res
+00002e00: 6f75 7263 6520 7468 6174 2069 7320 7265  ource that is re
+00002e10: 7175 6972 6564 2066 6f72 2061 7574 6865  quired for authe
+00002e20: 6e74 6963 6174 696f 6e20 6f72 2061 7574  ntication or aut
+00002e30: 686f 7269 7a61 7469 6f6e 2e27 5d2c 0a20  horization.'],. 
+00002e40: 2020 2027 7572 6e3a 6965 7466 3a70 6172     'urn:ietf:par
+00002e50: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
+00002e60: 7374 7265 616d 7320 7265 736f 7572 6365  streams resource
+00002e70: 2d63 6f6e 7374 7261 696e 7427 3a20 5b27  -constraint': ['
+00002e80: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
+00002e90: 2020 2020 2020 2027 5468 6520 7365 7276         'The serv
+00002ea0: 6572 206c 6163 6b73 2074 6865 2073 7973  er lacks the sys
+00002eb0: 7465 6d20 7265 736f 7572 6365 7320 6e65  tem resources ne
+00002ec0: 6365 7373 6172 7920 746f 2073 6572 7669  cessary to servi
+00002ed0: 6365 2074 6865 2073 7472 6561 6d2e 275d  ce the stream.']
+00002ee0: 2c0a 2020 2020 2775 726e 3a69 6574 663a  ,.    'urn:ietf:
+00002ef0: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00002f00: 7070 2d73 7472 6561 6d73 2072 6573 7472  pp-streams restr
+00002f10: 6963 7465 642d 786d 6c27 3a20 5b27 272c  icted-xml': ['',
+00002f20: 0a20 2020 2020 2020 2027 272c 0a20 2020  .        '',.   
+00002f30: 2020 2020 2027 5468 6520 656e 7469 7479       'The entity
+00002f40: 2068 6173 2061 7474 656d 7074 6564 2074   has attempted t
+00002f50: 6f20 7365 6e64 2072 6573 7472 6963 7465  o send restricte
+00002f60: 6420 584d 4c20 6665 6174 7572 6573 2073  d XML features s
+00002f70: 7563 6820 6173 2061 2063 6f6d 6d65 6e74  uch as a comment
+00002f80: 2c20 7072 6f63 6573 7369 6e67 2069 6e73  , processing ins
+00002f90: 7472 7563 7469 6f6e 2c20 4454 442c 2065  truction, DTD, e
+00002fa0: 6e74 6974 7920 7265 6665 7265 6e63 652c  ntity reference,
+00002fb0: 206f 7220 756e 6573 6361 7065 6420 6368   or unescaped ch
+00002fc0: 6172 6163 7465 722e 275d 2c0a 2020 2020  aracter.'],.    
+00002fd0: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
+00002fe0: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
+00002ff0: 6561 6d73 2073 6565 2d6f 7468 6572 2d68  eams see-other-h
+00003000: 6f73 7427 3a20 5b27 272c 0a20 2020 2020  ost': ['',.     
+00003010: 2020 2027 272c 0a20 2020 2020 2020 2027     '',.        '
+00003020: 5468 6520 7365 7276 6572 2077 696c 6c20  The server will 
+00003030: 6e6f 7420 7072 6f76 6964 6520 7365 7276  not provide serv
+00003040: 6963 6520 746f 2074 6865 2069 6e69 7469  ice to the initi
+00003050: 6174 696e 6720 656e 7469 7479 2062 7574  ating entity but
+00003060: 2069 7320 7265 6469 7265 6374 696e 6720   is redirecting 
+00003070: 7472 6166 6669 6320 746f 2061 6e6f 7468  traffic to anoth
+00003080: 6572 2068 6f73 742e 275d 2c0a 2020 2020  er host.'],.    
+00003090: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
+000030a0: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
+000030b0: 6561 6d73 2073 7973 7465 6d2d 7368 7574  eams system-shut
+000030c0: 646f 776e 273a 205b 2727 2c0a 2020 2020  down': ['',.    
+000030d0: 2020 2020 2727 2c0a 2020 2020 2020 2020      '',.        
+000030e0: 2754 6865 2073 6572 7665 7220 6973 2062  'The server is b
+000030f0: 6569 6e67 2073 6875 7420 646f 776e 2061  eing shut down a
+00003100: 6e64 2061 6c6c 2061 6374 6976 6520 7374  nd all active st
+00003110: 7265 616d 7320 6172 6520 6265 696e 6720  reams are being 
+00003120: 636c 6f73 6564 2e27 5d2c 0a20 2020 2027  closed.'],.    '
+00003130: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
+00003140: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
+00003150: 616d 7320 756e 6465 6669 6e65 642d 636f  ams undefined-co
+00003160: 6e64 6974 696f 6e27 3a20 5b27 272c 0a20  ndition': ['',. 
+00003170: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
+00003180: 2020 2027 5468 6520 6572 726f 7220 636f     'The error co
+00003190: 6e64 6974 696f 6e20 6973 206e 6f74 206f  ndition is not o
+000031a0: 6e65 206f 6620 7468 6f73 6520 6465 6669  ne of those defi
+000031b0: 6e65 6420 6279 2074 6865 206f 7468 6572  ned by the other
+000031c0: 2063 6f6e 6469 7469 6f6e 7320 696e 2074   conditions in t
+000031d0: 6869 7320 6c69 7374 2e27 5d2c 0a20 2020  his list.'],.   
+000031e0: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
+000031f0: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
+00003200: 7265 616d 7320 756e 7375 7070 6f72 7465  reams unsupporte
+00003210: 642d 656e 636f 6469 6e67 273a 205b 2727  d-encoding': [''
+00003220: 2c0a 2020 2020 2020 2020 2727 2c0a 2020  ,.        '',.  
+00003230: 2020 2020 2020 2754 6865 2069 6e69 7469        'The initi
+00003240: 6174 696e 6720 656e 7469 7479 2068 6173  ating entity has
+00003250: 2065 6e63 6f64 6564 2074 6865 2073 7472   encoded the str
+00003260: 6561 6d20 696e 2061 6e20 656e 636f 6469  eam in an encodi
+00003270: 6e67 2074 6861 7420 6973 206e 6f74 2073  ng that is not s
+00003280: 7570 706f 7274 6564 2062 7920 7468 6520  upported by the 
+00003290: 7365 7276 6572 2e27 5d2c 0a20 2020 2027  server.'],.    '
+000032a0: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
+000032b0: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
+000032c0: 616d 7320 756e 7375 7070 6f72 7465 642d  ams unsupported-
+000032d0: 7374 616e 7a61 2d74 7970 6527 3a20 5b27  stanza-type': ['
+000032e0: 272c 0a20 2020 2020 2020 2027 272c 0a20  ',.        '',. 
+000032f0: 2020 2020 2020 2027 5468 6520 696e 6974         'The init
+00003300: 6961 7469 6e67 2065 6e74 6974 7920 6861  iating entity ha
+00003310: 7320 7365 6e74 2061 2066 6972 7374 2d6c  s sent a first-l
+00003320: 6576 656c 2063 6869 6c64 206f 6620 7468  evel child of th
+00003330: 6520 7374 7265 616d 2074 6861 7420 6973  e stream that is
+00003340: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
+00003350: 7920 7468 6520 7365 7276 6572 2e27 5d2c  y the server.'],
+00003360: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
+00003370: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00003380: 702d 7374 7265 616d 7320 756e 7375 7070  p-streams unsupp
+00003390: 6f72 7465 642d 7665 7273 696f 6e27 3a20  orted-version': 
+000033a0: 5b27 272c 0a20 2020 2020 2020 2027 272c  ['',.        '',
+000033b0: 0a20 2020 2020 2020 2022 5468 6520 7661  .        "The va
+000033c0: 6c75 6520 6f66 2074 6865 2020 2020 2020  lue of the      
+000033d0: 2020 2776 6572 7369 6f6e 2720 6174 7472    'version' attr
+000033e0: 6962 7574 6520 7072 6f76 6964 6564 2062  ibute provided b
+000033f0: 7920 7468 6520 696e 6974 6961 7469 6e67  y the initiating
+00003400: 2065 6e74 6974 7920 696e 2074 6865 2073   entity in the s
+00003410: 7472 6561 6d20 6865 6164 6572 2073 7065  tream header spe
+00003420: 6369 6669 6573 2061 2076 6572 7369 6f6e  cifies a version
+00003430: 206f 6620 584d 5050 2074 6861 7420 6973   of XMPP that is
+00003440: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
+00003450: 7920 7468 6520 7365 7276 6572 2e22 5d2c  y the server."],
+00003460: 0a20 2020 2027 7572 6e3a 6965 7466 3a70  .    'urn:ietf:p
+00003470: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00003480: 702d 7374 7265 616d 7320 786d 6c2d 6e6f  p-streams xml-no
+00003490: 742d 7765 6c6c 2d66 6f72 6d65 6427 3a20  t-well-formed': 
+000034a0: 5b27 272c 0a20 2020 2020 2020 2027 272c  ['',.        '',
+000034b0: 0a20 2020 2020 2020 2027 5468 6520 696e  .        'The in
+000034c0: 6974 6961 7469 6e67 2065 6e74 6974 7920  itiating entity 
+000034d0: 6861 7320 7365 6e74 2058 4d4c 2074 6861  has sent XML tha
+000034e0: 7420 6973 206e 6f74 2077 656c 6c2d 666f  t is not well-fo
+000034f0: 726d 6564 2e27 5d0a 7d0a 0a5f 6572 726f  rmed.'].}.._erro
+00003500: 7263 6f64 6573 203d 207b 0a20 2020 2027  rcodes = {.    '
+00003510: 3330 3227 3a20 2772 6564 6972 6563 7427  302': 'redirect'
+00003520: 2c0a 2020 2020 2734 3030 273a 2027 756e  ,.    '400': 'un
+00003530: 6578 7065 6374 6564 2d72 6571 7565 7374  expected-request
+00003540: 272c 0a20 2020 2027 3430 3127 3a20 276e  ',.    '401': 'n
+00003550: 6f74 2d61 7574 686f 7269 7a65 6427 2c0a  ot-authorized',.
+00003560: 2020 2020 2734 3032 273a 2027 7061 796d      '402': 'paym
+00003570: 656e 742d 7265 7175 6972 6564 272c 0a20  ent-required',. 
+00003580: 2020 2027 3430 3327 3a20 2766 6f72 6269     '403': 'forbi
+00003590: 6464 656e 272c 0a20 2020 2027 3430 3427  dden',.    '404'
+000035a0: 3a20 2772 656d 6f74 652d 7365 7276 6572  : 'remote-server
+000035b0: 2d6e 6f74 2d66 6f75 6e64 272c 0a20 2020  -not-found',.   
+000035c0: 2027 3430 3527 3a20 276e 6f74 2d61 6c6c   '405': 'not-all
+000035d0: 6f77 6564 272c 0a20 2020 2027 3430 3627  owed',.    '406'
+000035e0: 3a20 276e 6f74 2d61 6363 6570 7461 626c  : 'not-acceptabl
+000035f0: 6527 2c0a 2020 2020 2734 3037 273a 2027  e',.    '407': '
+00003600: 7375 6273 6372 6970 7469 6f6e 2d72 6571  subscription-req
+00003610: 7569 7265 6427 2c0a 2020 2020 2734 3039  uired',.    '409
+00003620: 273a 2027 636f 6e66 6c69 6374 272c 0a20  ': 'conflict',. 
+00003630: 2020 2027 3530 3027 3a20 2775 6e64 6566     '500': 'undef
+00003640: 696e 6564 2d63 6f6e 6469 7469 6f6e 272c  ined-condition',
+00003650: 0a20 2020 2027 3530 3127 3a20 2766 6561  .    '501': 'fea
+00003660: 7475 7265 2d6e 6f74 2d69 6d70 6c65 6d65  ture-not-impleme
+00003670: 6e74 6564 272c 0a20 2020 2027 3530 3327  nted',.    '503'
+00003680: 3a20 2773 6572 7669 6365 2d75 6e61 7661  : 'service-unava
+00003690: 696c 6162 6c65 272c 0a20 2020 2027 3530  ilable',.    '50
+000036a0: 3427 3a20 2772 656d 6f74 652d 7365 7276  4': 'remote-serv
+000036b0: 6572 2d74 696d 656f 7574 272c 0a20 2020  er-timeout',.   
+000036c0: 2027 6361 6e63 656c 273a 2027 696e 7661   'cancel': 'inva
+000036d0: 6c69 642d 6672 6f6d 270a 7d0a 0a0a 5f6c  lid-from'.}..._l
+000036e0: 6f63 616c 7061 7274 5f65 7363 6170 655f  ocalpart_escape_
+000036f0: 6368 6172 7320 3d20 2720 2226 5c27 2f3a  chars = ' "&\'/:
+00003700: 3c3e 4027 0a0a 0a53 5452 4541 4d5f 4e4f  <>@'...STREAM_NO
+00003710: 545f 4155 5448 4f52 495a 4544 203d 2027  T_AUTHORIZED = '
+00003720: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
+00003730: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
+00003740: 616d 7320 6e6f 742d 6175 7468 6f72 697a  ams not-authoriz
+00003750: 6564 270a 5354 5245 414d 5f52 454d 4f54  ed'.STREAM_REMOT
+00003760: 455f 434f 4e4e 4543 5449 4f4e 5f46 4149  E_CONNECTION_FAI
+00003770: 4c45 4420 3d20 2775 726e 3a69 6574 663a  LED = 'urn:ietf:
+00003780: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00003790: 7070 2d73 7472 6561 6d73 2072 656d 6f74  pp-streams remot
+000037a0: 652d 636f 6e6e 6563 7469 6f6e 2d66 6169  e-connection-fai
+000037b0: 6c65 6427 0a53 4153 4c5f 4d45 4348 414e  led'.SASL_MECHAN
+000037c0: 4953 4d5f 544f 4f5f 5745 414b 203d 2027  ISM_TOO_WEAK = '
+000037d0: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
+000037e0: 786d 6c3a 6e73 3a78 6d70 702d 7361 736c  xml:ns:xmpp-sasl
+000037f0: 206d 6563 6861 6e69 736d 2d74 6f6f 2d77   mechanism-too-w
+00003800: 6561 6b27 0a53 5452 4541 4d5f 584d 4c5f  eak'.STREAM_XML_
+00003810: 4e4f 545f 5745 4c4c 5f46 4f52 4d45 4420  NOT_WELL_FORMED 
+00003820: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
+00003830: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00003840: 7472 6561 6d73 2078 6d6c 2d6e 6f74 2d77  treams xml-not-w
+00003850: 656c 6c2d 666f 726d 6564 270a 4552 525f  ell-formed'.ERR_
+00003860: 4a49 445f 4d41 4c46 4f52 4d45 4420 3d20  JID_MALFORMED = 
+00003870: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
+00003880: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7461  :xml:ns:xmpp-sta
+00003890: 6e7a 6173 206a 6964 2d6d 616c 666f 726d  nzas jid-malform
+000038a0: 6564 270a 5354 5245 414d 5f53 4545 5f4f  ed'.STREAM_SEE_O
+000038b0: 5448 4552 5f48 4f53 5420 3d20 2775 726e  THER_HOST = 'urn
+000038c0: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
+000038d0: 3a6e 733a 786d 7070 2d73 7472 6561 6d73  :ns:xmpp-streams
+000038e0: 2073 6565 2d6f 7468 6572 2d68 6f73 7427   see-other-host'
+000038f0: 0a53 5452 4541 4d5f 4241 445f 4e41 4d45  .STREAM_BAD_NAME
+00003900: 5350 4143 455f 5052 4546 4958 203d 2027  SPACE_PREFIX = '
+00003910: 7572 6e3a 6965 7466 3a70 6172 616d 733a  urn:ietf:params:
+00003920: 786d 6c3a 6e73 3a78 6d70 702d 7374 7265  xml:ns:xmpp-stre
+00003930: 616d 7320 6261 642d 6e61 6d65 7370 6163  ams bad-namespac
+00003940: 652d 7072 6566 6978 270a 4552 525f 5345  e-prefix'.ERR_SE
+00003950: 5256 4943 455f 554e 4156 4149 4c41 424c  RVICE_UNAVAILABL
+00003960: 4520 3d20 2775 726e 3a69 6574 663a 7061  E = 'urn:ietf:pa
+00003970: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
+00003980: 2d73 7461 6e7a 6173 2073 6572 7669 6365  -stanzas service
+00003990: 2d75 6e61 7661 696c 6162 6c65 270a 5354  -unavailable'.ST
+000039a0: 5245 414d 5f43 4f4e 4e45 4354 494f 4e5f  REAM_CONNECTION_
+000039b0: 5449 4d45 4f55 5420 3d20 2775 726e 3a69  TIMEOUT = 'urn:i
+000039c0: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
+000039d0: 733a 786d 7070 2d73 7472 6561 6d73 2063  s:xmpp-streams c
+000039e0: 6f6e 6e65 6374 696f 6e2d 7469 6d65 6f75  onnection-timeou
+000039f0: 7427 0a53 5452 4541 4d5f 554e 5355 5050  t'.STREAM_UNSUPP
+00003a00: 4f52 5445 445f 5645 5253 494f 4e20 3d20  ORTED_VERSION = 
+00003a10: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
+00003a20: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
+00003a30: 6561 6d73 2075 6e73 7570 706f 7274 6564  eams unsupported
+00003a40: 2d76 6572 7369 6f6e 270a 5354 5245 414d  -version'.STREAM
+00003a50: 5f49 4d50 524f 5045 525f 4144 4452 4553  _IMPROPER_ADDRES
+00003a60: 5349 4e47 203d 2027 7572 6e3a 6965 7466  SING = 'urn:ietf
+00003a70: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+00003a80: 6d70 702d 7374 7265 616d 7320 696d 7072  mpp-streams impr
+00003a90: 6f70 6572 2d61 6464 7265 7373 696e 6727  oper-addressing'
+00003aa0: 0a53 5452 4541 4d5f 554e 4445 4649 4e45  .STREAM_UNDEFINE
+00003ab0: 445f 434f 4e44 4954 494f 4e20 3d20 2775  D_CONDITION = 'u
+00003ac0: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00003ad0: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
+00003ae0: 6d73 2075 6e64 6566 696e 6564 2d63 6f6e  ms undefined-con
+00003af0: 6469 7469 6f6e 270a 5341 534c 5f4e 4f54  dition'.SASL_NOT
+00003b00: 5f41 5554 484f 5249 5a45 4420 3d20 2775  _AUTHORIZED = 'u
+00003b10: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00003b20: 6d6c 3a6e 733a 786d 7070 2d73 6173 6c20  ml:ns:xmpp-sasl 
+00003b30: 6e6f 742d 6175 7468 6f72 697a 6564 270a  not-authorized'.
+00003b40: 4552 525f 474f 4e45 203d 2027 7572 6e3a  ERR_GONE = 'urn:
+00003b50: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
+00003b60: 6e73 3a78 6d70 702d 7374 616e 7a61 7320  ns:xmpp-stanzas 
+00003b70: 676f 6e65 270a 5341 534c 5f54 454d 504f  gone'.SASL_TEMPO
+00003b80: 5241 5259 5f41 5554 485f 4641 494c 5552  RARY_AUTH_FAILUR
+00003b90: 4520 3d20 2775 726e 3a69 6574 663a 7061  E = 'urn:ietf:pa
+00003ba0: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
+00003bb0: 2d73 6173 6c20 7465 6d70 6f72 6172 792d  -sasl temporary-
+00003bc0: 6175 7468 2d66 6169 6c75 7265 270a 4552  auth-failure'.ER
+00003bd0: 525f 5245 4d4f 5445 5f53 4552 5645 525f  R_REMOTE_SERVER_
+00003be0: 4e4f 545f 464f 554e 4420 3d20 2775 726e  NOT_FOUND = 'urn
+00003bf0: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
+00003c00: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
+00003c10: 2072 656d 6f74 652d 7365 7276 6572 2d6e   remote-server-n
+00003c20: 6f74 2d66 6f75 6e64 270a 4552 525f 554e  ot-found'.ERR_UN
+00003c30: 4558 5045 4354 4544 5f52 4551 5545 5354  EXPECTED_REQUEST
+00003c40: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
+00003c50: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
+00003c60: 7374 616e 7a61 7320 756e 6578 7065 6374  stanzas unexpect
+00003c70: 6564 2d72 6571 7565 7374 270a 4552 525f  ed-request'.ERR_
+00003c80: 5245 4349 5049 454e 545f 554e 4156 4149  RECIPIENT_UNAVAI
+00003c90: 4c41 424c 4520 3d20 2775 726e 3a69 6574  LABLE = 'urn:iet
+00003ca0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00003cb0: 786d 7070 2d73 7461 6e7a 6173 2072 6563  xmpp-stanzas rec
+00003cc0: 6970 6965 6e74 2d75 6e61 7661 696c 6162  ipient-unavailab
+00003cd0: 6c65 270a 4552 525f 434f 4e46 4c49 4354  le'.ERR_CONFLICT
+00003ce0: 203d 2027 7572 6e3a 6965 7466 3a70 6172   = 'urn:ietf:par
+00003cf0: 616d 733a 786d 6c3a 6e73 3a78 6d70 702d  ams:xml:ns:xmpp-
+00003d00: 7374 616e 7a61 7320 636f 6e66 6c69 6374  stanzas conflict
+00003d10: 270a 5354 5245 414d 5f53 5953 5445 4d5f  '.STREAM_SYSTEM_
+00003d20: 5348 5554 444f 574e 203d 2027 7572 6e3a  SHUTDOWN = 'urn:
+00003d30: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
+00003d40: 6e73 3a78 6d70 702d 7374 7265 616d 7320  ns:xmpp-streams 
+00003d50: 7379 7374 656d 2d73 6875 7464 6f77 6e27  system-shutdown'
+00003d60: 0a53 5452 4541 4d5f 4241 445f 464f 524d  .STREAM_BAD_FORM
+00003d70: 4154 203d 2027 7572 6e3a 6965 7466 3a70  AT = 'urn:ietf:p
+00003d80: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00003d90: 702d 7374 7265 616d 7320 6261 642d 666f  p-streams bad-fo
+00003da0: 726d 6174 270a 4552 525f 5355 4253 4352  rmat'.ERR_SUBSCR
+00003db0: 4950 5449 4f4e 5f52 4551 5549 5245 4420  IPTION_REQUIRED 
+00003dc0: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
+00003dd0: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00003de0: 7461 6e7a 6173 2073 7562 7363 7269 7074  tanzas subscript
+00003df0: 696f 6e2d 7265 7175 6972 6564 270a 5354  ion-required'.ST
+00003e00: 5245 414d 5f49 4e54 4552 4e41 4c5f 5345  REAM_INTERNAL_SE
+00003e10: 5256 4552 5f45 5252 4f52 203d 2027 7572  RVER_ERROR = 'ur
+00003e20: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
+00003e30: 6c3a 6e73 3a78 6d70 702d 7374 7265 616d  l:ns:xmpp-stream
+00003e40: 7320 696e 7465 726e 616c 2d73 6572 7665  s internal-serve
+00003e50: 722d 6572 726f 7227 0a45 5252 5f4e 4f54  r-error'.ERR_NOT
+00003e60: 5f41 5554 484f 5249 5a45 4420 3d20 2775  _AUTHORIZED = 'u
+00003e70: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00003e80: 6d6c 3a6e 733a 786d 7070 2d73 7461 6e7a  ml:ns:xmpp-stanz
+00003e90: 6173 206e 6f74 2d61 7574 686f 7269 7a65  as not-authorize
+00003ea0: 6427 0a53 4153 4c5f 4142 4f52 5445 4420  d'.SASL_ABORTED 
+00003eb0: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
+00003ec0: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00003ed0: 6173 6c20 6162 6f72 7465 6427 0a45 5252  asl aborted'.ERR
+00003ee0: 5f52 4547 4953 5452 4154 494f 4e5f 5245  _REGISTRATION_RE
+00003ef0: 5155 4952 4544 203d 2027 7572 6e3a 6965  QUIRED = 'urn:ie
+00003f00: 7466 3a70 6172 616d 733a 786d 6c3a 6e73  tf:params:xml:ns
+00003f10: 3a78 6d70 702d 7374 616e 7a61 7320 7265  :xmpp-stanzas re
+00003f20: 6769 7374 7261 7469 6f6e 2d72 6571 7569  gistration-requi
+00003f30: 7265 6427 0a45 5252 5f49 4e54 4552 4e41  red'.ERR_INTERNA
+00003f40: 4c5f 5345 5256 4552 5f45 5252 4f52 203d  L_SERVER_ERROR =
+00003f50: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
+00003f60: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
+00003f70: 616e 7a61 7320 696e 7465 726e 616c 2d73  anzas internal-s
+00003f80: 6572 7665 722d 6572 726f 7227 0a53 4153  erver-error'.SAS
+00003f90: 4c5f 494e 434f 5252 4543 545f 454e 434f  L_INCORRECT_ENCO
+00003fa0: 4449 4e47 203d 2027 7572 6e3a 6965 7466  DING = 'urn:ietf
+00003fb0: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+00003fc0: 6d70 702d 7361 736c 2069 6e63 6f72 7265  mpp-sasl incorre
+00003fd0: 6374 2d65 6e63 6f64 696e 6727 0a53 5452  ct-encoding'.STR
+00003fe0: 4541 4d5f 484f 5354 5f47 4f4e 4520 3d20  EAM_HOST_GONE = 
+00003ff0: 2775 726e 3a69 6574 663a 7061 7261 6d73  'urn:ietf:params
+00004000: 3a78 6d6c 3a6e 733a 786d 7070 2d73 7472  :xml:ns:xmpp-str
+00004010: 6561 6d73 2068 6f73 742d 676f 6e65 270a  eams host-gone'.
+00004020: 5354 5245 414d 5f50 4f4c 4943 595f 5649  STREAM_POLICY_VI
+00004030: 4f4c 4154 494f 4e20 3d20 2775 726e 3a69  OLATION = 'urn:i
+00004040: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
+00004050: 733a 786d 7070 2d73 7472 6561 6d73 2070  s:xmpp-streams p
+00004060: 6f6c 6963 792d 7669 6f6c 6174 696f 6e27  olicy-violation'
+00004070: 0a53 5452 4541 4d5f 494e 5641 4c49 445f  .STREAM_INVALID_
+00004080: 584d 4c20 3d20 2775 726e 3a69 6574 663a  XML = 'urn:ietf:
+00004090: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+000040a0: 7070 2d73 7472 6561 6d73 2069 6e76 616c  pp-streams inval
+000040b0: 6964 2d78 6d6c 270a 5354 5245 414d 5f43  id-xml'.STREAM_C
+000040c0: 4f4e 464c 4943 5420 3d20 2775 726e 3a69  ONFLICT = 'urn:i
+000040d0: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
+000040e0: 733a 786d 7070 2d73 7472 6561 6d73 2063  s:xmpp-streams c
+000040f0: 6f6e 666c 6963 7427 0a53 5452 4541 4d5f  onflict'.STREAM_
+00004100: 5245 534f 5552 4345 5f43 4f4e 5354 5241  RESOURCE_CONSTRA
+00004110: 494e 5420 3d20 2775 726e 3a69 6574 663a  INT = 'urn:ietf:
+00004120: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00004130: 7070 2d73 7472 6561 6d73 2072 6573 6f75  pp-streams resou
+00004140: 7263 652d 636f 6e73 7472 6169 6e74 270a  rce-constraint'.
+00004150: 5354 5245 414d 5f55 4e53 5550 504f 5254  STREAM_UNSUPPORT
+00004160: 4544 5f45 4e43 4f44 494e 4720 3d20 2775  ED_ENCODING = 'u
+00004170: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00004180: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
+00004190: 6d73 2075 6e73 7570 706f 7274 6564 2d65  ms unsupported-e
+000041a0: 6e63 6f64 696e 6727 0a45 5252 5f4e 4f54  ncoding'.ERR_NOT
+000041b0: 5f41 4c4c 4f57 4544 203d 2027 7572 6e3a  _ALLOWED = 'urn:
+000041c0: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
+000041d0: 6e73 3a78 6d70 702d 7374 616e 7a61 7320  ns:xmpp-stanzas 
+000041e0: 6e6f 742d 616c 6c6f 7765 6427 0a45 5252  not-allowed'.ERR
+000041f0: 5f49 5445 4d5f 4e4f 545f 464f 554e 4420  _ITEM_NOT_FOUND 
+00004200: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
+00004210: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00004220: 7461 6e7a 6173 2069 7465 6d2d 6e6f 742d  tanzas item-not-
+00004230: 666f 756e 6427 0a45 5252 5f4e 4f54 5f41  found'.ERR_NOT_A
+00004240: 4343 4550 5441 424c 4520 3d20 2775 726e  CCEPTABLE = 'urn
+00004250: 3a69 6574 663a 7061 7261 6d73 3a78 6d6c  :ietf:params:xml
+00004260: 3a6e 733a 786d 7070 2d73 7461 6e7a 6173  :ns:xmpp-stanzas
+00004270: 206e 6f74 2d61 6363 6570 7461 626c 6527   not-acceptable'
+00004280: 0a53 5452 4541 4d5f 494e 5641 4c49 445f  .STREAM_INVALID_
+00004290: 4652 4f4d 203d 2027 7572 6e3a 6965 7466  FROM = 'urn:ietf
+000042a0: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+000042b0: 6d70 702d 7374 7265 616d 7320 696e 7661  mpp-streams inva
+000042c0: 6c69 642d 6672 6f6d 270a 4552 525f 4645  lid-from'.ERR_FE
+000042d0: 4154 5552 455f 4e4f 545f 494d 504c 454d  ATURE_NOT_IMPLEM
+000042e0: 454e 5445 4420 3d20 2775 726e 3a69 6574  ENTED = 'urn:iet
+000042f0: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00004300: 786d 7070 2d73 7461 6e7a 6173 2066 6561  xmpp-stanzas fea
+00004310: 7475 7265 2d6e 6f74 2d69 6d70 6c65 6d65  ture-not-impleme
+00004320: 6e74 6564 270a 4552 525f 4241 445f 5245  nted'.ERR_BAD_RE
+00004330: 5155 4553 5420 3d20 2775 726e 3a69 6574  QUEST = 'urn:iet
+00004340: 663a 7061 7261 6d73 3a78 6d6c 3a6e 733a  f:params:xml:ns:
+00004350: 786d 7070 2d73 7461 6e7a 6173 2062 6164  xmpp-stanzas bad
+00004360: 2d72 6571 7565 7374 270a 5354 5245 414d  -request'.STREAM
+00004370: 5f49 4e56 414c 4944 5f49 4420 3d20 2775  _INVALID_ID = 'u
+00004380: 726e 3a69 6574 663a 7061 7261 6d73 3a78  rn:ietf:params:x
+00004390: 6d6c 3a6e 733a 786d 7070 2d73 7472 6561  ml:ns:xmpp-strea
+000043a0: 6d73 2069 6e76 616c 6964 2d69 6427 0a53  ms invalid-id'.S
+000043b0: 5452 4541 4d5f 484f 5354 5f55 4e4b 4e4f  TREAM_HOST_UNKNO
+000043c0: 574e 203d 2027 7572 6e3a 6965 7466 3a70  WN = 'urn:ietf:p
+000043d0: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+000043e0: 702d 7374 7265 616d 7320 686f 7374 2d75  p-streams host-u
+000043f0: 6e6b 6e6f 776e 270a 4552 525f 554e 4445  nknown'.ERR_UNDE
+00004400: 4649 4e45 445f 434f 4e44 4954 494f 4e20  FINED_CONDITION 
+00004410: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
+00004420: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+00004430: 7461 6e7a 6173 2075 6e64 6566 696e 6564  tanzas undefined
+00004440: 2d63 6f6e 6469 7469 6f6e 270a 5341 534c  -condition'.SASL
+00004450: 5f49 4e56 414c 4944 5f4d 4543 4841 4e49  _INVALID_MECHANI
+00004460: 534d 203d 2027 7572 6e3a 6965 7466 3a70  SM = 'urn:ietf:p
+00004470: 6172 616d 733a 786d 6c3a 6e73 3a78 6d70  arams:xml:ns:xmp
+00004480: 702d 7361 736c 2069 6e76 616c 6964 2d6d  p-sasl invalid-m
+00004490: 6563 6861 6e69 736d 270a 5354 5245 414d  echanism'.STREAM
+000044a0: 5f52 4553 5452 4943 5445 445f 584d 4c20  _RESTRICTED_XML 
+000044b0: 3d20 2775 726e 3a69 6574 663a 7061 7261  = 'urn:ietf:para
+000044c0: 6d73 3a78 6d6c 3a6e 733a 786d 7070 2d73  ms:xml:ns:xmpp-s
+000044d0: 7472 6561 6d73 2072 6573 7472 6963 7465  treams restricte
+000044e0: 642d 786d 6c27 0a45 5252 5f52 4553 4f55  d-xml'.ERR_RESOU
+000044f0: 5243 455f 434f 4e53 5452 4149 4e54 203d  RCE_CONSTRAINT =
+00004500: 2027 7572 6e3a 6965 7466 3a70 6172 616d   'urn:ietf:param
+00004510: 733a 786d 6c3a 6e73 3a78 6d70 702d 7374  s:xml:ns:xmpp-st
+00004520: 616e 7a61 7320 7265 736f 7572 6365 2d63  anzas resource-c
+00004530: 6f6e 7374 7261 696e 7427 0a45 5252 5f52  onstraint'.ERR_R
+00004540: 454d 4f54 455f 5345 5256 4552 5f54 494d  EMOTE_SERVER_TIM
+00004550: 454f 5554 203d 2027 7572 6e3a 6965 7466  EOUT = 'urn:ietf
+00004560: 3a70 6172 616d 733a 786d 6c3a 6e73 3a78  :params:xml:ns:x
+00004570: 6d70 702d 7374 616e 7a61 7320 7265 6d6f  mpp-stanzas remo
+00004580: 7465 2d73 6572 7665 722d 7469 6d65 6f75  te-server-timeou
+00004590: 7427 0a53 4153 4c5f 494e 5641 4c49 445f  t'.SASL_INVALID_
+000045a0: 4155 5448 5a49 4420 3d20 2775 726e 3a69  AUTHZID = 'urn:i
+000045b0: 6574 663a 7061 7261 6d73 3a78 6d6c 3a6e  etf:params:xml:n
+000045c0: 733a 786d 7070 2d73 6173 6c20 696e 7661  s:xmpp-sasl inva
+000045d0: 6c69 642d 6175 7468 7a69 6427 0a45 5252  lid-authzid'.ERR
+000045e0: 5f50 4159 4d45 4e54 5f52 4551 5549 5245  _PAYMENT_REQUIRE
+000045f0: 4420 3d20 2775 726e 3a69 6574 663a 7061  D = 'urn:ietf:pa
+00004600: 7261 6d73 3a78 6d6c 3a6e 733a 786d 7070  rams:xml:ns:xmpp
+00004610: 2d73 7461 6e7a 6173 2070 6179 6d65 6e74  -stanzas payment
+00004620: 2d72 6571 7569 7265 6427 0a53 5452 4541  -required'.STREA
+00004630: 4d5f 494e 5641 4c49 445f 4e41 4d45 5350  M_INVALID_NAMESP
+00004640: 4143 4520 3d20 2775 726e 3a69 6574 663a  ACE = 'urn:ietf:
+00004650: 7061 7261 6d73 3a78 6d6c 3a6e 733a 786d  params:xml:ns:xm
+00004660: 7070 2d73 7472 6561 6d73 2069 6e76 616c  pp-streams inval
+00004670: 6964 2d6e 616d 6573 7061 6365 270a 4552  id-namespace'.ER
+00004680: 525f 5245 4449 5245 4354 203d 2027 7572  R_REDIRECT = 'ur
+00004690: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
+000046a0: 6c3a 6e73 3a78 6d70 702d 7374 616e 7a61  l:ns:xmpp-stanza
+000046b0: 7320 7265 6469 7265 6374 270a 5354 5245  s redirect'.STRE
+000046c0: 414d 5f55 4e53 5550 504f 5254 4544 5f53  AM_UNSUPPORTED_S
+000046d0: 5441 4e5a 415f 5459 5045 203d 2027 7572  TANZA_TYPE = 'ur
+000046e0: 6e3a 6965 7466 3a70 6172 616d 733a 786d  n:ietf:params:xm
+000046f0: 6c3a 6e73 3a78 6d70 702d 7374 7265 616d  l:ns:xmpp-stream
+00004700: 7320 756e 7375 7070 6f72 7465 642d 7374  s unsupported-st
+00004710: 616e 7a61 2d74 7970 6527 0a45 5252 5f46  anza-type'.ERR_F
+00004720: 4f52 4249 4444 454e 203d 2027 7572 6e3a  ORBIDDEN = 'urn:
+00004730: 6965 7466 3a70 6172 616d 733a 786d 6c3a  ietf:params:xml:
+00004740: 6e73 3a78 6d70 702d 7374 616e 7a61 7320  ns:xmpp-stanzas 
+00004750: 666f 7262 6964 6465 6e27 0a0a 0a64 6566  forbidden'...def
+00004760: 2069 7352 6573 756c 744e 6f64 6528 6e6f   isResultNode(no
+00004770: 6465 293a 0a20 2020 2022 2222 0a20 2020  de):.    """.   
+00004780: 2052 6574 7572 6e20 7472 7565 2069 6620   Return true if 
+00004790: 7468 6520 6e6f 6465 2069 7320 6120 706f  the node is a po
+000047a0: 7369 7469 7665 2072 6570 6c79 0a20 2020  sitive reply.   
+000047b0: 2022 2222 0a20 2020 2072 6574 7572 6e20   """.    return 
+000047c0: 6e6f 6465 2061 6e64 206e 6f64 652e 6765  node and node.ge
+000047d0: 7454 7970 6528 2920 3d3d 2027 7265 7375  tType() == 'resu
+000047e0: 6c74 270a 0a64 6566 2069 7345 7272 6f72  lt'..def isError
+000047f0: 4e6f 6465 286e 6f64 6529 3a0a 2020 2020  Node(node):.    
+00004800: 2222 220a 2020 2020 5265 7475 726e 2074  """.    Return t
+00004810: 7275 6520 6966 2074 6865 206e 6f64 6520  rue if the node 
+00004820: 6973 2061 206e 6567 6174 6976 6520 7265  is a negative re
+00004830: 706c 790a 2020 2020 2222 220a 2020 2020  ply.    """.    
+00004840: 7265 7475 726e 206e 6f64 6520 616e 6420  return node and 
+00004850: 6e6f 6465 2e67 6574 5479 7065 2829 203d  node.getType() =
+00004860: 3d20 2765 7272 6f72 270a 0a64 6566 2069  = 'error'..def i
+00004870: 734d 7563 504d 286d 6573 7361 6765 293a  sMucPM(message):
+00004880: 0a20 2020 206d 7563 5f75 7365 7220 3d20  .    muc_user = 
+00004890: 6d65 7373 6167 652e 6765 7454 6167 2827  message.getTag('
+000048a0: 7827 2c20 6e61 6d65 7370 6163 653d 4e61  x', namespace=Na
+000048b0: 6d65 7370 6163 652e 4d55 435f 5553 4552  mespace.MUC_USER
+000048c0: 290a 2020 2020 7265 7475 726e 2028 6d65  ).    return (me
+000048d0: 7373 6167 652e 6765 7454 7970 6528 2920  ssage.getType() 
+000048e0: 696e 2028 2763 6861 7427 2c20 2765 7272  in ('chat', 'err
+000048f0: 6f72 2729 2061 6e64 0a20 2020 2020 2020  or') and.       
+00004900: 2020 2020 206d 7563 5f75 7365 7220 6973       muc_user is
+00004910: 206e 6f74 204e 6f6e 6520 616e 640a 2020   not None and.  
+00004920: 2020 2020 2020 2020 2020 6e6f 7420 6d75            not mu
+00004930: 635f 7573 6572 2e67 6574 4368 696c 6472  c_user.getChildr
+00004940: 656e 2829 290a 0a63 6c61 7373 204e 6f64  en())..class Nod
+00004950: 6550 726f 6365 7373 6564 2845 7863 6570  eProcessed(Excep
+00004960: 7469 6f6e 293a 0a20 2020 2022 2222 0a20  tion):.    """. 
+00004970: 2020 2045 7863 6570 7469 6f6e 2074 6861     Exception tha
+00004980: 7420 7368 6f75 6c64 2062 6520 7261 6973  t should be rais
+00004990: 6564 2062 7920 6861 6e64 6c65 7220 7768  ed by handler wh
+000049a0: 656e 2074 6865 2068 616e 646c 696e 6720  en the handling 
+000049b0: 7368 6f75 6c64 2062 650a 2020 2020 7374  should be.    st
+000049c0: 6f70 7065 640a 2020 2020 2222 220a 0a63  opped.    """..c
+000049d0: 6c61 7373 2053 7472 6561 6d45 7272 6f72  lass StreamError
+000049e0: 2845 7863 6570 7469 6f6e 293a 0a20 2020  (Exception):.   
+000049f0: 2022 2222 0a20 2020 2042 6173 6520 6578   """.    Base ex
+00004a00: 6365 7074 696f 6e20 636c 6173 7320 666f  ception class fo
+00004a10: 7220 7374 7265 616d 2065 7272 6f72 730a  r stream errors.
+00004a20: 2020 2020 2222 220a 0a63 6c61 7373 2042      """..class B
+00004a30: 6164 466f 726d 6174 2853 7472 6561 6d45  adFormat(StreamE
+00004a40: 7272 6f72 293a 0a20 2020 2070 6173 730a  rror):.    pass.
+00004a50: 0a63 6c61 7373 2042 6164 4e61 6d65 7370  .class BadNamesp
+00004a60: 6163 6550 7265 6669 7828 5374 7265 616d  acePrefix(Stream
+00004a70: 4572 726f 7229 3a0a 2020 2020 7061 7373  Error):.    pass
+00004a80: 0a0a 636c 6173 7320 436f 6e66 6c69 6374  ..class Conflict
+00004a90: 2853 7472 6561 6d45 7272 6f72 293a 0a20  (StreamError):. 
+00004aa0: 2020 2070 6173 730a 0a63 6c61 7373 2043     pass..class C
+00004ab0: 6f6e 6e65 6374 696f 6e54 696d 656f 7574  onnectionTimeout
+00004ac0: 2853 7472 6561 6d45 7272 6f72 293a 0a20  (StreamError):. 
+00004ad0: 2020 2070 6173 730a 0a63 6c61 7373 2048     pass..class H
+00004ae0: 6f73 7447 6f6e 6528 5374 7265 616d 4572  ostGone(StreamEr
+00004af0: 726f 7229 3a0a 2020 2020 7061 7373 0a0a  ror):.    pass..
+00004b00: 636c 6173 7320 486f 7374 556e 6b6e 6f77  class HostUnknow
+00004b10: 6e28 5374 7265 616d 4572 726f 7229 3a0a  n(StreamError):.
+00004b20: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
+00004b30: 496d 7072 6f70 6572 4164 6472 6573 7369  ImproperAddressi
+00004b40: 6e67 2853 7472 6561 6d45 7272 6f72 293a  ng(StreamError):
+00004b50: 0a20 2020 2070 6173 730a 0a63 6c61 7373  .    pass..class
+00004b60: 2049 6e74 6572 6e61 6c53 6572 7665 7245   InternalServerE
+00004b70: 7272 6f72 2853 7472 6561 6d45 7272 6f72  rror(StreamError
+00004b80: 293a 0a20 2020 2070 6173 730a 0a63 6c61  ):.    pass..cla
+00004b90: 7373 2049 6e76 616c 6964 4672 6f6d 2853  ss InvalidFrom(S
+00004ba0: 7472 6561 6d45 7272 6f72 293a 0a20 2020  treamError):.   
+00004bb0: 2070 6173 730a 0a63 6c61 7373 2049 6e76   pass..class Inv
+00004bc0: 616c 6964 4944 2853 7472 6561 6d45 7272  alidID(StreamErr
+00004bd0: 6f72 293a 0a20 2020 2070 6173 730a 0a63  or):.    pass..c
+00004be0: 6c61 7373 2049 6e76 616c 6964 4e61 6d65  lass InvalidName
+00004bf0: 7370 6163 6528 5374 7265 616d 4572 726f  space(StreamErro
+00004c00: 7229 3a0a 2020 2020 7061 7373 0a0a 636c  r):.    pass..cl
+00004c10: 6173 7320 496e 7661 6c69 6458 4d4c 2853  ass InvalidXML(S
+00004c20: 7472 6561 6d45 7272 6f72 293a 0a20 2020  treamError):.   
+00004c30: 2070 6173 730a 0a63 6c61 7373 204e 6f74   pass..class Not
+00004c40: 4175 7468 6f72 697a 6564 2853 7472 6561  Authorized(Strea
+00004c50: 6d45 7272 6f72 293a 0a20 2020 2070 6173  mError):.    pas
+00004c60: 730a 0a63 6c61 7373 2050 6f6c 6963 7956  s..class PolicyV
+00004c70: 696f 6c61 7469 6f6e 2853 7472 6561 6d45  iolation(StreamE
+00004c80: 7272 6f72 293a 0a20 2020 2070 6173 730a  rror):.    pass.
+00004c90: 0a63 6c61 7373 2052 656d 6f74 6543 6f6e  .class RemoteCon
+00004ca0: 6e65 6374 696f 6e46 6169 6c65 6428 5374  nectionFailed(St
+00004cb0: 7265 616d 4572 726f 7229 3a0a 2020 2020  reamError):.    
+00004cc0: 7061 7373 0a0a 636c 6173 7320 5265 736f  pass..class Reso
+00004cd0: 7572 6365 436f 6e73 7472 6169 6e74 2853  urceConstraint(S
+00004ce0: 7472 6561 6d45 7272 6f72 293a 0a20 2020  treamError):.   
+00004cf0: 2070 6173 730a 0a63 6c61 7373 2052 6573   pass..class Res
+00004d00: 7472 6963 7465 6458 4d4c 2853 7472 6561  trictedXML(Strea
+00004d10: 6d45 7272 6f72 293a 0a20 2020 2070 6173  mError):.    pas
+00004d20: 730a 0a63 6c61 7373 2053 6565 4f74 6865  s..class SeeOthe
+00004d30: 7248 6f73 7428 5374 7265 616d 4572 726f  rHost(StreamErro
+00004d40: 7229 3a0a 2020 2020 7061 7373 0a0a 636c  r):.    pass..cl
+00004d50: 6173 7320 5379 7374 656d 5368 7574 646f  ass SystemShutdo
+00004d60: 776e 2853 7472 6561 6d45 7272 6f72 293a  wn(StreamError):
+00004d70: 0a20 2020 2070 6173 730a 0a63 6c61 7373  .    pass..class
+00004d80: 2055 6e64 6566 696e 6564 436f 6e64 6974   UndefinedCondit
+00004d90: 696f 6e28 5374 7265 616d 4572 726f 7229  ion(StreamError)
+00004da0: 3a0a 2020 2020 7061 7373 0a0a 636c 6173  :.    pass..clas
+00004db0: 7320 556e 7375 7070 6f72 7465 6445 6e63  s UnsupportedEnc
+00004dc0: 6f64 696e 6728 5374 7265 616d 4572 726f  oding(StreamErro
+00004dd0: 7229 3a0a 2020 2020 7061 7373 0a0a 636c  r):.    pass..cl
+00004de0: 6173 7320 556e 7375 7070 6f72 7465 6453  ass UnsupportedS
+00004df0: 7461 6e7a 6154 7970 6528 5374 7265 616d  tanzaType(Stream
+00004e00: 4572 726f 7229 3a0a 2020 2020 7061 7373  Error):.    pass
+00004e10: 0a0a 636c 6173 7320 556e 7375 7070 6f72  ..class Unsuppor
+00004e20: 7465 6456 6572 7369 6f6e 2853 7472 6561  tedVersion(Strea
+00004e30: 6d45 7272 6f72 293a 0a20 2020 2070 6173  mError):.    pas
+00004e40: 730a 0a63 6c61 7373 2058 4d4c 4e6f 7457  s..class XMLNotW
+00004e50: 656c 6c46 6f72 6d65 6428 5374 7265 616d  ellFormed(Stream
+00004e60: 4572 726f 7229 3a0a 2020 2020 7061 7373  Error):.    pass
+00004e70: 0a0a 636c 6173 7320 496e 7661 6c69 6453  ..class InvalidS
+00004e80: 7461 6e7a 6128 4578 6365 7074 696f 6e29  tanza(Exception)
+00004e90: 3a0a 2020 2020 7061 7373 0a0a 636c 6173  :.    pass..clas
+00004ea0: 7320 496e 7661 6c69 644a 6964 2845 7863  s InvalidJid(Exc
+00004eb0: 6570 7469 6f6e 293a 0a20 2020 2070 6173  eption):.    pas
+00004ec0: 730a 0a63 6c61 7373 204c 6f63 616c 7061  s..class Localpa
+00004ed0: 7274 4279 7465 4c69 6d69 7428 496e 7661  rtByteLimit(Inva
+00004ee0: 6c69 644a 6964 293a 0a20 2020 2064 6566  lidJid):.    def
+00004ef0: 205f 5f69 6e69 745f 5f28 7365 6c66 293a   __init__(self):
+00004f00: 0a20 2020 2020 2020 2049 6e76 616c 6964  .        Invalid
+00004f10: 4a69 642e 5f5f 696e 6974 5f5f 2873 656c  Jid.__init__(sel
+00004f20: 662c 2027 4c6f 6361 6c70 6172 7420 6d75  f, 'Localpart mu
+00004f30: 7374 2062 6520 6265 7477 6565 6e20 3120  st be between 1 
+00004f40: 616e 6420 3130 3233 2062 7974 6573 2729  and 1023 bytes')
+00004f50: 0a0a 636c 6173 7320 4c6f 6361 6c70 6172  ..class Localpar
+00004f60: 744e 6f74 416c 6c6f 7765 6443 6861 7228  tNotAllowedChar(
+00004f70: 496e 7661 6c69 644a 6964 293a 0a20 2020  InvalidJid):.   
+00004f80: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00004f90: 6c66 293a 0a20 2020 2020 2020 2049 6e76  lf):.        Inv
+00004fa0: 616c 6964 4a69 642e 5f5f 696e 6974 5f5f  alidJid.__init__
+00004fb0: 2873 656c 662c 2027 4e6f 7420 616c 6c6f  (self, 'Not allo
+00004fc0: 7765 6420 6368 6172 6163 7465 7220 696e  wed character in
+00004fd0: 206c 6f63 616c 7061 7274 2729 0a0a 636c   localpart')..cl
+00004fe0: 6173 7320 5265 736f 7572 6365 7061 7274  ass Resourcepart
+00004ff0: 4279 7465 4c69 6d69 7428 496e 7661 6c69  ByteLimit(Invali
+00005000: 644a 6964 293a 0a20 2020 2064 6566 205f  dJid):.    def _
+00005010: 5f69 6e69 745f 5f28 7365 6c66 293a 0a20  _init__(self):. 
+00005020: 2020 2020 2020 2049 6e76 616c 6964 4a69         InvalidJi
+00005030: 642e 5f5f 696e 6974 5f5f 2873 656c 662c  d.__init__(self,
+00005040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005050: 2020 2020 2020 2020 2020 2020 2027 5265               'Re
+00005060: 736f 7572 6365 7061 7274 206d 7573 7420  sourcepart must 
+00005070: 6265 2062 6574 7765 656e 2031 2061 6e64  be between 1 and
+00005080: 2031 3032 3320 6279 7465 7327 290a 0a63   1023 bytes')..c
+00005090: 6c61 7373 2052 6573 6f75 7263 6570 6172  lass Resourcepar
+000050a0: 744e 6f74 416c 6c6f 7765 6443 6861 7228  tNotAllowedChar(
+000050b0: 496e 7661 6c69 644a 6964 293a 0a20 2020  InvalidJid):.   
+000050c0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000050d0: 6c66 293a 0a20 2020 2020 2020 2049 6e76  lf):.        Inv
+000050e0: 616c 6964 4a69 642e 5f5f 696e 6974 5f5f  alidJid.__init__
+000050f0: 2873 656c 662c 2027 4e6f 7420 616c 6c6f  (self, 'Not allo
+00005100: 7765 6420 6368 6172 6163 7465 7220 696e  wed character in
+00005110: 2072 6573 6f75 7263 6570 6172 7427 290a   resourcepart').
+00005120: 0a63 6c61 7373 2044 6f6d 6169 6e70 6172  .class Domainpar
+00005130: 7442 7974 654c 696d 6974 2849 6e76 616c  tByteLimit(Inval
+00005140: 6964 4a69 6429 3a0a 2020 2020 6465 6620  idJid):.    def 
+00005150: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0a  __init__(self):.
+00005160: 2020 2020 2020 2020 496e 7661 6c69 644a          InvalidJ
+00005170: 6964 2e5f 5f69 6e69 745f 5f28 7365 6c66  id.__init__(self
+00005180: 2c20 2744 6f6d 6169 6e70 6172 7420 6d75  , 'Domainpart mu
+00005190: 7374 2062 6520 6265 7477 6565 6e20 3120  st be between 1 
+000051a0: 616e 6420 3130 3233 2062 7974 6573 2729  and 1023 bytes')
+000051b0: 0a0a 636c 6173 7320 446f 6d61 696e 7061  ..class Domainpa
+000051c0: 7274 4e6f 7441 6c6c 6f77 6564 4368 6172  rtNotAllowedChar
+000051d0: 2849 6e76 616c 6964 4a69 6429 3a0a 2020  (InvalidJid):.  
+000051e0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+000051f0: 656c 6629 3a0a 2020 2020 2020 2020 496e  elf):.        In
+00005200: 7661 6c69 644a 6964 2e5f 5f69 6e69 745f  validJid.__init_
+00005210: 5f28 7365 6c66 2c20 274e 6f74 2061 6c6c  _(self, 'Not all
+00005220: 6f77 6564 2063 6861 7261 6374 6572 2069  owed character i
+00005230: 6e20 646f 6d61 696e 7061 7274 2729 0a0a  n domainpart')..
+00005240: 636c 6173 7320 5374 616e 7a61 4d61 6c66  class StanzaMalf
+00005250: 6f72 6d65 6428 4578 6365 7074 696f 6e29  ormed(Exception)
+00005260: 3a0a 2020 2020 7061 7373 0a0a 636c 6173  :.    pass..clas
+00005270: 7320 4469 7363 6f49 6e66 6f4d 616c 666f  s DiscoInfoMalfo
+00005280: 726d 6564 2845 7863 6570 7469 6f6e 293a  rmed(Exception):
+00005290: 0a20 2020 2070 6173 730a 0a73 7472 6561  .    pass..strea
+000052a0: 6d5f 6578 6365 7074 696f 6e73 203d 207b  m_exceptions = {
+000052b0: 2762 6164 2d66 6f72 6d61 7427 3a20 4261  'bad-format': Ba
+000052c0: 6446 6f72 6d61 742c 0a20 2020 2020 2020  dFormat,.       
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+000052e0: 6164 2d6e 616d 6573 7061 6365 2d70 7265  ad-namespace-pre
+000052f0: 6669 7827 3a20 4261 644e 616d 6573 7061  fix': BadNamespa
+00005300: 6365 5072 6566 6978 2c0a 2020 2020 2020  cePrefix,.      
+00005310: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005320: 636f 6e66 6c69 6374 273a 2043 6f6e 666c  conflict': Confl
+00005330: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
+00005340: 2020 2020 2020 2020 2020 2763 6f6e 6e65            'conne
+00005350: 6374 696f 6e2d 7469 6d65 6f75 7427 3a20  ction-timeout': 
+00005360: 436f 6e6e 6563 7469 6f6e 5469 6d65 6f75  ConnectionTimeou
+00005370: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00005380: 2020 2020 2020 2020 2768 6f73 742d 676f          'host-go
+00005390: 6e65 273a 2048 6f73 7447 6f6e 652c 0a20  ne': HostGone,. 
+000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053b0: 2020 2020 2768 6f73 742d 756e 6b6e 6f77      'host-unknow
+000053c0: 6e27 3a20 486f 7374 556e 6b6e 6f77 6e2c  n': HostUnknown,
+000053d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000053e0: 2020 2020 2020 2769 6d70 726f 7065 722d        'improper-
+000053f0: 6164 6472 6573 7369 6e67 273a 2049 6d70  addressing': Imp
+00005400: 726f 7065 7241 6464 7265 7373 696e 672c  roperAddressing,
+00005410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005420: 2020 2020 2020 2769 6e74 6572 6e61 6c2d        'internal-
+00005430: 7365 7276 6572 2d65 7272 6f72 273a 2049  server-error': I
+00005440: 6e74 6572 6e61 6c53 6572 7665 7245 7272  nternalServerErr
+00005450: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00005460: 2020 2020 2020 2020 2027 696e 7661 6c69           'invali
+00005470: 642d 6672 6f6d 273a 2049 6e76 616c 6964  d-from': Invalid
+00005480: 4672 6f6d 2c0a 2020 2020 2020 2020 2020  From,.          
+00005490: 2020 2020 2020 2020 2020 2027 696e 7661             'inva
+000054a0: 6c69 642d 6964 273a 2049 6e76 616c 6964  lid-id': Invalid
+000054b0: 4944 2c0a 2020 2020 2020 2020 2020 2020  ID,.            
+000054c0: 2020 2020 2020 2020 2027 696e 7661 6c69           'invali
+000054d0: 642d 6e61 6d65 7370 6163 6527 3a20 496e  d-namespace': In
+000054e0: 7661 6c69 644e 616d 6573 7061 6365 2c0a  validNamespace,.
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 2020 2020 2027 696e 7661 6c69 642d 786d       'invalid-xm
+00005510: 6c27 3a20 496e 7661 6c69 6458 4d4c 2c0a  l': InvalidXML,.
+00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005530: 2020 2020 2027 6e6f 742d 6175 7468 6f72       'not-author
+00005540: 697a 6564 273a 204e 6f74 4175 7468 6f72  ized': NotAuthor
+00005550: 697a 6564 2c0a 2020 2020 2020 2020 2020  ized,.          
+00005560: 2020 2020 2020 2020 2020 2027 706f 6c69             'poli
+00005570: 6379 2d76 696f 6c61 7469 6f6e 273a 2050  cy-violation': P
+00005580: 6f6c 6963 7956 696f 6c61 7469 6f6e 2c0a  olicyViolation,.
+00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055a0: 2020 2020 2027 7265 6d6f 7465 2d63 6f6e       'remote-con
+000055b0: 6e65 6374 696f 6e2d 6661 696c 6564 273a  nection-failed':
+000055c0: 2052 656d 6f74 6543 6f6e 6e65 6374 696f   RemoteConnectio
+000055d0: 6e46 6169 6c65 642c 0a20 2020 2020 2020  nFailed,.       
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+000055f0: 6573 6f75 7263 652d 636f 6e73 7472 6169  esource-constrai
+00005600: 6e74 273a 2052 6573 6f75 7263 6543 6f6e  nt': ResourceCon
+00005610: 7374 7261 696e 742c 0a20 2020 2020 2020  straint,.       
+00005620: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+00005630: 6573 7472 6963 7465 642d 786d 6c27 3a20  estricted-xml': 
+00005640: 5265 7374 7269 6374 6564 584d 4c2c 0a20  RestrictedXML,. 
+00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005660: 2020 2020 2773 6565 2d6f 7468 6572 2d68      'see-other-h
+00005670: 6f73 7427 3a20 5365 654f 7468 6572 486f  ost': SeeOtherHo
+00005680: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
+00005690: 2020 2020 2020 2020 2027 7379 7374 656d           'system
+000056a0: 2d73 6875 7464 6f77 6e27 3a20 5379 7374  -shutdown': Syst
+000056b0: 656d 5368 7574 646f 776e 2c0a 2020 2020  emShutdown,.    
+000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056d0: 2027 756e 6465 6669 6e65 642d 636f 6e64   'undefined-cond
+000056e0: 6974 696f 6e27 3a20 556e 6465 6669 6e65  ition': Undefine
+000056f0: 6443 6f6e 6469 7469 6f6e 2c0a 2020 2020  dCondition,.    
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2027 756e 7375 7070 6f72 7465 642d 656e   'unsupported-en
+00005720: 636f 6469 6e67 273a 2055 6e73 7570 706f  coding': Unsuppo
+00005730: 7274 6564 456e 636f 6469 6e67 2c0a 2020  rtedEncoding,.  
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 2020 2027 756e 7375 7070 6f72 7465 642d     'unsupported-
+00005760: 7374 616e 7a61 2d74 7970 6527 3a20 556e  stanza-type': Un
+00005770: 7375 7070 6f72 7465 6453 7461 6e7a 6154  supportedStanzaT
+00005780: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00005790: 2020 2020 2020 2020 2020 2775 6e73 7570            'unsup
+000057a0: 706f 7274 6564 2d76 6572 7369 6f6e 273a  ported-version':
+000057b0: 2055 6e73 7570 706f 7274 6564 5665 7273   UnsupportedVers
+000057c0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+000057d0: 2020 2020 2020 2020 2020 2778 6d6c 2d6e            'xml-n
+000057e0: 6f74 2d77 656c 6c2d 666f 726d 6564 273a  ot-well-formed':
+000057f0: 2058 4d4c 4e6f 7457 656c 6c46 6f72 6d65   XMLNotWellForme
+00005800: 647d 0a0a 0a64 6566 2064 6570 7265 6361  d}...def depreca
+00005810: 7469 6f6e 5f77 6172 6e69 6e67 286d 6573  tion_warning(mes
+00005820: 7361 6765 293a 0a20 2020 2077 6172 6e69  sage):.    warni
+00005830: 6e67 732e 7761 726e 286d 6573 7361 6765  ngs.warn(message
+00005840: 2c20 4465 7072 6563 6174 696f 6e57 6172  , DeprecationWar
+00005850: 6e69 6e67 290a 0a0a 4066 756e 6374 6f6f  ning)...@functoo
+00005860: 6c73 2e6c 7275 5f63 6163 6865 286d 6178  ls.lru_cache(max
+00005870: 7369 7a65 3d4e 6f6e 6529 0a64 6566 2076  size=None).def v
+00005880: 616c 6964 6174 655f 6c6f 6361 6c70 6172  alidate_localpar
+00005890: 7428 6c6f 6361 6c70 6172 743a 2073 7472  t(localpart: str
+000058a0: 2920 2d3e 2073 7472 3a0a 2020 2020 6966  ) -> str:.    if
+000058b0: 206e 6f74 206c 6f63 616c 7061 7274 206f   not localpart o
+000058c0: 7220 6c65 6e28 6c6f 6361 6c70 6172 742e  r len(localpart.
+000058d0: 656e 636f 6465 2829 2920 3e20 3130 3233  encode()) > 1023
+000058e0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+000058f0: 4c6f 6361 6c70 6172 7442 7974 654c 696d  LocalpartByteLim
+00005900: 6974 0a0a 2020 2020 6966 206f 732e 656e  it..    if os.en
+00005910: 7669 726f 6e2e 6765 7428 274e 4258 4d50  viron.get('NBXMP
+00005920: 505f 454e 464f 5243 455f 5052 4543 4953  P_ENFORCE_PRECIS
+00005930: 2729 2069 7320 4e6f 6e65 3a0a 2020 2020  ') is None:.    
+00005940: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00005950: 2020 2020 2072 6574 7572 6e20 6e6f 6465       return node
+00005960: 7072 6570 286c 6f63 616c 7061 7274 290a  prep(localpart).
+00005970: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00005980: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+00005990: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+000059a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000059b0: 6e20 656e 666f 7263 655f 7072 6563 6973  n enforce_precis
+000059c0: 5f75 7365 726e 616d 6528 6c6f 6361 6c70  _username(localp
+000059d0: 6172 7429 0a20 2020 2020 2020 2020 2020  art).           
+000059e0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000059f0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00005a00: 2020 2072 6169 7365 204c 6f63 616c 7061     raise Localpa
+00005a10: 7274 4e6f 7441 6c6c 6f77 6564 4368 6172  rtNotAllowedChar
+00005a20: 0a0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
+00005a30: 2020 2072 6574 7572 6e20 656e 666f 7263     return enforc
+00005a40: 655f 7072 6563 6973 5f75 7365 726e 616d  e_precis_usernam
+00005a50: 6528 6c6f 6361 6c70 6172 7429 0a20 2020  e(localpart).   
+00005a60: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00005a70: 6e3a 0a20 2020 2020 2020 2072 6169 7365  n:.        raise
+00005a80: 204c 6f63 616c 7061 7274 4e6f 7441 6c6c   LocalpartNotAll
+00005a90: 6f77 6564 4368 6172 0a0a 0a40 6675 6e63  owedChar...@func
+00005aa0: 746f 6f6c 732e 6c72 755f 6361 6368 6528  tools.lru_cache(
+00005ab0: 6d61 7873 697a 653d 4e6f 6e65 290a 6465  maxsize=None).de
+00005ac0: 6620 7661 6c69 6461 7465 5f72 6573 6f75  f validate_resou
+00005ad0: 7263 6570 6172 7428 7265 736f 7572 6365  rcepart(resource
+00005ae0: 7061 7274 3a20 7374 7229 202d 3e20 7374  part: str) -> st
+00005af0: 723a 0a20 2020 2069 6620 6e6f 7420 7265  r:.    if not re
+00005b00: 736f 7572 6365 7061 7274 206f 7220 6c65  sourcepart or le
+00005b10: 6e28 7265 736f 7572 6365 7061 7274 2e65  n(resourcepart.e
+00005b20: 6e63 6f64 6528 2929 203e 2031 3032 333a  ncode()) > 1023:
+00005b30: 0a20 2020 2020 2020 2072 6169 7365 2052  .        raise R
+00005b40: 6573 6f75 7263 6570 6172 7442 7974 654c  esourcepartByteL
+00005b50: 696d 6974 0a0a 2020 2020 6966 206f 732e  imit..    if os.
+00005b60: 656e 7669 726f 6e2e 6765 7428 274e 4258  environ.get('NBX
+00005b70: 4d50 505f 454e 464f 5243 455f 5052 4543  MPP_ENFORCE_PREC
+00005b80: 4953 2729 2069 7320 4e6f 6e65 3a0a 2020  IS') is None:.  
+00005b90: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00005ba0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00005bb0: 736f 7572 6365 7072 6570 2872 6573 6f75  sourceprep(resou
+00005bc0: 7263 6570 6172 7429 0a20 2020 2020 2020  rcepart).       
+00005bd0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00005be0: 6e3a 0a20 2020 2020 2020 2020 2020 2074  n:.            t
+00005bf0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00005c00: 2020 2020 7265 7475 726e 2065 6e66 6f72      return enfor
+00005c10: 6365 5f70 7265 6369 735f 6f70 6171 7565  ce_precis_opaque
+00005c20: 2872 6573 6f75 7263 6570 6172 7429 0a20  (resourcepart). 
+00005c30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00005c40: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
+00005c50: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00005c60: 7365 2052 6573 6f75 7263 6570 6172 744e  se ResourcepartN
+00005c70: 6f74 416c 6c6f 7765 6443 6861 720a 0a20  otAllowedChar.. 
+00005c80: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00005c90: 7265 7475 726e 2065 6e66 6f72 6365 5f70  return enforce_p
+00005ca0: 7265 6369 735f 6f70 6171 7565 2872 6573  recis_opaque(res
+00005cb0: 6f75 7263 6570 6172 7429 0a20 2020 2065  ourcepart).    e
+00005cc0: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
+00005cd0: 0a20 2020 2020 2020 2072 6169 7365 2052  .        raise R
+00005ce0: 6573 6f75 7263 6570 6172 744e 6f74 416c  esourcepartNotAl
+00005cf0: 6c6f 7765 6443 6861 720a 0a0a 4066 756e  lowedChar...@fun
+00005d00: 6374 6f6f 6c73 2e6c 7275 5f63 6163 6865  ctools.lru_cache
+00005d10: 286d 6178 7369 7a65 3d4e 6f6e 6529 0a64  (maxsize=None).d
+00005d20: 6566 2076 616c 6964 6174 655f 646f 6d61  ef validate_doma
+00005d30: 696e 7061 7274 2864 6f6d 6169 6e70 6172  inpart(domainpar
+00005d40: 743a 2073 7472 2920 2d3e 2073 7472 3a0a  t: str) -> str:.
+00005d50: 2020 2020 6966 206e 6f74 2064 6f6d 6169      if not domai
+00005d60: 6e70 6172 743a 0a20 2020 2020 2020 2072  npart:.        r
+00005d70: 6169 7365 2044 6f6d 6169 6e70 6172 7442  aise DomainpartB
+00005d80: 7974 654c 696d 6974 0a0a 2020 2020 6970  yteLimit..    ip
+00005d90: 5f61 6464 7265 7373 203d 2064 6f6d 6169  _address = domai
+00005da0: 6e70 6172 742e 7374 7269 7028 275b 5d27  npart.strip('[]'
+00005db0: 290a 2020 2020 6966 2047 4c69 622e 686f  ).    if GLib.ho
+00005dc0: 7374 6e61 6d65 5f69 735f 6970 5f61 6464  stname_is_ip_add
+00005dd0: 7265 7373 2869 705f 6164 6472 6573 7329  ress(ip_address)
+00005de0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00005df0: 2069 705f 6164 6472 6573 730a 0a20 2020   ip_address..   
+00005e00: 206c 656e 6774 6820 3d20 6c65 6e28 646f   length = len(do
+00005e10: 6d61 696e 7061 7274 2e65 6e63 6f64 6528  mainpart.encode(
+00005e20: 2929 0a20 2020 2069 6620 6c65 6e67 7468  )).    if length
+00005e30: 203d 3d20 3020 6f72 206c 656e 6774 6820   == 0 or length 
+00005e40: 3e20 3130 3233 3a0a 2020 2020 2020 2020  > 1023:.        
+00005e50: 7261 6973 6520 446f 6d61 696e 7061 7274  raise Domainpart
+00005e60: 4279 7465 4c69 6d69 740a 0a20 2020 2069  ByteLimit..    i
+00005e70: 6620 646f 6d61 696e 7061 7274 2e65 6e64  f domainpart.end
+00005e80: 7377 6974 6828 272e 2729 3a20 2023 2052  swith('.'):  # R
+00005e90: 4643 3736 3232 2c20 332e 320a 2020 2020  FC7622, 3.2.    
+00005ea0: 2020 2020 646f 6d61 696e 7061 7274 203d      domainpart =
+00005eb0: 2064 6f6d 6169 6e70 6172 745b 3a2d 315d   domainpart[:-1]
+00005ec0: 0a0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
+00005ed0: 2020 2064 6f6d 6169 6e70 6172 7420 3d20     domainpart = 
+00005ee0: 6964 6e61 3230 3038 5f70 7265 7028 646f  idna2008_prep(do
+00005ef0: 6d61 696e 7061 7274 290a 2020 2020 6578  mainpart).    ex
+00005f00: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
+00005f10: 2020 2020 2020 2020 7261 6973 6520 446f          raise Do
+00005f20: 6d61 696e 7061 7274 4e6f 7441 6c6c 6f77  mainpartNotAllow
+00005f30: 6564 4368 6172 0a0a 2020 2020 7265 7475  edChar..    retu
+00005f40: 726e 2064 6f6d 6169 6e70 6172 740a 0a0a  rn domainpart...
+00005f50: 4066 756e 6374 6f6f 6c73 2e6c 7275 5f63  @functools.lru_c
+00005f60: 6163 6865 286d 6178 7369 7a65 3d4e 6f6e  ache(maxsize=Non
+00005f70: 6529 0a64 6566 2069 646e 6132 3030 385f  e).def idna2008_
+00005f80: 7072 6570 2864 6f6d 6169 6e3a 2073 7472  prep(domain: str
+00005f90: 2c20 746f 5f61 7363 6969 3a20 626f 6f6c  , to_ascii: bool
+00005fa0: 203d 2046 616c 7365 2920 2d3e 2073 7472   = False) -> str
+00005fb0: 3a0a 2020 2020 2727 270a 2020 2020 5072  :.    '''.    Pr
+00005fc0: 6570 6172 6520 7769 7468 2055 5453 3436  epare with UTS46
+00005fd0: 2063 6173 6520 6d61 7070 696e 6720 746f   case mapping to
+00005fe0: 2073 7461 7920 636f 6d70 6174 6962 656c   stay compatibel
+00005ff0: 2077 6974 6820 7468 6520 4944 4e41 3230   with the IDNA20
+00006000: 3033 0a20 2020 206d 6170 7069 6e67 2e20  03.    mapping. 
+00006010: 4675 7274 6865 7220 7472 7920 746f 2065  Further try to e
+00006020: 6e63 6f64 6520 7468 6520 646f 6d61 696e  ncode the domain
+00006030: 2074 6f20 6361 7463 6820 696c 6c65 6761   to catch illega
+00006040: 6c20 646f 6d61 696e 732e 0a20 2020 204f  l domains..    O
+00006050: 6e6c 7920 7265 7475 726e 2074 6865 2063  nly return the c
+00006060: 6173 6520 6d61 7070 6564 2064 6f6d 6169  ase mapped domai
+00006070: 6e20 6265 6361 7573 6520 6f6e 2074 6865  n because on the
+00006080: 2058 4d50 5020 7769 7265 2c55 5446 3820   XMPP wire,UTF8 
+00006090: 646f 6d61 696e 730a 2020 2020 6172 6520  domains.    are 
+000060a0: 6669 6e65 2e0a 2020 2020 2727 270a 2020  fine..    '''.  
+000060b0: 2020 646f 6d61 696e 203d 2069 646e 612e    domain = idna.
+000060c0: 7574 7334 365f 7265 6d61 7028 646f 6d61  uts46_remap(doma
+000060d0: 696e 290a 2020 2020 656e 636f 6465 645f  in).    encoded_
+000060e0: 646f 6d61 696e 203d 2069 646e 612e 656e  domain = idna.en
+000060f0: 636f 6465 2864 6f6d 6169 6e29 0a20 2020  code(domain).   
+00006100: 2069 6620 746f 5f61 7363 6969 3a0a 2020   if to_ascii:.  
+00006110: 2020 2020 2020 7265 7475 726e 2065 6e63        return enc
+00006120: 6f64 6564 5f64 6f6d 6169 6e2e 6465 636f  oded_domain.deco
+00006130: 6465 2829 0a20 2020 2072 6574 7572 6e20  de().    return 
+00006140: 646f 6d61 696e 0a0a 0a40 6675 6e63 746f  domain...@functo
+00006150: 6f6c 732e 6c72 755f 6361 6368 6528 6d61  ols.lru_cache(ma
+00006160: 7873 697a 653d 4e6f 6e65 290a 6465 6620  xsize=None).def 
+00006170: 6573 6361 7065 5f6c 6f63 616c 7061 7274  escape_localpart
+00006180: 286c 6f63 616c 7061 7274 3a20 7374 7229  (localpart: str)
+00006190: 202d 3e20 7374 723a 0a20 2020 2023 2068   -> str:.    # h
+000061a0: 7474 7073 3a2f 2f78 6d70 702e 6f72 672f  ttps://xmpp.org/
+000061b0: 6578 7465 6e73 696f 6e73 2f78 6570 2d30  extensions/xep-0
+000061c0: 3130 362e 6874 6d6c 2362 697a 7275 6c65  106.html#bizrule
+000061d0: 732d 616c 676f 7269 7468 6d0a 2020 2020  s-algorithm.    
+000061e0: 230a 2020 2020 2320 4966 2074 6865 7265  #.    # If there
+000061f0: 2061 7265 2061 6e79 2069 6e73 7461 6e63   are any instanc
+00006200: 6573 206f 6620 6368 6172 6163 7465 7220  es of character 
+00006210: 7365 7175 656e 6365 7320 7468 6174 2063  sequences that c
+00006220: 6f72 7265 7370 6f6e 640a 2020 2020 2320  orrespond.    # 
+00006230: 746f 2065 7363 6170 696e 6773 206f 6620  to escapings of 
+00006240: 7468 6520 6469 7361 6c6c 6f77 6564 2063  the disallowed c
+00006250: 6861 7261 6374 6572 730a 2020 2020 2320  haracters.    # 
+00006260: 2865 2e67 2e2c 2074 6865 2063 6861 7261  (e.g., the chara
+00006270: 6374 6572 2073 6571 7565 6e63 6520 225c  cter sequence "\
+00006280: 3237 2229 206f 7220 7468 6520 6573 6361  27") or the esca
+00006290: 7069 6e67 2063 6861 7261 6374 6572 0a20  ping character. 
+000062a0: 2020 2023 2028 692e 652e 2c20 7468 6520     # (i.e., the 
+000062b0: 6368 6172 6163 7465 7220 7365 7175 656e  character sequen
+000062c0: 6365 2022 5c35 6322 2920 696e 2074 6865  ce "\5c") in the
+000062d0: 2073 6f75 7263 6520 6164 6472 6573 732c   source address,
+000062e0: 0a20 2020 2023 2074 6865 206c 6561 6469  .    # the leadi
+000062f0: 6e67 2062 6163 6b73 6c61 7368 2063 6861  ng backslash cha
+00006300: 7261 6374 6572 204d 5553 5420 6265 2065  racter MUST be e
+00006310: 7363 6170 6564 2074 6f20 7468 6520 6368  scaped to the ch
+00006320: 6172 6163 7465 720a 2020 2020 2320 7365  aracter.    # se
+00006330: 7175 656e 6365 2022 5c35 6322 0a0a 2020  quence "\5c"..  
+00006340: 2020 666f 7220 6368 6172 2069 6e20 275c    for char in '\
+00006350: 5c27 202b 205f 6c6f 6361 6c70 6172 745f  \' + _localpart_
+00006360: 6573 6361 7065 5f63 6861 7273 3a0a 2020  escape_chars:.  
+00006370: 2020 2020 2020 7365 7120 3d20 225c 5c7b        seq = "\\{
+00006380: 3a30 3278 7d22 2e66 6f72 6d61 7428 6f72  :02x}".format(or
+00006390: 6428 6368 6172 2929 0a20 2020 2020 2020  d(char)).       
+000063a0: 206c 6f63 616c 7061 7274 203d 206c 6f63   localpart = loc
+000063b0: 616c 7061 7274 2e72 6570 6c61 6365 2873  alpart.replace(s
+000063c0: 6571 2c20 225c 5c35 637b 3a30 3278 7d22  eq, "\\5c{:02x}"
+000063d0: 2e66 6f72 6d61 7428 6f72 6428 6368 6172  .format(ord(char
+000063e0: 2929 290a 0a20 2020 2023 2045 7363 6170  )))..    # Escap
+000063f0: 6520 616c 6c20 6f74 6865 7220 6368 6172  e all other char
+00006400: 730a 2020 2020 666f 7220 6368 6172 2069  s.    for char i
+00006410: 6e20 5f6c 6f63 616c 7061 7274 5f65 7363  n _localpart_esc
+00006420: 6170 655f 6368 6172 733a 0a20 2020 2020  ape_chars:.     
+00006430: 2020 206c 6f63 616c 7061 7274 203d 206c     localpart = l
+00006440: 6f63 616c 7061 7274 2e72 6570 6c61 6365  ocalpart.replace
+00006450: 2863 6861 722c 2022 5c5c 7b3a 3032 787d  (char, "\\{:02x}
+00006460: 222e 666f 726d 6174 286f 7264 2863 6861  ".format(ord(cha
+00006470: 7229 2929 0a0a 2020 2020 7265 7475 726e  r)))..    return
+00006480: 206c 6f63 616c 7061 7274 0a0a 0a40 6675   localpart...@fu
+00006490: 6e63 746f 6f6c 732e 6c72 755f 6361 6368  nctools.lru_cach
+000064a0: 6528 6d61 7873 697a 653d 4e6f 6e65 290a  e(maxsize=None).
+000064b0: 6465 6620 756e 6573 6361 7065 5f6c 6f63  def unescape_loc
+000064c0: 616c 7061 7274 286c 6f63 616c 7061 7274  alpart(localpart
+000064d0: 3a20 7374 7229 202d 3e20 7374 723a 0a20  : str) -> str:. 
+000064e0: 2020 2069 6620 6c6f 6361 6c70 6172 742e     if localpart.
+000064f0: 7374 6172 7473 7769 7468 2827 5c5c 3230  startswith('\\20
+00006500: 2729 206f 7220 6c6f 6361 6c70 6172 742e  ') or localpart.
+00006510: 656e 6473 7769 7468 2827 5c5c 3230 2729  endswith('\\20')
+00006520: 3a0a 2020 2020 2020 2020 2320 4573 6361  :.        # Esca
+00006530: 7065 6420 4a49 4473 2061 7265 206e 6f74  ped JIDs are not
+00006540: 2061 6c6c 6f77 6564 2074 6f20 7374 6172   allowed to star
+00006550: 7420 6f72 2065 6e64 2077 6974 6820 5c32  t or end with \2
+00006560: 300a 2020 2020 2020 2020 2320 736f 2074  0.        # so t
+00006570: 6869 7320 6c6f 6361 6c70 6172 7420 6d75  his localpart mu
+00006580: 7374 2062 6520 616c 7265 6164 7920 756e  st be already un
+00006590: 6573 6361 7065 640a 2020 2020 2020 2020  escaped.        
+000065a0: 7265 7475 726e 206c 6f63 616c 7061 7274  return localpart
+000065b0: 0a0a 2020 2020 666f 7220 6368 6172 2069  ..    for char i
+000065c0: 6e20 5f6c 6f63 616c 7061 7274 5f65 7363  n _localpart_esc
+000065d0: 6170 655f 6368 6172 733a 0a20 2020 2020  ape_chars:.     
+000065e0: 2020 2073 6571 203d 2022 5c5c 7b3a 3032     seq = "\\{:02
+000065f0: 787d 222e 666f 726d 6174 286f 7264 2863  x}".format(ord(c
+00006600: 6861 7229 290a 2020 2020 2020 2020 6c6f  har)).        lo
+00006610: 6361 6c70 6172 7420 3d20 6c6f 6361 6c70  calpart = localp
+00006620: 6172 742e 7265 706c 6163 6528 7365 712c  art.replace(seq,
+00006630: 2063 6861 7229 0a0a 2020 2020 666f 7220   char)..    for 
+00006640: 6368 6172 2069 6e20 5f6c 6f63 616c 7061  char in _localpa
+00006650: 7274 5f65 7363 6170 655f 6368 6172 7320  rt_escape_chars 
+00006660: 2b20 225c 5c22 3a0a 2020 2020 2020 2020  + "\\":.        
+00006670: 7365 7120 3d20 225c 5c35 637b 3a30 3278  seq = "\\5c{:02x
+00006680: 7d22 2e66 6f72 6d61 7428 6f72 6428 6368  }".format(ord(ch
+00006690: 6172 2929 0a20 2020 2020 2020 206c 6f63  ar)).        loc
+000066a0: 616c 7061 7274 203d 206c 6f63 616c 7061  alpart = localpa
+000066b0: 7274 2e72 6570 6c61 6365 2873 6571 2c20  rt.replace(seq, 
+000066c0: 225c 5c7b 3a30 3278 7d22 2e66 6f72 6d61  "\\{:02x}".forma
+000066d0: 7428 6f72 6428 6368 6172 2929 290a 0a20  t(ord(char))).. 
+000066e0: 2020 2072 6574 7572 6e20 6c6f 6361 6c70     return localp
+000066f0: 6172 740a 0a0a 4064 6174 6163 6c61 7373  art...@dataclass
+00006700: 2866 726f 7a65 6e3d 5472 7565 290a 636c  (frozen=True).cl
+00006710: 6173 7320 4a49 443a 0a20 2020 206c 6f63  ass JID:.    loc
+00006720: 616c 7061 7274 3a20 4f70 7469 6f6e 616c  alpart: Optional
+00006730: 5b73 7472 5d20 3d20 4e6f 6e65 0a20 2020  [str] = None.   
+00006740: 2064 6f6d 6169 6e3a 204f 7074 696f 6e61   domain: Optiona
+00006750: 6c5b 7374 725d 203d 204e 6f6e 650a 2020  l[str] = None.  
+00006760: 2020 7265 736f 7572 6365 3a20 4f70 7469    resource: Opti
+00006770: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00006780: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00006790: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
+000067a0: 2020 2020 2020 2020 2020 6c6f 6361 6c70            localp
+000067b0: 6172 743a 204f 7074 696f 6e61 6c5b 7374  art: Optional[st
+000067c0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000067d0: 2020 2020 2020 2020 2020 2020 646f 6d61              doma
+000067e0: 696e 3a20 4f70 7469 6f6e 616c 5b73 7472  in: Optional[str
+000067f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00006800: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+00006810: 7263 653a 204f 7074 696f 6e61 6c5b 7374  rce: Optional[st
+00006820: 725d 203d 204e 6f6e 6529 3a0a 0a20 2020  r] = None):..   
+00006830: 2020 2020 2069 6620 6c6f 6361 6c70 6172       if localpar
+00006840: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00006850: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+00006860: 7061 7274 203d 2076 616c 6964 6174 655f  part = validate_
+00006870: 6c6f 6361 6c70 6172 7428 6c6f 6361 6c70  localpart(localp
+00006880: 6172 7429 0a20 2020 2020 2020 2020 2020  art).           
+00006890: 206f 626a 6563 742e 5f5f 7365 7461 7474   object.__setatt
+000068a0: 725f 5f28 7365 6c66 2c20 226c 6f63 616c  r__(self, "local
+000068b0: 7061 7274 222c 206c 6f63 616c 7061 7274  part", localpart
+000068c0: 290a 0a20 2020 2020 2020 2064 6f6d 6169  )..        domai
+000068d0: 6e20 3d20 7661 6c69 6461 7465 5f64 6f6d  n = validate_dom
+000068e0: 6169 6e70 6172 7428 646f 6d61 696e 290a  ainpart(domain).
+000068f0: 2020 2020 2020 2020 6f62 6a65 6374 2e5f          object._
+00006900: 5f73 6574 6174 7472 5f5f 2873 656c 662c  _setattr__(self,
+00006910: 2022 646f 6d61 696e 222c 2064 6f6d 6169   "domain", domai
+00006920: 6e29 0a0a 2020 2020 2020 2020 6966 2072  n)..        if r
+00006930: 6573 6f75 7263 6520 6973 206e 6f74 204e  esource is not N
+00006940: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006950: 2072 6573 6f75 7263 6520 3d20 7661 6c69   resource = vali
+00006960: 6461 7465 5f72 6573 6f75 7263 6570 6172  date_resourcepar
+00006970: 7428 7265 736f 7572 6365 290a 2020 2020  t(resource).    
+00006980: 2020 2020 2020 2020 6f62 6a65 6374 2e5f          object._
+00006990: 5f73 6574 6174 7472 5f5f 2873 656c 662c  _setattr__(self,
+000069a0: 2022 7265 736f 7572 6365 222c 2072 6573   "resource", res
+000069b0: 6f75 7263 6529 0a0a 2020 2020 4063 6c61  ource)..    @cla
+000069c0: 7373 6d65 7468 6f64 0a20 2020 2040 6675  ssmethod.    @fu
+000069d0: 6e63 746f 6f6c 732e 6c72 755f 6361 6368  nctools.lru_cach
+000069e0: 6528 6d61 7873 697a 653d 4e6f 6e65 290a  e(maxsize=None).
+000069f0: 2020 2020 6465 6620 6672 6f6d 5f73 7472      def from_str
+00006a00: 696e 6728 636c 732c 206a 6964 5f73 7472  ing(cls, jid_str
+00006a10: 696e 673a 2073 7472 2c20 666f 7263 655f  ing: str, force_
+00006a20: 6261 7265 3a20 626f 6f6c 203d 2046 616c  bare: bool = Fal
+00006a30: 7365 2920 2d3e 204a 4944 3a0a 2020 2020  se) -> JID:.    
+00006a40: 2020 2020 2320 6874 7470 733a 2f2f 746f      # https://to
+00006a50: 6f6c 732e 6965 7466 2e6f 7267 2f68 746d  ols.ietf.org/htm
+00006a60: 6c2f 7266 6337 3632 3223 7365 6374 696f  l/rfc7622#sectio
+00006a70: 6e2d 332e 320a 0a20 2020 2020 2020 2023  n-3.2..        #
+00006a80: 2052 656d 6f76 6520 616e 7920 706f 7274   Remove any port
+00006a90: 696f 6e20 6672 6f6d 2074 6865 2066 6972  ion from the fir
+00006aa0: 7374 2027 2f27 2063 6861 7261 6374 6572  st '/' character
+00006ab0: 2074 6f20 7468 6520 656e 6420 6f66 2074   to the end of t
+00006ac0: 6865 0a20 2020 2020 2020 2023 2073 7472  he.        # str
+00006ad0: 696e 6720 2869 6620 7468 6572 6520 6973  ing (if there is
+00006ae0: 2061 2027 2f27 2063 6861 7261 6374 6572   a '/' character
+00006af0: 2070 7265 7365 6e74 292e 0a0a 2020 2020   present)...    
+00006b00: 2020 2020 2320 5265 6d6f 7665 2061 6e79      # Remove any
+00006b10: 2070 6f72 7469 6f6e 2066 726f 6d20 7468   portion from th
+00006b20: 6520 6265 6769 6e6e 696e 6720 6f66 2074  e beginning of t
+00006b30: 6865 2073 7472 696e 6720 746f 2074 6865  he string to the
+00006b40: 2066 6972 7374 0a20 2020 2020 2020 2023   first.        #
+00006b50: 2027 4027 2063 6861 7261 6374 6572 2028   '@' character (
+00006b60: 6966 2074 6865 7265 2069 7320 616e 2027  if there is an '
+00006b70: 4027 2063 6861 7261 6374 6572 2070 7265  @' character pre
+00006b80: 7365 6e74 292e 0a0a 2020 2020 2020 2020  sent)...        
+00006b90: 6966 206a 6964 5f73 7472 696e 672e 6669  if jid_string.fi
+00006ba0: 6e64 2827 2f27 2920 213d 202d 313a 0a20  nd('/') != -1:. 
+00006bb0: 2020 2020 2020 2020 2020 2072 6573 742c             rest,
+00006bc0: 2072 6573 6f75 7263 6570 6172 7420 3d20   resourcepart = 
+00006bd0: 6a69 645f 7374 7269 6e67 2e73 706c 6974  jid_string.split
+00006be0: 2827 2f27 2c20 3129 0a20 2020 2020 2020  ('/', 1).       
+00006bf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006c00: 2020 2072 6573 742c 2072 6573 6f75 7263     rest, resourc
+00006c10: 6570 6172 7420 3d20 6a69 645f 7374 7269  epart = jid_stri
+00006c20: 6e67 2c20 4e6f 6e65 0a0a 2020 2020 2020  ng, None..      
+00006c30: 2020 6966 2072 6573 742e 6669 6e64 2827    if rest.find('
+00006c40: 4027 2920 213d 202d 313a 0a20 2020 2020  @') != -1:.     
+00006c50: 2020 2020 2020 206c 6f63 616c 7061 7274         localpart
+00006c60: 2c20 646f 6d61 696e 7061 7274 203d 2072  , domainpart = r
+00006c70: 6573 742e 7370 6c69 7428 2740 272c 2031  est.split('@', 1
+00006c80: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00006c90: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00006ca0: 6c70 6172 742c 2064 6f6d 6169 6e70 6172  lpart, domainpar
+00006cb0: 7420 3d20 4e6f 6e65 2c20 7265 7374 0a0a  t = None, rest..
+00006cc0: 2020 2020 2020 2020 6966 2066 6f72 6365          if force
+00006cd0: 5f62 6172 653a 0a20 2020 2020 2020 2020  _bare:.         
+00006ce0: 2020 2069 6620 6c6f 6361 6c70 6172 7420     if localpart 
+00006cf0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00006d00: 2020 2020 2020 2020 2072 6169 7365 204c           raise L
+00006d10: 6f63 616c 7061 7274 4279 7465 4c69 6d69  ocalpartByteLimi
+00006d20: 740a 2020 2020 2020 2020 2020 2020 7265  t.            re
+00006d30: 736f 7572 6365 7061 7274 203d 204e 6f6e  sourcepart = Non
+00006d40: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+00006d50: 6e20 636c 7328 6c6f 6361 6c70 6172 743d  n cls(localpart=
+00006d60: 6c6f 6361 6c70 6172 742c 0a20 2020 2020  localpart,.     
+00006d70: 2020 2020 2020 2020 2020 2020 2020 646f                do
+00006d80: 6d61 696e 3d64 6f6d 6169 6e70 6172 742c  main=domainpart,
+00006d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006da0: 2020 2020 7265 736f 7572 6365 3d72 6573      resource=res
+00006db0: 6f75 7263 6570 6172 7429 0a0a 2020 2020  ourcepart)..    
+00006dc0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00006dd0: 2040 6675 6e63 746f 6f6c 732e 6c72 755f   @functools.lru_
+00006de0: 6361 6368 6528 6d61 7873 697a 653d 4e6f  cache(maxsize=No
+00006df0: 6e65 290a 2020 2020 6465 6620 6672 6f6d  ne).    def from
+00006e00: 5f75 7365 725f 696e 7075 7428 636c 732c  _user_input(cls,
+00006e10: 2075 7365 725f 696e 7075 743a 2073 7472   user_input: str
+00006e20: 2c20 6573 6361 7065 643a 2062 6f6f 6c20  , escaped: bool 
+00006e30: 3d20 4661 6c73 6529 202d 3e20 4a49 443a  = False) -> JID:
+00006e40: 0a20 2020 2020 2020 2023 2055 7365 2074  .        # Use t
+00006e50: 6869 7320 6966 2077 6520 7761 6e74 204a  his if we want J
+00006e60: 4944 7320 746f 2062 6520 6573 6361 7065  IDs to be escape
+00006e70: 6420 6163 636f 7264 696e 6720 746f 2058  d according to X
+00006e80: 4550 2d30 3130 360a 2020 2020 2020 2020  EP-0106.        
+00006e90: 2320 5468 6520 7374 616e 6461 7264 204a  # The standard J
+00006ea0: 4944 2070 6172 7369 6e67 2063 616e 6e6f  ID parsing canno
+00006eb0: 7420 6265 2061 7070 6c69 6564 2062 6563  t be applied bec
+00006ec0: 6175 7365 2075 7365 725f 696e 7075 7420  ause user_input 
+00006ed0: 6973 0a20 2020 2020 2020 2023 206e 6f74  is.        # not
+00006ee0: 2061 2076 616c 6964 204a 4944 2e0a 0a20   a valid JID... 
+00006ef0: 2020 2020 2020 2023 204f 6e6c 7920 7573         # Only us
+00006f00: 6572 5f69 6e70 7574 2077 6869 6368 2061  er_input which a
+00006f10: 6674 6572 2065 7363 6170 696e 6720 7265  fter escaping re
+00006f20: 7375 6c74 2069 6e20 6120 6261 7265 204a  sult in a bare J
+00006f30: 4944 2063 616e 2062 650a 2020 2020 2020  ID can be.      
+00006f40: 2020 2320 7375 6363 6573 7366 756c 6c79    # successfully
+00006f50: 2070 6172 7365 642e 0a0a 2020 2020 2020   parsed...      
+00006f60: 2020 2320 5468 6520 6173 7375 6d70 7574    # The assumput
+00006f70: 696f 6e20 6973 2075 7365 725f 696e 7075  ion is user_inpu
+00006f80: 7420 6973 2061 2062 6172 6520 4a49 4420  t is a bare JID 
+00006f90: 736f 2077 6520 7374 6172 7420 7769 7468  so we start with
+00006fa0: 2061 6e0a 2020 2020 2020 2020 2320 7273   an.        # rs
+00006fb0: 706c 6974 206f 6e20 4020 6265 6361 7573  plit on @ becaus
+00006fc0: 6520 7765 2061 7373 756d 6520 7468 6572  e we assume ther
+00006fd0: 6520 6973 206e 6f20 7265 736f 7572 6365  e is no resource
+00006fe0: 2c20 736f 2074 6865 2063 6861 7220 400a  , so the char @.
+00006ff0: 2020 2020 2020 2020 2320 696e 2074 6865          # in the
+00007000: 206c 6f63 616c 7061 7274 2063 616e 206c   localpart can l
+00007010: 6174 6572 2062 6520 6573 6361 7065 642e  ater be escaped.
+00007020: 0a0a 2020 2020 2020 2020 6966 2065 7363  ..        if esc
+00007030: 6170 6564 3a0a 2020 2020 2020 2020 2020  aped:.          
+00007040: 2020 2320 666f 7220 636f 6e76 656e 6965    # for convenie
+00007050: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+00007060: 7265 7475 726e 2063 6c73 2e66 726f 6d5f  return cls.from_
+00007070: 7374 7269 6e67 2875 7365 725f 696e 7075  string(user_inpu
+00007080: 7429 0a0a 2020 2020 2020 2020 6966 2027  t)..        if '
+00007090: 4027 2069 6e20 7573 6572 5f69 6e70 7574  @' in user_input
+000070a0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+000070b0: 6361 6c70 6172 742c 2064 6f6d 6169 6e70  calpart, domainp
+000070c0: 6172 7420 3d20 7573 6572 5f69 6e70 7574  art = user_input
+000070d0: 2e72 7370 6c69 7428 2740 272c 2031 290a  .rsplit('@', 1).
+000070e0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000070f0: 6f63 616c 7061 7274 2e73 7461 7274 7377  ocalpart.startsw
+00007100: 6974 6828 2720 2729 206f 7220 6c6f 6361  ith(' ') or loca
+00007110: 6c70 6172 742e 656e 6473 7769 7468 2827  lpart.endswith('
+00007120: 2027 293a 0a20 2020 2020 2020 2020 2020   '):.           
+00007130: 2020 2020 2072 6169 7365 204c 6f63 616c       raise Local
+00007140: 7061 7274 4e6f 7441 6c6c 6f77 6564 4368  partNotAllowedCh
+00007150: 6172 0a0a 2020 2020 2020 2020 2020 2020  ar..            
+00007160: 6c6f 6361 6c70 6172 7420 3d20 6573 6361  localpart = esca
+00007170: 7065 5f6c 6f63 616c 7061 7274 286c 6f63  pe_localpart(loc
+00007180: 616c 7061 7274 290a 0a20 2020 2020 2020  alpart)..       
+00007190: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000071a0: 2020 206c 6f63 616c 7061 7274 203d 204e     localpart = N
+000071b0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000071c0: 646f 6d61 696e 7061 7274 203d 2075 7365  domainpart = use
+000071d0: 725f 696e 7075 740a 0a20 2020 2020 2020  r_input..       
+000071e0: 2072 6574 7572 6e20 636c 7328 6c6f 6361   return cls(loca
+000071f0: 6c70 6172 743d 6c6f 6361 6c70 6172 742c  lpart=localpart,
+00007200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007210: 2020 2020 646f 6d61 696e 3d64 6f6d 6169      domain=domai
+00007220: 6e70 6172 742c 0a20 2020 2020 2020 2020  npart,.         
+00007230: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+00007240: 6365 3d4e 6f6e 6529 0a0a 2020 2020 6465  ce=None)..    de
+00007250: 6620 5f5f 7374 725f 5f28 7365 6c66 2920  f __str__(self) 
+00007260: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+00007270: 6966 2073 656c 662e 6c6f 6361 6c70 6172  if self.localpar
+00007280: 743a 0a20 2020 2020 2020 2020 2020 206a  t:.            j
+00007290: 6964 203d 2066 277b 7365 6c66 2e6c 6f63  id = f'{self.loc
+000072a0: 616c 7061 7274 7d40 7b73 656c 662e 646f  alpart}@{self.do
+000072b0: 6d61 696e 7d27 0a20 2020 2020 2020 2065  main}'.        e
+000072c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000072d0: 206a 6964 203d 2063 6173 7428 7374 722c   jid = cast(str,
+000072e0: 2073 656c 662e 646f 6d61 696e 290a 0a20   self.domain).. 
+000072f0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00007300: 6573 6f75 7263 6520 6973 206e 6f74 204e  esource is not N
+00007310: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007320: 2072 6574 7572 6e20 6627 7b6a 6964 7d2f   return f'{jid}/
+00007330: 7b73 656c 662e 7265 736f 7572 6365 7d27  {self.resource}'
+00007340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007350: 6a69 640a 0a20 2020 2064 6566 205f 5f63  jid..    def __c
+00007360: 6f6e 666f 726d 5f5f 2873 656c 662c 2070  onform__(self, p
+00007370: 726f 746f 636f 6c3a 2073 716c 6974 6533  rotocol: sqlite3
+00007380: 2e50 7265 7061 7265 5072 6f74 6f63 6f6c  .PrepareProtocol
+00007390: 293a 0a20 2020 2020 2020 2069 6620 7072  ):.        if pr
+000073a0: 6f74 6f63 6f6c 2069 7320 7371 6c69 7465  otocol is sqlite
+000073b0: 332e 5072 6570 6172 6550 726f 746f 636f  3.PrepareProtoco
+000073c0: 6c3a 0a20 2020 2020 2020 2020 2020 2072  l:.            r
+000073d0: 6574 7572 6e20 7374 7228 7365 6c66 290a  eturn str(self).
+000073e0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+000073f0: 6c75 6545 7272 6f72 0a0a 2020 2020 6465  lueError..    de
+00007400: 6620 5f5f 6861 7368 5f5f 2873 656c 6629  f __hash__(self)
+00007410: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00007420: 2068 6173 6828 7374 7228 7365 6c66 2929   hash(str(self))
+00007430: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
+00007440: 2873 656c 662c 206f 7468 6572 3a20 556e  (self, other: Un
+00007450: 696f 6e5b 7374 722c 204a 4944 5d29 202d  ion[str, JID]) -
+00007460: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00007470: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00007480: 6865 722c 2073 7472 293a 0a20 2020 2020  her, str):.     
+00007490: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000074a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000074b0: 726e 204a 4944 2e66 726f 6d5f 7374 7269  rn JID.from_stri
+000074c0: 6e67 286f 7468 6572 2920 3d3d 2073 656c  ng(other) == sel
+000074d0: 660a 2020 2020 2020 2020 2020 2020 6578  f.            ex
+000074e0: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
+000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007500: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
+00007510: 2020 2020 2020 7265 7475 726e 2028 7365        return (se
+00007520: 6c66 2e6c 6f63 616c 7061 7274 203d 3d20  lf.localpart == 
+00007530: 6f74 6865 722e 6c6f 6361 6c70 6172 7420  other.localpart 
+00007540: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00007550: 2020 2020 7365 6c66 2e64 6f6d 6169 6e20      self.domain 
+00007560: 3d3d 206f 7468 6572 2e64 6f6d 6169 6e20  == other.domain 
+00007570: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00007580: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
+00007590: 6520 3d3d 206f 7468 6572 2e72 6573 6f75  e == other.resou
+000075a0: 7263 6529 0a0a 2020 2020 6465 6620 5f5f  rce)..    def __
+000075b0: 6e65 5f5f 2873 656c 662c 206f 7468 6572  ne__(self, other
+000075c0: 3a20 556e 696f 6e5b 7374 722c 204a 4944  : Union[str, JID
+000075d0: 5d29 202d 3e20 626f 6f6c 3a0a 2020 2020  ]) -> bool:.    
+000075e0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+000075f0: 656c 662e 5f5f 6571 5f5f 286f 7468 6572  elf.__eq__(other
+00007600: 290a 0a20 2020 2064 6566 2064 6f6d 6169  )..    def domai
+00007610: 6e5f 746f 5f61 7363 6969 2873 656c 6629  n_to_ascii(self)
+00007620: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00007630: 2072 6574 7572 6e20 6964 6e61 3230 3038   return idna2008
+00007640: 5f70 7265 7028 7365 6c66 2e64 6f6d 6169  _prep(self.domai
+00007650: 6e2c 2074 6f5f 6173 6369 693d 5472 7565  n, to_ascii=True
+00007660: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+00007670: 0a20 2020 2064 6566 2062 6172 6528 7365  .    def bare(se
+00007680: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+00007690: 2020 2020 6966 2073 656c 662e 6c6f 6361      if self.loca
+000076a0: 6c70 6172 7420 6973 206e 6f74 204e 6f6e  lpart is not Non
+000076b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000076c0: 6574 7572 6e20 6627 7b73 656c 662e 6c6f  eturn f'{self.lo
+000076d0: 6361 6c70 6172 747d 407b 7365 6c66 2e64  calpart}@{self.d
+000076e0: 6f6d 6169 6e7d 270a 2020 2020 2020 2020  omain}'.        
+000076f0: 7265 7475 726e 2073 656c 662e 646f 6d61  return self.doma
+00007700: 696e 0a0a 2020 2020 4070 726f 7065 7274  in..    @propert
+00007710: 790a 2020 2020 6465 6620 6973 5f62 6172  y.    def is_bar
+00007720: 6528 7365 6c66 2920 2d3e 2062 6f6f 6c3a  e(self) -> bool:
+00007730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007740: 7365 6c66 2e72 6573 6f75 7263 6520 6973  self.resource is
+00007750: 204e 6f6e 650a 0a20 2020 2064 6566 206e   None..    def n
+00007760: 6577 5f61 735f 6261 7265 2873 656c 6629  ew_as_bare(self)
+00007770: 202d 3e20 4a49 443a 0a20 2020 2020 2020   -> JID:.       
+00007780: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+00007790: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+000077a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000077b0: 6c66 0a20 2020 2020 2020 2072 6574 7572  lf.        retur
+000077c0: 6e20 4a49 442e 6672 6f6d 5f73 7472 696e  n JID.from_strin
+000077d0: 6728 7365 6c66 2e62 6172 6529 0a0a 2020  g(self.bare)..  
+000077e0: 2020 6465 6620 6261 7265 5f6d 6174 6368    def bare_match
+000077f0: 2873 656c 662c 206f 7468 6572 3a20 556e  (self, other: Un
+00007800: 696f 6e5b 7374 722c 204a 4944 5d29 202d  ion[str, JID]) -
+00007810: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00007820: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00007830: 6865 722c 2073 7472 293a 0a20 2020 2020  her, str):.     
+00007840: 2020 2020 2020 206f 7468 6572 203d 204a         other = J
+00007850: 4944 2e66 726f 6d5f 7374 7269 6e67 286f  ID.from_string(o
+00007860: 7468 6572 290a 2020 2020 2020 2020 7265  ther).        re
+00007870: 7475 726e 2073 656c 662e 6261 7265 203d  turn self.bare =
+00007880: 3d20 6f74 6865 722e 6261 7265 0a0a 2020  = other.bare..  
+00007890: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000078a0: 6465 6620 6973 5f64 6f6d 6169 6e28 7365  def is_domain(se
+000078b0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+000078c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000078d0: 2e6c 6f63 616c 7061 7274 2069 7320 4e6f  .localpart is No
+000078e0: 6e65 2061 6e64 2073 656c 662e 7265 736f  ne and self.reso
+000078f0: 7572 6365 2069 7320 4e6f 6e65 0a0a 2020  urce is None..  
+00007900: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00007910: 6465 6620 6973 5f66 756c 6c28 7365 6c66  def is_full(self
+00007920: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00007930: 2020 2072 6574 7572 6e20 2873 656c 662e     return (self.
+00007940: 6c6f 6361 6c70 6172 7420 6973 206e 6f74  localpart is not
+00007950: 204e 6f6e 6520 616e 640a 2020 2020 2020   None and.      
+00007960: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00007970: 6f6d 6169 6e20 6973 206e 6f74 204e 6f6e  omain is not Non
+00007980: 6520 616e 640a 2020 2020 2020 2020 2020  e and.          
+00007990: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+000079a0: 7263 6520 6973 206e 6f74 204e 6f6e 6529  rce is not None)
+000079b0: 0a0a 2020 2020 6465 6620 6e65 775f 7769  ..    def new_wi
+000079c0: 7468 2873 656c 662c 202a 2a6b 7761 7267  th(self, **kwarg
+000079d0: 733a 2064 6963 745b 7374 722c 2073 7472  s: dict[str, str
+000079e0: 5d29 202d 3e20 4a49 443a 0a20 2020 2020  ]) -> JID:.     
+000079f0: 2020 206e 6577 203d 2061 7364 6963 7428     new = asdict(
+00007a00: 7365 6c66 290a 2020 2020 2020 2020 6e65  self).        ne
+00007a10: 772e 7570 6461 7465 286b 7761 7267 7329  w.update(kwargs)
+00007a20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007a30: 4a49 4428 2a2a 6e65 7729 0a0a 2020 2020  JID(**new)..    
+00007a40: 6465 6620 746f 5f75 7365 725f 7374 7269  def to_user_stri
+00007a50: 6e67 2873 656c 662c 2073 686f 775f 7075  ng(self, show_pu
+00007a60: 6e79 636f 6465 3a20 626f 6f6c 203d 2054  nycode: bool = T
+00007a70: 7275 6529 202d 3e20 7374 723a 0a20 2020  rue) -> str:.   
+00007a80: 2020 2020 2064 6f6d 6169 6e20 3d20 7365       domain = se
+00007a90: 6c66 2e64 6f6d 6169 6e5f 746f 5f61 7363  lf.domain_to_asc
+00007aa0: 6969 2829 0a20 2020 2020 2020 2069 6620  ii().        if 
+00007ab0: 646f 6d61 696e 2e73 7461 7274 7377 6974  domain.startswit
+00007ac0: 6828 2778 6e2d 2d27 2920 616e 6420 7368  h('xn--') and sh
+00007ad0: 6f77 5f70 756e 7963 6f64 653a 0a20 2020  ow_punycode:.   
+00007ae0: 2020 2020 2020 2020 2064 6f6d 6169 6e5f           domain_
+00007af0: 656e 636f 6465 6420 3d20 6627 2028 7b64  encoded = f' ({d
+00007b00: 6f6d 6169 6e7d 2927 0a20 2020 2020 2020  omain})'.       
+00007b10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007b20: 2020 2064 6f6d 6169 6e5f 656e 636f 6465     domain_encode
+00007b30: 6420 3d20 2727 0a0a 2020 2020 2020 2020  d = ''..        
+00007b40: 6966 2073 656c 662e 6c6f 6361 6c70 6172  if self.localpar
+00007b50: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+00007b60: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
+00007b70: 7b73 656c 667d 7b64 6f6d 6169 6e5f 656e  {self}{domain_en
+00007b80: 636f 6465 647d 270a 0a20 2020 2020 2020  coded}'..       
+00007b90: 206c 6f63 616c 7061 7274 203d 2075 6e65   localpart = une
+00007ba0: 7363 6170 655f 6c6f 6361 6c70 6172 7428  scape_localpart(
+00007bb0: 7365 6c66 2e6c 6f63 616c 7061 7274 290a  self.localpart).
+00007bc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00007bd0: 2e72 6573 6f75 7263 6520 6973 204e 6f6e  .resource is Non
+00007be0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00007bf0: 6574 7572 6e20 6627 7b6c 6f63 616c 7061  eturn f'{localpa
+00007c00: 7274 7d40 7b73 656c 662e 646f 6d61 696e  rt}@{self.domain
+00007c10: 7d7b 646f 6d61 696e 5f65 6e63 6f64 6564  }{domain_encoded
+00007c20: 7d27 0a20 2020 2020 2020 2072 6574 7572  }'.        retur
+00007c30: 6e20 6627 7b6c 6f63 616c 7061 7274 7d40  n f'{localpart}@
+00007c40: 7b73 656c 662e 646f 6d61 696e 7d2f 7b73  {self.domain}/{s
+00007c50: 656c 662e 7265 736f 7572 6365 7d7b 646f  elf.resource}{do
+00007c60: 6d61 696e 5f65 6e63 6f64 6564 7d27 0a0a  main_encoded}'..
+00007c70: 2020 2020 6465 6620 746f 5f69 7269 2873      def to_iri(s
+00007c80: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00007c90: 2020 2020 7175 6572 793a 204f 7074 696f      query: Optio
+00007ca0: 6e61 6c5b 7374 7220 7c20 7475 706c 655b  nal[str | tuple[
+00007cb0: 7374 722c 206c 6973 745b 7475 706c 655b  str, list[tuple[
+00007cc0: 7374 722c 2073 7472 5d5d 5d5d 203d 204e  str, str]]]] = N
+00007cd0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00007ce0: 2020 2020 6672 6167 6d65 6e74 3a20 4f70      fragment: Op
+00007cf0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00007d00: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00007d10: 2020 2920 2d3e 2073 7472 3a0a 0a20 2020    ) -> str:..   
+00007d20: 2020 2020 2069 6620 7365 6c66 2e6c 6f63       if self.loc
+00007d30: 616c 7061 7274 3a0a 2020 2020 2020 2020  alpart:.        
+00007d40: 2020 2020 696e 6f64 6520 3d20 6573 6361      inode = esca
+00007d50: 7065 5f69 6e6f 6465 2873 656c 662e 6c6f  pe_inode(self.lo
+00007d60: 6361 6c70 6172 7429 0a20 2020 2020 2020  calpart).       
+00007d70: 2020 2020 2069 7061 7468 786d 7070 203d       ipathxmpp =
+00007d80: 2066 277b 696e 6f64 657d 407b 7365 6c66   f'{inode}@{self
+00007d90: 2e64 6f6d 6169 6e7d 270a 2020 2020 2020  .domain}'.      
+00007da0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007db0: 2020 2020 6970 6174 6878 6d70 7020 3d20      ipathxmpp = 
+00007dc0: 6627 7b73 656c 662e 646f 6d61 696e 7d27  f'{self.domain}'
+00007dd0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00007de0: 662e 7265 736f 7572 6365 2069 7320 6e6f  f.resource is no
+00007df0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00007e00: 2020 2020 6972 6573 203d 2065 7363 6170      ires = escap
+00007e10: 655f 6972 6573 2873 656c 662e 7265 736f  e_ires(self.reso
+00007e20: 7572 6365 290a 2020 2020 2020 2020 2020  urce).          
+00007e30: 2020 6970 6174 6878 6d70 7020 3d20 6627    ipathxmpp = f'
+00007e40: 7b69 7061 7468 786d 7070 7d2f 7b69 7265  {ipathxmpp}/{ire
+00007e50: 737d 270a 0a20 2020 2020 2020 2069 7269  s}'..        iri
+00007e60: 203d 2066 2778 6d70 703a 7b69 7061 7468   = f'xmpp:{ipath
+00007e70: 786d 7070 7d27 0a0a 2020 2020 2020 2020  xmpp}'..        
+00007e80: 6966 2071 7565 7279 2069 7320 6e6f 7420  if query is not 
+00007e90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007ea0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00007eb0: 7175 6572 792c 2073 7472 293a 0a20 2020  query, str):.   
+00007ec0: 2020 2020 2020 2020 2020 2020 2071 7565               que
+00007ed0: 7279 7479 7065 203d 2071 7565 7279 0a20  rytype = query. 
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+00007ef0: 7565 7279 7061 7261 6d73 203d 204e 6f6e  ueryparams = Non
+00007f00: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+00007f10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007f20: 2020 2020 7175 6572 7974 7970 652c 2071      querytype, q
+00007f30: 7565 7279 7061 7261 6d73 203d 2071 7565  ueryparams = que
+00007f40: 7279 0a0a 2020 2020 2020 2020 2020 2020  ry..            
+00007f50: 6971 7565 7279 7479 7065 203d 2076 616c  iquerytype = val
+00007f60: 6964 6174 655f 7175 6572 7974 7970 6528  idate_querytype(
+00007f70: 7175 6572 7974 7970 6529 0a20 2020 2020  querytype).     
+00007f80: 2020 2020 2020 2069 7269 202b 3d20 6627         iri += f'
+00007f90: 3f7b 6971 7565 7279 7479 7065 7d27 0a0a  ?{iquerytype}'..
+00007fa0: 2020 2020 2020 2020 2020 2020 6966 2071              if q
+00007fb0: 7565 7279 7061 7261 6d73 2069 7320 6e6f  ueryparams is no
+00007fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00007fd0: 2020 2020 2020 2020 666f 7220 696b 6579          for ikey
+00007fe0: 2c20 6976 616c 7565 2069 6e20 7175 6572  , ivalue in quer
+00007ff0: 7970 6172 616d 733a 0a20 2020 2020 2020  yparams:.       
+00008000: 2020 2020 2020 2020 2020 2020 2069 7661               iva
+00008010: 6c75 6520 3d20 6573 6361 7065 5f69 7661  lue = escape_iva
+00008020: 6c75 6528 6976 616c 7565 290a 2020 2020  lue(ivalue).    
+00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 696b 6579 203d 2076 616c 6964 6174 655f  ikey = validate_
+00008050: 696b 6579 2869 6b65 7929 0a20 2020 2020  ikey(ikey).     
+00008060: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00008070: 7269 202b 3d20 6627 3b7b 696b 6579 7d3d  ri += f';{ikey}=
+00008080: 7b69 7661 6c75 657d 270a 0a20 2020 2020  {ivalue}'..     
+00008090: 2020 2069 6620 6672 6167 6d65 6e74 2069     if fragment i
+000080a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000080b0: 2020 2020 2020 2020 6966 7261 676d 656e          ifragmen
+000080c0: 7420 3d20 6573 6361 7065 5f69 6672 6167  t = escape_ifrag
+000080d0: 6d65 6e74 2866 7261 676d 656e 7429 0a20  ment(fragment). 
+000080e0: 2020 2020 2020 2020 2020 2069 7269 202b             iri +
+000080f0: 3d20 6627 237b 6966 7261 676d 656e 747d  = f'#{ifragment}
+00008100: 270a 0a20 2020 2020 2020 2072 6574 7572  '..        retur
+00008110: 6e20 6972 690a 0a20 2020 2064 6566 2063  n iri..    def c
+00008120: 6f70 7928 7365 6c66 2920 2d3e 204a 4944  opy(self) -> JID
+00008130: 3a0a 2020 2020 2020 2020 6465 7072 6563  :.        deprec
+00008140: 6174 696f 6e5f 7761 726e 696e 6728 2763  ation_warning('c
+00008150: 6f70 7928 2920 6973 206e 6f74 206e 6565  opy() is not nee
+00008160: 6465 642c 204a 4944 2069 7320 696d 6d75  ded, JID is immu
+00008170: 7461 626c 6527 290a 2020 2020 2020 2020  table').        
+00008180: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00008190: 6173 7320 5374 7265 616d 4572 726f 724e  ass StreamErrorN
+000081a0: 6f64 6528 4e6f 6465 293a 0a20 2020 2064  ode(Node):.    d
+000081b0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000081c0: 2c20 6e6f 6465 293a 0a20 2020 2020 2020  , node):.       
+000081d0: 204e 6f64 652e 5f5f 696e 6974 5f5f 2873   Node.__init__(s
+000081e0: 656c 662c 206e 6f64 653d 6e6f 6465 290a  elf, node=node).
+000081f0: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
+00008200: 6578 743a 2064 6963 745b 4f70 7469 6f6e  ext: dict[Option
+00008210: 616c 5b73 7472 5d2c 2073 7472 5d20 3d20  al[str], str] = 
+00008220: 7b7d 0a0a 2020 2020 2020 2020 7465 7874  {}..        text
+00008230: 5f65 6c65 6d65 6e74 7320 3d20 7365 6c66  _elements = self
+00008240: 2e67 6574 5461 6773 2827 7465 7874 272c  .getTags('text',
+00008250: 206e 616d 6573 7061 6365 3d4e 616d 6573   namespace=Names
+00008260: 7061 6365 2e58 4d50 505f 5354 5245 414d  pace.XMPP_STREAM
+00008270: 5329 0a20 2020 2020 2020 2066 6f72 2065  S).        for e
+00008280: 6c65 6d65 6e74 2069 6e20 7465 7874 5f65  lement in text_e
+00008290: 6c65 6d65 6e74 733a 0a20 2020 2020 2020  lements:.       
+000082a0: 2020 2020 206c 616e 6720 3d20 656c 656d       lang = elem
+000082b0: 656e 742e 6765 7458 6d6c 4c61 6e67 2829  ent.getXmlLang()
+000082c0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+000082d0: 7420 3d20 656c 656d 656e 742e 6765 7444  t = element.getD
+000082e0: 6174 6128 290a 2020 2020 2020 2020 2020  ata().          
+000082f0: 2020 7365 6c66 2e5f 7465 7874 5b6c 616e    self._text[lan
+00008300: 675d 203d 2074 6578 740a 0a20 2020 2064  g] = text..    d
+00008310: 6566 2067 6574 5f63 6f6e 6469 7469 6f6e  ef get_condition
+00008320: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00008330: 616c 5b73 7472 5d3a 0a20 2020 2020 2020  al[str]:.       
+00008340: 2066 6f72 2074 6167 2069 6e20 7365 6c66   for tag in self
+00008350: 2e67 6574 4368 696c 6472 656e 2829 3a0a  .getChildren():.
+00008360: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00008370: 7461 672e 6765 744e 616d 6528 2920 213d  tag.getName() !=
+00008380: 2027 7465 7874 2720 616e 640a 2020 2020   'text' and.    
+00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 7461 672e 6765 744e 616d 6573 7061 6365  tag.getNamespace
+000083b0: 2829 203d 3d20 4e61 6d65 7370 6163 652e  () == Namespace.
+000083c0: 584d 5050 5f53 5452 4541 4d53 293a 0a20  XMPP_STREAMS):. 
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000083e0: 6574 7572 6e20 7461 672e 6765 744e 616d  eturn tag.getNam
+000083f0: 6528 290a 2020 2020 2020 2020 7265 7475  e().        retu
+00008400: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
+00008410: 2067 6574 5f74 6578 7428 7365 6c66 2c20   get_text(self, 
+00008420: 7072 6566 5f6c 616e 673a 204f 7074 696f  pref_lang: Optio
+00008430: 6e61 6c5b 7374 725d 203d 204e 6f6e 6529  nal[str] = None)
+00008440: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00008450: 2069 6620 7072 6566 5f6c 616e 6720 6973   if pref_lang is
+00008460: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008470: 2020 2020 2020 2074 6578 7420 3d20 7365         text = se
+00008480: 6c66 2e5f 7465 7874 2e67 6574 2870 7265  lf._text.get(pre
+00008490: 665f 6c61 6e67 290a 2020 2020 2020 2020  f_lang).        
+000084a0: 2020 2020 6966 2074 6578 7420 6973 206e      if text is n
+000084b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000084c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000084d0: 7465 7874 0a0a 2020 2020 2020 2020 6966  text..        if
+000084e0: 2073 656c 662e 5f74 6578 743a 0a20 2020   self._text:.   
+000084f0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+00008500: 7365 6c66 2e5f 7465 7874 2e67 6574 2827  self._text.get('
+00008510: 656e 2729 0a20 2020 2020 2020 2020 2020  en').           
+00008520: 2069 6620 7465 7874 2069 7320 6e6f 7420   if text is not 
+00008530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00008540: 2020 2020 2020 7265 7475 726e 2074 6578        return tex
+00008550: 740a 0a20 2020 2020 2020 2020 2020 2074  t..            t
+00008560: 6578 7420 3d20 7365 6c66 2e5f 7465 7874  ext = self._text
+00008570: 2e67 6574 284e 6f6e 6529 0a20 2020 2020  .get(None).     
+00008580: 2020 2020 2020 2069 6620 7465 7874 2069         if text i
+00008590: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000085a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000085b0: 726e 2074 6578 740a 2020 2020 2020 2020  rn text.        
+000085c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000085d0: 5f74 6578 742e 706f 7069 7465 6d28 295b  _text.popitem()[
+000085e0: 315d 0a20 2020 2020 2020 2072 6574 7572  1].        retur
+000085f0: 6e20 2727 0a0a 0a63 6c61 7373 2050 726f  n ''...class Pro
+00008600: 746f 636f 6c28 4e6f 6465 293a 0a20 2020  tocol(Node):.   
+00008610: 2022 2222 0a20 2020 2041 2022 7374 616e   """.    A "stan
+00008620: 7a61 2220 6f62 6a65 6374 2063 6c61 7373  za" object class
+00008630: 2e20 436f 6e74 6169 6e73 206d 6574 686f  . Contains metho
+00008640: 6473 2074 6861 7420 6172 6520 636f 6d6d  ds that are comm
+00008650: 6f6e 2066 6f72 2070 7265 7365 6e63 6573  on for presences
+00008660: 2c20 6971 730a 2020 2020 616e 6420 6d65  , iqs.    and me
+00008670: 7373 6167 6573 0a20 2020 2022 2222 0a0a  ssages.    """..
+00008680: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00008690: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+000086a0: 2020 2020 2020 2020 6e61 6d65 3d4e 6f6e          name=Non
+000086b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000086c0: 2020 2020 746f 3d4e 6f6e 652c 0a20 2020      to=None,.   
+000086d0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+000086e0: 703d 4e6f 6e65 2c0a 2020 2020 2020 2020  p=None,.        
+000086f0: 2020 2020 2020 2020 2066 726d 3d4e 6f6e           frm=Non
+00008700: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00008710: 2020 2020 6174 7472 733d 4e6f 6e65 2c0a      attrs=None,.
+00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008730: 2070 6179 6c6f 6164 3d4e 6f6e 652c 0a20   payload=None,. 
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 7469 6d65 7374 616d 703d 4e6f 6e65 2c0a  timestamp=None,.
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2078 6d6c 6e73 3d4e 6f6e 652c 0a20 2020   xmlns=None,.   
+00008780: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00008790: 6465 3d4e 6f6e 6529 3a0a 2020 2020 2020  de=None):.      
+000087a0: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
+000087b0: 6e73 7472 7563 746f 722c 206e 616d 6520  nstructor, name 
+000087c0: 6973 2074 6865 206e 616d 6520 6f66 2074  is the name of t
+000087d0: 6865 2073 7461 6e7a 610a 2020 2020 2020  he stanza.      
+000087e0: 2020 692e 652e 2027 6d65 7373 6167 6527    i.e. 'message'
+000087f0: 206f 7220 2770 7265 7365 6e63 6527 6f72   or 'presence'or
+00008800: 2027 6971 270a 0a20 2020 2020 2020 2074   'iq'..        t
+00008810: 6f20 6973 2074 6865 2076 616c 7565 206f  o is the value o
+00008820: 6620 2774 6f27 2061 7474 7269 6275 7265  f 'to' attribure
+00008830: 2c20 2774 7970 2720 2d20 2774 7970 6527  , 'typ' - 'type'
+00008840: 2061 7474 7269 6275 7465 0a20 2020 2020   attribute.     
+00008850: 2020 2066 726e 202d 2066 726f 6d20 6174     frn - from at
+00008860: 7472 6962 7572 652c 2061 7474 7273 202d  tribure, attrs -
+00008870: 206f 7468 6572 2061 7474 7269 6275 7465   other attribute
+00008880: 7320 6d61 7070 696e 672c 0a20 2020 2020  s mapping,.     
+00008890: 2020 2070 6179 6c6f 6164 202d 2073 616d     payload - sam
+000088a0: 6520 6d65 616e 696e 6720 6173 2066 6f72  e meaning as for
+000088b0: 2073 696d 706c 6578 6d6c 2070 6179 6c6f   simplexml paylo
+000088c0: 6164 2064 6566 696e 6974 696f 6e0a 2020  ad definition.  
+000088d0: 2020 2020 2020 7469 6d65 7374 616d 7020        timestamp 
+000088e0: 2d20 7468 6520 7469 6d65 2076 616c 7565  - the time value
+000088f0: 2074 6861 7420 6e65 6564 7320 746f 2062   that needs to b
+00008900: 6520 7374 616d 7065 6420 6f76 6572 2073  e stamped over s
+00008910: 7461 6e7a 610a 2020 2020 2020 2020 786d  tanza.        xm
+00008920: 6c6e 7320 2d20 6e61 6d65 7370 6163 6520  lns - namespace 
+00008930: 6f66 2074 6f70 2073 7461 6e7a 6120 6e6f  of top stanza no
+00008940: 6465 0a20 2020 2020 2020 206e 6f64 6520  de.        node 
+00008950: 2d20 7061 7273 6564 206f 7220 756e 7061  - parsed or unpa
+00008960: 7273 6564 2073 7461 6e61 2074 6f20 6265  rsed stana to be
+00008970: 2074 616b 656e 2061 7320 7072 6f74 6f74   taken as protot
+00008980: 7970 652e 0a20 2020 2020 2020 2022 2222  ype..        """
+00008990: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000089a0: 6174 7472 733a 0a20 2020 2020 2020 2020  attrs:.         
+000089b0: 2020 2061 7474 7273 203d 207b 7d0a 2020     attrs = {}.  
+000089c0: 2020 2020 2020 6966 2074 6f3a 0a20 2020        if to:.   
+000089d0: 2020 2020 2020 2020 2061 7474 7273 5b27           attrs['
+000089e0: 746f 275d 203d 2074 6f0a 2020 2020 2020  to'] = to.      
+000089f0: 2020 6966 2066 726d 3a0a 2020 2020 2020    if frm:.      
+00008a00: 2020 2020 2020 6174 7472 735b 2766 726f        attrs['fro
+00008a10: 6d27 5d20 3d20 6672 6d0a 2020 2020 2020  m'] = frm.      
+00008a20: 2020 6966 2074 7970 3a0a 2020 2020 2020    if typ:.      
+00008a30: 2020 2020 2020 6174 7472 735b 2774 7970        attrs['typ
+00008a40: 6527 5d20 3d20 7479 700a 2020 2020 2020  e'] = typ.      
+00008a50: 2020 4e6f 6465 2e5f 5f69 6e69 745f 5f28    Node.__init__(
+00008a60: 7365 6c66 2c20 7461 673d 6e61 6d65 2c20  self, tag=name, 
+00008a70: 6174 7472 733d 6174 7472 732c 2070 6179  attrs=attrs, pay
+00008a80: 6c6f 6164 3d70 6179 6c6f 6164 2c20 6e6f  load=payload, no
+00008a90: 6465 3d6e 6f64 6529 0a20 2020 2020 2020  de=node).       
+00008aa0: 2069 6620 6e6f 7420 6e6f 6465 2061 6e64   if not node and
+00008ab0: 2078 6d6c 6e73 3a0a 2020 2020 2020 2020   xmlns:.        
+00008ac0: 2020 2020 7365 6c66 2e73 6574 4e61 6d65      self.setName
+00008ad0: 7370 6163 6528 786d 6c6e 7329 0a20 2020  space(xmlns).   
+00008ae0: 2020 2020 2069 6620 7365 6c66 5b27 746f       if self['to
+00008af0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00008b00: 7365 6c66 2e73 6574 546f 2873 656c 665b  self.setTo(self[
+00008b10: 2774 6f27 5d29 0a20 2020 2020 2020 2069  'to']).        i
+00008b20: 6620 7365 6c66 5b27 6672 6f6d 275d 3a0a  f self['from']:.
+00008b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008b40: 2e73 6574 4672 6f6d 2873 656c 665b 2766  .setFrom(self['f
+00008b50: 726f 6d27 5d29 0a20 2020 2020 2020 2069  rom']).        i
+00008b60: 6620 286e 6f64 6520 616e 640a 2020 2020  f (node and.    
+00008b70: 2020 2020 2020 2020 2020 2020 6973 696e              isin
+00008b80: 7374 616e 6365 286e 6f64 652c 2050 726f  stance(node, Pro
+00008b90: 746f 636f 6c29 2061 6e64 0a20 2020 2020  tocol) and.     
+00008ba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008bb0: 5f5f 636c 6173 735f 5f20 3d3d 206e 6f64  __class__ == nod
+00008bc0: 652e 5f5f 636c 6173 735f 5f0a 2020 2020  e.__class__.    
+00008bd0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00008be0: 2769 6427 2069 6e20 7365 6c66 2e61 7474  'id' in self.att
+00008bf0: 7273 293a 0a20 2020 2020 2020 2020 2020  rs):.           
+00008c00: 2064 656c 2073 656c 662e 6174 7472 735b   del self.attrs[
+00008c10: 2769 6427 5d0a 2020 2020 2020 2020 7365  'id'].        se
+00008c20: 6c66 2e74 696d 6573 7461 6d70 203d 204e  lf.timestamp = N
+00008c30: 6f6e 650a 2020 2020 2020 2020 666f 7220  one.        for 
+00008c40: 6420 696e 2073 656c 662e 6765 7454 6167  d in self.getTag
+00008c50: 7328 2764 656c 6179 272c 206e 616d 6573  s('delay', names
+00008c60: 7061 6365 3d4e 616d 6573 7061 6365 2e44  pace=Namespace.D
+00008c70: 454c 4159 3229 3a0a 2020 2020 2020 2020  ELAY2):.        
+00008c80: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00008c90: 2020 2020 2020 2020 2069 6620 642e 6765           if d.ge
+00008ca0: 7441 7474 7228 2773 7461 6d70 2729 203c  tAttr('stamp') <
+00008cb0: 2073 656c 662e 6765 7454 696d 6573 7461   self.getTimesta
+00008cc0: 6d70 3228 293a 0a20 2020 2020 2020 2020  mp2():.         
+00008cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008ce0: 7365 7454 696d 6573 7461 6d70 2864 2e67  setTimestamp(d.g
+00008cf0: 6574 4174 7472 2827 7374 616d 7027 2929  etAttr('stamp'))
+00008d00: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00008d10: 6570 7420 4578 6365 7074 696f 6e3a 0a20  ept Exception:. 
+00008d20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00008d30: 6173 730a 2020 2020 2020 2020 6966 206e  ass.        if n
+00008d40: 6f74 2073 656c 662e 7469 6d65 7374 616d  ot self.timestam
+00008d50: 703a 0a20 2020 2020 2020 2020 2020 2066  p:.            f
+00008d60: 6f72 2078 2069 6e20 7365 6c66 2e67 6574  or x in self.get
+00008d70: 5461 6773 2827 7827 2c20 6e61 6d65 7370  Tags('x', namesp
+00008d80: 6163 653d 4e61 6d65 7370 6163 652e 4445  ace=Namespace.DE
+00008d90: 4c41 5929 3a0a 2020 2020 2020 2020 2020  LAY):.          
+00008da0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00008dc0: 6620 782e 6765 7441 7474 7228 2773 7461  f x.getAttr('sta
+00008dd0: 6d70 2729 203c 2073 656c 662e 6765 7454  mp') < self.getT
+00008de0: 696d 6573 7461 6d70 2829 3a0a 2020 2020  imestamp():.    
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e00: 2020 2020 7365 6c66 2e73 6574 5469 6d65      self.setTime
+00008e10: 7374 616d 7028 782e 6765 7441 7474 7228  stamp(x.getAttr(
+00008e20: 2773 7461 6d70 2729 290a 2020 2020 2020  'stamp')).      
+00008e30: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00008e40: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
+00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e60: 7061 7373 0a20 2020 2020 2020 2069 6620  pass.        if 
+00008e70: 7469 6d65 7374 616d 7020 6973 206e 6f74  timestamp is not
+00008e80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00008e90: 2020 2073 656c 662e 7365 7454 696d 6573     self.setTimes
+00008ea0: 7461 6d70 2874 696d 6573 7461 6d70 290a  tamp(timestamp).
+00008eb0: 0a20 2020 2064 6566 2069 7345 7272 6f72  .    def isError
+00008ec0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008ed0: 7265 7475 726e 2073 656c 662e 6765 7441  return self.getA
+00008ee0: 7474 7228 2774 7970 6527 2920 3d3d 2027  ttr('type') == '
+00008ef0: 6572 726f 7227 0a0a 2020 2020 6465 6620  error'..    def 
+00008f00: 6973 5265 7375 6c74 2873 656c 6629 3a0a  isResult(self):.
+00008f10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008f20: 656c 662e 6765 7441 7474 7228 2774 7970  elf.getAttr('typ
+00008f30: 6527 2920 3d3d 2027 7265 7375 6c74 270a  e') == 'result'.
+00008f40: 0a20 2020 2064 6566 2067 6574 546f 2873  .    def getTo(s
+00008f50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00008f60: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00008f70: 2076 616c 7565 206f 6620 7468 6520 2774   value of the 't
+00008f80: 6f27 2061 7474 7269 6275 7465 0a20 2020  o' attribute.   
+00008f90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00008fa0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00008fb0: 2020 7265 7475 726e 2073 656c 665b 2774    return self['t
+00008fc0: 6f27 5d0a 2020 2020 2020 2020 6578 6365  o'].        exce
+00008fd0: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
+00008fe0: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00008ff0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00009000: 6e65 0a0a 2020 2020 6465 6620 6765 7446  ne..    def getF
+00009010: 726f 6d28 7365 6c66 293a 0a20 2020 2020  rom(self):.     
+00009020: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00009030: 6574 7572 6e20 7661 6c75 6520 6f66 2074  eturn value of t
+00009040: 6865 2027 6672 6f6d 2720 6174 7472 6962  he 'from' attrib
+00009050: 7574 650a 2020 2020 2020 2020 2222 220a  ute.        """.
+00009060: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00009070: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009080: 7365 6c66 5b27 6672 6f6d 275d 0a20 2020  self['from'].   
+00009090: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000090a0: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
+000090b0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+000090c0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+000090d0: 2064 6566 2067 6574 5469 6d65 7374 616d   def getTimestam
+000090e0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000090f0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00009100: 7572 6e20 7468 6520 7469 6d65 7374 616d  urn the timestam
+00009110: 7020 696e 2074 6865 2027 7979 7979 6d6d  p in the 'yyyymm
+00009120: 6464 5468 686d 6d73 7327 2066 6f72 6d61  ddThhmmss' forma
+00009130: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00009140: 2020 2020 2020 6966 2073 656c 662e 7469        if self.ti
+00009150: 6d65 7374 616d 703a 0a20 2020 2020 2020  mestamp:.       
+00009160: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00009170: 2e74 696d 6573 7461 6d70 0a20 2020 2020  .timestamp.     
+00009180: 2020 2072 6574 7572 6e20 7469 6d65 2e73     return time.s
+00009190: 7472 6674 696d 6528 2725 5925 6d25 6454  trftime('%Y%m%dT
+000091a0: 2548 3a25 4d3a 2553 272c 2074 696d 652e  %H:%M:%S', time.
+000091b0: 676d 7469 6d65 2829 290a 0a20 2020 2064  gmtime())..    d
+000091c0: 6566 2067 6574 5469 6d65 7374 616d 7032  ef getTimestamp2
+000091d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000091e0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+000091f0: 726e 2074 6865 2074 696d 6573 7461 6d70  rn the timestamp
+00009200: 2069 6e20 7468 6520 2779 7979 796d 6d64   in the 'yyyymmd
+00009210: 6454 6868 6d6d 7373 2720 666f 726d 6174  dThhmmss' format
+00009220: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009230: 2020 2020 2069 6620 7365 6c66 2e74 696d       if self.tim
+00009240: 6573 7461 6d70 3a0a 2020 2020 2020 2020  estamp:.        
+00009250: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00009260: 7469 6d65 7374 616d 700a 2020 2020 2020  timestamp.      
+00009270: 2020 7265 7475 726e 2074 696d 652e 7374    return time.st
+00009280: 7266 7469 6d65 2827 2559 2d25 6d2d 2564  rftime('%Y-%m-%d
+00009290: 5425 483a 254d 3a25 535a 272c 2074 696d  T%H:%M:%SZ', tim
+000092a0: 652e 676d 7469 6d65 2829 290a 0a20 2020  e.gmtime())..   
+000092b0: 2064 6566 2067 6574 4a69 6428 7365 6c66   def getJid(self
+000092c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000092d0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+000092e0: 6520 7661 6c75 6520 6f66 2074 6865 2027  e value of the '
+000092f0: 6a69 6427 2061 7474 7269 6275 7465 0a20  jid' attribute. 
+00009300: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00009310: 2020 2061 7474 7220 3d20 7365 6c66 2e67     attr = self.g
+00009320: 6574 4174 7472 2827 6a69 6427 290a 2020  etAttr('jid').  
+00009330: 2020 2020 2020 6966 2061 7474 723a 0a20        if attr:. 
+00009340: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009350: 6e20 4a49 442e 6672 6f6d 5f73 7472 696e  n JID.from_strin
+00009360: 6728 6174 7472 290a 2020 2020 2020 2020  g(attr).        
+00009370: 7265 7475 726e 2061 7474 720a 0a20 2020  return attr..   
+00009380: 2064 6566 2067 6574 4944 2873 656c 6629   def getID(self)
+00009390: 202d 3e20 4f70 7469 6f6e 616c 5b73 7472   -> Optional[str
+000093a0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+000093b0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+000093c0: 6520 7661 6c75 6520 6f66 2074 6865 2027  e value of the '
+000093d0: 6964 2720 6174 7472 6962 7574 650a 2020  id' attribute.  
+000093e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000093f0: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
+00009400: 7441 7474 7228 2769 6427 290a 0a20 2020  tAttr('id')..   
+00009410: 2064 6566 2073 6574 546f 2873 656c 662c   def setTo(self,
+00009420: 2076 616c 3a20 556e 696f 6e5b 7374 722c   val: Union[str,
+00009430: 204a 4944 5d29 3a0a 2020 2020 2020 2020   JID]):.        
+00009440: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
+00009450: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
+00009460: 2027 746f 2720 6174 7472 6962 7574 650a   'to' attribute.
+00009470: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009480: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00009490: 7461 6e63 6528 7661 6c2c 204a 4944 293a  tance(val, JID):
+000094a0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+000094b0: 203d 204a 4944 2e66 726f 6d5f 7374 7269   = JID.from_stri
+000094c0: 6e67 2876 616c 290a 2020 2020 2020 2020  ng(val).        
+000094d0: 7365 6c66 2e73 6574 4174 7472 2827 746f  self.setAttr('to
+000094e0: 272c 2076 616c 290a 0a20 2020 2064 6566  ', val)..    def
+000094f0: 2067 6574 5479 7065 2873 656c 6629 202d   getType(self) -
+00009500: 3e20 4f70 7469 6f6e 616c 5b73 7472 5d3a  > Optional[str]:
+00009510: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009520: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
+00009530: 7661 6c75 6520 6f66 2074 6865 2027 7479  value of the 'ty
+00009540: 7065 2720 6174 7472 6962 7574 650a 2020  pe' attribute.  
+00009550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009560: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
+00009570: 7441 7474 7228 2774 7970 6527 290a 0a20  tAttr('type').. 
+00009580: 2020 2064 6566 2073 6574 4672 6f6d 2873     def setFrom(s
+00009590: 656c 662c 2076 616c 3a20 556e 696f 6e5b  elf, val: Union[
+000095a0: 7374 722c 204a 4944 5d29 3a0a 2020 2020  str, JID]):.    
+000095b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000095c0: 5365 7420 7468 6520 7661 6c75 6520 6f66  Set the value of
+000095d0: 2074 6865 2027 6672 6f6d 2720 6174 7472   the 'from' attr
+000095e0: 6962 7574 650a 2020 2020 2020 2020 2222  ibute.        ""
+000095f0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+00009600: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
+00009610: 204a 4944 293a 0a20 2020 2020 2020 2020   JID):.         
+00009620: 2020 2076 616c 203d 204a 4944 2e66 726f     val = JID.fro
+00009630: 6d5f 7374 7269 6e67 2876 616c 290a 2020  m_string(val).  
+00009640: 2020 2020 2020 7365 6c66 2e73 6574 4174        self.setAt
+00009650: 7472 2827 6672 6f6d 272c 2076 616c 290a  tr('from', val).
+00009660: 0a20 2020 2064 6566 2073 6574 5479 7065  .    def setType
+00009670: 2873 656c 662c 2076 616c 3a20 7374 7229  (self, val: str)
+00009680: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00009690: 2020 2020 2020 5365 7420 7468 6520 7661        Set the va
+000096a0: 6c75 6520 6f66 2074 6865 2027 7479 7065  lue of the 'type
+000096b0: 2720 6174 7472 6962 7574 650a 2020 2020  ' attribute.    
+000096c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000096d0: 7365 6c66 2e73 6574 4174 7472 2827 7479  self.setAttr('ty
+000096e0: 7065 272c 2076 616c 290a 0a20 2020 2064  pe', val)..    d
+000096f0: 6566 2073 6574 4944 2873 656c 662c 2076  ef setID(self, v
+00009700: 616c 3a20 7374 7229 3a0a 2020 2020 2020  al: str):.      
+00009710: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
+00009720: 7420 7468 6520 7661 6c75 6520 6f66 2074  t the value of t
+00009730: 6865 2027 6964 2720 6174 7472 6962 7574  he 'id' attribut
+00009740: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+00009750: 2020 2020 2020 7365 6c66 2e73 6574 4174        self.setAt
+00009760: 7472 2827 6964 272c 2076 616c 290a 0a20  tr('id', val).. 
+00009770: 2020 2064 6566 2067 6574 4572 726f 7228     def getError(
+00009780: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
+00009790: 6c5b 7374 725d 3a0a 2020 2020 2020 2020  l[str]:.        
+000097a0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+000097b0: 726e 2074 6865 2065 7272 6f72 2d63 6f6e  rn the error-con
+000097c0: 6469 7469 6f6e 2028 6966 2070 7265 7365  dition (if prese
+000097d0: 6e74 2920 6f72 2074 6865 2074 6578 7475  nt) or the textu
+000097e0: 616c 2064 6573 6372 6970 7469 6f6e 0a20  al description. 
+000097f0: 2020 2020 2020 206f 6620 7468 6520 6572         of the er
+00009800: 726f 7220 286f 7468 6572 7769 7365 290a  ror (otherwise).
+00009810: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009820: 2020 2020 6572 7274 6167 203d 2073 656c      errtag = sel
+00009830: 662e 6765 7454 6167 2827 6572 726f 7227  f.getTag('error'
+00009840: 290a 2020 2020 2020 2020 6966 2065 7272  ).        if err
+00009850: 7461 6720 6973 204e 6f6e 653a 0a20 2020  tag is None:.   
+00009860: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009870: 4e6f 6e65 0a20 2020 2020 2020 2066 6f72  None.        for
+00009880: 2074 6167 2069 6e20 6572 7274 6167 2e67   tag in errtag.g
+00009890: 6574 4368 696c 6472 656e 2829 3a0a 2020  etChildren():.  
+000098a0: 2020 2020 2020 2020 2020 6966 2028 7461            if (ta
+000098b0: 672e 6765 744e 616d 6528 2920 213d 2027  g.getName() != '
+000098c0: 7465 7874 2720 616e 640a 2020 2020 2020  text' and.      
+000098d0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+000098e0: 672e 6765 744e 616d 6573 7061 6365 2829  g.getNamespace()
+000098f0: 203d 3d20 4e61 6d65 7370 6163 652e 5354   == Namespace.ST
+00009900: 414e 5a41 5329 3a0a 2020 2020 2020 2020  ANZAS):.        
+00009910: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00009920: 6167 2e67 6574 4e61 6d65 2829 0a20 2020  ag.getName().   
+00009930: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00009940: 0a0a 2020 2020 6465 6620 6765 7441 7070  ..    def getApp
+00009950: 4572 726f 7228 7365 6c66 293a 0a20 2020  Error(self):.   
+00009960: 2020 2020 2065 7272 7461 6720 3d20 7365       errtag = se
+00009970: 6c66 2e67 6574 5461 6728 2765 7272 6f72  lf.getTag('error
+00009980: 2729 0a20 2020 2020 2020 2069 6620 6572  ').        if er
+00009990: 7274 6167 2069 7320 4e6f 6e65 3a0a 2020  rtag is None:.  
+000099a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000099b0: 204e 6f6e 650a 2020 2020 2020 2020 666f   None.        fo
+000099c0: 7220 7461 6720 696e 2065 7272 7461 672e  r tag in errtag.
+000099d0: 6765 7443 6869 6c64 7265 6e28 293a 0a20  getChildren():. 
+000099e0: 2020 2020 2020 2020 2020 2069 6620 2874             if (t
+000099f0: 6167 2e67 6574 4e61 6d65 2829 2021 3d20  ag.getName() != 
+00009a00: 2774 6578 7427 2061 6e64 0a20 2020 2020  'text' and.     
+00009a10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00009a20: 6167 2e67 6574 4e61 6d65 7370 6163 6528  ag.getNamespace(
+00009a30: 2920 213d 204e 616d 6573 7061 6365 2e53  ) != Namespace.S
+00009a40: 5441 4e5a 4153 293a 0a20 2020 2020 2020  TANZAS):.       
+00009a50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009a60: 7461 672e 6765 744e 616d 6528 290a 2020  tag.getName().  
+00009a70: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00009a80: 650a 0a20 2020 2064 6566 2067 6574 4170  e..    def getAp
+00009a90: 7045 7272 6f72 4e61 6d65 7370 6163 6528  pErrorNamespace(
+00009aa0: 7365 6c66 293a 0a20 2020 2020 2020 2065  self):.        e
+00009ab0: 7272 7461 6720 3d20 7365 6c66 2e67 6574  rrtag = self.get
+00009ac0: 5461 6728 2765 7272 6f72 2729 0a20 2020  Tag('error').   
+00009ad0: 2020 2020 2069 6620 6572 7274 6167 2069       if errtag i
+00009ae0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00009af0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00009b00: 2020 2020 2020 2020 666f 7220 7461 6720          for tag 
+00009b10: 696e 2065 7272 7461 672e 6765 7443 6869  in errtag.getChi
+00009b20: 6c64 7265 6e28 293a 0a20 2020 2020 2020  ldren():.       
+00009b30: 2020 2020 2069 6620 2874 6167 2e67 6574       if (tag.get
+00009b40: 4e61 6d65 2829 2021 3d20 2774 6578 7427  Name() != 'text'
+00009b50: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+00009b60: 2020 2020 2020 2020 2074 6167 2e67 6574           tag.get
+00009b70: 4e61 6d65 7370 6163 6528 2920 213d 204e  Namespace() != N
+00009b80: 616d 6573 7061 6365 2e53 5441 4e5a 4153  amespace.STANZAS
+00009b90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009ba0: 2020 2072 6574 7572 6e20 7461 672e 6765     return tag.ge
+00009bb0: 744e 616d 6573 7061 6365 2829 0a20 2020  tNamespace().   
+00009bc0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00009bd0: 0a0a 2020 2020 6465 6620 6765 7445 7272  ..    def getErr
+00009be0: 6f72 4d73 6728 7365 6c66 293a 0a20 2020  orMsg(self):.   
+00009bf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00009c00: 2052 6574 7572 6e20 7468 6520 7465 7874   Return the text
+00009c10: 7561 6c20 6465 7363 7269 7074 696f 6e20  ual description 
+00009c20: 6f66 2074 6865 2065 7272 6f72 2028 6966  of the error (if
+00009c30: 2070 7265 7365 6e74 290a 2020 2020 2020   present).      
+00009c40: 2020 6f72 2074 6865 2065 7272 6f72 2063    or the error c
+00009c50: 6f6e 6469 7469 6f6e 0a20 2020 2020 2020  ondition.       
+00009c60: 2022 2222 0a20 2020 2020 2020 2065 7272   """.        err
+00009c70: 7461 6720 3d20 7365 6c66 2e67 6574 5461  tag = self.getTa
+00009c80: 6728 2765 7272 6f72 2729 0a20 2020 2020  g('error').     
+00009c90: 2020 2069 6620 6572 7274 6167 3a0a 2020     if errtag:.  
+00009ca0: 2020 2020 2020 2020 2020 666f 7220 7461            for ta
+00009cb0: 6720 696e 2065 7272 7461 672e 6765 7443  g in errtag.getC
+00009cc0: 6869 6c64 7265 6e28 293a 0a20 2020 2020  hildren():.     
+00009cd0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00009ce0: 672e 6765 744e 616d 6528 2920 3d3d 2027  g.getName() == '
+00009cf0: 7465 7874 273a 0a20 2020 2020 2020 2020  text':.         
+00009d00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009d10: 6e20 7461 672e 6765 7444 6174 6128 290a  n tag.getData().
+00009d20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009d30: 726e 2073 656c 662e 6765 7445 7272 6f72  rn self.getError
+00009d40: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00009d50: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
+00009d60: 6765 7445 7272 6f72 436f 6465 2873 656c  getErrorCode(sel
+00009d70: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00009d80: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+00009d90: 6865 2065 7272 6f72 2063 6f64 652e 204f  he error code. O
+00009da0: 6273 6f6c 6574 652e 0a20 2020 2020 2020  bsolete..       
+00009db0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00009dc0: 7572 6e20 7365 6c66 2e67 6574 5461 6741  urn self.getTagA
+00009dd0: 7474 7228 2765 7272 6f72 272c 2027 636f  ttr('error', 'co
+00009de0: 6465 2729 0a0a 2020 2020 6465 6620 6765  de')..    def ge
+00009df0: 7445 7272 6f72 5479 7065 2873 656c 6629  tErrorType(self)
+00009e00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00009e10: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00009e20: 2065 7272 6f72 2063 6f64 652e 204f 6273   error code. Obs
+00009e30: 6f6c 6574 652e 0a20 2020 2020 2020 2022  olete..        "
+00009e40: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00009e50: 6e20 7365 6c66 2e67 6574 5461 6741 7474  n self.getTagAtt
+00009e60: 7228 2765 7272 6f72 272c 2027 7479 7065  r('error', 'type
+00009e70: 2729 0a0a 2020 2020 6465 6620 6765 7453  ')..    def getS
+00009e80: 7461 7475 7343 6f6e 6469 7469 6f6e 7328  tatusConditions(
+00009e90: 7365 6c66 2c20 6173 5f63 6f64 653d 4661  self, as_code=Fa
+00009ea0: 6c73 6529 3a0a 2020 2020 2020 2020 2222  lse):.        ""
+00009eb0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00009ec0: 2074 6865 2073 7461 7475 7320 636f 6e64   the status cond
+00009ed0: 6974 696f 6e73 206c 6973 7420 6173 2064  itions list as d
+00009ee0: 6566 696e 6564 2069 6e20 5845 502d 3033  efined in XEP-03
+00009ef0: 3036 2e0a 2020 2020 2020 2020 2222 220a  06..        """.
+00009f00: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00009f10: 2073 6574 2829 0a20 2020 2020 2020 2073   set().        s
+00009f20: 7461 7475 735f 7461 6773 203d 2073 656c  tatus_tags = sel
+00009f30: 662e 6765 7454 6167 7328 2773 7461 7475  f.getTags('statu
+00009f40: 7327 290a 2020 2020 2020 2020 666f 7220  s').        for 
+00009f50: 7374 6174 7573 2069 6e20 7374 6174 7573  status in status
+00009f60: 5f74 6167 733a 0a20 2020 2020 2020 2020  _tags:.         
+00009f70: 2020 2069 6620 6173 5f63 6f64 653a 0a20     if as_code:. 
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009f90: 6f64 6520 3d20 7374 6174 7573 2e67 6574  ode = status.get
+00009fa0: 4174 7472 2827 636f 6465 2729 0a20 2020  Attr('code').   
+00009fb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009fc0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+00009fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009fe0: 2020 2020 2020 7265 7375 6c74 2e61 6464        result.add
+00009ff0: 2863 6f64 6529 0a20 2020 2020 2020 2020  (code).         
+0000a000: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a010: 2020 2020 2020 2020 2066 6f72 2063 6f6e           for con
+0000a020: 6469 7469 6f6e 2069 6e20 7374 6174 7573  dition in status
+0000a030: 2e67 6574 4368 696c 6472 656e 2829 3a0a  .getChildren():.
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a050: 2020 2020 7265 7375 6c74 2e61 6464 2863      result.add(c
+0000a060: 6f6e 6469 7469 6f6e 2e67 6574 4e61 6d65  ondition.getName
+0000a070: 2829 290a 2020 2020 2020 2020 7265 7475  ()).        retu
+0000a080: 726e 206c 6973 7428 7265 7375 6c74 290a  rn list(result).
+0000a090: 0a20 2020 2064 6566 2073 6574 4572 726f  .    def setErro
+0000a0a0: 7228 7365 6c66 2c20 6572 726f 722c 2063  r(self, error, c
+0000a0b0: 6f64 653d 4e6f 6e65 293a 0a20 2020 2020  ode=None):.     
+0000a0c0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+0000a0d0: 6574 2074 6865 2065 7272 6f72 2063 6f64  et the error cod
+0000a0e0: 652e 204f 6273 6f6c 6574 652e 2055 7365  e. Obsolete. Use
+0000a0f0: 2065 7272 6f72 2d63 6f6e 6469 7469 6f6e   error-condition
+0000a100: 7320 696e 7374 6561 640a 2020 2020 2020  s instead.      
+0000a110: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000a120: 2063 6f64 653a 0a20 2020 2020 2020 2020   code:.         
+0000a130: 2020 2069 6620 7374 7228 636f 6465 2920     if str(code) 
+0000a140: 696e 205f 6572 726f 7263 6f64 6573 2e6b  in _errorcodes.k
+0000a150: 6579 7328 293a 0a20 2020 2020 2020 2020  eys():.         
+0000a160: 2020 2020 2020 2065 7272 6f72 203d 2045         error = E
+0000a170: 7272 6f72 4e6f 6465 285f 6572 726f 7263  rrorNode(_errorc
+0000a180: 6f64 6573 5b73 7472 2863 6f64 6529 5d2c  odes[str(code)],
+0000a190: 2074 6578 743d 6572 726f 7229 0a20 2020   text=error).   
+0000a1a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a1c0: 7272 6f72 203d 2045 7272 6f72 4e6f 6465  rror = ErrorNode
+0000a1d0: 2845 5252 5f55 4e44 4546 494e 4544 5f43  (ERR_UNDEFINED_C
+0000a1e0: 4f4e 4449 5449 4f4e 2c20 636f 6465 3d63  ONDITION, code=c
+0000a1f0: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2020 2020 2020 2074 7970 3d27 6361 6e63         typ='canc
+0000a220: 656c 272c 2074 6578 743d 6572 726f 7229  el', text=error)
+0000a230: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+0000a240: 696e 7374 616e 6365 2865 7272 6f72 2c20  instance(error, 
+0000a250: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+0000a260: 2020 6572 726f 7220 3d20 4572 726f 724e    error = ErrorN
+0000a270: 6f64 6528 6572 726f 7229 0a20 2020 2020  ode(error).     
+0000a280: 2020 2073 656c 662e 7365 7454 7970 6528     self.setType(
+0000a290: 2765 7272 6f72 2729 0a20 2020 2020 2020  'error').       
+0000a2a0: 2073 656c 662e 6164 6443 6869 6c64 286e   self.addChild(n
+0000a2b0: 6f64 653d 6572 726f 7229 0a0a 2020 2020  ode=error)..    
+0000a2c0: 6465 6620 7365 7454 696d 6573 7461 6d70  def setTimestamp
+0000a2d0: 2873 656c 662c 2076 616c 3d4e 6f6e 6529  (self, val=None)
+0000a2e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000a2f0: 2020 2020 2020 5365 7420 7468 6520 7469        Set the ti
+0000a300: 6d65 7374 616d 702e 2074 696d 6573 7461  mestamp. timesta
+0000a310: 6d70 2073 686f 756c 6420 6265 2074 6865  mp should be the
+0000a320: 2079 7979 796d 6d64 6454 6868 6d6d 7373   yyyymmddThhmmss
+0000a330: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0000a340: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+0000a350: 6f74 2076 616c 3a0a 2020 2020 2020 2020  ot val:.        
+0000a360: 2020 2020 7661 6c20 3d20 7469 6d65 2e73      val = time.s
+0000a370: 7472 6674 696d 6528 2725 5925 6d25 6454  trftime('%Y%m%dT
+0000a380: 2548 3a25 4d3a 2553 272c 2074 696d 652e  %H:%M:%S', time.
+0000a390: 676d 7469 6d65 2829 290a 2020 2020 2020  gmtime()).      
+0000a3a0: 2020 7365 6c66 2e74 696d 6573 7461 6d70    self.timestamp
+0000a3b0: 3d76 616c 0a20 2020 2020 2020 2073 656c  =val.        sel
+0000a3c0: 662e 7365 7454 6167 2827 7827 2c20 7b27  f.setTag('x', {'
+0000a3d0: 7374 616d 7027 3a20 7365 6c66 2e74 696d  stamp': self.tim
+0000a3e0: 6573 7461 6d70 7d2c 206e 616d 6573 7061  estamp}, namespa
+0000a3f0: 6365 3d4e 616d 6573 7061 6365 2e44 454c  ce=Namespace.DEL
+0000a400: 4159 290a 0a20 2020 2064 6566 2067 6574  AY)..    def get
+0000a410: 5072 6f70 6572 7469 6573 2873 656c 6629  Properties(self)
+0000a420: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000a430: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+0000a440: 206c 6973 7420 6f66 206e 616d 6573 7061   list of namespa
+0000a450: 6365 7320 746f 2077 6869 6368 2062 656c  ces to which bel
+0000a460: 6f6e 6773 2074 6865 0a20 2020 2020 2020  ongs the.       
+0000a470: 2064 6972 6563 7420 6368 696c 6473 206f   direct childs o
+0000a480: 6620 656c 656d 656e 740a 2020 2020 2020  f element.      
+0000a490: 2020 2222 220a 2020 2020 2020 2020 7072    """.        pr
+0000a4a0: 6f70 7320 3d20 5b5d 0a20 2020 2020 2020  ops = [].       
+0000a4b0: 2066 6f72 2063 6869 6c64 2069 6e20 7365   for child in se
+0000a4c0: 6c66 2e67 6574 4368 696c 6472 656e 2829  lf.getChildren()
+0000a4d0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0000a4e0: 6f70 203d 2063 6869 6c64 2e67 6574 4e61  op = child.getNa
+0000a4f0: 6d65 7370 6163 6528 290a 2020 2020 2020  mespace().      
+0000a500: 2020 2020 2020 6966 2070 726f 7020 6e6f        if prop no
+0000a510: 7420 696e 2070 726f 7073 3a0a 2020 2020  t in props:.    
+0000a520: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+0000a530: 732e 6170 7065 6e64 2870 726f 7029 0a20  s.append(prop). 
+0000a540: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
+0000a550: 6f70 730a 0a20 2020 2064 6566 2067 6574  ops..    def get
+0000a560: 5461 6728 7365 6c66 2c0a 2020 2020 2020  Tag(self,.      
+0000a570: 2020 2020 2020 2020 206e 616d 653a 2073           name: s
+0000a580: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+0000a590: 2020 2061 7474 7273 3a20 4f70 7469 6f6e     attrs: Option
+0000a5a0: 616c 5b64 6963 745b 7374 722c 2041 6e79  al[dict[str, Any
+0000a5b0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000a5c0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
+0000a5d0: 6163 653a 204f 7074 696f 6e61 6c5b 7374  ace: Optional[st
+0000a5e0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000a5f0: 2020 2020 2020 2020 2020 7072 6f74 6f63            protoc
+0000a600: 6f6c 3a20 626f 6f6c 203d 2046 616c 7365  ol: bool = False
+0000a610: 2920 2d3e 204f 7074 696f 6e61 6c5b 4e6f  ) -> Optional[No
+0000a620: 6465 5d3a 0a20 2020 2020 2020 2022 2222  de]:.        """
+0000a630: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+0000a640: 7468 6520 4e6f 6465 2069 6e73 7461 6e63  the Node instanc
+0000a650: 6520 666f 7220 7468 6520 7461 672e 0a20  e for the tag.. 
+0000a660: 2020 2020 2020 2049 6620 7072 6f74 6f63         If protoc
+0000a670: 6f6c 2069 7320 5472 7565 2063 6f6e 7665  ol is True conve
+0000a680: 7274 2074 6f20 6120 6e65 7720 5072 6f74  rt to a new Prot
+0000a690: 6f63 6f6c 2f4d 6573 7361 6765 2069 6e73  ocol/Message ins
+0000a6a0: 7461 6e63 652e 0a20 2020 2020 2020 2022  tance..        "
+0000a6b0: 2222 0a20 2020 2020 2020 2074 6167 203d  "".        tag =
+0000a6c0: 204e 6f64 652e 6765 7454 6167 2873 656c   Node.getTag(sel
+0000a6d0: 662c 206e 616d 652c 2061 7474 7273 2c20  f, name, attrs, 
+0000a6e0: 6e61 6d65 7370 6163 6529 0a20 2020 2020  namespace).     
+0000a6f0: 2020 2069 6620 7072 6f74 6f63 6f6c 2061     if protocol a
+0000a700: 6e64 2074 6167 3a0a 2020 2020 2020 2020  nd tag:.        
+0000a710: 2020 2020 6966 206e 616d 6520 3d3d 2027      if name == '
+0000a720: 6d65 7373 6167 6527 3a0a 2020 2020 2020  message':.      
+0000a730: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a740: 204d 6573 7361 6765 286e 6f64 653d 7461   Message(node=ta
+0000a750: 6729 0a20 2020 2020 2020 2020 2020 2072  g).            r
+0000a760: 6574 7572 6e20 5072 6f74 6f63 6f6c 286e  eturn Protocol(n
+0000a770: 6f64 653d 7461 6729 0a20 2020 2020 2020  ode=tag).       
+0000a780: 2072 6574 7572 6e20 7461 670a 0a20 2020   return tag..   
+0000a790: 2064 6566 205f 5f73 6574 6974 656d 5f5f   def __setitem__
+0000a7a0: 2873 656c 662c 2069 7465 6d3a 2073 7472  (self, item: str
+0000a7b0: 2c20 7661 6c3a 2055 6e69 6f6e 5b73 7472  , val: Union[str
+0000a7c0: 2c20 4a49 445d 293a 0a20 2020 2020 2020  , JID]):.       
+0000a7d0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+0000a7e0: 2074 6865 2069 7465 6d20 2769 7465 6d27   the item 'item'
+0000a7f0: 2074 6f20 7468 6520 7661 6c75 6520 2776   to the value 'v
+0000a800: 616c 270a 2020 2020 2020 2020 2222 220a  al'.        """.
+0000a810: 2020 2020 2020 2020 6966 2069 7465 6d20          if item 
+0000a820: 696e 205b 2774 6f27 2c20 2766 726f 6d27  in ['to', 'from'
+0000a830: 5d3a 0a20 2020 2020 2020 2020 2020 2069  ]:.            i
+0000a840: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+0000a850: 2876 616c 2c20 4a49 4429 3a0a 2020 2020  (val, JID):.    
+0000a860: 2020 2020 2020 2020 2020 2020 7661 6c20              val 
+0000a870: 3d20 4a49 442e 6672 6f6d 5f73 7472 696e  = JID.from_strin
+0000a880: 6728 7661 6c29 0a20 2020 2020 2020 2073  g(val).        s
+0000a890: 656c 662e 7365 7441 7474 7228 6974 656d  elf.setAttr(item
+0000a8a0: 2c20 7661 6c29 0a0a 0a63 6c61 7373 204d  , val)...class M
+0000a8b0: 6573 7361 6765 2850 726f 746f 636f 6c29  essage(Protocol)
+0000a8c0: 3a0a 2020 2020 2222 220a 2020 2020 584d  :.    """.    XM
+0000a8d0: 5050 204d 6573 7361 6765 2073 7461 6e7a  PP Message stanz
+0000a8e0: 6120 2d20 2270 7573 6822 206d 6563 6861  a - "push" mecha
+0000a8f0: 6e69 736d 0a20 2020 2022 2222 0a0a 2020  nism.    """..  
+0000a900: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000a910: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000a920: 2020 2020 2020 746f 3d4e 6f6e 652c 0a20        to=None,. 
+0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a940: 626f 6479 3d4e 6f6e 652c 0a20 2020 2020  body=None,.     
+0000a950: 2020 2020 2020 2020 2020 2020 7868 746d              xhtm
+0000a960: 6c3d 4e6f 6e65 2c0a 2020 2020 2020 2020  l=None,.        
+0000a970: 2020 2020 2020 2020 2074 7970 3d4e 6f6e           typ=Non
+0000a980: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000a990: 2020 2020 7375 626a 6563 743d 4e6f 6e65      subject=None
+0000a9a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a9b0: 2020 2061 7474 7273 3d4e 6f6e 652c 0a20     attrs=None,. 
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 6672 6d3d 4e6f 6e65 2c0a 2020 2020 2020  frm=None,.      
+0000a9e0: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
+0000a9f0: 6164 3d4e 6f6e 652c 0a20 2020 2020 2020  ad=None,.       
+0000aa00: 2020 2020 2020 2020 2020 7469 6d65 7374            timest
+0000aa10: 616d 703d 4e6f 6e65 2c0a 2020 2020 2020  amp=None,.      
+0000aa20: 2020 2020 2020 2020 2020 2078 6d6c 6e73             xmlns
+0000aa30: 3d4e 616d 6573 7061 6365 2e43 4c49 454e  =Namespace.CLIEN
+0000aa40: 542c 0a20 2020 2020 2020 2020 2020 2020  T,.             
+0000aa50: 2020 2020 6e6f 6465 3d4e 6f6e 6529 3a0a      node=None):.
+0000aa60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000aa70: 2020 2020 596f 7520 6361 6e20 7370 6563      You can spec
+0000aa80: 6966 7920 7265 6369 7069 656e 742c 2074  ify recipient, t
+0000aa90: 6578 7420 6f66 206d 6573 7361 6765 2c20  ext of message, 
+0000aaa0: 7479 7065 206f 6620 6d65 7373 6167 6520  type of message 
+0000aab0: 616e 790a 2020 2020 2020 2020 6164 6469  any.        addi
+0000aac0: 7469 6f6e 616c 2061 7474 7269 6275 7465  tional attribute
+0000aad0: 732c 2073 656e 6465 7220 6f66 2074 6865  s, sender of the
+0000aae0: 206d 6573 7361 6765 2c20 616e 7920 6164   message, any ad
+0000aaf0: 6469 7469 6f6e 616c 2070 6179 6c6f 6164  ditional payload
+0000ab00: 0a20 2020 2020 2020 2028 662e 652e 206a  .        (f.e. j
+0000ab10: 6162 6265 723a 783a 6465 6c61 7920 656c  abber:x:delay el
+0000ab20: 656d 656e 7429 2061 6e64 206e 616d 6573  ement) and names
+0000ab30: 7061 6365 2069 6e20 6f6e 6520 676f 2e0a  pace in one go..
+0000ab40: 0a20 2020 2020 2020 2041 6c74 6572 6e61  .        Alterna
+0000ab50: 7469 7665 6c79 2079 6f75 2063 616e 2070  tively you can p
+0000ab60: 6173 7320 696e 2074 6865 206f 7468 6572  ass in the other
+0000ab70: 2058 4d4c 206f 626a 6563 7420 6173 2074   XML object as t
+0000ab80: 6865 2027 6e6f 6465 270a 2020 2020 2020  he 'node'.      
+0000ab90: 2020 7061 7261 6d65 7465 6420 746f 2072    parameted to r
+0000aba0: 6570 6c69 6361 7465 2069 7420 6173 206d  eplicate it as m
+0000abb0: 6573 7361 6765 0a20 2020 2020 2020 2022  essage.        "
+0000abc0: 2222 0a20 2020 2020 2020 2050 726f 746f  "".        Proto
+0000abd0: 636f 6c2e 5f5f 696e 6974 5f5f 2873 656c  col.__init__(sel
+0000abe0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000abf0: 2020 2020 2020 2020 2020 2020 2027 6d65               'me
+0000ac00: 7373 6167 6527 2c0a 2020 2020 2020 2020  ssage',.        
 0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac20: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
-0000ac30: 3d74 696d 6573 7461 6d70 2c0a 2020 2020  =timestamp,.    
-0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2020 2020 786d 6c6e 733d 786d 6c6e        xmlns=xmln
-0000ac60: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000ac70: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
-0000ac80: 653d 6e6f 6465 290a 2020 2020 2020 2020  e=node).        
-0000ac90: 6966 2062 6f64 793a 0a20 2020 2020 2020  if body:.       
-0000aca0: 2020 2020 2073 656c 662e 7365 7442 6f64       self.setBod
-0000acb0: 7928 626f 6479 290a 2020 2020 2020 2020  y(body).        
-0000acc0: 6966 2078 6874 6d6c 2069 7320 6e6f 7420  if xhtml is not 
-0000acd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ace0: 2020 7365 6c66 2e73 6574 5848 544d 4c28    self.setXHTML(
-0000acf0: 7868 746d 6c29 0a20 2020 2020 2020 2069  xhtml).        i
-0000ad00: 6620 7375 626a 6563 7420 6973 206e 6f74  f subject is not
-0000ad10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000ad20: 2020 2073 656c 662e 7365 7453 7562 6a65     self.setSubje
-0000ad30: 6374 2873 7562 6a65 6374 290a 0a20 2020  ct(subject)..   
-0000ad40: 2064 6566 2067 6574 426f 6479 2873 656c   def getBody(sel
-0000ad50: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-0000ad60: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-0000ad70: 6578 7420 6f66 2074 6865 206d 6573 7361  ext of the messa
-0000ad80: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
-0000ad90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ada0: 6c66 2e67 6574 5461 6744 6174 6128 2762  lf.getTagData('b
-0000adb0: 6f64 7927 290a 0a20 2020 2064 6566 2067  ody')..    def g
-0000adc0: 6574 5848 544d 4c28 7365 6c66 293a 0a20  etXHTML(self):. 
-0000add0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ade0: 6c66 2e67 6574 5461 6728 2768 746d 6c27  lf.getTag('html'
-0000adf0: 2c20 6e61 6d65 7370 6163 653d 4e61 6d65  , namespace=Name
-0000ae00: 7370 6163 652e 5848 544d 4c5f 494d 290a  space.XHTML_IM).
-0000ae10: 0a20 2020 2064 6566 2067 6574 5375 626a  .    def getSubj
-0000ae20: 6563 7428 7365 6c66 293a 0a20 2020 2020  ect(self):.     
-0000ae30: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000ae40: 6574 7572 6e20 7375 626a 6563 7420 6f66  eturn subject of
-0000ae50: 2074 6865 206d 6573 7361 6765 0a20 2020   the message.   
-0000ae60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ae70: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
-0000ae80: 5461 6744 6174 6128 2773 7562 6a65 6374  TagData('subject
-0000ae90: 2729 0a0a 2020 2020 6465 6620 6765 7454  ')..    def getT
-0000aea0: 6872 6561 6428 7365 6c66 293a 0a20 2020  hread(self):.   
-0000aeb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000aec0: 2052 6574 7572 6e20 7468 7265 6164 206f   Return thread o
-0000aed0: 6620 7468 6520 6d65 7373 6167 650a 2020  f the message.  
-0000aee0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000aef0: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
-0000af00: 7454 6167 4461 7461 2827 7468 7265 6164  tTagData('thread
-0000af10: 2729 0a0a 2020 2020 6465 6620 6765 744f  ')..    def getO
-0000af20: 7269 6769 6e49 4428 7365 6c66 293a 0a20  riginID(self):. 
-0000af30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000af40: 2020 2052 6574 7572 6e20 6f72 6967 696e     Return origin
-0000af50: 2d69 6420 6f66 2074 6865 206d 6573 7361  -id of the messa
-0000af60: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
-0000af70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000af80: 6c66 2e67 6574 5461 6741 7474 7228 276f  lf.getTagAttr('o
-0000af90: 7269 6769 6e2d 6964 272c 206e 616d 6573  rigin-id', names
-0000afa0: 7061 6365 3d4e 616d 6573 7061 6365 2e53  pace=Namespace.S
-0000afb0: 4944 2c20 6174 7472 3d27 6964 2729 0a0a  ID, attr='id')..
-0000afc0: 2020 2020 6465 6620 6765 7453 7461 6e7a      def getStanz
-0000afd0: 6149 4441 7474 7273 2873 656c 6629 3a0a  aIDAttrs(self):.
-0000afe0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000aff0: 2020 2020 5265 7475 726e 2074 6865 2073      Return the s
-0000b000: 7461 6e7a 612d 6964 2061 7474 7269 6275  tanza-id attribu
-0000b010: 7465 7320 6f66 2074 6865 206d 6573 7361  tes of the messa
-0000b020: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
-0000b030: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0000b040: 2020 2020 2020 2020 6174 7472 7320 3d20          attrs = 
-0000b050: 7365 6c66 2e67 6574 5461 6728 2773 7461  self.getTag('sta
-0000b060: 6e7a 612d 6964 272c 206e 616d 6573 7061  nza-id', namespa
-0000b070: 6365 3d4e 616d 6573 7061 6365 2e53 4944  ce=Namespace.SID
-0000b080: 292e 6765 7441 7474 7273 2829 0a20 2020  ).getAttrs().   
-0000b090: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-0000b0a0: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-0000b0b0: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
-0000b0c0: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
-0000b0d0: 7572 6e20 6174 7472 735b 2769 6427 5d2c  urn attrs['id'],
-0000b0e0: 2061 7474 7273 5b27 6279 275d 0a0a 2020   attrs['by']..  
-0000b0f0: 2020 6465 6620 7365 7442 6f64 7928 7365    def setBody(se
-0000b100: 6c66 2c20 7661 6c29 3a0a 2020 2020 2020  lf, val):.      
-0000b110: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000b120: 7420 7468 6520 7465 7874 206f 6620 7468  t the text of th
-0000b130: 6520 6d65 7373 6167 6522 2222 0a20 2020  e message""".   
-0000b140: 2020 2020 2073 656c 662e 7365 7454 6167       self.setTag
-0000b150: 4461 7461 2827 626f 6479 272c 2076 616c  Data('body', val
-0000b160: 290a 0a20 2020 2064 6566 2073 6574 5848  )..    def setXH
-0000b170: 544d 4c28 7365 6c66 2c20 626f 6479 2c20  TML(self, body, 
-0000b180: 6164 643d 4661 6c73 6529 3a0a 2020 2020  add=False):.    
-0000b190: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000b1a0: 6528 626f 6479 2c20 7374 7229 3a0a 2020  e(body, str):.  
-0000b1b0: 2020 2020 2020 2020 2020 626f 6479 203d            body =
-0000b1c0: 204e 6f64 6528 6e6f 6465 3d62 6f64 7929   Node(node=body)
-0000b1d0: 0a20 2020 2020 2020 2069 6620 6164 643a  .        if add:
-0000b1e0: 0a20 2020 2020 2020 2020 2020 2078 6874  .            xht
-0000b1f0: 6d6c 203d 2073 656c 662e 6765 7454 6167  ml = self.getTag
-0000b200: 2827 6874 6d6c 272c 206e 616d 6573 7061  ('html', namespa
-0000b210: 6365 3d4e 616d 6573 7061 6365 2e58 4854  ce=Namespace.XHT
-0000b220: 4d4c 5f49 4d29 0a20 2020 2020 2020 2020  ML_IM).         
-0000b230: 2020 2069 6620 7868 746d 6c20 6973 206e     if xhtml is n
-0000b240: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000b250: 2020 2020 2020 2020 2078 6874 6d6c 2e61           xhtml.a
-0000b260: 6464 4368 696c 6428 6e6f 6465 3d62 6f64  ddChild(node=bod
-0000b270: 7929 0a20 2020 2020 2020 2020 2020 2065  y).            e
-0000b280: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b290: 2020 2020 2073 656c 662e 6164 6443 6869       self.addChi
-0000b2a0: 6c64 2827 6874 6d6c 272c 0a20 2020 2020  ld('html',.     
-0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2c0: 2020 2020 2020 2020 206e 616d 6573 7061           namespa
-0000b2d0: 6365 3d4e 616d 6573 7061 6365 2e58 4854  ce=Namespace.XHT
-0000b2e0: 4d4c 5f49 4d2c 0a20 2020 2020 2020 2020  ML_IM,.         
-0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b300: 2020 2020 2070 6179 6c6f 6164 3d62 6f64       payload=bod
-0000b310: 7929 0a20 2020 2020 2020 2065 6c73 653a  y).        else:
-0000b320: 0a20 2020 2020 2020 2020 2020 2078 6874  .            xht
-0000b330: 6d6c 5f6e 6f64 6573 203d 2073 656c 662e  ml_nodes = self.
-0000b340: 6765 7454 6167 7328 2768 746d 6c27 2c20  getTags('html', 
-0000b350: 6e61 6d65 7370 6163 653d 4e61 6d65 7370  namespace=Namesp
-0000b360: 6163 652e 5848 544d 4c5f 494d 290a 2020  ace.XHTML_IM).  
-0000b370: 2020 2020 2020 2020 2020 666f 7220 7868            for xh
-0000b380: 746d 6c20 696e 2078 6874 6d6c 5f6e 6f64  tml in xhtml_nod
-0000b390: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000b3a0: 2020 2020 7365 6c66 2e64 656c 4368 696c      self.delChil
-0000b3b0: 6428 7868 746d 6c29 0a20 2020 2020 2020  d(xhtml).       
-0000b3c0: 2020 2020 2073 656c 662e 6164 6443 6869       self.addChi
-0000b3d0: 6c64 2827 6874 6d6c 272c 206e 616d 6573  ld('html', names
-0000b3e0: 7061 6365 3d4e 616d 6573 7061 6365 2e58  pace=Namespace.X
-0000b3f0: 4854 4d4c 5f49 4d2c 2070 6179 6c6f 6164  HTML_IM, payload
-0000b400: 3d62 6f64 7929 0a0a 2020 2020 6465 6620  =body)..    def 
-0000b410: 7365 7453 7562 6a65 6374 2873 656c 662c  setSubject(self,
-0000b420: 2076 616c 293a 0a20 2020 2020 2020 2022   val):.        "
-0000b430: 2222 0a20 2020 2020 2020 2053 6574 2074  "".        Set t
-0000b440: 6865 2073 7562 6a65 6374 206f 6620 7468  he subject of th
-0000b450: 6520 6d65 7373 6167 650a 2020 2020 2020  e message.      
-0000b460: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-0000b470: 6c66 2e73 6574 5461 6744 6174 6128 2773  lf.setTagData('s
-0000b480: 7562 6a65 6374 272c 2076 616c 290a 0a20  ubject', val).. 
-0000b490: 2020 2064 6566 2073 6574 5468 7265 6164     def setThread
-0000b4a0: 2873 656c 662c 2076 616c 293a 0a20 2020  (self, val):.   
-0000b4b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000b4c0: 2053 6574 2074 6865 2074 6872 6561 6420   Set the thread 
-0000b4d0: 6f66 2074 6865 206d 6573 7361 6765 0a20  of the message. 
-0000b4e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000b4f0: 2020 2073 656c 662e 7365 7454 6167 4461     self.setTagDa
-0000b500: 7461 2827 7468 7265 6164 272c 2076 616c  ta('thread', val
-0000b510: 290a 0a20 2020 2064 6566 2073 6574 4f72  )..    def setOr
-0000b520: 6967 696e 4944 2873 656c 662c 2076 616c  iginID(self, val
-0000b530: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000b540: 2020 2020 2020 2053 6574 7320 7468 6520         Sets the 
-0000b550: 6f72 6967 696e 2d69 6420 6f66 2074 6865  origin-id of the
-0000b560: 206d 6573 7361 6765 0a20 2020 2020 2020   message.       
-0000b570: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-0000b580: 662e 7365 7454 6167 2827 6f72 6967 696e  f.setTag('origin
-0000b590: 2d69 6427 2c20 6e61 6d65 7370 6163 653d  -id', namespace=
-0000b5a0: 4e61 6d65 7370 6163 652e 5349 442c 2061  Namespace.SID, a
-0000b5b0: 7474 7273 3d7b 2769 6427 3a20 7661 6c7d  ttrs={'id': val}
-0000b5c0: 290a 0a20 2020 2064 6566 2062 7569 6c64  )..    def build
-0000b5d0: 5265 706c 7928 7365 6c66 2c20 7465 7874  Reply(self, text
-0000b5e0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0000b5f0: 2222 220a 2020 2020 2020 2020 4275 696c  """.        Buil
-0000b600: 6473 2061 6e64 2072 6574 7572 6e73 2061  ds and returns a
-0000b610: 6e6f 7468 6572 206d 6573 7361 6765 206f  nother message o
-0000b620: 626a 6563 7420 7769 7468 2073 7065 6369  bject with speci
-0000b630: 6669 6564 2074 6578 742e 2054 6865 2074  fied text. The t
-0000b640: 6f2c 0a20 2020 2020 2020 2066 726f 6d2c  o,.        from,
-0000b650: 2074 6872 6561 6420 616e 6420 7479 7065   thread and type
-0000b660: 2070 726f 7065 7274 6965 7320 6f66 206e   properties of n
-0000b670: 6577 206d 6573 7361 6765 2061 7265 2070  ew message are p
-0000b680: 7265 2d73 6574 2061 7320 7265 706c 7920  re-set as reply 
-0000b690: 746f 0a20 2020 2020 2020 2074 6869 7320  to.        this 
-0000b6a0: 6d65 7373 6167 650a 2020 2020 2020 2020  message.        
-0000b6b0: 2222 220a 2020 2020 2020 2020 6d20 3d20  """.        m = 
-0000b6c0: 4d65 7373 6167 6528 746f 3d73 656c 662e  Message(to=self.
-0000b6d0: 6765 7446 726f 6d28 292c 0a20 2020 2020  getFrom(),.     
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000b6f0: 726d 3d73 656c 662e 6765 7454 6f28 292c  rm=self.getTo(),
-0000b700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b710: 2020 2020 2062 6f64 793d 7465 7874 2c0a       body=text,.
-0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b730: 2020 2020 7479 703d 7365 6c66 2e67 6574      typ=self.get
-0000b740: 5479 7065 2829 290a 2020 2020 2020 2020  Type()).        
-0000b750: 7468 203d 2073 656c 662e 6765 7454 6872  th = self.getThr
-0000b760: 6561 6428 290a 2020 2020 2020 2020 6966  ead().        if
-0000b770: 2074 683a 0a20 2020 2020 2020 2020 2020   th:.           
-0000b780: 206d 2e73 6574 5468 7265 6164 2874 6829   m.setThread(th)
-0000b790: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000b7a0: 6d0a 0a20 2020 2064 6566 2067 6574 5374  m..    def getSt
-0000b7b0: 6174 7573 436f 6465 2873 656c 6629 3a0a  atusCode(self):.
-0000b7c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b7d0: 2020 2020 5265 7475 726e 2074 6865 2073      Return the s
-0000b7e0: 7461 7475 7320 636f 6465 206f 6620 7468  tatus code of th
-0000b7f0: 6520 6d65 7373 6167 6520 2866 6f72 2067  e message (for g
-0000b800: 726f 7570 6368 6174 2063 6f6e 6669 6720  roupchat config 
-0000b810: 6368 616e 6765 290a 2020 2020 2020 2020  change).        
-0000b820: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
-0000b830: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-0000b840: 6f72 2078 7461 6720 696e 2073 656c 662e  or xtag in self.
-0000b850: 6765 7454 6167 7328 2778 2729 3a0a 2020  getTags('x'):.  
-0000b860: 2020 2020 2020 2020 2020 666f 7220 6368            for ch
-0000b870: 696c 6420 696e 2078 7461 672e 6765 7454  ild in xtag.getT
-0000b880: 6167 7328 2773 7461 7475 7327 293a 0a20  ags('status'):. 
-0000b890: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000b8a0: 7474 7273 2e61 7070 656e 6428 6368 696c  ttrs.append(chil
-0000b8b0: 642e 6765 7441 7474 7228 2763 6f64 6527  d.getAttr('code'
-0000b8c0: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-0000b8d0: 6e20 6174 7472 730a 0a20 2020 2064 6566  n attrs..    def
-0000b8e0: 2073 6574 4d61 726b 6572 2873 656c 662c   setMarker(self,
-0000b8f0: 2074 7970 655f 2c20 6964 5f29 3a0a 2020   type_, id_):.  
-0000b900: 2020 2020 2020 7365 6c66 2e73 6574 5461        self.setTa
-0000b910: 6728 7479 7065 5f2c 206e 616d 6573 7061  g(type_, namespa
-0000b920: 6365 3d4e 616d 6573 7061 6365 2e43 4841  ce=Namespace.CHA
-0000b930: 544d 4152 4b45 5253 2c20 6174 7472 733d  TMARKERS, attrs=
-0000b940: 7b27 6964 273a 2069 645f 7d29 0a0a 2020  {'id': id_})..  
-0000b950: 2020 6465 6620 7365 744d 6172 6b61 626c    def setMarkabl
-0000b960: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0000b970: 2073 656c 662e 7365 7454 6167 2827 6d61   self.setTag('ma
-0000b980: 726b 6162 6c65 272c 206e 616d 6573 7061  rkable', namespa
-0000b990: 6365 3d4e 616d 6573 7061 6365 2e43 4841  ce=Namespace.CHA
-0000b9a0: 544d 4152 4b45 5253 290a 0a20 2020 2064  TMARKERS)..    d
-0000b9b0: 6566 2073 6574 5265 6365 6970 7452 6571  ef setReceiptReq
-0000b9c0: 7565 7374 2873 656c 6629 3a0a 2020 2020  uest(self):.    
-0000b9d0: 2020 2020 7365 6c66 2e73 6574 5461 6728      self.setTag(
-0000b9e0: 2772 6571 7565 7374 272c 206e 616d 6573  'request', names
-0000b9f0: 7061 6365 3d4e 616d 6573 7061 6365 2e52  pace=Namespace.R
-0000ba00: 4543 4549 5054 5329 0a0a 2020 2020 6465  ECEIPTS)..    de
-0000ba10: 6620 7365 7452 6563 6569 7074 5265 6365  f setReceiptRece
-0000ba20: 6976 6564 2873 656c 662c 2069 645f 293a  ived(self, id_):
-0000ba30: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000ba40: 7454 6167 2827 7265 6365 6976 6564 272c  tTag('received',
-0000ba50: 206e 616d 6573 7061 6365 3d4e 616d 6573   namespace=Names
-0000ba60: 7061 6365 2e52 4543 4549 5054 532c 2061  pace.RECEIPTS, a
-0000ba70: 7474 7273 3d7b 2769 6427 3a20 6964 5f7d  ttrs={'id': id_}
-0000ba80: 290a 0a20 2020 2064 6566 2073 6574 5265  )..    def setRe
-0000ba90: 706c 7928 7365 6c66 2c0a 2020 2020 2020  ply(self,.      
-0000baa0: 2020 2020 2020 2020 2020 2072 6563 6970             recip
-0000bab0: 6965 6e74 5f6a 6964 3a20 7374 722c 0a20  ient_jid: str,. 
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 7265 706c 795f 746f 5f69 643a 2073 7472  reply_to_id: str
-0000bae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000baf0: 2020 2066 616c 6c62 6163 6b5f 7374 6172     fallback_star
-0000bb00: 743a 2069 6e74 2c0a 2020 2020 2020 2020  t: int,.        
-0000bb10: 2020 2020 2020 2020 2066 616c 6c62 6163           fallbac
-0000bb20: 6b5f 656e 643a 2069 6e74 0a20 2020 2020  k_end: int.     
-0000bb30: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
-0000bb40: 204e 6f6e 653a 0a0a 2020 2020 2020 2020   None:..        
-0000bb50: 7365 6c66 2e73 6574 5461 6728 0a20 2020  self.setTag(.   
-0000bb60: 2020 2020 2020 2020 2027 7265 706c 7927           'reply'
-0000bb70: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
-0000bb80: 6d65 7370 6163 653d 4e61 6d65 7370 6163  mespace=Namespac
-0000bb90: 652e 5245 504c 592c 0a20 2020 2020 2020  e.REPLY,.       
-0000bba0: 2020 2020 2061 7474 7273 3d7b 0a20 2020       attrs={.   
-0000bbb0: 2020 2020 2020 2020 2020 2020 2027 6964               'id
-0000bbc0: 273a 2072 6570 6c79 5f74 6f5f 6964 2c0a  ': reply_to_id,.
-0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbe0: 2774 6f27 3a20 7265 6369 7069 656e 745f  'to': recipient_
-0000bbf0: 6a69 647d 290a 0a20 2020 2020 2020 2066  jid})..        f
-0000bc00: 616c 6c62 6163 6b5f 7461 6720 3d20 7365  allback_tag = se
-0000bc10: 6c66 2e73 6574 5461 6728 0a20 2020 2020  lf.setTag(.     
-0000bc20: 2020 2020 2020 2027 6661 6c6c 6261 636b         'fallback
-0000bc30: 272c 0a20 2020 2020 2020 2020 2020 206e  ',.            n
-0000bc40: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
-0000bc50: 6365 2e46 414c 4c42 4143 4b2c 0a20 2020  ce.FALLBACK,.   
-0000bc60: 2020 2020 2020 2020 2061 7474 7273 3d7b           attrs={
-0000bc70: 2766 6f72 273a 204e 616d 6573 7061 6365  'for': Namespace
-0000bc80: 2e52 4550 4c59 7d29 0a20 2020 2020 2020  .REPLY}).       
-0000bc90: 2066 616c 6c62 6163 6b5f 7461 672e 6164   fallback_tag.ad
-0000bca0: 6443 6869 6c64 280a 2020 2020 2020 2020  dChild(.        
-0000bcb0: 2020 2020 2762 6f64 7927 2c0a 2020 2020      'body',.    
-0000bcc0: 2020 2020 2020 2020 6174 7472 733d 7b0a          attrs={.
-0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2773 7461 7274 273a 2073 7472 2866 616c  'start': str(fal
-0000bcf0: 6c62 6163 6b5f 7374 6172 7429 2c0a 2020  lback_start),.  
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2765                'e
-0000bd10: 6e64 273a 2073 7472 2866 616c 6c62 6163  nd': str(fallbac
-0000bd20: 6b5f 656e 6429 7d29 0a0a 2020 2020 6465  k_end)})..    de
-0000bd30: 6620 7365 744f 4f42 2873 656c 662c 2075  f setOOB(self, u
-0000bd40: 726c 2c20 6465 7363 3d4e 6f6e 6529 3a0a  rl, desc=None):.
-0000bd50: 2020 2020 2020 2020 6f6f 6220 3d20 7365          oob = se
-0000bd60: 6c66 2e73 6574 5461 6728 2778 272c 206e  lf.setTag('x', n
-0000bd70: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
-0000bd80: 6365 2e58 5f4f 4f42 290a 2020 2020 2020  ce.X_OOB).      
-0000bd90: 2020 6f6f 622e 7365 7454 6167 4461 7461    oob.setTagData
-0000bda0: 2827 7572 6c27 2c20 7572 6c29 0a20 2020  ('url', url).   
-0000bdb0: 2020 2020 2069 6620 6465 7363 2069 7320       if desc is 
-0000bdc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000bdd0: 2020 2020 2020 6f6f 622e 7365 7454 6167        oob.setTag
-0000bde0: 4461 7461 2827 6465 7363 272c 2064 6573  Data('desc', des
-0000bdf0: 6329 0a0a 2020 2020 6465 6620 7365 7443  c)..    def setC
-0000be00: 6f72 7265 6374 696f 6e28 7365 6c66 2c20  orrection(self, 
-0000be10: 6964 5f29 3a0a 2020 2020 2020 2020 7365  id_):.        se
-0000be20: 6c66 2e73 6574 5461 6728 2772 6570 6c61  lf.setTag('repla
-0000be30: 6365 272c 206e 616d 6573 7061 6365 3d4e  ce', namespace=N
-0000be40: 616d 6573 7061 6365 2e43 4f52 5245 4354  amespace.CORRECT
-0000be50: 2c20 6174 7472 733d 7b27 6964 273a 2069  , attrs={'id': i
-0000be60: 645f 7d29 0a0a 2020 2020 6465 6620 7365  d_})..    def se
-0000be70: 7441 7474 656e 7469 6f6e 2873 656c 6629  tAttention(self)
-0000be80: 3a0a 2020 2020 2020 2020 7365 6c66 2e73  :.        self.s
-0000be90: 6574 5461 6728 2761 7474 656e 7469 6f6e  etTag('attention
-0000bea0: 272c 206e 616d 6573 7061 6365 3d4e 616d  ', namespace=Nam
-0000beb0: 6573 7061 6365 2e41 5454 454e 5449 4f4e  espace.ATTENTION
-0000bec0: 290a 0a20 2020 2064 6566 2073 6574 4869  )..    def setHi
-0000bed0: 6e74 2873 656c 662c 2068 696e 7429 3a0a  nt(self, hint):.
-0000bee0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000bef0: 5461 6728 6869 6e74 2c20 6e61 6d65 7370  Tag(hint, namesp
-0000bf00: 6163 653d 4e61 6d65 7370 6163 652e 4849  ace=Namespace.HI
-0000bf10: 4e54 5329 0a0a 2020 2020 6465 6620 7365  NTS)..    def se
-0000bf20: 7452 6561 6374 696f 6e73 2873 656c 662c  tReactions(self,
-0000bf30: 2074 6172 6765 745f 6964 3a20 7374 722c   target_id: str,
-0000bf40: 2065 6d6f 6a69 733a 2049 7465 7261 626c   emojis: Iterabl
-0000bf50: 655b 7374 725d 293a 0a20 2020 2020 2020  e[str]):.       
-0000bf60: 2072 6561 6374 696f 6e73 203d 2073 656c   reactions = sel
-0000bf70: 662e 6164 6443 6869 6c64 280a 2020 2020  f.addChild(.    
-0000bf80: 2020 2020 2020 2020 2772 6561 6374 696f          'reactio
-0000bf90: 6e73 272c 206e 616d 6573 7061 6365 3d4e  ns', namespace=N
-0000bfa0: 616d 6573 7061 6365 2e52 4541 4354 494f  amespace.REACTIO
-0000bfb0: 4e53 2c20 6174 7472 733d 7b22 6964 223a  NS, attrs={"id":
-0000bfc0: 2074 6172 6765 745f 6964 7d29 0a20 2020   target_id}).   
-0000bfd0: 2020 2020 2066 6f72 2065 2069 6e20 656d       for e in em
-0000bfe0: 6f6a 6973 3a0a 2020 2020 2020 2020 2020  ojis:.          
-0000bff0: 2020 7265 6163 7469 6f6e 732e 6164 6443    reactions.addC
-0000c000: 6869 6c64 280a 2020 2020 2020 2020 2020  hild(.          
-0000c010: 2020 2020 2020 2772 6561 6374 696f 6e27        'reaction'
-0000c020: 2c20 6e61 6d65 7370 6163 653d 4e61 6d65  , namespace=Name
-0000c030: 7370 6163 652e 5245 4143 5449 4f4e 532c  space.REACTIONS,
-0000c040: 2070 6179 6c6f 6164 3d5b 655d 290a 0a20   payload=[e]).. 
-0000c050: 2020 2064 6566 2067 6574 5265 6163 7469     def getReacti
-0000c060: 6f6e 7328 7365 6c66 2920 2d3e 204f 7074  ons(self) -> Opt
-0000c070: 696f 6e61 6c5b 7475 706c 655b 7374 722c  ional[tuple[str,
-0000c080: 2073 6574 5b73 7472 5d5d 5d3a 0a20 2020   set[str]]]:.   
-0000c090: 2020 2020 2072 6561 6374 696f 6e73 203d       reactions =
-0000c0a0: 2073 656c 662e 6765 7454 6167 2827 7265   self.getTag('re
-0000c0b0: 6163 7469 6f6e 7327 2c20 6e61 6d65 7370  actions', namesp
-0000c0c0: 6163 653d 4e61 6d65 7370 6163 652e 5245  ace=Namespace.RE
-0000c0d0: 4143 5449 4f4e 5329 0a20 2020 2020 2020  ACTIONS).       
-0000c0e0: 2069 6620 6e6f 7420 7265 6163 7469 6f6e   if not reaction
-0000c0f0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-0000c100: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-0000c110: 2020 2020 7265 6163 745f 746f 203d 2072      react_to = r
-0000c120: 6561 6374 696f 6e73 2e67 6574 4174 7472  eactions.getAttr
-0000c130: 2827 6964 2729 0a20 2020 2020 2020 2069  ('id').        i
-0000c140: 6620 6e6f 7420 7265 6163 745f 746f 3a0a  f not react_to:.
-0000c150: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c160: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-0000c170: 2074 6167 7320 3d20 7265 6163 7469 6f6e   tags = reaction
-0000c180: 732e 6765 7454 6167 7328 2772 6561 6374  s.getTags('react
-0000c190: 696f 6e27 2c20 6e61 6d65 7370 6163 653d  ion', namespace=
-0000c1a0: 4e61 6d65 7370 6163 652e 5245 4143 5449  Namespace.REACTI
-0000c1b0: 4f4e 5329 0a0a 2020 2020 2020 2020 2320  ONS)..        # 
-0000c1c0: 7374 7269 7028 2920 696e 2063 6173 6520  strip() in case 
-0000c1d0: 636c 6965 6e74 7320 7375 7272 6f75 6e64  clients surround
-0000c1e0: 2065 6d6f 6a69 7320 7769 7468 2077 6869   emojis with whi
-0000c1f0: 7465 7370 6163 650a 2020 2020 2020 2020  tespace.        
-0000c200: 7265 7475 726e 2072 6561 6374 5f74 6f2c  return react_to,
-0000c210: 207b 742e 6765 7444 6174 6128 292e 7374   {t.getData().st
-0000c220: 7269 7028 2920 666f 7220 7420 696e 2074  rip() for t in t
-0000c230: 6167 737d 0a0a 0a63 6c61 7373 2050 7265  ags}...class Pre
-0000c240: 7365 6e63 6528 5072 6f74 6f63 6f6c 293a  sence(Protocol):
-0000c250: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0000c260: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
-0000c270: 2020 2020 2020 2020 2020 746f 3d4e 6f6e            to=Non
-0000c280: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000c290: 2020 2020 7479 703d 4e6f 6e65 2c0a 2020      typ=None,.  
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000c2b0: 7269 6f72 6974 793d 4e6f 6e65 2c0a 2020  riority=None,.  
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c2d0: 686f 773d 4e6f 6e65 2c0a 2020 2020 2020  how=None,.      
-0000c2e0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-0000c2f0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0000c300: 2020 2020 2020 2020 2061 7474 7273 3d4e           attrs=N
-0000c310: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000c320: 2020 2020 2020 6672 6d3d 4e6f 6e65 2c0a        frm=None,.
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2074 696d 6573 7461 6d70 3d4e 6f6e 652c   timestamp=None,
-0000c350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c360: 2020 7061 796c 6f61 643d 4e6f 6e65 2c0a    payload=None,.
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2078 6d6c 6e73 3d4e 616d 6573 7061 6365   xmlns=Namespace
-0000c390: 2e43 4c49 454e 542c 0a20 2020 2020 2020  .CLIENT,.       
-0000c3a0: 2020 2020 2020 2020 2020 6e6f 6465 3d4e            node=N
-0000c3b0: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-0000c3c0: 220a 2020 2020 2020 2020 596f 7520 6361  ".        You ca
-0000c3d0: 6e20 7370 6563 6966 7920 7265 6369 7069  n specify recipi
-0000c3e0: 656e 742c 2074 7970 6520 6f66 206d 6573  ent, type of mes
-0000c3f0: 7361 6765 2c20 7072 696f 7269 7479 2c20  sage, priority, 
-0000c400: 7368 6f77 2061 6e64 2073 7461 7475 730a  show and status.
-0000c410: 2020 2020 2020 2020 7661 6c75 6573 2061          values a
-0000c420: 6e79 2061 6464 6974 696f 6e61 6c20 6174  ny additional at
-0000c430: 7472 6962 7574 6573 2c20 7365 6e64 6572  tributes, sender
-0000c440: 206f 6620 7468 6520 7072 6573 656e 6365   of the presence
-0000c450: 2c20 7469 6d65 7374 616d 702c 2061 6e79  , timestamp, any
-0000c460: 0a20 2020 2020 2020 2061 6464 6974 696f  .        additio
-0000c470: 6e61 6c20 7061 796c 6f61 6420 2866 2e65  nal payload (f.e
-0000c480: 2e20 6a61 6262 6572 3a78 3a64 656c 6179  . jabber:x:delay
-0000c490: 2065 6c65 6d65 6e74 2920 616e 6420 6e61   element) and na
-0000c4a0: 6d65 7370 6163 6520 696e 206f 6e65 0a20  mespace in one. 
-0000c4b0: 2020 2020 2020 2067 6f2e 2041 6c74 6572         go. Alter
-0000c4c0: 6e61 7469 7665 6c79 2079 6f75 2063 616e  natively you can
-0000c4d0: 2070 6173 7320 696e 2074 6865 206f 7468   pass in the oth
-0000c4e0: 6572 2058 4d4c 206f 626a 6563 7420 6173  er XML object as
-0000c4f0: 2074 6865 2027 6e6f 6465 270a 2020 2020   the 'node'.    
-0000c500: 2020 2020 7061 7261 6d65 7465 6420 746f      parameted to
-0000c510: 2072 6570 6c69 6361 7465 2069 7420 6173   replicate it as
-0000c520: 2070 7265 7365 6e63 650a 2020 2020 2020   presence.      
-0000c530: 2020 2222 220a 2020 2020 2020 2020 5072    """.        Pr
-0000c540: 6f74 6f63 6f6c 2e5f 5f69 6e69 745f 5f28  otocol.__init__(
-0000c550: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 2770 7265 7365 6e63 6527 2c0a 2020 2020  'presence',.    
-0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 2020 2020 746f 3d74 6f2c 0a20 2020        to=to,.   
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 2020 2020 2020 2074 7970 3d74 7970 2c0a         typ=typ,.
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 2020 2020 2020 6174 7472 733d            attrs=
-0000c5e0: 6174 7472 732c 0a20 2020 2020 2020 2020  attrs,.         
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c600: 2066 726d 3d66 726d 2c0a 2020 2020 2020   frm=frm,.      
+0000ac20: 2020 746f 3d74 6f2c 0a20 2020 2020 2020    to=to,.       
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac40: 2020 2074 7970 3d74 7970 2c0a 2020 2020     typ=typ,.    
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 6174 7472 733d 6174 7472        attrs=attr
+0000ac70: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000ac80: 2020 2020 2020 2020 2020 2020 2066 726d               frm
+0000ac90: 3d66 726d 2c0a 2020 2020 2020 2020 2020  =frm,.          
+0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 7061 796c 6f61 643d 7061 796c 6f61 642c  payload=payload,
+0000acc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000acd0: 2020 2020 2020 2020 2020 2074 696d 6573             times
+0000ace0: 7461 6d70 3d74 696d 6573 7461 6d70 2c0a  tamp=timestamp,.
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad00: 2020 2020 2020 2020 2020 786d 6c6e 733d            xmlns=
+0000ad10: 786d 6c6e 732c 0a20 2020 2020 2020 2020  xmlns,.         
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 206e 6f64 653d 6e6f 6465 290a 2020 2020   node=node).    
+0000ad40: 2020 2020 6966 2062 6f64 793a 0a20 2020      if body:.   
+0000ad50: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000ad60: 7442 6f64 7928 626f 6479 290a 2020 2020  tBody(body).    
+0000ad70: 2020 2020 6966 2078 6874 6d6c 2069 7320      if xhtml is 
+0000ad80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000ad90: 2020 2020 2020 7365 6c66 2e73 6574 5848        self.setXH
+0000ada0: 544d 4c28 7868 746d 6c29 0a20 2020 2020  TML(xhtml).     
+0000adb0: 2020 2069 6620 7375 626a 6563 7420 6973     if subject is
+0000adc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000add0: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
+0000ade0: 7562 6a65 6374 2873 7562 6a65 6374 290a  ubject(subject).
+0000adf0: 0a20 2020 2064 6566 2067 6574 426f 6479  .    def getBody
+0000ae00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ae10: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000ae20: 726e 2074 6578 7420 6f66 2074 6865 206d  rn text of the m
+0000ae30: 6573 7361 6765 0a20 2020 2020 2020 2022  essage.        "
+0000ae40: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000ae50: 6e20 7365 6c66 2e67 6574 5461 6744 6174  n self.getTagDat
+0000ae60: 6128 2762 6f64 7927 290a 0a20 2020 2064  a('body')..    d
+0000ae70: 6566 2067 6574 5848 544d 4c28 7365 6c66  ef getXHTML(self
+0000ae80: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0000ae90: 6e20 7365 6c66 2e67 6574 5461 6728 2768  n self.getTag('h
+0000aea0: 746d 6c27 2c20 6e61 6d65 7370 6163 653d  tml', namespace=
+0000aeb0: 4e61 6d65 7370 6163 652e 5848 544d 4c5f  Namespace.XHTML_
+0000aec0: 494d 290a 0a20 2020 2064 6566 2067 6574  IM)..    def get
+0000aed0: 5375 626a 6563 7428 7365 6c66 293a 0a20  Subject(self):. 
+0000aee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000aef0: 2020 2052 6574 7572 6e20 7375 626a 6563     Return subjec
+0000af00: 7420 6f66 2074 6865 206d 6573 7361 6765  t of the message
+0000af10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000af20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000af30: 2e67 6574 5461 6744 6174 6128 2773 7562  .getTagData('sub
+0000af40: 6a65 6374 2729 0a0a 2020 2020 6465 6620  ject')..    def 
+0000af50: 6765 7454 6872 6561 6428 7365 6c66 293a  getThread(self):
+0000af60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000af70: 2020 2020 2052 6574 7572 6e20 7468 7265       Return thre
+0000af80: 6164 206f 6620 7468 6520 6d65 7373 6167  ad of the messag
+0000af90: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+0000afa0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000afb0: 662e 6765 7454 6167 4461 7461 2827 7468  f.getTagData('th
+0000afc0: 7265 6164 2729 0a0a 2020 2020 6465 6620  read')..    def 
+0000afd0: 6765 744f 7269 6769 6e49 4428 7365 6c66  getOriginID(self
+0000afe0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000aff0: 2020 2020 2020 2052 6574 7572 6e20 6f72         Return or
+0000b000: 6967 696e 2d69 6420 6f66 2074 6865 206d  igin-id of the m
+0000b010: 6573 7361 6765 0a20 2020 2020 2020 2022  essage.        "
+0000b020: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000b030: 6e20 7365 6c66 2e67 6574 5461 6741 7474  n self.getTagAtt
+0000b040: 7228 276f 7269 6769 6e2d 6964 272c 206e  r('origin-id', n
+0000b050: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
+0000b060: 6365 2e53 4944 2c20 6174 7472 3d27 6964  ce.SID, attr='id
+0000b070: 2729 0a0a 2020 2020 6465 6620 6765 7453  ')..    def getS
+0000b080: 7461 6e7a 6149 4441 7474 7273 2873 656c  tanzaIDAttrs(sel
+0000b090: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+0000b0a0: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+0000b0b0: 6865 2073 7461 6e7a 612d 6964 2061 7474  he stanza-id att
+0000b0c0: 7269 6275 7465 7320 6f66 2074 6865 206d  ributes of the m
+0000b0d0: 6573 7361 6765 0a20 2020 2020 2020 2022  essage.        "
+0000b0e0: 2222 0a20 2020 2020 2020 2074 7279 3a0a  "".        try:.
+0000b0f0: 2020 2020 2020 2020 2020 2020 6174 7472              attr
+0000b100: 7320 3d20 7365 6c66 2e67 6574 5461 6728  s = self.getTag(
+0000b110: 2773 7461 6e7a 612d 6964 272c 206e 616d  'stanza-id', nam
+0000b120: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
+0000b130: 2e53 4944 292e 6765 7441 7474 7273 2829  .SID).getAttrs()
+0000b140: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000b150: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
+0000b160: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000b170: 6e65 2c20 4e6f 6e65 0a20 2020 2020 2020  ne, None.       
+0000b180: 2072 6574 7572 6e20 6174 7472 735b 2769   return attrs['i
+0000b190: 6427 5d2c 2061 7474 7273 5b27 6279 275d  d'], attrs['by']
+0000b1a0: 0a0a 2020 2020 6465 6620 7365 7442 6f64  ..    def setBod
+0000b1b0: 7928 7365 6c66 2c20 7661 6c29 3a0a 2020  y(self, val):.  
+0000b1c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b1d0: 2020 5365 7420 7468 6520 7465 7874 206f    Set the text o
+0000b1e0: 6620 7468 6520 6d65 7373 6167 6522 2222  f the message"""
+0000b1f0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000b200: 7454 6167 4461 7461 2827 626f 6479 272c  tTagData('body',
+0000b210: 2076 616c 290a 0a20 2020 2064 6566 2073   val)..    def s
+0000b220: 6574 5848 544d 4c28 7365 6c66 2c20 626f  etXHTML(self, bo
+0000b230: 6479 2c20 6164 643d 4661 6c73 6529 3a0a  dy, add=False):.
+0000b240: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000b250: 7461 6e63 6528 626f 6479 2c20 7374 7229  tance(body, str)
+0000b260: 3a0a 2020 2020 2020 2020 2020 2020 626f  :.            bo
+0000b270: 6479 203d 204e 6f64 6528 6e6f 6465 3d62  dy = Node(node=b
+0000b280: 6f64 7929 0a20 2020 2020 2020 2069 6620  ody).        if 
+0000b290: 6164 643a 0a20 2020 2020 2020 2020 2020  add:.           
+0000b2a0: 2078 6874 6d6c 203d 2073 656c 662e 6765   xhtml = self.ge
+0000b2b0: 7454 6167 2827 6874 6d6c 272c 206e 616d  tTag('html', nam
+0000b2c0: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
+0000b2d0: 2e58 4854 4d4c 5f49 4d29 0a20 2020 2020  .XHTML_IM).     
+0000b2e0: 2020 2020 2020 2069 6620 7868 746d 6c20         if xhtml 
+0000b2f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000b300: 2020 2020 2020 2020 2020 2020 2078 6874               xht
+0000b310: 6d6c 2e61 6464 4368 696c 6428 6e6f 6465  ml.addChild(node
+0000b320: 3d62 6f64 7929 0a20 2020 2020 2020 2020  =body).         
+0000b330: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b340: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+0000b350: 6443 6869 6c64 2827 6874 6d6c 272c 0a20  dChild('html',. 
+0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b370: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0000b380: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
+0000b390: 2e58 4854 4d4c 5f49 4d2c 0a20 2020 2020  .XHTML_IM,.     
+0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3b0: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
+0000b3c0: 3d62 6f64 7929 0a20 2020 2020 2020 2065  =body).        e
+0000b3d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000b3e0: 2078 6874 6d6c 5f6e 6f64 6573 203d 2073   xhtml_nodes = s
+0000b3f0: 656c 662e 6765 7454 6167 7328 2768 746d  elf.getTags('htm
+0000b400: 6c27 2c20 6e61 6d65 7370 6163 653d 4e61  l', namespace=Na
+0000b410: 6d65 7370 6163 652e 5848 544d 4c5f 494d  mespace.XHTML_IM
+0000b420: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000b430: 7220 7868 746d 6c20 696e 2078 6874 6d6c  r xhtml in xhtml
+0000b440: 5f6e 6f64 6573 3a0a 2020 2020 2020 2020  _nodes:.        
+0000b450: 2020 2020 2020 2020 7365 6c66 2e64 656c          self.del
+0000b460: 4368 696c 6428 7868 746d 6c29 0a20 2020  Child(xhtml).   
+0000b470: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+0000b480: 6443 6869 6c64 2827 6874 6d6c 272c 206e  dChild('html', n
+0000b490: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
+0000b4a0: 6365 2e58 4854 4d4c 5f49 4d2c 2070 6179  ce.XHTML_IM, pay
+0000b4b0: 6c6f 6164 3d62 6f64 7929 0a0a 2020 2020  load=body)..    
+0000b4c0: 6465 6620 7365 7453 7562 6a65 6374 2873  def setSubject(s
+0000b4d0: 656c 662c 2076 616c 293a 0a20 2020 2020  elf, val):.     
+0000b4e0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+0000b4f0: 6574 2074 6865 2073 7562 6a65 6374 206f  et the subject o
+0000b500: 6620 7468 6520 6d65 7373 6167 650a 2020  f the message.  
+0000b510: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b520: 2020 7365 6c66 2e73 6574 5461 6744 6174    self.setTagDat
+0000b530: 6128 2773 7562 6a65 6374 272c 2076 616c  a('subject', val
+0000b540: 290a 0a20 2020 2064 6566 2073 6574 5468  )..    def setTh
+0000b550: 7265 6164 2873 656c 662c 2076 616c 293a  read(self, val):
+0000b560: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000b570: 2020 2020 2053 6574 2074 6865 2074 6872       Set the thr
+0000b580: 6561 6420 6f66 2074 6865 206d 6573 7361  ead of the messa
+0000b590: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
+0000b5a0: 2020 2020 2020 2073 656c 662e 7365 7454         self.setT
+0000b5b0: 6167 4461 7461 2827 7468 7265 6164 272c  agData('thread',
+0000b5c0: 2076 616c 290a 0a20 2020 2064 6566 2073   val)..    def s
+0000b5d0: 6574 4f72 6967 696e 4944 2873 656c 662c  etOriginID(self,
+0000b5e0: 2076 616c 293a 0a20 2020 2020 2020 2022   val):.        "
+0000b5f0: 2222 0a20 2020 2020 2020 2053 6574 7320  "".        Sets 
+0000b600: 7468 6520 6f72 6967 696e 2d69 6420 6f66  the origin-id of
+0000b610: 2074 6865 206d 6573 7361 6765 0a20 2020   the message.   
+0000b620: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000b630: 2073 656c 662e 7365 7454 6167 2827 6f72   self.setTag('or
+0000b640: 6967 696e 2d69 6427 2c20 6e61 6d65 7370  igin-id', namesp
+0000b650: 6163 653d 4e61 6d65 7370 6163 652e 5349  ace=Namespace.SI
+0000b660: 442c 2061 7474 7273 3d7b 2769 6427 3a20  D, attrs={'id': 
+0000b670: 7661 6c7d 290a 0a20 2020 2064 6566 2062  val})..    def b
+0000b680: 7569 6c64 5265 706c 7928 7365 6c66 2c20  uildReply(self, 
+0000b690: 7465 7874 3d4e 6f6e 6529 3a0a 2020 2020  text=None):.    
+0000b6a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000b6b0: 4275 696c 6473 2061 6e64 2072 6574 7572  Builds and retur
+0000b6c0: 6e73 2061 6e6f 7468 6572 206d 6573 7361  ns another messa
+0000b6d0: 6765 206f 626a 6563 7420 7769 7468 2073  ge object with s
+0000b6e0: 7065 6369 6669 6564 2074 6578 742e 2054  pecified text. T
+0000b6f0: 6865 2074 6f2c 0a20 2020 2020 2020 2066  he to,.        f
+0000b700: 726f 6d2c 2074 6872 6561 6420 616e 6420  rom, thread and 
+0000b710: 7479 7065 2070 726f 7065 7274 6965 7320  type properties 
+0000b720: 6f66 206e 6577 206d 6573 7361 6765 2061  of new message a
+0000b730: 7265 2070 7265 2d73 6574 2061 7320 7265  re pre-set as re
+0000b740: 706c 7920 746f 0a20 2020 2020 2020 2074  ply to.        t
+0000b750: 6869 7320 6d65 7373 6167 650a 2020 2020  his message.    
+0000b760: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000b770: 6d20 3d20 4d65 7373 6167 6528 746f 3d73  m = Message(to=s
+0000b780: 656c 662e 6765 7446 726f 6d28 292c 0a20  elf.getFrom(),. 
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 2020 2066 726d 3d73 656c 662e 6765 7454     frm=self.getT
+0000b7b0: 6f28 292c 0a20 2020 2020 2020 2020 2020  o(),.           
+0000b7c0: 2020 2020 2020 2020 2062 6f64 793d 7465           body=te
+0000b7d0: 7874 2c0a 2020 2020 2020 2020 2020 2020  xt,.            
+0000b7e0: 2020 2020 2020 2020 7479 703d 7365 6c66          typ=self
+0000b7f0: 2e67 6574 5479 7065 2829 290a 2020 2020  .getType()).    
+0000b800: 2020 2020 7468 203d 2073 656c 662e 6765      th = self.ge
+0000b810: 7454 6872 6561 6428 290a 2020 2020 2020  tThread().      
+0000b820: 2020 6966 2074 683a 0a20 2020 2020 2020    if th:.       
+0000b830: 2020 2020 206d 2e73 6574 5468 7265 6164       m.setThread
+0000b840: 2874 6829 0a20 2020 2020 2020 2072 6574  (th).        ret
+0000b850: 7572 6e20 6d0a 0a20 2020 2064 6566 2067  urn m..    def g
+0000b860: 6574 5374 6174 7573 436f 6465 2873 656c  etStatusCode(sel
+0000b870: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+0000b880: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+0000b890: 6865 2073 7461 7475 7320 636f 6465 206f  he status code o
+0000b8a0: 6620 7468 6520 6d65 7373 6167 6520 2866  f the message (f
+0000b8b0: 6f72 2067 726f 7570 6368 6174 2063 6f6e  or groupchat con
+0000b8c0: 6669 6720 6368 616e 6765 290a 2020 2020  fig change).    
+0000b8d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000b8e0: 6174 7472 7320 3d20 5b5d 0a20 2020 2020  attrs = [].     
+0000b8f0: 2020 2066 6f72 2078 7461 6720 696e 2073     for xtag in s
+0000b900: 656c 662e 6765 7454 6167 7328 2778 2729  elf.getTags('x')
+0000b910: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0000b920: 7220 6368 696c 6420 696e 2078 7461 672e  r child in xtag.
+0000b930: 6765 7454 6167 7328 2773 7461 7475 7327  getTags('status'
+0000b940: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000b950: 2020 2061 7474 7273 2e61 7070 656e 6428     attrs.append(
+0000b960: 6368 696c 642e 6765 7441 7474 7228 2763  child.getAttr('c
+0000b970: 6f64 6527 2929 0a20 2020 2020 2020 2072  ode')).        r
+0000b980: 6574 7572 6e20 6174 7472 730a 0a20 2020  eturn attrs..   
+0000b990: 2064 6566 2073 6574 4d61 726b 6572 2873   def setMarker(s
+0000b9a0: 656c 662c 2074 7970 655f 2c20 6964 5f29  elf, type_, id_)
+0000b9b0: 3a0a 2020 2020 2020 2020 7365 6c66 2e73  :.        self.s
+0000b9c0: 6574 5461 6728 7479 7065 5f2c 206e 616d  etTag(type_, nam
+0000b9d0: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
+0000b9e0: 2e43 4841 544d 4152 4b45 5253 2c20 6174  .CHATMARKERS, at
+0000b9f0: 7472 733d 7b27 6964 273a 2069 645f 7d29  trs={'id': id_})
+0000ba00: 0a0a 2020 2020 6465 6620 7365 744d 6172  ..    def setMar
+0000ba10: 6b61 626c 6528 7365 6c66 293a 0a20 2020  kable(self):.   
+0000ba20: 2020 2020 2073 656c 662e 7365 7454 6167       self.setTag
+0000ba30: 2827 6d61 726b 6162 6c65 272c 206e 616d  ('markable', nam
+0000ba40: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
+0000ba50: 2e43 4841 544d 4152 4b45 5253 290a 0a20  .CHATMARKERS).. 
+0000ba60: 2020 2064 6566 2073 6574 5265 6365 6970     def setReceip
+0000ba70: 7452 6571 7565 7374 2873 656c 6629 3a0a  tRequest(self):.
+0000ba80: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000ba90: 5461 6728 2772 6571 7565 7374 272c 206e  Tag('request', n
+0000baa0: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
+0000bab0: 6365 2e52 4543 4549 5054 5329 0a0a 2020  ce.RECEIPTS)..  
+0000bac0: 2020 6465 6620 7365 7452 6563 6569 7074    def setReceipt
+0000bad0: 5265 6365 6976 6564 2873 656c 662c 2069  Received(self, i
+0000bae0: 645f 293a 0a20 2020 2020 2020 2073 656c  d_):.        sel
+0000baf0: 662e 7365 7454 6167 2827 7265 6365 6976  f.setTag('receiv
+0000bb00: 6564 272c 206e 616d 6573 7061 6365 3d4e  ed', namespace=N
+0000bb10: 616d 6573 7061 6365 2e52 4543 4549 5054  amespace.RECEIPT
+0000bb20: 532c 2061 7474 7273 3d7b 2769 6427 3a20  S, attrs={'id': 
+0000bb30: 6964 5f7d 290a 0a20 2020 2064 6566 2073  id_})..    def s
+0000bb40: 6574 5265 706c 7928 7365 6c66 2c0a 2020  etReply(self,.  
+0000bb50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000bb60: 6563 6970 6965 6e74 5f6a 6964 3a20 7374  ecipient_jid: st
+0000bb70: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000bb80: 2020 2020 7265 706c 795f 746f 5f69 643a      reply_to_id:
+0000bb90: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+0000bba0: 2020 2020 2020 2066 616c 6c62 6163 6b5f         fallback_
+0000bbb0: 7374 6172 743a 2069 6e74 2c0a 2020 2020  start: int,.    
+0000bbc0: 2020 2020 2020 2020 2020 2020 2066 616c               fal
+0000bbd0: 6c62 6163 6b5f 656e 643a 2069 6e74 0a20  lback_end: int. 
+0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbf0: 2920 2d3e 204e 6f6e 653a 0a0a 2020 2020  ) -> None:..    
+0000bc00: 2020 2020 7365 6c66 2e73 6574 5461 6728      self.setTag(
+0000bc10: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
+0000bc20: 706c 7927 2c0a 2020 2020 2020 2020 2020  ply',.          
+0000bc30: 2020 6e61 6d65 7370 6163 653d 4e61 6d65    namespace=Name
+0000bc40: 7370 6163 652e 5245 504c 592c 0a20 2020  space.REPLY,.   
+0000bc50: 2020 2020 2020 2020 2061 7474 7273 3d7b           attrs={
+0000bc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc70: 2027 6964 273a 2072 6570 6c79 5f74 6f5f   'id': reply_to_
+0000bc80: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000bc90: 2020 2020 2774 6f27 3a20 7265 6369 7069      'to': recipi
+0000bca0: 656e 745f 6a69 647d 290a 0a20 2020 2020  ent_jid})..     
+0000bcb0: 2020 2066 616c 6c62 6163 6b5f 7461 6720     fallback_tag 
+0000bcc0: 3d20 7365 6c66 2e73 6574 5461 6728 0a20  = self.setTag(. 
+0000bcd0: 2020 2020 2020 2020 2020 2027 6661 6c6c             'fall
+0000bce0: 6261 636b 272c 0a20 2020 2020 2020 2020  back',.         
+0000bcf0: 2020 206e 616d 6573 7061 6365 3d4e 616d     namespace=Nam
+0000bd00: 6573 7061 6365 2e46 414c 4c42 4143 4b2c  espace.FALLBACK,
+0000bd10: 0a20 2020 2020 2020 2020 2020 2061 7474  .            att
+0000bd20: 7273 3d7b 2766 6f72 273a 204e 616d 6573  rs={'for': Names
+0000bd30: 7061 6365 2e52 4550 4c59 7d29 0a20 2020  pace.REPLY}).   
+0000bd40: 2020 2020 2066 616c 6c62 6163 6b5f 7461       fallback_ta
+0000bd50: 672e 6164 6443 6869 6c64 280a 2020 2020  g.addChild(.    
+0000bd60: 2020 2020 2020 2020 2762 6f64 7927 2c0a          'body',.
+0000bd70: 2020 2020 2020 2020 2020 2020 6174 7472              attr
+0000bd80: 733d 7b0a 2020 2020 2020 2020 2020 2020  s={.            
+0000bd90: 2020 2020 2773 7461 7274 273a 2073 7472      'start': str
+0000bda0: 2866 616c 6c62 6163 6b5f 7374 6172 7429  (fallback_start)
+0000bdb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bdc0: 2020 2765 6e64 273a 2073 7472 2866 616c    'end': str(fal
+0000bdd0: 6c62 6163 6b5f 656e 6429 7d29 0a0a 2020  lback_end)})..  
+0000bde0: 2020 6465 6620 7365 744f 4f42 2873 656c    def setOOB(sel
+0000bdf0: 662c 2075 726c 2c20 6465 7363 3d4e 6f6e  f, url, desc=Non
+0000be00: 6529 3a0a 2020 2020 2020 2020 6f6f 6220  e):.        oob 
+0000be10: 3d20 7365 6c66 2e73 6574 5461 6728 2778  = self.setTag('x
+0000be20: 272c 206e 616d 6573 7061 6365 3d4e 616d  ', namespace=Nam
+0000be30: 6573 7061 6365 2e58 5f4f 4f42 290a 2020  espace.X_OOB).  
+0000be40: 2020 2020 2020 6f6f 622e 7365 7454 6167        oob.setTag
+0000be50: 4461 7461 2827 7572 6c27 2c20 7572 6c29  Data('url', url)
+0000be60: 0a20 2020 2020 2020 2069 6620 6465 7363  .        if desc
+0000be70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000be80: 2020 2020 2020 2020 2020 6f6f 622e 7365            oob.se
+0000be90: 7454 6167 4461 7461 2827 6465 7363 272c  tTagData('desc',
+0000bea0: 2064 6573 6329 0a0a 2020 2020 6465 6620   desc)..    def 
+0000beb0: 7365 7443 6f72 7265 6374 696f 6e28 7365  setCorrection(se
+0000bec0: 6c66 2c20 6964 5f29 3a0a 2020 2020 2020  lf, id_):.      
+0000bed0: 2020 7365 6c66 2e73 6574 5461 6728 2772    self.setTag('r
+0000bee0: 6570 6c61 6365 272c 206e 616d 6573 7061  eplace', namespa
+0000bef0: 6365 3d4e 616d 6573 7061 6365 2e43 4f52  ce=Namespace.COR
+0000bf00: 5245 4354 2c20 6174 7472 733d 7b27 6964  RECT, attrs={'id
+0000bf10: 273a 2069 645f 7d29 0a0a 2020 2020 6465  ': id_})..    de
+0000bf20: 6620 7365 7441 7474 656e 7469 6f6e 2873  f setAttention(s
+0000bf30: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0000bf40: 6c66 2e73 6574 5461 6728 2761 7474 656e  lf.setTag('atten
+0000bf50: 7469 6f6e 272c 206e 616d 6573 7061 6365  tion', namespace
+0000bf60: 3d4e 616d 6573 7061 6365 2e41 5454 454e  =Namespace.ATTEN
+0000bf70: 5449 4f4e 290a 0a20 2020 2064 6566 2073  TION)..    def s
+0000bf80: 6574 4869 6e74 2873 656c 662c 2068 696e  etHint(self, hin
+0000bf90: 7429 3a0a 2020 2020 2020 2020 7365 6c66  t):.        self
+0000bfa0: 2e73 6574 5461 6728 6869 6e74 2c20 6e61  .setTag(hint, na
+0000bfb0: 6d65 7370 6163 653d 4e61 6d65 7370 6163  mespace=Namespac
+0000bfc0: 652e 4849 4e54 5329 0a0a 2020 2020 6465  e.HINTS)..    de
+0000bfd0: 6620 7365 7452 6561 6374 696f 6e73 2873  f setReactions(s
+0000bfe0: 656c 662c 2074 6172 6765 745f 6964 3a20  elf, target_id: 
+0000bff0: 7374 722c 2065 6d6f 6a69 733a 2049 7465  str, emojis: Ite
+0000c000: 7261 626c 655b 7374 725d 293a 0a20 2020  rable[str]):.   
+0000c010: 2020 2020 2072 6561 6374 696f 6e73 203d       reactions =
+0000c020: 2073 656c 662e 6164 6443 6869 6c64 280a   self.addChild(.
+0000c030: 2020 2020 2020 2020 2020 2020 2772 6561              'rea
+0000c040: 6374 696f 6e73 272c 206e 616d 6573 7061  ctions', namespa
+0000c050: 6365 3d4e 616d 6573 7061 6365 2e52 4541  ce=Namespace.REA
+0000c060: 4354 494f 4e53 2c20 6174 7472 733d 7b22  CTIONS, attrs={"
+0000c070: 6964 223a 2074 6172 6765 745f 6964 7d29  id": target_id})
+0000c080: 0a20 2020 2020 2020 2066 6f72 2065 2069  .        for e i
+0000c090: 6e20 656d 6f6a 6973 3a0a 2020 2020 2020  n emojis:.      
+0000c0a0: 2020 2020 2020 7265 6163 7469 6f6e 732e        reactions.
+0000c0b0: 6164 6443 6869 6c64 280a 2020 2020 2020  addChild(.      
+0000c0c0: 2020 2020 2020 2020 2020 2772 6561 6374            'react
+0000c0d0: 696f 6e27 2c20 6e61 6d65 7370 6163 653d  ion', namespace=
+0000c0e0: 4e61 6d65 7370 6163 652e 5245 4143 5449  Namespace.REACTI
+0000c0f0: 4f4e 532c 2070 6179 6c6f 6164 3d5b 655d  ONS, payload=[e]
+0000c100: 290a 0a20 2020 2064 6566 2067 6574 5265  )..    def getRe
+0000c110: 6163 7469 6f6e 7328 7365 6c66 2920 2d3e  actions(self) ->
+0000c120: 204f 7074 696f 6e61 6c5b 7475 706c 655b   Optional[tuple[
+0000c130: 7374 722c 2073 6574 5b73 7472 5d5d 5d3a  str, set[str]]]:
+0000c140: 0a20 2020 2020 2020 2072 6561 6374 696f  .        reactio
+0000c150: 6e73 203d 2073 656c 662e 6765 7454 6167  ns = self.getTag
+0000c160: 2827 7265 6163 7469 6f6e 7327 2c20 6e61  ('reactions', na
+0000c170: 6d65 7370 6163 653d 4e61 6d65 7370 6163  mespace=Namespac
+0000c180: 652e 5245 4143 5449 4f4e 5329 0a20 2020  e.REACTIONS).   
+0000c190: 2020 2020 2069 6620 6e6f 7420 7265 6163       if not reac
+0000c1a0: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+0000c1b0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+0000c1c0: 2020 2020 2020 2020 7265 6163 745f 746f          react_to
+0000c1d0: 203d 2072 6561 6374 696f 6e73 2e67 6574   = reactions.get
+0000c1e0: 4174 7472 2827 6964 2729 0a20 2020 2020  Attr('id').     
+0000c1f0: 2020 2069 6620 6e6f 7420 7265 6163 745f     if not react_
+0000c200: 746f 3a0a 2020 2020 2020 2020 2020 2020  to:.            
+0000c210: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000c220: 2020 2020 2074 6167 7320 3d20 7265 6163       tags = reac
+0000c230: 7469 6f6e 732e 6765 7454 6167 7328 2772  tions.getTags('r
+0000c240: 6561 6374 696f 6e27 2c20 6e61 6d65 7370  eaction', namesp
+0000c250: 6163 653d 4e61 6d65 7370 6163 652e 5245  ace=Namespace.RE
+0000c260: 4143 5449 4f4e 5329 0a0a 2020 2020 2020  ACTIONS)..      
+0000c270: 2020 2320 7374 7269 7028 2920 696e 2063    # strip() in c
+0000c280: 6173 6520 636c 6965 6e74 7320 7375 7272  ase clients surr
+0000c290: 6f75 6e64 2065 6d6f 6a69 7320 7769 7468  ound emojis with
+0000c2a0: 2077 6869 7465 7370 6163 650a 2020 2020   whitespace.    
+0000c2b0: 2020 2020 7265 7475 726e 2072 6561 6374      return react
+0000c2c0: 5f74 6f2c 207b 742e 6765 7444 6174 6128  _to, {t.getData(
+0000c2d0: 292e 7374 7269 7028 2920 666f 7220 7420  ).strip() for t 
+0000c2e0: 696e 2074 6167 737d 0a0a 0a63 6c61 7373  in tags}...class
+0000c2f0: 2050 7265 7365 6e63 6528 5072 6f74 6f63   Presence(Protoc
+0000c300: 6f6c 293a 0a0a 2020 2020 6465 6620 5f5f  ol):..    def __
+0000c310: 696e 6974 5f5f 2873 656c 662c 0a20 2020  init__(self,.   
+0000c320: 2020 2020 2020 2020 2020 2020 2020 746f                to
+0000c330: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0000c340: 2020 2020 2020 2020 7479 703d 4e6f 6e65          typ=None
+0000c350: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c360: 2020 2070 7269 6f72 6974 793d 4e6f 6e65     priority=None
+0000c370: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c380: 2020 2073 686f 773d 4e6f 6e65 2c0a 2020     show=None,.  
+0000c390: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c3a0: 7461 7475 733d 4e6f 6e65 2c0a 2020 2020  tatus=None,.    
+0000c3b0: 2020 2020 2020 2020 2020 2020 2061 7474               att
+0000c3c0: 7273 3d4e 6f6e 652c 0a20 2020 2020 2020  rs=None,.       
+0000c3d0: 2020 2020 2020 2020 2020 6672 6d3d 4e6f            frm=No
+0000c3e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000c3f0: 2020 2020 2074 696d 6573 7461 6d70 3d4e       timestamp=N
+0000c400: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000c410: 2020 2020 2020 7061 796c 6f61 643d 4e6f        payload=No
+0000c420: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000c430: 2020 2020 2078 6d6c 6e73 3d4e 616d 6573       xmlns=Names
+0000c440: 7061 6365 2e43 4c49 454e 542c 0a20 2020  pace.CLIENT,.   
+0000c450: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+0000c460: 6465 3d4e 6f6e 6529 3a0a 2020 2020 2020  de=None):.      
+0000c470: 2020 2222 220a 2020 2020 2020 2020 596f    """.        Yo
+0000c480: 7520 6361 6e20 7370 6563 6966 7920 7265  u can specify re
+0000c490: 6369 7069 656e 742c 2074 7970 6520 6f66  cipient, type of
+0000c4a0: 206d 6573 7361 6765 2c20 7072 696f 7269   message, priori
+0000c4b0: 7479 2c20 7368 6f77 2061 6e64 2073 7461  ty, show and sta
+0000c4c0: 7475 730a 2020 2020 2020 2020 7661 6c75  tus.        valu
+0000c4d0: 6573 2061 6e79 2061 6464 6974 696f 6e61  es any additiona
+0000c4e0: 6c20 6174 7472 6962 7574 6573 2c20 7365  l attributes, se
+0000c4f0: 6e64 6572 206f 6620 7468 6520 7072 6573  nder of the pres
+0000c500: 656e 6365 2c20 7469 6d65 7374 616d 702c  ence, timestamp,
+0000c510: 2061 6e79 0a20 2020 2020 2020 2061 6464   any.        add
+0000c520: 6974 696f 6e61 6c20 7061 796c 6f61 6420  itional payload 
+0000c530: 2866 2e65 2e20 6a61 6262 6572 3a78 3a64  (f.e. jabber:x:d
+0000c540: 656c 6179 2065 6c65 6d65 6e74 2920 616e  elay element) an
+0000c550: 6420 6e61 6d65 7370 6163 6520 696e 206f  d namespace in o
+0000c560: 6e65 0a20 2020 2020 2020 2067 6f2e 2041  ne.        go. A
+0000c570: 6c74 6572 6e61 7469 7665 6c79 2079 6f75  lternatively you
+0000c580: 2063 616e 2070 6173 7320 696e 2074 6865   can pass in the
+0000c590: 206f 7468 6572 2058 4d4c 206f 626a 6563   other XML objec
+0000c5a0: 7420 6173 2074 6865 2027 6e6f 6465 270a  t as the 'node'.
+0000c5b0: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
+0000c5c0: 6420 746f 2072 6570 6c69 6361 7465 2069  d to replicate i
+0000c5d0: 7420 6173 2070 7265 7365 6e63 650a 2020  t as presence.  
+0000c5e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c5f0: 2020 5072 6f74 6f63 6f6c 2e5f 5f69 6e69    Protocol.__ini
+0000c600: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
 0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2020 2020 7061 796c 6f61 643d 7061 796c      payload=payl
-0000c630: 6f61 642c 0a20 2020 2020 2020 2020 2020  oad,.           
-0000c640: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000c650: 696d 6573 7461 6d70 3d74 696d 6573 7461  imestamp=timesta
-0000c660: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-0000c670: 2020 2020 2020 2020 2020 2020 2020 786d                xm
-0000c680: 6c6e 733d 786d 6c6e 732c 0a20 2020 2020  lns=xmlns,.     
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6a0: 2020 2020 206e 6f64 653d 6e6f 6465 290a       node=node).
-0000c6b0: 2020 2020 2020 2020 6966 2070 7269 6f72          if prior
-0000c6c0: 6974 793a 0a20 2020 2020 2020 2020 2020  ity:.           
-0000c6d0: 2073 656c 662e 7365 7450 7269 6f72 6974   self.setPriorit
-0000c6e0: 7928 7072 696f 7269 7479 290a 2020 2020  y(priority).    
-0000c6f0: 2020 2020 6966 2073 686f 773a 0a20 2020      if show:.   
-0000c700: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000c710: 7453 686f 7728 7368 6f77 290a 2020 2020  tShow(show).    
-0000c720: 2020 2020 6966 2073 7461 7475 733a 0a20      if status:. 
-0000c730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c740: 7365 7453 7461 7475 7328 7374 6174 7573  setStatus(status
-0000c750: 290a 0a20 2020 2064 6566 2067 6574 5072  )..    def getPr
-0000c760: 696f 7269 7479 2873 656c 6629 3a0a 2020  iority(self):.  
-0000c770: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c780: 2020 5265 7475 726e 2074 6865 2070 7269    Return the pri
-0000c790: 6f72 6974 7920 6f66 2074 6865 206d 6573  ority of the mes
-0000c7a0: 7361 6765 0a20 2020 2020 2020 2022 2222  sage.        """
-0000c7b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c7c0: 7365 6c66 2e67 6574 5461 6744 6174 6128  self.getTagData(
-0000c7d0: 2770 7269 6f72 6974 7927 290a 0a20 2020  'priority')..   
-0000c7e0: 2064 6566 2067 6574 5368 6f77 2873 656c   def getShow(sel
-0000c7f0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-0000c800: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-0000c810: 6865 2073 686f 7720 7661 6c75 6520 6f66  he show value of
-0000c820: 2074 6865 206d 6573 7361 6765 0a20 2020   the message.   
-0000c830: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c840: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
-0000c850: 5461 6744 6174 6128 2773 686f 7727 290a  TagData('show').
-0000c860: 0a20 2020 2064 6566 2067 6574 5374 6174  .    def getStat
-0000c870: 7573 2873 656c 6629 3a0a 2020 2020 2020  us(self):.      
-0000c880: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0000c890: 7475 726e 2074 6865 2073 7461 7475 7320  turn the status 
-0000c8a0: 7374 7269 6e67 206f 6620 7468 6520 6d65  string of the me
-0000c8b0: 7373 6167 650a 2020 2020 2020 2020 2222  ssage.        ""
-0000c8c0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000c8d0: 2073 656c 662e 6765 7454 6167 4461 7461   self.getTagData
-0000c8e0: 2827 7374 6174 7573 2729 206f 7220 2727  ('status') or ''
-0000c8f0: 0a0a 2020 2020 6465 6620 7365 7450 7269  ..    def setPri
-0000c900: 6f72 6974 7928 7365 6c66 2c20 7661 6c29  ority(self, val)
-0000c910: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000c920: 2020 2020 2020 5365 7420 7468 6520 7072        Set the pr
-0000c930: 696f 7269 7479 206f 6620 7468 6520 6d65  iority of the me
-0000c940: 7373 6167 650a 2020 2020 2020 2020 2222  ssage.        ""
-0000c950: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
-0000c960: 6574 5461 6744 6174 6128 2770 7269 6f72  etTagData('prior
-0000c970: 6974 7927 2c20 7661 6c29 0a0a 2020 2020  ity', val)..    
-0000c980: 6465 6620 7365 7453 686f 7728 7365 6c66  def setShow(self
-0000c990: 2c20 7661 6c29 3a0a 2020 2020 2020 2020  , val):.        
-0000c9a0: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
-0000c9b0: 7468 6520 7368 6f77 2076 616c 7565 206f  the show value o
-0000c9c0: 6620 7468 6520 6d65 7373 6167 650a 2020  f the message.  
-0000c9d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c9e0: 2020 6966 2076 616c 206e 6f74 2069 6e20    if val not in 
-0000c9f0: 5b27 6177 6179 272c 2027 6368 6174 272c  ['away', 'chat',
-0000ca00: 2027 646e 6427 2c20 2778 6127 5d3a 0a20   'dnd', 'xa']:. 
-0000ca10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000ca20: 2056 616c 7565 4572 726f 7228 2749 6e76   ValueError('Inv
-0000ca30: 616c 6964 2073 686f 7720 7661 6c75 653a  alid show value:
-0000ca40: 2025 7327 2025 2076 616c 290a 2020 2020   %s' % val).    
-0000ca50: 2020 2020 7365 6c66 2e73 6574 5461 6744      self.setTagD
-0000ca60: 6174 6128 2773 686f 7727 2c20 7661 6c29  ata('show', val)
-0000ca70: 0a0a 2020 2020 6465 6620 7365 7453 7461  ..    def setSta
-0000ca80: 7475 7328 7365 6c66 2c20 7661 6c29 3a0a  tus(self, val):.
-0000ca90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000caa0: 2020 2020 5365 7420 7468 6520 7374 6174      Set the stat
-0000cab0: 7573 2073 7472 696e 6720 6f66 2074 6865  us string of the
-0000cac0: 206d 6573 7361 6765 0a20 2020 2020 2020   message.       
-0000cad0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-0000cae0: 662e 7365 7454 6167 4461 7461 2827 7374  f.setTagData('st
-0000caf0: 6174 7573 272c 2076 616c 290a 0a20 2020  atus', val)..   
-0000cb00: 2064 6566 205f 6d75 635f 6765 7449 7465   def _muc_getIte
-0000cb10: 6d41 7474 7228 7365 6c66 2c20 7461 672c  mAttr(self, tag,
-0000cb20: 2061 7474 7229 3a0a 2020 2020 2020 2020   attr):.        
-0000cb30: 666f 7220 7874 6167 2069 6e20 7365 6c66  for xtag in self
-0000cb40: 2e67 6574 5461 6773 2827 7827 293a 0a20  .getTags('x'):. 
-0000cb50: 2020 2020 2020 2020 2020 2069 6620 7874             if xt
-0000cb60: 6167 2e67 6574 4e61 6d65 7370 6163 6528  ag.getNamespace(
-0000cb70: 2920 6e6f 7420 696e 2028 4e61 6d65 7370  ) not in (Namesp
-0000cb80: 6163 652e 4d55 435f 5553 4552 2c0a 2020  ace.MUC_USER,.  
-0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbb0: 2020 2020 2020 2020 204e 616d 6573 7061           Namespa
-0000cbc0: 6365 2e4d 5543 5f41 444d 494e 293a 0a20  ce.MUC_ADMIN):. 
-0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cbe0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000cbf0: 2020 2020 666f 7220 6368 696c 6420 696e      for child in
-0000cc00: 2078 7461 672e 6765 7454 6167 7328 7461   xtag.getTags(ta
-0000cc10: 6729 3a0a 2020 2020 2020 2020 2020 2020  g):.            
-0000cc20: 2020 2020 7265 7475 726e 2063 6869 6c64      return child
-0000cc30: 2e67 6574 4174 7472 2861 7474 7229 0a0a  .getAttr(attr)..
-0000cc40: 2020 2020 6465 6620 5f6d 7563 5f67 6574      def _muc_get
-0000cc50: 5375 6254 6167 4461 7461 4174 7472 2873  SubTagDataAttr(s
-0000cc60: 656c 662c 2074 6167 2c20 6174 7472 293a  elf, tag, attr):
-0000cc70: 0a20 2020 2020 2020 2066 6f72 2078 7461  .        for xta
-0000cc80: 6720 696e 2073 656c 662e 6765 7454 6167  g in self.getTag
-0000cc90: 7328 2778 2729 3a0a 2020 2020 2020 2020  s('x'):.        
-0000cca0: 2020 2020 6966 2078 7461 672e 6765 744e      if xtag.getN
-0000ccb0: 616d 6573 7061 6365 2829 206e 6f74 2069  amespace() not i
-0000ccc0: 6e20 284e 616d 6573 7061 6365 2e4d 5543  n (Namespace.MUC
-0000ccd0: 5f55 5345 522c 0a20 2020 2020 2020 2020  _USER,.         
-0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd00: 2020 4e61 6d65 7370 6163 652e 4d55 435f    Namespace.MUC_
-0000cd10: 4144 4d49 4e29 3a0a 2020 2020 2020 2020  ADMIN):.        
-0000cd20: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000cd30: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000cd40: 2063 6869 6c64 2069 6e20 7874 6167 2e67   child in xtag.g
-0000cd50: 6574 5461 6773 2827 6974 656d 2729 3a0a  etTags('item'):.
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 666f 7220 6363 6869 6c64 2069 6e20 6368  for cchild in ch
-0000cd80: 696c 642e 6765 7454 6167 7328 7461 6729  ild.getTags(tag)
-0000cd90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cda0: 2020 2020 2020 7265 7475 726e 2063 6368        return cch
-0000cdb0: 696c 642e 6765 7444 6174 6128 292c 2063  ild.getData(), c
-0000cdc0: 6368 696c 642e 6765 7441 7474 7228 6174  child.getAttr(at
-0000cdd0: 7472 290a 2020 2020 2020 2020 7265 7475  tr).        retu
-0000cde0: 726e 204e 6f6e 652c 204e 6f6e 650a 0a20  rn None, None.. 
-0000cdf0: 2020 2064 6566 2067 6574 526f 6c65 2873     def getRole(s
-0000ce00: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000ce10: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-0000ce20: 2074 6865 2070 7265 7365 6e63 6520 726f   the presence ro
-0000ce30: 6c65 2028 666f 7220 6772 6f75 7063 6861  le (for groupcha
-0000ce40: 7429 0a20 2020 2020 2020 2022 2222 0a20  t).        """. 
-0000ce50: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ce60: 6c66 2e5f 6d75 635f 6765 7449 7465 6d41  lf._muc_getItemA
-0000ce70: 7474 7228 2769 7465 6d27 2c20 2772 6f6c  ttr('item', 'rol
-0000ce80: 6527 290a 0a20 2020 2064 6566 2067 6574  e')..    def get
-0000ce90: 4166 6669 6c69 6174 696f 6e28 7365 6c66  Affiliation(self
-0000cea0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000ceb0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-0000cec0: 6520 7072 6573 656e 6365 2061 6666 696c  e presence affil
-0000ced0: 6961 7469 6f6e 2028 666f 7220 6772 6f75  iation (for grou
-0000cee0: 7063 6861 7429 0a20 2020 2020 2020 2022  pchat).        "
-0000cef0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0000cf00: 6e20 7365 6c66 2e5f 6d75 635f 6765 7449  n self._muc_getI
-0000cf10: 7465 6d41 7474 7228 2769 7465 6d27 2c20  temAttr('item', 
-0000cf20: 2761 6666 696c 6961 7469 6f6e 2729 0a0a  'affiliation')..
-0000cf30: 2020 2020 6465 6620 6765 744e 6577 4e69      def getNewNi
-0000cf40: 636b 2873 656c 6629 3a0a 2020 2020 2020  ck(self):.      
-0000cf50: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0000cf60: 7475 726e 2074 6865 2073 7461 7475 7320  turn the status 
-0000cf70: 636f 6465 206f 6620 7468 6520 7072 6573  code of the pres
-0000cf80: 656e 6365 2028 666f 7220 6772 6f75 7063  ence (for groupc
-0000cf90: 6861 7429 0a20 2020 2020 2020 2022 2222  hat).        """
-0000cfa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cfb0: 7365 6c66 2e5f 6d75 635f 6765 7449 7465  self._muc_getIte
-0000cfc0: 6d41 7474 7228 2769 7465 6d27 2c20 276e  mAttr('item', 'n
-0000cfd0: 6963 6b27 290a 0a20 2020 2064 6566 2067  ick')..    def g
-0000cfe0: 6574 4a69 6428 7365 6c66 293a 0a20 2020  etJid(self):.   
-0000cff0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000d000: 2052 6574 7572 6e20 7468 6520 7072 6573   Return the pres
-0000d010: 656e 6365 206a 6964 2028 666f 7220 6772  ence jid (for gr
-0000d020: 6f75 7063 6861 7429 0a20 2020 2020 2020  oupchat).       
-0000d030: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000d040: 7572 6e20 7365 6c66 2e5f 6d75 635f 6765  urn self._muc_ge
-0000d050: 7449 7465 6d41 7474 7228 2769 7465 6d27  tItemAttr('item'
-0000d060: 2c20 276a 6964 2729 0a0a 2020 2020 6465  , 'jid')..    de
-0000d070: 6620 6765 7452 6561 736f 6e28 7365 6c66  f getReason(self
-0000d080: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000d090: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
-0000d0a0: 6865 2072 6561 736f 6e20 6f66 2074 6865  he reason of the
-0000d0b0: 2070 7265 7365 6e63 6520 2866 6f72 2067   presence (for g
-0000d0c0: 726f 7570 6368 6174 290a 2020 2020 2020  roupchat).      
-0000d0d0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0000d0e0: 7475 726e 2073 656c 662e 5f6d 7563 5f67  turn self._muc_g
-0000d0f0: 6574 5375 6254 6167 4461 7461 4174 7472  etSubTagDataAttr
-0000d100: 2827 7265 6173 6f6e 272c 2027 2729 5b30  ('reason', '')[0
-0000d110: 5d0a 0a20 2020 2064 6566 2067 6574 4163  ]..    def getAc
-0000d120: 746f 7228 7365 6c66 293a 0a20 2020 2020  tor(self):.     
-0000d130: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000d140: 6574 7572 6e20 7468 6520 7265 6173 6f6e  eturn the reason
-0000d150: 206f 6620 7468 6520 7072 6573 656e 6365   of the presence
-0000d160: 2028 666f 7220 6772 6f75 7063 6861 7429   (for groupchat)
-0000d170: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d180: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000d190: 2e5f 6d75 635f 6765 7453 7562 5461 6744  ._muc_getSubTagD
-0000d1a0: 6174 6141 7474 7228 2761 6374 6f72 272c  ataAttr('actor',
-0000d1b0: 2027 6a69 6427 295b 315d 0a0a 2020 2020   'jid')[1]..    
-0000d1c0: 6465 6620 6765 7453 7461 7475 7343 6f64  def getStatusCod
-0000d1d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0000d1e0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-0000d1f0: 7572 6e20 7468 6520 7374 6174 7573 2063  urn the status c
-0000d200: 6f64 6520 6f66 2074 6865 2070 7265 7365  ode of the prese
-0000d210: 6e63 6520 2866 6f72 2067 726f 7570 6368  nce (for groupch
-0000d220: 6174 290a 2020 2020 2020 2020 2222 220a  at).        """.
-0000d230: 2020 2020 2020 2020 6174 7472 7320 3d20          attrs = 
-0000d240: 5b5d 0a20 2020 2020 2020 2066 6f72 2078  [].        for x
-0000d250: 7461 6720 696e 2073 656c 662e 6765 7454  tag in self.getT
-0000d260: 6167 7328 2778 2729 3a0a 2020 2020 2020  ags('x'):.      
-0000d270: 2020 2020 2020 666f 7220 6368 696c 6420        for child 
-0000d280: 696e 2078 7461 672e 6765 7454 6167 7328  in xtag.getTags(
-0000d290: 2773 7461 7475 7327 293a 0a20 2020 2020  'status'):.     
-0000d2a0: 2020 2020 2020 2020 2020 2061 7474 7273             attrs
-0000d2b0: 2e61 7070 656e 6428 6368 696c 642e 6765  .append(child.ge
-0000d2c0: 7441 7474 7228 2763 6f64 6527 2929 0a20  tAttr('code')). 
-0000d2d0: 2020 2020 2020 2072 6574 7572 6e20 6174         return at
-0000d2e0: 7472 730a 0a63 6c61 7373 2049 7128 5072  trs..class Iq(Pr
-0000d2f0: 6f74 6f63 6f6c 293a 0a20 2020 2022 2222  otocol):.    """
-0000d300: 0a20 2020 2058 4d50 5020 4971 206f 626a  .    XMPP Iq obj
-0000d310: 6563 7420 2d20 6765 742f 7365 7420 6469  ect - get/set di
-0000d320: 616c 6f67 206d 6563 6861 6e69 736d 0a20  alog mechanism. 
-0000d330: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
-0000d340: 5f5f 696e 6974 5f5f 2873 656c 662c 0a20  __init__(self,. 
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 7479 703a 204f 7074 696f 6e61 6c5b 7374  typ: Optional[st
-0000d370: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000d380: 2020 2020 2020 2020 2020 2020 7175 6572              quer
-0000d390: 794e 533a 204f 7074 696f 6e61 6c5b 7374  yNS: Optional[st
-0000d3a0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000d3b0: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-0000d3c0: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
-0000d3d0: 5b73 7472 2c20 7374 725d 5d20 3d20 4e6f  [str, str]] = No
-0000d3e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000d3f0: 2020 2020 2074 6f3a 204f 7074 696f 6e61       to: Optiona
-0000d400: 6c5b 556e 696f 6e5b 4a49 442c 2073 7472  l[Union[JID, str
-0000d410: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-0000d420: 2020 2020 2020 2020 2020 2020 6672 6d3a              frm:
-0000d430: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-0000d440: 4a49 442c 2073 7472 5d5d 203d 204e 6f6e  JID, str]] = Non
-0000d450: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000d460: 2020 2020 7061 796c 6f61 643a 204f 7074      payload: Opt
-0000d470: 696f 6e61 6c5b 6c69 7374 5b55 6e69 6f6e  ional[list[Union
-0000d480: 5b4e 6f64 652c 2073 7472 5d5d 5d20 3d20  [Node, str]]] = 
-0000d490: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000d4a0: 2020 2020 2020 2078 6d6c 6e73 3a20 7374         xmlns: st
-0000d4b0: 7220 3d20 4e61 6d65 7370 6163 652e 434c  r = Namespace.CL
-0000d4c0: 4945 4e54 2c0a 2020 2020 2020 2020 2020  IENT,.          
-0000d4d0: 2020 2020 2020 206e 6f64 653a 204f 7074         node: Opt
-0000d4e0: 696f 6e61 6c5b 4e6f 6465 5d20 3d20 4e6f  ional[Node] = No
-0000d4f0: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
-0000d500: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
-0000d510: 2073 7065 6369 6679 2074 7970 652c 2071   specify type, q
-0000d520: 7565 7279 206e 616d 6573 7061 6365 2061  uery namespace a
-0000d530: 6e79 2061 6464 6974 696f 6e61 6c20 6174  ny additional at
-0000d540: 7472 6962 7574 6573 2c0a 2020 2020 2020  tributes,.      
-0000d550: 2020 7265 6369 7069 656e 7420 6f66 2074    recipient of t
-0000d560: 6865 2069 712c 2073 656e 6465 7220 6f66  he iq, sender of
-0000d570: 2074 6865 2069 712c 2061 6e79 2061 6464   the iq, any add
-0000d580: 6974 696f 6e61 6c20 7061 796c 6f61 6420  itional payload 
-0000d590: 2866 2e65 2e0a 2020 2020 2020 2020 6a61  (f.e..        ja
-0000d5a0: 6262 6572 3a78 3a64 6174 6120 6e6f 6465  bber:x:data node
-0000d5b0: 2920 616e 6420 6e61 6d65 7370 6163 6520  ) and namespace 
-0000d5c0: 696e 206f 6e65 2067 6f2e 0a0a 2020 2020  in one go...    
-0000d5d0: 2020 2020 416c 7465 726e 6174 6976 656c      Alternativel
-0000d5e0: 7920 796f 7520 6361 6e20 7061 7373 2069  y you can pass i
-0000d5f0: 6e20 7468 6520 6f74 6865 7220 584d 4c20  n the other XML 
-0000d600: 6f62 6a65 6374 2061 7320 7468 6520 276e  object as the 'n
-0000d610: 6f64 6527 0a20 2020 2020 2020 2070 6172  ode'.        par
-0000d620: 616d 6574 6564 2074 6f20 7265 706c 6963  ameted to replic
-0000d630: 6174 6520 6974 2061 7320 616e 2069 710a  ate it as an iq.
-0000d640: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d650: 2020 2020 5072 6f74 6f63 6f6c 2e5f 5f69      Protocol.__i
-0000d660: 6e69 745f 5f28 7365 6c66 2c0a 2020 2020  nit__(self,.    
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2020 2020 2020 2769 7127 2c0a 2020 2020        'iq',.    
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6a0: 2020 2020 2020 746f 3d74 6f2c 0a20 2020        to=to,.   
-0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 2020 2020 2074 7970 3d74 7970 2c0a         typ=typ,.
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2020 2020 2020 2020 2020 6174 7472 733d            attrs=
-0000d6f0: 6174 7472 732c 0a20 2020 2020 2020 2020  attrs,.         
-0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2066 726d 3d66 726d 2c0a 2020 2020 2020   frm=frm,.      
+0000c620: 2020 2020 2770 7265 7365 6e63 6527 2c0a      'presence',.
+0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c640: 2020 2020 2020 2020 2020 746f 3d74 6f2c            to=to,
+0000c650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c660: 2020 2020 2020 2020 2020 2074 7970 3d74             typ=t
+0000c670: 7970 2c0a 2020 2020 2020 2020 2020 2020  yp,.            
+0000c680: 2020 2020 2020 2020 2020 2020 2020 6174                at
+0000c690: 7472 733d 6174 7472 732c 0a20 2020 2020  trs=attrs,.     
+0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6b0: 2020 2020 2066 726d 3d66 726d 2c0a 2020       frm=frm,.  
+0000c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6d0: 2020 2020 2020 2020 7061 796c 6f61 643d          payload=
+0000c6e0: 7061 796c 6f61 642c 0a20 2020 2020 2020  payload,.       
+0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c700: 2020 2074 696d 6573 7461 6d70 3d74 696d     timestamp=tim
+0000c710: 6573 7461 6d70 2c0a 2020 2020 2020 2020  estamp,.        
+0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c730: 2020 786d 6c6e 733d 786d 6c6e 732c 0a20    xmlns=xmlns,. 
+0000c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c750: 2020 2020 2020 2020 206e 6f64 653d 6e6f           node=no
+0000c760: 6465 290a 2020 2020 2020 2020 6966 2070  de).        if p
+0000c770: 7269 6f72 6974 793a 0a20 2020 2020 2020  riority:.       
+0000c780: 2020 2020 2073 656c 662e 7365 7450 7269       self.setPri
+0000c790: 6f72 6974 7928 7072 696f 7269 7479 290a  ority(priority).
+0000c7a0: 2020 2020 2020 2020 6966 2073 686f 773a          if show:
+0000c7b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c7c0: 662e 7365 7453 686f 7728 7368 6f77 290a  f.setShow(show).
+0000c7d0: 2020 2020 2020 2020 6966 2073 7461 7475          if statu
+0000c7e0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+0000c7f0: 656c 662e 7365 7453 7461 7475 7328 7374  elf.setStatus(st
+0000c800: 6174 7573 290a 0a20 2020 2064 6566 2067  atus)..    def g
+0000c810: 6574 5072 696f 7269 7479 2873 656c 6629  etPriority(self)
+0000c820: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c830: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+0000c840: 2070 7269 6f72 6974 7920 6f66 2074 6865   priority of the
+0000c850: 206d 6573 7361 6765 0a20 2020 2020 2020   message.       
+0000c860: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+0000c870: 7572 6e20 7365 6c66 2e67 6574 5461 6744  urn self.getTagD
+0000c880: 6174 6128 2770 7269 6f72 6974 7927 290a  ata('priority').
+0000c890: 0a20 2020 2064 6566 2067 6574 5368 6f77  .    def getShow
+0000c8a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000c8b0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000c8c0: 726e 2074 6865 2073 686f 7720 7661 6c75  rn the show valu
+0000c8d0: 6520 6f66 2074 6865 206d 6573 7361 6765  e of the message
+0000c8e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c8f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000c900: 2e67 6574 5461 6744 6174 6128 2773 686f  .getTagData('sho
+0000c910: 7727 290a 0a20 2020 2064 6566 2067 6574  w')..    def get
+0000c920: 5374 6174 7573 2873 656c 6629 3a0a 2020  Status(self):.  
+0000c930: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c940: 2020 5265 7475 726e 2074 6865 2073 7461    Return the sta
+0000c950: 7475 7320 7374 7269 6e67 206f 6620 7468  tus string of th
+0000c960: 6520 6d65 7373 6167 650a 2020 2020 2020  e message.      
+0000c970: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000c980: 7475 726e 2073 656c 662e 6765 7454 6167  turn self.getTag
+0000c990: 4461 7461 2827 7374 6174 7573 2729 206f  Data('status') o
+0000c9a0: 7220 2727 0a0a 2020 2020 6465 6620 7365  r ''..    def se
+0000c9b0: 7450 7269 6f72 6974 7928 7365 6c66 2c20  tPriority(self, 
+0000c9c0: 7661 6c29 3a0a 2020 2020 2020 2020 2222  val):.        ""
+0000c9d0: 220a 2020 2020 2020 2020 5365 7420 7468  ".        Set th
+0000c9e0: 6520 7072 696f 7269 7479 206f 6620 7468  e priority of th
+0000c9f0: 6520 6d65 7373 6167 650a 2020 2020 2020  e message.      
+0000ca00: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+0000ca10: 6c66 2e73 6574 5461 6744 6174 6128 2770  lf.setTagData('p
+0000ca20: 7269 6f72 6974 7927 2c20 7661 6c29 0a0a  riority', val)..
+0000ca30: 2020 2020 6465 6620 7365 7453 686f 7728      def setShow(
+0000ca40: 7365 6c66 2c20 7661 6c29 3a0a 2020 2020  self, val):.    
+0000ca50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ca60: 5365 7420 7468 6520 7368 6f77 2076 616c  Set the show val
+0000ca70: 7565 206f 6620 7468 6520 6d65 7373 6167  ue of the messag
+0000ca80: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+0000ca90: 2020 2020 2020 6966 2076 616c 206e 6f74        if val not
+0000caa0: 2069 6e20 5b27 6177 6179 272c 2027 6368   in ['away', 'ch
+0000cab0: 6174 272c 2027 646e 6427 2c20 2778 6127  at', 'dnd', 'xa'
+0000cac0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
+0000cad0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000cae0: 2749 6e76 616c 6964 2073 686f 7720 7661  'Invalid show va
+0000caf0: 6c75 653a 2025 7327 2025 2076 616c 290a  lue: %s' % val).
+0000cb00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000cb10: 5461 6744 6174 6128 2773 686f 7727 2c20  TagData('show', 
+0000cb20: 7661 6c29 0a0a 2020 2020 6465 6620 7365  val)..    def se
+0000cb30: 7453 7461 7475 7328 7365 6c66 2c20 7661  tStatus(self, va
+0000cb40: 6c29 3a0a 2020 2020 2020 2020 2222 220a  l):.        """.
+0000cb50: 2020 2020 2020 2020 5365 7420 7468 6520          Set the 
+0000cb60: 7374 6174 7573 2073 7472 696e 6720 6f66  status string of
+0000cb70: 2074 6865 206d 6573 7361 6765 0a20 2020   the message.   
+0000cb80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cb90: 2073 656c 662e 7365 7454 6167 4461 7461   self.setTagData
+0000cba0: 2827 7374 6174 7573 272c 2076 616c 290a  ('status', val).
+0000cbb0: 0a20 2020 2064 6566 205f 6d75 635f 6765  .    def _muc_ge
+0000cbc0: 7449 7465 6d41 7474 7228 7365 6c66 2c20  tItemAttr(self, 
+0000cbd0: 7461 672c 2061 7474 7229 3a0a 2020 2020  tag, attr):.    
+0000cbe0: 2020 2020 666f 7220 7874 6167 2069 6e20      for xtag in 
+0000cbf0: 7365 6c66 2e67 6574 5461 6773 2827 7827  self.getTags('x'
+0000cc00: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000cc10: 6620 7874 6167 2e67 6574 4e61 6d65 7370  f xtag.getNamesp
+0000cc20: 6163 6528 2920 6e6f 7420 696e 2028 4e61  ace() not in (Na
+0000cc30: 6d65 7370 6163 652e 4d55 435f 5553 4552  mespace.MUC_USER
+0000cc40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 2020 2020 2020 2020 2020 2020 204e 616d               Nam
+0000cc70: 6573 7061 6365 2e4d 5543 5f41 444d 494e  espace.MUC_ADMIN
+0000cc80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000cc90: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0000cca0: 2020 2020 2020 2020 666f 7220 6368 696c          for chil
+0000ccb0: 6420 696e 2078 7461 672e 6765 7454 6167  d in xtag.getTag
+0000ccc0: 7328 7461 6729 3a0a 2020 2020 2020 2020  s(tag):.        
+0000ccd0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000cce0: 6869 6c64 2e67 6574 4174 7472 2861 7474  hild.getAttr(att
+0000ccf0: 7229 0a0a 2020 2020 6465 6620 5f6d 7563  r)..    def _muc
+0000cd00: 5f67 6574 5375 6254 6167 4461 7461 4174  _getSubTagDataAt
+0000cd10: 7472 2873 656c 662c 2074 6167 2c20 6174  tr(self, tag, at
+0000cd20: 7472 293a 0a20 2020 2020 2020 2066 6f72  tr):.        for
+0000cd30: 2078 7461 6720 696e 2073 656c 662e 6765   xtag in self.ge
+0000cd40: 7454 6167 7328 2778 2729 3a0a 2020 2020  tTags('x'):.    
+0000cd50: 2020 2020 2020 2020 6966 2078 7461 672e          if xtag.
+0000cd60: 6765 744e 616d 6573 7061 6365 2829 206e  getNamespace() n
+0000cd70: 6f74 2069 6e20 284e 616d 6573 7061 6365  ot in (Namespace
+0000cd80: 2e4d 5543 5f55 5345 522c 0a20 2020 2020  .MUC_USER,.     
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 2020 2020 4e61 6d65 7370 6163 652e        Namespace.
+0000cdc0: 4d55 435f 4144 4d49 4e29 3a0a 2020 2020  MUC_ADMIN):.    
+0000cdd0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000cde0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000cdf0: 2066 6f72 2063 6869 6c64 2069 6e20 7874   for child in xt
+0000ce00: 6167 2e67 6574 5461 6773 2827 6974 656d  ag.getTags('item
+0000ce10: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000ce20: 2020 2020 666f 7220 6363 6869 6c64 2069      for cchild i
+0000ce30: 6e20 6368 696c 642e 6765 7454 6167 7328  n child.getTags(
+0000ce40: 7461 6729 3a0a 2020 2020 2020 2020 2020  tag):.          
+0000ce50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ce60: 2063 6368 696c 642e 6765 7444 6174 6128   cchild.getData(
+0000ce70: 292c 2063 6368 696c 642e 6765 7441 7474  ), cchild.getAtt
+0000ce80: 7228 6174 7472 290a 2020 2020 2020 2020  r(attr).        
+0000ce90: 7265 7475 726e 204e 6f6e 652c 204e 6f6e  return None, Non
+0000cea0: 650a 0a20 2020 2064 6566 2067 6574 526f  e..    def getRo
+0000ceb0: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+0000cec0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000ced0: 7475 726e 2074 6865 2070 7265 7365 6e63  turn the presenc
+0000cee0: 6520 726f 6c65 2028 666f 7220 6772 6f75  e role (for grou
+0000cef0: 7063 6861 7429 0a20 2020 2020 2020 2022  pchat).        "
+0000cf00: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000cf10: 6e20 7365 6c66 2e5f 6d75 635f 6765 7449  n self._muc_getI
+0000cf20: 7465 6d41 7474 7228 2769 7465 6d27 2c20  temAttr('item', 
+0000cf30: 2772 6f6c 6527 290a 0a20 2020 2064 6566  'role')..    def
+0000cf40: 2067 6574 4166 6669 6c69 6174 696f 6e28   getAffiliation(
+0000cf50: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000cf60: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+0000cf70: 6e20 7468 6520 7072 6573 656e 6365 2061  n the presence a
+0000cf80: 6666 696c 6961 7469 6f6e 2028 666f 7220  ffiliation (for 
+0000cf90: 6772 6f75 7063 6861 7429 0a20 2020 2020  groupchat).     
+0000cfa0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000cfb0: 6574 7572 6e20 7365 6c66 2e5f 6d75 635f  eturn self._muc_
+0000cfc0: 6765 7449 7465 6d41 7474 7228 2769 7465  getItemAttr('ite
+0000cfd0: 6d27 2c20 2761 6666 696c 6961 7469 6f6e  m', 'affiliation
+0000cfe0: 2729 0a0a 2020 2020 6465 6620 6765 744e  ')..    def getN
+0000cff0: 6577 4e69 636b 2873 656c 6629 3a0a 2020  ewNick(self):.  
+0000d000: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d010: 2020 5265 7475 726e 2074 6865 2073 7461    Return the sta
+0000d020: 7475 7320 636f 6465 206f 6620 7468 6520  tus code of the 
+0000d030: 7072 6573 656e 6365 2028 666f 7220 6772  presence (for gr
+0000d040: 6f75 7063 6861 7429 0a20 2020 2020 2020  oupchat).       
+0000d050: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+0000d060: 7572 6e20 7365 6c66 2e5f 6d75 635f 6765  urn self._muc_ge
+0000d070: 7449 7465 6d41 7474 7228 2769 7465 6d27  tItemAttr('item'
+0000d080: 2c20 276e 6963 6b27 290a 0a20 2020 2064  , 'nick')..    d
+0000d090: 6566 2067 6574 4a69 6428 7365 6c66 293a  ef getJid(self):
+0000d0a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d0b0: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
+0000d0c0: 7072 6573 656e 6365 206a 6964 2028 666f  presence jid (fo
+0000d0d0: 7220 6772 6f75 7063 6861 7429 0a20 2020  r groupchat).   
+0000d0e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d0f0: 2072 6574 7572 6e20 7365 6c66 2e5f 6d75   return self._mu
+0000d100: 635f 6765 7449 7465 6d41 7474 7228 2769  c_getItemAttr('i
+0000d110: 7465 6d27 2c20 276a 6964 2729 0a0a 2020  tem', 'jid')..  
+0000d120: 2020 6465 6620 6765 7452 6561 736f 6e28    def getReason(
+0000d130: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d140: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+0000d150: 6e73 2074 6865 2072 6561 736f 6e20 6f66  ns the reason of
+0000d160: 2074 6865 2070 7265 7365 6e63 6520 2866   the presence (f
+0000d170: 6f72 2067 726f 7570 6368 6174 290a 2020  or groupchat).  
+0000d180: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d190: 2020 7265 7475 726e 2073 656c 662e 5f6d    return self._m
+0000d1a0: 7563 5f67 6574 5375 6254 6167 4461 7461  uc_getSubTagData
+0000d1b0: 4174 7472 2827 7265 6173 6f6e 272c 2027  Attr('reason', '
+0000d1c0: 2729 5b30 5d0a 0a20 2020 2064 6566 2067  ')[0]..    def g
+0000d1d0: 6574 4163 746f 7228 7365 6c66 293a 0a20  etActor(self):. 
+0000d1e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d1f0: 2020 2052 6574 7572 6e20 7468 6520 7265     Return the re
+0000d200: 6173 6f6e 206f 6620 7468 6520 7072 6573  ason of the pres
+0000d210: 656e 6365 2028 666f 7220 6772 6f75 7063  ence (for groupc
+0000d220: 6861 7429 0a20 2020 2020 2020 2022 2222  hat).        """
+0000d230: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d240: 7365 6c66 2e5f 6d75 635f 6765 7453 7562  self._muc_getSub
+0000d250: 5461 6744 6174 6141 7474 7228 2761 6374  TagDataAttr('act
+0000d260: 6f72 272c 2027 6a69 6427 295b 315d 0a0a  or', 'jid')[1]..
+0000d270: 2020 2020 6465 6620 6765 7453 7461 7475      def getStatu
+0000d280: 7343 6f64 6528 7365 6c66 293a 0a20 2020  sCode(self):.   
+0000d290: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d2a0: 2052 6574 7572 6e20 7468 6520 7374 6174   Return the stat
+0000d2b0: 7573 2063 6f64 6520 6f66 2074 6865 2070  us code of the p
+0000d2c0: 7265 7365 6e63 6520 2866 6f72 2067 726f  resence (for gro
+0000d2d0: 7570 6368 6174 290a 2020 2020 2020 2020  upchat).        
+0000d2e0: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+0000d2f0: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
+0000d300: 6f72 2078 7461 6720 696e 2073 656c 662e  or xtag in self.
+0000d310: 6765 7454 6167 7328 2778 2729 3a0a 2020  getTags('x'):.  
+0000d320: 2020 2020 2020 2020 2020 666f 7220 6368            for ch
+0000d330: 696c 6420 696e 2078 7461 672e 6765 7454  ild in xtag.getT
+0000d340: 6167 7328 2773 7461 7475 7327 293a 0a20  ags('status'):. 
+0000d350: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000d360: 7474 7273 2e61 7070 656e 6428 6368 696c  ttrs.append(chil
+0000d370: 642e 6765 7441 7474 7228 2763 6f64 6527  d.getAttr('code'
+0000d380: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+0000d390: 6e20 6174 7472 730a 0a63 6c61 7373 2049  n attrs..class I
+0000d3a0: 7128 5072 6f74 6f63 6f6c 293a 0a20 2020  q(Protocol):.   
+0000d3b0: 2022 2222 0a20 2020 2058 4d50 5020 4971   """.    XMPP Iq
+0000d3c0: 206f 626a 6563 7420 2d20 6765 742f 7365   object - get/se
+0000d3d0: 7420 6469 616c 6f67 206d 6563 6861 6e69  t dialog mechani
+0000d3e0: 736d 0a20 2020 2022 2222 0a0a 2020 2020  sm.    """..    
+0000d3f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000d400: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000d410: 2020 2020 7479 703a 204f 7074 696f 6e61      typ: Optiona
+0000d420: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d440: 7175 6572 794e 533a 204f 7074 696f 6e61  queryNS: Optiona
+0000d450: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 6174 7472 733a 204f 7074 696f 6e61 6c5b  attrs: Optional[
+0000d480: 6469 6374 5b73 7472 2c20 7374 725d 5d20  dict[str, str]] 
+0000d490: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000d4a0: 2020 2020 2020 2020 2074 6f3a 204f 7074           to: Opt
+0000d4b0: 696f 6e61 6c5b 556e 696f 6e5b 4a49 442c  ional[Union[JID,
+0000d4c0: 2073 7472 5d5d 203d 204e 6f6e 652c 0a20   str]] = None,. 
+0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4e0: 6672 6d3a 204f 7074 696f 6e61 6c5b 556e  frm: Optional[Un
+0000d4f0: 696f 6e5b 4a49 442c 2073 7472 5d5d 203d  ion[JID, str]] =
+0000d500: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000d510: 2020 2020 2020 2020 7061 796c 6f61 643a          payload:
+0000d520: 204f 7074 696f 6e61 6c5b 6c69 7374 5b55   Optional[list[U
+0000d530: 6e69 6f6e 5b4e 6f64 652c 2073 7472 5d5d  nion[Node, str]]
+0000d540: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000d550: 2020 2020 2020 2020 2020 2078 6d6c 6e73             xmlns
+0000d560: 3a20 7374 7220 3d20 4e61 6d65 7370 6163  : str = Namespac
+0000d570: 652e 434c 4945 4e54 2c0a 2020 2020 2020  e.CLIENT,.      
+0000d580: 2020 2020 2020 2020 2020 206e 6f64 653a             node:
+0000d590: 204f 7074 696f 6e61 6c5b 4e6f 6465 5d20   Optional[Node] 
+0000d5a0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0000d5b0: 2022 2222 0a20 2020 2020 2020 2059 6f75   """.        You
+0000d5c0: 2063 616e 2073 7065 6369 6679 2074 7970   can specify typ
+0000d5d0: 652c 2071 7565 7279 206e 616d 6573 7061  e, query namespa
+0000d5e0: 6365 2061 6e79 2061 6464 6974 696f 6e61  ce any additiona
+0000d5f0: 6c20 6174 7472 6962 7574 6573 2c0a 2020  l attributes,.  
+0000d600: 2020 2020 2020 7265 6369 7069 656e 7420        recipient 
+0000d610: 6f66 2074 6865 2069 712c 2073 656e 6465  of the iq, sende
+0000d620: 7220 6f66 2074 6865 2069 712c 2061 6e79  r of the iq, any
+0000d630: 2061 6464 6974 696f 6e61 6c20 7061 796c   additional payl
+0000d640: 6f61 6420 2866 2e65 2e0a 2020 2020 2020  oad (f.e..      
+0000d650: 2020 6a61 6262 6572 3a78 3a64 6174 6120    jabber:x:data 
+0000d660: 6e6f 6465 2920 616e 6420 6e61 6d65 7370  node) and namesp
+0000d670: 6163 6520 696e 206f 6e65 2067 6f2e 0a0a  ace in one go...
+0000d680: 2020 2020 2020 2020 416c 7465 726e 6174          Alternat
+0000d690: 6976 656c 7920 796f 7520 6361 6e20 7061  ively you can pa
+0000d6a0: 7373 2069 6e20 7468 6520 6f74 6865 7220  ss in the other 
+0000d6b0: 584d 4c20 6f62 6a65 6374 2061 7320 7468  XML object as th
+0000d6c0: 6520 276e 6f64 6527 0a20 2020 2020 2020  e 'node'.       
+0000d6d0: 2070 6172 616d 6574 6564 2074 6f20 7265   parameted to re
+0000d6e0: 706c 6963 6174 6520 6974 2061 7320 616e  plicate it as an
+0000d6f0: 2069 710a 2020 2020 2020 2020 2222 220a   iq.        """.
+0000d700: 2020 2020 2020 2020 5072 6f74 6f63 6f6c          Protocol
+0000d710: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c0a  .__init__(self,.
 0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 2020 2020 786d 6c6e 733d 786d 6c6e 732c      xmlns=xmlns,
-0000d740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d750: 2020 2020 2020 2020 2020 206e 6f64 653d             node=
-0000d760: 6e6f 6465 290a 2020 2020 2020 2020 6966  node).        if
-0000d770: 2070 6179 6c6f 6164 3a0a 2020 2020 2020   payload:.      
-0000d780: 2020 2020 2020 7365 6c66 2e73 6574 5175        self.setQu
-0000d790: 6572 7950 6179 6c6f 6164 2870 6179 6c6f  eryPayload(paylo
-0000d7a0: 6164 290a 2020 2020 2020 2020 6966 2071  ad).        if q
-0000d7b0: 7565 7279 4e53 3a0a 2020 2020 2020 2020  ueryNS:.        
-0000d7c0: 2020 2020 7365 6c66 2e73 6574 5175 6572      self.setQuer
-0000d7d0: 794e 5328 7175 6572 794e 5329 0a0a 2020  yNS(queryNS)..  
-0000d7e0: 2020 6465 6620 6765 7451 7565 7279 2873    def getQuery(s
-0000d7f0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-0000d800: 5b4e 6f64 655d 3a0a 2020 2020 2020 2020  [Node]:.        
-0000d810: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-0000d820: 726e 2074 6865 2049 5127 7320 6368 696c  rn the IQ's chil
-0000d830: 6420 656c 656d 656e 7420 6966 2069 7420  d element if it 
-0000d840: 6578 6973 7473 2c20 4e6f 6e65 206f 7468  exists, None oth
-0000d850: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-0000d860: 2222 220a 2020 2020 2020 2020 6368 696c  """.        chil
-0000d870: 6472 656e 203d 2073 656c 662e 6765 7443  dren = self.getC
-0000d880: 6869 6c64 7265 6e28 290a 2020 2020 2020  hildren().      
-0000d890: 2020 6966 2063 6869 6c64 7265 6e20 616e    if children an
-0000d8a0: 6420 7365 6c66 2e67 6574 5479 7065 2829  d self.getType()
-0000d8b0: 2021 3d20 2765 7272 6f72 2720 616e 6420   != 'error' and 
-0000d8c0: 5c0a 2020 2020 2020 2020 6368 696c 6472  \.        childr
-0000d8d0: 656e 5b30 5d2e 6765 744e 616d 6528 2920  en[0].getName() 
-0000d8e0: 213d 2027 6572 726f 7227 3a0a 2020 2020  != 'error':.    
-0000d8f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0000d900: 6869 6c64 7265 6e5b 305d 0a20 2020 2020  hildren[0].     
-0000d910: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-0000d920: 2020 2020 6465 6620 6765 7451 7565 7279      def getQuery
-0000d930: 4e53 2873 656c 6629 202d 3e20 4f70 7469  NS(self) -> Opti
-0000d940: 6f6e 616c 5b73 7472 5d3a 0a20 2020 2020  onal[str]:.     
-0000d950: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000d960: 6574 7572 6e20 7468 6520 6e61 6d65 7370  eturn the namesp
-0000d970: 6163 6520 6f66 2074 6865 2027 7175 6572  ace of the 'quer
-0000d980: 7927 2063 6869 6c64 2065 6c65 6d65 6e74  y' child element
-0000d990: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d9a0: 2020 2020 2074 6167 203d 2073 656c 662e       tag = self.
-0000d9b0: 6765 7451 7565 7279 2829 0a20 2020 2020  getQuery().     
-0000d9c0: 2020 2069 6620 7461 673a 0a20 2020 2020     if tag:.     
-0000d9d0: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
-0000d9e0: 672e 6765 744e 616d 6573 7061 6365 2829  g.getNamespace()
-0000d9f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000da00: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
-0000da10: 7451 7565 7279 6e6f 6465 2873 656c 6629  tQuerynode(self)
-0000da20: 202d 3e20 4f70 7469 6f6e 616c 5b73 7472   -> Optional[str
-0000da30: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-0000da40: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-0000da50: 6520 276e 6f64 6527 2061 7474 7269 6275  e 'node' attribu
-0000da60: 7465 2076 616c 7565 206f 6620 7468 6520  te value of the 
-0000da70: 2771 7565 7279 2720 6368 696c 6420 656c  'query' child el
-0000da80: 656d 656e 740a 2020 2020 2020 2020 2222  ement.        ""
-0000da90: 220a 2020 2020 2020 2020 7461 6720 3d20  ".        tag = 
-0000daa0: 7365 6c66 2e67 6574 5175 6572 7928 290a  self.getQuery().
-0000dab0: 2020 2020 2020 2020 6966 2074 6167 3a0a          if tag:.
-0000dac0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dad0: 726e 2074 6167 2e67 6574 4174 7472 2827  rn tag.getAttr('
-0000dae0: 6e6f 6465 2729 0a20 2020 2020 2020 2072  node').        r
-0000daf0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-0000db00: 6465 6620 6765 7451 7565 7279 4368 696c  def getQueryChil
-0000db10: 6472 656e 2873 656c 6629 202d 3e20 4f70  dren(self) -> Op
-0000db20: 7469 6f6e 616c 5b6c 6973 745b 4e6f 6465  tional[list[Node
-0000db30: 5d5d 3a0a 2020 2020 2020 2020 2222 220a  ]]:.        """.
-0000db40: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-0000db50: 6865 2027 7175 6572 7927 2063 6869 6c64  he 'query' child
-0000db60: 2065 6c65 6d65 6e74 2063 6869 6c64 206e   element child n
-0000db70: 6f64 6573 0a20 2020 2020 2020 2022 2222  odes.        """
-0000db80: 0a20 2020 2020 2020 2074 6167 203d 2073  .        tag = s
-0000db90: 656c 662e 6765 7451 7565 7279 2829 0a20  elf.getQuery(). 
-0000dba0: 2020 2020 2020 2069 6620 7461 673a 0a20         if tag:. 
-0000dbb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000dbc0: 6e20 7461 672e 6765 7443 6869 6c64 7265  n tag.getChildre
-0000dbd0: 6e28 290a 2020 2020 2020 2020 7265 7475  n().        retu
-0000dbe0: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
-0000dbf0: 2067 6574 5175 6572 7943 6869 6c64 2873   getQueryChild(s
-0000dc00: 656c 662c 206e 616d 653a 204f 7074 696f  elf, name: Optio
-0000dc10: 6e61 6c5b 7374 725d 203d 204e 6f6e 6529  nal[str] = None)
-0000dc20: 202d 3e20 4f70 7469 6f6e 616c 5b4e 6f64   -> Optional[Nod
-0000dc30: 655d 3a0a 2020 2020 2020 2020 2222 220a  e]:.        """.
-0000dc40: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-0000dc50: 6865 2027 7175 6572 7927 2063 6869 6c64  he 'query' child
-0000dc60: 2065 6c65 6d65 6e74 2077 6974 6820 6e61   element with na
-0000dc70: 6d65 2c20 6f72 2074 6865 2066 6972 7374  me, or the first
-0000dc80: 2065 6c65 6d65 6e74 0a20 2020 2020 2020   element.       
-0000dc90: 2077 6869 6368 2069 7320 6e6f 7420 616e   which is not an
-0000dca0: 2065 7272 6f72 2065 6c65 6d65 6e74 0a20   error element. 
-0000dcb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000dcc0: 2020 2071 7565 7279 203d 2073 656c 662e     query = self.
-0000dcd0: 6765 7451 7565 7279 2829 0a20 2020 2020  getQuery().     
-0000dce0: 2020 2069 6620 6e6f 7420 7175 6572 793a     if not query:
-0000dcf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000dd00: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-0000dd10: 2066 6f72 206e 6f64 6520 696e 2071 7565   for node in que
-0000dd20: 7279 2e67 6574 4368 696c 6472 656e 2829  ry.getChildren()
-0000dd30: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000dd40: 206e 616d 6520 6973 206e 6f74 204e 6f6e   name is not Non
-0000dd50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000dd60: 2020 2069 6620 6e6f 6465 2e67 6574 4e61     if node.getNa
-0000dd70: 6d65 2829 203d 3d20 6e61 6d65 3a0a 2020  me() == name:.  
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 7265 7475 726e 206e 6f64 650a 2020    return node.  
-0000dda0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddc0: 6966 206e 6f64 652e 6765 744e 616d 6528  if node.getName(
-0000ddd0: 2920 213d 2027 6572 726f 7227 3a0a 2020  ) != 'error':.  
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddf0: 2020 7265 7475 726e 206e 6f64 650a 2020    return node.  
-0000de00: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000de10: 650a 0a20 2020 2064 6566 2073 6574 5175  e..    def setQu
-0000de20: 6572 7928 7365 6c66 2c20 6e61 6d65 3a20  ery(self, name: 
-0000de30: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000de40: 4e6f 6e65 2920 2d3e 204e 6f64 653a 0a20  None) -> Node:. 
-0000de50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000de60: 2020 2043 6861 6e67 6520 7468 6520 6e61     Change the na
-0000de70: 6d65 206f 6620 7468 6520 7175 6572 7920  me of the query 
-0000de80: 6e6f 6465 2c20 6372 6561 7469 6e67 2069  node, creating i
-0000de90: 7420 6966 206e 6565 6465 642e 204b 6565  t if needed. Kee
-0000dea0: 7020 7468 650a 2020 2020 2020 2020 6578  p the.        ex
-0000deb0: 6973 7469 6e67 206e 616d 6520 6966 206e  isting name if n
-0000dec0: 6f6e 6520 6973 2067 6976 656e 2028 7573  one is given (us
-0000ded0: 6520 2771 7565 7279 2720 6966 2069 7427  e 'query' if it'
-0000dee0: 7320 6120 6372 6561 7469 6f6e 292e 0a20  s a creation).. 
-0000def0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-0000df00: 6520 7175 6572 7920 6e6f 6465 2e0a 2020  e query node..  
-0000df10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000df20: 2020 7175 6572 7920 3d20 7365 6c66 2e67    query = self.g
-0000df30: 6574 5175 6572 7928 290a 2020 2020 2020  etQuery().      
-0000df40: 2020 6966 2071 7565 7279 2069 7320 4e6f    if query is No
-0000df50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000df60: 7175 6572 7920 3d20 7365 6c66 2e61 6464  query = self.add
-0000df70: 4368 696c 6428 2771 7565 7279 2729 0a20  Child('query'). 
-0000df80: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
-0000df90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000dfa0: 2020 2020 2020 2020 7175 6572 792e 7365          query.se
-0000dfb0: 744e 616d 6528 6e61 6d65 290a 2020 2020  tName(name).    
-0000dfc0: 2020 2020 7265 7475 726e 2071 7565 7279      return query
-0000dfd0: 0a0a 2020 2020 6465 6620 7365 7451 7565  ..    def setQue
-0000dfe0: 7279 4e53 2873 656c 662c 206e 616d 6573  ryNS(self, names
-0000dff0: 7061 6365 3a20 7374 7229 202d 3e20 4e6f  pace: str) -> No
-0000e000: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-0000e010: 2020 2020 2020 2020 5365 7420 7468 6520          Set the 
-0000e020: 6e61 6d65 7370 6163 6520 6f66 2074 6865  namespace of the
-0000e030: 2027 7175 6572 7927 2063 6869 6c64 2065   'query' child e
-0000e040: 6c65 6d65 6e74 0a20 2020 2020 2020 2022  lement.        "
-0000e050: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-0000e060: 7365 7451 7565 7279 2829 2e73 6574 4e61  setQuery().setNa
-0000e070: 6d65 7370 6163 6528 6e61 6d65 7370 6163  mespace(namespac
-0000e080: 6529 0a0a 2020 2020 6465 6620 7365 7451  e)..    def setQ
-0000e090: 7565 7279 5061 796c 6f61 6428 7365 6c66  ueryPayload(self
-0000e0a0: 2c20 7061 796c 6f61 643a 206c 6973 745b  , payload: list[
-0000e0b0: 556e 696f 6e5b 4e6f 6465 2c20 7374 725d  Union[Node, str]
-0000e0c0: 5d29 3a0a 2020 2020 2020 2020 2222 220a  ]):.        """.
-0000e0d0: 2020 2020 2020 2020 5365 7420 7468 6520          Set the 
-0000e0e0: 2771 7565 7279 2720 6368 696c 6420 656c  'query' child el
-0000e0f0: 656d 656e 7420 7061 796c 6f61 640a 2020  ement payload.  
-0000e100: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e110: 2020 7365 6c66 2e73 6574 5175 6572 7928    self.setQuery(
-0000e120: 292e 7365 7450 6179 6c6f 6164 2870 6179  ).setPayload(pay
-0000e130: 6c6f 6164 290a 0a20 2020 2064 6566 2073  load)..    def s
-0000e140: 6574 5175 6572 796e 6f64 6528 7365 6c66  etQuerynode(self
-0000e150: 2c20 6e6f 6465 3a20 7374 7229 202d 3e20  , node: str) -> 
-0000e160: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000e170: 220a 2020 2020 2020 2020 5365 7420 7468  ".        Set th
-0000e180: 6520 276e 6f64 6527 2061 7474 7269 6275  e 'node' attribu
-0000e190: 7465 2076 616c 7565 206f 6620 7468 6520  te value of the 
-0000e1a0: 2771 7565 7279 2720 6368 696c 6420 656c  'query' child el
-0000e1b0: 656d 656e 740a 2020 2020 2020 2020 2222  ement.        ""
-0000e1c0: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
-0000e1d0: 6574 5175 6572 7928 292e 7365 7441 7474  etQuery().setAtt
-0000e1e0: 7228 276e 6f64 6527 2c20 6e6f 6465 290a  r('node', node).
-0000e1f0: 0a20 2020 2064 6566 2062 7569 6c64 5265  .    def buildRe
-0000e200: 706c 7928 7365 6c66 2c20 7479 703a 2073  ply(self, typ: s
-0000e210: 7472 2920 2d3e 2049 713a 0a20 2020 2020  tr) -> Iq:.     
-0000e220: 2020 2022 2222 0a20 2020 2020 2020 2042     """.        B
-0000e230: 7569 6c64 2061 6e64 2072 6574 7572 6e20  uild and return 
-0000e240: 616e 6f74 6865 7220 4971 206f 626a 6563  another Iq objec
-0000e250: 7420 6f66 2073 7065 6369 6669 6564 2074  t of specified t
-0000e260: 7970 652e 2054 6865 2074 6f2c 2066 726f  ype. The to, fro
-0000e270: 6d20 616e 640a 2020 2020 2020 2020 7175  m and.        qu
-0000e280: 6572 7920 6368 696c 6420 6e6f 6465 206f  ery child node o
-0000e290: 6620 6e65 7720 4971 2061 7265 2070 7265  f new Iq are pre
-0000e2a0: 2d73 6574 2061 7320 7265 706c 7920 746f  -set as reply to
-0000e2b0: 2074 6869 7320 4971 2e0a 2020 2020 2020   this Iq..      
-0000e2c0: 2020 2222 220a 2020 2020 2020 2020 6971    """.        iq
-0000e2d0: 203d 2049 7128 7479 702c 0a20 2020 2020   = Iq(typ,.     
-0000e2e0: 2020 2020 2020 2020 2020 2074 6f3d 7365             to=se
-0000e2f0: 6c66 2e67 6574 4672 6f6d 2829 2c0a 2020  lf.getFrom(),.  
-0000e300: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-0000e310: 6d3d 7365 6c66 2e67 6574 546f 2829 2c0a  m=self.getTo(),.
-0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 6174 7472 733d 7b27 6964 273a 2073 656c  attrs={'id': sel
-0000e340: 662e 6765 7449 4428 297d 290a 2020 2020  f.getID()}).    
-0000e350: 2020 2020 6971 2e73 6574 5175 6572 7928      iq.setQuery(
-0000e360: 7365 6c66 2e67 6574 5175 6572 7928 292e  self.getQuery().
-0000e370: 6765 744e 616d 6528 2929 2e73 6574 4e61  getName()).setNa
-0000e380: 6d65 7370 6163 6528 7365 6c66 2e67 6574  mespace(self.get
-0000e390: 5175 6572 794e 5328 2929 0a20 2020 2020  QueryNS()).     
-0000e3a0: 2020 2072 6574 7572 6e20 6971 0a0a 2020     return iq..  
-0000e3b0: 2020 6465 6620 6275 696c 6453 696d 706c    def buildSimpl
-0000e3c0: 6552 6570 6c79 2873 656c 662c 2074 7970  eReply(self, typ
-0000e3d0: 3a20 7374 7229 202d 3e20 4971 3a0a 2020  : str) -> Iq:.  
-0000e3e0: 2020 2020 2020 7265 7475 726e 2049 7128        return Iq(
-0000e3f0: 7479 702c 0a20 2020 2020 2020 2020 2020  typ,.           
-0000e400: 2020 2020 2020 2074 6f3d 7365 6c66 2e67         to=self.g
-0000e410: 6574 4672 6f6d 2829 2c0a 2020 2020 2020  etFrom(),.      
-0000e420: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-0000e430: 733d 7b27 6964 273a 2073 656c 662e 6765  s={'id': self.ge
-0000e440: 7449 4428 297d 290a 0a0a 636c 6173 7320  tID()})...class 
-0000e450: 4861 7368 6573 284e 6f64 6529 3a0a 2020  Hashes(Node):.  
-0000e460: 2020 2222 220a 2020 2020 4861 7368 2065    """.    Hash e
-0000e470: 6c65 6d65 6e74 7320 666f 7220 7661 7269  lements for vari
-0000e480: 6f75 7320 5845 5073 2061 7320 6465 6669  ous XEPs as defi
-0000e490: 6e65 6420 696e 2058 4550 2d33 3030 0a0a  ned in XEP-300..
-0000e4a0: 2020 2020 5245 434f 4d45 4e44 4544 2048      RECOMENDED H
-0000e4b0: 4153 4820 5553 453a 0a20 2020 2041 6c67  ASH USE:.    Alg
-0000e4c0: 6f72 6974 686d 2020 2020 2053 7570 706f  orithm     Suppo
-0000e4d0: 7274 0a20 2020 204d 4432 2020 2020 2020  rt.    MD2      
-0000e4e0: 2020 2020 204d 5553 5420 4e4f 540a 2020       MUST NOT.  
-0000e4f0: 2020 4d44 3420 2020 2020 2020 2020 2020    MD4           
-0000e500: 4d55 5354 204e 4f54 0a20 2020 204d 4435  MUST NOT.    MD5
-0000e510: 2020 2020 2020 2020 2020 204d 4159 0a20             MAY. 
-0000e520: 2020 2053 4841 2d31 2020 2020 2020 2020     SHA-1        
-0000e530: 204d 5553 540a 2020 2020 5348 412d 3235   MUST.    SHA-25
-0000e540: 3620 2020 2020 2020 4d55 5354 0a20 2020  6       MUST.   
-0000e550: 2053 4841 2d35 3132 2020 2020 2020 2053   SHA-512       S
-0000e560: 484f 554c 440a 2020 2020 2222 220a 0a20  HOULD.    """.. 
-0000e570: 2020 2073 7570 706f 7274 6564 203d 2028     supported = (
-0000e580: 276d 6435 272c 2027 7368 612d 3127 2c20  'md5', 'sha-1', 
-0000e590: 2773 6861 2d32 3536 272c 2027 7368 612d  'sha-256', 'sha-
-0000e5a0: 3531 3227 290a 0a20 2020 2064 6566 205f  512')..    def _
-0000e5b0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6e73  _init__(self, ns
-0000e5c0: 703d 4e61 6d65 7370 6163 652e 4841 5348  p=Namespace.HASH
-0000e5d0: 4553 293a 0a20 2020 2020 2020 204e 6f64  ES):.        Nod
-0000e5e0: 652e 5f5f 696e 6974 5f5f 2873 656c 662c  e.__init__(self,
-0000e5f0: 204e 6f6e 652c 207b 7d2c 205b 5d2c 204e   None, {}, [], N
-0000e600: 6f6e 652c 204e 6f6e 652c 2046 616c 7365  one, None, False
-0000e610: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-0000e620: 7365 6c66 2e73 6574 4e61 6d65 7370 6163  self.setNamespac
-0000e630: 6528 6e73 7029 0a20 2020 2020 2020 2073  e(nsp).        s
-0000e640: 656c 662e 7365 744e 616d 6528 2768 6173  elf.setName('has
-0000e650: 6827 290a 0a20 2020 2064 6566 2063 616c  h')..    def cal
-0000e660: 6375 6c61 7465 4861 7368 2873 656c 662c  culateHash(self,
-0000e670: 2061 6c67 6f2c 2066 696c 655f 7374 7269   algo, file_stri
-0000e680: 6e67 293a 0a20 2020 2020 2020 2022 2222  ng):.        """
-0000e690: 0a20 2020 2020 2020 2043 616c 6375 6c61  .        Calcula
-0000e6a0: 7465 2074 6865 2068 6173 6820 616e 6420  te the hash and 
-0000e6b0: 6164 6420 6974 2e20 4974 2069 7320 7072  add it. It is pr
-0000e6c0: 6566 6572 6162 6c65 2064 6f69 6e67 2069  eferable doing i
-0000e6d0: 7420 6865 7265 0a20 2020 2020 2020 2069  t here.        i
-0000e6e0: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
-0000e6f0: 6974 2061 6c6c 206f 7665 7220 7468 6520  it all over the 
-0000e700: 706c 6163 6520 696e 2047 616a 696d 2e0a  place in Gajim..
-0000e710: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e720: 2020 2020 686c 203d 204e 6f6e 650a 2020      hl = None.  
-0000e730: 2020 2020 2020 6861 7368 5f20 3d20 4e6f        hash_ = No
-0000e740: 6e65 0a20 2020 2020 2020 2023 2066 696c  ne.        # fil
-0000e750: 655f 7374 7269 6e67 2063 616e 2062 6520  e_string can be 
-0000e760: 6120 7374 7269 6e67 206f 7220 6120 6669  a string or a fi
-0000e770: 6c65 0a20 2020 2020 2020 2069 6620 6973  le.        if is
-0000e780: 696e 7374 616e 6365 2866 696c 655f 7374  instance(file_st
-0000e790: 7269 6e67 2c20 7374 7229 3a0a 2020 2020  ring, str):.    
-0000e7a0: 2020 2020 2020 2020 6966 2061 6c67 6f20          if algo 
-0000e7b0: 3d3d 2027 7368 612d 3127 3a0a 2020 2020  == 'sha-1':.    
-0000e7c0: 2020 2020 2020 2020 2020 2020 686c 203d              hl =
-0000e7d0: 2068 6173 686c 6962 2e73 6861 3128 290a   hashlib.sha1().
-0000e7e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000e7f0: 2061 6c67 6f20 3d3d 2027 6d64 3527 3a0a   algo == 'md5':.
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e810: 686c 203d 2068 6173 686c 6962 2e6d 6435  hl = hashlib.md5
-0000e820: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
-0000e830: 6c69 6620 616c 676f 203d 3d20 2773 6861  lif algo == 'sha
-0000e840: 2d32 3536 273a 0a20 2020 2020 2020 2020  -256':.         
-0000e850: 2020 2020 2020 2068 6c20 3d20 6861 7368         hl = hash
-0000e860: 6c69 622e 7368 6132 3536 2829 0a20 2020  lib.sha256().   
-0000e870: 2020 2020 2020 2020 2065 6c69 6620 616c           elif al
-0000e880: 676f 203d 3d20 2773 6861 2d35 3132 273a  go == 'sha-512':
-0000e890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e8a0: 2068 6c20 3d20 6861 7368 6c69 622e 7368   hl = hashlib.sh
-0000e8b0: 6135 3132 2829 0a20 2020 2020 2020 2020  a512().         
-0000e8c0: 2020 2069 6620 686c 3a0a 2020 2020 2020     if hl:.      
-0000e8d0: 2020 2020 2020 2020 2020 686c 2e75 7064            hl.upd
-0000e8e0: 6174 6528 6669 6c65 5f73 7472 696e 6729  ate(file_string)
-0000e8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e900: 2068 6173 685f 203d 2068 6c2e 6865 7864   hash_ = hl.hexd
-0000e910: 6967 6573 7428 290a 2020 2020 2020 2020  igest().        
-0000e920: 656c 7365 3a20 2320 6966 2069 7420 6973  else: # if it is
-0000e930: 2061 2066 696c 650a 2020 2020 2020 2020   a file.        
-0000e940: 2020 2020 6966 2061 6c67 6f20 3d3d 2027      if algo == '
-0000e950: 7368 612d 3127 3a0a 2020 2020 2020 2020  sha-1':.        
-0000e960: 2020 2020 2020 2020 686c 203d 2068 6173          hl = has
-0000e970: 686c 6962 2e73 6861 3128 290a 2020 2020  hlib.sha1().    
-0000e980: 2020 2020 2020 2020 656c 6966 2061 6c67          elif alg
-0000e990: 6f20 3d3d 2027 6d64 3527 3a0a 2020 2020  o == 'md5':.    
-0000e9a0: 2020 2020 2020 2020 2020 2020 686c 203d              hl =
-0000e9b0: 2068 6173 686c 6962 2e6d 6435 2829 0a20   hashlib.md5(). 
-0000e9c0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000e9d0: 616c 676f 203d 3d20 2773 6861 2d32 3536  algo == 'sha-256
-0000e9e0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-0000e9f0: 2020 2068 6c20 3d20 6861 7368 6c69 622e     hl = hashlib.
-0000ea00: 7368 6132 3536 2829 0a20 2020 2020 2020  sha256().       
-0000ea10: 2020 2020 2065 6c69 6620 616c 676f 203d       elif algo =
-0000ea20: 3d20 2773 6861 2d35 3132 273a 0a20 2020  = 'sha-512':.   
-0000ea30: 2020 2020 2020 2020 2020 2020 2068 6c20               hl 
-0000ea40: 3d20 6861 7368 6c69 622e 7368 6135 3132  = hashlib.sha512
-0000ea50: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-0000ea60: 6620 686c 3a0a 2020 2020 2020 2020 2020  f hl:.          
-0000ea70: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-0000ea80: 6e20 6669 6c65 5f73 7472 696e 673a 0a20  n file_string:. 
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 2020 2068 6c2e 7570 6461 7465 286c 696e     hl.update(lin
-0000eab0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000eac0: 2020 2068 6173 685f 203d 2068 6c2e 6865     hash_ = hl.he
-0000ead0: 7864 6967 6573 7428 290a 2020 2020 2020  xdigest().      
-0000eae0: 2020 7265 7475 726e 2068 6173 685f 0a0a    return hash_..
-0000eaf0: 2020 2020 6465 6620 6164 6448 6173 6828      def addHash(
-0000eb00: 7365 6c66 2c20 6861 7368 5f2c 2061 6c67  self, hash_, alg
-0000eb10: 6f29 3a0a 2020 2020 2020 2020 7365 6c66  o):.        self
-0000eb20: 2e73 6574 4174 7472 2827 616c 676f 272c  .setAttr('algo',
-0000eb30: 2061 6c67 6f29 0a20 2020 2020 2020 2073   algo).        s
-0000eb40: 656c 662e 7365 7444 6174 6128 6861 7368  elf.setData(hash
-0000eb50: 5f29 0a0a 636c 6173 7320 4861 7368 6573  _)..class Hashes
-0000eb60: 3228 4e6f 6465 293a 0a20 2020 2022 2222  2(Node):.    """
-0000eb70: 0a20 2020 2048 6173 6820 656c 656d 656e  .    Hash elemen
-0000eb80: 7473 2066 6f72 2076 6172 696f 7573 2058  ts for various X
-0000eb90: 4550 7320 6173 2064 6566 696e 6564 2069  EPs as defined i
-0000eba0: 6e20 5845 502d 3330 300a 0a20 2020 2052  n XEP-300..    R
-0000ebb0: 4543 4f4d 454e 4445 4420 4841 5348 2055  ECOMENDED HASH U
-0000ebc0: 5345 3a0a 2020 2020 416c 676f 7269 7468  SE:.    Algorith
-0000ebd0: 6d20 2020 2020 5375 7070 6f72 740a 2020  m     Support.  
-0000ebe0: 2020 4d44 3220 2020 2020 2020 2020 2020    MD2           
-0000ebf0: 4d55 5354 204e 4f54 0a20 2020 204d 4434  MUST NOT.    MD4
-0000ec00: 2020 2020 2020 2020 2020 204d 5553 5420             MUST 
-0000ec10: 4e4f 540a 2020 2020 4d44 3520 2020 2020  NOT.    MD5     
-0000ec20: 2020 2020 2020 4d55 5354 204e 4f54 0a20        MUST NOT. 
-0000ec30: 2020 2053 4841 2d31 2020 2020 2020 2020     SHA-1        
-0000ec40: 2053 484f 554c 4420 4e4f 540a 2020 2020   SHOULD NOT.    
-0000ec50: 5348 412d 3235 3620 2020 2020 2020 4d55  SHA-256       MU
-0000ec60: 5354 0a20 2020 2053 4841 2d35 3132 2020  ST.    SHA-512  
-0000ec70: 2020 2020 2053 484f 554c 440a 2020 2020       SHOULD.    
-0000ec80: 5348 4133 2d32 3536 2020 2020 2020 4d55  SHA3-256      MU
-0000ec90: 5354 0a20 2020 2053 4841 332d 3531 3220  ST.    SHA3-512 
-0000eca0: 2020 2020 2053 484f 554c 440a 2020 2020       SHOULD.    
-0000ecb0: 424c 414b 4532 6232 3536 2020 2020 4d55  BLAKE2b256    MU
-0000ecc0: 5354 0a20 2020 2042 4c41 4b45 3262 3531  ST.    BLAKE2b51
-0000ecd0: 3220 2020 2053 484f 554c 440a 2020 2020  2    SHOULD.    
-0000ece0: 2222 220a 0a20 2020 2073 7570 706f 7274  """..    support
-0000ecf0: 6564 203d 2028 2773 6861 2d32 3536 272c  ed = ('sha-256',
-0000ed00: 2027 7368 612d 3531 3227 2c20 2773 6861   'sha-512', 'sha
-0000ed10: 332d 3235 3627 2c0a 2020 2020 2020 2020  3-256',.        
-0000ed20: 2020 2020 2020 2020 2027 7368 6133 2d35           'sha3-5
-0000ed30: 3132 272c 2027 626c 616b 6532 622d 3235  12', 'blake2b-25
-0000ed40: 3627 2c20 2762 6c61 6b65 3262 2d35 3132  6', 'blake2b-512
-0000ed50: 2729 0a0a 2020 2020 6465 6620 5f5f 696e  ')..    def __in
-0000ed60: 6974 5f5f 2873 656c 662c 206e 7370 3d4e  it__(self, nsp=N
-0000ed70: 616d 6573 7061 6365 2e48 4153 4845 535f  amespace.HASHES_
-0000ed80: 3229 3a0a 2020 2020 2020 2020 4e6f 6465  2):.        Node
-0000ed90: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c20  .__init__(self, 
-0000eda0: 4e6f 6e65 2c20 7b7d 2c20 5b5d 2c20 4e6f  None, {}, [], No
-0000edb0: 6e65 2c20 4e6f 6e65 2c20 4661 6c73 652c  ne, None, False,
-0000edc0: 204e 6f6e 6529 0a20 2020 2020 2020 2073   None).        s
-0000edd0: 656c 662e 7365 744e 616d 6573 7061 6365  elf.setNamespace
-0000ede0: 286e 7370 290a 2020 2020 2020 2020 7365  (nsp).        se
-0000edf0: 6c66 2e73 6574 4e61 6d65 2827 6861 7368  lf.setName('hash
-0000ee00: 2729 0a0a 2020 2020 6465 6620 6361 6c63  ')..    def calc
-0000ee10: 756c 6174 6548 6173 6828 7365 6c66 2c20  ulateHash(self, 
-0000ee20: 616c 676f 2c20 6669 6c65 5f73 7472 696e  algo, file_strin
-0000ee30: 6729 3a0a 2020 2020 2020 2020 2222 220a  g):.        """.
-0000ee40: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-0000ee50: 6520 7468 6520 6861 7368 2061 6e64 2061  e the hash and a
-0000ee60: 6464 2069 742e 2049 7420 6973 2070 7265  dd it. It is pre
-0000ee70: 6665 7261 626c 6520 646f 696e 6720 6974  ferable doing it
-0000ee80: 2068 6572 650a 2020 2020 2020 2020 696e   here.        in
-0000ee90: 7374 6561 6420 6f66 2064 6f69 6e67 2069  stead of doing i
-0000eea0: 7420 616c 6c20 6f76 6572 2074 6865 2070  t all over the p
-0000eeb0: 6c61 6365 2069 6e20 4761 6a69 6d2e 0a20  lace in Gajim.. 
-0000eec0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000eed0: 2020 2068 6c20 3d20 4e6f 6e65 0a20 2020     hl = None.   
-0000eee0: 2020 2020 2068 6173 685f 203d 204e 6f6e       hash_ = Non
-0000eef0: 650a 2020 2020 2020 2020 6966 2061 6c67  e.        if alg
-0000ef00: 6f20 3d3d 2027 7368 612d 3235 3627 3a0a  o == 'sha-256':.
-0000ef10: 2020 2020 2020 2020 2020 2020 686c 203d              hl =
-0000ef20: 2068 6173 686c 6962 2e73 6861 3235 3628   hashlib.sha256(
-0000ef30: 290a 2020 2020 2020 2020 656c 6966 2061  ).        elif a
-0000ef40: 6c67 6f20 3d3d 2027 7368 612d 3531 3227  lgo == 'sha-512'
-0000ef50: 3a0a 2020 2020 2020 2020 2020 2020 686c  :.            hl
-0000ef60: 203d 2068 6173 686c 6962 2e73 6861 3531   = hashlib.sha51
-0000ef70: 3228 290a 2020 2020 2020 2020 656c 6966  2().        elif
-0000ef80: 2061 6c67 6f20 3d3d 2027 7368 6133 2d32   algo == 'sha3-2
-0000ef90: 3536 273a 0a20 2020 2020 2020 2020 2020  56':.           
-0000efa0: 2068 6c20 3d20 6861 7368 6c69 622e 7368   hl = hashlib.sh
-0000efb0: 6133 5f32 3536 2829 0a20 2020 2020 2020  a3_256().       
-0000efc0: 2065 6c69 6620 616c 676f 203d 3d20 2773   elif algo == 's
-0000efd0: 6861 332d 3531 3227 3a0a 2020 2020 2020  ha3-512':.      
-0000efe0: 2020 2020 2020 686c 203d 2068 6173 686c        hl = hashl
-0000eff0: 6962 2e73 6861 335f 3531 3228 290a 2020  ib.sha3_512().  
-0000f000: 2020 2020 2020 656c 6966 2061 6c67 6f20        elif algo 
-0000f010: 3d3d 2027 626c 616b 6532 622d 3235 3627  == 'blake2b-256'
-0000f020: 3a0a 2020 2020 2020 2020 2020 2020 686c  :.            hl
-0000f030: 203d 2068 6173 686c 6962 2e62 6c61 6b65   = hashlib.blake
-0000f040: 3262 2864 6967 6573 745f 7369 7a65 3d33  2b(digest_size=3
-0000f050: 3229 0a20 2020 2020 2020 2065 6c69 6620  2).        elif 
-0000f060: 616c 676f 203d 3d20 2762 6c61 6b65 3262  algo == 'blake2b
-0000f070: 2d35 3132 273a 0a20 2020 2020 2020 2020  -512':.         
-0000f080: 2020 2068 6c20 3d20 6861 7368 6c69 622e     hl = hashlib.
-0000f090: 626c 616b 6532 6228 6469 6765 7374 5f73  blake2b(digest_s
-0000f0a0: 697a 653d 3634 290a 2020 2020 2020 2020  ize=64).        
-0000f0b0: 2320 6669 6c65 5f73 7472 696e 6720 6361  # file_string ca
-0000f0c0: 6e20 6265 2061 2073 7472 696e 6720 6f72  n be a string or
-0000f0d0: 2061 2066 696c 650a 2020 2020 2020 2020   a file.        
-0000f0e0: 6966 2068 6c20 6973 206e 6f74 204e 6f6e  if hl is not Non
-0000f0f0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0000f100: 6620 6973 696e 7374 616e 6365 2866 696c  f isinstance(fil
-0000f110: 655f 7374 7269 6e67 2c20 6279 7465 7329  e_string, bytes)
-0000f120: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f130: 2020 686c 2e75 7064 6174 6528 6669 6c65    hl.update(file
-0000f140: 5f73 7472 696e 6729 0a20 2020 2020 2020  _string).       
-0000f150: 2020 2020 2065 6c73 653a 2023 2069 6620       else: # if 
-0000f160: 6974 2069 7320 6120 6669 6c65 0a20 2020  it is a file.   
-0000f170: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f180: 206c 696e 6520 696e 2066 696c 655f 7374   line in file_st
-0000f190: 7269 6e67 3a0a 2020 2020 2020 2020 2020  ring:.          
-0000f1a0: 2020 2020 2020 2020 2020 686c 2e75 7064            hl.upd
-0000f1b0: 6174 6528 6c69 6e65 290a 2020 2020 2020  ate(line).      
-0000f1c0: 2020 2020 2020 6861 7368 5f20 3d20 6236        hash_ = b6
-0000f1d0: 3465 6e63 6f64 6528 686c 2e64 6967 6573  4encode(hl.diges
-0000f1e0: 7428 2929 2e64 6563 6f64 6528 2761 7363  t()).decode('asc
-0000f1f0: 6969 2729 0a20 2020 2020 2020 2072 6574  ii').        ret
-0000f200: 7572 6e20 6861 7368 5f0a 0a20 2020 2064  urn hash_..    d
-0000f210: 6566 2061 6464 4861 7368 2873 656c 662c  ef addHash(self,
-0000f220: 2068 6173 685f 2c20 616c 676f 293a 0a20   hash_, algo):. 
-0000f230: 2020 2020 2020 2073 656c 662e 7365 7441         self.setA
-0000f240: 7474 7228 2761 6c67 6f27 2c20 616c 676f  ttr('algo', algo
-0000f250: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000f260: 6574 4461 7461 2868 6173 685f 290a 0a0a  etData(hash_)...
-0000f270: 636c 6173 7320 4269 6e64 5265 7175 6573  class BindReques
-0000f280: 7428 4971 293a 0a20 2020 2064 6566 205f  t(Iq):.    def _
-0000f290: 5f69 6e69 745f 5f28 7365 6c66 2c20 7265  _init__(self, re
-0000f2a0: 736f 7572 6365 3a20 4f70 7469 6f6e 616c  source: Optional
-0000f2b0: 5b73 7472 5d29 3a0a 2020 2020 2020 2020  [str]):.        
-0000f2c0: 6966 2072 6573 6f75 7263 6520 6973 204e  if resource is N
-0000f2d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000f2e0: 2072 6573 203d 2072 6573 6f75 7263 650a   res = resource.
-0000f2f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000f300: 2020 2020 2020 2020 2020 7265 7320 3d20            res = 
-0000f310: 4e6f 6465 2827 7265 736f 7572 6365 272c  Node('resource',
-0000f320: 2070 6179 6c6f 6164 3d72 6573 6f75 7263   payload=resourc
-0000f330: 6529 0a20 2020 2020 2020 2049 712e 5f5f  e).        Iq.__
-0000f340: 696e 6974 5f5f 2873 656c 662c 2074 7970  init__(self, typ
-0000f350: 3d27 7365 7427 290a 2020 2020 2020 2020  ='set').        
-0000f360: 7365 6c66 2e61 6464 4368 696c 6428 6e6f  self.addChild(no
-0000f370: 6465 3d4e 6f64 6528 2762 696e 6427 2c0a  de=Node('bind',.
-0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3a0: 7b27 786d 6c6e 7327 3a20 4e61 6d65 7370  {'xmlns': Namesp
-0000f3b0: 6163 652e 4249 4e44 7d2c 0a20 2020 2020  ace.BIND},.     
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3d0: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
-0000f3e0: 6164 3d72 6573 2929 0a0a 0a63 6c61 7373  ad=res))...class
-0000f3f0: 2054 4c53 5265 7175 6573 7428 4e6f 6465   TLSRequest(Node
-0000f400: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0000f410: 745f 5f28 7365 6c66 293a 0a20 2020 2020  t__(self):.     
-0000f420: 2020 204e 6f64 652e 5f5f 696e 6974 5f5f     Node.__init__
-0000f430: 2873 656c 662c 2074 6167 3d27 7374 6172  (self, tag='star
-0000f440: 7474 6c73 272c 2061 7474 7273 3d7b 2778  ttls', attrs={'x
-0000f450: 6d6c 6e73 273a 204e 616d 6573 7061 6365  mlns': Namespace
-0000f460: 2e54 4c53 7d29 0a0a 0a63 6c61 7373 2053  .TLS})...class S
-0000f470: 6573 7369 6f6e 5265 7175 6573 7428 4971  essionRequest(Iq
-0000f480: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0000f490: 745f 5f28 7365 6c66 293a 0a20 2020 2020  t__(self):.     
-0000f4a0: 2020 2049 712e 5f5f 696e 6974 5f5f 2873     Iq.__init__(s
-0000f4b0: 656c 662c 2074 7970 3d27 7365 7427 290a  elf, typ='set').
-0000f4c0: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-0000f4d0: 4368 696c 6428 6e6f 6465 3d4e 6f64 6528  Child(node=Node(
-0000f4e0: 2773 6573 7369 6f6e 272c 2061 7474 7273  'session', attrs
-0000f4f0: 3d7b 2778 6d6c 6e73 273a 204e 616d 6573  ={'xmlns': Names
-0000f500: 7061 6365 2e53 4553 5349 4f4e 7d29 290a  pace.SESSION})).
-0000f510: 0a0a 636c 6173 7320 5374 7265 616d 4865  ..class StreamHe
-0000f520: 6164 6572 284e 6f64 6529 3a0a 2020 2020  ader(Node):.    
-0000f530: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000f540: 662c 2064 6f6d 6169 6e3a 2073 7472 2c20  f, domain: str, 
-0000f550: 6c61 6e67 3a20 4f70 7469 6f6e 616c 5b73  lang: Optional[s
-0000f560: 7472 5d20 3d20 4e6f 6e65 293a 0a20 2020  tr] = None):.   
-0000f570: 2020 2020 2069 6620 6c61 6e67 2069 7320       if lang is 
-0000f580: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000f590: 2020 6c61 6e67 203d 2027 656e 270a 2020    lang = 'en'.  
-0000f5a0: 2020 2020 2020 4e6f 6465 2e5f 5f69 6e69        Node.__ini
-0000f5b0: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
-0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5d0: 7461 673d 2773 7472 6561 6d3a 7374 7265  tag='stream:stre
-0000f5e0: 616d 272c 0a20 2020 2020 2020 2020 2020  am',.           
-0000f5f0: 2020 2020 2020 2020 2020 2061 7474 7273             attrs
-0000f600: 3d7b 2778 6d6c 6e73 273a 204e 616d 6573  ={'xmlns': Names
-0000f610: 7061 6365 2e43 4c49 454e 542c 0a20 2020  pace.CLIENT,.   
-0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f630: 2020 2020 2020 2020 2020 2776 6572 7369            'versi
-0000f640: 6f6e 273a 2027 312e 3027 2c0a 2020 2020  on': '1.0',.    
-0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f660: 2020 2020 2020 2020 2027 786d 6c6e 733a           'xmlns:
-0000f670: 7374 7265 616d 273a 204e 616d 6573 7061  stream': Namespa
-0000f680: 6365 2e53 5452 4541 4d53 2c0a 2020 2020  ce.STREAMS,.    
-0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6a0: 2020 2020 2020 2020 2027 746f 273a 2064           'to': d
-0000f6b0: 6f6d 6169 6e2c 0a20 2020 2020 2020 2020  omain,.         
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6d0: 2020 2020 2778 6d6c 3a6c 616e 6727 3a20      'xml:lang': 
-0000f6e0: 6c61 6e67 7d29 0a0a 0a63 6c61 7373 2057  lang})...class W
-0000f6f0: 6562 736f 636b 6574 4f70 656e 4865 6164  ebsocketOpenHead
-0000f700: 6572 284e 6f64 6529 3a0a 2020 2020 6465  er(Node):.    de
-0000f710: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0000f720: 2064 6f6d 6169 6e3a 2073 7472 2c20 6c61   domain: str, la
-0000f730: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
-0000f740: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
-0000f750: 2020 2069 6620 6c61 6e67 2069 7320 4e6f     if lang is No
-0000f760: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000f770: 6c61 6e67 203d 2027 656e 270a 2020 2020  lang = 'en'.    
-0000f780: 2020 2020 4e6f 6465 2e5f 5f69 6e69 745f      Node.__init_
-0000f790: 5f28 7365 6c66 2c0a 2020 2020 2020 2020  _(self,.        
-0000f7a0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000f7b0: 673d 276f 7065 6e27 2c0a 2020 2020 2020  g='open',.      
-0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7d0: 6174 7472 733d 7b27 786d 6c6e 7327 3a20  attrs={'xmlns': 
-0000f7e0: 4e61 6d65 7370 6163 652e 4652 414d 494e  Namespace.FRAMIN
-0000f7f0: 472c 0a20 2020 2020 2020 2020 2020 2020  G,.             
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2776 6572 7369 6f6e 273a 2027 312e 3027  'version': '1.0'
-0000f820: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000f840: 746f 273a 2064 6f6d 6169 6e2c 0a20 2020  to': domain,.   
+0000d730: 2020 2020 2020 2020 2020 2769 7127 2c0a            'iq',.
+0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d750: 2020 2020 2020 2020 2020 746f 3d74 6f2c            to=to,
+0000d760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d770: 2020 2020 2020 2020 2020 2074 7970 3d74             typ=t
+0000d780: 7970 2c0a 2020 2020 2020 2020 2020 2020  yp,.            
+0000d790: 2020 2020 2020 2020 2020 2020 2020 6174                at
+0000d7a0: 7472 733d 6174 7472 732c 0a20 2020 2020  trs=attrs,.     
+0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7c0: 2020 2020 2066 726d 3d66 726d 2c0a 2020       frm=frm,.  
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 2020 2020 2020 786d 6c6e 733d 786d          xmlns=xm
+0000d7f0: 6c6e 732c 0a20 2020 2020 2020 2020 2020  lns,.           
+0000d800: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000d810: 6f64 653d 6e6f 6465 290a 2020 2020 2020  ode=node).      
+0000d820: 2020 6966 2070 6179 6c6f 6164 3a0a 2020    if payload:.  
+0000d830: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000d840: 6574 5175 6572 7950 6179 6c6f 6164 2870  etQueryPayload(p
+0000d850: 6179 6c6f 6164 290a 2020 2020 2020 2020  ayload).        
+0000d860: 6966 2071 7565 7279 4e53 3a0a 2020 2020  if queryNS:.    
+0000d870: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000d880: 5175 6572 794e 5328 7175 6572 794e 5329  QueryNS(queryNS)
+0000d890: 0a0a 2020 2020 6465 6620 6765 7451 7565  ..    def getQue
+0000d8a0: 7279 2873 656c 6629 202d 3e20 4f70 7469  ry(self) -> Opti
+0000d8b0: 6f6e 616c 5b4e 6f64 655d 3a0a 2020 2020  onal[Node]:.    
+0000d8c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d8d0: 5265 7475 726e 2074 6865 2049 5127 7320  Return the IQ's 
+0000d8e0: 6368 696c 6420 656c 656d 656e 7420 6966  child element if
+0000d8f0: 2069 7420 6578 6973 7473 2c20 4e6f 6e65   it exists, None
+0000d900: 206f 7468 6572 7769 7365 2e0a 2020 2020   otherwise..    
+0000d910: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d920: 6368 696c 6472 656e 203d 2073 656c 662e  children = self.
+0000d930: 6765 7443 6869 6c64 7265 6e28 290a 2020  getChildren().  
+0000d940: 2020 2020 2020 6966 2063 6869 6c64 7265        if childre
+0000d950: 6e20 616e 6420 7365 6c66 2e67 6574 5479  n and self.getTy
+0000d960: 7065 2829 2021 3d20 2765 7272 6f72 2720  pe() != 'error' 
+0000d970: 616e 6420 5c0a 2020 2020 2020 2020 6368  and \.        ch
+0000d980: 696c 6472 656e 5b30 5d2e 6765 744e 616d  ildren[0].getNam
+0000d990: 6528 2920 213d 2027 6572 726f 7227 3a0a  e() != 'error':.
+0000d9a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d9b0: 726e 2063 6869 6c64 7265 6e5b 305d 0a20  rn children[0]. 
+0000d9c0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000d9d0: 6e65 0a0a 2020 2020 6465 6620 6765 7451  ne..    def getQ
+0000d9e0: 7565 7279 4e53 2873 656c 6629 202d 3e20  ueryNS(self) -> 
+0000d9f0: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
+0000da00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000da10: 2020 2052 6574 7572 6e20 7468 6520 6e61     Return the na
+0000da20: 6d65 7370 6163 6520 6f66 2074 6865 2027  mespace of the '
+0000da30: 7175 6572 7927 2063 6869 6c64 2065 6c65  query' child ele
+0000da40: 6d65 6e74 0a20 2020 2020 2020 2022 2222  ment.        """
+0000da50: 0a20 2020 2020 2020 2074 6167 203d 2073  .        tag = s
+0000da60: 656c 662e 6765 7451 7565 7279 2829 0a20  elf.getQuery(). 
+0000da70: 2020 2020 2020 2069 6620 7461 673a 0a20         if tag:. 
+0000da80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000da90: 6e20 7461 672e 6765 744e 616d 6573 7061  n tag.getNamespa
+0000daa0: 6365 2829 0a20 2020 2020 2020 2072 6574  ce().        ret
+0000dab0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 6465  urn None..    de
+0000dac0: 6620 6765 7451 7565 7279 6e6f 6465 2873  f getQuerynode(s
+0000dad0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000dae0: 5b73 7472 5d3a 0a20 2020 2020 2020 2022  [str]:.        "
+0000daf0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+0000db00: 6e20 7468 6520 276e 6f64 6527 2061 7474  n the 'node' att
+0000db10: 7269 6275 7465 2076 616c 7565 206f 6620  ribute value of 
+0000db20: 7468 6520 2771 7565 7279 2720 6368 696c  the 'query' chil
+0000db30: 6420 656c 656d 656e 740a 2020 2020 2020  d element.      
+0000db40: 2020 2222 220a 2020 2020 2020 2020 7461    """.        ta
+0000db50: 6720 3d20 7365 6c66 2e67 6574 5175 6572  g = self.getQuer
+0000db60: 7928 290a 2020 2020 2020 2020 6966 2074  y().        if t
+0000db70: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+0000db80: 7265 7475 726e 2074 6167 2e67 6574 4174  return tag.getAt
+0000db90: 7472 2827 6e6f 6465 2729 0a20 2020 2020  tr('node').     
+0000dba0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+0000dbb0: 2020 2020 6465 6620 6765 7451 7565 7279      def getQuery
+0000dbc0: 4368 696c 6472 656e 2873 656c 6629 202d  Children(self) -
+0000dbd0: 3e20 4f70 7469 6f6e 616c 5b6c 6973 745b  > Optional[list[
+0000dbe0: 4e6f 6465 5d5d 3a0a 2020 2020 2020 2020  Node]]:.        
+0000dbf0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000dc00: 726e 2074 6865 2027 7175 6572 7927 2063  rn the 'query' c
+0000dc10: 6869 6c64 2065 6c65 6d65 6e74 2063 6869  hild element chi
+0000dc20: 6c64 206e 6f64 6573 0a20 2020 2020 2020  ld nodes.       
+0000dc30: 2022 2222 0a20 2020 2020 2020 2074 6167   """.        tag
+0000dc40: 203d 2073 656c 662e 6765 7451 7565 7279   = self.getQuery
+0000dc50: 2829 0a20 2020 2020 2020 2069 6620 7461  ().        if ta
+0000dc60: 673a 0a20 2020 2020 2020 2020 2020 2072  g:.            r
+0000dc70: 6574 7572 6e20 7461 672e 6765 7443 6869  eturn tag.getChi
+0000dc80: 6c64 7265 6e28 290a 2020 2020 2020 2020  ldren().        
+0000dc90: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000dca0: 2064 6566 2067 6574 5175 6572 7943 6869   def getQueryChi
+0000dcb0: 6c64 2873 656c 662c 206e 616d 653a 204f  ld(self, name: O
+0000dcc0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000dcd0: 6f6e 6529 202d 3e20 4f70 7469 6f6e 616c  one) -> Optional
+0000dce0: 5b4e 6f64 655d 3a0a 2020 2020 2020 2020  [Node]:.        
+0000dcf0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000dd00: 726e 2074 6865 2027 7175 6572 7927 2063  rn the 'query' c
+0000dd10: 6869 6c64 2065 6c65 6d65 6e74 2077 6974  hild element wit
+0000dd20: 6820 6e61 6d65 2c20 6f72 2074 6865 2066  h name, or the f
+0000dd30: 6972 7374 2065 6c65 6d65 6e74 0a20 2020  irst element.   
+0000dd40: 2020 2020 2077 6869 6368 2069 7320 6e6f       which is no
+0000dd50: 7420 616e 2065 7272 6f72 2065 6c65 6d65  t an error eleme
+0000dd60: 6e74 0a20 2020 2020 2020 2022 2222 0a20  nt.        """. 
+0000dd70: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
+0000dd80: 656c 662e 6765 7451 7565 7279 2829 0a20  elf.getQuery(). 
+0000dd90: 2020 2020 2020 2069 6620 6e6f 7420 7175         if not qu
+0000dda0: 6572 793a 0a20 2020 2020 2020 2020 2020  ery:.           
+0000ddb0: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+0000ddc0: 2020 2020 2066 6f72 206e 6f64 6520 696e       for node in
+0000ddd0: 2071 7565 7279 2e67 6574 4368 696c 6472   query.getChildr
+0000dde0: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
+0000ddf0: 2020 6966 206e 616d 6520 6973 206e 6f74    if name is not
+0000de00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000de10: 2020 2020 2020 2069 6620 6e6f 6465 2e67         if node.g
+0000de20: 6574 4e61 6d65 2829 203d 3d20 6e61 6d65  etName() == name
+0000de30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000de40: 2020 2020 2020 7265 7475 726e 206e 6f64        return nod
+0000de50: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+0000de60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000de70: 2020 2020 6966 206e 6f64 652e 6765 744e      if node.getN
+0000de80: 616d 6528 2920 213d 2027 6572 726f 7227  ame() != 'error'
+0000de90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000dea0: 2020 2020 2020 7265 7475 726e 206e 6f64        return nod
+0000deb0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000dec0: 204e 6f6e 650a 0a20 2020 2064 6566 2073   None..    def s
+0000ded0: 6574 5175 6572 7928 7365 6c66 2c20 6e61  etQuery(self, na
+0000dee0: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
+0000def0: 5d20 3d20 4e6f 6e65 2920 2d3e 204e 6f64  ] = None) -> Nod
+0000df00: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0000df10: 2020 2020 2020 2043 6861 6e67 6520 7468         Change th
+0000df20: 6520 6e61 6d65 206f 6620 7468 6520 7175  e name of the qu
+0000df30: 6572 7920 6e6f 6465 2c20 6372 6561 7469  ery node, creati
+0000df40: 6e67 2069 7420 6966 206e 6565 6465 642e  ng it if needed.
+0000df50: 204b 6565 7020 7468 650a 2020 2020 2020   Keep the.      
+0000df60: 2020 6578 6973 7469 6e67 206e 616d 6520    existing name 
+0000df70: 6966 206e 6f6e 6520 6973 2067 6976 656e  if none is given
+0000df80: 2028 7573 6520 2771 7565 7279 2720 6966   (use 'query' if
+0000df90: 2069 7427 7320 6120 6372 6561 7469 6f6e   it's a creation
+0000dfa0: 292e 0a20 2020 2020 2020 2052 6574 7572  )..        Retur
+0000dfb0: 6e20 7468 6520 7175 6572 7920 6e6f 6465  n the query node
+0000dfc0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000dfd0: 2020 2020 2020 7175 6572 7920 3d20 7365        query = se
+0000dfe0: 6c66 2e67 6574 5175 6572 7928 290a 2020  lf.getQuery().  
+0000dff0: 2020 2020 2020 6966 2071 7565 7279 2069        if query i
+0000e000: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000e010: 2020 2020 7175 6572 7920 3d20 7365 6c66      query = self
+0000e020: 2e61 6464 4368 696c 6428 2771 7565 7279  .addChild('query
+0000e030: 2729 0a20 2020 2020 2020 2069 6620 6e61  ').        if na
+0000e040: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+0000e050: 2020 2020 2020 2020 2020 2020 7175 6572              quer
+0000e060: 792e 7365 744e 616d 6528 6e61 6d65 290a  y.setName(name).
+0000e070: 2020 2020 2020 2020 7265 7475 726e 2071          return q
+0000e080: 7565 7279 0a0a 2020 2020 6465 6620 7365  uery..    def se
+0000e090: 7451 7565 7279 4e53 2873 656c 662c 206e  tQueryNS(self, n
+0000e0a0: 616d 6573 7061 6365 3a20 7374 7229 202d  amespace: str) -
+0000e0b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000e0c0: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
+0000e0d0: 7468 6520 6e61 6d65 7370 6163 6520 6f66  the namespace of
+0000e0e0: 2074 6865 2027 7175 6572 7927 2063 6869   the 'query' chi
+0000e0f0: 6c64 2065 6c65 6d65 6e74 0a20 2020 2020  ld element.     
+0000e100: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0000e110: 656c 662e 7365 7451 7565 7279 2829 2e73  elf.setQuery().s
+0000e120: 6574 4e61 6d65 7370 6163 6528 6e61 6d65  etNamespace(name
+0000e130: 7370 6163 6529 0a0a 2020 2020 6465 6620  space)..    def 
+0000e140: 7365 7451 7565 7279 5061 796c 6f61 6428  setQueryPayload(
+0000e150: 7365 6c66 2c20 7061 796c 6f61 643a 206c  self, payload: l
+0000e160: 6973 745b 556e 696f 6e5b 4e6f 6465 2c20  ist[Union[Node, 
+0000e170: 7374 725d 5d29 3a0a 2020 2020 2020 2020  str]]):.        
+0000e180: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
+0000e190: 7468 6520 2771 7565 7279 2720 6368 696c  the 'query' chil
+0000e1a0: 6420 656c 656d 656e 7420 7061 796c 6f61  d element payloa
+0000e1b0: 640a 2020 2020 2020 2020 2222 220a 2020  d.        """.  
+0000e1c0: 2020 2020 2020 7365 6c66 2e73 6574 5175        self.setQu
+0000e1d0: 6572 7928 292e 7365 7450 6179 6c6f 6164  ery().setPayload
+0000e1e0: 2870 6179 6c6f 6164 290a 0a20 2020 2064  (payload)..    d
+0000e1f0: 6566 2073 6574 5175 6572 796e 6f64 6528  ef setQuerynode(
+0000e200: 7365 6c66 2c20 6e6f 6465 3a20 7374 7229  self, node: str)
+0000e210: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000e220: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
+0000e230: 7420 7468 6520 276e 6f64 6527 2061 7474  t the 'node' att
+0000e240: 7269 6275 7465 2076 616c 7565 206f 6620  ribute value of 
+0000e250: 7468 6520 2771 7565 7279 2720 6368 696c  the 'query' chil
+0000e260: 6420 656c 656d 656e 740a 2020 2020 2020  d element.      
+0000e270: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+0000e280: 6c66 2e73 6574 5175 6572 7928 292e 7365  lf.setQuery().se
+0000e290: 7441 7474 7228 276e 6f64 6527 2c20 6e6f  tAttr('node', no
+0000e2a0: 6465 290a 0a20 2020 2064 6566 2062 7569  de)..    def bui
+0000e2b0: 6c64 5265 706c 7928 7365 6c66 2c20 7479  ldReply(self, ty
+0000e2c0: 703a 2073 7472 2920 2d3e 2049 713a 0a20  p: str) -> Iq:. 
+0000e2d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e2e0: 2020 2042 7569 6c64 2061 6e64 2072 6574     Build and ret
+0000e2f0: 7572 6e20 616e 6f74 6865 7220 4971 206f  urn another Iq o
+0000e300: 626a 6563 7420 6f66 2073 7065 6369 6669  bject of specifi
+0000e310: 6564 2074 7970 652e 2054 6865 2074 6f2c  ed type. The to,
+0000e320: 2066 726f 6d20 616e 640a 2020 2020 2020   from and.      
+0000e330: 2020 7175 6572 7920 6368 696c 6420 6e6f    query child no
+0000e340: 6465 206f 6620 6e65 7720 4971 2061 7265  de of new Iq are
+0000e350: 2070 7265 2d73 6574 2061 7320 7265 706c   pre-set as repl
+0000e360: 7920 746f 2074 6869 7320 4971 2e0a 2020  y to this Iq..  
+0000e370: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e380: 2020 6971 203d 2049 7128 7479 702c 0a20    iq = Iq(typ,. 
+0000e390: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e3a0: 6f3d 7365 6c66 2e67 6574 4672 6f6d 2829  o=self.getFrom()
+0000e3b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e3c0: 2020 6672 6d3d 7365 6c66 2e67 6574 546f    frm=self.getTo
+0000e3d0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0000e3e0: 2020 2020 6174 7472 733d 7b27 6964 273a      attrs={'id':
+0000e3f0: 2073 656c 662e 6765 7449 4428 297d 290a   self.getID()}).
+0000e400: 2020 2020 2020 2020 6971 2e73 6574 5175          iq.setQu
+0000e410: 6572 7928 7365 6c66 2e67 6574 5175 6572  ery(self.getQuer
+0000e420: 7928 292e 6765 744e 616d 6528 2929 2e73  y().getName()).s
+0000e430: 6574 4e61 6d65 7370 6163 6528 7365 6c66  etNamespace(self
+0000e440: 2e67 6574 5175 6572 794e 5328 2929 0a20  .getQueryNS()). 
+0000e450: 2020 2020 2020 2072 6574 7572 6e20 6971         return iq
+0000e460: 0a0a 2020 2020 6465 6620 6275 696c 6453  ..    def buildS
+0000e470: 696d 706c 6552 6570 6c79 2873 656c 662c  impleReply(self,
+0000e480: 2074 7970 3a20 7374 7229 202d 3e20 4971   typ: str) -> Iq
+0000e490: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000e4a0: 2049 7128 7479 702c 0a20 2020 2020 2020   Iq(typ,.       
+0000e4b0: 2020 2020 2020 2020 2020 2074 6f3d 7365             to=se
+0000e4c0: 6c66 2e67 6574 4672 6f6d 2829 2c0a 2020  lf.getFrom(),.  
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 6174 7472 733d 7b27 6964 273a 2073 656c  attrs={'id': sel
+0000e4f0: 662e 6765 7449 4428 297d 290a 0a0a 636c  f.getID()})...cl
+0000e500: 6173 7320 4861 7368 6573 284e 6f64 6529  ass Hashes(Node)
+0000e510: 3a0a 2020 2020 2222 220a 2020 2020 4861  :.    """.    Ha
+0000e520: 7368 2065 6c65 6d65 6e74 7320 666f 7220  sh elements for 
+0000e530: 7661 7269 6f75 7320 5845 5073 2061 7320  various XEPs as 
+0000e540: 6465 6669 6e65 6420 696e 2058 4550 2d33  defined in XEP-3
+0000e550: 3030 0a0a 2020 2020 5245 434f 4d45 4e44  00..    RECOMEND
+0000e560: 4544 2048 4153 4820 5553 453a 0a20 2020  ED HASH USE:.   
+0000e570: 2041 6c67 6f72 6974 686d 2020 2020 2053   Algorithm     S
+0000e580: 7570 706f 7274 0a20 2020 204d 4432 2020  upport.    MD2  
+0000e590: 2020 2020 2020 2020 204d 5553 5420 4e4f           MUST NO
+0000e5a0: 540a 2020 2020 4d44 3420 2020 2020 2020  T.    MD4       
+0000e5b0: 2020 2020 4d55 5354 204e 4f54 0a20 2020      MUST NOT.   
+0000e5c0: 204d 4435 2020 2020 2020 2020 2020 204d   MD5           M
+0000e5d0: 4159 0a20 2020 2053 4841 2d31 2020 2020  AY.    SHA-1    
+0000e5e0: 2020 2020 204d 5553 540a 2020 2020 5348       MUST.    SH
+0000e5f0: 412d 3235 3620 2020 2020 2020 4d55 5354  A-256       MUST
+0000e600: 0a20 2020 2053 4841 2d35 3132 2020 2020  .    SHA-512    
+0000e610: 2020 2053 484f 554c 440a 2020 2020 2222     SHOULD.    ""
+0000e620: 220a 0a20 2020 2073 7570 706f 7274 6564  "..    supported
+0000e630: 203d 2028 276d 6435 272c 2027 7368 612d   = ('md5', 'sha-
+0000e640: 3127 2c20 2773 6861 2d32 3536 272c 2027  1', 'sha-256', '
+0000e650: 7368 612d 3531 3227 290a 0a20 2020 2064  sha-512')..    d
+0000e660: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000e670: 2c20 6e73 703d 4e61 6d65 7370 6163 652e  , nsp=Namespace.
+0000e680: 4841 5348 4553 293a 0a20 2020 2020 2020  HASHES):.       
+0000e690: 204e 6f64 652e 5f5f 696e 6974 5f5f 2873   Node.__init__(s
+0000e6a0: 656c 662c 204e 6f6e 652c 207b 7d2c 205b  elf, None, {}, [
+0000e6b0: 5d2c 204e 6f6e 652c 204e 6f6e 652c 2046  ], None, None, F
+0000e6c0: 616c 7365 2c20 4e6f 6e65 290a 2020 2020  alse, None).    
+0000e6d0: 2020 2020 7365 6c66 2e73 6574 4e61 6d65      self.setName
+0000e6e0: 7370 6163 6528 6e73 7029 0a20 2020 2020  space(nsp).     
+0000e6f0: 2020 2073 656c 662e 7365 744e 616d 6528     self.setName(
+0000e700: 2768 6173 6827 290a 0a20 2020 2064 6566  'hash')..    def
+0000e710: 2063 616c 6375 6c61 7465 4861 7368 2873   calculateHash(s
+0000e720: 656c 662c 2061 6c67 6f2c 2066 696c 655f  elf, algo, file_
+0000e730: 7374 7269 6e67 293a 0a20 2020 2020 2020  string):.       
+0000e740: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+0000e750: 6375 6c61 7465 2074 6865 2068 6173 6820  culate the hash 
+0000e760: 616e 6420 6164 6420 6974 2e20 4974 2069  and add it. It i
+0000e770: 7320 7072 6566 6572 6162 6c65 2064 6f69  s preferable doi
+0000e780: 6e67 2069 7420 6865 7265 0a20 2020 2020  ng it here.     
+0000e790: 2020 2069 6e73 7465 6164 206f 6620 646f     instead of do
+0000e7a0: 696e 6720 6974 2061 6c6c 206f 7665 7220  ing it all over 
+0000e7b0: 7468 6520 706c 6163 6520 696e 2047 616a  the place in Gaj
+0000e7c0: 696d 2e0a 2020 2020 2020 2020 2222 220a  im..        """.
+0000e7d0: 2020 2020 2020 2020 686c 203d 204e 6f6e          hl = Non
+0000e7e0: 650a 2020 2020 2020 2020 6861 7368 5f20  e.        hash_ 
+0000e7f0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2023  = None.        #
+0000e800: 2066 696c 655f 7374 7269 6e67 2063 616e   file_string can
+0000e810: 2062 6520 6120 7374 7269 6e67 206f 7220   be a string or 
+0000e820: 6120 6669 6c65 0a20 2020 2020 2020 2069  a file.        i
+0000e830: 6620 6973 696e 7374 616e 6365 2866 696c  f isinstance(fil
+0000e840: 655f 7374 7269 6e67 2c20 7374 7229 3a0a  e_string, str):.
+0000e850: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0000e860: 6c67 6f20 3d3d 2027 7368 612d 3127 3a0a  lgo == 'sha-1':.
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e880: 686c 203d 2068 6173 686c 6962 2e73 6861  hl = hashlib.sha
+0000e890: 3128 290a 2020 2020 2020 2020 2020 2020  1().            
+0000e8a0: 656c 6966 2061 6c67 6f20 3d3d 2027 6d64  elif algo == 'md
+0000e8b0: 3527 3a0a 2020 2020 2020 2020 2020 2020  5':.            
+0000e8c0: 2020 2020 686c 203d 2068 6173 686c 6962      hl = hashlib
+0000e8d0: 2e6d 6435 2829 0a20 2020 2020 2020 2020  .md5().         
+0000e8e0: 2020 2065 6c69 6620 616c 676f 203d 3d20     elif algo == 
+0000e8f0: 2773 6861 2d32 3536 273a 0a20 2020 2020  'sha-256':.     
+0000e900: 2020 2020 2020 2020 2020 2068 6c20 3d20             hl = 
+0000e910: 6861 7368 6c69 622e 7368 6132 3536 2829  hashlib.sha256()
+0000e920: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000e930: 6620 616c 676f 203d 3d20 2773 6861 2d35  f algo == 'sha-5
+0000e940: 3132 273a 0a20 2020 2020 2020 2020 2020  12':.           
+0000e950: 2020 2020 2068 6c20 3d20 6861 7368 6c69       hl = hashli
+0000e960: 622e 7368 6135 3132 2829 0a20 2020 2020  b.sha512().     
+0000e970: 2020 2020 2020 2069 6620 686c 3a0a 2020         if hl:.  
+0000e980: 2020 2020 2020 2020 2020 2020 2020 686c                hl
+0000e990: 2e75 7064 6174 6528 6669 6c65 5f73 7472  .update(file_str
+0000e9a0: 696e 6729 0a20 2020 2020 2020 2020 2020  ing).           
+0000e9b0: 2020 2020 2068 6173 685f 203d 2068 6c2e       hash_ = hl.
+0000e9c0: 6865 7864 6967 6573 7428 290a 2020 2020  hexdigest().    
+0000e9d0: 2020 2020 656c 7365 3a20 2320 6966 2069      else: # if i
+0000e9e0: 7420 6973 2061 2066 696c 650a 2020 2020  t is a file.    
+0000e9f0: 2020 2020 2020 2020 6966 2061 6c67 6f20          if algo 
+0000ea00: 3d3d 2027 7368 612d 3127 3a0a 2020 2020  == 'sha-1':.    
+0000ea10: 2020 2020 2020 2020 2020 2020 686c 203d              hl =
+0000ea20: 2068 6173 686c 6962 2e73 6861 3128 290a   hashlib.sha1().
+0000ea30: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000ea40: 2061 6c67 6f20 3d3d 2027 6d64 3527 3a0a   algo == 'md5':.
+0000ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea60: 686c 203d 2068 6173 686c 6962 2e6d 6435  hl = hashlib.md5
+0000ea70: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
+0000ea80: 6c69 6620 616c 676f 203d 3d20 2773 6861  lif algo == 'sha
+0000ea90: 2d32 3536 273a 0a20 2020 2020 2020 2020  -256':.         
+0000eaa0: 2020 2020 2020 2068 6c20 3d20 6861 7368         hl = hash
+0000eab0: 6c69 622e 7368 6132 3536 2829 0a20 2020  lib.sha256().   
+0000eac0: 2020 2020 2020 2020 2065 6c69 6620 616c           elif al
+0000ead0: 676f 203d 3d20 2773 6861 2d35 3132 273a  go == 'sha-512':
+0000eae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eaf0: 2068 6c20 3d20 6861 7368 6c69 622e 7368   hl = hashlib.sh
+0000eb00: 6135 3132 2829 0a20 2020 2020 2020 2020  a512().         
+0000eb10: 2020 2069 6620 686c 3a0a 2020 2020 2020     if hl:.      
+0000eb20: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
+0000eb30: 6e65 2069 6e20 6669 6c65 5f73 7472 696e  ne in file_strin
+0000eb40: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+0000eb50: 2020 2020 2020 2068 6c2e 7570 6461 7465         hl.update
+0000eb60: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
+0000eb70: 2020 2020 2020 2068 6173 685f 203d 2068         hash_ = h
+0000eb80: 6c2e 6865 7864 6967 6573 7428 290a 2020  l.hexdigest().  
+0000eb90: 2020 2020 2020 7265 7475 726e 2068 6173        return has
+0000eba0: 685f 0a0a 2020 2020 6465 6620 6164 6448  h_..    def addH
+0000ebb0: 6173 6828 7365 6c66 2c20 6861 7368 5f2c  ash(self, hash_,
+0000ebc0: 2061 6c67 6f29 3a0a 2020 2020 2020 2020   algo):.        
+0000ebd0: 7365 6c66 2e73 6574 4174 7472 2827 616c  self.setAttr('al
+0000ebe0: 676f 272c 2061 6c67 6f29 0a20 2020 2020  go', algo).     
+0000ebf0: 2020 2073 656c 662e 7365 7444 6174 6128     self.setData(
+0000ec00: 6861 7368 5f29 0a0a 636c 6173 7320 4861  hash_)..class Ha
+0000ec10: 7368 6573 3228 4e6f 6465 293a 0a20 2020  shes2(Node):.   
+0000ec20: 2022 2222 0a20 2020 2048 6173 6820 656c   """.    Hash el
+0000ec30: 656d 656e 7473 2066 6f72 2076 6172 696f  ements for vario
+0000ec40: 7573 2058 4550 7320 6173 2064 6566 696e  us XEPs as defin
+0000ec50: 6564 2069 6e20 5845 502d 3330 300a 0a20  ed in XEP-300.. 
+0000ec60: 2020 2052 4543 4f4d 454e 4445 4420 4841     RECOMENDED HA
+0000ec70: 5348 2055 5345 3a0a 2020 2020 416c 676f  SH USE:.    Algo
+0000ec80: 7269 7468 6d20 2020 2020 5375 7070 6f72  rithm     Suppor
+0000ec90: 740a 2020 2020 4d44 3220 2020 2020 2020  t.    MD2       
+0000eca0: 2020 2020 4d55 5354 204e 4f54 0a20 2020      MUST NOT.   
+0000ecb0: 204d 4434 2020 2020 2020 2020 2020 204d   MD4           M
+0000ecc0: 5553 5420 4e4f 540a 2020 2020 4d44 3520  UST NOT.    MD5 
+0000ecd0: 2020 2020 2020 2020 2020 4d55 5354 204e            MUST N
+0000ece0: 4f54 0a20 2020 2053 4841 2d31 2020 2020  OT.    SHA-1    
+0000ecf0: 2020 2020 2053 484f 554c 4420 4e4f 540a       SHOULD NOT.
+0000ed00: 2020 2020 5348 412d 3235 3620 2020 2020      SHA-256     
+0000ed10: 2020 4d55 5354 0a20 2020 2053 4841 2d35    MUST.    SHA-5
+0000ed20: 3132 2020 2020 2020 2053 484f 554c 440a  12       SHOULD.
+0000ed30: 2020 2020 5348 4133 2d32 3536 2020 2020      SHA3-256    
+0000ed40: 2020 4d55 5354 0a20 2020 2053 4841 332d    MUST.    SHA3-
+0000ed50: 3531 3220 2020 2020 2053 484f 554c 440a  512      SHOULD.
+0000ed60: 2020 2020 424c 414b 4532 6232 3536 2020      BLAKE2b256  
+0000ed70: 2020 4d55 5354 0a20 2020 2042 4c41 4b45    MUST.    BLAKE
+0000ed80: 3262 3531 3220 2020 2053 484f 554c 440a  2b512    SHOULD.
+0000ed90: 2020 2020 2222 220a 0a20 2020 2073 7570      """..    sup
+0000eda0: 706f 7274 6564 203d 2028 2773 6861 2d32  ported = ('sha-2
+0000edb0: 3536 272c 2027 7368 612d 3531 3227 2c20  56', 'sha-512', 
+0000edc0: 2773 6861 332d 3235 3627 2c0a 2020 2020  'sha3-256',.    
+0000edd0: 2020 2020 2020 2020 2020 2020 2027 7368               'sh
+0000ede0: 6133 2d35 3132 272c 2027 626c 616b 6532  a3-512', 'blake2
+0000edf0: 622d 3235 3627 2c20 2762 6c61 6b65 3262  b-256', 'blake2b
+0000ee00: 2d35 3132 2729 0a0a 2020 2020 6465 6620  -512')..    def 
+0000ee10: 5f5f 696e 6974 5f5f 2873 656c 662c 206e  __init__(self, n
+0000ee20: 7370 3d4e 616d 6573 7061 6365 2e48 4153  sp=Namespace.HAS
+0000ee30: 4845 535f 3229 3a0a 2020 2020 2020 2020  HES_2):.        
+0000ee40: 4e6f 6465 2e5f 5f69 6e69 745f 5f28 7365  Node.__init__(se
+0000ee50: 6c66 2c20 4e6f 6e65 2c20 7b7d 2c20 5b5d  lf, None, {}, []
+0000ee60: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4661  , None, None, Fa
+0000ee70: 6c73 652c 204e 6f6e 6529 0a20 2020 2020  lse, None).     
+0000ee80: 2020 2073 656c 662e 7365 744e 616d 6573     self.setNames
+0000ee90: 7061 6365 286e 7370 290a 2020 2020 2020  pace(nsp).      
+0000eea0: 2020 7365 6c66 2e73 6574 4e61 6d65 2827    self.setName('
+0000eeb0: 6861 7368 2729 0a0a 2020 2020 6465 6620  hash')..    def 
+0000eec0: 6361 6c63 756c 6174 6548 6173 6828 7365  calculateHash(se
+0000eed0: 6c66 2c20 616c 676f 2c20 6669 6c65 5f73  lf, algo, file_s
+0000eee0: 7472 696e 6729 3a0a 2020 2020 2020 2020  tring):.        
+0000eef0: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
+0000ef00: 756c 6174 6520 7468 6520 6861 7368 2061  ulate the hash a
+0000ef10: 6e64 2061 6464 2069 742e 2049 7420 6973  nd add it. It is
+0000ef20: 2070 7265 6665 7261 626c 6520 646f 696e   preferable doin
+0000ef30: 6720 6974 2068 6572 650a 2020 2020 2020  g it here.      
+0000ef40: 2020 696e 7374 6561 6420 6f66 2064 6f69    instead of doi
+0000ef50: 6e67 2069 7420 616c 6c20 6f76 6572 2074  ng it all over t
+0000ef60: 6865 2070 6c61 6365 2069 6e20 4761 6a69  he place in Gaji
+0000ef70: 6d2e 0a20 2020 2020 2020 2022 2222 0a20  m..        """. 
+0000ef80: 2020 2020 2020 2068 6c20 3d20 4e6f 6e65         hl = None
+0000ef90: 0a20 2020 2020 2020 2068 6173 685f 203d  .        hash_ =
+0000efa0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+0000efb0: 2061 6c67 6f20 3d3d 2027 7368 612d 3235   algo == 'sha-25
+0000efc0: 3627 3a0a 2020 2020 2020 2020 2020 2020  6':.            
+0000efd0: 686c 203d 2068 6173 686c 6962 2e73 6861  hl = hashlib.sha
+0000efe0: 3235 3628 290a 2020 2020 2020 2020 656c  256().        el
+0000eff0: 6966 2061 6c67 6f20 3d3d 2027 7368 612d  if algo == 'sha-
+0000f000: 3531 3227 3a0a 2020 2020 2020 2020 2020  512':.          
+0000f010: 2020 686c 203d 2068 6173 686c 6962 2e73    hl = hashlib.s
+0000f020: 6861 3531 3228 290a 2020 2020 2020 2020  ha512().        
+0000f030: 656c 6966 2061 6c67 6f20 3d3d 2027 7368  elif algo == 'sh
+0000f040: 6133 2d32 3536 273a 0a20 2020 2020 2020  a3-256':.       
+0000f050: 2020 2020 2068 6c20 3d20 6861 7368 6c69       hl = hashli
+0000f060: 622e 7368 6133 5f32 3536 2829 0a20 2020  b.sha3_256().   
+0000f070: 2020 2020 2065 6c69 6620 616c 676f 203d       elif algo =
+0000f080: 3d20 2773 6861 332d 3531 3227 3a0a 2020  = 'sha3-512':.  
+0000f090: 2020 2020 2020 2020 2020 686c 203d 2068            hl = h
+0000f0a0: 6173 686c 6962 2e73 6861 335f 3531 3228  ashlib.sha3_512(
+0000f0b0: 290a 2020 2020 2020 2020 656c 6966 2061  ).        elif a
+0000f0c0: 6c67 6f20 3d3d 2027 626c 616b 6532 622d  lgo == 'blake2b-
+0000f0d0: 3235 3627 3a0a 2020 2020 2020 2020 2020  256':.          
+0000f0e0: 2020 686c 203d 2068 6173 686c 6962 2e62    hl = hashlib.b
+0000f0f0: 6c61 6b65 3262 2864 6967 6573 745f 7369  lake2b(digest_si
+0000f100: 7a65 3d33 3229 0a20 2020 2020 2020 2065  ze=32).        e
+0000f110: 6c69 6620 616c 676f 203d 3d20 2762 6c61  lif algo == 'bla
+0000f120: 6b65 3262 2d35 3132 273a 0a20 2020 2020  ke2b-512':.     
+0000f130: 2020 2020 2020 2068 6c20 3d20 6861 7368         hl = hash
+0000f140: 6c69 622e 626c 616b 6532 6228 6469 6765  lib.blake2b(dige
+0000f150: 7374 5f73 697a 653d 3634 290a 2020 2020  st_size=64).    
+0000f160: 2020 2020 2320 6669 6c65 5f73 7472 696e      # file_strin
+0000f170: 6720 6361 6e20 6265 2061 2073 7472 696e  g can be a strin
+0000f180: 6720 6f72 2061 2066 696c 650a 2020 2020  g or a file.    
+0000f190: 2020 2020 6966 2068 6c20 6973 206e 6f74      if hl is not
+0000f1a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000f1b0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000f1c0: 2866 696c 655f 7374 7269 6e67 2c20 6279  (file_string, by
+0000f1d0: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
+0000f1e0: 2020 2020 2020 686c 2e75 7064 6174 6528        hl.update(
+0000f1f0: 6669 6c65 5f73 7472 696e 6729 0a20 2020  file_string).   
+0000f200: 2020 2020 2020 2020 2065 6c73 653a 2023           else: #
+0000f210: 2069 6620 6974 2069 7320 6120 6669 6c65   if it is a file
+0000f220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f230: 2066 6f72 206c 696e 6520 696e 2066 696c   for line in fil
+0000f240: 655f 7374 7269 6e67 3a0a 2020 2020 2020  e_string:.      
+0000f250: 2020 2020 2020 2020 2020 2020 2020 686c                hl
+0000f260: 2e75 7064 6174 6528 6c69 6e65 290a 2020  .update(line).  
+0000f270: 2020 2020 2020 2020 2020 6861 7368 5f20            hash_ 
+0000f280: 3d20 6236 3465 6e63 6f64 6528 686c 2e64  = b64encode(hl.d
+0000f290: 6967 6573 7428 2929 2e64 6563 6f64 6528  igest()).decode(
+0000f2a0: 2761 7363 6969 2729 0a20 2020 2020 2020  'ascii').       
+0000f2b0: 2072 6574 7572 6e20 6861 7368 5f0a 0a20   return hash_.. 
+0000f2c0: 2020 2064 6566 2061 6464 4861 7368 2873     def addHash(s
+0000f2d0: 656c 662c 2068 6173 685f 2c20 616c 676f  elf, hash_, algo
+0000f2e0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000f2f0: 7365 7441 7474 7228 2761 6c67 6f27 2c20  setAttr('algo', 
+0000f300: 616c 676f 290a 2020 2020 2020 2020 7365  algo).        se
+0000f310: 6c66 2e73 6574 4461 7461 2868 6173 685f  lf.setData(hash_
+0000f320: 290a 0a0a 636c 6173 7320 4269 6e64 5265  )...class BindRe
+0000f330: 7175 6573 7428 4971 293a 0a20 2020 2064  quest(Iq):.    d
+0000f340: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000f350: 2c20 7265 736f 7572 6365 3a20 4f70 7469  , resource: Opti
+0000f360: 6f6e 616c 5b73 7472 5d29 3a0a 2020 2020  onal[str]):.    
+0000f370: 2020 2020 6966 2072 6573 6f75 7263 6520      if resource 
+0000f380: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000f390: 2020 2020 2072 6573 203d 2072 6573 6f75       res = resou
+0000f3a0: 7263 650a 2020 2020 2020 2020 656c 7365  rce.        else
+0000f3b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000f3c0: 7320 3d20 4e6f 6465 2827 7265 736f 7572  s = Node('resour
+0000f3d0: 6365 272c 2070 6179 6c6f 6164 3d72 6573  ce', payload=res
+0000f3e0: 6f75 7263 6529 0a20 2020 2020 2020 2049  ource).        I
+0000f3f0: 712e 5f5f 696e 6974 5f5f 2873 656c 662c  q.__init__(self,
+0000f400: 2074 7970 3d27 7365 7427 290a 2020 2020   typ='set').    
+0000f410: 2020 2020 7365 6c66 2e61 6464 4368 696c      self.addChil
+0000f420: 6428 6e6f 6465 3d4e 6f64 6528 2762 696e  d(node=Node('bin
+0000f430: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 2020 2020 7b27 786d 6c6e 7327 3a20 4e61      {'xmlns': Na
+0000f460: 6d65 7370 6163 652e 4249 4e44 7d2c 0a20  mespace.BIND},. 
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000f490: 6179 6c6f 6164 3d72 6573 2929 0a0a 0a63  ayload=res))...c
+0000f4a0: 6c61 7373 2054 4c53 5265 7175 6573 7428  lass TLSRequest(
+0000f4b0: 4e6f 6465 293a 0a20 2020 2064 6566 205f  Node):.    def _
+0000f4c0: 5f69 6e69 745f 5f28 7365 6c66 293a 0a20  _init__(self):. 
+0000f4d0: 2020 2020 2020 204e 6f64 652e 5f5f 696e         Node.__in
+0000f4e0: 6974 5f5f 2873 656c 662c 2074 6167 3d27  it__(self, tag='
+0000f4f0: 7374 6172 7474 6c73 272c 2061 7474 7273  starttls', attrs
+0000f500: 3d7b 2778 6d6c 6e73 273a 204e 616d 6573  ={'xmlns': Names
+0000f510: 7061 6365 2e54 4c53 7d29 0a0a 0a63 6c61  pace.TLS})...cla
+0000f520: 7373 2053 6573 7369 6f6e 5265 7175 6573  ss SessionReques
+0000f530: 7428 4971 293a 0a20 2020 2064 6566 205f  t(Iq):.    def _
+0000f540: 5f69 6e69 745f 5f28 7365 6c66 293a 0a20  _init__(self):. 
+0000f550: 2020 2020 2020 2049 712e 5f5f 696e 6974         Iq.__init
+0000f560: 5f5f 2873 656c 662c 2074 7970 3d27 7365  __(self, typ='se
+0000f570: 7427 290a 2020 2020 2020 2020 7365 6c66  t').        self
+0000f580: 2e61 6464 4368 696c 6428 6e6f 6465 3d4e  .addChild(node=N
+0000f590: 6f64 6528 2773 6573 7369 6f6e 272c 2061  ode('session', a
+0000f5a0: 7474 7273 3d7b 2778 6d6c 6e73 273a 204e  ttrs={'xmlns': N
+0000f5b0: 616d 6573 7061 6365 2e53 4553 5349 4f4e  amespace.SESSION
+0000f5c0: 7d29 290a 0a0a 636c 6173 7320 5374 7265  }))...class Stre
+0000f5d0: 616d 4865 6164 6572 284e 6f64 6529 3a0a  amHeader(Node):.
+0000f5e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000f5f0: 2873 656c 662c 2064 6f6d 6169 6e3a 2073  (self, domain: s
+0000f600: 7472 2c20 6c61 6e67 3a20 4f70 7469 6f6e  tr, lang: Option
+0000f610: 616c 5b73 7472 5d20 3d20 4e6f 6e65 293a  al[str] = None):
+0000f620: 0a20 2020 2020 2020 2069 6620 6c61 6e67  .        if lang
+0000f630: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000f640: 2020 2020 2020 6c61 6e67 203d 2027 656e        lang = 'en
+0000f650: 270a 2020 2020 2020 2020 4e6f 6465 2e5f  '.        Node._
+0000f660: 5f69 6e69 745f 5f28 7365 6c66 2c0a 2020  _init__(self,.  
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 2020 7461 673d 2773 7472 6561 6d3a      tag='stream:
+0000f690: 7374 7265 616d 272c 0a20 2020 2020 2020  stream',.       
+0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000f6b0: 7474 7273 3d7b 2778 6d6c 6e73 273a 204e  ttrs={'xmlns': N
+0000f6c0: 616d 6573 7061 6365 2e43 4c49 454e 542c  amespace.CLIENT,
+0000f6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2776                'v
+0000f6f0: 6572 7369 6f6e 273a 2027 312e 3027 2c0a  ersion': '1.0',.
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f710: 2020 2020 2020 2020 2020 2020 2027 786d               'xm
+0000f720: 6c6e 733a 7374 7265 616d 273a 204e 616d  lns:stream': Nam
+0000f730: 6573 7061 6365 2e53 5452 4541 4d53 2c0a  espace.STREAMS,.
+0000f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f750: 2020 2020 2020 2020 2020 2020 2027 746f               'to
+0000f760: 273a 2064 6f6d 6169 6e2c 0a20 2020 2020  ': domain,.     
+0000f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f780: 2020 2020 2020 2020 2778 6d6c 3a6c 616e          'xml:lan
+0000f790: 6727 3a20 6c61 6e67 7d29 0a0a 0a63 6c61  g': lang})...cla
+0000f7a0: 7373 2057 6562 736f 636b 6574 4f70 656e  ss WebsocketOpen
+0000f7b0: 4865 6164 6572 284e 6f64 6529 3a0a 2020  Header(Node):.  
+0000f7c0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000f7d0: 656c 662c 2064 6f6d 6169 6e3a 2073 7472  elf, domain: str
+0000f7e0: 2c20 6c61 6e67 3a20 4f70 7469 6f6e 616c  , lang: Optional
+0000f7f0: 5b73 7472 5d20 3d20 4e6f 6e65 293a 0a20  [str] = None):. 
+0000f800: 2020 2020 2020 2069 6620 6c61 6e67 2069         if lang i
+0000f810: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000f820: 2020 2020 6c61 6e67 203d 2027 656e 270a      lang = 'en'.
+0000f830: 2020 2020 2020 2020 4e6f 6465 2e5f 5f69          Node.__i
+0000f840: 6e69 745f 5f28 7365 6c66 2c0a 2020 2020  nit__(self,.    
 0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 2020 2020 2020 2778 6d6c 3a6c            'xml:l
-0000f870: 616e 6727 3a20 6c61 6e67 7d29 0a0a 636c  ang': lang})..cl
-0000f880: 6173 7320 5765 6273 6f63 6b65 7443 6c6f  ass WebsocketClo
-0000f890: 7365 4865 6164 6572 284e 6f64 6529 3a0a  seHeader(Node):.
-0000f8a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000f8b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f8c0: 4e6f 6465 2e5f 5f69 6e69 745f 5f28 7365  Node.__init__(se
-0000f8d0: 6c66 2c20 7461 673d 2763 6c6f 7365 272c  lf, tag='close',
-0000f8e0: 2061 7474 7273 3d7b 2778 6d6c 6e73 273a   attrs={'xmlns':
-0000f8f0: 204e 616d 6573 7061 6365 2e46 5241 4d49   Namespace.FRAMI
-0000f900: 4e47 7d29 0a0a 0a63 6c61 7373 2046 6561  NG})...class Fea
-0000f910: 7475 7265 7328 4e6f 6465 293a 0a20 2020  tures(Node):.   
-0000f920: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0000f930: 6c66 2c20 6e6f 6465 3a20 4e6f 6465 293a  lf, node: Node):
-0000f940: 0a20 2020 2020 2020 204e 6f64 652e 5f5f  .        Node.__
-0000f950: 696e 6974 5f5f 2873 656c 662c 206e 6f64  init__(self, nod
-0000f960: 653d 6e6f 6465 290a 0a20 2020 2064 6566  e=node)..    def
-0000f970: 2068 6173 5f73 7461 7274 746c 7328 7365   has_starttls(se
-0000f980: 6c66 293a 0a20 2020 2020 2020 2074 6c73  lf):.        tls
-0000f990: 203d 2073 656c 662e 6765 7454 6167 2827   = self.getTag('
-0000f9a0: 7374 6172 7474 6c73 272c 206e 616d 6573  starttls', names
-0000f9b0: 7061 6365 3d4e 616d 6573 7061 6365 2e54  pace=Namespace.T
-0000f9c0: 4c53 290a 2020 2020 2020 2020 6966 2074  LS).        if t
-0000f9d0: 6c73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ls is not None:.
-0000f9e0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000f9f0: 6972 6564 203d 2074 6c73 2e67 6574 5461  ired = tls.getTa
-0000fa00: 6728 2772 6571 7569 7265 6427 2920 6973  g('required') is
-0000fa10: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-0000fa20: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000fa30: 652c 2072 6571 7569 7265 640a 2020 2020  e, required.    
-0000fa40: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000fa50: 2c20 4661 6c73 650a 0a20 2020 2064 6566  , False..    def
-0000fa60: 2068 6173 5f73 6173 6c28 7365 6c66 293a   has_sasl(self):
-0000fa70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fa80: 7365 6c66 2e67 6574 5461 6728 276d 6563  self.getTag('mec
-0000fa90: 6861 6e69 736d 7327 2c20 6e61 6d65 7370  hanisms', namesp
-0000faa0: 6163 653d 4e61 6d65 7370 6163 652e 5341  ace=Namespace.SA
-0000fab0: 534c 2920 6973 206e 6f74 204e 6f6e 650a  SL) is not None.
-0000fac0: 0a20 2020 2064 6566 2068 6173 5f73 6173  .    def has_sas
-0000fad0: 6c5f 3228 7365 6c66 293a 0a20 2020 2020  l_2(self):.     
-0000fae0: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-0000faf0: 6574 5461 6728 276d 6563 6861 6e69 736d  etTag('mechanism
-0000fb00: 7327 2c20 6e61 6d65 7370 6163 653d 4e61  s', namespace=Na
-0000fb10: 6d65 7370 6163 652e 5341 534c 3229 2069  mespace.SASL2) i
-0000fb20: 7320 6e6f 7420 4e6f 6e65 0a0a 2020 2020  s not None..    
-0000fb30: 6465 6620 6765 745f 6d65 6368 7328 7365  def get_mechs(se
-0000fb40: 6c66 2920 2d3e 2073 6574 5b73 7472 5d3a  lf) -> set[str]:
-0000fb50: 0a20 2020 2020 2020 206d 6563 6861 6e69  .        mechani
-0000fb60: 736d 7320 3d20 7365 6c66 2e67 6574 5461  sms = self.getTa
-0000fb70: 6728 276d 6563 6861 6e69 736d 7327 2c20  g('mechanisms', 
-0000fb80: 6e61 6d65 7370 6163 653d 4e61 6d65 7370  namespace=Namesp
-0000fb90: 6163 652e 5341 534c 3229 0a20 2020 2020  ace.SASL2).     
-0000fba0: 2020 2069 6620 6d65 6368 616e 6973 6d73     if mechanisms
-0000fbb0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000fbc0: 2020 2020 2020 6d65 6368 616e 6973 6d73        mechanisms
-0000fbd0: 203d 2073 656c 662e 6765 7454 6167 2827   = self.getTag('
-0000fbe0: 6d65 6368 616e 6973 6d73 272c 206e 616d  mechanisms', nam
-0000fbf0: 6573 7061 6365 3d4e 616d 6573 7061 6365  espace=Namespace
-0000fc00: 2e53 4153 4c29 0a20 2020 2020 2020 2020  .SASL).         
-0000fc10: 2020 2069 6620 6d65 6368 616e 6973 6d73     if mechanisms
-0000fc20: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000fc30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000fc40: 2073 6574 2829 0a20 2020 2020 2020 206d   set().        m
-0000fc50: 6563 6861 6e69 736d 7320 3d20 6d65 6368  echanisms = mech
-0000fc60: 616e 6973 6d73 2e67 6574 5461 6773 2827  anisms.getTags('
-0000fc70: 6d65 6368 616e 6973 6d27 290a 2020 2020  mechanism').    
-0000fc80: 2020 2020 7265 7475 726e 2073 6574 286d      return set(m
-0000fc90: 6563 682e 6765 7444 6174 6128 2920 666f  ech.getData() fo
-0000fca0: 7220 6d65 6368 2069 6e20 6d65 6368 616e  r mech in mechan
-0000fcb0: 6973 6d73 290a 0a20 2020 2064 6566 2067  isms)..    def g
-0000fcc0: 6574 5f64 6f6d 6169 6e5f 6261 7365 645f  et_domain_based_
-0000fcd0: 6e61 6d65 2873 656c 6629 3a0a 2020 2020  name(self):.    
-0000fce0: 2020 2020 686f 7374 6e61 6d65 203d 2073      hostname = s
-0000fcf0: 656c 662e 6765 7454 6167 2827 686f 7374  elf.getTag('host
-0000fd00: 6e61 6d65 272c 0a20 2020 2020 2020 2020  name',.         
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd20: 2020 2020 2020 6e61 6d65 7370 6163 653d        namespace=
-0000fd30: 4e61 6d65 7370 6163 652e 444f 4d41 494e  Namespace.DOMAIN
-0000fd40: 5f42 4153 4544 5f4e 414d 4529 0a20 2020  _BASED_NAME).   
-0000fd50: 2020 2020 2069 6620 686f 7374 6e61 6d65       if hostname
-0000fd60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000fd70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000fd80: 2068 6f73 746e 616d 652e 6765 7444 6174   hostname.getDat
-0000fd90: 6128 290a 2020 2020 2020 2020 7265 7475  a().        retu
-0000fda0: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
-0000fdb0: 2068 6173 5f62 696e 6428 7365 6c66 293a   has_bind(self):
-0000fdc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fdd0: 7365 6c66 2e67 6574 5461 6728 2762 696e  self.getTag('bin
-0000fde0: 6427 2c20 6e61 6d65 7370 6163 653d 4e61  d', namespace=Na
-0000fdf0: 6d65 7370 6163 652e 4249 4e44 2920 6973  mespace.BIND) is
-0000fe00: 206e 6f74 204e 6f6e 650a 0a20 2020 2064   not None..    d
-0000fe10: 6566 2073 6573 7369 6f6e 5f72 6571 7569  ef session_requi
-0000fe20: 7265 6428 7365 6c66 293a 0a20 2020 2020  red(self):.     
-0000fe30: 2020 2073 6573 7369 6f6e 203d 2073 656c     session = sel
-0000fe40: 662e 6765 7454 6167 2827 7365 7373 696f  f.getTag('sessio
-0000fe50: 6e27 2c20 6e61 6d65 7370 6163 653d 4e61  n', namespace=Na
-0000fe60: 6d65 7370 6163 652e 5345 5353 494f 4e29  mespace.SESSION)
-0000fe70: 0a20 2020 2020 2020 2069 6620 7365 7373  .        if sess
-0000fe80: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-0000fe90: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-0000fea0: 696f 6e61 6c20 3d20 7365 7373 696f 6e2e  ional = session.
-0000feb0: 6765 7454 6167 2827 6f70 7469 6f6e 616c  getTag('optional
-0000fec0: 2729 2069 7320 6e6f 7420 4e6f 6e65 0a20  ') is not None. 
-0000fed0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fee0: 6e20 6e6f 7420 6f70 7469 6f6e 616c 0a20  n not optional. 
-0000fef0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0000ff00: 6c73 650a 0a20 2020 2064 6566 2068 6173  lse..    def has
-0000ff10: 5f73 6d28 7365 6c66 293a 0a20 2020 2020  _sm(self):.     
-0000ff20: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-0000ff30: 6574 5461 6728 2773 6d27 2c20 6e61 6d65  etTag('sm', name
-0000ff40: 7370 6163 653d 4e61 6d65 7370 6163 652e  space=Namespace.
-0000ff50: 5354 5245 414d 5f4d 474d 5429 2069 7320  STREAM_MGMT) is 
-0000ff60: 6e6f 7420 4e6f 6e65 0a0a 2020 2020 6465  not None..    de
-0000ff70: 6620 6861 735f 726f 7374 6572 5f76 6572  f has_roster_ver
-0000ff80: 7369 6f6e 2873 656c 6629 3a0a 2020 2020  sion(self):.    
-0000ff90: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000ffa0: 6765 7454 6167 2827 7665 7227 2c20 6e61  getTag('ver', na
-0000ffb0: 6d65 7370 6163 653d 4e61 6d65 7370 6163  mespace=Namespac
-0000ffc0: 652e 524f 5354 4552 5f56 4552 2920 6973  e.ROSTER_VER) is
-0000ffd0: 206e 6f74 204e 6f6e 650a 0a20 2020 2064   not None..    d
-0000ffe0: 6566 2068 6173 5f72 6567 6973 7465 7228  ef has_register(
-0000fff0: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00010000: 6574 7572 6e20 7365 6c66 2e67 6574 5461  eturn self.getTa
-00010010: 6728 0a20 2020 2020 2020 2020 2020 2027  g(.            '
-00010020: 7265 6769 7374 6572 272c 206e 616d 6573  register', names
-00010030: 7061 6365 3d4e 616d 6573 7061 6365 2e52  pace=Namespace.R
-00010040: 4547 4953 5445 525f 4645 4154 5552 4529  EGISTER_FEATURE)
-00010050: 2069 7320 6e6f 7420 4e6f 6e65 0a0a 2020   is not None..  
-00010060: 2020 6465 6620 6861 735f 616e 6f6e 796d    def has_anonym
-00010070: 6f75 7328 7365 6c66 293a 0a20 2020 2020  ous(self):.     
-00010080: 2020 2072 6574 7572 6e20 2741 4e4f 4e59     return 'ANONY
-00010090: 4d4f 5553 2720 696e 2073 656c 662e 6765  MOUS' in self.ge
-000100a0: 745f 6d65 6368 7328 290a 0a0a 636c 6173  t_mechs()...clas
-000100b0: 7320 4572 726f 724e 6f64 6528 4e6f 6465  s ErrorNode(Node
-000100c0: 293a 0a20 2020 2022 2222 0a20 2020 2058  ):.    """.    X
-000100d0: 4d50 502d 7374 796c 6520 6572 726f 7220  MPP-style error 
-000100e0: 656c 656d 656e 740a 0a20 2020 2049 6e20  element..    In 
-000100f0: 7468 6520 6361 7365 206f 6620 7374 616e  the case of stan
-00010100: 7a61 2065 7272 6f72 2073 686f 756c 6420  za error should 
-00010110: 6265 2061 7474 6163 6865 6420 746f 2058  be attached to X
-00010120: 4d50 5020 7374 616e 7a61 2e0a 2020 2020  MPP stanza..    
-00010130: 496e 2074 6865 2063 6173 6520 6f66 2073  In the case of s
-00010140: 7472 6561 6d2d 6c65 7665 6c20 6572 726f  tream-level erro
-00010150: 7273 2073 686f 756c 6420 6265 2075 7365  rs should be use
-00010160: 6420 7365 7061 7261 7465 6c79 2e0a 2020  d separately..  
-00010170: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-00010180: 5f69 6e69 745f 5f28 7365 6c66 2c20 6e61  _init__(self, na
-00010190: 6d65 2c20 636f 6465 3d4e 6f6e 652c 2074  me, code=None, t
-000101a0: 7970 3d4e 6f6e 652c 2074 6578 743d 4e6f  yp=None, text=No
-000101b0: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
-000101c0: 0a20 2020 2020 2020 204d 616e 6461 746f  .        Mandato
-000101d0: 7279 2070 6172 616d 6574 6572 3a20 6e61  ry parameter: na
-000101e0: 6d65 202d 206e 616d 6520 6f66 2065 7272  me - name of err
-000101f0: 6f72 2063 6f6e 6469 7469 6f6e 2e0a 2020  or condition..  
-00010200: 2020 2020 2020 4f70 7469 6f6e 616c 2070        Optional p
-00010210: 6172 616d 6574 6572 733a 2063 6f64 652c  arameters: code,
-00010220: 2074 7970 2c20 7465 7874 2e0a 2020 2020   typ, text..    
-00010230: 2020 2020 5573 6564 2066 6f72 2062 6163      Used for bac
-00010240: 6b77 6172 6473 2063 6f6d 7061 7274 6962  kwards compartib
-00010250: 696c 6974 7920 7769 7468 206f 6c64 6572  ility with older
-00010260: 206a 6162 6265 7220 7072 6f74 6f63 6f6c   jabber protocol
-00010270: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00010280: 2020 2020 2020 6966 206e 616d 6520 696e        if name in
-00010290: 2045 5252 4f52 533a 0a20 2020 2020 2020   ERRORS:.       
-000102a0: 2020 2020 2063 6f64 2c20 7479 7065 5f2c       cod, type_,
-000102b0: 2074 7874 203d 2045 5252 4f52 535b 6e61   txt = ERRORS[na
-000102c0: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-000102d0: 6e73 203d 206e 616d 652e 7370 6c69 7428  ns = name.split(
-000102e0: 295b 305d 0a20 2020 2020 2020 2065 6c73  )[0].        els
-000102f0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-00010300: 6f64 2c20 6e73 2c20 7479 7065 5f2c 2074  od, ns, type_, t
-00010310: 7874 203d 2027 3530 3027 2c20 4e61 6d65  xt = '500', Name
-00010320: 7370 6163 652e 5354 414e 5a41 532c 2027  space.STANZAS, '
-00010330: 6361 6e63 656c 272c 2027 270a 2020 2020  cancel', ''.    
-00010340: 2020 2020 6966 2074 7970 3a0a 2020 2020      if typ:.    
-00010350: 2020 2020 2020 2020 7479 7065 5f20 3d20          type_ = 
-00010360: 7479 700a 2020 2020 2020 2020 6966 2063  typ.        if c
-00010370: 6f64 653a 0a20 2020 2020 2020 2020 2020  ode:.           
-00010380: 2063 6f64 203d 2063 6f64 650a 2020 2020   cod = code.    
-00010390: 2020 2020 6966 2074 6578 743a 0a20 2020      if text:.   
-000103a0: 2020 2020 2020 2020 2074 7874 203d 2074           txt = t
-000103b0: 6578 740a 2020 2020 2020 2020 4e6f 6465  ext.        Node
-000103c0: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c20  .__init__(self, 
-000103d0: 2765 7272 6f72 272c 207b 7d2c 205b 4e6f  'error', {}, [No
-000103e0: 6465 286e 616d 6529 5d29 0a20 2020 2020  de(name)]).     
-000103f0: 2020 2069 6620 7479 7065 5f3a 0a20 2020     if type_:.   
-00010400: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00010410: 7441 7474 7228 2774 7970 6527 2c20 7479  tAttr('type', ty
-00010420: 7065 5f29 0a20 2020 2020 2020 2069 6620  pe_).        if 
-00010430: 6e6f 7420 636f 643a 0a20 2020 2020 2020  not cod:.       
-00010440: 2020 2020 2073 656c 662e 7365 744e 616d       self.setNam
-00010450: 6528 2773 7472 6561 6d3a 6572 726f 7227  e('stream:error'
-00010460: 290a 2020 2020 2020 2020 6966 2074 7874  ).        if txt
-00010470: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00010480: 6c66 2e61 6464 4368 696c 6428 6e6f 6465  lf.addChild(node
-00010490: 3d4e 6f64 6528 6e73 202b 2027 2074 6578  =Node(ns + ' tex
-000104a0: 7427 2c20 7b7d 2c20 5b74 7874 5d29 290a  t', {}, [txt])).
-000104b0: 2020 2020 2020 2020 6966 2063 6f64 3a0a          if cod:.
-000104c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000104d0: 2e73 6574 4174 7472 2827 636f 6465 272c  .setAttr('code',
-000104e0: 2063 6f64 290a 0a63 6c61 7373 2045 7272   cod)..class Err
-000104f0: 6f72 2850 726f 746f 636f 6c29 3a0a 2020  or(Protocol):.  
-00010500: 2020 2222 220a 2020 2020 5573 6564 2074    """.    Used t
-00010510: 6f20 7175 6963 6b6c 7920 7472 616e 7366  o quickly transf
-00010520: 6f72 6d20 7265 6365 6976 6564 2073 7461  orm received sta
-00010530: 6e7a 6120 696e 746f 2065 7272 6f72 2072  nza into error r
-00010540: 6570 6c79 0a20 2020 2022 2222 0a0a 2020  eply.    """..  
-00010550: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00010560: 656c 662c 206e 6f64 652c 2065 7272 6f72  elf, node, error
-00010570: 2c20 7265 706c 793d 3129 3a0a 2020 2020  , reply=1):.    
-00010580: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010590: 4372 6561 7465 2065 7272 6f72 2072 6570  Create error rep
-000105a0: 6c79 2062 6173 696e 6720 6f6e 2074 6865  ly basing on the
-000105b0: 2072 6563 6569 7665 6420 276e 6f64 6527   received 'node'
-000105c0: 2073 7461 6e7a 6120 616e 6420 7468 6520   stanza and the 
-000105d0: 2765 7272 6f72 270a 2020 2020 2020 2020  'error'.        
-000105e0: 6572 726f 7220 636f 6e64 6974 696f 6e0a  error condition.
-000105f0: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
-00010600: 276e 6f64 6527 2069 7320 6e6f 7420 7468  'node' is not th
-00010610: 6520 7265 6365 6976 6564 2073 7461 6e7a  e received stanz
-00010620: 6120 6275 7420 6c6f 6361 6c6c 7920 6372  a but locally cr
-00010630: 6561 7465 6420 2827 746f 2720 616e 640a  eated ('to' and.
-00010640: 2020 2020 2020 2020 2766 726f 6d27 2066          'from' f
-00010650: 6965 6c64 7320 6e65 6564 7320 6e6f 7420  ields needs not 
-00010660: 7377 6170 7069 6e67 2920 7370 6563 6966  swapping) specif
-00010670: 7920 7468 6520 2772 6570 6c79 2720 6172  y the 'reply' ar
-00010680: 6775 6d65 6e74 2061 7320 6661 6c73 652e  gument as false.
-00010690: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000106a0: 2020 2020 2069 6620 6e6f 6465 2e67 6574       if node.get
-000106b0: 5479 7065 2829 203d 3d20 2765 7272 6f72  Type() == 'error
-000106c0: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
-000106d0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000106e0: 2743 616e e280 9974 2063 7265 6174 6520  'Can...t create 
-000106f0: 6572 726f 7220 7265 706c 7920 6672 6f6d  error reply from
-00010700: 2065 7272 6f72 2729 0a0a 2020 2020 2020   error')..      
-00010710: 2020 6966 2072 6570 6c79 3a0a 2020 2020    if reply:.    
-00010720: 2020 2020 2020 2020 5072 6f74 6f63 6f6c          Protocol
-00010730: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c0a  .__init__(self,.
-00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010750: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00010760: 3d6e 6f64 652e 6765 7446 726f 6d28 292c  =node.getFrom(),
-00010770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010780: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00010790: 6f64 653d 6e6f 6465 290a 2020 2020 2020  ode=node).      
-000107a0: 2020 2020 2020 7365 6c66 2e64 656c 4174        self.delAt
-000107b0: 7472 2827 6672 6f6d 2729 0a20 2020 2020  tr('from').     
-000107c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000107d0: 2020 2020 2050 726f 746f 636f 6c2e 5f5f       Protocol.__
-000107e0: 696e 6974 5f5f 2873 656c 662c 206e 6f64  init__(self, nod
-000107f0: 653d 6e6f 6465 290a 2020 2020 2020 2020  e=node).        
-00010800: 7365 6c66 2e73 6574 4572 726f 7228 6572  self.setError(er
-00010810: 726f 7229 0a0a 0a63 6c61 7373 2044 6174  ror)...class Dat
-00010820: 6146 6965 6c64 284e 6f64 6529 3a0a 2020  aField(Node):.  
-00010830: 2020 2222 220a 2020 2020 5468 6973 2063    """.    This c
-00010840: 6c61 7373 2069 7320 7573 6564 2069 6e20  lass is used in 
-00010850: 7468 6520 4461 7461 466f 726d 2063 6c61  the DataForm cla
-00010860: 7373 2074 6f20 6465 7363 7269 6265 2074  ss to describe t
-00010870: 6865 2073 696e 676c 6520 6461 7461 2069  he single data i
-00010880: 7465 6d0a 0a20 2020 2049 6620 796f 7520  tem..    If you 
-00010890: 6172 6520 776f 726b 696e 6720 7769 7468  are working with
-000108a0: 206a 6162 6265 723a 783a 6461 7461 2028   jabber:x:data (
-000108b0: 5845 502d 3030 3034 2c20 5845 502d 3030  XEP-0004, XEP-00
-000108c0: 3638 2c20 5845 502d 3031 3232 2920 7468  68, XEP-0122) th
-000108d0: 656e 0a20 2020 2079 6f75 2077 696c 6c20  en.    you will 
-000108e0: 6e65 6564 2074 6f20 776f 726b 2077 6974  need to work wit
-000108f0: 6820 696e 7374 616e 6365 7320 6f66 2074  h instances of t
-00010900: 6869 7320 636c 6173 732e 0a20 2020 2022  his class..    "
-00010910: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-00010920: 6974 5f5f 2873 656c 662c 0a20 2020 2020  it__(self,.     
-00010930: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00010940: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00010950: 2020 2020 2020 2020 7661 6c75 653d 4e6f          value=No
-00010960: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00010970: 2020 2020 2074 7970 3d4e 6f6e 652c 0a20       typ=None,. 
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 7265 7175 6972 6564 3d30 2c0a 2020 2020  required=0,.    
-000109a0: 2020 2020 2020 2020 2020 2020 2064 6573               des
-000109b0: 633d 4e6f 6e65 2c0a 2020 2020 2020 2020  c=None,.        
-000109c0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-000109d0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-000109e0: 2020 2020 2020 2020 6e6f 6465 3d4e 6f6e          node=Non
-000109f0: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
-00010a00: 2020 2020 2020 2020 4372 6561 7465 206e          Create n
-00010a10: 6577 2064 6174 6120 6669 656c 6420 6f66  ew data field of
-00010a20: 2073 7065 6369 6669 6564 206e 616d 652c   specified name,
-00010a30: 7661 6c75 6520 616e 6420 7479 7065 0a0a  value and type..
-00010a40: 2020 2020 2020 2020 416c 736f 2027 7265          Also 're
-00010a50: 7175 6972 6564 272c 2764 6573 6327 2061  quired','desc' a
-00010a60: 6e64 2027 6f70 7469 6f6e 7327 2066 6965  nd 'options' fie
-00010a70: 6c64 7320 6361 6e20 6265 2073 6574 2e20  lds can be set. 
-00010a80: 416c 7465 726e 6174 6976 656c 790a 2020  Alternatively.  
-00010a90: 2020 2020 2020 6f74 6865 7220 584d 4c20        other XML 
-00010aa0: 6f62 6a65 6374 2063 616e 2062 6520 7061  object can be pa
-00010ab0: 7373 6564 2069 6e20 6173 2074 6865 2027  ssed in as the '
-00010ac0: 6e6f 6465 2720 7061 7261 6d65 7465 640a  node' parameted.
-00010ad0: 2020 2020 2020 2020 746f 2072 6570 6c69          to repli
-00010ae0: 6361 7465 2069 7420 6173 2061 206e 6577  cate it as a new
-00010af0: 2064 6174 6166 696c 6564 2e0a 2020 2020   datafiled..    
-00010b00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010b10: 4e6f 6465 2e5f 5f69 6e69 745f 5f28 7365  Node.__init__(se
-00010b20: 6c66 2c20 2766 6965 6c64 272c 206e 6f64  lf, 'field', nod
-00010b30: 653d 6e6f 6465 290a 2020 2020 2020 2020  e=node).        
-00010b40: 6966 206e 616d 653a 0a20 2020 2020 2020  if name:.       
-00010b50: 2020 2020 2073 656c 662e 7365 7456 6172       self.setVar
-00010b60: 286e 616d 6529 0a20 2020 2020 2020 2069  (name).        i
-00010b70: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-00010b80: 7565 2c20 286c 6973 742c 2074 7570 6c65  ue, (list, tuple
-00010b90: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00010ba0: 7365 6c66 2e73 6574 5661 6c75 6573 2876  self.setValues(v
-00010bb0: 616c 7565 290a 2020 2020 2020 2020 656c  alue).        el
-00010bc0: 6966 2076 616c 7565 3a0a 2020 2020 2020  if value:.      
-00010bd0: 2020 2020 2020 7365 6c66 2e73 6574 5661        self.setVa
-00010be0: 6c75 6528 7661 6c75 6529 0a20 2020 2020  lue(value).     
-00010bf0: 2020 2069 6620 7479 703a 0a20 2020 2020     if typ:.     
-00010c00: 2020 2020 2020 2073 656c 662e 7365 7454         self.setT
-00010c10: 7970 6528 7479 7029 0a20 2020 2020 2020  ype(typ).       
-00010c20: 2065 6c69 6620 6e6f 7420 7479 7020 616e   elif not typ an
-00010c30: 6420 6e6f 7420 6e6f 6465 3a0a 2020 2020  d not node:.    
-00010c40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00010c50: 5479 7065 2827 7465 7874 2d73 696e 676c  Type('text-singl
-00010c60: 6527 290a 2020 2020 2020 2020 6966 2072  e').        if r
-00010c70: 6571 7569 7265 643a 0a20 2020 2020 2020  equired:.       
-00010c80: 2020 2020 2073 656c 662e 7365 7452 6571       self.setReq
-00010c90: 7569 7265 6428 7265 7175 6972 6564 290a  uired(required).
-00010ca0: 2020 2020 2020 2020 6966 2064 6573 633a          if desc:
-00010cb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010cc0: 662e 7365 7444 6573 6328 6465 7363 290a  f.setDesc(desc).
-00010cd0: 2020 2020 2020 2020 6966 206f 7074 696f          if optio
-00010ce0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00010cf0: 7365 6c66 2e73 6574 4f70 7469 6f6e 7328  self.setOptions(
-00010d00: 6f70 7469 6f6e 7329 0a0a 2020 2020 6465  options)..    de
-00010d10: 6620 7365 7452 6571 7569 7265 6428 7365  f setRequired(se
-00010d20: 6c66 2c20 7265 713d 3129 3a0a 2020 2020  lf, req=1):.    
-00010d30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010d40: 4368 616e 6765 2074 6865 2073 7461 7465  Change the state
-00010d50: 206f 6620 7468 6520 2772 6571 7569 7265   of the 'require
-00010d60: 6427 2066 6c61 670a 2020 2020 2020 2020  d' flag.        
-00010d70: 2222 220a 2020 2020 2020 2020 6966 2072  """.        if r
-00010d80: 6571 3a0a 2020 2020 2020 2020 2020 2020  eq:.            
-00010d90: 7365 6c66 2e73 6574 5461 6728 2772 6571  self.setTag('req
-00010da0: 7569 7265 6427 290a 2020 2020 2020 2020  uired').        
-00010db0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00010dc0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00010dd0: 2020 2020 2020 2073 656c 662e 6465 6c43         self.delC
-00010de0: 6869 6c64 2827 7265 7175 6972 6564 2729  hild('required')
-00010df0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00010e00: 6570 7420 5661 6c75 6545 7272 6f72 3a0a  ept ValueError:.
-00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e20: 7265 7475 726e 0a0a 2020 2020 6465 6620  return..    def 
-00010e30: 6973 5265 7175 6972 6564 2873 656c 6629  isRequired(self)
-00010e40: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010e50: 2020 2020 2020 5265 7475 726e 2069 6e20        Return in 
-00010e60: 7468 6973 2066 6965 6c64 2061 2072 6571  this field a req
-00010e70: 7569 7265 6420 6f6e 650a 2020 2020 2020  uired one.      
-00010e80: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00010e90: 7475 726e 2073 656c 662e 6765 7454 6167  turn self.getTag
-00010ea0: 2827 7265 7175 6972 6564 2729 0a0a 2020  ('required')..  
-00010eb0: 2020 6465 6620 7365 7444 6573 6328 7365    def setDesc(se
-00010ec0: 6c66 2c20 6465 7363 293a 0a20 2020 2020  lf, desc):.     
-00010ed0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00010ee0: 6574 2074 6865 2064 6573 6372 6970 7469  et the descripti
-00010ef0: 6f6e 206f 6620 7468 6973 2066 6965 6c64  on of this field
-00010f00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010f10: 2020 2020 2073 656c 662e 7365 7454 6167       self.setTag
-00010f20: 4461 7461 2827 6465 7363 272c 2064 6573  Data('desc', des
-00010f30: 6329 0a0a 2020 2020 6465 6620 6765 7444  c)..    def getD
-00010f40: 6573 6328 7365 6c66 293a 0a20 2020 2020  esc(self):.     
-00010f50: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00010f60: 6574 7572 6e20 7468 6520 6465 7363 7269  eturn the descri
-00010f70: 7074 696f 6e20 6f66 2074 6869 7320 6669  ption of this fi
-00010f80: 656c 640a 2020 2020 2020 2020 2222 220a  eld.        """.
-00010f90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00010fa0: 656c 662e 6765 7454 6167 4461 7461 2827  elf.getTagData('
-00010fb0: 6465 7363 2729 0a0a 2020 2020 6465 6620  desc')..    def 
-00010fc0: 7365 7456 616c 7565 2873 656c 662c 2076  setValue(self, v
-00010fd0: 616c 293a 0a20 2020 2020 2020 2022 2222  al):.        """
-00010fe0: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
-00010ff0: 2076 616c 7565 206f 6620 7468 6973 2066   value of this f
-00011000: 6965 6c64 0a20 2020 2020 2020 2022 2222  ield.        """
-00011010: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00011020: 7454 6167 4461 7461 2827 7661 6c75 6527  tTagData('value'
-00011030: 2c20 7661 6c29 0a0a 2020 2020 6465 6620  , val)..    def 
-00011040: 6765 7456 616c 7565 2873 656c 6629 3a0a  getValue(self):.
-00011050: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00011060: 656c 662e 6765 7454 6167 4461 7461 2827  elf.getTagData('
-00011070: 7661 6c75 6527 290a 0a20 2020 2064 6566  value')..    def
-00011080: 2073 6574 5661 6c75 6573 2873 656c 662c   setValues(self,
-00011090: 206c 7374 293a 0a20 2020 2020 2020 2022   lst):.        "
-000110a0: 2222 0a20 2020 2020 2020 2053 6574 2074  "".        Set t
-000110b0: 6865 2076 616c 7565 7320 6f66 2074 6869  he values of thi
-000110c0: 7320 6669 656c 6420 6173 2076 616c 7565  s field as value
-000110d0: 732d 6c69 7374 2e20 5265 706c 6163 6573  s-list. Replaces
-000110e0: 2061 6c6c 2070 7265 7669 6f75 7320 6669   all previous fi
-000110f0: 6c65 640a 2020 2020 2020 2020 7661 6c75  led.        valu
-00011100: 6573 2120 4966 2079 6f75 206e 6565 6420  es! If you need 
-00011110: 746f 206a 7573 7420 6164 6420 6120 7661  to just add a va
-00011120: 6c75 6520 2d20 7573 6520 6164 6456 616c  lue - use addVal
-00011130: 7565 206d 6574 686f 640a 2020 2020 2020  ue method.      
-00011140: 2020 2222 220a 2020 2020 2020 2020 7768    """.        wh
-00011150: 696c 6520 7365 6c66 2e67 6574 5461 6728  ile self.getTag(
-00011160: 2776 616c 7565 2729 3a0a 2020 2020 2020  'value'):.      
-00011170: 2020 2020 2020 7365 6c66 2e64 656c 4368        self.delCh
-00011180: 696c 6428 2776 616c 7565 2729 0a20 2020  ild('value').   
-00011190: 2020 2020 2066 6f72 2076 616c 2069 6e20       for val in 
-000111a0: 6c73 743a 0a20 2020 2020 2020 2020 2020  lst:.           
-000111b0: 2073 656c 662e 6164 6456 616c 7565 2876   self.addValue(v
-000111c0: 616c 290a 0a20 2020 2064 6566 2061 6464  al)..    def add
-000111d0: 5661 6c75 6528 7365 6c66 2c20 7661 6c29  Value(self, val)
-000111e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000111f0: 2020 2020 2020 4164 6420 6f6e 6520 6d6f        Add one mo
-00011200: 7265 2076 616c 7565 2074 6f20 7468 6973  re value to this
-00011210: 2066 6965 6c64 2e20 5573 6564 2069 6e20   field. Used in 
-00011220: 2767 6574 2720 6971 2773 206f 7220 7375  'get' iq's or su
-00011230: 6368 0a20 2020 2020 2020 2022 2222 0a20  ch.        """. 
-00011240: 2020 2020 2020 2073 656c 662e 6164 6443         self.addC
-00011250: 6869 6c64 2827 7661 6c75 6527 2c20 7b7d  hild('value', {}
-00011260: 2c20 5b76 616c 5d29 0a0a 2020 2020 6465  , [val])..    de
-00011270: 6620 6765 7456 616c 7565 7328 7365 6c66  f getValues(self
-00011280: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00011290: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-000112a0: 6520 6c69 7374 206f 6620 7661 6c75 6573  e list of values
-000112b0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000112c0: 2074 6869 7320 6669 656c 640a 2020 2020   this field.    
-000112d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000112e0: 7265 7420 3d20 5b5d 0a20 2020 2020 2020  ret = [].       
-000112f0: 2066 6f72 2074 6167 2069 6e20 7365 6c66   for tag in self
-00011300: 2e67 6574 5461 6773 2827 7661 6c75 6527  .getTags('value'
-00011310: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00011320: 6574 2e61 7070 656e 6428 7461 672e 6765  et.append(tag.ge
-00011330: 7444 6174 6128 2929 0a20 2020 2020 2020  tData()).       
-00011340: 2072 6574 7572 6e20 7265 740a 0a20 2020   return ret..   
-00011350: 2064 6566 2067 6574 4f70 7469 6f6e 7328   def getOptions(
-00011360: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00011370: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00011380: 6e20 6c61 6265 6c2d 6f70 7469 6f6e 2070  n label-option p
-00011390: 6169 7273 206c 6973 7420 6173 736f 6369  airs list associ
-000113a0: 6174 6564 2077 6974 6820 7468 6973 2066  ated with this f
-000113b0: 6965 6c64 0a20 2020 2020 2020 2022 2222  ield.        """
-000113c0: 0a20 2020 2020 2020 2072 6574 203d 205b  .        ret = [
-000113d0: 5d0a 2020 2020 2020 2020 666f 7220 7461  ].        for ta
-000113e0: 6720 696e 2073 656c 662e 6765 7454 6167  g in self.getTag
-000113f0: 7328 276f 7074 696f 6e27 293a 0a20 2020  s('option'):.   
-00011400: 2020 2020 2020 2020 2072 6574 2e61 7070           ret.app
-00011410: 656e 6428 5b74 6167 2e67 6574 4174 7472  end([tag.getAttr
-00011420: 2827 6c61 6265 6c27 292c 2074 6167 2e67  ('label'), tag.g
-00011430: 6574 5461 6744 6174 6128 2776 616c 7565  etTagData('value
-00011440: 2729 5d29 0a20 2020 2020 2020 2072 6574  ')]).        ret
-00011450: 7572 6e20 7265 740a 0a20 2020 2064 6566  urn ret..    def
-00011460: 2073 6574 4f70 7469 6f6e 7328 7365 6c66   setOptions(self
-00011470: 2c20 6c73 7429 3a0a 2020 2020 2020 2020  , lst):.        
-00011480: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
-00011490: 6c61 6265 6c2d 6f70 7469 6f6e 2070 6169  label-option pai
-000114a0: 7273 206c 6973 7420 6173 736f 6369 6174  rs list associat
-000114b0: 6564 2077 6974 6820 7468 6973 2066 6965  ed with this fie
-000114c0: 6c64 0a20 2020 2020 2020 2022 2222 0a20  ld.        """. 
-000114d0: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
-000114e0: 662e 6765 7454 6167 2827 6f70 7469 6f6e  f.getTag('option
-000114f0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-00011500: 7365 6c66 2e64 656c 4368 696c 6428 276f  self.delChild('o
-00011510: 7074 696f 6e27 290a 2020 2020 2020 2020  ption').        
-00011520: 666f 7220 6f70 7420 696e 206c 7374 3a0a  for opt in lst:.
-00011530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011540: 2e61 6464 4f70 7469 6f6e 286f 7074 290a  .addOption(opt).
-00011550: 0a20 2020 2064 6566 2061 6464 4f70 7469  .    def addOpti
-00011560: 6f6e 2873 656c 662c 206f 7074 293a 0a20  on(self, opt):. 
-00011570: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011580: 2020 2041 6464 206f 6e65 206d 6f72 6520     Add one more 
-00011590: 6c61 6265 6c2d 6f70 7469 6f6e 2070 6169  label-option pai
-000115a0: 7220 746f 2074 6869 7320 6669 656c 640a  r to this field.
-000115b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000115c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000115d0: 6528 6f70 742c 206c 6973 7429 3a0a 2020  e(opt, list):.  
-000115e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000115f0: 6464 4368 696c 6428 276f 7074 696f 6e27  ddChild('option'
-00011600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011610: 2020 2020 2020 2020 2020 2020 7b27 6c61              {'la
-00011620: 6265 6c27 3a20 6f70 745b 305d 7d29 2e73  bel': opt[0]}).s
-00011630: 6574 5461 6744 6174 6128 2776 616c 7565  etTagData('value
-00011640: 272c 206f 7074 5b31 5d29 0a20 2020 2020  ', opt[1]).     
-00011650: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00011660: 2020 2020 2073 656c 662e 6164 6443 6869       self.addChi
-00011670: 6c64 2827 6f70 7469 6f6e 2729 2e73 6574  ld('option').set
-00011680: 5461 6744 6174 6128 2776 616c 7565 272c  TagData('value',
-00011690: 206f 7074 290a 0a20 2020 2064 6566 2067   opt)..    def g
-000116a0: 6574 5479 7065 2873 656c 6629 3a0a 2020  etType(self):.  
-000116b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000116c0: 2020 4765 7420 7479 7065 206f 6620 7468    Get type of th
-000116d0: 6973 2066 6965 6c64 0a20 2020 2020 2020  is field.       
-000116e0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000116f0: 7572 6e20 7365 6c66 2e67 6574 4174 7472  urn self.getAttr
-00011700: 2827 7479 7065 2729 0a0a 2020 2020 6465  ('type')..    de
-00011710: 6620 7365 7454 7970 6528 7365 6c66 2c20  f setType(self, 
-00011720: 7661 6c29 3a0a 2020 2020 2020 2020 2222  val):.        ""
-00011730: 220a 2020 2020 2020 2020 5365 7420 7479  ".        Set ty
-00011740: 7065 206f 6620 7468 6973 2066 6965 6c64  pe of this field
-00011750: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011760: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00011770: 2e73 6574 4174 7472 2827 7479 7065 272c  .setAttr('type',
-00011780: 2076 616c 290a 0a20 2020 2064 6566 2067   val)..    def g
-00011790: 6574 5661 7228 7365 6c66 293a 0a20 2020  etVar(self):.   
-000117a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000117b0: 2047 6574 2027 7661 7227 2061 7474 7269   Get 'var' attri
-000117c0: 6275 7465 2076 616c 7565 206f 6620 7468  bute value of th
-000117d0: 6973 2066 6965 6c64 0a20 2020 2020 2020  is field.       
-000117e0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000117f0: 7572 6e20 7365 6c66 2e67 6574 4174 7472  urn self.getAttr
-00011800: 2827 7661 7227 290a 0a20 2020 2064 6566  ('var')..    def
-00011810: 2073 6574 5661 7228 7365 6c66 2c20 7661   setVar(self, va
-00011820: 6c29 3a0a 2020 2020 2020 2020 2222 220a  l):.        """.
-00011830: 2020 2020 2020 2020 5365 7420 2776 6172          Set 'var
-00011840: 2720 6174 7472 6962 7574 6520 7661 6c75  ' attribute valu
-00011850: 6520 6f66 2074 6869 7320 6669 656c 640a  e of this field.
-00011860: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011870: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011880: 7365 7441 7474 7228 2776 6172 272c 2076  setAttr('var', v
-00011890: 616c 290a 0a63 6c61 7373 2044 6174 6146  al)..class DataF
-000118a0: 6f72 6d28 4e6f 6465 293a 0a20 2020 2022  orm(Node):.    "
-000118b0: 2222 0a20 2020 2055 7365 6420 666f 7220  "".    Used for 
-000118c0: 6d61 6e69 7075 6c61 7469 6e67 2064 6174  manipulating dat
-000118d0: 6166 6f72 6d73 2069 6e20 584d 5050 0a0a  aforms in XMPP..
-000118e0: 2020 2020 5265 6c65 7661 6e74 2058 4550      Relevant XEP
-000118f0: 733a 2030 3030 342c 2030 3036 382c 2030  s: 0004, 0068, 0
-00011900: 3132 322e 2043 616e 2062 6520 7573 6564  122. Can be used
-00011910: 2069 6e20 6469 7363 6f2c 2070 7562 2d73   in disco, pub-s
-00011920: 7562 2061 6e64 206d 616e 790a 2020 2020  ub and many.    
-00011930: 6f74 6865 7220 6170 706c 6963 6174 696f  other applicatio
-00011940: 6e73 2e0a 2020 2020 2222 220a 2020 2020  ns..    """.    
-00011950: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00011960: 662c 2074 7970 3d4e 6f6e 652c 2064 6174  f, typ=None, dat
-00011970: 613d 4e6f 6e65 2c20 7469 746c 653d 4e6f  a=None, title=No
-00011980: 6e65 2c20 6e6f 6465 3d4e 6f6e 6529 3a0a  ne, node=None):.
-00011990: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000119a0: 2020 2020 4372 6561 7465 206e 6577 2064      Create new d
-000119b0: 6174 6166 6f72 6d20 6f66 2074 7970 6520  ataform of type 
-000119c0: 2774 7970 272e 2027 6461 7461 2720 6973  'typ'. 'data' is
-000119d0: 2074 6865 206c 6973 7420 6f66 2044 6174   the list of Dat
-000119e0: 6146 6965 6c64 0a20 2020 2020 2020 2069  aField.        i
-000119f0: 6e73 7461 6e63 6573 2074 6861 7420 7468  nstances that th
-00011a00: 6973 2064 6174 6166 6f72 6d20 636f 6e74  is dataform cont
-00011a10: 6169 6e73 2c20 2774 6974 6c65 2720 2d20  ains, 'title' - 
-00011a20: 7468 6520 7469 746c 6520 7374 7269 6e67  the title string
-00011a30: 2e20 2059 6f75 0a20 2020 2020 2020 2063  .  You.        c
-00011a40: 616e 2073 7065 6369 6679 2074 6865 2027  an specify the '
-00011a50: 6e6f 6465 2720 6172 6775 6d65 6e74 2061  node' argument a
-00011a60: 7320 7468 6520 6f74 6865 7220 6e6f 6465  s the other node
-00011a70: 2074 6f20 6265 2075 7365 6420 6173 2062   to be used as b
-00011a80: 6173 6520 666f 720a 2020 2020 2020 2020  ase for.        
-00011a90: 636f 6e73 7472 7563 7469 6e67 2074 6869  constructing thi
-00011aa0: 7320 6461 7461 666f 726d 0a0a 2020 2020  s dataform..    
-00011ab0: 2020 2020 7469 746c 6520 616e 6420 696e      title and in
-00011ac0: 7374 7275 6374 696f 6e73 2069 7320 6f70  structions is op
-00011ad0: 7469 6f6e 616c 2061 6e64 2053 484f 554c  tional and SHOUL
-00011ae0: 4420 4e4f 5420 636f 6e74 6169 6e20 6e65  D NOT contain ne
-00011af0: 776c 696e 6573 2e0a 2020 2020 2020 2020  wlines..        
-00011b00: 5365 7665 7261 6c20 696e 7374 7275 6374  Several instruct
-00011b10: 696f 6e73 204d 4159 2062 6520 7072 6573  ions MAY be pres
-00011b20: 656e 742e 0a20 2020 2020 2020 2027 7479  ent..        'ty
-00011b30: 7027 2063 616e 2062 6520 6f6e 6520 6f66  p' can be one of
-00011b40: 2028 2766 6f72 6d27 207c 2027 7375 626d   ('form' | 'subm
-00011b50: 6974 2720 7c20 2763 616e 6365 6c27 207c  it' | 'cancel' |
-00011b60: 2027 7265 7375 6c74 2720 290a 2020 2020   'result' ).    
-00011b70: 2020 2020 2774 7970 2720 6f66 2072 6570      'typ' of rep
-00011b80: 6c79 2069 7120 6361 6e20 6265 2028 2027  ly iq can be ( '
-00011b90: 7265 7375 6c74 2720 7c20 2773 6574 2720  result' | 'set' 
-00011ba0: 7c20 2773 6574 2720 7c20 2772 6573 756c  | 'set' | 'resul
-00011bb0: 7427 2029 0a20 2020 2020 2020 2020 2020  t' ).           
-00011bc0: 2072 6573 7065 6374 6976 656c 792e 0a20   respectively.. 
-00011bd0: 2020 2020 2020 2027 6361 6e63 656c 2720         'cancel' 
-00011be0: 666f 726d 2063 616e 206e 6f74 2063 6f6e  form can not con
-00011bf0: 7461 696e 2061 6e79 2066 6965 6c64 732e  tain any fields.
-00011c00: 2041 6c6c 206f 7468 6572 2066 6f72 6d73   All other forms
-00011c10: 2063 6f6e 7461 696e 730a 2020 2020 2020   contains.      
-00011c20: 2020 2020 2020 4154 204c 4541 5354 206f        AT LEAST o
-00011c30: 6e65 2066 6965 6c64 2e0a 2020 2020 2020  ne field..      
-00011c40: 2020 2774 6974 6c65 2720 4d41 5920 6265    'title' MAY be
-00011c50: 2069 6e63 6c75 6465 6420 696e 2066 6f72   included in for
-00011c60: 6d73 206f 6620 7479 7065 2022 666f 726d  ms of type "form
-00011c70: 2220 616e 6420 2272 6573 756c 7422 0a20  " and "result". 
-00011c80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011c90: 2020 204e 6f64 652e 5f5f 696e 6974 5f5f     Node.__init__
-00011ca0: 2873 656c 662c 2027 7827 2c20 6e6f 6465  (self, 'x', node
-00011cb0: 3d6e 6f64 6529 0a20 2020 2020 2020 2069  =node).        i
-00011cc0: 6620 6e6f 6465 3a0a 2020 2020 2020 2020  f node:.        
-00011cd0: 2020 2020 6e65 776b 6964 7320 3d20 5b5d      newkids = []
-00011ce0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00011cf0: 206e 2069 6e20 7365 6c66 2e67 6574 4368   n in self.getCh
-00011d00: 696c 6472 656e 2829 3a0a 2020 2020 2020  ildren():.      
-00011d10: 2020 2020 2020 2020 2020 6966 206e 2e67            if n.g
-00011d20: 6574 4e61 6d65 2829 203d 3d20 2766 6965  etName() == 'fie
-00011d30: 6c64 273a 0a20 2020 2020 2020 2020 2020  ld':.           
-00011d40: 2020 2020 2020 2020 206e 6577 6b69 6473           newkids
-00011d50: 2e61 7070 656e 6428 4461 7461 4669 656c  .append(DataFiel
-00011d60: 6428 6e6f 6465 3d6e 2929 0a20 2020 2020  d(node=n)).     
-00011d70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00011d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d90: 2020 2020 206e 6577 6b69 6473 2e61 7070       newkids.app
-00011da0: 656e 6428 6e29 0a20 2020 2020 2020 2020  end(n).         
-00011db0: 2020 2073 656c 662e 6b69 6473 203d 206e     self.kids = n
-00011dc0: 6577 6b69 6473 0a20 2020 2020 2020 2069  ewkids.        i
-00011dd0: 6620 7479 703a 0a20 2020 2020 2020 2020  f typ:.         
-00011de0: 2020 2073 656c 662e 7365 7454 7970 6528     self.setType(
-00011df0: 7479 7029 0a20 2020 2020 2020 2073 656c  typ).        sel
-00011e00: 662e 7365 744e 616d 6573 7061 6365 284e  f.setNamespace(N
-00011e10: 616d 6573 7061 6365 2e44 4154 4129 0a20  amespace.DATA). 
-00011e20: 2020 2020 2020 2069 6620 7469 746c 653a         if title:
-00011e30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011e40: 662e 7365 7454 6974 6c65 2874 6974 6c65  f.setTitle(title
-00011e50: 290a 2020 2020 2020 2020 6966 2064 6174  ).        if dat
-00011e60: 6120 6973 206e 6f74 204e 6f6e 653a 0a20  a is not None:. 
-00011e70: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00011e80: 696e 7374 616e 6365 2864 6174 612c 2064  instance(data, d
-00011e90: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
-00011ea0: 2020 2020 2020 6e65 7764 6174 6120 3d20        newdata = 
-00011eb0: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-00011ec0: 2020 2066 6f72 206e 616d 6520 696e 2064     for name in d
-00011ed0: 6174 612e 6b65 7973 2829 3a0a 2020 2020  ata.keys():.    
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 6e65 7764 6174 612e 6170 7065 6e64 2844  newdata.append(D
-00011f00: 6174 6146 6965 6c64 286e 616d 652c 2064  ataField(name, d
-00011f10: 6174 615b 6e61 6d65 5d29 290a 2020 2020  ata[name])).    
-00011f20: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00011f30: 203d 206e 6577 6461 7461 0a20 2020 2020   = newdata.     
-00011f40: 2020 2020 2020 2066 6f72 2063 6869 6c64         for child
-00011f50: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
-00011f60: 2020 2020 2020 2020 2020 6966 2063 6869            if chi
-00011f70: 6c64 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  ld.__class__.__n
-00011f80: 616d 655f 5f20 3d3d 2027 4461 7461 4669  ame__ == 'DataFi
-00011f90: 656c 6427 3a0a 2020 2020 2020 2020 2020  eld':.          
-00011fa0: 2020 2020 2020 2020 2020 7365 6c66 2e6b            self.k
-00011fb0: 6964 732e 6170 7065 6e64 2863 6869 6c64  ids.append(child
-00011fc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011fd0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00011fe0: 6528 6368 696c 642c 204e 6f64 6529 3a0a  e(child, Node):.
-00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012000: 2020 2020 7365 6c66 2e6b 6964 732e 6170      self.kids.ap
-00012010: 7065 6e64 2844 6174 6146 6965 6c64 286e  pend(DataField(n
-00012020: 6f64 653d 6368 696c 6429 290a 2020 2020  ode=child)).    
-00012030: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00012040: 3a20 2023 204d 7573 7420 6265 2061 2073  :  # Must be a s
-00012050: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00012060: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00012070: 6464 496e 7374 7275 6374 696f 6e73 2863  ddInstructions(c
-00012080: 6869 6c64 290a 0a20 2020 2064 6566 2067  hild)..    def g
-00012090: 6574 5479 7065 2873 656c 6629 3a0a 2020  etType(self):.  
-000120a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000120b0: 2020 5265 7475 726e 2074 6865 2074 7970    Return the typ
-000120c0: 6520 6f66 2064 6174 6166 6f72 6d0a 2020  e of dataform.  
-000120d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000120e0: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
-000120f0: 7441 7474 7228 2774 7970 6527 290a 0a20  tAttr('type').. 
-00012100: 2020 2064 6566 2073 6574 5479 7065 2873     def setType(s
-00012110: 656c 662c 2074 7970 293a 0a20 2020 2020  elf, typ):.     
-00012120: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00012130: 6574 2074 6865 2074 7970 6520 6f66 2064  et the type of d
-00012140: 6174 6166 6f72 6d0a 2020 2020 2020 2020  ataform.        
-00012150: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00012160: 2e73 6574 4174 7472 2827 7479 7065 272c  .setAttr('type',
-00012170: 2074 7970 290a 0a20 2020 2064 6566 2067   typ)..    def g
-00012180: 6574 5469 746c 6528 7365 6c66 293a 0a20  etTitle(self):. 
-00012190: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000121a0: 2020 2052 6574 7572 6e20 7468 6520 7469     Return the ti
-000121b0: 746c 6520 6f66 2064 6174 6166 6f72 6d0a  tle of dataform.
-000121c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000121d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000121e0: 6765 7454 6167 4461 7461 2827 7469 746c  getTagData('titl
-000121f0: 6527 290a 0a20 2020 2064 6566 2073 6574  e')..    def set
-00012200: 5469 746c 6528 7365 6c66 2c20 7465 7874  Title(self, text
-00012210: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00012220: 2020 2020 2020 2053 6574 2074 6865 2074         Set the t
-00012230: 6974 6c65 206f 6620 6461 7461 666f 726d  itle of dataform
-00012240: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012250: 2020 2020 2073 656c 662e 7365 7454 6167       self.setTag
-00012260: 4461 7461 2827 7469 746c 6527 2c20 7465  Data('title', te
-00012270: 7874 290a 0a20 2020 2064 6566 2067 6574  xt)..    def get
-00012280: 496e 7374 7275 6374 696f 6e73 2873 656c  Instructions(sel
-00012290: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000122a0: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-000122b0: 6865 2069 6e73 7472 7563 7469 6f6e 7320  he instructions 
-000122c0: 6f66 2064 6174 6166 6f72 6d0a 2020 2020  of dataform.    
-000122d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000122e0: 7265 7475 726e 2073 656c 662e 6765 7454  return self.getT
-000122f0: 6167 4461 7461 2827 696e 7374 7275 6374  agData('instruct
-00012300: 696f 6e73 2729 0a0a 2020 2020 6465 6620  ions')..    def 
-00012310: 7365 7449 6e73 7472 7563 7469 6f6e 7328  setInstructions(
-00012320: 7365 6c66 2c20 7465 7874 293a 0a20 2020  self, text):.   
-00012330: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012340: 2053 6574 2074 6865 2069 6e73 7472 7563   Set the instruc
-00012350: 7469 6f6e 7320 6f66 2064 6174 6166 6f72  tions of datafor
-00012360: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
-00012370: 2020 2020 2020 7365 6c66 2e73 6574 5461        self.setTa
-00012380: 6744 6174 6128 2769 6e73 7472 7563 7469  gData('instructi
-00012390: 6f6e 7327 2c20 7465 7874 290a 0a20 2020  ons', text)..   
-000123a0: 2064 6566 2061 6464 496e 7374 7275 6374   def addInstruct
-000123b0: 696f 6e73 2873 656c 662c 2074 6578 7429  ions(self, text)
-000123c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000123d0: 2020 2020 2020 4164 6420 6f6e 6520 6d6f        Add one mo
-000123e0: 7265 2069 6e73 7472 7563 7469 6f6e 2074  re instruction t
-000123f0: 6f20 7468 6520 6461 7461 666f 726d 0a20  o the dataform. 
-00012400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012410: 2020 2073 656c 662e 6164 6443 6869 6c64     self.addChild
-00012420: 2827 696e 7374 7275 6374 696f 6e73 272c  ('instructions',
-00012430: 207b 7d2c 205b 7465 7874 5d29 0a0a 2020   {}, [text])..  
-00012440: 2020 6465 6620 6765 7446 6965 6c64 2873    def getField(s
-00012450: 656c 662c 206e 616d 6529 3a0a 2020 2020  elf, name):.    
-00012460: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012470: 5265 7475 726e 2074 6865 2064 6174 6166  Return the dataf
-00012480: 6965 6c64 206f 626a 6563 7420 7769 7468  ield object with
-00012490: 206e 616d 6520 276e 616d 6527 2028 6966   name 'name' (if
-000124a0: 2065 7869 7374 7329 0a20 2020 2020 2020   exists).       
-000124b0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000124c0: 7572 6e20 7365 6c66 2e67 6574 5461 6728  urn self.getTag(
-000124d0: 2766 6965 6c64 272c 2061 7474 7273 3d7b  'field', attrs={
-000124e0: 2776 6172 273a 206e 616d 657d 290a 0a20  'var': name}).. 
-000124f0: 2020 2064 6566 2073 6574 4669 656c 6428     def setField(
-00012500: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
-00012510: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012520: 2043 7265 6174 6520 6966 206e 6573 7365   Create if nesse
-00012530: 7373 6172 7920 6f72 2067 6574 2074 6865  ssary or get the
-00012540: 2065 7869 7374 696e 6720 6461 7461 6669   existing datafi
-00012550: 656c 6420 6f62 6a65 6374 2077 6974 6820  eld object with 
-00012560: 6e61 6d65 0a20 2020 2020 2020 2027 6e61  name.        'na
-00012570: 6d65 2720 616e 6420 7265 7475 726e 2069  me' and return i
-00012580: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-00012590: 2020 2020 2020 6620 3d20 7365 6c66 2e67        f = self.g
-000125a0: 6574 4669 656c 6428 6e61 6d65 290a 2020  etField(name).  
-000125b0: 2020 2020 2020 6966 2066 3a0a 2020 2020        if f:.    
-000125c0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-000125d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000125e0: 7365 6c66 2e61 6464 4368 696c 6428 6e6f  self.addChild(no
-000125f0: 6465 3d44 6174 6146 6965 6c64 286e 616d  de=DataField(nam
-00012600: 6529 290a 0a20 2020 2064 6566 2061 7344  e))..    def asD
-00012610: 6963 7428 7365 6c66 293a 0a20 2020 2020  ict(self):.     
-00012620: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00012630: 6570 7265 7365 6e74 2064 6174 6166 6f72  epresent datafor
-00012640: 6d20 6173 2073 696d 706c 6520 6469 6374  m as simple dict
-00012650: 696f 6e61 7279 206d 6170 7069 6e67 206f  ionary mapping o
-00012660: 6620 6461 7461 6669 656c 6420 6e61 6d65  f datafield name
-00012670: 7320 746f 0a20 2020 2020 2020 2074 6865  s to.        the
-00012680: 6972 2076 616c 7565 730a 2020 2020 2020  ir values.      
-00012690: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-000126a0: 7420 3d20 7b7d 0a20 2020 2020 2020 2066  t = {}.        f
-000126b0: 6f72 2066 6965 6c64 2069 6e20 7365 6c66  or field in self
-000126c0: 2e67 6574 5461 6773 2827 6669 656c 6427  .getTags('field'
-000126d0: 293a 0a20 2020 2020 2020 2020 2020 206e  ):.            n
-000126e0: 616d 6520 3d20 6669 656c 642e 6765 7441  ame = field.getA
-000126f0: 7474 7228 2776 6172 2729 0a20 2020 2020  ttr('var').     
-00012700: 2020 2020 2020 2074 7970 203d 2066 6965         typ = fie
-00012710: 6c64 2e67 6574 5479 7065 2829 0a20 2020  ld.getType().   
-00012720: 2020 2020 2020 2020 2069 6620 7479 7020           if typ 
-00012730: 616e 6420 7479 702e 656e 6473 7769 7468  and typ.endswith
-00012740: 2827 2d6d 756c 7469 2729 3a0a 2020 2020  ('-multi'):.    
-00012750: 2020 2020 2020 2020 2020 2020 7661 6c20              val 
-00012760: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00012770: 2020 2020 2066 6f72 2069 2069 6e20 6669       for i in fi
-00012780: 656c 642e 6765 7454 6167 7328 2776 616c  eld.getTags('val
-00012790: 7565 2729 3a0a 2020 2020 2020 2020 2020  ue'):.          
-000127a0: 2020 2020 2020 2020 2020 7661 6c2e 6170            val.ap
-000127b0: 7065 6e64 2869 2e67 6574 4461 7461 2829  pend(i.getData()
-000127c0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000127d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000127e0: 2020 2020 7661 6c20 3d20 6669 656c 642e      val = field.
-000127f0: 6765 7454 6167 4461 7461 2827 7661 6c75  getTagData('valu
-00012800: 6527 290a 2020 2020 2020 2020 2020 2020  e').            
-00012810: 7265 745b 6e61 6d65 5d20 3d20 7661 6c0a  ret[name] = val.
-00012820: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00012830: 6765 7454 6167 2827 696e 7374 7275 6374  getTag('instruct
-00012840: 696f 6e73 2729 3a0a 2020 2020 2020 2020  ions'):.        
-00012850: 2020 2020 7265 745b 2769 6e73 7472 7563      ret['instruc
-00012860: 7469 6f6e 7327 5d20 3d20 7365 6c66 2e67  tions'] = self.g
-00012870: 6574 496e 7374 7275 6374 696f 6e73 2829  etInstructions()
-00012880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012890: 7265 740a 0a20 2020 2064 6566 205f 5f67  ret..    def __g
-000128a0: 6574 6974 656d 5f5f 2873 656c 662c 206e  etitem__(self, n
-000128b0: 616d 6529 3a0a 2020 2020 2020 2020 2222  ame):.        ""
-000128c0: 220a 2020 2020 2020 2020 5369 6d70 6c65  ".        Simple
-000128d0: 2064 6963 7469 6f6e 6172 7920 696e 7465   dictionary inte
-000128e0: 7266 6163 6520 666f 7220 6765 7474 696e  rface for gettin
-000128f0: 6720 6461 7461 6669 656c 6473 2076 616c  g datafields val
-00012900: 7565 7320 6279 2074 6865 6972 206e 616d  ues by their nam
-00012910: 6573 0a20 2020 2020 2020 2022 2222 0a20  es.        """. 
-00012920: 2020 2020 2020 2069 7465 6d20 3d20 7365         item = se
-00012930: 6c66 2e67 6574 4669 656c 6428 6e61 6d65  lf.getField(name
-00012940: 290a 2020 2020 2020 2020 6966 2069 7465  ).        if ite
-00012950: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
-00012960: 6574 7572 6e20 6974 656d 2e67 6574 5661  eturn item.getVa
-00012970: 6c75 6528 290a 2020 2020 2020 2020 7261  lue().        ra
-00012980: 6973 6520 496e 6465 7845 7272 6f72 2827  ise IndexError('
-00012990: 4e6f 2073 7563 6820 6669 656c 6427 290a  No such field').
-000129a0: 0a20 2020 2064 6566 205f 5f73 6574 6974  .    def __setit
-000129b0: 656d 5f5f 2873 656c 662c 206e 616d 652c  em__(self, name,
-000129c0: 2076 616c 293a 0a20 2020 2020 2020 2022   val):.        "
-000129d0: 2222 0a20 2020 2020 2020 2053 696d 706c  "".        Simpl
-000129e0: 6520 6469 6374 696f 6e61 7279 2069 6e74  e dictionary int
-000129f0: 6572 6661 6365 2066 6f72 2073 6574 7469  erface for setti
-00012a00: 6e67 2064 6174 6166 6965 6c64 7320 7661  ng datafields va
-00012a10: 6c75 6573 2062 7920 7468 6569 7220 6e61  lues by their na
-00012a20: 6d65 730a 2020 2020 2020 2020 2222 220a  mes.        """.
-00012a30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00012a40: 656c 662e 7365 7446 6965 6c64 286e 616d  elf.setField(nam
-00012a50: 6529 2e73 6574 5661 6c75 6528 7661 6c29  e).setValue(val)
-00012a60: 0a                                       .
+0000f860: 2020 7461 673d 276f 7065 6e27 2c0a 2020    tag='open',.  
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 2020 2020 6174 7472 733d 7b27 786d 6c6e      attrs={'xmln
+0000f890: 7327 3a20 4e61 6d65 7370 6163 652e 4652  s': Namespace.FR
+0000f8a0: 414d 494e 472c 0a20 2020 2020 2020 2020  AMING,.         
+0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8c0: 2020 2020 2776 6572 7369 6f6e 273a 2027      'version': '
+0000f8d0: 312e 3027 2c0a 2020 2020 2020 2020 2020  1.0',.          
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 2020 2027 746f 273a 2064 6f6d 6169 6e2c     'to': domain,
+0000f900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2778                'x
+0000f920: 6d6c 3a6c 616e 6727 3a20 6c61 6e67 7d29  ml:lang': lang})
+0000f930: 0a0a 636c 6173 7320 5765 6273 6f63 6b65  ..class Websocke
+0000f940: 7443 6c6f 7365 4865 6164 6572 284e 6f64  tCloseHeader(Nod
+0000f950: 6529 3a0a 2020 2020 6465 6620 5f5f 696e  e):.    def __in
+0000f960: 6974 5f5f 2873 656c 6629 3a0a 2020 2020  it__(self):.    
+0000f970: 2020 2020 4e6f 6465 2e5f 5f69 6e69 745f      Node.__init_
+0000f980: 5f28 7365 6c66 2c20 7461 673d 2763 6c6f  _(self, tag='clo
+0000f990: 7365 272c 2061 7474 7273 3d7b 2778 6d6c  se', attrs={'xml
+0000f9a0: 6e73 273a 204e 616d 6573 7061 6365 2e46  ns': Namespace.F
+0000f9b0: 5241 4d49 4e47 7d29 0a0a 0a63 6c61 7373  RAMING})...class
+0000f9c0: 2046 6561 7475 7265 7328 4e6f 6465 293a   Features(Node):
+0000f9d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000f9e0: 5f28 7365 6c66 2c20 6e6f 6465 3a20 4e6f  _(self, node: No
+0000f9f0: 6465 293a 0a20 2020 2020 2020 204e 6f64  de):.        Nod
+0000fa00: 652e 5f5f 696e 6974 5f5f 2873 656c 662c  e.__init__(self,
+0000fa10: 206e 6f64 653d 6e6f 6465 290a 0a20 2020   node=node)..   
+0000fa20: 2064 6566 2068 6173 5f73 7461 7274 746c   def has_starttl
+0000fa30: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0000fa40: 2074 6c73 203d 2073 656c 662e 6765 7454   tls = self.getT
+0000fa50: 6167 2827 7374 6172 7474 6c73 272c 206e  ag('starttls', n
+0000fa60: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
+0000fa70: 6365 2e54 4c53 290a 2020 2020 2020 2020  ce.TLS).        
+0000fa80: 6966 2074 6c73 2069 7320 6e6f 7420 4e6f  if tls is not No
+0000fa90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000faa0: 7265 7175 6972 6564 203d 2074 6c73 2e67  required = tls.g
+0000fab0: 6574 5461 6728 2772 6571 7569 7265 6427  etTag('required'
+0000fac0: 2920 6973 206e 6f74 204e 6f6e 650a 2020  ) is not None.  
+0000fad0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000fae0: 2054 7275 652c 2072 6571 7569 7265 640a   True, required.
+0000faf0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0000fb00: 616c 7365 2c20 4661 6c73 650a 0a20 2020  alse, False..   
+0000fb10: 2064 6566 2068 6173 5f73 6173 6c28 7365   def has_sasl(se
+0000fb20: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0000fb30: 7572 6e20 7365 6c66 2e67 6574 5461 6728  urn self.getTag(
+0000fb40: 276d 6563 6861 6e69 736d 7327 2c20 6e61  'mechanisms', na
+0000fb50: 6d65 7370 6163 653d 4e61 6d65 7370 6163  mespace=Namespac
+0000fb60: 652e 5341 534c 2920 6973 206e 6f74 204e  e.SASL) is not N
+0000fb70: 6f6e 650a 0a20 2020 2064 6566 2068 6173  one..    def has
+0000fb80: 5f73 6173 6c5f 3228 7365 6c66 293a 0a20  _sasl_2(self):. 
+0000fb90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000fba0: 6c66 2e67 6574 5461 6728 276d 6563 6861  lf.getTag('mecha
+0000fbb0: 6e69 736d 7327 2c20 6e61 6d65 7370 6163  nisms', namespac
+0000fbc0: 653d 4e61 6d65 7370 6163 652e 5341 534c  e=Namespace.SASL
+0000fbd0: 3229 2069 7320 6e6f 7420 4e6f 6e65 0a0a  2) is not None..
+0000fbe0: 2020 2020 6465 6620 6765 745f 6d65 6368      def get_mech
+0000fbf0: 7328 7365 6c66 2920 2d3e 2073 6574 5b73  s(self) -> set[s
+0000fc00: 7472 5d3a 0a20 2020 2020 2020 206d 6563  tr]:.        mec
+0000fc10: 6861 6e69 736d 7320 3d20 7365 6c66 2e67  hanisms = self.g
+0000fc20: 6574 5461 6728 276d 6563 6861 6e69 736d  etTag('mechanism
+0000fc30: 7327 2c20 6e61 6d65 7370 6163 653d 4e61  s', namespace=Na
+0000fc40: 6d65 7370 6163 652e 5341 534c 3229 0a20  mespace.SASL2). 
+0000fc50: 2020 2020 2020 2069 6620 6d65 6368 616e         if mechan
+0000fc60: 6973 6d73 2069 7320 4e6f 6e65 3a0a 2020  isms is None:.  
+0000fc70: 2020 2020 2020 2020 2020 6d65 6368 616e            mechan
+0000fc80: 6973 6d73 203d 2073 656c 662e 6765 7454  isms = self.getT
+0000fc90: 6167 2827 6d65 6368 616e 6973 6d73 272c  ag('mechanisms',
+0000fca0: 206e 616d 6573 7061 6365 3d4e 616d 6573   namespace=Names
+0000fcb0: 7061 6365 2e53 4153 4c29 0a20 2020 2020  pace.SASL).     
+0000fcc0: 2020 2020 2020 2069 6620 6d65 6368 616e         if mechan
+0000fcd0: 6973 6d73 2069 7320 4e6f 6e65 3a0a 2020  isms is None:.  
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000fcf0: 7475 726e 2073 6574 2829 0a20 2020 2020  turn set().     
+0000fd00: 2020 206d 6563 6861 6e69 736d 7320 3d20     mechanisms = 
+0000fd10: 6d65 6368 616e 6973 6d73 2e67 6574 5461  mechanisms.getTa
+0000fd20: 6773 2827 6d65 6368 616e 6973 6d27 290a  gs('mechanism').
+0000fd30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000fd40: 6574 286d 6563 682e 6765 7444 6174 6128  et(mech.getData(
+0000fd50: 2920 666f 7220 6d65 6368 2069 6e20 6d65  ) for mech in me
+0000fd60: 6368 616e 6973 6d73 290a 0a20 2020 2064  chanisms)..    d
+0000fd70: 6566 2067 6574 5f64 6f6d 6169 6e5f 6261  ef get_domain_ba
+0000fd80: 7365 645f 6e61 6d65 2873 656c 6629 3a0a  sed_name(self):.
+0000fd90: 2020 2020 2020 2020 686f 7374 6e61 6d65          hostname
+0000fda0: 203d 2073 656c 662e 6765 7454 6167 2827   = self.getTag('
+0000fdb0: 686f 7374 6e61 6d65 272c 0a20 2020 2020  hostname',.     
+0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdd0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
+0000fde0: 6163 653d 4e61 6d65 7370 6163 652e 444f  ace=Namespace.DO
+0000fdf0: 4d41 494e 5f42 4153 4544 5f4e 414d 4529  MAIN_BASED_NAME)
+0000fe00: 0a20 2020 2020 2020 2069 6620 686f 7374  .        if host
+0000fe10: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+0000fe20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000fe30: 7475 726e 2068 6f73 746e 616d 652e 6765  turn hostname.ge
+0000fe40: 7444 6174 6128 290a 2020 2020 2020 2020  tData().        
+0000fe50: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000fe60: 2064 6566 2068 6173 5f62 696e 6428 7365   def has_bind(se
+0000fe70: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0000fe80: 7572 6e20 7365 6c66 2e67 6574 5461 6728  urn self.getTag(
+0000fe90: 2762 696e 6427 2c20 6e61 6d65 7370 6163  'bind', namespac
+0000fea0: 653d 4e61 6d65 7370 6163 652e 4249 4e44  e=Namespace.BIND
+0000feb0: 2920 6973 206e 6f74 204e 6f6e 650a 0a20  ) is not None.. 
+0000fec0: 2020 2064 6566 2073 6573 7369 6f6e 5f72     def session_r
+0000fed0: 6571 7569 7265 6428 7365 6c66 293a 0a20  equired(self):. 
+0000fee0: 2020 2020 2020 2073 6573 7369 6f6e 203d         session =
+0000fef0: 2073 656c 662e 6765 7454 6167 2827 7365   self.getTag('se
+0000ff00: 7373 696f 6e27 2c20 6e61 6d65 7370 6163  ssion', namespac
+0000ff10: 653d 4e61 6d65 7370 6163 652e 5345 5353  e=Namespace.SESS
+0000ff20: 494f 4e29 0a20 2020 2020 2020 2069 6620  ION).        if 
+0000ff30: 7365 7373 696f 6e20 6973 206e 6f74 204e  session is not N
+0000ff40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000ff50: 206f 7074 696f 6e61 6c20 3d20 7365 7373   optional = sess
+0000ff60: 696f 6e2e 6765 7454 6167 2827 6f70 7469  ion.getTag('opti
+0000ff70: 6f6e 616c 2729 2069 7320 6e6f 7420 4e6f  onal') is not No
+0000ff80: 6e65 0a20 2020 2020 2020 2020 2020 2072  ne.            r
+0000ff90: 6574 7572 6e20 6e6f 7420 6f70 7469 6f6e  eturn not option
+0000ffa0: 616c 0a20 2020 2020 2020 2072 6574 7572  al.        retur
+0000ffb0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+0000ffc0: 2068 6173 5f73 6d28 7365 6c66 293a 0a20   has_sm(self):. 
+0000ffd0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000ffe0: 6c66 2e67 6574 5461 6728 2773 6d27 2c20  lf.getTag('sm', 
+0000fff0: 6e61 6d65 7370 6163 653d 4e61 6d65 7370  namespace=Namesp
+00010000: 6163 652e 5354 5245 414d 5f4d 474d 5429  ace.STREAM_MGMT)
+00010010: 2069 7320 6e6f 7420 4e6f 6e65 0a0a 2020   is not None..  
+00010020: 2020 6465 6620 6861 735f 726f 7374 6572    def has_roster
+00010030: 5f76 6572 7369 6f6e 2873 656c 6629 3a0a  _version(self):.
+00010040: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00010050: 656c 662e 6765 7454 6167 2827 7665 7227  elf.getTag('ver'
+00010060: 2c20 6e61 6d65 7370 6163 653d 4e61 6d65  , namespace=Name
+00010070: 7370 6163 652e 524f 5354 4552 5f56 4552  space.ROSTER_VER
+00010080: 2920 6973 206e 6f74 204e 6f6e 650a 0a20  ) is not None.. 
+00010090: 2020 2064 6566 2068 6173 5f72 6567 6973     def has_regis
+000100a0: 7465 7228 7365 6c66 293a 0a20 2020 2020  ter(self):.     
+000100b0: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
+000100c0: 6574 5461 6728 0a20 2020 2020 2020 2020  etTag(.         
+000100d0: 2020 2027 7265 6769 7374 6572 272c 206e     'register', n
+000100e0: 616d 6573 7061 6365 3d4e 616d 6573 7061  amespace=Namespa
+000100f0: 6365 2e52 4547 4953 5445 525f 4645 4154  ce.REGISTER_FEAT
+00010100: 5552 4529 2069 7320 6e6f 7420 4e6f 6e65  URE) is not None
+00010110: 0a0a 2020 2020 6465 6620 6861 735f 616e  ..    def has_an
+00010120: 6f6e 796d 6f75 7328 7365 6c66 293a 0a20  onymous(self):. 
+00010130: 2020 2020 2020 2072 6574 7572 6e20 2741         return 'A
+00010140: 4e4f 4e59 4d4f 5553 2720 696e 2073 656c  NONYMOUS' in sel
+00010150: 662e 6765 745f 6d65 6368 7328 290a 0a0a  f.get_mechs()...
+00010160: 636c 6173 7320 4572 726f 724e 6f64 6528  class ErrorNode(
+00010170: 4e6f 6465 293a 0a20 2020 2022 2222 0a20  Node):.    """. 
+00010180: 2020 2058 4d50 502d 7374 796c 6520 6572     XMPP-style er
+00010190: 726f 7220 656c 656d 656e 740a 0a20 2020  ror element..   
+000101a0: 2049 6e20 7468 6520 6361 7365 206f 6620   In the case of 
+000101b0: 7374 616e 7a61 2065 7272 6f72 2073 686f  stanza error sho
+000101c0: 756c 6420 6265 2061 7474 6163 6865 6420  uld be attached 
+000101d0: 746f 2058 4d50 5020 7374 616e 7a61 2e0a  to XMPP stanza..
+000101e0: 2020 2020 496e 2074 6865 2063 6173 6520      In the case 
+000101f0: 6f66 2073 7472 6561 6d2d 6c65 7665 6c20  of stream-level 
+00010200: 6572 726f 7273 2073 686f 756c 6420 6265  errors should be
+00010210: 2075 7365 6420 7365 7061 7261 7465 6c79   used separately
+00010220: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00010230: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00010240: 2c20 6e61 6d65 2c20 636f 6465 3d4e 6f6e  , name, code=Non
+00010250: 652c 2074 7970 3d4e 6f6e 652c 2074 6578  e, typ=None, tex
+00010260: 743d 4e6f 6e65 293a 0a20 2020 2020 2020  t=None):.       
+00010270: 2022 2222 0a20 2020 2020 2020 204d 616e   """.        Man
+00010280: 6461 746f 7279 2070 6172 616d 6574 6572  datory parameter
+00010290: 3a20 6e61 6d65 202d 206e 616d 6520 6f66  : name - name of
+000102a0: 2065 7272 6f72 2063 6f6e 6469 7469 6f6e   error condition
+000102b0: 2e0a 2020 2020 2020 2020 4f70 7469 6f6e  ..        Option
+000102c0: 616c 2070 6172 616d 6574 6572 733a 2063  al parameters: c
+000102d0: 6f64 652c 2074 7970 2c20 7465 7874 2e0a  ode, typ, text..
+000102e0: 2020 2020 2020 2020 5573 6564 2066 6f72          Used for
+000102f0: 2062 6163 6b77 6172 6473 2063 6f6d 7061   backwards compa
+00010300: 7274 6962 696c 6974 7920 7769 7468 206f  rtibility with o
+00010310: 6c64 6572 206a 6162 6265 7220 7072 6f74  lder jabber prot
+00010320: 6f63 6f6c 2e0a 2020 2020 2020 2020 2222  ocol..        ""
+00010330: 220a 2020 2020 2020 2020 6966 206e 616d  ".        if nam
+00010340: 6520 696e 2045 5252 4f52 533a 0a20 2020  e in ERRORS:.   
+00010350: 2020 2020 2020 2020 2063 6f64 2c20 7479           cod, ty
+00010360: 7065 5f2c 2074 7874 203d 2045 5252 4f52  pe_, txt = ERROR
+00010370: 535b 6e61 6d65 5d0a 2020 2020 2020 2020  S[name].        
+00010380: 2020 2020 6e73 203d 206e 616d 652e 7370      ns = name.sp
+00010390: 6c69 7428 295b 305d 0a20 2020 2020 2020  lit()[0].       
+000103a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000103b0: 2020 2063 6f64 2c20 6e73 2c20 7479 7065     cod, ns, type
+000103c0: 5f2c 2074 7874 203d 2027 3530 3027 2c20  _, txt = '500', 
+000103d0: 4e61 6d65 7370 6163 652e 5354 414e 5a41  Namespace.STANZA
+000103e0: 532c 2027 6361 6e63 656c 272c 2027 270a  S, 'cancel', ''.
+000103f0: 2020 2020 2020 2020 6966 2074 7970 3a0a          if typ:.
+00010400: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00010410: 5f20 3d20 7479 700a 2020 2020 2020 2020  _ = typ.        
+00010420: 6966 2063 6f64 653a 0a20 2020 2020 2020  if code:.       
+00010430: 2020 2020 2063 6f64 203d 2063 6f64 650a       cod = code.
+00010440: 2020 2020 2020 2020 6966 2074 6578 743a          if text:
+00010450: 0a20 2020 2020 2020 2020 2020 2074 7874  .            txt
+00010460: 203d 2074 6578 740a 2020 2020 2020 2020   = text.        
+00010470: 4e6f 6465 2e5f 5f69 6e69 745f 5f28 7365  Node.__init__(se
+00010480: 6c66 2c20 2765 7272 6f72 272c 207b 7d2c  lf, 'error', {},
+00010490: 205b 4e6f 6465 286e 616d 6529 5d29 0a20   [Node(name)]). 
+000104a0: 2020 2020 2020 2069 6620 7479 7065 5f3a         if type_:
+000104b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000104c0: 662e 7365 7441 7474 7228 2774 7970 6527  f.setAttr('type'
+000104d0: 2c20 7479 7065 5f29 0a20 2020 2020 2020  , type_).       
+000104e0: 2069 6620 6e6f 7420 636f 643a 0a20 2020   if not cod:.   
+000104f0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00010500: 744e 616d 6528 2773 7472 6561 6d3a 6572  tName('stream:er
+00010510: 726f 7227 290a 2020 2020 2020 2020 6966  ror').        if
+00010520: 2074 7874 3a0a 2020 2020 2020 2020 2020   txt:.          
+00010530: 2020 7365 6c66 2e61 6464 4368 696c 6428    self.addChild(
+00010540: 6e6f 6465 3d4e 6f64 6528 6e73 202b 2027  node=Node(ns + '
+00010550: 2074 6578 7427 2c20 7b7d 2c20 5b74 7874   text', {}, [txt
+00010560: 5d29 290a 2020 2020 2020 2020 6966 2063  ])).        if c
+00010570: 6f64 3a0a 2020 2020 2020 2020 2020 2020  od:.            
+00010580: 7365 6c66 2e73 6574 4174 7472 2827 636f  self.setAttr('co
+00010590: 6465 272c 2063 6f64 290a 0a63 6c61 7373  de', cod)..class
+000105a0: 2045 7272 6f72 2850 726f 746f 636f 6c29   Error(Protocol)
+000105b0: 3a0a 2020 2020 2222 220a 2020 2020 5573  :.    """.    Us
+000105c0: 6564 2074 6f20 7175 6963 6b6c 7920 7472  ed to quickly tr
+000105d0: 616e 7366 6f72 6d20 7265 6365 6976 6564  ansform received
+000105e0: 2073 7461 6e7a 6120 696e 746f 2065 7272   stanza into err
+000105f0: 6f72 2072 6570 6c79 0a20 2020 2022 2222  or reply.    """
+00010600: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00010610: 5f5f 2873 656c 662c 206e 6f64 652c 2065  __(self, node, e
+00010620: 7272 6f72 2c20 7265 706c 793d 3129 3a0a  rror, reply=1):.
+00010630: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010640: 2020 2020 4372 6561 7465 2065 7272 6f72      Create error
+00010650: 2072 6570 6c79 2062 6173 696e 6720 6f6e   reply basing on
+00010660: 2074 6865 2072 6563 6569 7665 6420 276e   the received 'n
+00010670: 6f64 6527 2073 7461 6e7a 6120 616e 6420  ode' stanza and 
+00010680: 7468 6520 2765 7272 6f72 270a 2020 2020  the 'error'.    
+00010690: 2020 2020 6572 726f 7220 636f 6e64 6974      error condit
+000106a0: 696f 6e0a 0a20 2020 2020 2020 2049 6620  ion..        If 
+000106b0: 7468 6520 276e 6f64 6527 2069 7320 6e6f  the 'node' is no
+000106c0: 7420 7468 6520 7265 6365 6976 6564 2073  t the received s
+000106d0: 7461 6e7a 6120 6275 7420 6c6f 6361 6c6c  tanza but locall
+000106e0: 7920 6372 6561 7465 6420 2827 746f 2720  y created ('to' 
+000106f0: 616e 640a 2020 2020 2020 2020 2766 726f  and.        'fro
+00010700: 6d27 2066 6965 6c64 7320 6e65 6564 7320  m' fields needs 
+00010710: 6e6f 7420 7377 6170 7069 6e67 2920 7370  not swapping) sp
+00010720: 6563 6966 7920 7468 6520 2772 6570 6c79  ecify the 'reply
+00010730: 2720 6172 6775 6d65 6e74 2061 7320 6661  ' argument as fa
+00010740: 6c73 652e 0a20 2020 2020 2020 2022 2222  lse..        """
+00010750: 0a20 2020 2020 2020 2069 6620 6e6f 6465  .        if node
+00010760: 2e67 6574 5479 7065 2829 203d 3d20 2765  .getType() == 'e
+00010770: 7272 6f72 273a 0a20 2020 2020 2020 2020  rror':.         
+00010780: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00010790: 726f 7228 2743 616e e280 9974 2063 7265  ror('Can...t cre
+000107a0: 6174 6520 6572 726f 7220 7265 706c 7920  ate error reply 
+000107b0: 6672 6f6d 2065 7272 6f72 2729 0a0a 2020  from error')..  
+000107c0: 2020 2020 2020 6966 2072 6570 6c79 3a0a        if reply:.
+000107d0: 2020 2020 2020 2020 2020 2020 5072 6f74              Prot
+000107e0: 6f63 6f6c 2e5f 5f69 6e69 745f 5f28 7365  ocol.__init__(se
+000107f0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010810: 2020 746f 3d6e 6f64 652e 6765 7446 726f    to=node.getFro
+00010820: 6d28 292c 0a20 2020 2020 2020 2020 2020  m(),.           
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 2020 206e 6f64 653d 6e6f 6465 290a 2020     node=node).  
+00010850: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00010860: 656c 4174 7472 2827 6672 6f6d 2729 0a20  elAttr('from'). 
+00010870: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010880: 2020 2020 2020 2020 2050 726f 746f 636f           Protoco
+00010890: 6c2e 5f5f 696e 6974 5f5f 2873 656c 662c  l.__init__(self,
+000108a0: 206e 6f64 653d 6e6f 6465 290a 2020 2020   node=node).    
+000108b0: 2020 2020 7365 6c66 2e73 6574 4572 726f      self.setErro
+000108c0: 7228 6572 726f 7229 0a0a 0a63 6c61 7373  r(error)...class
+000108d0: 2044 6174 6146 6965 6c64 284e 6f64 6529   DataField(Node)
+000108e0: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+000108f0: 6973 2063 6c61 7373 2069 7320 7573 6564  is class is used
+00010900: 2069 6e20 7468 6520 4461 7461 466f 726d   in the DataForm
+00010910: 2063 6c61 7373 2074 6f20 6465 7363 7269   class to descri
+00010920: 6265 2074 6865 2073 696e 676c 6520 6461  be the single da
+00010930: 7461 2069 7465 6d0a 0a20 2020 2049 6620  ta item..    If 
+00010940: 796f 7520 6172 6520 776f 726b 696e 6720  you are working 
+00010950: 7769 7468 206a 6162 6265 723a 783a 6461  with jabber:x:da
+00010960: 7461 2028 5845 502d 3030 3034 2c20 5845  ta (XEP-0004, XE
+00010970: 502d 3030 3638 2c20 5845 502d 3031 3232  P-0068, XEP-0122
+00010980: 2920 7468 656e 0a20 2020 2079 6f75 2077  ) then.    you w
+00010990: 696c 6c20 6e65 6564 2074 6f20 776f 726b  ill need to work
+000109a0: 2077 6974 6820 696e 7374 616e 6365 7320   with instances 
+000109b0: 6f66 2074 6869 7320 636c 6173 732e 0a20  of this class.. 
+000109c0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+000109d0: 5f5f 696e 6974 5f5f 2873 656c 662c 0a20  __init__(self,. 
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 6e61 6d65 3d4e 6f6e 652c 0a20 2020 2020  name=None,.     
+00010a00: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00010a10: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+00010a20: 2020 2020 2020 2020 2074 7970 3d4e 6f6e           typ=Non
+00010a30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00010a40: 2020 2020 7265 7175 6972 6564 3d30 2c0a      required=0,.
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 2064 6573 633d 4e6f 6e65 2c0a 2020 2020   desc=None,.    
+00010a70: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+00010a80: 696f 6e73 3d4e 6f6e 652c 0a20 2020 2020  ions=None,.     
+00010a90: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00010aa0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00010ab0: 2222 220a 2020 2020 2020 2020 4372 6561  """.        Crea
+00010ac0: 7465 206e 6577 2064 6174 6120 6669 656c  te new data fiel
+00010ad0: 6420 6f66 2073 7065 6369 6669 6564 206e  d of specified n
+00010ae0: 616d 652c 7661 6c75 6520 616e 6420 7479  ame,value and ty
+00010af0: 7065 0a0a 2020 2020 2020 2020 416c 736f  pe..        Also
+00010b00: 2027 7265 7175 6972 6564 272c 2764 6573   'required','des
+00010b10: 6327 2061 6e64 2027 6f70 7469 6f6e 7327  c' and 'options'
+00010b20: 2066 6965 6c64 7320 6361 6e20 6265 2073   fields can be s
+00010b30: 6574 2e20 416c 7465 726e 6174 6976 656c  et. Alternativel
+00010b40: 790a 2020 2020 2020 2020 6f74 6865 7220  y.        other 
+00010b50: 584d 4c20 6f62 6a65 6374 2063 616e 2062  XML object can b
+00010b60: 6520 7061 7373 6564 2069 6e20 6173 2074  e passed in as t
+00010b70: 6865 2027 6e6f 6465 2720 7061 7261 6d65  he 'node' parame
+00010b80: 7465 640a 2020 2020 2020 2020 746f 2072  ted.        to r
+00010b90: 6570 6c69 6361 7465 2069 7420 6173 2061  eplicate it as a
+00010ba0: 206e 6577 2064 6174 6166 696c 6564 2e0a   new datafiled..
+00010bb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010bc0: 2020 2020 4e6f 6465 2e5f 5f69 6e69 745f      Node.__init_
+00010bd0: 5f28 7365 6c66 2c20 2766 6965 6c64 272c  _(self, 'field',
+00010be0: 206e 6f64 653d 6e6f 6465 290a 2020 2020   node=node).    
+00010bf0: 2020 2020 6966 206e 616d 653a 0a20 2020      if name:.   
+00010c00: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00010c10: 7456 6172 286e 616d 6529 0a20 2020 2020  tVar(name).     
+00010c20: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00010c30: 2876 616c 7565 2c20 286c 6973 742c 2074  (value, (list, t
+00010c40: 7570 6c65 2929 3a0a 2020 2020 2020 2020  uple)):.        
+00010c50: 2020 2020 7365 6c66 2e73 6574 5661 6c75      self.setValu
+00010c60: 6573 2876 616c 7565 290a 2020 2020 2020  es(value).      
+00010c70: 2020 656c 6966 2076 616c 7565 3a0a 2020    elif value:.  
+00010c80: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00010c90: 6574 5661 6c75 6528 7661 6c75 6529 0a20  etValue(value). 
+00010ca0: 2020 2020 2020 2069 6620 7479 703a 0a20         if typ:. 
+00010cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010cc0: 7365 7454 7970 6528 7479 7029 0a20 2020  setType(typ).   
+00010cd0: 2020 2020 2065 6c69 6620 6e6f 7420 7479       elif not ty
+00010ce0: 7020 616e 6420 6e6f 7420 6e6f 6465 3a0a  p and not node:.
+00010cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010d00: 2e73 6574 5479 7065 2827 7465 7874 2d73  .setType('text-s
+00010d10: 696e 676c 6527 290a 2020 2020 2020 2020  ingle').        
+00010d20: 6966 2072 6571 7569 7265 643a 0a20 2020  if required:.   
+00010d30: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00010d40: 7452 6571 7569 7265 6428 7265 7175 6972  tRequired(requir
+00010d50: 6564 290a 2020 2020 2020 2020 6966 2064  ed).        if d
+00010d60: 6573 633a 0a20 2020 2020 2020 2020 2020  esc:.           
+00010d70: 2073 656c 662e 7365 7444 6573 6328 6465   self.setDesc(de
+00010d80: 7363 290a 2020 2020 2020 2020 6966 206f  sc).        if o
+00010d90: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
+00010da0: 2020 2020 7365 6c66 2e73 6574 4f70 7469      self.setOpti
+00010db0: 6f6e 7328 6f70 7469 6f6e 7329 0a0a 2020  ons(options)..  
+00010dc0: 2020 6465 6620 7365 7452 6571 7569 7265    def setRequire
+00010dd0: 6428 7365 6c66 2c20 7265 713d 3129 3a0a  d(self, req=1):.
+00010de0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010df0: 2020 2020 4368 616e 6765 2074 6865 2073      Change the s
+00010e00: 7461 7465 206f 6620 7468 6520 2772 6571  tate of the 'req
+00010e10: 7569 7265 6427 2066 6c61 670a 2020 2020  uired' flag.    
+00010e20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010e30: 6966 2072 6571 3a0a 2020 2020 2020 2020  if req:.        
+00010e40: 2020 2020 7365 6c66 2e73 6574 5461 6728      self.setTag(
+00010e50: 2772 6571 7569 7265 6427 290a 2020 2020  'required').    
+00010e60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010e70: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00010e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010e90: 6465 6c43 6869 6c64 2827 7265 7175 6972  delChild('requir
+00010ea0: 6564 2729 0a20 2020 2020 2020 2020 2020  ed').           
+00010eb0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00010ec0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00010ed0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00010ee0: 6465 6620 6973 5265 7175 6972 6564 2873  def isRequired(s
+00010ef0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00010f00: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00010f10: 2069 6e20 7468 6973 2066 6965 6c64 2061   in this field a
+00010f20: 2072 6571 7569 7265 6420 6f6e 650a 2020   required one.  
+00010f30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010f40: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
+00010f50: 7454 6167 2827 7265 7175 6972 6564 2729  tTag('required')
+00010f60: 0a0a 2020 2020 6465 6620 7365 7444 6573  ..    def setDes
+00010f70: 6328 7365 6c66 2c20 6465 7363 293a 0a20  c(self, desc):. 
+00010f80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010f90: 2020 2053 6574 2074 6865 2064 6573 6372     Set the descr
+00010fa0: 6970 7469 6f6e 206f 6620 7468 6973 2066  iption of this f
+00010fb0: 6965 6c64 0a20 2020 2020 2020 2022 2222  ield.        """
+00010fc0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00010fd0: 7454 6167 4461 7461 2827 6465 7363 272c  tTagData('desc',
+00010fe0: 2064 6573 6329 0a0a 2020 2020 6465 6620   desc)..    def 
+00010ff0: 6765 7444 6573 6328 7365 6c66 293a 0a20  getDesc(self):. 
+00011000: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011010: 2020 2052 6574 7572 6e20 7468 6520 6465     Return the de
+00011020: 7363 7269 7074 696f 6e20 6f66 2074 6869  scription of thi
+00011030: 7320 6669 656c 640a 2020 2020 2020 2020  s field.        
+00011040: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00011050: 726e 2073 656c 662e 6765 7454 6167 4461  rn self.getTagDa
+00011060: 7461 2827 6465 7363 2729 0a0a 2020 2020  ta('desc')..    
+00011070: 6465 6620 7365 7456 616c 7565 2873 656c  def setValue(sel
+00011080: 662c 2076 616c 293a 0a20 2020 2020 2020  f, val):.       
+00011090: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+000110a0: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
+000110b0: 6973 2066 6965 6c64 0a20 2020 2020 2020  is field.       
+000110c0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+000110d0: 662e 7365 7454 6167 4461 7461 2827 7661  f.setTagData('va
+000110e0: 6c75 6527 2c20 7661 6c29 0a0a 2020 2020  lue', val)..    
+000110f0: 6465 6620 6765 7456 616c 7565 2873 656c  def getValue(sel
+00011100: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00011110: 726e 2073 656c 662e 6765 7454 6167 4461  rn self.getTagDa
+00011120: 7461 2827 7661 6c75 6527 290a 0a20 2020  ta('value')..   
+00011130: 2064 6566 2073 6574 5661 6c75 6573 2873   def setValues(s
+00011140: 656c 662c 206c 7374 293a 0a20 2020 2020  elf, lst):.     
+00011150: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00011160: 6574 2074 6865 2076 616c 7565 7320 6f66  et the values of
+00011170: 2074 6869 7320 6669 656c 6420 6173 2076   this field as v
+00011180: 616c 7565 732d 6c69 7374 2e20 5265 706c  alues-list. Repl
+00011190: 6163 6573 2061 6c6c 2070 7265 7669 6f75  aces all previou
+000111a0: 7320 6669 6c65 640a 2020 2020 2020 2020  s filed.        
+000111b0: 7661 6c75 6573 2120 4966 2079 6f75 206e  values! If you n
+000111c0: 6565 6420 746f 206a 7573 7420 6164 6420  eed to just add 
+000111d0: 6120 7661 6c75 6520 2d20 7573 6520 6164  a value - use ad
+000111e0: 6456 616c 7565 206d 6574 686f 640a 2020  dValue method.  
+000111f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011200: 2020 7768 696c 6520 7365 6c66 2e67 6574    while self.get
+00011210: 5461 6728 2776 616c 7565 2729 3a0a 2020  Tag('value'):.  
+00011220: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00011230: 656c 4368 696c 6428 2776 616c 7565 2729  elChild('value')
+00011240: 0a20 2020 2020 2020 2066 6f72 2076 616c  .        for val
+00011250: 2069 6e20 6c73 743a 0a20 2020 2020 2020   in lst:.       
+00011260: 2020 2020 2073 656c 662e 6164 6456 616c       self.addVal
+00011270: 7565 2876 616c 290a 0a20 2020 2064 6566  ue(val)..    def
+00011280: 2061 6464 5661 6c75 6528 7365 6c66 2c20   addValue(self, 
+00011290: 7661 6c29 3a0a 2020 2020 2020 2020 2222  val):.        ""
+000112a0: 220a 2020 2020 2020 2020 4164 6420 6f6e  ".        Add on
+000112b0: 6520 6d6f 7265 2076 616c 7565 2074 6f20  e more value to 
+000112c0: 7468 6973 2066 6965 6c64 2e20 5573 6564  this field. Used
+000112d0: 2069 6e20 2767 6574 2720 6971 2773 206f   in 'get' iq's o
+000112e0: 7220 7375 6368 0a20 2020 2020 2020 2022  r such.        "
+000112f0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00011300: 6164 6443 6869 6c64 2827 7661 6c75 6527  addChild('value'
+00011310: 2c20 7b7d 2c20 5b76 616c 5d29 0a0a 2020  , {}, [val])..  
+00011320: 2020 6465 6620 6765 7456 616c 7565 7328    def getValues(
+00011330: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00011340: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+00011350: 6e20 7468 6520 6c69 7374 206f 6620 7661  n the list of va
+00011360: 6c75 6573 2061 7373 6f63 6961 7465 6420  lues associated 
+00011370: 7769 7468 2074 6869 7320 6669 656c 640a  with this field.
+00011380: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011390: 2020 2020 7265 7420 3d20 5b5d 0a20 2020      ret = [].   
+000113a0: 2020 2020 2066 6f72 2074 6167 2069 6e20       for tag in 
+000113b0: 7365 6c66 2e67 6574 5461 6773 2827 7661  self.getTags('va
+000113c0: 6c75 6527 293a 0a20 2020 2020 2020 2020  lue'):.         
+000113d0: 2020 2072 6574 2e61 7070 656e 6428 7461     ret.append(ta
+000113e0: 672e 6765 7444 6174 6128 2929 0a20 2020  g.getData()).   
+000113f0: 2020 2020 2072 6574 7572 6e20 7265 740a       return ret.
+00011400: 0a20 2020 2064 6566 2067 6574 4f70 7469  .    def getOpti
+00011410: 6f6e 7328 7365 6c66 293a 0a20 2020 2020  ons(self):.     
+00011420: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00011430: 6574 7572 6e20 6c61 6265 6c2d 6f70 7469  eturn label-opti
+00011440: 6f6e 2070 6169 7273 206c 6973 7420 6173  on pairs list as
+00011450: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
+00011460: 6973 2066 6965 6c64 0a20 2020 2020 2020  is field.       
+00011470: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00011480: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00011490: 7220 7461 6720 696e 2073 656c 662e 6765  r tag in self.ge
+000114a0: 7454 6167 7328 276f 7074 696f 6e27 293a  tTags('option'):
+000114b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000114c0: 2e61 7070 656e 6428 5b74 6167 2e67 6574  .append([tag.get
+000114d0: 4174 7472 2827 6c61 6265 6c27 292c 2074  Attr('label'), t
+000114e0: 6167 2e67 6574 5461 6744 6174 6128 2776  ag.getTagData('v
+000114f0: 616c 7565 2729 5d29 0a20 2020 2020 2020  alue')]).       
+00011500: 2072 6574 7572 6e20 7265 740a 0a20 2020   return ret..   
+00011510: 2064 6566 2073 6574 4f70 7469 6f6e 7328   def setOptions(
+00011520: 7365 6c66 2c20 6c73 7429 3a0a 2020 2020  self, lst):.    
+00011530: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011540: 5365 7420 6c61 6265 6c2d 6f70 7469 6f6e  Set label-option
+00011550: 2070 6169 7273 206c 6973 7420 6173 736f   pairs list asso
+00011560: 6369 6174 6564 2077 6974 6820 7468 6973  ciated with this
+00011570: 2066 6965 6c64 0a20 2020 2020 2020 2022   field.        "
+00011580: 2222 0a20 2020 2020 2020 2077 6869 6c65  "".        while
+00011590: 2073 656c 662e 6765 7454 6167 2827 6f70   self.getTag('op
+000115a0: 7469 6f6e 2729 3a0a 2020 2020 2020 2020  tion'):.        
+000115b0: 2020 2020 7365 6c66 2e64 656c 4368 696c      self.delChil
+000115c0: 6428 276f 7074 696f 6e27 290a 2020 2020  d('option').    
+000115d0: 2020 2020 666f 7220 6f70 7420 696e 206c      for opt in l
+000115e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+000115f0: 7365 6c66 2e61 6464 4f70 7469 6f6e 286f  self.addOption(o
+00011600: 7074 290a 0a20 2020 2064 6566 2061 6464  pt)..    def add
+00011610: 4f70 7469 6f6e 2873 656c 662c 206f 7074  Option(self, opt
+00011620: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00011630: 2020 2020 2020 2041 6464 206f 6e65 206d         Add one m
+00011640: 6f72 6520 6c61 6265 6c2d 6f70 7469 6f6e  ore label-option
+00011650: 2070 6169 7220 746f 2074 6869 7320 6669   pair to this fi
+00011660: 656c 640a 2020 2020 2020 2020 2222 220a  eld.        """.
+00011670: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00011680: 7461 6e63 6528 6f70 742c 206c 6973 7429  tance(opt, list)
+00011690: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000116a0: 6c66 2e61 6464 4368 696c 6428 276f 7074  lf.addChild('opt
+000116b0: 696f 6e27 2c0a 2020 2020 2020 2020 2020  ion',.          
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116d0: 7b27 6c61 6265 6c27 3a20 6f70 745b 305d  {'label': opt[0]
+000116e0: 7d29 2e73 6574 5461 6744 6174 6128 2776  }).setTagData('v
+000116f0: 616c 7565 272c 206f 7074 5b31 5d29 0a20  alue', opt[1]). 
+00011700: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011710: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+00011720: 6443 6869 6c64 2827 6f70 7469 6f6e 2729  dChild('option')
+00011730: 2e73 6574 5461 6744 6174 6128 2776 616c  .setTagData('val
+00011740: 7565 272c 206f 7074 290a 0a20 2020 2064  ue', opt)..    d
+00011750: 6566 2067 6574 5479 7065 2873 656c 6629  ef getType(self)
+00011760: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00011770: 2020 2020 2020 4765 7420 7479 7065 206f        Get type o
+00011780: 6620 7468 6973 2066 6965 6c64 0a20 2020  f this field.   
+00011790: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000117a0: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+000117b0: 4174 7472 2827 7479 7065 2729 0a0a 2020  Attr('type')..  
+000117c0: 2020 6465 6620 7365 7454 7970 6528 7365    def setType(se
+000117d0: 6c66 2c20 7661 6c29 3a0a 2020 2020 2020  lf, val):.      
+000117e0: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
+000117f0: 7420 7479 7065 206f 6620 7468 6973 2066  t type of this f
+00011800: 6965 6c64 0a20 2020 2020 2020 2022 2222  ield.        """
+00011810: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011820: 7365 6c66 2e73 6574 4174 7472 2827 7479  self.setAttr('ty
+00011830: 7065 272c 2076 616c 290a 0a20 2020 2064  pe', val)..    d
+00011840: 6566 2067 6574 5661 7228 7365 6c66 293a  ef getVar(self):
+00011850: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011860: 2020 2020 2047 6574 2027 7661 7227 2061       Get 'var' a
+00011870: 7474 7269 6275 7465 2076 616c 7565 206f  ttribute value o
+00011880: 6620 7468 6973 2066 6965 6c64 0a20 2020  f this field.   
+00011890: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000118a0: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+000118b0: 4174 7472 2827 7661 7227 290a 0a20 2020  Attr('var')..   
+000118c0: 2064 6566 2073 6574 5661 7228 7365 6c66   def setVar(self
+000118d0: 2c20 7661 6c29 3a0a 2020 2020 2020 2020  , val):.        
+000118e0: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
+000118f0: 2776 6172 2720 6174 7472 6962 7574 6520  'var' attribute 
+00011900: 7661 6c75 6520 6f66 2074 6869 7320 6669  value of this fi
+00011910: 656c 640a 2020 2020 2020 2020 2222 220a  eld.        """.
+00011920: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011930: 656c 662e 7365 7441 7474 7228 2776 6172  elf.setAttr('var
+00011940: 272c 2076 616c 290a 0a63 6c61 7373 2044  ', val)..class D
+00011950: 6174 6146 6f72 6d28 4e6f 6465 293a 0a20  ataForm(Node):. 
+00011960: 2020 2022 2222 0a20 2020 2055 7365 6420     """.    Used 
+00011970: 666f 7220 6d61 6e69 7075 6c61 7469 6e67  for manipulating
+00011980: 2064 6174 6166 6f72 6d73 2069 6e20 584d   dataforms in XM
+00011990: 5050 0a0a 2020 2020 5265 6c65 7661 6e74  PP..    Relevant
+000119a0: 2058 4550 733a 2030 3030 342c 2030 3036   XEPs: 0004, 006
+000119b0: 382c 2030 3132 322e 2043 616e 2062 6520  8, 0122. Can be 
+000119c0: 7573 6564 2069 6e20 6469 7363 6f2c 2070  used in disco, p
+000119d0: 7562 2d73 7562 2061 6e64 206d 616e 790a  ub-sub and many.
+000119e0: 2020 2020 6f74 6865 7220 6170 706c 6963      other applic
+000119f0: 6174 696f 6e73 2e0a 2020 2020 2222 220a  ations..    """.
+00011a00: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00011a10: 2873 656c 662c 2074 7970 3d4e 6f6e 652c  (self, typ=None,
+00011a20: 2064 6174 613d 4e6f 6e65 2c20 7469 746c   data=None, titl
+00011a30: 653d 4e6f 6e65 2c20 6e6f 6465 3d4e 6f6e  e=None, node=Non
+00011a40: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00011a50: 2020 2020 2020 2020 4372 6561 7465 206e          Create n
+00011a60: 6577 2064 6174 6166 6f72 6d20 6f66 2074  ew dataform of t
+00011a70: 7970 6520 2774 7970 272e 2027 6461 7461  ype 'typ'. 'data
+00011a80: 2720 6973 2074 6865 206c 6973 7420 6f66  ' is the list of
+00011a90: 2044 6174 6146 6965 6c64 0a20 2020 2020   DataField.     
+00011aa0: 2020 2069 6e73 7461 6e63 6573 2074 6861     instances tha
+00011ab0: 7420 7468 6973 2064 6174 6166 6f72 6d20  t this dataform 
+00011ac0: 636f 6e74 6169 6e73 2c20 2774 6974 6c65  contains, 'title
+00011ad0: 2720 2d20 7468 6520 7469 746c 6520 7374  ' - the title st
+00011ae0: 7269 6e67 2e20 2059 6f75 0a20 2020 2020  ring.  You.     
+00011af0: 2020 2063 616e 2073 7065 6369 6679 2074     can specify t
+00011b00: 6865 2027 6e6f 6465 2720 6172 6775 6d65  he 'node' argume
+00011b10: 6e74 2061 7320 7468 6520 6f74 6865 7220  nt as the other 
+00011b20: 6e6f 6465 2074 6f20 6265 2075 7365 6420  node to be used 
+00011b30: 6173 2062 6173 6520 666f 720a 2020 2020  as base for.    
+00011b40: 2020 2020 636f 6e73 7472 7563 7469 6e67      constructing
+00011b50: 2074 6869 7320 6461 7461 666f 726d 0a0a   this dataform..
+00011b60: 2020 2020 2020 2020 7469 746c 6520 616e          title an
+00011b70: 6420 696e 7374 7275 6374 696f 6e73 2069  d instructions i
+00011b80: 7320 6f70 7469 6f6e 616c 2061 6e64 2053  s optional and S
+00011b90: 484f 554c 4420 4e4f 5420 636f 6e74 6169  HOULD NOT contai
+00011ba0: 6e20 6e65 776c 696e 6573 2e0a 2020 2020  n newlines..    
+00011bb0: 2020 2020 5365 7665 7261 6c20 696e 7374      Several inst
+00011bc0: 7275 6374 696f 6e73 204d 4159 2062 6520  ructions MAY be 
+00011bd0: 7072 6573 656e 742e 0a20 2020 2020 2020  present..       
+00011be0: 2027 7479 7027 2063 616e 2062 6520 6f6e   'typ' can be on
+00011bf0: 6520 6f66 2028 2766 6f72 6d27 207c 2027  e of ('form' | '
+00011c00: 7375 626d 6974 2720 7c20 2763 616e 6365  submit' | 'cance
+00011c10: 6c27 207c 2027 7265 7375 6c74 2720 290a  l' | 'result' ).
+00011c20: 2020 2020 2020 2020 2774 7970 2720 6f66          'typ' of
+00011c30: 2072 6570 6c79 2069 7120 6361 6e20 6265   reply iq can be
+00011c40: 2028 2027 7265 7375 6c74 2720 7c20 2773   ( 'result' | 's
+00011c50: 6574 2720 7c20 2773 6574 2720 7c20 2772  et' | 'set' | 'r
+00011c60: 6573 756c 7427 2029 0a20 2020 2020 2020  esult' ).       
+00011c70: 2020 2020 2072 6573 7065 6374 6976 656c       respectivel
+00011c80: 792e 0a20 2020 2020 2020 2027 6361 6e63  y..        'canc
+00011c90: 656c 2720 666f 726d 2063 616e 206e 6f74  el' form can not
+00011ca0: 2063 6f6e 7461 696e 2061 6e79 2066 6965   contain any fie
+00011cb0: 6c64 732e 2041 6c6c 206f 7468 6572 2066  lds. All other f
+00011cc0: 6f72 6d73 2063 6f6e 7461 696e 730a 2020  orms contains.  
+00011cd0: 2020 2020 2020 2020 2020 4154 204c 4541            AT LEA
+00011ce0: 5354 206f 6e65 2066 6965 6c64 2e0a 2020  ST one field..  
+00011cf0: 2020 2020 2020 2774 6974 6c65 2720 4d41        'title' MA
+00011d00: 5920 6265 2069 6e63 6c75 6465 6420 696e  Y be included in
+00011d10: 2066 6f72 6d73 206f 6620 7479 7065 2022   forms of type "
+00011d20: 666f 726d 2220 616e 6420 2272 6573 756c  form" and "resul
+00011d30: 7422 0a20 2020 2020 2020 2022 2222 0a20  t".        """. 
+00011d40: 2020 2020 2020 204e 6f64 652e 5f5f 696e         Node.__in
+00011d50: 6974 5f5f 2873 656c 662c 2027 7827 2c20  it__(self, 'x', 
+00011d60: 6e6f 6465 3d6e 6f64 6529 0a20 2020 2020  node=node).     
+00011d70: 2020 2069 6620 6e6f 6465 3a0a 2020 2020     if node:.    
+00011d80: 2020 2020 2020 2020 6e65 776b 6964 7320          newkids 
+00011d90: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00011da0: 2066 6f72 206e 2069 6e20 7365 6c66 2e67   for n in self.g
+00011db0: 6574 4368 696c 6472 656e 2829 3a0a 2020  etChildren():.  
+00011dc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011dd0: 206e 2e67 6574 4e61 6d65 2829 203d 3d20   n.getName() == 
+00011de0: 2766 6965 6c64 273a 0a20 2020 2020 2020  'field':.       
+00011df0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+00011e00: 6b69 6473 2e61 7070 656e 6428 4461 7461  kids.append(Data
+00011e10: 4669 656c 6428 6e6f 6465 3d6e 2929 0a20  Field(node=n)). 
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011e30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00011e40: 2020 2020 2020 2020 206e 6577 6b69 6473           newkids
+00011e50: 2e61 7070 656e 6428 6e29 0a20 2020 2020  .append(n).     
+00011e60: 2020 2020 2020 2073 656c 662e 6b69 6473         self.kids
+00011e70: 203d 206e 6577 6b69 6473 0a20 2020 2020   = newkids.     
+00011e80: 2020 2069 6620 7479 703a 0a20 2020 2020     if typ:.     
+00011e90: 2020 2020 2020 2073 656c 662e 7365 7454         self.setT
+00011ea0: 7970 6528 7479 7029 0a20 2020 2020 2020  ype(typ).       
+00011eb0: 2073 656c 662e 7365 744e 616d 6573 7061   self.setNamespa
+00011ec0: 6365 284e 616d 6573 7061 6365 2e44 4154  ce(Namespace.DAT
+00011ed0: 4129 0a20 2020 2020 2020 2069 6620 7469  A).        if ti
+00011ee0: 746c 653a 0a20 2020 2020 2020 2020 2020  tle:.           
+00011ef0: 2073 656c 662e 7365 7454 6974 6c65 2874   self.setTitle(t
+00011f00: 6974 6c65 290a 2020 2020 2020 2020 6966  itle).        if
+00011f10: 2064 6174 6120 6973 206e 6f74 204e 6f6e   data is not Non
+00011f20: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00011f30: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+00011f40: 612c 2064 6963 7429 3a0a 2020 2020 2020  a, dict):.      
+00011f50: 2020 2020 2020 2020 2020 6e65 7764 6174            newdat
+00011f60: 6120 3d20 5b5d 0a20 2020 2020 2020 2020  a = [].         
+00011f70: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
+00011f80: 696e 2064 6174 612e 6b65 7973 2829 3a0a  in data.keys():.
+00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fa0: 2020 2020 6e65 7764 6174 612e 6170 7065      newdata.appe
+00011fb0: 6e64 2844 6174 6146 6965 6c64 286e 616d  nd(DataField(nam
+00011fc0: 652c 2064 6174 615b 6e61 6d65 5d29 290a  e, data[name])).
+00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fe0: 6461 7461 203d 206e 6577 6461 7461 0a20  data = newdata. 
+00011ff0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00012000: 6869 6c64 2069 6e20 6461 7461 3a0a 2020  hild in data:.  
+00012010: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012020: 2063 6869 6c64 2e5f 5f63 6c61 7373 5f5f   child.__class__
+00012030: 2e5f 5f6e 616d 655f 5f20 3d3d 2027 4461  .__name__ == 'Da
+00012040: 7461 4669 656c 6427 3a0a 2020 2020 2020  taField':.      
+00012050: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012060: 6c66 2e6b 6964 732e 6170 7065 6e64 2863  lf.kids.append(c
+00012070: 6869 6c64 290a 2020 2020 2020 2020 2020  hild).          
+00012080: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00012090: 7461 6e63 6528 6368 696c 642c 204e 6f64  tance(child, Nod
+000120a0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000120b0: 2020 2020 2020 2020 7365 6c66 2e6b 6964          self.kid
+000120c0: 732e 6170 7065 6e64 2844 6174 6146 6965  s.append(DataFie
+000120d0: 6c64 286e 6f64 653d 6368 696c 6429 290a  ld(node=child)).
+000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 656c 7365 3a20 2023 204d 7573 7420 6265  else:  # Must be
+00012100: 2061 2073 7472 696e 670a 2020 2020 2020   a string.      
+00012110: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012120: 6c66 2e61 6464 496e 7374 7275 6374 696f  lf.addInstructio
+00012130: 6e73 2863 6869 6c64 290a 0a20 2020 2064  ns(child)..    d
+00012140: 6566 2067 6574 5479 7065 2873 656c 6629  ef getType(self)
+00012150: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012160: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00012170: 2074 7970 6520 6f66 2064 6174 6166 6f72   type of datafor
+00012180: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
+00012190: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000121a0: 662e 6765 7441 7474 7228 2774 7970 6527  f.getAttr('type'
+000121b0: 290a 0a20 2020 2064 6566 2073 6574 5479  )..    def setTy
+000121c0: 7065 2873 656c 662c 2074 7970 293a 0a20  pe(self, typ):. 
+000121d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000121e0: 2020 2053 6574 2074 6865 2074 7970 6520     Set the type 
+000121f0: 6f66 2064 6174 6166 6f72 6d0a 2020 2020  of dataform.    
+00012200: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012210: 7365 6c66 2e73 6574 4174 7472 2827 7479  self.setAttr('ty
+00012220: 7065 272c 2074 7970 290a 0a20 2020 2064  pe', typ)..    d
+00012230: 6566 2067 6574 5469 746c 6528 7365 6c66  ef getTitle(self
+00012240: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012250: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+00012260: 6520 7469 746c 6520 6f66 2064 6174 6166  e title of dataf
+00012270: 6f72 6d0a 2020 2020 2020 2020 2222 220a  orm.        """.
+00012280: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00012290: 656c 662e 6765 7454 6167 4461 7461 2827  elf.getTagData('
+000122a0: 7469 746c 6527 290a 0a20 2020 2064 6566  title')..    def
+000122b0: 2073 6574 5469 746c 6528 7365 6c66 2c20   setTitle(self, 
+000122c0: 7465 7874 293a 0a20 2020 2020 2020 2022  text):.        "
+000122d0: 2222 0a20 2020 2020 2020 2053 6574 2074  "".        Set t
+000122e0: 6865 2074 6974 6c65 206f 6620 6461 7461  he title of data
+000122f0: 666f 726d 0a20 2020 2020 2020 2022 2222  form.        """
+00012300: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00012310: 7454 6167 4461 7461 2827 7469 746c 6527  tTagData('title'
+00012320: 2c20 7465 7874 290a 0a20 2020 2064 6566  , text)..    def
+00012330: 2067 6574 496e 7374 7275 6374 696f 6e73   getInstructions
+00012340: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00012350: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+00012360: 726e 2074 6865 2069 6e73 7472 7563 7469  rn the instructi
+00012370: 6f6e 7320 6f66 2064 6174 6166 6f72 6d0a  ons of dataform.
+00012380: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012390: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000123a0: 6765 7454 6167 4461 7461 2827 696e 7374  getTagData('inst
+000123b0: 7275 6374 696f 6e73 2729 0a0a 2020 2020  ructions')..    
+000123c0: 6465 6620 7365 7449 6e73 7472 7563 7469  def setInstructi
+000123d0: 6f6e 7328 7365 6c66 2c20 7465 7874 293a  ons(self, text):
+000123e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000123f0: 2020 2020 2053 6574 2074 6865 2069 6e73       Set the ins
+00012400: 7472 7563 7469 6f6e 7320 6f66 2064 6174  tructions of dat
+00012410: 6166 6f72 6d0a 2020 2020 2020 2020 2222  aform.        ""
+00012420: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
+00012430: 6574 5461 6744 6174 6128 2769 6e73 7472  etTagData('instr
+00012440: 7563 7469 6f6e 7327 2c20 7465 7874 290a  uctions', text).
+00012450: 0a20 2020 2064 6566 2061 6464 496e 7374  .    def addInst
+00012460: 7275 6374 696f 6e73 2873 656c 662c 2074  ructions(self, t
+00012470: 6578 7429 3a0a 2020 2020 2020 2020 2222  ext):.        ""
+00012480: 220a 2020 2020 2020 2020 4164 6420 6f6e  ".        Add on
+00012490: 6520 6d6f 7265 2069 6e73 7472 7563 7469  e more instructi
+000124a0: 6f6e 2074 6f20 7468 6520 6461 7461 666f  on to the datafo
+000124b0: 726d 0a20 2020 2020 2020 2022 2222 0a20  rm.        """. 
+000124c0: 2020 2020 2020 2073 656c 662e 6164 6443         self.addC
+000124d0: 6869 6c64 2827 696e 7374 7275 6374 696f  hild('instructio
+000124e0: 6e73 272c 207b 7d2c 205b 7465 7874 5d29  ns', {}, [text])
+000124f0: 0a0a 2020 2020 6465 6620 6765 7446 6965  ..    def getFie
+00012500: 6c64 2873 656c 662c 206e 616d 6529 3a0a  ld(self, name):.
+00012510: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012520: 2020 2020 5265 7475 726e 2074 6865 2064      Return the d
+00012530: 6174 6166 6965 6c64 206f 626a 6563 7420  atafield object 
+00012540: 7769 7468 206e 616d 6520 276e 616d 6527  with name 'name'
+00012550: 2028 6966 2065 7869 7374 7329 0a20 2020   (if exists).   
+00012560: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012570: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+00012580: 5461 6728 2766 6965 6c64 272c 2061 7474  Tag('field', att
+00012590: 7273 3d7b 2776 6172 273a 206e 616d 657d  rs={'var': name}
+000125a0: 290a 0a20 2020 2064 6566 2073 6574 4669  )..    def setFi
+000125b0: 656c 6428 7365 6c66 2c20 6e61 6d65 293a  eld(self, name):
+000125c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000125d0: 2020 2020 2043 7265 6174 6520 6966 206e       Create if n
+000125e0: 6573 7365 7373 6172 7920 6f72 2067 6574  essessary or get
+000125f0: 2074 6865 2065 7869 7374 696e 6720 6461   the existing da
+00012600: 7461 6669 656c 6420 6f62 6a65 6374 2077  tafield object w
+00012610: 6974 6820 6e61 6d65 0a20 2020 2020 2020  ith name.       
+00012620: 2027 6e61 6d65 2720 616e 6420 7265 7475   'name' and retu
+00012630: 726e 2069 740a 2020 2020 2020 2020 2222  rn it.        ""
+00012640: 220a 2020 2020 2020 2020 6620 3d20 7365  ".        f = se
+00012650: 6c66 2e67 6574 4669 656c 6428 6e61 6d65  lf.getField(name
+00012660: 290a 2020 2020 2020 2020 6966 2066 3a0a  ).        if f:.
+00012670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012680: 726e 2066 0a20 2020 2020 2020 2072 6574  rn f.        ret
+00012690: 7572 6e20 7365 6c66 2e61 6464 4368 696c  urn self.addChil
+000126a0: 6428 6e6f 6465 3d44 6174 6146 6965 6c64  d(node=DataField
+000126b0: 286e 616d 6529 290a 0a20 2020 2064 6566  (name))..    def
+000126c0: 2061 7344 6963 7428 7365 6c66 293a 0a20   asDict(self):. 
+000126d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000126e0: 2020 2052 6570 7265 7365 6e74 2064 6174     Represent dat
+000126f0: 6166 6f72 6d20 6173 2073 696d 706c 6520  aform as simple 
+00012700: 6469 6374 696f 6e61 7279 206d 6170 7069  dictionary mappi
+00012710: 6e67 206f 6620 6461 7461 6669 656c 6420  ng of datafield 
+00012720: 6e61 6d65 7320 746f 0a20 2020 2020 2020  names to.       
+00012730: 2074 6865 6972 2076 616c 7565 730a 2020   their values.  
+00012740: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012750: 2020 7265 7420 3d20 7b7d 0a20 2020 2020    ret = {}.     
+00012760: 2020 2066 6f72 2066 6965 6c64 2069 6e20     for field in 
+00012770: 7365 6c66 2e67 6574 5461 6773 2827 6669  self.getTags('fi
+00012780: 656c 6427 293a 0a20 2020 2020 2020 2020  eld'):.         
+00012790: 2020 206e 616d 6520 3d20 6669 656c 642e     name = field.
+000127a0: 6765 7441 7474 7228 2776 6172 2729 0a20  getAttr('var'). 
+000127b0: 2020 2020 2020 2020 2020 2074 7970 203d             typ =
+000127c0: 2066 6965 6c64 2e67 6574 5479 7065 2829   field.getType()
+000127d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000127e0: 7479 7020 616e 6420 7479 702e 656e 6473  typ and typ.ends
+000127f0: 7769 7468 2827 2d6d 756c 7469 2729 3a0a  with('-multi'):.
+00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012810: 7661 6c20 3d20 5b5d 0a20 2020 2020 2020  val = [].       
+00012820: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00012830: 6e20 6669 656c 642e 6765 7454 6167 7328  n field.getTags(
+00012840: 2776 616c 7565 2729 3a0a 2020 2020 2020  'value'):.      
+00012850: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00012860: 6c2e 6170 7065 6e64 2869 2e67 6574 4461  l.append(i.getDa
+00012870: 7461 2829 290a 2020 2020 2020 2020 2020  ta()).          
+00012880: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012890: 2020 2020 2020 2020 7661 6c20 3d20 6669          val = fi
+000128a0: 656c 642e 6765 7454 6167 4461 7461 2827  eld.getTagData('
+000128b0: 7661 6c75 6527 290a 2020 2020 2020 2020  value').        
+000128c0: 2020 2020 7265 745b 6e61 6d65 5d20 3d20      ret[name] = 
+000128d0: 7661 6c0a 2020 2020 2020 2020 6966 2073  val.        if s
+000128e0: 656c 662e 6765 7454 6167 2827 696e 7374  elf.getTag('inst
+000128f0: 7275 6374 696f 6e73 2729 3a0a 2020 2020  ructions'):.    
+00012900: 2020 2020 2020 2020 7265 745b 2769 6e73          ret['ins
+00012910: 7472 7563 7469 6f6e 7327 5d20 3d20 7365  tructions'] = se
+00012920: 6c66 2e67 6574 496e 7374 7275 6374 696f  lf.getInstructio
+00012930: 6e73 2829 0a20 2020 2020 2020 2072 6574  ns().        ret
+00012940: 7572 6e20 7265 740a 0a20 2020 2064 6566  urn ret..    def
+00012950: 205f 5f67 6574 6974 656d 5f5f 2873 656c   __getitem__(sel
+00012960: 662c 206e 616d 6529 3a0a 2020 2020 2020  f, name):.      
+00012970: 2020 2222 220a 2020 2020 2020 2020 5369    """.        Si
+00012980: 6d70 6c65 2064 6963 7469 6f6e 6172 7920  mple dictionary 
+00012990: 696e 7465 7266 6163 6520 666f 7220 6765  interface for ge
+000129a0: 7474 696e 6720 6461 7461 6669 656c 6473  tting datafields
+000129b0: 2076 616c 7565 7320 6279 2074 6865 6972   values by their
+000129c0: 206e 616d 6573 0a20 2020 2020 2020 2022   names.        "
+000129d0: 2222 0a20 2020 2020 2020 2069 7465 6d20  "".        item 
+000129e0: 3d20 7365 6c66 2e67 6574 4669 656c 6428  = self.getField(
+000129f0: 6e61 6d65 290a 2020 2020 2020 2020 6966  name).        if
+00012a00: 2069 7465 6d3a 0a20 2020 2020 2020 2020   item:.         
+00012a10: 2020 2072 6574 7572 6e20 6974 656d 2e67     return item.g
+00012a20: 6574 5661 6c75 6528 290a 2020 2020 2020  etValue().      
+00012a30: 2020 7261 6973 6520 496e 6465 7845 7272    raise IndexErr
+00012a40: 6f72 2827 4e6f 2073 7563 6820 6669 656c  or('No such fiel
+00012a50: 6427 290a 0a20 2020 2064 6566 205f 5f73  d')..    def __s
+00012a60: 6574 6974 656d 5f5f 2873 656c 662c 206e  etitem__(self, n
+00012a70: 616d 652c 2076 616c 293a 0a20 2020 2020  ame, val):.     
+00012a80: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00012a90: 696d 706c 6520 6469 6374 696f 6e61 7279  imple dictionary
+00012aa0: 2069 6e74 6572 6661 6365 2066 6f72 2073   interface for s
+00012ab0: 6574 7469 6e67 2064 6174 6166 6965 6c64  etting datafield
+00012ac0: 7320 7661 6c75 6573 2062 7920 7468 6569  s values by thei
+00012ad0: 7220 6e61 6d65 730a 2020 2020 2020 2020  r names.        
+00012ae0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00012af0: 726e 2073 656c 662e 7365 7446 6965 6c64  rn self.setField
+00012b00: 286e 616d 6529 2e73 6574 5661 6c75 6528  (name).setValue(
+00012b10: 7661 6c29 0a                             val).
```

### Comparing `nbxmpp-4.3.1/nbxmpp/sasl.py` & `nbxmpp-4.3.2/nbxmpp/sasl.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/simplexml.py` & `nbxmpp-4.3.2/nbxmpp/simplexml.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/smacks.py` & `nbxmpp-4.3.2/nbxmpp/smacks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/stringprep.py` & `nbxmpp-4.3.2/nbxmpp/stringprep.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/structs.py` & `nbxmpp-4.3.2/nbxmpp/structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,17 +295,21 @@
     id: str
     fallback_start: Optional[int]
     fallback_end: Optional[int]
 
 
 class ModerationData(NamedTuple):
     stanza_id: str
-    moderator_jid: str
-    reason: Optional[str] = None
-    timestamp: Optional[str] = None
+    moderator_jid: Optional[str]
+    by: Optional[JID]
+    reason: Optional[str]
+    timestamp: Optional[str]
+    stamp: float
+    is_tombstone: bool
+    occupant_id: Optional[str]
 
 
 class DiscoItems(NamedTuple):
     jid: JID
     node: str
     items: list[DiscoItem]
 
@@ -765,18 +769,26 @@
     def __init__(self, stanza):
         self._stanza_name = stanza.getName()
         self._error_node = stanza.getTag('error')
         self.condition = stanza.getError()
         self.condition_data = self._error_node.getTagData(self.condition)
         self.app_condition = stanza.getAppError()
         self.type = stanza.getErrorType()
+        self.by = None
         self.jid = stanza.getFrom()
         self.id = stanza.getID()
         self._text = {}
 
+        by = self._error_node.getAttr('by')
+        if by is not None:
+            try:
+                self.by = JID.from_string(by)
+            except Exception:
+                pass
+
         text_elements = self._error_node.getTags('text', namespace=Namespace.STANZAS)
         for element in text_elements:
             lang = element.getXmlLang()
             text = element.getData()
             self._text[lang] = text
 
     @classmethod
@@ -913,15 +925,15 @@
 
 
 class MAMData(NamedTuple):
     id: str
     query_id: str
     archive: JID
     namespace: str
-    timestamp: datetime
+    timestamp: float
 
     @property
     def is_ver_1(self) -> bool:
         return self.namespace == Namespace.MAM_1
 
     @property
     def is_ver_2(self) -> bool:
@@ -960,17 +972,19 @@
 @dataclass
 class MessageProperties:
     own_jid: JID
     carbon: Optional[CarbonData] = None
     type: MessageType = MessageType.NORMAL
     id: Optional[str] = None
     stanza_ids: list[StanzaIDData] = field(default_factory=list)
+    origin_id: Optional[str] = None
     from_: Optional[JID] = None
     to: Optional[JID] = None
     jid: Optional[JID] = None
+    remote_jid: Optional[JID] = None
     subject = None
     body: Optional[str] = None
     thread: Optional[str] = None
     user_timestamp = None
     timestamp: float = field(default_factory=time.time)
     has_server_delay: bool = False
     error = None
```

### Comparing `nbxmpp-4.3.1/nbxmpp/task.py` & `nbxmpp-4.3.2/nbxmpp/task.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/tcp.py` & `nbxmpp-4.3.2/nbxmpp/tcp.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/third_party/hsluv.py` & `nbxmpp-4.3.2/nbxmpp/third_party/hsluv.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/util.py` & `nbxmpp-4.3.2/nbxmpp/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/websocket.py` & `nbxmpp-4.3.2/nbxmpp/websocket.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp/xmppiri.py` & `nbxmpp-4.3.2/nbxmpp/xmppiri.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/nbxmpp.egg-info/PKG-INFO` & `nbxmpp-4.3.2/nbxmpp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbxmpp
-Version: 4.3.1
+Version: 4.3.2
 Summary: XMPP Library
 Author-email: Philipp Hörist <philipp@hoerist.com>, Yann Leboulanger <yann@leboulanger.org>
 License: GPL-3.0-or-later
 Project-URL: repository, https://dev.gajim.org/gajim/python-nbxmpp
 Keywords: chat,messaging,im,xmpp
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `nbxmpp-4.3.1/nbxmpp.egg-info/SOURCES.txt` & `nbxmpp-4.3.2/nbxmpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/pyproject.toml` & `nbxmpp-4.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/lib/__init__.py` & `nbxmpp-4.3.2/test/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/lib/util.py` & `nbxmpp-4.3.2/test/lib/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/lib/xmpp_mocks.py` & `nbxmpp-4.3.2/test/lib/xmpp_mocks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_activity.py` & `nbxmpp-4.3.2/test/unit/test_activity.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_avatar.py` & `nbxmpp-4.3.2/test/unit/test_avatar.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_bookmarks.py` & `nbxmpp-4.3.2/test/unit/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_datetime_parsing.py` & `nbxmpp-4.3.2/test/unit/test_datetime_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_delay_parsing.py` & `nbxmpp-4.3.2/test/unit/test_delay_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_entity_caps.py` & `nbxmpp-4.3.2/test/unit/test_entity_caps.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_error_parsing.py` & `nbxmpp-4.3.2/test/unit/test_error_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_http.py` & `nbxmpp-4.3.2/test/unit/test_http.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_jid_parsing.py` & `nbxmpp-4.3.2/test/unit/test_jid_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_location.py` & `nbxmpp-4.3.2/test/unit/test_location.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_mood.py` & `nbxmpp-4.3.2/test/unit/test_mood.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_muclumbus.py` & `nbxmpp-4.3.2/test/unit/test_muclumbus.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_pubsub.py` & `nbxmpp-4.3.2/test/unit/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_reactions.py` & `nbxmpp-4.3.2/test/unit/test_reactions.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_sasl_scram.py` & `nbxmpp-4.3.2/test/unit/test_sasl_scram.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_stringprep.py` & `nbxmpp-4.3.2/test/unit/test_stringprep.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_tune.py` & `nbxmpp-4.3.2/test/unit/test_tune.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.1/test/unit/test_xml_vulnerability.py` & `nbxmpp-4.3.2/test/unit/test_xml_vulnerability.py`

 * *Files identical despite different names*

