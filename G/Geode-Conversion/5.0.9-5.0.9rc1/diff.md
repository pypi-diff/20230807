# Comparing `tmp/Geode_Conversion-5.0.9-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.0.9rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1213301 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-06 00:59 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      178 b- defN 23-Jul-06 00:59 geode_conversion/model.py
--rw-rw-rw-  2.0 fat  2415616 b- defN 23-Jul-06 01:00 geode_conversion/bin/Geode-Conversion_model.dll
--rw-rw-rw-  2.0 fat   150528 b- defN 23-Jul-06 01:00 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2001 b- defN 23-Jul-06 01:00 Geode_Conversion-5.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-06 01:00 Geode_Conversion-5.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-06 01:00 Geode_Conversion-5.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-Jul-06 01:00 Geode_Conversion-5.0.9.dist-info/RECORD
-8 files, 2569342 bytes uncompressed, 1212013 bytes compressed:  52.8%
+Zip file size: 1213331 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-04 14:33 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Jul-04 14:33 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  2415616 b- defN 23-Jul-04 14:34 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   150528 b- defN 23-Jul-04 14:34 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2007 b- defN 23-Jul-04 14:34 Geode_Conversion-5.0.9rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-04 14:34 Geode_Conversion-5.0.9rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-04 14:34 Geode_Conversion-5.0.9rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      743 b- defN 23-Jul-04 14:34 Geode_Conversion-5.0.9rc1.dist-info/RECORD
+8 files, 2569360 bytes uncompressed, 1212019 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
 Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.0.9.dist-info/METADATA
+Filename: Geode_Conversion-5.0.9rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.0.9.dist-info/WHEEL
+Filename: Geode_Conversion-5.0.9rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.0.9.dist-info/top_level.txt
+Filename: Geode_Conversion-5.0.9rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.0.9.dist-info/RECORD
+Filename: Geode_Conversion-5.0.9rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/bin/Geode-Conversion_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001801a17a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Jul  6 01:00:25 2023
+Time/Date		Tue Jul  4 14:34:28 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000001a6000
 SizeOfInitializedData	00000000000a7800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000001a17a8
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00254000
 SizeOfHeaders		00000400
-CheckSum		0025c029
+CheckSum		00256b82
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -376,33 +376,33 @@
 	22ffc0	 2073  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
 	230406	 1881  ?set_polyhedron_adjacent@?$SolidMeshBuilder@$02@geode@@QEAAXAEBUPolyhedronFacet@2@I@Z
 
  0022b394	0022bb80 00000000 00000000 00233266 001a7590
 
 	DLL Name: OpenGeode_geometry.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	233218	  536  ?colocated_index_mapping@?$NNSearch@$01@geode@@QEBA?AUColocatedInfo@12@N@Z
-	2331f4	  334  ??1?$NNSearch@$01@geode@@QEAA@XZ
-	233186	  203  ??0?$NNSearch@$01@geode@@QEAA@V?$vector@V?$Point@$01@geode@@V?$allocator@V?$Point@$01@geode@@@std@@@std@@@Z
-	233138	  537  ?colocated_index_mapping@?$NNSearch@$02@geode@@QEBA?AUColocatedInfo@12@N@Z
-	233114	  335  ??1?$NNSearch@$02@geode@@QEAA@XZ
-	2330a6	  205  ??0?$NNSearch@$02@geode@@QEAA@V?$vector@V?$Point@$02@geode@@V?$allocator@V?$Point@$02@geode@@@std@@@std@@@Z
-	233066	  584  ?intersects@?$BoundingBox@$02@geode@@QEBA_NAEBV?$Ray@$02@2@@Z
-	233030	  605  ?mapping_morton@Impl@?$AABBTree@$02@geode@@QEBAII@Z
-	232fec	  623  ?node@Impl@?$AABBTree@$02@geode@@QEBAAEBV?$BoundingBox@$02@3@I@Z
-	232f9e	  570  ?get_recursive_iterators@Impl@?$AABBTree@$02@geode@@SA?AUIterator@123@III@Z
-	232f6e	  591  ?is_leaf@Impl@?$AABBTree@$02@geode@@SA_NII@Z
-	232f22	  201  ??0?$InfiniteLine@$02@geode@@QEAA@AEBV?$Vector@$02@1@AEBV?$Point@$02@1@@Z
-	232ef6	  615  ?nb_bboxes@?$AABBTree@$02@geode@@QEBAIXZ
-	232ed2	  330  ??1?$AABBTree@$02@geode@@QEAA@XZ
-	232ea6	   79  ??0?$AABBTree@$02@geode@@QEAA@$$QEAV01@@Z
-	232e62	  265  ??0?$Ray@$02@geode@@QEAA@AEBV?$Vector@$02@1@AEBV?$Point@$02@1@@Z
-	232dee	  560  ?direction@?$GenericLine@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$Vector@$02@2@XZ
-	232db2	  723  ?tetrahedron_signed_volume@geode@@YANAEBVTetrahedron@1@@Z
-	232d7c	  327  ??0Tetrahedron@geode@@QEAA@AEBV?$Point@$02@1@000@Z
+	233218	  534  ?colocated_index_mapping@?$NNSearch@$01@geode@@QEBA?AUColocatedInfo@12@N@Z
+	2331f4	  332  ??1?$NNSearch@$01@geode@@QEAA@XZ
+	233186	  201  ??0?$NNSearch@$01@geode@@QEAA@V?$vector@V?$Point@$01@geode@@V?$allocator@V?$Point@$01@geode@@@std@@@std@@@Z
+	233138	  535  ?colocated_index_mapping@?$NNSearch@$02@geode@@QEBA?AUColocatedInfo@12@N@Z
+	233114	  333  ??1?$NNSearch@$02@geode@@QEAA@XZ
+	2330a6	  203  ??0?$NNSearch@$02@geode@@QEAA@V?$vector@V?$Point@$02@geode@@V?$allocator@V?$Point@$02@geode@@@std@@@std@@@Z
+	233066	  582  ?intersects@?$BoundingBox@$02@geode@@QEBA_NAEBV?$Ray@$02@2@@Z
+	233030	  603  ?mapping_morton@Impl@?$AABBTree@$02@geode@@QEBAII@Z
+	232fec	  621  ?node@Impl@?$AABBTree@$02@geode@@QEBAAEBV?$BoundingBox@$02@3@I@Z
+	232f9e	  568  ?get_recursive_iterators@Impl@?$AABBTree@$02@geode@@SA?AUIterator@123@III@Z
+	232f6e	  589  ?is_leaf@Impl@?$AABBTree@$02@geode@@SA_NII@Z
+	232f22	  199  ??0?$InfiniteLine@$02@geode@@QEAA@AEBV?$Vector@$02@1@AEBV?$Point@$02@1@@Z
+	232ef6	  613  ?nb_bboxes@?$AABBTree@$02@geode@@QEBAIXZ
+	232ed2	  328  ??1?$AABBTree@$02@geode@@QEAA@XZ
+	232ea6	   77  ??0?$AABBTree@$02@geode@@QEAA@$$QEAV01@@Z
+	232e62	  263  ??0?$Ray@$02@geode@@QEAA@AEBV?$Vector@$02@1@AEBV?$Point@$02@1@@Z
+	232dee	  558  ?direction@?$GenericLine@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$Vector@$02@2@XZ
+	232db2	  721  ?tetrahedron_signed_volume@geode@@YANAEBVTetrahedron@1@@Z
+	232d7c	  325  ??0Tetrahedron@geode@@QEAA@AEBV?$Point@$02@1@000@Z
 
  0022b3a8	0022bab8 00000000 00000000 00233896 001a74c8
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	233834	  153  ?log_error@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
 	2337fe	  157  ?name@Identifier@geode@@QEBA?AVstring_view@absl@@XZ
@@ -46113,89 +46113,89 @@
 	  b8b0: 24 53 6f 6c 69 64 45 64 67 65 73 40 24 30 32 40
 	  b8c0: 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f
 	  b8d0: 24 61 72 72 61 79 40 49 24 30 31 40 73 74 64 40
 	  b8e0: 40 49 40 5a 00 00 6a 06 3f 6e 62 5f 65 64 67 65
 	  b8f0: 73 40 3f 24 53 75 72 66 61 63 65 45 64 67 65 73
 	  b900: 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42 41
 	  b910: 49 58 5a 00 4f 70 65 6e 47 65 6f 64 65 5f 6d 65
-	  b920: 73 68 2e 64 6c 6c 00 00 47 01 3f 3f 30 54 65 74
+	  b920: 73 68 2e 64 6c 6c 00 00 45 01 3f 3f 30 54 65 74
 	  b930: 72 61 68 65 64 72 6f 6e 40 67 65 6f 64 65 40 40
 	  b940: 51 45 41 41 40 41 45 42 56 3f 24 50 6f 69 6e 74
-	  b950: 40 24 30 32 40 31 40 30 30 30 40 5a 00 00 d3 02
+	  b950: 40 24 30 32 40 31 40 30 30 30 40 5a 00 00 d1 02
 	  b960: 3f 74 65 74 72 61 68 65 64 72 6f 6e 5f 73 69 67
 	  b970: 6e 65 64 5f 76 6f 6c 75 6d 65 40 67 65 6f 64 65
 	  b980: 40 40 59 41 4e 41 45 42 56 54 65 74 72 61 68 65
-	  b990: 64 72 6f 6e 40 31 40 40 5a 00 30 02 3f 64 69 72
+	  b990: 64 72 6f 6e 40 31 40 40 5a 00 2e 02 3f 64 69 72
 	  b9a0: 65 63 74 69 6f 6e 40 3f 24 47 65 6e 65 72 69 63
 	  b9b0: 4c 69 6e 65 40 56 3f 24 72 65 66 65 72 65 6e 63
 	  b9c0: 65 5f 77 72 61 70 70 65 72 40 24 24 43 42 56 3f
 	  b9d0: 24 50 6f 69 6e 74 40 24 30 32 40 67 65 6f 64 65
 	  b9e0: 40 40 40 73 74 64 40 40 24 30 32 40 67 65 6f 64
 	  b9f0: 65 40 40 51 45 42 41 41 45 42 56 3f 24 56 65 63
-	  ba00: 74 6f 72 40 24 30 32 40 32 40 58 5a 00 00 09 01
+	  ba00: 74 6f 72 40 24 30 32 40 32 40 58 5a 00 00 07 01
 	  ba10: 3f 3f 30 3f 24 52 61 79 40 24 30 32 40 67 65 6f
 	  ba20: 64 65 40 40 51 45 41 41 40 41 45 42 56 3f 24 56
 	  ba30: 65 63 74 6f 72 40 24 30 32 40 31 40 41 45 42 56
 	  ba40: 3f 24 50 6f 69 6e 74 40 24 30 32 40 31 40 40 5a
-	  ba50: 00 00 4f 00 3f 3f 30 3f 24 41 41 42 42 54 72 65
+	  ba50: 00 00 4d 00 3f 3f 30 3f 24 41 41 42 42 54 72 65
 	  ba60: 65 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 41
-	  ba70: 41 40 24 24 51 45 41 56 30 31 40 40 5a 00 4a 01
+	  ba70: 41 40 24 24 51 45 41 56 30 31 40 40 5a 00 48 01
 	  ba80: 3f 3f 31 3f 24 41 41 42 42 54 72 65 65 40 24 30
 	  ba90: 32 40 67 65 6f 64 65 40 40 51 45 41 41 40 58 5a
-	  baa0: 00 00 67 02 3f 6e 62 5f 62 62 6f 78 65 73 40 3f
+	  baa0: 00 00 65 02 3f 6e 62 5f 62 62 6f 78 65 73 40 3f
 	  bab0: 24 41 41 42 42 54 72 65 65 40 24 30 32 40 67 65
-	  bac0: 6f 64 65 40 40 51 45 42 41 49 58 5a 00 00 c9 00
+	  bac0: 6f 64 65 40 40 51 45 42 41 49 58 5a 00 00 c7 00
 	  bad0: 3f 3f 30 3f 24 49 6e 66 69 6e 69 74 65 4c 69 6e
 	  bae0: 65 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 41
 	  baf0: 41 40 41 45 42 56 3f 24 56 65 63 74 6f 72 40 24
 	  bb00: 30 32 40 31 40 41 45 42 56 3f 24 50 6f 69 6e 74
-	  bb10: 40 24 30 32 40 31 40 40 5a 00 4f 02 3f 69 73 5f
+	  bb10: 40 24 30 32 40 31 40 40 5a 00 4d 02 3f 69 73 5f
 	  bb20: 6c 65 61 66 40 49 6d 70 6c 40 3f 24 41 41 42 42
 	  bb30: 54 72 65 65 40 24 30 32 40 67 65 6f 64 65 40 40
-	  bb40: 53 41 5f 4e 49 49 40 5a 00 00 3a 02 3f 67 65 74
+	  bb40: 53 41 5f 4e 49 49 40 5a 00 00 38 02 3f 67 65 74
 	  bb50: 5f 72 65 63 75 72 73 69 76 65 5f 69 74 65 72 61
 	  bb60: 74 6f 72 73 40 49 6d 70 6c 40 3f 24 41 41 42 42
 	  bb70: 54 72 65 65 40 24 30 32 40 67 65 6f 64 65 40 40
 	  bb80: 53 41 3f 41 55 49 74 65 72 61 74 6f 72 40 31 32
-	  bb90: 33 40 49 49 49 40 5a 00 6f 02 3f 6e 6f 64 65 40
+	  bb90: 33 40 49 49 49 40 5a 00 6d 02 3f 6e 6f 64 65 40
 	  bba0: 49 6d 70 6c 40 3f 24 41 41 42 42 54 72 65 65 40
 	  bbb0: 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 41
 	  bbc0: 45 42 56 3f 24 42 6f 75 6e 64 69 6e 67 42 6f 78
-	  bbd0: 40 24 30 32 40 33 40 49 40 5a 00 00 5d 02 3f 6d
+	  bbd0: 40 24 30 32 40 33 40 49 40 5a 00 00 5b 02 3f 6d
 	  bbe0: 61 70 70 69 6e 67 5f 6d 6f 72 74 6f 6e 40 49 6d
 	  bbf0: 70 6c 40 3f 24 41 41 42 42 54 72 65 65 40 24 30
 	  bc00: 32 40 67 65 6f 64 65 40 40 51 45 42 41 49 49 40
-	  bc10: 5a 00 48 02 3f 69 6e 74 65 72 73 65 63 74 73 40
+	  bc10: 5a 00 46 02 3f 69 6e 74 65 72 73 65 63 74 73 40
 	  bc20: 3f 24 42 6f 75 6e 64 69 6e 67 42 6f 78 40 24 30
 	  bc30: 32 40 67 65 6f 64 65 40 40 51 45 42 41 5f 4e 41
 	  bc40: 45 42 56 3f 24 52 61 79 40 24 30 32 40 32 40 40
-	  bc50: 5a 00 cd 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
+	  bc50: 5a 00 cb 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
 	  bc60: 68 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 41
 	  bc70: 41 40 56 3f 24 76 65 63 74 6f 72 40 56 3f 24 50
 	  bc80: 6f 69 6e 74 40 24 30 32 40 67 65 6f 64 65 40 40
 	  bc90: 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 56 3f 24
 	  bca0: 50 6f 69 6e 74 40 24 30 32 40 67 65 6f 64 65 40
 	  bcb0: 40 40 73 74 64 40 40 40 73 74 64 40 40 40 5a 00
-	  bcc0: 4f 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
+	  bcc0: 4d 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
 	  bcd0: 24 30 32 40 67 65 6f 64 65 40 40 51 45 41 41 40
-	  bce0: 58 5a 00 00 19 02 3f 63 6f 6c 6f 63 61 74 65 64
+	  bce0: 58 5a 00 00 17 02 3f 63 6f 6c 6f 63 61 74 65 64
 	  bcf0: 5f 69 6e 64 65 78 5f 6d 61 70 70 69 6e 67 40 3f
 	  bd00: 24 4e 4e 53 65 61 72 63 68 40 24 30 32 40 67 65
 	  bd10: 6f 64 65 40 40 51 45 42 41 3f 41 55 43 6f 6c 6f
 	  bd20: 63 61 74 65 64 49 6e 66 6f 40 31 32 40 4e 40 5a
-	  bd30: 00 00 cb 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
+	  bd30: 00 00 c9 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
 	  bd40: 68 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 41
 	  bd50: 41 40 56 3f 24 76 65 63 74 6f 72 40 56 3f 24 50
 	  bd60: 6f 69 6e 74 40 24 30 31 40 67 65 6f 64 65 40 40
 	  bd70: 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 56 3f 24
 	  bd80: 50 6f 69 6e 74 40 24 30 31 40 67 65 6f 64 65 40
 	  bd90: 40 40 73 74 64 40 40 40 73 74 64 40 40 40 5a 00
-	  bda0: 4e 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
+	  bda0: 4c 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
 	  bdb0: 24 30 31 40 67 65 6f 64 65 40 40 51 45 41 41 40
-	  bdc0: 58 5a 00 00 18 02 3f 63 6f 6c 6f 63 61 74 65 64
+	  bdc0: 58 5a 00 00 16 02 3f 63 6f 6c 6f 63 61 74 65 64
 	  bdd0: 5f 69 6e 64 65 78 5f 6d 61 70 70 69 6e 67 40 3f
 	  bde0: 24 4e 4e 53 65 61 72 63 68 40 24 30 31 40 67 65
 	  bdf0: 6f 64 65 40 40 51 45 42 41 3f 41 55 43 6f 6c 6f
 	  be00: 63 61 74 65 64 49 6e 66 6f 40 31 32 40 4e 40 5a
 	  be10: 00 00 4f 70 65 6e 47 65 6f 64 65 5f 67 65 6f 6d
 	  be20: 65 74 72 79 2e 64 6c 6c 00 00 39 00 3f 3f 31 53
 	  be30: 69 6e 67 6c 65 74 6f 6e 40 67 65 6f 64 65 40 40
@@ -709403,17 +709403,16 @@
    18020fa37:	add    %ah,0x61(%rdx)
    18020fa3a:	and    %ah,%fs:0x6c(%rcx)
    18020fa3e:	insb   (%dx),%es:(%rdi)
    18020fa3f:	outsl  %ds:(%rsi),(%dx)
    18020fa40:	movsxd 0x74(%rcx),%esp
    18020fa43:	imul   $0x0,0x6e(%rdi),%ebp
    18020fa4a:	add    %al,(%rax)
-   18020fa4c:	sub    %edx,(%rdx)
-   18020fa4e:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   18020fa4f:	add    %al,%fs:(%rax)
+   18020fa4c:	hlt
+   18020fa4d:	sub    $0x64a4,%eax
    18020fa52:	add    %al,(%rax)
    18020fa54:	or     $0x60000000,%eax
    18020fa59:	add    (%rax),%eax
    18020fa5b:	add    %bh,(%rax)
    18020fa5d:	es and %eax,(%rax)
    18020fa60:	cmp    %bl,(%rdx)
    18020fa62:	and    %eax,(%rax)
@@ -767750,15 +767749,15 @@
    180232d6d:	outsl  %gs:(%rsi),(%dx)
    180232d6f:	fs gs pop %rdi
    180232d72:	insl   (%dx),%es:(%rdi)
    180232d73:	gs jae 0x180232dde
    180232d76:	cs fs insb (%dx),%es:(%rdi)
    180232d79:	insb   (%dx),%es:(%rdi)
    180232d7a:	add    %al,(%rax)
-   180232d7c:	rex.RXB add %r15d,(%r15)
+   180232d7c:	add    %r15d,(%r15)
    180232d7f:	(bad)
    180232d80:	xor    %dl,0x74(%rbp,%riz,2)
    180232d84:	jb     0x180232de7
    180232d86:	push   $0x6f726465
    180232d8b:	outsb  %ds:(%rsi),(%dx)
    180232d8c:	rex
    180232d8d:	outsl  %gs:(%esi),(%dx)
@@ -767775,15 +767774,15 @@
    180232d9e:	and    $0x50,%al
    180232da0:	outsl  %ds:(%rsi),(%dx)
    180232da1:	imul   $0x32302440,0x74(%rsi),%ebp
    180232da8:	rex xor %eax,0x30(%rax)
    180232dac:	xor    %dh,(%rax)
    180232dae:	rex pop %rdx
    180232db0:	add    %al,(%rax)
-   180232db2:	roll   %cl,(%rdx)
+   180232db2:	roll   (%rdx)
    180232db4:	(bad)
    180232db5:	je     0x180232e1c
    180232db7:	je     0x180232e2b
    180232db9:	(bad)
    180232dba:	push   $0x6f726465
    180232dbf:	outsb  %ds:(%rsi),(%dx)
    180232dc0:	pop    %rdi
@@ -767805,15 +767804,15 @@
    180232ddd:	push   %rsp
    180232dde:	gs je  0x180232e53
    180232de1:	(bad)
    180232de2:	push   $0x6f726465
    180232de7:	outsb  %ds:(%rsi),(%dx)
    180232de8:	rex xor %eax,0x40(%rax)
    180232dec:	pop    %rdx
-   180232ded:	add    %dh,(%rax)
+   180232ded:	add    %ch,(%rsi)
    180232def:	add    (%rdi),%bh
    180232df1:	imul   $0x6f697463,%fs:0x65(%rdx),%esi
    180232df9:	outsb  %ds:(%rsi),(%dx)
    180232dfa:	rex (bad)
    180232dfc:	and    $0x47,%al
    180232dfe:	outsb  %gs:(%rsi),(%dx)
    180232e00:	gs jb  0x180232e6c
@@ -767856,16 +767855,16 @@
    180232e50:	and    $0x56,%al
    180232e52:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
    180232e57:	rex and $0x30,%al
    180232e5a:	xor    0x32(%rax),%al
    180232e5d:	rex pop %rax
    180232e5f:	pop    %rdx
    180232e60:	add    %al,(%rax)
-   180232e62:	or     %eax,(%rcx)
-   180232e64:	(bad)
+   180232e62:	(bad)
+   180232e63:	add    %edi,(%rdi)
    180232e65:	(bad)
    180232e66:	xor    %bh,(%rdi)
    180232e68:	and    $0x52,%al
    180232e6a:	(bad)
    180232e6b:	jns    0x180232ead
    180232e6d:	and    $0x30,%al
    180232e6f:	xor    0x67(%rax),%al
@@ -767891,15 +767890,15 @@
    180232e94:	(bad)
    180232e95:	and    $0x50,%al
    180232e97:	outsl  %ds:(%rsi),(%dx)
    180232e98:	imul   $0x32302440,0x74(%rsi),%ebp
    180232e9f:	rex xor %eax,0x40(%rax)
    180232ea3:	pop    %rdx
    180232ea4:	add    %al,(%rax)
-   180232ea6:	rex.WRXB add %r15b,(%r15)
+   180232ea6:	rex.WRB add %r15b,(%r15)
    180232ea9:	(bad)
    180232eaa:	xor    %bh,(%rdi)
    180232eac:	and    $0x41,%al
    180232eae:	rex.B
    180232eaf:	rex.X
    180232eb0:	rex.X push %rsp
    180232eb2:	jb     0x180232f19
@@ -767914,15 +767913,15 @@
    180232ec5:	rex and $0x24,%al
    180232ec8:	push   %rcx
    180232ec9:	rex.RB
    180232eca:	push   %r14
    180232ecc:	xor    %dh,(%rcx)
    180232ece:	rex
    180232ecf:	rex pop %rdx
-   180232ed1:	add    %cl,0x1(%rdx)
+   180232ed1:	add    %cl,0x1(%rax)
    180232ed4:	(bad)
    180232ed5:	(bad)
    180232ed6:	xor    %edi,(%rdi)
    180232ed8:	and    $0x41,%al
    180232eda:	rex.B
    180232edb:	rex.X
    180232edc:	rex.X push %rsp
@@ -767934,15 +767933,15 @@
    180232eec:	rex push %rcx
    180232eee:	rex.RB
    180232eef:	rex.B
    180232ef0:	rex.B
    180232ef1:	rex pop %rax
    180232ef3:	pop    %rdx
    180232ef4:	add    %al,(%rax)
-   180232ef6:	add    (%edi),%bh
+   180232ef6:	add    %gs:(%rdi),%bh
    180232ef9:	outsb  %ds:(%rsi),(%dx)
    180232efa:	(bad)
    180232efb:	pop    %rdi
    180232efc:	(bad)
    180232f01:	jae    0x180232f43
    180232f03:	(bad)
    180232f04:	and    $0x41,%al
@@ -767957,18 +767956,15 @@
    180232f18:	rex push %rcx
    180232f1a:	rex.RB
    180232f1b:	rex.X
    180232f1c:	rex.B
    180232f1d:	rex.WB pop %r8
    180232f1f:	pop    %rdx
    180232f20:	add    %al,(%rax)
-   180232f22:	leave
-   180232f23:	add    %bh,(%rdi)
-   180232f25:	(bad)
-   180232f26:	xor    %bh,(%rdi)
+   180232f22:	movl   $0x3f303f3f,(%rax)
    180232f28:	and    $0x49,%al
    180232f2a:	outsb  %ds:(%rsi),(%dx)
    180232f2b:	imul   $0x6574,0x69(%rsi),%bp
    180232f31:	imul   $0x32302440,0x65(%rsi),%r13
    180232f39:	rex
    180232f3a:	outsl  %gs:(%esi),(%dx)
    180232f3d:	fs gs rex
@@ -767991,15 +767987,15 @@
    180232f5b:	rex.X push %rsi
    180232f5d:	(bad)
    180232f5e:	and    $0x50,%al
    180232f60:	outsl  %ds:(%rsi),(%dx)
    180232f61:	imul   $0x32302440,0x74(%rsi),%ebp
    180232f68:	rex xor %eax,0x40(%rax)
    180232f6c:	pop    %rdx
-   180232f6d:	add    %cl,0x2(%rdi)
+   180232f6d:	add    %cl,0x2(%rbp)
    180232f70:	(bad)
    180232f71:	imul   $0x6661656c,0x5f(%rbx),%esi
    180232f78:	rex
    180232f79:	rex.WB insl (%dx),%es:(%rdi)
    180232f7b:	jo     0x180232fe9
    180232f7d:	rex (bad)
    180232f7f:	and    $0x41,%al
@@ -768014,15 +768010,15 @@
    180232f93:	rex push %rbx
    180232f95:	pop    %r15
    180232f97:	rex.WRX
    180232f98:	rex.WB
    180232f99:	rex.WB
    180232f9a:	rex pop %rdx
    180232f9c:	add    %al,(%rax)
-   180232f9e:	cmp    (%rdx),%al
+   180232f9e:	cmp    %al,(%rdx)
    180232fa0:	(bad)
    180232fa1:	addr32 gs je 0x180233004
    180232fa5:	jb     0x18023300c
    180232fa7:	movsxd 0x72(%rbp),%esi
    180232faa:	jae    0x180233015
    180232fac:	jbe    0x180233013
    180232fae:	pop    %rdi
@@ -768048,15 +768044,15 @@
    180232fde:	je     0x18023304f
    180232fe0:	jb     0x180233022
    180232fe2:	xor    %esi,(%rdx)
    180232fe4:	xor    0x49(%rax),%eax
    180232fe7:	rex.WB
    180232fe8:	rex.WB
    180232fe9:	rex pop %rdx
-   180232feb:	add    %ch,0x2(%rdi)
+   180232feb:	add    %ch,0x2(%rbp)
    180232fee:	(bad)
    180232fef:	outsb  %ds:(%rsi),(%dx)
    180232ff0:	outsl  %ds:(%rsi),(%dx)
    180232ff1:	fs gs rex
    180232ff4:	rex.WB insl (%dx),%es:(%rdi)
    180232ff6:	jo     0x180233064
    180232ff8:	rex (bad)
@@ -768083,15 +768079,15 @@
    18023301d:	imul   $0x40786f42,%fs:0x67(%rsi),%ebp
    180233025:	and    $0x30,%al
    180233027:	xor    0x33(%rax),%al
    18023302a:	rex
    18023302b:	rex.WB
    18023302c:	rex pop %rdx
    18023302e:	add    %al,(%rax)
-   180233030:	pop    %rbp
+   180233030:	pop    %rbx
    180233031:	add    (%rdi),%bh
    180233033:	insl   (%dx),%es:(%rdi)
    180233034:	(bad)
    180233035:	jo     0x1802330a7
    180233037:	imul   $0x726f6d5f,0x67(%rsi),%ebp
    18023303e:	je     0x1802330af
    180233040:	outsb  %ds:(%rsi),(%dx)
@@ -768111,15 +768107,15 @@
    18023305c:	rex push %rcx
    18023305e:	rex.RB
    18023305f:	rex.X
    180233060:	rex.B
    180233061:	rex.WB
    180233062:	rex.WB
    180233063:	rex pop %rdx
-   180233065:	add    %cl,0x2(%rax)
+   180233065:	add    %al,0x2(%rsi)
    180233068:	(bad)
    180233069:	imul   $0x65737265,0x74(%rsi),%ebp
    180233070:	movsxd 0x40(%rbx,%rsi,2),%esi
    180233074:	(bad)
    180233075:	and    $0x42,%al
    180233077:	outsl  %ds:(%rsi),(%dx)
    180233078:	jne    0x1802330e8
@@ -768140,15 +768136,15 @@
    180233098:	and    $0x52,%al
    18023309a:	(bad)
    18023309b:	jns    0x1802330dd
    18023309d:	and    $0x30,%al
    18023309f:	xor    0x32(%rax),%al
    1802330a2:	rex
    1802330a3:	rex pop %rdx
-   1802330a5:	add    %cl,%ch
+   1802330a5:	add    %cl,%bl
    1802330a7:	add    %bh,(%rdi)
    1802330a9:	(bad)
    1802330aa:	xor    %bh,(%rdi)
    1802330ac:	and    $0x4e,%al
    1802330ae:	rex.WRX push %rbx
    1802330b0:	gs (bad)
    1802330b2:	jb     0x180233117
@@ -768193,15 +768189,15 @@
    180233105:	rex jae 0x18023317c
    180233108:	fs rex
    18023310a:	rex
    18023310b:	rex jae 0x180233182
    18023310e:	fs rex
    180233110:	rex
    180233111:	rex pop %rdx
-   180233113:	add    %cl,0x1(%rdi)
+   180233113:	add    %cl,0x1(%rbp)
    180233116:	(bad)
    180233117:	(bad)
    180233118:	xor    %edi,(%rdi)
    18023311a:	and    $0x4e,%al
    18023311c:	rex.WRX push %rbx
    18023311e:	gs (bad)
    180233120:	jb     0x180233185
@@ -768212,16 +768208,16 @@
    18023312e:	rex push %rcx
    180233130:	rex.RB
    180233131:	rex.B
    180233132:	rex.B
    180233133:	rex pop %rax
    180233135:	pop    %rdx
    180233136:	add    %al,(%rax)
-   180233138:	sbb    %eax,(%rdx)
-   18023313a:	(bad)
+   180233138:	(bad)
+   180233139:	add    (%rdi),%bh
    18023313b:	movsxd 0x6c(%rdi),%ebp
    18023313e:	outsl  %ds:(%rsi),(%dx)
    18023313f:	movsxd 0x74(%rcx),%esp
    180233142:	gs fs pop %rdi
    180233145:	imul   $0x6d5f7865,0x64(%rsi),%ebp
    18023314c:	(bad)
    18023314d:	jo     0x1802331bf
@@ -768245,15 +768241,15 @@
    180233177:	gs rex.WB outsb %fs:(%rsi),(%dx)
    18023317b:	outsw  %ds:(%rsi),(%dx)
    18023317d:	rex xor %esi,(%rdx)
    180233180:	rex
    180233181:	rex.WRX
    180233182:	rex pop %rdx
    180233184:	add    %al,(%rax)
-   180233186:	lret
+   180233186:	leave
    180233187:	add    %bh,(%rdi)
    180233189:	(bad)
    18023318a:	xor    %bh,(%rdi)
    18023318c:	and    $0x4e,%al
    18023318e:	rex.WRX push %rbx
    180233190:	gs (bad)
    180233192:	jb     0x1802331f7
@@ -768298,16 +768294,15 @@
    1802331e5:	rex jae 0x18023325c
    1802331e8:	fs rex
    1802331ea:	rex
    1802331eb:	rex jae 0x180233262
    1802331ee:	fs rex
    1802331f0:	rex
    1802331f1:	rex pop %rdx
-   1802331f3:	add    %cl,0x1(%rsi)
-   1802331f6:	(bad)
+   1802331f3:	add    %cl,0x3f(%rcx,%rax,1)
    1802331f7:	(bad)
    1802331f8:	xor    %edi,(%rdi)
    1802331fa:	and    $0x4e,%al
    1802331fc:	rex.WRX push %rbx
    1802331fe:	gs (bad)
    180233200:	jb     0x180233265
    180233202:	push   $0x31302440
@@ -768317,16 +768312,16 @@
    18023320e:	rex push %rcx
    180233210:	rex.RB
    180233211:	rex.B
    180233212:	rex.B
    180233213:	rex pop %rax
    180233215:	pop    %rdx
    180233216:	add    %al,(%rax)
-   180233218:	sbb    %al,(%rdx)
-   18023321a:	(bad)
+   180233218:	(bad)
+   180233219:	add    (%rdi),%bh
    18023321b:	movsxd 0x6c(%rdi),%ebp
    18023321e:	outsl  %ds:(%rsi),(%dx)
    18023321f:	movsxd 0x74(%rcx),%esp
    180233222:	gs fs pop %rdi
    180233225:	imul   $0x6d5f7865,0x64(%rsi),%ebp
    18023322c:	(bad)
    18023322d:	jo     0x18023329f
@@ -776299,28 +776294,24 @@
    180238777:	imul   $0x24406873,0x65(%rbp,%rcx,2),%esp
    18023877f:	xor    %dh,(%rdx)
    180238781:	rex
    180238782:	outsl  %gs:(%esi),(%dx)
    180238785:	fs gs rex
    180238788:	rex
    180238789:	rex (bad)
-   18023878b:	xor    %dil,0x66(%r8)
-   18023878f:	cmp    %dh,%gs:(%rdi)
-   180238792:	movsxd (%rax),%edi
-   180238794:	(bad)
-   180238795:	fs rex
-   180238797:	rex add %al,(%rax)
-   18023879a:	add    %al,(%rax)
-   18023879c:	add    %al,(%rax)
-   18023879e:	add    %al,(%rax)
-   1802387a0:	push   $0x18020f9
-	...
-   1802387ad:	add    %al,(%rax)
-   1802387af:	add    %ch,(%rsi)
-   1802387b1:	(bad)
+   18023878b:	xor    %dil,0x38(%r8)
+   18023878f:	cmp    %ah,%fs:0x31(%rdi,%rsi,1)
+   180238794:	xor    $0x404066,%eax
+   180238799:	add    %al,(%rax)
+   18023879b:	add    %al,(%rax)
+   18023879d:	add    %al,(%rax)
+   18023879f:	add    %ch,-0x7(%rax)
+   1802387a2:	and    %al,0x1(%rax)
+	...
+   1802387b0:	cs (bad)
    1802387b2:	push   %r14
    1802387b4:	rex.WB insl (%dx),%es:(%rdi)
    1802387b6:	jo     0x180238824
    1802387b8:	rex (bad)
    1802387ba:	and    $0x53,%al
    1802387bc:	jne    0x180238830
    1802387be:	data16 (bad)
@@ -776354,27 +776345,23 @@
    18023880c:	gs jae 0x180238877
    18023880f:	rex and $0x30,%al
    180238812:	xor    %eax,0x67(%rax)
    180238815:	outsl  %gs:(%rsi),(%dx)
    180238817:	fs gs rex
    18023881a:	rex
    18023881b:	rex (bad)
-   18023881d:	xor    %dil,0x66(%r8)
-   180238821:	cmp    %dh,%gs:(%rdi)
-   180238824:	movsxd (%rax),%edi
-   180238826:	(bad)
-   180238827:	fs rex
-   180238829:	rex add %al,(%rax)
-   18023882c:	add    %al,(%rax)
-   18023882e:	add    %al,(%rax)
-   180238830:	push   $0x18020f9
-	...
-   18023883d:	add    %al,(%rax)
-   18023883f:	add    %ch,(%rsi)
-   180238841:	(bad)
+   18023881d:	xor    %dil,0x38(%r8)
+   180238821:	cmp    %ah,%fs:0x31(%rdi,%rsi,1)
+   180238826:	xor    $0x404066,%eax
+   18023882b:	add    %al,(%rax)
+   18023882d:	add    %al,(%rax)
+   18023882f:	add    %ch,-0x7(%rax)
+   180238832:	and    %al,0x1(%rax)
+	...
+   180238840:	cs (bad)
    180238842:	push   %r14
    180238844:	rex.WB insl (%dx),%es:(%rdi)
    180238846:	jo     0x1802388b4
    180238848:	rex (bad)
    18023884a:	and    $0x53,%al
    18023884c:	jne    0x1802388c0
    18023884e:	data16 (bad)
@@ -776408,27 +776395,23 @@
    18023889c:	gs jae 0x180238907
    18023889f:	rex and $0x30,%al
    1802388a2:	xor    0x67(%rax),%al
    1802388a5:	outsl  %gs:(%rsi),(%dx)
    1802388a7:	fs gs rex
    1802388aa:	rex
    1802388ab:	rex (bad)
-   1802388ad:	xor    %dil,0x66(%r8)
-   1802388b1:	cmp    %dh,%gs:(%rdi)
-   1802388b4:	movsxd (%rax),%edi
-   1802388b6:	(bad)
-   1802388b7:	fs rex
-   1802388b9:	rex add %al,(%rax)
-   1802388bc:	add    %al,(%rax)
-   1802388be:	add    %al,(%rax)
-   1802388c0:	push   $0x18020f9
-	...
-   1802388cd:	add    %al,(%rax)
-   1802388cf:	add    %ch,(%rsi)
-   1802388d1:	(bad)
+   1802388ad:	xor    %dil,0x38(%r8)
+   1802388b1:	cmp    %ah,%fs:0x31(%rdi,%rsi,1)
+   1802388b6:	xor    $0x404066,%eax
+   1802388bb:	add    %al,(%rax)
+   1802388bd:	add    %al,(%rax)
+   1802388bf:	add    %ch,-0x7(%rax)
+   1802388c2:	and    %al,0x1(%rax)
+	...
+   1802388d0:	cs (bad)
    1802388d2:	push   %r14
    1802388d4:	pop    %rdi
    1802388d5:	push   %rdx
    1802388d6:	gs pop %di
    1802388d9:	movsxd 0x75(%rdi),%ebp
    1802388dc:	outsb  %ds:(%rsi),(%dx)
    1802388dd:	je     0x18023893e
```

## Comparing `Geode_Conversion-5.0.9.dist-info/METADATA` & `Geode_Conversion-5.0.9rc1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Geode-Conversion
-Version: 5.0.9
+Version: 5.0.9rc1
 Summary: Conversion module for Geode-solutions OpenGeode modules
 Home-page: https://github.com/Geode-solutions/Geode-Conversion
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.4.0)
+Requires-Dist: opengeode-core (==14.*,>=14.4.0rc5)
 
 <h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Conversion OpenGeode module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.9 Summary: Conversion
-module for Geode-solutions OpenGeode modules Home-page: https://github.com/
-Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.4.0)
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.9rc1 Summary:
+Conversion module for Geode-solutions OpenGeode modules Home-page: https://
+github.com/Geode-solutions/Geode-Conversion Author: Geode-solutions Author-
+email: contact@geode-solutions.com License: Proprietary Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+(==14.*,>=14.4.0rc5)
                ****** Geode-Conversionby Geode-solutions ******
                      **** Conversion OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Conversion-5.0.9.dist-info/RECORD` & `Geode_Conversion-5.0.9rc1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 geode_conversion/__init__.py,sha256=Ia-ZwhIAokDIC6uBDumiY-s6IwjLi8gNTQti1qPYKh4,171
 geode_conversion/model.py,sha256=w4pnyFhioSDpM5WfYbW6h0wyzZSYYvZewwttq1oMEy4,178
-geode_conversion/bin/Geode-Conversion_model.dll,sha256=nrCLt8I6uNgyahHEENWcdKzDJMZFsrYfrMsjPMg39NA,2415616
-geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=TXLVZ3Svv2vd1jBuLaonC6-xPh0u1wmuoEkURUnQCWw,150528
-Geode_Conversion-5.0.9.dist-info/METADATA,sha256=Oa6BJSki0lqOwDAa7k9dLfT6iuAdpGzfEsZKo260RAs,2001
-Geode_Conversion-5.0.9.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Conversion-5.0.9.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
-Geode_Conversion-5.0.9.dist-info/RECORD,,
+geode_conversion/bin/Geode-Conversion_model.dll,sha256=OReqoicDkkt-gyBnuk1TJ7oVMoHwOTYv_9kqoEJlMV0,2415616
+geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=jAzFxScsdo33Q_CUeINGBzqYBx1Zz0hGaqKh0KJ0GD0,150528
+Geode_Conversion-5.0.9rc1.dist-info/METADATA,sha256=hCUSaCqs5sdtGbMjbFSAyMG5gtdH6uEGX-WpH8RRug8,2007
+Geode_Conversion-5.0.9rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Conversion-5.0.9rc1.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
+Geode_Conversion-5.0.9rc1.dist-info/RECORD,,
```

