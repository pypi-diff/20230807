# Comparing `tmp/ECMpy2.0-1.0.1.tar.gz` & `tmp/ECMpy2.0-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ECMpy2.0-1.0.1.tar", last modified: Fri Aug  4 02:46:59 2023, max compression
+gzip compressed data, was "ECMpy2.0-1.0.2.tar", last modified: Mon Aug  7 08:09:49 2023, max compression
```

## Comparing `ECMpy2.0-1.0.1.tar` & `ECMpy2.0-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,1640 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-08-04 02:46:59.634269 ECMpy2.0-1.0.1/ECMpy/
--rw-rw-rw-   0        0        0    94027 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/AutoPACMEN_function.py
--rw-rw-rw-   0        0        0   121429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/ECMpy_function.py
--rw-rw-rw-   0        0        0       19 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/__init__.py
--rw-rw-rw-   0        0        0     4718 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/get_ecGEM_onestop.py
--rw-rw-rw-   0        0        0     8905 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/model.py
--rw-rw-rw-   0        0        0     9605 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/prediction_for_input.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/
--rw-rw-rw-   0        0        0      252 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      184 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      252 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2883 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      835 2023-08-04 02:40:07.000000 ECMpy2.0-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.229388 ECMpy2.0-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:47.425733 ECMpy2.0-1.0.2/ECMpy2.0-main/
+-rw-rw-rw-   0        0        0    10244 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/.DS_Store
+-rw-rw-rw-   0        0        0     1537 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/00.Model_preview.ipynb
+-rw-rw-rw-   0        0        0   147883 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/01.get_reactiion_kcat_using_DLKcat.ipynb
+-rw-rw-rw-   0        0        0    12625 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/01.get_reaction_kcat_using_AutoPACMEN.ipynb
+-rw-rw-rw-   0        0        0     4142 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/02.get_ecModel_using_ECMpy.ipynb
+-rw-rw-rw-   0        0        0     8953 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/03.ecModel_calibration.ipynb
+-rw-rw-rw-   0        0        0  4314555 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/04.ecModel_analysis.ipynb
+-rw-rw-rw-   0        0        0    39675 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/05.ecModel_ME.ipynb
+-rw-rw-rw-   0        0        0     3263 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/06.One-click_modeling.ipynb
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:47.429727 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/
+-rw-rw-rw-   0        0        0     6148 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/.DS_Store
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:48.496975 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acanthamoeba castellanii_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acetivibrio clariflavus_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acetivibrio thermocellus_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acetobacter aceti_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acetobacter xylinus_taxonomy_NA
+-rw-rw-rw-   0        0        0      141 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acetobacter_taxonomy
+-rw-rw-rw-   0        0        0      150 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acetomicrobium mobile_taxonomy
+-rw-rw-rw-   0        0        0      180 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acholeplasma laidlawii_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acidilobus saccharovorans_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acidithiobacillus ferrooxidans_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acidithiobacillus thiooxidans_taxonomy
+-rw-rw-rw-   0        0        0      206 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acinetobacter baumannii_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acinetobacter baylyi_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acinetobacter calcoaceticus (subsp. anitratus)_taxonomy_NA
+-rw-rw-rw-   0        0        0      240 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acinetobacter calcoaceticus subsp. anitratus_taxonomy
+-rw-rw-rw-   0        0        0      206 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acinetobacter calcoaceticus_taxonomy
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Acinetobacter sp._taxonomy
+-rw-rw-rw-   0        0        0      351 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Actinidia chinensis_taxonomy
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Actinomadura sp. R39_taxonomy
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Actinomadura sp._taxonomy
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Actinoplanes missouriensis_taxonomy
+-rw-rw-rw-   0        0        0      214 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Actinosynnema pretiosum subsp. auranticum_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Advenella mimigardefordensis_taxonomy
+-rw-rw-rw-   0        0        0      459 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aedes aegypti_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aeribacillus pallidus_taxonomy
+-rw-rw-rw-   0        0        0      152 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aeromonas veronii_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aeropyrum pernix_taxonomy
+-rw-rw-rw-   0        0        0      248 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Agaricus bisporus_taxonomy
+-rw-rw-rw-   0        0        0      233 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Agrobacterium tumefaciens_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alcaligenes faecalis_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alcanivorax borkumensis_taxonomy
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alicyclobacillus acidocaldarius subsp. acidocaldarius_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alicyclobacillus acidocaldarius_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alicyclobacillus hesperidum_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alkaliphilus oremlandii_taxonomy
+-rw-rw-rw-   0        0        0      455 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alligator mississippiensis_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Allochromatium vinosum_taxonomy
+-rw-rw-rw-   0        0        0      354 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alnus glutinosa_taxonomy
+-rw-rw-rw-   0        0        0      346 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alternanthera ficoidea_taxonomy
+-rw-rw-rw-   0        0        0      346 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alternanthera pungens_taxonomy
+-rw-rw-rw-   0        0        0      346 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alternanthera sessilis_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alteromonas macleodii_taxonomy
+-rw-rw-rw-   0        0        0      225 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Alteromonas sp._taxonomy
+-rw-rw-rw-   0        0        0      261 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Amborella trichopoda_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Amycolatopsis orientalis_taxonomy
+-rw-rw-rw-   0        0        0      217 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Amycolatopsis sp._taxonomy
+-rw-rw-rw-   0        0        0      237 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anabaena sp._taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anaerobiospirillum succiniciproducens_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anaerotignum propionicum_taxonomy
+-rw-rw-rw-   0        0        0      559 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anas platyrhynchos_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aneurinibacillus migulanus_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aneurinibacillus thermoaerophilus_taxonomy
+-rw-rw-rw-   0        0        0      421 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anguilla anguilla_taxonomy
+-rw-rw-rw-   0        0        0      498 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anopheles gambiae_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anoxybacillus flavithermus_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anoxybacillus gonensis_taxonomy
+-rw-rw-rw-   0        0        0      586 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Anser sp._taxonomy
+-rw-rw-rw-   0        0        0       76 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Antarctic bacterium TAB5_taxonomy
+-rw-rw-rw-   0        0        0      465 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Apis cerana indica_taxonomy
+-rw-rw-rw-   0        0        0      465 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Apis cerana japonica_taxonomy
+-rw-rw-rw-   0        0        0      447 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Apis mellifera_taxonomy
+-rw-rw-rw-   0        0        0      321 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aplysia californica_taxonomy
+-rw-rw-rw-   0        0        0      321 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aplysia fasciata_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aquaspirillum arcticum_taxonomy
+-rw-rw-rw-   0        0        0      132 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aquifex aeolicus_taxonomy
+-rw-rw-rw-   0        0        0      132 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aquifex pyrophilus_taxonomy
+-rw-rw-rw-   0        0        0      384 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arabidopsis thaliana_taxonomy
+-rw-rw-rw-   0        0        0      151 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Archaeoglobus fulgidus_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aromatoleum aromaticum_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aromatoleum evansii_taxonomy
+-rw-rw-rw-   0        0        0      422 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Artemisia spiciformis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Artemisia tridentata subsp. spiciformis_taxonomy_NA
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arthrobacter crystallopoietes_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arthrobacter globiformis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arthrobacter nicotinovorans_taxonomy_NA
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arthrobacter psychrolactophilus_taxonomy
+-rw-rw-rw-   0        0        0      207 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arthrobacter sp._taxonomy
+-rw-rw-rw-   0        0        0      248 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Arthrospira platensis_taxonomy
+-rw-rw-rw-   0        0        0      286 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ascaris suum_taxonomy
+-rw-rw-rw-   0        0        0      309 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus aculeatus_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus carbonarius_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus carneus_taxonomy
+-rw-rw-rw-   0        0        0      307 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus clavatus_taxonomy
+-rw-rw-rw-   0        0        0      309 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus flavus_taxonomy
+-rw-rw-rw-   0        0        0      307 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus fumigatus_taxonomy
+-rw-rw-rw-   0        0        0      309 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus nidulans_taxonomy
+-rw-rw-rw-   0        0        0      309 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus niger_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus niveus_taxonomy
+-rw-rw-rw-   0        0        0      309 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus oryzae_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Aspergillus sojae_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Astrosclera willeyana_taxonomy
+-rw-rw-rw-   0        0        0      141 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Autographa californica multiple nucleopolyhedrovirus_taxonomy
+-rw-rw-rw-   0        0        0      440 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Avena sativa_taxonomy
+-rw-rw-rw-   0        0        0      384 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Avicennia marina_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Azoarcus evansii_taxonomy_NA
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Azospirillum brasilense_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Azotobacter vinelandii_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Babesia bovis_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Babesia gibsoni_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus altitudinis_taxonomy
+-rw-rw-rw-   0        0        0      223 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus amyloliquefaciens_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus anthracis_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus cereus_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus coagulans_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus halodurans_taxonomy_NA
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus licheniformis_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus methanolicus_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus pumilus_taxonomy
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus sp. (in_ firmicutes)_taxonomy
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus sp. PS3_taxonomy
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus sp. YM55-1_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus sp._taxonomy_NA
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus subtilis_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacillus thuringiensis_taxonomy
+-rw-rw-rw-   0        0        0      380 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacopa monnieri_taxonomy
+-rw-rw-rw-   0        0        0      441 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteria Latreille et al. 1825_taxonomy
+-rw-rw-rw-   0        0        0       32 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteria_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteriophage T4_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteriophage phi-13_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteriophage phi-6_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteriophage phi-8_taxonomy_NA
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteroides fragilis_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteroides ovatus_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bacteroides thetaiotaomicron_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bamboo mosaic virus_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bartonella henselae_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bifidobacterium longum subsp. Longum_taxonomy_NA
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bifidobacterium longum subsp. infantis_taxonomy
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bifidobacterium longum subsp. longum_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bifidobacterium longum_taxonomy
+-rw-rw-rw-   0        0        0      253 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bjerkandera adusta_taxonomy
+-rw-rw-rw-   0        0        0      253 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bjerkandera fumosa_taxonomy
+-rw-rw-rw-   0        0        0      284 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bjerkandera sp._taxonomy
+-rw-rw-rw-   0        0        0      244 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Blastobotrys adeninivorans_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Blastochloris viridis_taxonomy
+-rw-rw-rw-   0        0        0      265 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Blastocladiella emersonii_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Blautia hydrogenotrophica_taxonomy
+-rw-rw-rw-   0        0        0      512 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bombyx mori_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bordetella pertussis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Borrelia burgdorferi_taxonomy_NA
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Borreliella burgdorferi_taxonomy
+-rw-rw-rw-   0        0        0      485 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bos taurus_taxonomy
+-rw-rw-rw-   0        0        0      528 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bothrops jararaca_taxonomy
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Botryococcus braunii_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bradyrhizobium diazoefficiens_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bradyrhizobium japonicum_taxonomy
+-rw-rw-rw-   0        0        0      255 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Branchiostoma floridae_taxonomy
+-rw-rw-rw-   0        0        0      255 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Branchiostoma lanceolatum_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brassica capitata_taxonomy_NA
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brassica juncea_taxonomy
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brassica napus_taxonomy
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brassica oleracea_taxonomy
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brassica rapa_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brucella abortus_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brucella anthropi_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brucella melitensis_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brucella microti_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brucella suis_taxonomy
+-rw-rw-rw-   0        0        0      285 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Brugia malayi_taxonomy
+-rw-rw-rw-   0        0        0      489 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Bubalus bubalis_taxonomy
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Buckleyzyma aurantiaca_taxonomy
+-rw-rw-rw-   0        0        0      224 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia cenocepacia J2315_taxonomy
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia cenocepacia_taxonomy
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia cepacia_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia glumae_taxonomy
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia mallei_taxonomy
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia pseudomallei_taxonomy
+-rw-rw-rw-   0        0        0      190 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia sp._taxonomy
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia thailandensis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia xenovorans LB400_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Burkholderia xenovorans_taxonomy_NA
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Butyrivibrio crossotus_taxonomy
+-rw-rw-rw-   0        0        0      312 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Caenorhabditis elegans_taxonomy
+-rw-rw-rw-   0        0        0      282 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Caldanaerobacter subterraneus subsp. tengcongensis MB4_taxonomy
+-rw-rw-rw-   0        0        0      225 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Caldanaerobacter subterraneus subsp. tengcongensis_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Caldibacillus thermoamylovorans_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Caldicellulosiruptor saccharolyticus_taxonomy
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Camelina sativa_taxonomy
+-rw-rw-rw-   0        0        0      345 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Camellia sinensis_taxonomy
+-rw-rw-rw-   0        0        0      462 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Camelus dromedarius_taxonomy
+-rw-rw-rw-   0        0        0      195 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Campylobacter jejuni subsp. jejuni_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Campylobacter jejuni_taxonomy
+-rw-rw-rw-   0        0        0      293 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Candida albicans_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Candida intermedia_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Candida mycoderma_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Candida tenuis_taxonomy_NA
+-rw-rw-rw-   0        0        0      293 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Candida tropicalis_taxonomy
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Candidatus Pelagibacter ubique_taxonomy
+-rw-rw-rw-   0        0        0      223 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Canid alphaherpesvirus 1_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Canis familiaris_taxonomy_NA
+-rw-rw-rw-   0        0        0      475 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Canis lupus familiaris_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Capitata_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Capra capra_taxonomy_NA
+-rw-rw-rw-   0        0        0      476 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Capra_taxonomy
+-rw-rw-rw-   0        0        0      396 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Capsicum frutescens_taxonomy
+-rw-rw-rw-   0        0        0      514 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Carassius auratus_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Carboxydothermus hydrogenoformans_taxonomy
+-rw-rw-rw-   0        0        0      256 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Catenaria anguillulae_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Caulobacter vibrioides_taxonomy
+-rw-rw-rw-   0        0        0      476 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cavia porcellus_taxonomy
+-rw-rw-rw-   0        0        0      210 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cellulomonas sp._taxonomy
+-rw-rw-rw-   0        0        0      543 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ceratitis capitata_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cereibacter sphaeroides_taxonomy
+-rw-rw-rw-   0        0        0      603 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chionodraco hamatus_taxonomy
+-rw-rw-rw-   0        0        0      190 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chlamydia pneumoniae_taxonomy
+-rw-rw-rw-   0        0        0      190 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chlamydia trachomatis_taxonomy
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chlamydomonas reinhardtii_taxonomy
+-rw-rw-rw-   0        0        0      248 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chlamydomonas sp._taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chlamydophila pneumoniae_taxonomy_NA
+-rw-rw-rw-   0        0        0      195 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chlorobaculum tepidum_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chloroflexus aurantiacus_taxonomy
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chromobacterium violaceum_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Chromohalobacter salexigens_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Citrobacter freundii_taxonomy
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Citrobacter koseri_taxonomy
+-rw-rw-rw-   0        0        0      192 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Citrobacter sp. S-77_taxonomy
+-rw-rw-rw-   0        0        0      192 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Citrobacter sp._taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Classical swine fever virus_taxonomy
+-rw-rw-rw-   0        0        0      301 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clonorchis sinensis_taxonomy
+-rw-rw-rw-   0        0        0      176 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridioides difficile_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridium acetobutylicum_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridium perfringens_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridium sp._taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridium subterminale_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridium tetani_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Clostridium thermocellum_taxonomy_NA
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cobetia marina_taxonomy
+-rw-rw-rw-   0        0        0      531 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Columba livia_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Colwellia maris_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Colwellia psychrerythraea_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Comamonas testosteroni_taxonomy
+-rw-rw-rw-   0        0        0      237 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Conticribra weissflogii_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Coprococcus eutactus_taxonomy
+-rw-rw-rw-   0        0        0      298 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corallomycetella repens_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium ammoniagenes_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium callunae_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium crenatum_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium glutamicum subsp. lactofermentum_taxonomy_NA
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium glutamicum_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium sp. U-96_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Corynebacterium sp._taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Coturnix coturnix japonica_taxonomy_NA
+-rw-rw-rw-   0        0        0      567 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Coturnix coturnix_taxonomy
+-rw-rw-rw-   0        0        0      567 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Coturnix japonica_taxonomy
+-rw-rw-rw-   0        0        0      510 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cricetulus griseus_taxonomy
+-rw-rw-rw-   0        0        0      206 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Crithidia fasciculata_taxonomy
+-rw-rw-rw-   0        0        0      248 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Crocosphaera subtropica_taxonomy
+-rw-rw-rw-   0        0        0      528 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Crotalus adamanteus_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cryptococcus flavus_taxonomy_NA
+-rw-rw-rw-   0        0        0      263 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cryptococcus neoformans_taxonomy
+-rw-rw-rw-   0        0        0      211 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cryptosporidium parvum_taxonomy
+-rw-rw-rw-   0        0        0      382 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cucumis sativus_taxonomy
+-rw-rw-rw-   0        0        0      357 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cuphea hookeriana_taxonomy
+-rw-rw-rw-   0        0        0      357 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cuphea palustris_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cupriavidus necator_taxonomy
+-rw-rw-rw-   0        0        0      139 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cyanidium caldarium_taxonomy
+-rw-rw-rw-   0        0        0      112 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cyanophora paradoxa_taxonomy
+-rw-rw-rw-   0        0        0      513 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cyprinus carpio_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Cytobacillus firmus_taxonomy
+-rw-rw-rw-   0        0        0      525 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Daboia russelii_taxonomy
+-rw-rw-rw-   0        0        0      510 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Danio rerio_taxonomy
+-rw-rw-rw-   0        0        0      330 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dasyatis pastinaca_taxonomy
+-rw-rw-rw-   0        0        0      449 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Daucus carota_taxonomy
+-rw-rw-rw-   0        0        0      265 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Debaryomyces hansenii_taxonomy
+-rw-rw-rw-   0        0        0      265 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Debaryomyces nepalensis_taxonomy
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dehalococcoides mccartyi_taxonomy
+-rw-rw-rw-   0        0        0      535 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Deinagkistrodon acutus_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Deinococcus radiodurans_taxonomy
+-rw-rw-rw-   0        0        0      151 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Delftia acidovorans_taxonomy
+-rw-rw-rw-   0        0        0      178 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Delftia sp._taxonomy
+-rw-rw-rw-   0        0        0      180 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Desulfitobacterium hafniense_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Desulfotalea psychrophila_taxonomy
+-rw-rw-rw-   0        0        0      205 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Desulfovibrio sp. A2_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Desulfurococcus amylolyticus_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dickeya chrysanthemi_taxonomy
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dictyoglomus turgidum_taxonomy
+-rw-rw-rw-   0        0        0      180 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dictyostelium discoideum_taxonomy
+-rw-rw-rw-   0        0        0      213 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dictyostelium sp._taxonomy
+-rw-rw-rw-   0        0        0      246 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dioszegia sp._taxonomy
+-rw-rw-rw-   0        0        0      290 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dirofilaria immitis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Drosophila lebanonensis_taxonomy_NA
+-rw-rw-rw-   0        0        0      605 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Drosophila melanogaster_taxonomy
+-rw-rw-rw-   0        0        0      572 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Drosophila virilis_taxonomy
+-rw-rw-rw-   0        0        0      312 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dugesia ryukyuensis_taxonomy
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dunaliella salina_taxonomy
+-rw-rw-rw-   0        0        0      513 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Dysdercus peruvianus_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Edwardsiella ictaluri_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Eimeria tenella_taxonomy
+-rw-rw-rw-   0        0        0      308 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Eisenia fetida_taxonomy
+-rw-rw-rw-   0        0        0      152 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Entamoeba histolytica_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Enterobacter cloacae_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Enterobacter sp. B13_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Enterococcus faecalis_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Enterococcus faecium_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Enterococcus gallinarum_taxonomy
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Enterococcus sp._taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Epstein-Barr virus_taxonomy_NA
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Equine infectious anemia virus_taxonomy
+-rw-rw-rw-   0        0        0      445 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Equus caballus_taxonomy
+-rw-rw-rw-   0        0        0      245 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Eremothecium gossypii_taxonomy
+-rw-rw-rw-   0        0        0      150 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Erwinia amylovora_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Erwinia chrysanthemi_taxonomy_NA
+-rw-rw-rw-   0        0        0      150 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Erwinia rhapontici_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Erysipelothrix rhusiopathiae_taxonomy
+-rw-rw-rw-   0        0        0      371 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Erythroxylum coca_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Escherichia coli K-12_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Escherichia coli P76440_taxonomy_NA
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Escherichia coli_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Escherichia phage T2_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Escherichia phage T4_taxonomy
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ethanoligenens harbinense_taxonomy
+-rw-rw-rw-   0        0        0      395 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Eucalyptus camaldulensis_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Euglena gracilis_taxonomy
+-rw-rw-rw-   0        0        0      468 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Euphorbia characias_taxonomy
+-rw-rw-rw-   0        0        0      254 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Exiguobacterium sp._taxonomy
+-rw-rw-rw-   0        0        0      317 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fasciola gigantica_taxonomy
+-rw-rw-rw-   0        0        0      223 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Felid alphaherpesvirus 1_taxonomy
+-rw-rw-rw-   0        0        0      471 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Felis catus_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ferroplasma acidiphilum_taxonomy
+-rw-rw-rw-   0        0        0      250 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fibrobacter succinogenes subsp. succinogenes S85_taxonomy
+-rw-rw-rw-   0        0        0      426 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Flaveria bidentis_taxonomy
+-rw-rw-rw-   0        0        0      426 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Flaveria pringlei_taxonomy
+-rw-rw-rw-   0        0        0      426 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Flaveria trinervia_taxonomy
+-rw-rw-rw-   0        0        0      209 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Flavobacterium frigidimaris_taxonomy
+-rw-rw-rw-   0        0        0      243 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Flavobacterium sp._taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Francisella tularensis_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fructobacillus fructosus_taxonomy
+-rw-rw-rw-   0        0        0      331 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fusarium oxysporum_taxonomy
+-rw-rw-rw-   0        0        0      328 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fusarium solani_taxonomy
+-rw-rw-rw-   0        0        0      331 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fusarium verticillioides_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Fusobacterium nucleatum subsp. nucleatum_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Gallus gallus_taxonomy_NA
+-rw-rw-rw-   0        0        0      246 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ganoderma lucidum_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Gemmata obscuriglobus_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Geobacillus kaustophilus_taxonomy
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Geobacillus sp. MAS1_taxonomy
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Geobacillus sp. Y4.1MC1_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Geobacillus stearothermophilus_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Geobacillus thermodenitrificans_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Geobacter sulfurreducens_taxonomy
+-rw-rw-rw-   0        0        0      151 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Giardia intestinalis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Giardia lamblia_taxonomy_NA
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Gluconobacter oxydans_taxonomy
+-rw-rw-rw-   0        0        0      178 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Glutamicibacter nicotianae_taxonomy
+-rw-rw-rw-   0        0        0      502 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Glycine max_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Gramella forsetii_taxonomy_NA
+-rw-rw-rw-   0        0        0      429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Gryllus firmus_taxonomy
+-rw-rw-rw-   0        0        0      261 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Haemonchus contortus_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Haemophilus influenzae_taxonomy
+-rw-rw-rw-   0        0        0      148 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Hafnia alvei_taxonomy
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Halalkalibacterium halodurans_taxonomy
+-rw-rw-rw-   0        0        0      172 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Halanaerobium hydrogeniformans_taxonomy
+-rw-rw-rw-   0        0        0      137 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Haliangium ochraceum_taxonomy
+-rw-rw-rw-   0        0        0      172 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Haloarcula japonica_taxonomy
+-rw-rw-rw-   0        0        0      172 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Haloarcula marismortui_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Haloferax volcanii_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Halothiobacillus neapolitanus_taxonomy
+-rw-rw-rw-   0        0        0      431 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Helianthus annuus_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Helicobacter pylori_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Herpes simplex virus_taxonomy_NA
+-rw-rw-rw-   0        0        0      610 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Hippoglossus hippoglossus_taxonomy
+-rw-rw-rw-   0        0        0      610 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Hippoglossus stenolepis_taxonomy
+-rw-rw-rw-   0        0        0      274 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Histoplasma capsulatum_taxonomy
+-rw-rw-rw-   0        0        0      528 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Homo sapiens_taxonomy
+-rw-rw-rw-   0        0        0      404 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Hordeum vulgare_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Human alphaherpesvirus 1_taxonomy
+-rw-rw-rw-   0        0        0      229 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Human gammaherpesvirus 4_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Human gammaherpesvirus 8_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Human herpesvirus 1_taxonomy_NA
+-rw-rw-rw-   0        0        0      241 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Huperzia serrata_taxonomy
+-rw-rw-rw-   0        0        0      140 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Hydrogenobacter thermophilus_taxonomy
+-rw-rw-rw-   0        0        0      177 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Hydrogenobaculum sp. Y04AAS1_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ignicoccus islandicus_taxonomy
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ignisphaera aggregans_taxonomy
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ipomoea batatas_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Klebsiella aerogenes_taxonomy
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Klebsiella pneumoniae subsp. pneumoniae_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Klebsiella pneumoniae_taxonomy
+-rw-rw-rw-   0        0        0      246 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Kluyveromyces lactis_taxonomy
+-rw-rw-rw-   0        0        0      246 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Kluyveromyces marxianus_taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Komagataeibacter xylinus_taxonomy
+-rw-rw-rw-   0        0        0      243 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Komagataella pastoris_taxonomy
+-rw-rw-rw-   0        0        0      242 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lachancea kluyveri_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lacticaseibacillus casei_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactiplantibacillus pentosus_taxonomy
+-rw-rw-rw-   0        0        0      211 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactiplantibacillus plantarum WCFS1_taxonomy
+-rw-rw-rw-   0        0        0      211 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactiplantibacillus plantarum subsp. plantarum_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactiplantibacillus plantarum_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus acidophilus_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus brevis_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus casei_taxonomy_NA
+-rw-rw-rw-   0        0        0      201 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus delbrueckii subsp. bulgaricus_taxonomy
+-rw-rw-rw-   0        0        0      201 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus delbrueckii subsp. lactis_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus delbrueckii_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus fermentum_taxonomy_NA
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus gasseri_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus helveticus_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus jensenii_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus plantarum_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus reuteri_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus sakei_taxonomy_NA
+-rw-rw-rw-   0        0        0      202 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus sp. 30A_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactobacillus sp. 30a_taxonomy_NA
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactococcus cremoris_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactococcus lactis subsp. cremoris_taxonomy_NA
+-rw-rw-rw-   0        0        0      192 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactococcus lactis subsp. lactis_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lactococcus lactis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lampetra japonica_taxonomy_NA
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lancefieldella rimae_taxonomy
+-rw-rw-rw-   0        0        0      470 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lathyrus cicera_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Latilactobacillus sakei_taxonomy
+-rw-rw-rw-   0        0        0      342 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Latimeria menadoensis_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Legionella pneumophila_taxonomy
+-rw-rw-rw-   0        0        0      266 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania amazonensis_taxonomy
+-rw-rw-rw-   0        0        0      267 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania braziliensis_taxonomy
+-rw-rw-rw-   0        0        0      266 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania chagasi_taxonomy
+-rw-rw-rw-   0        0        0      266 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania donovani_taxonomy
+-rw-rw-rw-   0        0        0      266 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania infantum_taxonomy
+-rw-rw-rw-   0        0        0      263 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania major_taxonomy
+-rw-rw-rw-   0        0        0      266 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leishmania mexicana_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leminorella grimontii_taxonomy
+-rw-rw-rw-   0        0        0      466 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lens culinaris_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lentilactobacillus buchneri_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leptospira biflexa serovar Patoc_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leptospira interrogans serovar Copenhageni_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leptospira interrogans_taxonomy
+-rw-rw-rw-   0        0        0      283 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lethenteron camtschaticum_taxonomy
+-rw-rw-rw-   0        0        0      508 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lethocerus indicus_taxonomy
+-rw-rw-rw-   0        0        0      414 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leucaena leucocephala_taxonomy
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leuconostoc mesenteroides subsp. mesenteroides_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Leuconostoc mesenteroides_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Levilactobacillus brevis_taxonomy
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ligilactobacillus saerimneri 30a_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Limosilactobacillus antri_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Limosilactobacillus fermentum_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Limosilactobacillus reuteri_taxonomy
+-rw-rw-rw-   0        0        0      267 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Limulus polyphemus_taxonomy
+-rw-rw-rw-   0        0        0      238 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lipomyces starkeyi_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Listeria monocytogenes_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Listeria seeligeri_taxonomy
+-rw-rw-rw-   0        0        0      408 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lithobates catesbeianus_taxonomy
+-rw-rw-rw-   0        0        0      473 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lotus japonicus_taxonomy
+-rw-rw-rw-   0        0        0      508 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lucilia cuprina_taxonomy
+-rw-rw-rw-   0        0        0      469 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lupinus luteus_taxonomy
+-rw-rw-rw-   0        0        0      392 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lycium ruthenicum_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Lysinibacillus sphaericus_taxonomy
+-rw-rw-rw-   0        0        0      548 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Macaca mulatta_taxonomy
+-rw-rw-rw-   0        0        0      548 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Macaca radiata_taxonomy
+-rw-rw-rw-   0        0        0      277 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Macadamia tetraphylla_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Magnaporthe grisea 70-15_taxonomy_NA
+-rw-rw-rw-   0        0        0      221 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Malassezia globosa_taxonomy
+-rw-rw-rw-   0        0        0      385 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Malus domestica_taxonomy
+-rw-rw-rw-   0        0        0      314 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mammalia_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mammalian orthoreovirus_taxonomy
+-rw-rw-rw-   0        0        0      400 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Manihot esculenta_taxonomy
+-rw-rw-rw-   0        0        0      249 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Marchantia polymorpha_taxonomy
+-rw-rw-rw-   0        0        0      474 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Medicago truncatula_taxonomy
+-rw-rw-rw-   0        0        0      178 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Megalodesulfovibrio gigas_taxonomy
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Megasphaera elsdenii_taxonomy
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Meiothermus ruber_taxonomy
+-rw-rw-rw-   0        0        0      571 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Meleagris gallopavo_taxonomy
+-rw-rw-rw-   0        0        0      512 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mesocricetus auratus_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mesorhizobium loti_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Metacordyceps brittlebankisoides_taxonomy_NA
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Metallosphaera sedula_taxonomy
+-rw-rw-rw-   0        0        0      297 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Metarhizium anisopliae_taxonomy
+-rw-rw-rw-   0        0        0      297 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Metarhizium brittlebankisoides_taxonomy
+-rw-rw-rw-   0        0        0      297 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Metarhizium flavoviride_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanobacterium thermoautotrophicus_taxonomy_NA
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanocaldococcus jannaschii_taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanocella conradii_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanococcus aeolicus_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanococcus maripaludis_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanococcus voltae_taxonomy
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanosarcina acetivorans C2A_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanosarcina acetivorans_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanosarcina mazei_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanosarcina thermophila_taxonomy
+-rw-rw-rw-   0        0        0      190 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanothermobacter thermautotrophicus_taxonomy
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methanothermus fervidus_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methylococcus capsulatus_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methylomonas aminofaciens_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methylomonas methanica_taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methylorubrum extorquens_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methylosinus trichosporium_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Methylotuvimicrobium alcaliphilum_taxonomy
+-rw-rw-rw-   0        0        0      214 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Microbacterium sp._taxonomy
+-rw-rw-rw-   0        0        0      492 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Microcebus murinus_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Micrococcus luteus_taxonomy
+-rw-rw-rw-   0        0        0      246 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Microcystis aeruginosa_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Micromonospora lupini_taxonomy
+-rw-rw-rw-   0        0        0      606 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Micropterus salmoides_taxonomy
+-rw-rw-rw-   0        0        0      412 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mimosa pudica_taxonomy
+-rw-rw-rw-   0        0        0      307 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mizuhopecten yessoensis_taxonomy
+-rw-rw-rw-   0        0        0      165 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Monopylocystis minor_taxonomy
+-rw-rw-rw-   0        0        0      159 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moorella thermoacetica_taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moraxella sp._taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moritella japonica_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moritella marina_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moritella profunda_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moritella sp._taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Moritella yayanosii_taxonomy
+-rw-rw-rw-   0        0        0      238 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mortierella alliacea_taxonomy
+-rw-rw-rw-   0        0        0      238 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mortierella alpina_taxonomy
+-rw-rw-rw-   0        0        0      507 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mus musculus_taxonomy
+-rw-rw-rw-   0        0        0      220 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycobacterium avium_taxonomy
+-rw-rw-rw-   0        0        0      180 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycobacterium leprae_taxonomy
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycobacterium marinum_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycobacterium smegmatis_taxonomy_NA
+-rw-rw-rw-   0        0        0      213 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycobacterium sp._taxonomy
+-rw-rw-rw-   0        0        0      221 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycobacterium tuberculosis_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycolicibacterium smegmatis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycoplasma hyorhinis_taxonomy_NA
+-rw-rw-rw-   0        0        0      206 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycoplasma mycoides_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycoplasma pneumoniae_taxonomy_NA
+-rw-rw-rw-   0        0        0      295 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mycothermus thermophilus_taxonomy
+-rw-rw-rw-   0        0        0      315 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Mytilus galloprovincialis_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Myxococcus xanthus_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Naegleria fowleri_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Natranaerobius thermophilus_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Natronomonas pharaonis_taxonomy
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Neisseria gonorrhoeae_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Neisseria meningitidis serogroup A _ serotype 4A_taxonomy_NA
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Neisseria meningitidis_taxonomy
+-rw-rw-rw-   0        0        0      278 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nelumbo nucifera_taxonomy
+-rw-rw-rw-   0        0        0      200 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Neospora caninum_taxonomy
+-rw-rw-rw-   0        0        0      293 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Neurospora crassa_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Niallia circulans_taxonomy
+-rw-rw-rw-   0        0        0      402 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nicotiana glutinosa_taxonomy
+-rw-rw-rw-   0        0        0      402 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nicotiana tabacum_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nitrosomonas europaea_taxonomy
+-rw-rw-rw-   0        0        0      214 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nocardioides sp. PD653_taxonomy
+-rw-rw-rw-   0        0        0      384 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Noccaea caerulescens_taxonomy
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nonomuraea sp._taxonomy
+-rw-rw-rw-   0        0        0      207 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nostoc punctiforme_taxonomy
+-rw-rw-rw-   0        0        0      233 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nostoc sp. PCC 7120 = FACHB-418_taxonomy
+-rw-rw-rw-   0        0        0      233 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Nostoc sp._taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Novosphingobium aromaticivorans_taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Novosphingobium capsulatum_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oceanobacillus iheyensis_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ochromonas danica_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oenococcus oeni_taxonomy
+-rw-rw-rw-   0        0        0      232 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ogataea angusta_taxonomy
+-rw-rw-rw-   0        0        0      232 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ogataea henricii_taxonomy
+-rw-rw-rw-   0        0        0      289 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Onchocerca volvulus_taxonomy
+-rw-rw-rw-   0        0        0      479 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oncorhynchus keta_taxonomy
+-rw-rw-rw-   0        0        0      479 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oncorhynchus kisutch_taxonomy
+-rw-rw-rw-   0        0        0      479 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oncorhynchus mykiss_taxonomy
+-rw-rw-rw-   0        0        0      371 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Opuntia ficus-indica_taxonomy
+-rw-rw-rw-   0        0        0      464 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oryctolagus cuniculus_taxonomy
+-rw-rw-rw-   0        0        0      403 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oryza sativa Indica Group_taxonomy
+-rw-rw-rw-   0        0        0      403 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oryza sativa Japonica Group_taxonomy
+-rw-rw-rw-   0        0        0      384 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oryza sativa_taxonomy
+-rw-rw-rw-   0        0        0      487 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ovis aries_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Oxalobacter formigenes_taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paenarthrobacter aurescens_taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paenarthrobacter nicotinovorans_taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paenarthrobacter ureafaciens_taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paenibacillus curdlanolyticus_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paenibacillus sp._taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paenibacillus thiaminolyticus_taxonomy
+-rw-rw-rw-   0        0        0      570 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pagrus major_taxonomy
+-rw-rw-rw-   0        0        0      411 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pandalus borealis_taxonomy
+-rw-rw-rw-   0        0        0      408 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Panicum miliaceum_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pantoea agglomerans_taxonomy
+-rw-rw-rw-   0        0        0      300 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Papaver somniferum_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paraburkholderia phenoliruptrix_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paraburkholderia xenovorans LB400_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paraburkholderia xenovorans_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paracoccus denitrificans_taxonomy
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Parageobacillus thermoglucosidasius_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paramecium bursaria Chlorella virus 1_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Paramecium bursaria chlorella virus 1_taxonomy_NA
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pasteurella multocida_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pectobacterium carotovorum subsp. carotovorum_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pectobacterium carotovorum_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pediococcus pentosaceus_taxonomy
+-rw-rw-rw-   0        0        0      228 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pelodictyon luteolum_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pelotomaculum thermopropionicum_taxonomy
+-rw-rw-rw-   0        0        0      399 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Penaeus merguiensis_taxonomy
+-rw-rw-rw-   0        0        0      399 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Penaeus vannamei_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Penicillium brevicompactum_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Penicillium canescens_taxonomy
+-rw-rw-rw-   0        0        0      318 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Penicillium chrysogenum_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Persephonella marina_taxonomy
+-rw-rw-rw-   0        0        0      140 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Petrotoga mobilis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Petunia hybrida_taxonomy_NA
+-rw-rw-rw-   0        0        0      380 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Petunia x hybrida_taxonomy
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Phaffia rhodozyma_taxonomy
+-rw-rw-rw-   0        0        0      255 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Phanerodontia chrysosporium_taxonomy
+-rw-rw-rw-   0        0        0      477 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Phaseolus vulgaris_taxonomy
+-rw-rw-rw-   0        0        0      251 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pholiota nameko_taxonomy
+-rw-rw-rw-   0        0        0      249 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Phormidium lapideum_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Photobacterium leiognathi_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Photobacterium phosphoreum_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Photobacterium profundum_taxonomy
+-rw-rw-rw-   0        0        0      249 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Physcomitrium patens_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Phytophthora capsici_taxonomy
+-rw-rw-rw-   0        0        0      297 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Picea abies_taxonomy
+-rw-rw-rw-   0        0        0      165 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Picrophilus oshimae_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Picrophilus torridus_taxonomy_NA
+-rw-rw-rw-   0        0        0      323 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pinus pinaster_taxonomy
+-rw-rw-rw-   0        0        0      323 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pinus pinea_taxonomy
+-rw-rw-rw-   0        0        0      467 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pisum sativum_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Planococcus sp._taxonomy_NA
+-rw-rw-rw-   0        0        0      195 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium berghei_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium cynomolgi_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium falciparum_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium gallinaceum_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium knowlesi_taxonomy
+-rw-rw-rw-   0        0        0      197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium vivax_taxonomy
+-rw-rw-rw-   0        0        0      195 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Plasmodium yoelii_taxonomy
+-rw-rw-rw-   0        0        0      451 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Platyrrhini_taxonomy
+-rw-rw-rw-   0        0        0      251 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pleurotus eryngii_taxonomy
+-rw-rw-rw-   0        0        0      251 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pleurotus ostreatus_taxonomy
+-rw-rw-rw-   0        0        0      251 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pleurotus sapidus_taxonomy
+-rw-rw-rw-   0        0        0      221 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pneumocystis carinii_taxonomy
+-rw-rw-rw-   0        0        0      221 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pneumocystis jirovecii_taxonomy
+-rw-rw-rw-   0        0        0      376 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Populus deltoides_taxonomy
+-rw-rw-rw-   0        0        0      403 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Populus sp._taxonomy
+-rw-rw-rw-   0        0        0      376 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Populus tremula_taxonomy
+-rw-rw-rw-   0        0        0      376 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Populus trichocarpa_taxonomy
+-rw-rw-rw-   0        0        0      203 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Porphyromonas gingivalis_taxonomy
+-rw-rw-rw-   0        0        0      196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Prevotella intermedia_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Priestia megaterium_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Prosthecobacter sp._taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Proteus mirabilis_taxonomy
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Proteus vulgaris_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Providencia alcalifaciens_taxonomy
+-rw-rw-rw-   0        0        0      411 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Prunella vulgaris_taxonomy
+-rw-rw-rw-   0        0        0      259 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudanabaena sp._taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudoalteromonas haloplanktis_taxonomy
+-rw-rw-rw-   0        0        0      207 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudoalteromonas sp._taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudoclostridium thermosuccinogenes_taxonomy
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas aeruginosa_taxonomy
+-rw-rw-rw-   0        0        0      263 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas amygdali pv. tabaci_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas dacunhae_taxonomy_NA
+-rw-rw-rw-   0        0        0      204 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas denitrificans (nom. rej.)_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas denitrificans_taxonomy_NA
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas fluorescens_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas phage phi6_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas phage phi8_taxonomy
+-rw-rw-rw-   0        0        0      223 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas protegens Pf-5_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas psychrophila_taxonomy
+-rw-rw-rw-   0        0        0      214 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas putida KT2440_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas putida_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas sp. WU-0701_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas sp._taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas stutzeri_taxonomy_NA
+-rw-rw-rw-   0        0        0      236 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas syringae_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudomonas taetrolens_taxonomy
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pseudothermotoga lettingae_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Psychrobacter arcticus_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Psychrobacter cryohalolentis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Psychrobacter sp. ANT206_taxonomy_NA
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Psychrobacter sp. PRwf-1_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Psychromonas ingrahamii_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Psychromonas marina_taxonomy
+-rw-rw-rw-   0        0        0      368 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Putranjiva roxburghii_taxonomy
+-rw-rw-rw-   0        0        0      300 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyricularia grisea_taxonomy
+-rw-rw-rw-   0        0        0      325 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyricularia oryzae 70-15_taxonomy
+-rw-rw-rw-   0        0        0      300 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyricularia oryzae_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrobaculum aerophilum_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrobaculum calidifontis_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrobaculum ferrireducens_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus furiosus_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus horikoshii OT3_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus horikoshii_taxonomy
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus sp._taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus woesei_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus yayanosii_taxonomy
+-rw-rw-rw-   0        0        0      128 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Pyrococcus_taxonomy
+-rw-rw-rw-   0        0        0      509 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Python bivittatus_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ralstonia solanacearum_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rana catesbeiana_taxonomy_NA
+-rw-rw-rw-   0        0        0      271 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rasamsonia emersonii_taxonomy
+-rw-rw-rw-   0        0        0      500 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rattus norvegicus_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhizobium etli_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhizobium leguminosarum_taxonomy
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhizomucor miehei_taxonomy
+-rw-rw-rw-   0        0        0      235 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhizosolenia setigera_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodobacter capsulatus_taxonomy
+-rw-rw-rw-   0        0        0      211 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodococcus erythropolis_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodococcus jostii_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodococcus opacus_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodococcus ruber_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodomicrobium vannielii_taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodopseudomonas palustris_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodopseudomonas viridis_taxonomy_NA
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodospirillum rubrum_taxonomy
+-rw-rw-rw-   0        0        0      202 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodothermus marinus_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Rhodotorula aurantiaca_taxonomy_NA
+-rw-rw-rw-   0        0        0      401 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ricinus communis_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ruegeria pomeroyi_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ruminococcus champanellensis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/SARS coronavirus_taxonomy_NA
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saccharolobus shibatae_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saccharolobus solfataricus_taxonomy
+-rw-rw-rw-   0        0        0      246 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saccharomyces cerevisiae_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saccharomyces kluyveri_taxonomy_NA
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saccharopolyspora erythraea_taxonomy
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saccharopolyspora rectivirgula_taxonomy
+-rw-rw-rw-   0        0        0      515 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saimiri sciureus_taxonomy
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Saitozyma flava_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmo trutta Labrax Coruhensis_taxonomy_NA
+-rw-rw-rw-   0        0        0      228 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella enterica subsp. enterica serovar Typhi_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella enterica subsp. enterica serovar Typhimurium A0A0F6B484 _and_taxonomy_NA
+-rw-rw-rw-   0        0        0      228 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella enterica subsp. enterica serovar Typhimurium_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella enterica typhimurium_taxonomy_NA
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella enterica_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella typhi_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Salmonella typhimurium_taxonomy_NA
+-rw-rw-rw-   0        0        0      564 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Scaptodrosophila lebanonensis_taxonomy
+-rw-rw-rw-   0        0        0      268 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Scheffersomyces stipitis_taxonomy
+-rw-rw-rw-   0        0        0      303 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Schistosoma mansoni_taxonomy
+-rw-rw-rw-   0        0        0      249 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Schizosaccharomyces pombe_taxonomy
+-rw-rw-rw-   0        0        0      357 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Scyliorhinus canicula_taxonomy
+-rw-rw-rw-   0        0        0      228 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Selaginella moellendorffii_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Selenomonas ruminantium_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Semliki Forest virus_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Semliki forest virus_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Serratia marcescens_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Serratia sp._taxonomy_NA
+-rw-rw-rw-   0        0        0      285 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Severe acute respiratory syndrome coronavirus_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shewanella benthica_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shewanella oneidensis_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shewanella sp. T3-3_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shewanella sp._taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shewanella violacea_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shewanella woodyi_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shigella flexneri_taxonomy
+-rw-rw-rw-   0        0        0      111 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Shrimp white spot syndrome virus_taxonomy
+-rw-rw-rw-   0        0        0      191 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sinorhizobium meliloti_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Slackia exigua_taxonomy
+-rw-rw-rw-   0        0        0      394 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Solanum chacoense_taxonomy
+-rw-rw-rw-   0        0        0      429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Solanum lycopersicum_taxonomy
+-rw-rw-rw-   0        0        0      429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Solanum pennellii_taxonomy
+-rw-rw-rw-   0        0        0      394 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Solanum tuberosum_taxonomy
+-rw-rw-rw-   0        0        0      291 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sordaria macrospora_taxonomy
+-rw-rw-rw-   0        0        0      418 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sorghum bicolor_taxonomy
+-rw-rw-rw-   0        0        0      195 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Southampton virus_taxonomy
+-rw-rw-rw-   0        0        0      120 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Spbetavirus SPbeta_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sphingobium chungbukense_taxonomy
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sphingomonas elodea_taxonomy
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sphingomonas sanxanigenens_taxonomy
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sphingomonas sp. A1_taxonomy
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sphingomonas sp. PAMC 26621_taxonomy
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sphingomonas sp._taxonomy
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Spinacia oleracea_taxonomy
+-rw-rw-rw-   0        0        0      516 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Spodoptera frugiperda_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sporolactobacillus inulinus_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sporolactobacillus laevolacticus_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sporomusa ovata_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sporomusa sphaeroides_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Staphylococcus aureus_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Staphylococcus carnosus_taxonomy
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Staphylococcus epidermidis RP62A_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Staphylococcus haemolyticus_taxonomy
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Staphylococcus phage phi 13_taxonomy
+-rw-rw-rw-   0        0        0      200 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Staphylococcus sp._taxonomy
+-rw-rw-rw-   0        0        0      204 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Stenotrophomonas maltophilia_taxonomy
+-rw-rw-rw-   0        0        0      241 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Stereum hirsutum_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus entericus_taxonomy
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus equi_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus gordonii_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus mutans_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus pneumoniae_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus pyogenes_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus suis_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptococcus thermophilus_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces acidiscabies_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces albidoflavus_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces ambofaciens_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces avermitilis_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces canarius_taxonomy
+-rw-rw-rw-   0        0        0      219 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces coelicolor_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces collinus_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces corchorusii_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces davaonensis_taxonomy
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces diastaticus_taxonomy
+-rw-rw-rw-   0        0        0      255 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces globisporus_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces griseochromogenes_taxonomy
+-rw-rw-rw-   0        0        0      250 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces griseus_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces lavendulae_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces lividans_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces murayamaensis_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces pristinaespiralis_taxonomy
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces rubiginosus_taxonomy
+-rw-rw-rw-   0        0        0      213 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces sp. R61_taxonomy
+-rw-rw-rw-   0        0        0      213 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces sp._taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces venezuelae_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces verticillus_taxonomy
+-rw-rw-rw-   0        0        0      220 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces violaceoruber_taxonomy
+-rw-rw-rw-   0        0        0      181 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Streptomyces viridifaciens_taxonomy
+-rw-rw-rw-   0        0        0      327 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Strongylocentrotus purpuratus_taxonomy
+-rw-rw-rw-   0        0        0      541 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Struthio camelus_taxonomy
+-rw-rw-rw-   0        0        0      224 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Stylophora pistillata_taxonomy
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfolobus acidocaldarius_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfolobus shibatae_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfolobus solfataricus_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfolobus tokodaii_taxonomy_NA
+-rw-rw-rw-   0        0        0      152 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfurihydrogenibium azorense_taxonomy
+-rw-rw-rw-   0        0        0      192 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfurihydrogenibium sp. YO3AOP1_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfurimonas denitrificans_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfurisphaera tokodaii str. 7_taxonomy
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sulfurisphaera tokodaii_taxonomy
+-rw-rw-rw-   0        0        0      469 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sus scrofa domesticus_taxonomy
+-rw-rw-rw-   0        0        0      452 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Sus scrofa_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Symbiobacterium thermophilum_taxonomy
+-rw-rw-rw-   0        0        0      174 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Symbiobacterium toebii_taxonomy
+-rw-rw-rw-   0        0        0      254 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechococcus elongatus PCC 7942 = FACHB-805_taxonomy
+-rw-rw-rw-   0        0        0      224 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechococcus elongatus_taxonomy
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechococcus phage S-PM2_taxonomy
+-rw-rw-rw-   0        0        0      257 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechococcus sp. PCC 7002_taxonomy
+-rw-rw-rw-   0        0        0      257 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechococcus sp._taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechocystis sp. PCC 6803 _ Kazusa_taxonomy_NA
+-rw-rw-rw-   0        0        0      257 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechocystis sp. PCC 6803_taxonomy
+-rw-rw-rw-   0        0        0      257 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Synechocystis sp._taxonomy
+-rw-rw-rw-   0        0        0      270 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Taenia crassiceps_taxonomy
+-rw-rw-rw-   0        0        0      270 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Taenia solium_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Talaromyces emersonii_taxonomy_NA
+-rw-rw-rw-   0        0        0      306 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Talaromyces piceae_taxonomy
+-rw-rw-rw-   0        0        0      308 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Talaromyces pinophilus_taxonomy
+-rw-rw-rw-   0        0        0      447 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Tenebrio molitor_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Tetragenococcus halophilus_taxonomy
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Tetrahymena thermophila_taxonomy
+-rw-rw-rw-   0        0        0      239 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thalassiosira pseudonana_taxonomy
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Theileria annulata_taxonomy
+-rw-rw-rw-   0        0        0      191 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoanaerobacter brockii_taxonomy
+-rw-rw-rw-   0        0        0      229 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoanaerobacter sp._taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoanaerobacter tengcongensis_taxonomy_NA
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoanaerobacterium saccharolyticum_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoanaerobacterium thermosaccharolyticum_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoanaerobacterium thermosulfurigenes_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoascus aurantiacus_taxonomy
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermobifida fusca_taxonomy
+-rw-rw-rw-   0        0        0      147 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus gammatolerans_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus kodakaraensis_taxonomy_NA
+-rw-rw-rw-   0        0        0      147 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus kodakarensis_taxonomy
+-rw-rw-rw-   0        0        0      147 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus litoralis_taxonomy
+-rw-rw-rw-   0        0        0      147 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus onnurineus_taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus sp._taxonomy
+-rw-rw-rw-   0        0        0      147 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermococcus waiotapuensis_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermocrispum agreste_taxonomy
+-rw-rw-rw-   0        0        0      217 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermocrispum sp. RD004668_taxonomy
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermodesulfobium narugense_taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermofilum pendens_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermomicrobium roseum_taxonomy
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermomonospora curvata_taxonomy
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermomyces lanuginosus_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoplasma acidophilum_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoplasma volcanium_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoproteus tenax_taxonomy
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermoproteus uzoniensis_taxonomy
+-rw-rw-rw-   0        0        0      237 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermosynechococcus vestitus_taxonomy
+-rw-rw-rw-   0        0        0      143 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermotoga maritima_taxonomy
+-rw-rw-rw-   0        0        0      143 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermotoga neapolitana_taxonomy
+-rw-rw-rw-   0        0        0      155 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermovibrio ammonificans_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus aquaticus_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus brockianus_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus caldophilus_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus sp. GH5_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus sp. NTU-237_taxonomy_NA
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus sp._taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus thermophilus HB27_taxonomy
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus thermophilus HB8_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus thermophilus_taxonomy
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thermus yunnanensis_taxonomy
+-rw-rw-rw-   0        0        0      191 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thiobacillus denitrificans ATCC 25259_taxonomy
+-rw-rw-rw-   0        0        0      607 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Thunnus thynnus_taxonomy
+-rw-rw-rw-   0        0        0      304 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Tolypocladium inflatum_taxonomy
+-rw-rw-rw-   0        0        0      202 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Toxoplasma gondii_taxonomy
+-rw-rw-rw-   0        0        0      600 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trematomus bernacchii_taxonomy
+-rw-rw-rw-   0        0        0      146 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Treponema denticola_taxonomy
+-rw-rw-rw-   0        0        0      294 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trichoderma reesei_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trichomonas vaginalis_taxonomy
+-rw-rw-rw-   0        0        0      211 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trichormus azollae_taxonomy
+-rw-rw-rw-   0        0        0      406 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Triticum aestivum_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Tritrichomonas foetus_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Tritrichomonas suis_taxonomy
+-rw-rw-rw-   0        0        0      231 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trypanosoma brucei brucei_taxonomy
+-rw-rw-rw-   0        0        0      206 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trypanosoma brucei_taxonomy
+-rw-rw-rw-   0        0        0      205 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trypanosoma congolense_taxonomy
+-rw-rw-rw-   0        0        0      209 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trypanosoma cruzi_taxonomy
+-rw-rw-rw-   0        0        0      205 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trypanosoma vivax_taxonomy
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Trypanosoma_taxonomy
+-rw-rw-rw-   0        0        0      301 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Turbatrix aceti_taxonomy
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Ureibacillus thermosphaericus_taxonomy
+-rw-rw-rw-   0        0        0      511 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Urocitellus richardsonii_taxonomy
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vaccinia virus_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Variovorax paradoxus_taxonomy
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Veillonella atypica_taxonomy
+-rw-rw-rw-   0        0        0      167 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio cholerae O1_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio cholerae serotype O1_taxonomy_NA
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio cholerae_taxonomy
+-rw-rw-rw-   0        0        0      172 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio harveyi_taxonomy
+-rw-rw-rw-   0        0        0      172 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio natriegens_taxonomy
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio sp._taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio splendidus_taxonomy
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vibrio vulnificus_taxonomy
+-rw-rw-rw-   0        0        0      473 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vigna radiata_taxonomy
+-rw-rw-rw-   0        0        0      380 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vitis vinifera_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vogesella indigofera_taxonomy
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Vulcanisaeta moutnovskia_taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Weizmannia coagulans_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/West Nile virus_taxonomy
+-rw-rw-rw-   0        0        0       79 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/White spot syndrome virus_taxonomy
+-rw-rw-rw-   0        0        0      396 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Withania somnifera_taxonomy
+-rw-rw-rw-   0        0        0      200 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Wolbachia endosymbiont of Brugia malayi_taxonomy
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Wolbachia pipientis_taxonomy
+-rw-rw-rw-   0        0        0      200 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Wolbachia sp._taxonomy
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Wolinella succinogenes_taxonomy
+-rw-rw-rw-   0        0        0      289 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Wuchereria bancrofti_taxonomy
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xanthomonas campestris pv. campestris_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xanthomonas campestris_taxonomy
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xanthomonas citri_taxonomy
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xanthomonas oryzae_taxonomy
+-rw-rw-rw-   0        0        0      185 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xanthomonas phaseoli pv. manihotis_taxonomy
+-rw-rw-rw-   0        0        0      418 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xenopus laevis_taxonomy
+-rw-rw-rw-   0        0        0      317 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xerophyta viscosa_taxonomy
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Xylella fastidiosa_taxonomy
+-rw-rw-rw-   0        0        0      263 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Yamadazyma tenuis_taxonomy
+-rw-rw-rw-   0        0        0      236 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Yarrowia lipolytica_taxonomy
+-rw-rw-rw-   0        0        0      152 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Yersinia intermedia_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Yersinia pestis_taxonomy
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Yersinia pseudotuberculosis_taxonomy
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Yokenella sp._taxonomy
+-rw-rw-rw-   0        0        0      156 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Zavarzinia compransoris_taxonomy
+-rw-rw-rw-   0        0        0      416 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Zea mays_taxonomy
+-rw-rw-rw-   0        0        0      148 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Zoogloea ramigera_taxonomy
+-rw-rw-rw-   0        0        0      239 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Zunongwangia sp._taxonomy
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/Zymomonas mobilis subsp. mobilis_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/[Bacillus] caldotenax_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/[Candida] glabrata_taxonomy_NA
+-rw-rw-rw-   0        0        0      317 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/[Candida] intermedia_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/equine infectious anemia virus_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/mammalian orthoreovirus_taxonomy_NA
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/plant_taxonomy_NA
+-rw-rw-rw-   0        0        0       77 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/synthetic construct_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured Acidobacteria bacterium_taxonomy_NA
+-rw-rw-rw-   0        0        0       98 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured Acidobacteriota bacterium_taxonomy
+-rw-rw-rw-   0        0        0       75 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured archaeon_taxonomy
+-rw-rw-rw-   0        0        0       76 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured bacterium_taxonomy
+-rw-rw-rw-   0        0        0       92 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured microorganism_taxonomy
+-rw-rw-rw-   0        0        0       76 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured rumen bacterium_taxonomy
+-rw-rw-rw-   0        0        0       76 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/uncultured soil bacterium_taxonomy
+-rw-rw-rw-   0        0        0       64 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/unidentified_taxonomy
+-rw-rw-rw-   0        0        0       23 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/ncbi_taxonomy/white spot syndrome virus_taxonomy_NA
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.153490 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/
+-rw-rw-rw-   0        0        0      846 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_10_3_1.json
+-rw-rw-rw-   0        0        0      312 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_10_5_1.json
+-rw-rw-rw-   0        0        0      802 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_1.json
+-rw-rw-rw-   0        0        0      427 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_15.json
+-rw-rw-rw-   0        0        0      494 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_16.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_21.json
+-rw-rw-rw-   0        0        0     1974 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_6.json
+-rw-rw-rw-   0        0        0     1914 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_7.json
+-rw-rw-rw-   0        0        0      408 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_1_9.json
+-rw-rw-rw-   0        0        0      480 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_11_2_1.json
+-rw-rw-rw-   0        0        0      168 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_11_1.json
+-rw-rw-rw-   0        0        0      137 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_11_15.json
+-rw-rw-rw-   0        0        0      103 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_11_16.json
+-rw-rw-rw-   0        0        0      395 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_11_4.json
+-rw-rw-rw-   0        0        0       88 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_11_49.json
+-rw-rw-rw-   0        0        0     2701 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_11_52.json
+-rw-rw-rw-   0        0        0      543 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_12_16.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_12_7.json
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_13_99_1.json
+-rw-rw-rw-   0        0        0      203 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_11_17.json
+-rw-rw-rw-   0        0        0      919 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_12_17.json
+-rw-rw-rw-   0        0        0      412 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_13_7.json
+-rw-rw-rw-   0        0        0      385 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_13_8.json
+-rw-rw-rw-   0        0        0     3982 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_14_1.json
+-rw-rw-rw-   0        0        0      919 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_14_19.json
+-rw-rw-rw-   0        0        0      198 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_14_38.json
+-rw-rw-rw-   0        0        0      425 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_15_15.json
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_15_16.json
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_16_1.json
+-rw-rw-rw-   0        0        0      306 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_16_4.json
+-rw-rw-rw-   0        0        0      176 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_17_4.json
+-rw-rw-rw-   0        0        0     1144 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_18_1.json
+-rw-rw-rw-   0        0        0      327 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_20_1.json
+-rw-rw-rw-   0        0        0      274 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_99_1.json
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_14_99_51.json
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_16_1_7.json
+-rw-rw-rw-   0        0        0       83 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_16_1_8.json
+-rw-rw-rw-   0        0        0      833 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_16_3_1.json
+-rw-rw-rw-   0        0        0       94 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_17_1_4.json
+-rw-rw-rw-   0        0        0      281 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_17_3_2.json
+-rw-rw-rw-   0        0        0      296 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_18_1_1.json
+-rw-rw-rw-   0        0        0    13484 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_1.json
+-rw-rw-rw-   0        0        0      101 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_100.json
+-rw-rw-rw-   0        0        0      245 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_103.json
+-rw-rw-rw-   0        0        0      359 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_133.json
+-rw-rw-rw-   0        0        0      106 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_169.json
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_17.json
+-rw-rw-rw-   0        0        0      204 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_193.json
+-rw-rw-rw-   0        0        0     1289 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_205.json
+-rw-rw-rw-   0        0        0     8934 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_21.json
+-rw-rw-rw-   0        0        0       91 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_215.json
+-rw-rw-rw-   0        0        0      442 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_22.json
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_23.json
+-rw-rw-rw-   0        0        0      308 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_25.json
+-rw-rw-rw-   0        0        0      359 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_267.json
+-rw-rw-rw-   0        0        0     2177 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_28.json
+-rw-rw-rw-   0        0        0      499 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_282.json
+-rw-rw-rw-   0        0        0      363 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_284.json
+-rw-rw-rw-   0        0        0      336 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_3.json
+-rw-rw-rw-   0        0        0      101 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_336.json
+-rw-rw-rw-   0        0        0      449 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_35.json
+-rw-rw-rw-   0        0        0     2132 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_37.json
+-rw-rw-rw-   0        0        0      651 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_38.json
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_383.json
+-rw-rw-rw-   0        0        0      473 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_39.json
+-rw-rw-rw-   0        0        0      340 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_399.json
+-rw-rw-rw-   0        0        0      233 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_4.json
+-rw-rw-rw-   0        0        0     1659 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_40.json
+-rw-rw-rw-   0        0        0      781 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_41.json
+-rw-rw-rw-   0        0        0     2902 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_42.json
+-rw-rw-rw-   0        0        0     1137 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_44.json
+-rw-rw-rw-   0        0        0      921 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_49.json
+-rw-rw-rw-   0        0        0     1645 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_51.json
+-rw-rw-rw-   0        0        0      362 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_6.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_60.json
+-rw-rw-rw-   0        0        0      740 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_72.json
+-rw-rw-rw-   0        0        0      186 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_79.json
+-rw-rw-rw-   0        0        0      264 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_8.json
+-rw-rw-rw-   0        0        0      165 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_81.json
+-rw-rw-rw-   0        0        0      194 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_85.json
+-rw-rw-rw-   0        0        0      678 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_86.json
+-rw-rw-rw-   0        0        0      590 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_1_95.json
+-rw-rw-rw-   0        0        0      350 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_2_3.json
+-rw-rw-rw-   0        0        0      758 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_2_7.json
+-rw-rw-rw-   0        0        0       97 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_2_8.json
+-rw-rw-rw-   0        0        0      414 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_3_15.json
+-rw-rw-rw-   0        0        0      272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_3_21.json
+-rw-rw-rw-   0        0        0      400 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_3_38.json
+-rw-rw-rw-   0        0        0      868 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_3_4.json
+-rw-rw-rw-   0        0        0      365 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_3_7.json
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_1_9_1.json
+-rw-rw-rw-   0        0        0      200 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_20_1_1.json
+-rw-rw-rw-   0        0        0      130 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_20_4_1.json
+-rw-rw-rw-   0        0        0      111 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_20_4_4.json
+-rw-rw-rw-   0        0        0      105 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_21_3_1.json
+-rw-rw-rw-   0        0        0      605 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_10.json
+-rw-rw-rw-   0        0        0     1178 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_11.json
+-rw-rw-rw-   0        0        0     1193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_12.json
+-rw-rw-rw-   0        0        0      282 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_19.json
+-rw-rw-rw-   0        0        0      190 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_22.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_24.json
+-rw-rw-rw-   0        0        0     3842 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_3.json
+-rw-rw-rw-   0        0        0      567 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_39.json
+-rw-rw-rw-   0        0        0      621 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_4.json
+-rw-rw-rw-   0        0        0      428 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_5.json
+-rw-rw-rw-   0        0        0       97 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_59.json
+-rw-rw-rw-   0        0        0      109 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_70.json
+-rw-rw-rw-   0        0        0      281 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_72.json
+-rw-rw-rw-   0        0        0       95 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_79.json
+-rw-rw-rw-   0        0        0       76 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_1_88.json
+-rw-rw-rw-   0        0        0      243 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_3_1.json
+-rw-rw-rw-   0        0        0       81 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_3_4.json
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_4_1 2_3_1_12 1_8_1_4.json
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_4_1.json
+-rw-rw-rw-   0        0        0      119 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_4_2 2_3_1_61 1_8_1_4.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_4_2.json
+-rw-rw-rw-   0        0        0      179 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_4_4.json
+-rw-rw-rw-   0        0        0      115 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_98_1.json
+-rw-rw-rw-   0        0        0      188 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_2_99_7.json
+-rw-rw-rw-   0        0        0      332 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_1.json
+-rw-rw-rw-   0        0        0      231 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_10.json
+-rw-rw-rw-   0        0        0      120 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_12.json
+-rw-rw-rw-   0        0        0      570 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_3.json
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_38.json
+-rw-rw-rw-   0        0        0       91 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_6.json
+-rw-rw-rw-   0        0        0      101 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_84.json
+-rw-rw-rw-   0        0        0      274 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_9.json
+-rw-rw-rw-   0        0        0      758 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_1_98.json
+-rw-rw-rw-   0        0        0      306 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_2_3.json
+-rw-rw-rw-   0        0        0      354 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_3_4.json
+-rw-rw-rw-   0        0        0      826 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_5_1.json
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_5_3.json
+-rw-rw-rw-   0        0        0      114 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_7_8.json
+-rw-rw-rw-   0        0        0      585 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_8_1.json
+-rw-rw-rw-   0        0        0      308 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_8_4.json
+-rw-rw-rw-   0        0        0      316 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_8_6.json
+-rw-rw-rw-   0        0        0     1290 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_8_7.json
+-rw-rw-rw-   0        0        0      731 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_8_8.json
+-rw-rw-rw-   0        0        0      575 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_3_98_1.json
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_1.json
+-rw-rw-rw-   0        0        0       87 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_13.json
+-rw-rw-rw-   0        0        0      774 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_2.json
+-rw-rw-rw-   0        0        0      218 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_21.json
+-rw-rw-rw-   0        0        0      981 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_3.json
+-rw-rw-rw-   0        0        0      323 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_4.json
+-rw-rw-rw-   0        0        0      110 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_1_8.json
+-rw-rw-rw-   0        0        0      736 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_3_1.json
+-rw-rw-rw-   0        0        0     5355 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_3_2.json
+-rw-rw-rw-   0        0        0      328 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_3_21.json
+-rw-rw-rw-   0        0        0      290 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_3_4.json
+-rw-rw-rw-   0        0        0       98 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_3_5.json
+-rw-rw-rw-   0        0        0      516 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_9_1.json
+-rw-rw-rw-   0        0        0      102 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_4_9_2.json
+-rw-rw-rw-   0        0        0      688 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_1.json
+-rw-rw-rw-   0        0        0      112 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_2.json
+-rw-rw-rw-   0        0        0      451 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_20.json
+-rw-rw-rw-   0        0        0      380 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_21.json
+-rw-rw-rw-   0        0        0     2233 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_3.json
+-rw-rw-rw-   0        0        0      376 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_30.json
+-rw-rw-rw-   0        0        0      425 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_34.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_36.json
+-rw-rw-rw-   0        0        0      213 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_37.json
+-rw-rw-rw-   0        0        0       78 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_38.json
+-rw-rw-rw-   0        0        0      106 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_39.json
+-rw-rw-rw-   0        0        0     2434 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_49.json
+-rw-rw-rw-   0        0        0      321 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_5.json
+-rw-rw-rw-   0        0        0      122 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_52.json
+-rw-rw-rw-   0        0        0      711 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_1_7.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_98_2.json
+-rw-rw-rw-   0        0        0      749 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_5_99_12.json
+-rw-rw-rw-   0        0        0      556 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_2_2.json
+-rw-rw-rw-   0        0        0      590 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_2_4.json
+-rw-rw-rw-   0        0        0      350 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_3_1.json
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_3_4.json
+-rw-rw-rw-   0        0        0     1101 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_5_2.json
+-rw-rw-rw-   0        0        0       99 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_5_5.json
+-rw-rw-rw-   0        0        0      152 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_99_1.json
+-rw-rw-rw-   0        0        0      956 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_6_99_3.json
+-rw-rw-rw-   0        0        0      102 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_7_1_13.json
+-rw-rw-rw-   0        0        0      247 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_7_1_14.json
+-rw-rw-rw-   0        0        0      470 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_7_2_1.json
+-rw-rw-rw-   0        0        0       99 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_7_3_1.json
+-rw-rw-rw-   0        0        0       89 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_7_3_3.json
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_1_16.json
+-rw-rw-rw-   0        0        0      639 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_1_4.json
+-rw-rw-rw-   0        0        0      366 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_1_7.json
+-rw-rw-rw-   0        0        0     1586 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_1_9.json
+-rw-rw-rw-   0        0        0      146 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_2_1.json
+-rw-rw-rw-   0        0        0       89 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_2_2.json
+-rw-rw-rw-   0        0        0      482 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_3_1.json
+-rw-rw-rw-   0        0        0       85 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_4_11.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_4_13.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_4_14.json
+-rw-rw-rw-   0        0        0      202 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_4_2.json
+-rw-rw-rw-   0        0        0      245 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_8_5_1.json
+-rw-rw-rw-   0        0        0      407 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/1_9_3_1.json
+-rw-rw-rw-   0        0        0       88 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_10.json
+-rw-rw-rw-   0        0        0      125 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_107.json
+-rw-rw-rw-   0        0        0       88 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_11.json
+-rw-rw-rw-   0        0        0       99 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_13.json
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_2.json
+-rw-rw-rw-   0        0        0     1042 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_45.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_6.json
+-rw-rw-rw-   0        0        0      109 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_72.json
+-rw-rw-rw-   0        0        0      178 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_1_79.json
+-rw-rw-rw-   0        0        0     2326 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_2_1.json
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_2_2.json
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_3_2.json
+-rw-rw-rw-   0        0        0     1474 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_1_3_3.json
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_2_1_1.json
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_2_1_6.json
+-rw-rw-rw-   0        0        0      302 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_2_1_7.json
+-rw-rw-rw-   0        0        0      251 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_2_1_9 4_2_99_20.json
+-rw-rw-rw-   0        0        0      114 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_2_1_9.json
+-rw-rw-rw-   0        0        0      146 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_1.json
+-rw-rw-rw-   0        0        0      117 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_117.json
+-rw-rw-rw-   0        0        0      610 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_157.json
+-rw-rw-rw-   0        0        0      153 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_16.json
+-rw-rw-rw-   0        0        0       91 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_174.json
+-rw-rw-rw-   0        0        0       98 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_191.json
+-rw-rw-rw-   0        0        0       81 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_241.json
+-rw-rw-rw-   0        0        0      872 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_30.json
+-rw-rw-rw-   0        0        0      269 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_38.json
+-rw-rw-rw-   0        0        0      189 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_39.json
+-rw-rw-rw-   0        0        0      266 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_4.json
+-rw-rw-rw-   0        0        0      199 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_41.json
+-rw-rw-rw-   0        0        0      529 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_46.json
+-rw-rw-rw-   0        0        0      290 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_47.json
+-rw-rw-rw-   0        0        0       90 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_57.json
+-rw-rw-rw-   0        0        0       76 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_6.json
+-rw-rw-rw-   0        0        0      778 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_74.json
+-rw-rw-rw-   0        0        0      334 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_8.json
+-rw-rw-rw-   0        0        0      124 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_85.json
+-rw-rw-rw-   0        0        0      258 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_87.json
+-rw-rw-rw-   0        0        0      533 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_1_9.json
+-rw-rw-rw-   0        0        0       79 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_2_15.json
+-rw-rw-rw-   0        0        0      530 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_3_1.json
+-rw-rw-rw-   0        0        0     1252 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_3_13.json
+-rw-rw-rw-   0        0        0      439 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_3_16.json
+-rw-rw-rw-   0        0        0      105 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_3_3_5.json
+-rw-rw-rw-   0        0        0      437 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_1.json
+-rw-rw-rw-   0        0        0      345 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_13.json
+-rw-rw-rw-   0        0        0      301 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_17.json
+-rw-rw-rw-   0        0        0      446 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_19.json
+-rw-rw-rw-   0        0        0      108 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_227.json
+-rw-rw-rw-   0        0        0      429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_25.json
+-rw-rw-rw-   0        0        0      192 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_1_4.json
+-rw-rw-rw-   0        0        0      238 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_1.json
+-rw-rw-rw-   0        0        0      425 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_10.json
+-rw-rw-rw-   0        0        0       81 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_12.json
+-rw-rw-rw-   0        0        0      108 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_18.json
+-rw-rw-rw-   0        0        0      104 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_29.json
+-rw-rw-rw-   0        0        0      881 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_8.json
+-rw-rw-rw-   0        0        0      226 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_2_9.json
+-rw-rw-rw-   0        0        0       81 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_4_99_1.json
+-rw-rw-rw-   0        0        0      382 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_10.json
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_15.json
+-rw-rw-rw-   0        0        0      222 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_16.json
+-rw-rw-rw-   0        0        0      811 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_17.json
+-rw-rw-rw-   0        0        0      512 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_19.json
+-rw-rw-rw-   0        0        0      641 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_29.json
+-rw-rw-rw-   0        0        0      130 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_31.json
+-rw-rw-rw-   0        0        0     2197 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_47.json
+-rw-rw-rw-   0        0        0      456 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_48.json
+-rw-rw-rw-   0        0        0      788 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_54.json
+-rw-rw-rw-   0        0        0      764 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_55.json
+-rw-rw-rw-   0        0        0      101 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_58.json
+-rw-rw-rw-   0        0        0       89 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_6.json
+-rw-rw-rw-   0        0        0      193 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_7.json
+-rw-rw-rw-   0        0        0       87 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_9.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_5_1_90.json
+-rw-rw-rw-   0        0        0      845 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_1.json
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_11.json
+-rw-rw-rw-   0        0        0      112 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_16.json
+-rw-rw-rw-   0        0        0      535 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_19.json
+-rw-rw-rw-   0        0        0      538 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_2.json
+-rw-rw-rw-   0        0        0      566 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_39.json
+-rw-rw-rw-   0        0        0      134 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_42.json
+-rw-rw-rw-   0        0        0      378 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_5.json
+-rw-rw-rw-   0        0        0      327 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_52.json
+-rw-rw-rw-   0        0        0      202 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_62.json
+-rw-rw-rw-   0        0        0      644 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_85.json
+-rw-rw-rw-   0        0        0      373 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_6_1_9.json
+-rw-rw-rw-   0        0        0      326 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_10_2.json
+-rw-rw-rw-   0        0        0      404 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_11_1.json
+-rw-rw-rw-   0        0        0      478 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_11_10.json
+-rw-rw-rw-   0        0        0       81 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_11_11.json
+-rw-rw-rw-   0        0        0       94 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_11_4.json
+-rw-rw-rw-   0        0        0      464 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_13_3.json
+-rw-rw-rw-   0        0        0     1822 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_1.json
+-rw-rw-rw-   0        0        0      213 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_107.json
+-rw-rw-rw-   0        0        0     1521 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_11.json
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_121.json
+-rw-rw-rw-   0        0        0      292 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_13.json
+-rw-rw-rw-   0        0        0      374 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_145.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_165.json
+-rw-rw-rw-   0        0        0       83 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_17.json
+-rw-rw-rw-   0        0        0     1905 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_2.json
+-rw-rw-rw-   0        0        0      107 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_20.json
+-rw-rw-rw-   0        0        0      816 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_21.json
+-rw-rw-rw-   0        0        0      404 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_23.json
+-rw-rw-rw-   0        0        0      235 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_24.json
+-rw-rw-rw-   0        0        0      123 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_26.json
+-rw-rw-rw-   0        0        0      406 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_29.json
+-rw-rw-rw-   0        0        0      510 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_3.json
+-rw-rw-rw-   0        0        0       82 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_31.json
+-rw-rw-rw-   0        0        0      748 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_33.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_35.json
+-rw-rw-rw-   0        0        0      477 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_39.json
+-rw-rw-rw-   0        0        0      203 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_4.json
+-rw-rw-rw-   0        0        0     2563 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_40.json
+-rw-rw-rw-   0        0        0       87 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_49.json
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_55.json
+-rw-rw-rw-   0        0        0      296 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_59.json
+-rw-rw-rw-   0        0        0      338 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_6.json
+-rw-rw-rw-   0        0        0      357 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_60.json
+-rw-rw-rw-   0        0        0      132 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_63.json
+-rw-rw-rw-   0        0        0      244 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_71.json
+-rw-rw-rw-   0        0        0      269 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_1_74.json
+-rw-rw-rw-   0        0        0      686 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_2_1.json
+-rw-rw-rw-   0        0        0      180 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_2_15.json
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_2_2.json
+-rw-rw-rw-   0        0        0     2705 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_2_3.json
+-rw-rw-rw-   0        0        0      644 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_2_4.json
+-rw-rw-rw-   0        0        0      110 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_3_13.json
+-rw-rw-rw-   0        0        0      225 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_3_2.json
+-rw-rw-rw-   0        0        0      239 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_3_3.json
+-rw-rw-rw-   0        0        0      388 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_3_9.json
+-rw-rw-rw-   0        0        0      150 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_1.json
+-rw-rw-rw-   0        0        0      685 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_14.json
+-rw-rw-rw-   0        0        0      529 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_22.json
+-rw-rw-rw-   0        0        0      452 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_25.json
+-rw-rw-rw-   0        0        0      670 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_3.json
+-rw-rw-rw-   0        0        0      162 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_6.json
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_8.json
+-rw-rw-rw-   0        0        0      151 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_4_9.json
+-rw-rw-rw-   0        0        0      293 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_6_5.json
+-rw-rw-rw-   0        0        0     1184 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_1.json
+-rw-rw-rw-   0        0        0      164 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_12.json
+-rw-rw-rw-   0        0        0      362 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_18.json
+-rw-rw-rw-   0        0        0       78 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_2.json
+-rw-rw-rw-   0        0        0      596 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_23.json
+-rw-rw-rw-   0        0        0      150 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_24.json
+-rw-rw-rw-   0        0        0      346 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_27.json
+-rw-rw-rw-   0        0        0      345 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_3.json
+-rw-rw-rw-   0        0        0      134 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_38.json
+-rw-rw-rw-   0        0        0      917 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_4.json
+-rw-rw-rw-   0        0        0      300 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_48.json
+-rw-rw-rw-   0        0        0      621 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_59.json
+-rw-rw-rw-   0        0        0      201 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_60.json
+-rw-rw-rw-   0        0        0      116 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_62.json
+-rw-rw-rw-   0        0        0      648 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_69.json
+-rw-rw-rw-   0        0        0     1061 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_7_7.json
+-rw-rw-rw-   0        0        0      150 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_8_12.json
+-rw-rw-rw-   0        0        0      107 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_8_13.json
+-rw-rw-rw-   0        0        0      489 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_8_7.json
+-rw-rw-rw-   0        0        0      537 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_9_1.json
+-rw-rw-rw-   0        0        0      234 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_7_9_2.json
+-rw-rw-rw-   0        0        0      324 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_1_1.json
+-rw-rw-rw-   0        0        0      258 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_1_2.json
+-rw-rw-rw-   0        0        0      140 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_1_6.json
+-rw-rw-rw-   0        0        0      215 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_2_2.json
+-rw-rw-rw-   0        0        0       82 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_2_21.json
+-rw-rw-rw-   0        0        0      187 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_2_8.json
+-rw-rw-rw-   0        0        0       93 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_3_6.json
+-rw-rw-rw-   0        0        0      204 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_8_4_2.json
+-rw-rw-rw-   0        0        0      113 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/2_9_1_3.json
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_11_2.json
+-rw-rw-rw-   0        0        0      180 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_1_102.json
+-rw-rw-rw-   0        0        0      133 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_1_14.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_1_2.json
+-rw-rw-rw-   0        0        0       78 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_1_31.json
+-rw-rw-rw-   0        0        0      201 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_1_73.json
+-rw-rw-rw-   0        0        0      226 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_26_5.json
+-rw-rw-rw-   0        0        0      327 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_2_12.json
+-rw-rw-rw-   0        0        0     1044 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_2_2.json
+-rw-rw-rw-   0        0        0      171 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_2_4.json
+-rw-rw-rw-   0        0        0     1315 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_2_6.json
+-rw-rw-rw-   0        0        0      498 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_1.json
+-rw-rw-rw-   0        0        0      132 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_104.json
+-rw-rw-rw-   0        0        0     1426 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_11.json
+-rw-rw-rw-   0        0        0      331 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_18.json
+-rw-rw-rw-   0        0        0     3369 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_2.json
+-rw-rw-rw-   0        0        0      678 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_25.json
+-rw-rw-rw-   0        0        0      151 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_3.json
+-rw-rw-rw-   0        0        0      104 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_45.json
+-rw-rw-rw-   0        0        0       82 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_46.json
+-rw-rw-rw-   0        0        0     1258 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_5.json
+-rw-rw-rw-   0        0        0       98 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_6.json
+-rw-rw-rw-   0        0        0      286 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_7.json
+-rw-rw-rw-   0        0        0      112 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_74.json
+-rw-rw-rw-   0        0        0      450 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_89.json
+-rw-rw-rw-   0        0        0      421 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_91.json
+-rw-rw-rw-   0        0        0      351 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_3_97.json
+-rw-rw-rw-   0        0        0      360 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_4_12.json
+-rw-rw-rw-   0        0        0      283 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_4_16.json
+-rw-rw-rw-   0        0        0      396 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_4_17.json
+-rw-rw-rw-   0        0        0      173 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_4_35.json
+-rw-rw-rw-   0        0        0      274 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_4_4.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_5_1.json
+-rw-rw-rw-   0        0        0      331 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_7_2.json
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_1_8_2.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_10.json
+-rw-rw-rw-   0        0        0      663 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_122.json
+-rw-rw-rw-   0        0        0      774 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_14.json
+-rw-rw-rw-   0        0        0      256 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_2.json
+-rw-rw-rw-   0        0        0     2132 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_20.json
+-rw-rw-rw-   0        0        0      209 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_22.json
+-rw-rw-rw-   0        0        0     1986 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_23.json
+-rw-rw-rw-   0        0        0      279 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_28.json
+-rw-rw-rw-   0        0        0     1271 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_3.json
+-rw-rw-rw-   0        0        0      248 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_4.json
+-rw-rw-rw-   0        0        0      526 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_74.json
+-rw-rw-rw-   0        0        0      613 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_8.json
+-rw-rw-rw-   0        0        0      227 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_1_86.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_2_1.json
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_2_2_9.json
+-rw-rw-rw-   0        0        0      228 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_3_2_1.json
+-rw-rw-rw-   0        0        0      897 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_11_1.json
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_11_14.json
+-rw-rw-rw-   0        0        0      151 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_11_2.json
+-rw-rw-rw-   0        0        0      125 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_11_23.json
+-rw-rw-rw-   0        0        0       77 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_13_18.json
+-rw-rw-rw-   0        0        0      284 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_16_4.json
+-rw-rw-rw-   0        0        0      118 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_17_22.json
+-rw-rw-rw-   0        0        0      146 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_4_21_22.json
+-rw-rw-rw-   0        0        0      288 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_1.json
+-rw-rw-rw-   0        0        0      102 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_108.json
+-rw-rw-rw-   0        0        0      827 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_11.json
+-rw-rw-rw-   0        0        0      136 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_116.json
+-rw-rw-rw-   0        0        0      729 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_16.json
+-rw-rw-rw-   0        0        0       89 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_17.json
+-rw-rw-rw-   0        0        0      483 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_18.json
+-rw-rw-rw-   0        0        0      434 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_2.json
+-rw-rw-rw-   0        0        0     1334 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_4.json
+-rw-rw-rw-   0        0        0      158 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_5.json
+-rw-rw-rw-   0        0        0       87 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_1_78.json
+-rw-rw-rw-   0        0        0       81 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_2_17.json
+-rw-rw-rw-   0        0        0      583 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_2_3.json
+-rw-rw-rw-   0        0        0      323 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_2_5.json
+-rw-rw-rw-   0        0        0      897 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_3_1.json
+-rw-rw-rw-   0        0        0      216 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_3_13.json
+-rw-rw-rw-   0        0        0      111 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_3_18.json
+-rw-rw-rw-   0        0        0       95 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_3_4.json
+-rw-rw-rw-   0        0        0       75 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_10.json
+-rw-rw-rw-   0        0        0      593 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_11.json
+-rw-rw-rw-   0        0        0       90 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_16.json
+-rw-rw-rw-   0        0        0       93 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_2.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_26.json
+-rw-rw-rw-   0        0        0       79 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_3.json
+-rw-rw-rw-   0        0        0      444 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_4.json
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_4_9.json
+-rw-rw-rw-   0        0        0      183 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_5_99_6.json
+-rw-rw-rw-   0        0        0     1089 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_1.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_11.json
+-rw-rw-rw-   0        0        0      498 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_13.json
+-rw-rw-rw-   0        0        0     1400 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_15.json
+-rw-rw-rw-   0        0        0       99 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_16.json
+-rw-rw-rw-   0        0        0      209 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_17.json
+-rw-rw-rw-   0        0        0      351 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_22.json
+-rw-rw-rw-   0        0        0      641 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_23.json
+-rw-rw-rw-   0        0        0       93 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_28.json
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_29.json
+-rw-rw-rw-   0        0        0      351 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_3.json
+-rw-rw-rw-   0        0        0      661 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_5.json
+-rw-rw-rw-   0        0        0      316 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_52.json
+-rw-rw-rw-   0        0        0      269 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_53.json
+-rw-rw-rw-   0        0        0      610 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_55.json
+-rw-rw-rw-   0        0        0      243 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_65.json
+-rw-rw-rw-   0        0        0      732 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_7.json
+-rw-rw-rw-   0        0        0     1690 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_8.json
+-rw-rw-rw-   0        0        0     1265 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_1_9.json
+-rw-rw-rw-   0        0        0      313 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_2_1.json
+-rw-rw-rw-   0        0        0      364 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_4_10.json
+-rw-rw-rw-   0        0        0     1780 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_4_13.json
+-rw-rw-rw-   0        0        0      145 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_5_1.json
+-rw-rw-rw-   0        0        0       98 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_5_2.json
+-rw-rw-rw-   0        0        0      513 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/3_6_5_4.json
+-rw-rw-rw-   0        0        0      503 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_1.json
+-rw-rw-rw-   0        0        0      135 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_11.json
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_15.json
+-rw-rw-rw-   0        0        0     1509 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_17.json
+-rw-rw-rw-   0        0        0      572 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_18.json
+-rw-rw-rw-   0        0        0      656 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_19.json
+-rw-rw-rw-   0        0        0       98 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_2.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_20.json
+-rw-rw-rw-   0        0        0      191 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_22.json
+-rw-rw-rw-   0        0        0      148 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_23.json
+-rw-rw-rw-   0        0        0      549 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_28.json
+-rw-rw-rw-   0        0        0      560 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_31.json
+-rw-rw-rw-   0        0        0      138 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_36.json
+-rw-rw-rw-   0        0        0      627 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_48.json
+-rw-rw-rw-   0        0        0      907 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_49.json
+-rw-rw-rw-   0        0        0      250 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_50.json
+-rw-rw-rw-   0        0        0       89 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_8.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_85.json
+-rw-rw-rw-   0        0        0      170 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_1_9.json
+-rw-rw-rw-   0        0        0     3865 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_13.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_17.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_20.json
+-rw-rw-rw-   0        0        0       83 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_25.json
+-rw-rw-rw-   0        0        0      300 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_38.json
+-rw-rw-rw-   0        0        0      160 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_4.json
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_40.json
+-rw-rw-rw-   0        0        0      563 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_47.json
+-rw-rw-rw-   0        0        0      104 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_55.json
+-rw-rw-rw-   0        0        0       71 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_2_8.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_1.json
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_27.json
+-rw-rw-rw-   0        0        0      100 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_3.json
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_30.json
+-rw-rw-rw-   0        0        0     1037 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_39.json
+-rw-rw-rw-   0        0        0      138 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_4.json
+-rw-rw-rw-   0        0        0      119 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_3_40.json
+-rw-rw-rw-   0        0        0      537 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_99_1.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_1_99_3.json
+-rw-rw-rw-   0        0        0     1622 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_1.json
+-rw-rw-rw-   0        0        0      147 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_10.json
+-rw-rw-rw-   0        0        0     1359 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_11.json
+-rw-rw-rw-   0        0        0      221 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_113.json
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_122.json
+-rw-rw-rw-   0        0        0      175 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_17.json
+-rw-rw-rw-   0        0        0      996 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_2.json
+-rw-rw-rw-   0        0        0      485 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_20.json
+-rw-rw-rw-   0        0        0      726 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_22.json
+-rw-rw-rw-   0        0        0       97 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_24.json
+-rw-rw-rw-   0        0        0      109 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_33.json
+-rw-rw-rw-   0        0        0      432 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_40.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_42.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_46.json
+-rw-rw-rw-   0        0        0      373 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_51.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_59.json
+-rw-rw-rw-   0        0        0       82 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_75.json
+-rw-rw-rw-   0        0        0      207 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_80.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_81.json
+-rw-rw-rw-   0        0        0      169 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_91.json
+-rw-rw-rw-   0        0        0       79 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_1_99.json
+-rw-rw-rw-   0        0        0       85 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_2_1.json
+-rw-rw-rw-   0        0        0      123 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_2_19.json
+-rw-rw-rw-   0        0        0       84 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_2_7.json
+-rw-rw-rw-   0        0        0      254 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_1.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_12.json
+-rw-rw-rw-   0        0        0      109 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_22.json
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_3.json
+-rw-rw-rw-   0        0        0      450 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_4.json
+-rw-rw-rw-   0        0        0       80 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_74.json
+-rw-rw-rw-   0        0        0      207 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_3_9.json
+-rw-rw-rw-   0        0        0      100 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_2_99_20.json
+-rw-rw-rw-   0        0        0       86 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_1_1.json
+-rw-rw-rw-   0        0        0      433 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_1_15.json
+-rw-rw-rw-   0        0        0      149 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_1_17.json
+-rw-rw-rw-   0        0        0      337 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_1_18.json
+-rw-rw-rw-   0        0        0       95 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_1_19.json
+-rw-rw-rw-   0        0        0      394 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_2_1.json
+-rw-rw-rw-   0        0        0      116 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_2_2.json
+-rw-rw-rw-   0        0        0       91 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_2_3.json
+-rw-rw-rw-   0        0        0      113 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_2_7.json
+-rw-rw-rw-   0        0        0      115 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_3_6.json
+-rw-rw-rw-   0        0        0      105 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_3_3_7.json
+-rw-rw-rw-   0        0        0      821 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_4_1_1.json
+-rw-rw-rw-   0        0        0      536 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_4_1_21.json
+-rw-rw-rw-   0        0        0     1868 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_4_1_5.json
+-rw-rw-rw-   0        0        0      104 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_6_1_1.json
+-rw-rw-rw-   0        0        0      230 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/4_6_1_12.json
+-rw-rw-rw-   0        0        0      882 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_1_1.json
+-rw-rw-rw-   0        0        0      117 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_1_20.json
+-rw-rw-rw-   0        0        0     1436 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_1_3.json
+-rw-rw-rw-   0        0        0      166 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_1_7.json
+-rw-rw-rw-   0        0        0      343 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_3_1.json
+-rw-rw-rw-   0        0        0      356 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_3_13.json
+-rw-rw-rw-   0        0        0      314 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_3_14.json
+-rw-rw-rw-   0        0        0      890 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_3_2.json
+-rw-rw-rw-   0        0        0      529 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_3_3.json
+-rw-rw-rw-   0        0        0      211 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_1_3_4.json
+-rw-rw-rw-   0        0        0     2053 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_1.json
+-rw-rw-rw-   0        0        0       88 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_13.json
+-rw-rw-rw-   0        0        0      258 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_16.json
+-rw-rw-rw-   0        0        0      163 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_24.json
+-rw-rw-rw-   0        0        0      275 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_28.json
+-rw-rw-rw-   0        0        0      611 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_4.json
+-rw-rw-rw-   0        0        0     4325 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_5.json
+-rw-rw-rw-   0        0        0      460 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_6.json
+-rw-rw-rw-   0        0        0      154 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_8.json
+-rw-rw-rw-   0        0        0     1286 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_1_9.json
+-rw-rw-rw-   0        0        0      258 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_3_2.json
+-rw-rw-rw-   0        0        0      204 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_3_7.json
+-rw-rw-rw-   0        0        0      719 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_3_8.json
+-rw-rw-rw-   0        0        0      172 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_3_99_3.json
+-rw-rw-rw-   0        0        0      182 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_2_10.json
+-rw-rw-rw-   0        0        0      790 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_2_11.json
+-rw-rw-rw-   0        0        0      514 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_2_12.json
+-rw-rw-rw-   0        0        0      241 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_2_2.json
+-rw-rw-rw-   0        0        0      250 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_2_8.json
+-rw-rw-rw-   0        0        0      269 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_4_2.json
+-rw-rw-rw-   0        0        0      238 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_99_1.json
+-rw-rw-rw-   0        0        0      161 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_99_18.json
+-rw-rw-rw-   0        0        0      118 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_99_2.json
+-rw-rw-rw-   0        0        0      730 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/5_4_99_5.json
+-rw-rw-rw-   0        0        0      855 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_1_1_17.json
+-rw-rw-rw-   0        0        0      131 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_1_1_24.json
+-rw-rw-rw-   0        0        0       85 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_1_1_26.json
+-rw-rw-rw-   0        0        0      140 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_1_1_5.json
+-rw-rw-rw-   0        0        0      468 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_2_1_1.json
+-rw-rw-rw-   0        0        0     1410 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_2_1_13.json
+-rw-rw-rw-   0        0        0      123 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_2_1_30.json
+-rw-rw-rw-   0        0        0      104 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_1_13.json
+-rw-rw-rw-   0        0        0      334 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_1_2.json
+-rw-rw-rw-   0        0        0       94 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_1_8.json
+-rw-rw-rw-   0        0        0      609 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_1_9.json
+-rw-rw-rw-   0        0        0      907 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_1.json
+-rw-rw-rw-   0        0        0      241 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_10.json
+-rw-rw-rw-   0        0        0       96 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_12.json
+-rw-rw-rw-   0        0        0      243 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_2.json
+-rw-rw-rw-   0        0        0      131 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_3.json
+-rw-rw-rw-   0        0        0      613 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_4.json
+-rw-rw-rw-   0        0        0      210 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_5.json
+-rw-rw-rw-   0        0        0      345 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_8.json
+-rw-rw-rw-   0        0        0      293 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_2_9.json
+-rw-rw-rw-   0        0        0      229 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_3_2.json
+-rw-rw-rw-   0        0        0      142 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_3_3.json
+-rw-rw-rw-   0        0        0       97 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_4_18.json
+-rw-rw-rw-   0        0        0     1349 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_4_2.json
+-rw-rw-rw-   0        0        0      136 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_4_21.json
+-rw-rw-rw-   0        0        0      157 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_4_3.json
+-rw-rw-rw-   0        0        0      208 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_4_4.json
+-rw-rw-rw-   0        0        0      122 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_4_6.json
+-rw-rw-rw-   0        0        0      458 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_3_5_5.json
+-rw-rw-rw-   0        0        0      316 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/_cache/sabio_rk_total/6_4_1_2.json
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.153490 ECMpy2.0-1.0.2/ECMpy2.0-main/analysis/
+-rw-rw-rw-   0        0        0     6148 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/analysis/.DS_Store
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.153490 ECMpy2.0-1.0.2/ECMpy2.0-main/analysis/get_kcat_mw_by_AutoPACMEN/
+-rw-rw-rw-   0        0        0   311652 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/analysis/get_kcat_mw_by_AutoPACMEN/reaction_kcat_MW.csv
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.197431 ECMpy2.0-1.0.2/ECMpy2.0-main/data/
+-rw-rw-rw-   0        0        0     8196 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/.DS_Store
+-rw-rw-rw-   0        0        0   288653 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/EC_kcat_max.json
+-rw-rw-rw-   0        0        0  1040543 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/all--radius2--ngram3--dim20--layer_gnn3--window11--layer_cnn3--layer_output3--lr1e-3--lr_decay0.5--decay_interval10--weight_decay1e-6--iteration50
+-rw-rw-rw-   0        0        0      366 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/atom_dict.pickle
+-rw-rw-rw-   0        0        0  7971568 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/bigg_models_metabolites.txt
+-rw-rw-rw-   0        0        0       70 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/bond_dict.pickle
+-rw-rw-rw-   0        0        0   243209 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/edge_dict.pickle
+-rw-rw-rw-   0        0        0   243823 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/fingerprint_dict.pickle
+-rw-rw-rw-   0        0        0    48114 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/gene_abundance.csv
+-rw-rw-rw-   0        0        0  3684930 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/iBsu1147R.xml
+-rw-rw-rw-   0        0        0  3031762 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/iCW773R.xml
+-rw-rw-rw-   0        0        0 10365864 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/iML1515_new.xml
+-rw-rw-rw-   0        0        0   311654 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/reaction_kcat_MW_template.csv
+-rw-rw-rw-   0        0        0   135675 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/data/sequence_dict.pickle
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.197431 ECMpy2.0-1.0.2/ECMpy2.0-main/model/
+-rw-rw-rw-   0        0        0  5921734 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/model/iML1515_irr_enz_constraint_adj.json
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.213410 ECMpy2.0-1.0.2/ECMpy2.0-main/script/
+-rw-rw-rw-   0        0        0     6148 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/.DS_Store
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.213410 ECMpy2.0-1.0.2/ECMpy2.0-main/script/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0   118836 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/.ipynb_checkpoints/ECMpy_function-checkpoint.py
+-rw-rw-rw-   0        0        0     4718 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/.ipynb_checkpoints/get_ecGEM_onestop-checkpoint.py
+-rw-rw-rw-   0        0        0    94027 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/AutoPACMEN_function.py
+-rw-rw-rw-   0        0        0   121429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/ECMpy_function.py
+-rw-rw-rw-   0        0        0       19 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.217404 ECMpy2.0-1.0.2/ECMpy2.0-main/script/__pycache__/
+-rw-rw-rw-   0        0        0    49569 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/__pycache__/AutoPACMEN_function.cpython-37.pyc
+-rw-rw-rw-   0        0        0    77272 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/__pycache__/ECMpy_function.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7590 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/__pycache__/model.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7730 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/__pycache__/model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4718 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/get_ecGEM_onestop.py
+-rw-rw-rw-   0        0        0     8905 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/model.py
+-rw-rw-rw-   0        0        0     9605 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/ECMpy2.0-main/script/prediction_for_input.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:09:49.225394 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/
+-rw-rw-rw-   0        0        0      252 2023-08-07 08:09:46.000000 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    96840 2023-08-07 08:09:47.000000 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 08:09:46.000000 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 08:09:46.000000 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      184 2023-08-07 08:09:46.000000 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 08:09:46.000000 ECMpy2.0-1.0.2/ECMpy2.0.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-08-07 08:08:14.000000 ECMpy2.0-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      252 2023-08-07 08:09:49.229388 ECMpy2.0-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2883 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 08:09:49.229388 ECMpy2.0-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      835 2023-08-07 08:09:38.000000 ECMpy2.0-1.0.2/setup.py
```

### Comparing `ECMpy2.0-1.0.1/ECMpy/AutoPACMEN_function.py` & `ECMpy2.0-1.0.2/ECMpy2.0-main/script/AutoPACMEN_function.py`

 * *Files identical despite different names*

### Comparing `ECMpy2.0-1.0.1/ECMpy/ECMpy_function.py` & `ECMpy2.0-1.0.2/ECMpy2.0-main/script/ECMpy_function.py`

 * *Files identical despite different names*

### Comparing `ECMpy2.0-1.0.1/ECMpy/get_ecGEM_onestop.py` & `ECMpy2.0-1.0.2/ECMpy2.0-main/script/.ipynb_checkpoints/get_ecGEM_onestop-checkpoint.py`

 * *Files identical despite different names*

### Comparing `ECMpy2.0-1.0.1/ECMpy/model.py` & `ECMpy2.0-1.0.2/ECMpy2.0-main/script/model.py`

 * *Files identical despite different names*

### Comparing `ECMpy2.0-1.0.1/ECMpy/prediction_for_input.py` & `ECMpy2.0-1.0.2/ECMpy2.0-main/script/prediction_for_input.py`

 * *Files identical despite different names*

### Comparing `ECMpy2.0-1.0.1/README.md` & `ECMpy2.0-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ECMpy2.0-1.0.1/setup.py` & `ECMpy2.0-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ECMpy2.0',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
     include_package_data=True,
     install_requires=[
         'cobra==0.21.0',
         'openpyxl',
```

