# Comparing `tmp/aws_network_firewall-0.7.2.tar.gz` & `tmp/aws_network_firewall-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.7.2.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.7.3.tar", max compression
```

## Comparing `aws_network_firewall-0.7.2.tar` & `aws_network_firewall-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11335 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/README.md
--rw-r--r--   0        0        0       22 2023-07-31 14:39:01.500255 aws_network_firewall-0.7.2/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1776 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      352 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     6089 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/rule.py
--rw-r--r--   0        0        0      708 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/rule_set.py
--rw-r--r--   0        0        0     2043 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2766 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      211 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      473 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1283 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-31 14:39:01.504255 aws_network_firewall-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-08-07 09:42:13.262350 aws_network_firewall-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-08-07 09:42:13.262350 aws_network_firewall-0.7.3/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 09:42:14.126363 aws_network_firewall-0.7.3/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1776 2023-08-07 09:42:13.262350 aws_network_firewall-0.7.3/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-08-07 09:42:13.262350 aws_network_firewall-0.7.3/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-08-07 09:42:13.262350 aws_network_firewall-0.7.3/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      352 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     6089 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0      708 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/rule_set.py
+-rw-r--r--   0        0        0     2043 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2766 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      211 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1283 2023-08-07 09:42:13.266350 aws_network_firewall-0.7.3/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-08-07 09:42:14.130363 aws_network_firewall-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.3/PKG-INFO
```

### Comparing `aws_network_firewall-0.7.2/LICENSE.txt` & `aws_network_firewall-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/README.md` & `aws_network_firewall-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/account.py` & `aws_network_firewall-0.7.3/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.7.3/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.7.3/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.7.3/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.7.3/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/rule.py` & `aws_network_firewall-0.7.3/aws_network_firewall/rule.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,16 @@
             f"{destination.message} | {self.workload} | {self.name}"
             if destination.message
             else f"{self.workload} | {self.name}"
         )
 
         return [
             SuricataOption(name="msg", value=message),
-            SuricataOption(name="rev", value="1", quoted_value=False),
             SuricataOption(name="sid", value="XXX", quoted_value=False),
+            SuricataOption(name="rev", value="1", quoted_value=False),
         ]
 
     def __resolve_tls_version_rules(
         self, destination: Destination
     ) -> List[SuricataRule]:
         ssl_version = ",".join(destination.tls_versions)
```

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/rule_set.py` & `aws_network_firewall-0.7.3/aws_network_firewall/rule_set.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.7.3/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.7.3/aws_network_firewall/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.7.3/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.2/pyproject.toml` & `aws_network_firewall-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.7.2/PKG-INFO` & `aws_network_firewall-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

