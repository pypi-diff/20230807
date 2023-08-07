# Comparing `tmp/GailBot-0.1a9.tar.gz` & `tmp/GailBot-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GailBot-0.1a9.tar", last modified: Tue Jul  4 19:31:28 2023, max compression
+gzip compressed data, was "GailBot-0.2a0.tar", last modified: Mon Aug  7 17:10:49 2023, max compression
```

## Comparing `GailBot-0.1a9.tar` & `GailBot-0.2a0.tar`

### file list

```diff
@@ -1,184 +1,285 @@
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.326785 GailBot-0.1a9/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1066 2023-07-04 18:14:11.000000 GailBot-0.1a9/LICENSE
--rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2023-07-04 19:18:37.000000 GailBot-0.1a9/MANIFEST.in
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13332 2023-07-04 19:31:28.326631 GailBot-0.1a9/PKG-INFO
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11312 2023-07-04 19:27:24.000000 GailBot-0.1a9/README.md
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1349 2023-07-04 19:02:49.000000 GailBot-0.1a9/pyproject.toml
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4339 2023-07-04 18:17:43.000000 GailBot-0.1a9/requirements.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2023-07-04 19:31:28.326821 GailBot-0.1a9/setup.cfg
--rw-r--r--   0 muhammadumair   (501) staff       (20)      355 2023-07-04 18:14:11.000000 GailBot-0.1a9/setup.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.306103 GailBot-0.1a9/src/
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.310777 GailBot-0.1a9/src/GailBot.egg-info/
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13332 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/PKG-INFO
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6142 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)        1 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4401 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/requires.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)       23 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/top_level.txt
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.310928 GailBot-0.1a9/src/config_backend/
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.305546 GailBot-0.1a9/src/config_backend/engines/
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311079 GailBot-0.1a9/src/config_backend/engines/google/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      549 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/engines/google/google_config.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311224 GailBot-0.1a9/src/config_backend/engines/watson/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2196 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/engines/watson/watson_config.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311421 GailBot-0.1a9/src/config_backend/engines/whisper/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      929 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/engines/whisper/whisper_config.toml
--rw-r--r--   0 muhammadumair   (501) staff       (20)      546 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/paths.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311540 GailBot-0.1a9/src/config_backend/plugin/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      142 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/plugin/valid_plugin.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311905 GailBot-0.1a9/src/config_backend/services/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      407 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/services/default_setting.toml
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1119 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/services/format.md
--rw-r--r--   0 muhammadumair   (501) staff       (20)      448 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/services/service.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312017 GailBot-0.1a9/src/config_backend/settings/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      272 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/settings/default.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312275 GailBot-0.1a9/src/config_backend/toplevel/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1040 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/toplevel/ws_config.toml
--rw-r--r--   0 muhammadumair   (501) staff       (20)       40 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/toplevel/ws_root.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312414 GailBot-0.1a9/src/config_backend/util/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      163 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/util/log.toml
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312683 GailBot-0.1a9/src/gailbot/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      383 2023-07-04 19:31:15.000000 GailBot-0.1a9/src/gailbot/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    19613 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/api.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312835 GailBot-0.1a9/src/gailbot/configs/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      459 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313086 GailBot-0.1a9/src/gailbot/configs/confs/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/confs/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1163 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/confs/paths.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313196 GailBot-0.1a9/src/gailbot/configs/interfaces/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1767 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313335 GailBot-0.1a9/src/gailbot/configs/interfaces/config/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4599 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/config/ws_config.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.306691 GailBot-0.1a9/src/gailbot/configs/interfaces/core/
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313766 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      683 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/google.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      741 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/watson.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2111 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/whisper.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313881 GailBot-0.1a9/src/gailbot/configs/interfaces/core/setting/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      900 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/setting/defaults.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314014 GailBot-0.1a9/src/gailbot/configs/interfaces/core/util/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      384 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/util/logger.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314398 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       87 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      905 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/pluginsuite.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)       72 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/validstructure.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314682 GailBot-0.1a9/src/gailbot/configs/interfaces/services/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       62 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/services/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2096 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/services/service.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314799 GailBot-0.1a9/src/gailbot/core/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.315218 GailBot-0.1a9/src/gailbot/core/engines/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      323 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1560 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/engine.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1014 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/engineManager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2361 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/exception.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.315585 GailBot-0.1a9/src/gailbot/core/engines/google/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       26 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/google/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    12222 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/google/core.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2453 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/google/google.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.316538 GailBot-0.1a9/src/gailbot/core/engines/watson/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      260 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11778 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/am.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      367 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/codes.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    12608 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/core.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    17153 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/lm.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13326 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/recognition_results.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5190 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/recognize_callback.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4913 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/watson.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.317057 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      203 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5567 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/core.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.317443 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      199 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3363 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/diarize.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3460 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/utils.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2824 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/parsers.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2290 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperEngine.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.318402 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      641 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10466 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/alignment.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8927 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/transcribe.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    24565 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/transcribe_efficient.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8623 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/transcribe_naive.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8383 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/utils.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      412 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/vars.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.318775 GailBot-0.1a9/src/gailbot/core/pipeline/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      259 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/pipeline/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1046 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/pipeline/component.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11217 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/pipeline/pipeline.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.319515 GailBot-0.1a9/src/gailbot/core/utils/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      163 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2630 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/download.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    14146 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/general.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1400 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/logger.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    27794 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/media.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    14967 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/threads.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.320018 GailBot-0.1a9/src/gailbot/plugins/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      264 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.320503 GailBot-0.1a9/src/gailbot/plugins/loader/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      146 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8722 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/directoryloader.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      668 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/pluginLoader.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10540 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/urlloader.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10349 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/manager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1404 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/plugin.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     7991 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/suite.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.320754 GailBot-0.1a9/src/gailbot/services/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      110 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    21854 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/controller.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.321026 GailBot-0.1a9/src/gailbot/services/converter/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      179 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2651 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/converter.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.321864 GailBot-0.1a9/src/gailbot/services/converter/payload/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      290 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2946 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/audioPayload.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3588 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/conversationDirectoryPayload.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13278 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/payloadObject.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3740 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/transcribedDirPayload.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2105 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/videoPayload.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.322091 GailBot-0.1a9/src/gailbot/services/converter/plugin/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/plugin/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5659 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/plugin/pluginMethod.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.322856 GailBot-0.1a9/src/gailbot/services/converter/result/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      241 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1266 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/analysis.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1534 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/format.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      323 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/processingStatus.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1827 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/resultInterface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5585 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/transcribe.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.323090 GailBot-0.1a9/src/gailbot/services/organizer/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      211 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    18069 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/organizer.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.323355 GailBot-0.1a9/src/gailbot/services/organizer/settings/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      104 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.324108 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      268 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      534 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2685 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/googleInterface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      326 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/pluginSettingsInterface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2527 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/watsonInterface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2067 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/whisperInterface.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.324622 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      136 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3919 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/engineObject.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      185 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/pluginObject.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3441 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/settingObject.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    20186 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/settingManager.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.324998 GailBot-0.1a9/src/gailbot/services/organizer/source/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       81 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/source/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8305 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/source/source_manager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3203 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/source/source_object.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.325258 GailBot-0.1a9/src/gailbot/services/pipeline/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       37 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.325912 GailBot-0.1a9/src/gailbot/services/pipeline/components/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      146 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6085 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/analysisComponent.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2102 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/formatComponent.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      359 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/progress.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10197 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/transcribeComponent.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2079 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/pipeline.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.326150 GailBot-0.1a9/src/gailbot/workspace/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       37 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/workspace/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5610 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/workspace/manager.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.326393 GailBot-0.1a9/tests/
--rw-r--r--   0 muhammadumair   (501) staff       (20)    16540 2023-07-04 18:14:11.000000 GailBot-0.1a9/tests/test_api.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3335 2023-07-04 18:14:11.000000 GailBot-0.1a9/tests/test_small.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.864391 GailBot-0.2a0/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1066 2023-08-07 03:38:06.000000 GailBot-0.2a0/LICENSE
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       49 2023-08-07 03:38:06.000000 GailBot-0.2a0/MANIFEST.in
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10630 2023-08-07 17:10:49.863930 GailBot-0.2a0/PKG-INFO
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     8546 2023-08-07 03:48:15.000000 GailBot-0.2a0/README.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1412 2023-08-07 17:07:14.000000 GailBot-0.2a0/pyproject.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5014 2023-08-07 03:38:06.000000 GailBot-0.2a0/requirements.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       38 2023-08-07 17:10:49.864447 GailBot-0.2a0/setup.cfg
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      251 2023-08-07 03:38:06.000000 GailBot-0.2a0/setup.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.813331 GailBot-0.2a0/src/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.820170 GailBot-0.2a0/src/.idea/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      176 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/.gitignore
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.820621 GailBot-0.2a0/src/.idea/inspectionProfiles/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      574 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      174 2023-08-07 02:22:24.000000 GailBot-0.2a0/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      181 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/misc.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      258 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/modules.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      226 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/src.iml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      183 2023-08-07 02:22:24.000000 GailBot-0.2a0/src/.idea/vcs.xml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821393 GailBot-0.2a0/src/GailBot.egg-info/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10630 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/PKG-INFO
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     9006 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        1 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5075 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/requires.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       23 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/top_level.txt
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821672 GailBot-0.2a0/src/config_backend/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      230 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.812947 GailBot-0.2a0/src/config_backend/engines/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821830 GailBot-0.2a0/src/config_backend/engines/google/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      549 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/engines/google/google_config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821999 GailBot-0.2a0/src/config_backend/engines/watson/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2196 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/engines/watson/watson_config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.822169 GailBot-0.2a0/src/config_backend/engines/whisper/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      929 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/engines/whisper/whisper_config.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      546 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/paths.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.822409 GailBot-0.2a0/src/config_backend/plugin/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      142 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/plugin/valid_plugin.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.823342 GailBot-0.2a0/src/config_backend/services/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      407 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/services/default_setting.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1119 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/services/format.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      448 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/services/service.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.823670 GailBot-0.2a0/src/config_backend/settings/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      272 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/settings/default.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824086 GailBot-0.2a0/src/config_backend/toplevel/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1040 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/toplevel/ws_config.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       40 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/toplevel/ws_root.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824265 GailBot-0.2a0/src/config_backend/util/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      163 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/util/log.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824643 GailBot-0.2a0/src/gailbot/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      380 2023-08-07 17:09:46.000000 GailBot-0.2a0/src/gailbot/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    22765 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/api.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824930 GailBot-0.2a0/src/gailbot/configs/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      459 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.825420 GailBot-0.2a0/src/gailbot/configs/confs/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      162 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/confs/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1163 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/confs/paths.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.825661 GailBot-0.2a0/src/gailbot/configs/interfaces/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1767 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.825828 GailBot-0.2a0/src/gailbot/configs/interfaces/config/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4839 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/config/ws_config.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.813833 GailBot-0.2a0/src/gailbot/configs/interfaces/core/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.826329 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      834 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/google.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      889 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/watson.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2111 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/whisper.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.826488 GailBot-0.2a0/src/gailbot/configs/interfaces/core/setting/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1030 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/setting/defaults.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.826657 GailBot-0.2a0/src/gailbot/configs/interfaces/core/util/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      540 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/util/logger.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.827175 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      244 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1061 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/pluginsuite.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      229 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/validstructure.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.827657 GailBot-0.2a0/src/gailbot/configs/interfaces/services/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      220 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/services/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1921 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/services/service.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.827806 GailBot-0.2a0/src/gailbot/core/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.828565 GailBot-0.2a0/src/gailbot/core/engines/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      363 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1560 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/engine.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      976 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/engineManager.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2361 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/exception.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.829041 GailBot-0.2a0/src/gailbot/core/engines/google/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      184 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/google/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    12266 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/google/core.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2578 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/google/google.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.830613 GailBot-0.2a0/src/gailbot/core/engines/watson/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      260 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    11756 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/am.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      367 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/codes.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    12605 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/core.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    16999 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/lm.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    13203 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/recognition_results.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5085 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/recognize_callback.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4907 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/watson.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.831198 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      203 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5643 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/core.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.831460 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      199 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3460 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/utils.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2846 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/parsers.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2100 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/whisperEngine.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.831753 GailBot-0.2a0/src/gailbot/core/engines/whisperX/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperX/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2960 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperX/whisperX.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.832192 GailBot-0.2a0/src/gailbot/core/pipeline/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      259 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/pipeline/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1046 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/pipeline/component.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10631 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/pipeline/pipeline.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.833427 GailBot-0.2a0/src/gailbot/core/utils/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      163 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2630 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/download.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    14143 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/general.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1535 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/logger.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    27791 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/media.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    14816 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/threads.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.834036 GailBot-0.2a0/src/gailbot/plugins/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      264 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.834658 GailBot-0.2a0/src/gailbot/plugins/loader/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      303 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     9172 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/directoryloader.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      824 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/pluginLoader.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10696 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/urlloader.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10435 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/manager.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1364 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/plugin.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     7744 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/suite.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.834959 GailBot-0.2a0/src/gailbot/services/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      267 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    23896 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/controller.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.835480 GailBot-0.2a0/src/gailbot/services/converter/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      334 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2740 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/converter.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.836464 GailBot-0.2a0/src/gailbot/services/converter/payload/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      458 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3184 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/audioPayload.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3745 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/conversationDirectoryPayload.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    13064 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/payloadObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3926 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/transcribedDirPayload.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2224 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/videoPayload.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.836756 GailBot-0.2a0/src/gailbot/services/converter/plugin/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/plugin/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5744 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/plugin/pluginMethod.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.837699 GailBot-0.2a0/src/gailbot/services/converter/result/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      398 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1406 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/analysis.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1673 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/format.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      479 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/processingStatus.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1936 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/resultInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5590 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/transcribe.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.838022 GailBot-0.2a0/src/gailbot/services/organizer/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      368 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    18452 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/organizer.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.838468 GailBot-0.2a0/src/gailbot/services/organizer/settings/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      261 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.839770 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      425 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      665 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2853 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/googleInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      480 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/pluginSettingsInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2681 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/watsonInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2172 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2105 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperXInterface.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.840352 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      293 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4067 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/engineObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      339 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/pluginObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3539 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/settingObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    19968 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/settingManager.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.840846 GailBot-0.2a0/src/gailbot/services/organizer/source/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      238 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/source/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     8415 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/source/source_manager.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3330 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/source/source_object.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.841161 GailBot-0.2a0/src/gailbot/services/pipeline/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      275 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.841983 GailBot-0.2a0/src/gailbot/services/pipeline/components/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      146 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6078 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/analysisComponent.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2150 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/formatComponent.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      506 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/progress.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10230 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/transcribeComponent.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1949 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/pipeline.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.842704 GailBot-0.2a0/src/gailbot/workspace/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      275 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/workspace/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5567 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/workspace/manager.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.844093 GailBot-0.2a0/tests/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1602 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/README
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5448 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/UPDATELOG
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      172 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.844730 GailBot-0.2a0/tests/configs/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/configs/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/configs/configs_test_configs.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1301 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/configs/test_config.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.844920 GailBot-0.2a0/tests/core/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.846176 GailBot-0.2a0/tests/core/engines/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2493 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/data.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5456 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_google_engine.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1562 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_watson_am.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6491 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_watson_core.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2787 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_watson_lm.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5372 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_whisper.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1168 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_whisperx.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.846554 GailBot-0.2a0/tests/core/pipeline/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/pipeline/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4398 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/pipeline/test_pipeline.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.847409 GailBot-0.2a0/tests/core/utils/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       72 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test.csv
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    14074 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test_general.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     8668 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test_media.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     9413 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test_thread.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.848447 GailBot-0.2a0/tests/plugins/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      484 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/plugin_data.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5731 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/plugin_data_old.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6026 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/test_plugin.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6072 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/test_plugins_old.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.849948 GailBot-0.2a0/tests/small-test/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2371 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/gailbot_key.json
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.852379 GailBot-0.2a0/tests/small-test/hello-dir/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello1.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello2.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello3.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello4.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello1.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello2.wav
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.852879 GailBot-0.2a0/tests/small-test/invalidFile/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/invalidFile/invalidfile1
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/invalidFile/invalidfile2
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.853368 GailBot-0.2a0/tests/small-test/transcribed-input/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        6 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/.gailbot
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.817287 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.856479 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      102 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.S.ca
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      102 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.cha
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       63 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.csv
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      601 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.gailbot.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      324 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.talkbank.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       28 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2803 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/format.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135212 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/merged.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       60 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/words.csv
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.817491 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.857290 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/hello1.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135212 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/merged.wav
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.857891 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Transcript/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       43 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Transcript/hello1.csv
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1119 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/format.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      899 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/meta.json
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    17736 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_api.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.859774 GailBot-0.2a0/tests/test_data/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      328 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      785 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/data.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5863 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/path.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2058 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/payload_obj.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      471 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/result_data.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.859973 GailBot-0.2a0/tests/test_data/sample_suite/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      371 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/sample_suite/config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.817809 GailBot-0.2a0/tests/test_data/sample_suite/src/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.860163 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1341 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir/sample_module1.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.860352 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir2/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      854 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir2/sample_module2.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2966 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/setting_data.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.860752 GailBot-0.2a0/tests/test_data/test_suite/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      893 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.861097 GailBot-0.2a0/tests/test_data/test_suite/src/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.862862 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      570 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_fail1.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      507 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_fail2.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      980 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_succ1.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      493 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_succ2.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.863664 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      680 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/test_succ3.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      680 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/test_succ4.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      281 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/workspace.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3335 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_small.py
```

### Comparing `GailBot-0.1a9/LICENSE` & `GailBot-0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/README.md` & `GailBot-0.2a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,258 +1,194 @@
-# GailBot
-
-**NOTE**: This documentation is a work in progress and will be updated.
+Metadata-Version: 2.1
+Name: GailBot
+Version: 0.2a0
+Summary: GailBot API
+Author-email: Muhammad Umair <muhammad.umair@tufts.edu>
+Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
+License: MIT License
+        
+        Copyright (c) 2023 jasonycwu
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://sites.tufts.edu/hilab/gailbot-an-automatic-transcription-system-for-conversation-analysis/
+Project-URL: source, https://github.com/mumair01/GailBot
+Project-URL: tracker, https://github.com/mumair01/GailBot/issues
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
+# GailBot
 
 ## About
 
 Researchers studying human interaction, such as conversation analysts, psychologists, and linguists all rely on detailed transcriptions of language use. Ideally, these should include so-called paralinguistic features of talk, such as overlaps, prosody, and intonation, as they convey important information. However, transcribing these features by hand requires substantial amounts of time by trained transcribers. There are currently no Speech to Text (STT) systems that are able to annotate these features. To reduce the resources needed to create transcripts that include paralinguistic features, we developed a program called GailBot. GailBot combines STT services with plugins to automatically generate first drafts of conversation analytic transcripts. It also enables researchers to add new plugins to transcribe additional features, or to improve the plugins it currently uses. We argue that despite its limitations, GailBot represents a substantial improvement over existing dialogue transcription software.
 
 Find the full paper published by Dialogue and Discourse [here](https://journals.uic.edu/ojs/index.php/dad/article/view/11392).
 
-## Status
-
-GailBot version: 0.0.1x (Pre-release)
 
-Supported OS: MacOs 11.6, Ubuntu 20.04
+## Status
 
+GailBot version: 0.1a11 (Pre-release)
 Release type: API
 
-## Installation
-
-GailBot can be installed using pip or from the Github repository.
 
-### Pip installation
-
-To install program dependencies, execute the following:
-
-```
-pip install \
-    pyaudio \
-    ffmpeg
-```
-
-To install via pip, run the following commands:
+## Installation
 
+GailBot and the necessary dependencies can be installed using pip with the following commands:
 ```
 pip install --upgrade pip
 
-python3 -m pip install GailBot
+pip install gailbot
+pip install git+https://github.com/linto-ai/whisper-timestamped
+pip install git+https://github.com/m-bain/whisperx.git
 ```
 
-## Usage
-
-This GailBot release features a convenient API to use GailBot and create custom plugin suites.
-
-GailBot usage will consist of two main components: a driver code and optional plugin suites that may need to be applied.
 
-### GailBot API
+## Usage - GailBot API
 
-To support the driver code, GailBot provides two main classes that may be imported as follows in a python script:
+This release features a convenient API to use GailBot and create custom plugin suites. To use the API and its features, import the GailBot package like the following:
 
 ```
-from gailbot.core import GailBotController, GailBotSettings
+from gailbot import GailBot
 ```
 
-The GailBotController class provides the main API for transcribing sources, applying settings to different sources, and starting the transcription process. On the other hand, GailBotSettings are applied to each source and specify how that source is handled by the controller.
-
-The following code specifies how a GailBotController class is initialized and a GailBotSettings object is used to create a unique settings profile that then be applied to sources.
-
+Once you have imported the GailBot package, initialize an instance of GailBot called "gb" (or a name of your choosing) by doing the following ("ws_root" is takes a path to your workspace directory):
 
 ```
-from gailbot.core import GailBotController, GailBotSettings
-
-settings_dictionary = {
-        "core": {},
-        "plugins": {
-            "plugins_to_apply": ["demoPlugin"]
-        },
-        "engines": {
-            "engine_type": "watson",
-            "watson_engine": {
-                "watson_api_key": WATSON_API_KEY,
-                "watson_language_customization_id": WATSON_LANG_CUSTOM_ID,
-                "watson_base_language_model": WATSON_BASE_LANG_MODEL,
-                "watson_region": WATSON_REGION,
-
-            }
-        }
-    }
-
-controller = GailBotController(WORKSPACE_DIRECTORY_PATH)
-controller.create_new_settings_profile(
-        "demo_profile", settings_dictionary)
+gb = GailBot(ws_root="your_workspace_path")
 ```
+The GailBot API's methods are now available through your GailBot instance. Check out GailBot's backend documentation for a full list of method and their uses [here](https://gailbot-release-document.s3.us-east-2.amazonaws.com/Documentation/Backend_Technical_Documentation.pdf).
 
-In the above example, we first create a dictionary with key-value pairs that are required to create a GailBotSettings object. Note that "plugins_to_apply" is a list of plugin names that will be applied for that specific settings profile. Since GailBot currently supports IBM Watson STT, users must first create an [IBM Bluemix account](https://cloud.ibm.com/registration?target=catalog%3fcategory=watson&cm_mmc=Earned-_-Watson+Core+-+Platform-_-WW_WW-_-intercom&cm_mmca1=000000OF&cm_mmca2=10000409&). Next, a watson api key and region must be created with [IBM](https://cloud.ibm.com/catalog/services/speech-to-text) and specified in the settings profile.
-
-With the settings dictionary specified, we create an instance of GailBotController, specifying a path to a directory that GailBot will use as a private workspace. Finally, we create a new settings profile called "demo_profile" with the values defined in the settings dictionary.
-
-
-With the controller defined and at least one settings profile created, we are ready to transcribe a source as follows:
 
+### Example Usage 1 - Default Settings
+Now, we will try to use the GailBot on an input audio file.
+To do so, we will need initiate a GailBot instance, add input audio file as source, and transcribe. 
+This example uses GailBot's default settings with default engine (Whisper) and pre-installed plugin suite. Therefore, there is no need to create and apply profile settings.
+See the example below:
 ```
+from gailbot import GailBot
 
-controller.add_source("demo_audio_source", <PATH TO AUDIO FILE>, <PATH TO RESULT DIRECTORY>)
-controller. apply_settings_profile_to_source(
-    "demo_audio_source","demo_profile")
-assert controller.is_source_ready_to_transcribe("demo_audio_source)
-controller.transcribe()
-```
-
-
-In the above code example, we first add an audio source to an instance of GailBotController, giving it a unique identifier, the path to the audio source, and a result directory. Next, we apply the settings profile created earlier to the audio source we added. We then verify that the settings profile has been correctly applied and that the audio source is ready to transcribe. Finally, we start the transcription process and wait for results in the  specified results directory.
-
-### Supported Plugin Suites
-
-A core GailBot feature is its ability to apply plugin suites during the transcription process. While different use cases may require custom plugins (See section below), the Human Interaction Lab maintains and distributes pre-developed custom suites.
-
-The GailBot API provides a method for downloading HI-Lab plugin suites as follows:
-
-```
-gb = init_gb(<TRANSCRIPTION_WORKSPACE>)
-plugin_suite_paths = gb.download_plugin_suite_from_url(
-    <PLUGIN_SUITE_URL>, <LOCAL DIRECTORY PATH>)
-```
-
-The above code downloads a plugin suite from the specified URL and saves the plugin suite in a local directory.
-
-Below is a detailed list of HI-Lab maintained plugin suites:
-
-#### HiLabSuite
-
-This is the main plugin suite that is maintained by the Human Interaction Lab. It uses a multi-layered approach to generate a tree-like structure to store transcription results, supports multiple data views (word level, utterance level etc.), and produces output in various formats.
-
-**SUITE URL:**  https://sites.tufts.edu/hilab/files/2022/05/HiLabSuite.zip
-
-The following code demonstrates how this plugin suite may be used with GailBot:
+gb = GailBot(ws_root="your_workspace_path")
 
+gb.add_source(
+    source_path="your_source_file_path"
+    output_dir="your_output_directory_path"
+)
+gb.transcribe()
 ```
 
-PLUGINS_TO_APPLY = [
-    "constructTree",
-    "utteranceDict",
-    "speakerDict",
-    "conversationDict",
-    "convModelPlugin",
-    "overlaps",
-    "pauses",
-    "gaps",
-    "syllRate",
-    "layerPrint01",
-    "plainPrint",
-    "chat",
-    "txt",
-    "csvPlugin",
-    "csvWordLevel",
-    "XMLtoCSV",
-    "xmlSchema"
-]
-
-def get_settings_dict() -> Dict:
-    return {
-        "core": {},
-        "plugins": {
-            "plugins_to_apply": PLUGINS_TO_APPLY
-        },
-        "engines": {
-            "engine_type": "watson",
-            "watson_engine": {
-                "watson_api_key": WATSON_API_KEY,
-                 "watson_language_customization_id": "",
-                "watson_base_language_model": WATSON_BASE_LANG_MODEL,
-                "watson_region": WATSON_REGION,
-
-            }
-        }
-    }
-
-
-
-# Initialize GailBot
-gb = init_gb(TRANSCRIPTION_WORKSPACE)
-
-# Download plugin suite into local directory'./plugins'
-plugin_suite_paths = gb.download_plugin_suite_from_url(
-    "https://sites.tufts.edu/hilab/files/2022/05/HiLabSuite.zip", "./plugins")
-
-# Generate full path to the local directory on the current system
-path = os.path.join(os.getcwd(),plugin_suite_paths[0])
-
-# Register the plugins - print to verify expected plugins are loaded.
-print(gb.register_plugins(path))
-
-# Add a source with <SOURCE NAME> from the <SOURCE PATH>, which produces
-# results in <RESULT DIRECTORY PATH>
-assert gb.add_source(<SOURCE NAME>,
-                        <SOURCE PATH>, <RESULT DIRECTORY PATH>)
-
-# Create a settings profile for this plugin suite
-gb.create_new_settings_profile(<SETTINGS_PROFILE_NAME>, get_settings_dict())
-assert gb.is_settings_profile(<SETTINGS_PROFILE_NAME>)
-
-# Apply a settings profile with name <SETTINGS_PROFILE_NAME> to the source with
-# name <SOURCE NAME>
-assert gb.apply_settings_profile_to_source(
-    <SOURCE NAME>, <SETTINGS_PROFILE_NAME>)
+### Example Usage 2 - Custom Profile
+Here is an example of using GailBot with your customized transcription profile.
+To do so, you'll need to create a profile and apply it to input source files before transcribing with GailBot.
+See example on how to create a profile:
+```
+from gailbot import GailBot
+
+gb = GailBot(ws_root="your_workspace_path")
+
+gb.add_new_engine(
+    "new_google_engine", 
+    {"engine": "google", "google_api_key": GOOGLE_API_KEY}, 
+    overwrite=True,
+)
+
+TEST_PROFILE = {
+    "engine_setting_name": "new_google_engine",
+    "plugin_setting": ["gb_hilab_suite"],
+}
 
-# Start the transcription process.
-assert gb.is_source_ready_to_transcribe(<SOURCE NAME>)
+gb.add_source(source_path="path_to_your_source", output_dir="your_output_directory_path")
+gb.apply_setting_to_source("path_to_your_source", TEST_PROFILE)
 gb.transcribe()
 ```
+In the example above, we added Google Cloud STT engine called "new_google_engine" using your Google engine API key.
+Then, we used the Google engine to create a new profile called TEST_PROFILE. Here we also use GailBot's default plugin suite called gb_hilab_suite.
+Finally, we apply our custom profile to our input source and transcribe.
 
-In the above code, we initialize GailBot, create a new settings profile that applies plugins for the HILabPlugin suite, add a source to transcribe, and produce results by applying the plugin suite.
-
-Note that in the get_settings_dict() method, users will have to enter their custom WATSON_API_KEY, WATSON_REGION, and WATSON_BASE_LANG_MODEL. These are generated from the [IBM Watson](https://cloud.ibm.com/login) service.
 
+## Supported Plugin Suites
 
+A core GailBot feature is its ability to apply plugin suites during the transcription process. While different use cases may require custom plugins, the Human Interaction Lab maintains and distributes a pre-developed plugin suite -- HiLabSuite. For more information about the default plugin suite, click [here](https://sites.tufts.edu/hilab/gailbot-an-automatic-transcription-system-for-conversation-analysis/).
 
 ### Custom Plugins
 
+A core GailBot feature is its ability to allow researchers to develop and add custom plugins that may be applied during the transcription process, in addition to the provided built-in HiLabSuite. To create a compatible plugin suite for the Gailbot app, follow these steps:
 
-**NOTE**: This documentation is in progress and a more detailed version will be available soon!
+1. Prepare the Folder Structure and Files:
+Ensure your plugin suite directory contains the following files with specific names: "init.py," "CHANGELOG.md," "DOCUMENT.md," "TECH_DOCUMENT.md," "README.md," "format.md," and "config.toml." Include a subfolder named "src" within the main directory.
 
-A core GailBot feature is its ability to allow researchers to develop and add custom plugins that may be applied during the transcription process.
+    File Descriptions:
 
-The following is an example of how a minimal plugin may be developed.
+    init.py: Used for package initialization and can be left empty.
+    format.md: Provides users information about generated output files.
+    CHANGELOG.md: Documents version-to-version changes.
+    README.md: Offers a high-level explanation and purpose of the plugin suite.
+    DOCUMENT.md: Contains specifics about algorithms, plugins, and developers.
+    TECH_DOCUMENT.md: Explains technical aspects like logging implementation.
+    config.toml: Vital file that outlines plugin execution order and settings.
+
+2. Configure config.toml:
+Begin with setting suite_name = "<mySuite>", matching the directory name. Define metadata in the [metadata] section, including Author, Email, and Version.
+
+3. Define Plugins:
+For each plugin, create a section in config.toml under plugins section. Specify plugin_name, dependencies, rel_path, and module_name.
+
+    plugin_name: The name of your plugin.
+    dependencies: A list of plugins needed before this one.
+    rel_path: Path to the file with the plugin's apply function.
+    module_name: The name of the file without the .py suffix.
+
+4. Plugin Coding:
+Define each plugin as a class with the exact name from plugin_name.
+Inside the class, include an apply function with the signature def apply(self, dependency_outputs: Dict[str, Any], methods: <your methods>).
+At the end of the apply function, set self.is_successful = True.
+
+5. Dependencies and Output Flow:
+Use the dependency_outputs dictionary to pass outputs between plugins.
+When a plugin depends on another, it receives previous plugin outputs through this dictionary, with plugin class name as the key.
+Ensure plugin classes are properly formatted in config.toml for the apply function to run.
 
-```
-from typing import Dict, Any, List
-# Local imports
-from gailbot.plugins import GBPlugin, PluginMethodSuite, Utt
-
-
-class CombineTurns(GBPlugin):
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def apply(self, dependency_outputs: Dict[str, Any],
-                     methods: PluginMethodSuite) -> List[Utt]:
-        # Combine all the utterances in the utterance map into a single
-        # conversation.
-        combined = list()
-        turns_map: Dict[str, List[Utt]
-                        ] = dependency_outputs["turn_construct"]
-        for turns in turns_map.values():
-            combined.extend(turns)
-        combined.sort(key=lambda utt: utt.start_time_seconds)
-        self.successful = True
-        return combined
-```
+With correctly structured files, codes, and dependencies, your plugins will run as intended when uploaded to Gailbot. 
+Congratulations on creating your plugin suite for Gailbot, and thank you for following our tutorial! Happy transcribing!
 
 
 ## Contribute
 
 Users are encouraged to direct installation and usage questions, provide feedback, details regarding bugs, and development ideas by [email](mailto:hilab-dev@elist.tufts.edu).
 
+
 ## Acknowledgements
 
 Special thanks to members of the [Human Interaction Lab](https://sites.tufts.edu/hilab/) at Tufts University and interns that have worked on this project.
 
+
 ## Cite
 
 Users are encouraged to cite GailBot using the following BibTex:
 ```
 @article{umair2022gailbot,
   title={GailBot: An automatic transcription system for Conversation Analysis},
   author={Umair, Muhammad and Mertens, Julia Beret and Albert, Saul and de Ruiter, Jan P},
@@ -269,12 +205,13 @@
 Gailbot is a tool to be used to generate specialized transcripts. However, it
 is not responsible for output quality. Generated transcripts are meant to
 be first drafts that can be manually improved. They are not meant to replace
 manual transcription.
 
 GailBot may use external Speech-to-Text systems or third-party services. The
 development team is not responsible for any transactions between users and these
-services. Additionally, the development team does not guarantee the accuracy or correctness of any plugin. Plugins have been developed in good faith and we hope
+services. Additionally, the development team does not guarantee the accuracy or 
+correctness of any plugin. Plugins have been developed in good faith and we hope 
 that they are accurate. However, users should always verify results.
 
 By using GailBot, users agree to cite Gailbot and the Tufts Human Interaction Lab
 in any publications or results as a direct or indirect result of using Gailbot.
```

### Comparing `GailBot-0.1a9/pyproject.toml` & `GailBot-0.2a0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 version = {attr = "gailbot.__version__"}
 
 [tool.setuptools.packages.find]
 where =["src"]
 
 
 [project.urls]
-homepage = "https://github.com/mumair01/GailBot"
+homepage = "https://sites.tufts.edu/hilab/gailbot-an-automatic-transcription-system-for-conversation-analysis/"
 source = "https://github.com/mumair01/GailBot"
 tracker = "https://github.com/mumair01/GailBot/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `GailBot-0.1a9/requirements.txt` & `GailBot-0.2a0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 absl-py==1.4.0
 aiohttp==3.8.4
 aiosignal==1.3.1
 alembic==1.10.2
 altgraph==0.17.3
 antlr4-python3-runtime==4.9.3
+anyio==3.7.1
 appdirs==1.4.4
+arrow==1.2.3
 asteroid-filterbanks==0.4.0
 astunparse==1.6.3
 async-timeout==4.0.2
 attrs==22.2.0
 audioread==3.0.0
 auto-py-to-exe==2.33.0
+av==10.0.0
+backoff==2.2.1
 backports.cached-property==1.0.2
+beautifulsoup4==4.12.2
 black==23.1.0
 bleach==6.0.0
+blessed==1.20.0
 boto3==1.26.105
 botocore==1.29.105
 bottle==0.12.25
 bottle-websocket==0.2.9
 build==0.10.0
 cachetools==5.3.0
-pyannote.audio==2.1.1
 certifi==2022.12.7
 cffi==1.15.1
 cfgv==3.3.1
 charset-normalizer==3.1.0
 click==8.1.3
 cmaes==0.9.1
 cmudict==1.0.13
 colorama==0.4.6
+coloredlogs==15.0.1
 colorlog==6.7.0
 commonmark==0.9.1
 contourpy==1.0.7
 cPython==0.0.6
+croniter==1.4.1
 cryptography==40.0.2
+ctranslate2==3.18.0
 cycler==0.11.0
+Cython==3.0.0
 dacite==1.8.0
+dateutils==0.6.12
 decorator==4.4.2
+deepdiff==6.3.1
 dict-to-dataclass==0.0.8
 distlib==0.3.6
 dnspython==2.3.0
 docopt==0.6.2
 docutils==0.19
 dotted-dict==1.1.3
 dotwiz==0.4.0
 dtw-python==1.3.0
 Eel==0.16.0
-einops==0.3.2
+einops==0.6.1
 entrypoints==0.4
 exceptiongroup==1.1.1
 exif==1.6.0
+fastapi==0.101.0
+faster-whisper==0.7.1
 ffmpeg-python==0.2.0
 filelock==3.10.0
 flake8==6.0.0
 flatbuffers==23.3.3
 fonttools==4.39.2
 frozenlist==1.3.3
 fsspec==2023.3.0
@@ -67,79 +80,93 @@
 google-cloud-core==2.3.2
 google-cloud-speech==2.18.0
 google-pasta==0.2.0
 googleapis-common-protos==1.59.0
 greenlet==2.0.2
 grpcio==1.51.3
 grpcio-status==1.51.3
+h11==0.14.0
 h5py==3.8.0
 huggingface-hub==0.13.3
+humanfriendly==10.0
 HyperPyYAML==1.1.0
 ibm-cloud-sdk-core==3.16.2
 ibm-watson==7.0.0
 identify==2.5.21
 idna==3.4
 imageio==2.26.1
 imageio-ffmpeg==0.4.8
 importlib-metadata==5.2.0
 importlib-resources==5.12.0
 iniconfig==2.0.0
+inquirer==3.1.3
+itsdangerous==2.1.2
 jaraco.classes==3.2.3
 jedi==0.18.1
+Jinja2==3.1.2
 jmespath==1.0.1
 joblib==1.2.0
 julius==0.2.7
 keras==2.12.0
 keyring==23.13.1
 kiwisolver==1.4.4
 libclang==15.0.6.1
 librosa==0.9.2
+lightning==2.0.6
+lightning-cloud==0.5.37
+lightning-fabric==2.0.6
+lightning-utilities==0.9.0
 llvmlite==0.39.1
 lxml==4.9.2
 macholib==1.16.2
 Mako==1.2.4
 Markdown==3.4.1
 MarkupSafe==2.1.2
 matplotlib==3.7.1
 mccabe==0.7.0
 more-itertools==9.1.0
 moviepy==1.0.3
 mpmath==1.3.0
 multidict==6.0.4
 mypy-extensions==1.0.0
 networkx==2.8.8
+nltk==3.8.1
 nodeenv==1.7.0
 Nuitka==1.5.3
 numba==0.56.4
 numpy==1.23.5
 oauthlib==3.2.2
 omegaconf==2.3.0
+onnxruntime==1.15.1
 openai-whisper==20230314
 opt-einsum==3.3.0
 optuna==3.1.0
 ordered-set==4.1.0
 packaging==23.0
 pandas==1.5.3
 parso==0.8.3
 pathspec==0.11.1
 pep517==0.13.0
 Pillow==9.4.0
-pip==23.1.2
 pkginfo==1.9.6
 platformdirs==3.1.1
 pluggy==1.0.0
 plum-py==0.8.5
 pooch==1.7.0
 pre-commit==3.2.0
 primePy==1.3
 proglog==0.1.10
 proto-plus==1.22.2
 protobuf==4.22.1
 psutil==5.9.4
 py==1.11.0
+pyannote.core==5.0.0
+pyannote.database==5.0.1
+pyannote.metrics==3.2.1
+pyannote.pipeline==2.3
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 pycodestyle==2.10.0
 pycparser==2.21
 pydantic==1.10.6
 pyDeprecate==0.3.2
 pydub==0.25.1
@@ -157,19 +184,22 @@
 PyQt6==6.4.2
 PyQt6-Qt6==6.4.3
 PyQt6-sip==13.4.1
 pyqtconsole==1.2.2
 pytest==7.2.2
 python-configuration==0.8.2
 python-dateutil==2.8.1
+python-editor==1.0.4
+python-multipart==0.0.6
 pytorch-lightning==1.6.3
-pytorch-metric-learning==1.7.3
+pytorch-metric-learning==2.3.0
 pytz==2022.7.1
 PyYAML==6.0
 QtPy==2.2.0
+readchar==4.0.5
 readme-renderer==37.3
 regex==2022.10.31
 requests==2.28.2
 requests-oauthlib==1.3.1
 requests-toolbelt==0.10.1
 resampy==0.4.2
 rfc3986==2.0.0
@@ -179,64 +209,70 @@
 ruamel.yaml.clib==0.2.7
 s3transfer==0.6.0
 sacremoses==0.0.53
 scikit-learn==1.2.2
 scipy==1.10.1
 selenium==3.10.0
 semantic-version==2.10.0
-semver==2.13.0
+semver==3.0.1
 sentencepiece==0.1.97
-setuptools==65.5.0
 setuptools-rust==1.5.2
 shellingham==1.5.0.post1
 simplejson==3.18.4
 singledispatchmethod==1.0
 six==1.16.0
+sniffio==1.3.0
 sortedcontainers==2.4.0
 sounddevice==0.4.6
-SoundFile
-speechbrain==0.5.13
+soundfile==0.12.1
+soupsieve==2.4.1
+speechbrain==0.5.15
 SQLAlchemy==2.0.7
+starlette==0.27.0
+starsessions==1.3.0
 syllable==0.1.0
 syllables==1.0.7
 sympy==1.11.1
 tabulate==0.9.0
 tensorboard==2.12.0
 tensorboard-data-server==0.7.0
 tensorboard-plugin-wit==1.8.1
+tensorboardX==2.6.2
 tensorflow-estimator==2.12.0
 termcolor==2.2.0
 threadpoolctl==3.1.0
 tiktoken==0.3.1
 tokenizers==0.13.2
 toml==0.10.2
 tomli==2.0.1
-torch==1.13.1
+torch==2.0.1
 torch-audiomentations==0.11.0
 torch-pitch-shift==1.2.2
-torchaudio==0.13.1
+torchaudio==2.0.2
 torchmetrics==0.11.4
 torchvision==0.14.1
 tqdm==4.65.0
+traitlets==5.9.0
 transformers==4.27.2
 twine==4.0.2
 typed-ast==1.5.4
 typer==0.7.0
 typing_extensions==4.5.0
 urllib3==1.26.15
 userpaths==0.1.3
+uvicorn==0.23.2
 validators==0.20.0
 virtualenv==20.21.0
 wcwidth==0.2.6
 webencodings==0.5.1
 websocket-client==1.1.0
+websockets==11.0.3
 Werkzeug==2.2.3
-wheel==0.37.1
 whichcraft==0.6.1
 wrapt==1.15.0
 xattr==0.10.1
 yamllint==1.29.0
 yarl==1.8.2
 zipp==3.15.0
 zope.event==4.6
 zope.interface==6.0
-zstandard==0.20.0
+zstandard==0.20.0
```

### Comparing `GailBot-0.1a9/src/GailBot.egg-info/requires.txt` & `GailBot-0.2a0/src/GailBot.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 absl-py==1.4.0
 aiohttp==3.8.4
 aiosignal==1.3.1
 alembic==1.10.2
 altgraph==0.17.3
 antlr4-python3-runtime==4.9.3
+anyio==3.7.1
 appdirs==1.4.4
+arrow==1.2.3
 asteroid-filterbanks==0.4.0
 astunparse==1.6.3
 async-timeout==4.0.2
 attrs==22.2.0
 audioread==3.0.0
 auto-py-to-exe==2.33.0
+av==10.0.0
+backoff==2.2.1
 backports.cached-property==1.0.2
+beautifulsoup4==4.12.2
 black==23.1.0
 bleach==6.0.0
+blessed==1.20.0
 boto3==1.26.105
 botocore==1.29.105
 bottle==0.12.25
 bottle-websocket==0.2.9
 build==0.10.0
 cachetools==5.3.0
-pyannote.audio==2.1.1
 certifi==2022.12.7
 cffi==1.15.1
 cfgv==3.3.1
 charset-normalizer==3.1.0
 click==8.1.3
 cmaes==0.9.1
 cmudict==1.0.13
 colorama==0.4.6
+coloredlogs==15.0.1
 colorlog==6.7.0
 commonmark==0.9.1
 contourpy==1.0.7
 cPython==0.0.6
+croniter==1.4.1
 cryptography==40.0.2
+ctranslate2==3.18.0
 cycler==0.11.0
+Cython==3.0.0
 dacite==1.8.0
+dateutils==0.6.12
 decorator==4.4.2
+deepdiff==6.3.1
 dict-to-dataclass==0.0.8
 distlib==0.3.6
 dnspython==2.3.0
 docopt==0.6.2
 docutils==0.19
 dotted-dict==1.1.3
 dotwiz==0.4.0
 dtw-python==1.3.0
 Eel==0.16.0
-einops==0.3.2
+einops==0.6.1
 entrypoints==0.4
 exceptiongroup==1.1.1
 exif==1.6.0
+fastapi==0.101.0
+faster-whisper==0.7.1
 ffmpeg-python==0.2.0
 filelock==3.10.0
 flake8==6.0.0
 flatbuffers==23.3.3
 fonttools==4.39.2
 frozenlist==1.3.3
 fsspec==2023.3.0
@@ -67,79 +80,93 @@
 google-cloud-core==2.3.2
 google-cloud-speech==2.18.0
 google-pasta==0.2.0
 googleapis-common-protos==1.59.0
 greenlet==2.0.2
 grpcio==1.51.3
 grpcio-status==1.51.3
+h11==0.14.0
 h5py==3.8.0
 huggingface-hub==0.13.3
+humanfriendly==10.0
 HyperPyYAML==1.1.0
 ibm-cloud-sdk-core==3.16.2
 ibm-watson==7.0.0
 identify==2.5.21
 idna==3.4
 imageio==2.26.1
 imageio-ffmpeg==0.4.8
 importlib-metadata==5.2.0
 importlib-resources==5.12.0
 iniconfig==2.0.0
+inquirer==3.1.3
+itsdangerous==2.1.2
 jaraco.classes==3.2.3
 jedi==0.18.1
+Jinja2==3.1.2
 jmespath==1.0.1
 joblib==1.2.0
 julius==0.2.7
 keras==2.12.0
 keyring==23.13.1
 kiwisolver==1.4.4
 libclang==15.0.6.1
 librosa==0.9.2
+lightning==2.0.6
+lightning-cloud==0.5.37
+lightning-fabric==2.0.6
+lightning-utilities==0.9.0
 llvmlite==0.39.1
 lxml==4.9.2
 macholib==1.16.2
 Mako==1.2.4
 Markdown==3.4.1
 MarkupSafe==2.1.2
 matplotlib==3.7.1
 mccabe==0.7.0
 more-itertools==9.1.0
 moviepy==1.0.3
 mpmath==1.3.0
 multidict==6.0.4
 mypy-extensions==1.0.0
 networkx==2.8.8
+nltk==3.8.1
 nodeenv==1.7.0
 Nuitka==1.5.3
 numba==0.56.4
 numpy==1.23.5
 oauthlib==3.2.2
 omegaconf==2.3.0
+onnxruntime==1.15.1
 openai-whisper==20230314
 opt-einsum==3.3.0
 optuna==3.1.0
 ordered-set==4.1.0
 packaging==23.0
 pandas==1.5.3
 parso==0.8.3
 pathspec==0.11.1
 pep517==0.13.0
 Pillow==9.4.0
-pip==23.1.2
 pkginfo==1.9.6
 platformdirs==3.1.1
 pluggy==1.0.0
 plum-py==0.8.5
 pooch==1.7.0
 pre-commit==3.2.0
 primePy==1.3
 proglog==0.1.10
 proto-plus==1.22.2
 protobuf==4.22.1
 psutil==5.9.4
 py==1.11.0
+pyannote.core==5.0.0
+pyannote.database==5.0.1
+pyannote.metrics==3.2.1
+pyannote.pipeline==2.3
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 pycodestyle==2.10.0
 pycparser==2.21
 pydantic==1.10.6
 pyDeprecate==0.3.2
 pydub==0.25.1
@@ -157,19 +184,22 @@
 PyQt6==6.4.2
 PyQt6-Qt6==6.4.3
 PyQt6-sip==13.4.1
 pyqtconsole==1.2.2
 pytest==7.2.2
 python-configuration==0.8.2
 python-dateutil==2.8.1
+python-editor==1.0.4
+python-multipart==0.0.6
 pytorch-lightning==1.6.3
-pytorch-metric-learning==1.7.3
+pytorch-metric-learning==2.3.0
 pytz==2022.7.1
 PyYAML==6.0
 QtPy==2.2.0
+readchar==4.0.5
 readme-renderer==37.3
 regex==2022.10.31
 requests==2.28.2
 requests-oauthlib==1.3.1
 requests-toolbelt==0.10.1
 resampy==0.4.2
 rfc3986==2.0.0
@@ -179,62 +209,68 @@
 ruamel.yaml.clib==0.2.7
 s3transfer==0.6.0
 sacremoses==0.0.53
 scikit-learn==1.2.2
 scipy==1.10.1
 selenium==3.10.0
 semantic-version==2.10.0
-semver==2.13.0
+semver==3.0.1
 sentencepiece==0.1.97
-setuptools==65.5.0
 setuptools-rust==1.5.2
 shellingham==1.5.0.post1
 simplejson==3.18.4
 singledispatchmethod==1.0
 six==1.16.0
+sniffio==1.3.0
 sortedcontainers==2.4.0
 sounddevice==0.4.6
-SoundFile
-speechbrain==0.5.13
+soundfile==0.12.1
+soupsieve==2.4.1
+speechbrain==0.5.15
 SQLAlchemy==2.0.7
+starlette==0.27.0
+starsessions==1.3.0
 syllable==0.1.0
 syllables==1.0.7
 sympy==1.11.1
 tabulate==0.9.0
 tensorboard==2.12.0
 tensorboard-data-server==0.7.0
 tensorboard-plugin-wit==1.8.1
+tensorboardX==2.6.2
 tensorflow-estimator==2.12.0
 termcolor==2.2.0
 threadpoolctl==3.1.0
 tiktoken==0.3.1
 tokenizers==0.13.2
 toml==0.10.2
 tomli==2.0.1
-torch==1.13.1
+torch==2.0.1
 torch-audiomentations==0.11.0
 torch-pitch-shift==1.2.2
-torchaudio==0.13.1
+torchaudio==2.0.2
 torchmetrics==0.11.4
 torchvision==0.14.1
 tqdm==4.65.0
+traitlets==5.9.0
 transformers==4.27.2
 twine==4.0.2
 typed-ast==1.5.4
 typer==0.7.0
 typing_extensions==4.5.0
 urllib3==1.26.15
 userpaths==0.1.3
+uvicorn==0.23.2
 validators==0.20.0
 virtualenv==20.21.0
 wcwidth==0.2.6
 webencodings==0.5.1
 websocket-client==1.1.0
+websockets==11.0.3
 Werkzeug==2.2.3
-wheel==0.37.1
 whichcraft==0.6.1
 wrapt==1.15.0
 xattr==0.10.1
 yamllint==1.29.0
 yarl==1.8.2
 zipp==3.15.0
 zope.event==4.6
```

### Comparing `GailBot-0.1a9/src/config_backend/engines/google/google_config.toml` & `GailBot-0.2a0/src/config_backend/engines/google/google_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/config_backend/engines/watson/watson_config.toml` & `GailBot-0.2a0/src/config_backend/engines/watson/watson_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/config_backend/engines/whisper/whisper_config.toml` & `GailBot-0.2a0/src/config_backend/engines/whisper/whisper_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/config_backend/paths.toml` & `GailBot-0.2a0/src/config_backend/paths.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/config_backend/services/format.md` & `GailBot-0.2a0/src/config_backend/services/format.md`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/config_backend/toplevel/ws_config.toml` & `GailBot-0.2a0/src/config_backend/toplevel/ws_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/api.py` & `GailBot-0.2a0/src/gailbot/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
-# @Author: Muhammad Umair
-# @Date:   2023-01-10 14:06:17
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-06-15 15:40:20
-
+# @Author: Jason Y. Wu
+# @Date:   2023-08-04 13:59:52
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-06 20:52:08
 from typing import List, Dict, Union, Tuple, Callable
-import sys
-from .services import ServiceController, SettingDict
-from .workspace import WorkspaceManager
+
+from gailbot.services import ServiceController, SettingDict
+from gailbot.workspace import WorkspaceManager
 from .plugins.suite import PluginSuite
-from .core.utils.logger import makelogger
+from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("gb_api")
 
 
 class GailBot:
     """
     Class for API wrapper
     """
 
     def __init__(self, ws_root: str):
-        """initialize an gailbot object that provides a suite of functions
+        """initialize a gailbot object that provides a suite of functions
             to interact with gailbot
 
         Args:
             ws_root (str): the path to workspace root
         """
         self.ws_manager: WorkspaceManager = WorkspaceManager(ws_root)
         self.init_workspace()
@@ -42,81 +41,68 @@
             No return but instantiates a new workspace.
         """
         try:
             self.ws_manager.clear_gb_temp_dir()
             self.ws_manager.init_workspace()
             return True
         except Exception as e:
-            logger.error(
-                f"failed to reset workspace due to the error {e}", exc_info=e
-            )
+            logger.error(f"failed to reset workspace due to the error {e}", exc_info=e)
             return False
 
-    def transcribe(
-        self, sources: List[str] = None
-    ) -> Tuple[List[str], List[str]]:
-        """given a list of the source name, and transcribe the sources
-
-        Args:
-            sources (List[str], optional): a list of source name, which
-            can be either a list of source paths or the file name of the
-            source file without the file extension
-            if sources is None, the default is to transcribe all sources
-            that have been configured
-
-        Returns:
-            Tuple[bool, List[str]]:
-                returns a tuple of two lists of string
-                the first lists consist of files that are not valid input
-                the second lists consist of files that fails to be processed
-
+    def clear_workspace(self):
         """
-        return self.gb.transcribe(sources)
+        Clears current workspace
 
-    def clear_source_memory(self) -> bool:
-        return self.gb.clear_source_memory()
-
-    def add_sources(self, src_output_pairs: List[Tuple[str, str]]) -> bool:
+        Returns: None
         """
-        Adds a given list of sources
+        try:
+            self.ws_manager.clear_gb_temp_dir()
+            return True
+        except Exception as e:
+            logger.error(f"failed to reset workspace due to the error {e}", exc_info=e)
+            return False
 
-        Args:
-            src_output_pairs: List [Tuple [str, str]]: List of Tuples of strings
-                to strings, each representing the source path and output path of
-                a source to add
+    def reset_workspace(self) -> bool:
+        """
+        Reset the gailbot workspace
 
-        Returns:
-            Bool: True if each given source was successfully added, false if not
+        Returns: True if workspace successfully reset; false otherwise
         """
-        return self.gb.add_sources(src_output_pairs)
+        return self.ws_manager.reset_workspace()
+
+    ###########################################################################
+    # Sources                                                                 #
+    ###########################################################################
 
     def add_source(self, source_path: str, output_dir: str) -> bool:
         """
         Adds a given source
 
         Args:
             source_path : str: Source path of the given source
             output_dir : str: Path to the output directory of the given source
 
         Returns:
             Union[str, bool]: return the name if successfully added, false if not
         """
         return self.gb.add_source(source_path, output_dir)
 
-    def remove_source(self, source_name: str) -> bool:
+    def add_sources(self, src_output_pairs: List[Tuple[str, str]]) -> bool:
         """
-        Removes the given source
+        Adds a given list of sources
 
         Args:
-            source_name : str: Name of the existing source to remove
+            src_output_pairs: List [Tuple [str, str]]: List of Tuples of strings
+                to strings, each representing the source path and output path of
+                a source to add
 
         Returns:
-            Bool: True if source was successfully removed, false if not
+            Bool: True if each given source was successfully added, false if not
         """
-        return self.gb.remove_source(source_name)
+        return self.gb.add_sources(src_output_pairs)
 
     def is_source(self, name: str) -> bool:
         """
         Determines if a given name corresponds to an existing source
 
         Args:
             name: str: Name of the source to look for
@@ -135,64 +121,147 @@
             source_name: str: source name to access
 
         Returns:
             a string stores the output path of the source
         """
         return self.gb.get_source_out_dir(name)
 
-    def create_new_setting(self, name: str, setting: Dict[str, str]) -> bool:
+    def remove_source(self, source_name: str) -> bool:
         """
-        Creates a new setting profile
+        Removes the given source
 
         Args:
-            name: str: Name to assign to the newly created setting
-            setting : Dict[str, str]: Dictionary representation of the setting
+            source_name : str: Name of the existing source to remove
 
         Returns:
-            None
+            Bool: True if source was successfully removed, false if not
         """
-        return self.gb.create_new_setting(name, setting)
+        return self.gb.remove_source(source_name)
 
-    def get_src_setting_name(self, source_name: str) -> Union[bool, str]:
-        """given a source name, return the setting name applied to the source
+    def remove_sources(self, source_names: List[str]) -> bool:
+        """
+        Removes the given list of sources
+        Args:
+            source_name : str: Name of the existing sources to remove
+        Returns:
+            Bool: True if all sources were successfully removed, false if not
+        """
+        return self.gb.remove_sources(source_names)
+
+    def get_source_setting_dict(self, source_name) -> Union[bool, SettingDict]:
+        """
+        Given a source, returns its setting content as a dictionary
 
         Args:
-            source_name (str): the name that identify the source
+            source_name (str): the name of the source
 
         Returns:
-            Union[bool, str]: if the source is found, return the setting name
-                              applied to the source, else return false
+            Union[bool, Dict[str, Union[str, Dict]]]:  a dictionary that stores
+            the source setting content
         """
-        return self.gb.get_src_setting_name(source_name)
+        return self.gb.get_source_setting_dict(source_name)
 
-    def save_setting(self, setting_name: str) -> bool:
+    def clear_source_memory(self) -> bool:
         """
-        Saves the given setting
+        Clears source memory
+
+        Returns:
+            bool: True if successfully cleared, False if not
+        """
+        return self.gb.clear_source_memory()
+
+    def get_all_source_names(self) -> List[str]:
+        """
+        Returns list of all source names
+
+        Returns: List[str] : list of source names
+        """
+        return self.gb.get_all_source_names()
+
+    def get_src_setting_name(self, source_name: str) -> Union[bool, str]:
+        """given a source name, return the setting name applied to the source
 
         Args:
-            setting_name: str: Name of the setting to save
+            source_name (str): the name that identify the source
 
         Returns:
-            Bool: True if setting was successfully saved, false if not
+            Union[bool, str]: if the source is found, return the setting name
+                              applied to the source, else return false
         """
-        return self.gb.save_setting(setting_name)
+        return self.gb.get_src_setting_name(source_name)
 
     def get_source_setting_dict(self, source_name) -> Union[bool, SettingDict]:
         """
         Given a source, returns its setting content as a dictionary
 
         Args:
             source_name (str): the name of the source
 
         Returns:
             Union[bool, Dict[str, Union[str, Dict]]]:  a dictionary that stores
             the source setting content
         """
         return self.gb.get_source_setting_dict(source_name)
 
+    ###########################################################################
+    # Transcribe                                                              #
+    ###########################################################################
+
+    # def keep
+    def transcribe(self, sources: List[str] = None) -> Tuple[List[str], List[str]]:
+        """given a list of the source name, and transcribe the sources
+
+        Args:
+            sources (List[str], optional): a list of source name, which
+            can be either a list of source paths or the file name of the
+            source file without the file extension
+            if sources is None, the default is to transcribe all sources
+            that have been configured
+
+        Returns:
+            Tuple[bool, List[str]]:
+                returns a tuple of two lists of string
+                the first lists consist of files that are not valid input
+                the second lists consist of files that fails to be processed
+
+        """
+        return self.gb.transcribe(sources)
+
+    ###########################################################################
+    # Setting (Profile)                                                       #
+    ###########################################################################
+
+    def create_new_setting(
+        self, name: str, setting: Dict[str, str], overwrite: bool = True
+    ) -> bool:
+        """
+        Creates a new setting profile
+
+        Args:
+            name: str: Name to assign to the newly created setting profile
+            setting : Dict[str, str]: Dictionary representation of the setting
+            overwrite : bool
+
+        Returns:
+            True if setting was successfully created, false if not
+        """
+        return self.gb.create_new_setting(name, setting, overwrite)
+
+    def save_setting(self, setting_name: str) -> bool:
+        """
+        Saves the given setting
+
+        Args:
+            setting_name: str: Name of the setting to save
+
+        Returns:
+            Bool: True if setting was successfully saved, false if not
+        """
+        return self.gb.save_setting(setting_name)
+
     def get_setting_dict(self, setting_name: str) -> Union[bool, SettingDict]:
         """
         Given a setting name, returns the setting content in a dictionary
 
         Args:
             setting_name (str): name that identifies a setting
 
@@ -202,29 +271,26 @@
         """
         return self.gb.get_setting_dict(setting_name)
 
     def get_all_settings_data(self) -> Dict[str, SettingDict]:
         """
         given a setting name, return the setting content in a dictionary format
 
-        Args:
-            setting_name (string): setting name
-
         Returns:
             Union[bool, Dict[str, Union[str, Dict]]]: the setting content
         """
         return self.gb.get_all_settings_data()
 
     def get_all_profile_names(self) -> List[str]:
         """get the names fo available settings
 
         Returns:
             List[str]: a list of available setting names
         """
-        return self.gb.get_all_profile_names()
+        return self.gb.get_all_settings_names()
 
     def rename_setting(self, old_name: str, new_name: str) -> bool:
         """
         Renames a given setting to a given new name
 
         Args:
             old_name: str: original name of the setting to rename
@@ -232,31 +298,30 @@
 
         Returns:
             Bool: True if setting was successfully renamed, false if not
 
         """
         return self.gb.rename_setting(old_name, new_name)
 
-    def update_setting(
-        self, setting_name: str, new_setting: Dict[str, str]
-    ) -> bool:
+    def update_setting(self, setting_name: str, new_setting: Dict[str, str]) -> bool:
         """
         Updates a given setting to a newly given structure
 
         Args:
             setting_name: str: name of the setting to update
             new_setting: Dict[str, str]: dictionary representation of
                 the new structure of the setting
 
         Returns:
             Bool: true if setting was successfully updated, false if not
         """
         return self.gb.update_setting(setting_name, new_setting)
 
-    def get_plugin_setting(self, setting_name: str) -> Dict[str, str]:
+    # keep
+    def get_plugin_setting(self, setting_name: str) -> bool | list[str]:
         """
         Accesses the plugin setting of a given setting
 
         Args:
             setting_name: str: name of the setting to get the plugin setting of
 
         Returns:
@@ -272,14 +337,26 @@
             setting_name: str: name of the setting to remove
 
         Returns:
             Bool: True if setting was successfully removed, false if not
         """
         return self.gb.remove_setting(setting_name)
 
+    def remove_multiple_settings(self, setting_names: List[str]) -> bool:
+        """
+        Removes the given list of settings
+
+        Args:
+            setting_name: List[str]: names of the setting to remove
+
+        Returns:
+            Bool: True if all settings were successfully removed, false if not
+        """
+        return self.gb.remove_multiple_settings(setting_names)
+
     def is_setting(self, name: str) -> bool:
         """
         Determines if a given setting name corresponds to an existing setting
 
         Args:
             name: str: name of the setting to search fort
 
@@ -291,15 +368,15 @@
     def apply_setting_to_source(
         self, source: str, setting: str, overwrite: bool = True
     ) -> bool:
         """
         Applies a given setting to a given source
 
         Args:
-            source: str: name of the source to which to apply the given setting
+            source: str: name of the source to which to apply the given setting profile
             setting: str: name of the setting to apply to the given source
             overwrite: bool: determines if it should overwrite from an existing setting
                 Defaults to true
 
         Returns:
             Bool: true if setting was successfully applied, false if not
         """
@@ -308,15 +385,15 @@
     def apply_setting_to_sources(
         self, sources: List[str], setting: str, overwrite: bool = True
     ) -> bool:
         """
         Applies a given setting to a given list of sources
 
         Args:
-            sources: List[str]: list of names of the sources to which to apply the given setting
+            sources: List[str]: list of names of the sources to which to apply the given setting profile
             setting: str: name of the setting to apply to the given sources
             overwrite: bool: determines if it should overwrite from an existing setting
                 Defaults to true
 
         Returns:
             Bool: true if setting was successfully applied, false if not
 
@@ -357,26 +434,28 @@
             setting_name (str): the name of the default setting
 
         Returns:
             bool: true if default setting is set correctly
         """
         return self.gb.set_default_setting(setting_name)
 
-    def register_plugin_suite(
-        self, plugin_source: str
-    ) -> Union[List[str], str]:
+    ###########################################################################
+    # Plugin Suite                                                            #
+    ###########################################################################
+
+    def register_plugin_suite(self, plugin_source: str) -> Union[List[str], str]:
         """
         Registers a gailbot plugin suite
 
         Args:
             plugin_source : str: Name of the plugin suite to register
 
         Returns:
-            return the a list of plugin name if the plugin is registered,
-            return the string that stores the error message if the pluginsuite
+            return  a list of plugin name if the plugin is registered,
+            return the string that stores the error message if the plugin suite
             is not registered
         """
         return self.gb.register_plugin_suite(plugin_source)
 
     def get_plugin_suite(self, suite_name) -> PluginSuite:
         """
         Gets the plugin suite with a given name
@@ -409,14 +488,26 @@
             suite_name: str: name of the plugin suite to delete
 
         Returns:
             Bool: true if plugin suite was successfully removed, false if not
         """
         return self.gb.delete_plugin_suite(suite_name)
 
+    def delete_plugin_suites(self, suite_names: List[str]) -> bool:
+        """
+        Removes the given list of plugin suites
+
+        Args:
+            suite_name: List[str]: list of names of the plugin suites to delete
+
+        Returns:
+            Bool: true if all plugin suites were successfully removed, false if not
+        """
+        return self.gb.delete_plugin_suites(suite_names)
+
     def add_progress_display(self, source: str, displayer: Callable) -> bool:
         """
         Add a function displayer to track for the progress of source,
 
         Args:
             source (str): the name of the source
             displayer (Callable): displayer is a function that takes in a string as
@@ -493,25 +584,25 @@
             suite_name (str): the name of the suite
 
         Returns:
             bool: true if the suite is official false otherwise
         """
         return self.gb.is_official_suite(suite_name)
 
-    def reset_workspace(self) -> bool:
-        """reset the gailbot workspace"""
-        return self.ws_manager.reset_workspace()
-
     def get_suite_source_path(self, suite_name: str) -> str:
         """
         given the name of the  suite , return the path to the source
         code of the suite
         """
         return self.gb.get_suite_path(suite_name)
 
+    ###########################################################################
+    # Engines                                                                 #
+    ###########################################################################
+
     def get_engine_setting_names(self) -> List[str]:
         """get a list of available engine setting name
 
         Returns:
             List[str]: the list of engine setting name
         """
         return self.gb.get_engine_setting_names()
@@ -527,15 +618,15 @@
 
         Returns:
             bool: return True if the engine setting is successfully created
         """
         return self.gb.add_new_engine(name, setting, overwrite)
 
     def remove_engine_setting(self, name) -> bool:
-        """remove the engine setting identified by nanme
+        """remove the engine setting identified by name
 
         Args:
             name (str): the name of the engine setting to be removed
 
         Returns:
             bool:  return True if the engine setting is successfully removed
         """
@@ -550,15 +641,15 @@
 
         Returns:
             bool:  return True if the engine setting is successfully updated
         """
         return self.gb.update_engine_setting(name, setting_data)
 
     def get_engine_setting_data(self, name: str) -> Union[bool, Dict[str, str]]:
-        """get the enigine setting data
+        """get the engine setting data
 
         Args:
             name (str): the name of the engine setting
 
         Returns:
             Union[bool, Dict[str, str]]: if the engine setting name is available
             return the engine setting data as stored in a dictionary, else return False
@@ -568,34 +659,18 @@
     def is_engine_setting_in_use(self, name: str) -> bool:
         """check if the engine setting identified by name is in use
 
         Args:
             name (str): the name of the engine setting
 
         Returns:
-            bool: return true if the engine setting is in use, false other wise
+            bool: return true if the engine setting is in use, false otherwise
         """
         return self.gb.is_engine_setting_in_use(name)
 
     def is_engine_setting(self, name: str):
         """check if the given engine name is engine setting
 
         Args:
             name (str): the name of the engine setting
         """
         return self.gb.is_engine_setting(name)
-
-    def get_profile_src_path(self, name: str):
-        """get the  path to the profile setting source
-
-        Args:
-            name (str): the name of the profile
-        """
-        return self.gb.get_profile_src_path(name)
-
-    def get_engine_src_path(self, name: str):
-        """get the  path to the engine setting source
-
-        Args:
-            name (str): the name of the engine
-        """
-        return self.gb.get_engine_src_path(name)
```

### Comparing `GailBot-0.1a9/src/gailbot/configs/confs/paths.py` & `GailBot-0.2a0/src/gailbot/configs/confs/paths.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/__init__.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/config/ws_config.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/config/ws_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,111 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-07-24 14:08:12
 import os
 from dataclasses import dataclass
 from dict_to_dataclass import field_from_dict, DataclassFromDict
 import toml
 from typing import Dict
 
+
 @dataclass
 class OutputFolder(DataclassFromDict):
     root: str = field_from_dict()
     transcribe_result: str = field_from_dict()
     analysis_result: str = field_from_dict()
     metadata: str = field_from_dict()
     media_file: str = field_from_dict()
     format_result: str = field_from_dict()
 
+
 @dataclass
 class TemporaryFolder(DataclassFromDict):
     root: str = field_from_dict()
     transcribe_ws: str = field_from_dict()
     format_ws: str = field_from_dict()
     analysis_ws: str = field_from_dict()
     data_copy: str = field_from_dict()
 
+
 @dataclass
 class FileExtensions(DataclassFromDict):
     temp: str = field_from_dict()
     output: str = field_from_dict()
 
+
 @dataclass
-class EngineWS():
-    def __init__(self, ws_root:str, path_dict: Dict[str, str]) -> None:
+class EngineWS:
+    def __init__(self, ws_root: str, path_dict: Dict[str, str]) -> None:
         self.whisper = os.path.join(ws_root, path_dict["whisper"])
         self.google = os.path.join(ws_root, path_dict["google"])
         self.watson = os.path.join(ws_root, path_dict["watson"])
         self.google_api = os.path.join(ws_root, path_dict["google_api"])
 
+
 @dataclass
-class GailBotData():
-    def __init__(self, ws_root: str, path_dict: Dict[str,  str]) -> None:
-        self.root:        str = path_dict["root"]
-        self.setting_src: str = os.path.join(ws_root, self.root, path_dict["setting_src"])
-        self.plugin_src:  str = os.path.join(ws_root, self.root, path_dict["plugin_src"])
-        self.engine_src:  str = os.path.join(ws_root, self.root, path_dict["engine_setting"])
-        self.root:        str = os.path.join(ws_root, self.root)
+class GailBotData:
+    def __init__(self, ws_root: str, path_dict: Dict[str, str]) -> None:
+        self.root: str = path_dict["root"]
+        self.setting_src: str = os.path.join(
+            ws_root, self.root, path_dict["setting_src"]
+        )
+        self.plugin_src: str = os.path.join(ws_root, self.root, path_dict["plugin_src"])
+        self.engine_src: str = os.path.join(
+            ws_root, self.root, path_dict["engine_setting"]
+        )
+        self.root: str = os.path.join(ws_root, self.root)
+
 
 @dataclass
 class WorkSpaceConfig:
-    def __init__(self, config_path: str, ws_root:str) -> None:
+    def __init__(self, config_path: str, ws_root: str) -> None:
         d = toml.load(config_path)
         self._output_d: Dict = d["output"]
         self._workspace_d: Dict = d["workspace"]
         self._extension_d: Dict = d["file_extensions"]
         self._ws_root = ws_root
         # public path data
         self.workspace_root = os.path.join(self._ws_root, self._workspace_d["ws_root"])
         self.tempspace_root = os.path.join(
-            self.workspace_root, self._workspace_d["temporary"]["root"])
+            self.workspace_root, self._workspace_d["temporary"]["root"]
+        )
         self.gailbot_data: GailBotData = GailBotData(
-            self.workspace_root, self._workspace_d["gailbot_data"])
-        self.file_extension : FileExtensions = FileExtensions.from_dict(self._extension_d)
-        self.engine_ws: EngineWS = EngineWS(self.workspace_root, self._workspace_d["engine"])
+            self.workspace_root, self._workspace_d["gailbot_data"]
+        )
+        self.file_extension: FileExtensions = FileExtensions.from_dict(
+            self._extension_d
+        )
+        self.engine_ws: EngineWS = EngineWS(
+            self.workspace_root, self._workspace_d["engine"]
+        )
 
-    def get_temp_space(self, name:str)-> TemporaryFolder:
-        """ Given a name of the source, return a dataclass object that stores
+    def get_temp_space(self, name: str) -> TemporaryFolder:
+        """Given a name of the source, return a dataclass object that stores
             the temporary directory structures of source, including the
             full paths to every subdirectory in the temporary directory
 
         Args:
             name (str): the name of the source
 
         Returns:
             TemporaryFolder: a dataclass object that stores the full paths
             of every subdirectories within the temporary folders for a
             particular source
         """
         temp_dir: Dict[str, str] = self._workspace_d["temporary"].copy()
         for key, value in temp_dir.items():
-                temp_dir[key] = os.path.join(self.tempspace_root, name, value)
+            temp_dir[key] = os.path.join(self.tempspace_root, name, value)
         temp_dir["root"] = os.path.join(self.tempspace_root, name)
         return TemporaryFolder.from_dict(temp_dir)
 
     def get_output_space(self, root) -> OutputFolder:
-        """ Given a name of the source,  and the user selected output directory
+        """Given a name of the source,  and the user selected output directory
             root, return a dataclass object that stores
             the output directory structures of source, including the
             full paths to every subdirectory in the output directory
 
         Args:
             root (str): the root the directory of the output
             name (str): the name of the source
@@ -99,13 +120,11 @@
             new_output_dir[key] = os.path.join(root, value)
         new_output_dir["root"] = root
         return OutputFolder.from_dict(new_output_dir)
 
     def get_output_structure(self) -> OutputFolder:
         return OutputFolder.from_dict(self._output_d)
 
+
 def load_workspace_config(config_path, ws_root) -> WorkSpaceConfig:
-    """ public function that load the workspace data and return it """
+    """public function that load the workspace data and return it"""
     return WorkSpaceConfig(config_path, ws_root)
-
-
-
```

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/google.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/watson.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-07-24 14:34:21
 from dataclasses import dataclass
 from dict_to_dataclass import field_from_dict, DataclassFromDict
-from typing import Dict 
-import toml 
+from typing import Dict
+import toml
 
 
-@dataclass 
-class GoogleConfig(DataclassFromDict):
-    """Loads data from the Google STT configuration"""
+@dataclass
+class WatsonConfig(DataclassFromDict):
+    """Loads data from the Watson engine configuration"""
+
+    max_file_size_bytes: float = field_from_dict()
+    regions_uris: Dict = field_from_dict()
+    format_to_content: Dict = field_from_dict()
     defaults: Dict = field_from_dict()
-    name: str      = field_from_dict()
+    name: str = field_from_dict()
     workspace: str = field_from_dict()
-    maximum_size: int = field_from_dict()
-    maximum_duration: int = field_from_dict()
 
-def load_google_config(path: str):
-    """
-    Loads data from the Google STT configuration
+
+def load_watson_config(path: str):
+    """Loads data from the Watson engine configuration
 
     Args:
         path (str) : path to the toml file to load
     """
     d = toml.load(path)
-    return GoogleConfig.from_dict(d["google"])
+    return WatsonConfig.from_dict(d["watson"])
```

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/whisper.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/whisper.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/core/setting/defaults.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/core/setting/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-from dataclasses import dataclass 
-import os 
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-07-24 14:34:28
+from dataclasses import dataclass
+import os
 from dict_to_dataclass import field_from_dict, DataclassFromDict
 from typing import Dict, List
-import toml 
+import toml
 
 
-@dataclass 
+@dataclass
 class PluginDefault(DataclassFromDict):
-    suite : str = field_from_dict()
+    suite: str = field_from_dict()
     apply_plugins: List[str] = field_from_dict()
-    
+
+
 @dataclass
 class EngineDefault(DataclassFromDict):
-    name : str = field_from_dict()
-    whisper : Dict = field_from_dict()
-    watson : Dict = field_from_dict()
-    
-    
+    name: str = field_from_dict()
+    whisper: Dict = field_from_dict()
+    watson: Dict = field_from_dict()
+
+
 @dataclass
 class Default(DataclassFromDict):
     def __init__(self, plugin: PluginDefault, engine: EngineDefault) -> None:
         self.plugin: PluginDefault = plugin
-        self.engine: EngineDefault = engine 
-        
-def load_default_config(path:str) :
+        self.engine: EngineDefault = engine
+
+
+def load_default_config(path: str):
     d = toml.load(path)
     print(d)
     engine = EngineDefault.from_dict(d["engine"])
     plugin = PluginDefault.from_dict(d["plugins"])
-    return Default(plugin, engine)
+    return Default(plugin, engine)
```

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/pluginsuite.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/pluginsuite.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-07-24 14:34:37
 from dataclasses import dataclass
 
 
 @dataclass
 class PLUGIN_CONFIG:
     HILAB_BUCKET = "gailbot-plugin-suite-official"
     EN_KEY = b"25T_bNAjTALUgva1C-au0IKwESptsLAztLRVVEyCtZs="
     ENCRYPTED_API_ID = b"gAAAAABkU5CF3GwKfqwPBvgG4fibAHjZ2hE1pQdEb8Nkw06YubGZ9_mekBRgMiRXPrXo7C_6i-uuBpisZyL3FpFwg8zXvxR9_jrPocUkMjSmyHFJQUYojys="
     ENCRYPTED_API_KEY = b"gAAAAABkU5CF1Q_ebrx9OTuW0WWQypQKTk25JPPIrRGAyoDLgweyh-2tDnD4CdmUE_xpprxVMttgvz7FzR2sDMn6jJ3EyYNxUCHgudOBkwPoYYM7a6fMheNLlyT3x_SzszpnxfF2y7-m"
-    THREAD_NUM = 1
+    THREAD_NUM = 3
     DOCUMENT = "DOCUMENT.md"
     REQUIREMENT = "requirement.txt"
     OFFICIAL = ".gb_official"
     CONFIG = "config.toml"
     FORMAT = "format.md"
     HILAB_SUITE_ZIP = "https://gailbot-official-plugin-suite.s3.us-east-2.amazonaws.com/gb_hilab_suite.zip"
     OFFICIAL_KEY = b"KM1V0_HijdrehPVsFueXISED2Jxs0S_rR9zKAJzcW3A="
```

### Comparing `GailBot-0.1a9/src/gailbot/configs/interfaces/services/service.py` & `GailBot-0.2a0/src/gailbot/configs/interfaces/services/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,67 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-07-24 14:34:48
 from dataclasses import dataclass
 from dict_to_dataclass import field_from_dict, DataclassFromDict
-import toml 
+import toml
 from typing import List, Dict
 
+
+@dataclass
+class DirectoryName(DataclassFromDict):
+    temp_extension: str = field_from_dict()
+    output_extension: str = field_from_dict()
+    hidden_file: str = field_from_dict()
+    trans_result: str = field_from_dict()
+    temp_result: str = field_from_dict()
+    analysis_result: str = field_from_dict()
+
+
 @dataclass
-class DirectoryName(DataclassFromDict): 
-      temp_extension                   : str = field_from_dict()
-      output_extension                 : str = field_from_dict()
-      hidden_file                      : str = field_from_dict()
-      trans_result                     : str = field_from_dict()
-      temp_result                      : str = field_from_dict()
-      analysis_result                  : str = field_from_dict()
-@dataclass
-class Engines(DataclassFromDict): 
-      engine                     : str = field_from_dict()
-      google_name                : str = field_from_dict()
-      watson_name                : str = field_from_dict()
-      whisper_name               : str = field_from_dict()
-      audio_supported_format     : List[str] = field_from_dict()
-
-@dataclass 
-class Thread(DataclassFromDict): 
-      transcriber_num_threads  : int = field_from_dict()
-      payload_num_threads      : int = field_from_dict()
-      analysis_num_threads     : int = field_from_dict()
+class Engines(DataclassFromDict):
+    engine: str = field_from_dict()
+    google_name: str = field_from_dict()
+    watson_name: str = field_from_dict()
+    whisper_name: str = field_from_dict()
+    audio_supported_format: List[str] = field_from_dict()
+
+
+@dataclass
+class Thread(DataclassFromDict):
+    transcriber_num_threads: int = field_from_dict()
+    payload_num_threads: int = field_from_dict()
+    analysis_num_threads: int = field_from_dict()
+
+
 @dataclass
 class ServiceConfig(DataclassFromDict):
-    engines : Engines = field_from_dict()
-    directory_name : DirectoryName = field_from_dict()
-    thread : Thread = field_from_dict()
+    engines: Engines = field_from_dict()
+    directory_name: DirectoryName = field_from_dict()
+    thread: Thread = field_from_dict()
+
 
-@dataclass 
+@dataclass
 class ProfileData(DataclassFromDict):
     plugin_setting: List[str] = field_from_dict()
     engine_setting_name: str = field_from_dict()
-@dataclass 
-class DefaultSetting(DataclassFromDict): 
-    profile_name                     : str = field_from_dict()
-    profile_data                     : dict = field_from_dict()
-    engine_name                      : str = field_from_dict() 
-    engine_data                      : dict = field_from_dict()
-    profile_data_no_plugin           : dict = field_from_dict()
+
+
+@dataclass
+class DefaultSetting(DataclassFromDict):
+    profile_name: str = field_from_dict()
+    profile_data: dict = field_from_dict()
+    engine_name: str = field_from_dict()
+    engine_data: dict = field_from_dict()
+    profile_data_no_plugin: dict = field_from_dict()
 
 
 def load_service_config(path: str) -> ServiceConfig:
     d = toml.load(path)
     return ServiceConfig.from_dict(d)
 
+
 def load_default_setting(path: str) -> DefaultSetting:
     d = toml.load(path)
-    return DefaultSetting.from_dict(d)
+    return DefaultSetting.from_dict(d)
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/engine.py` & `GailBot-0.2a0/src/gailbot/core/engines/engine.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/engineManager.py` & `GailBot-0.2a0/src/gailbot/core/engines/engineManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-10 13:29:08
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 15:02:59
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:32:56
 from typing import Dict, List, Any
-from gailbot.core.engines import (
-    Engine,
-    Watson,
-    Google,
-    WhisperEngine
-)
-
-_ENGINES = {
-    "watson" : Watson,
-    "google" : Google,
-    "whisper" : WhisperEngine
-}
+from gailbot.core.engines import Engine, Watson, Google, WhisperEngine, WhisperX
+
+_ENGINES = {"watson": Watson, "google": Google, "whisper": WhisperEngine, "whisperX": WhisperX}
+
 
 class EngineManager:
-    """ 
+    """
     provides wrapper function to run available speech detect engines
     """
+
     def available_engines(self) -> List[str]:
         """
         Returns:
             List[str]: return a list of available engine
         """
         return list(_ENGINES.keys())
 
-    def is_engine(self, name : str) -> bool:
+    def is_engine(self, name: str) -> bool:
         return name in self.available_engines()
 
-    def init_engine(self, name : str, **kwargs) -> Engine:
+    def init_engine(self, name: str, **kwargs) -> Engine:
         if not self.is_engine(name):
-            raise Exception(
-                f"Engine not supported: {name}"
-            )
+            raise Exception(f"Engine not supported: {name}")
         engine = _ENGINES[name](**kwargs)
-        return engine
+        return engine
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/exception.py` & `GailBot-0.2a0/src/gailbot/core/engines/exception.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/google/core.py` & `GailBot-0.2a0/src/gailbot/core/engines/google/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,276 +1,300 @@
 # -*- coding: utf-8 -*-
 # @Author: Vivian Li, Siara Small
 # @Date:   2023-01-30 16:00
-# @Last Modified by:  Vivian Li
-# @Last Modified time: 2023-01-31 12:01:31
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:49:21
 
 # stdlib import
-import os 
+import os
 import io
 from copy import deepcopy
 from typing import Union
 from urllib import request
-from typing import Dict, List 
+from typing import Dict, List
 
 # internal import
 from gailbot.core.utils.general import (
-    get_extension, 
     get_extension,
-    is_directory, 
+    get_extension,
+    is_directory,
     make_dir,
-    get_name)
+    get_name,
+)
 from gailbot.core.utils.download import is_internet_connected
 from gailbot.core.utils.logger import makelogger
 from ...engines import exception as EXCEPTION
 from gailbot.configs import google_config_loader, workspace_config_loader
 from gailbot.core.utils.media import MediaHandler
 
-#external import
+# external import
 from google.cloud.speech_v1p1beta1.types import cloud_speech
 from google.cloud import speech_v1p1beta1 as speech
 
 logger = makelogger("google")
 GOOGLE_CONFIG = google_config_loader()
 
-class GoogleCore: 
+
+class GoogleCore:
     """
-    Implement core functionalities to transcribe an audio file through 
+    Implement core functionalities to transcribe an audio file through
     google STT engine
     """
+
     ENCODING_TABLE = {
-        "wav": speech.RecognitionConfig.AudioEncoding.LINEAR16, 
+        "wav": speech.RecognitionConfig.AudioEncoding.LINEAR16,
         "mp3": speech.RecognitionConfig.AudioEncoding.MP3,
         "opus": speech.RecognitionConfig.AudioEncoding.OGG_OPUS,
         "flac": speech.RecognitionConfig.AudioEncoding.FLAC,
-        "amr": speech.RecognitionConfig.AudioEncoding.AMR
+        "amr": speech.RecognitionConfig.AudioEncoding.AMR,
     }
-    
-    def __init__(self, google_api_key_config) -> None:  
+
+    def __init__(self, google_api_key_config) -> None:
         """initialize an instance of google engine
 
         Args:
             google_api_key_config (str): path to a json file that stores
             google cloud speech to text api key
-        """     
+        """
         self._init_status()
         client = GoogleCore.is_valid_google_api(google_api_key_config)
         self.workspace = workspace_config_loader().engine_ws.google
-        assert client 
+        assert client
         self.connected = True
         self.current_chunk_duration = GOOGLE_CONFIG.maximum_duration
-        
-    
+
     @staticmethod
     def is_valid_google_api(google_api_key_config: str):
-        """ Given a path to a json file that stores the google api key
-            return the google client if the api is valid, else return false     
+        """Given a path to a json file that stores the google api key
+            return the google client if the api is valid, else return false
 
         Args:
-            google_api_key_config (str): a path to a file that stores the google api 
-                                 key 
+            google_api_key_config (str): a path to a file that stores the google api
+                                 key
 
         Returns:
-            Union(SpeechCient, bool): if the api key is valid, return the google 
-                                      speech client, else return false 
+            Union(SpeechCient, bool): if the api key is valid, return the google
+                                      speech client, else return false
         """
         try:
-            assert get_extension(google_api_key_config) == "json", "The google api key file is in wrong format"
-            os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = google_api_key_config
-            client = speech.SpeechClient() 
-            return client  
+            assert (
+                get_extension(google_api_key_config) == "json"
+            ), "The google api key file is in wrong format"
+            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = google_api_key_config
+            client = speech.SpeechClient()
+            return client
         except Exception as e:
             logger.error("f failed to connect to google", exc_info=e)
-            return False 
-        
+            return False
+
     @property
     def supported_formats(self) -> List[str]:
         """
-        Access the supported audio formats 
+        Access the supported audio formats
 
         Returns:
             List[str] : list of supported formats
         """
-        return list[self.ENCODING_TABLE]
+        return List[self.ENCODING_TABLE]
 
     def is_file_supported(self, file: str) -> bool:
         """
         Determines if a given file is supported
 
         Args:
             file (str) : file name to check if supported
 
         Returns: True if the file is supported, false if not.
         """
         return get_extension(file) in self.supported_formats
-   
-    
-    def transcribe(self, audio_path: str, payload_workspace: str) -> List[Dict[str, str]]:
+
+    def transcribe(
+        self, audio_path: str, payload_workspace: str
+    ) -> List[Dict[str, str]]:
         """
         Transcribes the provided audio stream using a websocket connections.
-        And output the result to given output directory 
+        And output the result to given output directory
 
         Args:
-            audio_path (str) : 
+            audio_path (str) :
                 path to audio file that will be transcribed
-            output_directory (str) : 
+            output_directory (str) :
                 path to directory where the transcribed data will be stored
-        
+
         Return:
-            A list of dictionary that contains the utterance data of the 
-            audio file, each part of the audio file is stored in the format 
+            A list of dictionary that contains the utterance data of the
+            audio file, each part of the audio file is stored in the format
             {speaker: , start_time: , end: , text: }
         """
         logger.info("start transcribing audio using google cloud STT")
         if not is_internet_connected():
             raise EXCEPTION.TranscriptionError(EXCEPTION.ERROR.CONNECTION_ERROR)
-        # get the info of audio source and preprocess the audio if needed 
+        # get the info of audio source and preprocess the audio if needed
         mediaHandler = MediaHandler()
         stream = mediaHandler.read_file(audio_path)
         info = mediaHandler.info(stream)
         logger.info(f"the audio file information is {info}")
-        
+
         audio_duration = info["duration_seconds"]
-        audio_channels = info["channels"] 
+        audio_channels = info["channels"]
         audio_format = info["format"]
-       
-        #  convert stereo to mono 
+
+        #  convert stereo to mono
         if audio_channels > 1:
             logger.info("detect stereo audio file, converting to mono file")
             l_stream, _ = mediaHandler.stereo_to_mono(stream)
-            audio_path = mediaHandler.write_stream(l_stream, out_dir=payload_workspace, name=get_name(audio_path), format=info["format"])
-            
+            audio_path = mediaHandler.write_stream(
+                l_stream,
+                out_dir=payload_workspace,
+                name=get_name(audio_path),
+                format=info["format"],
+            )
+
         # convert the wav file to all bit 16 bit
         if audio_format.lower() == "wav":
             logger.info("detect wav file, converting to wav 16 bit header file")
-            wav_copy_ws = os.path.join(payload_workspace, f"{get_name(audio_path)}_wav_16bit")
+            wav_copy_ws = os.path.join(
+                payload_workspace, f"{get_name(audio_path)}_wav_16bit"
+            )
             if not is_directory(wav_copy_ws):
                 make_dir(wav_copy_ws)
-            output_for16 = os.path.join(wav_copy_ws, f"{get_name(audio_path)}_16bit.wav")
+            output_for16 = os.path.join(
+                wav_copy_ws, f"{get_name(audio_path)}_16bit.wav"
+            )
             audio_path = MediaHandler.convert_to_16bit_wav(audio_path, output_for16)
-        
+
         # chunk the audio lager than 60 seconds
         if audio_duration >= GOOGLE_CONFIG.maximum_duration:
             logger.info(f"audio length exceeds maximum limit")
-            # get the duration each chunk 
+            # get the duration each chunk
             chunk_duration = GoogleCore._get_chunk_duration(audio_path, audio_duration)
             self.current_chunk_duration = chunk_duration
-            # chunk the file 
-            audio_list = MediaHandler.chunk_audio_to_outpath(audio_path, payload_workspace, chunk_duration)
+            # chunk the file
+            audio_list = MediaHandler.chunk_audio_to_outpath(
+                audio_path, payload_workspace, chunk_duration
+            )
         else:
             audio_list = [audio_path]
-            
+
         try:
-            return  self._transcribe_list_file(audio_list, payload_workspace)
+            return self._transcribe_list_file(audio_list, payload_workspace)
         except Exception as e:
             logger.error(e, exc_info=e)
-            raise EXCEPTION.TranscriptionError(EXCEPTION.ERROR.GOOGLE_TRANSCRIPTION_FAILED)
-        
+            raise EXCEPTION.TranscriptionError(
+                EXCEPTION.ERROR.GOOGLE_TRANSCRIPTION_FAILED
+            )
+
     def _run_engine(self, audio_path: str, workspace) -> cloud_speech.RecognizeResponse:
-        """ 
-        run the google STT engine to transcribe the file 
-        
-        Args: 
+        """
+        run the google STT engine to transcribe the file
+
+        Args:
             audio_path (str):
                 path to audio file that will be transcribed
-        
+
         Return (cloud_speech.RecognizeResponse):
-            return the response data from google STT 
+            return the response data from google STT
         """
         logger.info(f"rung google engine on file {audio_path}")
         try:
             # initialize client
-            client = speech.SpeechClient() 
-            
-            # preprocessing the file 
+            client = speech.SpeechClient()
+
+            # preprocessing the file
             format = get_extension(audio_path).lower()
             encoding = self.ENCODING_TABLE[format]
             kwargs = deepcopy(GOOGLE_CONFIG.defaults)
-            
+
             # add additional key word arguments for file that is no in wav or flac format
             if not (format == "wav" or format == "flac"):
                 kwargs.update({"encoding": encoding, "sample_rate_hertz": 16000})
 
-            # read audio file 
+            # read audio file
             with io.open(audio_path, "rb") as audio:
                 content = audio.read()
-                audio = speech.RecognitionAudio(content = content)
+                audio = speech.RecognitionAudio(content=content)
                 self.read_audio = True
-           
-            # transcribe audio file 
+
+            # transcribe audio file
             config = speech.RecognitionConfig(**kwargs)
             self.transcribing = True
             response = client.recognize(config=config, audio=audio)
-        
+
         except Exception as e:
             logger.error(e, exc_info=e)
             self.transcribe_error = True
-            raise EXCEPTION.TranscriptionError(EXCEPTION.ERROR.GOOGLE_TRANSCRIPTION_FAILED)
+            raise EXCEPTION.TranscriptionError(
+                EXCEPTION.ERROR.GOOGLE_TRANSCRIPTION_FAILED
+            )
         else:
             logger.info("get google response ")
             self.transcribing = False
             self.transcribe_success = True
         return response
-      
-    def _prepare_utterance(self, response: cloud_speech.RecognizeResponse, offset = 0) -> List[Dict[str, str]]:
+
+    def _prepare_utterance(
+        self, response: cloud_speech.RecognizeResponse, offset=0
+    ) -> List[Dict[str, str]]:
         """
-        output the response data from google STT, convert the raw data to 
-        utterance data which is a list of dictionary in the format 
+        output the response data from google STT, convert the raw data to
+        utterance data which is a list of dictionary in the format
         {speaker: , start_time: , end: , text: }
-        
-        Args: 
-            output_directory(str) : output path 
-            response (cloud_speech.RecognizeResponse): raw response from google 
-        
+
+        Args:
+            output_directory(str) : output path
+            response (cloud_speech.RecognizeResponse): raw response from google
+
         Return:
-            A list of dictionary that contains the utterance data of the 
-            audio file, each part of the audio file is stored in the format 
+            A list of dictionary that contains the utterance data of the
+            audio file, each part of the audio file is stored in the format
             {speaker: , start_time: , end: , text: }
         """
 
         results = response.results
         logger.info("get the google response")
         status_result = {
             "connected": self.connected,
-            "read_audio": self.read_audio, 
-            "transcribing": self.transcribing, 
+            "read_audio": self.read_audio,
+            "transcribing": self.transcribing,
             "transcribe_success": self.transcribe_success,
             "transcribe_error": self.transcribe_error,
             "output_success": True,
             "request_id": response.request_id,
         }
-        
+
         logger.info(status_result)
         """ Prepare Utterance """
         utterances = list()
         for result in results:
             alternative = result.alternatives[0]
             if alternative.transcript:
                 for word in alternative.words:
                     utt = {
-                        "start":word.start_time.total_seconds() + float(offset), 
-                        "end":word.end_time.total_seconds() + float(offset),
+                        "start": word.start_time.total_seconds() + float(offset),
+                        "end": word.end_time.total_seconds() + float(offset),
                         "text": word.word,
-                        "speaker": str(word.speaker_tag)
+                        "speaker": str(word.speaker_tag),
                     }
                     utterances.append(utt)
         return utterances
-    
+
     def _init_status(self):
-        """ 
+        """
         Initializes the status
         """
         self.connected = False
         self.read_audio = False
         self.transcribing = False
         self.transcribe_success = False
         self.transcribe_error = False
         self.output_success = False
-    
-    def _transcribe_list_file(self, audios: List[str], workspace) -> List[Dict[str, str]]:
+
+    def _transcribe_list_file(
+        self, audios: List[str], workspace
+    ) -> List[Dict[str, str]]:
         """transcribe a list of audios and return the utterance result
 
         Args:
             audios (List[str]): a list of path to audio source
             workspace (str): the path to workspace
 
         Returns:
@@ -282,31 +306,30 @@
         for audio in audios:
             logger.info(f"transcribe {audio} in progress")
             response = self._run_engine(audio, workspace)
             assert response
             logger.info("geting the response in chunk")
             new_utt = self._prepare_utterance(response, offset)
             utterances.extend(new_utt)
-            offset += self.current_chunk_duration 
+            offset += self.current_chunk_duration
         return utterances
-    
+
     @staticmethod
     def _get_chunk_duration(file_path: str, file_duration: int) -> int:
-        """given the file path and file duration calculate the expected 
-           chunk duration that is able to send the chunked file to googl cloud 
+        """given the file path and file duration calculate the expected
+           chunk duration that is able to send the chunked file to googl cloud
 
         Args:
             file_path (str): a str to the file path
-            file_duration (int): the lenth of the file 
+            file_duration (int): the lenth of the file
 
         Returns:
-            int: the expected duration of each audio chunk 
+            int: the expected duration of each audio chunk
         """
         duration = GOOGLE_CONFIG.maximum_duration
         filesize = os.path.getsize(file_path)
         num_chunks = file_duration // GOOGLE_CONFIG.maximum_duration
         size_60 = filesize / num_chunks
         if size_60 >= GOOGLE_CONFIG.maximum_size:
-            duration = duration * (GOOGLE_CONFIG.maximum_size / size_60) 
+            duration = duration * (GOOGLE_CONFIG.maximum_size / size_60)
         logger.info(f"chunk audio to {duration}")
         return duration
-
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/google/google.py` & `GailBot-0.2a0/src/gailbot/core/engines/google/google.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,87 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:30:31
 
 from ..engine import Engine
 from ...engines import exception as Err
 from ..google.core import GoogleCore
 from typing import Any, List, Dict
 from typing import Dict, List, Union
-from gailbot.core.utils.logger import makelogger 
+from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("google engine")
+
+
 class Google(Engine):
-    """ 
-    An Engine that connect to Google Cloud STT, provide function to transcribe 
+    """
+    An Engine that connect to Google Cloud STT, provide function to transcribe
     audio file with Google Cloud STT
 
     Inheritance:
-        Engine 
+        Engine
     """
+
     ENGINE_NAME = "Google"
-    def __init__(self, google_api_key:str):
+
+    def __init__(self, google_api_key: str):
         logger.info("google engine initialized")
         self.core = GoogleCore(google_api_key)
         self.transcribe_success = False
-    
+
     def __repr__(self):
         return self.ENGINE_NAME
-    
+
     @property
     def supported_formats(self) -> List[str]:
-        """ 
-        a list of supported format that can be transcribe with the STT engine 
+        """
+        a list of supported format that can be transcribe with the STT engine
         """
         return self.core.supported_formats
-    
-    def transcribe(self, audio_path: str, payload_workspace:str) -> List[Dict[str, str]] :
-        """ use Google engine to transcribe the audio file 
+
+    def transcribe(
+        self, audio_path: str, payload_workspace: str
+    ) -> List[Dict[str, str]]:
+        """use Google engine to transcribe the audio file
 
         Args:
             audio_path (str): path to audio source
-            output_directory (str): path to output directory 
+            output_directory (str): path to output directory
 
         Raises:
             Err.TranscriptionError
 
         Returns:
-            A list of dictionary that contains the utterance data of the 
-            audio file, each part of the audio file is stored in the format 
+            A list of dictionary that contains the utterance data of the
+            audio file, each part of the audio file is stored in the format
             {speaker: , start_time: , end_time: , text: }
         """
         res = self.core.transcribe(audio_path, payload_workspace)
         self.transcribe_success = True
         return res
-    
+
     def is_file_supported(self, file_path: str) -> bool:
-        """ 
-        given a file path, return true if the file format is supported by 
-        the Google STT engine 
+        """
+        given a file path, return true if the file format is supported by
+        the Google STT engine
         """
         return self.core.is_file_supported(file_path)
-    
+
     def get_supported_formats(self) -> List[str]:
-        """ 
-        return a list of supported format that can be 
-        transcribe with the STT engine 
+        """
+        return a list of supported format that can be
+        transcribe with the STT engine
         """
         return self.core.supported_formats
-    
+
     def get_engine_name(self) -> str:
         return self.ENGINE_NAME
-    
+
     def was_transcription_successful(self) -> bool:
         return self.transcribe_success
-    
 
-    @staticmethod 
+    @staticmethod
     def is_valid_google_api(google_api_key) -> bool:
         engine = GoogleCore.is_valid_google_api(google_api_key)
-        return True if engine else False
+        return True if engine else False
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/watson/am.py` & `GailBot-0.2a0/src/gailbot/core/engines/watson/am.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-09 11:41:12
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 12:01:31
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:31:22
 
 # Standard library imports
 from typing import Any, BinaryIO, List, TextIO, Tuple, Dict, Callable, Union
 from enum import IntEnum
+
 # Local imports
 
 # Third party imports
 from ibm_watson import SpeechToTextV1, ApiException
 from ibm_cloud_sdk_core.authenticators import IAMAuthenticator
 from gailbot.core.engines import exception as ERR
 from ibm_watson.speech_to_text_v1 import CustomWord
 
 from gailbot.configs import watson_config_loader
 from gailbot.core.utils.media import MediaHandler
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 from .codes import WatsonReturnCodes
 
 WATSON_CONFIG = watson_config_loader()
 
+
 class WatsonAMInterface:
     """
     Responsible for interacting with the IBM Watson STT service and providing
     methods for interacting with acoustic models.
     """
-    def __init__(self, apikey : str, region : str):
 
+    def __init__(self, apikey: str, region: str):
         self.apikey = apikey
         self.region = region
         self.media_h = MediaHandler()
         self.connected_to_service = False
         # Parse confs
         self._regions = WATSON_CONFIG.regions_uris
         self._format_to_content_types = WATSON_CONFIG.format_to_content
         self._defaults = WATSON_CONFIG.defaults
         self.max_size_bytes = WATSON_CONFIG.max_file_size_bytes
 
         if not self._is_api_key_valid(apikey, self._regions[region]):
             raise Exception(f"Apikey {apikey} invalid")
         if not region in self._regions:
-            raise Exception(
-                f"Region {region} not in {list(self._regions.keys())}"
-            )
+            raise Exception(f"Region {region} not in {list(self._regions.keys())}")
         try:
             # Create the stt service and run
             authenticator = IAMAuthenticator(self.apikey)
             self.stt = SpeechToTextV1(authenticator=authenticator)
             self.stt.set_service_url(self._regions[self.region])
-        except: 
+        except:
             raise ERR.ConnectionError("ERROR: Failed to connect to the Watson STT")
         else:
-            self.connected_to_service  = True
-    
-    def get_custom_model(
-        self,
-        customization_id: str
-    ) -> Union[Dict[str, Any], None]:
+            self.connected_to_service = True
+
+    def get_custom_model(self, customization_id: str) -> Union[Dict[str, Any], None]:
         """
         Obtain information regarding a specific custom acoustic model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
@@ -73,104 +71,106 @@
                 Mapping from the following keys to their values:
                 customization_id, CREATED, updated,language, dialect,
                 versions, owner, name, description, base_model_name, status,
                 progress
                 None if unsuccessful.
         """
         _, resp = self._execute_watson_method(
-            self.stt.get_acoustic_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.get_acoustic_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return resp
 
     def get_custom_models(self) -> Dict[str, str]:
         """
         Obtain all custom acoustic models
 
         Returns:
             (Dict[str,str]):
                 Mapping from custom acoustic model to the customization id.
         """
         custom_models = dict()
         response = self._execute_watson_method(
-            self.stt.list_acoustic_models, [WatsonReturnCodes.OK])
+            self.stt.list_acoustic_models, [WatsonReturnCodes.OK]
+        )
         if response:
             for model in response["customizations"]:
                 custom_models[model["name"]] = model["customization_id"]
         return custom_models
 
     def create_custom_model(
-        self,
-        name : str,
-        base_model_name : str,
-        description : str
+        self, name: str, base_model_name: str, description: str
     ) -> bool:
         """
         Create a new custom acoustic model.
 
         Args:
             name (str): Name of the model.
             base_model_name (str):
                 Name of the base model. Must be a supported base model.
             description (str): Description of the model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.create_acoustic_model, [WatsonReturnCodes.CREATED],
-            [name, base_model_name], {"description": description})
+            self.stt.create_acoustic_model,
+            [WatsonReturnCodes.CREATED],
+            [name, base_model_name],
+            {"description": description},
+        )
         return response
 
     def delete_custom_model(self, customization_id: str) -> bool:
         """
         Delete an existing custom acoustic model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        response= self._execute_watson_method(
-            self.stt.delete_acoustic_model, [WatsonReturnCodes.OK],
-            [customization_id])
+        response = self._execute_watson_method(
+            self.stt.delete_acoustic_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return response
 
     def train_custom_model(self, customization_id: str) -> bool:
         """
         Train a custom acoustic model with a previously added resource.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.train_acoustic_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.train_acoustic_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return response
 
     def reset_custom_model(self, customization_id: str) -> bool:
         """
         Reset a custom acoustic model to remove all loaded resources.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.reset_acoustic_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.reset_acoustic_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return response
 
-    def upgrade_custom_model(self, customization_id: str, 
-                    custom_language_model_id: str = None) -> bool:
+    def upgrade_custom_model(
+        self, customization_id: str, custom_language_model_id: str = None
+    ) -> bool:
         """
         Upgrade the base model of the custom acoustic model to its latest
         version.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
             custom_language_model_id (str):
@@ -178,61 +178,68 @@
                 model was trained with a custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
             self.stt.upgrade_acoustic_model,
-            [customization_id, custom_language_model_id])
+            [customization_id, custom_language_model_id],
+        )
         return response
 
-    
-    def get_custom_audio_resources(self, customization_id: str) \
-            -> Union[List[Dict], None]:
+    def get_custom_audio_resources(
+        self, customization_id: str
+    ) -> Union[List[Dict], None]:
         """
         List information about all audio resources of the specified custom
         acoustic model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (Union[List[Dict],None]):
                 Each internal list contains the following keys:
                 "duration","name","details","status"
                 None if unsuccessful.
         """
-        response = self._execute_watson_method(
-            self.stt.list_audio, [customization_id])
+        response = self._execute_watson_method(self.stt.list_audio, [customization_id])
         if response:
             return response["audio"]
 
-        def get_custom_audio_resource(self, customization_id: str,
-                                  audio_name: str) -> Union[Dict, None]:
+        def get_custom_audio_resource(
+            self, customization_id: str, audio_name: str
+        ) -> Union[Dict, None]:
             """
             Obtain information about a specific custom acoustic model.
 
             Args:
                 customization_id (str): Unique ID of the custom acoustic model.
                 audio_name (str): Name of the specific audio resource.
 
             Returns:
                 (Dict): Contains the following keys:
                         "duration","name","details","status"
                         None if unsuccessful
             """
             response = self._execute_watson_method(
-                self.stt.get_audio, [WatsonReturnCodes.OK],
-                [customization_id, audio_name])
+                self.stt.get_audio,
+                [WatsonReturnCodes.OK],
+                [customization_id, audio_name],
+            )
             if response:
                 return response
 
-        def add_custom_audio_resource(self, customization_id: str,
-                                  audio_name: str, audio_resource: BinaryIO, content_type: str)\
-            -> bool:
+        def add_custom_audio_resource(
+            self,
+            customization_id: str,
+            audio_name: str,
+            audio_resource: BinaryIO,
+            content_type: str,
+        ) -> bool:
             """
             Add an audio resource to the specific custom acoustic model.
 
             Args:
                 customization_id (str): Unique ID of the custom acoustic model.
                 audio_name (str): Name of the specific audio resource.
                 audio_resource (BinaryIO):
@@ -245,78 +252,89 @@
                     audio/ogg;codecs=vorbis,audio/wav,audio/webm,
                     audio/webm;codecs=opus,audio/webm;codecs=vorbis]
 
             Returns:
                 (bool): True if successful. False otherwise.
             """
             response = self._execute_watson_method(
-                self.stt.add_audio, [WatsonReturnCodes.CREATED],
-                [customization_id, audio_name, audio_resource, content_type])
+                self.stt.add_audio,
+                [WatsonReturnCodes.CREATED],
+                [customization_id, audio_name, audio_resource, content_type],
+            )
             return response
 
-    def delete_custom_audio_resource(self, customization_id: str,
-                                     audio_name: str) -> bool:
+    def delete_custom_audio_resource(
+        self, customization_id: str, audio_name: str
+    ) -> bool:
         """
         Delete the specified resource from the custom audio model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
             audio_name (str): Name of the specific audio resource.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.delete_audio, [WatsonReturnCodes.OK],
-            [customization_id, audio_name])
+            self.stt.delete_audio,
+            [WatsonReturnCodes.OK],
+            [customization_id, audio_name],
+        )
         return response
-    
+
     ## PRIVATE ##
-    
+
     def _is_api_key_valid(self, apikey: str, url: str) -> bool:
         try:
             stt = self._initialize_stt_service(apikey)
             stt.set_service_url(url)
             stt.list_models()
             return True
         except:
             return False
 
     def _initialize_stt_service(self, apikey: str) -> SpeechToTextV1:
         authenticator = IAMAuthenticator(apikey)
         stt = SpeechToTextV1(authenticator=authenticator)
         return stt
-    
-    def _execute_watson_method(self, 
-                               method: Callable,
-                               expected_response_codes: List[WatsonReturnCodes], 
-                               args: List = [],
-                               kwargs: Dict = {}) -> Union[bool, Any]:
+
+    def _execute_watson_method(
+        self,
+        method: Callable,
+        expected_response_codes: List[WatsonReturnCodes],
+        args: List = [],
+        kwargs: Dict = {},
+    ) -> Union[bool, Any]:
         """
         Execute a watson method only if connected to watson.
 
         Args:
             method (Callable): Method to execute.
             expected_response_codes (List[WatsonReturnCodes]):
                 Watson codes that are expected for a successful response.
             args (List): Arguments to pass to the method.
             kwargs (Dict): Keyword arguments to method
 
         Returns:
            (Union[bool,Any]):
-                result from watson if successful. 
+                result from watson if successful.
                 False otherwise.
         """
         if not self.connected_to_service:
             raise ERR.ConnectionError
         try:
             resp = method(*args, **kwargs)
-            if any([resp.get_status_code() == expected
-                    for expected in expected_response_codes]):
+            if any(
+                [
+                    resp.get_status_code() == expected
+                    for expected in expected_response_codes
+                ]
+            ):
                 return resp.get_result()
             raise ERR.WatsonMethodExecutionError
         except ApiException as e:
             logger.info(f"Exception raised: {e}", exc_info=e)
             return False
         except ERR.WatsonMethodExecutionError as e:
             logger.info(f"Exception raised: {e}", exc_info=e)
-            return False
+            return False
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/watson/core.py` & `GailBot-0.2a0/src/gailbot/core/engines/watson/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-09 11:25:49
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 11:59:32
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:31:43
 
 """ TODO:
 1. keyword arguments : headers, customization weight are removed 
 """
 import os 
 from typing import List, Any, Dict, Union
 from itertools import chain
@@ -127,15 +127,15 @@
             base_language_model (str) : 
                 specifies the base_language_model 
             language_customization_id (str) : 
                 ID of the custom acoustic model
             acoustic_customization_id (str) : 
                 ID of the custom language model.
         """
-        # compress the audio if it is too bog
+        # compress the audio if it is too big
         path_copy = audio_path
         logger.info("transcribe the audio file with watson STT")
         try:
             new_path = os.path.join(payload_workspace, os.path.basename(audio_path))
             audio_path = MediaHandler.convert_to_16bit_wav(audio_path, new_path)
         except Exception as e:
             logger.error(e, exc_info=e)
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/watson/lm.py` & `GailBot-0.2a0/src/gailbot/core/engines/watson/lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,147 +1,143 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-09 11:30:48
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 12:00:25
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:31:54
 
 """ TODO:
 1. only function to create and delete model are tested 
    function to train the model are not tested 
 """
 # Standard library imports
 from typing import Any, BinaryIO, List, TextIO, Tuple, Dict, Callable, Union
 from enum import IntEnum
+
 # Local imports
 
 # Third party imports
 from gailbot.configs import watson_config_loader
 from gailbot.core.engines import exception as ERR
 from ibm_watson import SpeechToTextV1, ApiException
 from ibm_cloud_sdk_core.authenticators import IAMAuthenticator
 from ibm_watson.speech_to_text_v1 import CustomWord
 
 from gailbot.core.utils.media import MediaHandler
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 from .codes import WatsonReturnCodes
 
 WATSON_CONFIG = watson_config_loader()
+
+
 class WatsonLMInterface:
-    def __init__(self, apikey : str, region : str):
+    def __init__(self, apikey: str, region: str):
         self.connected_to_service = False
         self.apikey = apikey
         self.region = region
         self.media_h = MediaHandler()
 
         # Parse confs
         self._regions = WATSON_CONFIG.regions_uris
         self._format_to_content_types = WATSON_CONFIG.format_to_content
         self._defaults = WATSON_CONFIG.defaults
         self.max_size_bytes = WATSON_CONFIG.max_file_size_bytes
 
         if not self._is_api_key_valid(apikey, self._regions[region]):
             raise Exception(f"Apikey {apikey} invalid")
         if not region in self._regions:
-            raise Exception(
-                f"Region {region} not in {list(self._regions.keys())}"
-            )
+            raise Exception(f"Region {region} not in {list(self._regions.keys())}")
 
         try:
             # Create the stt service and run
             authenticator = IAMAuthenticator(self.apikey)
             self.stt = SpeechToTextV1(authenticator=authenticator)
             self.stt.set_service_url(self._regions[self.region])
         except:
             raise Exception("Connect to STT failed")
         else:
-            self.connected_to_service = True 
-        
-    def get_base_model(self, model_name : str) -> Dict:
+            self.connected_to_service = True
+
+    def get_base_model(self, model_name: str) -> Dict:
         """
         Obtain information regarding the given base language model.
 
         Args:
             model_name (str): Name of the language model.
 
         Returns:
             (Union[Dict[str,Any],None]):
                 Dictionary with keys: name, language, rate, url,
                 supported_features, description if successful.
                 None if unsuccessful.
         """
-        if not self.connected_to_service: return {}
+        if not self.connected_to_service:
+            return {}
         resp = self._execute_watson_method(
             self.stt.get_model, [WatsonReturnCodes.OK], model_name
         )
         return resp
 
     def get_base_models(self) -> List[str]:
         """
         Obtain a list of the names of base language models that are supported.
 
         Returns:
             (List[str]): Names of the base language models.
         """
-        if not self.connected_to_service: return []
-        resp = self._execute_watson_method(
-            self.stt.list_models, [WatsonReturnCodes.OK]
-        )
+        if not self.connected_to_service:
+            return []
+        resp = self._execute_watson_method(self.stt.list_models, [WatsonReturnCodes.OK])
         return [model["name"] for model in resp["models"]] if resp != None else []
 
-    def get_custom_model(
-        self,
-        customization_id: str
-    ) -> Dict:
+    def get_custom_model(self, customization_id: str) -> Dict:
         """
         Obtain information regarding a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[Dict[str,Any],None]):
                 Mapping from the following keys to their values:
                 customization_id, CREATED, updated,language, dialect,
                 versions, owner, name, description, base_model_name, status,
                 progress
                 None if unsuccessful.
         """
-        if not self.connected_to_service: return []
+        if not self.connected_to_service:
+            return []
         resp = self._execute_watson_method(
             self.stt.get_language_model, [WatsonReturnCodes.OK], customization_id
         )
         return resp
 
     def get_custom_models(self) -> Dict[str, str]:
         """
         Get custom language models
 
         Returns:
             (Dict[str,str]):
                  Mapping from custom model name to the customization id.
         """
-        if not self.connected_to_service: return {}
+        if not self.connected_to_service:
+            return {}
         custom_models = dict()
         resp = self._execute_watson_method(
             self.stt.list_language_models, [WatsonReturnCodes.OK]
         )
         if resp != None:
             for model in resp["customizations"]:
                 custom_models[model["name"]] = model["customization_id"]
         return custom_models
 
-    def create_custom_model(
-        self,
-        name: str, 
-        base_model_name : str,
-        description : str
-    ):
+    def create_custom_model(self, name: str, base_model_name: str, description: str):
         """
         Create a new custom language model.
         Does NOT create a new model if one with the same name already exists.
 
         Args:
             name (str): Name of the model.
             base_model_name (str):
@@ -150,271 +146,254 @@
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         if not self.connected_to_service or name in self.get_custom_models().keys():
             return False
         response = self._execute_watson_method(
-            self.stt.create_language_model, [WatsonReturnCodes.CREATED],
-            [name, base_model_name], {"description": description})
+            self.stt.create_language_model,
+            [WatsonReturnCodes.CREATED],
+            [name, base_model_name],
+            {"description": description},
+        )
         return response
 
     def delete_custom_model(self, customization_id: str) -> bool:
         """
         Delete an existing custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         success = self._execute_watson_method(
-            self.stt.delete_language_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.delete_language_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return success
 
     def train_custom_model(self, customization_id: str) -> bool:
         """
         Train a custom language model with a previously added resource.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         success = self._execute_watson_method(
-            self.stt.train_language_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.train_language_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return success
-   
+
     def reset_custom_model(self, customization_id: str) -> bool:
         """
         Reset a custom language model to remove all loaded resources.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.reset_language_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.reset_language_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return response
-    
+
     def upgrade_custom_model(self, customization_id: str) -> bool:
         """
         Upgrade the base model of the custom language model to its latest
         version.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.upgrade_language_model, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.upgrade_language_model, [WatsonReturnCodes.OK], [customization_id]
+        )
         return response
-    
+
     def get_corpora(self, customization_id: str) -> Dict:
         """
         Obtain the corpora used to train this custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[List[Dict],None]):
                 Each internal dict contains the keys: name,
                 out_of_vocabulary_words,total_words, status.
                 None if unsuccessful.
         """
         response = self._execute_watson_method(
-            self.stt.list_corpora, [WatsonReturnCodes.OK], [customization_id])
+            self.stt.list_corpora, [WatsonReturnCodes.OK], [customization_id]
+        )
         if response:
             return response["corpora"]
 
     def add_corpus(
-        self,
-        customization_id: str,
-        corpus_name: str,
-        corpus_file: BinaryIO
+        self, customization_id: str, corpus_name: str, corpus_file: BinaryIO
     ) -> bool:
         """
         Add a corpus to the specified custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             corpus_name (str): Name of the corpus
             corpus_file (BinaryIO): utf-8 encoded plain text file.
         """
         response = self._execute_watson_method(
-            self.stt.add_corpus, [WatsonReturnCodes.CREATED],
-            [customization_id, corpus_name, corpus_file, True])
+            self.stt.add_corpus,
+            [WatsonReturnCodes.CREATED],
+            [customization_id, corpus_name, corpus_file, True],
+        )
         return response
 
-    def delete_corpus(
-        self,
-        customization_id: str,
-        corpus_name: str
-    ) -> bool:
+    def delete_corpus(self, customization_id: str, corpus_name: str) -> bool:
         """
         Delete a corpus from a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             corpus_name (str): Name of the corpus to delete.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.delete_corpus, 
-            [WatsonReturnCodes.OK], 
-            [customization_id, corpus_name])
+            self.stt.delete_corpus,
+            [WatsonReturnCodes.OK],
+            [customization_id, corpus_name],
+        )
         return response
 
-    def get_corpus(
-        self,
-        customization_id: str,
-        corpus_name: str
-    ) -> Dict:
+    def get_corpus(self, customization_id: str, corpus_name: str) -> Dict:
         """
         Obtain information about a specific custom corpus used to train the
         custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             corpus_name (str): Name of the corpus.
 
         Returns:
             (Union[Dict[str,Any],None]): Contains the keys: "name",
             "out_of_vocabulary_words", "total_words","status"
             None if unsuccessful.
         """
         response = self._execute_watson_method(
-            self.stt.get_corpus, [WatsonReturnCodes.OK],
-            [customization_id, corpus_name])
+            self.stt.get_corpus, [WatsonReturnCodes.OK], [customization_id, corpus_name]
+        )
         return response
-    
-    def get_custom_works(
-        self,
-        customization_id : str
-    ) -> List[Dict]:
+
+    def get_custom_works(self, customization_id: str) -> List[Dict]:
         """
         Obtain all the custom words used to train a custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[List[Dict], None]):
                 Each dictionary contains the keys: "word","sounds_like",
                 "display_as","count","source"
                 None if unsuccessful.
         """
         response = self._execute_watson_method(
-            self.stt.list_words, [WatsonReturnCodes.OK],
-            [customization_id])
+            self.stt.list_words, [WatsonReturnCodes.OK], [customization_id]
+        )
         if response:
             return response["words"]
 
-    def add_custom_works(
-        self,
-        customization_id : str,
-        words : List[str]
-    ) -> bool:
+    def add_custom_works(self, customization_id: str, words: List[str]) -> bool:
         """
         Add one or more custom words to the specified custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             words (List[str]): List of words to add to the model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         custom_words = list()
         for word in words:
             custom_words.append(CustomWord(word=word))
         response = self._execute_watson_method(
-            self.stt.add_words, [WatsonReturnCodes.CREATED],
-            [customization_id, custom_words])
+            self.stt.add_words,
+            [WatsonReturnCodes.CREATED],
+            [customization_id, custom_words],
+        )
         return response
-    
-    def delete_custom_words(
-        self,
-        customization_id : str,
-        word : str
-    ) -> bool:
+
+    def delete_custom_words(self, customization_id: str, word: str) -> bool:
         """
         Delete a word from a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             word (str): Word to delete.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.delete_word, [WatsonReturnCodes.OK],
-            [customization_id, word])
+            self.stt.delete_word, [WatsonReturnCodes.OK], [customization_id, word]
+        )
         return response
 
-    def get_custom_grammars(
-        self,
-        customization_id : str
-    ) -> List[Dict]:
+    def get_custom_grammars(self, customization_id: str) -> List[Dict]:
         """
         Obtain a list of the grammars of a custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[List[Dict], None]):
                 Internal dictionaries contain the keys:
                 out_of_vocabulary_words","name","status"
                 None of unsuccessful.
         """
         response = self._execute_watson_method(
-            self.stt.list_grammars, [customization_id])
+            self.stt.list_grammars, [customization_id]
+        )
         if response:
             return response["grammars"]
-        
-    def get_custom_grammar(
-        self,
-        customization_id: str,
-        grammar_name: str
-    ) -> Dict:
+
+    def get_custom_grammar(self, customization_id: str, grammar_name: str) -> Dict:
         """
         Obtain information about a specific grammar in a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             grammar_name (str): Name of the custom grammar.
 
         Returns:
             (Union[Dict, None]):
                 Contains the keys: "out_of_vocabulary_words","name","status"
                 None of unsuccessful.
         """
         response = self._execute_watson_method(
-            self.stt.get_grammar, [WatsonReturnCodes.OK],
-            [customization_id, grammar_name])
+            self.stt.get_grammar,
+            [WatsonReturnCodes.OK],
+            [customization_id, grammar_name],
+        )
         return response
 
     def add_custom_grammar(
         self,
         customization_id: str,
         grammar_name: str,
         grammar_file: TextIO,
-        content_type: str
+        content_type: str,
     ) -> bool:
         """
         Add a grammar to the custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             grammar_name (str): Name of the custom grammar.
@@ -422,77 +401,81 @@
             content_type (str):
                 Format of the grammar. one of:
                     application/srgs, application/srgs+xml
 
         Returns:
             (bool): True if successfully added. False otherwise.
         """
-        response  = self._execute_watson_method(
-            self.stt.add_grammar, [WatsonReturnCodes.CREATED],
-            [customization_id, grammar_name, grammar_file, content_type, True])
+        response = self._execute_watson_method(
+            self.stt.add_grammar,
+            [WatsonReturnCodes.CREATED],
+            [customization_id, grammar_name, grammar_file, content_type, True],
+        )
         return response
 
-    def delete_custom_grammar(
-        self,
-        customization_id: str,
-        grammar_name: str
-    ) -> bool:
+    def delete_custom_grammar(self, customization_id: str, grammar_name: str) -> bool:
         """
         Delete the specific grammar from a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             grammar_name (str): Name of the custom grammar.
 
         Returns:
             (bool): True if successfully added. False otherwise.
         """
         response = self._execute_watson_method(
-            self.stt.delete_grammar, [WatsonReturnCodes.OK],
-            [customization_id, grammar_name])
+            self.stt.delete_grammar,
+            [WatsonReturnCodes.OK],
+            [customization_id, grammar_name],
+        )
         return response
 
     # Others
     def _execute_watson_method(
         self,
-        method : Callable,
+        method: Callable,
         expected_response_codes: List[WatsonReturnCodes],
         args: List = [],
-        kwargs: Dict = {}
+        kwargs: Dict = {},
     ) -> Union[bool, Any]:
         """
         Execute a watson method only if connected to watson.
 
         Args:
             method (Callable): Method to execute.
             expected_response_codes (List[WatsonReturnCodes]):
                 Watson codes that are expected for a successful response.
             args (List): Arguments to pass to the method.
             kwargs (Dict): Keyword arguments to method
 
         Returns:
             (Union[bool,Any]):
-                result from watson if successful. 
+                result from watson if successful.
                 False otherwise.
         """
         if not self.connected_to_service:
             raise ERR.ConnectionError("Error raised: connection error")
         try:
             resp = method(*args, **kwargs)
-            if any([resp.get_status_code() == expected
-                        for expected in expected_response_codes]):
+            if any(
+                [
+                    resp.get_status_code() == expected
+                    for expected in expected_response_codes
+                ]
+            ):
                 return resp.get_result()
             raise ERR.WatsonMethodExecutionError
         except ApiException as e:
             logger.info(f"Exception raised: {e}", exc_info=e)
             return False
         except ERR.WatsonMethodExecutionError as e:
             logger.info(f"Exception raised: {e}", exc_info=e)
             return False
-        
+
     def _is_api_key_valid(self, apikey: str, url: str) -> bool:
         """
         Determine if the given apikey is valid.
 
         Args:
             apikey (str): API key for the watson STT service.
 
@@ -515,8 +498,8 @@
             apikey (str): Valid API key for the watson STT service.
 
         Returns:
             (SpeechToTextV1)
         """
         authenticator = IAMAuthenticator(apikey)
         stt = SpeechToTextV1(authenticator=authenticator)
-        return stt
+        return stt
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/watson/recognition_results.py` & `GailBot-0.2a0/src/gailbot/core/engines/watson/recognition_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2021-12-02 13:13:08
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2021-12-05 21:22:35
-'''
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:31:59
+"""
     The classes in this script model the RecognitionResult object as per
     the documentation for IBM Watson STT service:
     https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-basic-response
-'''
+"""
 # Standard library imports
 from typing import Dict, Any, List
 from gailbot.core.utils.logger import makelogger
 import itertools
+
 # Local imports
 # Third party imports
 
 logger = makelogger("recognition_result")
+
+
 class Alternative:
     """
     Models the smallest unit of a transcription result.
     """
 
     def __init__(self, data: Dict) -> None:
         self.items = {
             "transcript": None,
             "confidence": None,
             "timestamps": None,
-            "word_confidence": None}
+            "word_confidence": None,
+        }
         self.configured = self._parse_data(data)
 
     def is_configured(self) -> bool:
         """
         Return True if the data was successfully parsed. False otherwise.
         """
         return self.configured
@@ -64,19 +68,15 @@
 
 class SpeakerLabel:
     """
     Models a SpeakerLabel data item returned from the IBM Watson STT service.
     """
 
     def __init__(self, data: Dict) -> None:
-        self.items = {
-            "from": None,
-            "to": None,
-            "speaker": None,
-            "confidence": None}
+        self.items = {"from": None, "to": None, "speaker": None, "confidence": None}
         self.configured = self._parse_data(data)
 
     def is_configured(self) -> bool:
         """
         Return True if the data was successfully parsed. False otherwise.
         """
         return self.configured
@@ -113,15 +113,16 @@
     """
 
     def __init__(self, data: Dict) -> None:
         self.items = {
             "keywords_result": list(),
             "word_alternatives": list(),
             "alternatives": list(),
-            "final": None}
+            "final": None,
+        }
         self.configured = self._parse_data(data)
 
     def is_configured(self) -> bool:
         """
         Return True if the data was successfully parsed. False otherwise.
         """
         return self.configured
@@ -147,29 +148,27 @@
         if "final" in results:
             self.items["final"] = results["final"]
         if "keywords_result" in results.keys():
             self.items["keywords_result"] = results["keywords_result"]
         if "word_alternatives" in results.keys():
             self.items["word_alternatives"] = results["word_alternatives"]
         if "alternatives" in results.keys():
-            self.items["alternatives"] = \
-                [Alternative(alt) for alt in results["alternatives"]]
+            self.items["alternatives"] = [
+                Alternative(alt) for alt in results["alternatives"]
+            ]
 
 
 class RecognitionResult:
     """
     Main class that models an entire RecognitionResult object that is returned
     from the IBM Watson STT service.
     """
 
     def __init__(self, watson_data: Dict) -> None:
-        self.items = {
-            "result_index": None,
-            "results": None,
-            "speaker_labels": None}
+        self.items = {"result_index": None, "results": None, "speaker_labels": None}
         self.configured = self._parse_data(watson_data)
 
     def is_configured(self) -> bool:
         """
         Return True if the data was successfully parsed. False otherwise.
         """
         return self.configured
@@ -211,21 +210,24 @@
                 List of dictionaries modeling SpeakerLabel objects.
                 Each dictionary has the keys: 'from', 'to', 'speaker',
                 'confidence'.
         """
         labels = list()
         if not self.items or not self.items["speaker_labels"]:
             return labels
-        
+
         for label in self.items["speaker_labels"]:
-            labels.append({
-                "start_time": label.get("from"),
-                "end_time": label.get("to"),
-                "speaker": label.get("speaker"),
-                "label_confidence": label.get("confidence")})
+            labels.append(
+                {
+                    "start_time": label.get("from"),
+                    "end_time": label.get("to"),
+                    "speaker": label.get("speaker"),
+                    "label_confidence": label.get("confidence"),
+                }
+            )
         return labels
 
     def get_keywords_results(self, only_final: bool = True) -> List[Any]:
         """
         Obtain a list of 'keyword_result' objects received from the IBM
         STT service.
 
@@ -234,16 +236,15 @@
                 True to obtain 'keyword_result' only from results that are
                 considered final and not interim. False to include all results,
                 both final and interim.
 
         Returns:
             (List[Any]): List of 'keyword_result' objects.
         """
-        return self._aggregate(
-            self.items["results"], "keywords_result", only_final)
+        return self._aggregate(self.items["results"], "keywords_result", only_final)
 
     def get_word_alternatives(self, only_final: bool = True) -> Any:
         """
         Obtain a list of 'word_alternative' objects received from the IBM
         STT service.
 
         Args:
@@ -251,19 +252,17 @@
                 True to obtain 'word_alternative' only from results that are
                 considered final and not interim. False to include all results,
                 both final and interim.
 
         Returns:
             (List[Any]): List of 'word_alternative' objects.
         """
-        return self._aggregate(
-            self.items["results"], "word_alternatives", only_final)
+        return self._aggregate(self.items["results"], "word_alternatives", only_final)
 
-    def get_transcript_from_alternatives(self, only_final: bool = True) \
-            -> List[str]:
+    def get_transcript_from_alternatives(self, only_final: bool = True) -> List[str]:
         """
         Obtain a list containing all 'transcript' items from all Alternative
         received as part of the IBM STT result.
 
         Args:
             only_final (bool):
                 True to obtain items only from results that are
@@ -271,19 +270,21 @@
                 both final and interim.
 
         Returns:
             (List[str]):
                 List of 'transcript' items for all Alternative objects.
         """
         alternatives = self._aggregate(
-            self.items["results"], "alternatives", only_final)[0]
+            self.items["results"], "alternatives", only_final
+        )[0]
         return [alternative.get("transcript") for alternative in alternatives]
 
-    def get_transcript_confidences_from_alternatives(self,
-                                                     only_final: bool = True) -> List[float]:
+    def get_transcript_confidences_from_alternatives(
+        self, only_final: bool = True
+    ) -> List[float]:
         """
         Obtain a list containing all 'transcript_confidence' objects from all
         Alternative received as part of the IBM STT result.
 
         Args:
             only_final (bool):
                 True to obtain items only from results that are
@@ -291,20 +292,22 @@
                 both final and interim.
 
         Returns:
             (List[float]):
                 List contianing confidence for each transcript obtained.
         """
         alternatives = self._aggregate(
-            self.items["results"], "alternatives", only_final)[0]
+            self.items["results"], "alternatives", only_final
+        )[0]
 
         return [alternative.get("confidence") for alternative in alternatives]
 
-    def get_timestamps_from_alternatives(self, only_final: bool = True) \
-            -> List[List[List[Any]]]:
+    def get_timestamps_from_alternatives(
+        self, only_final: bool = True
+    ) -> List[List[List[Any]]]:
         """
         Obtain a list containing all 'timestamps' objects from all
         Alternative received as part of the IBM STT result.
 
         Args:
             only_final (bool):
                 True to obtain items only from results that are
@@ -314,22 +317,21 @@
         Returns:
             (List[List[List[Any]]]):
                 One main list continaing lists, with each inner most list
                 representing one result of the form:
                 ['text', 'start time', 'end time']
         """
         alternatives = self._aggregate(
-            self.items["results"], "alternatives", only_final)
+            self.items["results"], "alternatives", only_final
+        )
         alternatives = list(itertools.chain(*alternatives))
-        timestamps = [alternative.get("timestamps")
-                      for alternative in alternatives]
+        timestamps = [alternative.get("timestamps") for alternative in alternatives]
         return [timestamp for timestamp in timestamps if timestamp != None]
 
-    def get_word_confidences_from_alternatives(self, only_final: bool = True) \
-            -> List:
+    def get_word_confidences_from_alternatives(self, only_final: bool = True) -> List:
         """
         Obtain a list containing all 'word_confidence' objects from all
         Alternative received as part of the IBM STT result.
 
         Args:
             only_final (bool):
                 True to obtain items only from results that are
@@ -339,17 +341,17 @@
         Returns:
             (List[List[List[Any]]]):
                 One main list continaing lists, with each inner most list
                 representing one result of the form:
                 ['text', 'confidence']
         """
         alternatives = self._aggregate(
-            self.items["results"], "alternatives", only_final)[0]
-        return [alternative.get("word_confidence")
-                for alternative in alternatives]
+            self.items["results"], "alternatives", only_final
+        )[0]
+        return [alternative.get("word_confidence") for alternative in alternatives]
 
     ############################### PRIVATE METHODS ##########################
 
     def _parse_data(self, watson_data: Dict) -> bool:
         """
         Parse a single RecognitionResult dictionary obtained from the IBM
         STT service.
@@ -374,18 +376,18 @@
                 results_array = list()
                 for results in watson_data["results"]:
                     results_array.append(Result({"results": results}))
                 self.items["results"] = results_array
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
-            
-            
-    def _aggregate(self, results: List[Result], aggregation_key: str,
-                   only_final: bool) -> List[Any]:
+
+    def _aggregate(
+        self, results: List[Result], aggregation_key: str, only_final: bool
+    ) -> List[Any]:
         """
         Aggregate the results from a list of Result objects, based on the
         aggregation key. If only_final = True, only use the results of
         Result objects considered final.
         """
         response = list()
         for item in results:
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/watson/recognize_callback.py` & `GailBot-0.2a0/src/gailbot/core/engines/watson/recognize_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2021-12-02 13:13:08
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 11:53:04
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:32:04
 # Standard imports
 from typing import Callable, Any, List, Dict
 import sys
+
 # Local imports
 # Third party imports
 from copy import deepcopy
 from ibm_watson.websocket import RecognizeCallback
 from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("callback")
 
+
 class WatsonException(Exception):
     def __init__(self, msg: str) -> None:
         super().__init__(msg)
-        self.msg = msg 
-    
+        self.msg = msg
+
+
 class CustomWatsonCallbacks(RecognizeCallback):
     """
     Extends the watson callback class to allow custom callbacks to be executed
     when an event occurs through the lifecycle of the websocket connection.
 
     Inherits:
         (RecognizeCallback)
     """
+
     def __init__(self) -> None:
         """
         Args:
             closure (List):
                 User object that is passed as the first parameter of every
                 callback during the lifecycle of the websocket connection.
         """
@@ -60,45 +64,45 @@
         """
         Called when a Websocket connection was made
         """
         logger.info("connected to watson")
         try:
             closure = self.closure
             closure["callback_status"]["on_connected"] = True
-        except Exception as e:            
-           logger.error(e, exc_info=e) 
-    
+        except Exception as e:
+            logger.error(e, exc_info=e)
+
     def on_error(self, error: str) -> None:
         """
         Called when there is an error in the Websocket connection.
         """
         logger.error(f"get error {error}", exc_info=error)
 
         closure = self.closure
         closure["callback_status"]["on_error"] = True
         closure["results"]["error"] = error
         raise WatsonException(error)
 
     def on_inactivity_timeout(self, error: str) -> None:
         """
         Called when there is an inactivity timeout.
-        """      
-        logger.info("inactivity time out") 
+        """
+        logger.info("inactivity time out")
         try:
             closure = self.closure
             closure["callback_status"]["on_inactivity_timeout"] = True
             closure["results"]["error"] = error
         except Exception as e:
             logger.error(f"timeout error {e}", exc_info=e)
 
     def on_listening(self) -> None:
         """
         Called when the service is listening for audio.
-        """   
-        logger.info("watson is listening")   
+        """
+        logger.info("watson is listening")
         try:
             closure = self.closure
             closure["callback_status"]["on_listening"] = True
         except Exception as e:
             logger.error(f"on listening error {e}", exc_info=e)
 
     def on_hypothesis(self, hypothesis: str) -> None:
@@ -131,26 +135,26 @@
         logger.info("on close")
         try:
             closure = self.closure
             closure["callback_status"]["on_close"] = True
         except Exception as e:
             logger.error(f"on close error {e}", exc_info=e)
 
-    def _init_closure(self) -> Dict:      
-        return  {
-                "callback_status": {
-                    "on_transcription": False,
-                    "on_connected": False,
-                    "on_error": False,
-                    "on_inactivity_timeout": False,
-                    "on_listening": False,
-                    "on_hypothesis": False,
-                    "on_data": False,
-                    "on_close": False
-                },
-                "results": {
-                    "error": None,
-                    "transcript": list(),
-                    "hypothesis": list(),
-                    "data": list()
-                }
-            }
+    def _init_closure(self) -> Dict:
+        return {
+            "callback_status": {
+                "on_transcription": False,
+                "on_connected": False,
+                "on_error": False,
+                "on_inactivity_timeout": False,
+                "on_listening": False,
+                "on_hypothesis": False,
+                "on_data": False,
+                "on_close": False,
+            },
+            "results": {
+                "error": None,
+                "transcript": list(),
+                "hypothesis": list(),
+                "data": list(),
+            },
+        }
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/watson/watson.py` & `GailBot-0.2a0/src/gailbot/core/engines/watson/watson.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 12:43:29
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-03-15 11:33:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:32:12
 import os
 from typing import Dict, Any, List
 from itertools import chain
 
 from .recognition_results import RecognitionResult
 from .recognize_callback import CustomWatsonCallbacks
 from .core import WatsonCore
 from .lm import WatsonLMInterface
 from .am import WatsonAMInterface
 from ..engine import Engine
 from gailbot.core.engines import exception as ERR
 from gailbot.configs import watson_config_loader
 from gailbot.core.utils.logger import makelogger
+
 WATSON_CONFIG = watson_config_loader()
 
 
 logger = makelogger("watson")
+
+
 class Watson(Engine):
     """
     An Engine that connect to IBM Watson STT, provide function to transcribe
     audio file with IBM Watson STT
 
     Inheritance:
         Engine
     """
+
     def __init__(
         self,
-        apikey : str,
-        region : str,
+        apikey: str,
+        region: str,
     ):
-        """ constructor for IBM Watson STT engine
+        """constructor for IBM Watson STT engine
 
         Args:
             apikey (str): User API key to Watson STT service.
             region (str): User API region. Must be in supported regions.
         """
         self.apikey = apikey
         self.region = region
         # NOTE: Exception raised if not connected to the service.
-        self.core = WatsonCore(apikey, region )
-        self.lm = WatsonLMInterface(apikey ,region)
+        self.core = WatsonCore(apikey, region)
+        self.lm = WatsonLMInterface(apikey, region)
         self.am = WatsonAMInterface(apikey, region)
         self.is_transcribe_success = False
 
     def __str__(self):
         return WATSON_CONFIG.name
 
     def __repr__(self):
         """Returns all the configurations and additional metadata"""
         return self.core.__repr__()
 
-    @staticmethod 
+    @staticmethod
     def valid_init_kwargs(apikey: str, region: str):
         return WatsonCore.valid_region_api(apikey, region)
 
     @property
     def supported_formats(self) -> List[str]:
         """
         a list of supported format that can be transcribe with the STT engine
@@ -76,22 +80,21 @@
     def defaults(self) -> Dict:
         """
         a dictionary that contains the default settings that will be
         applied to the IBM Watson STT engine
         """
         return self.core.defaults
 
-    
     def transcribe(
         self,
-        audio_path : str,
-        payload_workspace: str, 
-        base_model : str,
-        language_customization_id : str = "",
-        acoustic_customization_id : str = ""
+        audio_path: str,
+        payload_workspace: str,
+        base_model: str,
+        language_customization_id: str = "",
+        acoustic_customization_id: str = "",
     ) -> List[Dict[str, str]]:
         """Use the engine to transcribe an item
 
         Args:
         audio_path: str
             a path to the audio file that will be transcribed
         output_directory: str
@@ -110,31 +113,32 @@
         """
         try:
             utterances = self.core.transcribe(
                 audio_path,
                 payload_workspace,
                 base_model,
                 language_customization_id,
-                acoustic_customization_id)
+                acoustic_customization_id,
+            )
             self.is_transcribe_success = True
             return utterances
         except Exception as e:
             logger.error(e, exc_info=e)
-            raise ERR.TranscriptionError(error = e)
+            raise ERR.TranscriptionError(error=e)
 
     def language_customization_interface(self) -> WatsonLMInterface:
-        """ return the watson customized language model interface """
+        """return the watson customized language model interface"""
         return self.lm
 
     def acoustic_customization_interface(self) -> WatsonAMInterface:
-        """ return the watson customized acoustic model interface """
+        """return the watson customized acoustic model interface"""
         return self.am
 
     def get_engine_name(self) -> str:
-        """ return  the name of the watson engine"""
+        """return  the name of the watson engine"""
         return "watson"
 
     def get_supported_formats(self) -> List[str]:
         """
         return a list of supported format that can be
         transcribe with the STT engine
         """
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/core.py` & `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,168 +1,159 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-31 11:09:26
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-03-15 11:43:23
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:32:35
 
 
 import os
 from threading import Lock
 import json
 from typing import List, Dict, Any
 from dataclasses import asdict
 
 import torch
-import gailbot.core.engines.whisperEngine.whisperTimestamped as whisper
-from gailbot.core.engines.whisperEngine.whisperTimestamped.utils import (
-    force_cudnn_initialization
-)
+import whisper_timestamped as whisper
+from whisper_timestamped.transcribe import force_cudnn_initialization
 
-from .diarization.diarize import PyannoteDiarizer
 from .parsers import (
     parse_into_full_text,
     parse_into_word_dicts,
-    add_speaker_info_to_text
+    add_speaker_info_to_text,
 )
 
 from .parsers import parse_into_word_dicts
-from gailbot.configs import  whisper_config_loader, workspace_config_loader
-from gailbot.core.utils.general import (
-    is_file,
-    make_dir
-)
+from gailbot.configs import whisper_config_loader, workspace_config_loader
+from gailbot.core.utils.general import is_file, make_dir
 from gailbot.configs import whisper_config_loader
 from gailbot.core.utils.logger import makelogger
+
 logger = makelogger("whisper")
 
 WHISPER_CONFIG = whisper_config_loader()
 LOAD_MODEL_LOCK = Lock()
 
+
 class WhisperCore:
     """
     We are using this class as an adapter for the engine so that we can use
     multiple different instances of the underlying whisper package is required.
     """
 
     # NOTE: Intentionally limiting the supported formats since we have
     # not tested other formats.
     # TODO: I'm not sure if this is the best place to define the supported
     # formats.
-    _SUPPORTED_FORMATS = ("wav")
+    _SUPPORTED_FORMATS = "wav"
 
     def __init__(self):
         # initialize the workspace
         self.workspace_dir = workspace_config_loader().engine_ws.whisper
         logger.info(f"Whisper workspace path: {self.workspace_dir}")
-        self.cache_dir = os.path.join(self.workspace_dir,"cache")
-        self.models_dir = os.path.join(self.cache_dir,"models")
+        self.cache_dir = os.path.join(self.workspace_dir, "cache")
+        self.models_dir = os.path.join(self.cache_dir, "models")
         self.loadModelLock = Lock()
-        make_dir(self.workspace_dir,overwrite=False)
-        make_dir(self.cache_dir,overwrite=False)
-        make_dir(self.models_dir,overwrite=False)
+        make_dir(self.workspace_dir, overwrite=False)
+        make_dir(self.cache_dir, overwrite=False)
+        make_dir(self.models_dir, overwrite=False)
 
         # Load a GPU is it is available
         self.device = "cuda:0" if torch.cuda.is_available() else "cpu"
         if self.device.lower().startswith("cuda"):
             force_cudnn_initialization(self.device)
         logger.info(f"Whisper core initialized with device: {self.device}")
 
-
     def __repr__(self) -> str:
         configs = json.dumps(
-            asdict(WHISPER_CONFIG.transcribe_configs),
-            indent = 2, ensure_ascii = False
+            asdict(WHISPER_CONFIG.transcribe_configs), indent=2, ensure_ascii=False
         )
         return (
-            f"Whisper model: {WHISPER_CONFIG.model_name}" \
+            f"Whisper model: {WHISPER_CONFIG.model_name}"
             f"Transcribe configs:\n{configs}"
         )
 
-
     def transcribe(
-        self,
-        audio_path : str,
-        language : str = None,
-        detect_speaker : bool = False
+        self, audio_path: str, language: str = None, detect_speaker: bool = False
     ) -> List[Dict]:
         assert is_file(audio_path), f"ERROR: Invalid file path: {audio_path}"
-        
+
         # Load the model
         logger.info(f"start to load whisper model")
-        
+
         global LOAD_MODEL_LOCK
         with LOAD_MODEL_LOCK:
             whisper_model = whisper.load_model(
                 name=WHISPER_CONFIG.model_name,
                 device=self.device,
-                download_root=self.models_dir
+                download_root=self.models_dir,
             )
         logger.info(f"Whisper core using whisper model: {WHISPER_CONFIG.model_name}")
 
         # Load the diarization pipeline
-        diarization_pipeline = PyannoteDiarizer(self.models_dir)
+        # diarization_pipeline = PyannoteDiarizer(self.models_dir)
         logger.info("get the diarazation pipleine")
-        logger.info(f"received setting language: {language}, detect speaker {detect_speaker} audio_path {audio_path}")
-         
-        if language != None and not language in self.get_supported_languages():
-            raise Exception(
-                f"Unsupported language, must be one of: {self.get_supported_languages()}"
-            )
+        logger.info(
+            f"received setting language: {language}, detect speaker {detect_speaker} audio_path {audio_path}"
+        )
+
+        # if language != None and not language in self.get_supported_languages():
+        #     raise Exception(
+        #         f"Unsupported language, must be one of: {self.get_supported_languages()}"
+        #     )
 
         if language == None:
             logger.info("No language specified - auto detecting language")
 
         # Load the audio and models, transcribe, and return the parsed result
         logger.info("prepare to load audio")
         audio = whisper.load_audio(audio_path)
         logger.info("audio loaded")
 
         asr_result = whisper.transcribe(
             whisper_model,
             audio,
             language=language,
-            **asdict(WHISPER_CONFIG.transcribe_configs)
+            **asdict(WHISPER_CONFIG.transcribe_configs),
         )
 
         if WHISPER_CONFIG.transcribe_configs.verbose:
             logger.debug(parse_into_full_text(asr_result))
 
-        # Apply speaker diarization
-        if detect_speaker:
-            if self.device == "cpu":
-                logger.warning(
-                    f"Performing speaker diarization on {self.device} may take upto 10x "\
-                    f"the duration of the audio"
-                )
-            logger.info("Performing speaker diarization")
-            
-            try:
-                dir_result = diarization_pipeline(audio_path)
-                # Create and return results
-                res = add_speaker_info_to_text(asr_result, dir_result)
-                logger.info("get the result from parsed dict with speaker")
-                return res 
-            except ValueError as e:
-                logger.warn(e, exc_info=e)
-                return []
-        else:
-            res = parse_into_word_dicts(asr_result)
-            logger.info("get the result from parse")
-            return res  
+        res = parse_into_word_dicts(asr_result)
+        logger.info("get the result from parse")
+        return res
+
+        # # Apply speaker diarization
+        # # TODO: remove this part until line 151
+        # if detect_speaker:
+        #     if self.device == "cpu":
+        #         logger.warning(
+        #             f"Performing speaker diarization on {self.device} may take upto 10x "
+        #             f"the duration of the audio"
+        #         )
+        #     logger.info("Performing speaker diarization")
+
+        #     try:
+        #         dir_result = diarization_pipeline(audio_path)
+        #         # Create and return results
+        #         res = add_speaker_info_to_text(asr_result, dir_result)
+        #         logger.info("get the result from parsed dict with speaker")
+        #         return res
+        #     except ValueError as e:
+        #         logger.warn(e, exc_info=e)
+        #         return []
+        # else:
+        #     res = parse_into_word_dicts(asr_result)
+        #     logger.info("get the result from parse")
+        #     return res
 
     def get_supported_formats(self) -> List[str]:
         return list(self._SUPPORTED_FORMATS)
 
     def get_available_models(self) -> List[str]:
         return whisper.available_models()
 
-    def get_supported_languages(self) -> List[str]:
-        return whisper.supported_languages()
-
+    # def get_supported_languages(self) -> List[str]:
+    #     # return whisper.supported_languages()
+    #     return whisper.utils.supported_languages()
 
     ################ PRIVATE METHODS
-
-
-
-
-
-
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/utils.py` & `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/utils.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/parsers.py` & `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-31 16:53:33
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-02-07 17:57:45
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-04 14:56:15
 
 import sys
 import os
 import json
 from typing import Dict, List, Any, Tuple
+
 from pyannote.core import Segment
 from gailbot.core.utils.logger import makelogger
+
 _DEFAULT_SPEAKER = 0
 logger = makelogger("parsers")
-def parse_into_word_dicts(transcription : Dict) -> List[Dict]:
+
+
+def parse_into_word_dicts(transcription: Dict) -> List[Dict]:
     """
     Parse the results of the transcription into a list of dictionaries
     containing the speaker, start time, end time, and text.
 
     Format of the transcription is detailed here: https://github.com/linto-ai/whisper-timestamped
     """
     logger.info("parse into word dict")
@@ -24,61 +28,63 @@
     segments = transcription["segments"]
     try:
         for segment in segments:
             if not "words" in segment:
                 continue
             word_list = segment["words"]
             for item in word_list:
-                parsed.append({
-                    "start" : item["start"],
-                    "end" : item["end"],
-                    "text" : item["text"],
-                    # NOTE: Whisper does not generate speaker but I can
-                    # potentially add that in too.
-                    "speaker" : str(_DEFAULT_SPEAKER)
-                })
+                parsed.append(
+                    {
+                        "start": item["start"],
+                        "end": item["end"],
+                        "text": item["text"],
+                        # NOTE: Whisper does not generate speaker but I can
+                        # potentially add that in too.
+                        "speaker": str(_DEFAULT_SPEAKER),
+                    }
+                )
                 assert parsed
         logger.info("get the segment in to parsed dict")
     except Exception as e:
         logger.error(f"get the error from parsing word into dict", exc_info=e)
     return parsed
 
-def parse_into_timestamped_text(asr_res : Dict) -> List[Tuple]:
+
+def parse_into_timestamped_text(asr_res: Dict) -> List[Tuple]:
     """
     Parse results from whisper timestamped in terms of Segment
     """
     logger.info("parse to timestamp data ")
     timestamp_texts = []
-    for segment in asr_res['segments']:
+    for segment in asr_res["segments"]:
         if not "words" in segment:
             continue
         word_list = segment["words"]
         for item in word_list:
-            start = item['start']
-            end = item['end']
-            text = item['text']
+            start = item["start"]
+            end = item["end"]
+            text = item["text"]
             timestamp_texts.append((Segment(start, end), text))
     return timestamp_texts
 
-def parse_into_full_text(asr_res : Dict) -> str:
+
+def parse_into_full_text(asr_res: Dict) -> str:
     """
     Parse the transcription output into a string.
     """
     return asr_res["text"]
 
-def add_speaker_info_to_text(asr_res : Dict, dir_res : Dict) -> Dict:
+
+def add_speaker_info_to_text(asr_res: Dict, dir_res: Dict) -> Dict:
     """
     Add speaker information to transcription results using speaker
     diarization results. Returns dictionaries
     """
     logger.info("adding speaker tag into the result")
     spk_text = []
     timestamp_texts = parse_into_timestamped_text(asr_res)
     for seg, text in timestamp_texts:
         spk = dir_res.crop(seg).argmax()
-        spk_text.append({
-            "start" : seg.start,
-            "end" : seg.end,
-            "speaker" : spk,
-            "text" : text
-        })
+        spk_text.append(
+            {"start": seg.start, "end": seg.end, "speaker": spk, "text": text}
+        )
     return spk_text
```

### Comparing `GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperEngine.py` & `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/whisperEngine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 12:43:29
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-03-15 12:01:39
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:32:48
 
 from typing import Dict, Any, List
 import torch
 import multiprocessing
 from ..engine import Engine
 from .core import WhisperCore
-from gailbot.core.utils.general import (
-    get_extension
-)
-from gailbot.configs import  whisper_config_loader
+from gailbot.core.utils.general import get_extension
+from gailbot.configs import whisper_config_loader
 from gailbot.core.utils.logger import makelogger
+
 logger = makelogger("Whisper Engine")
 
 WHISPER_CONFIG = whisper_config_loader()
 
-class WhisperEngine(Engine):
 
+class WhisperEngine(Engine):
     def __init__(self):
         self.core = WhisperCore()
         self._successful = False
 
     def __str__(self):
         """Returns the name of the function"""
         return WHISPER_CONFIG.engine_name
@@ -32,18 +31,18 @@
         """Returns all the configurations and additional metadata"""
         return self.core.__repr__()
 
     #### Engine API Methods
 
     def transcribe(
         self,
-        audio_path : str,
-        payload_workspace : str,
-        language : str = None,
-        detect_speakers : bool = False,
+        audio_path: str,
+        payload_workspace: str,
+        language: str = None,
+        detect_speakers: bool = False,
     ) -> List[Dict]:
         """Use the engine to transcribe an item"""
         results = self.core.transcribe(audio_path, language, detect_speakers)
         self._successful = True
         return results
 
     def was_transcription_successful(self) -> bool:
@@ -66,15 +65,10 @@
         Determine if the given file is supported by the engine.
         """
         return get_extension(filepath) in self.get_supported_formats()
 
     #### Additional methods
 
     def get_available_models(self) -> List[str]:
-        """return the list of available model
-        """
+        """return the list of available model"""
         return self.core.get_available_models()
 
-    def get_supported_languages(self) -> List[str]:
-        """ return the list of available languages 
-        """
-        return self.core.get_supported_languages()
```

### Comparing `GailBot-0.1a9/src/gailbot/core/pipeline/component.py` & `GailBot-0.2a0/src/gailbot/core/pipeline/component.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/core/pipeline/pipeline.py` & `GailBot-0.2a0/src/gailbot/core/pipeline/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,226 +1,223 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 12:52:37
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-15 16:04:52
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:33:12
 from typing import List, Dict, Any
 from dataclasses import dataclass
 
 from .component import Component, ComponentState, ComponentResult
 from gailbot.core.utils.threads import ThreadPool
 from gailbot.core.utils.logger import makelogger
 
 import networkx as nx
 
 Failure = ComponentResult(ComponentState.FAILED, None, 0)
 logger = makelogger("pipeline")
+
+
 @dataclass
 class DataStream:
-    data : Any = None
-    
+    data: Any = None
+
+
 class Pipeline:
     """
     Defines a class for the pipeline that runs the dependency map.
     """
+
     def __init__(
         self,
-        dependency_map : Dict[str, List[str]],
-        components : Dict[str, Component],
-        num_threads: int 
+        dependency_map: Dict[str, List[str]],
+        components: Dict[str, Component],
+        num_threads: int,
     ):
         """
         Dependency map describes the execution order.
         """
         self.dependency_map = dependency_map
         self.components = components
         self.threadpool = ThreadPool(num_threads)
-        self._generate_dependency_graph(
-            dependency_map, components
-        )
-    
+        self._generate_dependency_graph(dependency_map, components)
+
     def __repr__(self) -> str:
         """
         Accesses the pipeline's dependency graph.
 
         Args:
             self
-        
+
         Returns:
             String representation of the pipeline's dependency graph.d
         """
         return str(self.get_dependency_graph())
 
     def __call__(
         self,
-        base_input : Any,
-        additional_component_kwargs : Dict = dict()
+        base_input: Any,
+        additional_component_kwargs: Dict = dict()
         # NOTE: base_input is passed only to the first component.
     ) -> Dict[str, ComponentState]:
         """
         Execute the pipeline by running all components in order of the dependency
         graph. This wraps data as DataStream before passing it b/w components.
-        Additionally, each component receives the output of its dependencies. 
+        Additionally, each component receives the output of its dependencies.
 
         Args:
-            base_input: 
-                a list of input arguments that will be passed to the first 
-                component of the graph 
-                
-            Additional_component_kwargs: 
+            base_input:
+                a list of input arguments that will be passed to the first
+                component of the graph
+
+            Additional_component_kwargs:
                 passed as a dereferenced dictionary to each component.
 
         Returns:
-            Dictionary containing keys mapping to the component states 
+            Dictionary containing keys mapping to the component states
             corresponding to the result of each task.
-            
-        Note: 
+
+        Note:
             each component is contained in a Component class
         """
         successors = self.get_dependency_graph()
-        logger.info(successors) 
+        logger.info(successors)
         logger.info(self.dependency_graph)
         logger.info(self.components)
-        
-        name_to_results : Dict[str, ComponentResult] = dict()   # map component name to result
-       
+
+        name_to_results: Dict[
+            str, ComponentResult
+        ] = dict()  # map component name to result
+
         while True:
-            # executables is a list of Component who currently has no dependent node 
+            # executables is a list of Component who currently has no dependent node
             executables: List[Component] = [
                 c for c, d in self.dependency_graph.in_degree if d == 0
             ]
-            
+            # NOTE: bug fix from July 3rd 2023
+            threadkey_to_exe: Dict[
+                str, Component
+            ] = dict()  # map thread key to executable
+
             # exit the loop if no nodes left.
             if len(executables) == 0:
                 break
-            
+
             for executable in executables:
-                threadkey_to_exe: Dict[str, Component] = dict()       # map thread key to executable
                 exe_name: str = self.component_to_name[executable]
                 dependency_resolved = True
-                
-                # check the result output of exe_name's dependency component 
+
+                # check the result output of exe_name's dependency component
                 if len(successors[exe_name]) > 0:
-                    dep_outputs : Dict[str, ComponentResult] = {
-                        k : name_to_results[k] for k in successors[exe_name]
+                    dep_outputs: Dict[str, ComponentResult] = {
+                        k: name_to_results[k] for k in successors[exe_name]
                     }
                 else:
                     dep_outputs = {
-                        "base" : ComponentResult(
-                            state=ComponentState.SUCCESS,
-                            result=base_input,
-                            runtime=0
+                        "base": ComponentResult(
+                            state=ComponentState.SUCCESS, result=base_input, runtime=0
                         )
                     }
-                    
+
                 for res in dep_outputs.values():
                     if res.state == ComponentState.FAILED:
                         name_to_results[exe_name] = Failure
                         if self.dependency_graph.has_node(executable):
                             self.dependency_graph.remove_node(executable)
                         dependency_resolved = False
- 
-                args = [dep_outputs]          
-                              
-                if dependency_resolved:                    
+
+                args = [dep_outputs]
+
+                if dependency_resolved:
                     key = self.threadpool.add_task(
-                        executable, 
-                        args = args, 
-                        kwargs = additional_component_kwargs) 
+                        executable, args=args, kwargs=additional_component_kwargs
+                    )
                     logger.info(f" the component {executable} get the thread key {key}")
-                    threadkey_to_exe[key] = executable           
+                    threadkey_to_exe[key] = executable
 
             # wait until all tasks finishes before next iteration
-            # self.threadpool.wait_for_all_completion(error_fun=lambda:None)
-            
+            self.threadpool.wait_for_all_completion(error_fun=lambda: None)
+
             for key, exe in threadkey_to_exe.items():
                 # get the task result from the thread pool
-                logger.info(key)
-                logger.info(exe)
                 exe_res = self.threadpool.get_task_result(key)
                 self.dependency_graph.remove_node(exe)
                 name = self.component_to_name[exe]
-               
+
                 if exe_res and exe_res.state == ComponentState.SUCCESS:
                     # add to result if success
                     name_to_results[name] = exe_res
                 else:
                     # add the failed result on failure
                     name_to_results[name] = Failure
-        
-                 
+
         # Regenerate graph
-        self._generate_dependency_graph(
-            self.dependency_map, self.components
-        )
+        self._generate_dependency_graph(self.dependency_map, self.components)
 
-        return {
-            k : v.state for k, v in name_to_results.items()
-        }
+        return {k: v.state for k, v in name_to_results.items()}
 
     def component_names(self) -> List[str]:
         """
         Gets names of all components in the dependency map.
-        
+
         Args:
             self
-        
+
         Returns:
             List of strings containing components.
         """
         return list(self.name_to_component.keys())
 
-    def is_component(self, name : str) -> bool:
+    def is_component(self, name: str) -> bool:
         return name in self.component_names()
 
-    def component_parents(self, name : str) -> List[str]:
+    def component_parents(self, name: str) -> List[str]:
         """
         Get the component(s) that the given component is dependent on.
 
         Args:
             name: string containing the name of the child component.
 
         Returns:
-            List of strings of the names of the given component's parent 
+            List of strings of the names of the given component's parent
             components.
 
-            Raises exception if the given name doesn't correspond to an 
+            Raises exception if the given name doesn't correspond to an
             existing component.
         """
         if not self.is_component(name):
             raise Exception(f"No component named {name}")
         edges = list(self.dependency_graph.in_edges(self.name_to_component[name]))
         return [self.component_to_name[e[0]] for e in edges]
 
-    def component_children(self, name : str) -> List[str]:
+    def component_children(self, name: str) -> List[str]:
         """
         Gets component(s) that are dependent on the given component.
 
         Args:
             name: string containing the name of the child component.
 
         Returns:
-            List of strings of the names of components that are dependent on the 
+            List of strings of the names of components that are dependent on the
             given component.
 
-            Raises exception if the given name doesn't correspond to an 
+            Raises exception if the given name doesn't correspond to an
             existing component.
         """
         if not self.is_component(name):
             raise Exception(f"No component named {name}")
         edges = list(self.dependency_graph.out_edges(self.name_to_component[name]))
         return [self.component_to_name[e[1]] for e in edges]
 
     def get_dependency_graph(self) -> Dict:
         """
         Returns a map from each component to the components it is dependent on.
 
         Args:
             self
-        
+
         Returns:
             Dictionary mapping the given component to the components it is dependent upon.
         """
         view = dict()
         for name in self.name_to_component:
             view[name] = self.component_parents(name)
         return view
@@ -231,84 +228,74 @@
 
     def _does_cycle_exist(self, graph: nx.Graph) -> bool:
         """
         Determines if there are existing cycles in the given graph.
 
         Args:
             graph: graph in which to determine if there are cycles.
-        
+
         Returns:
             True if there are any cycles in the given graph, false if not.
         """
         try:
             nx.find_cycle(graph, orientation="original")
             return True
         except:
             return False
 
     def _generate_dependency_graph(
-        self,
-        dependency_map : Dict[str, List[str]],
-        components : Dict[str, Component]
+        self, dependency_map: Dict[str, List[str]], components: Dict[str, Component]
     ) -> None:
         """
         Generates a dependency graph containing components from a given dictionary.
-        Assumes that the dependency_map keys are in order i.e, a component will 
+        Assumes that the dependency_map keys are in order i.e, a component will
         be seen as a key before it is seen as a dependency.
 
         Args:
             dependency_map: dictionary containing lists of strings to map between.
-            components: dictionary containing components to insert into the newly 
+            components: dictionary containing components to insert into the newly
                 created dependency graph.
 
         Returns:
             A graph of components mapping from the component's name to its dependencies.
 
             Raises exception if an element of the dependency graph does not correspond
                 to a valid element.
 
         """
         self.dependency_graph = nx.DiGraph()
         self.name_to_component = dict()
 
         # Verify that the same keys exist in both dicts
-        assert dependency_map.keys() == components.keys(), \
-            f"Component and dependency maps should have similar keys"
+        assert (
+            dependency_map.keys() == components.keys()
+        ), f"Component and dependency maps should have similar keys"
 
         # # Mapping from component name to dependencies
         for name, dependencies in dependency_map.items():
             # This node must exist as a Component
             if not name in components:
-                raise Exception(
-                    f"Node does not exist in the component map: {name}"
-                )
+                raise Exception(f"Node does not exist in the component map: {name}")
 
             # Component cannot be added twice
             if self.is_component(name):
                 raise Exception(f"Repeated component {name}")
 
             # Create a component and add to main graph
             self.dependency_graph.add_node(components[name])
             # We want to add directed edges from all the dependencies to the
             # current node. This implies that the dependencies should already
             # exist as nodes.
             for dep in dependencies:
                 if not dep in components:
-                    logger.error("not seen")
-                    raise Exception(
-                        f"Unseen component added as dependency {dep}"
-                    )
+                    raise Exception(f"Unseen component added as dependency")
                 self.dependency_graph.add_edge(components[dep], components[name])
 
             # NOTE: Cycles are not supported
             if self._does_cycle_exist(self.dependency_graph):
                 raise Exception(f"Cycle found in execution logic")
 
             self.name_to_component[name] = components[name]
 
-        self.component_to_name : Dict[Component, name] = {
-            v : k for k,v in self.name_to_component.items()
+        self.component_to_name: Dict[Component, name] = {
+            v: k for k, v in self.name_to_component.items()
         }
-
-
-
-
```

### Comparing `GailBot-0.1a9/src/gailbot/core/utils/download.py` & `GailBot-0.2a0/src/gailbot/core/utils/download.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a9/src/gailbot/core/utils/general.py` & `GailBot-0.2a0/src/gailbot/core/utils/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 16:28:03
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 14:39:45
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:33:36
 from enum import Enum 
 from typing import List, Dict
 import psutil
 import os
 import glob
 import shutil
 import itertools
```

### Comparing `GailBot-0.1a9/src/gailbot/core/utils/media.py` & `GailBot-0.2a0/src/gailbot/core/utils/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 16:28:17
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 14:33:08
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:33:45
 
 from typing import List, Union, Dict
 import os
 from dataclasses import dataclass
 from abc import ABC 
 from .general import (
     get_extension,
```

### Comparing `GailBot-0.1a9/src/gailbot/core/utils/threads.py` & `GailBot-0.2a0/src/gailbot/core/utils/threads.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,117 +1,131 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 15:53:06
-# @Last Modified by:   Vivian Li and Siara Small
-# @Last Modified time: 2023-01-26 16:07:48
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:33:51
 
 
 from dataclasses import dataclass
 from concurrent.futures import ThreadPoolExecutor, Future, wait
 from typing import Tuple, Callable, List, Dict, Any, Union
 from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("thread")
 
+
 #### Custom Exceptions for Threads ####
 class TaskNotFoundException(Exception):
-    def __init__(self, task_key  = None ) -> None:
-        self.task_key = task_key 
+    def __init__(self, task_key=None) -> None:
+        self.task_key = task_key
+
     def __str__(self) -> str:
         return "task" + str(self.task_key) + " is not found"
-        
+
+
 class TaskNotFinishedException(Exception):
-    def __init__(self, task_key  = None ) -> None:
-        self.task_key = task_key 
+    def __init__(self, task_key=None) -> None:
+        self.task_key = task_key
+
     def __str__(self) -> str:
         return "task" + str(self.task_key) + " is not finished"
 
+
 class TaskCancelException(Exception):
-    def __init__(self, task_key  = None ) -> None:
-        self.task_key = task_key 
+    def __init__(self, task_key=None) -> None:
+        self.task_key = task_key
+
     def __str__(self) -> str:
         return "task" + str(self.task_key) + " cannot be canceled"
 
+
 class TaskCreateError(Exception):
-    def __init__(self, msg  = None ) -> None:
+    def __init__(self, msg=None) -> None:
         self.msg = msg
+
     def __str__(self) -> str:
         return "task cannot be created due to the error " + self.msg
- 
+
+
 class ThreadError(Exception):
-    def __init__(self, task_key  = None, msg: str = None ) -> None:
-        self.task_key = task_key 
+    def __init__(self, task_key=None, msg: str = None) -> None:
+        self.task_key = task_key
         self.msg = msg
-        
+
     def __str__(self) -> str:
         return "task" + str(self.task_key) + " has an error " + self.msg
 
+
 ### Defines different possible statuses for a task ###
 @dataclass
 class Status:
     running = "RUNNING"
     pending = "PENDING"
     finished = "FINISHED"
     cancelled = "CANCELLED"
     error = "ERROR"
 
+
 class ThreadPool(ThreadPoolExecutor):
     """
-    Implement a threadpool that is able to run tasks parallel on different 
-    threads, support functions to query tasks status, return task result and 
-    add callback task to previous task   
-    
+    Implement a threadpool that is able to run tasks parallel on different
+    threads, support functions to query tasks status, return task result and
+    add callback task to previous task
+
     Inheritance:
-    ThreadPoolExecutor 
-    
+    ThreadPoolExecutor
+
     """
+
     def __init__(self, max_workers: int, *args, **kwargs) -> None:
-        """ 
-        Constructs a threadpool with the given size that is able to run tasks on different 
+        """
+        Constructs a threadpool with the given size that is able to run tasks on different
             threads.
 
         Args:
-            max_workers (int):  the maximum number of tasks that will be run 
+            max_workers (int):  the maximum number of tasks that will be run
                                 at the same time parallel
         """
         super().__init__(max_workers, *args, **kwargs)
-        self.num_thread = max_workers              
-        self.task_pool: Dict[Any, Future] = dict() # used to keeps track of the task status
-        self.next_key = 0                          # next available key
-
+        self.num_thread = max_workers
+        self.task_pool: Dict[
+            Any, Future
+        ] = dict()  # used to keeps track of the task status
+        self.next_key = 0  # next available key
 
     def get_num_threads(self) -> int:
         """
         Returns the number of threads available in the thread pool.
 
         Return:
-            int: Integer value representing the number of 
+            int: Integer value representing the number of
                  threads in the given thread pool.
         """
         return self.num_thread
 
     def add_task(
-        self, 
-        task: Callable, 
-        args: List = [], 
+        self,
+        task: Callable,
+        args: List = [],
         kwargs: Dict = {},
         error_fun: Callable = None,
-        key: Union[str, int] = None) -> Union[str, int]:
+        key: Union[str, int] = None,
+    ) -> Union[str, int]:
         """
         Adds the given task to the task pool.
 
         Args:
             fun: Callable: function that will be run in the threadpool
             args: List (Optional): a list argument to the function
             kwargs: Dict (Optional): a list of key word arguments to the function
-            error_fun: Callable (Optional): a function to handle the error 
-            key: Union[str, int](Optional): a user provided key that can be used to query 
-                                the task progress and result after submitting it 
+            error_fun: Callable (Optional): a function to handle the error
+            key: Union[str, int](Optional): a user provided key that can be used to query
+                                the task progress and result after submitting it
                                 to the threadpool, caller is responsible for
-                                providing unique key  
+                                providing unique key
         Return:
             Union[str, int]: key that will be used to keep track of the task in the thread.
         """
         logger.info(f"the task {task} is being added to the thread")
         try:
             if not callable(task) or type(args) != list or type(kwargs) != dict:
                 logger.error(f"type error in adding thread task ")
@@ -122,317 +136,327 @@
                 return key
             else:
                 self.task_pool[self.next_key] = worker
                 self.next_key += 1
                 return self.next_key - 1
         except Exception as e:
             logger.error(e, exc_info=e)
-            if error_fun: 
+            if error_fun:
                 error_fun()
-            else: 
+            else:
                 raise TaskCreateError(e)
 
-
     def check_task_status(self, key: Union[str, int]):
-        """ 
+        """
         Return a string representing the status of the current task.
 
         Args:
-            key: key to find the given task in the thread. 
-        
-        Returns: 
+            key: key to find the given task in the thread.
+
+        Returns:
             String representing the status of the current task.
         """
         self._task_in_pool(key)
         future: Future = self.task_pool[key]
         return future._state
 
     def get_tasks_with_status(self, status: Status) -> List[Tuple[int, str]]:
-        """ 
+        """
         Returns a list of tasks that match the status passed in by caller
 
         Args:
-            status (Status): Status ot the task 
-            
+            status (Status): Status ot the task
+
         Returns:
             A List[Tuple[int, str]] of tasks in the thread pool that
-                match the requested status. 
+                match the requested status.
         """
-        return [task_key for task_key in self.task_pool.keys() if self.check_task_status(task_key) == status ]
+        return [
+            task_key
+            for task_key in self.task_pool.keys()
+            if self.check_task_status(task_key) == status
+        ]
 
-    def get_task_result(self, key: Union[str, int], error_fun: Callable = None ):
-        """ 
+    def get_task_result(self, key: Union[str, int], error_fun: Callable = None):
+        """
         Gets the result from the given task.
 
         Args:
             key (int): Key to find the given task in the thread pool.
 
         Return:
             If result is successfully obtained, return the result of the given task.
-            else return false as default or call the error handling function passed 
+            else return false as default or call the error handling function passed
             in from user
         """
         self._task_in_pool(key)
         try:
             future = self.task_pool[key]
             return future.result()
         except Exception as e:
-            logger.error(f"task with task key {key} with future object {future} received an exception {e} , the function exception is {future.exception()}", exc_info=e)
-            if error_fun and callable(error_fun): 
+            logger.error(
+                f"task with task key {key} with future object {future} received an exception {e} , the function exception is {future.exception()}",
+                exc_info=e,
+            )
+            if error_fun and callable(error_fun):
                 logger.error(e)
                 error_fun()
                 return future.result()
-            else: 
-                raise ThreadError(key, f"received exception {e}") ##
+            else:
+                raise ThreadError(key, f"received exception {e}")  ##
 
-    def completed(self, key: Union[str, int], error_fun: Callable = None )-> bool:
-        """ 
+    def completed(self, key: Union[str, int], error_fun: Callable = None) -> bool:
+        """
         Checks if a given task has been completed.
 
         Args:
             key (int): Key to find the given task in the thread pool.
-            error_fun: Callable function used if there is an error when 
-                       executing the task. 
+            error_fun: Callable function used if there is an error when
+                       executing the task.
 
         Raise:
-            Raise ThreadError if the result of the given task is not 
+            Raise ThreadError if the result of the given task is not
             successfully obtained.
-        
+
         Return:
             bool: True if the given task has been completed, false if not.
         """
         self._task_in_pool(key)
         try:
             return self.task_pool[key].done()
-        except: 
-            if error_fun and callable(error_fun): 
+        except:
+            if error_fun and callable(error_fun):
                 error_fun()
-            else: 
+            else:
                 raise ThreadError(key, "ERROR: failed to get thread status")
 
-    def wait_for_all_completion(self, error_fun: Callable = None ):
-        """ 
+    def wait_for_all_completion(self, error_fun: Callable = None):
+        """
         Wait for all tasks in the thread pool to be completed.
 
         Args:
-            error_fun: Callable function used if there is an error when 
-                       executing the task. 
-        
+            error_fun: Callable function used if there is an error when
+                       executing the task.
+
         Raises:
             Raises a ThreadError if the function cannot be properly executed.
 
-        Return: 
-            Calls wait_for_task() for all tasks in the thread pool. 
+        Return:
+            Calls wait_for_task() for all tasks in the thread pool.
         """
         futures = self.task_pool.values()
-        wait(futures) 
-        
+        wait(futures)
 
-    def wait_for_task(self, key: Union[str, int], error_fun: Callable = None ):
-        """ 
+    def wait_for_task(self, key: Union[str, int], error_fun: Callable = None):
+        """
         Waits for a certain task in the thread pool to be completed.
 
         Args:
             key (int): Key to find the given task in the thread pool.
-            error_fun: Callable function used if there is an error when 
-                       executing the task. 
-        
+            error_fun: Callable function used if there is an error when
+                       executing the task.
+
         Raises:
             Raises a ThreadError if the task cannot be properly executed.
 
         Return:
             None
         """
         logger.info(f"wait for the task {key}")
         self._task_in_pool(key)
         future = self.task_pool[key]
         try:
             wait([future])
             assert not future.exception()
         except Exception as e:
             logger.error(e, exc_info=e)
-            if error_fun: 
+            if error_fun:
                 error_fun()
-            else: 
+            else:
                 raise ThreadError(key, f"received exception {e}")
-    
+
     def cancel(self, key: Union[str, int]) -> bool:
         """
         Cancels the task at the given key.
- 
+
         Args:
             key (int): Key to find the given task in the thread pool.
 
         Raises:
-            TaskCancelException if the task at the given key cannot be 
+            TaskCancelException if the task at the given key cannot be
             properly cancelled.
-        
+
         Return:
-            true if the thread is canceled 
+            true if the thread is canceled
         """
         self._task_in_pool(key)
         try:
             self.task_pool[key].cancel()
             if not self.task_pool[key].cancelled():
                 raise TaskCancelException(key)
             return True
         except:
             return False
 
     def cancel_all(self) -> None:
-        """ 
+        """
         Cancels all the running tasks in the thread pool.
 
         Raises:
             TaskCancelException if the current task cannot be properly cancelled.
-        
-        Return: 
+
+        Return:
             None
         """
         try:
             for task in self.task_pool.values():
                 if not task.done():
                     task.cancel()
             return True
         except:
             return False
 
     def add_callback_with_arg(
-        self, key: Union[str, int], fun: Callable, error_fun: Callable = None):
-        """ 
+        self, key: Union[str, int], fun: Callable, error_fun: Callable = None
+    ):
+        """
         Adds a function to the thread as a callback of a previous function
 
         Args:
             key (int): key to find the given task.
-            fun (Callable): function to be called as the callback. 
-            error_fun: Callable function used if there is an error 
+            fun (Callable): function to be called as the callback.
+            error_fun: Callable function used if there is an error
                        when executing the task.
-                       
+
         Raises:
             ThreadError if the callback function cannot be added
-            
-        Return: 
-            Returns the key that identify the newly added task 
+
+        Return:
+            Returns the key that identify the newly added task
         """
         self._task_in_pool(key)
         future = self.task_pool[key]
         res = [future.result()]
         if res and future.done():
             return self.add_task(fun, res)
         elif error_fun and callable(error_fun):
             error_fun()
-        else: 
+        else:
             raise ThreadError(key, "ERROR: Failed to add callback")
-    
+
     def add_callback(self, key: Union[str, int], fun: Callable):
-        """ add call back function fun that will run after the task identified
-            by key is finished running 
+        """add call back function fun that will run after the task identified
+            by key is finished running
 
         Args:
-            key (Union[str, int]): the key that identifies the existing an task  
-            fun (Callable): the call back function that will be added 
+            key (Union[str, int]): the key that identifies the existing an task
+            fun (Callable): the call back function that will be added
         """
         if not callable(fun):
             raise ThreadError(key, "ERROR: Non-function added as callback")
         future = self.task_pool[key]
         future.add_done_callback(fun)
-    
+
     def add_callback_on_result(
-        self, 
-        key: Union[str, int], 
-        fun: Callable, 
-        args: List = [], 
-        kwargs: Dict = {},  
-        error_fun: Callable = None) -> int:
-        """ 
+        self,
+        key: Union[str, int],
+        fun: Callable,
+        args: List = [],
+        kwargs: Dict = {},
+        error_fun: Callable = None,
+    ) -> int:
+        """
         Adds a task to the thread after one task has finished running.
 
         Args:
             key (int): Key to find the current task.
-            fun (Callable): function to be called after the current task has 
-                            been completed. 
+            fun (Callable): function to be called after the current task has
+                            been completed.
             error_fun: Callable function used if there is an error when
                       executing the task.
 
-        Raises: 
-            Raises ThreadError if the task identified by key is throws an 
-            exception 
-            
-            Raises TypeError if the arguments is not passed in correctly 
-        
+        Raises:
+            Raises ThreadError if the task identified by key is throws an
+            exception
+
+            Raises TypeError if the arguments is not passed in correctly
+
         Returns:
-            Returns the key that identify the newly added task 
+            Returns the key that identify the newly added task
         """
         self._task_in_pool(key)
         future = self.task_pool[key]
         wait([future])
         if not callable(fun) and type(args) == list and type(kwargs) == dict:
             logger.error(f"type error in adding thread task ")
-            raise TypeError(f"Type error in adding callback on result to thread task {key}")
+            raise TypeError(
+                f"Type error in adding callback on result to thread task {key}"
+            )
         try:
             future.result()
             return self.add_task(fun, args, kwargs)
         except Exception as e:
             logger.error(e, exc_info=e)
-            if error_fun: 
+            if error_fun:
                 error_fun()
-            else: 
-                raise ThreadError(key, f"ERROR: Failed to add callback task, get error {e}")
-    
+            else:
+                raise ThreadError(
+                    key, f"ERROR: Failed to add callback task, get error {e}"
+                )
+
     def is_busy(self) -> bool:
         """
         Determines if the thread queue has tasks in it.
 
         Returns:
             bool: True if the queue has non-zero tasks, false if otherwise.
         """
-        return self._work_queue.qsize() != 0 
-    
+        return self._work_queue.qsize() != 0
+
     def count_waiting_tasks(self) -> int:
         """
         Calculates the total number of tasks waiting in the queue.
 
         Returns:
             Integer representing the total waiting tasks
         """
         return self._work_queue.qsize()
 
-    def count_completed_tasks(self) -> int: 
-        """get the number of completed task 
+    def count_completed_tasks(self) -> int:
+        """get the number of completed task
 
         Returns:
-            int: the number of completed task 
+            int: the number of completed task
         """
-        num = 0 
+        num = 0
         for future in self.task_pool.values():
             if future.done():
                 num += 1
         return num
-    
+
     def count_total_tasks(self) -> int:
         """get the number of all the tasks that has been added to the threadpool,
-           which includes failure task, completed task, running task and pending task 
+           which includes failure task, completed task, running task and pending task
 
 
         Returns:
-            int:  the total number of task 
+            int:  the total number of task
         """
         return len(self.task_pool)
-        
+
     ############ private function  ##########
-    def _task_in_pool(self, key:int) -> None :
-        """ 
+    def _task_in_pool(self, key: int) -> None:
+        """
         Private function to determine if the given task is currently in the task pool.
 
         Args:
             key (int): key with which to find the given task in the thread.
 
         Raises:
-            Raises TaskNotFoundException if the given task is not currently 
+            Raises TaskNotFoundException if the given task is not currently
             in the thread.
-        
+
         Return:
             None
         """
         if not key in self.task_pool:
             raise TaskNotFoundException(key)
-
```

### Comparing `GailBot-0.1a9/src/gailbot/plugins/loader/directoryloader.py` & `GailBot-0.2a0/src/gailbot/plugins/loader/directoryloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:34:17
 import os
 import pip
 from cryptography.fernet import Fernet
 from typing import Dict, List, Union, TypedDict, Tuple
 from dataclasses import dataclass
 from .pluginLoader import PluginLoader
 from ..suite import PluginSuite
@@ -111,14 +116,15 @@
                 official = os.path.join(root, PLUGIN_CONFIG.OFFICIAL)
             if PLUGIN_CONFIG.FORMAT in files:
                 format = os.path.join(root, PLUGIN_CONFIG.FORMAT)
             if config and requirement and document and official and format:
                 break
 
         if not config or not document or not format:
+            logger.error(f"missing required file")
             return False
 
         # download required package
         try:
             if requirement:
                 self.download_packages(requirement, PROJECT_ROOT)
         except Exception as e:
@@ -138,14 +144,17 @@
         if suite:
             # validate
             if self.validate_official(official):
                 suite.set_to_official_suite()
             return [suite]
         else:
             delete(tgt_path)
+            logger.warn(
+                f"the plugin suite validation failed, delete suite at {tgt_path}"
+            )
             return False
 
     def download_packages(self, req_file, dest):
         """download packages listed under req_file to dest
 
         Args:
             req_file(str): a string that specifies the path to requirements.txt file
@@ -207,15 +216,15 @@
             if the plugin can be successfully loaded, return false otherwise
         """
         validated, conf = PluginTOMLLoader.validate_config(conf_path, suite_name)
         if validated:
             conf.update({"path": get_parent_path(conf_path)})
             return self.dict_config_loader.load(conf, suites_directory)
         else:
-            logger.error(f"Error: {conf}")
+            logger.error(f"Plugin suite toml file validation failed Error: {conf}")
             return False
 
     @staticmethod
     def validate_config(
         conf_path: str, suite_name: str
     ) -> Tuple[bool, Union[str, Dict]]:
         """
@@ -252,12 +261,14 @@
     """load a plugin suite from a dictionary that contains the configuration
     of all plugin dependencies and sources
     """
 
     def load(self, dict_conf: Dict, suites_directory: str) -> PluginSuite:
         if not type(dict_conf) == dict:
             return ""
-        suite = PluginSuite(dict_conf, suites_directory)
-        if suite.is_ready:
+        try:
+            suite = PluginSuite(dict_conf, suites_directory)
+            assert suite.is_ready
             return suite
-        else:
+        except Exception as e:
+            logger.error(e, exc_info=e)
             return False
```

### Comparing `GailBot-0.1a9/src/gailbot/plugins/loader/pluginLoader.py` & `GailBot-0.2a0/src/gailbot/plugins/loader/pluginLoader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-import os 
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:34:30
+import os
 from typing import Dict, List, Union, TypedDict, Tuple
 from abc import ABC
 from ..suite import PluginSuite
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.utils.general import (
     filepaths_in_dir,
     get_name,
@@ -14,11 +19,13 @@
 )
 from gailbot.core.utils.download import download_from_urls
 from pydantic import BaseModel, ValidationError
 from urllib.parse import urlparse
 
 logger = makelogger("plugin_loader")
 
+
 class PluginLoader(ABC):
-    """ base class for plugin loader """
+    """base class for plugin loader"""
+
     def load(self, *args, **kwargs) -> List[PluginSuite]:
-        raise NotImplementedError()
+        raise NotImplementedError()
```

### Comparing `GailBot-0.1a9/src/gailbot/plugins/loader/urlloader.py` & `GailBot-0.2a0/src/gailbot/plugins/loader/urlloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:34:44
 import os
 import re
 import boto3
 from botocore.exceptions import ParamValidationError
 from cryptography.fernet import Fernet
 from typing import Dict, List, Union, TypedDict, Tuple
 from abc import ABC
```

### Comparing `GailBot-0.1a9/src/gailbot/plugins/manager.py` & `GailBot-0.2a0/src/gailbot/plugins/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 13:22:01
 # @Last Modified by:   Jason Y. Wu
-# @Last Modified time: 2023-06-28 19:15:39
+# @Last Modified time: 2023-08-01 05:35:34
 from dataclasses import dataclass
 import toml
 import sys
 import os
 from typing import List, Union, Dict
 import validators
 from .suite import PluginSuite, MetaData
@@ -23,14 +23,15 @@
     subdirs_in_dir,
     delete,
     get_name,
     is_directory,
     filepaths_in_dir,
 )
 from gailbot.configs.interfaces import get_plugin_structure_config
+from gailbot.configs import PLUGIN_CONFIG
 
 EXPECTED_STRUCTURE = get_plugin_structure_config()
 logger = makelogger("plugin_manager")
 
 
 @dataclass
 class ERROR:
@@ -174,14 +175,15 @@
         make_dir(self.suites_dir, overwrite=False)
         make_dir(self.download_dir, overwrite=True)
 
     def delete_suite(self, name: str):
         """
         given a suite name, delete the plugin suite
         """
+        logger.warn(f"remove suite {name}")
         try:
             if self.is_suite(name):
                 delete(os.path.join(self.suites_dir, name))
                 del self.suites[name]
                 return True
             else:
                 return False
```

### Comparing `GailBot-0.1a9/src/gailbot/plugins/plugin.py` & `GailBot-0.2a0/src/gailbot/plugins/plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 13:22:45
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-12 13:29:53
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:35:38
 
 from typing import Any, Dict, TypedDict
 from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("plugin")
+
+
 class Utt(TypedDict):
-    start_time: str 
+    start_time: str
     end_time: str
-    speaker: str 
-    text:str 
+    speaker: str
+    text: str
+
+
 class Methods:
     """
     Methods that will be passed to a plugin.
-    These can be custom defined and may be useful as 
+    These can be custom defined and may be useful as
     a wrapper around objects
     that may want to be passed to a plugin.
     """
 
     def __init__(self):
         pass
 
+
 class Plugin:
     """
     Template superclass for any plugin.
     """
 
     def __init__(self) -> None:
         self.name = self.__class__
@@ -35,25 +40,20 @@
         pass
 
     @property
     def is_successful(self) -> bool:
         return self.successful
 
     def apply(
-        self,
-        dependency_outputs : Dict[str, Any],
-        methods : Methods,
-        *args,
-        **kwargs
+        self, dependency_outputs: Dict[str, Any], methods: Methods, *args, **kwargs
     ) -> Any:
         """
         Wrapper for plugin algorithm that has access to dependencies =,
         Args:
             dependency_outputs (Dict[str,Any]):
                 Mapping from all plugins this plugin is dependant on and their
                 outputs.
         """
         raise NotImplementedError()
-    
+
     def __repr__(self) -> str:
         return f"plugin {self.name}"
-
```

### Comparing `GailBot-0.1a9/src/gailbot/plugins/suite.py` & `GailBot-0.2a0/src/gailbot/plugins/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 13:22:39
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-16 13:10:57
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:35:51
 
 import sys
 import os
-from typing import Dict, List, Any, Tuple
+from typing import Dict, List, Any, Tuple, Callable
 import time
 from pydantic import BaseModel
 
-from .plugin import Plugin, Methods
+from gailbot.plugins.plugin import Plugin, Methods
 from gailbot.core.utils.logger import makelogger
 from gailbot.configs import PLUGIN_CONFIG
-from gailbot.core.pipeline import Pipeline, Component, ComponentResult, ComponentState
+from gailbot.core.pipeline import (
+    Pipeline,
+    Component,
+    ComponentResult,
+    ComponentState,
+)
 from gailbot.core.utils.general import is_file
 
 import importlib
 
-
 logger = makelogger("pluginSuite")
 
 
 class PluginResult(ComponentResult):
     """
     Class containing the result of a component object.
     """
@@ -57,17 +61,17 @@
         logger.info(plugin)
         self.plugin = plugin
 
     def __repr__(self):
         return str(self.plugin)
 
     def __call__(
-        self,
-        dependency_outputs: Dict[str, ComponentResult] = {},
-        methods: Methods = None,
+            self,
+            dependency_outputs: Dict[str, ComponentResult] = {},
+            methods: Methods = None,
     ):
         """
         In addition to dependency outputs, this expects methods which can be
         passed to the individual plugins.
         """
         # Extract the actual dependency results
         logger.info("plugin component called")
@@ -104,24 +108,14 @@
         self.dict_conf = dict_conf
         self.source_path = abs_path
         # metadata and document_path will be loaded in _load_from_config
         self.metadata: MetaData = None
         self.document_path: str = None
         self.formatmd_path: str = None
         self.dependency_map, self.plugins = self._load_from_config(dict_conf, abs_path)
-
-        # Wrap the plugins in PluginComponent
-        self.components = {k: PluginComponent(v) for k, v in self.plugins.items()}
-
-        # Init the pipeline based on the components
-        self.pipeline = Pipeline(
-            dependency_map=self.dependency_map,
-            components=self.components,
-            num_threads=PLUGIN_CONFIG.THREAD_NUM,
-        )
         # Add vars here from conf.
         self._name = dict_conf["suite_name"]
         self._is_ready = True
         self.is_official = False
 
     @property
     def name(self) -> str:
@@ -148,19 +142,19 @@
     def __call__(self, base_input: Any, methods: Methods) -> Dict:
         """
         Apply the specified plugins when possible and return the results
         summary
         """
         logger.info(methods)
         logger.info(base_input)
-
+        components = {k: PluginComponent(v()) for k, v in self.plugins.items()}
         pipeline = Pipeline(
             dependency_map=self.dependency_map,
-            components=self.components,
-            num_threads=1,
+            components=components,
+            num_threads=PLUGIN_CONFIG.THREAD_NUM,  # read from config
         )
 
         result = pipeline(
             base_input=base_input, additional_component_kwargs={"methods": methods}
         )
         return result
 
@@ -174,26 +168,26 @@
 
     def plugin_details(self, plugin_name: str) -> Dict:
         if self.is_plugin(plugin_name):
             return {"dependencies": self.dependency_map[plugin_name]}
 
     def dependency_graph(self) -> Dict:
         """Return the entire dependency graph as a dictionary"""
-        return self.pipeline.get_dependency_graph()
+        return self.dependency_map
 
     def get_meta_data(self) -> MetaData:
         """get the metadata about this plugin"""
         return self.metadata
 
     ##########
     # PRIVATE
     ##########
     def _load_from_config(
-        self, dict_config, abs_path: str
-    ) -> Tuple[Dict[str, List[str]], Dict[str, Plugin]]:
+            self, dict_config, abs_path: str
+    ) -> Tuple[Dict[str, List[str]], Dict[str, Callable]]:
         """
         load the plugin suite, the information about the each plugin name,
         and its path is stored in the dict_config, all path information
         is relative to the abs_path
 
         Args:
         dict_config must have the keys:
@@ -216,27 +210,26 @@
         logger.info(dict_config)
         logger.info(f"absolute path: {abs_path}")
 
         metadata = dict_config["metadata"]
         MetaData(**metadata)
         self.metadata = metadata
         self.document_path = os.path.join(abs_path, suite_name, PLUGIN_CONFIG.DOCUMENT)
-        self.formatmd_path = os.path.join(abs_path,suite_name, PLUGIN_CONFIG.FORMAT )
+        self.formatmd_path = os.path.join(abs_path, suite_name, PLUGIN_CONFIG.FORMAT)
         assert is_file(self.document_path)
-        
+
         for conf in dict_config["plugins"]:
             module_name = conf["module_name"]
             module_full_name = f"{suite_name}.{module_name}"
             rel_path = conf["rel_path"]
             path = os.path.join(abs_path, suite_name, rel_path)
             clazz_name = conf["plugin_name"]
             spec = importlib.util.spec_from_file_location(module_full_name, path)
             module = importlib.util.module_from_spec(spec)
             sys.modules[module_full_name] = module
             spec.loader.exec_module(module)
             clazz = getattr(module, clazz_name)
-            instance = clazz()
             dependency_map[clazz_name] = conf["dependencies"]
-            plugins[clazz_name] = instance
+            plugins[clazz_name] = clazz
         logger.info(f"plugin dependency map {dependency_map}")
         logger.info(f"pluins {plugins}")
         return dependency_map, plugins  # used to generate pipeline
```

### Comparing `GailBot-0.1a9/src/gailbot/services/controller.py` & `GailBot-0.2a0/src/gailbot/services/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,66 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 14:30:48
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-04 15:18:14
 from typing import Dict, List, Any, Tuple, Union, Callable
 
 from .organizer import Organizer, SettingDict
 from .converter import Converter
 from .pipeline import PipelineService
 from ..plugins import PluginManager, PluginSuite
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.utils.general import get_name
 from gailbot.workspace.manager import WorkspaceManager
 from gailbot.configs import service_config_loader, default_setting_loader
+
 CONFIG = service_config_loader()
 DEFAULT_SETTING = default_setting_loader()
 logger = makelogger("service_controller")
 """ Knows about all three sub modules """
 
 
 class ServiceController:
     def __init__(
-        self, ws_manager: WorkspaceManager, load_exist_setting: bool = False
+            self, ws_manager: WorkspaceManager, load_exist_setting: bool = False
     ) -> None:
         self.organizer = Organizer(ws_manager.setting_src, load_exist_setting)
         self.converter = Converter(ws_manager)
         self.plugin_manager = PluginManager(ws_manager.plugin_src)
         self.pipeline_service = PipelineService(
             self.plugin_manager, num_threads=CONFIG.thread.transcriber_num_threads
         )
         self.transcribed = set()  ## stores the file name of transcribed file
         self._init_default_setting()
-        
+
     def _init_default_setting(self):
         # add default engine setting
         if not self.organizer.is_engine_setting(DEFAULT_SETTING.engine_name):
-            self.organizer.add_new_engine(DEFAULT_SETTING.engine_name, DEFAULT_SETTING.engine_data)
+            self.organizer.add_new_engine(
+                DEFAULT_SETTING.engine_name, DEFAULT_SETTING.engine_data
+            )
         self.organizer.set_default_engine(DEFAULT_SETTING.engine_name)
-        
+
         # add default profile setting
         if not self.organizer.is_setting(DEFAULT_SETTING.profile_name):
-            plugin_suites = DEFAULT_SETTING.profile_data["plugin_setting"] 
+            plugin_suites = DEFAULT_SETTING.profile_data["plugin_setting"]
             for suite in plugin_suites:
                 if not self.plugin_manager.is_suite(suite):
-                    self.organizer.create_new_setting(DEFAULT_SETTING.profile_name,DEFAULT_SETTING.profile_data_no_plugin)
+                    self.organizer.create_new_setting(
+                        DEFAULT_SETTING.profile_name,
+                        DEFAULT_SETTING.profile_data_no_plugin,
+                    )
                     self.organizer.set_default_setting(DEFAULT_SETTING.profile_name)
                     return
-            self.organizer.create_new_setting(DEFAULT_SETTING.profile_name,DEFAULT_SETTING.profile_data)
+            self.organizer.create_new_setting(
+                DEFAULT_SETTING.profile_name, DEFAULT_SETTING.profile_data
+            )
         self.organizer.set_default_setting(DEFAULT_SETTING.profile_name)
-            
-        
+
     def add_sources(self, src_output_pairs: List[Tuple[str, str]]):
         """add a list of sources
 
         Args:
             src_output_pairs (List[Tuple [str, str]]): a list of pairs that
             stores the input path and the output path
 
@@ -88,14 +100,30 @@
                         full path to the source or the filename
 
 
         Returns:
             bool: return true if the source can be deleted correctly
         """
         return self.organizer.remove_source(name)
+    
+    def remove_sources(self, names: List[str]) -> bool:
+        """Remove the list of sources
+
+        Args:
+            names (List[str]): the names of the sources, which can be either the
+                        full path to the source or the filename
+
+
+        Returns:
+            bool: True if all sources have been successfully removed, False if not
+        """
+        for source_name in names:
+            if not self.organizer.remove_source(source_name):
+                return False
+        return True
 
     def is_source(self, name: str) -> bool:
         """check if a source exists
 
         Args:
             name (str): either the name of the source or the path to the source
 
@@ -112,26 +140,27 @@
             source_name: str: source name to access
 
         Returns:
             a string stores the output of the source
         """
         return self.organizer.get_source_outdir(name)
 
-    def create_new_setting(self, name: str, setting: SettingDict) -> bool:
+    def create_new_setting(self, name: str, setting: SettingDict, overwrite: bool = True) -> bool:
         """create a new setting
 
         Args:
             name (str): the name of the setting
             setting (Dict[str, str]): the setting content
+            overwrite (bool)
 
         Returns:
             bool: return true if the setting can be created, if the setting uses
                   an existing name, the setting cannot be created
         """
-        return self.organizer.create_new_setting(name, setting)
+        return self.organizer.create_new_setting(name, setting, overwrite)
 
     def save_setting(self, setting_name: str) -> bool:
         """save the setting locally on the disk
 
         Args:
             setting_name (str): the setting name of the setting
 
@@ -170,15 +199,15 @@
 
         Returns:
             Dict[str, SettingDict]: a dictionary that maps the setting name to
                 a setting content
         """
         return self.organizer.get_all_settings_data()
 
-    def get_all_profile_names(self) -> List[str]:
+    def get_all_settings_names(self) -> List[str]:
         """get the names fo available settings
 
         Returns:
             List[str]: a list of available setting names
         """
         return self.organizer.get_all_profile_names()
 
@@ -219,15 +248,15 @@
         Returns:
             Union[bool, SettingDict]: if the setting is found, returns its setting
             content stored in a dictionary, else returns false
         """
         return self.organizer.get_setting_dict(setting_name)
 
     def get_source_setting_dict(
-        self, source_name: str
+            self, source_name: str
     ) -> Union[bool, Dict[str, Union[str, Dict]]]:
         """given a source name, return the setting content of the source
             in a dictionary
 
         Args:
             source_name (str): name that identifies a source
 
@@ -244,14 +273,29 @@
             setting_name (str): the name of the setting that will be removed
 
         Returns:
             bool: true if the setting is removed, false otherwise
         """
         return self.organizer.remove_setting(setting_name)
 
+    def remove_multiple_settings(self, setting_names: List[str]) -> bool:
+        """
+        Removes the given list of settings
+
+        Args:
+            setting_name: List[str]: names of the setting to remove
+
+        Returns:
+            Bool: True if all settings were successfully removed, false if not
+        """ 
+        for setting_name in setting_names:
+            if not self.organizer.remove_setting(setting_name):
+                return False
+        return True
+
     def is_setting(self, name: str) -> bool:
         """check if a setting exists or not
 
         Args:
             name (str): names that identifies the settings
 
         Returns:
@@ -285,15 +329,15 @@
 
         Returns:
             bool: True if successfully set, false if not
         """
         return self.organizer.set_default_setting(setting_name)
 
     def apply_setting_to_sources(
-        self, sources: List[str], setting: str, overwrite: bool = True
+            self, sources: List[str], setting: str, overwrite: bool = True
     ) -> bool:
         """apply setting to a list of sources
 
         Args:
             sources (List[str]): a list of string that identifies the sources
             setting (str): the setting name
             overwrite (bool, optional): if true, overwrites  the existing setting
@@ -301,15 +345,15 @@
 
         Returns:
             bool: return true if settings can be applied
         """
         return self.organizer.apply_setting_to_sources(sources, setting, overwrite)
 
     def apply_setting_to_source(
-        self, source: str, setting: str, overwrite: bool = True
+            self, source: str, setting: str, overwrite: bool = True
     ) -> bool:
         """apply setting to a source
 
         Args:
             sources (str): a string that identifies the source
             setting (str): the setting name
             overwrite (bool, optional): if true, overwrites  the existing setting
@@ -393,14 +437,22 @@
         try:
             for src in self.transcribed:
                 self.organizer.remove_source(src)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
 
+    def get_all_source_names(self) -> List[str]:
+        """
+        Returns list of all source names
+
+        Returns: List[str] : list of source names
+        """
+        return self.organizer.get_all_source_names()
+
     def register_plugin_suite(self, plugin_source: str) -> Union[List[str], str]:
         """
         Registers a plugin suite to the object's plugin manager
 
         Args:
             plugin_source: str: plugin suite to register
 
@@ -453,14 +505,29 @@
             suite_name: str: name of the plugin suite to delete
 
         Returns:
             bool: True if successfully deleted, false if not
         """
         return self.plugin_manager.delete_suite(suite_name)
 
+    def delete_plugin_suites(self, suite_names: List[str]) -> bool:
+        """
+        Removes the given list of plugin suites
+
+        Args:
+            suite_name: List[str]: list of names of the plugin suites to delete
+
+        Returns:
+            Bool: true if all plugin suites were successfully removed, false if not
+        """  
+        for suite_name in suite_names:
+            if not self.plugin_manager.delete_suite(suite_name):
+                return False
+        return True
+
     def get_plugin_suite_metadata(self, suite_name: str):
         """get the metadata of a plugin suite identified by suite name
 
         Args:
             suite_name (str): the name of the suite
 
         Returns:
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/converter.py` & `GailBot-0.2a0/src/gailbot/services/converter/converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,89 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:38:26
 from typing import Dict, List, Union, Tuple
 
 from .payload import (
-    load_transcribed_dir_payload, 
-    load_audio_payload, 
+    load_transcribed_dir_payload,
+    load_audio_payload,
     load_conversation_dir_payload,
-    PayLoadObject)
+    PayLoadObject,
+)
 from gailbot.core.utils.logger import makelogger
 from ..organizer.source import SourceObject
 from gailbot.workspace.manager import WorkspaceManager
 
 logger = makelogger("converter")
-class Converter: 
+
+
+class Converter:
+    """
+    Provides functionality that converts the sourceObject to payload and
+    keeps track of the converted payloads
     """
-    Provides functionality that converts the sourceObject to payload and 
-    keeps track of the converted payloads 
-    """ 
+
     loaders = [
-        load_audio_payload, 
+        load_audio_payload,
         load_transcribed_dir_payload,
-        load_conversation_dir_payload]
-    
+        load_conversation_dir_payload,
+    ]
+
     """ mapping payload name to payloadObject """
+
     def __init__(self, ws_manager: WorkspaceManager) -> None:
         self.ws_manager = ws_manager
         self.payloads_dict: Dict[str, PayLoadObject] = dict()
-        
+
     def load_source(self, source: SourceObject) -> bool:
         """
         Loads a given source object with the correct loader
 
         Args:
             source: SourceObject: source to load
 
         Returns:
             bool: true if successfully loaded, false if not
         """
         for loader in self.loaders:
-            try: 
-                payloads: List [PayLoadObject] = loader(source, self.ws_manager)
+            try:
+                payloads: List[PayLoadObject] = loader(source, self.ws_manager)
                 logger.info(payloads)
                 if isinstance(payloads, list):
                     self.payloads_dict[source.name] = payloads
-                    return True 
+                    return True
             except Exception as e:
-                logger.error(e, exc_info=e) 
+                logger.error(e, exc_info=e)
         return False
 
-    
     def __call__(
-        self, sources: List[SourceObject]) -> Union[bool, Tuple [List[PayLoadObject], List[str]]]:
-        """ given a list of the source files, and convert them into a list of 
-           payload objects 
+        self, sources: List[SourceObject]
+    ) -> Union[bool, Tuple[List[PayLoadObject], List[str]]]:
+        """given a list of the source files, and convert them into a list of
+           payload objects
 
         Args:
             sources (List[SourceObject]): a list of source object
 
         Returns:
-            Union[bool, List[PayLoadObject]]: a list of payload object that are 
+            Union[bool, List[PayLoadObject]]: a list of payload object that are
             successfully converted by the converter
         """
         logger.info("converter is called")
         logger.info(sources)
         self.payloads_dict = dict()
         invalid = list()
-       
+
         try:
             for source in sources:
                 logger.info(source)
                 if not self.load_source(source):
                     invalid.append(source.name)
             logger.info(self.payloads_dict)
-            converters = sum(list(self.payloads_dict.values()), []) 
+            converters = sum(list(self.payloads_dict.values()), [])
             return converters, invalid
-        
-        except Exception as e: 
+
+        except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
-                
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/payload/audioPayload.py` & `GailBot-0.2a0/src/gailbot/services/converter/payload/audioPayload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,89 +1,101 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-03 19:03:04
 from typing import List, Union
 from .payloadObject import PayLoadObject, PayLoadStatus
 from ...organizer.source import SourceObject
-from gailbot.core.utils.general import (
-    get_extension,  
-    copy)
+from gailbot.core.utils.general import get_extension, copy
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.utils.media import AudioHandler
-import os 
+import os
 from gailbot.workspace.manager import WorkspaceManager
 from gailbot.configs import service_config_loader
 
 SUPPORTED_AUDIO = service_config_loader().engines.audio_supported_format
 MERGED_FILE_NAME = "merged"
 
 logger = makelogger("audioPayload")
 
+
 def load_audio_payload(
-    source: SourceObject, ws_manager: WorkspaceManager) -> Union[bool, List[PayLoadObject]]:
-    """ given a source object, convert it into an audio payload if the source 
-    
+    source: SourceObject, ws_manager: WorkspaceManager
+) -> Union[bool, List[PayLoadObject]]:
+    """given a source object, convert it into an audio payload if the source
+
     Args:
-        source (SourceObject): an instance of SourceObject that stores the 
+        source (SourceObject): an instance of SourceObject that stores the
         datafile and setting of the transcription
 
     Returns:
-        Union[bool, List[PayLoadObject]]: return the converted payload if the 
+        Union[bool, List[PayLoadObject]]: return the converted payload if the
         conversion is successful, return false other wise
     """
-    if not source.setting: 
+
+    if not source.setting:
+        logger.info("from source.setting")
         return False
     if not AudioPayload.is_supported(source.source_path()):
-        return False  
+        logger.info("from is_supported(...)")
+        return False
     try:
         return [AudioPayload(source, ws_manager)]
     except Exception as e:
         logger.error(source.__class__)
         logger.error(e, exc_info=e)
         return False
 
-class AudioPayload(PayLoadObject):  
+
+class AudioPayload(PayLoadObject):
     """
     Class for audio payload
     """
+
     def __init__(self, source: SourceObject, workspace: WorkspaceManager) -> None:
+        logger.info("HERE")
         super().__init__(source, workspace)
-    
+
     @staticmethod
     def is_supported(file_path: str) -> bool:
         """
         Determines if a given file path has a supported file extension
         """
         logger.info(file_path)
         return get_extension(file_path) in SUPPORTED_AUDIO
-    
+
     def _set_initial_status(self) -> None:
         """
         Sets the initial status of the payload object to initialized
         """
         self.status = PayLoadStatus.INITIALIZED
-    
+
     def _copy_file(self) -> None:
         """
         Copies file to workspace
         """
         extension = get_extension(self.original_source)
-        tgt_path =os.path.join(
-            self.workspace.data_copy, f"{self.name}.{extension}")
+        tgt_path = os.path.join(self.workspace.data_copy, f"{self.name}.{extension}")
         copy(self.original_source, tgt_path)
         self.data_files = [tgt_path]
-        
+
     def _merge_audio(self):
         try:
             handler = AudioHandler()
-            merged_path = handler.overlay_audios(self.data_files, self.out_dir.media_file, MERGED_FILE_NAME)
+            merged_path = handler.overlay_audios(
+                self.data_files, self.out_dir.media_file, MERGED_FILE_NAME
+            )
             self.merged_audio = merged_path
             assert merged_path
         except Exception as e:
             logger.error(e, exc_info=e)
-            
+
     @staticmethod
     def supported_format() -> List[str]:
         """
         Contains and accesses a list of the supported formats
         """
         return SUPPORTED_AUDIO
 
     def __repr__(self) -> str:
-        return "Audio payload"
+        return "Audio payload"
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/payload/conversationDirectoryPayload.py` & `GailBot-0.2a0/src/gailbot/services/converter/payload/conversationDirectoryPayload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,114 @@
-import os 
-from typing import List,  Union
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:36:39
+import os
+from typing import List, Union
 from .payloadObject import PayLoadObject, PayLoadStatus
 from ...organizer.source import SourceObject
-from gailbot.core.utils.general import (
-    paths_in_dir, 
-    is_directory, 
-    copy
-)
+from gailbot.core.utils.general import paths_in_dir, is_directory, copy
 from gailbot.core.utils.logger import makelogger
 from gailbot.workspace.manager import WorkspaceManager
 from .audioPayload import AudioPayload
 from gailbot.core.utils.media import AudioHandler
 
 MERGED_FILE_NAME = "merged"
 logger = makelogger("conversation_payload")
 
+
 def load_conversation_dir_payload(
-    source: SourceObject, 
-    ws_manager: WorkspaceManager
-) -> Union [bool, List[PayLoadObject]]:
-    """ Given a source object, convert it into an conversation directory payload 
+    source: SourceObject, ws_manager: WorkspaceManager
+) -> Union[bool, List[PayLoadObject]]:
+    """Given a source object, convert it into an conversation directory payload
         if the source stores a conversation directory
-    
+
     Args:
-        source (SourceObject): an instance of SourceObject that stores the 
+        source (SourceObject): an instance of SourceObject that stores the
         datafile and setting of the transcription
 
     Returns:
-        Union[bool, List[PayLoadObject]]: return the converted payload if the 
+        Union[bool, List[PayLoadObject]]: return the converted payload if the
         conversion is successful, return false other wise
     """
     original_source = source.source_path()
     if not is_directory(original_source) or not source.setting:
         return False
     if ConversationDirectoryPayload.is_supported(original_source):
         return [ConversationDirectoryPayload(source, ws_manager)]
-   
-    # NOTE: currently not support loading directory inside directory 
+
+    # NOTE: currently not support loading directory inside directory
     return False
-        
+
 
 class ConversationDirectoryPayload(PayLoadObject):
-    """ 
-    Stores a conversation directory with only audio files 
     """
+    Stores a conversation directory with only audio files
+    """
+
     def __init__(self, source: SourceObject, workspace: WorkspaceManager) -> None:
         super().__init__(source, workspace)
-    
-    @staticmethod 
+
+    @staticmethod
     def supported_format() -> str:
         """
         Contains and accesses a list of the supported formats
         """
         return "directory"
-        
+
     @staticmethod
     def is_supported(file_path: str) -> bool:
         """
         Determines if a given file path has a supported file extension
 
         Args:
             file_path: str: file path to check
-        
-        Returns: 
+
+        Returns:
             bool: True if it contains a supported file extension, false if not
         """
         logger.info(file_path)
         if not is_directory(file_path):
-            return False 
-        sub_paths = paths_in_dir(file_path, AudioPayload.supported_format(), recursive=False)
+            return False
+        sub_paths = paths_in_dir(
+            file_path, AudioPayload.supported_format(), recursive=False
+        )
         if len(sub_paths) == 0:
             return False
         return True
-     
+
     def _copy_file(self) -> None:
         """
         Copies file to workspace
         """
         try:
             tgt_path = os.path.join(self.workspace.data_copy, f"{self.name}")
             copy(self.original_source, tgt_path)
             self.data_files = []
-            sub_paths = paths_in_dir(tgt_path, AudioPayload.supported_format(), recursive=False)
+            sub_paths = paths_in_dir(
+                tgt_path, AudioPayload.supported_format(), recursive=False
+            )
             for path in sub_paths:
                 self.data_files.append(path)
         except Exception as e:
             logger.error(e, exc_info=e)
-    
+
     def _merge_audio(self):
         try:
             handler = AudioHandler()
-            merged_path = handler.overlay_audios(self.data_files, self.out_dir.media_file, MERGED_FILE_NAME)
+            merged_path = handler.overlay_audios(
+                self.data_files, self.out_dir.media_file, MERGED_FILE_NAME
+            )
             self.merged_audio = merged_path
             assert merged_path
         except Exception as e:
             logger.error(e, exc_info=e)
-    
+
     def _set_initial_status(self) -> None:
         """
         Sets the initial status of the payload object to initialized
         """
         self.status = PayLoadStatus.INITIALIZED
 
     def __repr__(self) -> str:
-        return "Conversation directory payload"
+        return "Conversation directory payload"
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/payload/payloadObject.py` & `GailBot-0.2a0/src/gailbot/services/converter/payload/payloadObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,128 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:37:02
 from abc import ABC
-from typing import List, Dict 
-import os 
-from enum import Enum 
+from typing import List, Dict
+import os
+from enum import Enum
 from datetime import datetime
 from gailbot.core.utils.general import write_json, copy, is_file
-from gailbot.configs import  OutputFolder, TemporaryFolder
+from gailbot.configs import OutputFolder, TemporaryFolder
 from gailbot.core.utils.logger import makelogger
 from ...organizer.source import SourceObject
 from ...organizer.settings import SettingObject
 from ..result import (
-    UttResult, 
-    AnalysisResult, 
-    FormatResult, 
+    UttResult,
+    AnalysisResult,
+    FormatResult,
     UttDict,
     AnalysisResultDict,
     FormatResultDict,
-    ProcessingStats
+    ProcessingStats,
 )
 from gailbot.core.utils.general import delete
 from gailbot.workspace import WorkspaceManager
 from gailbot.configs import service_config_loader
+
 MERGED_FILE_NAME = "merged"
 SERVICE_CONFIG = service_config_loader()
 OUTPUT_MARKER = SERVICE_CONFIG.directory_name.hidden_file
 logger = makelogger("payload object")
+
+
 class PayLoadStatus(Enum):
-    """ For tracking the status of the file in the payload """
-    INITIALIZED = 0 
+    """For tracking the status of the file in the payload"""
+
+    INITIALIZED = 0
     TRANSCRIBING = 1
     TRANSCRIBED = 2
     ANALYZING = 3
     ANALYZED = 4
     FORMATTING = 5
     FORMATTED = 6
-    FAILED = 7 
+    FAILED = 7
+
 
 class PayLoadObject(ABC):
-    """ super class of the payloadObject, interface includes necessary method 
-        that subclass needs to implement. 
-        Payload object contains the source that is waiting to be processed, 
-        keeps track of the stage of the processes, and provides methods 
-        for pipeline to run functions to transcribe, analyze and format 
-        the data stored in payload. 
+    """super class of the payloadObject, interface includes necessary method
+    that subclass needs to implement.
+    Payload object contains the source that is waiting to be processed,
+    keeps track of the stage of the processes, and provides methods
+    for pipeline to run functions to transcribe, analyze and format
+    the data stored in payload.
     """
-    original_source : str       # path to original source, should not be modified 
-    data_files: List[str]       # stores the path to the source that is safe to be used
-    data_file_format : str
+
+    original_source: str  # path to original source, should not be modified
+    data_files: List[str]  # stores the path to the source that is safe to be used
+    data_file_format: str
     """ we can abstract setting from pipeline, 
         but transcribe component will need to have access to the interfaces 
     """
-    
+
     name: str
-    engine_setting: Dict [str, str] 
-    plugin_setting: Dict [str, str] 
-    
-    status: PayLoadStatus 
-    
+    engine_setting: Dict[str, str]
+    plugin_setting: Dict[str, str]
+
+    status: PayLoadStatus
+
     workspace: TemporaryFolder  # workspace for storing temporary file , will be deleted afterward
-    out_dir: OutputFolder       # directory where all the output will be stored 
-    merged_audio: str 
+    out_dir: OutputFolder  # directory where all the output will be stored
+    merged_audio: str
+
     # payload result
     def __init__(self, source: SourceObject, workspace: WorkspaceManager) -> None:
-        """ initialize a payload object
+        """initialize a payload object
 
         Args:
-            source (SourceObject): A source object that stores the source data 
-            workspace (WorkspaceManager): a workspace manager that provide 
+            source (SourceObject): A source object that stores the source data
+            workspace (WorkspaceManager): a workspace manager that provide
                                           functions to initialize payload output
                                           directory and payload temporary workspace
-            
-        """ 
+
+        """
         self.name = source.name
         self.original_source: str = source.source_path()
         self.setting: SettingObject = source.setting
-        self.workspace: TemporaryFolder = \
-            workspace.get_file_temp_space(self.name)        
-        self.out_dir: OutputFolder = \
-            workspace.get_output_space(source.output)
+        self.workspace: TemporaryFolder = workspace.get_file_temp_space(self.name)
+        self.out_dir: OutputFolder = workspace.get_output_space(source.output)
         self.progress_display = source.progress_display
         self.transcription_result: UttResult = UttResult(self.workspace.transcribe_ws)
         self.analysis_result: AnalysisResult = AnalysisResult()
         self.format_result: FormatResult = FormatResult(self.workspace.format_ws)
         logger.info(f"ouputspace {self.out_dir.transcribe_result}")
         self._set_initial_status()
-        self._copy_file() 
+        self._copy_file()
         self._merge_audio()
-    
+
     def _merge_audio(self):
         raise NotImplementedError()
-     
-    def _set_initial_status(self) -> None: 
+
+    def _set_initial_status(self) -> None:
         raise NotImplementedError()
-    
+
     def _copy_file(self) -> None:
         raise NotImplementedError()
-        
+
     def is_supported(file_path: str) -> bool:
         raise NotImplementedError()
-    
+
     @staticmethod
     def supported_format() -> str:
         raise NotImplementedError()
-    
-    # functions that has been implemented on abstract class 
+
+    # functions that has been implemented on abstract class
     def get_source(self) -> List[str]:
         """
         Accesses and returns a list of the current sources
         """
         return self.data_files
-    
+
     @property
     def transcribed(self) -> bool:
         """
         Check if payload object is transcribed
 
         Returns:
             bool: true if transcribed, false if not
@@ -123,130 +133,123 @@
     def analyzed(self) -> bool:
         """
         Check if payload object is analyzed
 
         Returns:
             bool: true if analyzed, false if not
         """
-        return self.status == PayLoadStatus.ANALYZED 
-    
-    @property 
+        return self.status == PayLoadStatus.ANALYZED
+
+    @property
     def formatted(self) -> bool:
         """
         Check if payload object is formatted
 
         Returns:
             bool: true if formatted, false if not
         """
         return self.status == PayLoadStatus.FORMATTED
-    
-    @property 
+
+    @property
     def failed(self) -> bool:
-        """ 
+        """
         Check if payload object failed
-        
+
         Returns:
             bool: true if failed, false if not
         """
         return self.status == PayLoadStatus.FAILED
-    
+
     def set_transcribed(self):
         """
         Sets status of payload object to TRANSCRIBED
         """
         self.status = PayLoadStatus.TRANSCRIBED
-    
+
     def set_analyzed(self):
         """
         Sets status of payload object to ANALYZED
         """
         self.status = PayLoadStatus.ANALYZED
-        
+
     def set_formatted(self):
         """
         Sets status of payload object to FORMATTED
         """
         self.status = PayLoadStatus.FORMATTED
-   
+
     def set_failure(self):
-        """ 
+        """
         set the status of the payload object to be FAILED
         """
         self.status = PayLoadStatus.FAILED
-        
-        
+
     def get_engine(self) -> str:
         """
         Accesses and returns the current engine setting
 
         Returns:
             Current engine as a string
         """
         return self.setting.engine_setting.engine
-   
+
     def get_engine_init_setting(self) -> Dict[str, str]:
         """
         Accesses and returns the engine's initial settings
 
         Returns:
             Initial settings in the form of a dictionary
         """
         return self.setting.engine_setting.get_init_kwargs()
-     
+
     def get_engine_transcribe_setting(self) -> Dict[str, str]:
         """
         Accesses and returns the engine's transcription settings
 
         Returns:
             Transcription settings in the form of a dictionary
         """
         return self.setting.engine_setting.get_transcribe_kwargs()
-    
+
     def get_plugin_setting(self) -> List[str]:
         """
         Accesses and returns the plugin settings as a list
 
         Returns:
             List of strings of the current settings
         """
         return self.setting.plugin_setting.get_data()
-    
+
     def get_status(self) -> PayLoadStatus:
         """
         Accesses and returns the payload's status
 
         Returns:
             Current PayLoadStatus
         """
         return self.status
-    
-    def set_transcription_result(
-        self, 
-        result: Dict[str, List[UttDict]]
-    )-> bool:
+
+    def set_transcription_result(self, result: Dict[str, List[UttDict]]) -> bool:
         """
         Sets the transcription result to a given dictionary
 
         Args:
             result: Dict[str, List[UttDict]]: result to set
 
         Returns:
             bool: True if successfully set, false if not
         """
         try:
             self.transcription_result.save_data(result)
-            return True 
+            return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
-    def set_format_result(
-        self, 
-        result: Dict[str, FormatResultDict]
-    ) -> bool:
+
+    def set_format_result(self, result: Dict[str, FormatResultDict]) -> bool:
         """
         Sets the format result to a given dictionary
 
         Args:
             result: Dict[str, FormatResultDict]: result to set
 
         Returns:
@@ -254,19 +257,16 @@
         """
         try:
             self.format_result.save_data(result)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
-    def set_analysis_result(
-        self, 
-        result: Dict[str, AnalysisResultDict]
-    ) -> bool:
+
+    def set_analysis_result(self, result: Dict[str, AnalysisResultDict]) -> bool:
         """
         Sets the analysis result to a given dictionary
 
         Args:
             result: Dict[str, FormatResultDict]: result to set
 
         Returns:
@@ -274,155 +274,154 @@
         """
         try:
             self.analysis_result.save_data(result)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def set_transcription_process_stats(
-        self, 
-        stats: ProcessingStats
+        self, stats: ProcessingStats
     ) -> Dict[str, List[UttDict]]:
         """
         Sets the transcription processing stats.
 
         Args:
             stats:ProcessingStats: stats to set
         """
         return self.transcription_result.set_processing_stats(stats)
-    
+
     def set_analysis_process_stats(
-        self, 
-        stats:ProcessingStats
+        self, stats: ProcessingStats
     ) -> Dict[str, List[UttDict]]:
         """
         Sets the analysis processing stats.
 
         Args:
             stats:ProcessingStats: stats to set
         """
         return self.analysis_result.set_processing_stats(stats)
 
     def set_format_process_stats(
-        self, 
-        stats:ProcessingStats
+        self, stats: ProcessingStats
     ) -> Dict[str, List[UttDict]]:
         """
         Sets the formal processing stats.
 
         Args:
             stats:ProcessingStats: stats to set
         """
         return self.format_result.set_processing_stats(stats)
-    
+
     def get_transcription_result(self) -> Dict[str, List[UttDict]]:
         """
         Accesses the result of the current transcription
 
         Returns:
-            Transcription result in the form of a dictionary mapping strings 
+            Transcription result in the form of a dictionary mapping strings
             to lists of utterance dictionaries
         """
         return self.transcription_result.get_data()
-    
+
     def get_format_result(self) -> FormatResultDict:
         """
         Accesses the result of the current formatting
 
         Returns:
             Transcription result in the form of a FormatResultDict
         """
         return self.format_result.get_data()
-    
+
     def get_analyze_result(self) -> Dict[str, AnalysisResultDict]:
         """
         Accesses the result of the current analysis
 
         Returns:
-            Transcription result in the form of a dictionary mapping strings 
+            Transcription result in the form of a dictionary mapping strings
             to AnalysisResultDicts
         """
         return self.analysis_result.get_data()
-    
-    def output_transcription_result(self) -> bool: 
+
+    def output_transcription_result(self) -> bool:
         """
         Outputs the current transcription result to the output directory
 
         Returns:
             bool: true if successfully outputted, false if not
         """
         try:
             logger.info(self.out_dir.transcribe_result)
             assert self.transcription_result.output(self.out_dir.transcribe_result)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def output_meta_result(self) -> bool:
         """
         Outputs the current formatting result to the output directory
 
         Returns:
             bool: true if successfully outputted, false if not
         """
         metadata = {
             "Profile Setting": self.setting.get_data(),
             "Date": datetime.now().strftime("%Y-%m-%d %H:%M"),
             "Source": self.original_source,
             "Raw Audio": self.data_files,
-            "Plugin Results": self.analysis_result.get_data(), 
+            "Plugin Results": self.analysis_result.get_data(),
         }
         try:
             write_json(self.out_dir.metadata, metadata)
-            return True 
+            return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
+
     def output_analysis_result(self) -> bool:
         """
         Outputs the current analysis result to the output directory
 
         Returns:
             bool: true if successfully outputted, false if not
         """
         try:
             assert self.analysis_result.output(self.out_dir.analysis_result)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def output_format_result(self) -> bool:
-        """ 
+        """
         Outputs the current format result to the output directory
         """
         try:
             assert self.format_result.output(self.out_dir.format_result)
-            return True 
+            return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def save(self):
         """
         Saves the file and outputs all results to output directory
         """
         logger.info("saving the file")
         logger.info(self.out_dir.root)
         assert self.output_analysis_result()
         assert self.output_meta_result()
         assert self.output_transcription_result()
         assert self.output_format_result()
         with open(os.path.join(self.out_dir.root, OUTPUT_MARKER), "w+") as f:
             f.write(f"{self.name}")
         for file in self.data_files:
             if is_file(file):
-                copy(file, os.path.join(self.out_dir.media_file, os.path.basename(file)))
-        
+                copy(
+                    file, os.path.join(self.out_dir.media_file, os.path.basename(file))
+                )
+
     def clear_temporary_workspace(self):
         delete(self.workspace.root)
-    
+
     def __repr__(self) -> str:
-        return f"payload object {self.name}"
+        return f"payload object {self.name}"
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/payload/transcribedDirPayload.py` & `GailBot-0.2a0/src/gailbot/services/converter/payload/transcribedDirPayload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,103 +1,115 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:37:15
 from typing import Union
-import os 
+import os
 
 from .payloadObject import PayLoadObject, PayLoadStatus
 from ...organizer.source import SourceObject
 from gailbot.core.utils.general import is_directory, is_file, copy
 from gailbot.core.utils.logger import makelogger
 from gailbot.workspace.manager import WorkspaceManager
 from gailbot.configs import service_config_loader, workspace_config_loader
 
 HIDDEN_FILE = service_config_loader().directory_name.hidden_file
 OUTPUT_RESULT = workspace_config_loader().get_output_structure().transcribe_result
 logger = makelogger("transcribed_dir_payload")
 MERGED_FILE_NAME = "merged"
 
+
 def load_transcribed_dir_payload(
-    source: SourceObject, ws_manager: WorkspaceManager) -> Union[bool, PayLoadObject]:
-    """ given a source object, convert it into an PayloadObject  
-        if the source stores a gailbot output directory that contains 
-        the gailbot output result 
-    
+    source: SourceObject, ws_manager: WorkspaceManager
+) -> Union[bool, PayLoadObject]:
+    """given a source object, convert it into an PayloadObject
+        if the source stores a gailbot output directory that contains
+        the gailbot output result
+
     Args:
-        source (SourceObject): an instance of SourceObject that stores the 
+        source (SourceObject): an instance of SourceObject that stores the
         datafile and setting of the transcription
 
     Returns:
-        Union[bool, List[PayLoadObject]]: return the converted payload if the 
+        Union[bool, List[PayLoadObject]]: return the converted payload if the
         conversion is successful, return false other wise
     """
     if not source.setting:
         return False
     if not TranscribedDirPayload.is_supported(source.source_path()):
         return False
-    try: 
+    try:
         return [TranscribedDirPayload(source, ws_manager)]
     except Exception as e:
         logger.error(e, exc_info=e)
         return False
 
+
 class TranscribedDirPayload(PayLoadObject):
     """
     Class for a transcribed directory payload
     """
+
     def __init__(self, source: SourceObject, ws_manager: WorkspaceManager) -> None:
-        super().__init__(source, ws_manager) 
+        super().__init__(source, ws_manager)
         if not self.transcription_result.load_result(
-            os.path.join(self.data_files[0], OUTPUT_RESULT)):
+            os.path.join(self.data_files[0], OUTPUT_RESULT)
+        ):
             logger.error("result cannot be loaded")
             self.status = PayLoadStatus.INITIALIZED
-    
+
     @staticmethod
     def is_supported(file_path: str) -> bool:
         """
         Determines if a given file path has a supported file extension
 
         Args:
             file_path: str: name of the file path to check
 
         Returns:
             bool: True if the file path is supported, false if not
         """
         if not is_directory(file_path):
-            return False 
+            return False
         return is_file(os.path.join(file_path, HIDDEN_FILE))
-       
+
     def _copy_file(self) -> None:
         """
         Copies file to workspace
         """
         tgt_path = os.path.join(self.workspace.data_copy, f"{self.name}")
         copy(self.original_source, tgt_path)
         self.data_files = [tgt_path]
-    
+
     def _set_initial_status(self) -> None:
         """
         Sets the initial status of the payload object to initialized
         """
         self.status = PayLoadStatus.TRANSCRIBED
-    
+
     def _merge_audio(self):
-        try: 
+        try:
             for root, dirs, files in os.walk(self.original_source):
                 for file in files:
                     file_name, file_extension = os.path.splitext(file)
                     if file_name == MERGED_FILE_NAME:
                         logger.info(file)
-                        merged_path = copy(os.path.join(root,file), self.out_dir.media_file)
+                        merged_path = copy(
+                            os.path.join(root, file), self.out_dir.media_file
+                        )
                         self.merged_audio = merged_path
                         assert merged_path
                         break
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
+
     @staticmethod
     def supported_format() -> str:
         """
         Contains and accesses a list of the supported formats
         """
         return "transcribed directory"
 
     def __repr__(self) -> str:
-        return "Transcribed directory payload"
+        return "Transcribed directory payload"
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/payload/videoPayload.py` & `GailBot-0.2a0/src/gailbot/services/converter/payload/videoPayload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-import os 
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-31 16:21:27
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:37:16
+import os
 from .payloadObject import PayLoadObject, PayLoadStatus
 from ...organizer.source import SourceObject
 from typing import List, Union
-from gailbot.core.utils.general import (
-    get_extension, 
-    copy
-)
+from gailbot.core.utils.general import get_extension, copy
+
 """ NOTE: currently unused and not tested since gailbot does not support 
           for video transcription yet
 """
+
+
 def load_video_payload(source: SourceObject) -> Union[bool, List(PayLoadObject)]:
     """
     Loads an instance of the video payload with a given source object
     """
     if not source.setting:
         return False
     if not VideoPayload.is_supported(source.source_path):
         return False
     try:
         return [VideoPayload(source)]
     except:
         return False
-    
+
+
 class VideoPayload(PayLoadObject):
     def __init__(self, source) -> None:
         super().__init__(source)
-    
-    @staticmethod 
+
+    @staticmethod
     def is_supported(file_path: str) -> bool:
         """
         Determines if a given file path has a supported file extension
 
         Args:
             file_path: str: name of the file path to check
 
@@ -40,33 +46,33 @@
         return super().is_supported(file_path)
 
     def _copy_file(self) -> None:
         """
         Copies file to workspace
         """
         extension = get_extension(self.original_source)
-        tgt_path =os.path.join(self.workspace.data_copy, f"{self.name},{extension}")
+        tgt_path = os.path.join(self.workspace.data_copy, f"{self.name},{extension}")
         copy(self.original_source, tgt_path)
         self.data_files = [tgt_path]
-    
+
     def _set_initial_status(self) -> None:
         """
         Sets the initial status of the payload object to initialized
         """
         self.status = PayLoadStatus.INITIALIZED
-        
+
     @staticmethod
     def supported_format() -> str:
         """
         Contains and accesses a list of the supported formats
         """
         """ TODO: add the format """
         return ["mp4"]
-        
+
     def _convert_to_audio(self) -> bool:
         """
         Converts video file to audio file
         """
         raise NotImplementedError()
 
     def __repr__(self) -> str:
-        return "Video payload"
+        return "Video payload"
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/plugin/pluginMethod.py` & `GailBot-0.2a0/src/gailbot/services/converter/plugin/pluginMethod.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,169 +1,185 @@
-import os 
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:37:35
+import os
 from typing import Dict, Union, List, Any
 from gailbot.core.utils.general import write_toml, read_toml
 from ..payload.payloadObject import PayLoadObject, MERGED_FILE_NAME
 from gailbot.services.converter.result import UttDict
 from gailbot.plugins import Methods
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.utils.general import (
-    get_name, 
+    get_name,
     get_extension,
-    is_directory, 
+    is_directory,
     make_dir,
     write_csv,
     write_json,
     write_toml,
     write_yaml,
-    write_txt)
+    write_txt,
+)
 
 from pydantic import BaseModel
+
 MERGED = "merged.wav"
 
 logger = makelogger("pluginMethod")
 
 
 class UttObj(BaseModel):
-    start: float 
-    end: float 
-    speaker: str 
+    start: float
+    end: float
+    speaker: str
     text: str
 
+
 class GBPluginMethods(Methods):
     format_to_out_fun = {
-        "csv" : write_csv,
+        "csv": write_csv,
         "toml": write_toml,
         "yaml": write_yaml,
         "json": write_json,
-        "txt": write_txt
+        "txt": write_txt,
     }
-    
-    def __init__(self, payload: PayLoadObject, plugin_suite:str):
+
+    def __init__(self, payload: PayLoadObject, plugin_suite: str):
         self.payload: PayLoadObject = payload
         self.plugin_suite = plugin_suite
-        
-        self.work_path = os.path.join(self.payload.workspace.analysis_ws, self.plugin_suite)
+
+        self.work_path = os.path.join(
+            self.payload.workspace.analysis_ws, self.plugin_suite
+        )
         if not is_directory(self.work_path):
             make_dir(self.work_path)
-        
-        self.out_path = os.path.join(self.payload.out_dir.analysis_result, self.plugin_suite)
+
+        self.out_path = os.path.join(
+            self.payload.out_dir.analysis_result, self.plugin_suite
+        )
         if not is_directory(self.out_path):
             make_dir(self.out_path)
-        
+
     def get_audio_path(self) -> Dict[str, str]:
         """
         Returns a dictionary that maps the audio name to the audio source
         """
         return {get_name(path): path for path in self.payload.data_files}
-    
-    @property 
+
+    @property
     def merged_media(self):
-        """ 
-        return the path to the merged media file 
+        """
+        return the path to the merged media file
         """
         return self.payload.merged_audio
-        
+
     @property
     def filenames(self) -> List[str]:
         """
-        return the list of data file name 
+        return the list of data file name
         """
         return [get_name(file) for file in self.payload.data_files]
 
     @property
-    def utterances(self) -> Dict[str,List[UttDict]]:
-        """ 
+    def utterances(self) -> Dict[str, List[UttDict]]:
+        """
         Accesses and returns the utterance data
 
         Returns:
-            Dict[str,Dict]: return dictionary that maps audio name to the 
-                            transcription result  
+            Dict[str,Dict]: return dictionary that maps audio name to the
+                            transcription result
         """
         try:
             return self.payload.get_transcription_result()
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-                
+
     @property
     def temp_work_path(self) -> str:
         """
         Accesses and returns the temporary workspace path
 
         Returns:
             String containing the temporary workspace path
         """
         return self.work_path
-   
+
     @property
     def output_path(self) -> str:
         """
         Accesses and returns the output path
 
         Returns:
             String containing the output path
         """
         return self.out_path
-    
-    def get_utterance_objects(self) -> Dict[str, List[UttObj]]: 
-        """ 
-        Access and return the utterance data as utterance object 
+
+    def get_utterance_objects(self) -> Dict[str, List[UttObj]]:
+        """
+        Access and return the utterance data as utterance object
         """
         res = dict()
         data = self.payload.get_transcription_result()
-        for key, uttlist in data.items(): 
+        for key, uttlist in data.items():
             newlist = list()
             for utt in uttlist:
                 # NOTE: added since whisper returns none for undetected
-                #       speaker; may need to move this logic to plugin 
+                #       speaker; may need to move this logic to plugin
                 if not utt["speaker"]:
                     utt["speaker"] = "speaker_00"
                 newlist.append(UttObj(**utt))
             res[key] = newlist
         return res
-    
-    
-    def save_item(self, 
-                  data: Union [Dict[str, Any], List],
-                  name: str, 
-                  temporary: bool = True, 
-                  format: str = "json", 
-                  fun: callable = None,
-                  kwargs = None) -> bool :
+
+    def save_item(
+        self,
+        data: Union[Dict[str, Any], List],
+        name: str,
+        temporary: bool = True,
+        format: str = "json",
+        fun: callable = None,
+        kwargs=None,
+    ) -> bool:
         """function provided for the plugin to save file
 
         Args:
             data (Union[Dict[str, Any], List]): the data that will be outputed
             name (str): the name of the output file
-            temporary (bool, optional): if true, the file will be stored in 
-                                        temporary folder and discarded once the 
+            temporary (bool, optional): if true, the file will be stored in
+                                        temporary folder and discarded once the
                                         analysis process finishes. Defaults to True.
             format (str, optional): the format of the output file. Defaults to "json".
-            fun (callable, optional): user defined function to write the 
+            fun (callable, optional): user defined function to write the
                                       output. Defaults to None.
-            kwargs (dict, optional): user defined key word arguments that will 
-                                    be passed into user defined function. 
+            kwargs (dict, optional): user defined key word arguments that will
+                                    be passed into user defined function.
                                     Defaults to None.
 
         Returns:
-            bool: return true if the plugin is registered successfully , false otherwise 
+            bool: return true if the plugin is registered successfully , false otherwise
         """
         logger.info("plugin method, saving item is called")
         logger.info(data)
-        path = os.path.join(self.work_path, name + "." + format) if temporary else \
-               os.path.join(self.out_path,  name + "." + format)
+        path = (
+            os.path.join(self.work_path, name + "." + format)
+            if temporary
+            else os.path.join(self.out_path, name + "." + format)
+        )
         if fun:
             try:
                 fun(path, data, **kwargs)
                 return True
             except Exception as e:
                 logger.error(e, exc_info=e)
                 return False
         if format not in self.format_to_out_fun:
             logger.error("the output format is not supported")
-            return False 
+            return False
         try:
-            self.format_to_out_fun[format](path, data) 
+            self.format_to_out_fun[format](path, data)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
-            return False
+            return False
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/result/analysis.py` & `GailBot-0.2a0/src/gailbot/services/converter/result/analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-from typing import TypedDict,  Dict, List 
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:37:45
+from typing import TypedDict, Dict, List
 
 from .resultInterface import ResultInterface
 from gailbot.core.utils.logger import makelogger
+
 logger = makelogger("analysis-result")
 
+
 class AnalysisResultDict(TypedDict):
     plugin_suite: str
     success: List[str]
     failure: List[str]
 
+
 class AnalysisResult(ResultInterface):
     """
     Defines a class for the analysis result
     """
+
     def __init__(self):
-        self.data : Dict[str, AnalysisResultDict]= dict() 
-    
+        self.data: Dict[str, AnalysisResultDict] = dict()
+
     def save_data(self, data) -> bool:
         """
-        Saves the result data 
+        Saves the result data
 
         Args:
-            data: [AnalysisResultDict]: data to save, in the form 
+            data: [AnalysisResultDict]: data to save, in the form
             of a dictionary mapping strings to analysis results
 
         Returns:
             Bool: True if successfully saved, false if not
         """
         self.data = data
         return True
 
     def output(self, path) -> bool:
-        """ NOTE: currently no data for analysis will be written """
+        """NOTE: currently no data for analysis will be written"""
         try:
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return True
-        
+
     def get_data(self):
         """
         Accesses and object's data
 
         Returns:
             Data in the form Dict[str, AnalysisResultDict]
         """
-        return self.data 
+        return self.data
```

### Comparing `GailBot-0.1a9/src/gailbot/services/converter/result/transcribe.py` & `GailBot-0.2a0/src/gailbot/services/converter/result/transcribe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,197 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:38:16
 
-import os 
+import os
 from typing import TypedDict, List, Dict
 
 from gailbot.core.utils.general import (
-    write_csv, 
+    write_csv,
     read_csv,
-    write_json, 
-    get_name, 
+    write_json,
+    get_name,
     make_dir,
-    read_json, 
-    paths_in_dir, 
-    is_directory, 
-    is_file)
+    read_json,
+    paths_in_dir,
+    is_directory,
+    is_file,
+)
 from gailbot.core.utils.logger import makelogger
 from gailbot.configs import service_config_loader
 from .resultInterface import ResultInterface
 
 SERVICE_CONFIG = service_config_loader()
 logger = makelogger("transcribe_result")
 
 """
 TODO: 
 use .pickle to store temporary file to save memory
 """
+
+
 class UttDict(TypedDict):
     """
     Defines a class for the utterance dictionary
     """
-    speaker: str 
-    start_time: str 
-    end_time:str 
-    text:str 
-    
+
+    speaker: str
+    start: str
+    end: str
+    text: str
+
+
 class UttResult(ResultInterface):
     """
     Defines a class containing the utterance results of a transcription
     """
+
     def __init__(self, workspace: str, data: Dict[str, List[UttDict]] = None) -> None:
-        self.workspace = os.path.join(workspace, SERVICE_CONFIG.directory_name.temp_result)
+        self.workspace = os.path.join(
+            workspace, SERVICE_CONFIG.directory_name.temp_result
+        )
         make_dir(self.workspace, overwrite=True)
-        self.max_size = 1000 # TODO: move to toml 
-        self.data = data 
-        self.filenames :  Dict [str, str] = dict()
+        self.max_size = 1000  # TODO: move to toml
+        self.data = data
+        self.filenames: Dict[str, str] = dict()
         self.saved_to_disk: bool = False
-            
-    def save_data(
-        self, 
-        data: Dict[str, List[UttDict]]
-    ) -> bool:
+
+    def save_data(self, data: Dict[str, List[UttDict]]) -> bool:
         """
         Saves the given data to the output directory
 
-        Args:  
+        Args:
             data: Dict[str, List[UttDict]]: data to save
-        
+
         Returns:
             bool: True if successfully saved, false if not
         """
-        if len(data) == 0: 
+        if len(data) == 0:
             logger.error("the result is empty")
             return False
-        try: 
+        try:
             for name, result in data.items():
-                path = os.path.join(self.workspace, f"{name}.json")  
+                path = os.path.join(self.workspace, f"{name}.json")
                 write_json(path, result)
                 if name not in self.filenames:
                     self.filenames[name] = path
             self.saved_to_disk = True
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-           
+
     def output(self, path) -> bool:
         """
         Outputs the result to the output directory
 
         Args:
             path: output directory path
-        
+
         Returns:
             bool: True if successfully outputted, false if not
         """
         try:
             if self.saved_to_disk:
                 data = self.get_data()
-            else: 
-                data = self.data 
+            else:
+                data = self.data
             for name, result in data.items():
                 logger.info(path)
                 logger.info(name)
                 write_csv(os.path.join(path, name + ".csv"), result)
             return True
         except Exception as e:
             logger.error(f"the path is {path}")
             logger.error(e, exc_info=e)
         return False
-    
+
     def get_data(self) -> Dict[str, List[UttDict]]:
         """
         Accesses and returns the data of the current transcription result
 
         Returns:
             Data in the form Dict[str, List[UttDict]]
         """
         if self.saved_to_disk:
             files = paths_in_dir(self.workspace, ["json"])
             res = dict()
-            for file in files: 
+            for file in files:
                 res[get_name(file)] = read_json(file)
-            return res 
+            return res
         else:
-            return self.data 
-   
-    def get_one_file_data(self, name:str) -> Dict[str, List[UttDict]]:
-        """
-        Accesses and return the data of one file 
-
-        Args: 
-            name: the filename of one file 
-            
-        Return: a dictionary that contains the utterance data, the key of the 
-                dictionary will be the file name, and the value will be the 
+            return self.data
+
+    def get_one_file_data(self, name: str) -> Dict[str, List[UttDict]]:
+        """
+        Accesses and return the data of one file
+
+        Args:
+            name: the filename of one file
+
+        Return: a dictionary that contains the utterance data, the key of the
+                dictionary will be the file name, and the value will be the
                 list of utterance dictionary that stores the utterance data
-        """ 
+        """
         res = dict()
         path = self.filenames[name]
         res[name] = read_json(path)
-        return res 
-        
-        
+        return res
+
     def load_result(self, path: str) -> bool:
         """
         Loads the transcription result
 
         Args:
-            Path:str: path to the input 
+            Path:str: path to the input
 
-        Returns: 
-            Result in the form Dict[str, List[UttDict]] or false if not 
+        Returns:
+            Result in the form Dict[str, List[UttDict]] or false if not
             successfully accessed
         """
         if is_file(path):
             return self._read_from_file(path)
         elif is_directory(path):
             return self._read_from_dir(path)
-        else: 
+        else:
             return False
-    
+
     def _read_from_dir(self, path) -> Dict[str, List[UttDict]]:
         """
         Processes the result of a directory input
 
         Args:
             path: path to the directory to process
-        
+
         Returns:
             Dict[str, List[UttDict]]: dictionary containing the processed input
         """
         try:
             files = paths_in_dir(path, ["csv"])
             res = dict()
             for file in files:
                 res[get_name(file)] = read_csv(file)
             if res:
                 assert self.save_data(res)
-            return True 
+            return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def _read_from_file(self, path: str) -> Dict[str, List[UttDict]]:
         """
         Processes the result of a file input
 
         Args:
             path: path to the file to process
-        
+
         Returns:
             Dict[str, List[UttDict]]: dictionary containing the processed input
         """
         try:
             res = {get_name(path): read_csv(path)}
             assert self.save_data(res)
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/organizer.py` & `GailBot-0.2a0/src/gailbot/services/organizer/organizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,358 +1,373 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 14:30:48
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-04 15:23:04
 from typing import Dict, List, Union, Callable
 
 from .source import SourceObject, SourceManager
 from gailbot.core.utils.logger import makelogger
 from .settings import SettingManager, SettingObject, SettingDict
 from gailbot.configs import default_setting_loader
 
 logger = makelogger("organizer")
-CONFIG = default_setting_loader() 
-DEFAULT_SETTING_NAME = CONFIG.profile_name 
-DEFAULT_SETTING = CONFIG.profile_data 
+CONFIG = default_setting_loader()
+DEFAULT_SETTING_NAME = CONFIG.profile_name
+DEFAULT_SETTING = CONFIG.profile_data
 DEFAULT_ENGINE_NAME = CONFIG.engine_name
 DEFAULT_ENGINE_SETTING = CONFIG.engine_data
+
+
 class Organizer:
-    def __init__(self, setting_workspace: str, load_exist_setting: bool = False) -> None:
+    def __init__(
+            self, setting_workspace: str, load_exist_setting: bool = False
+    ) -> None:
         self.setting_manager = SettingManager(setting_workspace, load_exist_setting)
-        self.source_manager  = SourceManager()
-        
+        self.source_manager = SourceManager()
+
     def add_source(self, source_path: str, output: str) -> Union[str, bool]:
         """
         Adds given source to the output directory
 
         Args:
             source_path: str: path to the source to add
             output: str: path to the output directory
 
-        Returns: 
+        Returns:
             Union[str, bool]: return the name if successfully added, false if not
         """
+        logger.info(f"source_path: {source_path}, output: {output}")
         try:
             name = self.source_manager.add_source(source_path, output)
+            self.apply_setting_to_source(name, self.get_default_profile_setting_name())
             assert name
             return name
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def remove_source(self, source_name: str) -> bool:
         """
         Removes given source
 
         Args:
             source_path: str: path to the source to remove
 
-        Returns: 
+        Returns:
             bool: True if successfully removed, false if not
         """
         return self.source_manager.remove_source(source_name)
-    
+
     def is_source(self, source_name: str) -> bool:
         """
         Determines if given name corresponds to an existing source
 
         Args:
             source_name: str: name of potential source
 
         Returns:
             bool: true if the name corresponds to an existing source, false if not
         """
         return self.source_manager.is_source(source_name)
-    
-    def get_source(self, source_name: str) -> Union [bool, SourceObject]:
+
+    def get_source(self, source_name: str) -> Union[bool, SourceObject]:
         """
         Accesses source with a given name
 
         Args:
             source_name: str: source name to access
 
-        Returns:    
+        Returns:
             Source object associated with the given name or false if source object is not found
         """
         return self.source_manager.get_source(source_name)
-    
-    def get_source_outdir(self, source_name: str) -> Union [bool, str]:
+
+    def get_all_source_names(self) -> List[str]:
+        """
+        Returns list of all source names
+
+        Returns: List[str] : list of source names
+        """
+        return self.source_manager.source_names()
+
+    def get_source_outdir(self, source_name: str) -> Union[bool, str]:
         """
         Accesses source output directory with a given name
 
         Args:
             source_name: str: source name to access
 
-        Returns:    
+        Returns:
             a string stores the output of the source
         """
 
         return self.source_manager.get_source_outdir(source_name)
-    
+
     def get_source_setting(self, source_name: str) -> SettingObject:
         """
         Accesses the settings of a source with a given name
 
         Args:
             source_name: str: source name whose setting to access
 
-        Returns:    
+        Returns:
             Source settings associated with the given name or false if source object is not found
         """
         return self.source_manager.get_source_setting(source_name)
-    
+
     def is_setting_applied(self, source_name: str) -> bool:
         """
         Determines if a given source has configured settings
 
         Args:
             source_name: str: source name to access
 
         Returns:
             bool: True if given source is configured, false if not
         """
         return self.source_manager.is_source_configured(source_name)
-    
+
     def apply_setting_to_source(
-        self, source_name: str, setting_name:str, overwrite: bool = True) -> bool:
-        """apply setting to a source 
+            self, source_name: str, setting_name: str, overwrite: bool = True
+    ) -> bool:
+        """apply setting to a source
 
         Args:
             sources (str): a string that identifies the source
             setting (str): the setting name
-            overwrite (bool, optional): if true, overwrites  the existing setting 
+            overwrite (bool, optional): if true, overwrites  the existing setting
             . Defaults to True.
 
         Returns:
             bool: return true if settings can be applied
         """
         return self.source_manager.apply_setting_profile_to_source(
-            source_name, self.get_setting_obj(setting_name), overwrite)
+            source_name, self.get_setting_obj(setting_name), overwrite
+        )
 
     def apply_setting_to_sources(
-        self, sources: List[str], setting_name:str, overwrite: bool = True)-> bool:
+            self, sources: List[str], setting_name: str, overwrite: bool = True
+    ) -> bool:
         """apply setting to a list of sources
 
         Args:
             sources (List[str]): a list of string that identifies the sources
             setting (str): the setting name
-            overwrite (bool, optional): if true, overwrites  the existing setting 
+            overwrite (bool, optional): if true, overwrites  the existing setting
             . Defaults to True.
 
         Returns:
             bool: return true if settings can be applied
         """
         try:
             for source in sources:
                 logger.info(f"organizer change {source} setting to {setting_name}")
                 assert self.apply_setting_to_source(source, setting_name, overwrite)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
+
     def add_progress_display(self, source_name: str, displayer: Callable):
-        """ add a displayer function to the source to track the progress of the 
-            source in the pipeline 
+        """add a displayer function to the source to track the progress of the
+            source in the pipeline
 
         Args:
             source_name (str): the name of the source
-            displayer (Callable): a callable function that only takes in 
-                                  one argument that stores the progress message 
+            displayer (Callable): a callable function that only takes in
+                                  one argument that stores the progress message
                                   as a string
 
         Returns:
             bool: true if the displayer is added correctly, false other wise
         """
         return self.source_manager.add_progress_display(source_name, displayer)
-     
-    def create_new_setting(
-        self, setting_name: str, setting: SettingDict) -> bool: 
-        """ create a new setting
+
+    def create_new_setting(self, setting_name: str, setting: SettingDict, overwrite: bool = True) -> bool:
+        """create a new setting
 
         Args:
-            name (str): the name of the setting
+            setting_name (str): the name of the setting
             setting (Dict[str, str]): the setting content
+            overwrite (Boolean): if true, overwrite existing profile with the same name
 
         Returns:
-            bool: return true if the setting can be created, if the setting uses 
+            bool: return true if the setting can be created, if the setting uses
                   an existing name, the setting cannot be created
-        """ 
-        return self.setting_manager.add_new_setting(setting_name, setting)
-    
+        """
+        return self.setting_manager.add_new_setting(setting_name, setting, overwrite)
+
     def save_setting_profile(self, setting_name: str) -> str:
-        """ save the setting locally on the disk
+        """save the setting locally on the disk
 
         Args:
             setting_name (str): the setting name of the setting
 
         Returns:
-            bool: return true if the setting is saved correctly 
+            bool: return true if the setting is saved correctly
         """
         return self.setting_manager.save_setting(setting_name)
-    
-   
+
     def rename_setting(self, setting_name: str, new_name: str) -> bool:
         """rename a setting
 
         Args:
             old_name (str): the old name that identifies the setting
             new_name (str): the new name of the setting
 
         Returns:
-            bool: return true if the setting can be renamed correctly, 
+            bool: return true if the setting can be renamed correctly,
                   return false if the new setting name has been taken
         """
         try:
             self.setting_manager.rename_setting(setting_name, new_name)
             return True
         except:
             return False
-        
-   
+
     def remove_setting(self, setting_name: str) -> bool:
-        """remove a setting 
+        """remove a setting
 
         Args:
             setting_name (str): the name of the setting that will be removed
 
         Returns:
-            bool: true if the setting is removed, false otherwise 
+            bool: true if the setting is removed, false otherwise
         """
         if not self.setting_manager.is_setting(setting_name):
-            return False 
+            return False
         try:
             assert self.setting_manager.remove_setting(setting_name)
-            sources = self.source_manager.get_sources_with_setting(setting_name) 
+            sources = self.source_manager.get_sources_with_setting(setting_name)
             for source in sources:
                 self.remove_setting_from_source(source)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
-    
-    def update_setting(self, setting_name:str, new_setting: Dict[str,str]) -> bool:
+
+    def update_setting(self, setting_name: str, new_setting: Dict[str, str]) -> bool:
         """updating the setting with new setting content
 
         Args:
-            setting_name (str): the setting name that identifies the setting 
+            setting_name (str): the setting name that identifies the setting
             new_setting (SettingDict): the content of the new settings
 
         Returns:
             bool: return true if the setting can be updated correctly
         """
         return self.setting_manager.update_setting(setting_name, new_setting)
-        
-    def get_setting_obj(self, setting_name:str) -> SettingObject:
-        """ get setting object that is identified by setting name
+
+    def get_setting_obj(self, setting_name: str) -> SettingObject:
+        """get setting object that is identified by setting name
 
         Args:
             setting_name (str): the name that identifies the setting object
 
         Returns:
             SettingObject: a setting object that stores the setting data
         """
-        return self.setting_manager.get_setting(setting_name)    
-    
+        return self.setting_manager.get_setting(setting_name)
 
-    def get_setting_dict(self, setting_name:str) -> Union[bool, SettingDict]:
-        """ given a source name, return the setting content of the source 
-            in a dictionary 
+    def get_setting_dict(self, setting_name: str) -> Union[bool, SettingDict]:
+        """given a source name, return the setting content of the source
+            in a dictionary
 
         Args:
             source_name (str): name that identifies a source
 
         Returns:
-            Union[bool, SettingDict]: if the source is found, returns its setting 
-            content stored in a dictionary, else returns false  
+            Union[bool, SettingDict]: if the source is found, returns its setting
+            content stored in a dictionary, else returns false
         """
         return self.setting_manager.get_setting_dict(setting_name)
-    
 
-    def is_setting(self, setting_name: str) -> bool: 
+    def is_setting(self, setting_name: str) -> bool:
         """check if a setting exists or not
 
         Args:
             name (str): names that identifies the settings
 
         Returns:
             bool: return true if the setting exists, false otherwise
         """
         return self.setting_manager.is_setting(setting_name)
-    
-    
+
     def is_setting_in_use(self, setting_name: str) -> bool:
         """check if a setting is being used by any source
 
         Args:
             setting_name (str): the name of the setting
 
         Returns:
             bool: return true if the setting is being used, false otherwise
         """
         src_with_set = self.source_manager.get_sources_with_setting(setting_name)
-        if len(src_with_set) == 0 : 
-            return False 
+        if len(src_with_set) == 0:
+            return False
         else:
             return True
-    
+
     def remove_setting_from_source(self, source_name: str) -> bool:
-        """ given a source name, remove the current setting from the source, 
+        """given a source name, remove the current setting from the source,
             set the setting of the source to default
 
         Args:
             source_name (str): the name that identifies the source
 
         Returns:
             bool: return true if the setting is removed successfully false otherwise
         """
-        return self.apply_setting_to_source(
-            source_name, DEFAULT_SETTING_NAME, True)
-    
+        return self.apply_setting_to_source(source_name, DEFAULT_SETTING_NAME, True)
+
     def get_plugin_setting(self, name: str):
-        """ returns the plugin setting of the setting
+        """returns the plugin setting of the setting
 
         Args:
             setting_name (str): name that identifies a setting
 
         Returns:
-            Union[bool, Dict[str, str]]: if the setting is found, return the 
-            list of string that identifies which plugins are used, else return 
+            Union[bool, Dict[str, str]]: if the setting is found, return the
+            list of string that identifies which plugins are used, else return
             false
         """
         setting: SettingObject = self.setting_manager.get_setting(name)
         if setting:
             return setting.get_plugin_setting()
         else:
             return False
-    
-    def get_configured_sources(self, sources : List[str] = None) -> List[SourceObject]:
-        """ given the  a list of source name, return a list of the sourceObject
+
+    def get_configured_sources(self, sources: List[str] = None) -> List[SourceObject]:
+        """given the  a list of source name, return a list of the sourceObject
             that stores the source configured with setting
         Args:
-            sources (List[str], optional): a list of source name, if not 
+            sources (List[str], optional): a list of source name, if not
             given, return a list of configured source. Defaults to None.
 
         Returns:
-            List[SourceObject]: a list of source object that stores the source data 
+            List[SourceObject]: a list of source object that stores the source data
         """
         return self.source_manager.get_configured_sources(sources)
-   
-    def get_engine_setting_names(self) -> List[str]: 
-        """ get a list of available engine setting name
+
+    def get_engine_setting_names(self) -> List[str]:
+        """get a list of available engine setting name
 
         Returns:
             List[str]: the list of engine setting name
         """
         return self.setting_manager.get_engine_setting_names()
-    
-    def add_new_engine(self, name, setting, overwrite = False) -> bool:
-        """ add a new engine setting 
+
+    def add_new_engine(self, name, setting, overwrite=False) -> bool:
+        """add a new engine setting
 
         Args:
             name (str): the name of the engine setting
             setting (Dict[str, str]): the setting data stored in a dictionary
-            overwrite (bool, optional): if True, overwrite the existing 
+            overwrite (bool, optional): if True, overwrite the existing
                                         engine setting with the same name. Defaults to False.
 
         Returns:
             bool: return True if the engine setting is successfully created
         """
         return self.setting_manager.add_new_engine(name, setting, overwrite)
 
@@ -362,159 +377,155 @@
         Args:
             name (str): the name of the engine setting to be removed
 
         Returns:
             bool:  return True if the engine setting is successfully removed
         """
         return self.setting_manager.remove_engine_setting(name)
-    
+
     def update_engine_setting(self, name, setting_data: Dict[str, str]) -> bool:
-        """update the engine setting identified by name 
+        """update the engine setting identified by name
 
         Args:
             name (str): the name of the engine setting to be updated
             setting_data (Dict[str, str]): the content of the new setting
 
         Returns:
-            bool:  return True if the engine setting is successfully updated 
+            bool:  return True if the engine setting is successfully updated
         """
         return self.setting_manager.update_engine_setting(name, setting_data)
-    
+
     def is_engine_setting(self, name: str):
         """check if the given engine name is engine setting
 
         Args:
             name (str): the name of the engine setting
         """
         return self.setting_manager.is_engine_setting(name)
-     
-    def get_engine_setting_data(self, name:str) -> Union[bool, Dict[str, str]]:
-        """ get the enigine setting data 
+
+    def get_engine_setting_data(self, name: str) -> Union[bool, Dict[str, str]]:
+        """get the enigine setting data
 
         Args:
             name (str): the name of the engine setting
 
         Returns:
-            Union[bool, Dict[str, str]]: if the engine setting name is available 
+            Union[bool, Dict[str, str]]: if the engine setting name is available
             return the engine setting data as stored in a dictionary, else return False
         """
         return self.setting_manager.get_engine_setting_data(name)
-    
-    def is_engine_setting_in_use(self, name:str) -> bool:
-        """ check if the engine setting identified by name is in use
+
+    def is_engine_setting_in_use(self, name: str) -> bool:
+        """check if the engine setting identified by name is in use
 
         Args:
             name (str): the name of the engine setting
 
         Returns:
             bool: return true if the engine setting is in use, false other wise
         """
         return self.setting_manager.is_engine_setting_in_use(name)
-     
+
     def remove_all_settings(self) -> bool:
-        """ remove all settings except for the default setting
+        """remove all settings except for the default setting
 
         Returns:
-            bool: return true if the removal is successful 
+            bool: return true if the removal is successful
         """
         try:
             for setting in self.setting_manager.get_setting_names():
                 if setting != DEFAULT_SETTING_NAME:
                     assert self.remove_setting(setting)
 
             for source in self.source_manager.get_configured_sources():
                 assert source.setting_name() == DEFAULT_SETTING_NAME
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
+
     def get_setting_names(self) -> List[str]:
-        """ return a list of available setting names 
+        """return a list of available setting names
 
         Returns:
             List[str]: a list of available setting names
         """
         return self.setting_manager.get_setting_names()
-    
+
     def get_all_settings_data(self) -> Dict[str, SettingDict]:
-        """ 
+        """
         return a dictionary that stores all setting data
         """
         return self.setting_manager.get_all_settings_data()
 
     def get_all_profile_names(self) -> List[str]:
-        """ 
+        """
         return a list of string that stores all setting name
         """
         return self.setting_manager.get_setting_names()
-    
+
     def get_default_engine_setting_name(self) -> str:
-        """ get the default setting name
+        """get the default setting name
 
         Returns:
             str: a string that represent the default setting
         """
         return self.setting_manager.get_default_engine_setting_name()
-   
-   
+
     def get_default_profile_setting_name(self) -> str:
-        """ get the default setting name
+        """get the default setting name
 
         Returns:
             str: a string that represent the default setting
         """
         return self.setting_manager.get_default_profile_setting_name()
-    
-    
-    def set_default_setting(self, setting_name:str) -> bool:
-        """ set the default setting to setting_name
+
+    def set_default_setting(self, setting_name: str) -> bool:
+        """set the default setting to setting_name
 
         Args:
             setting_name (str)
-            
+
         Returns:
             bool:return true if the setting can be set, false otherwise
         """
         return self.setting_manager.set_to_default_setting(setting_name)
-    
-    def set_default_engine(self, engine_name:str) -> bool:
-        """ set the default setting to engine_name
+
+    def set_default_engine(self, engine_name: str) -> bool:
+        """set the default setting to engine_name
 
         Args:
             engine_name (str)
-            
+
         Returns:
             bool:return true if the setting can be set, false otherwise
         """
         return self.setting_manager.set_to_default_engine_setting(engine_name)
-    
-    def is_suite_in_use(self, suite_name:str) -> bool:
-        """given a suite_name, check if this suite is used 
+
+    def is_suite_in_use(self, suite_name: str) -> bool:
+        """given a suite_name, check if this suite is used
            in any of the setting
 
         Args:
             suite_name (str): the name of the plugin suite
 
         Returns:
-            bool: return true if the suite is used in any of the setting, 
+            bool: return true if the suite is used in any of the setting,
                   false otherwise
         """
         return self.setting_manager.is_suite_in_use(suite_name)
-    
-    
+
     def get_profile_src_path(self, name: str):
         """get the  path to the profile setting source
 
         Args:
-            name (str): the name of the profile 
+            name (str): the name of the profile
         """
         return self.setting_manager.get_profile_src_path(name)
 
-
     def get_engine_src_path(self, name: str):
         """get the  path to the engine setting source
 
         Args:
-            name (str): the name of the engine 
+            name (str): the name of the engine
         """
-        return self.setting_manager.get_engine_src_path(name)
+        return self.setting_manager.get_engine_src_path(name)
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/googleInterface.py` & `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/googleInterface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,73 +1,97 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:38:50
 import os
 from pydantic import BaseModel, ValidationError
 from typing import Dict, Union
 from .engineSettingInterface import EngineSettingInterface
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.engines.google import Google
-from gailbot.core.utils.general import copy, is_file, is_directory, make_dir, get_name, get_extension
-from gailbot.configs import  workspace_config_loader
+from gailbot.core.utils.general import (
+    copy,
+    is_file,
+    is_directory,
+    make_dir,
+    get_name,
+    get_extension,
+)
+from gailbot.configs import workspace_config_loader
 
 
 API_KEY_DIR = workspace_config_loader().engine_ws.google_api
 
 logger = makelogger("google_interface")
+
+
 class ValidateGoogle(BaseModel):
-    engine: str 
+    engine: str
     google_api_key: str
+
+
 class Transcribe(BaseModel):
-    """ 
+    """
     NOTE: google does not support additional kwargs in transcription
     """
-    pass 
+
+    pass
+
+
 class Init(BaseModel):
     # the path to a file that stores the google api key
-    google_api_key: str 
+    google_api_key: str
+
 
 class GoogleInterface(EngineSettingInterface):
     """
     Interface for the Google speech to text engine
     """
-    engine: str 
-    init: Init = None 
-    transcribe: Transcribe = None 
-    
+
+    engine: str
+    init: Init = None
+    transcribe: Transcribe = None
+
+
 def load_google_setting(setting: Dict[str, str]) -> Union[bool, EngineSettingInterface]:
-    """ given a dictionary, load the dictionary as a google setting 
+    """given a dictionary, load the dictionary as a google setting
 
     Args:
-        setting (Dict[str, str]): the dictionary that contains the setting data 
+        setting (Dict[str, str]): the dictionary that contains the setting data
 
     Returns:
-        Union[bool , SettingInterface]: if the setting dictionary is validated 
+        Union[bool , SettingInterface]: if the setting dictionary is validated
                                         by the google setting interface,
-                                        return the google setting interface 
-                                        as an instance of SettingInterface, 
+                                        return the google setting interface
+                                        as an instance of SettingInterface,
                                         else return false
     """
     logger.info(setting)
-    if  not "engine" in setting.keys() or setting["engine"] != "google": 
+    if not "engine" in setting.keys() or setting["engine"] != "google":
         return False
     try:
         setting = setting.copy()
         validate = ValidateGoogle(**setting)
         if not is_directory(API_KEY_DIR):
             make_dir(API_KEY_DIR)
-        
+
         # check that the api key is valid
         assert Google.is_valid_google_api(setting["google_api_key"])
-        
+
         # save a copied version of the api key file to the workspace
-        copied_api = os.path.join(API_KEY_DIR, get_name(setting["google_api_key"]) + ".json")
+        copied_api = os.path.join(
+            API_KEY_DIR, get_name(setting["google_api_key"]) + ".json"
+        )
         setting["google_api_key"] = copy(setting["google_api_key"], copied_api)
-    
-        google_set = dict ()
+
+        google_set = dict()
         google_set["engine"] = setting.pop("engine")
         google_set["init"] = dict()
         google_set["transcribe"] = dict()
         google_set["init"].update(setting)
         google_setting = GoogleInterface(**google_set)
-        
+
         return google_setting
     except ValidationError as e:
         logger.error(e, exc_info=e)
         return False
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/watsonInterface.py` & `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperInterface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,71 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:39:08
 from pydantic import BaseModel, ValidationError
-from typing import Dict, Union
+from typing import Dict, List, Union
 from .engineSettingInterface import EngineSettingInterface
 from gailbot.core.utils.logger import makelogger
-from gailbot.core.utils.download import is_internet_connected
-from gailbot.core.engines import Watson
-logger = makelogger("watson_interface")
 
-class ValidateWatson(BaseModel):
+logger = makelogger("whisperInterface")
+
+
+class ValidateWhisper(BaseModel):
     engine: str
-    apikey : str 
-    region: str 
-    base_model: str 
-    language_customization_id : str = None 
-    acoustic_customization_id : str = None 
-
-class InitSetting(BaseModel):
-    apikey : str 
-    region: str 
-    
+    language: str = None
+    detect_speakers: bool = False
+
+
+class Init(BaseModel):
+    pass
+
+
 class TranscribeSetting(BaseModel):
-    base_model: str 
-    language_customization_id : str = None 
-    acoustic_customization_id : str = None 
-    
-class WatsonInterface(EngineSettingInterface):
+    language: str = None
+    detect_speakers: bool = False
+
+
+class WhisperInterface(EngineSettingInterface):
     """
-    Interface for the Watson speech to text engine
+    Interface for the Whisper speech to text engine
     """
-    engine: str 
-    init : InitSetting
+
     transcribe: TranscribeSetting
-    
-    @property
-    def engine(self):
-        return "watson"
-
-    
-def load_watson_setting(setting: Dict[str, str]) -> Union[bool, EngineSettingInterface]:
-    """ given a dictionary, load the dictionary as a watson setting 
+    init: Init = None
+    engine: str
+
+
+def load_whisper_setting(
+    setting: Dict[str, str]
+) -> Union[bool, EngineSettingInterface]:
+    """given a dictionary, load the dictionary as a whisper setting
 
     Args:
-        setting (Dict[str, str]): the dictionary that contains the setting data 
+        setting (Dict[str, str]): the dictionary that contains the setting data
 
     Returns:
-        Union[bool , SettingInterface]: if the setting dictionary is validated 
-                                        by the watson setting interface,
-                                        return the google setting interface 
-                                        as an instance of SettingInterface, 
+        Union[bool , SettingInterface]: if the setting dictionary is validated
+                                        by the whisper setting interface,
+                                        return the google setting interface
+                                        as an instance of SettingInterface,
                                         else return false
-    """ 
-    if "engine" not in setting.keys() or setting["engine"] != "watson" or not is_internet_connected():
+    """
+    logger.info("initialize whisper engine")
+    if not "engine" in setting.keys() or setting["engine"] != "whisper":
         return False
     try:
         logger.info(setting)
         setting = setting.copy()
-        validate = ValidateWatson(**setting)
-        logger.info(validate)
-        watson_set = dict()
-        watson_set["engine"] = setting.pop("engine")
-        watson_set["init"] = dict()
-        watson_set["transcribe"] = dict()
-        watson_set["init"]["apikey"] = setting.pop("apikey")
-        watson_set["init"]["region"] = setting.pop("region")
-        watson_set["transcribe"].update(setting)
-        logger.info(watson_set)
-        watson_set = WatsonInterface(**watson_set)
-        assert Watson.valid_init_kwargs(watson_set.init.apikey, watson_set.init.region)
-        return watson_set
+        validate = ValidateWhisper(**setting)
+        whisper_set = dict()
+        whisper_set["engine"] = setting.pop("engine")
+        whisper_set["init"] = dict()
+        whisper_set["transcribe"] = dict()
+        whisper_set["transcribe"].update(setting)
+        whisper_set = WhisperInterface(**whisper_set)
+        return whisper_set
     except ValidationError as e:
         logger.error(e, exc_info=e)
-        return False
+        logger.error(f"error in validating whisper interface {e}")
+        return False
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/whisperInterface.py` & `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperXInterface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,68 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:39:08
 from pydantic import BaseModel, ValidationError
-from typing import Dict, List , Union
+from typing import Dict, List, Union
 from .engineSettingInterface import EngineSettingInterface
 from gailbot.core.utils.logger import makelogger
 
-logger = makelogger("whisperInterface")
-class ValidateWhisper(BaseModel): 
-    engine              :str
-    language            : str  = None
-    detect_speakers     : bool = False
-class Init(BaseModel): 
+logger = makelogger("whisperXInterface")
+
+
+class ValidateWhisperX(BaseModel):
+    engine: str
+    language: str = None
+
+
+class Init(BaseModel):
     pass
+
+
 class TranscribeSetting(BaseModel):
-    language            : str  = None
-    detect_speakers     : bool = False
-    
-class WhisperInterface(EngineSettingInterface):
+    language: str = None
+
+
+class WhisperXInterfacde(EngineSettingInterface):
     """
     Interface for the Whisper speech to text engine
     """
-    transcribe : TranscribeSetting
-    init: Init = None 
-    engine: str 
+    transcribe: TranscribeSetting
+    init: Init = None
+    engine: str
 
-def load_whisper_setting(setting: Dict[str, str]) -> Union[bool, EngineSettingInterface]:
-    """ given a dictionary, load the dictionary as a whisper setting 
+
+def load_whisperX_setting(
+        setting: Dict[str, str]
+) -> Union[bool, EngineSettingInterface]:
+    """given a dictionary, load the dictionary as a whisper setting
 
     Args:
-        setting (Dict[str, str]): the dictionary that contains the setting data 
+        setting (Dict[str, str]): the dictionary that contains the setting data
 
     Returns:
-        Union[bool , SettingInterface]: if the setting dictionary is validated 
+        Union[bool , SettingInterface]: if the setting dictionary is validated
                                         by the whisper setting interface,
-                                        return the google setting interface 
-                                        as an instance of SettingInterface, 
+                                        return the google setting interface
+                                        as an instance of SettingInterface,
                                         else return false
     """
     logger.info("initialize whisper engine")
-    if  not "engine" in setting.keys() or setting["engine"] != "whisper": 
+    if "engine" not in setting.keys() or setting["engine"] != "whisperX":
         return False
     try:
         logger.info(setting)
         setting = setting.copy()
-        validate = ValidateWhisper(**setting)
+        ValidateWhisperX(**setting)
         whisper_set = dict()
         whisper_set["engine"] = setting.pop("engine")
         whisper_set["init"] = dict()
         whisper_set["transcribe"] = dict()
         whisper_set["transcribe"].update(setting)
-        whisper_set = WhisperInterface(**whisper_set)
+        whisper_set = WhisperXInterfacde(**whisper_set)
         return whisper_set
     except ValidationError as e:
         logger.error(e, exc_info=e)
         logger.error(f"error in validating whisper interface {e}")
-        return False
+        return False
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/engineObject.py` & `GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/engineObject.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,102 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:39:21
 from typing import Dict, List, Union, TypedDict
 
 from ..interface import (
-    load_watson_setting, 
-    load_whisper_setting, 
-    load_google_setting, 
+    load_watson_setting,
+    load_whisper_setting,
+    load_google_setting,
     EngineSettingInterface,
-    PluginSettingsInterface
-    )
+    PluginSettingsInterface,
+)
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.utils.general import write_toml
 from gailbot.configs import default_setting_loader
+from ..interface.whisperXInterface import load_whisperX_setting
+
 logger = makelogger("engineObject")
 
-class EngineSetObj():
+
+class EngineSetObj:
     """
     store a single Engine setting
-     
+
     """
-    engine_setting: EngineSettingInterface   = None
-    name: str     = None                   
-    valid_interfaces = [load_whisper_setting, load_google_setting, load_watson_setting] 
-     
+
+    engine_setting: EngineSettingInterface = None
+    name: str = None
+    valid_interfaces = [load_whisper_setting, load_google_setting, load_watson_setting, load_whisperX_setting]
+
     def __init__(self, setting: Dict[str, str], name: str) -> None:
-        """ initializing an engine 
+        """initializing an engine
 
         Args:
             setting (Dict[str, str]): engine setting data stored in a dictionary
-            name (str): the name of the engine setting 
-        """ 
-        self.applied_in_profiles = set() # a set of profiles that applied this engine setting
+            name (str): the name of the engine setting
+        """
+        self.applied_in_profiles = (
+            set()
+        )  # a set of profiles that applied this engine setting
         self.name = name
         logger.info("initialize the setting object")
         assert self._load_engine_setting(setting)
         self.data = setting
-        self.engine = self.engine_setting.engine 
-    
+        self.engine = self.engine_setting.engine
+
     def get_init_kwargs(self):
         return self.engine_setting.get_init_kwargs()
-    
+
     def get_transcribe_kwargs(self):
         return self.engine_setting.get_transcribe_kwargs()
-    
+
     def get_name(self):
         """
         Accesses and returns the object's name
         """
         return self.name
-    
+
     def change_name(self, name):
         """
         Changes the profile name to a given new name
 
         Args:
             name: name to change to
         """
-        self.name = name 
-        
+        self.name = name
+
     def get_setting_dict(self) -> Dict[str, str]:
         """
         Accesses and returns the object's setting dict
         """
         return self.data
-    
+
     def update_setting(self, setting: Dict[str, str]) -> bool:
         """
         Updates the settings to a given dictionary
 
-        Args: 
+        Args:
             setting: Dict[str, str]: new setting
 
         Returns:
             bool: True if successfully updated, false if not
         """
         logger.info(setting)
         self._load_engine_setting(setting)
-       
+
         if self.engine_setting:
             self.data = setting
             return True
         else:
             return False
-    
-    def save_setting(self, output: str) -> bool: 
+
+    def save_setting(self, output: str) -> bool:
         """
         Saves the settings to the output directory
 
         Args:
             output:str: output directory path
 
         Returns:
@@ -95,26 +106,26 @@
         try:
             write_toml(output, self.data)
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
         else:
             return True
-        
+
     def is_in_use(self):
-        return len(self.applied_in_profiles) != 0 
-    
+        return len(self.applied_in_profiles) != 0
+
     def remove_applied_profile(self, profile_name):
         if profile_name in self.applied_in_profiles:
             self.applied_in_profiles.remove(profile_name)
-    
+
     def add_applied_profile(self, profile_name):
         self.applied_in_profiles.add(profile_name)
-     
-    def _load_engine_setting(self, setting : Dict[str, str]) -> bool:
+
+    def _load_engine_setting(self, setting: Dict[str, str]) -> bool:
         """
         Loads the engine settings
 
         Args:
             setting : List[str]: settings to load
 
         Returns:
@@ -125,9 +136,7 @@
             logger.info(option)
             set_obj = option(setting)
             if isinstance(set_obj, EngineSettingInterface):
                 self.engine_setting = set_obj
                 return True
         logger.info(f"setting {setting} cannot be loaded")
         return False
-    
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/settingObject.py` & `GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/settingObject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,90 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:39:32
 from typing import Dict, List, Union, TypedDict, Optional
 from .engineObject import EngineSetObj
 from .pluginObject import PluginSuiteSetObj
 from ..interface import (
-    load_watson_setting, 
-    load_whisper_setting, 
-    load_google_setting, 
+    load_watson_setting,
+    load_whisper_setting,
+    load_google_setting,
     EngineSettingInterface,
-    PluginSettingsInterface
-    )
+    PluginSettingsInterface,
+)
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.utils.general import write_toml
 from gailbot.configs import default_setting_loader
+
 logger = makelogger("setting_object")
 
+
 class SettingDict(TypedDict):
     engine_setting_name: str
     plugin_setting: List[str]
     engine_setting: Optional[Dict[str, str]]
 
-class SettingObject():
+
+class SettingObject:
     """
-    Store a single setting item 
+    Store a single setting item
     """
-    engine_setting: EngineSetObj   = None
-    plugin_setting: PluginSuiteSetObj  = None 
-    name: str     = None                   
-    valid_interfaces = [load_whisper_setting, load_google_setting, load_watson_setting] 
-     
-    def __init__(self, 
-                 engine_setting_name:str, 
-                 engine_setting: EngineSetObj ,
-                 plugin_setting: PluginSuiteSetObj, name: str) -> None:
+
+    engine_setting: EngineSetObj = None
+    plugin_setting: PluginSuiteSetObj = None
+    name: str = None
+    valid_interfaces = [load_whisper_setting, load_google_setting, load_watson_setting]
+
+    def __init__(
+        self,
+        engine_setting_name: str,
+        engine_setting: EngineSetObj,
+        plugin_setting: PluginSuiteSetObj,
+        name: str,
+    ) -> None:
         self.name = name
         self.engine_setting_name = engine_setting_name
         self.engine_setting = engine_setting
         self.plugin_setting = plugin_setting
-    
+
     def get_name(self):
         """
         Accesses and returns the object's name
         """
         return self.name
-    
+
     def change_profile_name(self, name):
         """
         Changes the profile name to a given new name
 
         Args:
             name: name to change to
         """
-        self.name = name 
-        
+        self.name = name
+
     def get_plugin_setting(self) -> List[str]:
         """
         Accesses and returns the object's plugin settings
         """
         return self.plugin_setting.get_data()
-    
+
     def get_data(self) -> SettingDict:
         """
         Accesses and returns the object's setting dict
         """
-        self.data = {"engine_setting": self.engine_setting.data, 
-                     "engine_setting_name": self.engine_setting.name, 
-                     "plugin_setting": self.plugin_setting.data}
+        self.data = {
+            "engine_setting": self.engine_setting.data,
+            "engine_setting_name": self.engine_setting.name,
+            "plugin_setting": self.plugin_setting.data,
+        }
         return self.data
-    
-    def save_setting(self, output: str) -> bool: 
+
+    def save_setting(self, output: str) -> bool:
         """
         Saves the settings to the output directory
 
         Args:
             output:str: output directory path
 
         Returns:
@@ -80,20 +94,22 @@
         try:
             write_toml(output, self.get_data())
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
         else:
             return True
-    
-    def update_setting(self, engine_setting: EngineSetObj, plugin_setting: PluginSuiteSetObj) -> bool:
+
+    def update_setting(
+        self, engine_setting: EngineSetObj, plugin_setting: PluginSuiteSetObj
+    ) -> bool:
         """
         Updates the settings to a given dictionary
 
-        Args: 
+        Args:
             setting: Dict[str, str]: new setting
 
         Returns:
             bool: True if successfully updated, false if not
         """
         try:
             logger.info(engine_setting)
@@ -102,8 +118,8 @@
             self.engine_setting = engine_setting
             self.engine_setting.add_applied_profile(self.name)
             self.plugin_setting = plugin_setting
             assert self.get_data()
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
-            return False 
+            return False
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/settings/settingManager.py` & `GailBot-0.2a0/src/gailbot/services/organizer/settings/settingManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,572 +1,581 @@
-'''
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:39:41
+"""
 # -*- coding: utf-8 -*-
 @Author  :   Vivian Li , Siara Small 
 @Date    :   2023/05/17
 @Last Modified By :   Vivian, Siara Small
 @Last Modified Time :   2023/05/17 19:50:58
-'''
-
+"""
 
 from typing import Dict, Union, List
 import os
 
 from .objects import SettingDict, SettingObject, PluginSuiteSetObj, EngineSetObj
 from gailbot.core.utils.general import (
-    is_file, 
-    is_directory, 
-    read_toml, 
-    get_name, 
-    make_dir, 
+    is_file,
+    is_directory,
+    read_toml,
+    get_name,
+    make_dir,
     delete,
-    filepaths_in_dir)
+    filepaths_in_dir,
+)
 from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("setting_manager")
 
+
 class ExistingSettingName(Exception):
     def __init__(self, name: str, *args: object) -> None:
         super().__init__(*args)
         self.name = name
+
     def __str__(self) -> str:
         return f"the setting name {self.name} already exist"
 
-class SettingManager():
+
+class SettingManager:
     """
-    Manages all available settings 
+    Manages all available settings
     """
-    profiles : Dict[str, SettingObject] = dict()
-    engine_settings  : Dict[str, EngineSetObj]   = dict()
-    
-    def __init__(self, workspace:str, load_exist: bool = True) -> None:
-        """ constructing the setting manager
+
+    profiles: Dict[str, SettingObject] = dict()
+    engine_settings: Dict[str, EngineSetObj] = dict()
+
+    def __init__(self, workspace: str, load_exist: bool = True) -> None:
+        """constructing the setting manager
 
         Args:
-            workspace (str): the path to the directory stores all the 
+            workspace (str): the path to the directory stores all the
                              setting files
-            load_exist (bool, optional): if true , load existing setting in 
+            load_exist (bool, optional): if true , load existing setting in
                              workspace. Defaults to True.
         """
         self.workspace = workspace
         self.engine_set_space = os.path.join(workspace, "engine_setting")
         self.default_setting = None
-        self.default_engine_setting = None 
-        
+        self.default_engine_setting = None
+
         if not is_directory(self.workspace):
             make_dir(self.workspace)
-        
+
         if not is_directory(self.engine_set_space):
             make_dir(self.engine_set_space)
-            
-        if load_exist: 
+
+        if load_exist:
             engine_files = filepaths_in_dir(self.engine_set_space, ["toml"])
             for file in engine_files:
                 self.load_set_from_file(file, self.add_new_engine, overwrite=True)
-                
+
             setting_files = filepaths_in_dir(self.workspace, ["toml"])
             for file in setting_files:
                 self.load_set_from_file(file, self.add_new_setting, overwrite=True)
-    
-    def load_set_from_file(self, file_path, addfun, overwrite: bool = False) ->bool:
-        """ load the setting from local file
+
+    def load_set_from_file(self, file_path, addfun, overwrite: bool = False) -> bool:
+        """load the setting from local file
 
         Args:
             file_path (str): the file path
             overwrite (bool, optional): if true, the loaded
             file will overwrite existing setting with same name. Defaults to False.
 
         Returns:
             bool: return true if the loading is successful, false if the file
-            cannot be loaded 
+            cannot be loaded
         """
         if is_file(file_path):
             data = read_toml(file_path)
             try:
                 name = get_name(file_path)
                 data = read_toml(file_path)
                 return addfun(name, data, overwrite)
             except Exception as e:
                 logger.error(e, exc_info=e)
                 return False
-    
+
     #####################################################################
     #               Functions for managing engine setting               #
     #####################################################################
     def get_engine_setting_names(self) -> List[str]:
         """return a list of available engine setting name
 
         Returns:
             List[str]: a list of engine setting names
         """
         return list(self.engine_settings.keys())
 
-    def add_new_engine(self, name, engine:Dict[str, str], overwrite: bool = False):
+    def add_new_engine(self, name, engine: Dict[str, str], overwrite: bool = False):
         """add a new engine setting
 
         Args:
             name (str): the name of the engine setting
-            engine (Dict[str, str]): the data of the engine setting, 
-                                     one required field is the type of the 
-                                     engine 
-            
+            engine (Dict[str, str]): the data of the engine setting,
+                                     one required field is the type of the
+                                     engine
+
             overwrite (bool, optional): if True, overwrite the existing engine s
                                         etting with the same name. Defaults to False.
 
         Raises:
             ExistingSettingName: if the engine setting name has been taken, and overwrite is set to False
 
         Returns:
-            bool: return true if the setting is successfully added, false otherwise 
-        """ 
-        if self.is_engine_setting(name) and (not overwrite): 
+            bool: return true if the setting is successfully added, false otherwise
+        """
+        if self.is_engine_setting(name) and (not overwrite):
             raise ExistingSettingName(name)
         try:
             setting: EngineSetObj = EngineSetObj(engine, name)
             assert setting.engine_setting
             self.engine_settings[name] = setting
             self.save_engine_setting(name)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
+
     def remove_engine_setting(self, name):
-        """remove the engine setting from the disk 
+        """remove the engine setting from the disk
 
         Args:
             name (str): the name of the engine setting
 
         Returns:
-            bool: return true if the engine setting is removed successfully 
+            bool: return true if the engine setting is removed successfully
         """
         try:
             assert self.is_engine_setting(name)
             assert not self.engine_settings[name].is_in_use()
             del self.engine_settings[name]
             if is_file(self.get_engine_src_path(name)):
                 delete(self.get_engine_src_path(name))
-            return True 
+            return True
         except Exception as e:
-            logger.error(e, exc_info=e) 
+            logger.error(e, exc_info=e)
             return False
-        
-    def is_engine_setting_in_use(self, name)->bool:
-        """check if the engine setting is in use 
+
+    def is_engine_setting_in_use(self, name) -> bool:
+        """check if the engine setting is in use
 
         Args:
             name (str): the name of the engine setting
         """
         return self.engine_settings[name].is_in_use()
-    
+
     def is_engine_setting(self, name):
         """check if the given setting is engine setting
 
         Args:
             name (str): the name that identify the engine setting
 
         Returns:
-            bool: true if the setting is engine setting false otherwise 
+            bool: true if the setting is engine setting false otherwise
         """
         return name in self.engine_settings
-    
-    def save_engine_setting(self, name:str) -> Union[bool, str]:
-        """save the setting as a local file 
+
+    def save_engine_setting(self, name: str) -> Union[bool, str]:
+        """save the setting as a local file
 
         Args:
             name (str): the setting name
 
         Returns:
-            Union[bool, str]: return the saved file path if the setting is 
+            Union[bool, str]: return the saved file path if the setting is
                               saved successfully, return false otherwise
         """
         try:
             out_path = self.get_engine_src_path(name)
             if is_file(out_path):
                 delete(out_path)
             self.engine_settings[name].save_setting(out_path)
             return out_path
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-    
-    def update_engine_setting(self, name:str, setting_data: Dict[str, str]) -> bool:
+
+    def update_engine_setting(self, name: str, setting_data: Dict[str, str]) -> bool:
         """
         update the engine setting
-        
+
         Args:
             name(str)
             setting_data(Dict[str, str])
-            
+
         Returns:
             bool
-        """ 
+        """
         if self.is_engine_setting(name):
             try:
                 engine_setting = self.engine_settings[name]
                 assert engine_setting.update_setting(setting_data)
                 assert self.save_engine_setting(name)
                 for profile in engine_setting.applied_in_profiles:
-                    ## update the engine setting on the disk 
+                    ## update the engine setting on the disk
                     self.save_setting(profile)
                 return True
             except Exception as e:
                 logger.error(e, exc_info=e)
                 return False
-                
-    def get_engine_src_path(self, name:str) -> str:
+
+    def get_engine_src_path(self, name: str) -> str:
         """given a engine setting name, return its path
 
         Args:
             name (str): the engine setting name
 
         Returns:
             str: a path to store the setting file
-            
+
         Note:
-            This is a function to form a path to the local setting file 
-            in a unified format, the path does not guaranteed to indicate 
+            This is a function to form a path to the local setting file
+            in a unified format, the path does not guaranteed to indicate
             an existing setting file
         """
-        return os.path.join(self.engine_set_space, name + ".toml")  
-    
-    def get_engine_setting_data(self, name:str) -> Union[bool, Dict[str, str]]:
-        """ get the setting data of the engine setting
+        return os.path.join(self.engine_set_space, name + ".toml")
+
+    def get_engine_setting_data(self, name: str) -> Union[bool, Dict[str, str]]:
+        """get the setting data of the engine setting
 
         Args:
             name (str): the name of the engine
 
         Returns:
-            Union[bool, Dict[str, str]]: return the dictionary that stores the 
-                                         the engine data if the data engine 
-                                         name is a valid engine in the setting 
-                                         manager, else return false 
-        """ 
+            Union[bool, Dict[str, str]]: return the dictionary that stores the
+                                         the engine data if the data engine
+                                         name is a valid engine in the setting
+                                         manager, else return false
+        """
         if self.is_engine_setting(name):
             return self.engine_settings[name].get_setting_dict()
         else:
             return False
-    
+
     def _get_profile_engine(self, profile_name: str) -> EngineSetObj:
-        """return the engine used in the profile identifies by profile name 
+        """return the engine used in the profile identifies by profile name
 
         Args:
             profile_name (str): the name of the profile to be queried
 
         Returns:
-            EngineSetObj: the engine object 
+            EngineSetObj: the engine object
         """
         profile_obj = self.profiles[profile_name]
         engine_obj = self.engine_settings[profile_obj.engine_setting_name]
         return engine_obj
 
-        
     def set_to_default_engine_setting(self, setting_name: str) -> bool:
         """set one setting to be the default setting
 
         Args:
             name (str): the name of the setting
 
         Returns:
-            bool: return true if the default setting can be set, 
+            bool: return true if the default setting can be set,
                   false otherwise
         """
         if setting_name in self.profiles:
-             self.default_engine_setting = setting_name
-             return True
+            self.default_engine_setting = setting_name
+            return True
         else:
-             return False 
+            return False
 
     def get_default_engine_setting_name(self) -> str:
-        """ return the name of the default engine 
+        """return the name of the default engine
 
         Returns:
             str: _description_
         """
         return self.default_engine_setting
-    
+
     #####################################################################
     #               Functions for managing profile setting              #
     #####################################################################
     def get_setting_names(self) -> List[str]:
-        """ return a list of available setting names 
+        """return a list of available setting names
 
         Returns:
-            List[str]: a list of setting names 
+            List[str]: a list of setting names
         """
         return list(self.profiles.keys())
-    
+
     def remove_setting(self, name: str) -> bool:
-        """ given the setting name, remove the setting and the local 
+        """given the setting name, remove the setting and the local
             setting file
         Args:
             name (str): the name that identify the setting
 
         Returns:
             bool: return true if the removal is successful, false if
-                  the setting does not exist 
+                  the setting does not exist
         """
         if self.is_setting(name):
             settingObj = self.profiles.pop(name)
-            self.engine_settings[settingObj.engine_setting_name].remove_applied_profile(name)
+            self.engine_settings[settingObj.engine_setting_name].remove_applied_profile(
+                name
+            )
             if is_file(self.get_profile_src_path(name)):
                 delete(self.get_profile_src_path(name))
             return True
         else:
             return False
-    
-    def get_setting(self, name:str) -> Union [SettingObject, bool]:
-        """ given the setting name, return the corresponding setting 
+
+    def get_setting(self, name: str) -> Union[SettingObject, bool]:
+        """given the setting name, return the corresponding setting
 
         Args:
             name (str): a name that identifies the setting
 
         Returns:
-            Union [SettingObject, bool]: return the setting object if the 
-            setting is found, return false if the setting does not exist 
+            Union [SettingObject, bool]: return the setting object if the
+            setting is found, return false if the setting does not exist
         """
         if self.is_setting(name):
             return self.profiles[name]
         else:
             return False
-        
-    def add_new_setting(self, 
-                        name: str, 
-                        data: SettingDict,
-                        overwrite: bool = False) -> Union[bool, str]:
-        """ add a new setting 
+
+    def add_new_setting(
+            self, name: str, data: SettingDict, overwrite: bool = True
+    ) -> Union[bool, str]:
+        """add a new setting
 
         Args:
             name (str): the setting name that identifies the setting
-            setting (Dict[str, str]): a dictionary that stores the setting
+            data (Dict[str, str]): a dictionary that stores the setting
             overwrite (bool, optional): if true, the given setting will overwrite
             an existing setting if a setting with the same name exist.
             Defaults to False.
 
         Returns:
-            Union[bool, str]: True if the setting creates successfully, 
-                              False otherwise 
-        
+            Union[bool, str]: True if the setting creates successfully,
+                              False otherwise
+
         Raises:
             ExistingSettingName: raised when the setting name already exist
-                                 and the overwrite option is set to false 
+                                 and the overwrite option is set to false
         """
         logger.info(f"get engine {data}")
-        if self.is_setting(name): 
+        if self.is_setting(name):
             if overwrite:
                 self.remove_setting(name)
             else:
                 raise ExistingSettingName(name)
         try:
             engine_set_name = data["engine_setting_name"]
             engine_obj = self.engine_settings[engine_set_name]
             plugin_obj = PluginSuiteSetObj(data["plugin_setting"])
             setting: SettingObject = SettingObject(
-                engine_setting=engine_obj, 
+                engine_setting=engine_obj,
                 engine_setting_name=engine_set_name,
                 plugin_setting=plugin_obj,
-                name=name)
+                name=name,
+            )
             self.engine_settings[engine_set_name].add_applied_profile(name)
             assert setting and setting.engine_setting
             self.profiles[name] = setting
             self.save_setting(name)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
 
     def is_setting(self, name: str) -> bool:
-        """ tell if a setting exists in the setting manager
+        """tell if a setting exists in the setting manager
 
         Args:
             name (str): the setting name
 
         Returns:
             bool: return true if the given name is an existing setting, false
-                  otherwise 
+                  otherwise
         """
         return name in self.profiles
 
     def update_setting(self, name: str, setting_data: SettingDict) -> bool:
-        """ update the setting
+        """update the setting
 
         Args:
             name (str): setting name
             setting_data (Dict[str, str]): the updated setting content
 
         Returns:
-            bool:   return true if the setting is updated, false if the 
-                    setting does not exist or the new setting dictionary 
-                    cannot be validated 
+            bool:   return true if the setting is updated, false if the
+                    setting does not exist or the new setting dictionary
+                    cannot be validated
         """
         if self.is_setting(name):
             try:
                 profile_setting = self.profiles[name]
                 orig_engine = profile_setting.engine_setting.name
                 engine_set_name = setting_data["engine_setting_name"]
                 engine_obj = self.engine_settings[engine_set_name]
                 plugin_obj = PluginSuiteSetObj(setting_data["plugin_setting"])
-                assert profile_setting.update_setting(engine_setting=engine_obj, plugin_setting=plugin_obj)
+                assert profile_setting.update_setting(
+                    engine_setting=engine_obj, plugin_setting=plugin_obj
+                )
                 assert self.save_setting(name)
                 return True
             except Exception as e:
                 logger.error(e, exc_info=e)
         else:
             return False
 
-    def rename_setting(self, name: str, new_name:str) ->bool:
-        """ rename a setting 
+    def rename_setting(self, name: str, new_name: str) -> bool:
+        """rename a setting
 
         Args:
-            name (str): the original name of the setting 
-            new_name (str): the new name of the setting 
+            name (str): the original name of the setting
+            new_name (str): the new name of the setting
 
         Returns:
-            bool: return true if the setting can be renamed, false 
+            bool: return true if the setting can be renamed, false
                   if the setting does not exist or if the new_name
                   has been taken by other existing setting
-        """        
+        """
         if self.is_setting(name):
             if self.is_setting(new_name):
-                logger.error(f"new name{ new_name} has been taken")
+                logger.error(f"new name{new_name} has been taken")
                 return False
-            
+
             temp = self.profiles.pop(name)
             engine_applied = self._get_profile_engine(name)
             engine_applied.remove_applied_profile(name)
-            
+
             temp.name = new_name
             engine_applied.add_applied_profile(new_name)
             self.profiles[new_name] = temp
             self.save_setting(new_name)
-            
-            if is_file(self.get_profile_src_path(name)): 
+
+            if is_file(self.get_profile_src_path(name)):
                 delete(self.get_profile_src_path(name))
             logger.info("update_setting")
             return self.profiles[new_name] != None
         else:
             logger.error("the setting is not found")
             return False
-    
-    def save_setting(self, name:str) -> Union[bool, str]:
-        """ save the setting as a local file
+
+    def save_setting(self, name: str) -> Union[bool, str]:
+        """save the setting as a local file
 
         Args:
             name (str): the setting name
 
         Returns:
             Union[bool, str]: return the saved file path if the setting
-                              is saved successfully, return false otherwise 
-            
-        """ 
-        try: 
+                              is saved successfully, return false otherwise
+
+        """
+        try:
             out_path = self.get_profile_src_path(name)
             if is_file(out_path):
                 delete(out_path)
-            self.profiles[name].save_setting(out_path) 
+            self.profiles[name].save_setting(out_path)
             return out_path
         except Exception as e:
             logger.error(e, exc_info=e)
-            return False   
-    
-    def get_setting_dict(self, setting_name:str) -> Union[bool, SettingDict]:
-        """ return the setting data as a dictionary 
+            return False
+
+    def get_setting_dict(self, setting_name: str) -> Union[bool, SettingDict]:
+        """return the setting data as a dictionary
 
         Args:
             setting_name (str): the name that identifies the setting
 
         Returns:
-            Union[bool, SettingDict]: if the setting exists, return the setting 
+            Union[bool, SettingDict]: if the setting exists, return the setting
                                       data, else return false
-        """ 
+        """
         if setting_name in self.profiles:
             return self.profiles[setting_name].get_data()
         else:
             return False
-    
-    def get_profile_src_path(self, name:str) -> str:
+
+    def get_profile_src_path(self, name: str) -> str:
         """given a setting name, return its path
 
         Args:
             name (str): the setting name
 
         Returns:
             str: a path to store the setting file
-            
+
         Note:
-            This is a function to form a path to the local setting file 
-            in a unified format, the path does not guaranteed to indicate 
+            This is a function to form a path to the local setting file
+            in a unified format, the path does not guaranteed to indicate
             an existing setting file
         """
         return os.path.join(self.workspace, name + ".toml")
-    
+
     def delete_all_settings(self) -> bool:
-        """ delete all settings 
+        """delete all settings
 
         Returns:
-            bool: True if the deletion is successful, false if not 
+            bool: True if the deletion is successful, false if not
         """
         try:
             for setting in self.get_setting_names():
                 if setting != "default":
                     self.remove_setting(setting)
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-        
+
     def get_all_settings_data(self) -> Dict[str, SettingDict]:
-        """ 
-        return a dictionary that stores all available setting data 
+        """
+        return a dictionary that stores all available setting data
         """
         setting_dict = dict()
         for key, setting_object in self.profiles.items():
             setting_dict[key] = setting_object.data
-            
+
         logger.info(f"setting data {setting_dict}")
-        return setting_dict 
+        return setting_dict
 
     def set_to_default_setting(self, setting_name: str) -> bool:
         """set one setting to be the default setting
 
         Args:
             name (str): the name of the setting
 
         Returns:
-            bool: return true if the default setting can be set, 
+            bool: return true if the default setting can be set,
                   false otherwise
         """
         if setting_name in self.profiles:
-             self.default_setting = setting_name
-             return True
+            self.default_setting = setting_name
+            return True
         else:
-             return False 
-    
-
+            return False
 
     def get_default_profile_setting_name(self) -> str:
         """get the default setting name
 
         Returns:
-            str: the default setting 
+            str: the default setting
         """
         return self.default_setting
-    
+
     #####################################################################
     #       function for managing plugin setting                        #
     #####################################################################
 
-    def is_suite_in_use(self, suite_name:str) -> bool:
-        """given a suite_name, check if this suite is used 
+    def is_suite_in_use(self, suite_name: str) -> bool:
+        """given a suite_name, check if this suite is used
            in any of the setting
 
         Args:
             suite_name (str): the name of the plugin suite
 
         Returns:
-            bool: return true if the suite is used in any of the setting, 
+            bool: return true if the suite is used in any of the setting,
                   false otherwise
         """
         for setting_obj in self.profiles.values():
             if suite_name in setting_obj.get_plugin_setting():
                 return True
         return False
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/source/source_manager.py` & `GailBot-0.2a0/src/gailbot/services/organizer/source/source_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,84 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 14:30:48
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-04 15:16:00
 from typing import List, Dict, Union
 import os
 from .source_object import SourceObject
 from ..settings import SettingObject
 from gailbot.core.utils.general import get_name, is_file, is_directory, is_path
 from gailbot.core.utils.logger import makelogger
 from gailbot.configs import workspace_config_loader
 
 OUTPUT_EXTENSION = workspace_config_loader().file_extension.output
 logger = makelogger("source_manager")
-class SourceManager():
+
+
+class SourceManager:
     """
     Holds and handles all functionality for managing all sources
     """
+
     def __init__(self) -> None:
-        self.sources : Dict[str, SourceObject] = dict()
-        
-        
-    def add_source(self, source_path: str, output: str) -> Union [str, bool]:
+        self.sources: Dict[str, SourceObject] = dict()
+
+    def add_source(self, source_path: str, output: str) -> Union[str, bool]:
         """
         Adds a source to the source manager object
 
         Args:
             source_path: str: path to the source object to add
             output: str: path to the output directory
-        
+
         Returns:
             Name of the source if it is successfully added, false if it is not
                 successfully added
         """
         try:
+            logger.info("in try")
             name = get_name(source_path)
             i = 0
             while name in self.sources.keys():
                 print(name)
                 if i:
                     i += 1
-                    name = name.replace("---" + str(i-1), "---"+str(i))
+                    name = name.replace("---" + str(i - 1), "---" + str(i))
                 else:
                     i += 1
                     name = f"{name}---{i}"
-            source  = SourceObject(source_path, name, output)
-            self.sources[name] = source  
+            source = SourceObject(source_path, name, output)
+            self.sources[name] = source
         except Exception as e:
+            logger.info("in exception")
             logger.error(e, exc_info=e)
             return False
         else:
+            logger.info("in else")
             return name
-        
+
     def remove_source(self, source_name: str) -> bool:
         """
         Removes a given source from the source manager's sources
 
         Args:
             source_name: str: name to remove
 
         Returns:
-            True if given source was successfully removed, false if given 
+            True if given source was successfully removed, false if given
             source was not found
         """
         logger.info(f"source {source_name} is removed")
         if not self.is_source(source_name):
             return False
         self.sources.pop(source_name)
         return True
-    
-        
-    def is_source(self, source:str) -> bool:
+
+    def is_source(self, source: str) -> bool:
         """
         Determines if a given source is currently in the source manager's sources
 
         Args:
             source: str: key of the source to search for
 
         Returns:
@@ -77,178 +86,172 @@
         """
         source_name = get_name(source) if is_path(source) else source
         if source_name in self.sources:
             return True
         else:
             return False
 
-    
     def source_names(self) -> List[str]:
         """
         Obtains all source names as a list
-        
+
         Returns:
             List of strings containing all source names
         """
         return list(self.sources.keys())
 
-    def get_source(self, source:str) -> Union[bool, SourceObject]:
+    def get_source(self, source: str) -> Union[bool, SourceObject]:
         """
         Gets the source associated with a given source name
 
         Args:
             source_name: str: string of name to search for
-        
+
         Returns:
             Source object associated with the given name
             Returns false if object with given name is not found
         """
         source_name = get_name(source) if is_path(source) else source
         if self.is_source(source_name):
             return self.sources[source_name]
         else:
             return False
-        
-    def get_source_outdir(self, source:str) -> Union[bool, str]:
+
+    def get_source_outdir(self, source: str) -> Union[bool, str]:
         """
         Gets the source output directory associated with a given source name
 
         Args:
             source_name: str: string of name to search for
-        
+
         Returns:
             Source object associated with the given name
             Returns false if object with given name is not found
         """
         source_name = get_name(source) if is_path(source) else source
         if self.is_source(source_name):
             logger.info("is source")
             return self.sources[source_name].output
         else:
             logger.error(source_name)
             return False
 
-    def get_source_setting(self, source:str) -> SettingObject:
+    def get_source_setting(self, source: str) -> SettingObject:
         """
         Gets the object;s source settings
 
         Args:
             source: str: source object to look for
-        
+
         Returns:
             SettingObject of the current source's settings
         """
         source_name = get_name(source) if is_path(source) else source
         if self.is_source(source_name):
             return self.sources[source_name].source_setting()
         else:
             return False
 
     def apply_setting_profile_to_source(
-        self, 
-        source:str, 
-        setting: SettingObject, 
-        overwrite: bool
+        self, source: str, setting: SettingObject, overwrite: bool
     ):
         """
         Applies the given settings to the given source
 
         Args:
             source: str: given source to update
             setting: SettingObject: setting object to apply
             overwrite: bool: whether or not to overwrite
-        
-        Returns:    
+
+        Returns:
             bool: True if successfully applied, false if not
         """
         source_name = get_name(source) if is_path(source) else source
         logger.info(f"apply setting {setting} to {source_name}")
         if self.is_source(source_name):
             self.sources[source_name].apply_setting(setting, overwrite)
             return self.sources[source_name].configured
         logger.error(f"not a valid source")
         return False
-   
+
     def add_progress_display(self, source: str, displayer: callable) -> bool:
-        """ 
-        Add function to display file progress 
+        """
+        Add function to display file progress
 
         Args:
             source (str): a string that identify the source
             displayer (callable): the function that check for file progress
 
         Returns:
             bool: True if the displayer is applied, false otherwise
         """
         source_name = get_name(source) if is_path(source) else source
         if self.is_source(source_name):
-            return self.sources[source_name].add_progress_display(displayer)    
+            return self.sources[source_name].add_progress_display(displayer)
         return False
-        
-    def get_sources_with_setting(self, setting_name:str) -> List[str]: 
+
+    def get_sources_with_setting(self, setting_name: str) -> List[str]:
         """
         Accesses all sources with a given settings profile
 
         Args:
             self
             setting_name: string of the settings profile to look for
 
         Returns:
             list of strings of all source names with the settings profile
         """
-        return [k for k,v in self.sources.items() if v.setting.get_name() == setting_name]
-    
-    
+        return [
+            k for k, v in self.sources.items() if v.setting.get_name() == setting_name
+        ]
+
     def get_configured_sources(self, sources: List[str] = None) -> List[SourceObject]:
-        """ given the  a list of source name, return a list of the sourceObject
+        """given the  a list of source name, return a list of the sourceObject
             that stores the source configured with setting
         Args:
-            sources (List[str], optional): a list of source name, if not 
+            sources (List[str], optional): a list of source name, if not
             given, return a list of configured source. Defaults to None.
 
         Returns:
-            List[SourceObject]: a list of source object that stores the source data 
+            List[SourceObject]: a list of source object that stores the source data
         """
         configured = []
         if not sources:
             for source in self.sources.values():
                 if source.setting != None:
                     configured.append(source)
             return configured
         else:
             for source in sources:
                 src = self.get_source(source)
                 if src.setting != None:
                     configured.append(source)
 
-    def is_source_configured(self, source:str) -> bool:
+    def is_source_configured(self, source: str) -> bool:
         """
         Determines if given source has been configured with settings
 
         Args:
             self
             source_name: string of the source name
 
         Returns:
             True if configured, false if not
         """
         source_name = get_name(source) if is_path(source) else source
         return self.sources[source_name].configured
-    
-    
+
     def __repr__(self) -> str:
-        return (f"Source manager with sources {self.source_names}")
-    
+        return f"Source manager with sources {self.source_names}"
+
     @staticmethod
-    def _is_path(source:str):
+    def _is_path(source: str):
         """
         Determines if a string is a path
 
         Args:
-            source: str: string to determine if is a path 
+            source: str: string to determine if is a path
 
         Returns:
             bool: true if given string is a path, false if not
         """
         return is_file(source) or is_directory(source)
-    
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/organizer/source/source_object.py` & `GailBot-0.2a0/src/gailbot/services/organizer/source/source_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,54 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:40:00
 from typing import Dict, Union, Callable
 from datetime import datetime
 from ..settings import SettingObject
 from gailbot.core.utils.logger import makelogger
 from gailbot.configs import workspace_config_loader
 import os
+
 OUT_PUT_EXTENSION = workspace_config_loader().file_extension.output
 
 logger = makelogger("source_object")
-class SourceObject():
+
+
+class SourceObject:
     name: str
     path: str
     output: str
     setting: SettingObject
     """
     Holds and handles all functionality for a single source object
     """
-    def __init__(self, path:str, name: str, output: str) -> None:
+
+    def __init__(self, path: str, name: str, output: str) -> None:
         self.name: str = name
         self.path: str = path
         timestamp = datetime.now().strftime("_%m_%d_%y-%H-%M-%S")
-        self.output:str = os.path.join(output, name + OUT_PUT_EXTENSION + timestamp)
-        self.setting: SettingObject = None  
-        self.progress_display: Callable = None 
-        
+        self.output: str = os.path.join(output, name + OUT_PUT_EXTENSION + timestamp)
+        self.setting: SettingObject = None
+        self.progress_display: Callable = None
 
     def source_details(self) -> Dict[str, Union[str, SettingObject]]:
         """
         Accesses and returns the details about the given source.
-        
+
         Returns:
             Dictionary containing the source name, source path, and settings profile
         """
-        return {"source_name": self.name, 
-                "source_path": self.path,
-                "settings": self.setting }
-    
+        return {
+            "source_name": self.name,
+            "source_path": self.path,
+            "settings": self.setting,
+        }
+
     def source_path(self):
         """
         Accesses the path of a source
 
         Returns:
             string containing the source path
         """
@@ -66,15 +76,15 @@
         """
         Determines if a given source was configured or not.
 
         Returns:
             Boolean representing whether or not the given source was configured
         """
         return self.setting != None
-    
+
     def apply_setting(self, setting: SettingObject, overwrite: bool = True):
         """
         Apply setting object
 
         Args:
             setting: SettingObject
             overwrite: bool
@@ -82,31 +92,31 @@
         Returns:
             None
         """
         logger.info(f"the setting object that is about to be applied is {setting}")
         if overwrite or not self.setting:
             self.setting = setting
             self.configured = True
-    
+
     def add_progress_display(self, displayer: Callable):
-        """ 
-        Add a function to the source object that will take 
+        """
+        Add a function to the source object that will take
         in one string as argument
-        
+
 
         Args:
-            displayer (Callable): a function that will take in the string 
-                                as a progress message 
+            displayer (Callable): a function that will take in the string
+                                as a progress message
 
 
         """
         if callable(displayer):
             self.progress_display = displayer
-            return True 
+            return True
         else:
             return False
 
     def __repr__(self) -> str:
         """
         Gets a message containing source details
         """
-        return (f"Source object with name {self.name} and path {self.path}")
+        return f"Source object with name {self.name} and path {self.path}"
```

### Comparing `GailBot-0.1a9/src/gailbot/services/pipeline/components/analysisComponent.py` & `GailBot-0.2a0/src/gailbot/services/pipeline/components/analysisComponent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,157 +1,161 @@
+# -*- coding: utf-8 -*-
+# @Author: Jason Y. Wu
+# @Date:   2023-07-17 19:21:51
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:53:17
 import time
 import os
 from typing import Any, List, Dict
 from gailbot.core.utils.general import copy, get_name
 from gailbot.core.utils.logger import makelogger
 from gailbot.core.pipeline import Component, ComponentState, ComponentResult
 from gailbot.core.utils.threads import ThreadPool
 
 from gailbot.plugins import PluginManager, PluginSuite
-from gailbot.services.converter.result import  ProcessingStats
+from gailbot.services.converter.result import ProcessingStats
 from gailbot.services.converter.payload import PayLoadObject
 from ...converter.plugin.pluginMethod import GBPluginMethods
 from ..components.progress import ProgressMessage
 from gailbot.configs import service_config_loader
 
 
 NUM_THREAD = service_config_loader().thread.analysis_num_threads
 logger = makelogger("analysisComponent")
 
+
 class PluginError(Exception):
     def __init__(self, msg) -> None:
-        self.msg = msg 
-        
+        self.msg = msg
+
     def __repr__(self) -> str:
         return f"Plugin Error: {self.msg}"
-    
+
     def __str__(self) -> str:
         return f"Plugin Error: {self.msg}"
+
+
 class AnalysisComponent(Component):
-    """ Responsible for running plugin after gailbot has obtained the
-        transcription result 
+    """Responsible for running plugin after gailbot has obtained the
+    transcription result
     """
+
     def __init__(self, plugin_manager: PluginManager):
         self.plugin_manager = plugin_manager
-        
+
     def __repr__(self):
         return "Analysis Component"
-        
-    def __call__(
-        self,
-        dependency_outputs : Dict[str, Any]
-    ) -> ComponentResult:
-        """ 
+
+    def __call__(self, dependency_outputs: Dict[str, Any]) -> ComponentResult:
+        """
         Extracts the payloads from the dependency_output and runs the analysis
-        
+
         Args:
-            dependency_outputs (Dict[str, Any]): dependency outputs that store 
-            the result from the transcription process, which include the 
-            payloads data and result state 
+            dependency_outputs (Dict[str, Any]): dependency outputs that store
+            the result from the transcription process, which include the
+            payloads data and result state
 
         Returns:
             ComponentResult: the result of the analysis process
         """
         threads = ThreadPool(NUM_THREAD)
         process_start_time = time.time()
         logger.info(dependency_outputs)
-        try: 
+        try:
             dependency_res: ComponentResult = dependency_outputs["transcription"]
             logger.info(f"result from transcription {dependency_res}")
             assert dependency_res.state == ComponentState.SUCCESS
-            
-            payloads: List [PayLoadObject] = dependency_res.result
+
+            payloads: List[PayLoadObject] = dependency_res.result
             logger.info(f"get payloads {payloads}")
             for payload in payloads:
                 if not payload.failed:
                     threads.add_task(self.analyze_payload, [payload])
             threads.wait_for_all_completion()
             threads.shutdown()
-            
+
             return ComponentResult(
-                state  = ComponentState.SUCCESS,
-                result = payloads,
-                runtime = time.time() - process_start_time)
+                state=ComponentState.SUCCESS,
+                result=payloads,
+                runtime=time.time() - process_start_time,
+            )
         except Exception as e:
             logger.error(e, exc_info=e)
             return ComponentResult(
-                state = ComponentState.FAILED,
-                result = payloads,
-                runtime = time.time() - process_start_time
+                state=ComponentState.FAILED,
+                result=payloads,
+                runtime=time.time() - process_start_time,
             )
 
     def analyze_payload(self, payload: PayLoadObject):
         logger.info("start analyzing payload")
         self.emit_progress(payload, ProgressMessage.Analyzing)
         start_time = time.time()
         suites = payload.setting.get_plugin_setting()
         logger.info(f"the following suites are applied: {suites}")
-      
-        # the dictionary that stores the result of all analysis 
+
+        # the dictionary that stores the result of all analysis
         analysis_result = dict()
-      
+
         if not suites:
             return True
-        
+
         # try applying plugin
         try:
             for suite_name in suites:
                 suite_result = dict()
                 suite_result["plugin_suite"] = suite_name
                 suite_result["success"] = list()
                 suite_result["failure"] = list()
-                
+
                 plugin_suite: PluginSuite = self.plugin_manager.get_suite(suite_name)
                 # check plugin suit is valid
                 if not plugin_suite:
                     self.emit_progress(payload, f"{suite_name} is not a valid plugin")
                     raise PluginError(f"{suite_name} is not a valid plugin")
                 logger.info(f"retrieved plugin suite {plugin_suite}")
-                
+
                 # create a method that get passed to plugin suite, and apply plugin suite
                 method = GBPluginMethods(payload, suite_name)
-                # calls the plugin suite 
-                res : Dict[str, ComponentState] = plugin_suite(base_input = None, methods = method)
-                
+                # calls the plugin suite
+                res: Dict[str, ComponentState] = plugin_suite(
+                    base_input=None, methods=method
+                )
+
                 # collect plugin suite result
                 logger.info(f"get the plugin result {res}")
                 for name, state in res.items():
                     if state == ComponentState.SUCCESS:
                         suite_result["success"].append(name)
                     else:
                         suite_result["failure"].append(name)
                 analysis_result[suite_name] = suite_result
             end_time = time.time()
             stats = ProcessingStats(
                 start_time=start_time,
                 end_time=end_time,
-                elapsed_time_sec=end_time - start_time
-            ) 
-            payload.set_analysis_process_stats(stats)   
+                elapsed_time_sec=end_time - start_time,
+            )
+            payload.set_analysis_process_stats(stats)
             payload.set_analysis_result(analysis_result)
-            
-            # only set the return result to be True if none of the plugin 
+
+            # only set the return result to be True if none of the plugin
             # in plugin suite fails
             for suite_result in analysis_result.values():
                 assert len(suite_result["failure"]) == 0
             self.emit_progress(payload, ProgressMessage.Analyzed)
-        
+
         except Exception as e:
-            logger.error(f"fail to apply the plugin suite {suite_name}, error {e}", exc_info=e)
+            logger.error(
+                f"fail to apply the plugin suite {suite_name}, error {e}", exc_info=e
+            )
             self.emit_progress(payload, ProgressMessage.Error)
             payload.set_failure()
-            return False 
+            return True
         else:
             payload.set_analyzed()
             return True
-        
+
     def emit_progress(self, payload: PayLoadObject, msg: str):
         if payload.progress_display:
             payload.progress_display(msg)
         time.sleep(0.1)
-
-                        
-
-
-
-
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/pipeline/components/transcribeComponent.py` & `GailBot-0.2a0/src/gailbot/services/pipeline/components/transcribeComponent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-03-15 10:31:49
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-03-15 12:22:53
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:53:46
 import copy
 import time
 import threading
 from gailbot.core.engines.engineManager import EngineManager
 from typing import Any, List, Dict
 from gailbot.core.pipeline import Component, ComponentState, ComponentResult
 from gailbot.core.utils.general import get_name
 from gailbot.core.utils.threads import ThreadPool
 from gailbot.core.utils.logger import makelogger
 
-from ...converter.result import  ProcessingStats
+from ...converter.result import ProcessingStats
 from ...converter.payload import PayLoadObject
 from ..components.progress import ProgressMessage
 from gailbot.configs import service_config_loader
+
 logger = makelogger("transcribeComponent")
 
 DEFULT_NUM_THREAD = service_config_loader().thread.transcriber_num_threads
 
+
 class InvalidEngineError(Exception):
     def __init__(self, engine: str, *args) -> None:
         super().__init__(*args)
         self.engine = engine
+
     def __repr__(self) -> str:
         return self.engine + "is not a valid engine"
 
+
 class TranscribeComponent(Component):
     """
     Responsible for running the transcription process
     """
-    def __init__(self, num_thread : int = DEFULT_NUM_THREAD):
-        self.engine_manager = EngineManager() # a wrapper class for managing
-                                              # and transcribing payload using engine
+
+    def __init__(self, num_thread: int = DEFULT_NUM_THREAD):
+        self.engine_manager = EngineManager()  # a wrapper class for managing
+        # and transcribing payload using engine
         self.num_thread = num_thread
         self.is_transcribing = False
 
     def __call__(self, dependency_output: Dict[str, ComponentResult]) -> Any:
         """
             Extracts the payload objects from the dependency_output and
             transcribes the datafiles in the payload object
@@ -55,30 +60,33 @@
             self.is_transcribing = True
             timer = threading.Timer(5, self._log_progress)
             timer.start()
             threadpool = ThreadPool(self.num_thread)
             logger.info(dependency_output)
             dep: ComponentResult = dependency_output["base"]
             # get the list of payloads from dependency_output
-            payloads : List[PayLoadObject] = dep.result
+            payloads: List[PayLoadObject] = dep.result
             process_start_time = time.time()
-            logger.info(f"received payloads {payloads}") 
+            logger.info(f"received payloads {payloads}")
             for payload in payloads:
                 self._display_progress(payload, ProgressMessage.Waiting)
                 if not payload.transcribed:
                     # add the payload to the threadpool
                     key = threadpool.add_task(
-                        task = self._transcribe_one_payload,
-                        args = [payload],
-                        key  = payload.name)
+                        task=self._transcribe_one_payload,
+                        args=[payload],
+                        key=payload.name,
+                    )
                     assert key == payload.name
-                    logger.info(f"payload {payload.name} is added to the threadpool, the key is {key}")
+                    logger.info(
+                        f"payload {payload.name} is added to the threadpool, the key is {key}"
+                    )
                 else:
                     self._display_progress(payload, ProgressMessage.Finished)
-           
+
             # get the result from the thread pool
             for payload in payloads:
                 if not payload.transcribed:
                     if not threadpool.get_task_result(payload.name):
                         payload.set_failure()
                     else:
                         payload.set_transcribed()
@@ -87,29 +95,28 @@
             logger.error(f"Transcription failure {e}", exc_info=e)
             threadpool.shutdown(wait=True)
             self.is_transcribing = False
             timer.cancel()
             return ComponentResult(
                 state=ComponentState.FAILED,
                 result=payloads,
-                runtime=time.time() - process_start_time
+                runtime=time.time() - process_start_time,
             )
         else:
             threadpool.shutdown(cancel_futures=True)
             self.is_transcribing = False
             timer.cancel()
             return ComponentResult(
                 state=ComponentState.SUCCESS,
                 result=payloads,
-                runtime=time.time() - process_start_time
+                runtime=time.time() - process_start_time,
             )
-      
 
-    def _transcribe_one_payload(self, payload : PayLoadObject) -> bool:
-        """ private function that transcribe each individual payload
+    def _transcribe_one_payload(self, payload: PayLoadObject) -> bool:
+        """private function that transcribe each individual payload
 
         Args:
             payload (PayLoadObject): payload object that stores the datafiles
 
         Raises:
             InvalidEngineError:
             raised when the engine setting uses an invalid engine
@@ -117,93 +124,104 @@
         Returns:
             : return True if the payload is transcribed successfully , false
               otherwise
         """
         try:
             logger.info(f"Payload {payload} being transcribed")
             self._display_progress(payload, "Start transcribing")
-            
+
             # Parse the payload
             start_time = time.time()
             transcribe_ws = payload.workspace.transcribe_ws
             data_files = payload.data_files
             num_file = len(data_files)
-            
+
             # Parse the settings
             engine_name = payload.get_engine()
             init_kwargs = payload.get_engine_init_setting()
             transcribe_kwargs = payload.get_engine_transcribe_setting()
-            logger.info(f"get transcribed setting engine_name: {engine_name} \
+            logger.info(
+                f"get transcribed setting engine_name: {engine_name} \
                           engine initialization setting {init_kwargs} \
-                          engine transcription setting {transcribe_kwargs}")
+                          engine transcription setting {transcribe_kwargs}"
+            )
 
             # check for valid engine engine
             if not self.engine_manager.is_engine(engine_name):
                 raise InvalidEngineError(engine_name)
-            
+
             # start to use engine to transcribe files in the payload
             utt_map = dict()
             threadpool = ThreadPool(DEFULT_NUM_THREAD)
-            
+
             # adding the task to transcribe individual file to the thread
             self._display_progress(payload, "Adding Task")
             for idx, file in enumerate(data_files):
                 transcribe_kwargs = copy.deepcopy(transcribe_kwargs)
-                transcribe_kwargs.update({"audio_path": file, "payload_workspace": transcribe_ws})
+                transcribe_kwargs.update(
+                    {"audio_path": file, "payload_workspace": transcribe_ws}
+                )
                 filename = threadpool.add_task(
                     self._transcribe_single_file,
-                    kwargs= {"engine_name" : engine_name,
-                            "init_kwargs" : init_kwargs,
-                            "transcribe_kwargs": transcribe_kwargs},
-                    key = get_name(file))
+                    kwargs={
+                        "engine_name": engine_name,
+                        "init_kwargs": init_kwargs,
+                        "transcribe_kwargs": transcribe_kwargs,
+                    },
+                    key=get_name(file),
+                )
                 assert filename == get_name(file)
-                
+
                 # add callback function to update the progress bar whenever
                 # each task is finished
                 threadpool.add_callback(
-                    filename, lambda fun: self._get_progress_bar(payload, threadpool))
-            
+                    filename, lambda fun: self._get_progress_bar(payload, threadpool)
+                )
+
             # display the initial progress
             self._get_progress_bar(payload, threadpool)
 
             # get the task result
             for file in data_files:
                 utt_map[get_name(file)] = threadpool.get_task_result(get_name(file))
-           
-            
+
             # if the transcription result is returned successfully
             end_time = time.time()
             stats = ProcessingStats(
                 start_time=start_time,
-                end_time = end_time,
-                elapsed_time_sec= end_time - start_time
+                end_time=end_time,
+                elapsed_time_sec=end_time - start_time,
             )
-            
+
             assert payload.set_transcription_result(utt_map)
-            assert payload.set_transcription_process_stats(stats)      
+            assert payload.set_transcription_process_stats(stats)
             self._display_progress(payload, ProgressMessage.Transcribed)
-             
+
         except Exception as e:
             self._display_progress(payload, ProgressMessage.Error)
-            logger.error(f"Failed to transcribed {len(data_files)} file in parallel due to the error {e}", exc_info=e)
+            logger.error(
+                f"Failed to transcribed {len(data_files)} file in parallel due to the error {e}",
+                exc_info=e,
+            )
             threadpool.shutdown(cancel_futures=True)
             return False
-        else: 
+        else:
             threadpool.shutdown(cancel_futures=True)
             return True
 
     def _log_progress(self):
-        """display log messages
-        """
+        """display log messages"""
         if self.is_transcribing:
-           logger.info("transcribing") 
-           timer = threading.Timer(5, self._log_progress)
-           timer.start()
+            logger.info("transcribing")
+            timer = threading.Timer(5, self._log_progress)
+            timer.start()
 
-    def _transcribe_single_file(self, engine_name, init_kwargs, transcribe_kwargs)  -> List[Dict[str, str]]:
+    def _transcribe_single_file(
+        self, engine_name, init_kwargs, transcribe_kwargs
+    ) -> List[Dict[str, str]]:
         """
         Transcribes a file with the given engine
 
         Args:
             engine: engine to perform the transcription
             init_kwargs: arguments with which to initialize the engine
             transcribe_kwargs: arguments with which to initialize the transcription
@@ -225,21 +243,20 @@
     def _get_progress_string(self, finished: int, total: int) -> str:
         BAR_FILL = "█"  # Full block
         BAR_EMPTY = "  "  # Light shade
         # Determine the length of the progress bar (50 characters)
         bar_length = 20
         # Calculate the number of filled and empty blocks in the progress bar
         filled_blocks = int(finished / total * bar_length)
-        percent = "..." if finished == 0 else '{:.2f}%'.format(finished / total * 100)
-        
+        percent = "..." if finished == 0 else "{:.2f}%".format(finished / total * 100)
+
         # Construct the progress bar string using Unicode block characters
-        bar =  "Transcribing " + (BAR_FILL * filled_blocks)  
+        bar = "Transcribing " + (BAR_FILL * filled_blocks)
         # Print the progress bar string
         return f"{bar} {percent}"
-    
+
     def _get_progress_bar(self, payload: PayLoadObject, threadpool: ThreadPool):
         if payload.progress_display:
             progress_str = self._get_progress_string(
-                threadpool.count_completed_tasks(), 
-                threadpool.count_total_tasks())
+                threadpool.count_completed_tasks(), threadpool.count_total_tasks()
+            )
             self._display_progress(payload, progress_str)
-
```

### Comparing `GailBot-0.1a9/src/gailbot/services/pipeline/pipeline.py` & `GailBot-0.2a0/src/gailbot/services/pipeline/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,63 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-08 15:16:01
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-01-12 14:37:40
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:40:23
 
 from typing import List
 
 from gailbot.core.pipeline import Pipeline, ComponentState
 from gailbot.plugins import PluginManager
 from gailbot.core.utils.logger import makelogger
 from ..converter import PayLoadObject
 from .components import TranscribeComponent, AnalysisComponent, FormatComponent
 
 logger = makelogger("service pipeline")
+
+
 class PipelineService:
     """
     Handles the higher level functionality of the pipeline
     """
-    def __init__(
-        self,
-        plugin_manager : PluginManager,
-        num_threads: int
-    ):
 
+    def __init__(self, plugin_manager: PluginManager, num_threads: int):
         transcribeComponent = TranscribeComponent()
         analysisComponent = AnalysisComponent(plugin_manager)
         formatComponent = FormatComponent()
 
         self.pipeline = Pipeline(
             dependency_map={
                 "transcription": [],
-                "analysis"     : ["transcription"],
-                "format"       : ["analysis"]
+                "analysis": ["transcription"],
+                "format": ["analysis"],
             },
-            components ={
-                "transcription" : transcribeComponent,
-                "analysis"      : analysisComponent,
-                "format"        : formatComponent
+            components={
+                "transcription": transcribeComponent,
+                "analysis": analysisComponent,
+                "format": formatComponent,
             },
-            num_threads = num_threads  
+            num_threads=num_threads,
         )
 
-    def __call__(self, payloads : List[PayLoadObject]) -> List[str]:
+    def __call__(self, payloads: List[PayLoadObject]) -> List[str]:
         """
         Creates and validates a pipeline from a list of payload objects
 
         Args:
             payloads : List[PayLoadObject]: list of objects to use as input
-            
-        Return: 
+
+        Return:
             return a list of payload object that fails to be transcribed
         """
-        res = self.pipeline(
-            base_input= payloads
-        )
+        res = self.pipeline(base_input=payloads)
         fails = []
-        
+
         for name, result in res.items():
             if not result == ComponentState.SUCCESS:
                 return [p.name for p in payloads]
-      
+
         for payload in payloads:
             if payload.failed:
                 fails.append(payload.name)
-        
-        return fails
 
-        
+        return fails
```

### Comparing `GailBot-0.1a9/src/gailbot/workspace/manager.py` & `GailBot-0.2a0/src/gailbot/workspace/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-06-15 15:27:03
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2023-06-15 15:39:02
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-08-01 05:41:44
 from dataclasses import dataclass
 from typing import Union, List
 
-from gailbot.configs import (
-    workspace_config_loader,
-    TemporaryFolder,
-    OutputFolder)
-from gailbot.core.utils.general import (
-    is_directory,
-    make_dir,
-    delete,
-    paths_in_dir)
+from gailbot.configs import workspace_config_loader, TemporaryFolder, OutputFolder
+from gailbot.core.utils.general import is_directory, make_dir, delete, paths_in_dir
 from gailbot.core.utils.logger import makelogger
 
 logger = makelogger("workspace")
+
+
 @dataclass
 class WorkspaceManager:
-    """ store the path data of the workspace, provide utility function to
-        create temporary and output directories
+    """store the path data of the workspace, provide utility function to
+    create temporary and output directories
     """
+
     def __init__(self, user_root: str) -> None:
-        self.path_config         = workspace_config_loader()
-        self.user_root:      str = user_root
-        self.setting_src:    str = self.path_config.gailbot_data.setting_src
-        self.plugin_src:     str = self.path_config.gailbot_data.plugin_src
+        self.path_config = workspace_config_loader()
+        self.user_root: str = user_root
+        self.setting_src: str = self.path_config.gailbot_data.setting_src
+        self.plugin_src: str = self.path_config.gailbot_data.plugin_src
         self.tempspace_root: str = self.path_config.tempspace_root
-        self.file_extension      = self.path_config.file_extension
+        self.file_extension = self.path_config.file_extension
 
     def init_workspace(self):
         """
         initializing the workspace
         """
         for path in self.path_config.gailbot_data.__dict__.values():
             logger.info(f"path received in workspace {path}")
@@ -43,52 +39,51 @@
         for path in self.path_config.engine_ws.__dict__.values():
             logger.info(f"path received for engine workspace {path}")
             if not is_directory(path):
                 make_dir(path, True)
 
         if not is_directory(self.path_config.tempspace_root):
             make_dir(self.path_config.tempspace_root)
-    
+
     def reset_workspace(self):
         try:
             if is_directory(self.path_config._ws_root):
                 delete(self.path_config._ws_root)
             make_dir(self.path_config._ws_root)
             self.init_workspace()
             return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
 
     def get_file_temp_space(self, name: str) -> Union[TemporaryFolder, bool]:
-        """ given the file name, create a directory for the file
+        """given the file name, create a directory for the file
             to store temporary files created during the transcription process
 
         Args:
             name (str): name of the file
 
         Returns:
             Union[TemporaryFolder, bool]: if the temporary folder is created
             successfully, return a TemporaryFolder dataclass object that
             stores the path of each subfolder under the temporary folder,
             else return False
         """
-        folder = self.path_config.get_temp_space(
-            name + self.file_extension.temp)
+        folder = self.path_config.get_temp_space(name + self.file_extension.temp)
         try:
             for path in folder.__dict__.values():
                 if not is_directory(path):
                     make_dir(path, True)
             return folder
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
 
     def get_output_space(self, outdir: str) -> Union[OutputFolder, bool]:
-        """ given the file name, and the root path of the output, create a
+        """given the file name, and the root path of the output, create a
             directory for the file to store output files
 
         Args:
             outdir (str): output path of the file
             name (str): name of the file
 
         Returns:
@@ -103,15 +98,14 @@
                 if not is_directory(path) and path[-1] == "/":
                     make_dir(path, True)
             return folder
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
 
-
     def clear_temp_space(self, temp_space: Union[str, TemporaryFolder]):
         """clear the temporary space of a certain file
 
         Args:
             temp_space (Union[str, TemporaryFolder]): either a
             Temporary folder object that stores the path to the temporary
             directories, or the name of the original file that can be used
@@ -120,16 +114,19 @@
         Returns:
             _type_: _description_
         """
         try:
             if isinstance(temp_space, TemporaryFolder):
                 delete(temp_space.root)
             else:
-                delete(self.path_config.get_temp_space(
-                    temp_space + self.file_extension.temp).root)
+                delete(
+                    self.path_config.get_temp_space(
+                        temp_space + self.file_extension.temp
+                    ).root
+                )
                 return True
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
 
     def clear_gb_temp_dir(self):
         """
@@ -142,20 +139,17 @@
             if is_directory(self.path_config.tempspace_root):
                 delete(self.path_config.tempspace_root)
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
 
     def get_setting_file(self) -> List[str]:
-        """ get the list of paths to the saved setting files
+        """get the list of paths to the saved setting files
 
         Returns:
             List[str]: a list of paths to the saved setting files
         """
         try:
-            return paths_in_dir(
-                self.path_config.gailbot_data.setting_src, ["toml"])
+            return paths_in_dir(self.path_config.gailbot_data.setting_src, ["toml"])
         except Exception as e:
             logger.error(e, exc_info=e)
             return False
-
-
```

### Comparing `GailBot-0.1a9/tests/test_api.py` & `GailBot-0.2a0/tests/test_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
 # @Date:   2023-01-12 14:26:59
 # @Last Modified by:   Jason Y. Wu
-# @Last Modified time: 2023-07-03 23:20:33
+# @Last Modified time: 2023-07-07 14:10:50
 from gailbot import GailBot
 from tests.test_data import PATH
 from tests.test_data import SETTING_DATA
 import logging
+import os
 
 
 def transcribe(
     files,
     setting_name="test",
     setting_data=SETTING_DATA.WHISPER_PROFILE,
     output=PATH.OUTPUT_ROOT,
@@ -547,7 +548,42 @@
     """
     Purpose: Test the Google transcription with a specific audio file in a demo scenario
     Expected Output: No failures or invalid transcriptions
     """
     fails, invalid = transcribe(
         [PATH.DEMO3], "google", SETTING_DATA.GOOGLE_PROFILE, output=PATH.GOOGLE_OUT_PATH
     )
+
+
+### demo for testing plugin ##
+def test_test_suite():
+    use_test_suite = {
+        "engine_setting_name": "whisper",
+        "plugin_setting": ["test_suite"],
+    }
+    gb = GailBot(PATH.USER_ROOT)
+    test_suite_path = PATH.TEST_SUITE_DIR
+    print(test_suite_path)
+    gb.register_plugin_suite(test_suite_path)
+    gb.create_new_setting("test_plugin_suite", use_test_suite)
+    gb.add_source(PATH.HELLO_1, PATH.OUTPUT_ROOT)
+    gb.apply_setting_to_source(PATH.HELLO_1, "test_plugin_suite")
+    gb.transcribe()
+    gb.remove_setting("test_plugin_suite")
+    gb.delete_plugin_suite("test_suite")
+
+
+def test_sample_suite():
+    use_sample_suite = {
+        "engine_setting_name": "whisper",
+        "plugin_setting": ["sample_suite"],
+    }
+    gb = GailBot(PATH.USER_ROOT)
+    sample_suite_path = PATH.SAMPLE_SUITE_DIR
+    print(sample_suite_path)
+    gb.register_plugin_suite(sample_suite_path)
+    gb.create_new_setting("sample_suite_test", use_sample_suite)
+    gb.add_source(PATH.HELLO_1, PATH.OUTPUT_ROOT)
+    gb.apply_setting_to_source(PATH.HELLO_1, "sample_suite_test")
+    gb.transcribe()
+    gb.remove_setting("sample_suite_test")
+    gb.delete_plugin_suite("sample_test")
```

### Comparing `GailBot-0.1a9/tests/test_small.py` & `GailBot-0.2a0/tests/test_small.py`

 * *Files identical despite different names*

