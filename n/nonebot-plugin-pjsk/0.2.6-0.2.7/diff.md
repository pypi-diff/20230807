# Comparing `tmp/nonebot_plugin_pjsk-0.2.6.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.6.tar", last modified: Sun Aug  6 08:46:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.7.tar", last modified: Mon Aug  7 11:38:10 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.6.tar` & `nonebot_plugin_pjsk-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-08-06 08:45:58.454255 nonebot_plugin_pjsk-0.2.6/LICENSE
--rw-r--r--   0        0        0     4800 2023-08-06 08:45:58.454255 nonebot_plugin_pjsk-0.2.6/README.md
--rw-r--r--   0        0        0      795 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     8728 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0     1216 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0    11391 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     4150 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2351 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1787 2023-08-06 08:46:16.752144 nonebot_plugin_pjsk-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5791 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-07 11:37:52.251467 nonebot_plugin_pjsk-0.2.7/LICENSE
+-rw-r--r--   0        0        0     6393 2023-08-07 11:37:52.251467 nonebot_plugin_pjsk-0.2.7/README.md
+-rw-r--r--   0        0        0      795 2023-08-07 11:37:52.295467 nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     8911 2023-08-07 11:37:52.295467 nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1057 2023-08-07 11:37:52.295467 nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0    11462 2023-08-07 11:37:52.295467 nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     4180 2023-08-07 11:37:52.295467 nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2584 2023-08-07 11:37:52.299467 nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1788 2023-08-07 11:38:10.763608 nonebot_plugin_pjsk-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     7385 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.6/LICENSE` & `nonebot_plugin_pjsk-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.6/README.md` & `nonebot_plugin_pjsk-0.2.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -108,16 +108,23 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-见 [config.py](./nonebot_plugin_pjsk/config.py) 文件  
-插件开箱即用，如无需要则无须配置
+插件开箱即用，所有配置项皆为可选。请**按需添加**下面的配置项到 `.env` 文件中
+
+|        配置项        | 必填 | 默认值  |                                                              说明                                                              |
+| :------------------: | :--: | :-----: | :----------------------------------------------------------------------------------------------------------------------------: |
+| `PJSK_ASSETS_PREFIX` |  否  |   ...   |                          TheOriginalAyaka/sekai-stickers 仓库 GitHubUserContent 地址，默认为国内镜像                           |
+|  `PJSK_REPO_PREFIX`  |  否  |   ...   |                                         本仓库 GitHubUserContent 地址，默认为国内镜像                                          |
+| `PJSK_EMOJI_SOURCE`  |  否  | `Apple` | Emoji 来源，可选值见 [这里](https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/imagetext_py.pyi#L217) |
+| `PJSK_HELP_AS_IMAGE` |  否  | `True`  |                                                  是否将帮助信息渲染为图片发送                                                  |
+|     `PJSK_REPLY`     |  否  | `True`  |                                                       是否回复消息发送者                                                       |
 
 ## 🎉 使用
 
 直接使用指令 `pjsk` 进入交互创建模式；  
 使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助
 
 ### 效果图
@@ -152,14 +159,24 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.7
+
+- 修复参数为 `0` 时不生效的 Bug
+- 现在可以关闭回复消息发送者的特性了
+- 命令参数调整：
+  - 删除 `--weight` 参数，因为没有实际意义
+  - `--rotate` 参数可以接受小数了
+  - `--stroke-width` 参数添加简写 `-W`
+  - `--line-spacing` 参数添加简写 `-C`
+
 ### 0.2.6
 
 - 插件会按角色名重新排序表情列表与表情 ID，以防数据源表情 ID 冲突
 - 角色列表名称展示优化
 
 ### 0.2.5
```

#### html2text {}

```diff
@@ -15,32 +15,46 @@
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½® è§ [config.py](./
-nonebot_plugin_pjsk/config.py) æä»¶
-æä»¶å¼ç®±å³ç¨ï¼å¦æ éè¦åæ é¡»éç½® ## ð ä½¿ç¨
-ç´æ¥ä½¿ç¨æä»¤ `pjsk` è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h`
-äºè§£ä½¿ç¨ Shell-Like æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾
-ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example](./readme/example-interact.png)   ä½¿ç¨
-Shell-Like æä»¤ ![example](./readme/example.png)  ## ð ç¢ç¢å¿µ -
-~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
+"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½®
+æä»¶å¼ç®±å³ç¨ï¼ææéç½®é¡¹çä¸ºå¯éãè¯·**æéæ·»å **ä¸é¢çéç½®é¡¹å°
+`.env` æä»¶ä¸­ | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | | :---------------
+---: | :--: | :-----: | :------------------------------------------------------
+----------------------------------------------------------------------: | |
+`PJSK_ASSETS_PREFIX` | å¦ | ... | TheOriginalAyaka/sekai-stickers ä»åº
+GitHubUserContent å°åï¼é»è®¤ä¸ºå½åéå | | `PJSK_REPO_PREFIX` | å¦ |
+... | æ¬ä»åº GitHubUserContent å°åï¼é»è®¤ä¸ºå½åéå | |
+`PJSK_EMOJI_SOURCE` | å¦ | `Apple` | Emoji æ¥æºï¼å¯éå¼è§ [è¿é]
+(https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/
+imagetext_py.pyi#L217) | | `PJSK_HELP_AS_IMAGE` | å¦ | `True` |
+æ¯å¦å°å¸®å©ä¿¡æ¯æ¸²æä¸ºå¾çåé | | `PJSK_REPLY` | å¦ | `True` |
+æ¯å¦åå¤æ¶æ¯åéè | ## ð ä½¿ç¨ ç´æ¥ä½¿ç¨æä»¤ `pjsk`
+è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h` äºè§£ä½¿ç¨ Shell-Like
+æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾  ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example]
+(./readme/example-interact.png)   ä½¿ç¨ Shell-Like æä»¤ ![example](./readme/
+example.png)  ## ð ç¢ç¢å¿µ - ~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
 å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æ issue æè [å ç¾¤](https://
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.6
-- æä»¶ä¼æè§è²åéæ°æåºè¡¨æåè¡¨ä¸è¡¨æ
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.7
+- ä¿®å¤åæ°ä¸º `0` æ¶ä¸çæç Bug -
+ç°å¨å¯ä»¥å³é­åå¤æ¶æ¯åéèçç¹æ§äº - å½ä»¤åæ°è°æ´ï¼ -
+å é¤ `--weight` åæ°ï¼å ä¸ºæ²¡æå®éæä¹ - `--rotate`
+åæ°å¯ä»¥æ¥åå°æ°äº - `--stroke-width` åæ°æ·»å ç®å `-W` - `--
+line-spacing` åæ°æ·»å ç®å `-C` ### 0.2.6 -
+æä»¶ä¼æè§è²åéæ°æåºè¡¨æåè¡¨ä¸è¡¨æ
 IDï¼ä»¥é²æ°æ®æºè¡¨æ ID å²çª - è§è²åè¡¨åç§°å±ç¤ºä¼å ### 0.2.5
 - ä½¿ç¨èªå·±åå¹¶çå­ä½æä»¶é¿åæäºå­ä¸æ¾ç¤ºçé®é¢ ### 0.2.4
 - å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
 å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
 éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
 0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
```

### Comparing `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
     usage="使用指令 `pjsk -h` 查看帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__main__.py` & `nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from nonebot.rule import ArgumentParser, Namespace
 from nonebot.typing import T_State
 from nonebot_plugin_saa import Image, MessageFactory, MessageSegmentFactory, Text
 from numpy import rad2deg
 
 from .config import config
 from .draw import (
-    DEFAULT_FONT_WEIGHT,
     DEFAULT_LINE_SPACING,
     DEFAULT_STROKE_WIDTH,
     TextTooLargeError,
     draw_sticker,
     get_all_characters,
     get_character_stickers,
     i2b,
@@ -39,17 +38,17 @@
     "--id",
     help="表情 ID，可以通过指令 `pjsk列表` 查询，不提供时则随机选择",
 )
 cmd_generate_parser.add_argument("-x", help="文字的中心 x 坐标")
 cmd_generate_parser.add_argument("-y", help="文字的中心 y 坐标")
 cmd_generate_parser.add_argument("-r", "--rotate", help="文字旋转的角度")
 cmd_generate_parser.add_argument("-s", "--size", help="文字的大小，不指定时会以默认大小为最大值自动调整")
-cmd_generate_parser.add_argument("-w", "--weight", help="文本粗细")
-cmd_generate_parser.add_argument("--stroke-width", help="文本描边宽度")
-cmd_generate_parser.add_argument("--line-spacing", help="文本行间距")
+# cmd_generate_parser.add_argument("-w", "--weight", help="文本粗细")
+cmd_generate_parser.add_argument("-W", "--stroke-width", help="文本描边宽度")
+cmd_generate_parser.add_argument("-C", "--line-spacing", help="文本行间距")
 
 cmd_generate = on_shell_command(
     "pjsk",
     parser=cmd_generate_parser,
     aliases={"啤酒烧烤"},
     priority=2,
 )
@@ -94,15 +93,15 @@
     if foo.status == 0:
         if config.pjsk_help_as_image:
             try:
                 img = await use_image_cache(render_help_image, "help", "JPEG")(HELP)
             except Exception:
                 logger.exception("Error occurred while rendering help image")
                 await matcher.finish("生成帮助图片时出错，请检查后台日志")
-            await MessageFactory([Image(img)]).finish(reply=True)
+            await MessageFactory([Image(img)]).finish(reply=config.pjsk_reply)
 
         await matcher.finish(HELP)
 
     await matcher.finish(f"参数解析出错：{foo.message}")
 
 
 # command or enter interact mode handler
@@ -120,25 +119,29 @@
     default_text = selected_sticker.default_text
     try:
         image = await draw_sticker(
             selected_sticker,
             text=" ".join(texts),  # if texts else default_text.text,
             x=resolve_value(args.x, default_text.x),
             y=resolve_value(args.y, default_text.y),
-            rotate=resolve_value(args.rotate, rad2deg(default_text.r / 10)),
+            rotate=(  # 惰性求值
+                args.rotate
+                if args.rotate is None
+                else resolve_value(args.rotate, rad2deg(default_text.r / 10), float)
+            ),
             font_size=resolve_value(args.size, default_text.s),
             stroke_width=resolve_value(args.stroke_width, DEFAULT_STROKE_WIDTH),
             line_spacing=resolve_value(args.line_spacing, DEFAULT_LINE_SPACING, float),
-            font_weight=resolve_value(args.weight, DEFAULT_FONT_WEIGHT),
+            # font_weight=resolve_value(args.weight, DEFAULT_FONT_WEIGHT),
             auto_adjust=args.size is None,
         )
     except Exception as e:
         await matcher.finish(format_draw_error(e))
 
-    await MessageFactory([Image(i2b(image))]).finish(reply=True)
+    await MessageFactory([Image(i2b(image))]).finish(reply=config.pjsk_reply)
 
 
 # interact mode or sticker list
 @cmd_sticker_list.handle()
 async def _(matcher: Matcher, arg: Message = CommandArg()):
     if remove_cmd_prefix(arg.extract_plain_text()).strip():
         matcher.set_arg("character", arg)
@@ -161,15 +164,15 @@
     try:
         image = await get_all_characters()
     except Exception:
         logger.exception("Error occurred while getting character list")
         await matcher.finish("获取角色列表图片出错，请检查后台日志")
 
     factory = MessageFactory([Image(image), Text(tip_text)])
-    await (factory.send if interact else factory.finish)(reply=True)
+    await (factory.send if interact else factory.finish)(reply=config.pjsk_reply)
 
 
 # sticker id list
 @cmd_generate.got("character")
 @cmd_sticker_list.got("character")
 async def _(matcher: Matcher, state: T_State, arg_msg: Message = Arg("character")):
     character = remove_cmd_prefix(arg_msg.extract_plain_text()).strip()
@@ -201,15 +204,15 @@
         await matcher.finish("没有找到对应名称的角色")
 
     segments: List[MessageSegmentFactory] = [Image(image)]
     if interact:
         segments.append(Text("请发送你要生成表情的 ID"))
 
     factory = MessageFactory(segments)
-    await (factory.send if interact else factory.finish)(reply=True)
+    await (factory.send if interact else factory.finish)(reply=config.pjsk_reply)
 
 
 # below are interact mode handlers
 @cmd_generate.got("sticker_id")
 async def _(matcher: Matcher, arg: str = ArgPlainText("sticker_id")):
     arg = remove_cmd_prefix(arg).strip()
     await handle_exit(matcher, arg)
@@ -232,8 +235,8 @@
     assert sticker_info is not None
 
     try:
         image = await draw_sticker(sticker_info, text=text, auto_adjust=True)
     except Exception as e:
         await matcher.finish(format_draw_error(e))
 
-    await MessageFactory([Image(i2b(image))]).finish(reply=True)
+    await MessageFactory([Image(i2b(image))]).finish(reply=config.pjsk_reply)
```

### Comparing `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 
     pjsk_assets_prefix: str = (
         "https://raw.gitmirror.com/TheOriginalAyaka/sekai-stickers/main/"
     )
     pjsk_repo_prefix: str = "https://raw.gitmirror.com/Agnes4m/nonebot_plugin_pjsk/main/"
 
     pjsk_emoji_source: str = "Apple"
-    """Emoji 来源，可选值见 https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/imagetext_py.pyi#L217"""
-
     pjsk_help_as_image: bool = True
-    """是否将帮助信息作为图片发送"""
+    pjsk_reply: bool = True
 
     @validator("pjsk_assets_prefix", "pjsk_repo_prefix")
     def check_url(cls, v):  # noqa: N805
         if not v.startswith(("http://", "https://")):
             raise ValueError("URL must start with http:// or https://")
         if not v.endswith("/"):
             v = f"{v}/"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .resource import (
     CACHE_FOLDER,
     FONT_PATHS,
     LOADED_STICKER_INFO,
     RESOURCE_FOLDER,
     StickerInfo,
 )
-from .utils import split_list
+from .utils import qor, split_list
 
 P = ParamSpec("P")
 ColorType = Union[str, Tuple[int, int, int], Tuple[int, int, int, int]]
 
 
 FONT: Optional[Font] = None
 SYSTEM_FONT: Optional[Font] = None
@@ -186,15 +186,15 @@
 
 
 def paste_text_on_image(
     image: Image.Image,
     text: Image.Image,
     x: int,
     y: int,
-    rotate: int,
+    rotate: float,
 ) -> Image.Image:
     image = resize_sticker(image, CANVAS_SIZE)
 
     text_bg = Image.new("RGBA", CANVAS_SIZE, (255, 255, 255, 0))
     text = text.rotate(-rotate, resample=Image.BICUBIC, expand=True)
     text_bg.paste(text, (x - text.size[0] // 2, y - text.size[1] // 2), text)
 
@@ -222,39 +222,39 @@
 
 
 async def draw_sticker(
     info: StickerInfo,
     text: Optional[str] = None,
     x: Optional[int] = None,
     y: Optional[int] = None,
-    rotate: Optional[int] = None,
+    rotate: Optional[float] = None,
     font_size: Optional[int] = None,
     stroke_width: Optional[int] = None,
     line_spacing: Optional[float] = None,
     font_weight: Optional[int] = None,
     auto_adjust: bool = False,  # noqa: FBT001
 ) -> Image.Image:
     default_text = info.default_text
     sticker_img = await anyio.Path(RESOURCE_FOLDER / info.img).read_bytes()
     text_img = await render_text(
-        text or default_text.text,
+        qor(text, default_text.text),
         info.color,
-        font_size or default_text.s,
-        font_weight or DEFAULT_FONT_WEIGHT,
-        stroke_width or DEFAULT_STROKE_WIDTH,
-        line_spacing or DEFAULT_LINE_SPACING,
+        qor(font_size, default_text.s),
+        qor(font_weight, DEFAULT_FONT_WEIGHT),
+        qor(stroke_width, DEFAULT_STROKE_WIDTH),
+        qor(line_spacing, DEFAULT_LINE_SPACING),
         max_width=CANVAS_SIZE[0] if auto_adjust else None,
         will_rotate=rotate,
     )
     return paste_text_on_image(
         Image.open(BytesIO(sticker_img)).convert("RGBA"),
         text_img,
-        x or default_text.x,
-        y or default_text.y,
-        rotate or rad2deg(default_text.r / 10),
+        qor(x, default_text.x),
+        qor(y, default_text.y),
+        rotate if rotate is not None else rad2deg(default_text.r / 10),  # 惰性求值
     )
 
 
 def render_summary_picture(
     image_list: List[Image.Image],
     padding: int = 15,
     line_max: int = 5,
@@ -305,15 +305,15 @@
         line = line[:-1]
     wrapped.append(line)
     wrapped.extend(wrap_line(tail, font, width))
     return wrapped
 
 
 async def render_help_image(text: str) -> Image.Image:
-    width = 900
+    width = 1130
     font_size = 24
     padding = 24
     font = ImageFont.truetype(str(FONT_PATHS[-1]), font_size)
 
     warped_lines: List[str] = list(
         itertools.chain.from_iterable(
             wrap_line(line, font, width - padding * 2) for line in text.split("\n")
```

### Comparing `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,24 +86,26 @@
     tasks: List[Coroutine] = [
         download(path.name) for path in FONT_PATHS if not path.exists()
     ]
     await asyncio.gather(*tasks)
 
 
 async def load_sticker_info():
-    logger.info("Updating sticker information")
+    logger.debug("Updating sticker information")
 
     path = anyio.Path(STICKER_INFO_CACHE)
     try:
         loaded_text = await async_request("src/characters.json", ResponseType.TEXT)
         await path.write_text(loaded_text, encoding="u8")
     except Exception as e:
         if not (await path.exists()):
             raise
-        logger.warning(f"Failed to load sticker information, using cached data: {e!r}")
+        logger.warning(
+            f"Failed to download sticker information, using cached data: {e!r}",
+        )
         loaded_text = await path.read_text(encoding="u8")
 
     LOADED_STICKER_INFO.clear()
     LOADED_STICKER_INFO.extend(parse_raw_as(List[StickerInfo], loaded_text))
     sort_stickers()
 
 
@@ -115,30 +117,30 @@
         path = anyio.Path(RESOURCE_FOLDER) / path_str
         if not (await (dir_name := path.parent).exists()):
             await dir_name.mkdir(parents=True, exist_ok=True)
 
         logger.opt(colors=True).info(f"Downloading sticker <y>{path.name}</y>")
         await path.write_bytes(await async_request(f"public/img/{path_str}"))
 
-    logger.info("Checking and downloading sticker assets")
+    logger.debug("Checking and downloading sticker assets")
     tasks: List[Coroutine] = [
         download(sticker_info.img)
         for sticker_info in LOADED_STICKER_INFO
         if not (RESOURCE_FOLDER / sticker_info.img).exists()
     ]
     await asyncio.gather(*tasks)
 
 
 async def check_and_download_resource():
     await load_sticker_info()
     await check_and_download_stickers()
 
 
 async def prepare_resource():
-    logger.info("Checking and downloading resources")
+    logger.debug("Checking and downloading resources")
     await asyncio.gather(
         check_and_download_resource(),
         check_and_download_font(),
     )
     logger.success("Successfully checked resources")
```

### Comparing `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.7/nonebot_plugin_pjsk/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from asyncio import Semaphore
 from enum import Enum, auto
-from typing import Any, Iterable, List, Literal, Optional, Type, TypeVar, overload
+from typing import (
+    Any,
+    Iterable,
+    List,
+    Literal,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
 
-from httpx import AsyncClient
+from aiohttp import ClientSession
 
 from .config import config
 
 T = TypeVar("T")
 TN = TypeVar("TN", int, float)
+TA = TypeVar("TA")
+TB = TypeVar("TB")
 
 
 class ResponseType(Enum):
     JSON = auto()
     TEXT = auto()
     BYTES = auto()
 
@@ -46,22 +58,22 @@
 async def async_request(
     url: str,
     response_type: ResponseType = ResponseType.BYTES,
     prefix: str = config.pjsk_assets_prefix,
 ) -> Any:
     if not url.startswith(("http://", "https://")):
         url = f"{prefix}{url}"
-    async with AsyncClient() as client:
-        response = await client.get(url)
-        response.raise_for_status()
-        if response_type == ResponseType.JSON:
-            return response.json()
-        if response_type == ResponseType.TEXT:
-            return response.text
-        return response.content
+    async with ClientSession() as session:
+        async with session.get(url) as response:
+            response.raise_for_status()
+            if response_type == ResponseType.JSON:
+                return await response.json()
+            if response_type == ResponseType.TEXT:
+                return await response.text()
+            return await response.read()
 
 
 def with_semaphore(semaphore: Semaphore):
     def decorator(func):
         async def wrapper(*args, **kwargs):
             async with semaphore:
                 return await func(*args, **kwargs)
@@ -97,7 +109,11 @@
         return default
     try:
         if value.startswith("^"):
             return default + expected_type(value[1:])
         return expected_type(value)  # type: ignore pylance 抽风
     except Exception as e:
         raise ResolveValueError(value) from e
+
+
+def qor(a: Optional[TA], b: TB) -> Union[TA, TB]:
+    return a if a is not None else b
```

### Comparing `nonebot_plugin_pjsk-0.2.6/pyproject.toml` & `nonebot_plugin_pjsk-0.2.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.6"
+version = "0.2.7"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-plugin-send-anything-anywhere>=0.2.7",
     "imagetext-py>=2.1.3",
-    "httpx>=0.24.1",
+    "aiohttp>=3.8.5",
     "numpy>=1.25.1",
     "anyio>=3.7.1",
 ]
 requires-python = ">=3.9,<4.0"
 keywords = [
     "pjsk",
     "nonebot2",
```

### Comparing `nonebot_plugin_pjsk-0.2.6/PKG-INFO` & `nonebot_plugin_pjsk-0.2.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.6
+Version: 0.2.7
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
 Requires-Dist: imagetext-py>=2.1.3
-Requires-Dist: httpx>=0.24.1
+Requires-Dist: aiohttp>=3.8.5
 Requires-Dist: numpy>=1.25.1
 Requires-Dist: anyio>=3.7.1
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 -->
 
 <div align="center">
@@ -133,16 +133,23 @@
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
-见 [config.py](./nonebot_plugin_pjsk/config.py) 文件  
-插件开箱即用，如无需要则无须配置
+插件开箱即用，所有配置项皆为可选。请**按需添加**下面的配置项到 `.env` 文件中
+
+|        配置项        | 必填 | 默认值  |                                                              说明                                                              |
+| :------------------: | :--: | :-----: | :----------------------------------------------------------------------------------------------------------------------------: |
+| `PJSK_ASSETS_PREFIX` |  否  |   ...   |                          TheOriginalAyaka/sekai-stickers 仓库 GitHubUserContent 地址，默认为国内镜像                           |
+|  `PJSK_REPO_PREFIX`  |  否  |   ...   |                                         本仓库 GitHubUserContent 地址，默认为国内镜像                                          |
+| `PJSK_EMOJI_SOURCE`  |  否  | `Apple` | Emoji 来源，可选值见 [这里](https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/imagetext_py.pyi#L217) |
+| `PJSK_HELP_AS_IMAGE` |  否  | `True`  |                                                  是否将帮助信息渲染为图片发送                                                  |
+|     `PJSK_REPLY`     |  否  | `True`  |                                                       是否回复消息发送者                                                       |
 
 ## 🎉 使用
 
 直接使用指令 `pjsk` 进入交互创建模式；  
 使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助
 
 ### 效果图
@@ -177,14 +184,24 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.7
+
+- 修复参数为 `0` 时不生效的 Bug
+- 现在可以关闭回复消息发送者的特性了
+- 命令参数调整：
+  - 删除 `--weight` 参数，因为没有实际意义
+  - `--rotate` 参数可以接受小数了
+  - `--stroke-width` 参数添加简写 `-W`
+  - `--line-spacing` 参数添加简写 `-C`
+
 ### 0.2.6
 
 - 插件会按角色名重新排序表情列表与表情 ID，以防数据源表情 ID 冲突
 - 角色列表名称展示优化
 
 ### 0.2.5
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.6 Summary: Project
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.7 Summary: Project
 Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
 https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Project-URL:
 Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk Requires-Python:
 <4.0,>=3.9 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-
 anything-anywhere>=0.2.7 Requires-Dist: imagetext-py>=2.1.3 Requires-Dist:
-httpx>=0.24.1 Requires-Dist: numpy>=1.25.1 Requires-Dist: anyio>=3.7.1
+aiohttp>=3.8.5 Requires-Dist: numpy>=1.25.1 Requires-Dist: anyio>=3.7.1
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
 ## ð¬ åè¨ -
@@ -29,32 +29,46 @@
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½® è§ [config.py](./
-nonebot_plugin_pjsk/config.py) æä»¶
-æä»¶å¼ç®±å³ç¨ï¼å¦æ éè¦åæ é¡»éç½® ## ð ä½¿ç¨
-ç´æ¥ä½¿ç¨æä»¤ `pjsk` è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h`
-äºè§£ä½¿ç¨ Shell-Like æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾
-ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example](./readme/example-interact.png)   ä½¿ç¨
-Shell-Like æä»¤ ![example](./readme/example.png)  ## ð ç¢ç¢å¿µ -
-~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
+"nonebot_plugin_pjsk" ] ```  ## âï¸ éç½®
+æä»¶å¼ç®±å³ç¨ï¼ææéç½®é¡¹çä¸ºå¯éãè¯·**æéæ·»å **ä¸é¢çéç½®é¡¹å°
+`.env` æä»¶ä¸­ | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | | :---------------
+---: | :--: | :-----: | :------------------------------------------------------
+----------------------------------------------------------------------: | |
+`PJSK_ASSETS_PREFIX` | å¦ | ... | TheOriginalAyaka/sekai-stickers ä»åº
+GitHubUserContent å°åï¼é»è®¤ä¸ºå½åéå | | `PJSK_REPO_PREFIX` | å¦ |
+... | æ¬ä»åº GitHubUserContent å°åï¼é»è®¤ä¸ºå½åéå | |
+`PJSK_EMOJI_SOURCE` | å¦ | `Apple` | Emoji æ¥æºï¼å¯éå¼è§ [è¿é]
+(https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/
+imagetext_py.pyi#L217) | | `PJSK_HELP_AS_IMAGE` | å¦ | `True` |
+æ¯å¦å°å¸®å©ä¿¡æ¯æ¸²æä¸ºå¾çåé | | `PJSK_REPLY` | å¦ | `True` |
+æ¯å¦åå¤æ¶æ¯åéè | ## ð ä½¿ç¨ ç´æ¥ä½¿ç¨æä»¤ `pjsk`
+è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h` äºè§£ä½¿ç¨ Shell-Like
+æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾  ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example]
+(./readme/example-interact.png)   ä½¿ç¨ Shell-Like æä»¤ ![example](./readme/
+example.png)  ## ð ç¢ç¢å¿µ - ~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
 å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æ issue æè [å ç¾¤](https://
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.6
-- æä»¶ä¼æè§è²åéæ°æåºè¡¨æåè¡¨ä¸è¡¨æ
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.7
+- ä¿®å¤åæ°ä¸º `0` æ¶ä¸çæç Bug -
+ç°å¨å¯ä»¥å³é­åå¤æ¶æ¯åéèçç¹æ§äº - å½ä»¤åæ°è°æ´ï¼ -
+å é¤ `--weight` åæ°ï¼å ä¸ºæ²¡æå®éæä¹ - `--rotate`
+åæ°å¯ä»¥æ¥åå°æ°äº - `--stroke-width` åæ°æ·»å ç®å `-W` - `--
+line-spacing` åæ°æ·»å ç®å `-C` ### 0.2.6 -
+æä»¶ä¼æè§è²åéæ°æåºè¡¨æåè¡¨ä¸è¡¨æ
 IDï¼ä»¥é²æ°æ®æºè¡¨æ ID å²çª - è§è²åè¡¨åç§°å±ç¤ºä¼å ### 0.2.5
 - ä½¿ç¨èªå·±åå¹¶çå­ä½æä»¶é¿åæäºå­ä¸æ¾ç¤ºçé®é¢ ### 0.2.4
 - å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
 å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
 éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
 0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
```

