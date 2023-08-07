# Comparing `tmp/hvcc-0.7.0.tar.gz` & `tmp/hvcc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvcc-0.7.0.tar", last modified: Wed Apr 12 14:10:04 2023, max compression
+gzip compressed data, was "hvcc-0.8.0.tar", last modified: Mon Aug  7 18:18:01 2023, max compression
```

## Comparing `hvcc-0.7.0.tar` & `hvcc-0.8.0.tar`

### file list

```diff
@@ -1,556 +1,538 @@
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.475034 hvcc-0.7.0/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    32005 2023-03-23 00:02:12.000000 hvcc-0.7.0/LICENSE
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      291 2023-03-23 00:02:12.000000 hvcc-0.7.0/MANIFEST.in
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-04-12 14:10:04.475034 hvcc-0.7.0/PKG-INFO
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6431 2023-04-12 13:45:43.000000 hvcc-0.7.0/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.355033 hvcc-0.7.0/hvcc/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14778 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.355033 hvcc-0.7.0/hvcc/core/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/core/hv2ir/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4237 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/BufferPool.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/Connection.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1688 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrConvolution.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1998 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrInlet.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1207 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrLorenz.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1486 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrOutlet.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1367 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrPack.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1695 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrReceive.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2345 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrSend.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1499 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrSwitchcase.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1705 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrTabhead.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1738 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrTabread.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1720 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrTabwrite.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2221 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangAdc.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10864 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangBinop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2055 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangBiquad.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2128 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangDac.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1523 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangDelay.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2010 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangIf.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1735 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangLine.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1481 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangMessage.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1704 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangNoise.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1592 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangPhasor.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1473 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangPrint.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1563 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangRandom.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2186 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangReceive.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2497 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSend.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3325 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSequence.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1473 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSlice.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1477 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSystem.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2161 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangTable.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4041 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangUnop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2927 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangVar.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2604 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangVario.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1039 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyException.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    43580 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10293 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyIrObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16786 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyLangObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11713 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyParser.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3954 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/LocalVars.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/hv2ir/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5472 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/hv2ir.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/core/json/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49936 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/json/heavy.ir.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    42899 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/json/heavy.lang.json
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/generators/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/generators/buildjson/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/buildjson/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3191 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/buildjson/buildjson.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2daisy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5107 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2daisy/c2daisy.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9377 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2daisy/parameters.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2daisy/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7851 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/static/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2daisy/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5101 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      418 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/templates/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2dpf/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2dpf/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7591 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/c2dpf.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2dpf/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1071 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/static/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2dpf/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2442 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6924 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4070 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4468 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3430 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2243 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3543 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1218 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_plugin
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      882 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_project
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5625 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2fabric/c2fabric.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1036 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/Android.mk
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      104 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/Application.mk
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      843 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5095 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3293 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1879 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12034 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11773 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2js/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/README.md
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10301 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2js/c2js.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2js/template/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6364 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/hv_worklet.js
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      323 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/hv_worklet_start.js
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8674 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/hv_wrapper.js
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5094 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/index.html
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2owl/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6825 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2owl/c2owl.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2owl/deps/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7309 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/deps/HvMessage.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10738 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/deps/HvUtils.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2owl/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7536 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/templates/HeavyOwl.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      511 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/templates/HeavyOwlConstants.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2pdext/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4826 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2pdext/c2pdext.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2pdext/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    28387 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/static/m_pd.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2pdext/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5138 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/templates/pd_external.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9581 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/templates/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5509 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2unity/c2unity.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/static/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/static/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11516 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5538 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1399 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/static/xcode/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1269 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/xcode/Info.plist
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1745 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/Android.mk
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      132 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/Application.mk
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1451 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15663 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4128 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       64 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/PluginList.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10393 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10411 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2079 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    26264 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2wwise/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9537 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2wwise/c2wwise.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2wwise/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1584 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/resources/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4603 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.387033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9669 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      182 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.def
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2866 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6266 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      481 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1261 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.387033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2162 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2470 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9180 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2231 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.391033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      530 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      345 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_Wwise{{type}}PluginFactory.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.391033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2939 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8432 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1994 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5019 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1816 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3015 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7157 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4129 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2234 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/stdafx.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4601 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7351 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2691 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8485 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14466 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/runtime/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      475 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/runtime/Hv_{{name}}_WwisePluginRegister.cpp
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    27569 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18316 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4208 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    24299 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      889 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Info.plist
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    25293 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       82 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/wwise.xcconfig
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.399033 hvcc-0.7.0/hvcc/generators/copyright/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/copyright/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/copyright/copyright_manager.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1570 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/copyright/default_template.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2285 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/filters.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.407033 hvcc-0.7.0/hvcc/generators/ir2c/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4509 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlBinop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1507 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlCast.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2507 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlDelay.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1798 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlIf.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3341 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlMessage.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1748 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlPack.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1863 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlPrint.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1757 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlRandom.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1060 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlReceive.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2209 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSend.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1740 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSlice.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2787 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSwitchcase.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1299 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSystem.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1648 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlTabhead.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1794 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlTabread.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1805 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlTabwrite.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2608 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlUnop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2141 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlVar.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6610 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/HeavyObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2479 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/HeavyTable.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1721 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/PrettyfyC.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3271 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalBiquad.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2301 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalCPole.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalConvolution.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1867 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalDel1.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1708 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalEnvelope.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1918 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalLine.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalLorenz.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3650 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalMath.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2819 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalPhasor.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2078 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalRPole.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1952 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalSamphold.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2038 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalSample.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1926 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalTabhead.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3188 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalTabread.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2389 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalTabwrite.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4561 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalVar.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12893 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ir2c.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3740 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ir2c_perf.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.423033 hvcc-0.7.0/hvcc/generators/ir2c/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9339 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4262 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11622 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContextInterface.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4072 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2033 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2040 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1256 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3597 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1494 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1405 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1250 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2505 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1035 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1094 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1697 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1300 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2151 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1167 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1577 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1675 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1750 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1354 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2367 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1538 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2525 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1401 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9062 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15439 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavyInternal.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4803 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3274 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    21847 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMath.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7317 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4680 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2623 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6071 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3270 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9283 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7085 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11740 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4821 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1429 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1386 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1769 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5852 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1392 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4974 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2891 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1189 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4976 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4917 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5679 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1724 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3743 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1537 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9492 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1753 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1379 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2427 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6188 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1783 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5551 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2890 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4251 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2625 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1653 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9710 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4553 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2319 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/ir2c/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11759 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2517 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2720 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.hpp
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/vs2015/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1263 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.sln
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13015 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9467 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2527 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/main.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/stdafx.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      305 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/stdafx.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      306 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/targetver.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/xcode/Heavy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2492 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy/main.c
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/xcode/Heavy.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    81361 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      934 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1141 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1626 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9797 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49663 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      170 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Prefix.pch
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      903 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1662 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2902 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.m
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16216 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18184 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      436 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/Credits.rtf
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       45 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/InfoPlist.strings
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      809 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/main.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4493 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1956 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.439033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      842 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2761 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.439033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3702 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1575 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      921 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13635 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.439033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1077 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1576 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Info.plist
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5995 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7428 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      777 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1049 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.m
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      901 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/main.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.443034 hvcc-0.7.0/hvcc/interpreters/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.447034 hvcc-0.7.0/hvcc/interpreters/pd2hv/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/Connection.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2977 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8422 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1664 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/HvSwitchcase.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2327 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/NotificationEnum.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1929 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdAudioIoObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5676 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdBinopObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9128 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1838 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLetObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3461 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLibSignalGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3078 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdMessageObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6952 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1900 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdPackObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    29733 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdParser.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2856 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRaw.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5686 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdReceiveObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRouteObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5537 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSelectObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3805 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSendObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2179 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTableObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2230 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTriggerObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3510 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdUnpackObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.447034 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      798 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      761 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.447034 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy_converted/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6569 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.475034 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/abs.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/abs~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/atan.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/atan2.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/b.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bang.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      872 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bendin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      413 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bendout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2107 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bng.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bp~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      627 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/change.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      372 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/clip.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      376 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/clip~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      117 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cnv.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cos.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      817 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cos~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      573 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2291 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      523 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      981 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      979 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      694 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      692 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       61 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/declare.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/del.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      657 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delay.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1339 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      343 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/div.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/env~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      268 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/exp.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      228 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/exp~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/f.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/float.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/floatatom.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1082 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ftom.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      369 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ftom~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1239 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hip~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hradio.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hsl.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      212 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/i.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      867 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/int.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2724 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/line.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      299 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/line~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      147 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/loadbang.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/log.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1088 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/lop~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1043 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/makenote.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1185 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/metro.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      250 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/midiin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      378 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/midiout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      258 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/midirealtimein.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      502 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/moses.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      492 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/mtof.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      366 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/mtof~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/nbx.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1234 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/noise~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      918 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/notein.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      422 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/noteout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1156 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/osc~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      914 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      451 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pgmout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      351 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/phasor~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pipe.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12790 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/poly.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      919 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      430 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/polytouchout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/powtodb~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      215 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/print.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/q8_rsqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      226 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/q8_sqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      835 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/random.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      337 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rpole~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      907 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      367 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rzero_rev~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      417 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rzero~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      615 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      269 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/samplerate~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      267 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sig~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      411 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/snapshot~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      359 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/spigot.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sqrt.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      909 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/stripnote.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      585 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/swap.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      332 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/symbol.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      179 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/symbolatom.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2361 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      292 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabplay~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      796 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2494 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1497 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      440 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tan.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      188 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tgl.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      869 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/timer.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      875 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/touchin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      373 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/touchout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      946 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/until.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2709 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vd~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vradio.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vsl.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      497 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/wrap.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      288 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/wrap~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5213 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/pd2hv.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1889 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/utils.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.355033 hvcc-0.7.0/hvcc.egg-info/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/PKG-INFO
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    20780 2023-04-12 14:10:04.000000 hvcc-0.7.0/hvcc.egg-info/SOURCES.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        1 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/dependency_links.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       60 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/entry_points.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       56 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/requires.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       11 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/top_level.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1047 2023-04-12 14:10:04.475034 hvcc-0.7.0/setup.cfg
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       38 2023-03-23 00:02:12.000000 hvcc-0.7.0/setup.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.614456 hvcc-0.8.0/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    32005 2021-04-14 08:50:26.000000 hvcc-0.8.0/LICENSE
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      291 2022-08-20 00:37:38.000000 hvcc-0.8.0/MANIFEST.in
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-08-07 18:18:01.614456 hvcc-0.8.0/PKG-INFO
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6508 2023-08-07 18:08:50.000000 hvcc-0.8.0/README.md
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.574456 hvcc-0.8.0/hvcc/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14562 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.574456 hvcc-0.8.0/hvcc/core/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/core/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/core/hv2ir/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4237 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/BufferPool.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/Connection.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1688 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrConvolution.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1998 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrInlet.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1207 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrLorenz.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1486 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrOutlet.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1367 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrPack.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1695 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrReceive.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2345 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrSend.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1499 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrSwitchcase.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1705 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrTabhead.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1763 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrTabread.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1720 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HIrTabwrite.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2221 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangAdc.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10864 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangBinop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2055 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangBiquad.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2128 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangDac.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1523 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangDelay.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2010 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangIf.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1735 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangLine.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1481 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangMessage.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1704 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangNoise.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1592 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangPhasor.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1473 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangPrint.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1563 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangRandom.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2186 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangReceive.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2497 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangSend.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3325 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangSequence.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1473 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangSlice.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1477 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangSystem.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2161 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangTable.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4041 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangUnop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2927 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangVar.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2604 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HLangVario.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1039 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HeavyException.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    43580 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HeavyGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10293 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HeavyIrObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16786 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/HeavyLangObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11754 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/core/hv2ir/HeavyParser.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3954 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/LocalVars.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/core/hv2ir/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5472 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/core/hv2ir/hv2ir.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/core/json/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    50409 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/core/json/heavy.ir.json
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    42899 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/core/json/heavy.lang.json
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/buildjson/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/buildjson/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3191 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/buildjson/buildjson.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2daisy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2daisy/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5107 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2daisy/c2daisy.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9377 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2daisy/parameters.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2daisy/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7851 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2daisy/static/README.md
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2daisy/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5101 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      418 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2daisy/templates/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2dpf/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2dpf/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6604 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2dpf/c2dpf.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2dpf/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1071 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2dpf/static/README.md
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2dpf/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2522 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7957 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4070 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4468 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3430 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2243 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5221 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1227 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/Makefile_plugin
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      882 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2dpf/templates/Makefile_project
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.578456 hvcc-0.8.0/hvcc/generators/c2js/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2js/README.md
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2js/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10301 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2js/c2js.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2js/template/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6364 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2js/template/hv_worklet.js
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      323 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2js/template/hv_worklet_start.js
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8674 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2js/template/hv_wrapper.js
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5094 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2js/template/index.html
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2owl/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2owl/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6825 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2owl/c2owl.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2owl/deps/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7309 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2owl/deps/HvMessage.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10738 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2owl/deps/HvUtils.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2owl/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7536 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2owl/templates/HeavyOwl.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      511 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2owl/templates/HeavyOwlConstants.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2pdext/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2pdext/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4429 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2pdext/c2pdext.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2pdext/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    45865 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2pdext/static/Makefile.pdlibbuilder
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    38410 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2pdext/static/m_pd.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2pdext/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      576 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2pdext/templates/Makefile
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5137 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/c2pdext/templates/pd_external.c
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5509 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2unity/c2unity.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2unity/static/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2unity/static/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11516 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5538 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1399 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/static/xcode/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1269 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/static/xcode/Info.plist
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2unity/templates/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2unity/templates/android/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/templates/android/jni/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1745 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/android/jni/Android.mk
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      132 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/android/jni/Application.mk
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/templates/linux/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1451 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/linux/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2unity/templates/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/templates/source/unity/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15663 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4128 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       64 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/source/unity/PluginList.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10393 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10411 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2079 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2unity/templates/xcode/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    26264 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2wwise/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9537 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/c2wwise/c2wwise.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/linux/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1584 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/linux/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/resources/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4603 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9669 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      182 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.def
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2866 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6266 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      481 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1261 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.582456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2162 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2470 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9180 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2231 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      530 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      345 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_Wwise{{type}}PluginFactory.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2939 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8432 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1994 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5019 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1816 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3015 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7157 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4129 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2234 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/stdafx.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4601 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7351 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2691 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8485 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14466 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/runtime/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      475 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/runtime/Hv_{{name}}_WwisePluginRegister.cpp
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    27569 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18316 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4208 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    24299 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      889 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/Info.plist
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    25293 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       82 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/wwise.xcconfig
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.586456 hvcc-0.8.0/hvcc/generators/copyright/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/copyright/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/copyright/copyright_manager.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1570 2022-10-02 01:32:33.000000 hvcc-0.8.0/hvcc/generators/copyright/default_template.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2285 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/filters.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.590456 hvcc-0.8.0/hvcc/generators/ir2c/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4509 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlBinop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1507 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlCast.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2507 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlDelay.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1798 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlIf.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3341 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlMessage.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1748 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlPack.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1863 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlPrint.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1757 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlRandom.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1060 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlReceive.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2209 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlSend.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1740 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlSlice.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3157 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlSwitchcase.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1299 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlSystem.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1648 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlTabhead.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1794 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlTabread.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1805 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlTabwrite.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2608 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlUnop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2141 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ControlVar.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6610 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/HeavyObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2479 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/HeavyTable.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1721 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/PrettyfyC.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3271 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalBiquad.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2301 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalCPole.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalConvolution.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1867 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalDel1.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1708 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalEnvelope.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1918 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalLine.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalLorenz.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3650 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalMath.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2819 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalPhasor.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2078 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalRPole.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1952 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalSamphold.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2038 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalSample.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1926 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalTabhead.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3626 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalTabread.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2389 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalTabwrite.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4561 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/SignalVar.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12941 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/generators/ir2c/ir2c.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3740 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/ir2c_perf.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/ir2c/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9339 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HeavyContext.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4262 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HeavyContext.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11622 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HeavyContextInterface.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4072 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlBinop.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2033 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlBinop.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2040 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlCast.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1256 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlCast.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3597 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlDelay.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1494 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlDelay.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1405 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlIf.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1250 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlIf.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2505 2023-07-19 22:53:31.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPack.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPack.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1035 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPrint.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1094 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPrint.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1697 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlRandom.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1300 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlRandom.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2151 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSlice.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSlice.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSystem.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1167 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSystem.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1577 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabhead.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabhead.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1675 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabread.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabread.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1750 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabwrite.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1354 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabwrite.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2367 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlUnop.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1538 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlUnop.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2525 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlVar.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1401 2023-07-30 17:34:15.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlVar.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9066 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvHeavy.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15439 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvHeavy.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1412 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvHeavyInternal.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4803 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvLightPipe.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3274 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvLightPipe.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    21847 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMath.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7317 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessage.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessage.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4680 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessagePool.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2623 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessagePool.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6071 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessageQueue.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3270 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessageQueue.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9303 2023-08-07 18:08:50.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalBiquad.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7085 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalBiquad.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2412 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalCPole.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11740 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalCPole.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4821 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalConvolution.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1429 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalConvolution.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1386 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalDel1.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1769 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalDel1.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5852 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalEnvelope.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1392 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalEnvelope.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4974 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLine.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2891 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLine.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1189 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLorenz.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4976 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLorenz.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4917 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalPhasor.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5679 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalPhasor.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1724 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalRPole.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3743 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalRPole.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1537 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSamphold.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9492 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSamphold.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1753 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSample.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1379 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSample.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3192 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabread.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6721 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabread.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1783 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabwrite.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5552 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabwrite.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2890 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalVar.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalVar.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4251 2023-07-26 10:15:23.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvTable.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2625 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvTable.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1653 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvUtils.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9710 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/HvUtils.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4553 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/cpuid.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2319 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/ir2c/static/cpuid.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/ir2c/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11759 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/ir2c/templates/Heavy_NAME.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2517 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/generators/ir2c/templates/Heavy_NAME.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2720 2023-07-19 22:53:31.000000 hvcc-0.8.0/hvcc/generators/ir2c/templates/Heavy_NAME.hpp
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/vs2015/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1263 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/Heavy.sln
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13015 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9467 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2527 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/main.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/stdafx.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      305 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/stdafx.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      306 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/vs2015/Heavy/targetver.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/xcode/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2492 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy/main.c
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    81361 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      934 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1141 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1626 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9797 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49663 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      170 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Prefix.pch
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      903 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1662 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2902 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.m
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16216 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Views/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18184 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      436 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/Credits.rtf
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       45 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/InfoPlist.strings
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      809 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/main.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.598456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/tinywav/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4493 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1956 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.602456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      842 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2761 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.602456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3702 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1575 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      921 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13635 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.602456 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1077 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1576 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Info.plist
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5995 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7428 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      777 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/ViewController.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1049 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/ViewController.m
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      901 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/main.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.602456 hvcc-0.8.0/hvcc/interpreters/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.602456 hvcc-0.8.0/hvcc/interpreters/pd2hv/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/Connection.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2977 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/HeavyGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8422 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/HeavyObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1664 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/HvSwitchcase.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2327 2023-02-07 11:39:19.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/NotificationEnum.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1929 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdAudioIoObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5676 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdBinopObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9128 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1838 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdLetObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3461 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdLibSignalGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3078 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdMessageObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6952 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1900 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdPackObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    29733 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdParser.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2856 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdRaw.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5686 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdReceiveObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdRouteObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5537 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdSelectObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3805 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdSendObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2179 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdTableObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2230 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdTriggerObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3510 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/PdUnpackObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.570456 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.602456 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      798 2023-07-16 12:23:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      761 2023-08-03 16:17:56.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.606456 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy_converted/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6569 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.614456 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/abs.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/abs~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/atan.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/atan2.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/b.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bang.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      872 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bendin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      413 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bendout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2107 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bng.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bp~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      627 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/change.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      372 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/clip.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      376 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/clip~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      117 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/cnv.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/cos.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      817 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/cos~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      573 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2291 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      523 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      981 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      979 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/czero~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      694 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      692 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       61 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/declare.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/del.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      657 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delay.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delread~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1339 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      343 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/div.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/env~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      268 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/exp.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      228 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/exp~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/f.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/float.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/floatatom.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1082 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ftom.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      369 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ftom~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1239 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/hip~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/hradio.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/hsl.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      212 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/i.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      867 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/int.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2724 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/line.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      299 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/line~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      147 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/loadbang.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/log.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1088 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/lop~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1043 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/makenote.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1185 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/metro.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      250 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/midiin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      378 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/midiout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      258 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/midirealtimein.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      502 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/moses.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      492 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/mtof.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      366 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/mtof~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/nbx.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1234 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/noise~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      918 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/notein.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      422 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/noteout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1156 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/osc~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      914 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      451 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/pgmout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      351 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/phasor~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/pipe.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12790 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/poly.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      919 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      430 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/polytouchout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/powtodb~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      215 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/print.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/q8_rsqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      226 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/q8_sqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      835 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/random.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      807 2023-07-15 22:59:12.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rffttest~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      337 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rpole~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      907 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      367 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rzero_rev~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      417 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rzero~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      615 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      269 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/samplerate~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      267 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/sig~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/sin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      411 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/snapshot~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      359 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/spigot.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/sqrt.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      909 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/stripnote.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      585 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/swap.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      332 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/symbol.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      179 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/symbolatom.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2361 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1788 2023-08-07 18:14:41.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabplay~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      796 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabread.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2494 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1497 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      440 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tan.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      188 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tgl.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      869 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/timer.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      875 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/touchin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      373 2023-08-02 09:48:51.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/touchout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      946 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/until.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2709 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/vd~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/vradio.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/vsl.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      497 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/wrap.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      288 2022-08-20 00:37:38.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/wrap~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5213 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/interpreters/pd2hv/pd2hv.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1889 2023-08-07 18:08:05.000000 hvcc-0.8.0/hvcc/utils.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-08-07 18:18:01.574456 hvcc-0.8.0/hvcc.egg-info/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-08-07 18:18:01.000000 hvcc-0.8.0/hvcc.egg-info/PKG-INFO
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    20260 2023-08-07 18:18:01.000000 hvcc-0.8.0/hvcc.egg-info/SOURCES.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        1 2023-08-07 18:18:01.000000 hvcc-0.8.0/hvcc.egg-info/dependency_links.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       60 2023-08-07 18:18:01.000000 hvcc-0.8.0/hvcc.egg-info/entry_points.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       56 2023-08-07 18:18:01.000000 hvcc-0.8.0/hvcc.egg-info/requires.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       11 2023-08-07 18:18:01.000000 hvcc-0.8.0/hvcc.egg-info/top_level.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1047 2023-08-07 18:18:01.614456 hvcc-0.8.0/setup.cfg
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       38 2022-08-20 00:37:38.000000 hvcc-0.8.0/setup.py
```

### Comparing `hvcc-0.7.0/LICENSE` & `hvcc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/PKG-INFO` & `hvcc-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hvcc
-Version: 0.7.0
+Version: 0.8.0
 Summary: `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 Home-page: https://github.com/Wasted-Audio/hvcc
-Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.7.0.tar.gz
+Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.8.0.tar.gz
 Author: Enzien Audio, Wasted Audio
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Compilers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hvcc-0.7.0/README.md` & `hvcc-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 ## Requirements
 
 * python 3.7 or higher
   * `jinja2` (for generator templating)
   * `importlib_resources` (for reading static resources)
   * `json2daisy` (for daisy integration)
   * `tox` (for tests, optional)
+  * `numpy/scipy` (for tests, optional)
+  * `midifile` (for tests, optional)
   * `clang/clang++` (for building tests, optional)
 
 ## Installation
 
 hvcc is available from pypi.org and can be installed using python3 pip:
 
 `$ pip3 install hvcc`
```

### Comparing `hvcc-0.7.0/hvcc/__init__.py` & `hvcc-0.8.0/hvcc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import sys
 from typing import List, Dict, Optional
 
 from hvcc.interpreters.pd2hv import pd2hv
 from hvcc.core.hv2ir import hv2ir
 from hvcc.generators.ir2c import ir2c
 from hvcc.generators.ir2c import ir2c_perf
-from hvcc.generators.c2fabric import c2fabric
 from hvcc.generators.c2js import c2js
 from hvcc.generators.c2daisy import c2daisy
 from hvcc.generators.c2dpf import c2dpf
 from hvcc.generators.c2owl import c2owl
 from hvcc.generators.c2pdext import c2pdext
 from hvcc.generators.c2wwise import c2wwise
 from hvcc.generators.c2unity import c2unity
@@ -254,19 +253,14 @@
         'num_input_channels': num_input_channels,
         'num_output_channels': num_output_channels,
         'externs': externs,
         'copyright': copyright,
         'verbose': verbose
     }
 
-    if "fabric" in generators:
-        if verbose:
-            print("--> Generating Fabric plugin")
-        results["c2fabric"] = c2fabric.c2fabric.compile(**gen_args)
-
     if "js" in generators:
         if verbose:
             print("--> Generating Javascript")
         results["c2js"] = c2js.c2js.compile(**gen_args)
 
     if "daisy" in generators:
         if verbose:
```

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/BufferPool.py` & `hvcc-0.8.0/hvcc/core/hv2ir/BufferPool.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/Connection.py` & `hvcc-0.8.0/hvcc/core/hv2ir/Connection.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrConvolution.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrConvolution.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrInlet.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrInlet.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrLorenz.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrLorenz.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrOutlet.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrOutlet.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrPack.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrPack.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrReceive.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrReceive.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrSend.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrSend.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrSwitchcase.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrSwitchcase.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrTabhead.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrTabhead.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrTabread.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrTabread.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(
         self,
         obj_type: str,
         args: Optional[Dict] = None,
         graph: Optional[HeavyGraph] = None,
         annotations: Optional[Dict] = None
     ) -> None:
-        assert obj_type in {"__tabread~if", "__tabread~f", "__tabreadu~f", "__tabread"}
+        assert obj_type in {"__tabread~if", "__tabread~f", "__tabread_stoppable~f", "__tabreadu~f", "__tabread"}
         super().__init__(obj_type, args=args, graph=graph, annotations=annotations)
 
     def reduce(self) -> Optional[tuple]:
         if self.graph is not None:
             table_obj = self.graph.resolve_object_for_name(
                 self.args["table"],
                 ["table", "__table"])
```

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HIrTabwrite.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HIrTabwrite.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangAdc.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangAdc.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangBinop.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangBinop.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangBiquad.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangBiquad.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangDac.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangDac.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangDelay.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangDelay.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangIf.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangIf.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangLine.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangLine.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangMessage.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangMessage.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangNoise.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangNoise.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangPhasor.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangPhasor.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangPrint.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangPrint.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangRandom.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangRandom.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangReceive.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangReceive.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangSend.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangSend.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangSequence.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangSequence.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangSlice.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangSlice.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangSystem.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangSystem.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangTable.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangTable.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangUnop.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangUnop.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangVar.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangVar.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HLangVario.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HLangVario.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HeavyException.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HeavyException.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HeavyGraph.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HeavyGraph.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HeavyIrObject.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HeavyIrObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HeavyLangObject.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HeavyLangObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/HeavyParser.py` & `hvcc-0.8.0/hvcc/core/hv2ir/HeavyParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,15 @@
     "line": HLangLine,
     "random": HLangRandom,
     "delay": HLangDelay,
     "table": HLangTable,
     "slice": HLangSlice,
     "__tabread~if": HIrTabread,
     "__tabread~f": HIrTabread,
+    "__tabread_stoppable~f": HIrTabread,
     "__tabreadu~f": HIrTabread,
     "__tabread": HIrTabread,
     "__tabhead~f": HIrTabhead,
     "__tabhead": HIrTabhead,
     "__tabwrite~f": HIrTabwrite,
     "__tabwrite_stoppable~f": HIrTabwrite,
     "__tabwrite": HIrTabwrite,
```

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/LocalVars.py` & `hvcc-0.8.0/hvcc/core/hv2ir/LocalVars.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/hv2ir/hv2ir.py` & `hvcc-0.8.0/hvcc/core/hv2ir/hv2ir.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/core/json/heavy.ir.json` & `hvcc-0.8.0/hvcc/core/json/heavy.ir.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939393939393939%*

 * *Differences: {"'__tabread_stoppable~f'": "OrderedDict([('inlets', ['-->', '-->', '-->']), ('ir', "*

 * *                            "OrderedDict([('control', True), ('signal', True), ('init', True)])), "*

 * *                            "('outlets', ['~f>', '-->', '-->']), ('args', "*

 * *                            "[OrderedDict([('default', None), ('value_type', 'string'), ('name', "*

 * *                            "'table'), ('description', 'The name of the table to reference.'), "*

 * *                            "('required', True)])]), ( […]*

```diff
@@ -2774,14 +2774,44 @@
             "init": true,
             "signal": false
         },
         "outlets": [
             "-->"
         ]
     },
+    "__tabread_stoppable~f": {
+        "args": [
+            {
+                "default": null,
+                "description": "The name of the table to reference.",
+                "name": "table",
+                "required": true,
+                "value_type": "string"
+            }
+        ],
+        "inlets": [
+            "-->",
+            "-->",
+            "-->"
+        ],
+        "ir": {
+            "control": true,
+            "init": true,
+            "signal": true
+        },
+        "outlets": [
+            "~f>",
+            "-->",
+            "-->"
+        ],
+        "perf": {
+            "avx": 1,
+            "sse": 1
+        }
+    },
     "__tabreadu~f": {
         "args": [
             {
                 "default": null,
                 "description": "The name of the table to reference.",
                 "name": "table",
                 "required": true,
```

### Comparing `hvcc-0.7.0/hvcc/core/json/heavy.lang.json` & `hvcc-0.8.0/hvcc/core/json/heavy.lang.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/buildjson/buildjson.py` & `hvcc-0.8.0/hvcc/generators/buildjson/buildjson.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2daisy/c2daisy.py` & `hvcc-0.8.0/hvcc/generators/c2daisy/c2daisy.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2daisy/parameters.py` & `hvcc-0.8.0/hvcc/generators/c2daisy/parameters.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2daisy/static/README.md` & `hvcc-0.8.0/hvcc/generators/c2daisy/static/README.md`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp` & `hvcc-0.8.0/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/c2dpf.py` & `hvcc-0.8.0/hvcc/generators/c2dpf/c2dpf.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 import os
 import shutil
 import time
 import jinja2
 from typing import Dict, Optional
 
-from ..buildjson import buildjson
 from ..copyright import copyright_manager
 from ..filters import filter_uniqueid
 
 
 class c2dpf:
     """ Generates a DPF wrapper for a given patch.
     """
@@ -52,16 +51,14 @@
             dpf_meta = patch_meta.get("dpf", {})
         else:
             dpf_meta = {}
 
         dpf_path = dpf_meta.get('dpf_path', '')
 
         copyright_c = copyright_manager.get_copyright_for_c(copyright)
-        # copyright_plist = copyright or u"Copyright {0} Enzien Audio, Ltd." \
-        #     " All Rights Reserved.".format(datetime.datetime.now().year)
 
         try:
             # ensure that the output directory does not exist
             out_dir = os.path.abspath(out_dir)
             if os.path.exists(out_dir):
                 shutil.rmtree(out_dir)
 
@@ -121,44 +118,28 @@
                     class_name=f"HeavyDPF_{patch_name}",
                     num_input_channels=num_input_channels,
                     num_output_channels=num_output_channels,
                     receivers=receiver_list,
                     pool_sizes_kb=externs["memoryPoolSizesKb"],
                     copyright=copyright_c))
 
-            # generate list of Heavy source files
-            # files = os.listdir(source_dir)
-
-            # ======================================================================================
-            # Linux
-
             # plugin makefile
             with open(os.path.join(source_dir, "Makefile"), "w") as f:
                 f.write(env.get_template("Makefile_plugin").render(
                     name=patch_name,
                     meta=dpf_meta,
                     dpf_path=dpf_path))
 
             # project makefile
             with open(os.path.join(source_dir, "../../Makefile"), "w") as f:
                 f.write(env.get_template("Makefile_project").render(
                     name=patch_name,
                     meta=dpf_meta,
                     dpf_path=dpf_path))
 
-            buildjson.generate_json(
-                out_dir,
-                linux_x64_args=["-j"])
-            # macos_x64_args=["-project", "{0}.xcodeproj".format(patch_name), "-arch",
-            #                 "x86_64", "-alltargets"],
-            # win_x64_args=["/property:Configuration=Release", "/property:Platform=x64",
-            #               "/t:Rebuild", "{0}.sln".format(patch_name), "/m"],
-            # win_x86_args=["/property:Configuration=Release", "/property:Platform=x86",
-            #               "/t:Rebuild", "{0}.sln".format(patch_name), "/m"])
-
             return {
                 "stage": "c2dpf",
                 "notifs": {
                     "has_error": False,
                     "exception": None,
                     "warnings": [],
                     "errors": []
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/static/README.md` & `hvcc-0.8.0/hvcc/generators/c2dpf/static/README.md`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 {%- if meta.plugin_clap_id is defined %}
 #define DISTRHO_PLUGIN_CLAP_ID              "{{meta.plugin_clap_id}}"
 {% else %}
 #define DISTRHO_PLUGIN_CLAP_ID              "urn.hvcc.{{name}}"
 {%- endif %}
 #define DISTRHO_PLUGIN_NUM_INPUTS           {{num_input_channels}}
 #define DISTRHO_PLUGIN_NUM_OUTPUTS          {{num_output_channels}}
-#define DISTRHO_PLUGIN_IS_SYNTH             {{1 if num_output_channels > 0 and meta.midi_input else 0}}
-#define DISTRHO_PLUGIN_HAS_UI               {{1 if meta.enable_ui else 0}}
+#define DISTRHO_PLUGIN_IS_SYNTH             {{1 if num_output_channels > 0 and meta.midi_input is defined and meta.midi_input > 0 else 0}}
+#define DISTRHO_PLUGIN_HAS_UI               {{1 if meta.enable_ui is defined and meta.enable_ui is sameas true else 0}}
 #define DISTRHO_PLUGIN_IS_RT_SAFE           1
 #define DISTRHO_PLUGIN_WANT_PROGRAMS        0
 #define DISTRHO_PLUGIN_WANT_STATE           0
 #define DISTRHO_PLUGIN_WANT_TIMEPOS         1
 #define DISTRHO_PLUGIN_WANT_FULL_STATE      0
 #define DISTRHO_PLUGIN_WANT_MIDI_INPUT      {{meta.midi_input if meta.midi_input is defined else 1}}
 #define DISTRHO_PLUGIN_WANT_MIDI_OUTPUT     {{meta.midi_output if meta.midi_output is defined else 1}}
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.cpp` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 #define MIDI_RT_CLOCK           0xF8
 #define MIDI_RT_START           0xFA
 #define MIDI_RT_CONTINUE        0xFB
 #define MIDI_RT_STOP            0xFC
 #define MIDI_RT_ACTIVESENSE     0xFE
 #define MIDI_RT_RESET           0xFF
 
+#define HV_HASH_DPF_BPM         0xDF8C2721
+
 // midi realtime messages
 std::set<int> mrtSet {
   MIDI_RT_CLOCK,
   MIDI_RT_START,
   MIDI_RT_CONTINUE,
   MIDI_RT_STOP,
   MIDI_RT_RESET
@@ -117,29 +119,45 @@
         parameter.unit = "Hz";
       {%- endif %}
         parameter.hints = kParameterIsAutomatable
       {%- if v.attributes.type == 'bool': %}
         | kParameterIsBoolean
       {%- elif v.attributes.type == 'trig': -%}
         | kParameterIsTrigger
+      {%- elif v.attributes.type == 'int': -%}
+        | kParameterIsInteger
       {%- elif v.attributes.type in ['log', 'log_hz']: -%}
         | kParameterIsLogarithmic
       {%- endif %};
         parameter.ranges.min = {{v.attributes.min}}f;
         parameter.ranges.max = {{v.attributes.max}}f;
         parameter.ranges.def = {{v.attributes.default}}f;
-      {%- if v.attributes.type == 'db': %}
+      {%- if v.attributes.type == 'db' and not (meta.enumerators is defined and meta.enumerators[v.display] is defined): %}
         {
-          ParameterEnumerationValue* const enumValues =  new ParameterEnumerationValue[1];
+          ParameterEnumerationValue* const enumValues = new ParameterEnumerationValue[1];
           enumValues[0].value = {{v.attributes.min}}f;
           enumValues[0].label = "-inf";
           parameter.enumValues.count = 1;
           parameter.enumValues.values = enumValues;
         }
       {%- endif %}
+      {%- if meta.enumerators is defined and meta.enumerators[v.display] is defined %}
+        {% set enums = meta.enumerators[v.display] %}
+        {% set enumlen = enums|length %}
+        if (ParameterEnumerationValue *values = new ParameterEnumerationValue[{{enumlen}}])
+        {
+          parameter.enumValues.restrictedMode = true;
+          {% for i in enums -%}
+          values[{{loop.index - 1}}].value = {{loop.index - 1}}.0f;
+          values[{{loop.index - 1}}].label = "{{i}}";
+          {% endfor -%}
+          parameter.enumValues.count = {{enumlen}};
+          parameter.enumValues.values = values;
+        }
+      {%- endif %}
         break;
     {% endfor %}
   }
   {% endif %}
 }
 
 // -------------------------------------------------------------------
@@ -184,15 +202,15 @@
 // }
 
 // void {{class_name}}::deactivate()
 // {
 
 // }
 
-{%- if meta.midi_input is defined and meta.midi_input == 1%}
+{%- if meta.midi_input is defined and meta.midi_input == 1 %}
 #if DISTRHO_PLUGIN_WANT_MIDI_INPUT
 {% include 'HeavyDPF_MIDI_Input.cpp' %}
 #endif
 {% endif %}
 
 {%- if meta.midi_output is defined and meta.midi_output == 1 %}
 #if DISTRHO_PLUGIN_WANT_MIDI_OUTPUT
@@ -209,14 +227,18 @@
 void {{class_name}}::run(const float** inputs, float** outputs, uint32_t frames, const MidiEvent* midiEvents, uint32_t midiEventCount)
 {
   handleMidiInput(frames, midiEvents, midiEventCount);
 #else
 void {{class_name}}::run(const float** inputs, float** outputs, uint32_t frames)
 {
 #endif
+  const TimePosition& timePos(getTimePosition());
+  if (timePos.playing && timePos.bbt.valid)
+    _context->sendMessageToReceiverV(HV_HASH_DPF_BPM, 0, "f", timePos.bbt.beatsPerMinute);
+
   _context->process((float**)inputs, outputs, frames);
 }
 
 // -------------------------------------------------------------------
 // Callbacks
 
 void {{class_name}}::sampleRateChanged(double newSampleRate)
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.hpp` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 
 #include "DistrhoUI.hpp"
 #include "ResizeHandle.hpp"
 
 START_NAMESPACE_DISTRHO
 
 // --------------------------------------------------------------------------------------------------------------------
-
 class ImGuiPluginUI : public UI
 {
     {% for k, v in receivers -%}
-        float f{{v.display|lower}} = {{v.attributes.default}}f;
-    {% endfor %}
+        {%- if v.attributes.type == 'bool': %}
+    bool f{{v.display|lower}} = {{v.attributes.default}}f != 0.0f;
+        {%- elif v.attributes.type == 'int': %}
+    int f{{v.display|lower}} = {{v.attributes.default}};
+        {%- else %}
+    float f{{v.display|lower}} = {{v.attributes.default}}f;
+        {%- endif %}
+    {%- endfor %}
+
     ResizeHandle fResizeHandle;
 
     // ----------------------------------------------------------------------------------------------------------------
 
 public:
    /**
       UI class constructor.
@@ -42,15 +48,19 @@
     */
     void parameterChanged(uint32_t index, float value) override
     {
     {%- if receivers|length > 0 %}
         switch (index) {
             {% for k, v  in receivers -%}
             case {{loop.index-1}}:
+                {%- if v.attributes.type == 'bool': %}
+                f{{v.display|lower}} = value != 0.0f;
+                {%- else %}
                 f{{v.display|lower}} = value;
+                {%- endif %}
                 break;
             {% endfor %}
             default: return;
         }
     {% else %}
         // nothing to do
     {%- endif %}
@@ -70,32 +80,63 @@
         const float margin = 20.0f * getScaleFactor();
 
         ImGui::SetNextWindowPos(ImVec2(margin, margin));
         ImGui::SetNextWindowSize(ImVec2(width - 2 * margin, height - 2 * margin));
 
         if (ImGui::Begin("{{name.replace('_', ' ')}}", nullptr, ImGuiWindowFlags_NoResize + ImGuiWindowFlags_NoCollapse))
         {
-    {% for k, v in receivers %}
-            if (ImGui::SliderFloat("{{v.display.replace('_', ' ')}}", &f{{v.display|lower}}, {{v.attributes.min}}f, {{v.attributes.max}}f))
+    {%- for k, v in receivers %}
+        {%- set v_display = v.display|lower %}
+        {%- if meta.enumerators is defined and meta.enumerators[v.display] is defined -%}
+            {%- set enums = meta.enumerators[v.display] -%}
+            {%- set enumlen = enums|length %}
+            {%- set enum_list = v_display + "_list" %}
+
+            const char* {{enum_list}}[{{enumlen}}] = {
+                {%- for i in enums %}
+                "{{i}}",
+                {%- endfor %}
+            };
+
+            if (ImGui::BeginCombo("{{v.display.replace('_', ' ')}}", {{enum_list}}[f{{v_display}}]))
+            {
+                for (int n = 0; n < {{enumlen}}; n++)
+                {
+                    bool is_selected = (f{{v_display}} == n);
+                    if (ImGui::Selectable({{enum_list}}[n], is_selected))
+                    {
+                        f{{v_display}} = n;
+                        editParameter({{loop.index-1}}, true);
+                        setParameterValue({{loop.index-1}}, f{{v_display}});
+                    }
+                    if (is_selected)
+                        ImGui::SetItemDefaultFocus();
+                }
+                ImGui::EndCombo();
+            }
+        {%- else %}
+            {%- if v.attributes.type == 'bool': %}
+            if (ImGui::Toggle("{{v.display.replace('_', ' ')}}", &f{{v_display}}))
+            {%- else %}
+            if (ImGui::SliderFloat("{{v.display.replace('_', ' ')}}", &f{{v_display}}, {{v.attributes.min}}f, {{v.attributes.max}}f))
+            {%- endif %}
             {
                 if (ImGui::IsItemActivated())
                 {
                     editParameter({{loop.index-1}}, true);
-                    if (ImGui::IsMouseDoubleClicked(0))
-                        f{{v.display|lower}} = {{v.attributes.default}}f;
-
-                    setParameterValue({{loop.index-1}}, f{{v.display|lower}});
+                    setParameterValue({{loop.index-1}}, f{{v_display}});
                 }
             }
+        {%- endif %}
     {% endfor %}
             if (ImGui::IsItemDeactivated())
             {
-            {% for i in range(0, receivers|length) -%}
+            {%- for i in range(0, receivers|length) %}
                 editParameter({{i}}, false);
-            {% endfor %}
+            {%- endfor %}
             }
         }
         ImGui::End();
     }
 
     DISTRHO_DECLARE_NON_COPYABLE_WITH_LEAK_DETECTOR(ImGuiPluginUI)
 };
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_plugin` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/Makefile_plugin`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 {%- if meta.makefile_dep is defined %}
 	{%- for dependency in meta.makefile_dep %}
 BUILD_CXX_FLAGS += -I ../../{{dpf_path}}{{dependency}}
 	{%- endfor %}
 {%- endif %}
 
 LINK_FLAGS += -lpthread
-CFLAGS += -Wno-unused-parameter
+CFLAGS += -Wno-unused-parameter -std=c11
 CXXFLAGS += -Wno-unused-parameter
 
 {% if meta.plugin_formats is defined %}
 	{%- for format in meta.plugin_formats %}
 TARGETS += {{format}}
 	{%- endfor %}
 {% else %}
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_project` & `hvcc-0.8.0/hvcc/generators/c2dpf/templates/Makefile_project`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2fabric/c2fabric.py` & `hvcc-0.8.0/hvcc/generators/c2unity/c2unity.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 import jinja2
 import os
 import shutil
 import time
 from typing import Dict, Optional
 
-from ..buildjson import buildjson
 from ..copyright import copyright_manager
-from ..filters import filter_templates, filter_xcode_build, filter_xcode_copy, filter_xcode_fileref
+from ..buildjson import buildjson
+from ..filters import filter_string_cap, filter_templates, filter_xcode_build, filter_xcode_fileref
 
 
-class c2fabric:
-    """Generates a DSP component for Fabric.
+class c2unity:
+    """Generates a Audio Native Plugin wrapper for Unity 5.
     """
 
     @classmethod
     def compile(
         cls,
         c_src_dir: str,
         out_dir: str,
@@ -41,83 +41,82 @@
         num_output_channels: int = 0,
         copyright: Optional[str] = None,
         verbose: Optional[bool] = False
     ) -> Dict:
 
         tick = time.time()
 
-        in_parameter_list = externs["parameters"]["in"]
-        out_parameter_list = externs["parameters"]["out"]
-        in_event_list = externs["events"]["in"]
-        out_event_list = externs["events"]["out"]
+        parameter_list = externs["parameters"]["in"]
+        event_list = externs["events"]["in"]
+        table_list = externs["tables"]
 
-        out_dir = os.path.join(out_dir, "fabric")
+        out_dir = os.path.join(out_dir, "unity")
         patch_name = patch_name or "heavy"
 
         copyright = copyright_manager.get_copyright_for_c(copyright)
 
         # initialise the jinja template environment
         env = jinja2.Environment()
         env.filters["xcode_build"] = filter_xcode_build
-        env.filters["xcode_copy"] = filter_xcode_copy
         env.filters["xcode_fileref"] = filter_xcode_fileref
+        env.filters["cap"] = filter_string_cap
         env.loader = jinja2.FileSystemLoader(
             encoding="utf-8-sig",
             searchpath=[os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates")])
 
+        static_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "static")
         src_out_dir = os.path.join(out_dir, "source")
 
         try:
             # ensure that the output directory does not exist
             out_dir = os.path.abspath(out_dir)
             if os.path.exists(out_dir):
                 shutil.rmtree(out_dir)
 
+            # copy over static files
+            shutil.copytree(static_dir, out_dir)
+
             # copy over generated C source files
             src_out_dir = os.path.join(out_dir, "source", "heavy")
             shutil.copytree(c_src_dir, src_out_dir)
 
-            files_to_copy = [f"Hv_{patch_name}_FabricDSP.cs", f"Hv_{patch_name}_FabricDSPEditor.cs"]
-
             # generate files from templates
             for f in env.list_templates(filter_func=filter_templates):
                 file_path = os.path.join(out_dir, f)
                 file_path = file_path.replace("{{name}}", patch_name)
 
                 if not os.path.exists(os.path.dirname(file_path)):
                     os.makedirs(os.path.dirname(file_path))
 
                 with open(file_path, "w") as g:
                     g.write(env.get_template(f).render(
                         patch_name=patch_name,
-                        project_name=f"Hv_{patch_name}_Fabric",
-                        lib_name=patch_name,
+                        files=os.listdir(src_out_dir),
                         num_input_channels=num_input_channels,
                         num_output_channels=num_output_channels,
-                        in_parameters=in_parameter_list,
-                        out_parameters=out_parameter_list,
-                        in_events=in_event_list,
-                        out_events=out_event_list,
+                        parameters=parameter_list,
+                        events=event_list,
+                        tables=table_list,
+                        pool_sizes_kb=externs["memoryPoolSizesKb"],
                         compile_files=os.listdir(src_out_dir),
-                        copy_files=files_to_copy,
                         copyright=copyright))
 
             buildjson.generate_json(
                 out_dir,
                 android_armv7a_args=["APP_ABI=armeabi-v7a", "-j"],
                 linux_x64_args=["-j"],
-                macos_x64_args=["-project", f"Hv_{patch_name}_Fabric.xcodeproj",
+                macos_x64_args=["-project", f"Hv_{patch_name}_Unity.xcodeproj",
                                 "-arch", "x86_64", "-alltargets"],
                 win_x64_args=["/property:Configuration=Release", "/property:Platform=x64",
-                              "/t:Rebuild", f"Hv_{patch_name}_Fabric.sln", "/m"],
+                              "/t:Rebuild", f"Hv_{patch_name}_Unity.sln", "/m"],
                 win_x86_args=["/property:Configuration=Release", "/property:Platform=x86",
-                              "/t:Rebuild", f"Hv_{patch_name}_Fabric.sln", "/m"])
+                              "/t:Rebuild", f"Hv_{patch_name}_Unity.sln", "/m"])
 
             return {
-                "stage": "c2fabric",
+                "stage": "c2unity",
                 "notifs": {
                     "has_error": False,
                     "exception": None,
                     "warnings": [],
                     "errors": []
                 },
                 "in_dir": c_src_dir,
@@ -125,15 +124,15 @@
                 "out_dir": out_dir,
                 "out_file": "",
                 "compile_time": time.time() - tick
             }
 
         except Exception as e:
             return {
-                "stage": "c2fabric",
+                "stage": "c2unity",
                 "notifs": {
                     "has_error": True,
                     "exception": e,
                     "warnings": [],
                     "errors": [{
                         "enum": -1,
                         "message": str(e)
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Microsoft Visual Studio Solution File, Format Version 12.00
 # Visual Studio 14
 VisualStudioVersion = 14.0.23107.0
 MinimumVisualStudioVersion = 10.0.40219.1
-Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "lib{{lib_name}}", "lib{{lib_name}}.vcxproj", "{F7CFEF5A-54BD-42E8-A59E-54ABAEB4EA9C}"
+Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "Hv_{{patch_name}}_AudioLib", "Hv_{{patch_name}}_AudioLib.vcxproj", "{F7CFEF5A-54BD-42E8-A59E-54ABAEB4EA9C}"
+EndProject
+Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "AudioPlugin_Hv_{{patch_name}}", "AudioPlugin_Hv_{{patch_name}}.vcxproj", "{F748C943-E015-44C9-A1CE-B5125DB06999}"
 EndProject
 Global
 	GlobalSection(SolutionConfigurationPlatforms) = preSolution
 		Release|x64 = Release|x64
 		Release|x86 = Release|x86
 		Debug|x64 = Debug|x64
 		Debug|x86 = Debug|x86
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj`

 * *Files 18% similar despite different names*

#### Comparing `hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj`

```diff
@@ -15,27 +15,32 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <ItemGroup>
-    {%- for f in compile_files if f.endswith((&quot;.c&quot;, &quot;.cpp&quot;)) %}
+    {%- for f in files if f.endswith((&quot;.c&quot;, &quot;.cpp&quot;)) %}
     <ClCompile Include="../source/heavy/{{f}}"/>
     {%- endfor %}
+    <ClCompile Include="../source/unity/AudioPluginUtil.cpp"/>
+    <ClCompile Include="../source/unity/Hv_{{patch_name}}_AudioPlugin.cpp"/>
   </ItemGroup>
   <ItemGroup>
-    {%- for f in compile_files if f.endswith((&quot;.h&quot;, &quot;.hpp&quot;)) %}
+    {%- for f in files if f.endswith((&quot;.h&quot;, &quot;.hpp&quot;)) %}
     <ClInclude Include="../source/heavy/{{f}}"/>
     {%- endfor %}
+    <ClInclude Include="../source/unity/AudioPluginInterface.h"/>
+    <ClInclude Include="../source/unity/AudioPluginUtil.h"/>
+    <ClInclude Include="../source/unity/PluginList.h"/>
   </ItemGroup>
   <PropertyGroup Label="Globals">
     <ProjectGuid>{F748C943-E015-44C9-A1CE-B5125DB06999}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>lib{{patch_name}}</RootNamespace>
+    <RootNamespace>{{name}}</RootNamespace>
     <WindowsTargetPlatformVersion>8.1</WindowsTargetPlatformVersion>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>DynamicLibrary</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <PlatformToolset>v140</PlatformToolset>
@@ -74,159 +79,111 @@
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
-    <LinkIncremental>true</LinkIncremental>
-    <OutDir>$(SolutionDir)..\build\win\x86\debug\Plugins\x86\win\</OutDir>
-    <IntDir>$(SolutionDir)win\x86\debug\</IntDir>
-    <TargetName>lib{{lib_name}}</TargetName>
+    <LinkIncremental>false</LinkIncremental>
+    <OutDir>$(SolutionDir)..\build\win\x86\debug\</OutDir>
+    <IntDir>$(SolutionDir)intermediate\win\x86\debug\$(ProjectName)\</IntDir>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
-    <LinkIncremental>true</LinkIncremental>
-    <OutDir>$(SolutionDir)..\build\win\x64\debug\Plugins\x64\win\</OutDir>
-    <IntDir>$(SolutionDir)win\x64\debug\</IntDir>
-    <TargetName>lib{{lib_name}}</TargetName>
+    <LinkIncremental>false</LinkIncremental>
+    <OutDir>$(SolutionDir)..\build\win\x64\debug\</OutDir>
+    <IntDir>$(SolutionDir)intermediate\win\x64\debug\$(ProjectName)\</IntDir>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <LinkIncremental>false</LinkIncremental>
-    <OutDir>$(SolutionDir)..\build\win\x86\release\Plugins\x86\win\</OutDir>
-    <IntDir>$(SolutionDir)win\x86\release</IntDir>
-    <TargetName>lib{{lib_name}}</TargetName>
-    <GenerateManifest>false</GenerateManifest>
+    <OutDir>$(SolutionDir)..\build\win\x86\release\</OutDir>
+    <IntDir>$(SolutionDir)intermediate\win\x86\release\$(ProjectName)\</IntDir>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
-    <OutDir>$(SolutionDir)..\build\win\x64\release\Plugins\x64\win\</OutDir>
-    <IntDir>$(SolutionDir)win\x64\release\</IntDir>
-    <TargetName>lib{{lib_name}}</TargetName>
-    <GenerateManifest>false</GenerateManifest>
+    <OutDir>$(SolutionDir)..\build\win\x64\release\</OutDir>
+    <IntDir>$(SolutionDir)intermediate\win\x64\release\$(ProjectName)\</IntDir>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_WINDOWS;_CRT_SECURE_NO_WARNINGS;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
+      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
+      <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
+      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
-      <ProfileGuidedDatabase>$(IntDir)$(TargetName).pgd</ProfileGuidedDatabase>
-      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
-      <LinkTimeCodeGeneration>UseLinkTimeCodeGeneration</LinkTimeCodeGeneration>
     </Link>
-    <PostBuildEvent>
-      <Command>md $(OutDir)..\..\..\Editor\
-        {%- for f in copy_files %}
-        {%- if f.endswith(&quot;Editor.cs&quot;) %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\Editor\{{f}}
-        {%- else %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\{{f}}
-        {%- endif %}
-        {%- endfor %}</Command>
-    </PostBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>_DEBUG;_WINDOWS;_CRT_SECURE_NO_WARNINGS;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>_DEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
+      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
+      <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
+      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
-      <ProfileGuidedDatabase>$(IntDir)$(TargetName).pgd</ProfileGuidedDatabase>
-      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
-      <LinkTimeCodeGeneration>UseLinkTimeCodeGeneration</LinkTimeCodeGeneration>
     </Link>
-    <PostBuildEvent>
-      <Command>md $(OutDir)..\..\..\Editor\
-        {%- for f in copy_files %}
-        {%- if f.endswith(&quot;Editor.cs&quot;) %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\Editor\{{f}}
-        {%- else %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\{{f}}
-        {%- endif %}
-        {%- endfor %}</Command>
-    </PostBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
       <WarningLevel>Level3</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_WINDOWS;_CRT_SECURE_NO_WARNINGS;HV_SIMD_SSE%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
-      <DebugInformationFormat>None</DebugInformationFormat>
+      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
-      <GenerateDebugInformation>false</GenerateDebugInformation>
+      <GenerateDebugInformation>No</GenerateDebugInformation>
+      <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
+      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
-      <ProfileGuidedDatabase>$(IntDir)$(TargetName).pgd</ProfileGuidedDatabase>
-      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
-      <FullProgramDatabaseFile>false</FullProgramDatabaseFile>
       <LinkTimeCodeGeneration>UseLinkTimeCodeGeneration</LinkTimeCodeGeneration>
     </Link>
-    <PostBuildEvent>
-      <Command>md $(OutDir)..\..\..\Editor\
-        {%- for f in copy_files %}
-        {%- if f.endswith(&quot;Editor.cs&quot;) %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\Editor\{{f}}
-        {%- else %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\{{f}}
-        {%- endif %}
-        {%- endfor %}</Command>
-    </PostBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <ClCompile>
       <WarningLevel>Level3</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>NDEBUG;_WINDOWS;_CRT_SECURE_NO_WARNINGS;HV_SIMD_SSE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>NDEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;HV_SIMD_SSE;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
-      <DebugInformationFormat>None</DebugInformationFormat>
+      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
-      <GenerateDebugInformation>false</GenerateDebugInformation>
+      <GenerateDebugInformation>No</GenerateDebugInformation>
+      <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
+      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
-      <ProfileGuidedDatabase>$(IntDir)$(TargetName).pgd</ProfileGuidedDatabase>
-      <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
-      <FullProgramDatabaseFile>false</FullProgramDatabaseFile>
       <LinkTimeCodeGeneration>UseLinkTimeCodeGeneration</LinkTimeCodeGeneration>
     </Link>
-    <PostBuildEvent>
-      <Command>md $(OutDir)..\..\..\Editor\
-        {%- for f in copy_files %}
-        {%- if f.endswith(&quot;Editor.cs&quot;) %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\Editor\{{f}}
-        {%- else %}
-        copy $(SolutionDir)..\source\fabric\{{f}} $(OutDir)..\..\..\{{f}}
-        {%- endif %}
-        {%- endfor %}</Command>
-    </PostBuildEvent>
   </ItemDefinitionGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2js/c2js.py` & `hvcc-0.8.0/hvcc/generators/c2js/c2js.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2js/template/hv_worklet.js` & `hvcc-0.8.0/hvcc/generators/c2js/template/hv_worklet.js`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2js/template/hv_wrapper.js` & `hvcc-0.8.0/hvcc/generators/c2js/template/hv_wrapper.js`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2js/template/index.html` & `hvcc-0.8.0/hvcc/generators/c2js/template/index.html`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2owl/c2owl.py` & `hvcc-0.8.0/hvcc/generators/c2owl/c2owl.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2owl/deps/HvMessage.c` & `hvcc-0.8.0/hvcc/generators/c2owl/deps/HvMessage.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2owl/deps/HvUtils.h` & `hvcc-0.8.0/hvcc/generators/c2owl/deps/HvUtils.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2owl/templates/HeavyOwl.hpp` & `hvcc-0.8.0/hvcc/generators/c2owl/templates/HeavyOwl.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2pdext/c2pdext.py` & `hvcc-0.8.0/hvcc/generators/c2pdext/c2pdext.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 import shutil
 import time
 import jinja2
 from typing import Dict, Optional
 
 from ..copyright import copyright_manager
-from ..filters import filter_max, filter_xcode_build, filter_xcode_fileref
+from ..filters import filter_max
 
 
 class c2pdext:
     """Generates a Pure Data external wrapper for a given patch.
     """
 
     @classmethod
@@ -47,63 +47,56 @@
         out_dir = os.path.join(out_dir, "pdext")
         receiver_list = externs["parameters"]["in"]
 
         copyright = copyright_manager.get_copyright_for_c(copyright)
 
         patch_name = patch_name or "heavy"
         ext_name = f"{patch_name}~"
-        struct_name = patch_name + "_tilde"
+        struct_name = f"{patch_name}_tilde"
 
         # ensure that the output directory does not exist
         out_dir = os.path.abspath(out_dir)
         if os.path.exists(out_dir):
             shutil.rmtree(out_dir)
 
         # copy over generated C source files
         shutil.copytree(c_src_dir, out_dir)
 
         # copy over static files
         shutil.copy(
             os.path.join(os.path.dirname(os.path.abspath(__file__)), "static", "m_pd.h"),
-            out_dir)
+            f"{out_dir}/")
+        shutil.copy(
+            os.path.join(os.path.dirname(os.path.abspath(__file__)), "static", "Makefile.pdlibbuilder"),
+            f"{out_dir}/../")
 
         try:
             # initialise the jinja template environment
             env = jinja2.Environment()
             env.filters["max"] = filter_max
-            env.filters["xcode_build"] = filter_xcode_build
-            env.filters["xcode_fileref"] = filter_xcode_fileref
             env.loader = jinja2.FileSystemLoader(
                 os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates"))
 
             # generate Pd external wrapper from template
-            pdext_path = os.path.join(out_dir, f"{struct_name}.c")
+            pdext_path = os.path.join(out_dir, f"{ext_name}.c")
             with open(pdext_path, "w") as f:
                 f.write(env.get_template("pd_external.c").render(
                     name=patch_name,
                     struct_name=struct_name,
                     display_name=ext_name,
                     num_input_channels=num_input_channels,
                     num_output_channels=num_output_channels,
                     receivers=receiver_list,
                     copyright=copyright))
 
-            # generate Xcode project
-            xcode_path = os.path.join(out_dir, f"{struct_name}.xcodeproj")
-            os.mkdir(xcode_path)  # create the xcode project bundle
-            pbxproj_path = os.path.join(xcode_path, "project.pbxproj")
-
-            # generate list of source files
-            files = [g for g in os.listdir(out_dir) if g.endswith((".h", ".hpp", ".c", ".cpp"))]
-
-            # render the pbxproj file
-            with open(pbxproj_path, "w") as f:
-                f.write(env.get_template("project.pbxproj").render(
-                    name=ext_name,
-                    files=files))
+            # generate Makefile from template
+            pdext_path = os.path.join(out_dir, "../Makefile")
+            with open(pdext_path, "w") as f:
+                f.write(env.get_template("Makefile").render(
+                    name=patch_name))
 
             return {
                 "stage": "c2pdext",
                 "notifs": {
                     "has_error": False,
                     "exception": None,
                     "warnings": [],
@@ -127,10 +120,10 @@
                         "enum": -1,
                         "message": str(e)
                     }]
                 },
                 "in_dir": c_src_dir,
                 "in_file": "",
                 "out_dir": out_dir,
-                "out_file": os.path.basename(pdext_path),
+                "out_file": "",
                 "compile_time": time.time() - tick
             }
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2pdext/templates/pd_external.c` & `hvcc-0.8.0/hvcc/generators/c2pdext/templates/pd_external.c`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 static void printHook(HeavyContextInterface *c, const char *receiverName, const char *msgString, const HvMessage *m) {
   double timestampMs = 1000.0 * ((double) hv_msg_getTimestamp(m)) / hv_getSampleRate(c);
   post("[{{display_name}} @ %0.3gms] %s: %s", timestampMs, receiverName, msgString);
 }
 
 static void sendHook(HeavyContextInterface *c, const char *receiverName, unsigned int receiverHash, const HvMessage * m) {
-  if (!strcmp(receiverName, "#HV_TO_PD")) {
+  if (!strcmp(receiverName, "HV_TO_PD")) {
     t_outlet *const outlet = ((t_{{struct_name}} *) hv_getUserData(c))->msgOutlet;
     if (hv_msg_getNumElements(m) == 1) {
       if (hv_msg_isFloat(m, 0)) {
         outlet_float(outlet, hv_msg_getFloat(m, 0));
       } else if (hv_msg_isBang(m, 0)) {
         outlet_bang(outlet);
       } else if (hv_msg_isSymbol(m, 0)) {
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h` & `hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp` & `hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h` & `hvcc-0.8.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/static/xcode/Info.plist` & `hvcc-0.8.0/hvcc/generators/c2unity/static/xcode/Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/Android.mk` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/linux/Makefile` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/linux/Makefile`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj`

 * *Files 14% similar despite different names*

#### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj`

```diff
@@ -18,29 +18,24 @@
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <ItemGroup>
     {%- for f in files if f.endswith((&quot;.c&quot;, &quot;.cpp&quot;)) %}
     <ClCompile Include="../source/heavy/{{f}}"/>
     {%- endfor %}
-    <ClCompile Include="../source/unity/AudioPluginUtil.cpp"/>
-    <ClCompile Include="../source/unity/Hv_{{patch_name}}_AudioPlugin.cpp"/>
   </ItemGroup>
   <ItemGroup>
     {%- for f in files if f.endswith((&quot;.h&quot;, &quot;.hpp&quot;)) %}
     <ClInclude Include="../source/heavy/{{f}}"/>
     {%- endfor %}
-    <ClInclude Include="../source/unity/AudioPluginInterface.h"/>
-    <ClInclude Include="../source/unity/AudioPluginUtil.h"/>
-    <ClInclude Include="../source/unity/PluginList.h"/>
   </ItemGroup>
   <PropertyGroup Label="Globals">
     <ProjectGuid>{F748C943-E015-44C9-A1CE-B5125DB06999}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>{{name}}</RootNamespace>
+    <RootNamespace>Hv_{{patch_name}}_AudioLib</RootNamespace>
     <WindowsTargetPlatformVersion>8.1</WindowsTargetPlatformVersion>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>DynamicLibrary</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <PlatformToolset>v140</PlatformToolset>
@@ -105,85 +100,93 @@
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
       <Optimization>Disabled</Optimization>
       <PreprocessorDefinitions>WIN32;_DEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
-      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
       <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
     </Link>
+    <PostBuildEvent>
+      <Command>copy $(SolutionDir)..\source\unity\Hv_{{patch_name}}_AudioLib.cs $(OutDir)\Hv_{{patch_name}}_AudioLib.cs</Command>
+    </PostBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
       <Optimization>Disabled</Optimization>
       <PreprocessorDefinitions>_DEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
-      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
       <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
     </Link>
+    <PostBuildEvent>
+      <Command>copy $(SolutionDir)..\source\unity\Hv_{{patch_name}}_AudioLib.cs $(OutDir)\Hv_{{patch_name}}_AudioLib.cs</Command>
+    </PostBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
       <WarningLevel>Level3</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
       <PreprocessorDefinitions>WIN32;NDEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
-      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
       <GenerateDebugInformation>No</GenerateDebugInformation>
       <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
       <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
       <LinkTimeCodeGeneration>UseLinkTimeCodeGeneration</LinkTimeCodeGeneration>
     </Link>
+    <PostBuildEvent>
+      <Command>copy $(SolutionDir)..\source\unity\Hv_{{patch_name}}_AudioLib.cs $(OutDir)\Hv_{{patch_name}}_AudioLib.cs</Command>
+    </PostBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <ClCompile>
       <WarningLevel>Level3</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
       <PreprocessorDefinitions>NDEBUG;_WINDOWS;_USRDLL;_CRT_SECURE_NO_WARNINGS;HV_SIMD_SSE;_XKEYCHECK_H;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
-      <AdditionalIncludeDirectories>$(SolutionDir)..\source</AdditionalIncludeDirectories>
     </ClCompile>
     <Link>
       <SubSystem>Windows</SubSystem>
       <GenerateDebugInformation>No</GenerateDebugInformation>
       <ProgramDatabaseFile>$(IntDir)$(ProjectName).pdb</ProgramDatabaseFile>
       <ImportLibrary>$(IntDir)$(TargetName).lib</ImportLibrary>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
       <AdditionalDependencies>mincore.lib</AdditionalDependencies>
       <IgnoreSpecificDefaultLibraries>kernel32.lib; ole32.lib; system32.lib; advapi32.dll</IgnoreSpecificDefaultLibraries>
       <LinkTimeCodeGeneration>UseLinkTimeCodeGeneration</LinkTimeCodeGeneration>
     </Link>
+    <PostBuildEvent>
+      <Command>copy $(SolutionDir)..\source\unity\Hv_{{patch_name}}_AudioLib.cs $(OutDir)\Hv_{{patch_name}}_AudioLib.cs</Command>
+    </PostBuildEvent>
   </ItemDefinitionGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj` & `hvcc-0.8.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/c2wwise.py` & `hvcc-0.8.0/hvcc/generators/c2wwise/c2wwise.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/linux/Makefile` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/linux/Makefile`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/stdafx.h` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/include/stdafx.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Info.plist` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj` & `hvcc-0.8.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/copyright/copyright_manager.py` & `hvcc-0.8.0/hvcc/generators/copyright/copyright_manager.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/copyright/default_template.txt` & `hvcc-0.8.0/hvcc/generators/copyright/default_template.txt`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/filters.py` & `hvcc-0.8.0/hvcc/generators/filters.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlBinop.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlBinop.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlCast.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlCast.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlDelay.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlDelay.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlIf.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlIf.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlMessage.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlMessage.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlPack.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlPack.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlPrint.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlPrint.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlRandom.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlRandom.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlReceive.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlReceive.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlSend.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlSend.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlSlice.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlSlice.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlSwitchcase.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlSwitchcase.py`

 * *Files 20% similar despite different names*

```diff
@@ -52,15 +52,23 @@
         objects: Dict
     ) -> List[str]:
         # generate the onMessage implementation
         out_list = [
             f"cSwitchcase_{obj_id}_onMessage(HeavyContextInterface *_c, void *o, int letIn, "
             f"const HvMessage *const m, void *sendMessage) {{"
         ]
-        out_list.append("switch (msg_getHash(m, 0)) {")
+        out_list.append("int msgIndex = 0;")
+        out_list.append("switch (msg_getHash(m, msgIndex)) {")
+        out_list.append(f"case {cls.get_hash_string('symbol')}: {{ // \"symbol\"")
+        out_list.append("msgIndex = 1;")
+        out_list.append("break;")
+        out_list.append("}")  # end symbol case
+        out_list.append("}")  # end type switch
+
+        out_list.append("switch (msg_getHash(m, msgIndex)) {")
         cases = objects[obj_id]["args"]["cases"]
         for i, c in enumerate(cases):
             hv_hash = cls.get_hash_string(c)
             out_list.append(f"case {hv_hash}: {{ // \"{c}\"")
             out_list.extend(
                 cls._get_on_message_list(on_message_list[i], get_obj_class, objects))
             out_list.append("break;")
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlSystem.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlSystem.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlTabhead.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlTabhead.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlTabread.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlTabread.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlTabwrite.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlTabwrite.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlUnop.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlUnop.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ControlVar.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ControlVar.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/HeavyObject.py` & `hvcc-0.8.0/hvcc/generators/ir2c/HeavyObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/HeavyTable.py` & `hvcc-0.8.0/hvcc/generators/ir2c/HeavyTable.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/PrettyfyC.py` & `hvcc-0.8.0/hvcc/generators/ir2c/PrettyfyC.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalBiquad.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalBiquad.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalCPole.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalCPole.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalConvolution.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalConvolution.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalDel1.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalDel1.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalEnvelope.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalEnvelope.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalLine.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalLine.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalLorenz.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalLorenz.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalMath.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalMath.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalPhasor.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalPhasor.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalRPole.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalRPole.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalSamphold.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalSamphold.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalSample.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalSample.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalTabhead.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalTabhead.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalTabread.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalTabread.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from typing import Dict, List
 
 from .HeavyObject import HeavyObject
 
 
 class SignalTabread(HeavyObject):
-    """Handles __tabread~if, __tabread~f, __tabreadu~f
+    """Handles __tabread~if, __tabread~f, __tabreadu~f, __tabread_stoppable~f
     """
 
     c_struct = "SignalTabread"
     preamble = "sTabread"
 
     @classmethod
     def get_C_header_set(cls) -> set:
@@ -40,19 +40,19 @@
 
     @classmethod
     def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "sTabread_init(&sTabread_{0}, &hTable_{1}, {2});".format(
                 obj_id,
                 args["table_id"],
-                "true" if obj_type == "__tabread~f" else "false")]
+                "true" if obj_type in {"__tabread~f", "__tabread_stoppable~f"} else "false")]
 
     @classmethod
     def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
-        if obj_type in ["__tabread~f", "__tabreadu~f"]:
+        if obj_type in ["__tabread~f", "__tabreadu~f", "__tabread_stoppable~f"]:
             return [
                 "sTabread_onMessage(_c, &Context(_c)->sTabread_{0}, {1}, m, &sTabread_{0}_sendMessage);".format(
                     obj_id,
                     inlet_index)]
         else:  # "__tabread~if"
             return [f"sTabread_onMessage(_c, &Context(_c)->sTabread_{obj_id}, {inlet_index}, m, NULL);"]
 
@@ -67,14 +67,21 @@
                 )]
         elif obj_type == "__tabread~f":
             return [
                 "__hv_tabread_f(&sTabread_{0}, {1});".format(
                     process_dict["id"],
                     ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
                 )]
+        elif obj_type == "__tabread_stoppable~f":
+            return [
+                "__hv_tabread_stoppable_f(this, &sTabread_{0}, {1}, &{2}_{0}_sendMessage);".format(
+                    process_dict["id"],
+                    ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]]),
+                    cls.preamble
+                )]
         elif obj_type == "__tabreadu~f":
             return [
                 "__hv_tabreadu_f(&sTabread_{0}, {1});".format(
                     process_dict["id"],
                     ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
                 )]
         else:
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalTabwrite.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalTabwrite.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/SignalVar.py` & `hvcc-0.8.0/hvcc/generators/ir2c/SignalVar.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ir2c.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ir2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         "__env~f": SignalEnvelope,
         "__line~f": SignalLine,
         "__lorenz~f": SignalLorenz,
         "__del1~f": SignalDel1,
         "__tabread~if": SignalTabread,
         "__tabread~f": SignalTabread,
         "__tabreadu~f": SignalTabread,
+        "__tabread_stoppable~f": SignalTabread,
         "__tabhead~f": SignalTabhead,
         "__tabwrite~f": SignalTabwrite,
         "__tabwrite_stoppable~f": SignalTabwrite,
         "__phasor~f": SignalPhasor,
         "__phasor_k~f": SignalPhasor,
         "__sample~f": SignalSample,
         "__samphold~f": SignalSamphold,
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/ir2c_perf.py` & `hvcc-0.8.0/hvcc/generators/ir2c/ir2c_perf.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.cpp` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HeavyContext.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.hpp` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HeavyContext.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContextInterface.hpp` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HeavyContextInterface.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlBinop.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlBinop.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlCast.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlCast.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlDelay.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlDelay.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlIf.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlIf.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPack.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPack.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPrint.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlPrint.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlRandom.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlRandom.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSlice.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSlice.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSystem.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlSystem.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabhead.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabhead.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabread.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabread.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabwrite.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlTabwrite.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlUnop.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlUnop.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlVar.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvControlVar.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.cpp` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvHeavy.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #include "HeavyContext.hpp"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-#if !HV_WIN
+#if HV_APPLE
 #pragma mark - Heavy Table
 #endif
 
 HV_EXPORT bool hv_table_setLength(HeavyContextInterface *c, hv_uint32_t tableHash, hv_uint32_t newSampleLength) {
   hv_assert(c != nullptr);
   return c->setLengthForTable(tableHash, newSampleLength);
 }
@@ -37,15 +37,15 @@
 HV_EXPORT hv_uint32_t hv_table_getLength(HeavyContextInterface *c, hv_uint32_t tableHash) {
   hv_assert(c != nullptr);
   return c->getLengthForTable(tableHash);
 }
 
 
 
-#if !HV_WIN
+#if HV_APPLE
 #pragma mark - Heavy Message
 #endif
 
 HV_EXPORT hv_size_t hv_msg_getByteSize(hv_uint32_t numElements) {
   return msg_getCoreSize(numElements);
 }
 
@@ -119,15 +119,15 @@
 
 HV_EXPORT void hv_msg_free(HvMessage *m) {
   msg_free(m);
 }
 
 
 
-#if !HV_WIN
+#if HV_APPLE
 #pragma mark - Heavy Common
 #endif
 
 HV_EXPORT int hv_getSize(HeavyContextInterface *c) {
   hv_assert(c != nullptr);
   return (int) c->getSize();
 }
@@ -286,15 +286,15 @@
   hv_assert(c != nullptr);
   hv_assert(destinationHash != nullptr);
   hv_assert(outMsg != nullptr);
   return c->getNextSentMessage(destinationHash, outMsg, msgLength);
 }
 
 
-#if !HV_WIN
+#if HV_APPLE
 #pragma mark - Heavy Common
 #endif
 
 HV_EXPORT int hv_process(HeavyContextInterface *c, float **inputBuffers, float **outputBuffers, int n) {
   hv_assert(c != nullptr);
   return c->process(inputBuffers, outputBuffers, n);
 }
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvHeavy.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavyInternal.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvHeavyInternal.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvLightPipe.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvLightPipe.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMath.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMath.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessage.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessage.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessagePool.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessagePool.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessageQueue.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvMessageQueue.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalBiquad.c`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
  * PERFORMANCE OF THIS SOFTWARE.
  */
 
 #include "HvSignalBiquad.h"
 
 // http://reanimator-web.appspot.com/articles/simdiir
-// http://musicdsp.org/files/Audio-EQ-Cookbook.txt
+// https://webaudio.github.io/Audio-EQ-Cookbook/audio-eq-cookbook.html
 
 hv_size_t sBiquad_init(SignalBiquad *o) {
 #if HV_SIMD_AVX
   o->x = _mm256_setzero_ps();
 #elif HV_SIMD_SSE
   o->x = _mm_setzero_ps();
 #elif HV_SIMD_NEON
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalBiquad.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalCPole.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalCPole.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalConvolution.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalConvolution.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalDel1.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalDel1.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalEnvelope.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalEnvelope.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLine.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLine.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLorenz.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalLorenz.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalPhasor.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalPhasor.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalRPole.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalRPole.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSamphold.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSamphold.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSample.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalSample.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabwrite.c`

 * *Files 18% similar despite different names*

```diff
@@ -10,68 +10,45 @@
  * AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
  * INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
  * LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
  * OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
  * PERFORMANCE OF THIS SOFTWARE.
  */
 
-#include "HvSignalTabread.h"
+#include "HvSignalTabwrite.h"
 
-hv_size_t sTabread_init(SignalTabread *o, HvTable *table, bool forceAlignedLoads) {
+hv_size_t sTabwrite_init(SignalTabwrite *o, HvTable *table) {
   o->table = table;
   o->head = 0;
-  o->forceAlignedLoads = forceAlignedLoads;
   return 0;
 }
 
-void sTabread_onMessage(HeavyContextInterface *_c, SignalTabread *o, int letIn, const HvMessage *m,
+void sTabwrite_onMessage(HeavyContextInterface *_c, SignalTabwrite *o, int letIn, const HvMessage *m,
     void (*sendMessage)(HeavyContextInterface *, int, const HvMessage *)) {
   switch (letIn) {
-    case 0: {
-      if (o->table != NULL) {
-        switch (msg_getType(m,0)) {
-          case HV_MSG_BANG: o->head = 0; break;
-          case HV_MSG_FLOAT: {
-            hv_uint32_t h = (hv_uint32_t) hv_abs_f(msg_getFloat(m,0));
-            if (msg_getFloat(m,0) < 0.0f) {
-              // if input is negative, wrap around the end of the table
-              h = hTable_getSize(o->table) - h;
-            }
-            o->head = o->forceAlignedLoads ? (h & ~HV_N_SIMD_MASK) : h;
-
-            // output new head
-            HvMessage *n = HV_MESSAGE_ON_STACK(1);
-            msg_initWithFloat(n, msg_getTimestamp(m), (float) o->head);
-            sendMessage(_c, 1, n);
-            break;
+    // inlet 0 is the signal inlet
+    case 1: {
+      switch (msg_getType(m,0)) {
+        case HV_MSG_BANG: o->head = 0; break;
+        case HV_MSG_FLOAT: {
+          o->head = (msg_getFloat(m,0) >= 0.0f) ? (hv_uint32_t) msg_getFloat(m,0) : HV_TABWRITE_STOPPED;
+          break;
+        }
+        case HV_MSG_SYMBOL: {
+          if (msg_compareSymbol(m, 0, "stop")) {
+            o->head = HV_TABWRITE_STOPPED;
           }
-          default: break;
+          break;
         }
+        default: break;
       }
       break;
     }
-    case 1: {
+    case 2: {
       if (msg_isHashLike(m,0)) {
         o->table = hv_table_get(_c, msg_getHash(m,0));
       }
       break;
     }
     default: break;
   }
 }
-
-
-
-#if HV_APPLE
-#pragma mark - Tabhead
-#endif
-
-void sTabhead_onMessage(HeavyContextInterface *_c, SignalTabhead *o, const HvMessage *m) {
-  if (msg_isHashLike(m,0)) {
-    o->table = hv_table_get(_c, msg_getHash(m,0));
-  }
-}
-
-hv_size_t sTabhead_init(SignalTabhead *o, HvTable *table) {
-  o->table = table;
-  return 0;
-}
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabread.h`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 typedef struct SignalTabread {
   HvTable *table; // the table to read
   hv_uint32_t head;
+  hv_uint32_t end;
   bool forceAlignedLoads; // false by default, true if using __hv_tabread_f
+  bool playing; // false by default, only __hv_tabread_stoppable_f may respond to it
 } SignalTabread;
 
 // random access to a table
 hv_size_t sTabread_init(SignalTabread *o, HvTable *table, bool forceAlignedLoads);
 
 
 
@@ -39,38 +41,38 @@
 #endif
 
 static inline void __hv_tabread_if(SignalTabread *o, hv_bIni_t bIn, hv_bOutf_t bOut) {
   const float *const b = hTable_getBuffer(o->table);
 #if HV_SIMD_AVX
   const hv_int32_t *const i = (hv_int32_t *) &bIn;
 
-  hv_assert(i[0] >= 0 && i[0] < hTable_getAllocated(o->table));
-  hv_assert(i[1] >= 0 && i[1] < hTable_getAllocated(o->table));
-  hv_assert(i[2] >= 0 && i[2] < hTable_getAllocated(o->table));
-  hv_assert(i[3] >= 0 && i[3] < hTable_getAllocated(o->table));
-  hv_assert(i[4] >= 0 && i[4] < hTable_getAllocated(o->table));
-  hv_assert(i[5] >= 0 && i[5] < hTable_getAllocated(o->table));
-  hv_assert(i[6] >= 0 && i[6] < hTable_getAllocated(o->table));
-  hv_assert(i[7] >= 0 && i[7] < hTable_getAllocated(o->table));
+  hv_assert(i[0] >= 0 && (hv_uint32_t) i[0] < hTable_getAllocated(o->table));
+  hv_assert(i[1] >= 0 && (hv_uint32_t) i[1] < hTable_getAllocated(o->table));
+  hv_assert(i[2] >= 0 && (hv_uint32_t) i[2] < hTable_getAllocated(o->table));
+  hv_assert(i[3] >= 0 && (hv_uint32_t) i[3] < hTable_getAllocated(o->table));
+  hv_assert(i[4] >= 0 && (hv_uint32_t) i[4] < hTable_getAllocated(o->table));
+  hv_assert(i[5] >= 0 && (hv_uint32_t) i[5] < hTable_getAllocated(o->table));
+  hv_assert(i[6] >= 0 && (hv_uint32_t) i[6] < hTable_getAllocated(o->table));
+  hv_assert(i[7] >= 0 && (hv_uint32_t) i[7] < hTable_getAllocated(o->table));
 
   *bOut = _mm256_set_ps(b[i[7]], b[i[6]], b[i[5]], b[i[4]], b[i[3]], b[i[2]], b[i[1]], b[i[0]]);
 #elif HV_SIMD_SSE
   const hv_int32_t *const i = (hv_int32_t *) &bIn;
 
-  hv_assert(i[0] >= 0 && ((hv_uint32_t) i[0]) < hTable_getAllocated(o->table));
-  hv_assert(i[1] >= 0 && ((hv_uint32_t) i[1]) < hTable_getAllocated(o->table));
-  hv_assert(i[2] >= 0 && ((hv_uint32_t) i[2]) < hTable_getAllocated(o->table));
-  hv_assert(i[3] >= 0 && ((hv_uint32_t) i[3]) < hTable_getAllocated(o->table));
+  hv_assert(i[0] >= 0 && (hv_uint32_t) i[0] < hTable_getAllocated(o->table));
+  hv_assert(i[1] >= 0 && (hv_uint32_t) i[1] < hTable_getAllocated(o->table));
+  hv_assert(i[2] >= 0 && (hv_uint32_t) i[2] < hTable_getAllocated(o->table));
+  hv_assert(i[3] >= 0 && (hv_uint32_t) i[3] < hTable_getAllocated(o->table));
 
   *bOut = _mm_set_ps(b[i[3]], b[i[2]], b[i[1]], b[i[0]]);
 #elif HV_SIMD_NEON
-  hv_assert((bIn[0] >= 0) && (bIn[0] < hTable_getAllocated(o->table)));
-  hv_assert((bIn[1] >= 0) && (bIn[1] < hTable_getAllocated(o->table)));
-  hv_assert((bIn[2] >= 0) && (bIn[2] < hTable_getAllocated(o->table)));
-  hv_assert((bIn[3] >= 0) && (bIn[3] < hTable_getAllocated(o->table)));
+  hv_assert((bIn[0] >= 0) && (hv_uint32_t) bIn[0] < hTable_getAllocated(o->table));
+  hv_assert((bIn[1] >= 0) && (hv_uint32_t) bIn[1] < hTable_getAllocated(o->table));
+  hv_assert((bIn[2] >= 0) && (hv_uint32_t) bIn[2] < hTable_getAllocated(o->table));
+  hv_assert((bIn[3] >= 0) && (hv_uint32_t) bIn[3] < hTable_getAllocated(o->table));
 
   *bOut = (float32x4_t) {b[bIn[0]], b[bIn[1]], b[bIn[2]], b[bIn[3]]};
 #else // HV_SIMD_NONE
   hv_assert(bIn >= 0 && ((hv_uint32_t) bIn < hTable_getAllocated(o->table)));
 
   *bOut = b[bIn];
 #endif
@@ -111,44 +113,43 @@
 #else // HV_SIMD_NONE
   *bOut = *(hTable_getBuffer(o->table) + head);
 #endif
   o->head = head + HV_N_SIMD;
 }
 
 // this tabread can be instructed to stop. It is mainly intended for linear reads that only process a portion of a buffer.
-static inline void __hv_tabread_stoppable_f(SignalTabread *o, hv_bOutf_t bOut) {
-#if HV_SIMD_AVX
-  if (o->head == ~0x0) {
-    *bOut = _mm256_setzero_ps();
-  } else {
-    *bOut = _mm256_load_ps(hTable_getBuffer(o->table) + o->head);
-    o->head += HV_N_SIMD;
+static inline void __hv_tabread_stoppable_f(HeavyContextInterface *_c, SignalTabread *o, hv_bOutf_t bOut,
+  void (*sendMessage)(HeavyContextInterface *, int, const HvMessage *))
+{
+  hv_uint32_t head = o->head;
+  if (head >= hTable_getAllocated(o->table)) { // stop when we reach the table bounds
+    o->playing = false;
   }
-#elif HV_SIMD_SSE
-  if (o->head == ~0x0) {
-    *bOut = _mm_setzero_ps();
+  if (!o->playing) {
+    __hv_zero_f(bOut); // output silence when not playing
   } else {
-    *bOut = _mm_load_ps(hTable_getBuffer(o->table) + o->head);
-    o->head += HV_N_SIMD;
-  }
+    if (o->end > o->head) { // only play when end is further than play head
+#if HV_SIMD_AVX
+      *bOut = _mm256_loadu_ps(hTable_getBuffer(o->table) + head);
+#elif HV_SIMD_SSE
+      *bOut = _mm_load_ps(hTable_getBuffer(o->table) + head);
 #elif HV_SIMD_NEON
-  if (o->head == ~0x0) {
-    *bOut = vdupq_n_f32(0.0f);
-  } else {
-    *bOut = vld1q_f32(hTable_getBuffer(o->table) + o->head);
-    o->head += HV_N_SIMD;
-  }
+      *bOut = vld1q_f32(hTable_getBuffer(o->table) + head);
 #else // HV_SIMD_NONE
-  if (o->head == ~0x0) {
-    *bOut = 0.0f;
-  } else {
-    *bOut = *(hTable_getBuffer(o->table) + o->head);
-    o->head += HV_N_SIMD;
-  }
+      *bOut = *(hTable_getBuffer(o->table) + head);
 #endif
+      o->head = head + HV_N_SIMD;
+    } else {
+      o->playing = false;
+      __hv_zero_f(bOut); // output silence when not playing
+      HvMessage *n = HV_MESSAGE_ON_STACK(1);
+      msg_initWithBang(n, 0);
+      sendMessage(_c, 2, n);
+    }
+  }
 }
 
 void sTabread_onMessage(HeavyContextInterface *_c, SignalTabread *o, int letIn, const HvMessage *m,
     void (*sendMessage)(HeavyContextInterface *, int, const HvMessage *));
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalTabwrite.h`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
   *(hTable_getBuffer(o->table) + head) = bIn;
 #endif
   head += HV_N_SIMD;
   o->head = head; // update local write head
   hTable_setHead(o->table, head); // update remote write head
 }
 
-// this tabread can be instructed to stop. It is mainly intended for linear reads that only process a portion of a buffer.
+// this tabwrite can be instructed to stop. It is mainly intended for linear reads that only process a portion of a buffer.
 // Stores are unaligned, which can be slow but allows any indicies to be written to.
 // TODO(mhroth): this is not stopping!
 static inline void __hv_tabwrite_stoppable_f(SignalTabwrite *o, hv_bInf_t bIn) {
   if (o->head != HV_TABWRITE_STOPPED) {
 #if HV_SIMD_AVX
     _mm256_storeu_ps(hTable_getBuffer(o->table) + o->head, bIn);
 #elif HV_SIMD_SSE
```

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalVar.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvSignalVar.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvTable.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvTable.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvUtils.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/HvUtils.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.c` & `hvcc-0.8.0/hvcc/generators/ir2c/static/cpuid.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.h` & `hvcc-0.8.0/hvcc/generators/ir2c/static/cpuid.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.cpp` & `hvcc-0.8.0/hvcc/generators/ir2c/templates/Heavy_NAME.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.h` & `hvcc-0.8.0/hvcc/generators/ir2c/templates/Heavy_NAME.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.hpp` & `hvcc-0.8.0/hvcc/generators/ir2c/templates/Heavy_NAME.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.sln` & `hvcc-0.8.0/hvcc/generators/vs2015/Heavy/Heavy.sln`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj` & `hvcc-0.8.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters` & `hvcc-0.8.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/main.c` & `hvcc-0.8.0/hvcc/generators/vs2015/Heavy/main.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy/main.c` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy/main.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/main.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/main.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Info.plist` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.h` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/ViewController.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/ViewController.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/main.m` & `hvcc-0.8.0/hvcc/generators/xcode/Heavy_iOS/main.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/Connection.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/Connection.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyGraph.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/HeavyGraph.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/HeavyObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/HvSwitchcase.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/HvSwitchcase.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/NotificationEnum.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/NotificationEnum.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdAudioIoObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdAudioIoObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdBinopObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdBinopObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdGraph.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdGraph.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLetObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdLetObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLibSignalGraph.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdLibSignalGraph.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdMessageObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdMessageObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdPackObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdPackObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdParser.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdParser.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRaw.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdRaw.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdReceiveObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdReceiveObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRouteObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdRouteObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSelectObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdSelectObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSendObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdSendObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTableObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdTableObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTriggerObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdTriggerObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdUnpackObject.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/PdUnpackObject.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bendin.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bendin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bp~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/bp~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/change.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/change.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cos~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/cos~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/czero~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delay.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delay.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delread~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ftom.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/ftom.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hip~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/hip~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/int.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/int.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/line.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/line.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/lop~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/lop~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/makenote.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/makenote.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/metro.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/metro.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/noise~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/noise~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/notein.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/notein.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/osc~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/osc~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/poly.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/poly.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/random.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/random.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/swap.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/swap.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabread.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/timer.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/timer.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/touchin.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/touchin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/until.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/until.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vd~.pd` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/libs/pd/vd~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/interpreters/pd2hv/pd2hv.py` & `hvcc-0.8.0/hvcc/interpreters/pd2hv/pd2hv.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc/utils.py` & `hvcc-0.8.0/hvcc/utils.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.7.0/hvcc.egg-info/PKG-INFO` & `hvcc-0.8.0/hvcc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hvcc
-Version: 0.7.0
+Version: 0.8.0
 Summary: `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 Home-page: https://github.com/Wasted-Audio/hvcc
-Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.7.0.tar.gz
+Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.8.0.tar.gz
 Author: Enzien Audio, Wasted Audio
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Compilers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hvcc-0.7.0/hvcc.egg-info/SOURCES.txt` & `hvcc-0.8.0/hvcc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,24 +74,14 @@
 hvcc/generators/c2dpf/templates/HeavyDPF.hpp
 hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp
 hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp
 hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp
 hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp
 hvcc/generators/c2dpf/templates/Makefile_plugin
 hvcc/generators/c2dpf/templates/Makefile_project
-hvcc/generators/c2fabric/__init__.py
-hvcc/generators/c2fabric/c2fabric.py
-hvcc/generators/c2fabric/templates/android/jni/Android.mk
-hvcc/generators/c2fabric/templates/android/jni/Application.mk
-hvcc/generators/c2fabric/templates/linux/Makefile
-hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs
-hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs
-hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln
-hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj
-hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/project.pbxproj
 hvcc/generators/c2js/README.md
 hvcc/generators/c2js/__init__.py
 hvcc/generators/c2js/c2js.py
 hvcc/generators/c2js/template/hv_worklet.js
 hvcc/generators/c2js/template/hv_worklet_start.js
 hvcc/generators/c2js/template/hv_wrapper.js
 hvcc/generators/c2js/template/index.html
@@ -99,17 +89,18 @@
 hvcc/generators/c2owl/c2owl.py
 hvcc/generators/c2owl/deps/HvMessage.c
 hvcc/generators/c2owl/deps/HvUtils.h
 hvcc/generators/c2owl/templates/HeavyOwl.hpp
 hvcc/generators/c2owl/templates/HeavyOwlConstants.h
 hvcc/generators/c2pdext/__init__.py
 hvcc/generators/c2pdext/c2pdext.py
+hvcc/generators/c2pdext/static/Makefile.pdlibbuilder
 hvcc/generators/c2pdext/static/m_pd.h
+hvcc/generators/c2pdext/templates/Makefile
 hvcc/generators/c2pdext/templates/pd_external.c
-hvcc/generators/c2pdext/templates/project.pbxproj
 hvcc/generators/c2unity/__init__.py
 hvcc/generators/c2unity/c2unity.py
 hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h
 hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp
 hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h
 hvcc/generators/c2unity/static/xcode/Info.plist
 hvcc/generators/c2unity/templates/android/jni/Android.mk
@@ -425,14 +416,15 @@
 hvcc/interpreters/pd2hv/libs/pd/polytouchout.pd
 hvcc/interpreters/pd2hv/libs/pd/powtodb.pd
 hvcc/interpreters/pd2hv/libs/pd/powtodb~.pd
 hvcc/interpreters/pd2hv/libs/pd/print.pd
 hvcc/interpreters/pd2hv/libs/pd/q8_rsqrt~.pd
 hvcc/interpreters/pd2hv/libs/pd/q8_sqrt~.pd
 hvcc/interpreters/pd2hv/libs/pd/random.pd
+hvcc/interpreters/pd2hv/libs/pd/rffttest~.pd
 hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd
 hvcc/interpreters/pd2hv/libs/pd/rmstodb~.pd
 hvcc/interpreters/pd2hv/libs/pd/rpole~.pd
 hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd
 hvcc/interpreters/pd2hv/libs/pd/rzero_rev~.pd
 hvcc/interpreters/pd2hv/libs/pd/rzero~.pd
 hvcc/interpreters/pd2hv/libs/pd/samphold~.pd
```

### Comparing `hvcc-0.7.0/setup.cfg` & `hvcc-0.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = hvcc
-version = 0.7.0
+version = 0.8.0
 license = GPLv3
 author = Enzien Audio, Wasted Audio
 description = `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 url = https://github.com/Wasted-Audio/hvcc
-download_url = https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.7.0.tar.gz
+download_url = https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.8.0.tar.gz
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Topic :: Software Development :: Compilers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

