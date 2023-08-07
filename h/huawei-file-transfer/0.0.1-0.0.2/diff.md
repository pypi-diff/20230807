# Comparing `tmp/huawei_file_transfer-0.0.1.tar.gz` & `tmp/huawei_file_transfer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei_file_transfer-0.0.1.tar", last modified: Fri Aug  4 05:24:52 2023, max compression
+gzip compressed data, was "huawei_file_transfer-0.0.2.tar", last modified: Mon Aug  7 07:51:33 2023, max compression
```

## Comparing `huawei_file_transfer-0.0.1.tar` & `huawei_file_transfer-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 05:24:52.501287 huawei_file_transfer-0.0.1/
--rw-rw-rw-   0        0        0     1073 2023-08-04 02:01:25.000000 huawei_file_transfer-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3883 2023-08-04 05:24:52.502284 huawei_file_transfer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3318 2023-08-04 04:40:45.000000 huawei_file_transfer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 05:24:52.482338 huawei_file_transfer-0.0.1/huawei_file_transfer/
--rw-rw-rw-   0        0        0     5400 2023-08-04 02:31:22.000000 huawei_file_transfer-0.0.1/huawei_file_transfer/__init__.py
--rw-rw-rw-   0        0        0    15508 2023-08-04 02:34:42.000000 huawei_file_transfer-0.0.1/huawei_file_transfer/custom_huawei.py
--rw-rw-rw-   0        0        0    18205 2023-08-04 02:27:21.000000 huawei_file_transfer-0.0.1/huawei_file_transfer/custom_ssh_dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-08-04 05:24:52.498295 huawei_file_transfer-0.0.1/huawei_file_transfer.egg-info/
--rw-rw-rw-   0        0        0     3883 2023-08-04 05:24:52.000000 huawei_file_transfer-0.0.1/huawei_file_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-08-04 05:24:52.000000 huawei_file_transfer-0.0.1/huawei_file_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 05:24:52.000000 huawei_file_transfer-0.0.1/huawei_file_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-08-04 05:24:52.000000 huawei_file_transfer-0.0.1/huawei_file_transfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-04 05:24:52.503281 huawei_file_transfer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-08-04 05:23:27.000000 huawei_file_transfer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:51:33.823170 huawei_file_transfer-0.0.2/
+-rw-rw-rw-   0        0        0     1073 2023-08-04 02:01:25.000000 huawei_file_transfer-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3901 2023-08-07 07:51:33.824171 huawei_file_transfer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3318 2023-08-04 04:40:45.000000 huawei_file_transfer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:51:33.809206 huawei_file_transfer-0.0.2/huawei_file_transfer/
+-rw-rw-rw-   0        0        0     6057 2023-08-07 06:43:45.000000 huawei_file_transfer-0.0.2/huawei_file_transfer/__init__.py
+-rw-rw-rw-   0        0        0    16233 2023-08-07 07:44:29.000000 huawei_file_transfer-0.0.2/huawei_file_transfer/custom_huawei.py
+-rw-rw-rw-   0        0        0    18205 2023-08-04 02:27:21.000000 huawei_file_transfer-0.0.2/huawei_file_transfer/custom_ssh_dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:51:33.821174 huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/
+-rw-rw-rw-   0        0        0     3901 2023-08-07 07:51:33.000000 huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-08-07 07:51:33.000000 huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:51:33.000000 huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 07:51:33.000000 huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-07 07:51:33.000000 huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-07 07:51:33.825166 huawei_file_transfer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-08-07 06:54:21.000000 huawei_file_transfer-0.0.2/setup.py
```

### Comparing `huawei_file_transfer-0.0.1/LICENSE.txt` & `huawei_file_transfer-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huawei_file_transfer-0.0.1/PKG-INFO` & `huawei_file_transfer-0.0.2/huawei_file_transfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: huawei_file_transfer
-Version: 0.0.1
-Summary: huawei_file_transfer huawei_file_transfer is a Netmiko-based function that provides file transfer capabilities for Huawei devices
+Name: huawei-file-transfer
+Version: 0.0.2
+Summary: huawei_file_transfer-V0.0.2 huawei_file_transfer-V0.0.2 is a Netmiko-based function that provides file transfer capabilities for Huawei devices
 Home-page: https://github.com/ranmaolin/huawei_file_transfer
 Author: RanMaoLin
 Author-email: 809780971@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <img src="https://img.shields.io/badge/Python-3.6-blue.svg">
 <img src="https://img.shields.io/badge/Python-3.7-blue.svg">
 <img src="https://img.shields.io/badge/Python-3.8-blue.svg">
 <img src="https://img.shields.io/badge/Python-3.9-blue.svg">
```

### Comparing `huawei_file_transfer-0.0.1/README.md` & `huawei_file_transfer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `huawei_file_transfer-0.0.1/huawei_file_transfer/__init__.py` & `huawei_file_transfer-0.0.2/huawei_file_transfer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         "file_verified": False,
     }
     nottransferred_but_verified = {
         "file_exists": True,
         "file_transferred": False,
         "file_verified": True,
     }
+    if "huawei" in ssh_conn.device_type:
+        huawei = True
+    else:
+        huawei = False
     if "cisco_ios" in ssh_conn.device_type or "cisco_xe" in ssh_conn.device_type:
         cisco_ios = True
     else:
         cisco_ios = False
     if not cisco_ios and inline_transfer:
         raise ValueError("Inline Transfer only supported for Cisco IOS/Cisco IOS-XE")
 
@@ -127,17 +131,22 @@
                         return nottransferred_but_verified
                     else:
                         # File exists, you can overwrite it, MD5 is wrong (transfer file)
                         verifyspace_and_transferfile(scp_transfer)
                         if scp_transfer.verify_file():
                             return transferred_and_verified
                         else:
-                            raise ValueError(
-                                "MD5 failure between source and destination files"
-                            )
+                            if huawei:
+                                raise ValueError(
+                                    "Size_check failure between source and destination files"
+                                )
+                            else:
+                                raise ValueError(
+                                    "MD5 failure between source and destination files"
+                                )
                 else:
                     # File exists, you can overwrite it, but MD5 not allowed (transfer file)
                     verifyspace_and_transferfile(scp_transfer)
                     return transferred_and_notverified
             else:
                 # File exists, but you can't overwrite it.
                 if verify_file:
@@ -145,13 +154,19 @@
                         return nottransferred_but_verified
                 msg = "File already exists and overwrite_file is disabled"
                 raise ValueError(msg)
         else:
             verifyspace_and_transferfile(scp_transfer)
             # File doesn't exist
             if verify_file:
-                if scp_transfer.verify_file():
-                    return transferred_and_verified
+                if huawei:
+                    if scp_transfer.verify_file():
+                        return transferred_and_verified
+                    else:
+                        raise ValueError("size_check failure between source and destination files")
                 else:
-                    raise ValueError("MD5 failure between source and destination files")
+                    if scp_transfer.verify_file():
+                        return transferred_and_verified
+                    else:
+                        raise ValueError("MD5 failure between source and destination files")
             else:
                 return transferred_and_notverified
```

### Comparing `huawei_file_transfer-0.0.1/huawei_file_transfer/custom_huawei.py` & `huawei_file_transfer-0.0.2/huawei_file_transfer/custom_huawei.py`

 * *Files 3% similar despite different names*

```diff
@@ -339,40 +339,41 @@
             remote_cmd = f"dir {self.file_system}/{remote_file}"
 
         remote_out = self.ssh_ctl_chan._send_command_str(remote_cmd)
         if re.search("Such file or path doesn't exist", remote_out, flags=re.I):
             raise IOError("Unable to find file on remote system")
         # Match line containing file name
         escape_file_name = re.escape(remote_file)
-        pattern = r".*({}).*".format(escape_file_name)
+        huawei_size_pattern = "(\d+((\,){0,1}\d+){0,3})"
+        pattern = r"\d+\s+\S+\s+({}).*({}).*".format(huawei_size_pattern, escape_file_name)
         match = re.search(pattern, remote_out)
         if match:
-            file_size = match.group(0)
-            file_size = file_size.split()[0]
+            file_size = match.group(1)
+            file_size = file_size.replace(",", "")
             return int(file_size)
 
         raise IOError("Unable to find file on remote system")
 
-    @staticmethod
-    def process_md5(md5_output: str, pattern: str = r"= (.*)") -> str:
-        """Not needed on NX-OS."""
-        raise NotImplementedError
-
-    def remote_md5(
-            self, base_cmd: str = "show file", remote_file: Optional[str] = None
-    ) -> str:
-        if remote_file is None:
-            if self.direction == "put":
-                remote_file = self.dest_file
-            elif self.direction == "get":
-                remote_file = self.source_file
-        remote_md5_cmd = f"{base_cmd} {self.file_system}{remote_file} md5sum"
-        output = self.ssh_ctl_chan._send_command_str(remote_md5_cmd, read_timeout=300)
-        output = output.strip()
-        return output
+    # @staticmethod
+    # def process_md5(md5_output: str, pattern: str = r"= (.*)") -> str:
+    #     """Not needed on NX-OS."""
+    #     raise NotImplementedError
+
+    # def remote_md5(
+    #         self, base_cmd: str = "show file", remote_file: Optional[str] = None
+    # ) -> str:
+    #     if remote_file is None:
+    #         if self.direction == "put":
+    #             remote_file = self.dest_file
+    #         elif self.direction == "get":
+    #             remote_file = self.source_file
+    #     remote_md5_cmd = f"{base_cmd} {self.file_system}{remote_file} md5sum"
+    #     output = self.ssh_ctl_chan._send_command_str(remote_md5_cmd, read_timeout=300)
+    #     output = output.strip()
+    #     return output
 
     def enable_scp(self, cmd: str = "") -> None:
         raise NotImplementedError
 
     def disable_scp(self, cmd: str = "") -> None:
         raise NotImplementedError
 
@@ -409,7 +410,20 @@
         if self.direction == "put":
             space_avail = self.remote_space_available(search_pattern=search_pattern)
         elif self.direction == "get":
             space_avail = self.local_space_available()
         if space_avail > self.file_size:
             return True
         return False
+
+    def verify_file(self):
+        """Verify the file has been transferred correctly."""
+        return self.compare_size()
+    
+    def compare_size(self):
+        """Compare size of file on network device to size of local file."""
+        if self.direction == "put":
+            remote_size = self.remote_file_size(remote_file=self.dest_file)
+            return os.stat(self.source_file).st_size == remote_size
+        elif self.direction == "get":
+            local_size = self.remote_file_size(remote_file=self.source_file)
+            return os.stat(self.dest_file).st_size == local_size
```

### Comparing `huawei_file_transfer-0.0.1/huawei_file_transfer/custom_ssh_dispatcher.py` & `huawei_file_transfer-0.0.2/huawei_file_transfer/custom_ssh_dispatcher.py`

 * *Files identical despite different names*

### Comparing `huawei_file_transfer-0.0.1/huawei_file_transfer.egg-info/PKG-INFO` & `huawei_file_transfer-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: huawei-file-transfer
-Version: 0.0.1
-Summary: huawei_file_transfer huawei_file_transfer is a Netmiko-based function that provides file transfer capabilities for Huawei devices
+Name: huawei_file_transfer
+Version: 0.0.2
+Summary: huawei_file_transfer-V0.0.2 huawei_file_transfer-V0.0.2 is a Netmiko-based function that provides file transfer capabilities for Huawei devices
 Home-page: https://github.com/ranmaolin/huawei_file_transfer
 Author: RanMaoLin
 Author-email: 809780971@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <img src="https://img.shields.io/badge/Python-3.6-blue.svg">
 <img src="https://img.shields.io/badge/Python-3.7-blue.svg">
 <img src="https://img.shields.io/badge/Python-3.8-blue.svg">
 <img src="https://img.shields.io/badge/Python-3.9-blue.svg">
```

### Comparing `huawei_file_transfer-0.0.1/setup.py` & `huawei_file_transfer-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="huawei_file_transfer",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",  # 包版本号，便于维护版本
+    version="0.0.2",  # 包版本号，便于维护版本
     author="RanMaoLin",  # 作者，可以写自己的姓名
     author_email="809780971@qq.com",  # 作者联系方式，可写自己的邮箱地址
-    description="huawei_file_transfer huawei_file_transfer is a Netmiko-based function that provides file transfer capabilities for Huawei devices",  # 包的简述
+    description="huawei_file_transfer-V0.0.2 huawei_file_transfer-V0.0.2 is a Netmiko-based function that provides file transfer capabilities for Huawei devices",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/ranmaolin/huawei_file_transfer",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',  # 对python的最低版本要求
+    install_requires=[
+        'netmiko>=4.2.0'
+        ],
+    python_requires='>=3.7, <4',  # 对python的最低版本要求
 )
```

