# Comparing `tmp/notifications_sender-0.1.0.tar.gz` & `tmp/notifications_sender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notifications_sender-0.1.0.tar", max compression
+gzip compressed data, was "notifications_sender-0.2.0.tar", max compression
```

## Comparing `notifications_sender-0.1.0.tar` & `notifications_sender-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       72 2023-08-03 13:52:02.528880 notifications_sender-0.1.0/notifications_sender/__init__.py
--rw-r--r--   0        0        0    10184 2023-08-03 13:50:51.515615 notifications_sender-0.1.0/notifications_sender/send_notifications.py
--rw-r--r--   0        0        0      352 2023-08-03 13:53:43.961080 notifications_sender-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 notifications_sender-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-08-03 13:52:02.528880 notifications_sender-0.2.0/notifications_sender/__init__.py
+-rw-r--r--   0        0        0    10178 2023-08-07 07:36:58.494731 notifications_sender-0.2.0/notifications_sender/send_notifications.py
+-rw-r--r--   0        0        0      352 2023-08-07 07:37:20.994428 notifications_sender-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 notifications_sender-0.2.0/PKG-INFO
```

### Comparing `notifications_sender-0.1.0/notifications_sender/send_notifications.py` & `notifications_sender-0.2.0/notifications_sender/send_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import dateparser
 import datetime
 import pandas as pd
 import smtplib
-from datetime import datetime, timedelta
 from dateutil.relativedelta import relativedelta
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.policy import SMTPUTF8
 
 
 # DAY_OF_MAILING_BIRTHDAYS = 3
@@ -113,16 +112,16 @@
     teams_members_birthdays = pd.read_csv(LINK_BIRTHDAYS)
     teams_members_birthdays['День рождения (дата)'] = teams_members_birthdays['День рождения'].apply(parse_date_birthday)
     teams_members_with_birthday_today = []
     teams_members_with_birthday_in_next_month = []
     for _, team_member in teams_members_birthdays.iterrows():
         team_member_birthday = team_member['День рождения (дата)']
         if (team_member_birthday.day == current_date.day and team_member_birthday.month == current_date.month) or \
-                (team_member_birthday.weekday() == 5 and team_member_birthday.day == (current_date + timedelta(days=1)).day and team_member_birthday.month == (current_date + timedelta(days=1)).month) or \
-                (team_member_birthday.weekday() == 6 and team_member_birthday.day == (current_date + timedelta(days=2)).day and team_member_birthday.month == (current_date + timedelta(days=2)).month):
+                (team_member_birthday.weekday() == 5 and team_member_birthday.day == (current_date + datetime.timedelta(days=1)).day and team_member_birthday.month == (current_date + datetime.timedelta(days=1)).month) or \
+                (team_member_birthday.weekday() == 6 and team_member_birthday.day == (current_date + datetime.timedelta(days=2)).day and team_member_birthday.month == (current_date + datetime.timedelta(days=2)).month):
 
             teams_members_with_birthday_today.append(team_member)
         if team_member_birthday.month == (current_date + relativedelta(months=1)).month:
             teams_members_with_birthday_in_next_month.append(team_member)
 
     if current_date.day == DAY_OF_MAILING_BIRTHDAYS and len(teams_members_with_birthday_in_next_month) != 0:
         msg = MIMEMultipart("alternative", policy=SMTPUTF8)
```

### Comparing `notifications_sender-0.1.0/PKG-INFO` & `notifications_sender-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifications-sender
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Alexander
 Author-email: cahr2001@mail.ru
 Requires-Python: >3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

