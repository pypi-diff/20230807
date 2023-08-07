# Comparing `tmp/sastadev-0.0.4a2.tar.gz` & `tmp/sastadev-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sastadev-0.0.4a2.tar", last modified: Mon Jun  5 11:57:04 2023, max compression
+gzip compressed data, was "sastadev-0.1.0.tar", last modified: Mon Aug  7 07:10:28 2023, max compression
```

## Comparing `sastadev-0.0.4a2.tar` & `sastadev-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,152 @@
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      143 2023-05-26 18:33:04.000000 sastadev-0.0.4a2/MANIFEST.in
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/PKG-INFO
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      207 2022-05-25 12:11:06.000000 sastadev-0.0.4a2/README.md
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/sastadev/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1533 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/LICENSE
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      136 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/__init__.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     4753 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/alpinoparsing.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    11249 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/celexlexicon.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      365 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/config.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    23928 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/deregularise.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)   111180 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/inflectioncorrection.tsv.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     5419 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/lexicon.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      197 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/memoize.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     5296 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/metadata.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1436 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/namepartlexicon.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.600349 sastadev-0.0.4a2/sastadev/names/
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/sastadev/names/nameparts/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)   104652 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/names/nameparts/namepartlexicon.csv
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/py.typed
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     2029 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/query.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1957 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/sastatoken.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     3269 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/sastatypes.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)     1282 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/sentence_parser.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    15967 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/stringfunctions.py
--rw-rw-r--   0 sheean    (1000) sheean    (1000)    76835 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev/treebankfunctions.py
-drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/sastadev.egg-info/
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      567 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/PKG-INFO
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      662 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/SOURCES.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/dependency_links.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        5 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/requires.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)        9 2023-06-05 11:57:04.000000 sastadev-0.0.4a2/sastadev.egg-info/top_level.txt
--rw-rw-r--   0 sheean    (1000) sheean    (1000)       38 2023-06-05 11:57:04.604349 sastadev-0.0.4a2/setup.cfg
--rw-rw-r--   0 sheean    (1000) sheean    (1000)      687 2023-06-05 11:56:46.000000 sastadev-0.0.4a2/setup.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.304365 sastadev-0.1.0/
+-rw-r--r--   0 a3248526   (502) staff       (20)     1533 2023-05-09 07:39:30.000000 sastadev-0.1.0/LICENSE
+-rw-r--r--   0 a3248526   (502) staff       (20)     3440 2023-08-07 07:10:28.304196 sastadev-0.1.0/PKG-INFO
+-rw-r--r--   0 a3248526   (502) staff       (20)     3048 2023-08-07 07:07:44.000000 sastadev-0.1.0/README.md
+-rw-r--r--   0 a3248526   (502) staff       (20)      328 2023-08-07 07:07:44.000000 sastadev-0.1.0/pyproject.toml
+-rw-r--r--   0 a3248526   (502) staff       (20)       38 2023-08-07 07:10:28.304412 sastadev-0.1.0/setup.cfg
+-rw-r--r--   0 a3248526   (502) staff       (20)      945 2023-08-07 07:07:44.000000 sastadev-0.1.0/setup.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.259735 sastadev-0.1.0/src/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.273169 sastadev-0.1.0/src/sastadev/
+-rw-r--r--   0 a3248526   (502) staff       (20)    11748 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/ASTApostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    39194 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/CHAT_Annotation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    23856 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/SAFreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1591 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/SRFreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1037 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/STAPpostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7260 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/Sziplus.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    10338 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/TARSPpostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5863 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/TARSPscreening.py
+-rw-r--r--   0 a3248526   (502) staff       (20)       64 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/__init__.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    56218 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/__main__.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1338 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/allresults.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3108 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/alpino.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4798 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/alpinoparsing.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13788 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/asta_neo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    12520 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/asta_queries.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13102 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/astaforms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    19783 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/basicreplacements.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    11294 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/celexlexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3667 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/checkcorrection.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9590 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/cleanCHILDEStokens.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3613 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/compounds.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      739 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/conf.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      383 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/constants.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    58858 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/corrector.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    38948 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/correcttreebank.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      770 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/counterfunctions.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.274684 sastadev-0.1.0/src/sastadev/data/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.259974 sastadev-0.1.0/src/sastadev/data/celexlexicon/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.289158 sastadev-0.1.0/src/sastadev/data/celexlexicon/dutch/
+-rw-r--r--   0 a3248526   (502) staff       (20) 10433870 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/celexlexicon/dutch/DMLCD.txt
+-rw-r--r--   0 a3248526   (502) staff       (20) 11540324 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)  4092534 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/celexlexicon/dutch/DSLCD.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.295752 sastadev-0.1.0/src/sastadev/data/compoundfiles/
+-rw-r--r--   0 a3248526   (502) staff       (20)  4216927 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)  1403658 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)   332732 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip
+-rw-r--r--   0 a3248526   (502) staff       (20)      390 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/expandedqueries.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.296120 sastadev-0.1.0/src/sastadev/data/filledpauseslexicon/
+-rw-r--r--   0 a3248526   (502) staff       (20)      145 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/filledpauseslexicon/filledpauseslexicon.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.296473 sastadev-0.1.0/src/sastadev/data/form_templates/
+-rw-r--r--   0 a3248526   (502) staff       (20)    48437 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    13350 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/form_templates/TARSP Form Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)   111180 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/inflectioncorrection.tsv.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.296930 sastadev-0.1.0/src/sastadev/data/macros/
+-rw-r--r--   0 a3248526   (502) staff       (20)    10249 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/macros/newimperatives.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    21128 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/macros/sastamacros1.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    10375 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/macros/sastamacros2.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.297991 sastadev-0.1.0/src/sastadev/data/methods/
+-rw-r--r--   0 a3248526   (502) staff       (20)    12711 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/ASTA Index Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    12471 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/ASTA_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    17518 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/STAP_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    17595 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/STAP_Index_Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    25892 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    25632 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/TARSP Index Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    26318 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/methods/TARSP_07062021.xlsx
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.298423 sastadev-0.1.0/src/sastadev/data/names/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.300914 sastadev-0.1.0/src/sastadev/data/names/Woonplaatsen/
+-rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)    66586 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.301963 sastadev-0.1.0/src/sastadev/data/names/fn10k_versie1/
+-rw-r--r--   0 a3248526   (502) staff       (20)  1088716 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml
+-rw-r--r--   0 a3248526   (502) staff       (20)     1442 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl
+-rw-r--r--   0 a3248526   (502) staff       (20)   134136 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/fn10k_versie1.zip
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.302480 sastadev-0.1.0/src/sastadev/data/names/hoofdsteden/
+-rw-r--r--   0 a3248526   (502) staff       (20)     8762 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)     7950 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.302688 sastadev-0.1.0/src/sastadev/data/names/nameparts/
+-rw-r--r--   0 a3248526   (502) staff       (20)   104652 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/nameparts/namepartlexicon.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)  2160410 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/names/voornamentop10000.xml
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.302936 sastadev-0.1.0/src/sastadev/data/top3000/
+-rw-r--r--   0 a3248526   (502) staff       (20)   186224 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/data/top3000/Woordenlijsten Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    35894 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/dedup.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    23956 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/deregularise.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7380 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/exampletrees.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      993 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/expandquery.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3652 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/external_functions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1630 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/filefunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9032 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/find_ngram.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      473 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/forms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6814 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/generatemacros.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5251 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/goldcountreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    17456 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/iedims.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5275 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/imperatives.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5485 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/lexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      959 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/macrolength.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2831 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/macros.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      197 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/memoize.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5298 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/metadata.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      583 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/methodinfo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2525 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/methods.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    10782 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/mismatches.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9027 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/mksilver.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1542 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/mwe2pep.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1462 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/namepartlexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1028 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/phonetics.py
+-rw-r--r--   0 a3248526   (502) staff       (20)        0 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/py.typed
+-rw-r--r--   0 a3248526   (502) staff       (20)     2043 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/query.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5735 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/queryfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1718 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/readcsv.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7308 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/readmethod.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1599 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/rpf1.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1863 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/sasta_explanation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2292 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/sastatok.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1957 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/sastatoken.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3289 2023-08-07 07:09:35.000000 sastadev-0.1.0/src/sastadev/sastatypes.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1329 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/sentence_parser.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13468 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/smallclauses.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3358 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/stapforms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    15967 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/stringfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    31189 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/sva.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1614 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/targets.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4692 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/tarspform.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6434 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/tblex.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1475 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/tokeniseCHILDES.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      880 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/tokenmd.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4341 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/top3000.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    77130 2023-08-07 07:09:35.000000 sastadev-0.1.0/src/sastadev/treebankfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2091 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/xenx.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5144 2023-08-07 07:07:44.000000 sastadev-0.1.0/src/sastadev/xlsx.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.274307 sastadev-0.1.0/src/sastadev.egg-info/
+-rw-r--r--   0 a3248526   (502) staff       (20)     3440 2023-08-07 07:10:28.000000 sastadev-0.1.0/src/sastadev.egg-info/PKG-INFO
+-rw-r--r--   0 a3248526   (502) staff       (20)     4128 2023-08-07 07:10:28.000000 sastadev-0.1.0/src/sastadev.egg-info/SOURCES.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)        1 2023-08-07 07:10:28.000000 sastadev-0.1.0/src/sastadev.egg-info/dependency_links.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       52 2023-08-07 07:10:28.000000 sastadev-0.1.0/src/sastadev.egg-info/entry_points.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       33 2023-08-07 07:10:28.000000 sastadev-0.1.0/src/sastadev.egg-info/requires.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)        9 2023-08-07 07:10:28.000000 sastadev-0.1.0/src/sastadev.egg-info/top_level.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:28.825737 sastadev-0.1.0/tests/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2023-08-07 07:10:30.826687 sastadev-0.1.0/tests/__pycache__/
+-rw-r--r--   0 a3248526   (502) staff       (20)    15132 2023-08-07 07:10:28.828588 sastadev-0.1.0/tests/__pycache__/test_adjacency.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     1168 2023-08-07 07:10:28.854657 sastadev-0.1.0/tests/__pycache__/test_explanation.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     2655 2023-08-07 07:10:28.861668 sastadev-0.1.0/tests/__pycache__/test_hyphens.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     7255 2023-08-07 07:10:30.288936 sastadev-0.1.0/tests/__pycache__/test_indexexpansion.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     6907 2023-08-07 07:10:30.290597 sastadev-0.1.0/tests/__pycache__/test_lxml.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     2145 2023-08-07 07:10:30.292611 sastadev-0.1.0/tests/__pycache__/test_smallclauses.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)    15020 2023-08-07 07:10:30.826631 sastadev-0.1.0/tests/__pycache__/test_vobij.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)    13386 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_adjacency.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      960 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_explanation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      634 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_hyphens.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6946 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_indexexpansion.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7187 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_lxml.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1971 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_smallclauses.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14153 2023-08-07 07:07:44.000000 sastadev-0.1.0/tests/test_vobij.py
```

### Comparing `sastadev-0.0.4a2/sastadev/LICENSE` & `sastadev-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a2/sastadev/alpinoparsing.py` & `sastadev-0.1.0/src/sastadev/alpinoparsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 * previewing a parse tree:
 
 .. autofunction:: alpinoparsing::previewurl
 
 '''
 
+import logging
 import re
 import urllib.parse
 import urllib.request
 
 from lxml import etree  # type: ignore
-from memoize import memoize
 
-import logging
-#from sastatypes import SynTree, URL
+from sastadev.memoize import memoize
+
+#from sastadev.sastatypes import SynTree, URL
 
-#from config import SDLOGGER
-#from sastatypes import SynTree, URL
+#from sastadev.config import settings.logger
+#from sastadev.sastatypes import SynTree, URL
 
 urllibrequestversion = urllib.request.__version__
 
 alpino_special_symbols_pattern = r'[\[\]]'
 alpino_special_symbols_re = re.compile(alpino_special_symbols_pattern)
 
 gretelurl = 'https://gretel.hum.uu.nl/api/src/router.php/parse_sentence/'
```

### Comparing `sastadev-0.0.4a2/sastadev/celexlexicon.py` & `sastadev-0.1.0/src/sastadev/celexlexicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 '''
 
 import csv
 import os
 import re
 import sys
 from collections import defaultdict
-
-import treebankfunctions
-from config import SD_DIR
 from typing import Dict, List, Optional, Tuple
-from sastatypes import CELEX_INFL, SynTree, WordInfo
+
+from sastadev import treebankfunctions
+from sastadev.conf import settings
+from sastadev.sastatypes import CELEX_INFL, SynTree, WordInfo
 
 backslash = '\\'
 celexsep = backslash
 
 pospattern = r'^.*\[(?P<pos>.)\]$'
 posre = re.compile(pospattern)
 
@@ -48,15 +48,15 @@
 # verbs that do not necessarily have a t suffix  in present tense singular
 no_t_verbs = {'mogen', 'kunnen', 'zullen', 'willen'}
 
 logfile = sys.stderr
 
 # initialisation
 # read the celex lexicon
-inputfolder = os.path.join(SD_DIR, 'celexlexicondata', 'dutch')
+inputfolder = os.path.join(settings.SD_DIR, 'data', 'celexlexicon', 'dutch')
 
 dmwfilename = 'DMWCDOK.txt'
 dmwfullname = os.path.join(inputfolder, dmwfilename)
 dmwdict: Dict[str, List[str]] = {}
 dmwlemmakeyinflindex: Dict[Tuple[str, str], List[str]] = defaultdict(list)
 dmwkeydict = {}
```

### Comparing `sastadev-0.0.4a2/sastadev/deregularise.py` & `sastadev-0.1.0/src/sastadev/deregularise.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,19 @@
   **Remark** The functions should be extended so that also inflection information is
   returned.
 
   **Remark** Instead os a single correction a list of corrections should be returned. a selection can be made on the basis of inflectinnal information.
 
 '''
 import csv
-import re
 import os
-from typing import cast, Dict, List, Optional, Tuple
-from config import SD_DIR
+import re
+from typing import Dict, List, Optional, Tuple, cast
+
+from sastadev.conf import settings
 
 tab = '\t'
 plussym = '+'
 
 # maybe also add a variant with e- as prefix instead of ge-, and also without ge-
 
 
@@ -624,14 +625,14 @@
 # eigenlijk nog de inflectiecode erbij@@@
 
 #: The dictionary *correction* consists of items with a string as key and a tuple of
 #: two strings (corrected form, metadata) as value. This dictionary is filled by
 #: reading from the file with the name in the constant *correctionfilename* upon
 #: initialisation of the module *deregularise*
 correction: Dict[str, Tuple[str, str]] = {}
-correctionfile = open(os.path.join(SD_DIR, correctionfilename), 'r', encoding='utf8')
+correctionfile = open(os.path.join(settings.SD_DIR, 'data', correctionfilename), 'r', encoding='utf8')
 myreader = csv.reader(correctionfile, delimiter=tab)
 for row in myreader:
     wrong = row[0]
     good = row[1]
     meta = row[2]
     correction[wrong] = good, meta
```

### Comparing `sastadev-0.0.4a2/sastadev/inflectioncorrection.tsv.txt` & `sastadev-0.1.0/src/sastadev/data/inflectioncorrection.tsv.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a2/sastadev/lexicon.py` & `sastadev-0.1.0/src/sastadev/lexicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 Currently we especially use the CELEX lexicon.
 This module also contains some special word lists. Perhaps we should set up a special Exception List module
 for this purpose.
 
 
 '''
 
-import celexlexicon
-import treebankfunctions
-from namepartlexicon import namepart_isa_namepart, namepart_isa_namepart_uc
-
 from typing import Any, Dict, List, Optional
-from sastatypes import CELEX_INFL, DCOITuple, Lemma, SynTree, WordInfo
+
+from sastadev import celexlexicon, treebankfunctions
+from sastadev.namepartlexicon import (namepart_isa_namepart,
+                                      namepart_isa_namepart_uc)
+from sastadev.sastatypes import CELEX_INFL, DCOITuple, Lemma, SynTree, WordInfo
 
 space = ' '
 
 celex = 'celex'
 alpino = 'alpino'
 
 # the CHAT codes xxx and yyy must be recognised as valid codes and as valid words in some cases
```

### Comparing `sastadev-0.0.4a2/sastadev/metadata.py` & `sastadev-0.1.0/src/sastadev/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from lxml import etree
 from typing import List
 
+from lxml import etree
+
 bpl_none, bpl_word, bpl_node, bpl_delete, bpl_indeze, bpl_extra_grammatical, bpl_wordlemma = tuple(range(7))
 defaultpenalty = 10
 defaultbackplacement = bpl_none
 
 SASTA = 'SASTA'
 
 xmlformat = '''
```

### Comparing `sastadev-0.0.4a2/sastadev/namepartlexicon.py` & `sastadev-0.1.0/src/sastadev/namepartlexicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 .. autofunction:: namepart_isa_namepart
 .. autofunction:: namepart_isa_namepart_uc
 
 '''
 
 import csv
 import os
-
-from config import SD_DIR
 from typing import Dict
 
+from sastadev.conf import settings
+
 tab: str = '\t'
 namepartlexicon: Dict[str, int] = {}
 
 
 def namepart_isa_namepart(word: str) -> bool:
     '''
     The function namepart_isa_namepart checks whether the string *word* occurs in the namepartlexicon dictionary.
@@ -43,14 +43,14 @@
     else:
         uc = word[0].isupper()
         found = word in namepartlexicon
         result = uc and found
     return result
 
 
-namepartfilename = os.path.join(SD_DIR, 'names', 'nameparts', 'namepartlexicon.csv')
+namepartfilename = os.path.join(settings.SD_DIR, 'data', 'names', 'nameparts', 'namepartlexicon.csv')
 with open(namepartfilename, 'r', encoding='utf8') as namepartfile:
     csvreader = csv.reader(namepartfile, delimiter=tab)
     for row in csvreader:
         namepart = row[0]
         frq = int(row[1])
         namepartlexicon[namepart] = frq
```

### Comparing `sastadev-0.0.4a2/sastadev/names/nameparts/namepartlexicon.csv` & `sastadev-0.1.0/src/sastadev/data/names/nameparts/namepartlexicon.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a2/sastadev/query.py` & `sastadev-0.1.0/src/sastadev/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from config import SDLOGGER
+from sastadev.conf import settings
 
 pre_process_str, core_process_str, post_process_str, form_process_str = 'pre', 'core', 'post', 'form'
 pre_process, core_process, post_process, form_process = 0, 1, 2, 3
 
 
 def getprocess(process):
     if process.lower() == core_process_str:
@@ -11,15 +11,15 @@
         result = post_process
     elif process.lower() == pre_process_str:
         result = pre_process
     elif process.lower() == form_process_str:
         result = form_process
     else:
         result = -1
-        SDLOGGER.error('Illegal value for process {}'.format(process))
+        settings.LOGGER.error('Illegal value for process {}'.format(process))
     return result
 
 
 def clean(valstr):
     result = valstr.strip().lower()
     return result
```

### Comparing `sastadev-0.0.4a2/sastadev/sastatoken.py` & `sastadev-0.1.0/src/sastadev/sastatoken.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a2/sastadev/sastatypes.py` & `sastadev-0.1.0/src/sastadev/sastatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 '''
 This module contains definitions of types used in multiple modules
 '''
 
-from typing import Dict, List, Tuple, Callable, Optional, Union
-from typing_extensions import TypeAlias
-from lxml import etree  # type: ignore
 from collections import Counter
-from query import Query
-from sastatoken import Token
+from typing import Callable, Dict, List, Optional, Tuple, Union
+
+from lxml import etree  # type: ignore
+from typing_extensions import TypeAlias
+
+from sastadev.query import Query
+from sastadev.sastatoken import Token
 
 AltId: TypeAlias = int
 BackPlacement: TypeAlias = int
 CapitalName: TypeAlias = str
 CountryName: TypeAlias = str
 ContinentName: TypeAlias = str
 CELEXPosCode: TypeAlias = str
```

### Comparing `sastadev-0.0.4a2/sastadev/sentence_parser.py` & `sastadev-0.1.0/src/sastadev/sentence_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from functools import lru_cache
 import socket
 from contextlib import contextmanager
+from functools import lru_cache
 
 from lxml import etree
 
-import config
-
-from alpinoparsing import escape_alpino_input, isempty
+import sastadev.conf
+from sastadev.alpinoparsing import escape_alpino_input, isempty
 
 
 class AlpinoSentenceParser:
     ''' Assumes a Alpino server is running on provided host:port,
     with assume_input_is_tokenized=off '''
     @contextmanager
     def connection(self):
         try:
-            s = socket.create_connection((config.ALPINO_HOST, config.ALPINO_PORT))
+            s = socket.create_connection((sastadev.conf.settings.ALPINO_HOST, sastadev.conf.settings.ALPINO_PORT))
             yield s
             s.close()
         except socket.error:
             raise
 
     def parse_sentence(self, sentence: str, buffer_size=8096) -> str:
         sentence = escape_alpino_input(sentence)
```

### Comparing `sastadev-0.0.4a2/sastadev/stringfunctions.py` & `sastadev-0.1.0/src/sastadev/stringfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.0.4a2/sastadev/treebankfunctions.py` & `sastadev-0.1.0/src/sastadev/treebankfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 '''
 
 # import sys
 import re
 # import logging
 from copy import copy, deepcopy
-from lxml import etree
-from config import SDLOGGER
-from stringfunctions import allconsonants
-# from lexicon import informlexiconpos, isa_namepart_uc, informlexicon, isa_namepart
-#import lexicon as lex
-from config import PARSE_FUNC
-
-from sastatoken import Token
-from metadata import Meta
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
-from sastatypes import FileName, OptPhiTriple, PhiTriple, Position, PositionMap, PositionStr, Span, SynTree, UttId
+from lxml import etree
+
+# from sastadev.lexicon import informlexiconpos, isa_namepart_uc, informlexicon, isa_namepart
+#import lexicon as lex
+from sastadev.conf import settings
+from sastadev.metadata import Meta
+from sastadev.sastatoken import Token
+from sastadev.sastatypes import (FileName, OptPhiTriple, PhiTriple, Position,
+                                 PositionMap, PositionStr, Span, SynTree,
+                                 UttId)
+from sastadev.stringfunctions import allconsonants
 
 
 class Metadata:
     '''
     contains 3 elements, each a string: type, name, value
     '''
 
@@ -437,15 +438,15 @@
     if v1 in persons and v2 in persons:
         result = valmerge(v1, v2, persons)
     elif v1 in numbers and v2 in numbers:
         result = valmerge(v1, v2, numbers)
     elif v1 in genders and v2 in genders:
         result = valmerge(v1, v2, genders)
     else:
-        SDLOGGER.error('Phimax: Illegal or incompatible value combination: V1={}, v2={}'.format(v1, v2))
+        settings.LOGGER.error('Phimax: Illegal or incompatible value combination: V1={}, v2={}'.format(v1, v2))
         result = v1
     return result
 
 
 def merge(phi1: OptPhiTriple, phi2: OptPhiTriple) -> OptPhiTriple:
     if phi1 is None or phi2 is None:
         return None
@@ -634,19 +635,19 @@
         for node in syntree.iter():
             if 'pt' in node.attrib or 'pos' in node.attrib:
                 if 'word' in node.attrib and 'end' in node.attrib:
                     newel = (node.attrib['word'], int(node.attrib['end']))
                     resultlist.append(newel)
                 else:
                     if 'word' not in node.attrib:
-                        SDLOGGER.error('No word in pt or pos node')
+                        settings.LOGGER.error('No word in pt or pos node')
                     if 'end' not in node.attrib:
-                        SDLOGGER.error('No end in pt or pos node')
+                        settings.LOGGER.error('No end in pt or pos node')
                     for el in node.attrib:
-                        SDLOGGER.info('{}\t{}'.format(el, node.attrib[el]))
+                        settings.LOGGER.info('{}\t{}'.format(el, node.attrib[el]))
         sortedresultlist = sorted(resultlist, key=lambda x: x[1])
         theyield = [w for (w, _) in sortedresultlist]
     return theyield
 
 
 def parent(node: SynTree) -> Optional[SynTree]:
     pnodes = node.xpath('parent::node')
@@ -1221,42 +1222,42 @@
         return newstree
 
 
 def getstree(fullname: FileName) -> SynTree:
     try:
         thefile = open(fullname, 'r', encoding='utf8')
     except FileNotFoundError as e:
-        SDLOGGER.error('File not found: {}'.format(e))
+        settings.LOGGER.error('File not found: {}'.format(e))
         return None
     except etree.ParseError as e:
-        SDLOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
+        settings.LOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
         return None
     except OSError as e:
-        SDLOGGER.error('OS Error: {}; file: {}'.format(e, fullname))
+        settings.LOGGER.error('OS Error: {}; file: {}'.format(e, fullname))
         return None
     except Exception:
-        SDLOGGER.error('Error: Unknown error in file {}'.format(fullname))
+        settings.LOGGER.error('Error: Unknown error in file {}'.format(fullname))
         return None
 
     with thefile:
         try:
             tree = etree.parse(thefile)
         except etree.ParseError as e:
-            SDLOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
+            settings.LOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
             return None
         except UnicodeDecodeError as e:
-            SDLOGGER.error('Unicode error: {} in file {}'.format(e, fullname))
+            settings.LOGGER.error('Unicode error: {} in file {}'.format(e, fullname))
             try:
                 windowsfile = open(fullname, 'r')
                 tree = etree.parse(windowsfile)
             except ValueError as e:
-                SDLOGGER.error('Char Descoding Error: {}; file: {}'.format(e, fullname))
+                settings.LOGGER.error('Char Descoding Error: {}; file: {}'.format(e, fullname))
                 return None
             except etree.ParseError as e:
-                SDLOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
+                settings.LOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
                 return None
             else:
                 return tree
         else:
             return tree
 
 
@@ -1390,15 +1391,15 @@
         lmc = lastmainclauseof(stree)
         print(getmarkedutt(lmc, stree))
 
 
 def getsentid(stree: SynTree) -> UttId:
     sentidlist = stree.xpath(sentidxpath)
     if sentidlist == []:
-        SDLOGGER.error('Missing sentid')
+        settings.LOGGER.error('Missing sentid')
         result = 'None'
     else:
         result = str(sentidlist[0])
     return result
 
 
 def testindextransform() -> None:
@@ -1418,15 +1419,15 @@
 
 def adaptsentence(stree: SynTree) -> SynTree:
     # adapt the sentence
     # find the sentence element's parent and its index
     sentid = getsentid(stree)
     sentencenode = stree.find('.//sentence')
     if sentencenode is None:
-        SDLOGGER.ERROR('No sentence element found for stree with sentid={}'.format(sentid))
+        settings.LOGGER.ERROR('No sentence element found for stree with sentid={}'.format(sentid))
         return stree
     sentencenodeparent = sentencenode.getparent()
     sentencenodeindex = sentencenodeparent.index(sentencenode)
     sentencenodeparent.remove(sentencenode)
     # del sentencenodeparent[sentencenodeindex]
     theyield = getyield(stree)
     theyieldstr = space.join(theyield)
@@ -1450,21 +1451,21 @@
     # determine the index of node1
     sentid = getsentid(stree)
     parentindex = get_parentandindex(node1, stree)
     if parentindex is None:
         result = stree
     else:
         parent, index = parentindex
-        # SDLOGGER.debug(simpleshow(parent))
+        # settings.LOGGER.debug(simpleshow(parent))
         del parent[index]
-        # SDLOGGER.debug(simpleshow(parent))
+        # settings.LOGGER.debug(simpleshow(parent))
         parent.insert(index, node2)
-        # SDLOGGER.debug(simpleshow(parent))
+        # settings.LOGGER.debug(simpleshow(parent))
         result = stree
-        # SDLOGGER.debug(simpleshow(stree))
+        # settings.LOGGER.debug(simpleshow(stree))
 
     # adapt the sentence
     # find the sentence element's parent and its index
     sentencenode = stree.find('.//sentence')
     sentencenodeparent = sentencenode.getparent()
     sentencenodeindex = sentencenodeparent.index(sentencenode)
     del sentencenodeparent[sentencenodeindex]
@@ -1580,15 +1581,15 @@
         elif child.tag == 'comments':
             comments = child
         elif child.tag == 'node':
             node = child
         elif child.tag == 'parser':
             parser = child
         else:
-            SDLOGGER.error('Unknown tag encountered in tree: {}'.format(child.tag))
+            settings.LOGGER.error('Unknown tag encountered in tree: {}'.format(child.tag))
     return parser, metadata, node, sentence, comments
 
 
 comma = ','
 
 
 def str2list(liststr: str, sep: str = comma) -> List[str]:
@@ -1646,15 +1647,15 @@
     return result
 
 
 def gettreepos(origpos: PositionStr, reverseindex: List[PositionStr]) -> PositionStr:  # origuttpos2treepos
     if origpos in reverseindex:
         result = str(reverseindex.index(origpos))
     else:
-        SDLOGGER.error('origpos {} not in reverseindex: {}'.format(origpos, reverseindex))
+        settings.LOGGER.error('origpos {} not in reverseindex: {}'.format(origpos, reverseindex))
         result = str(0)
     return result
 
 
 def deletewordnode(tree: SynTree, begin: Position) -> SynTree:
     newtree = deepcopy(tree)
     if newtree is None:
@@ -1869,24 +1870,24 @@
                 'end' in node.attrib and 'begin' in node.attrib:
             intend = int(node.attrib['end'])
             if intend in tokenposdict:
                 newendint = tokenposdict[intend]
                 node.attrib['end'] = str(newendint)
                 node.attrib['begin'] = str(newendint - 1)
             else:
-                SDLOGGER.error('Correcttreebank:updatetokenpos: Missing key in tokenposdict: key={key}'.format(key=intend))
+                settings.LOGGER.error('Correcttreebank:updatetokenpos: Missing key in tokenposdict: key={key}'.format(key=intend))
                 fulltrees = node.xpath('ancestor::node[@cat="top"]')
                 if fulltrees != []:
                     fulltree = fulltrees[0]
                 else:
                     fulltree = node
                 sent = getyield(fulltree)
-                SDLOGGER.error('utterance={}'.format(sent))
+                settings.LOGGER.error('utterance={}'.format(sent))
                 # etree.dump(resulttree)
-                SDLOGGER.error('tokenposdict={}'.format(tokenposdict))
+                settings.LOGGER.error('tokenposdict={}'.format(tokenposdict))
         elif 'cat' in node.attrib:
             children = [ch for ch in node]
             (b, e) = getbeginend(children)
             node.attrib['begin'] = b
             node.attrib['end'] = e
     return node
 
@@ -1908,27 +1909,27 @@
 
 def treewithtokenpos(thetree: SynTree, tokenlist: List[Token]) -> SynTree:
     resulttree = deepcopy(thetree)
     thetreeleaves = getnodeyield(thetree)
     intbegins = [int(getattval(n, 'begin')) for n in thetreeleaves]
     tokenlistbegins = [t.pos + t.subpos for t in tokenlist]
     if len(intbegins) != len(tokenlistbegins):
-        SDLOGGER.error('token mismatch')
-        SDLOGGER.error('tree yield={}'.format(getyield(thetree)))
-        SDLOGGER.error('tokenlist={}'.format(tokenlist))
-        SDLOGGER.error('intbegins={}'.format(intbegins))
-        SDLOGGER.error('tokenlistbegins ={}'.format(tokenlistbegins))
+        settings.LOGGER.error('token mismatch')
+        settings.LOGGER.error('tree yield={}'.format(getyield(thetree)))
+        settings.LOGGER.error('tokenlist={}'.format(tokenlist))
+        settings.LOGGER.error('intbegins={}'.format(intbegins))
+        settings.LOGGER.error('tokenlistbegins ={}'.format(tokenlistbegins))
     pospairs = zip(intbegins, tokenlistbegins)
     thetreetokenposdict = {treepos + 1: tokenpos + 1 for treepos, tokenpos in pospairs}
     resulttree = updatetokenpos(resulttree, thetreetokenposdict)
     return resulttree
 
 
 def fatparse(utterance: str, tokenlist: List[Token]) -> SynTree:
-    stree = PARSE_FUNC(utterance)
+    stree = settings.PARSE_FUNC(utterance)
     fatstree = deepcopy(stree)
     treeinflate(fatstree, start=10, inc=10)
     debug = False
     if debug:
         showtree(fatstree, text='fatparse: fatstree')
     reducedtokenlist = [token for token in tokenlist if not token.skip]
     fatstree = treewithtokenpos(fatstree, reducedtokenlist)
```

