# Comparing `tmp/deduce-2.0.3.tar.gz` & `tmp/deduce-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deduce-2.0.3.tar", max compression
+gzip compressed data, was "deduce-2.1.0.tar", max compression
```

## Comparing `deduce-2.0.3.tar` & `deduce-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     7660 2023-04-06 08:47:49.092359 deduce-2.0.3/LICENSE.md
--rw-r--r--   0        0        0     6438 2023-04-06 08:47:49.092359 deduce-2.0.3/README.md
--rw-r--r--   0        0        0    10189 2023-04-06 08:47:49.096359 deduce-2.0.3/config.json
--rw-r--r--   0        0        0    62362 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/first_names.txt
--rw-r--r--   0        0        0     8389 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/institutions.txt
--rw-r--r--   0        0        0    26132 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/interfix_surnames.txt
--rw-r--r--   0        0        0     1660 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/interfixes.txt
--rw-r--r--   0        0        0     2838 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/medical_terms.txt
--rw-r--r--   0        0        0      106 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/prefixes.txt
--rw-r--r--   0        0        0    24182 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/residences.txt
--rw-r--r--   0        0        0      452 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/stop_words.txt
--rw-r--r--   0        0        0    62481 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/surnames.txt
--rw-r--r--   0        0        0     6813 2023-04-06 08:47:49.096359 deduce-2.0.3/data/lookup_lists/top_1000_terms.txt
--rw-r--r--   0        0        0      213 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/__init__.py
--rw-r--r--   0        0        0     5591 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/backwards_compat.py
--rw-r--r--   0        0        0     7858 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/deduce.py
--rw-r--r--   0        0        0     5582 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/lookup_sets.py
--rw-r--r--   0        0        0      486 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/pattern/__init__.py
--rw-r--r--   0        0        0     3693 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/pattern/name.py
--rw-r--r--   0        0        0     4744 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/pattern/name_context.py
--rw-r--r--   0        0        0     3691 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/pattern/name_patient.py
--rw-r--r--   0        0        0     1491 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/person.py
--rw-r--r--   0        0        0        0 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/process/__init__.py
--rw-r--r--   0        0        0     2828 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/process/annotation_processing.py
--rw-r--r--   0        0        0     4007 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/process/annotator.py
--rw-r--r--   0        0        0     1936 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/process/redact.py
--rw-r--r--   0        0        0      118 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/str/__init__.py
--rw-r--r--   0        0        0     2074 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/str/processor.py
--rw-r--r--   0        0        0     5053 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/tokenize.py
--rw-r--r--   0        0        0     2298 2023-04-06 08:47:49.096359 deduce-2.0.3/deduce/utils.py
--rw-r--r--   0        0        0     1561 2023-04-06 08:47:49.100359 deduce-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     7897 1970-01-01 00:00:00.000000 deduce-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7660 2023-08-07 12:47:07.459025 deduce-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     6652 2023-08-07 12:47:07.459025 deduce-2.1.0/README.md
+-rw-r--r--   0        0        0    10895 2023-08-07 12:47:07.459025 deduce-2.1.0/config.json
+-rw-r--r--   0        0        0    62362 2023-08-07 12:47:07.459025 deduce-2.1.0/data/lookup_lists/first_names.txt
+-rw-r--r--   0        0        0     8389 2023-08-07 12:47:07.459025 deduce-2.1.0/data/lookup_lists/institutions.txt
+-rw-r--r--   0        0        0    26132 2023-08-07 12:47:07.459025 deduce-2.1.0/data/lookup_lists/interfix_surnames.txt
+-rw-r--r--   0        0        0     1660 2023-08-07 12:47:07.459025 deduce-2.1.0/data/lookup_lists/interfixes.txt
+-rw-r--r--   0        0        0     2838 2023-08-07 12:47:07.463024 deduce-2.1.0/data/lookup_lists/medical_terms.txt
+-rw-r--r--   0        0        0      106 2023-08-07 12:47:07.463024 deduce-2.1.0/data/lookup_lists/prefixes.txt
+-rw-r--r--   0        0        0    24182 2023-08-07 12:47:07.463024 deduce-2.1.0/data/lookup_lists/residences.txt
+-rw-r--r--   0        0        0      452 2023-08-07 12:47:07.463024 deduce-2.1.0/data/lookup_lists/stop_words.txt
+-rw-r--r--   0        0        0    62481 2023-08-07 12:47:07.463024 deduce-2.1.0/data/lookup_lists/surnames.txt
+-rw-r--r--   0        0        0     6813 2023-08-07 12:47:07.463024 deduce-2.1.0/data/lookup_lists/top_1000_terms.txt
+-rw-r--r--   0        0        0      127 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/__init__.py
+-rw-r--r--   0        0        0     7541 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/deduce.py
+-rw-r--r--   0        0        0     5582 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/lookup_sets.py
+-rw-r--r--   0        0        0      486 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/pattern/__init__.py
+-rw-r--r--   0        0        0     3693 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/pattern/name.py
+-rw-r--r--   0        0        0     4744 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/pattern/name_context.py
+-rw-r--r--   0        0        0     3691 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/pattern/name_patient.py
+-rw-r--r--   0        0        0     1491 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/person.py
+-rw-r--r--   0        0        0        0 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/process/__init__.py
+-rw-r--r--   0        0        0     2828 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/process/annotation_processing.py
+-rw-r--r--   0        0        0     7055 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/process/annotator.py
+-rw-r--r--   0        0        0     1936 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/process/redact.py
+-rw-r--r--   0        0        0      118 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/str/__init__.py
+-rw-r--r--   0        0        0     2070 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/str/processor.py
+-rw-r--r--   0        0        0     5053 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/tokenizer.py
+-rw-r--r--   0        0        0     2645 2023-08-07 12:47:07.463024 deduce-2.1.0/deduce/utils.py
+-rw-r--r--   0        0        0     1561 2023-08-07 12:47:07.463024 deduce-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7959 1970-01-01 00:00:00.000000 deduce-2.1.0/PKG-INFO
```

### Comparing `deduce-2.0.3/LICENSE.md` & `deduce-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/README.md` & `deduce-2.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 
 <!-- start include in docs -->
 
 > Deduce 2.0.0 has been released! It includes a 10x speedup, and way more features for customizing and tailoring. Some small changes are needed to keep going from version 1, read more about it here: [docs/migrating-to-v2](https://deduce.readthedocs.io/en/latest/migrating.html)
 
 De-identify clinial text written in Dutch using `deduce`, a rule-based de-identification method for Dutch clinical text.
 
-The development, principles and validation of `deduce` were initially described in [Menger et al. (2017)](http://www.sciencedirect.com/science/article/pii/S0736585316307365). De-identification of clinical text is needed for using text data for analysis, to comply with legal requirements and to protect the privacy of patients. Our rule-based method removes Protected Health Information (PHI) in the following categories:
+The development, principles and validation of `deduce` were initially described in [Menger et al. (2017)](http://www.sciencedirect.com/science/article/pii/S0736585316307365). De-identification of clinical text is needed for using text data for analysis, to comply with legal requirements and to protect the privacy of patients. By default, our rule-based method removes Protected Health Information (PHI) in the following categories:
 
 * Person names, including initials
 * Geographical locations smaller than a country
 * Names of institutions that are related to patient treatment
-* Dates
+* Dates (combinations of day, month and year)
 * Ages
-* Patient numbers
+* BSN numbers
+* Identifiers (7+ digits without a specific format, e.g. patient identifiers, AGB, BIG)
 * Telephone numbers
-* E-mail addresses and URLs
+* E-mail addresses 
+* URLs
 
 If you use `deduce`, please cite the following paper:  
 
 [Menger, V.J., Scheepers, F., van Wijk, L.M., Spruit, M. (2017). DEDUCE: A pattern matching method for automatic de-identification of Dutch medical text, Telematics and Informatics, 2017, ISSN 0736-5853](http://www.sciencedirect.com/science/article/pii/S0736585316307365)
 
 ## Installation
 
@@ -57,61 +59,64 @@
 The basic way to use `deduce`, is to pass text to the `deidentify` method of a `Deduce` object:
 
 ```python
 from deduce import Deduce
 
 deduce = Deduce()
 
-text = """Dit is stukje tekst met daarin de naam Jan Jansen. De patient J. Jansen 
-        (e: j.jnsen@email.com, t: 06-12345678) is 64 jaar oud en woonachtig 
-        in Utrecht. Hij werd op 10 oktober door arts Peter de Visser ontslagen 
-        van de kliniek van het UMCU."""
+text = (
+    "betreft: Jan Jansen, bsn 111222333, patnr 000334433. De patient J. Jansen is 64 jaar oud en woonachtig in "
+    "Utrecht. Hij werd op 10 oktober 2018 door arts Peter de Visser ontslagen van de kliniek van het UMCU. "
+    "Voor nazorg kan hij worden bereikt via j.JNSEN.123@gmail.com of (06)12345678."
+)
 
 doc = deduce.deidentify(text)
 ```
 
 The output is available in the `Document` object:
 
 ```python
 from pprint import pprint
 
 pprint(doc.annotations)
 
-AnnotationSet({Annotation(text='Jan Jansen', start_char=39, end_char=49, tag='persoon', length=10),
-               Annotation(text='Peter de Visser', start_char=185, end_char=200, tag='persoon', length=15),
-               Annotation(text='j.jnsen@email.com', start_char=76, end_char=93, tag='url', length=17),
-               Annotation(text='10 oktober', start_char=164, end_char=174, tag='datum', length=10),
-               Annotation(text='patient J. Jansen', start_char=54, end_char=71, tag='persoon', length=17),
-               Annotation(text='64', start_char=114, end_char=116, tag='leeftijd', length=2),
-               Annotation(text='UMCU', start_char=234, end_char=238, tag='instelling', length=4),
-               Annotation(text='06-12345678', start_char=98, end_char=109, tag='telefoonnummer', length=11),
-               Annotation(text='Utrecht', start_char=143, end_char=150, tag='locatie', length=7)})
+AnnotationSet({
+    Annotation(text="(06)12345678", start_char=272, end_char=284, tag="telefoonnummer"),
+    Annotation(text="111222333", start_char=25, end_char=34, tag="bsn"),
+    Annotation(text="Peter de Visser", start_char=153, end_char=168, tag="persoon"),
+    Annotation(text="j.JNSEN.123@gmail.com", start_char=247, end_char=268, tag="email"),
+    Annotation(text="patient J. Jansen", start_char=56, end_char=73, tag="patient"),
+    Annotation(text="Jan Jansen", start_char=9, end_char=19, tag="patient"),
+    Annotation(text="10 oktober 2018", start_char=127, end_char=142, tag="datum"),
+    Annotation(text="64", start_char=77, end_char=79, tag="leeftijd"),
+    Annotation(text="000334433", start_char=42, end_char=51, tag="id"),
+    Annotation(text="Utrecht", start_char=106, end_char=113, tag="locatie"),
+    Annotation(text="UMCU", start_char=202, end_char=206, tag="instelling"),
+})
 
 print(doc.deidentified_text)
 
-"""Dit is stukje tekst met daarin de naam <PERSOON-1>. De <PERSOON-2> 
-(e: <URL-1>, t: <TELEFOONNUMMER-1>) is <LEEFTIJD-1> jaar oud en woonachtig 
-in <LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-3> ontslagen 
-van de kliniek van het <INSTELLING-1>."""
+"""betreft: <PERSOON-1>, bsn <BSN-1>, patnr <ID-1>. De <PERSOON-1> is <LEEFTIJD-1> jaar oud en woonachtig in 
+<LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-2> ontslagen van de kliniek van het <INSTELLING-1>. 
+Voor nazorg kan hij worden bereikt via <EMAIL-1> of <TELEFOONNUMMER-1>."""
 ```
 
 Aditionally, if the names of the patient are known, they may be added as `metadata`, where they will be picked up by `deduce`:
 
 ```python
 from deduce.person import Person
 
 patient = Person(first_names=["Jan"], initials="JJ", surname="Jansen")
 doc = deduce.deidentify(text, metadata={'patient': patient})
 
 print (doc.deidentified_text)
 
-"""Dit is stukje tekst met daarin de naam <PATIENT>. De <PATIENT> 
-(e: <URL-1>, t: <TELEFOONNUMMER-1>) is <LEEFTIJD-1> jaar oud en woonachtig 
-in <LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-1> ontslagen 
-van de kliniek van het <INSTELLING-1>."""
+"""betreft: <PATIENT>, bsn <BSN-1>, patnr <ID-1>. De <PATIENT> is <LEEFTIJD-1> jaar oud en woonachtig in 
+<LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-2> ontslagen van de kliniek van het <INSTELLING-1>. 
+Voor nazorg kan hij worden bereikt via <EMAIL-1> of <TELEFOONNUMMER-1>."""
 ```
 
 As you can see, adding known names keeps references to `<PATIENT>` in text. It also increases recall, as not all known names are contained in the lookup lists. 
 
 <!-- end getting started -->
 
 ## Documentation
```

### Comparing `deduce-2.0.3/config.json` & `deduce-2.1.0/config.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7705158730158731%*

 * *Differences: {"'adjacent_annotations_slack'": "'[\\\\. \\\\-,]?[\\\\. ]?'",*

 * * "'annotators'": "{'age': {'args': {'regexp_pattern': "*

 * *                 "'(?i)((((\\\\d-|\\\\d\\\\d-))?(\\\\d[,\\\\.]\\\\d|\\\\d{1,3}))([ "*

 * *                 '-](jarige|jarig|jaar)))(?!\\\\w)(?! '*

 * *                 "(geleden|na|aanwezig|getrouwd|gestopt|gerookt|gebruikt|gestaakt))', "*

 * *                 "'capturing_group': 2}}, 'email': {'group': 'email_addresses', 'args': "*

 * *                 "{'regexp_pattern': "*

 * *                 "'(([-a-zA-Z0-9:%. […]*

```diff
@@ -1,64 +1,102 @@
 {
-    "adjacent_annotations_slack": "[\\.\\s\\-,]?[\\.\\s]?",
+    "adjacent_annotations_slack": "[\\. \\-,]?[\\. ]?",
     "annotators": {
         "age": {
             "annotator_type": "regexp",
             "args": {
-                "capturing_group": 1,
-                "regexp_pattern": "(\\d{1,3})([ -](jarige|jarig|jaar))",
+                "capturing_group": 2,
+                "regexp_pattern": "(?i)((((\\d-|\\d\\d-))?(\\d[,\\.]\\d|\\d{1,3}))([ -](jarige|jarig|jaar)))(?!\\w)(?! (geleden|na|aanwezig|getrouwd|gestopt|gerookt|gebruikt|gestaakt))",
                 "tag": "leeftijd"
             },
             "group": "ages"
         },
         "altrecht": {
             "annotator_type": "regexp",
             "args": {
                 "regexp_pattern": "[aA][lL][tT][rR][eE][cC][hH][tT]((\\s[A-Z][\\w]*)*)",
                 "tag": "instelling"
             },
             "group": "institutions"
         },
-        "date_1": {
+        "bsn": {
+            "annotator_type": "custom",
+            "args": {
+                "bsn_regexp": "(?<!\\d)(\\d{9})(?!\\d)",
+                "capture_group": 1,
+                "class": "BsnAnnotator",
+                "module": "deduce.process.annotator",
+                "priority": 100,
+                "tag": "bsn"
+            },
+            "group": "identifiers"
+        },
+        "date_dmy_1": {
+            "annotator_type": "regexp",
+            "args": {
+                "capturing_group": 1,
+                "regexp_pattern": "(?<!\\d)(([1-9]|0[1-9]|[12][0-9]|3[01])(?P<sep>[-/\\. ])([1-9]|0[1-9]|1[012])(?P=sep)((19|20|\\'|`)?\\d{2}))(?!\\d)",
+                "tag": "datum"
+            },
+            "group": "dates"
+        },
+        "date_dmy_2": {
             "annotator_type": "regexp",
             "args": {
                 "capturing_group": 1,
-                "regexp_pattern": "(([1-9]|0[1-9]|[12][0-9]|3[01])[- /.](0[1-9]|1[012]|[1-9])([- /.]{,2}(\\d{4}|\\d{2}))?)(\\D|$)",
+                "regexp_pattern": "(?i)(?<!\\d)(([1-9]|0[1-9]|[12][0-9]|3[01])[-/\\. ]{,2}(januari|jan|februari|feb|maart|mrt|april|apr|mei|juni|jun|juli|jul|augustus|aug|september|sep|sept|oktober|okt|november|nov|december|dec)[-/\\. ]((19|20|\\'|`)?\\d{2}))(?!\\d)",
                 "tag": "datum"
             },
             "group": "dates"
         },
-        "date_2": {
+        "date_ymd_1": {
             "annotator_type": "regexp",
             "args": {
                 "capturing_group": 1,
-                "regexp_pattern": "(\\d{1,2}[^\\w]{,2}(januari|februari|maart|april|mei|juni|juli|augustus|september|oktober|november|december)([- /.]{,2}(\\d{4}|\\d{2}))?)(\\D|$)",
+                "regexp_pattern": "(?<!\\d)(((19|20|\\'|`)\\d{2})(?P<sep>[-/\\. ])([1-9]|0[1-9]|1[012])(?P=sep)([1-9]|0[1-9]|[12][0-9]|3[01]))(\\D|$)",
+                "tag": "datum"
+            },
+            "group": "dates"
+        },
+        "date_ymd_2": {
+            "annotator_type": "regexp",
+            "args": {
+                "capturing_group": 1,
+                "regexp_pattern": "(?i)(?<!\\d)(((19|20|\\'|`)\\d{2})[-/\\. ]{,2}(januari|jan|februari|feb|maart|mrt|april|apr|mei|juni|jun|juli|jul|augustus|aug|september|sep|sept|oktober|okt|november|nov|december|dec)[-/\\. ]([1-9]|0[1-9]|[12][0-9]|3[01]))(?!\\d)",
                 "tag": "datum"
             },
             "group": "dates"
         },
         "email": {
             "annotator_type": "regexp",
             "args": {
-                "regexp_pattern": "([\\w-]+(?:\\.[\\w-]+)*)@((?:[\\w-]+\\.)*\\w[\\w-]{0,66})\\.([a-z]{2,6}(?:\\.[a-z]{2})?)",
-                "tag": "url"
+                "regexp_pattern": "(([-a-zA-Z0-9:%._\\+~#=]{1,256})@([-a-zA-Z0-9:%._\\+~#=]{1,256})(\\.)(com|net|org|co|us|uk|nl|be|fr|sp|gov|nu))",
+                "tag": "email"
             },
-            "group": "urls"
+            "group": "email_addresses"
         },
         "first_name_lookup": {
             "annotator_type": "token_pattern",
             "args": {
                 "pattern": {
                     "class": "FirstNameLookupPattern",
                     "module": "deduce.pattern",
                     "tag": "voornaam_onbekend"
                 }
             },
             "group": "names"
         },
+        "identifier": {
+            "annotator_type": "regexp",
+            "args": {
+                "regexp_pattern": "\\d{7,}",
+                "tag": "id"
+            },
+            "group": "identifiers"
+        },
         "initial_interfix": {
             "annotator_type": "token_pattern",
             "args": {
                 "pattern": {
                     "class": "InitiaalInterfixCapitalPattern",
                     "module": "deduce.pattern",
                     "tag": "initiaal+interfix+naam"
@@ -134,22 +172,14 @@
                     "naam",
                     "interfix",
                     "prefix"
                 ]
             },
             "group": "names"
         },
-        "patient_number": {
-            "annotator_type": "regexp",
-            "args": {
-                "regexp_pattern": "\\d{7}",
-                "tag": "patientnummer"
-            },
-            "group": "patient_numbers"
-        },
         "person_first_name": {
             "annotator_type": "token_pattern",
             "args": {
                 "pattern": {
                     "class": "PersonFirstNamePattern",
                     "module": "deduce.pattern",
                     "tag": "voornaam_patient"
@@ -186,38 +216,26 @@
                     "class": "PersonSurnamePattern",
                     "module": "deduce.pattern",
                     "tag": "achternaam_patient"
                 }
             },
             "group": "names"
         },
-        "phone_1": {
-            "annotator_type": "regexp",
-            "args": {
-                "regexp_pattern": "(((0)[1-9]{2}[0-9][-]?[1-9][0-9]{5})|((\\+31|0|0031)[1-9][0-9][-]?[1-9][0-9]{6}))",
-                "tag": "telefoonnummer"
-            },
-            "group": "phone_numbers"
-        },
-        "phone_2": {
-            "annotator_type": "regexp",
+        "phone": {
+            "annotator_type": "custom",
             "args": {
-                "regexp_pattern": "(((\\+31|0|0031)6)[-]?[1-9][0-9]{7})",
+                "class": "PhoneNumberAnnotator",
+                "max_digits": 11,
+                "min_digits": 9,
+                "module": "deduce.process.annotator",
+                "phone_regexp": "(?<!\\d)(\\(?(0031|\\+31|0)(1[035]|2[0347]|3[03568]|4[03456]|5[0358]|6|7|88|800|91|90[069]|[1-5]\\d{2})\\)?) ?-? ?((\\d{2,4}[ -]?)+\\d{2,4})",
                 "tag": "telefoonnummer"
             },
             "group": "phone_numbers"
         },
-        "phone_3": {
-            "annotator_type": "regexp",
-            "args": {
-                "regexp_pattern": "((\\(\\d{3}\\)|\\d{3})\\s?\\d{3}\\s?\\d{2}\\s?\\d{2})",
-                "tag": "telefoonnummer"
-            },
-            "group": "phones"
-        },
         "postal_code": {
             "annotator_type": "regexp",
             "args": {
                 "capturing_group": 1,
                 "regexp_pattern": "(\\d{4} (?!MG)[A-Z]{2}|\\d{4}(?!mg|MG)[a-zA-Z]{2})(\\W|$)",
                 "tag": "locatie"
             },
@@ -266,31 +284,29 @@
                     "class": "SurnameLookupPattern",
                     "module": "deduce.pattern",
                     "tag": "achternaam_onbekend"
                 }
             },
             "group": "names"
         },
-        "url_1": {
-            "annotator_type": "regexp",
-            "args": {
-                "regexp_pattern": "((?!mailto:)((?:http|https|ftp)://)(?:\\S+(?::\\S*)?@)?(?:(?:(?:[1-9]\\d?|1\\d\\d|2[01]\\d|22[0-3])(?:\\.(?:1?\\d{1,2}|2[0-4]\\d|25[0-5])){2}(\\.(?:[0-9]\\d?|1\\d\\d|2[0-4]\\d|25[0-4]))|((?:[a-z\\u00a1-\\uffff0-9]+-?)*[a-z\\u00a1-\\uffff0-9]+)(?:\\.(?:[a-z\\u00a1-\\uffff0-9]+-?)*[a-z\\u00a1-\\uffff0-9]+)*(\\.([a-z\\u00a1-\\uffff]{2,})))|localhost)(?::\\d{2,5})?(?:([/?#])[^\\s]*)?)",
-                "tag": "url"
-            },
-            "group": "urls"
-        },
-        "url_2": {
+        "url": {
             "annotator_type": "regexp",
             "args": {
-                "regexp_pattern": "([\\w\\d.-]{3,}(\\.)(nl|com|net|be)(/[^\\s]+)?)",
+                "regexp_pattern": "((https?:\\/\\/(?:www\\.)?)?([-a-zA-Z0-9:%._\\+~#=]{1,256})(\\.)(com|net|org|co|us|uk|nl|be|fr|sp|gov|nu)(\\b)([():%_\\+.~,]*[-a-zA-Z-0-9#?&/=]+)*)",
                 "tag": "url"
             },
             "group": "urls"
         }
     },
     "redactor_close_char": ">",
     "redactor_open_char": "<",
     "resolve_overlap_strategy": {
-        "ascending": false,
-        "attribute": "length"
+        "ascending": [
+            false,
+            false
+        ],
+        "attributes": [
+            "priority",
+            "length"
+        ]
     }
 }
```

### Comparing `deduce-2.0.3/data/lookup_lists/first_names.txt` & `deduce-2.1.0/data/lookup_lists/first_names.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/institutions.txt` & `deduce-2.1.0/data/lookup_lists/institutions.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/interfix_surnames.txt` & `deduce-2.1.0/data/lookup_lists/interfix_surnames.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/interfixes.txt` & `deduce-2.1.0/data/lookup_lists/interfixes.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/medical_terms.txt` & `deduce-2.1.0/data/lookup_lists/medical_terms.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/residences.txt` & `deduce-2.1.0/data/lookup_lists/residences.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/surnames.txt` & `deduce-2.1.0/data/lookup_lists/surnames.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/data/lookup_lists/top_1000_terms.txt` & `deduce-2.1.0/data/lookup_lists/top_1000_terms.txt`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/deduce.py` & `deduce-2.1.0/deduce/deduce.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 import json
 import os
 import re
-import warnings
 from pathlib import Path
-from typing import Any, Optional
+from typing import Optional
 
-import deprecated
 import docdeid as dd
 
-import deduce.backwards_compat
 from deduce import utils
 from deduce.lookup_sets import get_lookup_sets
 from deduce.process.annotation_processing import (
     DeduceMergeAdjacentAnnotations,
     PersonAnnotationConverter,
 )
 from deduce.process.annotator import AnnotationContextPatternAnnotator
 from deduce.process.redact import DeduceRedactor
-from deduce.tokenize import DeduceTokenizer
-
-warnings.simplefilter(action="once")
+from deduce.tokenizer import DeduceTokenizer
 
 
 class Deduce(dd.DocDeid):
     """
     Main class for de-identifiation.
 
     Inherits from ``docdeid.DocDeid``, and as such, most information is available in the documentation there.
     """
 
-    def __init__(self, config_file: Optional[str] = None) -> None:
+    def __init__(self, config_file: Optional[str] = None, use_config_defaults: Optional[bool] = True) -> None:
         super().__init__()
 
-        self.config = self._initialize_config(config_file)
+        self.config_file = config_file
+        self.use_config_defaults = use_config_defaults
+
+        self.config = self._initialize_config()
+
         self.lookup_sets = get_lookup_sets()
         self.tokenizers = self._initialize_tokenizers()
         self.initialize_doc_processors()
 
-    @staticmethod
-    def _initialize_config(config_file: Optional[str] = None) -> dict:
+    def _initialize_config(self) -> dict:
         """
         Initialize the config file.
 
-        Args:
-            config_file: The filepath of the config file.
-
         Returns:
-            The contents of the config file as a dictionary.
+            The config as a dictionary, based provided input file and default logic.
         """
 
-        config_path = Path(config_file) if config_file else Path(os.path.dirname(__file__)).parent / "config.json"
+        if self.config_file is None and not self.use_config_defaults:
+            raise ValueError("Please specify a config file, or set use_config_defaults to True")
+
+        default_config_path = Path(os.path.dirname(__file__)).parent / "config.json"
+
+        if self.use_config_defaults:
+
+            with open(default_config_path, "r", encoding="utf-8") as file:
+                config = json.load(file)
+
+        if self.config_file is not None:
 
-        with open(config_path, "r", encoding="utf-8") as file:
-            return json.load(file)
+            with open(Path(self.config_file), "r", encoding="utf-8") as file:
+                custom_config = json.load(file)
+
+            config = utils.overwrite_dict(config, custom_config)
+
+        return config
 
     def _initialize_tokenizers(self) -> dict:
         """Initializes tokenizers."""
 
         merge_terms = dd.ds.LookupSet()
         merge_terms.add_items_from_iterable(["A1", "A2", "A3", "A4", "\n", "\r", "\t"])
         merge_terms += self.lookup_sets["interfixes"]
@@ -83,19 +92,23 @@
         config = self.config.copy()  # copy to prevent accidental overwrites, deletes, etc
 
         self.processors = self._initialize_annotators(
             config["annotators"].copy(), self.lookup_sets, self.tokenizers["default"]
         )
         self.processors["names"].add_processor("person_annotation_converter", PersonAnnotationConverter())
 
-        sort_by_attr = self.config["resolve_overlap_strategy"]["attribute"]
-        sort_by = [sort_by_attr]
-        sort_by_callbacks = (
-            {sort_by_attr: lambda x: -x} if not config["resolve_overlap_strategy"]["ascending"] else None
-        )
+        sort_by_attrs = self.config["resolve_overlap_strategy"]["attributes"]
+        sort_by_ascending = self.config["resolve_overlap_strategy"]["ascending"]
+
+        sort_by = []
+        sort_by_callbacks = {}
+
+        for attr, ascending in zip(sort_by_attrs, sort_by_ascending):
+            sort_by.append(attr)
+            sort_by_callbacks[attr] = (lambda x: x) if ascending else (lambda y: -y)
 
         post_group = dd.process.DocProcessorGroup()
         self.processors.add_processor("post_processing", post_group)
 
         post_group.add_processor(
             "overlap_resolver",
             dd.process.OverlapResolver(sort_by=sort_by, sort_by_callbacks=sort_by_callbacks),
@@ -117,14 +130,15 @@
 
     def __init__(self) -> None:
         self.annotator_creators = {
             "token_pattern": self._get_token_pattern_annotator,
             "annotation_context": self._get_annotation_context_pattern_annotator,
             "regexp": self._get_regexp_annotator,
             "multi_token": self._get_multi_token_annotator,
+            "custom": self._get_custom_annotator,
         }
 
     @staticmethod
     def _get_token_pattern_annotator(args: dict, extras: dict) -> dd.process.Annotator:
         pattern = utils.import_and_initialize(args.pop("pattern"), extras=extras)
         return dd.process.TokenPatternAnnotator(pattern=pattern)
 
@@ -146,14 +160,19 @@
             args["lookup_values"] = lookup_set.items()
             args["matching_pipeline"] = lookup_set.matching_pipeline
 
         args["tokenizer"] = DeduceTokenizer()
 
         return dd.process.MultiTokenLookupAnnotator(**args)
 
+    @staticmethod
+    def _get_custom_annotator(args: dict, extras: dict) -> dd.process.Annotator:
+
+        return utils.import_and_initialize(args=args, extras=extras)
+
     def get_annotators(self, annotator_cnfg: dict, extras: dict) -> dd.process.DocProcessorGroup:
         """
         Get the annotators, requested in the annotator config.
 
         Args:
             annotator_cnfg: A dictionary containing configuration on which annotators to initialize.
             extras: Any additional objects passed to pattern or annotator init, if present
@@ -178,34 +197,7 @@
 
                 group = annotators[annotator_info["group"]]
 
             annotator = self.annotator_creators[annotator_info["annotator_type"]](annotator_info["args"], extras)
             group.add_processor(annotator_name, annotator)
 
         return annotators
-
-
-# Backwards compatibility stuff beneath this line.
-deduce.backwards_compat._BackwardsCompat.set_deduce_model(Deduce())
-deprecation_info = {
-    "version": "2.0.0",
-    "reason": "Please use Deduce().deidentify(text) instead. "
-    "See: https://deduce.readthedocs.io/en/latest/migrating.html",
-}
-
-
-@deprecated.deprecated(**deprecation_info)
-def annotate_text(*args, **kwargs) -> Any:
-    """Backwards compatibility function for annotating text."""
-    return deduce.backwards_compat.annotate_text_backwardscompat(*args, **kwargs)
-
-
-@deprecated.deprecated(**deprecation_info)
-def annotate_text_structured(*args, **kwargs) -> Any:
-    """Backwards compatibility function for annotating text structured."""
-    return deduce.backwards_compat.annotate_text_structured_backwardscompat(*args, **kwargs)
-
-
-@deprecated.deprecated(**deprecation_info)
-def deidentify_annotations(*args, **kwargs) -> Any:
-    """Backwards compatibility function for deidentifying annotations."""
-    return deduce.backwards_compat.deidentify_annotations_backwardscompat(*args, **kwargs)
```

### Comparing `deduce-2.0.3/deduce/lookup_sets.py` & `deduce-2.1.0/deduce/lookup_sets.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/pattern/name.py` & `deduce-2.1.0/deduce/pattern/name.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/pattern/name_context.py` & `deduce-2.1.0/deduce/pattern/name_context.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/pattern/name_patient.py` & `deduce-2.1.0/deduce/pattern/name_patient.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/person.py` & `deduce-2.1.0/deduce/person.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/process/annotation_processing.py` & `deduce-2.1.0/deduce/process/annotation_processing.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/process/redact.py` & `deduce-2.1.0/deduce/process/redact.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/str/processor.py` & `deduce-2.1.0/deduce/str/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __init__(self, filter_values: list[str]) -> None:
         self.filter_values = filter_values
 
     def process(self, item: str) -> str:
         for filter_value in self.filter_values:
 
             item = re.sub(
-                r"(^" + filter_value + r"\s|\s" + filter_value + r"\s|\s" + filter_value + r"$)",
+                r"(^" + filter_value + r" | " + filter_value + r" | " + filter_value + r"$)",
                 "",
                 item,
             )
 
         return item
```

### Comparing `deduce-2.0.3/deduce/tokenize.py` & `deduce-2.1.0/deduce/tokenizer.py`

 * *Files identical despite different names*

### Comparing `deduce-2.0.3/deduce/utils.py` & `deduce-2.1.0/deduce/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,7 +69,24 @@
     cls = class_for_name(args.pop("module"), args.pop("class"))
 
     for arg_name, arg in extras.items():
         if arg_name in cls.__init__.__code__.co_varnames:
             args[arg_name] = arg
 
     return cls(**args)
+
+
+def overwrite_dict(base: dict, add: dict) -> dict:
+    """
+    Overwrites the items of the first dict with those of the second.
+
+    Accepts nested dictionaries.
+    """
+
+    for k, v in add.items():
+
+        if isinstance(v, dict):
+            base[k] = overwrite_dict(base.get(k, {}), v)
+        else:
+            base[k] = v
+
+    return base
```

### Comparing `deduce-2.0.3/pyproject.toml` & `deduce-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deduce"
-version = "2.0.3"
+version = "2.1.0"
 description = "Deduce: de-identification method for Dutch medical text"
 authors = ["Vincent Menger <vmenger@protonmail.com>"]
 maintainers = ["Vincent Menger <vmenger@protonmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/vmenger/deduce/"
 keywords = ["de-identification", "clinical text", "dutch", "nlp"]
@@ -23,15 +23,15 @@
 
 [tool.sphinx]
 author = "Vincent Menger"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rapidfuzz = "^2.11.1"
-docdeid = "0.1.6"
+docdeid = "0.1.8"
 regex = "^2022.9.13"
 deprecated = "^1.2.13"
 
 [tool.poetry.group.dev]
 optional = false
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `deduce-2.0.3/PKG-INFO` & `deduce-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deduce
-Version: 2.0.3
+Version: 2.1.0
 Summary: Deduce: de-identification method for Dutch medical text
 Home-page: https://github.com/vmenger/deduce/
 License: LGPL-3.0-or-later
 Keywords: de-identification,clinical text,dutch,nlp
 Author: Vincent Menger
 Author-email: vmenger@protonmail.com
 Maintainer: Vincent Menger
@@ -13,23 +13,20 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
-Requires-Dist: docdeid (==0.1.6)
+Requires-Dist: docdeid (==0.1.8)
 Requires-Dist: rapidfuzz (>=2.11.1,<3.0.0)
 Requires-Dist: regex (>=2022.9.13,<2023.0.0)
 Project-URL: Repository, https://github.com/vmenger/deduce/
 Description-Content-Type: text/markdown
 
 # deduce
 
@@ -47,24 +44,26 @@
 
 <!-- start include in docs -->
 
 > Deduce 2.0.0 has been released! It includes a 10x speedup, and way more features for customizing and tailoring. Some small changes are needed to keep going from version 1, read more about it here: [docs/migrating-to-v2](https://deduce.readthedocs.io/en/latest/migrating.html)
 
 De-identify clinial text written in Dutch using `deduce`, a rule-based de-identification method for Dutch clinical text.
 
-The development, principles and validation of `deduce` were initially described in [Menger et al. (2017)](http://www.sciencedirect.com/science/article/pii/S0736585316307365). De-identification of clinical text is needed for using text data for analysis, to comply with legal requirements and to protect the privacy of patients. Our rule-based method removes Protected Health Information (PHI) in the following categories:
+The development, principles and validation of `deduce` were initially described in [Menger et al. (2017)](http://www.sciencedirect.com/science/article/pii/S0736585316307365). De-identification of clinical text is needed for using text data for analysis, to comply with legal requirements and to protect the privacy of patients. By default, our rule-based method removes Protected Health Information (PHI) in the following categories:
 
 * Person names, including initials
 * Geographical locations smaller than a country
 * Names of institutions that are related to patient treatment
-* Dates
+* Dates (combinations of day, month and year)
 * Ages
-* Patient numbers
+* BSN numbers
+* Identifiers (7+ digits without a specific format, e.g. patient identifiers, AGB, BIG)
 * Telephone numbers
-* E-mail addresses and URLs
+* E-mail addresses 
+* URLs
 
 If you use `deduce`, please cite the following paper:  
 
 [Menger, V.J., Scheepers, F., van Wijk, L.M., Spruit, M. (2017). DEDUCE: A pattern matching method for automatic de-identification of Dutch medical text, Telematics and Informatics, 2017, ISSN 0736-5853](http://www.sciencedirect.com/science/article/pii/S0736585316307365)
 
 ## Installation
 
@@ -90,61 +89,64 @@
 The basic way to use `deduce`, is to pass text to the `deidentify` method of a `Deduce` object:
 
 ```python
 from deduce import Deduce
 
 deduce = Deduce()
 
-text = """Dit is stukje tekst met daarin de naam Jan Jansen. De patient J. Jansen 
-        (e: j.jnsen@email.com, t: 06-12345678) is 64 jaar oud en woonachtig 
-        in Utrecht. Hij werd op 10 oktober door arts Peter de Visser ontslagen 
-        van de kliniek van het UMCU."""
+text = (
+    "betreft: Jan Jansen, bsn 111222333, patnr 000334433. De patient J. Jansen is 64 jaar oud en woonachtig in "
+    "Utrecht. Hij werd op 10 oktober 2018 door arts Peter de Visser ontslagen van de kliniek van het UMCU. "
+    "Voor nazorg kan hij worden bereikt via j.JNSEN.123@gmail.com of (06)12345678."
+)
 
 doc = deduce.deidentify(text)
 ```
 
 The output is available in the `Document` object:
 
 ```python
 from pprint import pprint
 
 pprint(doc.annotations)
 
-AnnotationSet({Annotation(text='Jan Jansen', start_char=39, end_char=49, tag='persoon', length=10),
-               Annotation(text='Peter de Visser', start_char=185, end_char=200, tag='persoon', length=15),
-               Annotation(text='j.jnsen@email.com', start_char=76, end_char=93, tag='url', length=17),
-               Annotation(text='10 oktober', start_char=164, end_char=174, tag='datum', length=10),
-               Annotation(text='patient J. Jansen', start_char=54, end_char=71, tag='persoon', length=17),
-               Annotation(text='64', start_char=114, end_char=116, tag='leeftijd', length=2),
-               Annotation(text='UMCU', start_char=234, end_char=238, tag='instelling', length=4),
-               Annotation(text='06-12345678', start_char=98, end_char=109, tag='telefoonnummer', length=11),
-               Annotation(text='Utrecht', start_char=143, end_char=150, tag='locatie', length=7)})
+AnnotationSet({
+    Annotation(text="(06)12345678", start_char=272, end_char=284, tag="telefoonnummer"),
+    Annotation(text="111222333", start_char=25, end_char=34, tag="bsn"),
+    Annotation(text="Peter de Visser", start_char=153, end_char=168, tag="persoon"),
+    Annotation(text="j.JNSEN.123@gmail.com", start_char=247, end_char=268, tag="email"),
+    Annotation(text="patient J. Jansen", start_char=56, end_char=73, tag="patient"),
+    Annotation(text="Jan Jansen", start_char=9, end_char=19, tag="patient"),
+    Annotation(text="10 oktober 2018", start_char=127, end_char=142, tag="datum"),
+    Annotation(text="64", start_char=77, end_char=79, tag="leeftijd"),
+    Annotation(text="000334433", start_char=42, end_char=51, tag="id"),
+    Annotation(text="Utrecht", start_char=106, end_char=113, tag="locatie"),
+    Annotation(text="UMCU", start_char=202, end_char=206, tag="instelling"),
+})
 
 print(doc.deidentified_text)
 
-"""Dit is stukje tekst met daarin de naam <PERSOON-1>. De <PERSOON-2> 
-(e: <URL-1>, t: <TELEFOONNUMMER-1>) is <LEEFTIJD-1> jaar oud en woonachtig 
-in <LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-3> ontslagen 
-van de kliniek van het <INSTELLING-1>."""
+"""betreft: <PERSOON-1>, bsn <BSN-1>, patnr <ID-1>. De <PERSOON-1> is <LEEFTIJD-1> jaar oud en woonachtig in 
+<LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-2> ontslagen van de kliniek van het <INSTELLING-1>. 
+Voor nazorg kan hij worden bereikt via <EMAIL-1> of <TELEFOONNUMMER-1>."""
 ```
 
 Aditionally, if the names of the patient are known, they may be added as `metadata`, where they will be picked up by `deduce`:
 
 ```python
 from deduce.person import Person
 
 patient = Person(first_names=["Jan"], initials="JJ", surname="Jansen")
 doc = deduce.deidentify(text, metadata={'patient': patient})
 
 print (doc.deidentified_text)
 
-"""Dit is stukje tekst met daarin de naam <PATIENT>. De <PATIENT> 
-(e: <URL-1>, t: <TELEFOONNUMMER-1>) is <LEEFTIJD-1> jaar oud en woonachtig 
-in <LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-1> ontslagen 
-van de kliniek van het <INSTELLING-1>."""
+"""betreft: <PATIENT>, bsn <BSN-1>, patnr <ID-1>. De <PATIENT> is <LEEFTIJD-1> jaar oud en woonachtig in 
+<LOCATIE-1>. Hij werd op <DATUM-1> door arts <PERSOON-2> ontslagen van de kliniek van het <INSTELLING-1>. 
+Voor nazorg kan hij worden bereikt via <EMAIL-1> of <TELEFOONNUMMER-1>."""
 ```
 
 As you can see, adding known names keeps references to `<PATIENT>` in text. It also increases recall, as not all known names are contained in the lookup lists. 
 
 <!-- end getting started -->
 
 ## Documentation
```

