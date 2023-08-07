# Comparing `tmp/pami-2023.8.6.2.tar.gz` & `tmp/pami-2023.8.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.8.6.2.tar", last modified: Mon Aug  7 12:14:34 2023, max compression
+gzip compressed data, was "pami-2023.8.6.3.tar", last modified: Mon Aug  7 13:04:21 2023, max compression
```

## Comparing `pami-2023.8.6.2.tar` & `pami-2023.8.6.3.tar`

### file list

```diff
@@ -1,439 +1,439 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.611455 pami-2023.8.6.2/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.8.6.2/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.529804 pami-2023.8.6.2/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.529997 pami-2023.8.6.2/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.531873 pami-2023.8.6.2/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.8.6.2/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.8.6.2/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.8.6.2/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.532097 pami-2023.8.6.2/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.533455 pami-2023.8.6.2/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.8.6.2/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.8.6.2/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.533597 pami-2023.8.6.2/PAMI/coveragePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.534330 pami-2023.8.6.2/PAMI/coveragePattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.8.6.2/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.8.6.2/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.535352 pami-2023.8.6.2/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.537440 pami-2023.8.6.2/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4194 2023-08-07 03:01:33.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.537902 pami-2023.8.6.2/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.539546 pami-2023.8.6.2/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15113 2023-08-06 15:38:03.000000 pami-2023.8.6.2/PAMI/extras/dbStats/sequentialDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-07-30 05:40:09.000000 pami-2023.8.6.2/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9475 2023-08-06 15:38:03.000000 pami-2023.8.6.2/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.540235 pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.540874 pami-2023.8.6.2/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.541913 pami-2023.8.6.2/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-07-28 06:47:15.000000 pami-2023.8.6.2/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 06:55:18.000000 pami-2023.8.6.2/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2428 2023-08-02 09:17:46.000000 pami-2023.8.6.2/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.542143 pami-2023.8.6.2/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.542384 pami-2023.8.6.2/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.542873 pami-2023.8.6.2/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.544483 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.544639 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.545998 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13539 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21425 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.546143 pami-2023.8.6.2/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.547207 pami-2023.8.6.2/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13211 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12603 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13581 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13664 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20368 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.548064 pami-2023.8.6.2/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-07-28 04:20:39.000000 pami-2023.8.6.2/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.549373 pami-2023.8.6.2/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5835 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13146 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13904 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12502 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14048 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14219 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16723 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13776 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.549898 pami-2023.8.6.2/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25085 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.550677 pami-2023.8.6.2/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5611 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14955 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12298 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16532 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.551197 pami-2023.8.6.2/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-07-28 04:20:39.000000 pami-2023.8.6.2/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.551343 pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.551816 pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25491 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.552078 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.552873 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20917 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26298 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.553029 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.555336 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-07-29 15:37:17.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27143 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.555504 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.556431 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-07-29 15:44:25.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-07-29 15:44:25.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.556617 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.557655 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23759 2023-08-04 05:55:40.000000 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-07-28 04:20:39.000000 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.557955 pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.558602 pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.558781 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.560183 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.560532 pami-2023.8.6.2/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.560732 pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.561518 pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-07-29 16:51:12.000000 pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.561780 pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.562251 pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.562434 pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.563425 pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-07-29 16:07:24.000000 pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.563688 pami-2023.8.6.2/PAMI/highUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.565152 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.565693 pami-2023.8.6.2/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.566481 pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.566829 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.568866 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-07-29 16:07:24.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.577004 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.577618 pami-2023.8.6.2/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.579918 pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.580059 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.581133 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-07-29 11:47:49.000000 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.581406 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.582069 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.582224 pami-2023.8.6.2/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.583306 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.583797 pami-2023.8.6.2/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.584312 pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.584937 pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-06 15:38:03.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5769 2023-08-07 03:11:13.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    30244 2023-08-07 03:36:58.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.585659 pami-2023.8.6.2/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.586394 pami-2023.8.6.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-07-29 16:46:35.000000 pami-2023.8.6.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.586550 pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.586997 pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.587155 pami-2023.8.6.2/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.589196 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.589754 pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.590489 pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.591138 pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.591684 pami-2023.8.6.2/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-28 05:36:37.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5380 2023-08-07 03:07:52.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24445 2023-08-07 03:35:37.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.592053 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.592607 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.593202 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.593454 pami-2023.8.6.2/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.594021 pami-2023.8.6.2/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.594217 pami-2023.8.6.2/PAMI/relativeFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.595001 pami-2023.8.6.2/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-01 01:42:22.000000 pami-2023.8.6.2/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.595189 pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.595640 pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.595794 pami-2023.8.6.2/PAMI/sequence/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequence/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.595891 pami-2023.8.6.2/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.597052 pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18133 2023-08-02 09:17:46.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.597738 pami-2023.8.6.2/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.597845 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.599173 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-07-29 11:25:56.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-07-29 11:57:55.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-07-29 11:57:55.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.599754 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.600162 pami-2023.8.6.2/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.600315 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.602178 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.602357 pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.603880 pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.604482 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.605544 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-07-29 11:28:40.000000 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-07-29 11:28:40.000000 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.605813 pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.606593 pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.606785 pami-2023.8.6.2/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.607468 pami-2023.8.6.2/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-07-29 11:29:36.000000 pami-2023.8.6.2/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.607734 pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.608603 pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.608784 pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.609535 pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-07-29 11:29:37.000000 pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-07 12:14:34.611252 pami-2023.8.6.2/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    60578 2023-08-02 07:28:07.000000 pami-2023.8.6.2/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 12:14:34.610826 pami-2023.8.6.2/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-07 12:14:34.000000 pami-2023.8.6.2/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15566 2023-08-07 12:14:34.000000 pami-2023.8.6.2/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-07 12:14:34.000000 pami-2023.8.6.2/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-07 12:14:34.000000 pami-2023.8.6.2/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-07 12:14:34.000000 pami-2023.8.6.2/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-07 12:14:34.611533 pami-2023.8.6.2/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1405 2023-08-07 12:14:24.000000 pami-2023.8.6.2/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.910264 pami-2023.8.6.3/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.8.6.3/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.831052 pami-2023.8.6.3/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.831239 pami-2023.8.6.3/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.833095 pami-2023.8.6.3/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.833351 pami-2023.8.6.3/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.834959 pami-2023.8.6.3/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.835111 pami-2023.8.6.3/PAMI/coveragePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.835912 pami-2023.8.6.3/PAMI/coveragePattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.836935 pami-2023.8.6.3/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.838320 pami-2023.8.6.3/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4194 2023-08-07 03:01:33.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.838695 pami-2023.8.6.3/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.840145 pami-2023.8.6.3/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15113 2023-08-06 15:38:03.000000 pami-2023.8.6.3/PAMI/extras/dbStats/sequentialDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-07-30 05:40:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9475 2023-08-06 15:38:03.000000 pami-2023.8.6.3/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.840779 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.841309 pami-2023.8.6.3/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.842264 pami-2023.8.6.3/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-07-28 06:47:15.000000 pami-2023.8.6.3/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 06:55:18.000000 pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2428 2023-08-02 09:17:46.000000 pami-2023.8.6.3/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.842488 pami-2023.8.6.3/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.842749 pami-2023.8.6.3/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.843127 pami-2023.8.6.3/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.849851 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.850012 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.851095 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13539 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21425 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.851267 pami-2023.8.6.3/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.852505 pami-2023.8.6.3/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13211 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12603 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13581 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13664 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20368 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.853164 pami-2023.8.6.3/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-07-28 04:20:39.000000 pami-2023.8.6.3/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.855073 pami-2023.8.6.3/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5835 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13146 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13904 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12502 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14048 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14219 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16723 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13776 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.855690 pami-2023.8.6.3/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25085 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.856696 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5611 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14955 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12298 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16532 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.857714 pami-2023.8.6.3/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-07-28 04:20:39.000000 pami-2023.8.6.3/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.857884 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.858710 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25491 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.859182 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.860356 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20917 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26298 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.860529 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.861591 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-07-29 15:37:17.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27143 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.861789 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.862974 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-07-29 15:44:25.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-07-29 15:44:25.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.863146 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.864195 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23759 2023-08-04 05:55:40.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-07-28 04:20:39.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.864422 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.865131 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.865311 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.866657 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.866965 pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.867236 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.868083 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-07-29 16:51:12.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.868420 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.868886 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.869053 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.870047 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-07-29 16:07:24.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.870293 pami-2023.8.6.3/PAMI/highUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.871751 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.872297 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.873024 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.873469 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.874437 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-07-29 16:07:24.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.874921 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.875076 pami-2023.8.6.3/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.875923 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.876082 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.877079 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-07-29 11:47:49.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.877267 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.877929 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.878083 pami-2023.8.6.3/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.880137 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50375 2023-08-07 12:47:16.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4176 2023-08-07 12:52:30.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24120 2023-08-07 12:44:11.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17698 2023-08-07 12:45:06.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-08-07 12:52:30.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.880643 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5613 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.881729 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28489 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4272 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.882362 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-08-06 15:38:03.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5775 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    30244 2023-08-07 03:36:58.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.883125 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7835 2023-08-07 12:59:08.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884127 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-07-29 16:46:35.000000 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884279 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884789 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.884947 pami-2023.8.6.3/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.887479 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15647 2023-08-07 12:59:48.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25202 2023-08-07 12:59:10.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24998 2023-08-07 12:59:10.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16367 2023-08-07 12:59:10.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33300 2023-08-07 12:59:56.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.888268 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.888848 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.889332 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.889901 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-28 05:36:37.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5380 2023-08-07 03:07:52.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24445 2023-08-07 03:35:37.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.890220 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.890683 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.891128 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.891299 pami-2023.8.6.3/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.893556 pami-2023.8.6.3/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.893874 pami-2023.8.6.3/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.894484 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-01 01:42:22.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.894624 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.895032 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.895185 pami-2023.8.6.3/PAMI/sequence/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequence/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.895281 pami-2023.8.6.3/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.896240 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18133 2023-08-02 09:17:46.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.896925 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.897034 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.898303 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-07-29 11:25:56.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-07-29 11:57:55.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-07-29 11:57:55.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.898752 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.899121 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.899257 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.901802 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.901992 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.903188 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.903529 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.904683 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-07-29 11:28:40.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-07-29 11:28:40.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.904978 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.905776 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.906005 pami-2023.8.6.3/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.906766 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-07-29 11:29:36.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.907081 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.907931 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.908093 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.908751 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-07-29 11:29:37.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-07 13:04:21.910051 pami-2023.8.6.3/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    60578 2023-08-02 07:28:07.000000 pami-2023.8.6.3/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-07 13:04:21.909680 pami-2023.8.6.3/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    61265 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15566 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-07 13:04:21.000000 pami-2023.8.6.3/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-07 13:04:21.910357 pami-2023.8.6.3/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1405 2023-08-07 13:04:00.000000 pami-2023.8.6.3/setup.py
```

### Comparing `pami-2023.8.6.2/LICENSE` & `pami-2023.8.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.8.6.3/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.8.6.3/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.8.6.3/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/correlatedPattern/__init__.py` & `pami-2023.8.6.3/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2023.8.6.3/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.8.6.3/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/coveragePattern/basic/CMine.py` & `pami-2023.8.6.3/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/coveragePattern/basic/CPPG.py` & `pami-2023.8.6.3/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/coveragePattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.8.6.3/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.8.6.3/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/sequentialDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/sequentialDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.8.6.3/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.8.6.3/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.8.6.3/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.8.6.3/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.8.6.3/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.8.6.3/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.8.6.3/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.8.6.3/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.8.6.3/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.8.6.3/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2023.8.6.3/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/plotPointOnMap.py` & `pami-2023.8.6.3/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.8.6.3/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.8.6.3/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.8.6.3/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/extras/topKPatterns.py` & `pami-2023.8.6.3/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.8.6.3/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.8.6.3/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.8.6.3/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.8.6.3/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.8.6.3/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.8.6.3/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.8.6.3/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.8.6.3/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.8.6.3/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.8.6.3/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.8.6.3/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.8.6.3/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.8.6.3/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2023.8.6.3/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.8.6.3/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #     from PAMI.periodicFrequentPattern.basic import PPPGrowth as alg
 #
-#     obj = alg.PPPGrowth(iFile, periodicSupport, period)
+#     obj = alg.PPPGrowth(iFile, minPS, period)
 #
 #     obj.startMine()
 #
 #     partialPeriodicPatterns = obj.getPatterns()
 #
 #     print("Total number of partial periodic Patterns:", len(partialPeriodicPatterns))
 #
@@ -50,15 +50,15 @@
 
 
 from PAMI.partialPeriodicPattern.basic import Gabstract as _abstract
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import sys as _sys
 
-_periodicSupport = float()
+_minPS = float()
 _period = float()
 _relativePS = float()
 _frequentList = {}
 _lno = int()
 
 class _Node(object):
     """
@@ -237,28 +237,28 @@
 
                 :param conditionalPatterns : conditional_patterns generated from condition_pattern method for
                                         respective node
                 :type conditionalPatterns : list
                 :param conditionalTimeStamps : represents the timestamps of conditional patterns of a node
                 :type conditionalTimeStamps : list
         """
-        global _periodicSupport, _period
+        global _minPS, _period
         patterns = []
         timeStamps = []
         data1 = {}
         for i in range(len(conditionalPatterns)):
             for j in conditionalPatterns[i]:
                 if j in data1:
                     data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
                     data1[j] = conditionalTimeStamps[i]
         updatedDictionary = {}
         for m in data1:
             updatedDictionary[m] = self._getPeriodicSupport(data1[m], temp + [m])
-        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _periodicSupport}
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _minPS}
         count = 0
         for p in conditionalPatterns:
             p1 = [v for v in p if v in updatedDictionary]
             trans = sorted(p1, key=lambda x: (updatedDictionary.get(x), -x), reverse=True)
             if len(trans) > 0:
                 patterns.append(trans)
                 timeStamps.append(conditionalTimeStamps[count])
@@ -267,19 +267,19 @@
 
     def _generatePatterns(self, prefix):
         """generates the patterns
 
                 :param prefix : forms the combination of items
                 :type prefix : list
                         """
-        global _periodicSupport, _relativePS
+        global _minPS, _relativePS
         for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
             pattern = prefix[:]
             pattern.append(i)
-            if self.info[i][0] >= _periodicSupport and self.info[i][1] >= _relativePS:
+            if self.info[i][0] >= _minPS and self.info[i][1] >= _relativePS:
                 yield pattern, self.info[i]
                 patterns, timeStamps, info = self._getConditionalPatterns(i, pattern)
                 conditionalTree = _Tree()
                 conditionalTree.info = info.copy()
                 for pat in range(len(patterns)):
                     conditionalTree._addTransaction(patterns[pat], timeStamps[pat])
                 if len(patterns) > 0:
@@ -301,19 +301,19 @@
 
     Parameters:
     ------------
         self.iFile : file
             Name of the Input file or path of the input file
         self. oFile : file
             Name of the output file or path of the output file
-        periodicSupport: float or int or str
-            The user can specify periodicSupport either in count or proportion of database size.
-            If the program detects the data type of periodicSupport is integer, then it treats periodicSupport is expressed in count.
+        minPS: float or int or str
+            The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: periodicSupport=10 will be treated as integer, while periodicSupport=10.0 will be treated as float
+            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
         period: float or int or str
             The user can specify period either in count or proportion of database size.
             If the program detects the data type of period is integer, then it treats period is expressed in count.
             Otherwise, it will be treated as float.
             Example: period=10 will be treated as integer, while period=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
@@ -367,29 +367,29 @@
             main program to mine the partial periodic patterns
 
     Executing the code on terminal:
     -----------------------------------
 
         Format:
         -----------
-          >>> python3 PPPGrowth.py <inputFile> <outputFile> <periodicSupport> <period>
+          >>> python3 PPPGrowth.py <inputFile> <outputFile> <minPS> <period>
 
         Examples:
         -----------
-          >>> python3 PPPGrowth.py sampleDB.txt patterns.txt 10.0 2.0   (periodicSupport and period will be considered in percentage of database transactions)
+          >>> python3 PPPGrowth.py sampleDB.txt patterns.txt 10.0 2.0   (minPS and period will be considered in percentage of database transactions)
 
           >>> python3 PPPGrowth.py sampleDB.txt patterns.txt 10 2     (periodicSupprot and period will be considered in count)
 
     Sample run of the importing code:
     --------------------------------------------
     .. code-block:: python
 
         from PAMI.periodicFrequentPattern.basic import PPPGrowth as alg
 
-        obj = alg.PPPGrowth(iFile, periodicSupport, period)
+        obj = alg.PPPGrowth(iFile, minPS, period)
 
         obj.startMine()
 
         partialPeriodicPatterns = obj.getPatterns()
 
         print("Total number of partial periodic Patterns:", len(partialPeriodicPatterns))
 
@@ -411,15 +411,15 @@
 
 
     Credits:
     ------------------
     The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
 
         """
-    _periodicSupport = float()
+    _minPS = float()
     _period = float()
     _relativePS = {}
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
@@ -481,27 +481,27 @@
                     calculates the support of each item in the dataset and assign the ranks to the items
                     by decreasing support and returns the frequent items list
 
                     """
         global _frequentList
         data = {}
         self._period = self._convert(self._period)
-        self._periodicSupport = self._convert(self._periodicSupport)
+        self._minPS = self._convert(self._minPS)
         self._relativePS = float(self._relativePS)
         for tr in self._Database:
             for i in range(1, len(tr)):
                 if tr[i] not in data:
                     data[tr[i]] = [0, int(tr[0]), 1]
                 else:
                     lp = int(tr[0]) - data[tr[i]][1]
                     if lp <= self._period:
                         data[tr[i]][0] += 1
                     data[tr[i]][1] = int(tr[0])
                     data[tr[i]][2] += 1
-        data = {k: [v[0], 1, v[2]] for k, v in data.items() if v[0] >= self._periodicSupport}
+        data = {k: [v[0], 1, v[2]] for k, v in data.items() if v[0] >= self._minPS}
         print(len(data))
         pfList = [k for k, v in sorted(data.items(), key=lambda x: x[1], reverse=True)]
         self._rank = dict([(index, item) for (item, index) in enumerate(pfList)])
         for x, y in self._rank.items():
             _frequentList[y] = data[x][2]
         return data, pfList
 
@@ -575,25 +575,25 @@
         return value
 
     def startMine(self):
         """
                    Main method where the patterns are mined by constructing tree.
 
                """
-        global _periodicSupport, _period, _relativePS, _lno
+        global _minPS, _period, _relativePS, _lno
         self._startTime = float()
         self._startTime = _abstract._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._periodicSupport is None:
+        if self._minPS is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
         generatedItems, pfList = self._partialPeriodicOneItem()
-        _periodicSupport, _period, _relativePS, _lno = self._periodicSupport, self._period, self._relativePS, len(self._Database)
-        # print(_periodicSupport, _period, _relativePS)
+        _minPS, _period, _relativePS, _lno = self._minPS, self._period, self._relativePS, len(self._Database)
+        # print(_minPS, _period, _relativePS)
         updatedTransactions = self._updateTransactions(generatedItems)
         for x, y in self._rank.items():
             self._rankdup[y] = x
         info = {self._rank[k]: v for k, v in generatedItems.items()}
         Tree = self._buildTree(updatedTransactions, info)
         patterns = Tree._generatePatterns([])
         self._finalPatterns = {}
@@ -729,15 +729,15 @@
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from PAMI.partialPeriodicPattern.basic import Gabstract as _abstract
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import sys as _sys
 
-_periodicSupport = float()
+_minPS = float()
 _period = float()
 _relativePS = float()
 _frequentList = {}
 _lno = int()
 
 class _Node(object):
     """
@@ -918,28 +918,28 @@
 
                 :param conditionalPatterns : conditional_patterns generated from condition_pattern method for
                                         respective node
                 :type conditionalPatterns : list
                 :param conditionalTimeStamps : represents the timestamps of conditional patterns of a node
                 :type conditionalTimeStamps : list
         """
-        global _periodicSupport, _period
+        global _minPS, _period
         patterns = []
         timeStamps = []
         data1 = {}
         for i in range(len(conditionalPatterns)):
             for j in conditionalPatterns[i]:
                 if j in data1:
                     data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
                     data1[j] = conditionalTimeStamps[i]
         updatedDictionary = {}
         for m in data1:
             updatedDictionary[m] = self._getPeriodicSupport(data1[m], temp + [m])
-        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _periodicSupport}
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _minPS}
         count = 0
         for p in conditionalPatterns:
             p1 = [v for v in p if v in updatedDictionary]
             trans = sorted(p1, key=lambda x: (updatedDictionary.get(x), -x), reverse=True)
             if len(trans) > 0:
                 patterns.append(trans)
                 timeStamps.append(conditionalTimeStamps[count])
@@ -948,19 +948,19 @@
 
     def _generatePatterns(self, prefix):
         """generates the patterns
 
                 :param prefix : forms the combination of items
                 :type prefix : list
                         """
-        global _periodicSupport, _relativePS
+        global _minPS, _relativePS
         for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
             pattern = prefix[:]
             pattern.append(i)
-            if self.info[i][0] >= _periodicSupport and self.info[i][1] >= _relativePS:
+            if self.info[i][0] >= _minPS and self.info[i][1] >= _relativePS:
                 yield pattern, self.info[i]
                 patterns, timeStamps, info = self._getConditionalPatterns(i, pattern)
                 conditionalTree = _Tree()
                 conditionalTree.info = info.copy()
                 for pat in range(len(patterns)):
                     conditionalTree._addTransaction(patterns[pat], timeStamps[pat])
                 if len(patterns) > 0:
@@ -977,19 +977,19 @@
 
     Parameters:
     ----------
         self.iFile : file
             Name of the Input file or path of the input file
         self. oFile : file
             Name of the output file or path of the output file
-        periodicSupport: float or int or str
-            The user can specify periodicSupport either in count or proportion of database size.
-            If the program detects the data type of periodicSupport is integer, then it treats periodicSupport is expressed in count.
+        minPS: float or int or str
+            The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: periodicSupport=10 will be treated as integer, while periodicSupport=10.0 will be treated as float
+            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
         period: float or int or str
             The user can specify period either in count or proportion of database size.
             If the program detects the data type of period is integer, then it treats period is expressed in count.
             Otherwise, it will be treated as float.
             Example: period=10 will be treated as integer, while period=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
@@ -1038,25 +1038,25 @@
             updates the transactions by removing the aperiodic items and sort the transactions with items
             by decreasing support
         buildTree()
             constrcuts the main tree by setting the root node as null
         startMine()
             main program to mine the partial periodic patterns
 
-        Format: python3 PPPGrowth.py <inputFile> <outputFile> <periodicSupport> <period>
+        Format: python3 PPPGrowth.py <inputFile> <outputFile> <minPS> <period>
 
-        Examples: python3 PPPGrowth.py sampleDB.txt patterns.txt 10.0 2.0   (periodicSupport and period will be considered in percentage of database transactions)
+        Examples: python3 PPPGrowth.py sampleDB.txt patterns.txt 10.0 2.0   (minPS and period will be considered in percentage of database transactions)
 
-                  python3 PPPGrowth.py sampleDB.txt patterns.txt 10 2     (periodicSupprot and period will be considered in count)
+                  python3 PPPGrowth.py sampleDB.txt patterns.txt 10 2     (periodic Support and period will be considered in count)
 
         Sample run of the importing code:
         -----------
         from PAMI.periodicFrequentPattern.basic import PPPGrowth as alg
 
-        obj = alg.PPPGrowth(iFile, periodicSupport, period)
+        obj = alg.PPPGrowth(iFile, minPS, period)
 
         obj.startMine()
 
         partialPeriodicPatterns = obj.getPatterns()
 
         print("Total number of partial periodic Patterns:", len(partialPeriodicPatterns))
 
@@ -1078,15 +1078,15 @@
 
 
         Credits:
         -------
         The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
 
         """
-    _periodicSupport = float()
+    _minPS = float()
     _period = float()
     _relativePS = {}
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
@@ -1148,29 +1148,29 @@
                     calculates the support of each item in the dataset and assign the ranks to the items
                     by decreasing support and returns the frequent items list
 
                     """
         global _frequentList
         data = {}
         self._period = self._convert(self._period)
-        self._periodicSupport = self._convert(self._periodicSupport)
+        self._minPS = self._convert(self._minPS)
         self._relativePS = self._convert(self._relativePS)
         for tr in self._Database:
             for i in range(1, len(tr)):
                 if tr[i] not in data:
                     data[tr[i]] = [0, int(tr[0]), 1]
                 else:
                     lp = int(tr[0]) - data[tr[i]][1]
                     if lp <= self._period:
                         data[tr[i]][0] += 1
                     data[tr[i]][1] = int(tr[0])
                     data[tr[i]][2] += 1
         for x, y in data.items():
             data[x][0] = data[x][0]/abs(self._lno - 1)
-        data = {k: [v[0], 1, v[2]] for k, v in data.items() if v[0] >= self._periodicSupport}
+        data = {k: [v[0], 1, v[2]] for k, v in data.items() if v[0] >= self._minPS}
         #print(data)
         pfList = [k for k, v in sorted(data.items(), key=lambda x: x[1], reverse=True)]
         self._rank = dict([(index, item) for (item, index) in enumerate(pfList)])
         for x, y in self._rank.items():
             _frequentList[y] = data[x][2]
         return data, pfList
 
@@ -1244,24 +1244,24 @@
         return value
 
     def startMine(self):
         """
                    Main method where the patterns are mined by constructing tree.
 
                """
-        global _periodicSupport, _period, _relativePS, _lno
+        global _minPS, _period, _relativePS, _lno
         self._startTime = _abstract._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._periodicSupport is None:
+        if self._minPS is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
         generatedItems, pfList = self._partialPeriodicOneItem()
-        _periodicSupport, _period, _relativePS, _lno = self._periodicSupport, self._period, self._relativePS, len(self._Database)
-        print(_periodicSupport, _period, _relativePS)
+        _minPS, _period, _relativePS, _lno = self._minPS, self._period, self._relativePS, len(self._Database)
+        print(_minPS, _period, _relativePS)
         updatedTransactions = self._updateTransactions(generatedItems)
         for x, y in self._rank.items():
             self._rankdup[y] = x
         info = {self._rank[k]: v for k, v in generatedItems.items()}
         Tree = self._buildTree(updatedTransactions, info)
         patterns = Tree._generatePatterns([])
         self._finalPatterns = {}
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
         ...
 
         Attributes
         ----------
         iFile : str
             Input file name or path of the input file
-        minSup: float
-            UserSpecified minimum support value. It has to be given in terms of count of total number of transactions
+        minPS: float
+            UserSpecified minimum period-support value. It has to be given in terms of count of total number of transactions
             in the input database/file
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
@@ -53,27 +53,26 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, periodicSupport, period, relativePS, sep='\t'):
+    def __init__(self, iFile, periodicSupport, period, sep='\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param minSup: UserSpecified minimum support value. It has to be given in terms of count of total number of
+        :param minPS: UserSpecified minimum period-support value. It has to be given in terms of count of total number of
         transactions in the input database/file
-        :type minSup: float
+        :type minPS: float
         """
 
         self._iFile = iFile
         self._periodicSupport = periodicSupport
         self._period = period
-        self._relativePS = relativePS
         self._sep = sep
         self._finalPatterns = {}
         self._oFile = str()
         self._startTime = float()
         self._endTime = float()
         self._memoryUSS = float()
         self._memoryRSS = float()
@@ -118,7 +117,13 @@
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
+
+    @_abstractmethod
+    def printResults(self):
+        """ To print all the results of execution"""
+
+        pass
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
 #         from PAMI.periodicFrequentPattern.basic import PPPGrowth as alg
 #
-#         obj = alg.PPPGrowth(iFile, periodicSupport, period)
+#         obj = alg.PPPGrowth(iFile, minPS, period)
 #
 #         obj.startMine()
 #
 #         partialPeriodicPatterns = obj.getPatterns()
 #
 #         print("Total number of partial periodic Patterns:", len(partialPeriodicPatterns))
 #
@@ -54,15 +54,15 @@
 
 
 from PAMI.partialPeriodicPattern.basic import abstract as _abstract
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import sys as _sys
 
-_periodicSupport = float()
+_minPS = float()
 _period = float()
 _lno = int()
 
 class _Node(object):
     """
         A class used to represent the node of frequentPatternTree
         ...
@@ -234,28 +234,28 @@
 
                 :param conditionalPatterns : conditional_patterns generated from condition_pattern method for
                                         respective node
                 :type conditionalPatterns : list
                 :param conditionalTimeStamps : represents the timestamps of conditional patterns of a node
                 :type conditionalTimeStamps : list
         """
-        global _periodicSupport, _period
+        global _minPS, _period
         patterns = []
         timeStamps = []
         data1 = {}
         for i in range(len(conditionalPatterns)):
             for j in conditionalPatterns[i]:
                 if j in data1:
                     data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
                     data1[j] = conditionalTimeStamps[i]
         updatedDictionary = {}
         for m in data1:
             updatedDictionary[m] = self._getPeriodicSupport(data1[m])
-        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v >= _periodicSupport}
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v >= _minPS}
         count = 0
         for p in conditionalPatterns:
             p1 = [v for v in p if v in updatedDictionary]
             trans = sorted(p1, key=lambda x: (updatedDictionary.get(x), -x), reverse=True)
             if len(trans) > 0:
                 patterns.append(trans)
                 timeStamps.append(conditionalTimeStamps[count])
@@ -296,19 +296,19 @@
 
     Parameters:
     ----------
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
-        periodicSupport: float or int or str
-            The user can specify periodicSupport either in count or proportion of database size.
-            If the program detects the data type of periodicSupport is integer, then it treats periodicSupport is expressed in count.
+        minPS: float or int or str
+            The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: periodicSupport=10 will be treated as integer, while periodicSupport=10.0 will be treated as float
+            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
         period: float or int or str
             The user can specify period either in count or proportion of database size.
             If the program detects the data type of period is integer, then it treats period is expressed in count.
             Otherwise, it will be treated as float.
             Example: period=10 will be treated as integer, while period=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
@@ -361,29 +361,29 @@
         startMine()
             main program to mine the partial periodic patterns
 
     Executing the code on terminal:
     -----------------------------------
         Format:
         --------
-           >>> python3 PPPGrowth.py <inputFile> <outputFile> <periodicSupport> <period>
+           >>> python3 PPPGrowth.py <inputFile> <outputFile> <minPS> <period>
     
         Examples:
         --------
-           >>> python3 PPPGrowth.py sampleDB.txt patterns.txt 10.0 2.0   (periodicSupport and period will be considered in percentage of database transactions)
+           >>> python3 PPPGrowth.py sampleDB.txt patterns.txt 10.0 2.0   (minPS and period will be considered in percentage of database transactions)
 
            >>> python3 PPPGrowth.py sampleDB.txt patterns.txt 10 2     (periodicSupprot and period will be considered in count)
 
     Sample run of the importing code:
     -----------------------------------------
     .. code-block:: python
 
         from PAMI.periodicFrequentPattern.basic import PPPGrowth as alg
 
-        obj = alg.PPPGrowth(iFile, periodicSupport, period)
+        obj = alg.PPPGrowth(iFile, minPS, period)
 
         obj.startMine()
 
         partialPeriodicPatterns = obj.getPatterns()
 
         print("Total number of partial periodic Patterns:", len(partialPeriodicPatterns))
 
@@ -405,15 +405,15 @@
 
 
     Credits:
     -----------------
     The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
 
     """
-    _periodicSupport = float()
+    _minPS = float()
     _period = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
@@ -471,26 +471,26 @@
         """
                     calculates the support of each item in the dataset and assign the ranks to the items
                     by decreasing support and returns the frequent items list
 
                     """
         data = {}
         self._period = self._convert(self._period)
-        self._periodicSupport = self._convert(self._periodicSupport)
+        self._minPS = self._convert(self._minPS)
         for tr in self._Database:
             for i in range(1, len(tr)):
                 if tr[i] not in data:
                     data[tr[i]] = [0, int(tr[0]), 1]
                 else:
                     lp = int(tr[0]) - data[tr[i]][1]
                     if lp <= self._period:
                         data[tr[i]][0] += 1
                     data[tr[i]][1] = int(tr[0])
                     data[tr[i]][2] += 1
-        data = {k: v[0] for k, v in data.items() if v[0] >= self._periodicSupport}
+        data = {k: v[0] for k, v in data.items() if v[0] >= self._minPS}
         pfList = [k for k, v in sorted(data.items(), key=lambda x: x[1], reverse=True)]
         self._rank = dict([(index, item) for (item, index) in enumerate(pfList)])
         return data, pfList
 
     def _updateTransactions(self, dict1):
         """remove the items which are not frequent from transactions and updates the transactions with rank of items
 
@@ -558,23 +558,23 @@
         return value
 
     def startMine(self):
         """
                    Main method where the patterns are mined by constructing tree.
 
                """
-        global _periodicSupport, _period, _lno
+        global _minPS, _period, _lno
         self._startTime = _abstract._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._periodicSupport is None:
+        if self._minPS is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
         generatedItems, pfList = self._partialPeriodicOneItem()
-        _periodicSupport, _period, _lno = self._periodicSupport, self._period, len(self._Database)
+        _minPS, _period, _lno = self._minPS, self._period, len(self._Database)
         updatedTransactions = self._updateTransactions(generatedItems)
         for x, y in self._rank.items():
             self._rankdup[y] = x
         info = {self._rank[k]: v for k, v in generatedItems.items()}
         Tree = self._buildTree(updatedTransactions, info)
         patterns = Tree._generatePatterns([])
         self._finalPatterns = {}
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 
+
+
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
+
 #
-#     from PAMI.periodicFrequentPattern.basic import PPP_ECLAT as alg
+#     import PAMI.partialPeriodicPattern.topk.Topk_PPPGrowth as alg
 #
-#     obj = alg.PPP_ECLAT(iFile, periodicSupport, period)
+#     obj = alg.Topk_PPPGrowth(iFile, k, periodicity)
 #
 #     obj.startMine()
 #
-#     Patterns = obj.getPatterns()
+#     partialPeriodicPatterns = obj.getPatterns()
 #
-#     print("Total number of partial periodic patterns:", len(Patterns))
+#     print("Total number of top partial periodic Patterns:", len(partialPeriodicPatterns))
 #
 #     obj.save(oFile)
 #
-#     Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -45,378 +49,379 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-
-from PAMI.partialPeriodicPattern.basic import abstract as _ab
+from PAMI.partialPeriodicPattern.topk import abstract as _abstract
+import validators as _validators
+from urllib.request import urlopen as _urlopen
+import sys as _sys
 
 
-class PPP_ECLAT(_ab._partialPeriodicPatterns):
+class Topk_PPPGrowth(_abstract.partialPeriodicPatterns):
     """
-    Descripition:
-    ----------------------
-        3pEclat is the fundamental approach to mine the partial periodic frequent patterns.
+    Description:
+    -------------
+        Top - K is and algorithm to discover top partial periodic patterns in a temporal  database.
 
     Reference:
-    -----------
-        To be published
+    ----------
 
 
-    Parameters:
-    ----------
-        self.iFile : file
-            Name of the Input file or path of the input file
-        self. oFile : file
-            Name of the output file or path of the output file
-        periodicSupport: float or int or str
-            The user can specify periodicSupport either in count or proportion of database size.
-            If the program detects the data type of periodicSupport is integer, then it treats periodicSupport is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: periodicSupport=10 will be treated as integer, while periodicSupport=10.0 will be treated as float
-        period: float or int or str
-            The user can specify period either in count or proportion of database size.
-            If the program detects the data type of period is integer, then it treats period is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: period=10 will be treated as integer, while period=10.0 will be treated as float
-        sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-            However, the users can override their default separator.
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
-        Database : list
-            To store the transactions of a database in list
-        mapSupport : Dictionary
-            To maintain the information of item and their frequency
-        lno : int
-            it represents the total no of transactions
-        tree : class
-            it represents the Tree class
-        finalPatterns : dict
-            it represents to store the patterns
-        tidList : dict
-            stores the timestamps of an item
+    Attributes:
+    ------------
+            iFile : str
+                Input file name or path of the input file
+            k: int
+                User specified count of top partial periodic patterns
+            sep : str
+                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+                However, the users can override their default separator.
+            oFile : str
+                Name of the output file or the path of the output file
+            startTime:float
+                To record the start time of the mining process
+            endTime:float
+                To record the completion time of the mining process
+            finalPatterns: dict
+                Storing the complete set of patterns in a dictionary variable
+            memoryUSS : float
+                To store the total amount of USS memory consumed by the program
+            memoryRSS : float
+                To store the total amount of RSS memory consumed by the program
 
     Methods:
-    -------
-        startMine()
-            Mining process will start from here
-        getPatterns()
-            Complete set of patterns will be retrieved with this function
-        save(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
-        getPatternsAsDataFrame()
-            Complete set of frequent patterns will be loaded in to a dataframe
-        getMemoryUSS()
-            Total amount of USS memory consumed by the mining process will be retrieved from this function
-        getMemoryRSS()
-            Total amount of RSS memory consumed by the mining process will be retrieved from this function
-        getRuntime()
-            Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingOneitemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent
-        getPeriodAndSupport()
-            Calculates the support and period for a list of timestamps.
-        Generation()
-            Used to implement prefix class equivalence method to generate the periodic patterns recursively
+    --------
+            startMine()
+                Mining process will start from here
+            getPatterns()
+                Complete set of patterns will be retrieved with this function
+            save(oFile)
+                Complete set of frequent patterns will be loaded in to a output file
+            getPatternsAsDataFrame()
+                Complete set of frequent patterns will be loaded in to a dataframe
+            getMemoryUSS()
+                Total amount of USS memory consumed by the mining process will be retrieved from this function
+            getMemoryRSS()
+                Total amount of RSS memory consumed by the mining process will be retrieved from this function
+            getRuntime()
+                Total amount of runtime taken by the mining process will be retrieved from this function
+            creatingItemSets()
+                Scans the dataset or dataframes and stores in list format
+            frequentOneItem()
+                Generates one frequent patterns
+            eclatGeneration(candidateList)
+                It will generate the combinations of frequent items
+            generateFrequentPatterns(tidList)
+                It will generate the combinations of frequent items from a list of items
 
     Executing the code on terminal:
-    ----------------------------------------
+    -------------------------------
 
         Format:
-        -----------
-           >>> python3 PPP_ECLAT.py <inputFile> <outputFile> <periodicSupport> <period>
+        ------
+            >>> python3 FAE.py <inputFile> <outputFile> <k> <periodicity>
 
         Examples:
-        -----------
-           >>> python3 PPP_ECLAT.py sampleDB.txt patterns.txt 0.3 0.4   (periodicSupport and period will be considered in percentage of database transactions)
-
-           >>> python3 threePEeclat.py sampleDB.txt patterns.txt 3 4     (periodicSupport and period will be considered in support count or frequency)
+        ---------
+            >>> python3 FAE.py sampleDB.txt patterns.txt 10 3
 
 
-    Sample run of importing the code:
-    -----------------------------------------
+    Sample run of the importing code:
+    ---------------------------------
     .. code-block:: python
 
-        from PAMI.periodicFrequentPattern.basic import PPP_ECLAT as alg
+            import PAMI.partialPeriodicPattern.topk.Topk_PPPGrowth as alg
 
-        obj = alg.PPP_ECLAT(iFile, periodicSupport,period)
+            obj = alg.Topk_PPPGrowth(iFile, k, periodicity)
 
-        obj.startMine()
+            obj.startMine()
 
-        Patterns = obj.getPatterns()
+            partialPeriodicPatterns = obj.getPatterns()
 
-        print("Total number of partial periodic patterns:", len(Patterns))
+            print("Total number of top partial periodic Patterns:", len(partialPeriodicPatterns))
 
-        obj.save(oFile)
+            obj.save(oFile)
 
-        Df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-        memUSS = obj.getMemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
-        print("Total Memory in USS:", memUSS)
+            print("Total Memory in USS:", memUSS)
 
-        memRSS = obj.getMemoryRSS()
+            memRSS = obj.getMemoryRSS()
 
-        print("Total Memory in RSS", memRSS)
+            print("Total Memory in RSS", memRSS)
 
-        run = obj.getRuntime()
+            run = obj.getRuntime()
 
-        print("Total ExecutionTime in seconds:", run)
+            print("Total ExecutionTime in seconds:", run)
 
     Credits:
-    ------------------
-
-    The complete program was written by P.RaviKumar  under the supervision of Professor Rage Uday Kiran.\n
-
+    ---------
+            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
+    """
 
-        """
     _startTime = float()
     _endTime = float()
+    _k = int()
+    _periodicity = " "
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
-    _mapSupport = {}
-    _itemsetCount = 0
-    _writer = None
-    _periodicSupport = str()
-    _period = str()
-    _tidList = {}
-    _lno = 0
     _Database = []
+    _tidList = {}
+    _lno = int()
+    _minimum = int()
+    _mapSupport = {}
 
-    def _convert(self, value):
-        """
-        To convert the given user specified value
-
-        :param value: user specified value
-
-        :return: converted value
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
-
-    def _getPeriodicSupport(self, timeStamps):
+    def _creatingItemSets(self):
         """
-            calculates the support and periodicity with list of timestamps
+            Storing the complete transactions of the database/input file in a database variable
 
-            :param timeStamps : timestamps of a pattern
-
-            :type timeStamps : list
         """
-        timeStamps.sort()
-        per = 0
-        for i in range(len(timeStamps) - 1):
-            j = i + 1
-            if abs(timeStamps[j] - timeStamps[i]) <= self._period:
-                per += 1
-        return per
-
-    def _creatingItemSets(self):
         self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            data, tids = [], []
+        if isinstance(self._iFile, _abstract._pd.DataFrame):
+            timeStamp, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'TS' in i:
-                tids = self._iFile['TS'].tolist()
+                timeStamp = self._iFile['TS'].tolist()
             if 'Transactions' in i:
                 data = self._iFile['Transactions'].tolist()
             for i in range(len(data)):
-                tr = [tids[i][0]]
+                tr = [timeStamp[i]]
                 tr = tr + data[i]
                 self._Database.append(tr)
             self._lno = len(self._Database)
-
+            # print(self.Database)
         if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
+            if _validators.url(self._iFile):
+                data = _urlopen(self._iFile)
                 for line in data:
-                    line.strip()
                     self._lno += 1
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
                     self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             self._lno += 1
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _creatingOneitemSets(self):
+    def _convert(self, value):
         """
-           Scans the Temporal database / Input file and stores the 1-length partial-periodic patterns.
+        To convert the given user specified value
+        :param value: user specified value
+        :return: converted value
         """
-        plist = []
-        self._tidList = {}
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+
+    def _frequentOneItem(self):
+        """
+        Generating one frequent patterns
+        """
+
         self._mapSupport = {}
-        self._period = self._convert(self._period)
+        self._tidList = {}
+        self._periodicity = self._convert(self._periodicity)
+        self._k = int(self._convert(self._k))
         for line in self._Database:
-            s = line
-            n = int(s[0])
-            for i in range(1, len(s)):
-                si = s[i]
+            n = int(line[0])
+            for i in range(1, len(line)):
+                si = line[i]
                 if self._mapSupport.get(si) is None:
-                    self._mapSupport[si] = [0, n]
+                    self._mapSupport[si] = [1, 0, n]
                     self._tidList[si] = [n]
                 else:
-                    lp = n - self._mapSupport[si][1]
-                    if lp <= self._period:
-                        self._mapSupport[si][0] += 1
-                    self._mapSupport[si][1] = n
+                    self._mapSupport[si][0] += 1
+                    period = abs(n - self._mapSupport[si][2])
+                    if period <= self._periodicity:
+                        self._mapSupport[si][1] += 1
+                    self._mapSupport[si][2] = n
                     self._tidList[si].append(n)
-        self._periodicSupport = self._convert(self._periodicSupport)
-        self._mapSupport = {k: v[0] for k, v in self._mapSupport.items() if v[0] >= self._periodicSupport}
-        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        for x, y in self._mapSupport.items():
+            period = abs(self._lno - self._mapSupport[x][2])
+            if period <= self._periodicity:
+                self._mapSupport[x][1] += 1
+        self._mapSupport = {k: v[1] for k, v in self._mapSupport.items()}
+        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[0], reverse=True)]
+        self._finalPatterns = {}
+        for i in plist:
+            if self._mapSupport[i] == 0:
+                continue
+            if len(self._finalPatterns) >= self._k:
+                break
+            else:
+                self._finalPatterns[i] = self._mapSupport[i]
+        print(len(self._finalPatterns),  self._k, self._periodicity)
+        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+        plist = list(self._finalPatterns.keys())
         return plist
 
-    def _save(self, prefix, suffix, tidSetX):
+    def _getSupportAndPeriod(self, timeStamps):
+        """To calculate the periodicity and support
+        :param timeStamps: Timestamps of an item set
+        :return: support, periodicity
         """
-            saves the patterns that satisfy the partial periodic property.
 
-            :param prefix: the prefix of a pattern
+        timeStamps.sort()
+        sup = 0
+        for j in range(len(timeStamps) - 1):
+            per = abs(timeStamps[j + 1] - timeStamps[j])
+            if per <= self._periodicity:
+                sup += 1
+        return sup
 
-            :type prefix: list
+    def _save(self, prefix, suffix, tidSetI):
+        """Saves the patterns that satisfy the periodic frequent property.
 
-            :param suffix : the suffix of a patterns
+            :param prefix: the prefix of a pattern
 
-            :type suffix : list
+            :type prefix: list
 
-            :param tidSetX : the timestamp of a patterns
+            :param suffix: the suffix of a patterns
 
-            :type tidSetX : list
+            :type suffix: list
 
+            :param tidSetI: the timestamp of a patterns
 
+            :type tidSetI: list
         """
+
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = self._getPeriodicSupport(tidSetX)
-        if val >= self._periodicSupport:
-            sample = str()
-            for i in prefix:
-                sample = sample + i + "\t"
-            self._finalPatterns[sample] = val
+        val = self._getSupportAndPeriod(tidSetI)
+        sample = str()
+        for i in prefix:
+            sample = sample + i + "\t"
+        if len(self._finalPatterns) < self._k:
+            if val >= self._minimum:
+                self._finalPatterns[sample] = val
+                self._finalPatterns = {k: v for k, v in
+                                       sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
+                self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+        else:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
+                if val > y:
+                    del self._finalPatterns[x]
+                    self._finalPatterns[x] = y
+                    self._finalPatterns = {k: v for k, v in
+                                           sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
+                    self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+                    return
 
     def _Generation(self, prefix, itemSets, tidSets):
-        """
-            Generates the patterns following Equivalence-class methods
-
-            :param prefix :  main equivalence prefix
-
-            :type prefix : partial-periodic item or pattern
+        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
-            :param itemSets : patterns which are items combined with prefix and satisfying the periodicity
-                            and partial property with their timestamps
+            :param prefix:  main equivalence prefix
 
-            :type itemSets : list
+            :type prefix: periodic-frequent item or pattern
 
-            :param tidSets : timestamps of the items in the argument itemSets
+            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
+                            and frequent with their timestamps
 
-            :type tidSets : list
+            :type itemSets: list
 
+            :param tidSets: timestamps of the items in the argument itemSets
 
-                    """
+            :type tidSets: list
+        """
         if len(itemSets) == 1:
             i = itemSets[0]
-            tidi = tidSets[0]
-            self._save(prefix, [i], tidi)
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
             return
         for i in range(len(itemSets)):
             itemI = itemSets[i]
             if itemI is None:
                 continue
-            tidSetX = tidSets[i]
+            tidSetI = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
             for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
-                y = list(set(tidSetX).intersection(tidSetJ))
-                val = self._getPeriodicSupport(y)
-                if val >= self._periodicSupport:
+                y = list(set(tidSetI).intersection(tidSetJ))
+                val = self._getSupportAndPeriod(y)
+                if val >= self._minimum:
                     classItemSets.append(itemJ)
                     classTidSets.append(y)
-            newprefix = list(set(itemSetX)) + prefix
-            self._Generation(newprefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetX)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
 
     def startMine(self):
         """
-            Main program start with extracting the periodic frequent items from the database and
-            performs prefix equivalence to form the combinations and generates partial-periodic patterns.
+            Main function of the program
 
         """
-        self._startTime = _ab._time.time()
+        self._startTime = _abstract._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._k is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        plist = self._creatingOneitemSets()
-        self._finalPatterns = {}
+        plist = self._frequentOneItem()
         for i in range(len(plist)):
             itemI = plist[i]
-            tidSetX = self._tidList[itemI]
+            tidSetI = self._tidList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i + 1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetX).intersection(tidSetJ))
-                val = self._getPeriodicSupport(y1)
-                if val >= self._periodicSupport:
+                y1 = list(set(tidSetI).intersection(tidSetJ))
+                val = self._getSupportAndPeriod(y1)
+                if val >= self._minimum:
                     itemSets.append(itemJ)
                     tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-            self._save(None, itemSetX, tidSetX)
-        print("Partial Periodic Patterns were generated successfully using 3PEclat algorithm")
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
+        print("TopK partial periodic patterns were generated successfully")
+        self._endTime = _abstract._time.time()
+        process = _abstract._psutil.Process(_abstract._os.getpid())
         self._memoryUSS = float()
+        self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-        :return: returning USS memory consumed by the mining process
+                    :return: returning USS memory consumed by the mining process
 
-        :rtype: float
+                    :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
@@ -424,16 +429,15 @@
 
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
 
         :rtype: float
         """
 
         return self._endTime - self._startTime
@@ -442,66 +446,58 @@
         """Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
 
         :rtype: pd.DataFrame
         """
 
-        dataframe = {}
+        dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicSupport'])
-        return dataframe
+            dataFrame = _abstract._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        return dataFrame
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of Partial Periodic Patterns:", len(self.getPatterns()))
+        print("Top K Partial Periodic Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
-        if len(_ab._sys.argv) == 6:
-            _ap = PPP_ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
-        if len(_ab._sys.argv) == 5:
-            _ap = PPP_ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+    if len(_sys.argv) == 5 or len(_sys.argv) == 6:
+        if len(_sys.argv) == 6:
+            _ap = Topk_PPPGrowth(_sys.argv[1], _sys.argv[3], _sys.argv[4], _sys.argv[5])
+        if len(_sys.argv) == 5:
+            _ap = Topk_PPPGrowth(_sys.argv[1], _sys.argv[3], _sys.argv[4])
         _ap.startMine()
-        print("Total number of Partial Periodic Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
+        print("Top K Partial Periodic Patterns:", len(_ap.getPatterns()))
+        _ap.save(_sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        for i in [100, 200, 300, 400, 500]:
-            _ap = PPP_ECLAT('/Users/Likhitha/Downloads/temporal_T10I4D100K.csv', i, 5000, '\t')
-            _ap.startMine()
-            print("Total number of Maximal Partial Periodic Patterns:", len(_ap.getPatterns()))
-            _ap.save('/Users/Likhitha/Downloads/output.txt')
-            print("Total Memory in USS:", _ap.getMemoryUSS())
-            print("Total Memory in RSS", _ap.getMemoryRSS())
-            print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
         ...
 
         Attributes
         ----------
         iFile : str
             Input file name or path of the input file
-        minSup: float
-            UserSpecified minimum support value. It has to be given in terms of count of total number of transactions
+        minPS: float
+            UserSpecified minimum period-support value. It has to be given in terms of count of total number of transactions
             in the input database/file
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
@@ -53,25 +53,25 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, periodicSupport, period, sep='\t'):
+    def __init__(self, iFile, minPS, period, sep='\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param minSup: UserSpecified minimum support value. It has to be given in terms of count of total number of
+        :param minPS: UserSpecified minimum period-support value. It has to be given in terms of count of total number of
         transactions in the input database/file
-        :type minSup: float
+        :type minPS: float
         """
 
         self._iFile = iFile
-        self._periodicSupport = periodicSupport
+        self._minPS = minPS
         self._period = period
         self._sep = sep
         self._finalPatterns = {}
         self._oFile = str()
         self._startTime = float()
         self._endTime = float()
         self._memoryUSS = float()
@@ -80,16 +80,16 @@
     '''@abstractmethod
     def iFile(self):
         """Variable to store the input file path/file name"""
 
         pass
 
     @abstractmethod
-    def periodicSupport(self):
-        """Variable to store the user-specified minimum support value"""
+    def minPS(self):
+        """Variable to store the user-specified minimum period-support value"""
 
         pass
 
     def period(self):
         """Variable to store the user specified maximum periodicity value"""
 
         pass
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
     employ in PAMI
         ...
     Attributes:
     ----------
         iFile : str
             Input file name or path of the input file
-        minSup: float
-            UserSpecified minimum support value. It has to be given in terms of count of total number of transactions
+        minPS: float
+            UserSpecified minimum period-support value. It has to be given in terms of count of total number of transactions
             in the input database/file
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
@@ -53,17 +53,17 @@
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
     def __init__(self, iFile, periodicSupport, period, sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param minSup: UserSpecified minimum support value. It has to be given in terms of count of total number of
+        :param minPS: UserSpecified minimum period-support value. It has to be given in terms of count of total number of
         transactions in the input database/file
-        :type minSup: float
+        :type minPS: float
         """
 
         self._iFile = iFile
         self._periodicSupport = periodicSupport
         self._period = period
         self._sep = sep
         self._finalPatterns = {}
@@ -77,15 +77,15 @@
     def iFile(self):
         """Variable to store the input file path/file name"""
 
         pass
 
     @abstractmethod
     def periodicSupport(self):
-        """Variable to store the user-specified minimum support value"""
+        """Variable to store the user-specified minimum period-support value"""
 
         pass
 
     @abstractmethod
     def period(self):
         """Variable to store the user specified maximum periodicity value"""
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
         periodicSupport : int/float
-            The user given minimum support
+            The user given minimum period-support
         period : int/float
             The user given maximum period
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-from abc import ABC as _ABC, abstractmethod as _abstractmethod
+from abc import ABC as _ABC , abstractmethod as _abstractmethod
 import time as _time
-import math as _math
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _combinations
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 
 
-class _partialPeriodicPatterns(_ABC):
+
+class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
     employ in PAMI
 
         ...
 
-        Attributes
-        ----------
+    Attributes:
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: float
             UserSpecified minimum support value. It has to be given in terms of count of total number of transactions
             in the input database/file
+        minRS: float
+            UserSpecified minimum relative support value. calculated as
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-        Methods
-        -------
+    Methods:
+    -------
         startMine()
             Mining process will start from here
         getFrequentPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -53,33 +55,32 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, periodicSupport, period, sep='\t'):
+    def __init__(self, iFile, minSup, minRatio, sep='\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minSup: UserSpecified minimum support value. It has to be given in terms of count of total number of
         transactions in the input database/file
-        :type minSup: float
+        :type minSup: str
         """
 
         self._iFile = iFile
-        self._periodicSupport = periodicSupport
-        self._period = period
+        self._minSup = minSup
+        self._minRatio = minRatio
         self._sep = sep
         self._finalPatterns = {}
-        self._oFile = str()
         self._startTime = float()
         self._endTime = float()
-        self._memoryUSS = float()
         self._memoryRSS = float()
+        self._memoryUSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -120,10 +121,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print the results of execution."""
 
-        pass
+        pass
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/__init__.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     def __init__(self, iFile, minPS, period, numWorkers=1,sep='\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minPS: UserSpecified minimum period-support value. It has to be given in terms of count of total number of
         transactions in the input database/file
-        :type minSup: float
+        :type minPS: float
         """
 
         self._iFile = iFile
         self._minPS = minPS
         self._period = period
         self._numWorkers = numWorkers
         self._sep = sep
@@ -82,15 +82,15 @@
     def iFile(self):
         """Variable to store the input file path/file name"""
 
         pass
 
     @abstractmethod
     def minPS(self):
-        """Variable to store the user-specified minimum support value"""
+        """Variable to store the user-specified minimum period-support value"""
 
         pass
         
     @abstractmethod
     def period(self):
         """Variable to store the user specified maximum periodicity value"""
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,18 @@
         employ in PAMI
 
     Attributes:
     ----------
         iFile : str
             Input file name or path of the input file
         k: int or float or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
         periodicity: int or float or str
             The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
@@ -80,18 +80,18 @@
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
     def __init__(self, iFile, k, periodicity, sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param k: The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats k is expressed in count.
+        :param k: The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats k is expressed in count.
             Otherwise, it will be treated as float.
-            Example: k=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: k=10 will be treated as integer, while minPS=10.0 will be treated as float
         :type k: int or float or str
         :param periodicity: The user can specify periodicity either in count or proportion of database size.
             If the program detects the data type of periodicity is integer, then it treats periodicity is expressed in count.
             Otherwise, it will be treated as float.
             Example: periodicity=10 will be treated as integer, while periodicity=10.0 will be treated as float
         :type periodicity: int or float or str
         :param sep: separator used in user specified input file
@@ -112,16 +112,16 @@
     '''@abstractmethod
     def _iFile(self):
         """Variable to store the input file path/file name"""
 
         pass
 
     @abstractmethod
-    def _minSup(self):
-        """Variable to store the user-specified minimum support value"""
+    def _minPS(self):
+        """Variable to store the user-specified minimum period-support value"""
 
         pass
 
     @abstractmethod
     def _maxPer(self):
         """Variable to store the user specified maximum periodicity value"""
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 
-
-
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
-
 #
-#     import PAMI.partialPeriodicPattern.topk.Topk_PPPGrowth as alg
+#     from PAMI.periodicFrequentPattern.basic import PPP_ECLAT as alg
 #
-#     obj = alg.Topk_PPPGrowth(iFile, k, periodicity)
+#     obj = alg.PPP_ECLAT(iFile, minPS, period)
 #
 #     obj.startMine()
 #
-#     partialPeriodicPatterns = obj.getPatterns()
+#     Patterns = obj.getPatterns()
 #
-#     print("Total number of top partial periodic Patterns:", len(partialPeriodicPatterns))
+#     print("Total number of partial periodic patterns:", len(Patterns))
 #
 #     obj.save(oFile)
 #
-#     Df = obj.getPatternInDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
 
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -49,379 +45,378 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.partialPeriodicPattern.topk import abstract as _abstract
-import validators as _validators
-from urllib.request import urlopen as _urlopen
-import sys as _sys
+
+from PAMI.partialPeriodicPattern.basic import abstract as _ab
 
 
-class Topk_PPPGrowth(_abstract.partialPeriodicPatterns):
+class PPP_ECLAT(_ab._partialPeriodicPatterns):
     """
-    Description:
-    -------------
-        Top - K is and algorithm to discover top partial periodic patterns in a temporal  database.
+    Descripition:
+    ----------------------
+        3pEclat is the fundamental approach to mine the partial periodic frequent patterns.
 
     Reference:
-    ----------
+    -----------
+        To be published
 
 
-    Attributes:
-    ------------
-            iFile : str
-                Input file name or path of the input file
-            k: int
-                User specified count of top partial periodic patterns
-            sep : str
-                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-                However, the users can override their default separator.
-            oFile : str
-                Name of the output file or the path of the output file
-            startTime:float
-                To record the start time of the mining process
-            endTime:float
-                To record the completion time of the mining process
-            finalPatterns: dict
-                Storing the complete set of patterns in a dictionary variable
-            memoryUSS : float
-                To store the total amount of USS memory consumed by the program
-            memoryRSS : float
-                To store the total amount of RSS memory consumed by the program
+    Parameters:
+    ----------
+        self.iFile : file
+            Name of the Input file or path of the input file
+        self. oFile : file
+            Name of the output file or path of the output file
+        minPS: float or int or str
+            The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
+        period: float or int or str
+            The user can specify period either in count or proportion of database size.
+            If the program detects the data type of period is integer, then it treats period is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: period=10 will be treated as integer, while period=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
+        Database : list
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            it represents the total no of transactions
+        tree : class
+            it represents the Tree class
+        finalPatterns : dict
+            it represents to store the patterns
+        tidList : dict
+            stores the timestamps of an item
 
     Methods:
-    --------
-            startMine()
-                Mining process will start from here
-            getPatterns()
-                Complete set of patterns will be retrieved with this function
-            save(oFile)
-                Complete set of frequent patterns will be loaded in to a output file
-            getPatternsAsDataFrame()
-                Complete set of frequent patterns will be loaded in to a dataframe
-            getMemoryUSS()
-                Total amount of USS memory consumed by the mining process will be retrieved from this function
-            getMemoryRSS()
-                Total amount of RSS memory consumed by the mining process will be retrieved from this function
-            getRuntime()
-                Total amount of runtime taken by the mining process will be retrieved from this function
-            creatingItemSets()
-                Scans the dataset or dataframes and stores in list format
-            frequentOneItem()
-                Generates one frequent patterns
-            eclatGeneration(candidateList)
-                It will generate the combinations of frequent items
-            generateFrequentPatterns(tidList)
-                It will generate the combinations of frequent items from a list of items
+    -------
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        save(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingOneitemSets()
+            Scan the database and store the items with their timestamps which are periodic frequent
+        getPeriodAndSupport()
+            Calculates the support and period for a list of timestamps.
+        Generation()
+            Used to implement prefix class equivalence method to generate the periodic patterns recursively
 
     Executing the code on terminal:
-    -------------------------------
+    ----------------------------------------
 
         Format:
-        ------
-            >>> python3 FAE.py <inputFile> <outputFile> <k> <periodicity>
+        -----------
+           >>> python3 PPP_ECLAT.py <inputFile> <outputFile> <minPS> <period>
 
         Examples:
-        ---------
-            >>> python3 FAE.py sampleDB.txt patterns.txt 10 3
+        -----------
+           >>> python3 PPP_ECLAT.py sampleDB.txt patterns.txt 0.3 0.4   (minPS and period will be considered in percentage of database transactions)
+
+           >>> python3 threePEeclat.py sampleDB.txt patterns.txt 3 4     (minPS and period will be considered in support count or frequency)
 
 
-    Sample run of the importing code:
-    ---------------------------------
+    Sample run of importing the code:
+    -----------------------------------------
     .. code-block:: python
 
-            import PAMI.partialPeriodicPattern.topk.Topk_PPPGrowth as alg
+        from PAMI.periodicFrequentPattern.basic import PPP_ECLAT as alg
 
-            obj = alg.Topk_PPPGrowth(iFile, k, periodicity)
+        obj = alg.PPP_ECLAT(iFile, minPS,period)
 
-            obj.startMine()
+        obj.startMine()
 
-            partialPeriodicPatterns = obj.getPatterns()
+        Patterns = obj.getPatterns()
 
-            print("Total number of top partial periodic Patterns:", len(partialPeriodicPatterns))
+        print("Total number of partial periodic patterns:", len(Patterns))
 
-            obj.save(oFile)
+        obj.save(oFile)
 
-            Df = obj.getPatternInDataFrame()
+        Df = obj.getPatternsAsDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+        memUSS = obj.getMemoryUSS()
 
-            print("Total Memory in USS:", memUSS)
+        print("Total Memory in USS:", memUSS)
 
-            memRSS = obj.getMemoryRSS()
+        memRSS = obj.getMemoryRSS()
 
-            print("Total Memory in RSS", memRSS)
+        print("Total Memory in RSS", memRSS)
 
-            run = obj.getRuntime()
+        run = obj.getRuntime()
 
-            print("Total ExecutionTime in seconds:", run)
+        print("Total ExecutionTime in seconds:", run)
 
     Credits:
-    ---------
-            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    ------------------
+
+    The complete program was written by P.RaviKumar  under the supervision of Professor Rage Uday Kiran.\n
+
 
-    """
 
+        """
     _startTime = float()
     _endTime = float()
-    _k = int()
-    _periodicity = " "
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
-    _Database = []
-    _tidList = {}
-    _lno = int()
-    _minimum = int()
     _mapSupport = {}
+    _itemsetCount = 0
+    _writer = None
+    _minPS = str()
+    _period = str()
+    _tidList = {}
+    _lno = 0
+    _Database = []
 
-    def _creatingItemSets(self):
+    def _convert(self, value):
+        """
+        To convert the given user specified value
+
+        :param value: user specified value
+
+        :return: converted value
         """
-            Storing the complete transactions of the database/input file in a database variable
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
+
+    def _getPeriodicSupport(self, timeStamps):
+        """
+            calculates the support and periodicity with list of timestamps
 
+            :param timeStamps : timestamps of a pattern
+
+            :type timeStamps : list
         """
+        timeStamps.sort()
+        per = 0
+        for i in range(len(timeStamps) - 1):
+            j = i + 1
+            if abs(timeStamps[j] - timeStamps[i]) <= self._period:
+                per += 1
+        return per
+
+    def _creatingItemSets(self):
         self._Database = []
-        if isinstance(self._iFile, _abstract._pd.DataFrame):
-            timeStamp, data = [], []
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            data, tids = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'TS' in i:
-                timeStamp = self._iFile['TS'].tolist()
+                tids = self._iFile['TS'].tolist()
             if 'Transactions' in i:
                 data = self._iFile['Transactions'].tolist()
             for i in range(len(data)):
-                tr = [timeStamp[i]]
+                tr = [tids[i][0]]
                 tr = tr + data[i]
                 self._Database.append(tr)
             self._lno = len(self._Database)
-            # print(self.Database)
+
         if isinstance(self._iFile, str):
-            if _validators.url(self._iFile):
-                data = _urlopen(self._iFile)
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
                 for line in data:
+                    line.strip()
                     self._lno += 1
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
                     self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             self._lno += 1
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _convert(self, value):
+    def _creatingOneitemSets(self):
         """
-        To convert the given user specified value
-        :param value: user specified value
-        :return: converted value
+           Scans the Temporal database / Input file and stores the 1-length partial-periodic patterns.
         """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
-
-    def _frequentOneItem(self):
-        """
-        Generating one frequent patterns
-        """
-
-        self._mapSupport = {}
+        plist = []
         self._tidList = {}
-        self._periodicity = self._convert(self._periodicity)
-        self._k = int(self._convert(self._k))
+        self._mapSupport = {}
+        self._period = self._convert(self._period)
         for line in self._Database:
-            n = int(line[0])
-            for i in range(1, len(line)):
-                si = line[i]
+            s = line
+            n = int(s[0])
+            for i in range(1, len(s)):
+                si = s[i]
                 if self._mapSupport.get(si) is None:
-                    self._mapSupport[si] = [1, 0, n]
+                    self._mapSupport[si] = [0, n]
                     self._tidList[si] = [n]
                 else:
-                    self._mapSupport[si][0] += 1
-                    period = abs(n - self._mapSupport[si][2])
-                    if period <= self._periodicity:
-                        self._mapSupport[si][1] += 1
-                    self._mapSupport[si][2] = n
+                    lp = n - self._mapSupport[si][1]
+                    if lp <= self._period:
+                        self._mapSupport[si][0] += 1
+                    self._mapSupport[si][1] = n
                     self._tidList[si].append(n)
-        for x, y in self._mapSupport.items():
-            period = abs(self._lno - self._mapSupport[x][2])
-            if period <= self._periodicity:
-                self._mapSupport[x][1] += 1
-        self._mapSupport = {k: v[1] for k, v in self._mapSupport.items()}
-        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[0], reverse=True)]
-        self._finalPatterns = {}
-        for i in plist:
-            if self._mapSupport[i] == 0:
-                continue
-            if len(self._finalPatterns) >= self._k:
-                break
-            else:
-                self._finalPatterns[i] = self._mapSupport[i]
-        print(len(self._finalPatterns),  self._k, self._periodicity)
-        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-        plist = list(self._finalPatterns.keys())
+        self._minPS = self._convert(self._minPS)
+        self._mapSupport = {k: v[0] for k, v in self._mapSupport.items() if v[0] >= self._minPS}
+        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         return plist
 
-    def _getSupportAndPeriod(self, timeStamps):
-        """To calculate the periodicity and support
-        :param timeStamps: Timestamps of an item set
-        :return: support, periodicity
+    def _save(self, prefix, suffix, tidSetX):
         """
-
-        timeStamps.sort()
-        sup = 0
-        for j in range(len(timeStamps) - 1):
-            per = abs(timeStamps[j + 1] - timeStamps[j])
-            if per <= self._periodicity:
-                sup += 1
-        return sup
-
-    def _save(self, prefix, suffix, tidSetI):
-        """Saves the patterns that satisfy the periodic frequent property.
+            saves the patterns that satisfy the partial periodic property.
 
             :param prefix: the prefix of a pattern
 
             :type prefix: list
 
-            :param suffix: the suffix of a patterns
+            :param suffix : the suffix of a patterns
 
-            :type suffix: list
+            :type suffix : list
 
-            :param tidSetI: the timestamp of a patterns
+            :param tidSetX : the timestamp of a patterns
+
+            :type tidSetX : list
 
-            :type tidSetI: list
-        """
 
+        """
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = self._getSupportAndPeriod(tidSetI)
-        sample = str()
-        for i in prefix:
-            sample = sample + i + "\t"
-        if len(self._finalPatterns) < self._k:
-            if val >= self._minimum:
-                self._finalPatterns[sample] = val
-                self._finalPatterns = {k: v for k, v in
-                                       sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-        else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
-                if val > y:
-                    del self._finalPatterns[x]
-                    self._finalPatterns[x] = y
-                    self._finalPatterns = {k: v for k, v in
-                                           sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                    self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-                    return
+        val = self._getPeriodicSupport(tidSetX)
+        if val >= self._minPS:
+            sample = str()
+            for i in prefix:
+                sample = sample + i + "\t"
+            self._finalPatterns[sample] = val
 
     def _Generation(self, prefix, itemSets, tidSets):
-        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+        """
+            Generates the patterns following Equivalence-class methods
 
-            :param prefix:  main equivalence prefix
+            :param prefix :  main equivalence prefix
 
-            :type prefix: periodic-frequent item or pattern
+            :type prefix : partial-periodic item or pattern
 
-            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
-                            and frequent with their timestamps
+            :param itemSets : patterns which are items combined with prefix and satisfying the periodicity
+                            and partial property with their timestamps
 
-            :type itemSets: list
+            :type itemSets : list
 
-            :param tidSets: timestamps of the items in the argument itemSets
+            :param tidSets : timestamps of the items in the argument itemSets
 
-            :type tidSets: list
-        """
+            :type tidSets : list
+
+
+                    """
         if len(itemSets) == 1:
             i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
+            tidi = tidSets[0]
+            self._save(prefix, [i], tidi)
             return
         for i in range(len(itemSets)):
             itemI = itemSets[i]
             if itemI is None:
                 continue
-            tidSetI = tidSets[i]
+            tidSetX = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
             for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
-                y = list(set(tidSetI).intersection(tidSetJ))
-                val = self._getSupportAndPeriod(y)
-                if val >= self._minimum:
+                y = list(set(tidSetX).intersection(tidSetJ))
+                val = self._getPeriodicSupport(y)
+                if val >= self._minPS:
                     classItemSets.append(itemJ)
                     classTidSets.append(y)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
+            newprefix = list(set(itemSetX)) + prefix
+            self._Generation(newprefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetX)
 
     def startMine(self):
         """
-            Main function of the program
+            Main program start with extracting the periodic frequent items from the database and
+            performs prefix equivalence to form the combinations and generates partial-periodic patterns.
 
         """
-        self._startTime = _abstract._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._k is None:
-            raise Exception("Please enter the Minimum Support")
+        self._startTime = _ab._time.time()
         self._creatingItemSets()
-        plist = self._frequentOneItem()
+        plist = self._creatingOneitemSets()
+        self._finalPatterns = {}
         for i in range(len(plist)):
             itemI = plist[i]
-            tidSetI = self._tidList[itemI]
+            tidSetX = self._tidList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i + 1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetI).intersection(tidSetJ))
-                val = self._getSupportAndPeriod(y1)
-                if val >= self._minimum:
+                y1 = list(set(tidSetX).intersection(tidSetJ))
+                val = self._getPeriodicSupport(y1)
+                if val >= self._minPS:
                     itemSets.append(itemJ)
                     tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print("TopK partial periodic patterns were generated successfully")
-        self._endTime = _abstract._time.time()
-        process = _abstract._psutil.Process(_abstract._os.getpid())
-        self._memoryUSS = float()
+            self._save(None, itemSetX, tidSetX)
+        print("Partial Periodic Patterns were generated successfully using 3PEclat algorithm")
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """
+        Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-                    :return: returning USS memory consumed by the mining process
+        :return: returning USS memory consumed by the mining process
 
-                    :rtype: float
+        :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
@@ -429,15 +424,16 @@
 
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
-        """Calculating the total amount of runtime taken by the mining process
+        """
+        Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
 
         :rtype: float
         """
 
         return self._endTime - self._startTime
@@ -446,58 +442,66 @@
         """Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
 
         :rtype: pd.DataFrame
         """
 
-        dataFrame = {}
+        dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
-            dataFrame = _abstract._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        return dataFrame
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicSupport'])
+        return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Top K Partial Periodic Patterns:", len(self.getPatterns()))
+        print("Total number of Partial Periodic Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_sys.argv) == 5 or len(_sys.argv) == 6:
-        if len(_sys.argv) == 6:
-            _ap = Topk_PPPGrowth(_sys.argv[1], _sys.argv[3], _sys.argv[4], _sys.argv[5])
-        if len(_sys.argv) == 5:
-            _ap = Topk_PPPGrowth(_sys.argv[1], _sys.argv[3], _sys.argv[4])
+    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
+        if len(_ab._sys.argv) == 6:
+            _ap = PPP_ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+        if len(_ab._sys.argv) == 5:
+            _ap = PPP_ECLAT(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
-        print("Top K Partial Periodic Patterns:", len(_ap.getPatterns()))
-        _ap.save(_sys.argv[2])
+        print("Total number of Partial Periodic Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        for i in [100, 200, 300, 400, 500]:
+            _ap = PPP_ECLAT('/Users/Likhitha/Downloads/temporal_T10I4D100K.csv', i, 5000, '\t')
+            _ap.startMine()
+            print("Total number of Maximal Partial Periodic Patterns:", len(_ap.getPatterns()))
+            _ap.save('/Users/Likhitha/Downloads/output.txt')
+            print("Total Memory in USS:", _ap.getMemoryUSS())
+            print("Total Memory in RSS", _ap.getMemoryRSS())
+            print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,16 @@
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
+            #s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of periodic-frequent patterns after completion of the mining process
 
         :return: returning periodic-frequent patterns
         :rtype: dict
```

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,16 @@
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.replace(' ', '\t').strip() + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
+            #s1 = x.replace(' ', '\t').strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of periodic-frequent patterns after completion of the mining process
 
         :return: returning periodic-frequent patterns
         :rtype: dict
```

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,16 @@
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.replace(' ','\t').strip() + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
+            #s1 = x.replace(' ','\t').strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of periodic-frequent patterns after completion of the mining process
 
         :return: returning periodic-frequent patterns
         :rtype: dict
```

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,16 @@
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
+            #s1 = x.replace(' ', '\t') + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of periodic-frequent patterns after completion of the mining process
 
         :return: returning periodic-frequent patterns
         :rtype: dict
```

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -883,15 +883,16 @@
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.replace(' ', '\t').strip() + ":" + str(y[0]) + ":" + str(y[1])
+            s1 = x + ":" + str(y[0]) + ":" + str(y[1])
+            #s1 = x.replace(' ', '\t').strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of periodic-frequent patterns after completion of the mining process
 
         :return: returning periodic-frequent patterns
         :rtype: dict
```

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.8.6.3/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.8.6.3/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2023.8.6.3/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-from abc import ABC as _ABC , abstractmethod as _abstractmethod
+from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
+import math as _math
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _combinations
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 
 
-
-class _frequentPatterns(_ABC):
+class _partialPeriodicPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
     employ in PAMI
 
         ...
 
-    Attributes:
-    ----------
+        Attributes
+        ----------
         iFile : str
             Input file name or path of the input file
-        minSup: float
-            UserSpecified minimum support value. It has to be given in terms of count of total number of transactions
+        minPS: float
+            UserSpecified minimum period-support value. It has to be given in terms of count of total number of transactions
             in the input database/file
-        minRS: float
-            UserSpecified minimum relative support value. calculated as
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods:
-    -------
+        Methods
+        -------
         startMine()
             Mining process will start from here
         getFrequentPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -55,32 +53,34 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, minSup, minRatio, sep='\t'):
+    def __init__(self, iFile, minPS, period, relativePS, sep='\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param minSup: UserSpecified minimum support value. It has to be given in terms of count of total number of
+        :param minPS: UserSpecified minimum period-support value. It has to be given in terms of count of total number of
         transactions in the input database/file
-        :type minSup: str
+        :type minPS: float
         """
 
         self._iFile = iFile
-        self._minSup = minSup
-        self._minRatio = minRatio
+        self._minPS = minPS
+        self._period = period
+        self._relativePS = relativePS
         self._sep = sep
         self._finalPatterns = {}
+        self._oFile = str()
         self._startTime = float()
         self._endTime = float()
-        self._memoryRSS = float()
         self._memoryUSS = float()
+        self._memoryRSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -118,13 +118,7 @@
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
-
-    @_abstractmethod
-    def printResults(self):
-        """ To print the results of execution."""
-
-        pass
```

### Comparing `pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.8.6.3/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.8.6.3/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.8.6.3/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2023.8.6.3/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.6.3/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/PKG-INFO` & `pami-2023.8.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.6.2
+Version: 2023.8.6.3
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pami-2023.8.6.2/README.md` & `pami-2023.8.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/pami.egg-info/PKG-INFO` & `pami-2023.8.6.3/pami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.6.2
+Version: 2023.8.6.3
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pami-2023.8.6.2/pami.egg-info/SOURCES.txt` & `pami-2023.8.6.3/pami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pami-2023.8.6.2/setup.py` & `pami-2023.8.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2023.08.06.02',
+    version='2023.08.06.03',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
```

