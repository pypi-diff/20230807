# Comparing `tmp/biliarchiver-0.0.36.tar.gz` & `tmp/biliarchiver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliarchiver-0.0.36.tar", max compression
+gzip compressed data, was "biliarchiver-0.0.9.tar", max compression
```

## Comparing `biliarchiver-0.0.36.tar` & `biliarchiver-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,13 @@
--rw-r--r--   0        0        0      131 2023-07-07 09:38:51.631616 biliarchiver-0.0.36/README.md
--rw-r--r--   0        0        0    10869 2023-08-04 15:37:39.781354 biliarchiver-0.0.36/biliarchiver/_biliarchiver_upload_bvid.py
--rw-r--r--   0        0        0    12676 2023-07-27 08:51:31.836489 biliarchiver-0.0.36/biliarchiver/archive_bvid.py
--rw-r--r--   0        0        0     9645 2023-08-04 11:34:54.426941 biliarchiver-0.0.36/biliarchiver/cli_tools/bili_archive_bvids.py
--rw-r--r--   0        0        0     9307 2023-07-28 09:27:19.771125 biliarchiver-0.0.36/biliarchiver/cli_tools/bili_get_bvids.py
--rw-r--r--   0        0        0     2522 2023-07-23 08:20:04.085341 biliarchiver-0.0.36/biliarchiver/cli_tools/bili_upload.py
--rw-r--r--   0        0        0      413 2023-07-07 09:38:51.635616 biliarchiver-0.0.36/biliarchiver/cli_tools/biliarchiver.py
--rw-r--r--   0        0        0     2221 2023-07-20 09:58:51.188806 biliarchiver-0.0.36/biliarchiver/config.py
--rw-r--r--   0        0        0      577 2023-07-27 14:47:04.901042 biliarchiver-0.0.36/biliarchiver/exception.py
--rw-r--r--   0        0        0     3105 2023-08-04 15:04:00.580371 biliarchiver-0.0.36/biliarchiver/utils/dirLock.py
--rw-r--r--   0        0        0      237 2023-07-07 09:38:51.635616 biliarchiver-0.0.36/biliarchiver/utils/ffmpeg.py
--rw-r--r--   0        0        0     1085 2023-07-18 04:24:04.652661 biliarchiver-0.0.36/biliarchiver/utils/http_patch.py
--rw-r--r--   0        0        0     1278 2023-07-07 09:38:51.635616 biliarchiver-0.0.36/biliarchiver/utils/identifier.py
--rw-r--r--   0        0        0      690 2023-07-24 14:21:52.343746 biliarchiver-0.0.36/biliarchiver/utils/storage.py
--rw-r--r--   0        0        0     1606 2023-07-25 18:36:58.299641 biliarchiver-0.0.36/biliarchiver/utils/version_check.py
--rw-r--r--   0        0        0     2783 2023-08-07 10:03:42.710435 biliarchiver-0.0.36/biliarchiver/utils/xml_chars.py
--rw-r--r--   0        0        0       32 2023-08-07 10:04:37.597941 biliarchiver-0.0.36/biliarchiver/version.py
--rw-r--r--   0        0        0      665 2023-08-07 10:04:32.797635 biliarchiver-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 biliarchiver-0.0.36/setup.py
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 biliarchiver-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.9/README.md
+-rw-r--r--   0        0        0     7575 2023-06-06 19:48:46.123664 biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py
+-rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.9/biliarchiver/archive_bvid.py
+-rw-r--r--   0        0        0     4734 2023-06-07 04:48:33.598085 biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py
+-rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py
+-rw-r--r--   0        0        0     1490 2023-06-07 04:52:11.184454 biliarchiver-0.0.9/biliarchiver/bili_uploade.py
+-rw-r--r--   0        0        0     2018 2023-06-06 19:20:55.302758 biliarchiver-0.0.9/biliarchiver/config.py
+-rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.9/biliarchiver/utils/dirLock.py
+-rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.9/biliarchiver/utils/string.py
+-rw-r--r--   0        0        0       31 2023-06-06 19:35:41.648702 biliarchiver-0.0.9/biliarchiver/version.py
+-rw-r--r--   0        0        0      530 2023-06-07 04:58:02.482737 biliarchiver-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/PKG-INFO
```

### Comparing `biliarchiver-0.0.36/biliarchiver/_biliarchiver_upload_bvid.py` & `biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,96 @@
 import json
 import os
-from pathlib import Path, PurePath
+from pathlib import Path
 import time
-from typing import List
-from urllib.parse import urlparse
 from internetarchive import get_item
 from requests import Response
 from rich import print
-from biliarchiver.exception import VideosBasePathNotFoundError, VideosNotFinishedDownloadError
 
-from biliarchiver.utils.identifier import human_readable_upper_part_map
+from biliarchiver.utils.string import human_readable_upper_part_map
 from biliarchiver.config import BILIBILI_IDENTIFIER_PERFIX, config
 from biliarchiver.utils.dirLock import UploadLock, AlreadyRunningError
-from biliarchiver.utils.xml_chars import xml_chars_legalize
 from biliarchiver.version import BILI_ARCHIVER_VERSION
 
-def upload_bvid(bvid: str, *, update_existing: bool = False, collection: str):
+def upload_bvid(bvid):
     try:
         lock_dir = config.storage_home_dir / '.locks' / bvid
         os.makedirs(lock_dir, exist_ok=True)
         with UploadLock(lock_dir): # type: ignore
-            _upload_bvid(bvid, update_existing=update_existing, collection=collection)
+            _upload_bvid(bvid)
     except AlreadyRunningError:
         print(f'已经有一个上传 {bvid} 的进程在运行，跳过')
-    except VideosBasePathNotFoundError:
-        print(f'没有找到 {bvid} 对应的文件夹。可能是因已存在 IA item 而跳过了下载，或者你传入了错误的 bvid')
-    except VideosNotFinishedDownloadError:
-        print(f'{bvid} 的视频还没有下载完成，跳过')
     except Exception as e:
         print(f'上传 {bvid} 时出错：')
         raise e
 
-def _upload_bvid(bvid: str, *, update_existing: bool = False, collection: str):
+def _upload_bvid(bvid: str):
     access_key, secret_key = read_ia_keys(config.ia_key_file)
 
     # identifier format: BiliBili-{bvid}_p{pid}-{upper_part} 
     upper_part = human_readable_upper_part_map(string=bvid, backward=True)
     OLD_videos_basepath: Path = config.storage_home_dir / 'videos' / bvid
     videos_basepath: Path = config.storage_home_dir / 'videos' / f'{bvid}-{upper_part}'
-
     if os.path.exists(OLD_videos_basepath):
         print(f'检测到旧的视频主目录 {OLD_videos_basepath}，将其重命名为 {videos_basepath}...')
         os.rename(OLD_videos_basepath, videos_basepath)
-
-    if not os.path.exists(videos_basepath):
-        raise VideosBasePathNotFoundError(f'{videos_basepath}')
-    if not (videos_basepath / "_all_downloaded.mark").exists():
-        raise VideosNotFinishedDownloadError(f'{videos_basepath}')
-
     for local_identifier in os.listdir(videos_basepath):
         remote_identifier = f'{local_identifier}-{upper_part}'
-        if os.path.exists(f'{videos_basepath}/{local_identifier}/_uploaded.mark') and not update_existing:
+        if os.path.exists(f'{videos_basepath}/{local_identifier}/_uploaded.mark'):
             print(f'{local_identifier} => {remote_identifier} 已经上传过了(_uploaded.mark)')
             continue
         if local_identifier.startswith('_') :
-            print(f'跳过带 _ 前缀的 local_identifier: {local_identifier}')
+            print(f'跳过 {local_identifier}')
             continue
         if not local_identifier.startswith(BILIBILI_IDENTIFIER_PERFIX):
             print(f'{local_identifier} 不是以 {BILIBILI_IDENTIFIER_PERFIX} 开头的正确 local_identifier')
             continue
         if not os.path.exists(f'{videos_basepath}/{local_identifier}/_downloaded.mark'):
             print(f'{local_identifier} 没有下载完成')
             continue
 
         pid = local_identifier.split('_')[-1][1:]
         file_basename = local_identifier[len(BILIBILI_IDENTIFIER_PERFIX)+1:]
 
         print(f'=== 开始上传 {local_identifier} => {remote_identifier} ===')
         item = get_item(remote_identifier)
-        if item.exists and not update_existing:
+        if item.exists:
             print(f'item {remote_identifier} 已存在(item.exists)')
             if item.metadata.get("upload-state") == "uploaded":
                 print(f'{remote_identifier} 已经上传过了，跳过(item.metadata.uploaded)')
                 with open(f'{videos_basepath}/{local_identifier}/_uploaded.mark', 'w', encoding='utf-8') as f:
                     f.write('')
                 continue
-        with open(f'{videos_basepath}/{local_identifier}/extra/{file_basename}.info.json', 'r', encoding='utf-8') as f:
-            bv_info = json.load(f)
-
-        cover_url: str = bv_info['data']['View']['pic']
-        cover_suffix = PurePath(urlparse(cover_url).path).suffix
-
         filedict = {} # "remote filename": "local filename"
         for filename in os.listdir(f'{videos_basepath}/{local_identifier}/extra'):
             file = f'{videos_basepath}/{local_identifier}/extra/{filename}'
             if os.path.isfile(file):
                 if file.startswith('_'):
                     continue
                 filedict[filename] = file
-                
-                # 复制一份 cover 作为 itemimage
-                if filename == f'{bvid}_p{pid}{cover_suffix}':
-                    filedict[f'{bvid}_p{pid}_itemimage{cover_suffix}'] = file
 
         for filename in os.listdir(f'{videos_basepath}/{local_identifier}'):
             file = f'{videos_basepath}/{local_identifier}/{filename}'
             if os.path.isfile(file):
                 if os.path.basename(file).startswith('_'):
                     continue
                 if not os.path.isfile(file):
-                   continue
+                    continue
                 filedict[filename] = file
-
-        assert (f'{file_basename}.mp4' in filedict) or (f'{file_basename}.flv' in filedict)
-
+        
 
         # IA 去重
         for file_in_item in item.files:
             if file_in_item["name"] in filedict:
                 filedict.pop(file_in_item["name"])
                 print(f"File {file_in_item['name']} already exists in {remote_identifier}.")
 
 
+        with open(f'{videos_basepath}/{local_identifier}/extra/{file_basename}.info.json', 'r', encoding='utf-8') as f:
+            bv_info = json.load(f)
         # with open(f'{videos_basepath}/_videos_info.json', 'r', encoding='utf-8') as f:
         #     videos_info = json.load(f)
 
         tags = ['BiliBili', 'video']
         for tag in bv_info['data']['Tags']:
             tags.append(tag['tag_name'])
         pubdate = bv_info['data']['View']['pubdate']
@@ -126,107 +101,66 @@
                 cid = page['cid']
                 p_part = page['part']
                 break
 
         assert cid is not None
         assert p_part is not None
 
-        aid = bv_info['data']['View']['aid']
-        owner_mid = bv_info['data']['View']['owner']['mid']
-        owner_creator: str = bv_info['data']['View']['owner']['name'] # UP 主
-
-        mids: List[int] = [owner_mid]
-        creators: List[str] = [owner_creator]
-        if bv_info['data']['View'].get('staff') is not None:
-            mids = [] # owner_mid 在 staff 也有
-            creators = []
-            for staff in bv_info['data']['View']['staff']:
-                mids.append(staff['mid']) if staff['mid'] not in mids else None
-                creators.append(staff['name']) if staff['name'] not in creators else None
-        external_identifier = [f"urn:bilibili:video:aid:{aid}",
-                               f"urn:bilibili:video:bvid:{bvid}",
-                               f"urn:bilibili:video:cid:{cid}"]
-        for mid in mids:
-            external_identifier.append(f"urn:bilibili:video:mid:{mid}")
-
         md = {
             "mediatype": "movies",
-            "collection": collection,
+            "collection": 'opensource_movies',
             "title": bv_info['data']['View']['title'] + f' P{pid} ' + p_part ,
             "description": remote_identifier + ' uploading...',
-            'creator': creators if len(creators) > 1 else owner_creator, # type: list[str] | str
+            'creator': bv_info['data']['View']['owner']['name'], # UP 主
             # UTC time
-            'date': time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(pubdate)),
+            'date': time.strftime("%Y-%m-%d", time.gmtime(pubdate)),
             'year': time.strftime("%Y", time.gmtime(pubdate)),
-            # 'aid': aid,
-            # 'bvid': bvid,
-            # 'cid': cid,
-            # 'mid': mid,
-            "external-identifier": external_identifier,
+            'aid': bv_info['data']['View']['aid'],
+            'bvid': bvid,
+            'cid': cid,
+            'mid': bv_info['data']['View']['owner']['mid'],
             "subject": "; ".join(
                 tags
             ),  # Keywords should be separated by ; but it doesn't matter much; the alternative is to set one per field with subject[0], subject[1], ...
             "upload-state": "uploading",
             'originalurl': f'https://www.bilibili.com/video/{bvid}/?p={pid}',
             'scanner': f'biliarchiver v{BILI_ARCHIVER_VERSION} (dev)',
         }
-
         print(filedict)
         print(md)
 
-        # remove XML illegal characters
-        _md_before = hash(json.dumps(md))
-        md = xml_chars_legalize(obj=md)
-        assert isinstance(md, dict)
-        if hash(json.dumps(md)) != _md_before:
-            print(f"Removed XML illegal characters from metadata, cleaned metadata:")
-            print(md)
-
         if filedict:
             r = item.upload(
                 files=filedict,
                 metadata=md,
                 access_key=access_key,
                 secret_key=secret_key,
                 verbose=True,
                 queue_derive=True,
                 retries=5,
             )
 
-        tries = 100
+        tries = 30
         item = get_item(remote_identifier) # refresh item
         while not item.exists and tries > 0:
             print(f"Waiting for item to be created ({tries})  ...", end='\r')
             time.sleep(30)
             item = get_item(remote_identifier)
             tries -= 1
 
         new_md = {}
         if item.metadata.get("upload-state") != "uploaded":
-            new_md["upload-state"] = "uploaded"
-        if item.metadata.get("creator") != md['creator']:
-            new_md["creator"] = md['creator']
-        if item.metadata.get("description", "") != bv_info['data']['View']['desc']:
-            new_md["description"] = bv_info['data']['View']['desc']
+            new_md.update({"upload-state": "uploaded"})
+        if item.metadata.get("description") != bv_info['data']['View']['desc']:
+            new_md.update({"description": bv_info['data']['View']['desc']})
         if item.metadata.get("scanner") != md['scanner']:
-            new_md["scanner"] = md['scanner']
-        if item.metadata.get("external-identifier") != md['external-identifier']:
-            new_md["external-identifier"] = md['external-identifier']
+            new_md.update({"scanner": md['scanner']})
         if new_md:
             print(f"Updating metadata:")
             print(new_md)
-
-            # remove XML illegal characters
-            _md_before = hash(json.dumps(new_md))
-            new_md = xml_chars_legalize(obj=new_md)
-            assert isinstance(new_md, dict)
-            if hash(json.dumps(new_md)) != _md_before:
-                print(f"Removed XML illegal characters from metadata, cleaned metadata:")
-                print(new_md)
-
             r = item.modify_metadata(
                 metadata=new_md,
                 access_key=access_key,
                 secret_key=secret_key,
             )
             assert isinstance(r, Response)
             r.raise_for_status()
```

### Comparing `biliarchiver-0.0.36/biliarchiver/config.py` & `biliarchiver-0.0.9/biliarchiver/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,49 +12,45 @@
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 @dataclass
-class _Config(metaclass=singleton):
+class Config(metaclass=singleton):
     video_concurrency: int = 3 
     part_concurrency: int = 10
     stream_retry: int = 20
     storage_home_dir: Path = Path('bilibili_archive_dir/').expanduser()
     ia_key_file: Path = Path('~/.bili_ia_keys.txt').expanduser()
-    cookies_file: Path = Path('~/.cookies.txt').expanduser()
 
     def __init__(self):
         self.is_right_pwd()
         if not os.path.exists(CONFIG_FILE):
             print(f'{CONFIG_FILE} 不存在，创建中...')
             self.save()
         with open(CONFIG_FILE, 'r', encoding='utf-8') as f:
-            print(f'Loading {CONFIG_FILE} ...')
+            print(f'读取 {CONFIG_FILE}...')
             config_file = json.load(f)
 
         self.video_concurrency: int = config_file['video_concurrency']
         self.part_concurrency: int = config_file['part_concurrency']
         self.stream_retry: int = config_file['stream_retry']
 
         self.storage_home_dir: Path = Path(config_file['storage_home_dir']).expanduser()
         self.ia_key_file: Path = Path(config_file['ia_key_file']).expanduser()
-        self.cookies_file: Path = Path(config_file['cookies_file']).expanduser()
-
 
     def save(self):
         with open(CONFIG_FILE, 'w', encoding='utf-8') as f:
             json.dump({
                 'video_concurrency': self.video_concurrency,
                 'part_concurrency': self.part_concurrency,
                 'stream_retry': self.stream_retry,
                 'storage_home_dir': str(self.storage_home_dir),
                 'ia_key_file': str(self.ia_key_file),
-                'cookies_file': str(self.cookies_file),
             }, f, ensure_ascii=False, indent=4)
 
     def is_right_pwd(self):
         if not os.path.exists('biliarchiver.home'):
             raise Exception('先在当前工作目录创建 biliarchiver.home 文件')
 
-config = _Config()
+config = Config()
```

### Comparing `biliarchiver-0.0.36/biliarchiver/utils/dirLock.py` & `biliarchiver-0.0.9/biliarchiver/utils/dirLock.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,20 +64,16 @@
             
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         assert self.fcntl is not None
         if self.lock_file_fd is None:
             raise IOError("Lock file not opened.")
         self.fcntl.lockf(self.lock_file_fd, self.fcntl.LOCK_UN)
-        self.lock_file_fd.close() # lock_file_fd.close() 之后，其他进程有机会在本进程删掉锁文件之前拿到新锁
-        try:
-            os.remove(self.lock_file) # 删除文件不影响其他进程已持有的 inode 新锁
-        except FileNotFoundError:
-            # 如果抢到新锁的是本进程，删除文件的是其他进程，那么本进程再删除时自然会 FileNotFoundError，忽略就好
-            pass
+        self.lock_file_fd.close()
+        os.remove(self.lock_file)
         # print("Released lock.")
 
     # decorator
     def __call__(self, func):
         def wrapper(*args, **kwargs):
             with self:
                 return func(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biliarchiver-0.0.36/biliarchiver/utils/identifier.py` & `biliarchiver-0.0.9/biliarchiver/utils/string.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.36/PKG-INFO` & `biliarchiver-0.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: biliarchiver
-Version: 0.0.36
+Version: 0.0.9
 Summary: 
 Author: yzqzss
 Author-email: yzqzss@yandex.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bilix (==0.18.4)
-Requires-Dist: browser-cookie3 (>=0.19.1,<0.20.0)
-Requires-Dist: danmakuc (>=0.3.6,<0.4.0)
+Requires-Dist: bilix (==0.18.3)
 Requires-Dist: internetarchive (>=3.5.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # biliarchiver
 
-> 基于 bilix 的 BiliBili 存档工具
+## 基于 bilix 的 BiliBili 存档工具
 
-## Install
+~~ IA iteam identifier 格式兼容 tubeup ~~。  
+现在不兼容了，Tubeup 不适合存 B 站视频，它的 identifier 设计不科学，大规模存档必定会撞车。
 
-```bash
-pip install biliarchiver
-```
+目前，我可能随时 commit 乱飞且动不动就 git push -f 这个仓库。（为了在我的 vps 和本地之间同步代码）
 
-## Usage
-
-待补充。
+userscript.js 还没适配新换的 identifier 格式。
```

