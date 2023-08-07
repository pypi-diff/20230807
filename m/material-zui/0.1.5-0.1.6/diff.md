# Comparing `tmp/material_zui-0.1.5.tar.gz` & `tmp/material_zui-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.1.5.tar", max compression
+gzip compressed data, was "material_zui-0.1.6.tar", max compression
```

## Comparing `material_zui-0.1.5.tar` & `material_zui-0.1.6.tar`

### file list

```diff
@@ -1,108 +1,109 @@
--rw-r--r--   0        0        0     1268 2023-07-31 06:57:57.592257 material_zui-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.5/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.5/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.5/src/material_zui/bard/__init__.py
--rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.5/src/material_zui/bard/google_bard.py
--rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.5/src/material_zui/bard/index.py
--rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.5/src/material_zui/bing_ai/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.5/src/material_zui/bing_ai/bing_ai.py
--rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.5/src/material_zui/bing_ai/index.py
--rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.5/src/material_zui/bing_ai/result.py
--rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.5/src/material_zui/bing_ai/type.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.5/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.5/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.5/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.5/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.5/src/material_zui/crawl/image.py
--rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.5/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.5/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.5/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.5/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.5/src/material_zui/date_time/__init__.pyc
--rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.5/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0      123 2023-07-16 12:10:14.125544 material_zui-0.1.5/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.5/src/material_zui/date_time/index.pyc
--rw-r--r--   0        0        0     2211 2023-07-16 13:22:45.935630 material_zui-0.1.5/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.5/src/material_zui/dict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.5/src/material_zui/dict/common.py
--rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.5/src/material_zui/dict/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.5/src/material_zui/env/__init__.py
--rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.5/src/material_zui/env/env.py
--rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.5/src/material_zui/env/index.py
--rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.5/src/material_zui/fake/__init__.py
--rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.5/src/material_zui/fake/index.py
--rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.5/src/material_zui/fake/number.py
--rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.5/src/material_zui/file/__init__.py
--rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.5/src/material_zui/file/check.py
--rw-r--r--   0        0        0     2115 2023-07-02 11:49:59.755643 material_zui-0.1.5/src/material_zui/file/common.py
--rw-r--r--   0        0        0      912 2023-07-29 05:10:16.021864 material_zui-0.1.5/src/material_zui/file/download.py
--rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.5/src/material_zui/file/excel.py
--rw-r--r--   0        0        0      410 2023-07-29 04:56:18.852441 material_zui-0.1.5/src/material_zui/file/index.py
--rw-r--r--   0        0        0     1757 2023-07-02 11:37:34.980074 material_zui-0.1.5/src/material_zui/file/read.py
--rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.5/src/material_zui/file/type.py
--rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.5/src/material_zui/file/write.py
--rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.5/src/material_zui/generate/__init__.py
--rw-r--r--   0        0        0     2002 2023-06-27 07:49:36.922442 material_zui-0.1.5/src/material_zui/generate/common.py
--rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.5/src/material_zui/generate/index.py
--rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.5/src/material_zui/gpt/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.5/src/material_zui/gpt/gpt_vietnam.py
--rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.5/src/material_zui/gpt/index.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.5/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.5/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.5/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.5/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.5/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.5/src/material_zui/image/data.py
--rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.5/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.5/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.5/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.5/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.5/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.5/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.5/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.5/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       21 2023-07-30 11:44:27.414884 material_zui-0.1.5/src/material_zui/list/__init__.py
--rw-r--r--   0        0        0     4415 2023-07-30 13:24:18.913364 material_zui-0.1.5/src/material_zui/list/common.py
--rw-r--r--   0        0        0      154 2023-07-30 13:24:35.996722 material_zui-0.1.5/src/material_zui/list/index.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.5/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.5/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.5/src/material_zui/log/log.py
--rw-r--r--   0        0        0       21 2023-07-29 03:49:37.553797 material_zui-0.1.5/src/material_zui/network/__init__.py
--rw-r--r--   0        0        0     2606 2023-07-31 06:13:07.060055 material_zui-0.1.5/src/material_zui/network/common.py
--rw-r--r--   0        0        0       70 2023-07-29 11:25:06.057119 material_zui-0.1.5/src/material_zui/network/index.py
--rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.5/src/material_zui/number/__init__.py
--rw-r--r--   0        0        0      380 2023-07-29 05:39:04.869919 material_zui-0.1.5/src/material_zui/number/common.py
--rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.5/src/material_zui/number/index.py
--rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.5/src/material_zui/os/__init__.py
--rw-r--r--   0        0        0      840 2023-07-12 02:26:10.443342 material_zui-0.1.5/src/material_zui/os/common.py
--rw-r--r--   0        0        0      125 2023-07-12 02:29:41.294270 material_zui-0.1.5/src/material_zui/os/index.py
--rw-r--r--   0        0        0      330 2023-07-12 02:54:51.769004 material_zui-0.1.5/src/material_zui/os/terminal.py
--rw-r--r--   0        0        0     1480 2023-07-31 06:43:38.844082 material_zui-0.1.5/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.5/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.5/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.5/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.5/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.5/src/material_zui/selenium/__init__.py
--rw-r--r--   0        0        0     4155 2023-07-31 01:53:50.526065 material_zui-0.1.5/src/material_zui/selenium/chrome.py
--rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.5/src/material_zui/selenium/common.py
--rw-r--r--   0        0        0     2836 2023-07-30 03:31:40.599764 material_zui-0.1.5/src/material_zui/selenium/firefox.py
--rw-r--r--   0        0        0      150 2023-07-16 03:36:28.421675 material_zui-0.1.5/src/material_zui/selenium/index.py
--rw-r--r--   0        0        0     9288 2023-07-30 03:32:09.290158 material_zui-0.1.5/src/material_zui/selenium/selenium.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.5/src/material_zui/setup.py
--rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.5/src/material_zui/string/__init__.py
--rw-r--r--   0        0        0     3403 2023-07-29 11:24:14.277396 material_zui-0.1.5/src/material_zui/string/common.py
--rw-r--r--   0        0        0      345 2023-07-29 11:24:14.137397 material_zui-0.1.5/src/material_zui/string/index.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.5/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.5/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       21 2023-07-29 05:45:31.405279 material_zui-0.1.5/src/material_zui/thread/__init__.py
--rw-r--r--   0        0        0      455 2023-07-30 14:11:11.539245 material_zui-0.1.5/src/material_zui/thread/common.py
--rw-r--r--   0        0        0       37 2023-07-29 05:53:44.309345 material_zui-0.1.5/src/material_zui/thread/index.py
--rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.5/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.5/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.5/src/material_zui/utility/__init__.py
--rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.5/src/material_zui/utility/common.py
--rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.5/src/material_zui/utility/index.py
--rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.5/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.5/src/material_zui/validate/common.py
--rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.5/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 material_zui-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1268 2023-08-07 04:51:30.928691 material_zui-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.6/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.6/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.6/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.6/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.6/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.6/src/material_zui/bing_ai/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.6/src/material_zui/bing_ai/bing_ai.py
+-rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.6/src/material_zui/bing_ai/index.py
+-rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.6/src/material_zui/bing_ai/result.py
+-rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.6/src/material_zui/bing_ai/type.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.6/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.6/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2225 2023-08-07 04:40:15.184256 material_zui-0.1.6/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.6/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.6/src/material_zui/crawl/image.py
+-rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.6/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.6/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.6/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.6/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.6/src/material_zui/date_time/__init__.pyc
+-rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.6/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0      143 2023-08-06 05:17:57.162814 material_zui-0.1.6/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.6/src/material_zui/date_time/index.pyc
+-rw-r--r--   0        0        0     2527 2023-08-06 05:17:57.286815 material_zui-0.1.6/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.6/src/material_zui/dict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.6/src/material_zui/dict/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.6/src/material_zui/dict/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.6/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.6/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.6/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.6/src/material_zui/fake/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.6/src/material_zui/fake/index.py
+-rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.6/src/material_zui/fake/number.py
+-rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.6/src/material_zui/file/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.6/src/material_zui/file/check.py
+-rw-r--r--   0        0        0     2755 2023-08-07 03:17:28.950762 material_zui-0.1.6/src/material_zui/file/common.py
+-rw-r--r--   0        0        0      912 2023-07-29 05:10:16.021864 material_zui-0.1.6/src/material_zui/file/download.py
+-rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.6/src/material_zui/file/excel.py
+-rw-r--r--   0        0        0      470 2023-08-07 03:16:11.325903 material_zui-0.1.6/src/material_zui/file/index.py
+-rw-r--r--   0        0        0     1757 2023-07-02 11:37:34.980074 material_zui-0.1.6/src/material_zui/file/read.py
+-rw-r--r--   0        0        0      972 2023-08-07 03:17:29.030763 material_zui-0.1.6/src/material_zui/file/remove.py
+-rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.6/src/material_zui/file/type.py
+-rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.6/src/material_zui/file/write.py
+-rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.6/src/material_zui/generate/__init__.py
+-rw-r--r--   0        0        0     2002 2023-06-27 07:49:36.922442 material_zui-0.1.6/src/material_zui/generate/common.py
+-rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.6/src/material_zui/generate/index.py
+-rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.6/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.6/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.6/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.6/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.6/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.6/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.6/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.6/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.6/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.6/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.6/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.6/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.6/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.6/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.6/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.6/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.6/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       21 2023-07-30 11:44:27.414884 material_zui-0.1.6/src/material_zui/list/__init__.py
+-rw-r--r--   0        0        0     4668 2023-08-06 12:20:59.880852 material_zui-0.1.6/src/material_zui/list/common.py
+-rw-r--r--   0        0        0      184 2023-08-06 12:20:59.724853 material_zui-0.1.6/src/material_zui/list/index.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.6/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-06 12:21:44.396562 material_zui-0.1.6/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      767 2023-08-06 12:24:22.023566 material_zui-0.1.6/src/material_zui/log/log.py
+-rw-r--r--   0        0        0       21 2023-07-29 03:49:37.553797 material_zui-0.1.6/src/material_zui/network/__init__.py
+-rw-r--r--   0        0        0     3022 2023-08-01 02:49:27.923745 material_zui-0.1.6/src/material_zui/network/common.py
+-rw-r--r--   0        0        0      110 2023-08-01 01:56:43.438120 material_zui-0.1.6/src/material_zui/network/index.py
+-rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.6/src/material_zui/number/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-29 05:39:04.869919 material_zui-0.1.6/src/material_zui/number/common.py
+-rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.6/src/material_zui/number/index.py
+-rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.6/src/material_zui/os/__init__.py
+-rw-r--r--   0        0        0      840 2023-07-12 02:26:10.443342 material_zui-0.1.6/src/material_zui/os/common.py
+-rw-r--r--   0        0        0      125 2023-07-12 02:29:41.294270 material_zui-0.1.6/src/material_zui/os/index.py
+-rw-r--r--   0        0        0      330 2023-07-12 02:54:51.769004 material_zui-0.1.6/src/material_zui/os/terminal.py
+-rw-r--r--   0        0        0     1480 2023-07-31 06:43:38.844082 material_zui-0.1.6/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.6/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.6/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.6/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.6/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.6/src/material_zui/selenium/__init__.py
+-rw-r--r--   0        0        0     4110 2023-08-06 03:49:00.463474 material_zui-0.1.6/src/material_zui/selenium/chrome.py
+-rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.6/src/material_zui/selenium/common.py
+-rw-r--r--   0        0        0     2836 2023-07-30 03:31:40.599764 material_zui-0.1.6/src/material_zui/selenium/firefox.py
+-rw-r--r--   0        0        0      150 2023-07-16 03:36:28.421675 material_zui-0.1.6/src/material_zui/selenium/index.py
+-rw-r--r--   0        0        0     9084 2023-08-06 14:19:57.991524 material_zui-0.1.6/src/material_zui/selenium/selenium.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.6/src/material_zui/setup.py
+-rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.6/src/material_zui/string/__init__.py
+-rw-r--r--   0        0        0     3411 2023-08-06 03:36:41.050336 material_zui-0.1.6/src/material_zui/string/common.py
+-rw-r--r--   0        0        0      345 2023-07-29 11:24:14.137397 material_zui-0.1.6/src/material_zui/string/index.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.6/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.6/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       21 2023-07-29 05:45:31.405279 material_zui-0.1.6/src/material_zui/thread/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-30 14:11:11.539245 material_zui-0.1.6/src/material_zui/thread/common.py
+-rw-r--r--   0        0        0       37 2023-07-29 05:53:44.309345 material_zui-0.1.6/src/material_zui/thread/index.py
+-rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.6/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.6/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.6/src/material_zui/utility/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.6/src/material_zui/utility/common.py
+-rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.6/src/material_zui/utility/index.py
+-rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.6/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.6/src/material_zui/validate/common.py
+-rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.6/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 material_zui-0.1.6/PKG-INFO
```

### Comparing `material_zui-0.1.5/pyproject.toml` & `material_zui-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.1.5"
+version = "0.1.6"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
```

### Comparing `material_zui-0.1.5/src/material_zui/ResizeImage.py` & `material_zui-0.1.6/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/bard/google_bard.py` & `material_zui-0.1.6/src/material_zui/bard/google_bard.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/bing_ai/bing_ai.py` & `material_zui-0.1.6/src/material_zui/bing_ai/bing_ai.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/bing_ai/result.py` & `material_zui-0.1.6/src/material_zui/bing_ai/result.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/compress/text.py` & `material_zui-0.1.6/src/material_zui/compress/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-def encode(line):
+from typing import Any, TypeVar
+
+T = TypeVar('T')
+
+
+def encode(lines: list[str]) -> list[str]:
     """
     INPUT:  A line of ASCII String.
     OUTPUT: A List of Run-Length Encoded of the input string.
     """
-    if not line:
+    if not lines:
         return [""]
     else:
-        last_char = line[0]
-        length = len(line)
+        last_char = lines[0]
+        length = len(lines)
         i = 1
-        while i < length and last_char == line[i]:
+        while i < length and last_char == lines[i]:
             i += 1
-        return [str(i), last_char] + encode(line[i:])
+        return [str(i), last_char] + encode(lines[i:])
 
 
-def decode(parsed_string):
+def decode(parsed_string: Any) -> str:
     """
     INPUT:  A List of List parsed from encoded string
     OUTPUT: A String of Decoded line
     """
     decoded = ""
     for item in parsed_string:
         try:
```

### Comparing `material_zui-0.1.5/src/material_zui/crawl/image.py` & `material_zui-0.1.6/src/material_zui/crawl/image.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/crontab/index.py` & `material_zui-0.1.6/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/date_time/time.py` & `material_zui-0.1.6/src/material_zui/date_time/time.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,28 +66,40 @@
 
 def time_to_seconds(value: str) -> int:
     """Converts a string time to seconds.
     Args:
       value: A string time in the format HH:MM:SS.
     Returns:
       The number of seconds in the time string.
+    - ex: ('00:12:34') => 754
     """
     while len(value.split(":")) < 3:
         value = f'00:{value}'
     hours, minutes, seconds = value.split(":")
     seconds = int(hours) * 3600 + int(minutes) * 60 + int(seconds)
     return seconds
 
 
-def second_to_time(seconds: int) -> str:
+def second_to_str_time(seconds: int) -> str:
     """Converts seconds to time in the format HH:MM:SS.
     Args:
       seconds: The number of seconds.
 
     Returns:
       A string representing the time in the format HH:MM:SS.
     """
     hours = seconds // 3600
     minutes = (seconds % 3600) // 60
     seconds = seconds % 60
     time_str = f"{hours:02d}:{minutes:02d}:{seconds:02d}"
     return time_str
+
+
+def second_to_time(seconds: int) -> dict[{'hours': int, 'minutes': int, 'seconds': int}]:
+    hours = seconds // 3600
+    minutes = (seconds % 3600) // 60
+    seconds = seconds % 60
+    return {
+        'hours': hours,
+        'minutes': minutes,
+        'seconds': seconds
+    }
```

### Comparing `material_zui-0.1.5/src/material_zui/file/check.py` & `material_zui-0.1.6/src/material_zui/file/check.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/file/common.py` & `material_zui-0.1.6/src/material_zui/file/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import os
 from anyio import Path
 
-from material_zui.list import map_to, filter_to
+from material_zui.list import map_to, filter_to, sort_alphabetically
 from .type import ZuiFile
 
 
-def get_names(directory_path: str) -> list[str]:
+def get_names(directory_path: str, is_sort: bool = True, limit: int = 0) -> list[str]:
     '''
     Get all file names in a directory
     '''
-    return os.listdir(directory_path)
+    paths = os.listdir(directory_path)
+    paths = sort_alphabetically(paths) if is_sort else paths
+    return paths[:limit] if limit else paths
 
 
-def get_paths(directory_path: str) -> list[str]:
-    filenames = get_names(directory_path)
+def get_file_names(directory_path: str, is_sort: bool = True, limit: int = 0) -> list[str]:
+    '''
+    Get all file names in a directory
+    '''
+    file_names = get_names(directory_path, is_sort)
+    file_names = filter_to(file_names, lambda file_name,
+                           _: is_file(file_name))
+    return file_names[:limit] if limit else file_names
+
+
+def get_paths(directory_path: str, is_sort: bool = True, limit: int = 0) -> list[str]:
+    filenames = get_names(directory_path, is_sort, limit)
     return [os.path.join(directory_path, filename) for filename in filenames]
 
 
 def get_file_info(file_path: str) -> ZuiFile:
     """
     The function takes a file path as input and returns information about the file such as its name,
     extension, and directory name.
@@ -31,20 +43,24 @@
     file_name = path.name
     name = path.stem
     ext = os.path.splitext(file_path)[1][1:]
     dir_name = os.path.dirname(file_path)
     return {'file_name': file_name, 'name': name, 'dir_name': dir_name, 'ext': ext}
 
 
-# def get_files_info(directory_path: str) -> list[ZuiFile]:
-#     return map_to(get_paths(directory_path), lambda file_path, _: get_file_info(file_path))
-def get_files_info(directory_path: str, ext: str = '') -> list[ZuiFile]:
+def get_files_info(directory_path: str, ext: str = '', is_sort: bool = True, limit: int = 0) -> list[ZuiFile]:
     """
     Returns a list of file information for all files in the specified directory path with the given file extension (if provided). 
 
     :param directory_path: A string representing the path to the directory to search for files.
     :param ext: An optional string representing the file extension to filter files by.
     :return: A list of ZuiFile objects containing information about each file in the directory (if no extension provided) or only files with the specified extension.
     """
-    files_info = map_to(get_paths(directory_path),
+    files_info = map_to(get_paths(directory_path, is_sort),
                         lambda file_path, _: get_file_info(file_path))
-    return files_info if ext == '' else filter_to(files_info, lambda file_info, _: file_info['ext'] == ext)
+    files_info = filter_to(
+        files_info, lambda file_info, _: file_info['ext'] == ext) if ext else files_info
+    return files_info[:limit] if limit else files_info
+
+
+def is_file(file_name: str) -> bool:
+    return bool(file_name) and len(file_name.split('.')) == 2
```

### Comparing `material_zui-0.1.5/src/material_zui/file/download.py` & `material_zui-0.1.6/src/material_zui/file/download.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/file/excel.py` & `material_zui-0.1.6/src/material_zui/file/excel.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/file/read.py` & `material_zui-0.1.6/src/material_zui/file/read.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/file/write.py` & `material_zui-0.1.6/src/material_zui/file/write.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/generate/common.py` & `material_zui-0.1.6/src/material_zui/generate/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/gpt/gpt_vietnam.py` & `material_zui-0.1.6/src/material_zui/gpt/gpt_vietnam.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/colorization.py` & `material_zui-0.1.6/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/combine.py` & `material_zui-0.1.6/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/common.py` & `material_zui-0.1.6/src/material_zui/image/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/convert.py` & `material_zui-0.1.6/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.6/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.6/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/remove_background.py` & `material_zui-0.1.6/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/to_svg.py` & `material_zui-0.1.6/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/transparent_background.py` & `material_zui-0.1.6/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/image/upscale.py` & `material_zui-0.1.6/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/list/common.py` & `material_zui-0.1.6/src/material_zui/list/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,24 @@
             random_index = random.randint(0, len_items - 1)
             random_item = items[random_index]
             if not is_unique or random_item not in random_items:
                 random_items.append(random_item)
         return random_items
     return inner
 
+
+def sort_alphabetically(items: list[str], is_reverse: bool = False) -> list[str]:
+    list_asc = sorted(items, key=str.lower)
+    return reverse(items) if is_reverse else list_asc
+
+
+def is_list(value: Any) -> bool:
+    return isinstance(value, list)
+
+
 # numbers: list[int] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 # def is_even(number: int) -> bool:
 #     return number % 2 == 0
 # even_numbers = filter(is_even, numbers)
 
 # class ZuiList:
 #     def __init__(self, items: list[T]) -> None:
```

### Comparing `material_zui-0.1.5/src/material_zui/network/common.py` & `material_zui-0.1.6/src/material_zui/network/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 
 
 def is_valid_url(url: str) -> bool:
     parsed_url = urlparse(url)
     return bool(parsed_url.scheme and parsed_url.netloc)
 
 
-def is_proxy_working(proxy_url: str, timeout: int | None = None) -> dict[str, Any] | None:
+# def is_proxy_working(proxy_url: str, timeout: int | None = None) -> dict[str, Any] | None:
+    # try:
+    #     check_host = 'https://httpbin.org/ip'
+    #     response = requests.get(check_host, proxies={
+    #                             "http": proxy_url, "https": proxy_url}, timeout=timeout)
+    #     return response.json()
+    # except:
+    #     return None
+
+def is_proxy_working(proxy_url: str, timeout: int | None = 10) -> bool:
     try:
-        check_host = 'https://httpbin.org/ip'
-        response = requests.get(check_host, proxies={
-                                "http": proxy_url, "https": proxy_url}, timeout=timeout)
-        return response.json()
-    except:
-        return None
+        response = requests.get("https://www.google.com",
+                                proxies={"http": f'http://{proxy_url}', "https": f'https://{proxy_url}'}, timeout=timeout)
+        return response.status_code == 200
+    except requests.exceptions.ConnectionError:
+        return False
 
 
-def proxies_working(urls: list[str], timeout: int | None = None):
+def proxies_working(urls: list[str], timeout: int | None = 20):
     results: list[dict[str, Any]] = []
     for url in urls:
         result = is_proxy_working(url, timeout)
+        print(url, result)
         if result:
             results.append(result)
     return results
 
 
 def proxies_working_fp(timeout: int | None = None) -> Callable[[list[str]], list[dict[str, Any]]]:
     def inner(urls: list[str]) -> list[dict[str, Any]]:
```

### Comparing `material_zui-0.1.5/src/material_zui/os/common.py` & `material_zui-0.1.6/src/material_zui/os/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/readme.md` & `material_zui-0.1.6/src/material_zui/readme.md`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/regex/index.py` & `material_zui-0.1.6/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/replicate/index.py` & `material_zui-0.1.6/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/selenium/chrome.py` & `material_zui-0.1.6/src/material_zui/selenium/chrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         - Use for case need authorization, you just need to start `chrome beta` -> login account -> close browswer then
             - start `chrome` on debug mode -> call this method to connect to browser opened
         1. Install `chrome beta` for better automation: https://www.google.com/chrome/beta
         2. Start `chrome` by command: `google-chrome-beta --remote-debugging-port={port}`
                 - `port` must the same with input parameter of this method
         '''
         if not self.is_connected:
-            print(host, port, debug_address)
             self.set_option(host, port, debug_address)
             self.set_service(executable_path, port)
 
             self.driver = webdriver.Chrome(
                 options=self._options, service=self._service)  # type: ignore
             if time_to_wait:
                 self.driver.set_page_load_timeout(time_to_wait)
```

### Comparing `material_zui-0.1.5/src/material_zui/selenium/firefox.py` & `material_zui-0.1.6/src/material_zui/selenium/firefox.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/selenium/selenium.py` & `material_zui-0.1.6/src/material_zui/selenium/selenium.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import platform
-from typing import Any
+from typing import Any, Callable
 
 from bs4 import BeautifulSoup
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
@@ -111,14 +111,20 @@
     def switch_to_frame(self, xpath_value: str) -> None:
         '''
         @xpath_value: must be end with `frame/iframe` like `//*[@id="main"]/div[2]/div/iframe`
         '''
         frame_element = self.find_element_by_xpath(xpath_value)
         self.driver.switch_to.frame(frame_element)
 
+    def switch_to_default_content(self) -> None:
+        '''
+        Out to frame/iframe
+        '''
+        self.driver.switch_to.default_content()
+
     def upload_file(self, xpath_value: str, video_relative_path: str) -> None:
         '''
         @xpath_value: must be end with `input` like `//*[@id="root"]/div/div/div/div/div/div/div/input`
         @video_relative_path: video relative path, from root project directory
         '''
         file_input = self.find_element_by_xpath(xpath_value)
         abs_path = os.path.abspath(video_relative_path)
@@ -172,33 +178,28 @@
         except:
             if time_to_try:
                 time_to_try -= 1
                 return self.send_keys(xpath_value, key_value,
                                       clear_before_send_keys, delay_time, time_to_try)
             return None
 
-    # def send_keys(self, xpath_value: str, key_value: str, clear_before_send_keys: bool = True, delay_time: int = 10, time_to_try: int = 10):
-    #     '''
-    #     Send keys then return that element
-    #     @xpath_value: only valid with element selector can input value
-    #     @clear_before_send_keys:
-    #     - True: clear input before send keys
-    #     - False: value will input after existed value
-    #     '''
-    #     element = self.wait_get(xpath_value, delay_time, time_to_try)
-    #     # element = self.find_element_by_xpath(xpath_value)
-    #     element.click()
-    #     self.delay(10)
-    #     if clear_before_send_keys:
-    #         element.send_keys(Keys.CONTROL + 'a')
-    #         self.delay()
-    #         element.send_keys(Keys.BACKSPACE)
-    #     self.delay()
-    #     element.send_keys(key_value)
-    #     return element
+    def wait_until(self, condition: Callable[[], bool], delay: int = 0, time_to_try: int = 10) -> None:
+        is_continue = time_to_try > 0
+        count = 0
+        try:
+            while is_continue:
+                if count > time_to_try:
+                    is_continue = False
+                count += 1
+
+                if condition():
+                    is_continue = False
+                self.delay(delay)
+        except:
+            self.wait_until(condition, delay, time_to_try-count)
 
     def wait_get(self, xpath_value: str, delay_time: int = 10, time_to_try: int = 10) -> WebElement:
         '''
         - Total wait time of this function is `delay_time x time_to_try`, default is `10x10 = 100 seconds`
         - @delay_time: delay time for each `time_to_try`
         - @time_to_try: how many time to try
         '''
```

### Comparing `material_zui-0.1.5/src/material_zui/setup.py` & `material_zui-0.1.6/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/src/material_zui/string/common.py` & `material_zui-0.1.6/src/material_zui/string/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     consecutive spaces within the string with a single space.
 
     :param text: A string that may contain extra spaces that need to be trimmed down to a single space
     :type text: str
     :return: The function `trim_space` takes a string `text` as input and returns a new string with all
     consecutive spaces replaced by a single space, and leading/trailing spaces removed.
     """
-    return replace_all(r' +', ' ')(text)
+    return replace_all(r' +', ' ')(text.strip())
 
 
 def not_empty(value: Any) -> bool:
     return value != None and len(value) > 0
 
 
 def limit_by_byte(byte_limit: int = 256) -> Callable[[str], str]:
```

### Comparing `material_zui-0.1.5/src/material_zui/utility/common.py` & `material_zui-0.1.6/src/material_zui/utility/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.5/PKG-INFO` & `material_zui-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.1.5
+Version: 0.1.6
 Summary: Material Zui
 Keywords: material,zui,material zui,zui material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: material-zui Version: 0.1.5 Summary: Material Zui
+Metadata-Version: 2.1 Name: material-zui Version: 0.1.6 Summary: Material Zui
 Keywords: material,zui,material zui,zui material Author: chauhmnguyen Author-
 email: chauhoangminhnguyen@gmail.com Requires-Python: >=3.10,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: beautifulsoup4
 (>=4.12.2,<5.0.0) Requires-Dist: edgegpt (>=0.11.6,<0.12.0) Requires-Dist:
 flask (>=2.3.2,<3.0.0) Requires-Dist: free-proxy (>=1.1.1,<2.0.0) Requires-
 Dist: huggingface-hub (>=0.15.1,<0.16.0) Requires-Dist: langchain
```

