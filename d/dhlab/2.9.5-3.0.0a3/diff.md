# Comparing `tmp/dhlab-2.9.5.tar.gz` & `tmp/dhlab-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhlab-2.9.5.tar", last modified: Wed Oct 26 14:23:59 2022, max compression
+gzip compressed data, was "dhlab-3.0.0a3.tar", max compression
```

## Comparing `dhlab-2.9.5.tar` & `dhlab-3.0.0a3.tar`

### file list

```diff
@@ -1,109 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.494017 dhlab-2.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/bump-version.yml
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/upload-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-10-26 14:23:47.000000 dhlab-2.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    19548 2022-10-26 14:23:47.000000 dhlab-2.9.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-26 14:23:47.000000 dhlab-2.9.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-10-26 14:23:47.000000 dhlab-2.9.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-10-26 14:23:59.506018 dhlab-2.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-10-26 14:23:47.000000 dhlab-2.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/api/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28463 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/dhlab_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/nb_ngram_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4492 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/nb_search_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/css_style_sheets/
--rw-r--r--   0 runner    (1001) docker     (121)    72064 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/grade3.css
--rw-r--r--   0 runner    (1001) docker     (121)    72138 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/monokai.css
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook.css
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_2.css
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_blue.css
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/graph_networkx_louvain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/images/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/images/nbpictures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15394 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/graph_networkx_louvain.py
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/module_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/nb_external_files.py
--rw-r--r--   0 runner    (1001) docker     (121)    14179 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/nbpictures.py
--rw-r--r--   0 runner    (1001) docker     (121)    71589 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/nbtext.py
--rw-r--r--   0 runner    (1001) docker     (121)     8822 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/token_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/module_update.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/nbpictures.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/nbtext.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/nbtokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/ngram/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/ngram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/ngram/nb_ngram.py
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/ngram/ngram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/text/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/chunking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5538 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/conc_coll.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/corpus.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/geo_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/nb_search_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/nbtokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/token_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/trigram_lang_model/
--rw-r--r--   0 runner    (1001) docker     (121)   126476 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/trigram_lang_model/nno_trilangmodel.json
--rw-r--r--   0 runner    (1001) docker     (121)   126751 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/trigram_lang_model/nob_trilangmodel.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     3832 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/wordbank/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/wordbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/wordbank/wordbank.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/DOCS_CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/_images/NB-symbol-farge.png
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/_images/dhlab_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/_images/nb_symbol_farge_z5B_icon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    10923 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/docs_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/docs_notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/notebooks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/package_summary.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_images.rst
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_ngrams.rst
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_text.rst
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-26 14:23:47.000000 dhlab-2.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-26 14:23:47.000000 dhlab-2.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-26 14:23:59.506018 dhlab-2.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-26 14:23:47.000000 dhlab-2.9.5/tests/test_nbtext.py
+-rw-r--r--   0        0        0     7242 2023-08-07 07:57:39.716202 dhlab-3.0.0a3/CHANGELOG.md
+-rw-r--r--   0        0        0     1076 2023-08-07 07:57:39.716202 dhlab-3.0.0a3/LICENSE
+-rw-r--r--   0        0        0     2340 2023-08-07 07:57:39.716202 dhlab-3.0.0a3/README.md
+-rw-r--r--   0        0        0      600 2023-08-07 07:57:39.716202 dhlab-3.0.0a3/dhlab/__init__.py
+-rw-r--r--   0        0        0       87 2023-08-07 07:57:39.716202 dhlab-3.0.0a3/dhlab/api/__init__.py
+-rw-r--r--   0        0        0    35119 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/api/dhlab_api.py
+-rw-r--r--   0        0        0     1950 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/api/nb_ngram_api.py
+-rw-r--r--   0        0        0     5036 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/api/nb_search_api.py
+-rw-r--r--   0        0        0      358 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/constants.py
+-rw-r--r--   0        0        0    72064 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/css_style_sheets/grade3.css
+-rw-r--r--   0        0        0    72138 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/css_style_sheets/monokai.css
+-rw-r--r--   0        0        0      922 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/css_style_sheets/nb_notebook.css
+-rw-r--r--   0        0        0     1008 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/css_style_sheets/nb_notebook_2.css
+-rw-r--r--   0        0        0      996 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/css_style_sheets/nb_notebook_blue.css
+-rw-r--r--   0        0        0       38 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/images/__init__.py
+-rw-r--r--   0        0        0     4383 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/images/nbpictures.py
+-rw-r--r--   0        0        0       27 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/metadata/__init__.py
+-rw-r--r--   0        0        0      412 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/metadata/metadata.py
+-rw-r--r--   0        0        0     2184 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/metadata/natbib.py
+-rw-r--r--   0        0        0    14068 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/nbpictures.py
+-rw-r--r--   0        0        0     9708 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/nbtokenizer.py
+-rw-r--r--   0        0        0        1 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/ngram/__init__.py
+-rw-r--r--   0        0        0     3156 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/ngram/nb_ngram.py
+-rw-r--r--   0        0        0     2504 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/ngram/ngram.py
+-rw-r--r--   0        0        0        1 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/__init__.py
+-rw-r--r--   0        0        0      916 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/chunking.py
+-rw-r--r--   0        0        0     1206 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/collocations.py
+-rw-r--r--   0        0        0     1168 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/concordance.py
+-rw-r--r--   0        0        0     2034 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/corpus.py
+-rw-r--r--   0        0        0     1377 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/dispersion.py
+-rw-r--r--   0        0        0      721 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/frequencies.py
+-rw-r--r--   0        0        0      990 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/utils.py
+-rw-r--r--   0        0        0      578 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/text/wildcard.py
+-rw-r--r--   0        0        0     1784 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/utils/__init__.py
+-rw-r--r--   0        0        0     2274 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/utils/display.py
+-rw-r--r--   0        0        0     3840 2023-08-07 07:57:39.720202 dhlab-3.0.0a3/dhlab/utils/files.py
+-rw-r--r--   0        0        0     2016 2023-08-07 07:57:50.656209 dhlab-3.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3851 1970-01-01 00:00:00.000000 dhlab-3.0.0a3/PKG-INFO
```

### Comparing `dhlab-2.9.5/dhlab/api/dhlab_api.py` & `dhlab-3.0.0a3/dhlab/api/dhlab_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,92 @@
 from typing import Union, List, Tuple, Dict
 
 import pandas as pd
 import requests
+
+# from requests import HTTPError, JSONDecodeError, ConnectionError
 from pandas import DataFrame, Series
 
 from dhlab.constants import BASE_URL
 
 pd.options.display.max_rows = 100
 
+# wildcard search for words
+
+
+def wildcard_search(word, factor=2, freq_limit=10, limit=50):
+    res = requests.get(
+        f"{BASE_URL}/wildcard_word_search",
+        params={"word": word, "factor": factor, "freq_lim": freq_limit, "limit": limit},
+    )
+    # columns = ["key", "name", "alternatename", "latitude", "longitude", "feature class", "feature code"]
+    return pd.DataFrame.from_dict(res.json(), orient="index", columns=["freq"])
+
 
 # fetch metadata
 
 
-def ner_from_urn(urn: str = None, model: str = None) -> DataFrame:
+def images(text=None, part=True):
+    """Retrive images from bokhylla
+    :param text: fulltext query expression for sqlite
+    :param part: if a number the whole page is shown
+    ... bug prevents these from going thru
+    :param delta: if part=True then show additional pixels around image
+    :parsm hits: number of images"""
+
+    params = locals()
+    r = requests.get(f"{BASE_URL}/images", params=params)
+    js = r.json()
+    return js
+
+
+def ner_from_urn(
+    urn: str = None, model: str = None, start_page=0, to_page=0
+) -> DataFrame:
     """Get NER annotations for a text (``urn``) using a spacy ``model``.
 
     :param str urn: uniform resource name, example: ``URN:NBN:no-nb_digibok_2011051112001``
     :param str model: name of a spacy model.
         Check which models are available with :func:`show_spacy_models`
     :return: Dataframe with annotations and their frequencies
     """
 
     params = locals()
     r = requests.get(f"{BASE_URL}/ner_urn", params=params)
     df = pd.read_json(r.json())
     return df
 
 
-def pos_from_urn(urn: str = None, model: str = None) -> DataFrame:
+def pos_from_urn(
+    urn: str = None, model: str = None, start_page=0, to_page=0
+) -> DataFrame:
     """Get part of speech tags and dependency parse annotations for a text (``urn``) with a SpaCy ``model``.
 
     :param str urn: uniform resource name, example: ``URN:NBN:no-nb_digibok_2011051112001``
     :param str model: name of a spacy model.
         Check which models are available with :func:`show_spacy_models`
     :return: Dataframe with annotations and their frequencies
     """
     params = locals()
     r = requests.get(f"{BASE_URL}/pos_urn", params=params)
     df = pd.read_json(r.json())
     return df
 
 
-def show_spacy_models():
+def show_spacy_models() -> List:
     """Show available SpaCy model names."""
-    r = requests.get(f"{BASE_URL}/ner_models")
-    return r.json()
+    try:
+        r = requests.get(f"{BASE_URL}/ner_models")
+        # r.raise_for_status()
+        res = r.json()
+    except:  # (HTTPError, JSONDecodeError, ConnectionError) as error:
+        # print(error.__doc__, error)
+        print("Server-request gikk ikke gjennom. Kan ikke vise SpaCy-modellnavn.")
+        res = []
+    return res
 
 
 def get_places(urn: str) -> DataFrame:
     """Look up placenames in a specific URN.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/places <https://api.nb.no/dhlab/#/default/post_places>`_.
@@ -58,18 +96,18 @@
     params = locals()
     r = requests.post(f"{BASE_URL}/places", json=params)
     # print(r.status_code)
     return pd.DataFrame(r.json())
 
 
 def geo_lookup(
-        places: List,
-        feature_class: str = None,
-        feature_code: str = None,
-        field: str = "alternatename",
+    places: List,
+    feature_class: str = None,
+    feature_code: str = None,
+    field: str = "alternatename",
 ) -> DataFrame:
     """From a list of places, return their geolocations
 
     :param list places: a list of place names - max 1000
     :param str feature_class: which GeoNames feature class to return. Example: ``P``
     :param str feature_code: which GeoNames feature code to return. Example: ``PPL``
     :param str field: which name field to match - default "alternatename".
@@ -92,18 +130,18 @@
         "feature_class",
         "feature_code",
     ]
     return pd.DataFrame(res.json(), columns=columns)
 
 
 def get_dispersion(
-        urn: str = None,
-        words: List = None,
-        window: int = 300,
-        pr: int = 100,
+    urn: str = None,
+    words: List = None,
+    window: int = 300,
+    pr: int = 100,
 ) -> Series:
     """Count occurrences of words in the given URN object.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint ``/dispersion``.
 
     :param str urn: uniform resource name, example: ``URN:NBN:no-nb_digibok_2011051112001``
     :param list words: list of words. Defaults to a list of punctuation marks.
@@ -126,25 +164,33 @@
         ``["URN:NBN:no-nb_digibok_2008051404065", "URN:NBN:no-nb_digibok_2010092120011"]``
     """
     params = locals()
     r = requests.post(f"{BASE_URL}/get_metadata", json=params)
     return DataFrame(r.json())
 
 
+def get_identifiers(identifiers: list = None) -> list:
+    """Convert a list of identifiers, oaiid, sesamid, urns or isbn10 to dhlabids"""
+    res = requests.post(
+        f"{BASE_URL}/identifiers",
+        json={"identifiers": [i for i in identifiers if i != ""]},
+    )
+    return res.json()
+
+
 def get_chunks(urn: str = None, chunk_size: int = 300) -> Union[Dict, List]:
     """Get the text in the document ``urn`` as frequencies of chunks
      of the given ``chunk_size``.
 
     Calls the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     ``/chunks``.
 
     :param str urn: uniform resource name, example: ``URN:NBN:no-nb_digibok_2011051112001``
     :param int chunk_size: Number of tokens to include in each chunk.
     :return: list of dicts with the resulting chunk frequencies, or an empty dict
-    .. todo:: Verify unit of ``chunk_size``
     """
 
     if urn is None:
         return {}
     r = requests.get(f"{BASE_URL}/chunks", params=locals())
     if r.status_code == 200:
         result = r.json()
@@ -187,19 +233,19 @@
         f"{BASE_URL}/evaluate", json={"wordbags": wordbags, "urns": urns}
     )
     df = pd.DataFrame(res.json()).transpose()
     return df
 
 
 def get_reference(
-        corpus: str = "digavis",
-        from_year: int = 1950,
-        to_year: int = 1955,
-        lang: str = "nob",
-        limit: int = 100000,
+    corpus: str = "digavis",
+    from_year: int = 1950,
+    to_year: int = 1955,
+    lang: str = "nob",
+    limit: int = 100000,
 ) -> DataFrame:
     """Reference frequency list of the n most frequent words from a given corpus in a given period.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/reference_corpus <https://api.nb.no/dhlab/#/default/get_reference_corpus>`_.
 
     :param str corpus: Document type to include in the corpus, can be either ``'digibok'`` or
@@ -236,23 +282,23 @@
         res = pd.DataFrame.from_dict(r.json(), orient="index", columns=["urn"])
     else:
         res = pd.DataFrame()
     return res
 
 
 def _ngram_doc(
-        doctype: str = None,
-        word: Union[List, str] = ["."],
-        title: str = None,
-        period: Tuple[int, int] = None,
-        publisher: str = None,
-        lang: str = None,
-        city: str = None,
-        ddk: str = None,
-        topic: str = None,
+    doctype: str = None,
+    word: Union[List, str] = ["."],
+    title: str = None,
+    period: Tuple[int, int] = None,
+    publisher: str = None,
+    lang: str = None,
+    city: str = None,
+    ddk: str = None,
+    topic: str = None,
 ) -> DataFrame:
     """Count occurrences of one or more words over a time period.
 
     The type of document to search through is decided by the ``doctype``.
     Filter the selection of documents with metadata.
     Use % as wildcard where appropriate - no wildcards in ``word`` or ``lang``.
 
@@ -288,18 +334,18 @@
     df = pd.concat([df.loc[x] for x in columns], axis=1)
     df.columns = columns
     # df.index = df.index.map(pd.Timestamp)
     return df
 
 
 def reference_words(
-        words: List = None,
-        doctype: str = "digibok",
-        from_year: Union[str, int] = 1800,
-        to_year: Union[str, int] = 2000,
+    words: List = None,
+    doctype: str = "digibok",
+    from_year: Union[str, int] = 1800,
+    to_year: Union[str, int] = 2000,
 ) -> DataFrame:
     """Collect reference data for a list of words over a time period.
 
     Reference data are the absolute and relative frequencies of the ``words``
     across all documents of the given ``doctype`` in the given time period
     (``from_year`` - ``to_year``).
 
@@ -322,23 +368,75 @@
     if r.status_code == 200:
         res = pd.DataFrame(r.json(), columns=["word", "freq", "relative"])
     else:
         res = pd.DataFrame()
     return res
 
 
+def _ngram_doc(
+    doctype: str = None,
+    word: Union[List, str] = ["."],
+    title: str = None,
+    period: Tuple[int, int] = None,
+    publisher: str = None,
+    lang: str = None,
+    city: str = None,
+    ddk: str = None,
+    topic: str = None,
+) -> pd.DataFrame:
+    """Count occurrences of one or more words over a time period.
+
+    The type of document to search through is decided by the ``endpoint``.
+    Filter the selection of documents with metadata.
+    Use % as wildcard where appropriate - no wildcards in ``word`` or ``lang``.
+
+    :param str doctype: API endpoint for the document type to get ngrams for.
+        Can be ``'book'``, ``'periodicals'``, or ``'newspapers'``.
+    :param word: Word(s) to search for.
+        Can be several words in a single string, separated by comma.
+    :type word: str or list of str
+    :param title: Title of a specific document to search through.
+    :param tuple[int,int] period: Start and end years of a time period,
+        given as ``(start year, end year)``.
+    :param str publisher: Name of a publisher.
+    :param str lang: Language as a 3-letter ISO code (e.g. ``"nob"`` or ``"nno"``)
+    :param str city: City of publication.
+    :param str ddk: `Dewey Decimal Classification
+        <https://no.wikipedia.org/wiki/Deweys_desimalklassifikasjon>`_ identifier.
+    :param str topic: Topic of the documents.
+    :return: a `pandas.DataFrame` with the resulting frequency counts of the word(s),
+        spread across years. One year per row.
+    """
+    params = locals()
+    if isinstance(word, str):
+        # assume a comma separated string
+        word = [w.strip() for w in word.split(",")]
+    params["word"] = tuple(word)
+    params = {x: params[x] for x in params if not params[x] is None}
+    r = requests.post(BASE_URL + "/ngram_" + doctype, json=params)
+    # print(r.status_code)
+    df = pd.DataFrame.from_dict(r.json(), orient="index")
+    df.index = df.index.map(lambda x: tuple(x.split()))
+    columns = df.index.levels[0]
+    df = pd.concat([df.loc[x] for x in columns], axis=1)
+    df.columns = columns
+    # df.index = df.index.map(pd.Timestamp)
+    return df
+
+
+# @_docstring_parameters_from(_ngram_doc, drop="doctype")
 def ngram_book(
-        word: Union[List, str] = ["."],
-        title: str = None,
-        period: Tuple[int, int] = None,
-        publisher: str = None,
-        lang: str = None,
-        city: str = None,
-        ddk: str = None,
-        topic: str = None,
+    word: Union[List, str] = ["."],
+    title: str = None,
+    period: Tuple[int, int] = None,
+    publisher: str = None,
+    lang: str = None,
+    city: str = None,
+    ddk: str = None,
+    topic: str = None,
 ) -> DataFrame:
     """Count occurrences of one or more words in books over a given time period.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/ngram_book`.
 
     Filter the selection of books with metadata.
@@ -359,38 +457,39 @@
     :param str topic: Topic of the documents.
     :return: a ``pandas.DataFrame`` with the resulting frequency counts of the word(s),
         spread across years. One year per row.
     """
     params = locals()
     if isinstance(word, str):
         # assume a comma separated string
-        word = [w.strip() for w in word.split(',')]
-    params['word'] = tuple(word)
+        word = [w.strip() for w in word.split(",")]
+    params["word"] = tuple(word)
     params = {x: params[x] for x in params if not params[x] is None}
     r = requests.post(BASE_URL + "/ngram_book", json=params)
     # print(r.status_code)
-    df = pd.DataFrame.from_dict(r.json(), orient='index')
+    df = pd.DataFrame.from_dict(r.json(), orient="index")
     df.index = df.index.map(lambda x: tuple(x.split()))
     columns = df.index.levels[0]
     df = pd.concat([df.loc[x] for x in columns], axis=1)
     df.columns = columns
     # df.index = df.index.map(pd.Timestamp)
     return df
 
 
+# @_docstring_parameters_from(_ngram_doc, drop="doctype")
 def ngram_periodicals(
-        word: Union[List, str] = ["."],
-        title: str = None,
-        period: Tuple[int, int] = None,
-        publisher: str = None,
-        lang: str = None,
-        city: str = None,
-        ddk: str = None,
-        topic: str = None,
-        **kwargs,
+    word: Union[List, str] = ["."],
+    title: str = None,
+    period: Tuple[int, int] = None,
+    publisher: str = None,
+    lang: str = None,
+    city: str = None,
+    ddk: str = None,
+    topic: str = None,
+    **kwargs,
 ) -> DataFrame:
     """Get a time series of frequency counts for ``word`` in periodicals.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/ngram_periodicals`.
 
     :param word: Word(s) to search for.
@@ -408,32 +507,32 @@
     :param str topic: Topic of the documents.
     :return: a ``pandas.DataFrame`` with the resulting frequency counts of the word(s),
         spread across years. One year per row.
     """
     params = locals()
     if isinstance(word, str):
         # assume a comma separated string
-        word = [w.strip() for w in word.split(',')]
-    params['word'] = tuple(word)
+        word = [w.strip() for w in word.split(",")]
+    params["word"] = tuple(word)
     params = {x: params[x] for x in params if not params[x] is None}
     r = requests.post(BASE_URL + "/ngram_periodicals", json=params)
     # print(r.status_code)
-    df = pd.DataFrame.from_dict(r.json(), orient='index')
+    df = pd.DataFrame.from_dict(r.json(), orient="index")
     df.index = df.index.map(lambda x: tuple(x.split()))
     columns = df.index.levels[0]
     df = pd.concat([df.loc[x] for x in columns], axis=1)
     df.columns = columns
     # df.index = df.index.map(pd.Timestamp)
     return df
 
 
 def ngram_news(
-        word: Union[List, str] = ["."],
-        title: str = None,
-        period: Tuple[int, int] = None,
+    word: Union[List, str] = ["."],
+    title: str = None,
+    period: Tuple[int, int] = None,
 ) -> DataFrame:
     """Get a time series of frequency counts for ``word`` in newspapers.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/ngram_newspapers`.
 
     :param word: Word(s) to search for.
@@ -445,40 +544,40 @@
     :type period: tuple of ints
     :return: a ``pandas.DataFrame`` with the resulting frequency counts of the word(s),
         spread across the dates given in the time period. Either one year or one day per row.
     """
     params = locals()
     if isinstance(word, str):
         # assume a comma separated string
-        word = [w.strip() for w in word.split(',')]
-    params['word'] = tuple(word)
+        word = [w.strip() for w in word.split(",")]
+    params["word"] = tuple(word)
     params = {x: params[x] for x in params if not params[x] is None}
     r = requests.post(BASE_URL + "/ngram_newspapers", json=params)
     # print(r.status_code)
-    df = pd.DataFrame.from_dict(r.json(), orient='index')
+    df = pd.DataFrame.from_dict(r.json(), orient="index")
     df.index = df.index.map(lambda x: tuple(x.split()))
     columns = df.index.levels[0]
     df = pd.concat([df.loc[x] for x in columns], axis=1)
     df.columns = columns
     # df.index = df.index.map(pd.Timestamp)
     return df
 
 
 def get_document_frequencies(
-        urns: List[str] = None, cutoff: int = 0, words: List[str] = None
+    urns: List[str] = None, cutoff: int = 0, words: List[str] = None
 ) -> DataFrame:
     """Fetch frequency counts of ``words`` in documents (``urns``).
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/frequencies`.
 
     :param list urns: list of uniform resource name strings, for example:
         ``["URN:NBN:no-nb_digibok_2008051404065", "URN:NBN:no-nb_digibok_2010092120011"]``
     :param int cutoff: minimum frequency of a word to be counted
-    :param list words: a list of words to be counted - if left None, whole document is returned.
+    :param list words: a list of words to be counted - if left None, whole document is returned. If not None both the counts and their relative frequency is returned.
     """
     params = locals()
     r = requests.post(f"{BASE_URL}/frequencies", json=params)
     result = r.json()
     # check if words are passed - return differs a bit
     if words is None:
         structure = dict()
@@ -487,53 +586,80 @@
                 structure[u[0][0]] = dict([(x[1], x[2]) for x in u])
             except IndexError:
                 pass
         df = pd.DataFrame(structure)
         df = df.sort_values(by=df.columns[0], ascending=False).fillna(0)
     else:
         df = pd.DataFrame(result)
-        df.columns = ["urn", "word", "count", "urncount"]
-        df = pd.pivot_table(df, values="count", index="word", columns="urn").fillna(0)
+        df.columns = ["urn", "word", "freq", "urncount"]
+        df["relfreq"] = df["freq"] / df.urncount
+        df = pd.pivot_table(
+            df, values=["freq", "relfreq"], index="word", columns="urn"
+        ).fillna(0)
     return df
 
 
 def get_word_frequencies(
-        urns: List[str] = None, cutoff: int = 0, words: List[str] = None
+    urns: List[str] = None, cutoff: int = 0, words: List[str] = None
 ) -> DataFrame:
     """Fetch frequency numbers for ``words`` in documents (``urns``).
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/frequencies`.
 
     :param list urns: list of uniform resource name strings, for example:
         ``["URN:NBN:no-nb_digibok_2008051404065", "URN:NBN:no-nb_digibok_2010092120011"]``
     :param int cutoff: minimum frequency of a word to be counted
     :param list words: a list of words to be counted - should not be left None.
     """
     return get_document_frequencies(urns, cutoff, words)
 
 
+def get_urn_frequencies(urns: List[str] = None, dhlabid: List = None) -> DataFrame:
+    """Fetch frequency counts of documents as URNs or DH-lab ids.
+
+    Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
+    `/frequencies`.
+
+    :param list urns: list of uniform resource name strings, for example:
+        ``["URN:NBN:no-nb_digibok_2008051404065", "URN:NBN:no-nb_digibok_2010092120011"]``
+    :param list dhlabid: list of numbers for dhlabid:
+        ``[1000001, 2000003]``
+    """
+    if dhlabid == None:
+        params = {"urns": urns}
+    else:
+        params = {"dhlabid": dhlabid}
+    r = requests.post(f"{BASE_URL}/urn_frequencies", json=params)
+    result = r.json()
+    # check if words are passed - return differs a bit
+    df = pd.DataFrame(result)
+    df.columns = ["urn", "freq"]
+    return df
+
+
 def get_document_corpus(**kwargs):
     return document_corpus(**kwargs)
 
 
 def document_corpus(
-        doctype: str = None,
-        author: str = None,
-        freetext: str = None,
-        fulltext: str = None,
-        from_year: int = None,
-        to_year: int = None,
-        from_timestamp: int = None,
-        to_timestamp: int = None,
-        title: str = None,
-        ddk: str = None,
-        subject: str = None,
-        lang: str = None,
-        limit: int = None,
+    doctype: str = None,
+    author: str = None,
+    freetext: str = None,
+    fulltext: str = None,
+    from_year: int = None,
+    to_year: int = None,
+    from_timestamp: int = None,
+    to_timestamp: int = None,
+    title: str = None,
+    ddk: str = None,
+    subject: str = None,
+    lang: str = None,
+    limit: int = None,
+    order_by: str = None,
 ) -> DataFrame:
     """Fetch a corpus based on metadata.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/build_corpus <https://api.nb.no/dhlab/#/default/post_build_corpus>`_.
 
     :param str doctype: ``"digibok"``, ``"digavis"``, ``"digitidsskrift"`` or ``"digistorting"``
@@ -549,30 +675,31 @@
     :param str title: Name or title of a document.
     :param str ddk: `Dewey Decimal Classification
         <https://no.wikipedia.org/wiki/Deweys_desimalklassifikasjon>`_ identifier.
     :param str subject: subject (keywords) of the publication.
     :param str lang: Language of the publication, as a 3-letter ISO code.
         Example: ``"nob"`` or ``"nno"``
     :param int limit: number of items to sample.
+    :param str order_by: order of elements in the corpus object. Typically used in combination with a limit. Example ``"random"`` (random order, the slowest), ``"rank"`` (ordered by relevance, faster) or ``"first"`` (breadth-first, using the order in the database table, the fastest method)
     :return: a ``pandas.DataFrame`` with the corpus information.
     """
     parms = locals()
     params = {x: parms[x] for x in parms if not parms[x] is None}
 
     r = requests.post(BASE_URL + "/build_corpus", json=params)
 
     return pd.DataFrame(r.json())
 
 
 def urn_collocation(
-        urns: List = None,
-        word: str = "arbeid",
-        before: int = 5,
-        after: int = 0,
-        samplesize: int = 200000,
+    urns: List = None,
+    word: str = "arbeid",
+    before: int = 5,
+    after: int = 0,
+    samplesize: int = 200000,
 ) -> DataFrame:
     """Create a collocation from a list of URNs.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/urncolldist_urn`.
 
     :param list urns: list of uniform resource name strings, for example:
@@ -589,15 +716,15 @@
         "urn": urns,
         "word": word,
         "before": before,
         "after": after,
         "samplesize": samplesize,
     }
     r = requests.post(BASE_URL + "/urncolldist_urn", json=params)
-    return pd.read_json(r.text)
+    return pd.read_json(r.json())
 
 
 def totals(top_words: int = 50000) -> DataFrame:
     """Get aggregated raw frequencies of all words in the National Library's database.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/totals/{top_words} <https://api.nb.no/dhlab/#/default/get_totals__top_words_>`_.
@@ -606,15 +733,15 @@
     :return: a ``pandas.DataFrame`` with the most frequent words.
     """
     r = requests.get(BASE_URL + f"/totals/{top_words}")
     return pd.DataFrame.from_dict(dict(r.json()), orient="index", columns=["freq"])
 
 
 def concordance(
-        urns: list = None, words: str = None, window: int = 25, limit: int = 100
+    urns: list = None, words: str = None, window: int = 25, limit: int = 100
 ) -> DataFrame:
     """Get a list of concordances from the National Library's database.
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/conc <https://api.nb.no/dhlab/#/default/post_conc>`_.
 
     :param list urns: uniform resource names, for example:
@@ -630,15 +757,15 @@
     else:
         params = {"urns": urns, "query": words, "window": window, "limit": limit}
         r = requests.post(BASE_URL + "/conc", json=params)
     return pd.DataFrame(r.json())
 
 
 def concordance_counts(
-        urns: list = None, words: str = None, window: int = 25, limit: int = 100
+    urns: list = None, words: str = None, window: int = 25, limit: int = 100
 ) -> DataFrame:
     """Count concordances (keyword in context) for a corpus query (used for collocation analysis).
 
     Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
     `/conccount <https://api.nb.no/dhlab/#/default/post_conccount>`_.
 
     :param list urns: uniform resource names, for example:
@@ -654,22 +781,83 @@
     else:
         params = {"urns": urns, "query": words, "window": window, "limit": limit}
         r = requests.post(BASE_URL + "/conccount", json=params)
     return pd.DataFrame(r.json())
 
 
 def konkordans(
-        urns: list = None, words: str = None, window: int = 25, limit: int = 100
+    urns: list = None, words: str = None, window: int = 25, limit: int = 100
 ):
     """Wrapper for :func:`concordance`."""
     return concordance(**locals())
 
 
+def word_concordance(
+    urn: list = None,
+    dhlabid: list = None,
+    words: list = None,
+    before: int = 12,
+    after: int = 12,
+    limit: int = 100,
+    samplesize: int = 50000,
+) -> DataFrame:
+    """Get a list of concordances from the National Library's database.
+
+    Call the API :py:obj:`~dhlab.constants.BASE_URL` endpoint
+    `/conc <https://api.nb.no/dhlab/#/default/conc_word_urn>`_.
+
+    :param list urns: dhlab serial ids. (server can take both urns and dhlabid but so we may rewrite this to)
+    :param str words: Word(s) to search for -- must be a list
+    :param int before: between 0-24.
+    :param int after: between 0-24 (before + sum <= 24)
+    :param int limit: max. number of concordances per server process.
+    :param int samplesize: samples from urns.
+    :return: a table of concordances
+    """
+
+    # server checks if either dhlabid or urns are present in the parameters, so only one of them
+    # is passed. The return is dhlabid anyhow.
+
+    if dhlabid is not None:
+        params = {
+            "dhlabid": dhlabid,
+            "words": words,
+            "before": before,
+            "after": after,
+            "limit": limit,
+            "samplesize": samplesize,
+        }
+    elif urns is not None:
+        params = {
+            "urn": urns,
+            "words": words,
+            "before": before,
+            "after": after,
+            "limit": limit,
+            "samplesize": samplesize,
+        }
+    else:
+        params = {
+            "words": words,
+            "before": before,
+            "after": after,
+            "limit": limit,
+            "samplesize": samplesize,
+        }
+
+    r = requests.post(BASE_URL + "/conc_word_urn", json=params)
+
+    return pd.DataFrame(
+        [x for y in r.json() for x in y],
+        columns=["dhlabid", "before", "target", "after"],
+    )
+
+
 def collocation(
-        corpusquery: str = "norge", word: str = "arbeid", before: int = 5, after: int = 0
+    corpusquery: str = "norge", word: str = "arbeid", before: int = 5, after: int = 0
 ) -> DataFrame:
     """Make a collocation from a corpus query.
 
     :param str corpusquery: query string
     :param str word: target word for the collocations.
     :param int before: number of words prior to ``word``
     :param int after: number of words following ``word``
@@ -678,15 +866,15 @@
     params = {
         "metadata_query": corpusquery,
         "word": word,
         "before": before,
         "after": after,
     }
     r = requests.post(BASE_URL + "/urncolldist", json=params)
-    return pd.read_json(r.text)
+    return pd.read_json(r.json())
 
 
 # Norwegian word bank
 
 
 def word_variant(word: str, form: str, lang: str = "nob") -> list:
     """Find alternative ``form`` for a given ``word`` form.
```

### Comparing `dhlab-2.9.5/dhlab/api/nb_search_api.py` & `dhlab-3.0.0a3/dhlab/api/nb_search_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,164 @@
+from typing import Iterable
+
 import pandas as pd
 import requests
 
 
-def load_picture(url):
+def load_picture(url: str):
+    """Load the raw image object from a URL."""
     r = requests.get(url, stream=True)
     r.raw.decode_content = True
     # print(r.status_code)
     return r.raw
 
 
-def iiif_manifest(urn):
+def iiif_manifest(urn: str):
+    """Fetch the IIIF manifest of the images that the book"""
     r = requests.get(f"https://api.nb.no/catalog/v1/iiif/{urn}/manifest")
     return r.json()
 
 
-def mods(urn):
+def mods(urn: str):
     r = requests.get(f"https://api.nb.no:443/catalog/v1/metadata/{urn}/mods")
     return r.json()
 
 
-def super_search(term, number=50, page=0, mediatype='bilder'):
-    """Søk etter term og få ut json"""
+def super_search(
+    term: str, number: int = 50, page: int = 0, mediatype: str = "bilder"
+) -> dict:
+    """Search for a term, return a json object with the matches.
+
+    :param str term: Search term, word, or token. Default is the empty string.
+    :param int number: Size of the response. Maximum 50.
+    :param int page: The page number to search from.
+        .. todo:: Fill in description.
+    :param str mediatype: Default 'bilder'.
+        .. todo::  Which other value options are available for this parameter?
+    :return: a dict (json object) with the search results.
+    """
+    url = "https://api.nb.no:443/catalog/v1/items"
     number = min(number, 50)
-    if term == '':
+    if term == "":
         r = requests.get(
-            "https://api.nb.no:443/catalog/v1/items",
-            params={
-                'filter': f'mediatype:{mediatype}',
-                'page': page,
-                'size': number
-            }
+            url,
+            params={"filter": f"mediatype:{mediatype}", "page": page, "size": number},
         )
     else:
         r = requests.get(
-            "https://api.nb.no:443/catalog/v1/items",
+            url,
             params={
-                'q': term,
-                'filter': f'mediatype:{mediatype}',
-                'page': page,
-                'size': number
-            }
+                "q": term,
+                "filter": f"mediatype:{mediatype}",
+                "page": page,
+                "size": number,
+            },
         )
     return r.json()
 
 
-def total_search(size=50, page=0):
-    """Finn de første antallet = 'size' fra side 'page' og få ut json"""
-    size = min(size, 50)
-    r = requests.get(
-        "https://api.nb.no:443/catalog/v1/items",
-        params={
-            'filter': 'mediatype:bilder',
-            'page': page,
-            'size': size
-        }
-    )
-    return r.json()
-
+def total_search(size: int = 50, page: int = 0) -> dict:
+    """Retrieve the first ``size`` occurrences from ``page``.
 
-def get_df(frases, title='aftenposten'):
-    """get document phrases"""
-    querystring = " + ".join(['"' + frase + '"' for frase in frases])
-    query = {
-        'q': querystring,
-        'size': 1,
-        'aggs': 'year',
+    Wrapper-function for :func:`super_search` with arguments
+    ``medietype="bilder"`` and ``term=''``.
+    """
+    return super_search(term="", number=size, page=page, mediatype="bilder")
+
+
+def get_df(phrases: Iterable, title: str = "aftenposten"):
+    """Get ``phrases`` from documents of ``title``, and aggregate their frequencies."""
+    querystring = " + ".join(['"' + frase + '"' for frase in phrases])
+    query = {
+        "q": querystring,
+        "size": 1,
+        "aggs": "year",
         # 'filter':'mediatype:{mt}'.format(mt=media),
-        'filter': f'title:{title}'
+        "filter": f"title:{title}",
     }
     r = requests.get("https://api.nb.no/catalog/v1/items", params=query)
-    aggs = r.json()['_embedded']['aggregations'][0]['buckets']
-    return {x['key']: x['count'] for x in aggs}
-
+    aggs = r.json()["_embedded"]["aggregations"][0]["buckets"]
+    return {x["key"]: x["count"] for x in aggs}
 
-def get_json(frases, mediatype='aviser'):
 
-    querystring = " + ".join(['"' + frase + '"' for frase in frases])
+def get_json(phrases, mediatype="aviser"):
+    querystring = " + ".join(['"' + frase + '"' for frase in phrases])
     query = {
-        'q': querystring,
-        'size': 1,
-        'snippets': mediatype,
-        'aggs': 'year',
-
+        "q": querystring,
+        "size": 1,
+        "snippets": mediatype,
+        "aggs": "year",
         #        'filter':'mediatype:{mt}'.format(mt=mediatype),
-        'searchType': 'FULL_TEXT_SEARCH'
+        "searchType": "FULL_TEXT_SEARCH"
         # 'filter':'title:{title}'.format(title=title)
     }
     r = requests.get("https://api.nb.no/catalog/v1/items", params=query)
     aggs = r.json()
     return aggs
 
 
-def get_data(frase, media='avis', title='jazznytt'):
-
+def get_data(frase, media="avis", title="jazznytt"):
     query = {
-        'q': '"' + frase + '""',
-        'size': 1,
-        'aggs': 'year',
-        'filter': 'mediatype:{mt}'.format(mt=media),
-        'filter': 'title:{title}'.format(title=title)
+        "q": '"' + frase + '""',
+        "size": 1,
+        "aggs": "year",
+        "filter": "mediatype:{mt}".format(mt=media),
+        "filter": "title:{title}".format(title=title),
     }
     r = requests.get("https://api.nb.no/catalog/v1/items", params=query)
     return r.json()
 
 
-def get_data_and(frases, title='aftenposten', media='avis'):
-
+def get_data_and(frases, title="aftenposten", media="avis"):
     querystring = " + ".join(['"' + frase + '"' for frase in frases])
     print(querystring)
     query = {
-        'q': querystring,
-        'size': 1,
-        'aggs': 'year',
+        "q": querystring,
+        "size": 1,
+        "aggs": "year",
         # 'filter':'mediatype:{mt}'.format(mt=media),
-        'filter': 'title:{title}'.format(title=title)
+        "filter": "title:{title}".format(title=title),
     }
     r = requests.get("https://api.nb.no/catalog/v1/items", params=query)
     return r.json()
 
 
-def get_df_pd(frase, media='bøker'):
+def get_df_pd(frase, media="bøker"):
     return pd.DataFrame.from_dict(
-        get_df(frase, media=media), orient='index').sort_index()
+        get_df(frase, media=media), orient="index"
+    ).sort_index()
 
 
 def get_konks(urn, phrase, window=1000, n=1000):
-
     querystring = '"' + phrase + '"'
-    query = {
-        'q': querystring,
-        'fragments': n,
-        'fragSize': window
-
-    }
+    query = {"q": querystring, "fragments": n, "fragSize": window}
     r = requests.get(
-        "https://api.nb.no/catalog/v1/items/{urn}/contentfragments".format(urn=urn), params=query)
+        "https://api.nb.no/catalog/v1/items/{urn}/contentfragments".format(urn=urn),
+        params=query,
+    )
     res = r.json()
     results = []
     try:
-        for x in res['contentFragments']:
-            urn = x['pageid']
-            hit = x['text']
-            splits = hit.split('<em>')
-            s2 = splits[1].split('</em>')
+        for x in res["contentFragments"]:
+            urn = x["pageid"]
+            hit = x["text"]
+            splits = hit.split("<em>")
+            s2 = splits[1].split("</em>")
             before = splits[0]
             word = s2[0]
             after = s2[1]
-            results.append({'urn': urn, 'before': before,
-                           'word': word, 'after': after})
+            results.append({"urn": urn, "before": before, "word": word, "after": after})
     except BaseException:
         results = []
     return results
 
 
 def get_phrase_info(urn, phrase, window=1000, n=1000):
-
     querystring = '"' + phrase + '"'
     query = {
-        'q': querystring,
-
+        "q": querystring,
     }
     r = requests.get(
-        f"https://api.nb.no/catalog/v1/items/{urn}/contentfragments",
-        params=query)
+        f"https://api.nb.no/catalog/v1/items/{urn}/contentfragments", params=query
+    )
     res = r.json()
     return res
```

### Comparing `dhlab-2.9.5/dhlab/css_style_sheets/grade3.css` & `dhlab-3.0.0a3/dhlab/css_style_sheets/grade3.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.5/dhlab/css_style_sheets/monokai.css` & `dhlab-3.0.0a3/dhlab/css_style_sheets/monokai.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook.css` & `dhlab-3.0.0a3/dhlab/css_style_sheets/nb_notebook.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_2.css` & `dhlab-3.0.0a3/dhlab/css_style_sheets/nb_notebook_2.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_blue.css` & `dhlab-3.0.0a3/dhlab/css_style_sheets/nb_notebook_blue.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.5/dhlab/images/nbpictures.py` & `dhlab-3.0.0a3/dhlab/images/nbpictures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,132 +1,158 @@
+from typing import Union
 from IPython.display import HTML
 from PIL import Image
 
-from dhlab.api.nb_search_api import iiif_manifest, super_search, total_search, load_picture
+from dhlab.api.nb_search_api import (
+    iiif_manifest,
+    super_search,
+    total_search,
+    load_picture,
+)
 
 
 def pages(urn, scale=800):
     a = iiif_manifest(urn)
-    return [page['images'][0]['resource']['@id'].replace(f"full/full/", "full/0,{s}/") for page in
-            a['sequences'][0]['canvases']]
+    return [
+        page["images"][0]["resource"]["@id"].replace(f"full/full/", "full/0,{s}/")
+        for page in a["sequences"][0]["canvases"]
+    ]
 
 
 def get_url(urn, page=1, part=200):
     # urn as digit
-    urn = "URN:NBN:no-nb_digibok_" + urn + '_{0:04d}'.format(page)
+    urn = "URN:NBN:no-nb_digibok_" + urn + "_{0:04d}".format(page)
     print(urn)
     url = f"https://www.nb.no/services/image/resolver/{urn}/full/0,{part}/native.jpg"
     return url
 
 
 def page_urn(urn, page=1):
     # urn as digit
-    return "URN:NBN:no-nb_digibok_" + urn + '_{0:04d}'.format(page)
+    return "URN:NBN:no-nb_digibok_" + urn + "_{0:04d}".format(page)
 
 
-def find_urls(term, number=50, page=0, mediatype='bilder'):
+def find_urls(term, number=50, page=0, mediatype="bilder"):
     """generates urls from super_search for pictures"""
     x = super_search(term, number, page, mediatype=mediatype)
     try:
         urls = [
-            f['_links']['thumbnail_custom']['href']
-            for f in x['_embedded']['items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-               and 'thumbnail_custom' in f['_links']
+            f["_links"]["thumbnail_custom"]["href"]
+            for f in x["_embedded"]["items"]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
     except:
         urls = []
     return urls
 
 
 def find_urls2(term, number=50, page=0):
     """generates urls from super_search for pictures"""
     x = super_search(term, number, page)
     try:
         urls = [
-            f['_links']['thumbnail_custom']['href']
-            for f in x['_embedded']['mediaTypeResults'][0]['result']['_embedded']['items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-               and 'thumbnail_custom' in f['_links']
+            f["_links"]["thumbnail_custom"]["href"]
+            for f in x["_embedded"]["mediaTypeResults"][0]["result"]["_embedded"][
+                "items"
+            ]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
     except:
-        urls = [' ... hmm ...']
+        urls = [" ... hmm ..."]
     return urls
 
 
-def get_picture_from_urn(urn, width=0, height=300):
+def get_picture_from_urn(urn: Union[int, str], width: int = 0, height: int = 300):
+    """Fetch the Image object with its URN identifier.
+
+    :meta private:
+
+    :param urn: The uniform resource name number
+    :param width: Resolution width of the image.
+    :param height: Resolution height of the image.
+    :return: An :py:class:`~PIL.Image.Image` object.
+    """
     meta = iiif_manifest(urn)
-    if 'error' not in meta:
+    if "error" not in meta:
         if width == 0 and height == 0:
             url = f"https://www.nb.no/services/image/resolver/{urn}/full/full/0/native.jpg"
         else:
             url = f"https://www.nb.no/services/image/resolver/{urn}/full/{width},{height}/0/native.jpg"
         # print(url)
     return Image.open(load_picture(url))
 
 
 def get_picture_from_url(url, width=0, height=300):
-    return Image.open(
-        load_picture(
-            url.format(width=width, height=height)
-        )
-    )
+    return Image.open(load_picture(url.format(width=width, height=height)))
 
 
 def get_metadata_from_url(url):
     import re
+
     urn = re.findall("(URN.*?)(?:/)", url)[0]
     triple = iiif_manifest(urn)
     # print(urn, triple)
     r = dict()
-    if not 'error' in triple:
-        r = {x['label']: x['value'] for x in triple['metadata'] if 'label' in x}
+    if not "error" in triple:
+        r = {x["label"]: x["value"] for x in triple["metadata"] if "label" in x}
     else:
-        r = triple['error']
+        r = triple["error"]
     return r
 
 
 def find_urns(term):
     """From result of super_search, to be fed into iiif_manifest"""
 
     ss = super_search(term)
     urns = [
-        f['metadata']['identifiers']['urn']
-        for f in ss['_embedded']['mediaTypeResults'][0]['result']['_embedded']['items']
-        if 'urn' in f['metadata']['identifiers']
+        f["metadata"]["identifiers"]["urn"]
+        for f in ss["_embedded"]["mediaTypeResults"][0]["result"]["_embedded"]["items"]
+        if "urn" in f["metadata"]["identifiers"]
     ]
     return urns
 
 
 def total_urls(number=50, page=0):
-    """find urls sequentially """
+    """find urls sequentially"""
     x = total_search(number, page)
     try:
         urls = [
-            f['_links']['thumbnail_custom']['href']
-            for f in x['_embedded']['items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-               and 'thumbnail_custom' in f['_links']
+            f["_links"]["thumbnail_custom"]["href"]
+            for f in x["_embedded"]["items"]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
     except:
         urls = []
     return urls
 
 
 def json2html(meta):
-    items = ["<dt>{key}</dt><dd>{val}</dd>".format(key=key, val=meta[key]) for key in meta]
-    result = "<dl>{items}</dl>".format(items=' '.join(items))
+    items = [
+        "<dt>{key}</dt><dd>{val}</dd>".format(key=key, val=meta[key]) for key in meta
+    ]
+    result = "<dl>{items}</dl>".format(items=" ".join(items))
     return result
 
 
 def display_finds(r):
     """A list of urls in r is displayed as HTML"""
-    rows = ["<tr><td><img src='{row}'</td><td>{meta}</td></tr>".format(row=row, meta=json2html(
-        get_metadata_from_url(row))).format(width=0, height=200) for row in r]
-    return HTML("""<html><head></head>
+    rows = [
+        "<tr><td><img src='{row}'</td><td>{meta}</td></tr>".format(
+            row=row, meta=json2html(get_metadata_from_url(row))
+        ).format(width=0, height=200)
+        for row in r
+    ]
+    return HTML(
+        """<html><head></head>
      <body>
      <table>
      {rows}
      </table>
      </body>
      </html>
-     """.format(rows=' '.join(rows)))
+     """.format(
+            rows=" ".join(rows)
+        )
+    )
```

### Comparing `dhlab-2.9.5/dhlab/legacy/nbpictures.py` & `dhlab-3.0.0a3/dhlab/nbpictures.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,150 +6,156 @@
 from PIL import Image
 
 small_scale = 0.59
 large_scale = 1.58
 
 
 def nb_search(
-        term='', creator='',
-        number=50,
-        page=0,
-        mediatype='bøker',
-        lang="nob",
-        period=(18000101, 20401231),
-        extra_filters=None,
-        extra_conditions=None
+    term="",
+    creator="",
+    number=50,
+    page=0,
+    mediatype="bøker",
+    lang="nob",
+    period=(18000101, 20401231),
+    extra_filters=None,
+    extra_conditions=None,
 ):
     """Søk etter term og få ut json"""
     number = min(number, 50)
 
     filters = []
     aq = []
 
     if extra_filters is not None:
         filters += extra_filters
-    params = {
-        'page': page,
-        'size': number
-    }
+    params = {"page": page, "size": number}
     if extra_conditions is not None:
         for x in extra_conditions:
             params[x] = extra_conditions[x]
 
-    if lang != '':
-        aq.append(f'languages:{lang}')
+    if lang != "":
+        aq.append(f"languages:{lang}")
 
-    if creator != '':
-        filters.append(f'creator:{creator}')
+    if creator != "":
+        filters.append(f"creator:{creator}")
 
-    if mediatype != '':
-        filters.append(f'mediatype:{mediatype}')
+    if mediatype != "":
+        filters.append(f"mediatype:{mediatype}")
 
     if period != ():
-        filters.append(f'date:[{period[0]} TO {period[1]}]')
+        filters.append(f"date:[{period[0]} TO {period[1]}]")
 
     if filters:
-        params['filter'] = filters
+        params["filter"] = filters
 
     if aq:
-        params['aq'] = aq
+        params["aq"] = aq
 
-    if term != '':
-        params['q'] = term
+    if term != "":
+        params["q"] = term
 
     r = requests.get("https://api.nb.no:443/catalog/v1/items", params=params)
     return r.json()
 
 
 def div_wrapper(div_content):
     return f"""<div>{div_content}</div>"""
 
 
 def display_books(books, width=100):
-    """A dictionary of urns - urls is displayed """
+    """A dictionary of urns - urls is displayed"""
 
     def html_wrapper(body):
         return f"""<style>
     img {{
         width:{width}px;
         height:auto;
         max-width:100%}}
     </style>
     <body>{body}</body>"""
 
     book_divs = ""
     for u in books:
         mf = iiif_manifest(u)
         thumbnail = f"<img src = '{mf['thumbnail']['@id']}'></img>"
-        metainfo = '\n'.join(
-            [f"<b>{x['label']}</b>{x['value']}" for x in mf['metadata']])
-        imgs = '\n'.join(
-            [f"<img src='{pic_url}'></img>" for pic_url in books[u]])
+        metainfo = "\n".join(
+            [f"<b>{x['label']}</b>{x['value']}" for x in mf["metadata"]]
+        )
+        imgs = "\n".join([f"<img src='{pic_url}'></img>" for pic_url in books[u]])
         book_divs += div_wrapper(thumbnail + metainfo + imgs)
     return html_wrapper(book_divs)
 
 
 def markdown_books(books, width=100):
-    """A dictionary of urns - urls is displayed """
+    """A dictionary of urns - urls is displayed"""
 
     book_divs = ""
     for u in books:
         mf = iiif_manifest(u)
         thumbnail = f"<h3>Forside</h3> <img src='{mf['thumbnail']['@id']}'></img>\n\n"
-        metainfo = '\n'.join([
-            f"<h3>Metadata</h3> <b>{x['label']}</b> {x['value']}"
-            for x in mf['metadata']
-        ])
-        imgs = '\n'.join([
-            f"<img style='float:right' src='{pic_url}' width = {width}></img>"
-            for pic_url in books[u]
-        ])
+        metainfo = "\n".join(
+            [
+                f"<h3>Metadata</h3> <b>{x['label']}</b> {x['value']}"
+                for x in mf["metadata"]
+            ]
+        )
+        imgs = "\n".join(
+            [
+                f"<img style='float:right' src='{pic_url}' width = {width}></img>"
+                for pic_url in books[u]
+            ]
+        )
         book_divs += div_wrapper(thumbnail + metainfo + imgs)
     return book_divs
 
 
 def iiif_manifest(urn):
-    if 'URN' not in str(urn) and 'digibok' not in str(urn):
+    if "URN" not in str(urn) and "digibok" not in str(urn):
         urn = "URN:NBN:no-nb_digibok_" + str(urn)
-    elif 'URN' not in str(urn):
+    elif "URN" not in str(urn):
         urn = "URN:NBN:no-nb_" + str(urn)
     r = requests.get(f"https://api.nb.no/catalog/v1/iiif/{urn}/manifest")
     return r.json()
 
 
 def urns_from_super(
-        term='',
-        creator='',
-        number=50,
-        page=0,
-        mediatype='bøker',
-        lang="nob",
-        period=(18000101, 20401231),
-        filters=None,
-        conditions=None
+    term="",
+    creator="",
+    number=50,
+    page=0,
+    mediatype="bøker",
+    lang="nob",
+    period=(18000101, 20401231),
+    filters=None,
+    conditions=None,
 ):
-    res = nb_search(term, mediatype=mediatype, creator=creator, number=number,
-                    page=page, lang=lang, period=period, extra_filters=filters,
-                    extra_conditions=conditions)
-    ids = [x['metadata']['identifiers'] for x in res['_embedded']['items']]
-    return [x['urn'] for x in ids if 'urn' in x]
+    res = nb_search(
+        term,
+        mediatype=mediatype,
+        creator=creator,
+        number=number,
+        page=page,
+        lang=lang,
+        period=period,
+        extra_filters=filters,
+        extra_conditions=conditions,
+    )
+    ids = [x["metadata"]["identifiers"] for x in res["_embedded"]["items"]]
+    return [x["urn"] for x in ids if "urn" in x]
 
 
 def get_illustration_data_from_book(urn):
-    if 'digibok' in str(urn):
+    if "digibok" in str(urn):
         urn = re.findall("[0-9]{13}", str(urn))[0]
-    r = requests.get(
-        'https://api.nb.no/ngram/illustrations',
-        json={
-            'urn': urn})
+    r = requests.get("https://api.nb.no/ngram/illustrations", json={"urn": urn})
     return r.json()
 
 
-def get_urls_from_illustration_data(
-        illus, part=True, scale=None, cuts=True, delta=0):
+def get_urls_from_illustration_data(illus, part=True, scale=None, cuts=True, delta=0):
     """
     Restricted images must not go over 1024 x 1024 pixels.
 
     :param illus: dictionary of this format:
 
         ``{'height': 270, 'hpos': 251, 'page': 'digibok_2017081626006_0018',
         'resolution': 400, 'vpos': 791, 'width': 373}``
@@ -157,133 +163,139 @@
     :param part: If True, return a cut out of the image
     :param scale: To be filled in
     :param cuts: If true, allow cropping of image
     :param delta: To be filled in
     :return: URL of the image
     """
     if scale is None:
-        if illus['resolution'] >= 300 or illus['resolution'] < 100:
+        if illus["resolution"] >= 300 or illus["resolution"] < 100:
             scale = large_scale
         else:
             scale = small_scale
 
-    height = int(illus['height']) + 2 * delta
-    width = int(illus['width']) + 2 * delta
-    vpos = int(illus['vpos']) - delta
-    hpos = int(illus['hpos']) - delta
+    height = int(illus["height"]) + 2 * delta
+    width = int(illus["width"]) + 2 * delta
+    vpos = int(illus["vpos"]) - delta
+    hpos = int(illus["hpos"]) - delta
 
     if cuts:
         if width * scale > 1024:
             width = int(1024 / scale)
         if height * scale > 1024:
             height = int(1024 / scale)
 
-    urn = "URN:NBN:no-nb_" + illus['page']
+    urn = "URN:NBN:no-nb_" + illus["page"]
     url_prefix = "https://www.nb.no/services/image/resolver"
     if part:
         # return cut out
         url = (
             f"{url_prefix}/"
             f"{urn}/"
             f"{int(hpos * scale)},"
             f"{int(vpos * scale)},"
             f"{int(width * scale)},"
             f"{int(height * scale)}"
             f"/full/0/native.jpg"
         )
     else:
         # return whole page
-        url = (
-            f"{url_prefix}/"
-            f"{urn}/"
-            f"full/"
-            f"0,{part}/"
-            f"0/native.jpg"
-        )
+        url = f"{url_prefix}/" f"{urn}/" f"full/" f"0,{part}/" f"0/native.jpg"
 
     return url
 
 
-def show_illustrations_urn(urn, tilgjengelig='fritt'):
+def show_illustrations_urn(urn, tilgjengelig="fritt"):
     display(
         Markdown(
-            '\n'.join([
-                '**' + x['label'] + '**: ' + x['value']
-                for x in iiif_manifest(urn)['metadata']
-            ])
+            "\n".join(
+                [
+                    "**" + x["label"] + "**: " + x["value"]
+                    for x in iiif_manifest(urn)["metadata"]
+                ]
+            )
         )
     )
 
-    if tilgjengelig.lower().startswith('fri'):
+    if tilgjengelig.lower().startswith("fri"):
         c = False
     else:
         c = True
     return display_finds(
         [
-            get_urls_from_illustration_data(u, cuts=c) for u in
-            get_illustration_data_from_book(urn)
+            get_urls_from_illustration_data(u, cuts=c)
+            for u in get_illustration_data_from_book(urn)
         ]
     )
 
 
 def display_finds_meta(r):
     """A list of urls in r is displayed as HTML"""
-    rows = [(f"<tr><td><img src='{row}'</td><td><a href = {row} target='_'>"
-             f"{row}</a></td></tr>") for row in r]
-    return HTML(f"""<html><head></head>
+    rows = [
+        (
+            f"<tr><td><img src='{row}'</td><td><a href = {row} target='_'>"
+            f"{row}</a></td></tr>"
+        )
+        for row in r
+    ]
+    return HTML(
+        f"""<html><head></head>
      <body>
      <table>
      {' '.join(rows)}
      </table>
      </body>
      </html>
-     """)
+     """
+    )
 
 
 def display_finds(r):
     """A list of urls in r is displayed as HTML"""
     rows = [f"<tr><td><img src='{row}'</td></tr>" for row in r]
-    return HTML(f"""<html><head></head>
+    return HTML(
+        f"""<html><head></head>
      <body>
      <table>
      {' '.join(rows)}
      </table>
      </body>
      </html>
-     """)
+     """
+    )
 
 
 def url2urn(url):
     return re.findall("URN:.*[0-9]{13}", url)[0]
 
 
 def mods(urn):
     r = requests.get(f"https://api.nb.no:443/catalog/v1/metadata/{urn}/mods")
     return r.json()
 
 
 def pages(urn, scale=800):
     a = iiif_manifest(urn)
-    return [page['images'][0]['resource']['@id'].replace(
-        "full/full/", f"full/0,{scale}/"
-    ) for page in a['sequences'][0]['canvases']]
+    return [
+        page["images"][0]["resource"]["@id"].replace("full/full/", f"full/0,{scale}/")
+        for page in a["sequences"][0]["canvases"]
+    ]
 
 
 def load_picture(url):
     r = requests.get(url, stream=True)
     r.raw.decode_content = True
     return r.raw
 
 
 def get_url(urn, page=1, part=200):
     """From a representaion of URN mapped to digibok.
 
-     A URN is a serial number or any string with serial number.
-     """
-    urnserial = re.findall('[0-9]+', str(urn))
+    A URN is a serial number or any string with serial number.
+    """
+    urnserial = re.findall("[0-9]+", str(urn))
     if urnserial:
         urnserial = urnserial[0]
     else:
         return ""
     urn = f"URN:NBN:no-nb_digibok_{urnserial}_{page:04d}"
     print(urn)
     url_prefix = "https://www.nb.no/services/image/resolver"
@@ -292,226 +304,218 @@
 
 
 def page_urn(urn, page=1):
     # urn as digit
     return f"URN:NBN:no-nb_digibok_{urn}_{page:04d}"
 
 
-def super_search(term, number=50, page=0, mediatype='bilder'):
+def super_search(term, number=50, page=0, mediatype="bilder"):
     """Søk etter term og få ut json"""
     number = min(number, 50)
-    if term == '':
+    if term == "":
         r = requests.get(
             "https://api.nb.no:443/catalog/v1/items",
-            params={
-                'filter': f'mediatype:{mediatype}',
-                'page': page,
-                'size': number
-            }
+            params={"filter": f"mediatype:{mediatype}", "page": page, "size": number},
         )
     else:
         r = requests.get(
             "https://api.nb.no:443/catalog/v1/items",
             params={
-                'q': term,
-                'filter': f'mediatype:{mediatype}',
-                'page': page,
-                'size': number
-            }
+                "q": term,
+                "filter": f"mediatype:{mediatype}",
+                "page": page,
+                "size": number,
+            },
         )
     return r.json()
 
 
-def find_urls(term, number=50, page=0, mediatype='bilder'):
+def find_urls(term, number=50, page=0, mediatype="bilder"):
     """generates urls from super_search for pictures"""
     x = super_search(term, number, page, mediatype=mediatype)
     try:
         urls = [
-            f['_links']['thumbnail_custom']['href']
-            for f in x['_embedded']['items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-            and 'thumbnail_custom' in f['_links']
+            f["_links"]["thumbnail_custom"]["href"]
+            for f in x["_embedded"]["items"]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
-    except BaseException:  # PEP8: E722 do not use bare 'except', too broad exception clause
+    except (
+        BaseException
+    ):  # PEP8: E722 do not use bare 'except', too broad exception clause
         urls = []
     return urls
 
 
 def find_urls2(term, number=50, page=0):
     """generates urls from super_search for pictures"""
     x = super_search(term, number, page)
     try:
         urls = [
-            f['_links']['thumbnail_custom']['href']
-            for f in
-            x['_embedded']['mediaTypeResults'][0]['result']['_embedded'][
-                'items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-            and 'thumbnail_custom' in f['_links']
+            f["_links"]["thumbnail_custom"]["href"]
+            for f in x["_embedded"]["mediaTypeResults"][0]["result"]["_embedded"][
+                "items"
+            ]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
-    except BaseException:  # PEP8: E722 do not use bare 'except', too broad exception clause
-        urls = [' ... hmm ...']
+    except (
+        BaseException
+    ):  # PEP8: E722 do not use bare 'except', too broad exception clause
+        urls = [" ... hmm ..."]
     return urls
 
 
 def get_picture_from_urn(urn, width=0, height=300):
     meta = iiif_manifest(urn)
     url_prefix = "https://www.nb.no/services/image/resolver"
-    if 'error' not in meta:
+    if "error" not in meta:
         if width == 0 and height == 0:
             url = f"{url_prefix}/{urn}/full/full/0/native.jpg"
         else:
             url = f"{url_prefix}/{urn}/full/{width},{height}/0/native.jpg"
         # print(url)
     return Image.open(load_picture(url))
 
 
 def get_picture_from_url(url, width=0, height=300):
-    return Image.open(
-        load_picture(
-            url.format(width=width, height=height)
-        )
-    )
+    return Image.open(load_picture(url.format(width=width, height=height)))
 
 
 def get_metadata_from_url(url):
     urn = re.findall("(URN.*?)(?:/)", url)[0]
     triple = iiif_manifest(urn)
     # print(urn, triple)
     r = {}  # Local variable 'r' value is not used
-    if 'error' not in triple:
-        r = {x['label']: x['value']
-             for x in triple['metadata'] if 'label' in x}
+    if "error" not in triple:
+        r = {x["label"]: x["value"] for x in triple["metadata"] if "label" in x}
     else:
-        r = triple['error']
+        r = triple["error"]
     return r
 
 
 def find_urns(term):
     """From result of super_search, to be fed into iiif_manifest."""
 
     ss = super_search(term)
     urns = [
-        f['metadata']['identifiers']['urn']
-        for f in
-        ss['_embedded']['mediaTypeResults'][0]['result']['_embedded']['items']
-        if 'urn' in f['metadata']['identifiers']
+        f["metadata"]["identifiers"]["urn"]
+        for f in ss["_embedded"]["mediaTypeResults"][0]["result"]["_embedded"]["items"]
+        if "urn" in f["metadata"]["identifiers"]
     ]
     return urns
 
 
 def total_search(size=50, page=0):
     """Finn de første antallet = 'size' fra side 'page' og få ut json"""
     size = min(size, 50)
     r = requests.get(
         "https://api.nb.no:443/catalog/v1/items",
-        params={
-            'filter': 'mediatype:bilder',
-            'page': page,
-            'size': size
-        }
+        params={"filter": "mediatype:bilder", "page": page, "size": size},
     )
     return r.json()
 
 
 def total_urls(number=50, page=0):
     """find urls sequentially"""
     x = total_search(number, page)
     try:
         urls = [
-            f['_links']['thumbnail_custom']['href']
-            for f in x['_embedded']['items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-            and 'thumbnail_custom' in f['_links']
+            f["_links"]["thumbnail_custom"]["href"]
+            for f in x["_embedded"]["items"]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
-    except BaseException:  # PEP8: E722 do not use bare 'except', too broad exception clause
+    except (
+        BaseException
+    ):  # PEP8: E722 do not use bare 'except', too broad exception clause
         urls = []
     return urls
 
 
-def find_urns_sesam(term='', creator='', number=50,
-                    page=0, mediatype='bilder'):
+def find_urns_sesam(term="", creator="", number=50, page=0, mediatype="bilder"):
     """generates urls from super_search for pictures"""
-    x = nb_search(term=term, creator=creator, number=number, page=page,
-                  mediatype=mediatype)
+    x = nb_search(
+        term=term, creator=creator, number=number, page=page, mediatype=mediatype
+    )
     try:
         sesamid = [
-            f['id']
-            for f in x['_embedded']['items']
-            if f['accessInfo']['accessAllowedFrom'] == 'EVERYWHERE'
-            and 'thumbnail_custom' in f['_links']
+            f["id"]
+            for f in x["_embedded"]["items"]
+            if f["accessInfo"]["accessAllowedFrom"] == "EVERYWHERE"
+            and "thumbnail_custom" in f["_links"]
         ]
     except BaseException:
         sesamid = []
     return sesamid
 
 
-def save_pictures(pages_, urn, root='.'):
+def save_pictures(pages_, urn, root="."):
     """Save picture references in pages on the form::
 
         pages = {
             urn1: [page1, page2, ..., pageN],
             urn2: [page1, ..., pageM],
             ...
             urnK: [page1, ..., pageL]}
 
     Parameter urn is one of the keys in pages,
     where each page reference is a URL.
     """
 
     # In case urn is an actual URN, works also if urn is passed as sesamid
 
-    folder_name = urn.split(':')[-1]
+    folder_name = urn.split(":")[-1]
     folder_ref = os.path.join(root, folder_name)
     try:
         os.mkdir(folder_ref)
 
     except FileExistsError:
         pass
 
     for p in pages_[urn]:
         # pell ut entydig referanse til bildet fra URL-en i bildelisten som
         # filnavn
 
-        filename = p.split('/')[6].split(':')[-1] + '.jpg'
+        filename = p.split("/")[6].split(":")[-1] + ".jpg"
 
         path = os.path.join(folder_ref, filename)
         get_picture_from_url(p).save(path)
 
     return True
 
 
-def save_all_pages(pages_, root='.'):
+def save_all_pages(pages_, root="."):
     """Save picture references in pages on the form::
 
         pages = {
             urn1 : [page1, page2, ..., pageN],
             urn2: [page1, ..., pageM],
             ...
             urnK: [page1, ..., pageL]
         }
 
     Each page reference is a URL.
     """
 
     # In case urn is an actual URN, works also if urn is passed as sesamid
     for urn in pages_:
-        folder_name = urn.split(':')[-1]
+        folder_name = urn.split(":")[-1]
         folder_ref = os.path.join(root, folder_name)
         try:
             os.mkdir(folder_ref)
 
         except FileExistsError:
             pass
 
         for p in pages_[urn]:
             # pell ut entydig referanse til bildet fra URL-en i bildelisten som
             # filnavn
 
-            filename = p.split('/')[6].split(':')[-1] + '.jpg'
+            filename = p.split("/")[6].split(":")[-1] + ".jpg"
 
             path = os.path.join(folder_ref, filename)
             get_picture_from_url(p).save(path)
 
     return True
```

### Comparing `dhlab-2.9.5/dhlab/ngram/nb_ngram.py` & `dhlab-3.0.0a3/dhlab/ngram/nb_ngram.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,98 @@
 import pandas as pd
 
 from dhlab.api.nb_ngram_api import get_ngram
 
 
-def nb_ngram(terms: str,
-             corpus: str = 'bok',
-             smooth: int = 1,
-             years: tuple = (1810, 2010),
-             mode: str = 'relative',
-            lang: str = 'nob'):
+def nb_ngram(
+    terms: str,
+    corpus: str = "bok",
+    smooth: int = 1,
+    years: tuple = (1810, 2010),
+    mode: str = "relative",
+    lang: str = "nob",
+):
     """Extract N-gram frequencies from given ``terms`` and ``years``.
+    `lang` param is not supported for corpus=`avis` and will be set to None if `avis` is passed.
 
     :param terms: comma
     :param corpus:
     :param smooth:
     :param years:
     :param mode:
     :param lang:
     :return: A sorted Pandas DataFrame index
 
     :meta private:
     """
-    df = ngram_conv(get_ngram(terms, corpus=corpus, lang = lang), smooth=smooth, years=years, mode=mode)
+    # Set default lang for 'bok'-corpus
+    if corpus == "avis":
+        lang = None
+
+    df = ngram_conv(
+        get_ngram(terms, corpus=corpus, lang=lang),
+        smooth=smooth,
+        years=years,
+        mode=mode,
+    )
     df.index = df.index.astype(int)
     return df.sort_index()
 
+
 ## tar tilbake til original den her virker ikke LGJ
-def ngram_conv_old(ngrams, smooth: int = 1, years: tuple = (1810, 2013), mode: str = 'relative'):
+def ngram_conv_old(
+    ngrams, smooth: int = 1, years: tuple = (1810, 2013), mode: str = "relative"
+):
     """Construct a dataframe with ngram mean frequencies per year over a given time period.
 
     :param ngrams: TODO: FIll in appropriate type and description.
     :param smooth: Smoothing factor for the graph visualisation.
     :param years: Tuple with start and end years for the time period of interest
     :param mode: Frequency measure. Defaults to 'relative'.
     :return: pandas dataframe with mean values for each year
 
     :meta private:
     """
     ngc = {}
     # check if relative frequency or absolute frequency is in question
-    if mode.startswith('rel') or mode == 'y':
-        arg = 'y'
+    if mode.startswith("rel") or mode == "y":
+        arg = "y"
     else:
-        arg = 'f'
+        arg = "f"
     for x in ngrams:
         if x and isinstance(x, list):
-            ngc[x['key']] = {
-                z['x']: z[arg]
-                for z in x['values']
-                if years[1] >= int(z['x']) >= years[0]
+            ngc[x["key"]] = {
+                z["x"]: z[arg]
+                for z in x["values"]
+                if years[1] >= int(z["x"]) >= years[0]
             }
-    return pd.DataFrame(ngc).rolling(window=smooth, win_type='triang').mean()
+    return pd.DataFrame(ngc).rolling(window=smooth, win_type="triang").mean()
 
 
-def ngram_conv(ngrams, smooth=1, years=(1810,2013), mode='relative'):
+def ngram_conv(ngrams, smooth=1, years=(1810, 2013), mode="relative"):
     """Construct a dataframe with ngram mean frequencies per year over a given time period.
 
     :param ngrams: TODO: FIll in appropriate type and description.
     :param smooth: Smoothing factor for the graph visualisation.
     :param years: Tuple with start and end years for the time period of interest
     :param mode: Frequency measure. Defaults to 'relative'.
     :return: pandas dataframe with mean values for each year
 
     :meta private:
     """
     ngc = {}
     # check if relative frequency or absolute frequency is in question
-    if mode.startswith('rel') or mode=='y':
-        arg = 'y'
+    if mode.startswith("rel") or mode == "y":
+        arg = "y"
     else:
-        arg = 'f'
+        arg = "f"
     for x in ngrams:
         # check if x is a non empty ngram - empty ngrams are coded as empty lists
         # if x is non emtpy it accepts keys - look at alternative isinstance(x, dict)?
         if x != []:
-            ngc[x['key']] = {z['x']:z[arg] for z in x['values'] if int(z['x']) <= int(years[1]) and int(z['x']) >= int(years[0])}
-    
-    return pd.DataFrame(ngc).rolling(window=smooth, win_type='triang').mean()
+            ngc[x["key"]] = {
+                z["x"]: z[arg]
+                for z in x["values"]
+                if int(z["x"]) <= int(years[1]) and int(z["x"]) >= int(years[0])
+            }
+
+    return pd.DataFrame(ngc).rolling(window=smooth, win_type="triang").mean()
```

### Comparing `dhlab-2.9.5/dhlab/text/chunking.py` & `dhlab-3.0.0a3/dhlab/text/chunking.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.5/dhlab/utils/display.py` & `dhlab-3.0.0a3/dhlab/utils/display.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from urllib.parse import urlparse
 
 import requests
-from IPython.display import HTML
+from IPython.display import HTML, display
 
 
-def code_toggle(button_text = "Klikk for å vise/skjule kodeceller"):
-    from IPython.display import HTML, display
-
+def code_toggle(button_text="Klikk for å vise/skjule kodeceller"):
     display(
         HTML(
-        '''<div>
+            """<div>
                 <style>
                  .mybutton {
                     background-color: lightgrey;
                     border: none;
                     color: white;
                     padding: 10px 16px;
                     text-align: center;
@@ -21,50 +19,57 @@
                     display: inline-block;
                     font-size: 16px;
                     margin: 4px 2px;
                     cursor: pointer;
                 }
             </style>
             <script>
-                code_show=true; 
+                code_show=true;
                 function code_toggle() {
                  if (code_show){
                  $('div.input').hide();
                  } else {
                  $('div.input').show();
                  }
                  code_show = !code_show
-                } 
+                }
                 $( document ).ready(code_toggle);
             </script>
             <form  action="javascript:code_toggle()">
-                <input class='mybutton' type="submit" value=''' + '"'  + button_text + '"' + '''>
+                <input class='mybutton' type="submit" value="""
+            + '"'
+            + button_text
+            + '"'
+            + """>
             </form>
-        </div>'''
-        ))
+        </div>"""
+        )
+    )
 
 
-def css(url = "https://raw.githubusercontent.com/Yoonsen/Modules/master/css_style_sheets/nb_notebook.css"):
-    """Associate a css stylesheet with the notebook, 
+def css(
+    url="https://raw.githubusercontent.com/Yoonsen/Modules/master/css_style_sheets/nb_notebook.css",
+):
+    """Associate a css stylesheet with the notebook,
     just specify a file or web reference, default is a custom css"""
-    
+
     uri = urlparse(url)
     css_file = ""
-    
-    if uri.scheme.startswith('http'):
+
+    if uri.scheme.startswith("http"):
         query = requests.get(url)
         if query.status_code == 200:
-            css_file  = query.text
-    
-    elif uri.scheme == "file": 
+            css_file = query.text
+
+    elif uri.scheme == "file":
         # assume on form "file:/// on windows there is drive letter on unix not"
         file_path = url[7:]
-        if file_path[2] == ':': # then windows drive reference
+        if file_path[2] == ":":  # then windows drive reference
             file_path = file_path[1:]
-        with open(file_path, encoding='utf-8') as file:
+        with open(file_path, encoding="utf-8") as file:
             css_file = file.read()
-    else: 
+    else:
         # assume string is a file locator
-        with open(url, encoding='utf-8') as file:
+        with open(url, encoding="utf-8") as file:
             css_file = file.read()
-    
-    return HTML("<style>{css_code}</style>".format(css_code = css_file))
+
+    return HTML(f"<style>{css_file}</style>")
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 from urllib.parse import urlparse import requests from IPython.display import
-HTML def code_toggle(button_text = "Klikk for Ã¥ vise/skjule kodeceller"): from
-IPython.display import HTML, display display( HTML( '''
- + '"' + button_text + '"' + '''>
-''' )) def css(url = "https://raw.githubusercontent.com/Yoonsen/Modules/master/
-css_style_sheets/nb_notebook.css"): """Associate a css stylesheet with the
+HTML, display def code_toggle(button_text="Klikk for Ã¥ vise/skjule
+kodeceller"): display( HTML( """
+ + '"' + button_text + '"' + """>
+""" ) ) def css( url="https://raw.githubusercontent.com/Yoonsen/Modules/master/
+css_style_sheets/nb_notebook.css", ): """Associate a css stylesheet with the
 notebook, just specify a file or web reference, default is a custom css""" uri
-= urlparse(url) css_file = "" if uri.scheme.startswith('http'): query =
+= urlparse(url) css_file = "" if uri.scheme.startswith("http"): query =
 requests.get(url) if query.status_code == 200: css_file = query.text elif
 uri.scheme == "file": # assume on form "file:/// on windows there is drive
-letter on unix not" file_path = url[7:] if file_path[2] == ':': # then windows
-drive reference file_path = file_path[1:] with open(file_path, encoding='utf-
-8') as file: css_file = file.read() else: # assume string is a file locator
-with open(url, encoding='utf-8') as file: css_file = file.read() return HTML("
-".format(css_code = css_file))
+letter on unix not" file_path = url[7:] if file_path[2] == ":": # then windows
+drive reference file_path = file_path[1:] with open(file_path, encoding="utf-
+8") as file: css_file = file.read() else: # assume string is a file locator
+with open(url, encoding="utf-8") as file: css_file = file.read() return HTML(f"
+")
```

### Comparing `dhlab-2.9.5/dhlab/utils/files.py` & `dhlab-3.0.0a3/dhlab/utils/files.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,92 +8,98 @@
 
 def printmd(S):
     """Use ``IPython.display`` to render markdown text."""
     display(Markdown(S))
     return
 
 
-def download_from_github(filename=None, user=None, repository=None, branch='master',
-                         overwrite=False,
-                         silent=False):
+def download_from_github(
+    filename=None,
+    user=None,
+    repository=None,
+    branch="master",
+    overwrite=False,
+    silent=False,
+):
     """Fetch a file from Github and write it to working directory.
 
     :param filename:     Filename, including file extension (e.g. `.py` or `.txt`)
     :param user:         Github username of the repo owner.
     :param repository:   Github repository name.
     :param branch:       Name of the repo branch. Defaults to 'master'.
     :param overwrite:    Whether to overwrite existing files in working directory. Defaults to not
                          overwrite.
     :param silent:       Whether to output logging messages to stdout. Default is not silent.
     """
 
     nba = requests.get(
         f"https://raw.githubusercontent.com/{user}/{repository}/{branch}/{filename}",
-        headers={'Cache-Control': 'no-cache'}
+        headers={"Cache-Control": "no-cache"},
     )
     if nba.status_code == 200:
         file_exists = os.path.exists(filename)
         if file_exists and not overwrite:
             if not silent:
                 printmd(
                     f"File {os.path.abspath(filename)} exists - call `download_from_github('{filename}', overwrite "
-                    f"= True)` in order to download module `{filename}` anyway")
+                    f"= True)` in order to download module `{filename}` anyway"
+                )
         else:
-            with open(filename, 'w+', encoding='utf-8') as pyfile:
+            with open(filename, "w+", encoding="utf-8") as pyfile:
                 pyfile.write(nba.text)
                 pyfile.flush()
                 pyfile.close()
             if not silent:
                 printmd(f"Downloaded file `{os.path.abspath(filename)}`")
     else:
         printmd(f"Failed to download {filename} with http code {nba.status_code}")
 
 
 def get_file_from_github(url, overwrite=False, silent=False):
     """Fetch a file on github.
 
     it is enough with reference
     it will look in raw user content for the file.
-    
+
     :param overwrite: defaults to no overwrite
     :param silent: default is not silent"""
 
     if url.startswith("https://github.com/") or url.startswith("github.com"):
-        trail = url.split("github.com")[-1].replace('blob/', '')
+        trail = url.split("github.com")[-1].replace("blob/", "")
         fileref = f"""https://raw.githubusercontent.com{trail}"""
     elif url.startswith("raw.githubusercontent"):
         fileref = f"""https://{url}"""
     elif url.startswith("https://raw.githubusercontent"):
         fileref = url
     else:
         return "is this is a file on github?"
 
-    nba = requests.get(
-        f"{fileref}",
-        headers={'Cache-Control': 'no-cache'}
-    )
+    nba = requests.get(f"{fileref}", headers={"Cache-Control": "no-cache"})
     if nba.status_code == 200:
         filename = os.path.basename(fileref)
         file_exists = os.path.exists(filename)
         if file_exists and not overwrite:
             if not silent:
                 printmd(
                     f"File {os.path.abspath(filename)} exists -"
                     f" call `download('{filename}', overwrite = True)` in order to "
-                    f"download `{filename}` anyway")
+                    f"download `{filename}` anyway"
+                )
         else:
             nba = nba.text
-            with open(filename, 'w', encoding='UTF-8') as pyfile:
+            with open(filename, "w", encoding="UTF-8") as pyfile:
                 pyfile.write(nba)
                 pyfile.flush()
                 pyfile.close()
             if not silent:
                 printmd(f"Downloaded file `{os.path.abspath(filename)}`")
     else:
-        printmd(f"Failed to download {fileref} with http response code {nba.status_code}")
+        printmd(
+            f"Failed to download {fileref} with http response code {nba.status_code}"
+        )
 
     return
 
 
 @contextlib.contextmanager
 def working_directory(path):
     """Changes working directory and returns to previous on exit.
```

### Comparing `dhlab-2.9.5/docs/LICENSE` & `dhlab-3.0.0a3/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MIT License
-Copyright (c) 2022 The National Library of Norway
+
+Copyright (c) 2023 Nasjonalbiblioteket
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

