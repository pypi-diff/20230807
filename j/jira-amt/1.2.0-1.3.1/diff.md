# Comparing `tmp/jira_amt-1.2.0.tar.gz` & `tmp/jira_amt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira_amt-1.2.0.tar", max compression
+gzip compressed data, was "jira_amt-1.3.1.tar", max compression
```

## Comparing `jira_amt-1.2.0.tar` & `jira_amt-1.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-08-06 10:14:53.763165 jira_amt-1.2.0/LICENSE
--rw-r--r--   0        0        0     3086 2023-08-06 10:14:53.763165 jira_amt-1.2.0/README.md
--rw-r--r--   0        0        0      263 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/__init__.py
--rw-r--r--   0        0        0      161 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/__main__.py
--rw-r--r--   0        0        0     5886 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/cli.py
--rw-r--r--   0        0        0     1971 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/config.py
--rw-r--r--   0        0        0     4574 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/jira.py
--rw-r--r--   0        0        0     1261 2023-08-06 10:14:53.763165 jira_amt-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 jira_amt-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-07 09:36:21.053286 jira_amt-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3987 2023-08-07 09:36:21.053286 jira_amt-1.3.1/README.md
+-rw-r--r--   0        0        0      263 2023-08-07 09:36:21.053286 jira_amt-1.3.1/jira_amt/__init__.py
+-rw-r--r--   0        0        0      161 2023-08-07 09:36:21.053286 jira_amt-1.3.1/jira_amt/__main__.py
+-rw-r--r--   0        0        0     5886 2023-08-07 09:36:21.053286 jira_amt-1.3.1/jira_amt/cli.py
+-rw-r--r--   0        0        0     1971 2023-08-07 09:36:21.053286 jira_amt-1.3.1/jira_amt/config.py
+-rw-r--r--   0        0        0     4726 2023-08-07 09:36:21.053286 jira_amt-1.3.1/jira_amt/jira.py
+-rw-r--r--   0        0        0     1261 2023-08-07 09:36:21.053286 jira_amt-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 jira_amt-1.3.1/PKG-INFO
```

### Comparing `jira_amt-1.2.0/LICENSE` & `jira_amt-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jira_amt-1.2.0/README.md` & `jira_amt-1.3.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # Jira Asset Manager
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) ![GitHub release (release name instead of tag name)](https://img.shields.io/github/v/release/hatamiarash7/jira-asset-manager?sort=date) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-asset-manager)
 
 Manage Jira assets in your code or CLI.
 
+- [Jira Asset Manager](#jira-asset-manager)
+  - [Requirements](#requirements)
+  - [Install](#install)
+  - [How-to](#how-to)
+  - [CLI](#cli)
+    - [Create assets](#create-assets)
+    - [Update assets](#update-assets)
+    - [Add comment](#add-comment)
+  - [Package](#package)
+    - [Get asset](#get-asset)
+    - [Create asset](#create-asset)
+    - [Update asset](#update-asset)
+    - [Add comment](#add-comment-1)
+  - [Support 💛](#support-)
+  - [Contributing 🤝](#contributing-)
+
 ## Requirements
 
 - Python 3.8+
 
 ## Install
 
 ```bash
@@ -31,14 +47,18 @@
 
 This command will get everything from your Jira server and save them to `~/.jira` directory for later use. With this data, you don't need to know/use ID of each asset/attribute.
 
 ## CLI
 
 There is some commands to manage assets. Check them using the `--help` flag.
 
+### Create assets
+
+The asset creation in CLI is not make sense, because you need to enter all attributes in command line. But you can use it in your code.
+
 ### Update assets
 
 You can update asset's attribute using it's name. The script will get the asset id from the name automatically.
 
 ```bash
 jira-amt attr <schema> <object> <asset name> <attr name> <attr value>
 jira-amt attr "ITSM" "Servers" "Server-1" "IP" "1.2.3.4"
@@ -68,14 +88,16 @@
 )
 ```
 
 ### Get asset
 
 ```python
 asset = jira.get_asset("schema", "object", "asset's name")
+
+print(asset.text)
 ```
 
 ### Create asset
 
 ```python
 input = {
     "Name": "Server-1",
@@ -84,14 +106,30 @@
     "OS": "Debian",
     "IP": "1.2.3.4"
 }
 
 asset = jira.create_asset("schema", "object", input)
 ```
 
+### Update asset
+
+```python
+asset = jira.get_asset("schema", "object", "asset's name")
+
+print(asset.text)
+```
+
+### Add comment
+
+```python
+result = jira.add_comment("schema", "object", "asset's name", "comment")
+
+print(result.status_code)
+```
+
 ## Support 💛
 
 [![Donate with Bitcoin](https://img.shields.io/badge/Bitcoin-bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz-orange)](https://donatebadges.ir/donate/Bitcoin/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://img.shields.io/badge/Ethereum-0x0831bD72Ea8904B38Be9D6185Da2f930d6078094-blueviolet)](https://donatebadges.ir/donate/Ethereum/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 
 <div><a href="https://payping.ir/@hatamiarash7"><img src="https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg" height="128" width="128"></a></div>
 
 ## Contributing 🤝
```

#### html2text {}

```diff
@@ -1,35 +1,46 @@
 # Jira Asset Manager [![made-with-python](https://img.shields.io/badge/
 Made%20with-Python-1f425f.svg)](https://www.python.org/) ![GitHub release
 (release name instead of tag name)](https://img.shields.io/github/v/release/
 hatamiarash7/jira-asset-manager?sort=date) ![GitHub](https://img.shields.io/
 github/license/hatamiarash7/jira-asset-manager) Manage Jira assets in your code
-or CLI. ## Requirements - Python 3.8+ ## Install ```bash pip install jira-amt
-``` ## How-to You need to add these environment variables to use the CLI: |
-Variable | Description | | ----------- | --------------------------------------
------------- | | JIRA_SERVER | Jira server address like `https://
+or CLI. - [Jira Asset Manager](#jira-asset-manager) - [Requirements]
+(#requirements) - [Install](#install) - [How-to](#how-to) - [CLI](#cli) -
+[Create assets](#create-assets) - [Update assets](#update-assets) - [Add
+comment](#add-comment) - [Package](#package) - [Get asset](#get-asset) -
+[Create asset](#create-asset) - [Update asset](#update-asset) - [Add comment]
+(#add-comment-1) - [Support ð](#support-) - [Contributing ð¤]
+(#contributing-) ## Requirements - Python 3.8+ ## Install ```bash pip install
+jira-amt ``` ## How-to You need to add these environment variables to use the
+CLI: | Variable | Description | | ----------- | -------------------------------
+------------------- | | JIRA_SERVER | Jira server address like `https://
 jira.domain.com` | | JIRA_PAT | Your personal access token | After setting
 these variables, you can configure the CLI: ```bash jira-amt init ``` This
 command will get everything from your Jira server and save them to `~/.jira`
 directory for later use. With this data, you don't need to know/use ID of each
 asset/attribute. ## CLI There is some commands to manage assets. Check them
-using the `--help` flag. ### Update assets You can update asset's attribute
+using the `--help` flag. ### Create assets The asset creation in CLI is not
+make sense, because you need to enter all attributes in command line. But you
+can use it in your code. ### Update assets You can update asset's attribute
 using it's name. The script will get the asset id from the name automatically.
 ```bash jira-amt attr      jira-amt attr "ITSM" "Servers" "Server-1" "IP"
 "1.2.3.4" ``` ### Add comment You can add comment to an asset using it's name.
 The script will get the asset id from the name automatically. ```bash jira-amt
 comment     jira-amt comment "ITSM" "Servers" "Server-1" "This is a comment"
 ``` --- ## Package You can use this package in your code to manage Jira assets.
 ```python from jira_amt.jira import JiraAssetHandler jira = JiraAssetHandler
 ( server="https://jira.domain.com", pat="ABCD1234" ) ``` ### Get asset
-```python asset = jira.get_asset("schema", "object", "asset's name") ``` ###
-Create asset ```python input = { "Name": "Server-1", "Status": "Running",
-"Environment": "Production", "OS": "Debian", "IP": "1.2.3.4" } asset =
-jira.create_asset("schema", "object", input) ``` ## Support ð [![Donate with
-Bitcoin](https://img.shields.io/badge/Bitcoin-
+```python asset = jira.get_asset("schema", "object", "asset's name") print
+(asset.text) ``` ### Create asset ```python input = { "Name": "Server-1",
+"Status": "Running", "Environment": "Production", "OS": "Debian", "IP":
+"1.2.3.4" } asset = jira.create_asset("schema", "object", input) ``` ### Update
+asset ```python asset = jira.get_asset("schema", "object", "asset's name")
+print(asset.text) ``` ### Add comment ```python result = jira.add_comment
+("schema", "object", "asset's name", "comment") print(result.status_code) ```
+## Support ð [![Donate with Bitcoin](https://img.shields.io/badge/Bitcoin-
 bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz-orange)](https://donatebadges.ir/
 donate/Bitcoin/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with
 Ethereum](https://img.shields.io/badge/Ethereum-
 0x0831bD72Ea8904B38Be9D6185Da2f930d6078094-blueviolet)](https://
 donatebadges.ir/donate/Ethereum/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 [https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg]
 ## Contributing ð¤ Don't be shy and reach out to us if you want to contribute
```

### Comparing `jira_amt-1.2.0/jira_amt/cli.py` & `jira_amt-1.3.1/jira_amt/cli.py`

 * *Files identical despite different names*

### Comparing `jira_amt-1.2.0/jira_amt/config.py` & `jira_amt-1.3.1/jira_amt/config.py`

 * *Files identical despite different names*

### Comparing `jira_amt-1.2.0/jira_amt/jira.py` & `jira_amt-1.3.1/jira_amt/jira.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,16 +66,26 @@
         data = {
             "objectTypeId": config.getObject(schema_id+":"+schema, object),
             "attributes": input
         }
         return self._make_api_call("POST", path, data)
 
     def update_asset(self, schema, object, asset_name, attr_name, attr_value):
-        attr_value = config.getAttributeValue(object, attr_name, attr_value)
-        attr_name = config.getAttribute(object, attr_name)
+        attr_value = config.getAttributeValue(
+            object+"."+schema,
+            attr_name,
+            attr_value
+        )
+        attr_name = config.getAttribute(
+            object+"."+schema,
+            attr_name
+        )
+
+        print(attr_value)
+        print(attr_name)
 
         object = self.get_asset(schema, object, asset_name)
         id = json.loads(object.text)['matchedFilterValues'][0]['objectId']
 
         path = f"/object/{id}"
         data = {
             "objectTypeId": config.JIRA_OBJECT,
@@ -90,15 +100,15 @@
 
     # ------ Comments ------
 
     def add_comment(self, schema, object, asset_name, comment):
         object = self.get_asset(schema, object, asset_name)
         id = json.loads(object.text)['matchedFilterValues'][0]['objectId']
 
-        path = f"/comment/create"
+        path = "/comment/create"
         data = {
             "comment": comment,
             "objectId": f"{id}",
             "role": 0
         }
 
         return self._make_api_call("POST", path, data)
@@ -116,15 +126,15 @@
     def get_attributes(self, objectType):
         path = f'/objecttype/{objectType}/attributes'
         return self._make_api_call("GET", path, {})
 
     # ------ Status ------
 
     def get_global_statustypes(self):
-        path = f'/config/statustype'
+        path = '/config/statustype'
         return self._make_api_call("GET", path, {})
 
     def get_statustypes(self, id):
         path = f'/config/statustype?objectSchemaId={id}'
         return self._make_api_call("GET", path, {})
 
     def _make_api_call(self, method, path, data):
```

### Comparing `jira_amt-1.2.0/pyproject.toml` & `jira_amt-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 license = "MIT"
 name = "jira-amt"
 packages = [
   {include = "jira_amt"},
 ]
 readme = "README.md"
 repository = "https://github.com/hatamiarash7/jira-asset-manager"
-version = "1.2.0"
+version = "1.3.1"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2"
 tomlkit = "^0.12.0"
 typer = {extras = [
   "all",
```

### Comparing `jira_amt-1.2.0/PKG-INFO` & `jira_amt-1.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6a69 7261  : 2.1.Name: jira
 00000020: 2d61 6d74 0a56 6572 7369 6f6e 3a20 312e  -amt.Version: 1.
-00000030: 322e 300a 5375 6d6d 6172 793a 204d 616e  2.0.Summary: Man
+00000030: 332e 310a 5375 6d6d 6172 793a 204d 616e  3.1.Summary: Man
 00000040: 6167 6520 4a69 7261 2061 7373 6574 732e  age Jira assets.
 00000050: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000060: 733a 2f2f 6172 6173 682d 6861 7461 6d69  s://arash-hatami
 00000070: 2e69 720a 4c69 6365 6e73 653a 204d 4954  .ir.License: MIT
 00000080: 0a4b 6579 776f 7264 733a 206a 6972 612c  .Keywords: jira,
 00000090: 6173 7365 740a 4175 7468 6f72 3a20 4172  asset.Author: Ar
 000000a0: 6173 6820 4861 7461 6d69 0a41 7574 686f  ash Hatami.Autho
@@ -83,177 +83,233 @@
 00000520: 4875 625d 2868 7474 7073 3a2f 2f69 6d67  Hub](https://img
 00000530: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
 00000540: 7562 2f6c 6963 656e 7365 2f68 6174 616d  ub/license/hatam
 00000550: 6961 7261 7368 372f 6a69 7261 2d61 7373  iarash7/jira-ass
 00000560: 6574 2d6d 616e 6167 6572 290a 0a4d 616e  et-manager)..Man
 00000570: 6167 6520 4a69 7261 2061 7373 6574 7320  age Jira assets 
 00000580: 696e 2079 6f75 7220 636f 6465 206f 7220  in your code or 
-00000590: 434c 492e 0a0a 2323 2052 6571 7569 7265  CLI...## Require
-000005a0: 6d65 6e74 730a 0a2d 2050 7974 686f 6e20  ments..- Python 
-000005b0: 332e 382b 0a0a 2323 2049 6e73 7461 6c6c  3.8+..## Install
-000005c0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-000005d0: 7374 616c 6c20 6a69 7261 2d61 6d74 0a60  stall jira-amt.`
-000005e0: 6060 0a0a 2323 2048 6f77 2d74 6f0a 0a59  ``..## How-to..Y
-000005f0: 6f75 206e 6565 6420 746f 2061 6464 2074  ou need to add t
-00000600: 6865 7365 2065 6e76 6972 6f6e 6d65 6e74  hese environment
-00000610: 2076 6172 6961 626c 6573 2074 6f20 7573   variables to us
-00000620: 6520 7468 6520 434c 493a 0a0a 7c20 5661  e the CLI:..| Va
-00000630: 7269 6162 6c65 2020 2020 7c20 4465 7363  riable    | Desc
-00000640: 7269 7074 696f 6e20 2020 2020 2020 2020  ription         
-00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00000670: 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  .| ----------- |
-00000680: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000006a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000006b0: 2d2d 2d20 7c0a 7c20 4a49 5241 5f53 4552  --- |.| JIRA_SER
-000006c0: 5645 5220 7c20 4a69 7261 2073 6572 7665  VER | Jira serve
-000006d0: 7220 6164 6472 6573 7320 6c69 6b65 2060  r address like `
-000006e0: 6874 7470 733a 2f2f 6a69 7261 2e64 6f6d  https://jira.dom
-000006f0: 6169 6e2e 636f 6d60 207c 0a7c 204a 4952  ain.com` |.| JIR
-00000700: 415f 5041 5420 2020 207c 2059 6f75 7220  A_PAT    | Your 
-00000710: 7065 7273 6f6e 616c 2061 6363 6573 7320  personal access 
-00000720: 746f 6b65 6e20 2020 2020 2020 2020 2020  token           
-00000730: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00000740: 0a41 6674 6572 2073 6574 7469 6e67 2074  .After setting t
-00000750: 6865 7365 2076 6172 6961 626c 6573 2c20  hese variables, 
-00000760: 796f 7520 6361 6e20 636f 6e66 6967 7572  you can configur
-00000770: 6520 7468 6520 434c 493a 0a0a 6060 6062  e the CLI:..```b
-00000780: 6173 680a 6a69 7261 2d61 6d74 2069 6e69  ash.jira-amt ini
-00000790: 740a 6060 600a 0a54 6869 7320 636f 6d6d  t.```..This comm
-000007a0: 616e 6420 7769 6c6c 2067 6574 2065 7665  and will get eve
-000007b0: 7279 7468 696e 6720 6672 6f6d 2079 6f75  rything from you
-000007c0: 7220 4a69 7261 2073 6572 7665 7220 616e  r Jira server an
-000007d0: 6420 7361 7665 2074 6865 6d20 746f 2060  d save them to `
-000007e0: 7e2f 2e6a 6972 6160 2064 6972 6563 746f  ~/.jira` directo
-000007f0: 7279 2066 6f72 206c 6174 6572 2075 7365  ry for later use
-00000800: 2e20 5769 7468 2074 6869 7320 6461 7461  . With this data
-00000810: 2c20 796f 7520 646f 6e27 7420 6e65 6564  , you don't need
-00000820: 2074 6f20 6b6e 6f77 2f75 7365 2049 4420   to know/use ID 
-00000830: 6f66 2065 6163 6820 6173 7365 742f 6174  of each asset/at
-00000840: 7472 6962 7574 652e 0a0a 2323 2043 4c49  tribute...## CLI
-00000850: 0a0a 5468 6572 6520 6973 2073 6f6d 6520  ..There is some 
-00000860: 636f 6d6d 616e 6473 2074 6f20 6d61 6e61  commands to mana
-00000870: 6765 2061 7373 6574 732e 2043 6865 636b  ge assets. Check
-00000880: 2074 6865 6d20 7573 696e 6720 7468 6520   them using the 
-00000890: 602d 2d68 656c 7060 2066 6c61 672e 0a0a  `--help` flag...
-000008a0: 2323 2320 5570 6461 7465 2061 7373 6574  ### Update asset
-000008b0: 730a 0a59 6f75 2063 616e 2075 7064 6174  s..You can updat
-000008c0: 6520 6173 7365 7427 7320 6174 7472 6962  e asset's attrib
-000008d0: 7574 6520 7573 696e 6720 6974 2773 206e  ute using it's n
-000008e0: 616d 652e 2054 6865 2073 6372 6970 7420  ame. The script 
-000008f0: 7769 6c6c 2067 6574 2074 6865 2061 7373  will get the ass
-00000900: 6574 2069 6420 6672 6f6d 2074 6865 206e  et id from the n
-00000910: 616d 6520 6175 746f 6d61 7469 6361 6c6c  ame automaticall
-00000920: 792e 0a0a 6060 6062 6173 680a 6a69 7261  y...```bash.jira
-00000930: 2d61 6d74 2061 7474 7220 3c73 6368 656d  -amt attr <schem
-00000940: 613e 203c 6f62 6a65 6374 3e20 3c61 7373  a> <object> <ass
-00000950: 6574 206e 616d 653e 203c 6174 7472 206e  et name> <attr n
-00000960: 616d 653e 203c 6174 7472 2076 616c 7565  ame> <attr value
-00000970: 3e0a 6a69 7261 2d61 6d74 2061 7474 7220  >.jira-amt attr 
-00000980: 2249 5453 4d22 2022 5365 7276 6572 7322  "ITSM" "Servers"
-00000990: 2022 5365 7276 6572 2d31 2220 2249 5022   "Server-1" "IP"
-000009a0: 2022 312e 322e 332e 3422 0a60 6060 0a0a   "1.2.3.4".```..
-000009b0: 2323 2320 4164 6420 636f 6d6d 656e 740a  ### Add comment.
-000009c0: 0a59 6f75 2063 616e 2061 6464 2063 6f6d  .You can add com
-000009d0: 6d65 6e74 2074 6f20 616e 2061 7373 6574  ment to an asset
-000009e0: 2075 7369 6e67 2069 7427 7320 6e61 6d65   using it's name
-000009f0: 2e20 5468 6520 7363 7269 7074 2077 696c  . The script wil
-00000a00: 6c20 6765 7420 7468 6520 6173 7365 7420  l get the asset 
-00000a10: 6964 2066 726f 6d20 7468 6520 6e61 6d65  id from the name
-00000a20: 2061 7574 6f6d 6174 6963 616c 6c79 2e0a   automatically..
-00000a30: 0a60 6060 6261 7368 0a6a 6972 612d 616d  .```bash.jira-am
-00000a40: 7420 636f 6d6d 656e 7420 3c73 6368 656d  t comment <schem
-00000a50: 613e 203c 6f62 6a65 6374 3e20 3c61 7373  a> <object> <ass
-00000a60: 6574 206e 616d 653e 203c 636f 6d6d 656e  et name> <commen
-00000a70: 743e 0a6a 6972 612d 616d 7420 636f 6d6d  t>.jira-amt comm
-00000a80: 656e 7420 2249 5453 4d22 2022 5365 7276  ent "ITSM" "Serv
-00000a90: 6572 7322 2022 5365 7276 6572 2d31 2220  ers" "Server-1" 
-00000aa0: 2254 6869 7320 6973 2061 2063 6f6d 6d65  "This is a comme
-00000ab0: 6e74 220a 6060 600a 0a2d 2d2d 0a0a 2323  nt".```..---..##
-00000ac0: 2050 6163 6b61 6765 0a0a 596f 7520 6361   Package..You ca
-00000ad0: 6e20 7573 6520 7468 6973 2070 6163 6b61  n use this packa
-00000ae0: 6765 2069 6e20 796f 7572 2063 6f64 6520  ge in your code 
-00000af0: 746f 206d 616e 6167 6520 4a69 7261 2061  to manage Jira a
-00000b00: 7373 6574 732e 0a0a 6060 6070 7974 686f  ssets...```pytho
-00000b10: 6e0a 6672 6f6d 206a 6972 615f 616d 742e  n.from jira_amt.
-00000b20: 6a69 7261 2069 6d70 6f72 7420 4a69 7261  jira import Jira
-00000b30: 4173 7365 7448 616e 646c 6572 0a0a 6a69  AssetHandler..ji
-00000b40: 7261 203d 204a 6972 6141 7373 6574 4861  ra = JiraAssetHa
-00000b50: 6e64 6c65 7228 0a20 2020 2073 6572 7665  ndler(.    serve
-00000b60: 723d 2268 7474 7073 3a2f 2f6a 6972 612e  r="https://jira.
-00000b70: 646f 6d61 696e 2e63 6f6d 222c 0a20 2020  domain.com",.   
-00000b80: 2070 6174 3d22 4142 4344 3132 3334 220a   pat="ABCD1234".
-00000b90: 290a 6060 600a 0a23 2323 2047 6574 2061  ).```..### Get a
-00000ba0: 7373 6574 0a0a 6060 6070 7974 686f 6e0a  sset..```python.
-00000bb0: 6173 7365 7420 3d20 6a69 7261 2e67 6574  asset = jira.get
-00000bc0: 5f61 7373 6574 2822 7363 6865 6d61 222c  _asset("schema",
-00000bd0: 2022 6f62 6a65 6374 222c 2022 6173 7365   "object", "asse
-00000be0: 7427 7320 6e61 6d65 2229 0a60 6060 0a0a  t's name").```..
-00000bf0: 2323 2320 4372 6561 7465 2061 7373 6574  ### Create asset
-00000c00: 0a0a 6060 6070 7974 686f 6e0a 696e 7075  ..```python.inpu
-00000c10: 7420 3d20 7b0a 2020 2020 224e 616d 6522  t = {.    "Name"
-00000c20: 3a20 2253 6572 7665 722d 3122 2c0a 2020  : "Server-1",.  
-00000c30: 2020 2253 7461 7475 7322 3a20 2252 756e    "Status": "Run
-00000c40: 6e69 6e67 222c 0a20 2020 2022 456e 7669  ning",.    "Envi
-00000c50: 726f 6e6d 656e 7422 3a20 2250 726f 6475  ronment": "Produ
-00000c60: 6374 696f 6e22 2c0a 2020 2020 224f 5322  ction",.    "OS"
-00000c70: 3a20 2244 6562 6961 6e22 2c0a 2020 2020  : "Debian",.    
-00000c80: 2249 5022 3a20 2231 2e32 2e33 2e34 220a  "IP": "1.2.3.4".
-00000c90: 7d0a 0a61 7373 6574 203d 206a 6972 612e  }..asset = jira.
-00000ca0: 6372 6561 7465 5f61 7373 6574 2822 7363  create_asset("sc
-00000cb0: 6865 6d61 222c 2022 6f62 6a65 6374 222c  hema", "object",
-00000cc0: 2069 6e70 7574 290a 6060 600a 0a23 2320   input).```..## 
-00000cd0: 5375 7070 6f72 7420 f09f 929b 0a0a 5b21  Support ......[!
-00000ce0: 5b44 6f6e 6174 6520 7769 7468 2042 6974  [Donate with Bit
-00000cf0: 636f 696e 5d28 6874 7470 733a 2f2f 696d  coin](https://im
-00000d00: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000d10: 6765 2f42 6974 636f 696e 2d62 6331 716d  ge/Bitcoin-bc1qm
-00000d20: 6d68 3676 7433 3636 797a 6a74 3367 726a  mh6vt366yzjt3grj
-00000d30: 786a 6a71 796e 7272 7873 3366 7275 6e38  xjjqynrrxs3frun8
-00000d40: 676e 7872 7a2d 6f72 616e 6765 295d 2868  gnxrz-orange)](h
-00000d50: 7474 7073 3a2f 2f64 6f6e 6174 6562 6164  ttps://donatebad
-00000d60: 6765 732e 6972 2f64 6f6e 6174 652f 4269  ges.ir/donate/Bi
-00000d70: 7463 6f69 6e2f 6263 3171 6d6d 6836 7674  tcoin/bc1qmmh6vt
-00000d80: 3336 3679 7a6a 7433 6772 6a78 6a6a 7179  366yzjt3grjxjjqy
-00000d90: 6e72 7278 7333 6672 756e 3867 6e78 727a  nrrxs3frun8gnxrz
-00000da0: 2920 5b21 5b44 6f6e 6174 6520 7769 7468  ) [![Donate with
-00000db0: 2045 7468 6572 6575 6d5d 2868 7474 7073   Ethereum](https
-00000dc0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000dd0: 6f2f 6261 6467 652f 4574 6865 7265 756d  o/badge/Ethereum
-00000de0: 2d30 7830 3833 3162 4437 3245 6138 3930  -0x0831bD72Ea890
-00000df0: 3442 3338 4265 3944 3631 3835 4461 3266  4B38Be9D6185Da2f
-00000e00: 3933 3064 3630 3738 3039 342d 626c 7565  930d6078094-blue
-00000e10: 7669 6f6c 6574 295d 2868 7474 7073 3a2f  violet)](https:/
-00000e20: 2f64 6f6e 6174 6562 6164 6765 732e 6972  /donatebadges.ir
-00000e30: 2f64 6f6e 6174 652f 4574 6865 7265 756d  /donate/Ethereum
-00000e40: 2f30 7830 3833 3162 4437 3245 6138 3930  /0x0831bD72Ea890
-00000e50: 3442 3338 4265 3944 3631 3835 4461 3266  4B38Be9D6185Da2f
-00000e60: 3933 3064 3630 3738 3039 3429 0a0a 3c64  930d6078094)..<d
-00000e70: 6976 3e3c 6120 6872 6566 3d22 6874 7470  iv><a href="http
-00000e80: 733a 2f2f 7061 7970 696e 672e 6972 2f40  s://payping.ir/@
-00000e90: 6861 7461 6d69 6172 6173 6837 223e 3c69  hatamiarash7"><i
-00000ea0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000eb0: 6364 6e2e 7061 7970 696e 672e 6972 2f73  cdn.payping.ir/s
-00000ec0: 7461 7469 6373 2f50 6179 7069 6e67 2d6c  tatics/Payping-l
-00000ed0: 6f67 6f2f 5472 7573 742f 626c 7565 2e73  ogo/Trust/blue.s
-00000ee0: 7667 2220 6865 6967 6874 3d22 3132 3822  vg" height="128"
-00000ef0: 2077 6964 7468 3d22 3132 3822 3e3c 2f61   width="128"></a
-00000f00: 3e3c 2f64 6976 3e0a 0a23 2320 436f 6e74  ></div>..## Cont
-00000f10: 7269 6275 7469 6e67 20f0 9fa4 9d0a 0a44  ributing ......D
-00000f20: 6f6e 2774 2062 6520 7368 7920 616e 6420  on't be shy and 
-00000f30: 7265 6163 6820 6f75 7420 746f 2075 7320  reach out to us 
-00000f40: 6966 2079 6f75 2077 616e 7420 746f 2063  if you want to c
-00000f50: 6f6e 7472 6962 7574 6520 f09f 9889 0a0a  ontribute ......
-00000f60: 312e 2046 6f72 6b20 6974 210a 322e 2043  1. Fork it!.2. C
-00000f70: 7265 6174 6520 796f 7572 2066 6561 7475  reate your featu
-00000f80: 7265 2062 7261 6e63 683a 2060 6769 7420  re branch: `git 
-00000f90: 6368 6563 6b6f 7574 202d 6220 6d79 2d6e  checkout -b my-n
-00000fa0: 6577 2d66 6561 7475 7265 600a 332e 2043  ew-feature`.3. C
-00000fb0: 6f6d 6d69 7420 796f 7572 2063 6861 6e67  ommit your chang
-00000fc0: 6573 3a20 6067 6974 2063 6f6d 6d69 7420  es: `git commit 
-00000fd0: 2d61 6d20 2741 6464 2073 6f6d 6520 6665  -am 'Add some fe
-00000fe0: 6174 7572 6527 600a 342e 2050 7573 6820  ature'`.4. Push 
-00000ff0: 746f 2074 6865 2062 7261 6e63 683a 2060  to the branch: `
-00001000: 6769 7420 7075 7368 206f 7269 6769 6e20  git push origin 
-00001010: 6d79 2d6e 6577 2d66 6561 7475 7265 600a  my-new-feature`.
-00001020: 0a                                       .
+00000590: 434c 492e 0a0a 2d20 5b4a 6972 6120 4173  CLI...- [Jira As
+000005a0: 7365 7420 4d61 6e61 6765 725d 2823 6a69  set Manager](#ji
+000005b0: 7261 2d61 7373 6574 2d6d 616e 6167 6572  ra-asset-manager
+000005c0: 290a 2020 2d20 5b52 6571 7569 7265 6d65  ).  - [Requireme
+000005d0: 6e74 735d 2823 7265 7175 6972 656d 656e  nts](#requiremen
+000005e0: 7473 290a 2020 2d20 5b49 6e73 7461 6c6c  ts).  - [Install
+000005f0: 5d28 2369 6e73 7461 6c6c 290a 2020 2d20  ](#install).  - 
+00000600: 5b48 6f77 2d74 6f5d 2823 686f 772d 746f  [How-to](#how-to
+00000610: 290a 2020 2d20 5b43 4c49 5d28 2363 6c69  ).  - [CLI](#cli
+00000620: 290a 2020 2020 2d20 5b43 7265 6174 6520  ).    - [Create 
+00000630: 6173 7365 7473 5d28 2363 7265 6174 652d  assets](#create-
+00000640: 6173 7365 7473 290a 2020 2020 2d20 5b55  assets).    - [U
+00000650: 7064 6174 6520 6173 7365 7473 5d28 2375  pdate assets](#u
+00000660: 7064 6174 652d 6173 7365 7473 290a 2020  pdate-assets).  
+00000670: 2020 2d20 5b41 6464 2063 6f6d 6d65 6e74    - [Add comment
+00000680: 5d28 2361 6464 2d63 6f6d 6d65 6e74 290a  ](#add-comment).
+00000690: 2020 2d20 5b50 6163 6b61 6765 5d28 2370    - [Package](#p
+000006a0: 6163 6b61 6765 290a 2020 2020 2d20 5b47  ackage).    - [G
+000006b0: 6574 2061 7373 6574 5d28 2367 6574 2d61  et asset](#get-a
+000006c0: 7373 6574 290a 2020 2020 2d20 5b43 7265  sset).    - [Cre
+000006d0: 6174 6520 6173 7365 745d 2823 6372 6561  ate asset](#crea
+000006e0: 7465 2d61 7373 6574 290a 2020 2020 2d20  te-asset).    - 
+000006f0: 5b55 7064 6174 6520 6173 7365 745d 2823  [Update asset](#
+00000700: 7570 6461 7465 2d61 7373 6574 290a 2020  update-asset).  
+00000710: 2020 2d20 5b41 6464 2063 6f6d 6d65 6e74    - [Add comment
+00000720: 5d28 2361 6464 2d63 6f6d 6d65 6e74 2d31  ](#add-comment-1
+00000730: 290a 2020 2d20 5b53 7570 706f 7274 20f0  ).  - [Support .
+00000740: 9f92 9b5d 2823 7375 7070 6f72 742d 290a  ...](#support-).
+00000750: 2020 2d20 5b43 6f6e 7472 6962 7574 696e    - [Contributin
+00000760: 6720 f09f a49d 5d28 2363 6f6e 7472 6962  g ....](#contrib
+00000770: 7574 696e 672d 290a 0a23 2320 5265 7175  uting-)..## Requ
+00000780: 6972 656d 656e 7473 0a0a 2d20 5079 7468  irements..- Pyth
+00000790: 6f6e 2033 2e38 2b0a 0a23 2320 496e 7374  on 3.8+..## Inst
+000007a0: 616c 6c0a 0a60 6060 6261 7368 0a70 6970  all..```bash.pip
+000007b0: 2069 6e73 7461 6c6c 206a 6972 612d 616d   install jira-am
+000007c0: 740a 6060 600a 0a23 2320 486f 772d 746f  t.```..## How-to
+000007d0: 0a0a 596f 7520 6e65 6564 2074 6f20 6164  ..You need to ad
+000007e0: 6420 7468 6573 6520 656e 7669 726f 6e6d  d these environm
+000007f0: 656e 7420 7661 7269 6162 6c65 7320 746f  ent variables to
+00000800: 2075 7365 2074 6865 2043 4c49 3a0a 0a7c   use the CLI:..|
+00000810: 2056 6172 6961 626c 6520 2020 207c 2044   Variable    | D
+00000820: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d    |.| ----------
+00000860: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  - | ------------
+00000870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000890: 2d2d 2d2d 2d2d 207c 0a7c 204a 4952 415f  ------ |.| JIRA_
+000008a0: 5345 5256 4552 207c 204a 6972 6120 7365  SERVER | Jira se
+000008b0: 7276 6572 2061 6464 7265 7373 206c 696b  rver address lik
+000008c0: 6520 6068 7474 7073 3a2f 2f6a 6972 612e  e `https://jira.
+000008d0: 646f 6d61 696e 2e63 6f6d 6020 7c0a 7c20  domain.com` |.| 
+000008e0: 4a49 5241 5f50 4154 2020 2020 7c20 596f  JIRA_PAT    | Yo
+000008f0: 7572 2070 6572 736f 6e61 6c20 6163 6365  ur personal acce
+00000900: 7373 2074 6f6b 656e 2020 2020 2020 2020  ss token        
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 207c 0a0a 4166 7465 7220 7365 7474 696e   |..After settin
+00000930: 6720 7468 6573 6520 7661 7269 6162 6c65  g these variable
+00000940: 732c 2079 6f75 2063 616e 2063 6f6e 6669  s, you can confi
+00000950: 6775 7265 2074 6865 2043 4c49 3a0a 0a60  gure the CLI:..`
+00000960: 6060 6261 7368 0a6a 6972 612d 616d 7420  ``bash.jira-amt 
+00000970: 696e 6974 0a60 6060 0a0a 5468 6973 2063  init.```..This c
+00000980: 6f6d 6d61 6e64 2077 696c 6c20 6765 7420  ommand will get 
+00000990: 6576 6572 7974 6869 6e67 2066 726f 6d20  everything from 
+000009a0: 796f 7572 204a 6972 6120 7365 7276 6572  your Jira server
+000009b0: 2061 6e64 2073 6176 6520 7468 656d 2074   and save them t
+000009c0: 6f20 607e 2f2e 6a69 7261 6020 6469 7265  o `~/.jira` dire
+000009d0: 6374 6f72 7920 666f 7220 6c61 7465 7220  ctory for later 
+000009e0: 7573 652e 2057 6974 6820 7468 6973 2064  use. With this d
+000009f0: 6174 612c 2079 6f75 2064 6f6e 2774 206e  ata, you don't n
+00000a00: 6565 6420 746f 206b 6e6f 772f 7573 6520  eed to know/use 
+00000a10: 4944 206f 6620 6561 6368 2061 7373 6574  ID of each asset
+00000a20: 2f61 7474 7269 6275 7465 2e0a 0a23 2320  /attribute...## 
+00000a30: 434c 490a 0a54 6865 7265 2069 7320 736f  CLI..There is so
+00000a40: 6d65 2063 6f6d 6d61 6e64 7320 746f 206d  me commands to m
+00000a50: 616e 6167 6520 6173 7365 7473 2e20 4368  anage assets. Ch
+00000a60: 6563 6b20 7468 656d 2075 7369 6e67 2074  eck them using t
+00000a70: 6865 2060 2d2d 6865 6c70 6020 666c 6167  he `--help` flag
+00000a80: 2e0a 0a23 2323 2043 7265 6174 6520 6173  ...### Create as
+00000a90: 7365 7473 0a0a 5468 6520 6173 7365 7420  sets..The asset 
+00000aa0: 6372 6561 7469 6f6e 2069 6e20 434c 4920  creation in CLI 
+00000ab0: 6973 206e 6f74 206d 616b 6520 7365 6e73  is not make sens
+00000ac0: 652c 2062 6563 6175 7365 2079 6f75 206e  e, because you n
+00000ad0: 6565 6420 746f 2065 6e74 6572 2061 6c6c  eed to enter all
+00000ae0: 2061 7474 7269 6275 7465 7320 696e 2063   attributes in c
+00000af0: 6f6d 6d61 6e64 206c 696e 652e 2042 7574  ommand line. But
+00000b00: 2079 6f75 2063 616e 2075 7365 2069 7420   you can use it 
+00000b10: 696e 2079 6f75 7220 636f 6465 2e0a 0a23  in your code...#
+00000b20: 2323 2055 7064 6174 6520 6173 7365 7473  ## Update assets
+00000b30: 0a0a 596f 7520 6361 6e20 7570 6461 7465  ..You can update
+00000b40: 2061 7373 6574 2773 2061 7474 7269 6275   asset's attribu
+00000b50: 7465 2075 7369 6e67 2069 7427 7320 6e61  te using it's na
+00000b60: 6d65 2e20 5468 6520 7363 7269 7074 2077  me. The script w
+00000b70: 696c 6c20 6765 7420 7468 6520 6173 7365  ill get the asse
+00000b80: 7420 6964 2066 726f 6d20 7468 6520 6e61  t id from the na
+00000b90: 6d65 2061 7574 6f6d 6174 6963 616c 6c79  me automatically
+00000ba0: 2e0a 0a60 6060 6261 7368 0a6a 6972 612d  ...```bash.jira-
+00000bb0: 616d 7420 6174 7472 203c 7363 6865 6d61  amt attr <schema
+00000bc0: 3e20 3c6f 626a 6563 743e 203c 6173 7365  > <object> <asse
+00000bd0: 7420 6e61 6d65 3e20 3c61 7474 7220 6e61  t name> <attr na
+00000be0: 6d65 3e20 3c61 7474 7220 7661 6c75 653e  me> <attr value>
+00000bf0: 0a6a 6972 612d 616d 7420 6174 7472 2022  .jira-amt attr "
+00000c00: 4954 534d 2220 2253 6572 7665 7273 2220  ITSM" "Servers" 
+00000c10: 2253 6572 7665 722d 3122 2022 4950 2220  "Server-1" "IP" 
+00000c20: 2231 2e32 2e33 2e34 220a 6060 600a 0a23  "1.2.3.4".```..#
+00000c30: 2323 2041 6464 2063 6f6d 6d65 6e74 0a0a  ## Add comment..
+00000c40: 596f 7520 6361 6e20 6164 6420 636f 6d6d  You can add comm
+00000c50: 656e 7420 746f 2061 6e20 6173 7365 7420  ent to an asset 
+00000c60: 7573 696e 6720 6974 2773 206e 616d 652e  using it's name.
+00000c70: 2054 6865 2073 6372 6970 7420 7769 6c6c   The script will
+00000c80: 2067 6574 2074 6865 2061 7373 6574 2069   get the asset i
+00000c90: 6420 6672 6f6d 2074 6865 206e 616d 6520  d from the name 
+00000ca0: 6175 746f 6d61 7469 6361 6c6c 792e 0a0a  automatically...
+00000cb0: 6060 6062 6173 680a 6a69 7261 2d61 6d74  ```bash.jira-amt
+00000cc0: 2063 6f6d 6d65 6e74 203c 7363 6865 6d61   comment <schema
+00000cd0: 3e20 3c6f 626a 6563 743e 203c 6173 7365  > <object> <asse
+00000ce0: 7420 6e61 6d65 3e20 3c63 6f6d 6d65 6e74  t name> <comment
+00000cf0: 3e0a 6a69 7261 2d61 6d74 2063 6f6d 6d65  >.jira-amt comme
+00000d00: 6e74 2022 4954 534d 2220 2253 6572 7665  nt "ITSM" "Serve
+00000d10: 7273 2220 2253 6572 7665 722d 3122 2022  rs" "Server-1" "
+00000d20: 5468 6973 2069 7320 6120 636f 6d6d 656e  This is a commen
+00000d30: 7422 0a60 6060 0a0a 2d2d 2d0a 0a23 2320  t".```..---..## 
+00000d40: 5061 636b 6167 650a 0a59 6f75 2063 616e  Package..You can
+00000d50: 2075 7365 2074 6869 7320 7061 636b 6167   use this packag
+00000d60: 6520 696e 2079 6f75 7220 636f 6465 2074  e in your code t
+00000d70: 6f20 6d61 6e61 6765 204a 6972 6120 6173  o manage Jira as
+00000d80: 7365 7473 2e0a 0a60 6060 7079 7468 6f6e  sets...```python
+00000d90: 0a66 726f 6d20 6a69 7261 5f61 6d74 2e6a  .from jira_amt.j
+00000da0: 6972 6120 696d 706f 7274 204a 6972 6141  ira import JiraA
+00000db0: 7373 6574 4861 6e64 6c65 720a 0a6a 6972  ssetHandler..jir
+00000dc0: 6120 3d20 4a69 7261 4173 7365 7448 616e  a = JiraAssetHan
+00000dd0: 646c 6572 280a 2020 2020 7365 7276 6572  dler(.    server
+00000de0: 3d22 6874 7470 733a 2f2f 6a69 7261 2e64  ="https://jira.d
+00000df0: 6f6d 6169 6e2e 636f 6d22 2c0a 2020 2020  omain.com",.    
+00000e00: 7061 743d 2241 4243 4431 3233 3422 0a29  pat="ABCD1234".)
+00000e10: 0a60 6060 0a0a 2323 2320 4765 7420 6173  .```..### Get as
+00000e20: 7365 740a 0a60 6060 7079 7468 6f6e 0a61  set..```python.a
+00000e30: 7373 6574 203d 206a 6972 612e 6765 745f  sset = jira.get_
+00000e40: 6173 7365 7428 2273 6368 656d 6122 2c20  asset("schema", 
+00000e50: 226f 626a 6563 7422 2c20 2261 7373 6574  "object", "asset
+00000e60: 2773 206e 616d 6522 290a 0a70 7269 6e74  's name")..print
+00000e70: 2861 7373 6574 2e74 6578 7429 0a60 6060  (asset.text).```
+00000e80: 0a0a 2323 2320 4372 6561 7465 2061 7373  ..### Create ass
+00000e90: 6574 0a0a 6060 6070 7974 686f 6e0a 696e  et..```python.in
+00000ea0: 7075 7420 3d20 7b0a 2020 2020 224e 616d  put = {.    "Nam
+00000eb0: 6522 3a20 2253 6572 7665 722d 3122 2c0a  e": "Server-1",.
+00000ec0: 2020 2020 2253 7461 7475 7322 3a20 2252      "Status": "R
+00000ed0: 756e 6e69 6e67 222c 0a20 2020 2022 456e  unning",.    "En
+00000ee0: 7669 726f 6e6d 656e 7422 3a20 2250 726f  vironment": "Pro
+00000ef0: 6475 6374 696f 6e22 2c0a 2020 2020 224f  duction",.    "O
+00000f00: 5322 3a20 2244 6562 6961 6e22 2c0a 2020  S": "Debian",.  
+00000f10: 2020 2249 5022 3a20 2231 2e32 2e33 2e34    "IP": "1.2.3.4
+00000f20: 220a 7d0a 0a61 7373 6574 203d 206a 6972  ".}..asset = jir
+00000f30: 612e 6372 6561 7465 5f61 7373 6574 2822  a.create_asset("
+00000f40: 7363 6865 6d61 222c 2022 6f62 6a65 6374  schema", "object
+00000f50: 222c 2069 6e70 7574 290a 6060 600a 0a23  ", input).```..#
+00000f60: 2323 2055 7064 6174 6520 6173 7365 740a  ## Update asset.
+00000f70: 0a60 6060 7079 7468 6f6e 0a61 7373 6574  .```python.asset
+00000f80: 203d 206a 6972 612e 6765 745f 6173 7365   = jira.get_asse
+00000f90: 7428 2273 6368 656d 6122 2c20 226f 626a  t("schema", "obj
+00000fa0: 6563 7422 2c20 2261 7373 6574 2773 206e  ect", "asset's n
+00000fb0: 616d 6522 290a 0a70 7269 6e74 2861 7373  ame")..print(ass
+00000fc0: 6574 2e74 6578 7429 0a60 6060 0a0a 2323  et.text).```..##
+00000fd0: 2320 4164 6420 636f 6d6d 656e 740a 0a60  # Add comment..`
+00000fe0: 6060 7079 7468 6f6e 0a72 6573 756c 7420  ``python.result 
+00000ff0: 3d20 6a69 7261 2e61 6464 5f63 6f6d 6d65  = jira.add_comme
+00001000: 6e74 2822 7363 6865 6d61 222c 2022 6f62  nt("schema", "ob
+00001010: 6a65 6374 222c 2022 6173 7365 7427 7320  ject", "asset's 
+00001020: 6e61 6d65 222c 2022 636f 6d6d 656e 7422  name", "comment"
+00001030: 290a 0a70 7269 6e74 2872 6573 756c 742e  )..print(result.
+00001040: 7374 6174 7573 5f63 6f64 6529 0a60 6060  status_code).```
+00001050: 0a0a 2323 2053 7570 706f 7274 20f0 9f92  ..## Support ...
+00001060: 9b0a 0a5b 215b 446f 6e61 7465 2077 6974  ...[![Donate wit
+00001070: 6820 4269 7463 6f69 6e5d 2868 7474 7073  h Bitcoin](https
+00001080: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001090: 6f2f 6261 6467 652f 4269 7463 6f69 6e2d  o/badge/Bitcoin-
+000010a0: 6263 3171 6d6d 6836 7674 3336 3679 7a6a  bc1qmmh6vt366yzj
+000010b0: 7433 6772 6a78 6a6a 7179 6e72 7278 7333  t3grjxjjqynrrxs3
+000010c0: 6672 756e 3867 6e78 727a 2d6f 7261 6e67  frun8gnxrz-orang
+000010d0: 6529 5d28 6874 7470 733a 2f2f 646f 6e61  e)](https://dona
+000010e0: 7465 6261 6467 6573 2e69 722f 646f 6e61  tebadges.ir/dona
+000010f0: 7465 2f42 6974 636f 696e 2f62 6331 716d  te/Bitcoin/bc1qm
+00001100: 6d68 3676 7433 3636 797a 6a74 3367 726a  mh6vt366yzjt3grj
+00001110: 786a 6a71 796e 7272 7873 3366 7275 6e38  xjjqynrrxs3frun8
+00001120: 676e 7872 7a29 205b 215b 446f 6e61 7465  gnxrz) [![Donate
+00001130: 2077 6974 6820 4574 6865 7265 756d 5d28   with Ethereum](
+00001140: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001150: 6c64 732e 696f 2f62 6164 6765 2f45 7468  lds.io/badge/Eth
+00001160: 6572 6575 6d2d 3078 3038 3331 6244 3732  ereum-0x0831bD72
+00001170: 4561 3839 3034 4233 3842 6539 4436 3138  Ea8904B38Be9D618
+00001180: 3544 6132 6639 3330 6436 3037 3830 3934  5Da2f930d6078094
+00001190: 2d62 6c75 6576 696f 6c65 7429 5d28 6874  -blueviolet)](ht
+000011a0: 7470 733a 2f2f 646f 6e61 7465 6261 6467  tps://donatebadg
+000011b0: 6573 2e69 722f 646f 6e61 7465 2f45 7468  es.ir/donate/Eth
+000011c0: 6572 6575 6d2f 3078 3038 3331 6244 3732  ereum/0x0831bD72
+000011d0: 4561 3839 3034 4233 3842 6539 4436 3138  Ea8904B38Be9D618
+000011e0: 3544 6132 6639 3330 6436 3037 3830 3934  5Da2f930d6078094
+000011f0: 290a 0a3c 6469 763e 3c61 2068 7265 663d  )..<div><a href=
+00001200: 2268 7474 7073 3a2f 2f70 6179 7069 6e67  "https://payping
+00001210: 2e69 722f 4068 6174 616d 6961 7261 7368  .ir/@hatamiarash
+00001220: 3722 3e3c 696d 6720 7372 633d 2268 7474  7"><img src="htt
+00001230: 7073 3a2f 2f63 646e 2e70 6179 7069 6e67  ps://cdn.payping
+00001240: 2e69 722f 7374 6174 6963 732f 5061 7970  .ir/statics/Payp
+00001250: 696e 672d 6c6f 676f 2f54 7275 7374 2f62  ing-logo/Trust/b
+00001260: 6c75 652e 7376 6722 2068 6569 6768 743d  lue.svg" height=
+00001270: 2231 3238 2220 7769 6474 683d 2231 3238  "128" width="128
+00001280: 223e 3c2f 613e 3c2f 6469 763e 0a0a 2323  "></a></div>..##
+00001290: 2043 6f6e 7472 6962 7574 696e 6720 f09f   Contributing ..
+000012a0: a49d 0a0a 446f 6e27 7420 6265 2073 6879  ....Don't be shy
+000012b0: 2061 6e64 2072 6561 6368 206f 7574 2074   and reach out t
+000012c0: 6f20 7573 2069 6620 796f 7520 7761 6e74  o us if you want
+000012d0: 2074 6f20 636f 6e74 7269 6275 7465 20f0   to contribute .
+000012e0: 9f98 890a 0a31 2e20 466f 726b 2069 7421  .....1. Fork it!
+000012f0: 0a32 2e20 4372 6561 7465 2079 6f75 7220  .2. Create your 
+00001300: 6665 6174 7572 6520 6272 616e 6368 3a20  feature branch: 
+00001310: 6067 6974 2063 6865 636b 6f75 7420 2d62  `git checkout -b
+00001320: 206d 792d 6e65 772d 6665 6174 7572 6560   my-new-feature`
+00001330: 0a33 2e20 436f 6d6d 6974 2079 6f75 7220  .3. Commit your 
+00001340: 6368 616e 6765 733a 2060 6769 7420 636f  changes: `git co
+00001350: 6d6d 6974 202d 616d 2027 4164 6420 736f  mmit -am 'Add so
+00001360: 6d65 2066 6561 7475 7265 2760 0a34 2e20  me feature'`.4. 
+00001370: 5075 7368 2074 6f20 7468 6520 6272 616e  Push to the bran
+00001380: 6368 3a20 6067 6974 2070 7573 6820 6f72  ch: `git push or
+00001390: 6967 696e 206d 792d 6e65 772d 6665 6174  igin my-new-feat
+000013a0: 7572 6560 0a0a                           ure`..
```

