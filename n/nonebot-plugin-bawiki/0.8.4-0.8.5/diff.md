# Comparing `tmp/nonebot_plugin_bawiki-0.8.4.tar.gz` & `tmp/nonebot_plugin_bawiki-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.8.4.tar", last modified: Fri Aug  4 12:49:32 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.8.5.tar", last modified: Mon Aug  7 09:47:36 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.8.4.tar` & `nonebot_plugin_bawiki-0.8.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/LICENSE
--rw-r--r--   0        0        0    10040 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/README.md
--rw-r--r--   0        0        0      734 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0      947 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/__init__.py
--rw-r--r--   0        0        0     3742 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/arona.py
--rw-r--r--   0        0        0     2870 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/calender.py
--rw-r--r--   0        0        0     1265 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/clear_cache.py
--rw-r--r--   0        0        0     1228 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/craft.py
--rw-r--r--   0        0        0     1017 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/emoji.py
--rw-r--r--   0        0        0     2600 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/event.py
--rw-r--r--   0        0        0      986 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/furniture.py
--rw-r--r--   0        0        0     6372 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/gacha.py
--rw-r--r--   0        0        0     3555 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/global_future.py
--rw-r--r--   0        0        0     1795 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/level_guide.py
--rw-r--r--   0        0        0     3645 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/manga.py
--rw-r--r--   0        0        0     4376 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/raid.py
--rw-r--r--   0        0        0     3953 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_fav.py
--rw-r--r--   0        0        0     1878 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_rank.py
--rw-r--r--   0        0        0     1644 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
--rw-r--r--   0        0        0     2031 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_schale.py
--rw-r--r--   0        0        0     3395 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/time_atk.py
--rw-r--r--   0        0        0     4210 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/voice.py
--rw-r--r--   0        0        0     1152 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0        0 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/__init__.py
--rw-r--r--   0        0        0     1541 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/arona.py
--rw-r--r--   0        0        0     5647 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/bawiki.py
--rw-r--r--   0        0        0     7495 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gacha.py
--rw-r--r--   0        0        0    15476 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gamekee.py
--rw-r--r--   0        0        0    19374 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/schaledb.py
--rw-r--r--   0        0        0     1358 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/__init__.py
--rw-r--r--   0        0        0     1784 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/manual.py
--rw-r--r--   0        0        0     2226 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/pic_menu.py
--rw-r--r--   0        0        0     1251 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/__init__.py
--rw-r--r--   0        0        0    21514 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-08-04 12:49:10.961550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gradient.png
--rw-r--r--   0        0        0     4658 2023-08-04 12:49:10.961550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1481 2023-08-04 12:49:32.221767 nonebot_plugin_bawiki-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    11491 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/LICENSE
+-rw-r--r--   0        0        0    10196 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/README.md
+-rw-r--r--   0        0        0      734 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0      947 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/__init__.py
+-rw-r--r--   0        0        0     3742 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/arona.py
+-rw-r--r--   0        0        0     2870 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/calender.py
+-rw-r--r--   0        0        0     1534 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/clear_cache.py
+-rw-r--r--   0        0        0     1228 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/craft.py
+-rw-r--r--   0        0        0     1017 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/emoji.py
+-rw-r--r--   0        0        0     2600 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/event.py
+-rw-r--r--   0        0        0      986 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/furniture.py
+-rw-r--r--   0        0        0     6372 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/gacha.py
+-rw-r--r--   0        0        0     3555 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/global_future.py
+-rw-r--r--   0        0        0     1795 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/level_guide.py
+-rw-r--r--   0        0        0     3645 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/manga.py
+-rw-r--r--   0        0        0     4376 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/raid.py
+-rw-r--r--   0        0        0     3953 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_fav.py
+-rw-r--r--   0        0        0     1878 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_rank.py
+-rw-r--r--   0        0        0     1644 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
+-rw-r--r--   0        0        0     2031 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_wiki_schale.py
+-rw-r--r--   0        0        0     3395 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/time_atk.py
+-rw-r--r--   0        0        0     4210 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/voice.py
+-rw-r--r--   0        0        0     1153 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/__init__.py
+-rw-r--r--   0        0        0     1542 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/arona.py
+-rw-r--r--   0        0        0     5647 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/bawiki.py
+-rw-r--r--   0        0        0     7495 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/gacha.py
+-rw-r--r--   0        0        0    15476 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/gamekee.py
+-rw-r--r--   0        0        0    19374 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/schaledb.py
+-rw-r--r--   0        0        0     1358 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/help/__init__.py
+-rw-r--r--   0        0        0     1784 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/help/manual.py
+-rw-r--r--   0        0        0     2226 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/help/pic_menu.py
+-rw-r--r--   0        0        0     1251 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/__init__.py
+-rw-r--r--   0        0        0    21514 2023-08-07 09:47:18.938290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-08-07 09:47:18.942290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-08-07 09:47:18.946290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gradient.png
+-rw-r--r--   0        0        0     4709 2023-08-07 09:47:18.946290 nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1481 2023-08-07 09:47:36.298324 nonebot_plugin_bawiki-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0    11647 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.5/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.8.4/LICENSE` & `nonebot_plugin_bawiki-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/README.md` & `nonebot_plugin_bawiki-0.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,29 +98,29 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-在 nonebot2 项目的`.env`文件中添加下表中的配置
+在 nonebot2 项目的 `.env` 文件中添加下表中的配置
 
 |            配置项             | 必填 | 默认值  |                           说明                            |
 | :---------------------------: | :--: | :-----: | :-------------------------------------------------------: |
 |          `BA_PROXY`           |  否  | `None`  |  访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理  |
 |     `BA_GACHA_COOL_DOWN`      |  否  |   `0`   |                每群每人的抽卡冷却，单位秒                 |
 |      `BA_VOICE_USE_CARD`      |  否  | `False` |            是否使用自定义音乐卡片发送角色语音             |
 |       `BA_GAMEKEE_URL`        |  否  |   ...   |                   GameKee 数据源的地址                    |
 |        `BA_SCHALE_URL`        |  否  |   ...   |                SchaleDB Json 数据源的地址                 |
 |    `BA_SCHALE_MIRROR_URL`     |  否  |   ...   |                  SchaleDB 网页截图的地址                  |
 |      `BA_BAWIKI_DB_URL`       |  否  |   ...   |                    bawiki-data 的地址                     |
 |      `BA_ARONA_API_URL`       |  否  |   ...   |                  Arona Bot 数据源的地址                   |
 |      `BA_ARONA_CDN_URL`       |  否  |   ...   |                  Arona Bot 图片 CDN 地址                  |
 | `BA_CLEAR_REQ_CACHE_INTERVAL` |  否  |   `3`   |             插件清理请求缓存的间隔，单位小时              |
-|  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  |   ...   | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
+|  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  | `False` | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
 
 由于 CDN 可能并不给力，如果有条件的话本人推荐使用代理直接访问原地址，下面是对应 `.env` 配置：
 
 ```ini
 BA_PROXY=http://127.0.0.1:7890
 BA_SCHALE_URL=https://schale.gg/
 BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
@@ -171,14 +171,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.5
+
+- 修复 [#41](https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki/issues/41)
+- 配置项 `BA_AUTO_CLEAR_ARONA_CACHE` 默认值改为 `False`
+
 ### 0.8.4
 
 - 现在会对 GameKee 的日程表分页了
 - `ba羁绊` 指令带图发送失败时会提醒用户
 - 修复 `ba学生wiki` 截图失败的 bug，同时优化截图样式
 - 漫画获取不再依赖 bawiki-data 数据源，现在直接从 GameKee 现爬；加入了搜索漫画功能，并且图片过多会使用合并转发的方式发送
```

#### html2text {}

```diff
@@ -14,30 +14,30 @@
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
 nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
 conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | | :---------------------------: | :--: | :-----: | :------
--------------------------------------------------: | | `BA_PROXY` | å¦ |
-`None` | è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç |
-| `BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ |
-| `BA_VOICE_USE_CARD` | å¦ | `False` |
+"nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
+æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |
+:---------------------------: | :--: | :-----: | :-----------------------------
+--------------------------: | | `BA_PROXY` | å¦ | `None` | è®¿é®
+`SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+`BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
+`BA_VOICE_USE_CARD` | å¦ | `False` |
 æ¯å¦ä½¿ç¨èªå®ä¹é³ä¹å¡çåéè§è²è¯­é³ | | `BA_GAMEKEE_URL` | å¦
 | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` | å¦ | ... | SchaleDB
 Json æ°æ®æºçå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
 ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
 çå°å | | `BA_ARONA_API_URL` | å¦ | ... | Arona Bot æ°æ®æºçå°å | |
 `BA_ARONA_CDN_URL` | å¦ | ... | Arona Bot å¾ç CDN å°å | |
 `BA_CLEAR_REQ_CACHE_INTERVAL` | å¦ | `3` |
 æä»¶æ¸çè¯·æ±ç¼å­çé´éï¼åä½å°æ¶ | |
-`BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | ... |
+`BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | `False` |
 æ¯å¦å¨æä»¶æ¯æ¬¡å è½½æ¶èªå¨æ¸çä» Arona Bot
 æ°æ®æºç¼å­çå¾ç | ç±äº CDN
 å¯è½å¹¶ä¸ç»åï¼å¦æææ¡ä»¶çè¯æ¬äººæ¨èä½¿ç¨ä»£çç´æ¥è®¿é®åå°åï¼ä¸é¢æ¯å¯¹åº
 `.env` éç½®ï¼ ```ini BA_PROXY=http://127.0.0.1:7890 BA_SCHALE_URL=https://
 schale.gg/ BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
 BA_BAWIKI_DB_URL=https://bawiki.lgc2333.top/ ``` ## ð ä½¿ç¨ ### æä»¤è¡¨
 å¼å®¹ [nonebot-plugin-PicMenu](https://github.com/hamo-reid/
@@ -52,14 +52,16 @@
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
+0.8.5 - ä¿®å¤ [#41](https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki/
+issues/41) - éç½®é¡¹ `BA_AUTO_CLEAR_ARONA_CACHE` é»è®¤å¼æ¹ä¸º `False` ###
 0.8.4 - ç°å¨ä¼å¯¹ GameKee çæ¥ç¨è¡¨åé¡µäº - `baç¾ç»`
 æä»¤å¸¦å¾åéå¤±è´¥æ¶ä¼æéç¨æ· - ä¿®å¤ `baå­¦çwiki`
 æªå¾å¤±è´¥ç bugï¼åæ¶ä¼åæªå¾æ ·å¼ - æ¼«ç»è·åä¸åä¾èµ
 bawiki-data æ°æ®æºï¼ç°å¨ç´æ¥ä» GameKee
 ç°ç¬ï¼å å¥äºæç´¢æ¼«ç»åè½ï¼å¹¶ä¸å¾çè¿å¤ä¼ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé
 ## 0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
 æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
```

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from .command import load_commands  # noqa: E402
 from .config import Cfg as Cfg  # noqa: E402
 from .help import extra, register_help_cmd, usage  # noqa: E402
 
-__version__ = "0.8.4"
+__version__ = "0.8.5"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=usage,
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
     type="application",
     config=Cfg,
```

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/__init__.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/arona.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/arona.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/calender.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/calender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/clear_cache.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/clear_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import shutil
+from pathlib import Path
 from typing import TYPE_CHECKING
 
-import anyio
 from nonebot import on_command
 from nonebot.internal.matcher import Matcher
 from nonebot.permission import SUPERUSER
 
 from ..resource import CACHE_PATH
 from ..util import clear_req_cache
 
@@ -26,18 +25,31 @@
             "- <ft color=(238,120,0)>ba清空缓存</ft>\n"
             "- <ft color=(238,120,0)>ba清除缓存</ft>"
         ),
     },
 ]
 
 
+def clear_cache_dir() -> int:
+    counter = 0
+
+    def run(path: Path):
+        nonlocal counter
+        for p in path.iterdir():
+            if p.is_dir():
+                run(p)
+            else:
+                p.unlink()
+                counter += 1
+
+    run(CACHE_PATH)
+    return counter
+
+
 cmd_clear_cache = on_command("ba清空缓存", aliases={"ba清除缓存"}, permission=SUPERUSER)
 
 
 @cmd_clear_cache.handle()
 async def _(matcher: Matcher):
-    clear_req_cache()
-
-    async for path in anyio.Path(CACHE_PATH).iterdir():
-        await path.unlink() if path.is_file() else shutil.rmtree(path)
-
-    await matcher.finish("缓存已清空～")
+    req_count = clear_req_cache()
+    cache_count = clear_cache_dir()
+    await matcher.finish(f"已清除 {req_count} 项请求缓存与 {cache_count} 项文件缓存～")
```

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/craft.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/craft.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/emoji.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/emoji.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/event.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/furniture.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/furniture.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/gacha.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/global_future.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/global_future.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/level_guide.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/level_guide.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/manga.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/manga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/raid.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/raid.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_fav.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_fav.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_rank.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_schale.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/stu_wiki_schale.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/time_atk.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/time_atk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/voice.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/command/voice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ba_schale_url: str = "https://schale.lgc.cyberczy.xyz/"
     ba_schale_mirror_url: str = "https://schale.lgc.cyberczy.xyz/"
     ba_bawiki_db_url: str = "https://bawiki.lgc.cyberczy.xyz/"
     ba_arona_api_url: str = "https://arona.diyigemt.com/"
     ba_arona_cdn_url: str = "https://arona.cdn.diyigemt.com/"
 
     ba_clear_req_cache_interval: int = 3
-    ba_auto_clear_arona_cache: bool = True
+    ba_auto_clear_arona_cache: bool = False
 
     @validator(
         "ba_gamekee_url",
         "ba_schale_url",
         "ba_schale_mirror_url",
         "ba_bawiki_db_url",
         "ba_arona_api_url",
```

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/arona.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/arona.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from pydantic import BaseModel
 
 from ..config import config
 from ..resource import CACHE_PATH
 from ..util import async_req
 
 ARONA_CACHE_PATH = CACHE_PATH / "arona"
-if ARONA_CACHE_PATH.exists() and config.ba_auto_clear_arona_cache:
+if config.ba_auto_clear_arona_cache and ARONA_CACHE_PATH.exists():
     shutil.rmtree(ARONA_CACHE_PATH)
 if not ARONA_CACHE_PATH.exists():
     ARONA_CACHE_PATH.mkdir(parents=True)
 
+
 IMAGE_TYPE_MAP = {
     1: "学生攻略",
     2: "主线地图",
     3: "杂图",
 }
```

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/bawiki.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gacha.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gamekee.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/schaledb.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/data/schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/__init__.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/help/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/manual.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/help/manual.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/pic_menu.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/help/pic_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/__init__.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/calender_banner.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_new.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_star.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gradient.png` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/resource/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.8.5/nonebot_plugin_bawiki/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,18 @@
         and (json is None or json == c.json)
         and (params is None or params == c.params)
     ):
         return c.content
     return None
 
 
-def clear_req_cache():
+def clear_req_cache() -> int:
+    count = len(req_cache)
     req_cache.clear()
+    return count
 
 
 if config.ba_clear_req_cache_interval > 0:
 
     @scheduler.scheduled_job("interval", hours=config.ba_clear_req_cache_interval)
     async def _():
         clear_req_cache()
```

### Comparing `nonebot_plugin_bawiki-0.8.4/pyproject.toml` & `nonebot_plugin_bawiki-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.8.4"
+version = "0.8.5"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
```

### Comparing `nonebot_plugin_bawiki-0.8.4/PKG-INFO` & `nonebot_plugin_bawiki-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.8.4
+Version: 0.8.5
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -133,29 +133,29 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-在 nonebot2 项目的`.env`文件中添加下表中的配置
+在 nonebot2 项目的 `.env` 文件中添加下表中的配置
 
 |            配置项             | 必填 | 默认值  |                           说明                            |
 | :---------------------------: | :--: | :-----: | :-------------------------------------------------------: |
 |          `BA_PROXY`           |  否  | `None`  |  访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理  |
 |     `BA_GACHA_COOL_DOWN`      |  否  |   `0`   |                每群每人的抽卡冷却，单位秒                 |
 |      `BA_VOICE_USE_CARD`      |  否  | `False` |            是否使用自定义音乐卡片发送角色语音             |
 |       `BA_GAMEKEE_URL`        |  否  |   ...   |                   GameKee 数据源的地址                    |
 |        `BA_SCHALE_URL`        |  否  |   ...   |                SchaleDB Json 数据源的地址                 |
 |    `BA_SCHALE_MIRROR_URL`     |  否  |   ...   |                  SchaleDB 网页截图的地址                  |
 |      `BA_BAWIKI_DB_URL`       |  否  |   ...   |                    bawiki-data 的地址                     |
 |      `BA_ARONA_API_URL`       |  否  |   ...   |                  Arona Bot 数据源的地址                   |
 |      `BA_ARONA_CDN_URL`       |  否  |   ...   |                  Arona Bot 图片 CDN 地址                  |
 | `BA_CLEAR_REQ_CACHE_INTERVAL` |  否  |   `3`   |             插件清理请求缓存的间隔，单位小时              |
-|  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  |   ...   | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
+|  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  | `False` | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
 
 由于 CDN 可能并不给力，如果有条件的话本人推荐使用代理直接访问原地址，下面是对应 `.env` 配置：
 
 ```ini
 BA_PROXY=http://127.0.0.1:7890
 BA_SCHALE_URL=https://schale.gg/
 BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
@@ -206,14 +206,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.5
+
+- 修复 [#41](https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki/issues/41)
+- 配置项 `BA_AUTO_CLEAR_ARONA_CACHE` 默认值改为 `False`
+
 ### 0.8.4
 
 - 现在会对 GameKee 的日程表分页了
 - `ba羁绊` 指令带图发送失败时会提醒用户
 - 修复 `ba学生wiki` 截图失败的 bug，同时优化截图样式
 - 漫画获取不再依赖 bawiki-data 数据源，现在直接从 GameKee 现爬；加入了搜索漫画功能，并且图片过多会使用合并转发的方式发送
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.4 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.5 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -34,30 +34,30 @@
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
 nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
 conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | | :---------------------------: | :--: | :-----: | :------
--------------------------------------------------: | | `BA_PROXY` | å¦ |
-`None` | è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç |
-| `BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ |
-| `BA_VOICE_USE_CARD` | å¦ | `False` |
+"nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
+æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |
+:---------------------------: | :--: | :-----: | :-----------------------------
+--------------------------: | | `BA_PROXY` | å¦ | `None` | è®¿é®
+`SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+`BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
+`BA_VOICE_USE_CARD` | å¦ | `False` |
 æ¯å¦ä½¿ç¨èªå®ä¹é³ä¹å¡çåéè§è²è¯­é³ | | `BA_GAMEKEE_URL` | å¦
 | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` | å¦ | ... | SchaleDB
 Json æ°æ®æºçå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
 ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
 çå°å | | `BA_ARONA_API_URL` | å¦ | ... | Arona Bot æ°æ®æºçå°å | |
 `BA_ARONA_CDN_URL` | å¦ | ... | Arona Bot å¾ç CDN å°å | |
 `BA_CLEAR_REQ_CACHE_INTERVAL` | å¦ | `3` |
 æä»¶æ¸çè¯·æ±ç¼å­çé´éï¼åä½å°æ¶ | |
-`BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | ... |
+`BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | `False` |
 æ¯å¦å¨æä»¶æ¯æ¬¡å è½½æ¶èªå¨æ¸çä» Arona Bot
 æ°æ®æºç¼å­çå¾ç | ç±äº CDN
 å¯è½å¹¶ä¸ç»åï¼å¦æææ¡ä»¶çè¯æ¬äººæ¨èä½¿ç¨ä»£çç´æ¥è®¿é®åå°åï¼ä¸é¢æ¯å¯¹åº
 `.env` éç½®ï¼ ```ini BA_PROXY=http://127.0.0.1:7890 BA_SCHALE_URL=https://
 schale.gg/ BA_SCHALE_MIRROR_URL=https://schale.lgc2333.top/
 BA_BAWIKI_DB_URL=https://bawiki.lgc2333.top/ ``` ## ð ä½¿ç¨ ### æä»¤è¡¨
 å¼å®¹ [nonebot-plugin-PicMenu](https://github.com/hamo-reid/
@@ -72,14 +72,16 @@
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
+0.8.5 - ä¿®å¤ [#41](https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki/
+issues/41) - éç½®é¡¹ `BA_AUTO_CLEAR_ARONA_CACHE` é»è®¤å¼æ¹ä¸º `False` ###
 0.8.4 - ç°å¨ä¼å¯¹ GameKee çæ¥ç¨è¡¨åé¡µäº - `baç¾ç»`
 æä»¤å¸¦å¾åéå¤±è´¥æ¶ä¼æéç¨æ· - ä¿®å¤ `baå­¦çwiki`
 æªå¾å¤±è´¥ç bugï¼åæ¶ä¼åæªå¾æ ·å¼ - æ¼«ç»è·åä¸åä¾èµ
 bawiki-data æ°æ®æºï¼ç°å¨ç´æ¥ä» GameKee
 ç°ç¬ï¼å å¥äºæç´¢æ¼«ç»åè½ï¼å¹¶ä¸å¾çè¿å¤ä¼ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé
 ## 0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
 æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
```

