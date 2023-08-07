# Comparing `tmp/scilightcon-0.2.0.tar.gz` & `tmp/scilightcon-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilightcon-0.2.0.tar", last modified: Mon Aug  7 07:19:52 2023, max compression
+gzip compressed data, was "scilightcon-0.2.0.post1.tar", last modified: Mon Aug  7 07:28:43 2023, max compression
```

## Comparing `scilightcon-0.2.0.tar` & `scilightcon-0.2.0.post1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.583548 scilightcon-0.2.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     1073 2023-08-07 07:18:38.000000 scilightcon-0.2.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      355 2023-08-07 07:18:38.000000 scilightcon-0.2.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      805 2023-08-07 07:19:52.579548 scilightcon-0.2.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      270 2023-08-07 07:18:38.000000 scilightcon-0.2.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.555548 scilightcon-0.2.0/scilightcon/
--rw-r--r--   0 vsts      (1001) docker     (123)      211 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.559548 scilightcon-0.2.0/scilightcon/control/
--rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/control/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.559548 scilightcon-0.2.0/scilightcon/datasets/
--rw-r--r--   0 vsts      (1001) docker     (123)      557 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8841 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/_base.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7516 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/_logs_reader.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.563548 scilightcon-0.2.0/scilightcon/datasets/data/
--rw-r--r--   0 vsts      (1001) docker     (123)     1685 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/Ar_lines.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.567548 scilightcon-0.2.0/scilightcon/datasets/data/EO/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46206 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    49586 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    50284 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    39791 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    52825 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    57433 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    57324 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    58434 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    40227 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    48209 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    44452 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    48918 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv
--rw-r--r--   0 vsts      (1001) docker     (123)      385 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/Hg_lines.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   320206 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s
--rw-r--r--   0 vsts      (1001) docker     (123)     9279 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/White_LED_spectrum.csv
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)  1040787 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/atmosphere.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     1042 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/data_test_detect_peaks.csv
--rw-r--r--   0 vsts      (1001) docker     (123)      531 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/data_test_detect_peaks.csv.gz
--rw-r--r--   0 vsts      (1001) docker     (123)     1042 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   596451 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/logsreader_test.zip
--rw-r--r--   0 vsts      (1001) docker     (123)     7053 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    10678 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     6663 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/reflection_EKSMA_Ag.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     6485 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/reflection_EKSMA_Al.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     7022 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/reflection_EKSMA_Au.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   229421 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/test_beam_profile.pkl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    53154 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    53084 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    52943 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    54475 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    22273 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    24603 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    22273 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    22304 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    22303 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56664 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56615 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56563 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56513 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56467 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56416 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56377 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56368 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56416 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56282 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56301 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56307 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56381 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56307 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55966 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56010 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56059 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56028 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55955 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55829 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55911 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55799 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55700 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129739 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129672 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129557 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129478 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129231 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56457 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56447 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56396 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56369 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56361 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56303 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56294 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56267 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56187 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56159 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56144 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    56084 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129490 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129560 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129593 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129727 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   129769 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     7443 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    11204 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    11270 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    11036 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     7377 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     7397 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     7527 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    55366 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    54473 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   105252 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5742 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5742 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5742 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5529 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5501 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5501 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     5501 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    75410 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    75272 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    74840 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    74216 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    73546 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    73503 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    73485 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    73746 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv
--rw-r--r--   0 vsts      (1001) docker     (123)  1212522 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/datasets/data/toolbox_materials.pkl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/fitting/
--rw-r--r--   0 vsts      (1001) docker     (123)      206 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/fitting/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3235 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/fitting/_detect_peaks.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8406 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/fitting/_fitting_2d_beam_profiles.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/imaging/
--rw-r--r--   0 vsts      (1001) docker     (123)       64 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/imaging/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/optics/
--rw-r--r--   0 vsts      (1001) docker     (123)    32475 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/optics/_GVD_and_TOD_calculator.py
--rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/optics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11775 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/optics/_materials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1038 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/optics/_spectra.py
--rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/optics/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/plot/
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/plot/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/signals/
--rw-r--r--   0 vsts      (1001) docker     (123)       63 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/signals/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.579548 scilightcon-0.2.0/scilightcon/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)      342 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4160 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/utils/_analyze_s2_data.py
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (123)      819 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/utils/_fixes.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-07 07:18:38.000000 scilightcon-0.2.0/scilightcon/utils/_interpolate_and_multiply.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:19:52.555548 scilightcon-0.2.0/scilightcon.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      805 2023-08-07 07:19:52.000000 scilightcon-0.2.0/scilightcon.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     8028 2023-08-07 07:19:52.000000 scilightcon-0.2.0/scilightcon.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-07 07:19:52.000000 scilightcon-0.2.0/scilightcon.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-07 07:19:52.000000 scilightcon-0.2.0/scilightcon.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-08-07 07:19:52.000000 scilightcon-0.2.0/scilightcon.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-07 07:19:52.583548 scilightcon-0.2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-08-07 07:18:38.000000 scilightcon-0.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.586630 scilightcon-0.2.0.post1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1073 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      355 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     1175 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      638 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.562629 scilightcon-0.2.0.post1/scilightcon/
+-rw-r--r--   0 vsts      (1001) docker     (123)      213 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.562629 scilightcon-0.2.0.post1/scilightcon/control/
+-rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/control/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.562629 scilightcon-0.2.0.post1/scilightcon/datasets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      557 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8841 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/_base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7516 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/_logs_reader.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.566629 scilightcon-0.2.0.post1/scilightcon/datasets/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1685 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/Ar_lines.csv
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.570629 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    46206 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    49586 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    50284 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    39791 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    52825 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    57433 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    57324 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    58434 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    40227 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    48209 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    44452 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    48918 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)      385 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/Hg_lines.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   320206 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s
+-rw-r--r--   0 vsts      (1001) docker     (123)     9279 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/White_LED_spectrum.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  1040787 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/atmosphere.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     1042 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/data_test_detect_peaks.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)      531 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/data_test_detect_peaks.csv.gz
+-rw-r--r--   0 vsts      (1001) docker     (123)     1042 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   596451 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/logsreader_test.zip
+-rw-r--r--   0 vsts      (1001) docker     (123)     7053 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    10678 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     6663 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EKSMA_Ag.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     6485 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EKSMA_Al.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     7022 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EKSMA_Au.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   229421 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/test_beam_profile.pkl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    53154 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    53084 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    52943 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    54475 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    22273 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    24603 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    22273 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    22304 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    22303 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56664 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56615 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56563 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56513 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56467 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56416 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56377 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56368 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56416 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56282 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56301 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56307 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56381 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56307 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55966 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56010 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56059 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56028 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55955 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55829 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55911 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55799 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55700 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129739 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129672 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129557 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129478 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129231 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56457 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56447 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56396 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56369 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56361 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56303 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56294 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56267 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56187 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56159 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56144 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    56084 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129490 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129560 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129593 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129727 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   129769 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     7443 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    11204 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    11270 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    11036 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     7377 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     7397 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     7527 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    55366 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    54473 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   105252 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5742 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5742 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5742 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5529 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5501 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5501 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     5501 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    75410 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    75272 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    74840 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    74216 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    73546 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    73503 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    73485 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    73746 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)  1212522 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/datasets/data/toolbox_materials.pkl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/fitting/
+-rw-r--r--   0 vsts      (1001) docker     (123)      206 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/fitting/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3235 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/fitting/_detect_peaks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8406 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/fitting/_fitting_2d_beam_profiles.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/imaging/
+-rw-r--r--   0 vsts      (1001) docker     (123)       64 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/imaging/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/optics/
+-rw-r--r--   0 vsts      (1001) docker     (123)    32475 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/optics/_GVD_and_TOD_calculator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/optics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11775 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/optics/_materials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1038 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/optics/_spectra.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/optics/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/plot/
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/plot/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/signals/
+-rw-r--r--   0 vsts      (1001) docker     (123)       63 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/signals/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.582630 scilightcon-0.2.0.post1/scilightcon/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)      342 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4160 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/utils/_analyze_s2_data.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      819 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/utils/_fixes.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/scilightcon/utils/_interpolate_and_multiply.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 07:28:43.562629 scilightcon-0.2.0.post1/scilightcon.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1175 2023-08-07 07:28:43.000000 scilightcon-0.2.0.post1/scilightcon.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     8028 2023-08-07 07:28:43.000000 scilightcon-0.2.0.post1/scilightcon.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-07 07:28:43.000000 scilightcon-0.2.0.post1/scilightcon.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-07 07:28:43.000000 scilightcon-0.2.0.post1/scilightcon.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-08-07 07:28:43.000000 scilightcon-0.2.0.post1/scilightcon.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-07 07:28:43.586630 scilightcon-0.2.0.post1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-08-07 07:27:36.000000 scilightcon-0.2.0.post1/setup.py
```

### Comparing `scilightcon-0.2.0/LICENSE` & `scilightcon-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/PKG-INFO` & `scilightcon-0.2.0.post1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilightcon
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: A lightcon scipack
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/scilightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,13 @@
 License-File: LICENSE
 
 # Welcome
 
 Read documentation at `doc\site\index.html`
 
 [![Build Status](https://dev.azure.com/LCURS/Shared/_apis/build/status%2Flight-conversion-public.scilightcon?branchName=main)](https://dev.azure.com/LCURS/Shared/_build/latest?definitionId=98&branchName=main)
+
+[![PyPI version scilightcon](https://badge.fury.io/py/ansicolortags.svg)](https://pypi.python.org/pypi/scilightcon/)
+
+[![PyPI version scilightcon](https://img.shields.io/pypi/v/ansicolortags.svg)](https://pypi.python.org/pypi/scilightcon/)
+
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/scilightcon/)
```

### Comparing `scilightcon-0.2.0/scilightcon/datasets/__init__.py` & `scilightcon-0.2.0.post1/scilightcon/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/_base.py` & `scilightcon-0.2.0.post1/scilightcon/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/_logs_reader.py` & `scilightcon-0.2.0.post1/scilightcon/datasets/_logs_reader.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/Ar_lines.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/Ar_lines.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/White_LED_spectrum.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/White_LED_spectrum.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/atmosphere.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/atmosphere.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/data_test_detect_peaks.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/data_test_detect_peaks.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/data_test_detect_peaks.csv.gz` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/data_test_detect_peaks.csv.gz`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/logsreader_test.zip` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/logsreader_test.zip`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/reflection_EKSMA_Ag.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EKSMA_Ag.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/reflection_EKSMA_Al.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EKSMA_Al.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/reflection_EKSMA_Au.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/reflection_EKSMA_Au.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/test_beam_profile.pkl` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/test_beam_profile.pkl`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/datasets/data/toolbox_materials.pkl` & `scilightcon-0.2.0.post1/scilightcon/datasets/data/toolbox_materials.pkl`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/fitting/_detect_peaks.py` & `scilightcon-0.2.0.post1/scilightcon/fitting/_detect_peaks.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/fitting/_fitting_2d_beam_profiles.py` & `scilightcon-0.2.0.post1/scilightcon/fitting/_fitting_2d_beam_profiles.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/optics/_GVD_and_TOD_calculator.py` & `scilightcon-0.2.0.post1/scilightcon/optics/_GVD_and_TOD_calculator.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/optics/_materials.py` & `scilightcon-0.2.0.post1/scilightcon/optics/_materials.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/optics/_spectra.py` & `scilightcon-0.2.0.post1/scilightcon/optics/_spectra.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/utils/_analyze_s2_data.py` & `scilightcon-0.2.0.post1/scilightcon/utils/_analyze_s2_data.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/utils/_fixes.py` & `scilightcon-0.2.0.post1/scilightcon/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon/utils/_interpolate_and_multiply.py` & `scilightcon-0.2.0.post1/scilightcon/utils/_interpolate_and_multiply.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/scilightcon.egg-info/PKG-INFO` & `scilightcon-0.2.0.post1/scilightcon.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilightcon
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: A lightcon scipack
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/scilightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,13 @@
 License-File: LICENSE
 
 # Welcome
 
 Read documentation at `doc\site\index.html`
 
 [![Build Status](https://dev.azure.com/LCURS/Shared/_apis/build/status%2Flight-conversion-public.scilightcon?branchName=main)](https://dev.azure.com/LCURS/Shared/_build/latest?definitionId=98&branchName=main)
+
+[![PyPI version scilightcon](https://badge.fury.io/py/ansicolortags.svg)](https://pypi.python.org/pypi/scilightcon/)
+
+[![PyPI version scilightcon](https://img.shields.io/pypi/v/ansicolortags.svg)](https://pypi.python.org/pypi/scilightcon/)
+
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/ansicolortags.svg)](https://pypi.python.org/pypi/scilightcon/)
```

### Comparing `scilightcon-0.2.0/scilightcon.egg-info/SOURCES.txt` & `scilightcon-0.2.0.post1/scilightcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0/setup.py` & `scilightcon-0.2.0.post1/setup.py`

 * *Files identical despite different names*

