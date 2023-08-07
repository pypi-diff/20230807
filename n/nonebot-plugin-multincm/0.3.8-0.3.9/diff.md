# Comparing `tmp/nonebot_plugin_multincm-0.3.8.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.8.tar", last modified: Wed Jun 28 17:38:30 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.9.tar", last modified: Mon Aug  7 09:24:29 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.8.tar` & `nonebot_plugin_multincm-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/LICENSE
--rw-r--r--   0        0        0     9711 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/README.md
--rw-r--r--   0        0        0     1853 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    13936 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      819 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5556 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    15330 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2928 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2279 2023-06-28 17:38:18.367872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-06-28 17:38:18.371872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0      577 2023-06-28 17:38:18.371872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/res/lyric.html.jinja
--rw-r--r--   0        0        0     2750 2023-06-28 17:38:18.371872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/res/song_list.html.jinja
--rw-r--r--   0        0        0     3007 2023-06-28 17:38:18.371872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-06-28 17:38:18.371872 nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      824 2023-06-28 17:38:30.395984 nonebot_plugin_multincm-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    10567 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/LICENSE
+-rw-r--r--   0        0        0     9848 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/README.md
+-rw-r--r--   0        0        0     1816 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    13986 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      820 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      175 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5562 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0     1211 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/draw/__init__.py
+-rw-r--r--   0        0        0     8018 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/draw/pil.py
+-rw-r--r--   0        0        0     2790 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/draw/playwright.py
+-rw-r--r--   0        0        0     2004 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/draw/shared.py
+-rw-r--r--   0        0        0     2928 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2373 2023-08-07 09:24:10.178826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-08-07 09:24:10.182826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0      577 2023-08-07 09:24:10.182826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/res/lyric.html.jinja
+-rw-r--r--   0        0        0     2750 2023-08-07 09:24:10.182826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/res/song_list.html.jinja
+-rw-r--r--   0        0        0     3007 2023-08-07 09:24:10.182826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0     2318 2023-08-07 09:24:10.182826 nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      824 2023-08-07 09:24:29.790941 nonebot_plugin_multincm-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    10704 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.9/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.8/LICENSE` & `nonebot_plugin_multincm-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.8/README.md` & `nonebot_plugin_multincm-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 |         `NCM_EMAIL`         |  否  |      无      |                       邮箱登录用，登录邮箱                        |
 |       `NCM_PASSWORD`        |  否  |      无      |                帐号明文密码，邮箱登录时为邮箱密码                 |
 |     `NCM_PASSWORD_HASH`     |  否  |      无      |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
 |      `NCM_LIST_LIMIT`       |  否  |     `20`     |                      歌曲列表每页的最大数量                       |
 |       `NCM_LIST_FONT`       |  否  |      无      |                      渲染歌曲列表使用的字体                       |
 |     `NCM_MAX_NAME_LEN`      |  否  |    `600`     |              歌曲列表中歌名列的最大文本宽度（像素）               |
 |    `NCM_MAX_ARTIST_LEN`     |  否  |    `400`     |              歌曲列表中歌手列的最大文本宽度（像素）               |
-|    `NCM_MSG_CACHE_TIME`     |  否  |    `3600`    | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|    `NCM_MSG_CACHE_TIME`     |  否  |   `43200`    | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
 |     `NCM_AUTO_RESOLVE`      |  否  |   `False`    |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
 |  `NCM_ILLEGAL_CMD_FINISH`   |  否  |   `False`    |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
 |    `NCM_USE_PLAYWRIGHT`     |  否  |   `False`    |           是否使用 `playwright` 绘制歌曲列表与歌词图片            |
 |    `NCM_LRC_EMPTY_LINE`     |  否  |  `--------`  |                        填充歌词空行的字符                         |
 |    `NCM_DELETE_LIST_MSG`    |  否  |    `True`    |               是否在退出点歌模式后自动撤回歌曲列表                |
 | `NCM_DELETE_LIST_MSG_DELAY` |  否  | `[0.5, 2.0]` |              自动撤回歌曲列表消息间隔时间（单位秒）               |
 
@@ -217,14 +217,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.9
+
+- 让 `htmlrender` 成为真正的可选依赖
+- 把配置项 `NCM_MSG_CACHE_TIME` 的默认值改为 `43200`（12 小时）
+
 ### 0.3.8
 
 - 修改及统一表格背景色
 
 ### 0.3.7
 
 - 添加配置项 `NCM_DELETE_LIST_MSG` 和 `NCM_DELETE_LIST_MSG_DELAY`（[#5](https://github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/5)）
```

#### html2text {}

```diff
@@ -40,17 +40,17 @@
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
-`NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
-ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
-| `False` |
+`NCM_MSG_CACHE_TIME` | å¦ | `43200` | ç¼å­ Bot
+å·²åéé³ä¹å¡ççé³ä¹ ID å ç¨æ·æè¿ä¸æ¬¡æä½
+çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦ | `False` |
 å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | |
 `NCM_ILLEGAL_CMD_FINISH` | å¦ | `False` |
 å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | |
 `NCM_USE_PLAYWRIGHT` | å¦ | `False` | æ¯å¦ä½¿ç¨ `playwright`
 ç»å¶æ­æ²åè¡¨ä¸æ­è¯å¾ç | | `NCM_LRC_EMPTY_LINE` | å¦ | `--------` |
 å¡«åæ­è¯ç©ºè¡çå­ç¬¦ | | `NCM_DELETE_LIST_MSG` | å¦ | `True` |
 æ¯å¦å¨éåºç¹æ­æ¨¡å¼åèªå¨æ¤åæ­æ²åè¡¨ | |
@@ -79,15 +79,17 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.8 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.9 - è®© `htmlrender`
+æä¸ºçæ­£çå¯éä¾èµ - æéç½®é¡¹ `NCM_MSG_CACHE_TIME`
+çé»è®¤å¼æ¹ä¸º `43200`ï¼12 å°æ¶ï¼ ### 0.3.8 -
 ä¿®æ¹åç»ä¸è¡¨æ ¼èæ¯è² ### 0.3.7 - æ·»å éç½®é¡¹
 `NCM_DELETE_LIST_MSG` å `NCM_DELETE_LIST_MSG_DELAY`ï¼[#5](https://
 github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/5)ï¼ ### 0.3.6 -
 æ¯æä½¿ç¨ `nonebot-plugin-htmlrender` (`playwright`)
 æ¸²ææ­æ²åè¡¨ä¸æ­è¯å¾çï¼é»è®¤ä¸å¯ç¨ï¼å¦è¦å¯ç¨éè¦èªè¡å®è£
 `nonebot-plugin-multincm[playwright]`ï¼ - æ·»å éç½®é¡¹ `NCM_USE_PLAYWRIGHT`
 ä¸ `NCM_LRC_EMPTY_LINE` ### 0.3.5 - ð NoneBot 2.0 ð ### 0.3.4 -
```

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
-require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 __plugin_meta__ = PluginMetadata(
     name="MultiNCM",
     description="网易云多选点歌",
     usage=(
         "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     get_track_audio,
     get_track_info,
     get_track_lrc,
     get_voice_info,
     search_song,
     search_voice,
 )
-from .draw import draw_search_res, format_lrc, str_to_pic
+from .draw import draw_search_res, str_to_pic
 from .msg_cache import (
     CALLING_MAP,
     SongCache,
     SongType,
     chat_last_song_cache,
     song_msg_id_cache,
 )
@@ -57,15 +57,15 @@
     SearchResult,
     Song,
     SongInfo,
     SongSearchResult,
     VoiceBaseInfo,
     VoiceResource,
 )
-from .utils import format_alias, format_artists
+from .utils import format_alias, format_artists, format_lrc
 
 LIST_MSG_ID_KEY = "list_msg_id"
 SONG_CACHE_KEY = "song_cache"
 CHECK_REPLY_KEY = "check_reply"
 SEARCH_PARAM_KEY = "param"
 SEARCH_CACHE_KEY = "cache"
 SONG_TYPE_KEY = "type"
@@ -191,15 +191,15 @@
     # 管你妈那么多闲事干嘛，直接上最高就得了
     # bitrate = (
     #     song.privilege.pl if is_song and song.privilege.plLevel else None
     # ) or 999999
 
     try:
         audio_info = await get_track_audio([song_id], bitrate)
-    except:
+    except Exception:
         logger.exception(f"获取{calling}播放链接失败")
         await finish_with_delete_msg(f"获取{calling}播放链接失败，请检查后台输出")
 
     if not audio_info:
         await finish_with_delete_msg(f"抱歉，没有获取到{calling}播放链接")
 
     info = audio_info[0]
@@ -264,15 +264,15 @@
     song_type: SongType = state[SONG_TYPE_KEY]
     calling = CALLING_MAP[song_type]
 
     if not (res := cache.get(page)):
         func = search_song if song_type == "song" else search_voice
         try:
             res = await func(param, page=page)
-        except:
+        except Exception:
             logger.exception(f"搜索{calling}失败")
             await finish_with_delete_msg(f"搜索{calling}失败，请检查后台输出")
 
     is_song = isinstance(res, SongSearchResult)
     total_count = res.songCount if is_song else res.totalCount
     results = res.songs if is_song else res.resources
     if not results:
@@ -283,15 +283,15 @@
     state[MAX_PAGE_KEY] = ceil(total_count / config.ncm_list_limit)
 
     if page == 1 and len(results) == 1:
         await get_cache_by_index(cache, 1)
 
     try:
         pic = await draw_search_res(res, page)
-    except:
+    except Exception:
         logger.exception(f"绘制{calling}列表失败")
         await finish_with_delete_msg(f"绘制{calling}列表失败，请检查后台输出")
 
     return MessageSegment.image(pic)
 
 
 async def send_page(page: int = 1, reject: bool = False, pause: bool = False):
@@ -434,15 +434,15 @@
 
     try:
         if song_cache.type == "voice":
             song = await get_voice_info(song_cache.id)
         else:
             song = await get_track_info([song_cache.id])
             song = song[0] if song else None
-    except:
+    except Exception:
         logger.exception(f"获取{calling}信息失败")
         await matcher.finish(f"获取{calling}信息失败，请检查后台输出")
 
     if not song:
         await matcher.finish(f"未获取到对应{calling}信息")
 
     await send_music(song)
@@ -461,15 +461,15 @@
 
     if song_cache.type == "voice":
         await matcher.finish("电台节目无法获取歌词")
 
     song_id = song_cache.id
     try:
         lrc_data = await get_track_lrc(song_id)
-    except:
+    except Exception:
         logger.exception("获取歌曲歌词失败")
         await matcher.finish("获取歌曲歌词失败，请检查后台输出")
 
     lrc = format_lrc(lrc_data)
     if not lrc:
         await matcher.finish("该歌曲没有歌词")
```

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ncm_email: Optional[str] = None
     ncm_password: Optional[str] = None
     ncm_password_hash: Optional[str] = None
     ncm_list_limit: int = 20
     ncm_list_font: Optional[str] = None
     ncm_max_name_len: int = 600
     ncm_max_artist_len: int = 400
-    ncm_msg_cache_time: int = 3600
+    ncm_msg_cache_time: int = 43200
     ncm_auto_resolve: bool = False
     ncm_illegal_cmd_finish: bool = False
     ncm_use_playwright: bool = False
     ncm_lrc_empty_line: Optional[str] = "--------"
     ncm_delete_list_msg: bool = True
     ncm_delete_list_msg_delay: Tuple[float, float] = (0.5, 2.0)
```

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         assert ret["account"]
     except Exception as e:
         if await (pth := anyio.Path(SESSION_FILE)).exists():
             await pth.unlink()
 
         if retry:
             logger.warning("恢复缓存会话失败，尝试使用正常流程登录")
-            await login(False)
+            await login(retry=False)
             return
 
         raise RuntimeError("登录态异常，请重新登录") from e
 
     session = GetCurrentSession()
     logger.info(f"登录成功，欢迎您，{session.nickname} [{session.uid}]")
```

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/msg_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     def __del__(self):
         scheduler.remove_job(self._job)
 
     def __getitem__(self, __key: KT) -> VT:
         return super().__getitem__(__key)[1]
 
     @overload
-    def get(self, __key: KT, __default: Literal[None] = None) -> Optional[VT]:
+    def get(
+        self,
+        __key: KT,
+        __default: Literal[None] = None,  # noqa: RUF013
+    ) -> Optional[VT]:
         ...
 
     @overload
     def get(self, __key: KT, __default: VT = ...) -> VT:
         ...
 
     def get(self, __key, __default=None):
@@ -58,15 +62,19 @@
             yield v[1]
 
     def items(self) -> Iterable[Tuple[KT, VT]]:
         for k, v in super().items():
             yield k, v[1]
 
     @overload
-    def pop(self, __key: KT, __default: Literal[None] = None) -> Optional[VT]:
+    def pop(
+        self,
+        __key: KT,
+        __default: Literal[None] = None,  # noqa: RUF013
+    ) -> Optional[VT]:
         ...
 
     @overload
     def pop(self, __key: KT, __default: VT = ...) -> VT:
         ...
 
     def pop(self, __key, __default=None):
```

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/res/lyric.html.jinja` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/res/lyric.html.jinja`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/res/song_list.html.jinja` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/res/song_list.html.jinja`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.8/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.9/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.8/pyproject.toml` & `nonebot_plugin_multincm-0.3.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.8"
+version = "0.3.9"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.3.8/PKG-INFO` & `nonebot_plugin_multincm-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.8
+Version: 0.3.9
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
@@ -166,15 +166,15 @@
 |         `NCM_EMAIL`         |  否  |      无      |                       邮箱登录用，登录邮箱                        |
 |       `NCM_PASSWORD`        |  否  |      无      |                帐号明文密码，邮箱登录时为邮箱密码                 |
 |     `NCM_PASSWORD_HASH`     |  否  |      无      |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
 |      `NCM_LIST_LIMIT`       |  否  |     `20`     |                      歌曲列表每页的最大数量                       |
 |       `NCM_LIST_FONT`       |  否  |      无      |                      渲染歌曲列表使用的字体                       |
 |     `NCM_MAX_NAME_LEN`      |  否  |    `600`     |              歌曲列表中歌名列的最大文本宽度（像素）               |
 |    `NCM_MAX_ARTIST_LEN`     |  否  |    `400`     |              歌曲列表中歌手列的最大文本宽度（像素）               |
-|    `NCM_MSG_CACHE_TIME`     |  否  |    `3600`    | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|    `NCM_MSG_CACHE_TIME`     |  否  |   `43200`    | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
 |     `NCM_AUTO_RESOLVE`      |  否  |   `False`    |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
 |  `NCM_ILLEGAL_CMD_FINISH`   |  否  |   `False`    |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
 |    `NCM_USE_PLAYWRIGHT`     |  否  |   `False`    |           是否使用 `playwright` 绘制歌曲列表与歌词图片            |
 |    `NCM_LRC_EMPTY_LINE`     |  否  |  `--------`  |                        填充歌词空行的字符                         |
 |    `NCM_DELETE_LIST_MSG`    |  否  |    `True`    |               是否在退出点歌模式后自动撤回歌曲列表                |
 | `NCM_DELETE_LIST_MSG_DELAY` |  否  | `[0.5, 2.0]` |              自动撤回歌曲列表消息间隔时间（单位秒）               |
 
@@ -240,14 +240,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.9
+
+- 让 `htmlrender` 成为真正的可选依赖
+- 把配置项 `NCM_MSG_CACHE_TIME` 的默认值改为 `43200`（12 小时）
+
 ### 0.3.8
 
 - 修改及统一表格背景色
 
 ### 0.3.7
 
 - 添加配置项 `NCM_DELETE_LIST_MSG` 和 `NCM_DELETE_LIST_MSG_DELAY`（[#5](https://github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/5)）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.8 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.9 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
 pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -52,17 +52,17 @@
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
-`NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
-ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
-| `False` |
+`NCM_MSG_CACHE_TIME` | å¦ | `43200` | ç¼å­ Bot
+å·²åéé³ä¹å¡ççé³ä¹ ID å ç¨æ·æè¿ä¸æ¬¡æä½
+çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦ | `False` |
 å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | |
 `NCM_ILLEGAL_CMD_FINISH` | å¦ | `False` |
 å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | |
 `NCM_USE_PLAYWRIGHT` | å¦ | `False` | æ¯å¦ä½¿ç¨ `playwright`
 ç»å¶æ­æ²åè¡¨ä¸æ­è¯å¾ç | | `NCM_LRC_EMPTY_LINE` | å¦ | `--------` |
 å¡«åæ­è¯ç©ºè¡çå­ç¬¦ | | `NCM_DELETE_LIST_MSG` | å¦ | `True` |
 æ¯å¦å¨éåºç¹æ­æ¨¡å¼åèªå¨æ¤åæ­æ²åè¡¨ | |
@@ -91,15 +91,17 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.8 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.9 - è®© `htmlrender`
+æä¸ºçæ­£çå¯éä¾èµ - æéç½®é¡¹ `NCM_MSG_CACHE_TIME`
+çé»è®¤å¼æ¹ä¸º `43200`ï¼12 å°æ¶ï¼ ### 0.3.8 -
 ä¿®æ¹åç»ä¸è¡¨æ ¼èæ¯è² ### 0.3.7 - æ·»å éç½®é¡¹
 `NCM_DELETE_LIST_MSG` å `NCM_DELETE_LIST_MSG_DELAY`ï¼[#5](https://
 github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/5)ï¼ ### 0.3.6 -
 æ¯æä½¿ç¨ `nonebot-plugin-htmlrender` (`playwright`)
 æ¸²ææ­æ²åè¡¨ä¸æ­è¯å¾çï¼é»è®¤ä¸å¯ç¨ï¼å¦è¦å¯ç¨éè¦èªè¡å®è£
 `nonebot-plugin-multincm[playwright]`ï¼ - æ·»å éç½®é¡¹ `NCM_USE_PLAYWRIGHT`
 ä¸ `NCM_LRC_EMPTY_LINE` ### 0.3.5 - ð NoneBot 2.0 ð ### 0.3.4 -
```

