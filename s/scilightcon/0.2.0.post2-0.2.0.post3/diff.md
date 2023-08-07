# Comparing `tmp/scilightcon-0.2.0.post2.tar.gz` & `tmp/scilightcon-0.2.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilightcon-0.2.0.post2.tar", last modified: Mon Aug  7 07:44:15 2023, max compression
+gzip compressed data, was "scilightcon-0.2.0.post3.tar", last modified: Mon Aug  7 09:17:25 2023, max compression
```

## Comparing `scilightcon-0.2.0.post2.tar` & `scilightcon-0.2.0.post3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/
--rw-rw-rw-   0        0        0     1094 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/LICENSE
--rw-rw-rw-   0        0        0      368 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/MANIFEST.in
--rw-rw-rw-   0        0        0     1201 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.760517 scilightcon-0.2.0.post2/scilightcon/
--rw-rw-rw-   0        0        0      227 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.760517 scilightcon-0.2.0.post2/scilightcon/control/
--rw-rw-rw-   0        0        0       69 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.776143 scilightcon-0.2.0.post2/scilightcon/datasets/
--rw-rw-rw-   0        0        0      574 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/__init__.py
--rw-rw-rw-   0        0        0     9072 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/_base.py
--rw-rw-rw-   0        0        0     7685 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/_logs_reader.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.776143 scilightcon-0.2.0.post2/scilightcon/datasets/data/
--rw-rw-rw-   0        0        0     1685 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/Ar_lines.csv
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.791767 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/
--rw-rw-rw-   0        0        0        0 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/__init__.py
--rw-rw-rw-   0        0        0    46206 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv
--rw-rw-rw-   0        0        0    49586 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv
--rw-rw-rw-   0        0        0    50284 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv
--rw-rw-rw-   0        0        0    39791 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv
--rw-rw-rw-   0        0        0    52825 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv
--rw-rw-rw-   0        0        0    57433 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv
--rw-rw-rw-   0        0        0    57324 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv
--rw-rw-rw-   0        0        0    58434 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv
--rw-rw-rw-   0        0        0    40227 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv
--rw-rw-rw-   0        0        0    48209 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv
--rw-rw-rw-   0        0        0    44452 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv
--rw-rw-rw-   0        0        0    48918 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv
--rw-rw-rw-   0        0        0      385 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/Hg_lines.csv
--rw-rw-rw-   0        0        0   320206 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s
--rw-rw-rw-   0        0        0     9518 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/White_LED_spectrum.csv
--rw-rw-rw-   0        0        0        0 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/__init__.py
--rw-rw-rw-   0        0        0  1061194 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/atmosphere.csv
--rw-rw-rw-   0        0        0     1042 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/data_test_detect_peaks.csv
--rw-rw-rw-   0        0        0      531 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/data_test_detect_peaks.csv.gz
--rw-rw-rw-   0        0        0     1042 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv
--rw-rw-rw-   0        0        0   596451 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/logsreader_test.zip
--rw-rw-rw-   0        0        0     7053 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv
--rw-rw-rw-   0        0        0    10678 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv
--rw-rw-rw-   0        0        0     6663 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EKSMA_Ag.csv
--rw-rw-rw-   0        0        0     6485 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EKSMA_Al.csv
--rw-rw-rw-   0        0        0     7022 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EKSMA_Au.csv
--rw-rw-rw-   0        0        0   229421 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/test_beam_profile.pkl
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/
--rw-rw-rw-   0        0        0        0 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/__init__.py
--rw-rw-rw-   0        0        0    53154 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv
--rw-rw-rw-   0        0        0    53084 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv
--rw-rw-rw-   0        0        0    52943 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv
--rw-rw-rw-   0        0        0    54475 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv
--rw-rw-rw-   0        0        0    22273 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv
--rw-rw-rw-   0        0        0    24603 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv
--rw-rw-rw-   0        0        0    22273 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv
--rw-rw-rw-   0        0        0    22304 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv
--rw-rw-rw-   0        0        0    22303 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv
--rw-rw-rw-   0        0        0    56664 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv
--rw-rw-rw-   0        0        0    56615 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv
--rw-rw-rw-   0        0        0    56563 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv
--rw-rw-rw-   0        0        0    56513 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv
--rw-rw-rw-   0        0        0    56467 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv
--rw-rw-rw-   0        0        0    56416 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv
--rw-rw-rw-   0        0        0    56377 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv
--rw-rw-rw-   0        0        0    56368 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv
--rw-rw-rw-   0        0        0    56416 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv
--rw-rw-rw-   0        0        0    56282 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv
--rw-rw-rw-   0        0        0    56301 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv
--rw-rw-rw-   0        0        0    56307 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv
--rw-rw-rw-   0        0        0    56381 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv
--rw-rw-rw-   0        0        0    56307 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv
--rw-rw-rw-   0        0        0    55966 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv
--rw-rw-rw-   0        0        0    56010 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv
--rw-rw-rw-   0        0        0    56059 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv
--rw-rw-rw-   0        0        0    56028 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv
--rw-rw-rw-   0        0        0    55955 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv
--rw-rw-rw-   0        0        0    55829 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv
--rw-rw-rw-   0        0        0    55911 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv
--rw-rw-rw-   0        0        0    55799 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv
--rw-rw-rw-   0        0        0    55700 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv
--rw-rw-rw-   0        0        0   129739 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv
--rw-rw-rw-   0        0        0   129672 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv
--rw-rw-rw-   0        0        0   129557 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv
--rw-rw-rw-   0        0        0   129478 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv
--rw-rw-rw-   0        0        0   129231 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv
--rw-rw-rw-   0        0        0    56457 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv
--rw-rw-rw-   0        0        0    56447 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv
--rw-rw-rw-   0        0        0    56396 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv
--rw-rw-rw-   0        0        0    56369 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv
--rw-rw-rw-   0        0        0    56361 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv
--rw-rw-rw-   0        0        0    56303 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv
--rw-rw-rw-   0        0        0    56294 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv
--rw-rw-rw-   0        0        0    56267 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv
--rw-rw-rw-   0        0        0    56187 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv
--rw-rw-rw-   0        0        0    56159 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv
--rw-rw-rw-   0        0        0    56144 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv
--rw-rw-rw-   0        0        0    56084 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv
--rw-rw-rw-   0        0        0   129490 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv
--rw-rw-rw-   0        0        0   129560 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv
--rw-rw-rw-   0        0        0   129593 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv
--rw-rw-rw-   0        0        0   129727 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv
--rw-rw-rw-   0        0        0   129769 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv
--rw-rw-rw-   0        0        0     7443 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv
--rw-rw-rw-   0        0        0    11204 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv
--rw-rw-rw-   0        0        0    11270 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv
--rw-rw-rw-   0        0        0    11036 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv
--rw-rw-rw-   0        0        0     7377 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv
--rw-rw-rw-   0        0        0     7397 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv
--rw-rw-rw-   0        0        0     7527 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv
--rw-rw-rw-   0        0        0    55366 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv
--rw-rw-rw-   0        0        0    54473 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv
--rw-rw-rw-   0        0        0   105252 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv
--rw-rw-rw-   0        0        0     5742 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv
--rw-rw-rw-   0        0        0     5742 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv
--rw-rw-rw-   0        0        0     5742 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv
--rw-rw-rw-   0        0        0     5529 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv
--rw-rw-rw-   0        0        0     5501 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv
--rw-rw-rw-   0        0        0     5501 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv
--rw-rw-rw-   0        0        0     5501 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv
--rw-rw-rw-   0        0        0    75410 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv
--rw-rw-rw-   0        0        0    75272 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv
--rw-rw-rw-   0        0        0    74840 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv
--rw-rw-rw-   0        0        0    74216 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv
--rw-rw-rw-   0        0        0    73546 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv
--rw-rw-rw-   0        0        0    73503 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv
--rw-rw-rw-   0        0        0    73485 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv
--rw-rw-rw-   0        0        0    73746 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv
--rw-rw-rw-   0        0        0  1212522 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/datasets/data/toolbox_materials.pkl
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/fitting/
--rw-rw-rw-   0        0        0      214 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/fitting/__init__.py
--rw-rw-rw-   0        0        0     3319 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/fitting/_detect_peaks.py
--rw-rw-rw-   0        0        0     8604 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/fitting/_fitting_2d_beam_profiles.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/imaging/
--rw-rw-rw-   0        0        0       64 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/imaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/optics/
--rw-rw-rw-   0        0        0    32475 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/optics/_GVD_and_TOD_calculator.py
--rw-rw-rw-   0        0        0      357 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/optics/__init__.py
--rw-rw-rw-   0        0        0    12006 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/optics/_materials.py
--rw-rw-rw-   0        0        0     1070 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/optics/_spectra.py
--rw-rw-rw-   0        0        0      357 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/optics/_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/plot/
--rw-rw-rw-   0        0        0       67 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/plot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/signals/
--rw-rw-rw-   0        0        0       63 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/signals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/scilightcon/utils/
--rw-rw-rw-   0        0        0      342 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/utils/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/utils/_analyze_s2_data.py
--rw-rw-rw-   0        0        0       59 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/utils/_constants.py
--rw-rw-rw-   0        0        0      819 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/utils/_fixes.py
--rw-rw-rw-   0        0        0     1142 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/scilightcon/utils/_interpolate_and_multiply.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:44:15.760517 scilightcon-0.2.0.post2/scilightcon.egg-info/
--rw-rw-rw-   0        0        0     1201 2023-08-07 07:44:15.000000 scilightcon-0.2.0.post2/scilightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8028 2023-08-07 07:44:15.000000 scilightcon-0.2.0.post2/scilightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 07:44:15.000000 scilightcon-0.2.0.post2/scilightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-07 07:44:15.000000 scilightcon-0.2.0.post2/scilightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-07 07:44:15.000000 scilightcon-0.2.0.post2/scilightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 07:44:15.838672 scilightcon-0.2.0.post2/setup.cfg
--rw-rw-rw-   0        0        0     1659 2023-08-07 07:40:22.000000 scilightcon-0.2.0.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/
+-rw-rw-rw-   0        0        0     1094 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/LICENSE
+-rw-rw-rw-   0        0        0      368 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2274 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     1706 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.127222 scilightcon-0.2.0.post3/scilightcon/
+-rw-rw-rw-   0        0        0      227 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.127222 scilightcon-0.2.0.post3/scilightcon/control/
+-rw-rw-rw-   0        0        0       69 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.127222 scilightcon-0.2.0.post3/scilightcon/datasets/
+-rw-rw-rw-   0        0        0      574 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/__init__.py
+-rw-rw-rw-   0        0        0     9072 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/_base.py
+-rw-rw-rw-   0        0        0     7685 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/_logs_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.142846 scilightcon-0.2.0.post3/scilightcon/datasets/data/
+-rw-rw-rw-   0        0        0     1685 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/Ar_lines.csv
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.158491 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/
+-rw-rw-rw-   0        0        0        0 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/__init__.py
+-rw-rw-rw-   0        0        0    46206 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv
+-rw-rw-rw-   0        0        0    49586 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv
+-rw-rw-rw-   0        0        0    50284 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv
+-rw-rw-rw-   0        0        0    39791 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv
+-rw-rw-rw-   0        0        0    52825 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv
+-rw-rw-rw-   0        0        0    57433 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv
+-rw-rw-rw-   0        0        0    57324 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv
+-rw-rw-rw-   0        0        0    58434 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv
+-rw-rw-rw-   0        0        0    40227 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv
+-rw-rw-rw-   0        0        0    48209 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv
+-rw-rw-rw-   0        0        0    44452 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv
+-rw-rw-rw-   0        0        0    48918 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv
+-rw-rw-rw-   0        0        0      385 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/Hg_lines.csv
+-rw-rw-rw-   0        0        0   320206 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s
+-rw-rw-rw-   0        0        0     9518 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/White_LED_spectrum.csv
+-rw-rw-rw-   0        0        0        0 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0  1061194 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/atmosphere.csv
+-rw-rw-rw-   0        0        0     1042 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/data_test_detect_peaks.csv
+-rw-rw-rw-   0        0        0      531 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/data_test_detect_peaks.csv.gz
+-rw-rw-rw-   0        0        0     1042 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv
+-rw-rw-rw-   0        0        0   596451 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/logsreader_test.zip
+-rw-rw-rw-   0        0        0     7053 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv
+-rw-rw-rw-   0        0        0    10678 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv
+-rw-rw-rw-   0        0        0     6663 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EKSMA_Ag.csv
+-rw-rw-rw-   0        0        0     6485 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EKSMA_Al.csv
+-rw-rw-rw-   0        0        0     7022 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EKSMA_Au.csv
+-rw-rw-rw-   0        0        0   229421 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/test_beam_profile.pkl
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.220973 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/
+-rw-rw-rw-   0        0        0        0 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/__init__.py
+-rw-rw-rw-   0        0        0    53154 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv
+-rw-rw-rw-   0        0        0    53084 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv
+-rw-rw-rw-   0        0        0    52943 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv
+-rw-rw-rw-   0        0        0    54475 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv
+-rw-rw-rw-   0        0        0    22273 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv
+-rw-rw-rw-   0        0        0    24603 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv
+-rw-rw-rw-   0        0        0    22273 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv
+-rw-rw-rw-   0        0        0    22304 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv
+-rw-rw-rw-   0        0        0    22303 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv
+-rw-rw-rw-   0        0        0    56664 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv
+-rw-rw-rw-   0        0        0    56615 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv
+-rw-rw-rw-   0        0        0    56563 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv
+-rw-rw-rw-   0        0        0    56513 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv
+-rw-rw-rw-   0        0        0    56467 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv
+-rw-rw-rw-   0        0        0    56416 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv
+-rw-rw-rw-   0        0        0    56377 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv
+-rw-rw-rw-   0        0        0    56368 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv
+-rw-rw-rw-   0        0        0    56416 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv
+-rw-rw-rw-   0        0        0    56282 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv
+-rw-rw-rw-   0        0        0    56301 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv
+-rw-rw-rw-   0        0        0    56307 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv
+-rw-rw-rw-   0        0        0    56381 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv
+-rw-rw-rw-   0        0        0    56307 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv
+-rw-rw-rw-   0        0        0    55966 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv
+-rw-rw-rw-   0        0        0    56010 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv
+-rw-rw-rw-   0        0        0    56059 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv
+-rw-rw-rw-   0        0        0    56028 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv
+-rw-rw-rw-   0        0        0    55955 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv
+-rw-rw-rw-   0        0        0    55829 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv
+-rw-rw-rw-   0        0        0    55911 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv
+-rw-rw-rw-   0        0        0    55799 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv
+-rw-rw-rw-   0        0        0    55700 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv
+-rw-rw-rw-   0        0        0   129739 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv
+-rw-rw-rw-   0        0        0   129672 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv
+-rw-rw-rw-   0        0        0   129557 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv
+-rw-rw-rw-   0        0        0   129478 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv
+-rw-rw-rw-   0        0        0   129231 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv
+-rw-rw-rw-   0        0        0    56457 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv
+-rw-rw-rw-   0        0        0    56447 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv
+-rw-rw-rw-   0        0        0    56396 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv
+-rw-rw-rw-   0        0        0    56369 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv
+-rw-rw-rw-   0        0        0    56361 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv
+-rw-rw-rw-   0        0        0    56303 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv
+-rw-rw-rw-   0        0        0    56294 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv
+-rw-rw-rw-   0        0        0    56267 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv
+-rw-rw-rw-   0        0        0    56187 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv
+-rw-rw-rw-   0        0        0    56159 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv
+-rw-rw-rw-   0        0        0    56144 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv
+-rw-rw-rw-   0        0        0    56084 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv
+-rw-rw-rw-   0        0        0   129490 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv
+-rw-rw-rw-   0        0        0   129560 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv
+-rw-rw-rw-   0        0        0   129593 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv
+-rw-rw-rw-   0        0        0   129727 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv
+-rw-rw-rw-   0        0        0   129769 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv
+-rw-rw-rw-   0        0        0     7443 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv
+-rw-rw-rw-   0        0        0    11204 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv
+-rw-rw-rw-   0        0        0    11270 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv
+-rw-rw-rw-   0        0        0    11036 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv
+-rw-rw-rw-   0        0        0     7377 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv
+-rw-rw-rw-   0        0        0     7397 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv
+-rw-rw-rw-   0        0        0     7527 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv
+-rw-rw-rw-   0        0        0    55366 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv
+-rw-rw-rw-   0        0        0    54473 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv
+-rw-rw-rw-   0        0        0   105252 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv
+-rw-rw-rw-   0        0        0     5742 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv
+-rw-rw-rw-   0        0        0     5742 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv
+-rw-rw-rw-   0        0        0     5742 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv
+-rw-rw-rw-   0        0        0     5529 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv
+-rw-rw-rw-   0        0        0     5501 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv
+-rw-rw-rw-   0        0        0     5501 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv
+-rw-rw-rw-   0        0        0     5501 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv
+-rw-rw-rw-   0        0        0    75410 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv
+-rw-rw-rw-   0        0        0    75272 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv
+-rw-rw-rw-   0        0        0    74840 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv
+-rw-rw-rw-   0        0        0    74216 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv
+-rw-rw-rw-   0        0        0    73546 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv
+-rw-rw-rw-   0        0        0    73503 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv
+-rw-rw-rw-   0        0        0    73485 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv
+-rw-rw-rw-   0        0        0    73746 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv
+-rw-rw-rw-   0        0        0  1212522 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/datasets/data/toolbox_materials.pkl
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.220973 scilightcon-0.2.0.post3/scilightcon/fitting/
+-rw-rw-rw-   0        0        0      214 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/fitting/__init__.py
+-rw-rw-rw-   0        0        0     3319 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/fitting/_detect_peaks.py
+-rw-rw-rw-   0        0        0     8604 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/fitting/_fitting_2d_beam_profiles.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.220973 scilightcon-0.2.0.post3/scilightcon/imaging/
+-rw-rw-rw-   0        0        0       64 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/imaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/scilightcon/optics/
+-rw-rw-rw-   0        0        0    32475 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/optics/_GVD_and_TOD_calculator.py
+-rw-rw-rw-   0        0        0      357 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/optics/__init__.py
+-rw-rw-rw-   0        0        0    12006 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/optics/_materials.py
+-rw-rw-rw-   0        0        0     1070 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/optics/_spectra.py
+-rw-rw-rw-   0        0        0      357 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/optics/_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/scilightcon/plot/
+-rw-rw-rw-   0        0        0       67 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/plot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/scilightcon/signals/
+-rw-rw-rw-   0        0        0       63 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/signals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/scilightcon/utils/
+-rw-rw-rw-   0        0        0      342 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/utils/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/utils/_analyze_s2_data.py
+-rw-rw-rw-   0        0        0       59 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/utils/_constants.py
+-rw-rw-rw-   0        0        0      819 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/utils/_fixes.py
+-rw-rw-rw-   0        0        0     1142 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/scilightcon/utils/_interpolate_and_multiply.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:17:25.127222 scilightcon-0.2.0.post3/scilightcon.egg-info/
+-rw-rw-rw-   0        0        0     2274 2023-08-07 09:17:24.000000 scilightcon-0.2.0.post3/scilightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8028 2023-08-07 09:17:25.000000 scilightcon-0.2.0.post3/scilightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:17:24.000000 scilightcon-0.2.0.post3/scilightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-07 09:17:24.000000 scilightcon-0.2.0.post3/scilightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 09:17:24.000000 scilightcon-0.2.0.post3/scilightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:17:25.236644 scilightcon-0.2.0.post3/setup.cfg
+-rw-rw-rw-   0        0        0     1659 2023-08-07 09:14:45.000000 scilightcon-0.2.0.post3/setup.py
```

### Comparing `scilightcon-0.2.0.post2/LICENSE` & `scilightcon-0.2.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/__init__.py` & `scilightcon-0.2.0.post3/scilightcon/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/_base.py` & `scilightcon-0.2.0.post3/scilightcon/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/_logs_reader.py` & `scilightcon-0.2.0.post3/scilightcon/datasets/_logs_reader.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/Ar_lines.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/Ar_lines.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_400nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_450nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_500nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_550nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_600nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_650nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_700nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_lp_750nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_400nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_500nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_600nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/EO/transmission_EO_sp_700nm.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/Shot-to-shot_LAB4 PHAROS_25.0kHz_1030nm_InGaAs_20210917_1337.s2s`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/White_LED_spectrum.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/White_LED_spectrum.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/atmosphere.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/atmosphere.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/data_test_detect_peaks.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/data_test_detect_peaks.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/data_test_detect_peaks.csv.gz` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/data_test_detect_peaks.csv.gz`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/data_test_detect_peaks_extracted.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/logsreader_test.zip` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/logsreader_test.zip`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EDMUND_rr_Al.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EDMUND_rr_Au.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EKSMA_Ag.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EKSMA_Ag.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EKSMA_Al.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EKSMA_Al.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/reflection_EKSMA_Au.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/reflection_EKSMA_Au.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/test_beam_profile.pkl` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/test_beam_profile.pkl`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP425.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_DMLP650.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FB340-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH343-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH400-40.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH515-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH520-40.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FBH550-40.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0400.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0600.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0650.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0750.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0800.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0850.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0900.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL0950.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1000.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1050.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1100.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1150.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1200.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1250.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1300.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1350.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1400.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FEL1500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1000.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1050.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1100.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1250.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FELH1500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0600.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0650.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0750.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0800.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0850.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0900.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES0950.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FES1000.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0450.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0500.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0600.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FESH0750.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB37.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGB39.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS550.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS700.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGS900.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV11.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FGUV5.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL514.5-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_FL530-10.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_MF460-60.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV01B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV02B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV06B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV10B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV20B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV30B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NDUV40B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE01B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE06B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE10B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE20B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE30B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE40B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE50B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/thorlabs/transmission_THORLABS_NE60B.csv`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/datasets/data/toolbox_materials.pkl` & `scilightcon-0.2.0.post3/scilightcon/datasets/data/toolbox_materials.pkl`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/fitting/_detect_peaks.py` & `scilightcon-0.2.0.post3/scilightcon/fitting/_detect_peaks.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/fitting/_fitting_2d_beam_profiles.py` & `scilightcon-0.2.0.post3/scilightcon/fitting/_fitting_2d_beam_profiles.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/optics/_GVD_and_TOD_calculator.py` & `scilightcon-0.2.0.post3/scilightcon/optics/_GVD_and_TOD_calculator.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/optics/_materials.py` & `scilightcon-0.2.0.post3/scilightcon/optics/_materials.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/optics/_spectra.py` & `scilightcon-0.2.0.post3/scilightcon/optics/_spectra.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/utils/_analyze_s2_data.py` & `scilightcon-0.2.0.post3/scilightcon/utils/_analyze_s2_data.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/utils/_fixes.py` & `scilightcon-0.2.0.post3/scilightcon/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon/utils/_interpolate_and_multiply.py` & `scilightcon-0.2.0.post3/scilightcon/utils/_interpolate_and_multiply.py`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/scilightcon.egg-info/SOURCES.txt` & `scilightcon-0.2.0.post3/scilightcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scilightcon-0.2.0.post2/setup.py` & `scilightcon-0.2.0.post3/setup.py`

 * *Files identical despite different names*

