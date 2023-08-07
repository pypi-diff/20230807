# Comparing `tmp/pytextrank-3.2.4.tar.gz` & `tmp/pytextrank-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytextrank-3.2.4.tar", last modified: Wed Jul 27 22:03:31 2022, max compression
+gzip compressed data, was "dist/pytextrank-3.2.5.tar", last modified: Mon Aug  7 19:50:33 2023, max compression
```

## Comparing `pytextrank-3.2.4.tar` & `pytextrank-3.2.5.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/
--rw-r--r--   0 paco       (501) staff       (20)     1224 2021-10-10 01:11:11.000000 pytextrank-3.2.4/.pre-commit-config.yaml
--rw-r--r--   0 paco       (501) staff       (20)     4901 2022-07-27 22:02:18.000000 pytextrank-3.2.4/CHANGELOG.md
--rw-r--r--   0 paco       (501) staff       (20)      293 2021-03-20 18:22:10.000000 pytextrank-3.2.4/CITATION
--rw-r--r--   0 paco       (501) staff       (20)     4802 2021-03-20 18:22:10.000000 pytextrank-3.2.4/CONTRIBUTING.md
--rw-r--r--   0 paco       (501) staff       (20)     1074 2022-02-04 20:10:22.000000 pytextrank-3.2.4/LICENSE
--rw-r--r--   0 paco       (501) staff       (20)      687 2022-07-27 21:35:23.000000 pytextrank-3.2.4/MANIFEST.in
--rw-r--r--   0 paco       (501) staff       (20)    11217 2022-07-27 22:03:31.000000 pytextrank-3.2.4/PKG-INFO
--rw-r--r--   0 paco       (501) staff       (20)     7615 2022-07-27 21:35:23.000000 pytextrank-3.2.4/README.md
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/bin/
--rwxr-xr-x   0 paco       (501) staff       (20)      337 2021-03-09 19:29:14.000000 pytextrank-3.2.4/bin/nb_md.sh
--rwxr-xr-x   0 paco       (501) staff       (20)     1335 2021-07-17 19:45:35.000000 pytextrank-3.2.4/bin/preview.py
--rwxr-xr-x   0 paco       (501) staff       (20)      187 2021-07-17 19:45:35.000000 pytextrank-3.2.4/bin/push_pypi.sh
--rwxr-xr-x   0 paco       (501) staff       (20)     3318 2021-07-17 19:45:35.000000 pytextrank-3.2.4/bin/vis_doc.py
--rw-r--r--   0 paco       (501) staff       (20)     3380 2021-02-14 22:57:50.000000 pytextrank-3.2.4/code_of_conduct.md
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/dat/
--rw-r--r--   0 paco       (501) staff       (20)     2464 2019-11-05 20:18:24.000000 pytextrank-3.2.4/dat/ars.txt
--rw-r--r--   0 paco       (501) staff       (20)      844 2021-03-20 18:22:10.000000 pytextrank-3.2.4/dat/cfc.txt
--rw-r--r--   0 paco       (501) staff       (20)     1063 2019-11-05 20:18:24.000000 pytextrank-3.2.4/dat/gen.txt
--rw-r--r--   0 paco       (501) staff       (20)     2999 2019-11-05 20:18:24.000000 pytextrank-3.2.4/dat/lee.txt
--rw-r--r--   0 paco       (501) staff       (20)      565 2019-11-05 20:18:24.000000 pytextrank-3.2.4/dat/mih.txt
--rw-r--r--   0 paco       (501) staff       (20)     1757 2019-11-05 20:18:24.000000 pytextrank-3.2.4/dat/suz.txt
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/deprecated/
--rw-r--r--   0 paco       (501) staff       (20)      133 2021-10-10 01:11:11.000000 pytextrank-3.2.4/deprecated/WARNING.md
--rw-r--r--   0 paco       (501) staff       (20)    80398 2021-10-10 01:11:11.000000 pytextrank-3.2.4/deprecated/example.ipynb
--rwxr-xr-x   0 paco       (501) staff       (20)    18567 2021-10-10 01:11:11.000000 pytextrank-3.2.4/deprecated/oldsrc.py
--rwxr-xr-x   0 paco       (501) staff       (20)     1650 2021-10-10 01:11:11.000000 pytextrank-3.2.4/deprecated/test.py
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/docs/
--rw-r--r--   0 paco       (501) staff       (20)     5276 2022-02-04 20:10:22.000000 pytextrank-3.2.4/docs/ack.md
--rw-r--r--   0 paco       (501) staff       (20)      310 2022-03-06 22:26:05.000000 pytextrank-3.2.4/docs/apidocs.yml
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/docs/assets/
--rw-r--r--   0 paco       (501) staff       (20)     1656 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/assets/favicon.png
--rw-r--r--   0 paco       (501) staff       (20)    78263 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/assets/logo.png
--rw-r--r--   0 paco       (501) staff       (20)     9137 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/assets/noam.jpg
--rw-r--r--   0 paco       (501) staff       (20)     1471 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/biblio.jinja
--rw-r--r--   0 paco       (501) staff       (20)     8601 2022-03-06 22:26:05.000000 pytextrank-3.2.4/docs/biblio.md
--rw-r--r--   0 paco       (501) staff       (20)     3531 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/build.md
--rw-r--r--   0 paco       (501) staff       (20)     2290 2020-03-02 20:00:36.000000 pytextrank-3.2.4/docs/codecov_io.svg
--rw-r--r--   0 paco       (501) staff       (20)      439 2021-10-10 01:11:11.000000 pytextrank-3.2.4/docs/depend.md
--rw-r--r--   0 paco       (501) staff       (20)    56801 2022-03-06 22:41:08.000000 pytextrank-3.2.4/docs/explain_algo.md
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/docs/explain_algo_files/
--rw-r--r--   0 paco       (501) staff       (20)    73044 2021-03-05 23:56:51.000000 pytextrank-3.2.4/docs/explain_algo_files/explain_algo_20_1.png
--rw-r--r--   0 paco       (501) staff       (20)    70426 2022-03-06 22:41:08.000000 pytextrank-3.2.4/docs/explain_algo_files/explain_algo_23_0.png
--rw-r--r--   0 paco       (501) staff       (20)    10853 2022-03-06 22:41:10.000000 pytextrank-3.2.4/docs/explain_summ.md
--rw-r--r--   0 paco       (501) staff       (20)     1939 2021-03-25 19:11:35.000000 pytextrank-3.2.4/docs/faq.md
--rw-r--r--   0 paco       (501) staff       (20)      748 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/glossary.jinja
--rw-r--r--   0 paco       (501) staff       (20)    12444 2022-03-06 22:26:05.000000 pytextrank-3.2.4/docs/glossary.md
--rw-r--r--   0 paco       (501) staff       (20)     4567 2022-03-23 15:41:28.000000 pytextrank-3.2.4/docs/index.md
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/docs/javascripts/
--rw-r--r--   0 paco       (501) staff       (20)      231 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/javascripts/config.js
--rw-r--r--   0 paco       (501) staff       (20)    22126 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/mkrefs.ttl
--rw-r--r--   0 paco       (501) staff       (20)     1131 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/mkrefs.yml
--rw-r--r--   0 paco       (501) staff       (20)     9137 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/noam.jpg
--rw-r--r--   0 paco       (501) staff       (20)     4102 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/overview.md
--rw-r--r--   0 paco       (501) staff       (20)     1380 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/ref.jinja
--rw-r--r--   0 paco       (501) staff       (20)    23730 2022-03-06 22:26:05.000000 pytextrank-3.2.4/docs/ref.md
--rw-r--r--   0 paco       (501) staff       (20)    34339 2022-03-06 22:41:12.000000 pytextrank-3.2.4/docs/sample.md
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/docs/sample_files/
--rw-r--r--   0 paco       (501) staff       (20)   122228 2021-05-04 23:46:59.000000 pytextrank-3.2.4/docs/sample_files/sample_27_0.svg
--rw-r--r--   0 paco       (501) staff       (20)   122409 2022-03-06 22:41:12.000000 pytextrank-3.2.4/docs/sample_files/sample_36_0.svg
--rw-r--r--   0 paco       (501) staff       (20)     2100 2021-03-25 19:11:35.000000 pytextrank-3.2.4/docs/setup.md
--rw-r--r--   0 paco       (501) staff       (20)     1610 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/start.md
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/docs/stylesheets/
--rw-r--r--   0 paco       (501) staff       (20)      260 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/stylesheets/extra.css
--rw-r--r--   0 paco       (501) staff       (20)     3459 2021-07-17 19:45:35.000000 pytextrank-3.2.4/docs/talks.md
--rw-r--r--   0 paco       (501) staff       (20)      277 2021-03-09 19:29:14.000000 pytextrank-3.2.4/docs/todo.md
--rw-r--r--   0 paco       (501) staff       (20)     1082 2021-03-20 18:22:10.000000 pytextrank-3.2.4/docs/tutorial.md
--rw-r--r--   0 paco       (501) staff       (20)      220 2021-10-10 01:11:11.000000 pytextrank-3.2.4/environment.yml
--rwxr-xr-x   0 paco       (501) staff       (20)     1277 2021-07-07 15:46:34.000000 pytextrank-3.2.4/error.py
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/examples/
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/examples/.ipynb_checkpoints/
--rw-r--r--   0 paco       (501) staff       (20)       72 2021-03-14 23:58:00.000000 pytextrank-3.2.4/examples/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0 paco       (501) staff       (20)   166415 2021-03-23 18:59:09.000000 pytextrank-3.2.4/examples/.ipynb_checkpoints/explain_algo-checkpoint.ipynb
--rw-r--r--   0 paco       (501) staff       (20)    17250 2021-03-20 04:26:31.000000 pytextrank-3.2.4/examples/.ipynb_checkpoints/explain_summ-checkpoint.ipynb
--rw-r--r--   0 paco       (501) staff       (20)   196214 2022-03-06 22:39:51.000000 pytextrank-3.2.4/examples/.ipynb_checkpoints/sample-checkpoint.ipynb
--rw-r--r--   0 paco       (501) staff       (20)   166415 2021-03-25 19:11:35.000000 pytextrank-3.2.4/examples/explain_algo.ipynb
--rw-r--r--   0 paco       (501) staff       (20)    17250 2021-03-20 18:22:10.000000 pytextrank-3.2.4/examples/explain_summ.ipynb
--rw-r--r--   0 paco       (501) staff       (20)   196923 2022-07-27 21:35:23.000000 pytextrank-3.2.4/examples/sample.ipynb
--rw-r--r--   0 paco       (501) staff       (20)      599 2021-07-17 19:45:35.000000 pytextrank-3.2.4/lgtm.yml
--rw-r--r--   0 paco       (501) staff       (20)     1052 2021-03-26 15:32:15.000000 pytextrank-3.2.4/meta.yaml
--rw-r--r--   0 paco       (501) staff       (20)     1756 2022-03-06 22:26:05.000000 pytextrank-3.2.4/mkdocs.yml
--rwxr-xr-x   0 paco       (501) staff       (20)     1205 2022-03-06 22:26:05.000000 pytextrank-3.2.4/pkg_doc.py
--rwxr-xr-x   0 paco       (501) staff       (20)    13844 2021-07-17 19:45:35.000000 pytextrank-3.2.4/pyfixdoc.py
--rw-r--r--   0 paco       (501) staff       (20)    16053 2021-07-17 19:45:35.000000 pytextrank-3.2.4/pylintrc
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/pytextrank/
--rw-r--r--   0 paco       (501) staff       (20)     4633 2022-03-06 22:26:05.000000 pytextrank-3.2.4/pytextrank/__init__.py
--rw-r--r--   0 paco       (501) staff       (20)    27788 2022-03-07 19:13:52.000000 pytextrank-3.2.4/pytextrank/base.py
--rw-r--r--   0 paco       (501) staff       (20)     4589 2022-07-27 21:35:23.000000 pytextrank-3.2.4/pytextrank/biasedrank.py
--rw-r--r--   0 paco       (501) staff       (20)     4090 2021-07-17 19:45:35.000000 pytextrank-3.2.4/pytextrank/positionrank.py
--rw-r--r--   0 paco       (501) staff       (20)    13346 2022-07-27 21:35:23.000000 pytextrank-3.2.4/pytextrank/topicrank.py
--rw-r--r--   0 paco       (501) staff       (20)     4307 2021-07-17 19:45:35.000000 pytextrank-3.2.4/pytextrank/util.py
--rw-r--r--   0 paco       (501) staff       (20)     1334 2022-03-07 19:13:52.000000 pytextrank-3.2.4/pytextrank/version.py
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/pytextrank.egg-info/
--rw-r--r--   0 paco       (501) staff       (20)    11217 2022-07-27 22:03:30.000000 pytextrank-3.2.4/pytextrank.egg-info/PKG-INFO
--rw-r--r--   0 paco       (501) staff       (20)     2045 2022-07-27 22:03:30.000000 pytextrank-3.2.4/pytextrank.egg-info/SOURCES.txt
--rw-r--r--   0 paco       (501) staff       (20)        1 2022-07-27 22:03:30.000000 pytextrank-3.2.4/pytextrank.egg-info/dependency_links.txt
--rw-r--r--   0 paco       (501) staff       (20)        1 2019-11-05 20:30:26.000000 pytextrank-3.2.4/pytextrank.egg-info/not-zip-safe
--rw-r--r--   0 paco       (501) staff       (20)      511 2022-07-27 22:03:30.000000 pytextrank-3.2.4/pytextrank.egg-info/requires.txt
--rw-r--r--   0 paco       (501) staff       (20)       11 2022-07-27 22:03:30.000000 pytextrank-3.2.4/pytextrank.egg-info/top_level.txt
--rw-r--r--   0 paco       (501) staff       (20)      309 2022-07-27 21:35:23.000000 pytextrank-3.2.4/requirements-dev.txt
--rw-r--r--   0 paco       (501) staff       (20)       16 2021-07-17 19:45:35.000000 pytextrank-3.2.4/requirements-viz.txt
--rw-r--r--   0 paco       (501) staff       (20)      102 2021-10-10 01:11:11.000000 pytextrank-3.2.4/requirements.txt
--rw-r--r--   0 paco       (501) staff       (20)     1837 2022-03-07 19:16:57.000000 pytextrank-3.2.4/ru.py
--rwxr-xr-x   0 paco       (501) staff       (20)     3738 2022-03-06 22:26:05.000000 pytextrank-3.2.4/sample.py
--rw-r--r--   0 paco       (501) staff       (20)       38 2022-07-27 22:03:31.000000 pytextrank-3.2.4/setup.cfg
--rw-r--r--   0 paco       (501) staff       (20)     3719 2022-03-06 22:44:13.000000 pytextrank-3.2.4/setup.py
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/tests/
--rw-r--r--   0 paco       (501) staff       (20)     2300 2022-03-06 22:26:05.000000 pytextrank-3.2.4/tests/conftest.py
--rw-r--r--   0 paco       (501) staff       (20)     5451 2022-07-27 22:02:18.000000 pytextrank-3.2.4/tests/test_base.py
--rw-r--r--   0 paco       (501) staff       (20)     2372 2022-07-27 21:35:23.000000 pytextrank-3.2.4/tests/test_biasedrank.py
--rw-r--r--   0 paco       (501) staff       (20)     1521 2022-02-04 19:59:51.000000 pytextrank-3.2.4/tests/test_positionrank.py
--rw-r--r--   0 paco       (501) staff       (20)     6183 2022-07-27 22:02:18.000000 pytextrank-3.2.4/tests/test_topicrank.py
--rwxr-xr-x   0 paco       (501) staff       (20)      783 2021-07-17 19:45:35.000000 pytextrank-3.2.4/tests/trace.py
--rwxr-xr-x   0 paco       (501) staff       (20)     1410 2021-10-09 22:42:21.000000 pytextrank-3.2.4/tmp_api.py
--rw-r--r--   0 paco       (501) staff       (20)     1477 2020-02-23 18:45:41.000000 pytextrank-3.2.4/udpipe.py
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/wip/
-drwxr-xr-x   0 paco       (501) staff       (20)        0 2022-07-27 22:03:31.000000 pytextrank-3.2.4/wip/.ipynb_checkpoints/
--rw-r--r--   0 paco       (501) staff       (20)    15643 2021-03-17 03:20:40.000000 pytextrank-3.2.4/wip/.ipynb_checkpoints/error-checkpoint.ipynb
--rw-r--r--   0 paco       (501) staff       (20)    15643 2021-03-20 18:22:10.000000 pytextrank-3.2.4/wip/error.ipynb
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/
+-rw-r--r--   0 paco       (501) staff       (20)     1224 2021-10-10 01:11:11.000000 pytextrank-3.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 paco       (501) staff       (20)     4901 2022-07-27 22:02:18.000000 pytextrank-3.2.5/CHANGELOG.md
+-rw-r--r--   0 paco       (501) staff       (20)      293 2021-03-20 18:22:10.000000 pytextrank-3.2.5/CITATION
+-rw-r--r--   0 paco       (501) staff       (20)     4802 2021-03-20 18:22:10.000000 pytextrank-3.2.5/CONTRIBUTING.md
+-rw-r--r--   0 paco       (501) staff       (20)     1074 2022-02-04 20:10:22.000000 pytextrank-3.2.5/LICENSE
+-rw-r--r--   0 paco       (501) staff       (20)      687 2022-07-27 21:35:23.000000 pytextrank-3.2.5/MANIFEST.in
+-rw-r--r--   0 paco       (501) staff       (20)     9672 2023-08-07 19:50:33.000000 pytextrank-3.2.5/PKG-INFO
+-rw-r--r--   0 paco       (501) staff       (20)     7647 2023-08-07 19:27:14.000000 pytextrank-3.2.5/README.md
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/bin/
+-rwxr-xr-x   0 paco       (501) staff       (20)      337 2021-03-09 19:29:14.000000 pytextrank-3.2.5/bin/nb_md.sh
+-rwxr-xr-x   0 paco       (501) staff       (20)     1335 2021-07-17 19:45:35.000000 pytextrank-3.2.5/bin/preview.py
+-rwxr-xr-x   0 paco       (501) staff       (20)      187 2021-07-17 19:45:35.000000 pytextrank-3.2.5/bin/push_pypi.sh
+-rwxr-xr-x   0 paco       (501) staff       (20)     3318 2021-07-17 19:45:35.000000 pytextrank-3.2.5/bin/vis_doc.py
+-rw-r--r--   0 paco       (501) staff       (20)     3380 2021-02-14 22:57:50.000000 pytextrank-3.2.5/code_of_conduct.md
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/dat/
+-rw-r--r--   0 paco       (501) staff       (20)     2464 2019-11-05 20:18:24.000000 pytextrank-3.2.5/dat/ars.txt
+-rw-r--r--   0 paco       (501) staff       (20)      844 2021-03-20 18:22:10.000000 pytextrank-3.2.5/dat/cfc.txt
+-rw-r--r--   0 paco       (501) staff       (20)     1063 2019-11-05 20:18:24.000000 pytextrank-3.2.5/dat/gen.txt
+-rw-r--r--   0 paco       (501) staff       (20)     2999 2019-11-05 20:18:24.000000 pytextrank-3.2.5/dat/lee.txt
+-rw-r--r--   0 paco       (501) staff       (20)      565 2019-11-05 20:18:24.000000 pytextrank-3.2.5/dat/mih.txt
+-rw-r--r--   0 paco       (501) staff       (20)     1757 2019-11-05 20:18:24.000000 pytextrank-3.2.5/dat/suz.txt
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/deprecated/
+-rw-r--r--   0 paco       (501) staff       (20)      133 2021-10-10 01:11:11.000000 pytextrank-3.2.5/deprecated/WARNING.md
+-rw-r--r--   0 paco       (501) staff       (20)    80398 2021-10-10 01:11:11.000000 pytextrank-3.2.5/deprecated/example.ipynb
+-rwxr-xr-x   0 paco       (501) staff       (20)    18567 2021-10-10 01:11:11.000000 pytextrank-3.2.5/deprecated/oldsrc.py
+-rwxr-xr-x   0 paco       (501) staff       (20)     1650 2021-10-10 01:11:11.000000 pytextrank-3.2.5/deprecated/test.py
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/docs/
+-rw-r--r--   0 paco       (501) staff       (20)     5308 2023-08-07 19:21:59.000000 pytextrank-3.2.5/docs/ack.md
+-rw-r--r--   0 paco       (501) staff       (20)      310 2022-03-06 22:26:05.000000 pytextrank-3.2.5/docs/apidocs.yml
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/docs/assets/
+-rw-r--r--   0 paco       (501) staff       (20)     1656 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/assets/favicon.png
+-rw-r--r--   0 paco       (501) staff       (20)    78263 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/assets/logo.png
+-rw-r--r--   0 paco       (501) staff       (20)     9137 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/assets/noam.jpg
+-rw-r--r--   0 paco       (501) staff       (20)     1471 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/biblio.jinja
+-rw-r--r--   0 paco       (501) staff       (20)     8601 2022-03-06 22:26:05.000000 pytextrank-3.2.5/docs/biblio.md
+-rw-r--r--   0 paco       (501) staff       (20)     3531 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/build.md
+-rw-r--r--   0 paco       (501) staff       (20)     2290 2020-03-02 20:00:36.000000 pytextrank-3.2.5/docs/codecov_io.svg
+-rw-r--r--   0 paco       (501) staff       (20)      439 2021-10-10 01:11:11.000000 pytextrank-3.2.5/docs/depend.md
+-rw-r--r--   0 paco       (501) staff       (20)    56801 2022-03-06 22:41:08.000000 pytextrank-3.2.5/docs/explain_algo.md
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/docs/explain_algo_files/
+-rw-r--r--   0 paco       (501) staff       (20)    73044 2021-03-05 23:56:51.000000 pytextrank-3.2.5/docs/explain_algo_files/explain_algo_20_1.png
+-rw-r--r--   0 paco       (501) staff       (20)    70426 2022-03-06 22:41:08.000000 pytextrank-3.2.5/docs/explain_algo_files/explain_algo_23_0.png
+-rw-r--r--   0 paco       (501) staff       (20)    10853 2022-03-06 22:41:10.000000 pytextrank-3.2.5/docs/explain_summ.md
+-rw-r--r--   0 paco       (501) staff       (20)     1939 2021-03-25 19:11:35.000000 pytextrank-3.2.5/docs/faq.md
+-rw-r--r--   0 paco       (501) staff       (20)      748 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/glossary.jinja
+-rw-r--r--   0 paco       (501) staff       (20)    12444 2022-03-06 22:26:05.000000 pytextrank-3.2.5/docs/glossary.md
+-rw-r--r--   0 paco       (501) staff       (20)     4567 2022-03-23 15:41:28.000000 pytextrank-3.2.5/docs/index.md
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/docs/javascripts/
+-rw-r--r--   0 paco       (501) staff       (20)      231 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/javascripts/config.js
+-rw-r--r--   0 paco       (501) staff       (20)    22126 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/mkrefs.ttl
+-rw-r--r--   0 paco       (501) staff       (20)     1131 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/mkrefs.yml
+-rw-r--r--   0 paco       (501) staff       (20)     9137 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/noam.jpg
+-rw-r--r--   0 paco       (501) staff       (20)     4102 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/overview.md
+-rw-r--r--   0 paco       (501) staff       (20)     1380 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/ref.jinja
+-rw-r--r--   0 paco       (501) staff       (20)    23730 2022-03-06 22:26:05.000000 pytextrank-3.2.5/docs/ref.md
+-rw-r--r--   0 paco       (501) staff       (20)    34339 2022-03-06 22:41:12.000000 pytextrank-3.2.5/docs/sample.md
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/docs/sample_files/
+-rw-r--r--   0 paco       (501) staff       (20)   122228 2021-05-04 23:46:59.000000 pytextrank-3.2.5/docs/sample_files/sample_27_0.svg
+-rw-r--r--   0 paco       (501) staff       (20)   122409 2022-03-06 22:41:12.000000 pytextrank-3.2.5/docs/sample_files/sample_36_0.svg
+-rw-r--r--   0 paco       (501) staff       (20)     2100 2021-03-25 19:11:35.000000 pytextrank-3.2.5/docs/setup.md
+-rw-r--r--   0 paco       (501) staff       (20)     1610 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/start.md
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/docs/stylesheets/
+-rw-r--r--   0 paco       (501) staff       (20)      260 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/stylesheets/extra.css
+-rw-r--r--   0 paco       (501) staff       (20)     3459 2021-07-17 19:45:35.000000 pytextrank-3.2.5/docs/talks.md
+-rw-r--r--   0 paco       (501) staff       (20)      277 2021-03-09 19:29:14.000000 pytextrank-3.2.5/docs/todo.md
+-rw-r--r--   0 paco       (501) staff       (20)     1082 2021-03-20 18:22:10.000000 pytextrank-3.2.5/docs/tutorial.md
+-rw-r--r--   0 paco       (501) staff       (20)      220 2021-10-10 01:11:11.000000 pytextrank-3.2.5/environment.yml
+-rwxr-xr-x   0 paco       (501) staff       (20)     1277 2021-07-07 15:46:34.000000 pytextrank-3.2.5/error.py
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/examples/
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/examples/.ipynb_checkpoints/
+-rw-r--r--   0 paco       (501) staff       (20)       72 2021-03-14 23:58:00.000000 pytextrank-3.2.5/examples/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)   166415 2021-03-23 18:59:09.000000 pytextrank-3.2.5/examples/.ipynb_checkpoints/explain_algo-checkpoint.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)    17250 2021-03-20 04:26:31.000000 pytextrank-3.2.5/examples/.ipynb_checkpoints/explain_summ-checkpoint.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)   197422 2023-08-07 04:52:30.000000 pytextrank-3.2.5/examples/.ipynb_checkpoints/sample-checkpoint.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)   166415 2021-03-25 19:11:35.000000 pytextrank-3.2.5/examples/explain_algo.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)    17250 2021-03-20 18:22:10.000000 pytextrank-3.2.5/examples/explain_summ.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)   196941 2023-08-07 19:17:45.000000 pytextrank-3.2.5/examples/sample.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)      489 2023-06-27 03:38:04.000000 pytextrank-3.2.5/foo.py
+-rw-r--r--   0 paco       (501) staff       (20)      599 2021-07-17 19:45:35.000000 pytextrank-3.2.5/lgtm.yml
+-rw-r--r--   0 paco       (501) staff       (20)     1052 2021-03-26 15:32:15.000000 pytextrank-3.2.5/meta.yaml
+-rw-r--r--   0 paco       (501) staff       (20)     1756 2022-03-06 22:26:05.000000 pytextrank-3.2.5/mkdocs.yml
+-rwxr-xr-x   0 paco       (501) staff       (20)     1205 2022-03-06 22:26:05.000000 pytextrank-3.2.5/pkg_doc.py
+-rwxr-xr-x   0 paco       (501) staff       (20)    13844 2021-07-17 19:45:35.000000 pytextrank-3.2.5/pyfixdoc.py
+-rw-r--r--   0 paco       (501) staff       (20)    16053 2021-07-17 19:45:35.000000 pytextrank-3.2.5/pylintrc
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/pytextrank/
+-rw-r--r--   0 paco       (501) staff       (20)     4633 2022-03-06 22:26:05.000000 pytextrank-3.2.5/pytextrank/__init__.py
+-rw-r--r--   0 paco       (501) staff       (20)    27788 2022-03-07 19:13:52.000000 pytextrank-3.2.5/pytextrank/base.py
+-rw-r--r--   0 paco       (501) staff       (20)     4589 2022-07-27 21:35:23.000000 pytextrank-3.2.5/pytextrank/biasedrank.py
+-rw-r--r--   0 paco       (501) staff       (20)     4090 2021-07-17 19:45:35.000000 pytextrank-3.2.5/pytextrank/positionrank.py
+-rw-r--r--   0 paco       (501) staff       (20)    13346 2022-07-27 21:35:23.000000 pytextrank-3.2.5/pytextrank/topicrank.py
+-rw-r--r--   0 paco       (501) staff       (20)     4307 2021-07-17 19:45:35.000000 pytextrank-3.2.5/pytextrank/util.py
+-rw-r--r--   0 paco       (501) staff       (20)     1334 2023-08-07 19:40:13.000000 pytextrank-3.2.5/pytextrank/version.py
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/pytextrank.egg-info/
+-rw-r--r--   0 paco       (501) staff       (20)     9672 2023-08-07 19:50:31.000000 pytextrank-3.2.5/pytextrank.egg-info/PKG-INFO
+-rw-r--r--   0 paco       (501) staff       (20)     2052 2023-08-07 19:50:31.000000 pytextrank-3.2.5/pytextrank.egg-info/SOURCES.txt
+-rw-r--r--   0 paco       (501) staff       (20)        1 2023-08-07 19:50:31.000000 pytextrank-3.2.5/pytextrank.egg-info/dependency_links.txt
+-rw-r--r--   0 paco       (501) staff       (20)        1 2019-11-05 20:30:26.000000 pytextrank-3.2.5/pytextrank.egg-info/not-zip-safe
+-rw-r--r--   0 paco       (501) staff       (20)      538 2023-08-07 19:50:31.000000 pytextrank-3.2.5/pytextrank.egg-info/requires.txt
+-rw-r--r--   0 paco       (501) staff       (20)       11 2023-08-07 19:50:31.000000 pytextrank-3.2.5/pytextrank.egg-info/top_level.txt
+-rw-r--r--   0 paco       (501) staff       (20)      339 2023-08-07 19:37:39.000000 pytextrank-3.2.5/requirements-dev.txt
+-rw-r--r--   0 paco       (501) staff       (20)       16 2021-07-17 19:45:35.000000 pytextrank-3.2.5/requirements-viz.txt
+-rw-r--r--   0 paco       (501) staff       (20)      102 2023-08-07 19:26:06.000000 pytextrank-3.2.5/requirements.txt
+-rw-r--r--   0 paco       (501) staff       (20)     1837 2022-03-07 19:16:57.000000 pytextrank-3.2.5/ru.py
+-rwxr-xr-x   0 paco       (501) staff       (20)     3738 2022-03-06 22:26:05.000000 pytextrank-3.2.5/sample.py
+-rw-r--r--   0 paco       (501) staff       (20)       38 2023-08-07 19:50:33.000000 pytextrank-3.2.5/setup.cfg
+-rw-r--r--   0 paco       (501) staff       (20)     3719 2022-03-06 22:44:13.000000 pytextrank-3.2.5/setup.py
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/tests/
+-rw-r--r--   0 paco       (501) staff       (20)     2300 2022-03-06 22:26:05.000000 pytextrank-3.2.5/tests/conftest.py
+-rw-r--r--   0 paco       (501) staff       (20)     5451 2022-07-27 22:02:18.000000 pytextrank-3.2.5/tests/test_base.py
+-rw-r--r--   0 paco       (501) staff       (20)     2372 2022-07-27 21:35:23.000000 pytextrank-3.2.5/tests/test_biasedrank.py
+-rw-r--r--   0 paco       (501) staff       (20)     1521 2022-02-04 19:59:51.000000 pytextrank-3.2.5/tests/test_positionrank.py
+-rw-r--r--   0 paco       (501) staff       (20)     6183 2022-07-27 22:02:18.000000 pytextrank-3.2.5/tests/test_topicrank.py
+-rwxr-xr-x   0 paco       (501) staff       (20)      783 2021-07-17 19:45:35.000000 pytextrank-3.2.5/tests/trace.py
+-rwxr-xr-x   0 paco       (501) staff       (20)     1410 2021-10-09 22:42:21.000000 pytextrank-3.2.5/tmp_api.py
+-rw-r--r--   0 paco       (501) staff       (20)     1477 2020-02-23 18:45:41.000000 pytextrank-3.2.5/udpipe.py
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/wip/
+drwxr-xr-x   0 paco       (501) staff       (20)        0 2023-08-07 19:50:33.000000 pytextrank-3.2.5/wip/.ipynb_checkpoints/
+-rw-r--r--   0 paco       (501) staff       (20)    15643 2021-03-17 03:20:40.000000 pytextrank-3.2.5/wip/.ipynb_checkpoints/error-checkpoint.ipynb
+-rw-r--r--   0 paco       (501) staff       (20)    15643 2021-03-20 18:22:10.000000 pytextrank-3.2.5/wip/error.ipynb
```

### Comparing `pytextrank-3.2.4/.pre-commit-config.yaml` & `pytextrank-3.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/CHANGELOG.md` & `pytextrank-3.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/CONTRIBUTING.md` & `pytextrank-3.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/LICENSE` & `pytextrank-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/MANIFEST.in` & `pytextrank-3.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/README.md` & `pytextrank-3.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 ## License and Copyright
 
 Source code for **PyTextRank** plus its logo, documentation, and examples
 have an [MIT license](https://spdx.org/licenses/MIT.html) which is
 succinct and simplifies use in commercial applications.
 
-All materials herein are Copyright &copy; 2016-2022 Derwen, Inc.
+All materials herein are Copyright &copy; 2016-2023 Derwen, Inc.
 
 
 ## Attribution
 
 Please use the following BibTeX entry for citing **PyTextRank** if you 
 use it in your research or software:
 ```bibtex
@@ -168,14 +168,15 @@
 [@CaptXiong](https://github.com/CaptXiong),
 [@Lord-V15](https://github.com/Lord-V15),
 [@anna-droid-beep](https://github.com/anna-droid-beep),
 [@dvsrepo](https://github.com/dvsrepo),
 [@clabornd](https://github.com/clabornd),
 [@dayalstrub-cma](https://github.com/dayalstrub-cma),
 [@kavorite](https://github.com/kavorite),
+[@0dB](https://github.com/0dB),
 [@htmartin](https://github.com/htmartin),
 [@williamsmj](https://github.com/williamsmj/),
 [@mattkohl](https://github.com/mattkohl),
 [@vanita5](https://github.com/vanita5),
 [@HarshGrandeur](https://github.com/HarshGrandeur),
 [@mnowotka](https://github.com/mnowotka),
 [@kjam](https://github.com/kjam),
```

### Comparing `pytextrank-3.2.4/bin/preview.py` & `pytextrank-3.2.5/bin/preview.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/bin/vis_doc.py` & `pytextrank-3.2.5/bin/vis_doc.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/code_of_conduct.md` & `pytextrank-3.2.5/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/dat/ars.txt` & `pytextrank-3.2.5/dat/ars.txt`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/dat/cfc.txt` & `pytextrank-3.2.5/dat/cfc.txt`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/dat/gen.txt` & `pytextrank-3.2.5/dat/gen.txt`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/dat/lee.txt` & `pytextrank-3.2.5/dat/lee.txt`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/dat/mih.txt` & `pytextrank-3.2.5/dat/mih.txt`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/dat/suz.txt` & `pytextrank-3.2.5/dat/suz.txt`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/deprecated/example.ipynb` & `pytextrank-3.2.5/deprecated/example.ipynb`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/deprecated/oldsrc.py` & `pytextrank-3.2.5/deprecated/oldsrc.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/deprecated/test.py` & `pytextrank-3.2.5/deprecated/test.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/ack.md` & `pytextrank-3.2.5/docs/ack.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 [@CaptXiong](https://github.com/CaptXiong),
 [@Lord-V15](https://github.com/Lord-V15),
 [@anna-droid-beep](https://github.com/anna-droid-beep),
 [@dvsrepo](https://github.com/dvsrepo),
 [@clabornd](https://github.com/clabornd),
 [@dayalstrub-cma](https://github.com/dayalstrub-cma),
 [@kavorite](https://github.com/kavorite),
+[@0dB](https://github.com/0dB),
 [@htmartin](https://github.com/htmartin),
 [@williamsmj](https://github.com/williamsmj/),
 [@mattkohl](https://github.com/mattkohl),
 [@vanita5](https://github.com/vanita5),
 [@HarshGrandeur](https://github.com/HarshGrandeur),
 [@mnowotka](https://github.com/mnowotka),
 [@kjam](https://github.com/kjam),
@@ -110,15 +111,15 @@
 
 ## License and Copyright
 
 Source code for **pytextrank** plus its logo, documentation, and examples
 have an [MIT license](https://spdx.org/licenses/MIT.html) which is
 succinct and simplifies use in commercial applications.
 
-All materials herein are Copyright &copy; 2016-2022 Derwen, Inc.
+All materials herein are Copyright &copy; 2016-2023 Derwen, Inc.
 
 [![logo for Derwen, Inc.](https://derwen.ai/static/block_logo.png)](https://derwen.ai/)
 
 
 ## Production Use Cases
 
   * [Derwen](https://derwen.ai/) and its client projects
```

#### html2text {}

```diff
@@ -1,66 +1,66 @@
 # Acknowledgements ## Contributors Many thanks to our open source [sponsors]
 (https://github.com/sponsors/ceteri); and to our contributors: [@louisguitton]
 (https://github.com/louisguitton), [@Ankush-Chander](https://github.com/Ankush-
 Chander), [@tomaarsen](https://github.com/tomaarsen), [@CaptXiong](https://
 github.com/CaptXiong), [@Lord-V15](https://github.com/Lord-V15), [@anna-droid-
 beep](https://github.com/anna-droid-beep), [@dvsrepo](https://github.com/
 dvsrepo), [@clabornd](https://github.com/clabornd), [@dayalstrub-cma](https://
-github.com/dayalstrub-cma), [@kavorite](https://github.com/kavorite),
-[@htmartin](https://github.com/htmartin), [@williamsmj](https://github.com/
-williamsmj/), [@mattkohl](https://github.com/mattkohl), [@vanita5](https://
-github.com/vanita5), [@HarshGrandeur](https://github.com/HarshGrandeur),
-[@mnowotka](https://github.com/mnowotka), [@kjam](https://github.com/kjam),
-[@SaiThejeshwar](https://github.com/SaiThejeshwar), [@laxatives](https://
-github.com/laxatives), [@dimmu](https://github.com/dimmu), [@JasonZhangzy1757]
-(https://github.com/JasonZhangzy1757), [@jake-aft](https://github.com/jake-
-aft), [@junchen1992](https://github.com/junchen1992), [@shyamcody](https://
-github.com/shyamcody), [@chikubee](https://github.com/chikubee); also to
-[@mihalcea](https://github.com/mihalcea) who leads outstanding NLP research
-work, encouragement from the wonderful folks at Explosion who develop [spaCy]
-(https://github.com/explosion/spaCy), plus general support from [Derwen, Inc.]
-(https://derwen.ai/) ## Project Lead [Paco Nathan](https://derwen.ai/paco) is
-lead committer on **pytextrank** and lead author for its documentation and
-tutorial. By day he's the Managing Partner at [Derwen, Inc.](https://derwen.ai/
-) Paco's formal background is in Mathematics (advisor: [Richard Cottle](https:/
-/engineering.stanford.edu/people/richard-cottle)) and Computer Science
-(advisor: [Douglas Lenat](https://en.wikipedia.org/wiki/Douglas_Lenat)), with
-additional work in Design and Linguistics. His business experience includes:
-Director, VP, and CTO positions leading data teams and machine learning
-projects; former CTO/Board member at two publicly-traded tech firms on NASDAQ
-OTC:BB; and an equity partner at [Amplify Partners](https://derwen.ai/s/
-hcxhybks9nbh). Cited in 2015 as one of the [Top 30 People in Big Data and
-Analytics](http://www.kdnuggets.com/2015/02/top-30-people-big-data-
-analytics.html) by Innovation Enterprise. * ~40 years tech industry experience,
-ranging from Bell Labs to early-stage start-ups * 7+ years R&D in *neural
-networks* (incl. h/w accelerators) during 1980-90s * early "guinea pig" for
-Amazon AWS (2006), who led the first large-scale Hadoop use case on [cloud
-computing](../glossary/#cloud-computing) (2008) * former Director, Community
-Evangelism at Databricks (2014-2015) for [Apache Spark](https://
-spark.apache.org/) * lead committer on [kglab](https://derwen.ai/docs/kgl/);
-open source community work on [Jupyter](https://jupyter.org/), [Ray](https://
-ray.io/), [Cascading](https://www.cascading.org/) * consultant to enterprise
-organizations for [data strategy](../glossary/#data-strategy); advisor to
-several AI start-ups, including [Recognai](https://derwen.ai/s/hk4g),
-[KUNGFU.AI](https://derwen.ai/s/rwg8prbgqp36), [Primer](https://derwen.ai/s/
-tm9jxzcm67hc) As an author/speaker/instructor, Paco has taught many people
-(+9000) in industry across a range of topics â [*data science*](../glossary/
-#data-science), [*natural language*](../glossary/#natural-language), [*cloud
-computing*](../glossary/#cloud-computing), [*reinforcement learning*](../
-glossary/#reinforcement-learning), [*computable content*](../glossary/
+github.com/dayalstrub-cma), [@kavorite](https://github.com/kavorite), [@0dB]
+(https://github.com/0dB), [@htmartin](https://github.com/htmartin),
+[@williamsmj](https://github.com/williamsmj/), [@mattkohl](https://github.com/
+mattkohl), [@vanita5](https://github.com/vanita5), [@HarshGrandeur](https://
+github.com/HarshGrandeur), [@mnowotka](https://github.com/mnowotka), [@kjam]
+(https://github.com/kjam), [@SaiThejeshwar](https://github.com/SaiThejeshwar),
+[@laxatives](https://github.com/laxatives), [@dimmu](https://github.com/dimmu),
+[@JasonZhangzy1757](https://github.com/JasonZhangzy1757), [@jake-aft](https://
+github.com/jake-aft), [@junchen1992](https://github.com/junchen1992),
+[@shyamcody](https://github.com/shyamcody), [@chikubee](https://github.com/
+chikubee); also to [@mihalcea](https://github.com/mihalcea) who leads
+outstanding NLP research work, encouragement from the wonderful folks at
+Explosion who develop [spaCy](https://github.com/explosion/spaCy), plus general
+support from [Derwen, Inc.](https://derwen.ai/) ## Project Lead [Paco Nathan]
+(https://derwen.ai/paco) is lead committer on **pytextrank** and lead author
+for its documentation and tutorial. By day he's the Managing Partner at
+[Derwen, Inc.](https://derwen.ai/) Paco's formal background is in Mathematics
+(advisor: [Richard Cottle](https://engineering.stanford.edu/people/richard-
+cottle)) and Computer Science (advisor: [Douglas Lenat](https://
+en.wikipedia.org/wiki/Douglas_Lenat)), with additional work in Design and
+Linguistics. His business experience includes: Director, VP, and CTO positions
+leading data teams and machine learning projects; former CTO/Board member at
+two publicly-traded tech firms on NASDAQ OTC:BB; and an equity partner at
+[Amplify Partners](https://derwen.ai/s/hcxhybks9nbh). Cited in 2015 as one of
+the [Top 30 People in Big Data and Analytics](http://www.kdnuggets.com/2015/02/
+top-30-people-big-data-analytics.html) by Innovation Enterprise. * ~40 years
+tech industry experience, ranging from Bell Labs to early-stage start-ups * 7+
+years R&D in *neural networks* (incl. h/w accelerators) during 1980-90s * early
+"guinea pig" for Amazon AWS (2006), who led the first large-scale Hadoop use
+case on [cloud computing](../glossary/#cloud-computing) (2008) * former
+Director, Community Evangelism at Databricks (2014-2015) for [Apache Spark]
+(https://spark.apache.org/) * lead committer on [kglab](https://derwen.ai/docs/
+kgl/); open source community work on [Jupyter](https://jupyter.org/), [Ray]
+(https://ray.io/), [Cascading](https://www.cascading.org/) * consultant to
+enterprise organizations for [data strategy](../glossary/#data-strategy);
+advisor to several AI start-ups, including [Recognai](https://derwen.ai/s/
+hk4g), [KUNGFU.AI](https://derwen.ai/s/rwg8prbgqp36), [Primer](https://
+derwen.ai/s/tm9jxzcm67hc) As an author/speaker/instructor, Paco has taught many
+people (+9000) in industry across a range of topics â [*data science*](../
+glossary/#data-science), [*natural language*](../glossary/#natural-language),
+[*cloud computing*](../glossary/#cloud-computing), [*reinforcement learning*]
+(../glossary/#reinforcement-learning), [*computable content*](../glossary/
 #computable-content), etc. â and through guest lectures at Stanford, CMU,
 UC Berkeley, U da CoruÃ±a, U Manchester, KTH, NYU, GWU, U Maryland, Cal Poly,
 UT/Austin, Northeastern, U Virginia, CU Boulder. [profile_for_Paco_at_Stack
 Overflow,_Q&A_for_professional_and_enthusiast_programmers] ## Attribution
 Please use the following BibTeX entry for citing **pytextrank** if you use it
 in your research or software: ``` @software{PyTextRank, author = {Paco Nathan},
 title = {{PyTextRank, a Python implementation of TextRank for phrase extraction
 and summarization of text documents}}, year = 2016, publisher = {Derwen}, doi =
 {10.5281/zenodo.4637885}, url = {https://github.com/DerwenAI/pytextrank} } ```
 **DOI:**
 doi.org/10.5281/zenodo.4637885> ## License and Copyright Source code for
 **pytextrank** plus its logo, documentation, and examples have an [MIT license]
 (https://spdx.org/licenses/MIT.html) which is succinct and simplifies use in
-commercial applications. All materials herein are Copyright © 2016-2022 Derwen,
+commercial applications. All materials herein are Copyright © 2016-2023 Derwen,
 Inc. [![logo for Derwen, Inc.](https://derwen.ai/static/block_logo.png)](https:
 //derwen.ai/) ## Production Use Cases * [Derwen](https://derwen.ai/) and its
 client projects
```

### Comparing `pytextrank-3.2.4/docs/assets/favicon.png` & `pytextrank-3.2.5/docs/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/assets/logo.png` & `pytextrank-3.2.5/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/assets/noam.jpg` & `pytextrank-3.2.5/docs/assets/noam.jpg`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/biblio.jinja` & `pytextrank-3.2.5/docs/biblio.jinja`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/biblio.md` & `pytextrank-3.2.5/docs/biblio.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/build.md` & `pytextrank-3.2.5/docs/build.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/codecov_io.svg` & `pytextrank-3.2.5/docs/codecov_io.svg`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/explain_algo.md` & `pytextrank-3.2.5/docs/explain_algo.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/explain_algo_files/explain_algo_20_1.png` & `pytextrank-3.2.5/docs/explain_algo_files/explain_algo_20_1.png`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/explain_algo_files/explain_algo_23_0.png` & `pytextrank-3.2.5/docs/explain_algo_files/explain_algo_23_0.png`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/explain_summ.md` & `pytextrank-3.2.5/docs/explain_summ.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/faq.md` & `pytextrank-3.2.5/docs/faq.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/glossary.jinja` & `pytextrank-3.2.5/docs/glossary.jinja`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/glossary.md` & `pytextrank-3.2.5/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/index.md` & `pytextrank-3.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/mkrefs.ttl` & `pytextrank-3.2.5/docs/mkrefs.ttl`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/mkrefs.yml` & `pytextrank-3.2.5/docs/mkrefs.yml`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/noam.jpg` & `pytextrank-3.2.5/docs/noam.jpg`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/overview.md` & `pytextrank-3.2.5/docs/overview.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/ref.jinja` & `pytextrank-3.2.5/docs/ref.jinja`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/ref.md` & `pytextrank-3.2.5/docs/ref.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/sample.md` & `pytextrank-3.2.5/docs/sample.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/sample_files/sample_27_0.svg` & `pytextrank-3.2.5/docs/sample_files/sample_27_0.svg`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/sample_files/sample_36_0.svg` & `pytextrank-3.2.5/docs/sample_files/sample_36_0.svg`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/setup.md` & `pytextrank-3.2.5/docs/setup.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/start.md` & `pytextrank-3.2.5/docs/start.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/talks.md` & `pytextrank-3.2.5/docs/talks.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/docs/tutorial.md` & `pytextrank-3.2.5/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/error.py` & `pytextrank-3.2.5/error.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/examples/.ipynb_checkpoints/explain_algo-checkpoint.ipynb` & `pytextrank-3.2.5/examples/.ipynb_checkpoints/explain_algo-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/examples/.ipynb_checkpoints/explain_summ-checkpoint.ipynb` & `pytextrank-3.2.5/examples/.ipynb_checkpoints/explain_summ-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/examples/.ipynb_checkpoints/sample-checkpoint.ipynb` & `pytextrank-3.2.5/examples/sample.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9846972309496491%*

 * *Differences: {"'cells'": '{7: {\'outputs\': {1: {\'data\': {\'text/plain\': {insert: [(43, " \'attrs\': '*

 * *            '{\'token.dep\': {\'assigns\': [\'parser\'], \'requires\': []},\\n"), (46, "  '*

 * *            '\'token.is_sent_start\': {\'assigns\': [\'parser\'], \'requires\': []},\\n"), (47, "  '*

 * *            '\'token.ent_iob\': {\'assigns\': [\'ner\'], \'requires\': []},\\n"), (49, "  '*

 * *            '\'doc.ents\': {\'assigns\': [\'ner\'], \'requires\': []},\\n"), (50, "  '*

 * *            '\'doc.sents\': {\'assigns\': [\'pa […]*

```diff
@@ -169,24 +169,24 @@
                             " 'problems': {'tok2vec': [],\n",
                             "  'tagger': [],\n",
                             "  'parser': [],\n",
                             "  'attribute_ruler': [],\n",
                             "  'lemmatizer': [],\n",
                             "  'ner': [],\n",
                             "  'textrank': []},\n",
-                            " 'attrs': {'token.ent_iob': {'assigns': ['ner'], 'requires': []},\n",
+                            " 'attrs': {'token.dep': {'assigns': ['parser'], 'requires': []},\n",
                             "  'token.ent_type': {'assigns': ['ner'], 'requires': []},\n",
-                            "  'token.tag': {'assigns': ['tagger'], 'requires': []},\n",
-                            "  'token.dep': {'assigns': ['parser'], 'requires': []},\n",
                             "  'token.head': {'assigns': ['parser'], 'requires': []},\n",
-                            "  'doc.sents': {'assigns': ['parser'], 'requires': []},\n",
-                            "  'doc.ents': {'assigns': ['ner'], 'requires': []},\n",
+                            "  'token.is_sent_start': {'assigns': ['parser'], 'requires': []},\n",
+                            "  'token.ent_iob': {'assigns': ['ner'], 'requires': []},\n",
                             "  'doc.tensor': {'assigns': ['tok2vec'], 'requires': []},\n",
+                            "  'doc.ents': {'assigns': ['ner'], 'requires': []},\n",
+                            "  'doc.sents': {'assigns': ['parser'], 'requires': []},\n",
                             "  'token.lemma': {'assigns': ['lemmatizer'], 'requires': []},\n",
-                            "  'token.is_sent_start': {'assigns': ['parser'], 'requires': []}}}"
+                            "  'token.tag': {'assigns': ['tagger'], 'requires': []}}}"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -272,15 +272,15 @@
             "id": "adaptive-paper",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| tr.elapsed_time: 5.707979202270508\n"
+                        "ic| tr.elapsed_time: 7.581949234008789\n"
                     ]
                 }
             ],
             "source": [
                 "tr = doc._.textrank\n",
                 "ic(tr.elapsed_time);"
             ]
@@ -302,111 +302,107 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase.rank: 0.17054248030845812\n",
+                        "ic| phrase.rank: 0.18359439311764025\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'mixed types'\n",
                         "ic| phrase.chunks: [mixed types]\n",
-                        "ic| phrase.rank: 0.15757771579579002\n",
-                        "    phrase.count: 1\n",
-                        "    phrase.text: 'minimal generating sets'\n",
-                        "ic| phrase.chunks: [minimal generating sets]\n",
-                        "ic| phrase.rank: 0.1573942320091846\n",
+                        "ic| phrase.rank: 0.1784796193107821\n",
                         "    phrase.count: 3\n",
                         "    phrase.text: 'systems'\n",
                         "ic| phrase.chunks: [systems, systems, systems]\n",
-                        "ic| phrase.rank: 0.14894241299658317\n",
+                        "ic| phrase.rank: 0.15037838042245094\n",
+                        "    phrase.count: 1\n",
+                        "    phrase.text: 'minimal generating sets'\n",
+                        "ic| phrase.chunks: [minimal generating sets]\n",
+                        "ic| phrase.rank: 0.14740065982407313\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'nonstrict inequations'\n",
                         "ic| phrase.chunks: [nonstrict inequations]\n",
-                        "ic| phrase.rank: 0.14039169904589088\n",
+                        "ic| phrase.rank: 0.13946027725597837\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'strict inequations'\n",
                         "ic| phrase.chunks: [strict inequations]\n",
-                        "ic| phrase.rank: 0.11698198658021898\n",
-                        "    phrase.count: 1\n",
-                        "    phrase.text: 'natural numbers'\n",
-                        "ic| phrase.chunks: [natural numbers]\n",
-                        "ic| phrase.rank: 0.11559770516796158\n",
+                        "ic| phrase.rank: 0.1195023546245721\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'linear Diophantine equations'\n",
                         "ic| phrase.chunks: [linear Diophantine equations]\n",
-                        "ic| phrase.rank: 0.11407086615794945\n",
+                        "ic| phrase.rank: 0.11450088293222845\n",
+                        "    phrase.count: 1\n",
+                        "    phrase.text: 'natural numbers'\n",
+                        "ic| phrase.chunks: [natural numbers]\n",
+                        "ic| phrase.rank: 0.10780718173686318\n",
                         "    phrase.count: 3\n",
                         "    phrase.text: 'solutions'\n",
                         "ic| phrase.chunks: [solutions, solutions, solutions]\n",
-                        "ic| phrase.rank: 0.10165710454752863\n",
+                        "ic| phrase.rank: 0.10529828014583348\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'linear constraints'\n",
                         "ic| phrase.chunks: [linear constraints]\n",
-                        "ic| phrase.rank: 0.09237587396226833\n",
+                        "ic| phrase.rank: 0.1036960590708142\n",
+                        "    phrase.count: 1\n",
+                        "    phrase.text: 'all the considered types systems'\n",
+                        "ic| phrase.chunks: [all the considered types systems]\n",
+                        "ic| phrase.rank: 0.08812713074893187\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'a minimal supporting set'\n",
                         "ic| phrase.chunks: [a minimal supporting set]\n",
-                        "ic| phrase.rank: 0.08845296671843554\n",
+                        "ic| phrase.rank: 0.08243620500315359\n",
                         "    phrase.count: 1\n",
-                        "    phrase.text: 'all the considered types systems'\n",
-                        "ic| phrase.chunks: [all the considered types systems]\n",
-                        "ic| phrase.rank: 0.08294839224739124\n",
+                        "    phrase.text: 'a system'\n",
+                        "ic| phrase.chunks: [a system]\n",
+                        "ic| phrase.rank: 0.07944607954086784\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'a minimal set'\n",
                         "ic| phrase.chunks: [a minimal set]\n",
-                        "ic| phrase.rank: 0.08107274369298882\n",
+                        "ic| phrase.rank: 0.0763527926213032\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'algorithms'\n",
                         "ic| phrase.chunks: [algorithms]\n",
-                        "ic| phrase.rank: 0.07429406639612553\n",
-                        "    phrase.count: 1\n",
-                        "    phrase.text: 'construction'\n",
-                        "ic| phrase.chunks: [construction]\n",
-                        "ic| phrase.rank: 0.07269728177551771\n",
+                        "ic| phrase.rank: 0.07593126037016427\n",
                         "    phrase.count: 1\n",
-                        "    phrase.text: 'a system'\n",
-                        "ic| phrase.chunks: [a system]\n",
-                        "ic| phrase.rank: 0.07130948853545689\n",
+                        "    phrase.text: 'all types'\n",
+                        "ic| phrase.chunks: [all types]\n",
+                        "ic| phrase.rank: 0.07309361902551355\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'Diophantine'\n",
                         "ic| phrase.chunks: [Diophantine]\n",
-                        "ic| phrase.rank: 0.07034880604533804\n",
+                        "ic| phrase.rank: 0.0702090100898443\n",
                         "    phrase.count: 1\n",
-                        "    phrase.text: 'all types'\n",
-                        "ic| phrase.chunks: [all types]\n",
-                        "ic| phrase.rank: 0.06480303503167001\n",
-                        "    phrase.count: 1\n",
-                        "    phrase.text: 'Upper bounds'\n",
-                        "ic| phrase.chunks: [Upper bounds]\n",
-                        "ic| phrase.rank: 0.05969087234318076\n",
+                        "    phrase.text: 'construction'\n",
+                        "ic| phrase.chunks: [construction]\n",
+                        "ic| phrase.rank: 0.05800111772673988\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'the set'\n",
                         "ic| phrase.chunks: [the set]\n",
-                        "ic| phrase.rank: 0.05837512270115124\n",
+                        "ic| phrase.rank: 0.054251394765316464\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'components'\n",
                         "ic| phrase.chunks: [components]\n",
-                        "ic| phrase.rank: 0.048602276273752514\n",
+                        "ic| phrase.rank: 0.04516904342912139\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'Compatibility'\n",
                         "ic| phrase.chunks: [Compatibility]\n",
-                        "ic| phrase.rank: 0.048602276273752514\n",
+                        "ic| phrase.rank: 0.04516904342912139\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'compatibility'\n",
                         "ic| phrase.chunks: [compatibility]\n",
-                        "ic| phrase.rank: 0.0472624878442175\n",
+                        "ic| phrase.rank: 0.04435648606848154\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'the corresponding algorithms'\n",
                         "ic| phrase.chunks: [the corresponding algorithms]\n",
-                        "ic| phrase.rank: 0.04548690742119631\n",
+                        "ic| phrase.rank: 0.042273783712246285\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'Criteria'\n",
                         "ic| phrase.chunks: [Criteria]\n",
-                        "ic| phrase.rank: 0.021009502595385022\n",
+                        "ic| phrase.rank: 0.01952542432474353\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'These criteria'\n",
                         "ic| phrase.chunks: [These criteria]\n"
                     ]
                 }
             ],
             "source": [
@@ -414,44 +410,51 @@
                 "    ic(phrase.rank, phrase.count, phrase.text)\n",
                 "    ic(phrase.chunks)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "medium-vertex",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
             "source": [
                 "## Stop Words\n",
                 "\n",
                 "To show use of the *stop words* feature, first we'll output a baseline..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "separated-mambo",
             "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                },
                 "scrolled": true,
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='words', chunks=[words, words], count=2, rank=0.15746606699141763)\n",
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.12965916420829138)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.10571655249620954)\n",
-                        "ic| phrase: Phrase(text='the remaining words', chunks=[the remaining words], count=1, rank=0.09329379463860477)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.08981955768260336)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.0843351188899575)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.07936404910104827)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07400094270083186)\n",
-                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.07073416034725326)\n",
-                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.06710956557420322)\n"
+                        "ic| phrase: Phrase(text='words', chunks=[words, words], count=2, rank=0.16137018222637944)\n",
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.13367291641220508)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.1095023226326187)\n",
+                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.10745197034799042)\n",
+                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.10502825160040344)\n",
+                        "ic| phrase: Phrase(text='the remaining words', chunks=[the remaining words], count=1, rank=0.09559863808781449)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09162794519014893)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.08555365347028678)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.07894442579092492)\n",
+                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.07747520663125698)\n"
                     ]
                 }
             ],
             "source": [
                 "text = pathlib.Path(\"../dat/gen.txt\").read_text()\n",
                 "doc = nlp(text)\n",
                 "\n",
@@ -477,24 +480,24 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.14407775200046075)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.11286475216345385)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09589788430130489)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09004754289053603)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08473538778364878)\n",
-                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.07909136977858265)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07900911166567022)\n",
-                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07165073049436399)\n",
-                        "ic| phrase: Phrase(text='TextRank', chunks=[TextRank, TextRank, TextRank, TextRank], count=4, rank=0.06888311869751775)\n",
-                        "ic| phrase: Phrase(text='every sentence', chunks=[every sentence], count=1, rank=0.06654666312136172)\n"
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.1490464677880926)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.117318519527749)\n",
+                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.11512161354108796)\n",
+                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.11252482346188267)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09816426515530181)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09165889278462461)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08457790386936588)\n",
+                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.08300479194058319)\n",
+                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.08179233228776425)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07919192237459494)\n"
                     ]
                 }
             ],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"textrank\", config={ \"stopwords\": { \"word\": [\"NOUN\"] } })\n",
                 "\n",
@@ -528,36 +531,36 @@
             "id": "living-cholesterol",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences, the sentences], count=2, rank=0.14407775200046075)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.11286475216345385)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09589788430130489)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09004754289053603)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08473538778364878)\n",
-                        "ic| phrase: Phrase(text='sentence', chunks=[every sentence, every other sentence], count=2, rank=0.07909136977858265)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07900911166567022)\n",
-                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07165073049436399)\n",
-                        "ic| phrase: Phrase(text='TextRank', chunks=[TextRank, TextRank, TextRank, TextRank], count=4, rank=0.06888311869751775)\n",
-                        "ic| phrase: Phrase(text='two sentences', chunks=[the two sentences, two sentences], count=2, rank=0.06654666312136172)\n"
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences, the sentences], count=2, rank=0.1490464677880926)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.117318519527749)\n",
+                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.11512161354108796)\n",
+                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.11252482346188267)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09816426515530181)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09165889278462461)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08457790386936588)\n",
+                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.08300479194058319)\n",
+                        "ic| phrase: Phrase(text='sentence', chunks=[every sentence, every other sentence], count=2, rank=0.08179233228776425)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07919192237459494)\n"
                     ]
                 }
             ],
             "source": [
                 "from spacy.tokens import Span\n",
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "\n",
                 "\n",
                 "@spacy.registry.misc(\"prefix_scrubber\")\n",
                 "def prefix_scrubber():\n",
                 "\tdef scrubber_func(span: Span) -> str:\n",
-                "\t\twhile span[0].text in (\"a\", \"the\", \"their\", \"every\", \"other\"):\n",
+                "\t\twhile len(span) > 1 and span[0].text in (\"a\", \"the\", \"their\", \"every\", \"other\"):\n",
                 "\t\t\tspan = span[1:]\n",
                 "\t\treturn span.text\n",
                 "\treturn scrubber_func\n",
                 "\n",
                 "nlp.add_pipe(\"textrank\", config={ \"stopwords\": { \"word\": [\"NOUN\"] }, \"scrubber\": {\"@misc\": \"prefix_scrubber\"}})\n",
                 "\n",
                 "doc = nlp(text)\n",
@@ -606,24 +609,24 @@
             "id": "7535d038-0cb1-4bb3-90df-9b5a87e32b94",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences, the sentences], count=2, rank=0.14407775200046075)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.11286475216345385)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09589788430130489)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09004754289053603)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08473538778364878)\n",
-                        "ic| phrase: Phrase(text='other sentence', chunks=[every other sentence], count=1, rank=0.07909136977858265)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07900911166567022)\n",
-                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07165073049436399)\n",
-                        "ic| phrase: Phrase(text='TextRank', chunks=[TextRank, TextRank, TextRank, TextRank], count=4, rank=0.06888311869751775)\n",
-                        "ic| phrase: Phrase(text='sentence', chunks=[every sentence], count=1, rank=0.06654666312136172)\n"
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences, the sentences], count=2, rank=0.1490464677880926)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.117318519527749)\n",
+                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.11512161354108796)\n",
+                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.11252482346188267)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09816426515530181)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09165889278462461)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08457790386936588)\n",
+                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.08300479194058319)\n",
+                        "ic| phrase: Phrase(text='other sentence', chunks=[every other sentence], count=1, rank=0.08179233228776425)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07919192237459494)\n"
                     ]
                 }
             ],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"textrank\", config={ \"stopwords\": { \"word\": [\"NOUN\"] }, \"scrubber\": {\"@misc\": \"articles_scrubber\"}})\n",
                 "\n",
@@ -664,23 +667,23 @@
             "id": "8af03b4c-77f3-4d1a-883f-ce880d202e86",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.14407775200046075)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09589788430130489)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09004754289053603)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08473538778364878)\n",
-                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.07909136977858265)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07900911166567022)\n",
-                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07165073049436399)\n",
-                        "ic| phrase: Phrase(text='every sentence', chunks=[every sentence], count=1, rank=0.06654666312136172)\n",
-                        "ic| phrase: Phrase(text='the sentences', chunks=[the sentences], count=1, rank=0.06654666312136172)\n"
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.1490464677880926)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09816426515530181)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09165889278462461)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08457790386936588)\n",
+                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.08300479194058319)\n",
+                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.08179233228776425)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07919192237459494)\n",
+                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07346227481329015)\n",
+                        "ic| phrase: Phrase(text='TextRank', chunks=[TextRank], count=1, rank=0.07058237377923389)\n"
                     ]
                 }
             ],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"textrank\", config={ \"stopwords\": { \"word\": [\"NOUN\"] }, \"scrubber\": {\"@misc\": \"entity_scrubber\"}})\n",
                 "\n",
@@ -718,15 +721,15 @@
             "id": "classical-fairy",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "-rw-r--r--  1 paco  staff    17K Mar  6 14:39 lemma_graph.dot\n"
+                        "-rw-rw-r-- 1 ankushchander ankushchander 17K Jun  4 11:56 lemma_graph.dot\r\n"
                     ]
                 }
             ],
             "source": [
                 "!ls -lth lemma_graph.dot"
             ]
         },
@@ -738,15 +741,15 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: graphviz in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (0.17)\n"
+                        "Requirement already satisfied: graphviz in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (0.19.1)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install graphviz"
             ]
         },
@@ -774,1664 +777,1629 @@
             "outputs": [
                 {
                     "data": {
                         "image/svg+xml": [
                             "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 2.49.2 (20211016.1639)\n",
+                            "<!-- Generated by graphviz version 2.43.0 (0)\n",
                             " -->\n",
-                            "<!-- Pages: 1 -->\n",
-                            "<svg width=\"17390pt\" height=\"80pt\"\n",
-                            " viewBox=\"0.00 0.00 17390.33 80.23\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 76.23)\">\n",
-                            "<polygon fill=\"white\" stroke=\"transparent\" points=\"-4,4 -4,-76.23 17386.33,-76.23 17386.33,4 -4,4\"/>\n",
+                            "<!-- Title: %3 Pages: 1 -->\n",
+                            "<svg width=\"20016pt\" height=\"80pt\"\n",
+                            " viewBox=\"0.00 0.00 20015.53 80.16\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 76.16)\">\n",
+                            "<title>%3</title>\n",
+                            "<polygon fill=\"white\" stroke=\"transparent\" points=\"-4,4 -4,-76.16 20011.53,-76.16 20011.53,4 -4,4\"/>\n",
                             "<!-- (&#39;quick&#39;, &#39;ADJ&#39;) -->\n",
                             "<g id=\"node1\" class=\"node\">\n",
                             "<title>(&#39;quick&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"98.14\" cy=\"-18\" rx=\"98.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"98.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;quick&#39;, &#39;ADJ&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"116.99\" cy=\"-18\" rx=\"116.98\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"116.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;quick&#39;, &#39;ADJ&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;description&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node2\" class=\"node\">\n",
                             "<title>(&#39;description&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"342.14\" cy=\"-18\" rx=\"128.08\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"342.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;description&#39;, &#39;NOUN&#39;) (0.0053)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"409.99\" cy=\"-18\" rx=\"157.87\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"409.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;description&#39;, &#39;NOUN&#39;) (0.0056)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;quick&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;description&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge1\" class=\"edge\">\n",
                             "<title>(&#39;quick&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;description&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M196.31,-18C198.8,-18 201.28,-18 203.76,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"203.97,-21.5 213.97,-18 203.97,-14.5 203.97,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M234.02,-18C236.62,-18 239.23,-18 241.84,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"241.89,-21.5 251.89,-18 241.89,-14.5 241.89,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;popular&#39;, &#39;ADJ&#39;) -->\n",
                             "<g id=\"node3\" class=\"node\">\n",
                             "<title>(&#39;popular&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"594.14\" cy=\"-18\" rx=\"105.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"594.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;popular&#39;, &#39;ADJ&#39;) (0.0095)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"713.99\" cy=\"-18\" rx=\"128.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"713.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;popular&#39;, &#39;ADJ&#39;) (0.0100)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;quick&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;) -->\n",
                             "<g id=\"edge2\" class=\"edge\">\n",
                             "<title>(&#39;quick&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M140.12,-34.38C161.85,-41.99 189.02,-50.19 214.14,-54 326.63,-71.05 357.5,-70.02 470.14,-54 493.33,-50.7 518.25,-44.1 539.62,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"540.72,-40.76 549.17,-34.38 538.58,-34.09 540.72,-40.76\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M166.06,-34.39C191.4,-42 223.01,-50.2 251.99,-54 391.24,-72.25 428.57,-70.94 567.99,-54 595.56,-50.65 625.43,-43.87 650.92,-37.09\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"652.1,-40.39 660.83,-34.39 650.26,-33.64 652.1,-40.39\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node4\" class=\"node\">\n",
                             "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"841.14\" cy=\"-18\" rx=\"122.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"841.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;algorithm&#39;, &#39;NOUN&#39;) (0.0114)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1010.99\" cy=\"-18\" rx=\"151.37\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1010.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;algorithm&#39;, &#39;NOUN&#39;) (0.0276)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;quick&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge3\" class=\"edge\">\n",
                             "<title>(&#39;quick&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M140.12,-34.38C161.85,-41.99 189.02,-50.19 214.14,-54 320.92,-70.19 592.98,-67.46 700.14,-54 726.69,-50.66 755.4,-43.93 779.95,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"781.16,-40.47 789.84,-34.39 779.27,-33.73 781.16,-40.47\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M166.06,-34.39C191.4,-42 223.01,-50.2 251.99,-54 381.99,-71.04 711.6,-67.73 841.99,-54 874.15,-50.61 909.2,-43.69 939,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"939.96,-40.19 948.89,-34.49 938.35,-33.37 939.96,-40.19\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;description&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;) -->\n",
                             "<g id=\"edge4\" class=\"edge\">\n",
                             "<title>(&#39;description&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M470.6,-18C473.05,-18 475.49,-18 477.93,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"477.97,-21.5 487.97,-18 477.97,-14.5 477.97,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M567.93,-18C570.55,-18 573.17,-18 575.79,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"575.9,-21.5 585.9,-18 575.9,-14.5 575.9,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;description&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge5\" class=\"edge\">\n",
                             "<title>(&#39;description&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M395.3,-34.39C422.73,-42.01 456.91,-50.21 488.14,-54 581.68,-65.36 606.65,-65.75 700.14,-54 726.69,-50.66 755.4,-43.93 779.95,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"781.16,-40.47 789.84,-34.39 779.27,-33.73 781.16,-40.47\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M474.7,-34.49C507.75,-42.09 548.75,-50.23 585.99,-54 699.19,-65.46 728.84,-65.92 841.99,-54 874.15,-50.61 909.2,-43.69 939,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"939.96,-40.19 948.89,-34.49 938.35,-33.37 939.96,-40.19\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;implementation&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node5\" class=\"node\">\n",
                             "<title>(&#39;implementation&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1127.14\" cy=\"-18\" rx=\"144.87\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1127.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;implementation&#39;, &#39;NOUN&#39;) (0.0094)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1358.99\" cy=\"-18\" rx=\"178.97\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1358.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;implementation&#39;, &#39;NOUN&#39;) (0.0097)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;description&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implementation&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge6\" class=\"edge\">\n",
                             "<title>(&#39;description&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implementation&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M395.3,-34.39C422.73,-42.01 456.91,-50.21 488.14,-54 593.15,-66.75 858.99,-65.47 964.14,-54 995.07,-50.63 1028.72,-43.75 1057.37,-36.91\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1058.39,-40.26 1067.28,-34.49 1056.74,-33.46 1058.39,-40.26\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M474.7,-34.49C507.75,-42.09 548.75,-50.23 585.99,-54 713.34,-66.89 1034.51,-65.55 1161.99,-54 1199.81,-50.57 1241.21,-43.52 1276.26,-36.55\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1277.34,-39.91 1286.45,-34.5 1275.95,-33.05 1277.34,-39.91\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge7\" class=\"edge\">\n",
                             "<title>(&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M700.27,-18C702.88,-18 705.49,-18 708.1,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"708.16,-21.5 718.16,-18 708.16,-14.5 708.16,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M842.19,-18C844.51,-18 846.83,-18 849.15,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"849.33,-21.5 859.33,-18 849.33,-14.5 849.33,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;implementation&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge8\" class=\"edge\">\n",
                             "<title>(&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;implementation&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M639.11,-34.38C662.36,-42 691.4,-50.2 718.14,-54 826.39,-69.4 855.45,-65.86 964.14,-54 995.07,-50.63 1028.72,-43.75 1057.37,-36.91\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1058.39,-40.26 1067.28,-34.49 1056.74,-33.46 1058.39,-40.26\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M767.15,-34.39C794.58,-42.01 828.76,-50.21 859.99,-54 993.23,-70.18 1028.32,-66.11 1161.99,-54 1199.81,-50.57 1241.21,-43.52 1276.26,-36.55\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1277.34,-39.91 1286.45,-34.5 1275.95,-33.05 1277.34,-39.91\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node6\" class=\"node\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1391.14\" cy=\"-18\" rx=\"101.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1391.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;text&#39;, &#39;NOUN&#39;) (0.0151)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1679.99\" cy=\"-18\" rx=\"124.28\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1679.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;text&#39;, &#39;NOUN&#39;) (0.0157)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge9\" class=\"edge\">\n",
                             "<title>(&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M639.11,-34.38C662.36,-42 691.4,-50.2 718.14,-54 840.03,-71.34 1150.36,-72.02 1272.14,-54 1294.25,-50.73 1317.95,-44.21 1338.33,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1339.66,-40.86 1348.04,-34.38 1337.45,-34.22 1339.66,-40.86\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node15\" class=\"node\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3718.14\" cy=\"-18\" rx=\"126.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"3718.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;algorithm&#39;, &#39;PROPN&#39;) (0.0193)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge11\" class=\"edge\">\n",
-                            "<title>(&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M639.11,-34.38C662.36,-42 691.4,-50.2 718.14,-54 875.23,-76.34 3416.66,-73.39 3574.14,-54 3601.35,-50.65 3630.81,-43.87 3655.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3657.01,-40.42 3665.72,-34.39 3655.15,-33.68 3657.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M767.15,-34.39C794.58,-42.01 828.76,-50.21 859.99,-54 1009.56,-72.17 1388.48,-72.66 1537.99,-54 1564.84,-50.65 1593.89,-43.87 1618.68,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1619.63,-40.45 1628.32,-34.39 1617.74,-33.71 1619.63,-40.45\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node34\" class=\"node\">\n",
+                            "<g id=\"node33\" class=\"node\">\n",
                             "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13065.14\" cy=\"-18\" rx=\"127.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"13065.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;PageRank&#39;, &#39;PROPN&#39;) (0.0149)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13362.99\" cy=\"-18\" rx=\"155.17\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"13362.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;PageRank&#39;, &#39;PROPN&#39;) (0.0157)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"edge10\" class=\"edge\">\n",
                             "<title>(&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M639.11,-34.38C662.36,-42 691.4,-50.2 718.14,-54 885.91,-77.86 12750.92,-74.43 12919.14,-54 12946.71,-50.65 12976.58,-43.87 13002.07,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13003.25,-40.39 13011.98,-34.39 13001.41,-33.64 13003.25,-40.39\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M767.15,-34.39C794.58,-42.01 828.76,-50.21 859.99,-54 1029.99,-74.65 13019.64,-71.54 13189.99,-54 13222.89,-50.61 13258.76,-43.69 13289.27,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13290.43,-40.14 13299.4,-34.49 13288.87,-33.32 13290.43,-40.14\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Google&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node35\" class=\"node\">\n",
+                            "<g id=\"node34\" class=\"node\">\n",
                             "<title>(&#39;Google&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6351.14\" cy=\"-18\" rx=\"117.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"6351.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Google&#39;, &#39;PROPN&#39;) (0.0103)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13047.99\" cy=\"-18\" rx=\"141.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"13047.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Google&#39;, &#39;PROPN&#39;) (0.0103)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge12\" class=\"edge\">\n",
+                            "<g id=\"edge11\" class=\"edge\">\n",
                             "<title>(&#39;popular&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M639.11,-34.38C662.36,-42 691.4,-50.2 718.14,-54 869.34,-75.5 6064.71,-73.84 6216.14,-54 6241.5,-50.68 6268.87,-43.98 6292.29,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6293.47,-40.57 6302.07,-34.39 6291.49,-33.85 6293.47,-40.57\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M767.15,-34.39C794.58,-42.01 828.76,-50.21 859.99,-54 1025.84,-74.15 12722.95,-72.56 12888.99,-54 12919.05,-50.64 12951.72,-43.81 12979.59,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12980.77,-40.31 12989.62,-34.49 12979.07,-33.52 12980.77,-40.31\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implementation&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge13\" class=\"edge\">\n",
+                            "<g id=\"edge12\" class=\"edge\">\n",
                             "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implementation&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M964.03,-18C966.68,-18 969.33,-18 971.98,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"972.19,-21.5 982.19,-18 972.19,-14.5 972.19,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1162.56,-18C1165.04,-18 1167.52,-18 1170.01,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1170.21,-21.5 1180.21,-18 1170.21,-14.5 1170.21,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge14\" class=\"edge\">\n",
                             "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M892.44,-34.39C918.93,-42.01 951.94,-50.2 982.14,-54 1110.02,-70.07 1144.64,-72.86 1272.14,-54 1294.25,-50.73 1317.95,-44.21 1338.33,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1339.66,-40.86 1348.04,-34.38 1337.45,-34.22 1339.66,-40.86\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1338.23,-70.67 1380.1,-73.7 1537.99,-54 1564.84,-50.65 1593.89,-43.87 1618.68,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1619.63,-40.45 1628.32,-34.39 1617.74,-33.71 1619.63,-40.45\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node7\" class=\"node\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1652.14\" cy=\"-18\" rx=\"141.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1652.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;summarization&#39;, &#39;NOUN&#39;) (0.0214)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1996.99\" cy=\"-18\" rx=\"174.67\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1996.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;summarization&#39;, &#39;NOUN&#39;) (0.0221)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge15\" class=\"edge\">\n",
+                            "<g id=\"edge16\" class=\"edge\">\n",
                             "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M892.44,-34.39C918.93,-42.01 951.94,-50.2 982.14,-54 1094.59,-68.13 1379.5,-66.52 1492.14,-54 1522.52,-50.62 1555.55,-43.75 1583.67,-36.91\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1584.54,-40.3 1593.4,-34.49 1582.85,-33.5 1584.54,-40.3\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1317.89,-68.53 1665.91,-66.77 1803.99,-54 1841.06,-50.57 1881.63,-43.52 1915.96,-36.55\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1916.85,-39.94 1925.94,-34.5 1915.44,-33.09 1916.85,-39.94\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;base&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node15\" class=\"node\">\n",
+                            "<title>(&#39;base&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4454.99\" cy=\"-18\" rx=\"123.48\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"4454.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;base&#39;, &#39;VERB&#39;) (0.0124)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge13\" class=\"edge\">\n",
+                            "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1353.14,-72.24 4141.24,-75.71 4313.99,-54 4340.54,-50.66 4369.25,-43.93 4393.8,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4395.01,-40.47 4403.69,-34.39 4393.11,-33.73 4395.01,-40.47\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;weight&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node16\" class=\"node\">\n",
+                            "<title>(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4729.99\" cy=\"-18\" rx=\"133.78\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"4729.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;weight&#39;, &#39;VERB&#39;) (0.0144)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge15\" class=\"edge\">\n",
+                            "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1367.73,-73.77 4390.49,-75.9 4577.99,-54 4606.77,-50.64 4638.01,-43.81 4664.63,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4665.81,-40.31 4674.6,-34.39 4664.04,-33.54 4665.81,-40.31\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node50\" class=\"node\">\n",
+                            "<g id=\"node17\" class=\"node\">\n",
                             "<title>(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12573.14\" cy=\"-18\" rx=\"107.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"12573.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;graph&#39;, &#39;NOUN&#39;) (0.0110)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5014.99\" cy=\"-18\" rx=\"133.48\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"5014.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;graph&#39;, &#39;NOUN&#39;) (0.0213)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge16\" class=\"edge\">\n",
+                            "<g id=\"edge17\" class=\"edge\">\n",
                             "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M892.44,-34.39C918.93,-42.01 951.94,-50.2 982.14,-54 1140.14,-73.85 12289.44,-76.09 12447.14,-54 12470.68,-50.7 12496,-44.1 12517.72,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"12518.94,-40.72 12527.43,-34.38 12516.84,-34.05 12518.94,-40.72\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1383.53,-75.44 4660.72,-77.9 4863.99,-54 4892.47,-50.65 4923.36,-43.87 4949.74,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4950.83,-40.41 4959.62,-34.49 4949.05,-33.64 4950.83,-40.41\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;) -->\n",
+                            "<g id=\"edge18\" class=\"edge\">\n",
+                            "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1341.72,-71.03 12727.37,-72.07 12888.99,-54 12919.05,-50.64 12951.72,-43.81 12979.59,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12980.77,-40.31 12989.62,-34.49 12979.07,-33.52 12980.77,-40.31\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;use&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node35\" class=\"node\">\n",
+                            "<title>(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12193.99\" cy=\"-18\" rx=\"118.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"12193.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;use&#39;, &#39;VERB&#39;) (0.0146)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge19\" class=\"edge\">\n",
+                            "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1330.24,-69.83 11908.17,-73.49 12057.99,-54 12083.53,-50.68 12111.1,-43.98 12134.7,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12135.93,-40.55 12144.55,-34.39 12133.97,-33.83 12135.93,-40.55\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;rank&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node36\" class=\"node\">\n",
+                            "<title>(&#39;rank&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12452.99\" cy=\"-18\" rx=\"122.68\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"12452.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;rank&#39;, &#39;VERB&#39;) (0.0121)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge20\" class=\"edge\">\n",
+                            "<title>(&#39;algorithm&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1073.09,-34.49C1104.82,-42.08 1144.19,-50.23 1179.99,-54 1333.75,-70.2 12158.58,-73.27 12311.99,-54 12338.54,-50.66 12367.25,-43.93 12391.8,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12393.01,-40.47 12401.69,-34.39 12391.11,-33.73 12393.01,-40.47\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;implementation&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge17\" class=\"edge\">\n",
+                            "<g id=\"edge21\" class=\"edge\">\n",
                             "<title>(&#39;implementation&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1272.29,-18C1274.62,-18 1276.94,-18 1279.27,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1279.47,-21.5 1289.47,-18 1279.47,-14.5 1279.47,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1537.98,-18C1540.48,-18 1542.98,-18 1545.47,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1545.74,-21.5 1555.74,-18 1545.74,-14.5 1545.74,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;implementation&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge18\" class=\"edge\">\n",
+                            "<g id=\"edge22\" class=\"edge\">\n",
                             "<title>(&#39;implementation&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1187,-34.49C1217.59,-42.08 1255.57,-50.23 1290.14,-54 1379.39,-63.74 1402.91,-63.91 1492.14,-54 1522.52,-50.62 1555.55,-43.75 1583.67,-36.91\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1584.54,-40.3 1593.4,-34.49 1582.85,-33.5 1584.54,-40.3\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1431.53,-34.5C1468.56,-42.09 1514.44,-50.23 1555.99,-54 1665.76,-63.95 1694.24,-64.15 1803.99,-54 1841.06,-50.57 1881.63,-43.52 1915.96,-36.55\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1916.85,-39.94 1925.94,-34.5 1915.44,-33.09 1916.85,-39.94\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;exist&#39;, &#39;VERB&#39;) -->\n",
                             "<g id=\"node8\" class=\"node\">\n",
                             "<title>(&#39;exist&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1932.14\" cy=\"-18\" rx=\"102.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1932.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;exist&#39;, &#39;VERB&#39;) (0.0120)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2331.99\" cy=\"-18\" rx=\"124.28\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"2331.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;exist&#39;, &#39;VERB&#39;) (0.0125)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;implementation&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;exist&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge19\" class=\"edge\">\n",
+                            "<g id=\"edge23\" class=\"edge\">\n",
                             "<title>(&#39;implementation&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;exist&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1187,-34.49C1217.59,-42.08 1255.57,-50.23 1290.14,-54 1405.46,-66.58 1697.37,-70.84 1812.14,-54 1834.53,-50.71 1858.54,-44.15 1879.15,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1880.27,-40.84 1888.67,-34.38 1878.08,-34.19 1880.27,-40.84\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1431.53,-34.5C1468.56,-42.09 1514.44,-50.23 1555.99,-54 1696.3,-66.72 2050.19,-71.45 2189.99,-54 2216.84,-50.65 2245.89,-43.87 2270.68,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2271.63,-40.45 2280.32,-34.39 2269.74,-33.71 2271.63,-40.45\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge20\" class=\"edge\">\n",
+                            "<g id=\"edge24\" class=\"edge\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1492.58,-18C1495.08,-18 1497.58,-18 1500.08,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1500.35,-21.5 1510.35,-18 1500.35,-14.5 1500.35,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1804.44,-18C1806.92,-18 1809.41,-18 1811.89,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1812.11,-21.5 1822.11,-18 1812.11,-14.5 1812.11,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;exist&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge21\" class=\"edge\">\n",
+                            "<g id=\"edge25\" class=\"edge\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;exist&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1434.24,-34.38C1456.54,-41.99 1484.41,-50.19 1510.14,-54 1642.92,-73.64 1679.34,-73.49 1812.14,-54 1834.53,-50.71 1858.54,-44.15 1879.15,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1880.27,-40.84 1888.67,-34.38 1878.08,-34.19 1880.27,-40.84\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1731.66,-34.39C1758.34,-42.01 1791.58,-50.21 1821.99,-54 1984.29,-74.25 2027.69,-74.25 2189.99,-54 2216.84,-50.65 2245.89,-43.87 2270.68,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2271.63,-40.45 2280.32,-34.39 2269.74,-33.71 2271.63,-40.45\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;today&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node9\" class=\"node\">\n",
                             "<title>(&#39;today&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2161.14\" cy=\"-18\" rx=\"107.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"2161.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;today&#39;, &#39;NOUN&#39;) (0.0127)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2605.99\" cy=\"-18\" rx=\"131.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"2605.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;today&#39;, &#39;NOUN&#39;) (0.0132)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;today&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge22\" class=\"edge\">\n",
+                            "<g id=\"edge26\" class=\"edge\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;today&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1434.24,-34.38C1456.54,-41.99 1484.41,-50.19 1510.14,-54 1625.55,-71.07 1919.6,-70.18 2035.14,-54 2058.68,-50.7 2084,-44.1 2105.72,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2106.94,-40.72 2115.43,-34.38 2104.84,-34.05 2106.94,-40.72\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1731.66,-34.39C1758.34,-42.01 1791.58,-50.21 1821.99,-54 1961.79,-71.45 2316.08,-70.55 2455.99,-54 2484.41,-50.64 2515.23,-43.81 2541.51,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2542.57,-40.34 2551.34,-34.39 2540.78,-33.57 2542.57,-40.34\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;remove&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node45\" class=\"node\">\n",
+                            "<g id=\"node43\" class=\"node\">\n",
                             "<title>(&#39;remove&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15211.14\" cy=\"-18\" rx=\"113.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"15211.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;remove&#39;, &#39;VERB&#39;) (0.0097)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"18262.99\" cy=\"-18\" rx=\"136.48\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"18262.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;remove&#39;, &#39;VERB&#39;) (0.0102)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;remove&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge23\" class=\"edge\">\n",
+                            "<g id=\"edge27\" class=\"edge\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;remove&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1434.24,-34.38C1456.54,-41.99 1484.41,-50.19 1510.14,-54 1603.36,-67.79 14986.75,-66.6 15080.14,-54 15104.68,-50.69 15131.12,-44.04 15153.77,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15155.01,-40.63 15163.56,-34.39 15152.98,-33.93 15155.01,-40.63\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1731.66,-34.39C1758.34,-42.01 1791.58,-50.21 1821.99,-54 1934.22,-68.01 17996.63,-66.96 18108.99,-54 18138.14,-50.64 18169.79,-43.81 18196.78,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18197.68,-40.37 18206.49,-34.49 18195.94,-33.6 18197.68,-40.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;stop&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node46\" class=\"node\">\n",
+                            "<g id=\"node44\" class=\"node\">\n",
                             "<title>(&#39;stop&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15443.14\" cy=\"-18\" rx=\"100.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"15443.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;stop&#39;, &#39;VERB&#39;) (0.0109)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"18539.99\" cy=\"-18\" rx=\"122.38\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"18539.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;stop&#39;, &#39;VERB&#39;) (0.0115)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;stop&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge24\" class=\"edge\">\n",
+                            "<g id=\"edge28\" class=\"edge\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;stop&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1434.24,-34.38C1456.54,-41.99 1484.41,-50.19 1510.14,-54 1605.04,-68.04 15229.24,-68.04 15324.14,-54 15346.25,-50.73 15369.95,-44.21 15390.33,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15391.66,-40.86 15400.04,-34.38 15389.45,-34.22 15391.66,-40.86\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1731.66,-34.39C1758.34,-42.01 1791.58,-50.21 1821.99,-54 1936.22,-68.25 18284.77,-68.35 18398.99,-54 18425.54,-50.66 18454.25,-43.93 18478.8,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18480.01,-40.47 18488.69,-34.39 18478.11,-33.73 18480.01,-40.47\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;stem&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node47\" class=\"node\">\n",
+                            "<g id=\"node45\" class=\"node\">\n",
                             "<title>(&#39;stem&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15664.14\" cy=\"-18\" rx=\"102.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"15664.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;stem&#39;, &#39;VERB&#39;) (0.0137)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"18804.99\" cy=\"-18\" rx=\"124.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"18804.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;stem&#39;, &#39;VERB&#39;) (0.0144)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;stem&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge25\" class=\"edge\">\n",
+                            "<g id=\"edge29\" class=\"edge\">\n",
                             "<title>(&#39;text&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;stem&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1434.24,-34.38C1456.54,-41.99 1484.41,-50.19 1510.14,-54 1606.55,-68.26 15447.72,-68.15 15544.14,-54 15566.53,-50.71 15590.54,-44.15 15611.15,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15612.27,-40.84 15620.67,-34.38 15610.08,-34.19 15612.27,-40.84\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1731.66,-34.39C1758.34,-42.01 1791.58,-50.21 1821.99,-54 1938.03,-68.48 18545.93,-68.38 18661.99,-54 18689.02,-50.65 18718.27,-43.87 18743.24,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18744.24,-40.44 18752.94,-34.39 18742.37,-33.69 18744.24,-40.44\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge30\" class=\"edge\">\n",
+                            "<g id=\"edge34\" class=\"edge\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1786.7,-23.72C1801.95,-22.65 1811.83,-20.74 1811.83,-18 1811.83,-15.92 1806.15,-14.32 1796.77,-13.21\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1796.97,-9.71 1786.7,-12.28 1796.33,-16.68 1796.97,-9.71\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2163.61,-23.46C2179.66,-22.35 2189.82,-20.53 2189.82,-18 2189.82,-16.06 2183.86,-14.54 2173.87,-13.44\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2173.87,-9.93 2163.61,-12.54 2173.26,-16.9 2173.87,-9.93\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;exist&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge26\" class=\"edge\">\n",
+                            "<g id=\"edge30\" class=\"edge\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;exist&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1754.13,-5.5C1783.06,-3.98 1811.98,-4.19 1840.9,-6.14\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1840.9,-9.65 1851.13,-6.9 1841.42,-2.67 1840.9,-9.65\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2121.96,-5.37C2156.06,-3.97 2190.16,-4.26 2224.26,-6.22\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2224.16,-9.72 2234.36,-6.85 2224.6,-2.73 2224.16,-9.72\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;today&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge28\" class=\"edge\">\n",
+                            "<g id=\"edge32\" class=\"edge\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;today&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1725.44,-33.5C1756.36,-39.29 1792.85,-45.15 1826.14,-48 1920.02,-56.03 1944.59,-59.24 2038.14,-48 2058.03,-45.61 2079.34,-41.12 2098.54,-36.33\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2099.56,-39.68 2108.37,-33.81 2097.82,-32.9 2099.56,-39.68\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2085.25,-33.58C2122.13,-39.35 2165.51,-45.17 2204.99,-48 2317.59,-56.08 2346.67,-59.34 2458.99,-48 2483.25,-45.55 2509.43,-40.88 2532.88,-35.94\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2533.71,-39.34 2542.74,-33.81 2532.23,-32.5 2533.71,-39.34\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;module&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node10\" class=\"node\">\n",
                             "<title>(&#39;module&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2402.14\" cy=\"-18\" rx=\"115.08\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"2402.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;module&#39;, &#39;NOUN&#39;) (0.0141)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2895.99\" cy=\"-18\" rx=\"139.98\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"2895.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;module&#39;, &#39;NOUN&#39;) (0.0148)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;module&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge27\" class=\"edge\">\n",
+                            "<g id=\"edge31\" class=\"edge\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;module&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1715.57,-34.12C1749.09,-41.81 1791.08,-50.17 1829.14,-54 2023.71,-73.59 2075.29,-79.77 2269.14,-54 2294.14,-50.68 2321.11,-43.98 2344.19,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2345.24,-40.6 2353.82,-34.39 2343.24,-33.89 2345.24,-40.6\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2073.26,-34.21C2113.19,-41.89 2163,-50.19 2207.99,-54 2442.7,-73.88 2503.91,-80.33 2737.99,-54 2767.87,-50.64 2800.34,-43.81 2828.03,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2829.15,-40.32 2838,-34.49 2827.45,-33.53 2829.15,-40.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;gensim&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node11\" class=\"node\">\n",
                             "<title>(&#39;gensim&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2649.14\" cy=\"-18\" rx=\"113.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"2649.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;gensim&#39;, &#39;NOUN&#39;) (0.0147)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3192.99\" cy=\"-18\" rx=\"139.98\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"3192.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;gensim&#39;, &#39;NOUN&#39;) (0.0154)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;gensim&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge29\" class=\"edge\">\n",
+                            "<g id=\"edge33\" class=\"edge\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;gensim&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1715.57,-34.12C1749.09,-41.81 1791.08,-50.17 1829.14,-54 1981.26,-69.31 2365.61,-74.29 2517.14,-54 2541.85,-50.69 2568.49,-44.04 2591.32,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2592.62,-40.62 2601.19,-34.39 2590.61,-33.91 2592.62,-40.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2073.26,-34.21C2113.19,-41.89 2163,-50.19 2207.99,-54 2391.33,-69.53 2853.16,-74.69 3035.99,-54 3065.69,-50.64 3097.95,-43.81 3125.46,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3126.53,-40.33 3135.37,-34.49 3124.82,-33.55 3126.53,-40.33\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;implement&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"node12\" class=\"node\">\n",
                             "<title>(&#39;implement&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"2907.14\" cy=\"-18\" rx=\"126.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"2907.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;implement&#39;, &#39;NOUN&#39;) (0.0153)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3505.99\" cy=\"-18\" rx=\"155.17\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"3505.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;implement&#39;, &#39;NOUN&#39;) (0.0160)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implement&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge31\" class=\"edge\">\n",
+                            "<g id=\"edge35\" class=\"edge\">\n",
                             "<title>(&#39;summarization&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implement&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1715.57,-34.12C1749.09,-41.81 1791.08,-50.17 1829.14,-54 2035.65,-74.79 2557.14,-79.36 2763.14,-54 2790.35,-50.65 2819.81,-43.87 2844.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2846.01,-40.42 2854.72,-34.39 2844.15,-33.68 2846.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2073.26,-34.21C2113.19,-41.89 2163,-50.19 2207.99,-54 2457.1,-75.1 3084.3,-79.6 3332.99,-54 3365.89,-50.61 3401.76,-43.69 3432.27,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3433.43,-40.14 3442.4,-34.49 3431.87,-33.32 3433.43,-40.14\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;exist&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge33\" class=\"edge\">\n",
+                            "<g id=\"edge37\" class=\"edge\">\n",
                             "<title>(&#39;exist&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1851.13,-29.1C1822.21,-31.45 1793.29,-32.08 1764.36,-30.97\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1764.28,-27.46 1754.13,-30.5 1763.96,-34.45 1764.28,-27.46\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2234.36,-29.15C2200.26,-31.44 2166.16,-32.06 2132.06,-30.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2132.08,-27.49 2121.96,-30.63 2131.83,-34.49 2132.08,-27.49\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;exist&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;today&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge32\" class=\"edge\">\n",
+                            "<g id=\"edge36\" class=\"edge\">\n",
                             "<title>(&#39;exist&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;today&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2035.01,-18C2037.67,-18 2040.33,-18 2042.99,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2043.24,-21.5 2053.24,-18 2043.24,-14.5 2043.24,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2456.15,-18C2458.75,-18 2461.35,-18 2463.96,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2464,-21.5 2474,-18 2464,-14.5 2464,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;exist&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;module&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge34\" class=\"edge\">\n",
+                            "<g id=\"edge38\" class=\"edge\">\n",
                             "<title>(&#39;exist&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;module&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1975.99,-34.38C1998.67,-42 2027.01,-50.19 2053.14,-54 2148.14,-67.83 2173.98,-66.65 2269.14,-54 2294.14,-50.68 2321.11,-43.98 2344.19,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2345.24,-40.6 2353.82,-34.39 2343.24,-33.89 2345.24,-40.6\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2383.66,-34.39C2410.34,-42.01 2443.58,-50.21 2473.99,-54 2590.42,-68.53 2621.39,-67.12 2737.99,-54 2767.87,-50.64 2800.34,-43.81 2828.03,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2829.15,-40.32 2838,-34.49 2827.45,-33.53 2829.15,-40.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;today&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge35\" class=\"edge\">\n",
+                            "<g id=\"edge39\" class=\"edge\">\n",
                             "<title>(&#39;today&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;summarization&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2120.7,-34.8C2095.68,-44.28 2062.61,-55.16 2032.14,-60 1944.35,-73.93 1920.45,-70.17 1832.14,-60 1793.84,-55.59 1751.85,-46.07 1718.06,-37.21\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1718.87,-33.8 1708.31,-34.61 1717.07,-40.56 1718.87,-33.8\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2557.76,-34.81C2527.98,-44.3 2488.75,-55.18 2452.99,-60 2346.4,-74.36 2318.04,-70.41 2210.99,-60 2165.21,-55.55 2114.69,-45.87 2074.23,-36.92\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2074.96,-33.49 2064.44,-34.72 2073.43,-40.32 2074.96,-33.49\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;today&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;module&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge36\" class=\"edge\">\n",
+                            "<g id=\"edge40\" class=\"edge\">\n",
                             "<title>(&#39;today&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;module&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2269.4,-18C2271.88,-18 2274.36,-18 2276.84,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2277.03,-21.5 2287.03,-18 2277.03,-14.5 2277.03,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2737.96,-18C2740.62,-18 2743.27,-18 2745.93,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"2746.17,-21.5 2756.17,-18 2746.17,-14.5 2746.17,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;today&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;gensim&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge37\" class=\"edge\">\n",
+                            "<g id=\"edge41\" class=\"edge\">\n",
                             "<title>(&#39;today&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;gensim&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2206.85,-34.38C2230.48,-42 2259.99,-50.2 2287.14,-54 2388.38,-68.18 2415.82,-67.57 2517.14,-54 2541.85,-50.69 2568.49,-44.04 2591.32,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2592.62,-40.62 2601.19,-34.39 2590.61,-33.91 2592.62,-40.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2660.64,-34.39C2688.83,-42.01 2723.94,-50.21 2755.99,-54 2879.57,-68.62 2912.33,-68 3035.99,-54 3065.69,-50.64 3097.95,-43.81 3125.46,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3126.53,-40.33 3135.37,-34.49 3124.82,-33.55 3126.53,-40.33\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;module&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;gensim&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge38\" class=\"edge\">\n",
+                            "<g id=\"edge42\" class=\"edge\">\n",
                             "<title>(&#39;module&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;gensim&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2517.44,-18C2519.94,-18 2522.43,-18 2524.93,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2525.19,-21.5 2535.19,-18 2525.19,-14.5 2525.19,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3035.79,-18C3038.12,-18 3040.45,-18 3042.77,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3042.98,-21.5 3052.98,-18 3042.98,-14.5 3042.98,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;module&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implement&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge39\" class=\"edge\">\n",
+                            "<g id=\"edge43\" class=\"edge\">\n",
                             "<title>(&#39;module&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implement&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2450.46,-34.39C2475.43,-42 2506.57,-50.2 2535.14,-54 2635.59,-67.35 2662.57,-66.38 2763.14,-54 2790.35,-50.65 2819.81,-43.87 2844.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2846.01,-40.42 2854.72,-34.39 2844.15,-33.68 2846.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2953.61,-34.49C2983.06,-42.08 3019.65,-50.23 3052.99,-54 3176.64,-68 3209.2,-66.74 3332.99,-54 3365.89,-50.61 3401.76,-43.69 3432.27,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3433.43,-40.14 3442.4,-34.49 3431.87,-33.32 3433.43,-40.14\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"node13\" class=\"node\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3178.14\" cy=\"-18\" rx=\"126.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"3178.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;TextRank&#39;, &#39;PROPN&#39;) (0.0190)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3832.99\" cy=\"-18\" rx=\"153.27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"3832.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;TextRank&#39;, &#39;PROPN&#39;) (0.0199)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;module&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge40\" class=\"edge\">\n",
+                            "<g id=\"edge44\" class=\"edge\">\n",
                             "<title>(&#39;module&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2450.46,-34.39C2475.43,-42 2506.57,-50.2 2535.14,-54 2645.06,-68.61 2924.08,-67.55 3034.14,-54 3061.35,-50.65 3090.81,-43.87 3115.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3117.01,-40.42 3125.72,-34.39 3115.15,-33.68 3117.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M2953.61,-34.49C2983.06,-42.08 3019.65,-50.23 3052.99,-54 3187.24,-69.2 3526.6,-67.91 3660.99,-54 3693.71,-50.61 3729.37,-43.69 3759.7,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3760.81,-40.15 3769.77,-34.49 3759.24,-33.33 3760.81,-40.15\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;gensim&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implement&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge41\" class=\"edge\">\n",
+                            "<g id=\"edge45\" class=\"edge\">\n",
                             "<title>(&#39;gensim&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;implement&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2763.02,-18C2765.35,-18 2767.67,-18 2770,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"2770.19,-21.5 2780.19,-18 2770.19,-14.5 2770.19,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3332.98,-18C3335.45,-18 3337.93,-18 3340.4,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3340.55,-21.5 3350.55,-18 3340.55,-14.5 3340.55,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;gensim&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge42\" class=\"edge\">\n",
+                            "<g id=\"edge46\" class=\"edge\">\n",
                             "<title>(&#39;gensim&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2696.72,-34.39C2721.3,-42 2751.98,-50.2 2780.14,-54 2892.02,-69.09 2922.1,-67.79 3034.14,-54 3061.35,-50.65 3090.81,-43.87 3115.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3117.01,-40.42 3125.72,-34.39 3115.15,-33.68 3117.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3250.98,-34.49C3280.63,-42.08 3317.44,-50.23 3350.99,-54 3487.9,-69.4 3523.94,-68.19 3660.99,-54 3693.71,-50.61 3729.37,-43.69 3759.7,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3760.81,-40.15 3769.77,-34.49 3759.24,-33.33 3760.81,-40.15\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;unsupervised&#39;, &#39;ADJ&#39;) -->\n",
                             "<g id=\"node14\" class=\"node\">\n",
                             "<title>(&#39;unsupervised&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3448.14\" cy=\"-18\" rx=\"126.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"3448.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;unsupervised&#39;, &#39;ADJ&#39;) (0.0144)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4158.99\" cy=\"-18\" rx=\"154.87\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"4158.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;unsupervised&#39;, &#39;ADJ&#39;) (0.0148)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;gensim&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;unsupervised&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge43\" class=\"edge\">\n",
+                            "<g id=\"edge47\" class=\"edge\">\n",
                             "<title>(&#39;gensim&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;unsupervised&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2696.72,-34.39C2721.3,-42 2751.98,-50.2 2780.14,-54 2895.54,-69.57 3188.57,-68.23 3304.14,-54 3331.35,-50.65 3360.81,-43.87 3385.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3387.01,-40.42 3395.72,-34.39 3385.15,-33.68 3387.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3250.98,-34.49C3280.63,-42.08 3317.44,-50.23 3350.99,-54 3491.22,-69.77 3845.62,-68.45 3985.99,-54 4018.89,-50.61 4054.76,-43.69 4085.27,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4086.43,-40.14 4095.4,-34.49 4084.87,-33.32 4086.43,-40.14\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge50\" class=\"edge\">\n",
+                            "<title>(&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3442.4,-34.49C3409.91,-42.08 3369.61,-50.23 3332.99,-54 3214.01,-66.25 1298.94,-66.53 1179.99,-54 1147.83,-50.61 1112.78,-43.69 1082.98,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1083.63,-33.37 1073.09,-34.49 1082.02,-40.19 1083.63,-33.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge44\" class=\"edge\">\n",
+                            "<g id=\"edge48\" class=\"edge\">\n",
                             "<title>(&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3033.91,-18C3036.54,-18 3039.17,-18 3041.8,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3041.94,-21.5 3051.94,-18 3041.94,-14.5 3041.94,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3661.51,-18C3664.14,-18 3666.78,-18 3669.42,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3669.59,-21.5 3679.59,-18 3669.59,-14.5 3669.59,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;unsupervised&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge45\" class=\"edge\">\n",
+                            "<g id=\"edge49\" class=\"edge\">\n",
                             "<title>(&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;unsupervised&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2959.93,-34.39C2987.17,-42.01 3021.12,-50.21 3052.14,-54 3163.31,-67.59 3192.98,-67.68 3304.14,-54 3331.35,-50.65 3360.81,-43.87 3385.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3387.01,-40.42 3395.72,-34.39 3385.15,-33.68 3387.01,-40.42\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3569.96,-34.49C3602.63,-42.08 3643.16,-50.23 3679.99,-54 3815.28,-67.85 3850.7,-67.93 3985.99,-54 4018.89,-50.61 4054.76,-43.69 4085.27,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4086.43,-40.14 4095.4,-34.49 4084.87,-33.32 4086.43,-40.14\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge46\" class=\"edge\">\n",
-                            "<title>(&#39;implement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M2959.93,-34.39C2987.17,-42.01 3021.12,-50.21 3052.14,-54 3167.28,-68.08 3459.01,-68.17 3574.14,-54 3601.35,-50.65 3630.81,-43.87 3655.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3657.01,-40.42 3665.72,-34.39 3655.15,-33.68 3657.01,-40.42\"/>\n",
+                            "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge52\" class=\"edge\">\n",
+                            "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3769.77,-34.49C3737.47,-42.08 3697.4,-50.23 3660.99,-54 3523.89,-68.19 1317.06,-68.44 1179.99,-54 1147.83,-50.61 1112.78,-43.69 1082.98,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1083.63,-33.37 1073.09,-34.49 1082.02,-40.19 1083.63,-33.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;unsupervised&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge47\" class=\"edge\">\n",
+                            "<g id=\"edge51\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;unsupervised&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3304.44,-18C3306.89,-18 3309.33,-18 3311.78,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3311.84,-21.5 3321.84,-18 3311.84,-14.5 3311.84,-21.5\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge48\" class=\"edge\">\n",
-                            "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3433.3,-67.68 3462.98,-67.68 3574.14,-54 3601.35,-50.65 3630.81,-43.87 3655.95,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3657.01,-40.42 3665.72,-34.39 3655.15,-33.68 3657.01,-40.42\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;base&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node16\" class=\"node\">\n",
-                            "<title>(&#39;base&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"3963.14\" cy=\"-18\" rx=\"101.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"3963.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;base&#39;, &#39;VERB&#39;) (0.0127)</text>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3986.44,-18C3989.04,-18 3991.65,-18 3994.25,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3994.3,-21.5 4004.3,-18 3994.3,-14.5 3994.3,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge49\" class=\"edge\">\n",
+                            "<g id=\"edge53\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3437.27,-68.17 3729.39,-70.98 3844.14,-54 3866.25,-50.73 3889.95,-44.21 3910.33,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3911.66,-40.86 3920.04,-34.38 3909.45,-34.22 3911.66,-40.86\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;use&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node36\" class=\"node\">\n",
-                            "<title>(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6584.14\" cy=\"-18\" rx=\"97.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"6584.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;use&#39;, &#39;VERB&#39;) (0.0148)</text>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4141.03,-68.27 4177.29,-71.18 4313.99,-54 4340.54,-50.66 4369.25,-43.93 4393.8,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4395.01,-40.47 4403.69,-34.39 4393.11,-33.73 4395.01,-40.47\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge53\" class=\"edge\">\n",
+                            "<g id=\"edge59\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3495.66,-75.36 6296.32,-80.42 6469.14,-54 6490.46,-50.74 6513.26,-44.27 6532.88,-37.7\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6534.22,-40.94 6542.54,-34.38 6531.94,-34.32 6534.22,-40.94\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4115.25,-65.58 11947.06,-68.43 12057.99,-54 12083.53,-50.68 12111.1,-43.98 12134.7,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12135.93,-40.55 12144.55,-34.39 12133.97,-33.83 12135.93,-40.55\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;work&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node38\" class=\"node\">\n",
+                            "<title>(&#39;work&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"17705.99\" cy=\"-18\" rx=\"124.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"17705.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;work&#39;, &#39;VERB&#39;) (0.0059)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;work&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge54\" class=\"edge\">\n",
+                            "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;work&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4191.3,-73.5 17376.1,-77.16 17562.99,-54 17590.02,-50.65 17619.27,-43.87 17644.24,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"17645.24,-40.44 17653.94,-34.39 17643.37,-33.69 17645.24,-40.44\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;follow&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node39\" class=\"node\">\n",
+                            "<title>(&#39;follow&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"17978.99\" cy=\"-18\" rx=\"129.98\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"17978.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;follow&#39;, &#39;VERB&#39;) (0.0109)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;follow&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge55\" class=\"edge\">\n",
+                            "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;follow&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4195,-73.89 17640.31,-76.86 17830.99,-54 17859.04,-50.64 17889.46,-43.81 17915.38,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"17916.33,-40.37 17925.08,-34.39 17914.52,-33.6 17916.33,-40.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node52\" class=\"node\">\n",
+                            "<g id=\"node50\" class=\"node\">\n",
                             "<title>(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9688.14\" cy=\"-18\" rx=\"118.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"9688.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;sentence&#39;, &#39;NOUN&#39;) (0.0830)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7620.99\" cy=\"-18\" rx=\"147.57\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"7620.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;sentence&#39;, &#39;NOUN&#39;) (0.0889)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge52\" class=\"edge\">\n",
+                            "<g id=\"edge58\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3493.87,-75.14 9379.54,-76.17 9551.14,-54 9576.97,-50.66 9604.88,-43.93 9628.72,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9629.7,-40.53 9638.33,-34.39 9627.75,-33.81 9629.7,-40.53\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4194.68,-73.86 7264.36,-74.43 7454.99,-54 7486.46,-50.63 7520.73,-43.75 7549.91,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7551.1,-40.22 7560.01,-34.49 7549.47,-33.41 7551.1,-40.22\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;edge&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node55\" class=\"node\">\n",
+                            "<g id=\"node53\" class=\"node\">\n",
                             "<title>(&#39;edge&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10159.14\" cy=\"-18\" rx=\"104.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"10159.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;edge&#39;, &#39;NOUN&#39;) (0.0399)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8184.99\" cy=\"-18\" rx=\"128.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"8184.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;edge&#39;, &#39;NOUN&#39;) (0.0421)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge51\" class=\"edge\">\n",
+                            "<g id=\"edge57\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3414.71,-65.4 9944.84,-67.33 10037.14,-54 10059.88,-50.72 10084.28,-44.16 10105.24,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10106.49,-40.8 10114.92,-34.38 10104.33,-34.14 10106.49,-40.8\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4115.47,-65.61 7927.72,-67.52 8038.99,-54 8066.56,-50.65 8096.43,-43.87 8121.92,-37.09\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8123.1,-40.39 8131.83,-34.39 8121.26,-33.64 8123.1,-40.39\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node56\" class=\"node\">\n",
+                            "<g id=\"node54\" class=\"node\">\n",
                             "<title>(&#39;weight&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10619.14\" cy=\"-18\" rx=\"112.38\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"10619.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;weight&#39;, &#39;NOUN&#39;) (0.0071)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15956.99\" cy=\"-18\" rx=\"137.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"15956.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;weight&#39;, &#39;NOUN&#39;) (0.0071)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;weight&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge50\" class=\"edge\">\n",
+                            "<g id=\"edge56\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;weight&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3420.92,-66.16 10389.51,-67.31 10488.14,-54 10512.68,-50.69 10539.12,-44.04 10561.77,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10563.01,-40.63 10571.56,-34.39 10560.98,-33.93 10563.01,-40.63\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4166.96,-70.97 15638.19,-72.54 15800.99,-54 15830.63,-50.62 15862.83,-43.75 15890.24,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"15891.28,-40.26 15900.11,-34.39 15889.56,-33.47 15891.28,-40.26\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Okapi&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node67\" class=\"node\">\n",
+                            "<g id=\"node65\" class=\"node\">\n",
                             "<title>(&#39;Okapi&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7291.14\" cy=\"-18\" rx=\"113.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"7291.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Okapi&#39;, &#39;PROPN&#39;) (0.0096)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11322.99\" cy=\"-18\" rx=\"136.48\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"11322.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Okapi&#39;, &#39;PROPN&#39;) (0.0096)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Okapi&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge54\" class=\"edge\">\n",
+                            "<g id=\"edge60\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Okapi&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3427.95,-67.03 7054.49,-68.25 7160.14,-54 7184.68,-50.69 7211.12,-44.04 7233.77,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7235.01,-40.63 7243.56,-34.39 7232.98,-33.93 7235.01,-40.63\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4201.95,-74.61 10971.27,-76.8 11168.99,-54 11198.14,-50.64 11229.79,-43.81 11256.78,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11257.68,-40.37 11266.49,-34.49 11255.94,-33.6 11257.68,-40.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;BM25&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node68\" class=\"node\">\n",
+                            "<g id=\"node66\" class=\"node\">\n",
                             "<title>(&#39;BM25&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11603.14\" cy=\"-18\" rx=\"113.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"11603.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;BM25&#39;, &#39;PROPN&#39;) (0.0112)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11614.99\" cy=\"-18\" rx=\"137.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"11614.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;BM25&#39;, &#39;PROPN&#39;) (0.0111)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;BM25&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge55\" class=\"edge\">\n",
+                            "<g id=\"edge61\" class=\"edge\">\n",
                             "<title>(&#39;TextRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;BM25&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3230.56,-34.39C3257.61,-42.01 3291.32,-50.21 3322.14,-54 3434.47,-67.83 11358.96,-69.02 11471.14,-54 11495.85,-50.69 11522.49,-44.04 11545.32,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11546.62,-40.62 11555.19,-34.39 11544.61,-33.91 11546.62,-40.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M3895.84,-34.49C3927.94,-42.08 3967.78,-50.23 4003.99,-54 4209.96,-75.45 11253.24,-77.43 11458.99,-54 11488.63,-50.62 11520.83,-43.75 11548.24,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11549.28,-40.26 11558.11,-34.39 11547.56,-33.47 11549.28,-40.26\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge56\" class=\"edge\">\n",
-                            "<title>(&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3574.44,-18C3576.89,-18 3579.33,-18 3581.78,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3581.84,-21.5 3591.84,-18 3581.84,-14.5 3581.84,-21.5\"/>\n",
+                            "<!-- (&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge62\" class=\"edge\">\n",
+                            "<title>(&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4095.4,-34.49C4062.91,-42.08 4022.61,-50.23 3985.99,-54 3830.92,-69.96 1335.02,-70.33 1179.99,-54 1147.83,-50.61 1112.78,-43.69 1082.98,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1083.63,-33.37 1073.09,-34.49 1082.02,-40.19 1083.63,-33.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge57\" class=\"edge\">\n",
+                            "<g id=\"edge63\" class=\"edge\">\n",
                             "<title>(&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3500.56,-34.39C3527.61,-42.01 3561.32,-50.21 3592.14,-54 3703.3,-67.68 3733.35,-70.39 3844.14,-54 3866.25,-50.73 3889.95,-44.21 3910.33,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3911.66,-40.86 3920.04,-34.38 3909.45,-34.22 3911.66,-40.86\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;weight&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node17\" class=\"node\">\n",
-                            "<title>(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4193.14\" cy=\"-18\" rx=\"110.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"4193.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;weight&#39;, &#39;VERB&#39;) (0.0146)</text>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4313.93,-18C4316.37,-18 4318.81,-18 4321.25,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4321.28,-21.5 4331.28,-18 4321.28,-14.5 4321.28,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge58\" class=\"edge\">\n",
-                            "<title>(&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3500.56,-34.39C3527.61,-42.01 3561.32,-50.21 3592.14,-54 3696.24,-66.82 3960.22,-68.23 4064.14,-54 4088.32,-50.69 4114.36,-44.04 4136.67,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4137.78,-40.67 4146.31,-34.39 4135.72,-33.98 4137.78,-40.67\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge59\" class=\"edge\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;base&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3844.47,-18C3846.79,-18 3849.11,-18 3851.44,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3851.62,-21.5 3861.62,-18 3851.62,-14.5 3851.62,-21.5\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge60\" class=\"edge\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3770.56,-34.39C3797.61,-42.01 3831.32,-50.21 3862.14,-54 3951.25,-64.97 3975.19,-66.18 4064.14,-54 4088.32,-50.69 4114.36,-44.04 4136.67,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4137.78,-40.67 4146.31,-34.39 4135.72,-33.98 4137.78,-40.67\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;graphs&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node18\" class=\"node\">\n",
-                            "<title>(&#39;graphs&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4433.14\" cy=\"-18\" rx=\"111.58\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"4433.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;graphs&#39;, &#39;NOUN&#39;) (0.0146)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;graphs&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge61\" class=\"edge\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;graphs&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3770.56,-34.39C3797.61,-42.01 3831.32,-50.21 3862.14,-54 3959.41,-65.97 4206.03,-67.2 4303.14,-54 4327.5,-50.69 4353.74,-44.04 4376.22,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4377.39,-40.65 4385.94,-34.39 4375.35,-33.96 4377.39,-40.65\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge62\" class=\"edge\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3770.56,-34.39C3797.61,-42.01 3831.32,-50.21 3862.14,-54 3991.94,-69.98 6086.47,-70.99 6216.14,-54 6241.5,-50.68 6268.87,-43.98 6292.29,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6293.47,-40.57 6302.07,-34.39 6291.49,-33.85 6293.47,-40.57\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge63\" class=\"edge\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3770.56,-34.39C3797.61,-42.01 3831.32,-50.21 3862.14,-54 4005.89,-71.7 6325.97,-75.89 6469.14,-54 6490.46,-50.74 6513.26,-44.27 6532.88,-37.7\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6534.22,-40.94 6542.54,-34.38 6531.94,-34.32 6534.22,-40.94\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;rank&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node37\" class=\"node\">\n",
-                            "<title>(&#39;rank&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6801.14\" cy=\"-18\" rx=\"101.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"6801.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;rank&#39;, &#39;VERB&#39;) (0.0123)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;) -->\n",
                             "<g id=\"edge64\" class=\"edge\">\n",
-                            "<title>(&#39;algorithm&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M3770.56,-34.39C3797.61,-42.01 3831.32,-50.21 3862.14,-54 4017.58,-73.14 6526.19,-76.74 6681.14,-54 6703.62,-50.7 6727.73,-44.1 6748.41,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6749.55,-40.75 6757.95,-34.29 6747.36,-34.1 6749.55,-40.75\"/>\n",
+                            "<title>(&#39;unsupervised&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4222.58,-34.49C4255.07,-42.08 4295.37,-50.23 4331.99,-54 4440.75,-65.2 4469.39,-66.68 4577.99,-54 4606.77,-50.64 4638.01,-43.81 4664.63,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4665.81,-40.31 4674.6,-34.39 4664.04,-33.54 4665.81,-40.31\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;) -->\n",
                             "<g id=\"edge65\" class=\"edge\">\n",
                             "<title>(&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;weight&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4064.66,-18C4067.26,-18 4069.86,-18 4072.46,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4072.48,-21.5 4082.48,-18 4072.48,-14.5 4072.48,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4578.52,-18C4580.98,-18 4583.43,-18 4585.89,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4585.98,-21.5 4595.98,-18 4585.98,-14.5 4585.98,-21.5\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graphs&#39;, &#39;NOUN&#39;) -->\n",
+                            "<!-- (&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge66\" class=\"edge\">\n",
-                            "<title>(&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graphs&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4006.33,-34.29C4028.87,-41.93 4057.1,-50.18 4083.14,-54 4179.88,-68.2 4206.25,-67.17 4303.14,-54 4327.5,-50.69 4353.74,-44.04 4376.22,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4377.39,-40.65 4385.94,-34.39 4375.35,-33.96 4377.39,-40.65\"/>\n",
+                            "<title>(&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4506.29,-34.39C4532.77,-42.01 4565.78,-50.2 4595.99,-54 4714.17,-68.85 4745.69,-67.91 4863.99,-54 4892.47,-50.65 4923.36,-43.87 4949.74,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4950.83,-40.41 4959.62,-34.49 4949.05,-33.64 4950.83,-40.41\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;paper&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node19\" class=\"node\">\n",
+                            "<g id=\"node18\" class=\"node\">\n",
                             "<title>(&#39;paper&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4671.14\" cy=\"-18\" rx=\"107.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"4671.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;paper&#39;, &#39;NOUN&#39;) (0.0172)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5298.99\" cy=\"-18\" rx=\"132.68\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"5298.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;paper&#39;, &#39;NOUN&#39;) (0.0162)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge67\" class=\"edge\">\n",
                             "<title>(&#39;base&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4006.33,-34.29C4028.87,-41.93 4057.1,-50.18 4083.14,-54 4184.72,-68.91 4443.47,-68.24 4545.14,-54 4568.68,-50.7 4594,-44.1 4615.72,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4616.94,-40.72 4625.43,-34.38 4614.84,-34.05 4616.94,-40.72\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4506.29,-34.39C4532.77,-42.01 4565.78,-50.2 4595.99,-54 4717.7,-69.29 5026.16,-68.32 5147.99,-54 5176.59,-50.64 5207.62,-43.81 5234.07,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5235.19,-40.32 5243.97,-34.39 5233.41,-33.55 5235.19,-40.32\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graphs&#39;, &#39;NOUN&#39;) -->\n",
+                            "<!-- (&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge68\" class=\"edge\">\n",
-                            "<title>(&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graphs&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4303.77,-18C4306.22,-18 4308.67,-18 4311.12,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4311.2,-21.5 4321.2,-18 4311.2,-14.5 4311.2,-21.5\"/>\n",
+                            "<title>(&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4864.14,-18C4866.58,-18 4869.03,-18 4871.47,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"4871.52,-21.5 4881.52,-18 4871.52,-14.5 4871.52,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge69\" class=\"edge\">\n",
                             "<title>(&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4239.6,-34.39C4263.61,-42 4293.59,-50.2 4321.14,-54 4419.76,-67.6 4446.55,-67.81 4545.14,-54 4568.68,-50.7 4594,-44.1 4615.72,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4616.94,-40.72 4625.43,-34.38 4614.84,-34.05 4616.94,-40.72\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4785.38,-34.39C4813.95,-42.01 4849.53,-50.21 4881.99,-54 4999.41,-67.72 5030.58,-67.8 5147.99,-54 5176.59,-50.64 5207.62,-43.81 5234.07,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5235.19,-40.32 5243.97,-34.39 5233.41,-33.55 5235.19,-40.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Mihalcea&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node20\" class=\"node\">\n",
+                            "<g id=\"node19\" class=\"node\">\n",
                             "<title>(&#39;Mihalcea&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"4921.14\" cy=\"-18\" rx=\"124.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"4921.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Mihalcea&#39;, &#39;PROPN&#39;) (0.0148)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5600.99\" cy=\"-18\" rx=\"151.37\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"5600.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Mihalcea&#39;, &#39;PROPN&#39;) (0.0138)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"edge70\" class=\"edge\">\n",
                             "<title>(&#39;weight&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4239.6,-34.39C4263.61,-42 4293.59,-50.2 4321.14,-54 4421.96,-67.91 4678.15,-66.6 4779.14,-54 4805.99,-50.65 4835.04,-43.87 4859.83,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4860.78,-40.45 4869.47,-34.39 4858.89,-33.71 4860.78,-40.45\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M4785.38,-34.39C4813.95,-42.01 4849.53,-50.21 4881.99,-54 5003.39,-68.18 5310.44,-66.8 5431.99,-54 5464.15,-50.61 5499.2,-43.69 5529,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5529.96,-40.19 5538.89,-34.49 5528.35,-33.37 5529.96,-40.19\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;graphs&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;) -->\n",
+                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge71\" class=\"edge\">\n",
-                            "<title>(&#39;graphs&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4545.17,-18C4547.66,-18 4550.15,-18 4552.64,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4552.88,-21.5 4562.88,-18 4552.88,-14.5 4552.88,-21.5\"/>\n",
+                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5148.39,-18C5151.01,-18 5153.63,-18 5156.24,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5156.33,-21.5 5166.33,-18 5156.33,-14.5 5156.33,-21.5\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;graphs&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;) -->\n",
+                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"edge72\" class=\"edge\">\n",
-                            "<title>(&#39;graphs&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4480.35,-34.39C4504.74,-42 4535.18,-50.2 4563.14,-54 4658.27,-66.93 4683.88,-65.89 4779.14,-54 4805.99,-50.65 4835.04,-43.87 4859.83,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4860.78,-40.45 4869.47,-34.39 4858.89,-33.71 4860.78,-40.45\"/>\n",
+                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5070.36,-34.49C5098.68,-42.08 5133.87,-50.22 5165.99,-54 5283.4,-67.8 5314.42,-66.38 5431.99,-54 5464.15,-50.61 5499.2,-43.69 5529,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5529.96,-40.19 5538.89,-34.49 5528.35,-33.37 5529.96,-40.19\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;et&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node21\" class=\"node\">\n",
+                            "<g id=\"node20\" class=\"node\">\n",
                             "<title>(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5160.14\" cy=\"-18\" rx=\"96.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"5160.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;et&#39;, &#39;PROPN&#39;) (0.0228)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5888.99\" cy=\"-18\" rx=\"118.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"5888.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;et&#39;, &#39;PROPN&#39;) (0.0224)</text>\n",
                             "</g>\n",
-                            "<!-- (&#39;graphs&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;) -->\n",
+                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"edge73\" class=\"edge\">\n",
-                            "<title>(&#39;graphs&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4480.35,-34.39C4504.74,-42 4535.18,-50.2 4563.14,-54 4669.28,-68.42 4939.26,-70.19 5045.14,-54 5066.55,-50.73 5089.45,-44.22 5109.13,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5110.49,-40.85 5118.81,-34.28 5108.21,-34.23 5110.49,-40.85\"/>\n",
+                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5070.36,-34.49C5098.68,-42.08 5133.87,-50.22 5165.99,-54 5295.32,-69.2 5622.84,-70.69 5751.99,-54 5777.82,-50.66 5805.73,-43.93 5829.57,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5830.55,-40.53 5839.18,-34.39 5828.6,-33.81 5830.55,-40.53\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;) -->\n",
+                            "<!-- (&#39;vertex&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"node48\" class=\"node\">\n",
+                            "<title>(&#39;vertex&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7074.99\" cy=\"-18\" rx=\"135.68\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"7074.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;vertex&#39;, &#39;NOUN&#39;) (0.0086)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;vertex&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge74\" class=\"edge\">\n",
+                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;vertex&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5070.36,-34.49C5098.68,-42.08 5133.87,-50.22 5165.99,-54 5359.66,-76.77 6727.27,-76.34 6920.99,-54 6950.26,-50.62 6982.06,-43.75 7009.11,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7010.05,-40.28 7018.85,-34.39 7008.3,-33.5 7010.05,-40.28\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;be&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"node49\" class=\"node\">\n",
+                            "<title>(&#39;be&#39;, &#39;VERB&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7341.99\" cy=\"-18\" rx=\"113.18\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"7341.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;be&#39;, &#39;VERB&#39;) (0.0123)</text>\n",
+                            "</g>\n",
+                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;be&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge75\" class=\"edge\">\n",
+                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;be&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5070.36,-34.49C5098.68,-42.08 5133.87,-50.22 5165.99,-54 5278.82,-67.26 7098.4,-69.19 7210.99,-54 7235.53,-50.69 7261.96,-44.04 7284.62,-37.35\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7285.85,-40.63 7294.41,-34.39 7283.83,-33.93 7285.85,-40.63\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge76\" class=\"edge\">\n",
+                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5070.36,-34.49C5098.68,-42.08 5133.87,-50.22 5165.99,-54 5292.29,-68.85 7328.55,-67.55 7454.99,-54 7486.46,-50.63 7520.73,-43.75 7549.91,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7551.1,-40.22 7560.01,-34.49 7549.47,-33.41 7551.1,-40.22\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;) -->\n",
+                            "<g id=\"edge77\" class=\"edge\">\n",
                             "<title>(&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mihalcea&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4779.05,-18C4781.55,-18 4784.05,-18 4786.54,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4786.81,-21.5 4796.81,-18 4786.81,-14.5 4786.81,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5431.7,-18C5434.17,-18 5436.63,-18 5439.1,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5439.23,-21.5 5449.23,-18 5439.23,-14.5 5439.23,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge75\" class=\"edge\">\n",
+                            "<g id=\"edge78\" class=\"edge\">\n",
                             "<title>(&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4716.85,-34.38C4740.48,-42 4769.99,-50.2 4797.14,-54 4906.3,-69.29 4936.18,-70.66 5045.14,-54 5066.55,-50.73 5089.45,-44.22 5109.13,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5110.49,-40.85 5118.81,-34.28 5108.21,-34.23 5110.49,-40.85\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5354.01,-34.39C5382.39,-42.01 5417.74,-50.21 5449.99,-54 5583.29,-69.67 5618.87,-71.2 5751.99,-54 5777.82,-50.66 5805.73,-43.93 5829.57,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5830.55,-40.53 5839.18,-34.39 5828.6,-33.81 5830.55,-40.53\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;al&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node22\" class=\"node\">\n",
+                            "<g id=\"node21\" class=\"node\">\n",
                             "<title>(&#39;al&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5372.14\" cy=\"-18\" rx=\"96.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"5372.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;al&#39;, &#39;PROPN&#39;) (0.0304)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6143.99\" cy=\"-18\" rx=\"118.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"6143.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;al&#39;, &#39;PROPN&#39;) (0.0372)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge76\" class=\"edge\">\n",
+                            "<g id=\"edge79\" class=\"edge\">\n",
                             "<title>(&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4716.85,-34.38C4740.48,-42 4769.99,-50.2 4797.14,-54 4898.38,-68.18 5156.09,-69.45 5257.14,-54 5278.55,-50.73 5301.45,-44.22 5321.13,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5322.49,-40.85 5330.81,-34.28 5320.21,-34.23 5322.49,-40.85\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5354.01,-34.39C5382.39,-42.01 5417.74,-50.21 5449.99,-54 5573.14,-68.48 5885.03,-70 6007.99,-54 6033.53,-50.68 6061.1,-43.98 6084.7,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"6085.93,-40.55 6094.55,-34.39 6083.97,-33.83 6085.93,-40.55\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Barrios&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node71\" class=\"node\">\n",
+                            "<g id=\"node69\" class=\"node\">\n",
                             "<title>(&#39;Barrios&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5809.14\" cy=\"-18\" rx=\"117.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"5809.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Barrios&#39;, &#39;PROPN&#39;) (0.0077)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6423.99\" cy=\"-18\" rx=\"143.77\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"6423.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Barrios&#39;, &#39;PROPN&#39;) (0.0079)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Barrios&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge77\" class=\"edge\">\n",
+                            "<g id=\"edge80\" class=\"edge\">\n",
                             "<title>(&#39;paper&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Barrios&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4716.85,-34.38C4740.48,-42 4769.99,-50.2 4797.14,-54 4893.53,-67.5 5576.62,-66.56 5673.14,-54 5698.68,-50.68 5726.25,-43.98 5749.85,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5751.08,-40.55 5759.7,-34.39 5749.12,-33.83 5751.08,-40.55\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5354.01,-34.39C5382.39,-42.01 5417.74,-50.21 5449.99,-54 5629.2,-75.07 6082.62,-73.69 6261.99,-54 6292.73,-50.63 6326.18,-43.75 6354.65,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"6355.62,-40.27 6364.5,-34.49 6353.96,-33.47 6355.62,-40.27\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Mihalcea&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge78\" class=\"edge\">\n",
+                            "<g id=\"edge81\" class=\"edge\">\n",
                             "<title>(&#39;Mihalcea&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5045.31,-18C5047.93,-18 5050.54,-18 5053.16,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5053.25,-21.5 5063.25,-18 5053.25,-14.5 5053.25,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5752.58,-18C5755.02,-18 5757.45,-18 5759.89,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5759.9,-21.5 5769.9,-18 5759.9,-14.5 5759.9,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Mihalcea&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge79\" class=\"edge\">\n",
+                            "<g id=\"edge82\" class=\"edge\">\n",
                             "<title>(&#39;Mihalcea&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M4972.82,-34.39C4999.49,-42.01 5032.73,-50.21 5063.14,-54 5148.7,-64.68 5171.91,-67.03 5257.14,-54 5278.55,-50.73 5301.45,-44.22 5321.13,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5322.49,-40.85 5330.81,-34.28 5320.21,-34.23 5322.49,-40.85\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M5663.09,-34.49C5694.82,-42.08 5734.19,-50.23 5769.99,-54 5875.19,-65.08 5903.1,-67.65 6007.99,-54 6033.53,-50.68 6061.1,-43.98 6084.7,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"6085.93,-40.55 6094.55,-34.39 6083.97,-33.83 6085.93,-40.55\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;et&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge80\" class=\"edge\">\n",
+                            "<g id=\"edge83\" class=\"edge\">\n",
                             "<title>(&#39;et&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5257.03,-18C5259.65,-18 5262.28,-18 5264.9,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5265.02,-21.5 5275.02,-18 5265.02,-14.5 5265.02,-21.5\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;.&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node72\" class=\"node\">\n",
-                            "<title>(&#39;.&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"5580.14\" cy=\"-18\" rx=\"92.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"5580.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;.&#39;, &#39;PROPN&#39;) (0.0386)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;et&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;.&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge81\" class=\"edge\">\n",
-                            "<title>(&#39;et&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;.&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5201.48,-34.28C5223.06,-41.92 5250.12,-50.17 5275.14,-54 5360.37,-67.03 5383.98,-67.47 5469.14,-54 5489.76,-50.74 5511.76,-44.27 5530.7,-37.71\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5532.05,-40.94 5540.29,-34.28 5529.7,-34.35 5532.05,-40.94\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;al&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;.&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge82\" class=\"edge\">\n",
-                            "<title>(&#39;al&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;.&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5469.24,-18C5471.73,-18 5474.23,-18 5476.73,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5477,-21.5 5487,-18 5477,-14.5 5477,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M6008.02,-18C6010.49,-18 6012.95,-18 6015.42,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"6015.55,-21.5 6025.55,-18 6015.55,-14.5 6015.55,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;add&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node23\" class=\"node\">\n",
+                            "<g id=\"node22\" class=\"node\">\n",
                             "<title>(&#39;add&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9452.14\" cy=\"-18\" rx=\"98.58\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"9452.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;add&#39;, &#39;VERB&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11049.99\" cy=\"-18\" rx=\"118.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"11049.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;add&#39;, &#39;VERB&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;incubator&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node24\" class=\"node\">\n",
+                            "<g id=\"node23\" class=\"node\">\n",
                             "<title>(&#39;incubator&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8719.14\" cy=\"-18\" rx=\"122.38\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"8719.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;incubator&#39;, &#39;NOUN&#39;) (0.0053)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10160.99\" cy=\"-18\" rx=\"150.27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"10160.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;incubator&#39;, &#39;NOUN&#39;) (0.0056)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;add&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;incubator&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge83\" class=\"edge\">\n",
+                            "<g id=\"edge84\" class=\"edge\">\n",
                             "<title>(&#39;add&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;incubator&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9410.16,-34.38C9388.44,-41.99 9361.26,-50.19 9336.14,-54 9231.34,-69.89 8964.3,-67.3 8859.14,-54 8832.77,-50.66 8804.26,-43.93 8779.89,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8780.65,-33.75 8770.07,-34.39 8778.74,-40.48 8780.65,-33.75\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11000.18,-34.39C10974.45,-42 10942.38,-50.2 10912.99,-54 10784.28,-70.63 10458.05,-67.67 10328.99,-54 10297.01,-50.61 10262.17,-43.69 10232.55,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10233.25,-33.39 10222.72,-34.49 10231.64,-40.2 10233.25,-33.39\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;student&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node25\" class=\"node\">\n",
+                            "<g id=\"node24\" class=\"node\">\n",
                             "<title>(&#39;student&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8973.14\" cy=\"-18\" rx=\"113.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"8973.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;student&#39;, &#39;NOUN&#39;) (0.0068)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10470.99\" cy=\"-18\" rx=\"141.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"10470.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;student&#39;, &#39;NOUN&#39;) (0.0072)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;add&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;student&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge84\" class=\"edge\">\n",
+                            "<g id=\"edge85\" class=\"edge\">\n",
                             "<title>(&#39;add&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;student&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9410.16,-34.38C9388.44,-41.99 9361.26,-50.19 9336.14,-54 9234.2,-69.46 9206.33,-67.79 9104.14,-54 9079.61,-50.69 9053.17,-44.04 9030.51,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9031.3,-33.93 9020.72,-34.39 9029.28,-40.63 9031.3,-33.93\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11000.18,-34.39C10974.45,-42 10942.38,-50.2 10912.99,-54 10788.69,-70.06 10755.56,-67.84 10630.99,-54 10600.61,-50.62 10567.58,-43.75 10539.46,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10540.28,-33.5 10529.73,-34.49 10538.59,-40.3 10540.28,-33.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Olavur&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node26\" class=\"node\">\n",
+                            "<g id=\"node25\" class=\"node\">\n",
                             "<title>(&#39;Olavur&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9220.14\" cy=\"-18\" rx=\"115.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"9220.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Olavur&#39;, &#39;PROPN&#39;) (0.0087)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10771.99\" cy=\"-18\" rx=\"141.07\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"10771.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Olavur&#39;, &#39;PROPN&#39;) (0.0092)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;add&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;Olavur&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge85\" class=\"edge\">\n",
+                            "<g id=\"edge86\" class=\"edge\">\n",
                             "<title>(&#39;add&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;Olavur&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9352.91,-18C9350.72,-18 9348.54,-18 9346.36,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9346.14,-14.5 9336.14,-18 9346.14,-21.5 9346.14,-14.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10930.8,-18C10928.32,-18 10925.84,-18 10923.36,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10923.16,-14.5 10913.16,-18 10923.16,-21.5 10923.16,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;incubator&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;student&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge86\" class=\"edge\">\n",
+                            "<g id=\"edge87\" class=\"edge\">\n",
                             "<title>(&#39;incubator&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;student&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8841.68,-18C8844.17,-18 8846.66,-18 8849.15,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8849.39,-21.5 8859.39,-18 8849.39,-14.5 8849.39,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10311.15,-18C10313.79,-18 10316.43,-18 10319.07,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10319.25,-21.5 10329.25,-18 10319.25,-14.5 10319.25,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;incubator&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Olavur&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge87\" class=\"edge\">\n",
+                            "<g id=\"edge88\" class=\"edge\">\n",
                             "<title>(&#39;incubator&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Olavur&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8770.07,-34.39C8796.36,-42.01 8829.14,-50.2 8859.14,-54 8959.67,-66.72 8986.69,-67.35 9087.14,-54 9112.14,-50.68 9139.11,-43.98 9162.19,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9163.24,-40.6 9171.82,-34.39 9161.24,-33.89 9163.24,-40.6\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10222.72,-34.49C10254.26,-42.08 10293.39,-50.23 10328.99,-54 10454.51,-67.3 10487.55,-68.02 10612.99,-54 10643.05,-50.64 10675.72,-43.81 10703.59,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10704.77,-40.31 10713.62,-34.49 10703.07,-33.52 10704.77,-40.31\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Mortensen&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node27\" class=\"node\">\n",
+                            "<g id=\"node26\" class=\"node\">\n",
                             "<title>(&#39;Mortensen&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8449.14\" cy=\"-18\" rx=\"129.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"8449.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Mortensen&#39;, &#39;PROPN&#39;) (0.0100)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9832.99\" cy=\"-18\" rx=\"159.77\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"9832.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Mortensen&#39;, &#39;PROPN&#39;) (0.0106)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;incubator&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mortensen&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge88\" class=\"edge\">\n",
+                            "<g id=\"edge89\" class=\"edge\">\n",
                             "<title>(&#39;incubator&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mortensen&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8596.72,-18C8594.08,-18 8591.44,-18 8588.79,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8588.6,-14.5 8578.6,-18 8588.6,-21.5 8588.6,-14.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10010.85,-18C10008.36,-18 10005.87,-18 10003.38,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10003.15,-14.5 9993.15,-18 10003.15,-21.5 10003.15,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;student&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Olavur&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge89\" class=\"edge\">\n",
+                            "<g id=\"edge90\" class=\"edge\">\n",
                             "<title>(&#39;student&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Olavur&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9086.99,-18C9089.44,-18 9091.89,-18 9094.34,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9094.42,-21.5 9104.42,-18 9094.42,-14.5 9094.42,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10612.97,-18C10615.45,-18 10617.94,-18 10620.43,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"10620.67,-21.5 10630.67,-18 10620.67,-14.5 10620.67,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;student&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mortensen&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge90\" class=\"edge\">\n",
+                            "<g id=\"edge91\" class=\"edge\">\n",
                             "<title>(&#39;student&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Mortensen&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8925.19,-34.39C8900.42,-42 8869.51,-50.2 8841.14,-54 8733.66,-68.39 8704.81,-66.91 8597.14,-54 8569.09,-50.64 8538.67,-43.81 8512.75,-37\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8513.61,-33.6 8503.05,-34.39 8511.8,-40.37 8513.61,-33.6\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10412.25,-34.49C10382.23,-42.08 10344.95,-50.23 10310.99,-54 10178.47,-68.72 10143.66,-67.28 10010.99,-54 9977.02,-50.6 9939.94,-43.63 9908.46,-36.73\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9908.97,-33.26 9898.45,-34.49 9907.45,-40.09 9908.97,-33.26\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node28\" class=\"node\">\n",
+                            "<g id=\"node27\" class=\"node\">\n",
                             "<title>(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7519.14\" cy=\"-18\" rx=\"96.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"7519.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;see&#39;, &#39;VERB&#39;) (0.0208)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8714.99\" cy=\"-18\" rx=\"117.78\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"8714.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;see&#39;, &#39;VERB&#39;) (0.0215)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;student&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge91\" class=\"edge\">\n",
+                            "<g id=\"edge92\" class=\"edge\">\n",
                             "<title>(&#39;student&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8925.19,-34.39C8900.42,-42 8869.51,-50.2 8841.14,-54 8708.22,-71.8 7766.71,-74.27 7634.14,-54 7612.73,-50.73 7589.84,-44.22 7570.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7571.07,-34.23 7560.48,-34.28 7568.79,-40.85 7571.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10412.25,-34.49C10382.23,-42.08 10344.95,-50.23 10310.99,-54 10149.76,-71.91 9011.86,-74.93 8850.99,-54 8825.45,-50.68 8797.88,-43.98 8774.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8775.01,-33.83 8764.43,-34.39 8773.05,-40.55 8775.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Olavur&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Mortensen&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge92\" class=\"edge\">\n",
+                            "<g id=\"edge93\" class=\"edge\">\n",
                             "<title>(&#39;Olavur&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Mortensen&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9171.82,-34.39C9146.86,-42 9115.71,-50.2 9087.14,-54 8979.2,-68.35 8705.26,-66.96 8597.14,-54 8569.09,-50.64 8538.67,-43.81 8512.75,-37\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8513.61,-33.6 8503.05,-34.39 8511.8,-40.37 8513.61,-33.6\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10713.62,-34.49C10683.79,-42.08 10646.74,-50.23 10612.99,-54 10480.04,-68.86 10144.1,-67.33 10010.99,-54 9977.02,-50.6 9939.94,-43.63 9908.46,-36.73\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9908.97,-33.26 9898.45,-34.49 9907.45,-40.09 9908.97,-33.26\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Olavur&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge93\" class=\"edge\">\n",
+                            "<g id=\"edge94\" class=\"edge\">\n",
                             "<title>(&#39;Olavur&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9171.82,-34.39C9146.86,-42 9115.71,-50.2 9087.14,-54 8927.1,-75.28 7793.73,-78.4 7634.14,-54 7612.73,-50.73 7589.84,-44.22 7570.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7571.07,-34.23 7560.48,-34.28 7568.79,-40.85 7571.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10713.62,-34.49C10683.79,-42.08 10646.74,-50.23 10612.99,-54 10418.42,-75.75 9045.13,-79.26 8850.99,-54 8825.45,-50.68 8797.88,-43.98 8774.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8775.01,-33.83 8764.43,-34.39 8773.05,-40.55 8775.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;previous&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"node29\" class=\"node\">\n",
+                            "<g id=\"node28\" class=\"node\">\n",
                             "<title>(&#39;previous&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7743.14\" cy=\"-18\" rx=\"109.38\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"7743.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;previous&#39;, &#39;ADJ&#39;) (0.0130)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8982.99\" cy=\"-18\" rx=\"131.88\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"8982.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;previous&#39;, &#39;ADJ&#39;) (0.0136)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;Olavur&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;previous&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge94\" class=\"edge\">\n",
+                            "<g id=\"edge95\" class=\"edge\">\n",
                             "<title>(&#39;Olavur&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;previous&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9171.82,-34.39C9146.86,-42 9115.71,-50.2 9087.14,-54 8953.1,-71.82 8004.08,-72.62 7870.14,-54 7846.42,-50.7 7820.91,-44.1 7799.01,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7799.82,-34.02 7789.23,-34.38 7797.73,-40.7 7799.82,-34.02\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M10713.62,-34.49C10683.79,-42.08 10646.74,-50.23 10612.99,-54 10449.56,-72.27 9296.29,-73.32 9132.99,-54 9104.57,-50.64 9073.75,-43.81 9047.47,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9048.2,-33.57 9037.64,-34.39 9046.41,-40.34 9048.2,-33.57\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Mortensen&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge95\" class=\"edge\">\n",
+                            "<g id=\"edge96\" class=\"edge\">\n",
                             "<title>(&#39;Mortensen&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8395.61,-34.39C8367.99,-42.01 8333.57,-50.21 8302.14,-54 8154.77,-71.78 7780.88,-76.43 7634.14,-54 7612.73,-50.73 7589.84,-44.22 7570.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7571.07,-34.23 7560.48,-34.28 7568.79,-40.85 7571.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M9767.53,-34.49C9734.1,-42.09 9692.64,-50.23 9654.99,-54 9477.21,-71.8 9028.16,-77.05 8850.99,-54 8825.45,-50.68 8797.88,-43.98 8774.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8775.01,-33.83 8764.43,-34.39 8773.05,-40.55 8775.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Mortensen&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;previous&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge96\" class=\"edge\">\n",
+                            "<g id=\"edge97\" class=\"edge\">\n",
                             "<title>(&#39;Mortensen&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;previous&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8395.61,-34.39C8367.99,-42.01 8333.57,-50.21 8302.14,-54 8206.83,-65.5 7965.23,-67.22 7870.14,-54 7846.42,-50.7 7820.91,-44.1 7799.01,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7799.82,-34.02 7789.23,-34.38 7797.73,-40.7 7799.82,-34.02\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M9767.53,-34.49C9734.1,-42.09 9692.64,-50.23 9654.99,-54 9539.57,-65.56 9248.19,-67.63 9132.99,-54 9104.57,-50.64 9073.75,-43.81 9047.47,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9048.2,-33.57 9037.64,-34.39 9046.41,-40.34 9048.2,-33.57\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;post&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node30\" class=\"node\">\n",
+                            "<g id=\"node29\" class=\"node\">\n",
                             "<title>(&#39;post&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7973.14\" cy=\"-18\" rx=\"102.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"7973.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;post&#39;, &#39;NOUN&#39;) (0.0160)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9258.99\" cy=\"-18\" rx=\"126.18\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"9258.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;post&#39;, &#39;NOUN&#39;) (0.0168)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;Mortensen&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;post&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge97\" class=\"edge\">\n",
+                            "<g id=\"edge98\" class=\"edge\">\n",
                             "<title>(&#39;Mortensen&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;post&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8395.61,-34.39C8367.99,-42.01 8333.57,-50.21 8302.14,-54 8210.36,-65.07 8185.62,-67.32 8094.14,-54 8071.58,-50.71 8047.37,-44.16 8026.59,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8027.58,-34.17 8016.99,-34.38 8025.4,-40.82 8027.58,-34.17\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M9767.53,-34.49C9734.1,-42.09 9692.64,-50.23 9654.99,-54 9543.55,-65.16 9514.15,-67.68 9402.99,-54 9375.78,-50.65 9346.32,-43.87 9321.18,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9321.98,-33.68 9311.41,-34.39 9320.12,-40.42 9321.98,-33.68\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;previous&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge98\" class=\"edge\">\n",
+                            "<g id=\"edge99\" class=\"edge\">\n",
                             "<title>(&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;previous&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7616.27,-18C7618.71,-18 7621.14,-18 7623.58,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7623.61,-21.5 7633.61,-18 7623.61,-14.5 7623.61,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8832.76,-18C8835.42,-18 8838.07,-18 8840.72,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8840.95,-21.5 8850.95,-18 8840.95,-14.5 8840.95,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;post&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge99\" class=\"edge\">\n",
+                            "<g id=\"edge100\" class=\"edge\">\n",
                             "<title>(&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;post&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7560.48,-34.28C7582.06,-41.92 7609.12,-50.17 7634.14,-54 7729.92,-68.64 7756.26,-67.96 7852.14,-54 7874.7,-50.71 7898.91,-44.16 7919.7,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7920.88,-40.82 7929.3,-34.38 7918.7,-34.17 7920.88,-40.82\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8764.43,-34.39C8789.96,-42 8821.8,-50.2 8850.99,-54 8967.34,-69.14 8998.54,-68.34 9114.99,-54 9142.2,-50.65 9171.66,-43.87 9196.8,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9197.86,-40.42 9206.57,-34.39 9196,-33.68 9197.86,-40.42\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;blog&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node31\" class=\"node\">\n",
+                            "<g id=\"node30\" class=\"node\">\n",
                             "<title>(&#39;blog&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8198.14\" cy=\"-18\" rx=\"103.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"8198.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;blog&#39;, &#39;NOUN&#39;) (0.0268)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9528.99\" cy=\"-18\" rx=\"126.18\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"9528.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;blog&#39;, &#39;NOUN&#39;) (0.0281)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;blog&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge100\" class=\"edge\">\n",
+                            "<g id=\"edge101\" class=\"edge\">\n",
                             "<title>(&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;blog&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7560.48,-34.28C7582.06,-41.92 7609.12,-50.17 7634.14,-54 7731.24,-68.84 7978.93,-68.04 8076.14,-54 8098.88,-50.72 8123.28,-44.16 8144.24,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8145.49,-40.8 8153.92,-34.38 8143.33,-34.14 8145.49,-40.8\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8764.43,-34.39C8789.96,-42 8821.8,-50.2 8850.99,-54 8968.66,-69.31 9267.21,-68.5 9384.99,-54 9412.2,-50.65 9441.66,-43.87 9466.8,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9467.86,-40.42 9476.57,-34.39 9466,-33.68 9467.86,-40.42\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge102\" class=\"edge\">\n",
+                            "<g id=\"edge103\" class=\"edge\">\n",
                             "<title>(&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7560.48,-34.28C7582.06,-41.92 7609.12,-50.17 7634.14,-54 7739.42,-70.09 9445.52,-67.65 9551.14,-54 9576.97,-50.66 9604.88,-43.93 9628.72,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9629.7,-40.53 9638.33,-34.39 9627.75,-33.81 9629.7,-40.53\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8665.55,-34.39C8640.02,-42 8608.17,-50.2 8578.99,-54 8408.43,-76.19 7976.19,-70.59 7804.99,-54 7769.17,-50.53 7729.97,-43.34 7696.99,-36.29\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7697.48,-32.82 7686.96,-34.12 7695.99,-39.66 7697.48,-32.82\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;similar&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"node57\" class=\"node\">\n",
+                            "<g id=\"node55\" class=\"node\">\n",
                             "<title>(&#39;similar&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10385.14\" cy=\"-18\" rx=\"103.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"10385.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;similar&#39;, &#39;ADJ&#39;) (0.0221)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"8454.99\" cy=\"-18\" rx=\"124.28\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"8454.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;similar&#39;, &#39;ADJ&#39;) (0.0229)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge101\" class=\"edge\">\n",
+                            "<g id=\"edge102\" class=\"edge\">\n",
                             "<title>(&#39;see&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7560.48,-34.28C7582.06,-41.92 7609.12,-50.17 7634.14,-54 7778.57,-76.08 10119.55,-75.05 10264.14,-54 10286.7,-50.71 10310.91,-44.16 10331.7,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10332.88,-40.82 10341.3,-34.38 10330.7,-34.17 10332.88,-40.82\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8597.19,-18C8594.56,-18 8591.93,-18 8589.3,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8589.15,-14.5 8579.15,-18 8589.15,-21.5 8589.15,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;previous&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;post&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge103\" class=\"edge\">\n",
+                            "<g id=\"edge104\" class=\"edge\">\n",
                             "<title>(&#39;previous&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;post&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7852.75,-18C7855.2,-18 7857.64,-18 7860.09,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7860.15,-21.5 7870.15,-18 7860.15,-14.5 7860.15,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M9115.06,-18C9117.55,-18 9120.04,-18 9122.53,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9122.77,-21.5 9132.77,-18 9122.77,-14.5 9122.77,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;previous&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;blog&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge104\" class=\"edge\">\n",
+                            "<g id=\"edge105\" class=\"edge\">\n",
                             "<title>(&#39;previous&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;blog&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7789.23,-34.38C7813.05,-42 7842.79,-50.2 7870.14,-54 7960.83,-66.6 7985.53,-67.09 8076.14,-54 8098.88,-50.72 8123.28,-44.16 8144.24,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8145.49,-40.8 8153.92,-34.38 8143.33,-34.14 8145.49,-40.8\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M9037.64,-34.39C9065.83,-42.01 9100.94,-50.21 9132.99,-54 9244.21,-67.16 9273.83,-67.68 9384.99,-54 9412.2,-50.65 9441.66,-43.87 9466.8,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9467.86,-40.42 9476.57,-34.39 9466,-33.68 9467.86,-40.42\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;post&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;blog&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge105\" class=\"edge\">\n",
+                            "<g id=\"edge106\" class=\"edge\">\n",
                             "<title>(&#39;post&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;blog&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M8075.97,-18C8078.62,-18 8081.26,-18 8083.91,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"8084.11,-21.5 8094.11,-18 8084.11,-14.5 8084.11,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M9385.29,-18C9387.74,-18 9390.18,-18 9392.63,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"9392.69,-21.5 9402.69,-18 9392.69,-14.5 9392.69,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;build&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node32\" class=\"node\">\n",
+                            "<g id=\"node31\" class=\"node\">\n",
                             "<title>(&#39;build&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14291.14\" cy=\"-18\" rx=\"103.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"14291.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;build&#39;, &#39;VERB&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14853.99\" cy=\"-18\" rx=\"125.38\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"14853.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;build&#39;, &#39;VERB&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;build&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge107\" class=\"edge\">\n",
+                            "<g id=\"edge108\" class=\"edge\">\n",
                             "<title>(&#39;build&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14246.92,-34.38C14224.05,-42 14195.48,-50.2 14169.14,-54 14076.69,-67.36 810.62,-67.15 718.14,-54 694.95,-50.7 670.03,-44.1 648.66,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"649.7,-34.09 639.11,-34.38 647.57,-40.76 649.7,-34.09\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14801.94,-34.39C14775.08,-42.01 14741.6,-50.21 14710.99,-54 14520.08,-77.66 1050.96,-77.2 859.99,-54 832.42,-50.65 802.55,-43.87 777.06,-37.09\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"777.72,-33.64 767.15,-34.39 775.88,-40.39 777.72,-33.64\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;top&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node33\" class=\"node\">\n",
+                            "<g id=\"node32\" class=\"node\">\n",
                             "<title>(&#39;top&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14512.14\" cy=\"-18\" rx=\"99.38\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"14512.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;top&#39;, &#39;NOUN&#39;) (0.0053)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15117.99\" cy=\"-18\" rx=\"120.78\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"15117.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;top&#39;, &#39;NOUN&#39;) (0.0056)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;build&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;top&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge106\" class=\"edge\">\n",
+                            "<g id=\"edge107\" class=\"edge\">\n",
                             "<title>(&#39;build&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;top&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14395.17,-18C14397.61,-18 14400.05,-18 14402.49,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"14402.53,-21.5 14412.53,-18 14402.53,-14.5 14402.53,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14979.54,-18C14981.98,-18 14984.41,-18 14986.85,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"14986.85,-21.5 14996.85,-18 14986.85,-14.5 14986.85,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;build&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge108\" class=\"edge\">\n",
+                            "<g id=\"edge109\" class=\"edge\">\n",
                             "<title>(&#39;build&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14246.92,-34.38C14224.05,-42 14195.48,-50.2 14169.14,-54 14063.68,-69.24 13315.91,-66.93 13210.14,-54 13182.75,-50.65 13153.09,-43.87 13127.77,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13128.5,-33.66 13117.93,-34.39 13126.65,-40.41 13128.5,-33.66\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14801.94,-34.39C14775.08,-42.01 14741.6,-50.21 14710.99,-54 14581.43,-70.06 13665.86,-67.37 13535.99,-54 13503.09,-50.61 13467.22,-43.69 13436.71,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13437.11,-33.32 13426.58,-34.49 13435.55,-40.14 13437.11,-33.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge109\" class=\"edge\">\n",
+                            "<g id=\"edge110\" class=\"edge\">\n",
                             "<title>(&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;popular&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14469.79,-34.38C14447.87,-41.99 14420.47,-50.19 14395.14,-54 14301.22,-68.12 812.17,-67.37 718.14,-54 694.95,-50.7 670.03,-44.1 648.66,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"649.7,-34.09 639.11,-34.38 647.57,-40.76 649.7,-34.09\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15067.43,-34.39C15041.33,-42.01 15008.79,-50.2 14978.99,-54 14881.73,-66.39 957.32,-65.82 859.99,-54 832.42,-50.65 802.55,-43.87 777.06,-37.09\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"777.72,-33.64 767.15,-34.39 775.88,-40.39 777.72,-33.64\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge111\" class=\"edge\">\n",
-                            "<title>(&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14469.79,-34.38C14447.87,-41.99 14420.47,-50.19 14395.14,-54 14250.48,-75.75 4007.34,-71.87 3862.14,-54 3834.93,-50.65 3805.47,-43.87 3780.33,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3781.13,-33.68 3770.56,-34.39 3779.27,-40.42 3781.13,-33.68\"/>\n",
+                            "<!-- (&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge112\" class=\"edge\">\n",
+                            "<title>(&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15067.43,-34.39C15041.33,-42.01 15008.79,-50.2 14978.99,-54 14788.87,-78.22 1370.59,-74.08 1179.99,-54 1147.83,-50.61 1112.78,-43.69 1082.98,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1083.63,-33.37 1073.09,-34.49 1082.02,-40.19 1083.63,-33.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge110\" class=\"edge\">\n",
+                            "<g id=\"edge111\" class=\"edge\">\n",
                             "<title>(&#39;top&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14469.79,-34.38C14447.87,-41.99 14420.47,-50.19 14395.14,-54 14264.94,-73.58 13340.83,-69.98 13210.14,-54 13182.75,-50.65 13153.09,-43.87 13127.77,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13128.5,-33.66 13117.93,-34.39 13126.65,-40.41 13128.5,-33.66\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15067.43,-34.39C15041.33,-42.01 15008.79,-50.2 14978.99,-54 14819.94,-74.26 13695.48,-70.42 13535.99,-54 13503.09,-50.61 13467.22,-43.69 13436.71,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13437.11,-33.32 13426.58,-34.49 13435.55,-40.14 13437.11,-33.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge115\" class=\"edge\">\n",
+                            "<g id=\"edge113\" class=\"edge\">\n",
                             "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13011.98,-34.39C12984.55,-42.01 12950.37,-50.21 12919.14,-54 12754.56,-73.99 1146.64,-74.67 982.14,-54 955.59,-50.66 926.88,-43.93 902.33,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"903.02,-33.73 892.44,-34.39 901.12,-40.47 903.02,-33.73\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13299.4,-34.49C13266.91,-42.08 13226.61,-50.23 13189.99,-54 13024.06,-71.08 1345.88,-71.47 1179.99,-54 1147.83,-50.61 1112.78,-43.69 1082.98,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1083.63,-33.37 1073.09,-34.49 1082.02,-40.19 1083.63,-33.37\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge112\" class=\"edge\">\n",
-                            "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13011.98,-34.39C12984.55,-42.01 12950.37,-50.21 12919.14,-54 12794.27,-69.17 3986.99,-69.37 3862.14,-54 3834.93,-50.65 3805.47,-43.87 3780.33,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3781.13,-33.68 3770.56,-34.39 3779.27,-40.42 3781.13,-33.68\"/>\n",
+                            "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge116\" class=\"edge\">\n",
+                            "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13299.4,-34.49C13266.91,-42.08 13226.61,-50.23 13189.99,-54 13079.13,-65.41 5276.67,-67.01 5165.99,-54 5137.51,-50.65 5106.62,-43.87 5080.24,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5080.93,-33.64 5070.36,-34.49 5079.15,-40.41 5080.93,-33.64\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge113\" class=\"edge\">\n",
+                            "<g id=\"edge114\" class=\"edge\">\n",
                             "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Google&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13011.98,-34.39C12984.55,-42.01 12950.37,-50.21 12919.14,-54 12741.78,-75.54 6664.31,-77.05 6487.14,-54 6461.6,-50.68 6434.03,-43.98 6410.43,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6411.16,-33.83 6400.58,-34.39 6409.2,-40.55 6411.16,-33.83\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13207.39,-18C13204.92,-18 13202.44,-18 13199.97,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13199.8,-14.5 13189.8,-18 13199.8,-21.5 13199.8,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge114\" class=\"edge\">\n",
+                            "<g id=\"edge115\" class=\"edge\">\n",
                             "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13011.98,-34.39C12984.55,-42.01 12950.37,-50.21 12919.14,-54 12747.65,-74.83 6870.94,-79.89 6700.14,-54 6678.46,-50.71 6655.26,-44.16 6635.34,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6636.44,-34.21 6625.85,-34.28 6634.18,-40.83 6636.44,-34.21\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge116\" class=\"edge\">\n",
-                            "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13011.98,-34.39C12984.55,-42.01 12950.37,-50.21 12919.14,-54 12822.08,-65.79 12795.97,-67.56 12699.14,-54 12675.6,-50.7 12650.28,-44.1 12628.56,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"12629.44,-34.05 12618.85,-34.38 12627.34,-40.72 12629.44,-34.05\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13299.4,-34.49C13266.91,-42.08 13226.61,-50.23 13189.99,-54 12999.88,-73.57 12519.5,-78.66 12329.99,-54 12304.45,-50.68 12276.88,-43.98 12253.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12254.01,-33.83 12243.43,-34.39 12252.05,-40.55 12254.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;score&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node62\" class=\"node\">\n",
+                            "<g id=\"node60\" class=\"node\">\n",
                             "<title>(&#39;score&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13317.14\" cy=\"-18\" rx=\"106.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"13317.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;score&#39;, &#39;NOUN&#39;) (0.0106)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13666.99\" cy=\"-18\" rx=\"130.78\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"13666.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;score&#39;, &#39;NOUN&#39;) (0.0112)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge117\" class=\"edge\">\n",
                             "<title>(&#39;PageRank&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13192.62,-18C13195.08,-18 13197.54,-18 13200.01,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13200.13,-21.5 13210.13,-18 13200.13,-14.5 13200.13,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13518.55,-18C13521.04,-18 13523.53,-18 13526.01,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13526.24,-21.5 13536.24,-18 13526.24,-14.5 13526.24,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Google&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;) -->\n",
                             "<g id=\"edge118\" class=\"edge\">\n",
                             "<title>(&#39;Google&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6469.01,-18C6471.47,-18 6473.94,-18 6476.41,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6476.55,-21.5 6486.55,-18 6476.55,-14.5 6476.55,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12989.62,-34.49C12959.79,-42.08 12922.74,-50.23 12888.99,-54 12765.54,-67.8 12453.17,-70.03 12329.99,-54 12304.45,-50.68 12276.88,-43.98 12253.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12254.01,-33.83 12243.43,-34.39 12252.05,-40.55 12254.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Google&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;) -->\n",
                             "<g id=\"edge119\" class=\"edge\">\n",
                             "<title>(&#39;Google&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6400.58,-34.39C6426.11,-42 6457.96,-50.2 6487.14,-54 6572.64,-65.12 6595.83,-66.52 6681.14,-54 6703.62,-50.7 6727.73,-44.1 6748.41,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6749.55,-40.75 6757.95,-34.29 6747.36,-34.1 6749.55,-40.75\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12989.62,-34.49C12959.79,-42.08 12922.74,-50.23 12888.99,-54 12758.25,-68.62 12723.5,-70.51 12592.99,-54 12566.62,-50.66 12538.11,-43.93 12513.74,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12514.49,-33.75 12503.92,-34.39 12512.59,-40.48 12514.49,-33.75\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;webpage&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node38\" class=\"node\">\n",
+                            "<g id=\"node37\" class=\"node\">\n",
                             "<title>(&#39;webpage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7040.14\" cy=\"-18\" rx=\"119.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"7040.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;webpage&#39;, &#39;NOUN&#39;) (0.0200)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12740.99\" cy=\"-18\" rx=\"147.57\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"12740.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;webpage&#39;, &#39;NOUN&#39;) (0.0201)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;Google&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;webpage&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge120\" class=\"edge\">\n",
                             "<title>(&#39;Google&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;webpage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6400.58,-34.39C6426.11,-42 6457.96,-50.2 6487.14,-54 6670.04,-77.8 6719.2,-77.47 6902.14,-54 6928.15,-50.66 6956.26,-43.93 6980.28,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6981.31,-40.52 6989.96,-34.39 6979.38,-33.79 6981.31,-40.52\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12906.21,-18C12903.76,-18 12901.31,-18 12898.86,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12898.79,-14.5 12888.79,-18 12898.79,-21.5 12898.79,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;) -->\n",
                             "<g id=\"edge121\" class=\"edge\">\n",
                             "<title>(&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;rank&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6682.05,-18C6684.53,-18 6687.02,-18 6689.5,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6689.72,-21.5 6699.72,-18 6689.72,-14.5 6689.72,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12312.36,-18C12314.83,-18 12317.3,-18 12319.78,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12319.94,-21.5 12329.94,-18 12319.94,-14.5 12319.94,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;webpage&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge122\" class=\"edge\">\n",
                             "<title>(&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;webpage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6625.85,-34.28C6647.62,-41.92 6674.91,-50.18 6700.14,-54 6788.9,-67.46 6813.09,-65.42 6902.14,-54 6928.15,-50.66 6956.26,-43.93 6980.28,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6981.31,-40.52 6989.96,-34.39 6979.38,-33.79 6981.31,-40.52\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12243.43,-34.39C12268.96,-42 12300.8,-50.2 12329.99,-54 12438.41,-68.11 12467.29,-65.72 12575.99,-54 12607.28,-50.63 12641.34,-43.75 12670.35,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12671.48,-40.23 12680.38,-34.49 12669.84,-33.43 12671.48,-40.23\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;Okapi&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"edge123\" class=\"edge\">\n",
                             "<title>(&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;Okapi&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6625.85,-34.28C6647.62,-41.92 6674.91,-50.18 6700.14,-54 6801.21,-69.32 7058.84,-67.67 7160.14,-54 7184.68,-50.69 7211.12,-44.04 7233.77,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7235.01,-40.63 7243.56,-34.39 7232.98,-33.93 7235.01,-40.63\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12144.55,-34.39C12119.02,-42 12087.17,-50.2 12057.99,-54 11929.96,-70.66 11605.25,-68.79 11476.99,-54 11447.84,-50.64 11416.19,-43.81 11389.2,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11390.04,-33.6 11379.49,-34.49 11388.3,-40.37 11390.04,-33.6\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;BM25&#39;, &#39;PROPN&#39;) -->\n",
                             "<g id=\"edge124\" class=\"edge\">\n",
                             "<title>(&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;BM25&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6625.85,-34.28C6647.62,-41.92 6674.91,-50.18 6700.14,-54 6831.17,-73.86 11339.79,-71.59 11471.14,-54 11495.85,-50.69 11522.49,-44.04 11545.32,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11546.62,-40.62 11555.19,-34.39 11544.61,-33.91 11546.62,-40.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12144.55,-34.39C12119.02,-42 12087.17,-50.2 12057.99,-54 11931.06,-70.52 11897.16,-68.57 11769.99,-54 11740.66,-50.64 11708.8,-43.81 11681.64,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11682.42,-33.58 11671.86,-34.49 11680.68,-40.36 11682.42,-33.58\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;function&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node69\" class=\"node\">\n",
+                            "<g id=\"node67\" class=\"node\">\n",
                             "<title>(&#39;function&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11852.14\" cy=\"-18\" rx=\"117.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"11852.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;function&#39;, &#39;NOUN&#39;) (0.0125)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11913.99\" cy=\"-18\" rx=\"143.77\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"11913.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;function&#39;, &#39;NOUN&#39;) (0.0127)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;function&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge125\" class=\"edge\">\n",
                             "<title>(&#39;use&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;function&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6625.85,-34.28C6647.62,-41.92 6674.91,-50.18 6700.14,-54 6837.93,-74.89 11578.96,-72.11 11717.14,-54 11742.5,-50.68 11769.87,-43.98 11793.29,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11794.47,-40.57 11803.07,-34.39 11792.49,-33.85 11794.47,-40.57\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12075.64,-18C12073.04,-18 12070.44,-18 12067.84,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12067.82,-14.5 12057.82,-18 12067.82,-21.5 12067.82,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;rank&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;webpage&#39;, &#39;NOUN&#39;) -->\n",
                             "<g id=\"edge126\" class=\"edge\">\n",
                             "<title>(&#39;rank&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;webpage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6902.9,-18C6905.35,-18 6907.8,-18 6910.25,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6910.33,-21.5 6920.33,-18 6910.33,-14.5 6910.33,-21.5\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;textrank&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node39\" class=\"node\">\n",
-                            "<title>(&#39;textrank&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16802.14\" cy=\"-18\" rx=\"117.78\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"16802.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;textrank&#39;, &#39;NOUN&#39;) (0.0041)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;work&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node40\" class=\"node\">\n",
-                            "<title>(&#39;work&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"17042.14\" cy=\"-18\" rx=\"103.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"17042.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;work&#39;, &#39;VERB&#39;) (0.0059)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;textrank&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;work&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge127\" class=\"edge\">\n",
-                            "<title>(&#39;textrank&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;work&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16919.8,-18C16922.45,-18 16925.09,-18 16927.74,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"16927.96,-21.5 16937.96,-18 16927.96,-14.5 16927.96,-21.5\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;follow&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node41\" class=\"node\">\n",
-                            "<title>(&#39;follow&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"17273.14\" cy=\"-18\" rx=\"109.38\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"17273.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;follow&#39;, &#39;VERB&#39;) (0.0109)</text>\n",
-                            "</g>\n",
-                            "<!-- (&#39;textrank&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;follow&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge128\" class=\"edge\">\n",
-                            "<title>(&#39;textrank&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;follow&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16851.58,-34.39C16877.11,-42 16908.96,-50.2 16938.14,-54 17029.81,-65.93 17054.58,-66.73 17146.14,-54 17169.86,-50.7 17195.38,-44.1 17217.27,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"17218.55,-40.7 17227.06,-34.38 17216.47,-34.02 17218.55,-40.7\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M12575.9,-18C12578.34,-18 12580.79,-18 12583.24,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12583.31,-21.5 12593.31,-18 12583.31,-14.5 12583.31,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;work&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;follow&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge129\" class=\"edge\">\n",
+                            "<g id=\"edge127\" class=\"edge\">\n",
                             "<title>(&#39;work&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;follow&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M17146.36,-18C17148.8,-18 17151.24,-18 17153.67,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"17153.7,-21.5 17163.7,-18 17153.7,-14.5 17153.7,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M17831.03,-18C17833.64,-18 17836.25,-18 17838.86,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"17838.94,-21.5 17848.94,-18 17838.94,-14.5 17838.94,-21.5\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;pre&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node42\" class=\"node\">\n",
-                            "<title>(&#39;pre&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16368.14\" cy=\"-18\" rx=\"99.38\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"16368.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;pre&#39;, &#39;NOUN&#39;) (0.0041)</text>\n",
+                            "<!-- (&#39;Pre&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"node40\" class=\"node\">\n",
+                            "<title>(&#39;Pre&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"19649.99\" cy=\"-18\" rx=\"122.38\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"19649.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Pre&#39;, &#39;NOUN&#39;) (0.0044)</text>\n",
                             "</g>\n",
-                            "<!-- (&#39;pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge132\" class=\"edge\">\n",
-                            "<title>(&#39;pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16325.69,-34.29C16303.54,-41.93 16275.77,-50.18 16250.14,-54 16148.9,-69.1 1611.4,-68.98 1510.14,-54 1488.03,-50.73 1464.34,-44.21 1443.96,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1444.83,-34.22 1434.24,-34.38 1442.62,-40.86 1444.83,-34.22\"/>\n",
+                            "<!-- (&#39;Pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge130\" class=\"edge\">\n",
+                            "<title>(&#39;Pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19599.06,-34.39C19572.77,-42.01 19539.99,-50.2 19509.99,-54 19388.13,-69.42 1943.88,-69.21 1821.99,-54 1795.14,-50.65 1766.09,-43.87 1741.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1742.24,-33.71 1731.66,-34.39 1740.35,-40.45 1742.24,-33.71\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;&#45;&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node43\" class=\"node\">\n",
+                            "<g id=\"node41\" class=\"node\">\n",
                             "<title>(&#39;&#45;&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16576.14\" cy=\"-18\" rx=\"90.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"16576.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;&#45;&#39;, &#39;NOUN&#39;) (0.0053)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"19898.99\" cy=\"-18\" rx=\"108.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"19898.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;&#45;&#39;, &#39;NOUN&#39;) (0.0056)</text>\n",
                             "</g>\n",
-                            "<!-- (&#39;pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;&#45;&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge130\" class=\"edge\">\n",
-                            "<title>(&#39;pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;&#45;&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16467.67,-18C16470.27,-18 16472.86,-18 16475.46,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"16475.47,-21.5 16485.47,-18 16475.47,-14.5 16475.47,-21.5\"/>\n",
+                            "<!-- (&#39;Pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;&#45;&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge128\" class=\"edge\">\n",
+                            "<title>(&#39;Pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;&#45;&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19772.54,-18C19775.14,-18 19777.73,-18 19780.32,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"19780.33,-21.5 19790.33,-18 19780.33,-14.5 19780.33,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;process&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node44\" class=\"node\">\n",
+                            "<g id=\"node42\" class=\"node\">\n",
                             "<title>(&#39;process&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16137.14\" cy=\"-18\" rx=\"113.18\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"16137.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;process&#39;, &#39;VERB&#39;) (0.0068)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"19371.99\" cy=\"-18\" rx=\"137.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"19371.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;process&#39;, &#39;VERB&#39;) (0.0072)</text>\n",
                             "</g>\n",
-                            "<!-- (&#39;pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;process&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge131\" class=\"edge\">\n",
-                            "<title>(&#39;pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;process&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16268.32,-18C16265.71,-18 16263.09,-18 16260.48,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"16260.39,-14.5 16250.39,-18 16260.39,-21.5 16260.39,-14.5\"/>\n",
+                            "<!-- (&#39;Pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;process&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge129\" class=\"edge\">\n",
+                            "<title>(&#39;Pre&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;process&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19527.69,-18C19525.09,-18 19522.5,-18 19519.91,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"19519.9,-14.5 19509.9,-18 19519.9,-21.5 19519.9,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;&#45;&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge134\" class=\"edge\">\n",
+                            "<g id=\"edge132\" class=\"edge\">\n",
                             "<title>(&#39;&#45;&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16537.04,-34.28C16516.6,-41.92 16490.95,-50.17 16467.14,-54 16364.59,-70.5 1612.89,-69.2 1510.14,-54 1488.03,-50.73 1464.34,-44.21 1443.96,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1444.83,-34.22 1434.24,-34.38 1442.62,-40.86 1444.83,-34.22\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19852.9,-34.38C19829.08,-42 19799.34,-50.2 19771.99,-54 19648.52,-71.16 1945.68,-69.44 1821.99,-54 1795.14,-50.65 1766.09,-43.87 1741.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1742.24,-33.71 1731.66,-34.39 1740.35,-40.45 1742.24,-33.71\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;&#45;&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;process&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge133\" class=\"edge\">\n",
+                            "<g id=\"edge131\" class=\"edge\">\n",
                             "<title>(&#39;&#45;&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;process&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16537.04,-34.28C16516.6,-41.92 16490.95,-50.17 16467.14,-54 16380.26,-67.98 16356.36,-65.68 16269.14,-54 16244.43,-50.69 16217.79,-44.04 16194.96,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"16195.68,-33.91 16185.09,-34.39 16193.66,-40.62 16195.68,-33.91\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19852.9,-34.38C19829.08,-42 19799.34,-50.2 19771.99,-54 19664.58,-68.93 19635.74,-66.27 19527.99,-54 19498.35,-50.62 19466.15,-43.75 19438.74,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"19439.42,-33.47 19428.87,-34.39 19437.69,-40.26 19439.42,-33.47\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;&#45;&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;remove&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge135\" class=\"edge\">\n",
+                            "<g id=\"edge133\" class=\"edge\">\n",
                             "<title>(&#39;&#45;&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;remove&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16537.04,-34.28C16516.6,-41.92 16490.95,-50.17 16467.14,-54 16343.73,-73.85 15466.02,-70.71 15342.14,-54 15317.61,-50.69 15291.17,-44.04 15268.51,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15269.3,-33.93 15258.72,-34.39 15267.28,-40.63 15269.3,-33.93\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19852.9,-34.38C19829.08,-42 19799.34,-50.2 19771.99,-54 19622.98,-74.71 18567.46,-71.13 18417.99,-54 18388.53,-50.62 18356.53,-43.75 18329.3,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18330.05,-33.49 18319.5,-34.39 18328.31,-40.27 18330.05,-33.49\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;process&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge136\" class=\"edge\">\n",
+                            "<g id=\"edge134\" class=\"edge\">\n",
                             "<title>(&#39;process&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;text&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16089.19,-34.39C16064.42,-42 16033.51,-50.2 16005.14,-54 15905.37,-67.36 1609.72,-68.73 1510.14,-54 1488.03,-50.73 1464.34,-44.21 1443.96,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1444.83,-34.22 1434.24,-34.38 1442.62,-40.86 1444.83,-34.22\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19315.12,-34.49C19286.04,-42.08 19249.93,-50.23 19216.99,-54 19096.98,-67.75 1941.86,-68.96 1821.99,-54 1795.14,-50.65 1766.09,-43.87 1741.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1742.24,-33.71 1731.66,-34.39 1740.35,-40.45 1742.24,-33.71\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;process&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remove&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge137\" class=\"edge\">\n",
+                            "<g id=\"edge135\" class=\"edge\">\n",
                             "<title>(&#39;process&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remove&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16089.19,-34.39C16064.42,-42 16033.51,-50.2 16005.14,-54 15859.11,-73.56 15488.15,-73.7 15342.14,-54 15317.61,-50.69 15291.17,-44.04 15268.51,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15269.3,-33.93 15258.72,-34.39 15267.28,-40.63 15269.3,-33.93\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19315.12,-34.49C19286.04,-42.08 19249.93,-50.23 19216.99,-54 19040.59,-74.22 18594.39,-74.22 18417.99,-54 18388.53,-50.62 18356.53,-43.75 18329.3,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18330.05,-33.49 18319.5,-34.39 18328.31,-40.27 18330.05,-33.49\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;process&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stop&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge138\" class=\"edge\">\n",
+                            "<g id=\"edge136\" class=\"edge\">\n",
                             "<title>(&#39;process&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stop&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M16089.19,-34.39C16064.42,-42 16033.51,-50.2 16005.14,-54 15907.35,-67.1 15658.73,-68.56 15561.14,-54 15539.2,-50.73 15515.71,-44.21 15495.5,-37.61\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15496.46,-34.24 15485.87,-34.38 15494.23,-40.88 15496.46,-34.24\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M19315.12,-34.49C19286.04,-42.08 19249.93,-50.23 19216.99,-54 19098.43,-67.59 18798.38,-68.98 18679.99,-54 18653.62,-50.66 18625.11,-43.93 18600.74,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18601.49,-33.75 18590.92,-34.39 18599.59,-40.48 18601.49,-33.75\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;remove&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stop&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge139\" class=\"edge\">\n",
+                            "<g id=\"edge137\" class=\"edge\">\n",
                             "<title>(&#39;remove&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stop&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M15324.42,-18C15326.9,-18 15329.38,-18 15331.86,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15332.04,-21.5 15342.04,-18 15332.04,-14.5 15332.04,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M18399.6,-18C18402.24,-18 18404.87,-18 18407.51,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18407.69,-21.5 18417.69,-18 18407.69,-14.5 18407.69,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;remove&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stem&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge140\" class=\"edge\">\n",
+                            "<g id=\"edge138\" class=\"edge\">\n",
                             "<title>(&#39;remove&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stem&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M15258.72,-34.39C15283.3,-42 15313.98,-50.2 15342.14,-54 15431.11,-66 15455.32,-67.04 15544.14,-54 15566.53,-50.71 15590.54,-44.15 15611.15,-37.52\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15612.27,-40.84 15620.67,-34.38 15610.08,-34.19 15612.27,-40.84\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M18319.5,-34.39C18348.64,-42.01 18384.92,-50.21 18417.99,-54 18525.73,-66.35 18554.37,-67.34 18661.99,-54 18689.02,-50.65 18718.27,-43.87 18743.24,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18744.24,-40.44 18752.94,-34.39 18742.37,-33.69 18744.24,-40.44\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;remain&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node48\" class=\"node\">\n",
+                            "<g id=\"node46\" class=\"node\">\n",
                             "<title>(&#39;remain&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15895.14\" cy=\"-18\" rx=\"110.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"15895.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;remain&#39;, &#39;VERB&#39;) (0.0231)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"19081.99\" cy=\"-18\" rx=\"134.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"19081.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;remain&#39;, &#39;VERB&#39;) (0.0243)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;remove&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remain&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge141\" class=\"edge\">\n",
+                            "<g id=\"edge139\" class=\"edge\">\n",
                             "<title>(&#39;remove&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remain&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M15258.72,-34.39C15283.3,-42 15313.98,-50.2 15342.14,-54 15435.74,-66.63 15673.58,-66.91 15767.14,-54 15791.14,-50.69 15816.98,-44.04 15839.12,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15840.17,-40.69 15848.68,-34.39 15838.09,-34 15840.17,-40.69\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M18319.5,-34.39C18348.64,-42.01 18384.92,-50.21 18417.99,-54 18531.03,-66.95 18816.98,-67.2 18929.99,-54 18958.65,-50.65 18989.75,-43.87 19016.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"19017.45,-40.4 19026.24,-34.49 19015.68,-33.63 19017.45,-40.4\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;stop&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stem&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge142\" class=\"edge\">\n",
+                            "<g id=\"edge140\" class=\"edge\">\n",
                             "<title>(&#39;stop&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;stem&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M15544.15,-18C15546.43,-18 15548.72,-18 15551,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15551.02,-21.5 15561.02,-18 15551.02,-14.5 15551.02,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M18662.4,-18C18664.86,-18 18667.33,-18 18669.8,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18669.94,-21.5 18679.94,-18 18669.94,-14.5 18669.94,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;stop&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remain&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge143\" class=\"edge\">\n",
+                            "<g id=\"edge141\" class=\"edge\">\n",
                             "<title>(&#39;stop&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remain&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M15485.87,-34.38C15507.97,-41.99 15535.61,-50.19 15561.14,-54 15651.7,-67.51 15676.44,-66.51 15767.14,-54 15791.14,-50.69 15816.98,-44.04 15839.12,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15840.17,-40.69 15848.68,-34.39 15838.09,-34 15840.17,-40.69\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M18590.92,-34.39C18617.21,-42.01 18649.99,-50.2 18679.99,-54 18790.22,-67.95 18819.63,-66.89 18929.99,-54 18958.65,-50.65 18989.75,-43.87 19016.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"19017.45,-40.4 19026.24,-34.49 19015.68,-33.63 19017.45,-40.4\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;stem&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remain&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge144\" class=\"edge\">\n",
+                            "<g id=\"edge142\" class=\"edge\">\n",
                             "<title>(&#39;stem&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;remain&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M15767.01,-18C15769.47,-18 15771.94,-18 15774.4,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"15774.53,-21.5 15784.53,-18 15774.53,-14.5 15774.53,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M18929.96,-18C18932.3,-18 18934.63,-18 18936.96,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"18937.19,-21.5 18947.19,-18 18937.19,-14.5 18937.19,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;create&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node49\" class=\"node\">\n",
+                            "<g id=\"node47\" class=\"node\">\n",
                             "<title>(&#39;create&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12340.14\" cy=\"-18\" rx=\"107.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"12340.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;create&#39;, &#39;VERB&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"17431.99\" cy=\"-18\" rx=\"131.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"17431.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;create&#39;, &#39;VERB&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge145\" class=\"edge\">\n",
+                            "<g id=\"edge143\" class=\"edge\">\n",
                             "<title>(&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12447.54,-18C12450.02,-18 12452.51,-18 12454.99,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"12455.2,-21.5 12465.2,-18 12455.2,-14.5 12455.2,-21.5\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;vertex&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node51\" class=\"node\">\n",
-                            "<title>(&#39;vertex&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12809.14\" cy=\"-18\" rx=\"110.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"12809.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;vertex&#39;, &#39;NOUN&#39;) (0.0100)</text>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M17377.71,-34.39C17349.71,-42.01 17314.83,-50.21 17282.99,-54 17115.88,-73.9 5333.13,-73.65 5165.99,-54 5137.51,-50.65 5106.62,-43.87 5080.24,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5080.93,-33.64 5070.36,-34.49 5079.15,-40.41 5080.93,-33.64\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;vertex&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge146\" class=\"edge\">\n",
+                            "<g id=\"edge144\" class=\"edge\">\n",
                             "<title>(&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;vertex&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12385.48,-34.38C12408.92,-42 12438.2,-50.2 12465.14,-54 12560.2,-67.42 12586.04,-67.12 12681.14,-54 12705.14,-50.69 12730.98,-44.04 12753.12,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"12754.17,-40.69 12762.68,-34.39 12752.09,-34 12754.17,-40.69\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge147\" class=\"edge\">\n",
-                            "<title>(&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12294.8,-34.38C12271.36,-42 12242.09,-50.2 12215.14,-54 12084.66,-72.42 9974.06,-69 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M17377.71,-34.39C17349.71,-42.01 17314.83,-50.21 17282.99,-54 17144.33,-70.51 7367.71,-70 7228.99,-54 7199.72,-50.62 7167.92,-43.75 7140.87,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7141.68,-33.5 7131.13,-34.39 7139.93,-40.28 7141.68,-33.5\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;vertex&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge148\" class=\"edge\">\n",
-                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;vertex&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12681.46,-18C12683.76,-18 12686.05,-18 12688.35,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"12688.42,-21.5 12698.42,-18 12688.42,-14.5 12688.42,-21.5\"/>\n",
+                            "<!-- (&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;be&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge145\" class=\"edge\">\n",
+                            "<title>(&#39;create&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;be&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M17377.71,-34.39C17349.71,-42.01 17314.83,-50.21 17282.99,-54 17147.7,-70.11 7608.02,-72.22 7472.99,-54 7448.45,-50.69 7422.02,-44.04 7399.36,-37.35\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7400.15,-33.93 7389.57,-34.39 7398.12,-40.63 7400.15,-33.93\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge149\" class=\"edge\">\n",
-                            "<title>(&#39;graph&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12527.43,-34.38C12503.8,-42 12474.29,-50.2 12447.14,-54 12303.87,-74.07 9986.87,-70.47 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<!-- (&#39;vertex&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;be&#39;, &#39;VERB&#39;) -->\n",
+                            "<g id=\"edge146\" class=\"edge\">\n",
+                            "<title>(&#39;vertex&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;be&#39;, &#39;VERB&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7210.84,-18C7213.45,-18 7216.07,-18 7218.68,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7218.77,-21.5 7228.77,-18 7218.77,-14.5 7218.77,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;vertex&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge150\" class=\"edge\">\n",
+                            "<g id=\"edge147\" class=\"edge\">\n",
                             "<title>(&#39;vertex&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12762.68,-34.39C12738.67,-42 12708.7,-50.2 12681.14,-54 12524.95,-75.55 9999.78,-71.95 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7131.13,-34.39C7160.08,-42.01 7196.12,-50.21 7228.99,-54 7328.77,-65.51 7355.12,-64.71 7454.99,-54 7486.46,-50.63 7520.73,-43.75 7549.91,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7551.1,-40.22 7560.01,-34.49 7549.47,-33.41 7551.1,-40.22\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;be&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge148\" class=\"edge\">\n",
+                            "<title>(&#39;be&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7455.33,-18C7457.98,-18 7460.62,-18 7463.26,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7463.45,-21.5 7473.45,-18 7463.45,-14.5 7463.45,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge153\" class=\"edge\">\n",
+                            "<g id=\"edge151\" class=\"edge\">\n",
                             "<title>(&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9800.43,-23.95C9815.25,-22.94 9825.08,-20.95 9825.08,-18 9825.08,-15.79 9819.55,-14.12 9810.53,-12.99\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9810.71,-9.49 9800.43,-12.05 9810.06,-16.46 9810.71,-9.49\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7761.08,-23.68C7776.54,-22.6 7786.53,-20.71 7786.53,-18 7786.53,-15.95 7780.79,-14.36 7771.29,-13.25\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7771.35,-9.74 7761.08,-12.32 7770.72,-16.71 7771.35,-9.74\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;other&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"node54\" class=\"node\">\n",
+                            "<g id=\"node52\" class=\"node\">\n",
                             "<title>(&#39;other&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"9940.14\" cy=\"-18\" rx=\"96.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"9940.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;other&#39;, &#39;ADJ&#39;) (0.0171)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"7921.99\" cy=\"-18\" rx=\"116.98\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"7921.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;other&#39;, &#39;ADJ&#39;) (0.0182)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;other&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge151\" class=\"edge\">\n",
+                            "<g id=\"edge149\" class=\"edge\">\n",
                             "<title>(&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;other&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9775.75,-5.75C9802.04,-4.04 9828.33,-4.08 9854.61,-5.89\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9854.45,-9.39 9864.69,-6.67 9854.99,-2.41 9854.45,-9.39\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7728.28,-5.61C7759.23,-4.02 7790.19,-4.14 7821.14,-5.97\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7820.98,-9.47 7831.19,-6.62 7821.44,-2.48 7820.98,-9.47\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge152\" class=\"edge\">\n",
+                            "<g id=\"edge150\" class=\"edge\">\n",
                             "<title>(&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9751.33,-33.33C9778.49,-39.18 9810.69,-45.12 9840.14,-48 9928.61,-56.65 9951.93,-58.95 10040.14,-48 10059.32,-45.62 10079.84,-41.16 10098.36,-36.39\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10099.35,-39.75 10108.12,-33.8 10097.56,-32.98 10099.35,-39.75\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7697.26,-33.5C7729.44,-39.29 7767.39,-45.15 7801.99,-48 7908.3,-56.75 7935.89,-59.01 8041.99,-48 8065.51,-45.56 8090.86,-40.92 8113.58,-36\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8114.48,-39.39 8123.49,-33.81 8112.97,-32.56 8114.48,-39.39\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;percentage&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node64\" class=\"node\">\n",
+                            "<g id=\"node62\" class=\"node\">\n",
                             "<title>(&#39;percentage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"10876.14\" cy=\"-18\" rx=\"126.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"10876.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;percentage&#39;, &#39;NOUN&#39;) (0.0237)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16270.99\" cy=\"-18\" rx=\"157.87\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"16270.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;percentage&#39;, &#39;NOUN&#39;) (0.0251)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;percentage&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge154\" class=\"edge\">\n",
+                            "<g id=\"edge152\" class=\"edge\">\n",
                             "<title>(&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;percentage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9743.2,-34.02C9772.58,-41.74 9809.52,-50.15 9843.14,-54 10039.19,-76.47 10535.27,-77.95 10731.14,-54 10758.53,-50.65 10788.19,-43.87 10813.51,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10814.63,-40.41 10823.35,-34.39 10812.78,-33.66 10814.63,-40.41\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7686.96,-34.12C7721.82,-41.81 7765.46,-50.17 7804.99,-54 8034.19,-76.21 15865.88,-77.19 16094.99,-54 16128.59,-50.6 16165.25,-43.63 16196.38,-36.73\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16197.29,-40.11 16206.28,-34.49 16195.75,-33.28 16197.29,-40.11\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;appear&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node65\" class=\"node\">\n",
+                            "<g id=\"node63\" class=\"node\">\n",
                             "<title>(&#39;appear&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11131.14\" cy=\"-18\" rx=\"109.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"11131.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;appear&#39;, &#39;VERB&#39;) (0.0428)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16580.99\" cy=\"-18\" rx=\"133.78\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"16580.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;appear&#39;, &#39;VERB&#39;) (0.0454)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;appear&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge155\" class=\"edge\">\n",
+                            "<g id=\"edge153\" class=\"edge\">\n",
                             "<title>(&#39;sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;appear&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9743.2,-34.02C9772.58,-41.74 9809.52,-50.15 9843.14,-54 9971.19,-68.68 10875.46,-71.61 11003.14,-54 11027.14,-50.69 11052.98,-44.04 11075.12,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11076.17,-40.69 11084.68,-34.39 11074.09,-34 11076.17,-40.69\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7686.96,-34.12C7721.82,-41.81 7765.46,-50.17 7804.99,-54 7924.21,-65.55 16310.02,-67.9 16428.99,-54 16457.77,-50.64 16489.01,-43.81 16515.63,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16516.81,-40.31 16525.6,-34.39 16515.04,-33.54 16516.81,-40.31\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;connect&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node53\" class=\"node\">\n",
+                            "<g id=\"node51\" class=\"node\">\n",
                             "<title>(&#39;connect&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"12101.14\" cy=\"-18\" rx=\"113.98\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"12101.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;connect&#39;, &#39;VERB&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"17144.99\" cy=\"-18\" rx=\"137.58\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"17144.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;connect&#39;, &#39;VERB&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;connect&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge156\" class=\"edge\">\n",
+                            "<g id=\"edge154\" class=\"edge\">\n",
                             "<title>(&#39;connect&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12053.56,-34.39C12028.98,-42 11998.31,-50.2 11970.14,-54 11853.04,-69.8 9960.54,-67.45 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M17088.11,-34.39C17058.78,-42.01 17022.27,-50.21 16988.99,-54 16862.25,-68.43 7931.95,-66.3 7804.99,-54 7769.17,-50.53 7729.97,-43.34 7696.99,-36.29\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7697.48,-32.82 7686.96,-34.12 7695.99,-39.66 7697.48,-32.82\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;connect&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;other&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge157\" class=\"edge\">\n",
+                            "<g id=\"edge155\" class=\"edge\">\n",
                             "<title>(&#39;connect&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;other&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M12053.56,-34.39C12028.98,-42 11998.31,-50.2 11970.14,-54 11864.65,-68.23 10159.34,-70.22 10054.14,-54 10033,-50.74 10010.4,-44.27 9990.94,-37.7\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9991.97,-34.35 9981.37,-34.38 9989.67,-40.96 9991.97,-34.35\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M17088.11,-34.39C17058.78,-42.01 17022.27,-50.21 16988.99,-54 16865.73,-68.04 8179.99,-70.12 8056.99,-54 8031.63,-50.68 8004.26,-43.98 7980.84,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7981.64,-33.85 7971.06,-34.39 7979.67,-40.57 7981.64,-33.85\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;other&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge158\" class=\"edge\">\n",
+                            "<g id=\"edge156\" class=\"edge\">\n",
                             "<title>(&#39;other&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M9864.69,-29.33C9838.4,-31.59 9812.11,-32.08 9785.83,-30.82\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9785.93,-27.32 9775.75,-30.25 9785.54,-34.31 9785.93,-27.32\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M7831.19,-29.38C7800.24,-31.58 7769.28,-32.07 7738.33,-30.84\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7738.43,-27.35 7728.28,-30.39 7738.11,-34.34 7738.43,-27.35\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;other&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge159\" class=\"edge\">\n",
+                            "<g id=\"edge157\" class=\"edge\">\n",
                             "<title>(&#39;other&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10037.24,-18C10039.56,-18 10041.88,-18 10044.2,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10044.38,-21.5 10054.38,-18 10044.38,-14.5 10044.38,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8039.11,-18C8041.59,-18 8044.08,-18 8046.56,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8046.77,-21.5 8056.77,-18 8046.77,-14.5 8046.77,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge161\" class=\"edge\">\n",
+                            "<g id=\"edge159\" class=\"edge\">\n",
                             "<title>(&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10120.01,-34.8C10095.78,-44.28 10063.74,-55.16 10034.14,-60 9951.68,-73.48 9928.99,-70.82 9846.14,-60 9812.64,-55.62 9776.13,-46.23 9746.65,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9747.53,-34.05 9736.94,-34.49 9745.49,-40.75 9747.53,-34.05\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8138.05,-34.81C8109.06,-44.29 8070.87,-55.18 8035.99,-60 7935.61,-73.88 7908.71,-71.17 7807.99,-60 7768.26,-55.59 7724.63,-46.07 7689.52,-37.21\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7689.94,-33.7 7679.38,-34.61 7688.2,-40.48 7689.94,-33.7\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge160\" class=\"edge\">\n",
+                            "<g id=\"edge158\" class=\"edge\">\n",
                             "<title>(&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10264.2,-18C10266.65,-18 10269.11,-18 10271.57,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10271.68,-21.5 10281.68,-18 10271.68,-14.5 10271.68,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8313.13,-18C8315.59,-18 8318.04,-18 8320.5,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8320.59,-21.5 8330.59,-18 8320.59,-14.5 8320.59,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;percentage&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge162\" class=\"edge\">\n",
+                            "<g id=\"edge160\" class=\"edge\">\n",
                             "<title>(&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;percentage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10203.73,-34.38C10226.79,-42 10255.6,-50.2 10282.14,-54 10380.91,-68.16 10632.1,-66.11 10731.14,-54 10758.53,-50.65 10788.19,-43.87 10813.51,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10814.63,-40.41 10823.35,-34.39 10812.78,-33.66 10814.63,-40.41\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8238.15,-34.39C8265.58,-42.01 8299.76,-50.21 8330.99,-54 8545.08,-80.01 15880.42,-75.72 16094.99,-54 16128.59,-50.6 16165.25,-43.63 16196.38,-36.73\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16197.29,-40.11 16206.28,-34.49 16195.75,-33.28 16197.29,-40.11\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;appear&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge163\" class=\"edge\">\n",
+                            "<g id=\"edge161\" class=\"edge\">\n",
                             "<title>(&#39;edge&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;appear&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10203.73,-34.38C10226.79,-42 10255.6,-50.2 10282.14,-54 10440.74,-76.73 10844.42,-75.9 11003.14,-54 11027.14,-50.69 11052.98,-44.04 11075.12,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11076.17,-40.69 11084.68,-34.39 11074.09,-34 11076.17,-40.69\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8238.15,-34.39C8265.58,-42.01 8299.76,-50.21 8330.99,-54 8442.64,-67.56 16317.28,-67.05 16428.99,-54 16457.77,-50.64 16489.01,-43.81 16515.63,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16516.81,-40.31 16525.6,-34.39 16515.04,-33.54 16516.81,-40.31\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge166\" class=\"edge\">\n",
+                            "<g id=\"edge164\" class=\"edge\">\n",
                             "<title>(&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10571.56,-34.39C10546.98,-42 10516.31,-50.2 10488.14,-54 10346.09,-73.16 9985.54,-70.32 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15900.11,-34.39C15870.78,-42.01 15834.27,-50.21 15800.99,-54 15580.31,-79.13 8026.07,-75.42 7804.99,-54 7769.17,-50.53 7729.97,-43.34 7696.99,-36.29\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7697.48,-32.82 7686.96,-34.12 7695.99,-39.66 7697.48,-32.82\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge164\" class=\"edge\">\n",
+                            "<g id=\"edge162\" class=\"edge\">\n",
                             "<title>(&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10571.56,-34.39C10546.98,-42 10516.31,-50.2 10488.14,-54 10397.41,-66.24 10372.77,-66.99 10282.14,-54 10259.23,-50.72 10234.63,-44.16 10213.49,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10214.33,-34.12 10203.73,-34.38 10212.18,-40.78 10214.33,-34.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15900.11,-34.39C15870.78,-42.01 15834.27,-50.21 15800.99,-54 15697.91,-65.74 8433.98,-66.51 8330.99,-54 8303.42,-50.65 8273.55,-43.87 8248.06,-37.09\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8248.72,-33.64 8238.15,-34.39 8246.88,-40.39 8248.72,-33.64\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge165\" class=\"edge\">\n",
+                            "<g id=\"edge163\" class=\"edge\">\n",
                             "<title>(&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10506.7,-18C10504.1,-18 10501.5,-18 10498.9,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10498.89,-14.5 10488.89,-18 10498.89,-21.5 10498.89,-14.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15900.11,-34.39C15870.78,-42.01 15834.27,-50.21 15800.99,-54 15602.16,-76.64 8795.56,-78.78 8596.99,-54 8570.14,-50.65 8541.09,-43.87 8516.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8517.24,-33.71 8506.66,-34.39 8515.35,-40.45 8517.24,-33.71\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;percentage&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge167\" class=\"edge\">\n",
+                            "<g id=\"edge165\" class=\"edge\">\n",
                             "<title>(&#39;weight&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;percentage&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10731.83,-18C10734.29,-18 10736.74,-18 10739.2,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10739.31,-21.5 10749.3,-18 10739.3,-14.5 10739.31,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M16094.98,-18C16097.58,-18 16100.19,-18 16102.8,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16102.85,-21.5 16112.85,-18 16102.85,-14.5 16102.85,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;similar&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge168\" class=\"edge\">\n",
+                            "<g id=\"edge166\" class=\"edge\">\n",
                             "<title>(&#39;similar&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M10341.3,-34.38C10318.62,-42 10290.28,-50.19 10264.14,-54 10171.56,-67.48 9936.09,-64.65 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M8403.32,-34.39C8376.64,-42.01 8343.4,-50.21 8312.99,-54 8200.97,-67.98 7917.35,-64.89 7804.99,-54 7769.17,-50.53 7729.97,-43.34 7696.99,-36.29\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7697.48,-32.82 7686.96,-34.12 7695.99,-39.66 7697.48,-32.82\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;run&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node58\" class=\"node\">\n",
+                            "<g id=\"node56\" class=\"node\">\n",
                             "<title>(&#39;run&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14727.14\" cy=\"-18\" rx=\"97.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"14727.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;run&#39;, &#39;VERB&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15374.99\" cy=\"-18\" rx=\"118.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"15374.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;run&#39;, &#39;VERB&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge170\" class=\"edge\">\n",
+                            "<g id=\"edge168\" class=\"edge\">\n",
                             "<title>(&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;algorithm&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14685.43,-34.28C14663.66,-41.92 14636.37,-50.18 14611.14,-54 14517.56,-68.19 1076.05,-65.8 982.14,-54 955.59,-50.66 926.88,-43.93 902.33,-37.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"903.02,-33.73 892.44,-34.39 901.12,-40.47 903.02,-33.73\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge169\" class=\"edge\">\n",
-                            "<title>(&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14685.43,-34.28C14663.66,-41.92 14636.37,-50.18 14611.14,-54 14457.23,-77.33 13364.66,-72.89 13210.14,-54 13182.75,-50.65 13153.09,-43.87 13127.77,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13128.5,-33.66 13117.93,-34.39 13126.65,-40.41 13128.5,-33.66\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15325.55,-34.39C15300.02,-42 15268.17,-50.2 15238.99,-54 15045.36,-79.19 1374.18,-74.45 1179.99,-54 1147.83,-50.61 1112.78,-43.69 1082.98,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1083.63,-33.37 1073.09,-34.49 1082.02,-40.19 1083.63,-33.37\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge171\" class=\"edge\">\n",
+                            "<g id=\"edge169\" class=\"edge\">\n",
                             "<title>(&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;graph&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14685.43,-34.28C14663.66,-41.92 14636.37,-50.18 14611.14,-54 14506.12,-69.92 12804.34,-68.73 12699.14,-54 12675.6,-50.7 12650.28,-44.1 12628.56,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"12629.44,-34.05 12618.85,-34.38 12627.34,-40.72 12629.44,-34.05\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15325.55,-34.39C15300.02,-42 15268.17,-50.2 15238.99,-54 15100.26,-72.05 5304.94,-70.33 5165.99,-54 5137.51,-50.65 5106.62,-43.87 5080.24,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5080.93,-33.64 5070.36,-34.49 5079.15,-40.41 5080.93,-33.64\"/>\n",
+                            "</g>\n",
+                            "<!-- (&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
+                            "<g id=\"edge167\" class=\"edge\">\n",
+                            "<title>(&#39;run&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15325.55,-34.39C15300.02,-42 15268.17,-50.2 15238.99,-54 15051.35,-78.41 13724.22,-73.38 13535.99,-54 13503.09,-50.61 13467.22,-43.69 13436.71,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13437.11,-33.32 13426.58,-34.49 13435.55,-40.14 13437.11,-33.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;pick&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"node59\" class=\"node\">\n",
+                            "<g id=\"node57\" class=\"node\">\n",
                             "<title>(&#39;pick&#39;, &#39;VERB&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14068.14\" cy=\"-18\" rx=\"101.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"14068.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;pick&#39;, &#39;VERB&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14589.99\" cy=\"-18\" rx=\"120.78\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"14589.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;pick&#39;, &#39;VERB&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge174\" class=\"edge\">\n",
+                            "<g id=\"edge172\" class=\"edge\">\n",
                             "<title>(&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14024.95,-34.29C14002.41,-41.93 13974.18,-50.18 13948.14,-54 13785.88,-77.81 13372.93,-73.91 13210.14,-54 13182.75,-50.65 13153.09,-43.87 13127.77,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13128.5,-33.66 13117.93,-34.39 13126.65,-40.41 13128.5,-33.66\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14539.43,-34.39C14513.33,-42.01 14480.79,-50.2 14450.99,-54 14249.29,-79.7 13738.25,-74.82 13535.99,-54 13503.09,-50.61 13467.22,-43.69 13436.71,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13437.11,-33.32 13426.58,-34.49 13435.55,-40.14 13437.11,-33.32\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;vertices(sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node60\" class=\"node\">\n",
-                            "<title>(&#39;vertices(sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13592.14\" cy=\"-18\" rx=\"150.27\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"13592.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;vertices(sentence&#39;, &#39;NOUN&#39;) (0.0053)</text>\n",
+                            "<!-- (&#39;vertices(sentences&#39;, &#39;PROPN&#39;) -->\n",
+                            "<g id=\"node58\" class=\"node\">\n",
+                            "<title>(&#39;vertices(sentences&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14011.99\" cy=\"-18\" rx=\"196.07\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"14011.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;vertices(sentences&#39;, &#39;PROPN&#39;) (0.0056)</text>\n",
                             "</g>\n",
-                            "<!-- (&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;vertices(sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge172\" class=\"edge\">\n",
-                            "<title>(&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;vertices(sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14024.95,-34.29C14002.41,-41.93 13974.18,-50.18 13948.14,-54 13865.47,-66.13 13843.23,-62.8 13760.14,-54 13728.16,-50.61 13693.32,-43.69 13663.7,-36.82\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13664.41,-33.39 13653.87,-34.49 13662.79,-40.2 13664.41,-33.39\"/>\n",
+                            "<!-- (&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;vertices(sentences&#39;, &#39;PROPN&#39;) -->\n",
+                            "<g id=\"edge170\" class=\"edge\">\n",
+                            "<title>(&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;vertices(sentences&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14539.43,-34.39C14513.33,-42.01 14480.79,-50.2 14450.99,-54 14352.23,-66.58 14326.2,-62.25 14226.99,-54 14185.44,-50.55 14139.84,-43.4 14101.37,-36.38\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"14101.7,-32.88 14091.23,-34.5 14100.43,-39.76 14101.7,-32.88\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;high&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"node61\" class=\"node\">\n",
+                            "<g id=\"node59\" class=\"node\">\n",
                             "<title>(&#39;high&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"13854.14\" cy=\"-18\" rx=\"94.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"13854.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;high&#39;, &#39;ADJ&#39;) (0.0068)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14338.99\" cy=\"-18\" rx=\"112.38\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"14338.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;high&#39;, &#39;ADJ&#39;) (0.0072)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;high&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge173\" class=\"edge\">\n",
+                            "<g id=\"edge171\" class=\"edge\">\n",
                             "<title>(&#39;pick&#39;, &#39;VERB&#39;)&#45;&gt;(&#39;high&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13966.35,-18C13963.85,-18 13961.36,-18 13958.86,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13958.6,-14.5 13948.6,-18 13958.6,-21.5 13958.6,-14.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14469.02,-18C14466.68,-18 14464.34,-18 14462,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"14461.74,-14.5 14451.74,-18 14461.74,-21.5 14461.74,-14.5\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;vertices(sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge176\" class=\"edge\">\n",
-                            "<title>(&#39;vertices(sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13530.41,-34.49C13498.88,-42.08 13459.74,-50.23 13424.14,-54 13329.56,-64.02 13304.55,-65.54 13210.14,-54 13182.75,-50.65 13153.09,-43.87 13127.77,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13128.5,-33.66 13117.93,-34.39 13126.65,-40.41 13128.5,-33.66\"/>\n",
+                            "<!-- (&#39;vertices(sentences&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
+                            "<g id=\"edge174\" class=\"edge\">\n",
+                            "<title>(&#39;vertices(sentences&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13933.12,-34.5C13892.88,-42.09 13843.04,-50.24 13797.99,-54 13681.95,-63.69 13651.82,-65.92 13535.99,-54 13503.09,-50.61 13467.22,-43.69 13436.71,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13437.11,-33.32 13426.58,-34.49 13435.55,-40.14 13437.11,-33.32\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;vertices(sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;high&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge175\" class=\"edge\">\n",
-                            "<title>(&#39;vertices(sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;high&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13742.33,-18C13744.79,-18 13747.24,-18 13749.7,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13749.8,-21.5 13759.8,-18 13749.8,-14.5 13749.8,-21.5\"/>\n",
+                            "<!-- (&#39;vertices(sentences&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;high&#39;, &#39;ADJ&#39;) -->\n",
+                            "<g id=\"edge173\" class=\"edge\">\n",
+                            "<title>(&#39;vertices(sentences&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;high&#39;, &#39;ADJ&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14208.38,-18C14211.02,-18 14213.66,-18 14216.31,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"14216.49,-21.5 14226.49,-18 14216.49,-14.5 14216.49,-21.5\"/>\n",
                             "</g>\n",
-                            "<!-- (&#39;vertices(sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge177\" class=\"edge\">\n",
-                            "<title>(&#39;vertices(sentence&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13441.85,-18C13439.21,-18 13436.57,-18 13433.93,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13433.76,-14.5 13423.76,-18 13433.76,-21.5 13433.76,-14.5\"/>\n",
+                            "<!-- (&#39;vertices(sentences&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;) -->\n",
+                            "<g id=\"edge175\" class=\"edge\">\n",
+                            "<title>(&#39;vertices(sentences&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M13815.29,-18C13812.82,-18 13810.35,-18 13807.87,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13807.71,-14.5 13797.71,-18 13807.71,-21.5 13807.71,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;high&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge178\" class=\"edge\">\n",
+                            "<g id=\"edge176\" class=\"edge\">\n",
                             "<title>(&#39;high&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;PageRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13813.92,-34.28C13792.91,-41.92 13766.56,-50.17 13742.14,-54 13625.35,-72.31 13327.49,-68.35 13210.14,-54 13182.75,-50.65 13153.09,-43.87 13127.77,-37.09\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13128.5,-33.66 13117.93,-34.39 13126.65,-40.41 13128.5,-33.66\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14291.41,-34.39C14266.83,-42 14236.16,-50.2 14207.99,-54 14060,-73.96 13684.54,-69.29 13535.99,-54 13503.09,-50.61 13467.22,-43.69 13436.71,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13437.11,-33.32 13426.58,-34.49 13435.55,-40.14 13437.11,-33.32\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;high&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge179\" class=\"edge\">\n",
+                            "<g id=\"edge177\" class=\"edge\">\n",
                             "<title>(&#39;high&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;score&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M13813.92,-34.28C13792.91,-41.92 13766.56,-50.17 13742.14,-54 13610.42,-74.65 13574.17,-72.63 13442.14,-54 13418.77,-50.7 13393.66,-44.1 13372.11,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"13373.07,-34.07 13362.48,-34.38 13370.96,-40.74 13373.07,-34.07\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M14291.41,-34.39C14266.83,-42 14236.16,-50.2 14207.99,-54 14035.33,-77.29 13988.99,-74.6 13815.99,-54 13787.75,-50.64 13757.13,-43.81 13731.03,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"13731.83,-33.59 13721.27,-34.39 13730.03,-40.35 13731.83,-33.59\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;original&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"node63\" class=\"node\">\n",
+                            "<g id=\"node61\" class=\"node\">\n",
                             "<title>(&#39;original&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"11365.14\" cy=\"-18\" rx=\"105.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"11365.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;original&#39;, &#39;ADJ&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"16860.99\" cy=\"-18\" rx=\"128.08\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"16860.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;original&#39;, &#39;ADJ&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;original&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge180\" class=\"edge\">\n",
+                            "<g id=\"edge178\" class=\"edge\">\n",
                             "<title>(&#39;original&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11320.17,-34.38C11296.92,-42 11267.88,-50.2 11241.14,-54 11132.25,-69.49 3431.3,-67.44 3322.14,-54 3294.93,-50.65 3265.47,-43.87 3240.33,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3241.13,-33.68 3230.56,-34.39 3239.27,-40.42 3241.13,-33.68\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M16807.83,-34.39C16780.4,-42.01 16746.22,-50.21 16714.99,-54 16539.74,-75.29 4179.58,-72.28 4003.99,-54 3971.46,-50.61 3936,-43.69 3905.85,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3906.37,-33.35 3895.84,-34.49 3904.79,-40.16 3906.37,-33.35\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;original&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge182\" class=\"edge\">\n",
+                            "<g id=\"edge180\" class=\"edge\">\n",
                             "<title>(&#39;original&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;edge&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11320.17,-34.38C11296.92,-42 11267.88,-50.2 11241.14,-54 11135.65,-69 10387.62,-69.12 10282.14,-54 10259.23,-50.72 10234.63,-44.16 10213.49,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10214.33,-34.12 10203.73,-34.38 10212.18,-40.78 10214.33,-34.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M16807.83,-34.39C16780.4,-42.01 16746.22,-50.21 16714.99,-54 16599.39,-68.04 8446.58,-68.04 8330.99,-54 8303.42,-50.65 8273.55,-43.87 8248.06,-37.09\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8248.72,-33.64 8238.15,-34.39 8246.88,-40.39 8248.72,-33.64\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;original&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;weight&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge181\" class=\"edge\">\n",
+                            "<g id=\"edge179\" class=\"edge\">\n",
                             "<title>(&#39;original&#39;, &#39;ADJ&#39;)&#45;&gt;(&#39;weight&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11320.17,-34.38C11296.92,-42 11267.88,-50.2 11241.14,-54 11132.9,-69.4 10857.48,-68.72 10749.14,-54 10724.78,-50.69 10698.54,-44.04 10676.06,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10676.93,-33.96 10666.35,-34.39 10674.89,-40.65 10676.93,-33.96\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M16807.83,-34.39C16780.4,-42.01 16746.22,-50.21 16714.99,-54 16582.19,-70.13 16245.91,-69.14 16112.99,-54 16083.35,-50.62 16051.15,-43.75 16023.74,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16024.42,-33.47 16013.87,-34.39 16022.69,-40.26 16024.42,-33.47\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;percentage&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;appear&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge183\" class=\"edge\">\n",
+                            "<g id=\"edge181\" class=\"edge\">\n",
                             "<title>(&#39;percentage&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;appear&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11003.14,-18C11005.77,-18 11008.39,-18 11011.02,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11011.14,-21.5 11021.14,-18 11011.14,-14.5 11011.14,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M16429.02,-18C16431.61,-18 16434.21,-18 16436.81,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"16436.83,-21.5 16446.83,-18 16436.83,-14.5 16436.83,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Gensim&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"node66\" class=\"node\">\n",
+                            "<g id=\"node64\" class=\"node\">\n",
                             "<title>(&#39;Gensim&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"14961.14\" cy=\"-18\" rx=\"118.88\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"14961.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Gensim&#39;, &#39;PROPN&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"15655.99\" cy=\"-18\" rx=\"144.87\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"15655.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;Gensim&#39;, &#39;PROPN&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;Gensim&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge184\" class=\"edge\">\n",
+                            "<g id=\"edge182\" class=\"edge\">\n",
                             "<title>(&#39;Gensim&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;TextRank&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14911.33,-34.39C14885.61,-42 14853.53,-50.2 14824.14,-54 14665.71,-74.47 3480.69,-73.52 3322.14,-54 3294.93,-50.65 3265.47,-43.87 3240.33,-37.08\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"3241.13,-33.68 3230.56,-34.39 3239.27,-40.42 3241.13,-33.68\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15596.13,-34.49C15565.54,-42.08 15527.56,-50.23 15492.99,-54 15334.36,-71.31 4162.7,-70.53 4003.99,-54 3971.46,-50.61 3936,-43.69 3905.85,-36.82\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"3906.37,-33.35 3895.84,-34.49 3904.79,-40.16 3906.37,-33.35\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Gensim&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge185\" class=\"edge\">\n",
+                            "<g id=\"edge183\" class=\"edge\">\n",
                             "<title>(&#39;Gensim&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;use&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14911.33,-34.39C14885.61,-42 14853.53,-50.2 14824.14,-54 14712.24,-68.46 6811.7,-70.91 6700.14,-54 6678.46,-50.71 6655.26,-44.16 6635.34,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"6636.44,-34.21 6625.85,-34.28 6634.18,-40.83 6636.44,-34.21\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15596.13,-34.49C15565.54,-42.08 15527.56,-50.23 15492.99,-54 15318.3,-73.06 12504.24,-76.67 12329.99,-54 12304.45,-50.68 12276.88,-43.98 12253.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"12254.01,-33.83 12243.43,-34.39 12252.05,-40.55 12254.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Gensim&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Okapi&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge186\" class=\"edge\">\n",
+                            "<g id=\"edge184\" class=\"edge\">\n",
                             "<title>(&#39;Gensim&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;Okapi&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M14911.33,-34.39C14885.61,-42 14853.53,-50.2 14824.14,-54 14722.18,-67.17 7524.02,-67.74 7422.14,-54 7397.61,-50.69 7371.17,-44.04 7348.51,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7349.3,-33.93 7338.72,-34.39 7347.28,-40.63 7349.3,-33.93\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M15596.13,-34.49C15565.54,-42.08 15527.56,-50.23 15492.99,-54 15382.09,-66.1 11587.81,-66.78 11476.99,-54 11447.84,-50.64 11416.19,-43.81 11389.2,-36.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11390.04,-33.6 11379.49,-34.49 11388.3,-40.37 11390.04,-33.6\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Okapi&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge189\" class=\"edge\">\n",
+                            "<g id=\"edge187\" class=\"edge\">\n",
                             "<title>(&#39;Okapi&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7404.25,-18C7406.87,-18 7409.49,-18 7412.1,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7412.2,-21.5 7422.2,-18 7412.2,-14.5 7412.2,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11266.49,-34.49C11237.6,-42.08 11201.72,-50.23 11168.99,-54 11041.06,-68.75 8978.69,-70.62 8850.99,-54 8825.45,-50.68 8797.88,-43.98 8774.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8775.01,-33.83 8764.43,-34.39 8773.05,-40.55 8775.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Okapi&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;BM25&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge187\" class=\"edge\">\n",
+                            "<g id=\"edge185\" class=\"edge\">\n",
                             "<title>(&#39;Okapi&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;BM25&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7338.72,-34.39C7363.3,-42 7393.98,-50.2 7422.14,-54 7533.6,-69.04 11359.66,-68.93 11471.14,-54 11495.85,-50.69 11522.49,-44.04 11545.32,-37.35\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11546.62,-40.62 11555.19,-34.39 11544.61,-33.91 11546.62,-40.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11459.58,-18C11462.06,-18 11464.53,-18 11467.01,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11467.18,-21.5 11477.18,-18 11467.18,-14.5 11467.18,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Okapi&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;function&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge188\" class=\"edge\">\n",
+                            "<g id=\"edge186\" class=\"edge\">\n",
                             "<title>(&#39;Okapi&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;function&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M7338.72,-34.39C7363.3,-42 7393.98,-50.2 7422.14,-54 7540.38,-69.95 11598.85,-69.5 11717.14,-54 11742.5,-50.68 11769.87,-43.98 11793.29,-37.26\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11794.47,-40.57 11803.07,-34.39 11792.49,-33.85 11794.47,-40.57\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11379.49,-34.49C11408.37,-42.08 11444.26,-50.23 11476.99,-54 11598.85,-68.05 11631.06,-67.47 11752.99,-54 11783.55,-50.63 11816.79,-43.75 11845.09,-36.91\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11846.01,-40.28 11854.88,-34.49 11844.33,-33.49 11846.01,-40.28\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;BM25&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge191\" class=\"edge\">\n",
+                            "<g id=\"edge189\" class=\"edge\">\n",
                             "<title>(&#39;BM25&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11555.19,-34.39C11530.42,-42 11499.51,-50.2 11471.14,-54 11365.5,-68.15 7739.5,-70.11 7634.14,-54 7612.73,-50.73 7589.84,-44.22 7570.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7571.07,-34.23 7560.48,-34.28 7568.79,-40.85 7571.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11558.11,-34.39C11528.78,-42.01 11492.27,-50.21 11458.99,-54 11315.03,-70.4 8994.67,-72.69 8850.99,-54 8825.45,-50.68 8797.88,-43.98 8774.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8775.01,-33.83 8764.43,-34.39 8773.05,-40.55 8775.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;BM25&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge192\" class=\"edge\">\n",
+                            "<g id=\"edge190\" class=\"edge\">\n",
                             "<title>(&#39;BM25&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11555.19,-34.39C11530.42,-42 11499.51,-50.2 11471.14,-54 11364.98,-68.22 10613.15,-69.31 10507.14,-54 10484.4,-50.72 10460,-44.16 10439.04,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10439.95,-34.14 10429.36,-34.38 10437.79,-40.8 10439.95,-34.14\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11558.11,-34.39C11528.78,-42.01 11492.27,-50.21 11458.99,-54 11301.01,-71.99 8754.77,-73.69 8596.99,-54 8570.14,-50.65 8541.09,-43.87 8516.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8517.24,-33.71 8506.66,-34.39 8515.35,-40.45 8517.24,-33.71\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;BM25&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;function&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge190\" class=\"edge\">\n",
+                            "<g id=\"edge188\" class=\"edge\">\n",
                             "<title>(&#39;BM25&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;function&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11716.94,-18C11719.39,-18 11721.84,-18 11724.29,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"11724.37,-21.5 11734.37,-18 11724.37,-14.5 11724.37,-21.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11752.81,-18C11755.24,-18 11757.68,-18 11760.11,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11760.12,-21.5 11770.12,-18 11760.12,-14.5 11760.12,-21.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;function&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;) -->\n",
-                            "<g id=\"edge193\" class=\"edge\">\n",
+                            "<g id=\"edge191\" class=\"edge\">\n",
                             "<title>(&#39;function&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;see&#39;, &#39;VERB&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11803.07,-34.39C11777.73,-42 11746.12,-50.2 11717.14,-54 11604.69,-68.74 7746.26,-71.14 7634.14,-54 7612.73,-50.73 7589.84,-44.22 7570.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"7571.07,-34.23 7560.48,-34.28 7568.79,-40.85 7571.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11854.88,-34.49C11824.66,-42.08 11787.15,-50.23 11752.99,-54 11592.74,-71.7 9010.86,-74.8 8850.99,-54 8825.45,-50.68 8797.88,-43.98 8774.28,-37.26\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8775.01,-33.83 8764.43,-34.39 8773.05,-40.55 8775.01,-33.83\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;function&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge195\" class=\"edge\">\n",
+                            "<g id=\"edge193\" class=\"edge\">\n",
                             "<title>(&#39;function&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;sentence&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11803.07,-34.39C11777.73,-42 11746.12,-50.2 11717.14,-54 11613.91,-67.53 9946.58,-65.85 9843.14,-54 9813.2,-50.57 9780.62,-43.52 9753.1,-36.57\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"9753.76,-33.12 9743.2,-34.02 9752.01,-39.9 9753.76,-33.12\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11854.88,-34.49C11824.66,-42.08 11787.15,-50.23 11752.99,-54 11534.98,-78.08 8023.3,-75.16 7804.99,-54 7769.17,-50.53 7729.97,-43.34 7696.99,-36.29\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"7697.48,-32.82 7686.96,-34.12 7695.99,-39.66 7697.48,-32.82\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;function&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;) -->\n",
-                            "<g id=\"edge194\" class=\"edge\">\n",
+                            "<g id=\"edge192\" class=\"edge\">\n",
                             "<title>(&#39;function&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;similar&#39;, &#39;ADJ&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M11803.07,-34.39C11777.73,-42 11746.12,-50.2 11717.14,-54 11583.84,-71.47 10640.2,-73.22 10507.14,-54 10484.4,-50.72 10460,-44.16 10439.04,-37.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"10439.95,-34.14 10429.36,-34.38 10437.79,-40.8 10439.95,-34.14\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M11854.88,-34.49C11824.66,-42.08 11787.15,-50.23 11752.99,-54 11578.72,-73.25 8770.97,-75.71 8596.99,-54 8570.14,-50.65 8541.09,-43.87 8516.3,-37.08\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"8517.24,-33.71 8506.66,-34.39 8515.35,-40.45 8517.24,-33.71\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;improvement&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"node70\" class=\"node\">\n",
+                            "<g id=\"node68\" class=\"node\">\n",
                             "<title>(&#39;improvement&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6080.14\" cy=\"-18\" rx=\"135.68\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"6080.14\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;improvement&#39;, &#39;NOUN&#39;) (0.0041)</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"6752.99\" cy=\"-18\" rx=\"167.87\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"6752.99\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">(&#39;improvement&#39;, &#39;NOUN&#39;) (0.0044)</text>\n",
                             "</g>\n",
                             "<!-- (&#39;improvement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;) -->\n",
-                            "<g id=\"edge196\" class=\"edge\">\n",
+                            "<g id=\"edge194\" class=\"edge\">\n",
                             "<title>(&#39;improvement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;paper&#39;, &#39;NOUN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6024.02,-34.49C5995.32,-42.08 5959.67,-50.22 5927.14,-54 5802.42,-68.48 4921.48,-71.41 4797.14,-54 4773.6,-50.7 4748.28,-44.1 4726.56,-37.44\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"4727.44,-34.05 4716.85,-34.38 4725.34,-40.72 4727.44,-34.05\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M6684.92,-34.5C6650.17,-42.09 6607.07,-50.23 6567.99,-54 6444.34,-65.92 5573.36,-68.5 5449.99,-54 5421.39,-50.64 5390.36,-43.81 5363.91,-37\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5364.57,-33.55 5354.01,-34.39 5362.79,-40.32 5364.57,-33.55\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;improvement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge198\" class=\"edge\">\n",
+                            "<g id=\"edge196\" class=\"edge\">\n",
                             "<title>(&#39;improvement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M6024.02,-34.49C5995.32,-42.08 5959.67,-50.22 5927.14,-54 5783.22,-70.7 5418.37,-75.89 5275.14,-54 5253.73,-50.73 5230.84,-44.22 5211.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5212.07,-34.23 5201.48,-34.28 5209.79,-40.85 5212.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M6684.92,-34.5C6650.17,-42.09 6607.07,-50.23 6567.99,-54 6448.1,-65.56 6145.44,-69.43 6025.99,-54 6000.16,-50.66 5972.25,-43.93 5948.41,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5949.38,-33.81 5938.8,-34.39 5947.43,-40.53 5949.38,-33.81\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;improvement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Barrios&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge197\" class=\"edge\">\n",
+                            "<g id=\"edge195\" class=\"edge\">\n",
                             "<title>(&#39;improvement&#39;, &#39;NOUN&#39;)&#45;&gt;(&#39;Barrios&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5944.27,-18C5941.83,-18 5939.39,-18 5936.95,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5936.91,-14.5 5926.91,-18 5936.91,-21.5 5936.91,-14.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M6585.28,-18C6582.84,-18 6580.4,-18 6577.96,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"6577.93,-14.5 6567.93,-18 6577.93,-21.5 6577.93,-14.5\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Barrios&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge199\" class=\"edge\">\n",
+                            "<g id=\"edge197\" class=\"edge\">\n",
                             "<title>(&#39;Barrios&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;et&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5759.7,-34.39C5734.17,-42 5702.33,-50.2 5673.14,-54 5585.44,-65.41 5362.57,-67.36 5275.14,-54 5253.73,-50.73 5230.84,-44.22 5211.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5212.07,-34.23 5201.48,-34.28 5209.79,-40.85 5212.07,-34.23\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M6364.5,-34.49C6334.1,-42.08 6296.36,-50.23 6261.99,-54 6157.73,-65.45 6130.01,-67.44 6025.99,-54 6000.16,-50.66 5972.25,-43.93 5948.41,-37.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"5949.38,-33.81 5938.8,-34.39 5947.43,-40.53 5949.38,-33.81\"/>\n",
                             "</g>\n",
                             "<!-- (&#39;Barrios&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge200\" class=\"edge\">\n",
+                            "<g id=\"edge198\" class=\"edge\">\n",
                             "<title>(&#39;Barrios&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;al&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5759.7,-34.39C5734.17,-42 5702.33,-50.2 5673.14,-54 5591.17,-64.67 5568.86,-66.49 5487.14,-54 5465.73,-50.73 5442.84,-44.22 5423.16,-37.62\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5424.07,-34.23 5413.48,-34.28 5421.79,-40.85 5424.07,-34.23\"/>\n",
-                            "</g>\n",
-                            "<!-- (&#39;Barrios&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;.&#39;, &#39;PROPN&#39;) -->\n",
-                            "<g id=\"edge201\" class=\"edge\">\n",
-                            "<title>(&#39;Barrios&#39;, &#39;PROPN&#39;)&#45;&gt;(&#39;.&#39;, &#39;PROPN&#39;)</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M5691.5,-18C5688.73,-18 5685.96,-18 5683.19,-18\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"5683.17,-14.5 5673.17,-18 5683.17,-21.5 5683.17,-14.5\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M6280.06,-18C6277.58,-18 6275.09,-18 6272.61,-18\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"6272.39,-14.5 6262.39,-18 6272.39,-21.5 6272.39,-14.5\"/>\n",
                             "</g>\n",
                             "</g>\n",
                             "</svg>\n"
                         ],
                         "text/plain": [
-                            "<graphviz.files.Source at 0x7fdbd2043ad0>"
+                            "<graphviz.sources.Source at 0x7f0d939857c0>"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2468,30 +2436,29 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: altair in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (4.1.0)\n",
-                        "Requirement already satisfied: entrypoints in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from altair) (0.3)\n",
-                        "Requirement already satisfied: jinja2 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from altair) (3.0.2)\n",
-                        "Requirement already satisfied: toolz in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from altair) (0.11.1)\n",
-                        "Requirement already satisfied: pandas>=0.18 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from altair) (1.3.3)\n",
-                        "Requirement already satisfied: jsonschema in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from altair) (4.1.0)\n",
-                        "Requirement already satisfied: numpy in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from altair) (1.21.2)\n",
-                        "Requirement already satisfied: python-dateutil>=2.7.3 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from pandas>=0.18->altair) (2.8.2)\n",
-                        "Requirement already satisfied: pytz>=2017.3 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from pandas>=0.18->altair) (2021.3)\n",
-                        "Requirement already satisfied: MarkupSafe>=2.0 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from jinja2->altair) (2.0.1)\n",
-                        "Requirement already satisfied: importlib-metadata in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from jsonschema->altair) (4.8.1)\n",
-                        "Requirement already satisfied: attrs>=17.4.0 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from jsonschema->altair) (21.2.0)\n",
-                        "Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from jsonschema->altair) (0.18.0)\n",
-                        "Requirement already satisfied: six>=1.5 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from python-dateutil>=2.7.3->pandas>=0.18->altair) (1.16.0)\n",
-                        "Requirement already satisfied: typing-extensions>=3.6.4 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from importlib-metadata->jsonschema->altair) (3.10.0.2)\n",
-                        "Requirement already satisfied: zipp>=0.5 in /Users/paco/src/pytextrank/venv/lib/python3.7/site-packages (from importlib-metadata->jsonschema->altair) (3.6.0)\n"
+                        "Requirement already satisfied: altair in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (4.2.0)\n",
+                        "Requirement already satisfied: jsonschema>=3.0 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from altair) (4.4.0)\n",
+                        "Requirement already satisfied: jinja2 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from altair) (3.0.3)\n",
+                        "Requirement already satisfied: numpy in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from altair) (1.22.3)\n",
+                        "Requirement already satisfied: entrypoints in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from altair) (0.4)\n",
+                        "Requirement already satisfied: toolz in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from altair) (0.11.2)\n",
+                        "Requirement already satisfied: pandas>=0.18 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from altair) (1.4.1)\n",
+                        "Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from jsonschema>=3.0->altair) (0.18.1)\n",
+                        "Requirement already satisfied: attrs>=17.4.0 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from jsonschema>=3.0->altair) (21.4.0)\n",
+                        "Requirement already satisfied: importlib-resources>=1.4.0; python_version < \"3.9\" in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from jsonschema>=3.0->altair) (5.4.0)\n",
+                        "Requirement already satisfied: MarkupSafe>=2.0 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from jinja2->altair) (2.1.0)\n",
+                        "Requirement already satisfied: pytz>=2020.1 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from pandas>=0.18->altair) (2021.3)\n",
+                        "Requirement already satisfied: python-dateutil>=2.8.1 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from pandas>=0.18->altair) (2.8.2)\n",
+                        "Requirement already satisfied: zipp>=3.1.0; python_version < \"3.10\" in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from importlib-resources>=1.4.0; python_version < \"3.9\"->jsonschema>=3.0->altair) (3.7.0)\n",
+                        "Requirement already satisfied: six>=1.5 in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (from python-dateutil>=2.8.1->pandas>=0.18->altair) (1.16.0)\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install \"altair\""
             ]
         },
@@ -2501,37 +2468,44 @@
             "id": "located-international",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "<div id=\"altair-viz-6d29793142bc4ab2be9ab6ce0a31f62f\"></div>\n",
+                            "<div id=\"altair-viz-1c43da2df37a46868707574f462c9478\"></div>\n",
                             "<script type=\"text/javascript\">\n",
+                            "  var VEGA_DEBUG = (typeof VEGA_DEBUG == \"undefined\") ? {} : VEGA_DEBUG;\n",
                             "  (function(spec, embedOpt){\n",
                             "    let outputDiv = document.currentScript.previousElementSibling;\n",
-                            "    if (outputDiv.id !== \"altair-viz-6d29793142bc4ab2be9ab6ce0a31f62f\") {\n",
-                            "      outputDiv = document.getElementById(\"altair-viz-6d29793142bc4ab2be9ab6ce0a31f62f\");\n",
+                            "    if (outputDiv.id !== \"altair-viz-1c43da2df37a46868707574f462c9478\") {\n",
+                            "      outputDiv = document.getElementById(\"altair-viz-1c43da2df37a46868707574f462c9478\");\n",
                             "    }\n",
                             "    const paths = {\n",
                             "      \"vega\": \"https://cdn.jsdelivr.net/npm//vega@5?noext\",\n",
                             "      \"vega-lib\": \"https://cdn.jsdelivr.net/npm//vega-lib?noext\",\n",
-                            "      \"vega-lite\": \"https://cdn.jsdelivr.net/npm//vega-lite@4.8.1?noext\",\n",
+                            "      \"vega-lite\": \"https://cdn.jsdelivr.net/npm//vega-lite@4.17.0?noext\",\n",
                             "      \"vega-embed\": \"https://cdn.jsdelivr.net/npm//vega-embed@6?noext\",\n",
                             "    };\n",
                             "\n",
-                            "    function loadScript(lib) {\n",
-                            "      return new Promise(function(resolve, reject) {\n",
-                            "        var s = document.createElement('script');\n",
-                            "        s.src = paths[lib];\n",
-                            "        s.async = true;\n",
-                            "        s.onload = () => resolve(paths[lib]);\n",
-                            "        s.onerror = () => reject(`Error loading script: ${paths[lib]}`);\n",
-                            "        document.getElementsByTagName(\"head\")[0].appendChild(s);\n",
-                            "      });\n",
+                            "    function maybeLoadScript(lib, version) {\n",
+                            "      var key = `${lib.replace(\"-\", \"\")}_version`;\n",
+                            "      return (VEGA_DEBUG[key] == version) ?\n",
+                            "        Promise.resolve(paths[lib]) :\n",
+                            "        new Promise(function(resolve, reject) {\n",
+                            "          var s = document.createElement('script');\n",
+                            "          document.getElementsByTagName(\"head\")[0].appendChild(s);\n",
+                            "          s.async = true;\n",
+                            "          s.onload = () => {\n",
+                            "            VEGA_DEBUG[key] = version;\n",
+                            "            return resolve(paths[lib]);\n",
+                            "          };\n",
+                            "          s.onerror = () => reject(`Error loading script: ${paths[lib]}`);\n",
+                            "          s.src = paths[lib];\n",
+                            "        });\n",
                             "    }\n",
                             "\n",
                             "    function showError(err) {\n",
                             "      outputDiv.innerHTML = `<div class=\"error\" style=\"color:red;\">${err}</div>`;\n",
                             "      throw err;\n",
                             "    }\n",
                             "\n",
@@ -2539,24 +2513,22 @@
                             "      vegaEmbed(outputDiv, spec, embedOpt)\n",
                             "        .catch(err => showError(`Javascript Error: ${err.message}<br>This usually means there's a typo in your chart specification. See the javascript console for the full traceback.`));\n",
                             "    }\n",
                             "\n",
                             "    if(typeof define === \"function\" && define.amd) {\n",
                             "      requirejs.config({paths});\n",
                             "      require([\"vega-embed\"], displayChart, err => showError(`Error loading script: ${err.message}`));\n",
-                            "    } else if (typeof vegaEmbed === \"function\") {\n",
-                            "      displayChart(vegaEmbed);\n",
                             "    } else {\n",
-                            "      loadScript(\"vega\")\n",
-                            "        .then(() => loadScript(\"vega-lite\"))\n",
-                            "        .then(() => loadScript(\"vega-embed\"))\n",
+                            "      maybeLoadScript(\"vega\", \"5\")\n",
+                            "        .then(() => maybeLoadScript(\"vega-lite\", \"4.17.0\"))\n",
+                            "        .then(() => maybeLoadScript(\"vega-embed\", \"6\"))\n",
                             "        .catch(showError)\n",
                             "        .then(() => displayChart(vegaEmbed));\n",
                             "    }\n",
-                            "  })({\"config\": {\"view\": {\"continuousWidth\": 400, \"continuousHeight\": 300}}, \"data\": {\"name\": \"data-5a70d50020d6016af92c8759f37c158c\"}, \"mark\": \"bar\", \"encoding\": {\"color\": {\"type\": \"quantitative\", \"field\": \"count\"}, \"tooltip\": [{\"type\": \"nominal\", \"field\": \"text\"}, {\"type\": \"quantitative\", \"field\": \"rank\"}, {\"type\": \"quantitative\", \"field\": \"count\"}], \"x\": {\"type\": \"quantitative\", \"field\": \"index\"}, \"y\": {\"type\": \"quantitative\", \"field\": \"rank\"}}, \"title\": \"Keyphrase profile of the document\", \"$schema\": \"https://vega.github.io/schema/vega-lite/v4.8.1.json\", \"datasets\": {\"data-5a70d50020d6016af92c8759f37c158c\": [{\"index\": 0, \"text\": \"sentences\", \"count\": 1, \"rank\": 0.14407775200046075}, {\"index\": 1, \"text\": \"INELIGIBLE_PHRASE\", \"count\": 21, \"rank\": 0.11286475216345385}, {\"index\": 2, \"text\": \"gensim implements TextRank\", \"count\": 1, \"rank\": 0.09589788430130489}, {\"index\": 3, \"text\": \"text summarization\", \"count\": 1, \"rank\": 0.09004754289053603}, {\"index\": 4, \"text\": \"ranking webpages\", \"count\": 1, \"rank\": 0.08473538778364878}, {\"index\": 5, \"text\": \"every other sentence\", \"count\": 1, \"rank\": 0.07909136977858265}, {\"index\": 6, \"text\": \"Okapi BM25 function\", \"count\": 1, \"rank\": 0.07900911166567022}, {\"index\": 7, \"text\": \"original TextRank\", \"count\": 1, \"rank\": 0.07165073049436399}, {\"index\": 8, \"text\": \"every sentence\", \"count\": 1, \"rank\": 0.06654666312136172}, {\"index\": 9, \"text\": \"the sentences\", \"count\": 1, \"rank\": 0.06654666312136172}, {\"index\": 10, \"text\": \"the popular PageRank algorithm\", \"count\": 1, \"rank\": 0.05335888932629289}, {\"index\": 11, \"text\": \"vertices\", \"count\": 1, \"rank\": 0.049900427583598826}, {\"index\": 12, \"text\": \"implementations\", \"count\": 1, \"rank\": 0.04843744036176572}, {\"index\": 13, \"text\": \"the two sentences\", \"count\": 1, \"rank\": 0.04832514712775797}, {\"index\": 14, \"text\": \"the summarization module\", \"count\": 1, \"rank\": 0.047089290608111706}, {\"index\": 15, \"text\": \"an edge\", \"count\": 2, \"rank\": 0.046108819024674536}, {\"index\": 16, \"text\": \"the edge\", \"count\": 1, \"rank\": 0.046108819024674536}, {\"index\": 17, \"text\": \"an unsupervised algorithm\", \"count\": 1, \"rank\": 0.04590933165691038}, {\"index\": 18, \"text\": \"the highest PageRank score\", \"count\": 1, \"rank\": 0.045894401837491466}, {\"index\": 19, \"text\": \"another incubator student Olavur Mortensen\", \"count\": 1, \"rank\": 0.044786361545027256}, {\"index\": 20, \"text\": \"weighted-graphs\", \"count\": 1, \"rank\": 0.0426755744719463}, {\"index\": 21, \"text\": \"his previous post\", \"count\": 1, \"rank\": 0.04254933225827145}, {\"index\": 22, \"text\": \"the PageRank algorithm\", \"count\": 1, \"rank\": 0.04050691407679936}, {\"index\": 23, \"text\": \"the remaining words\", \"count\": 1, \"rank\": 0.03802068505128614}, {\"index\": 24, \"text\": \"this blog\", \"count\": 1, \"rank\": 0.03778525440103907}, {\"index\": 25, \"text\": \"-\", \"count\": 1, \"rank\": 0.036368977979322474}, {\"index\": 26, \"text\": \"top\", \"count\": 1, \"rank\": 0.036368977979322474}, {\"index\": 27, \"text\": \"some popular algorithms\", \"count\": 1, \"rank\": 0.036106721162100744}, {\"index\": 28, \"text\": \"the percentage\", \"count\": 1, \"rank\": 0.03552664300233543}, {\"index\": 29, \"text\": \"Pre\", \"count\": 1, \"rank\": 0.03210407351764978}, {\"index\": 30, \"text\": \"TextRank\", \"count\": 1, \"rank\": 0.03210407351764978}, {\"index\": 31, \"text\": \"a paper\", \"count\": 2, \"rank\": 0.03024778334849052}, {\"index\": 32, \"text\": \"the text\", \"count\": 1, \"rank\": 0.028412169295393176}, {\"index\": 33, \"text\": \"a graph\", \"count\": 1, \"rank\": 0.024205867965342968}, {\"index\": 34, \"text\": \"the graph\", \"count\": 1, \"rank\": 0.024205867965342968}, {\"index\": 35, \"text\": \"The weight\", \"count\": 1, \"rank\": 0.019436270737826597}, {\"index\": 36, \"text\": \"the weights\", \"count\": 1, \"rank\": 0.019436270737826597}, {\"index\": 37, \"text\": \"the vertices(sentences\", \"count\": 1, \"rank\": 0.01679811138121072}, {\"index\": 38, \"text\": \"an improvement\", \"count\": 1, \"rank\": 0.014828236389998911}, {\"index\": 39, \"text\": \"It\", \"count\": 3, \"rank\": 0.0}, {\"index\": 40, \"text\": \"both\", \"count\": 1, \"rank\": 0.0}, {\"index\": 41, \"text\": \"that\", \"count\": 1, \"rank\": 0.0}, {\"index\": 42, \"text\": \"them\", \"count\": 1, \"rank\": 0.0}, {\"index\": 43, \"text\": \"words\", \"count\": 2, \"rank\": 0.0}]}}, {\"mode\": \"vega-lite\"});\n",
+                            "  })({\"config\": {\"view\": {\"continuousWidth\": 400, \"continuousHeight\": 300}}, \"data\": {\"name\": \"data-5965071246e5cc6f31218c318d02a4a9\"}, \"mark\": \"bar\", \"encoding\": {\"color\": {\"field\": \"count\", \"type\": \"quantitative\"}, \"tooltip\": [{\"field\": \"text\", \"type\": \"nominal\"}, {\"field\": \"rank\", \"type\": \"quantitative\"}, {\"field\": \"count\", \"type\": \"quantitative\"}], \"x\": {\"field\": \"index\", \"type\": \"quantitative\"}, \"y\": {\"field\": \"rank\", \"type\": \"quantitative\"}}, \"title\": \"Keyphrase profile of the document\", \"$schema\": \"https://vega.github.io/schema/vega-lite/v4.17.0.json\", \"datasets\": {\"data-5965071246e5cc6f31218c318d02a4a9\": [{\"index\": 0, \"text\": \"sentences\", \"count\": 1, \"rank\": 0.1490464677880926}, {\"index\": 1, \"text\": \"INELIGIBLE_PHRASE\", \"count\": 23, \"rank\": 0.117318519527749}, {\"index\": 2, \"text\": \"gensim implements TextRank\", \"count\": 1, \"rank\": 0.09816426515530181}, {\"index\": 3, \"text\": \"text summarization\", \"count\": 1, \"rank\": 0.09165889278462461}, {\"index\": 4, \"text\": \"ranking webpages\", \"count\": 1, \"rank\": 0.08457790386936588}, {\"index\": 5, \"text\": \"algorithm\", \"count\": 1, \"rank\": 0.08300479194058319}, {\"index\": 6, \"text\": \"every other sentence\", \"count\": 1, \"rank\": 0.08179233228776425}, {\"index\": 7, \"text\": \"Okapi BM25 function\", \"count\": 1, \"rank\": 0.07919192237459494}, {\"index\": 8, \"text\": \"original TextRank\", \"count\": 1, \"rank\": 0.07346227481329015}, {\"index\": 9, \"text\": \"TextRank\", \"count\": 1, \"rank\": 0.07058237377923389}, {\"index\": 10, \"text\": \"every sentence\", \"count\": 1, \"rank\": 0.06884161463937452}, {\"index\": 11, \"text\": \"the sentences\", \"count\": 1, \"rank\": 0.06884161463937452}, {\"index\": 12, \"text\": \"the popular PageRank algorithm\", \"count\": 1, \"rank\": 0.058972231409406994}, {\"index\": 13, \"text\": \"an unsupervised algorithm\", \"count\": 1, \"rank\": 0.05146145004848928}, {\"index\": 14, \"text\": \"the two sentences\", \"count\": 1, \"rank\": 0.04999170506706116}, {\"index\": 15, \"text\": \"implementations\", \"count\": 1, \"rank\": 0.049247069633071704}, {\"index\": 16, \"text\": \"some popular algorithms\", \"count\": 1, \"rank\": 0.04844800911815122}, {\"index\": 17, \"text\": \"the summarization module\", \"count\": 1, \"rank\": 0.04799616735126701}, {\"index\": 18, \"text\": \"an edge\", \"count\": 2, \"rank\": 0.04736003578863279}, {\"index\": 19, \"text\": \"the edge\", \"count\": 1, \"rank\": 0.04736003578863279}, {\"index\": 20, \"text\": \"weighted-graphs\", \"count\": 1, \"rank\": 0.047282336383492746}, {\"index\": 21, \"text\": \"the highest PageRank score\", \"count\": 1, \"rank\": 0.04718391770797767}, {\"index\": 22, \"text\": \"vertices\", \"count\": 1, \"rank\": 0.04641299033085316}, {\"index\": 23, \"text\": \"his previous post\", \"count\": 1, \"rank\": 0.043598118485007026}, {\"index\": 24, \"text\": \"the remaining words\", \"count\": 1, \"rank\": 0.03901099892577118}, {\"index\": 25, \"text\": \"this blog\", \"count\": 1, \"rank\": 0.038692631750879905}, {\"index\": 26, \"text\": \"-\", \"count\": 1, \"rank\": 0.037391134223308885}, {\"index\": 27, \"text\": \"top\", \"count\": 1, \"rank\": 0.037391134223308885}, {\"index\": 28, \"text\": \"the percentage\", \"count\": 1, \"rank\": 0.03659173939555081}, {\"index\": 29, \"text\": \"a graph\", \"count\": 1, \"rank\": 0.03374212306836418}, {\"index\": 30, \"text\": \"the graph\", \"count\": 1, \"rank\": 0.03374212306836418}, {\"index\": 31, \"text\": \"Pre\", \"count\": 1, \"rank\": 0.0330064018036623}, {\"index\": 32, \"text\": \"a paper\", \"count\": 2, \"rank\": 0.029419087253952227}, {\"index\": 33, \"text\": \"the text\", \"count\": 1, \"rank\": 0.02895327990693777}, {\"index\": 34, \"text\": \"the PageRank\", \"count\": 1, \"rank\": 0.02893422106324092}, {\"index\": 35, \"text\": \"another incubator student\", \"count\": 1, \"rank\": 0.02825035234732957}, {\"index\": 36, \"text\": \"The weight\", \"count\": 1, \"rank\": 0.019503690081504852}, {\"index\": 37, \"text\": \"the weights\", \"count\": 1, \"rank\": 0.019503690081504852}, {\"index\": 38, \"text\": \"the vertices(sentences\", \"count\": 1, \"rank\": 0.017270225127306253}, {\"index\": 39, \"text\": \"an improvement\", \"count\": 1, \"rank\": 0.015245003973060306}, {\"index\": 40, \"text\": \"It\", \"count\": 3, \"rank\": 0.0}, {\"index\": 41, \"text\": \"them\", \"count\": 1, \"rank\": 0.0}, {\"index\": 42, \"text\": \"words\", \"count\": 2, \"rank\": 0.0}]}}, {\"mode\": \"vega-lite\"});\n",
                             "</script>"
                         ],
                         "text/plain": [
                             "alt.Chart(...)"
                         ]
                     },
                     "execution_count": 21,
@@ -2568,78 +2540,102 @@
                 "tr = doc._.textrank\n",
                 "tr.plot_keyphrases()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "administrative-sleeve",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
             "source": [
                 "## Extractive Summarization\n",
                 "\n",
                 "Again, working with the most recent document above, we'll summarize based on its top `15` phrases, yielding its top `5` sentences..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "id": "afraid-retail",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "ic| sent: First, a quick description of some popular algorithms & implementations for text summarization that exist today: the summarization module in gensim implements TextRank, an unsupervised algorithm based on weighted-graphs from a paper by Mihalcea et al.\n",
                         "ic| sent: Gensim\u2019s TextRank uses Okapi BM25 function to see how similar the sentences are.\n",
-                        "ic| sent: Create a graph where vertices are sentences.\n",
                         "ic| sent: It is built on top of the popular PageRank algorithm that Google used for ranking webpages.\n",
-                        "ic| sent: In original TextRank the weights of an edge between two sentences is the percentage of words appearing in both of them.\n"
+                        "ic| sent: Create a graph where vertices are sentences.\n",
+                        "ic| sent: Run the PageRank algorithm on the graph.\n"
                     ]
                 }
             ],
             "source": [
                 "for sent in tr.summary(limit_phrases=15, limit_sentences=5):\n",
                 "    ic(sent)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "02cee695-efab-4264-9738-3f5e9f765bfb",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
             "source": [
                 "## Using TopicRank\n",
                 "\n",
                 "The *TopicRank* enhanced algorithm is simple to use in the `spaCy` pipeline and it supports the other features described above:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "id": "7a77525e-9b74-45ba-af71-21aa8f5849f2",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
             "outputs": [],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"topicrank\");"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "sophisticated-crossing",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
             "source": [
                 "Let's load an example text:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "id": "judicial-andrews",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "\" Chelsea 'opted against' signing Salomon Rond\u00f3n on deadline day.\\n\\nChelsea reportedly opted against signing Salom\u00f3n Rond\u00f3n on deadline day despite their long search for a new centre forward. With Olivier Giroud expected to leave, the Blues targeted Edinson Cavani, Dries Mertens and Moussa Dembele \u2013 only to end up with none of them. According to Telegraph Sport, Dalian Yifang offered Rond\u00f3n to Chelsea only for them to prefer keeping Giroud at the club. Manchester United were also linked with the Venezuela international before agreeing a deal for Shanghai Shenhua striker Odion Ighalo. Manager Frank Lampard made no secret of his transfer window frustration, hinting that to secure top four football he \u2018needed\u2019 signings. Their draw against Leicester on Saturday means they have won just four of the last 13 Premier League matches.\""
                         ]
                     },
@@ -2653,15 +2649,19 @@
                 "text"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
             "id": "96ca4cfe-1dc0-4e81-a2e8-a60ff295bf39",
-            "metadata": {},
+            "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "ic| phrase: Phrase(text='Salomon Rond\u00f3n', chunks=[Salomon Rond\u00f3n, Salom\u00f3n Rond\u00f3n, Rond\u00f3n], count=3, rank=0.07866221348202057)\n",
                         "ic| phrase: Phrase(text='Chelsea', chunks=[Chelsea, Chelsea, Chelsea], count=3, rank=0.06832817272016853)\n",
@@ -2681,36 +2681,129 @@
                 "\n",
                 "for phrase in doc._.phrases[:10]:\n",
                 "    ic(phrase)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "7865c45a",
+            "metadata": {
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
+            "source": [
+                "## Using Biased TextRank\n",
+                "\n",
+                "The *Biased TextRank* enhanced algorithm is simple to use in the `spaCy` pipeline and it supports the other features described above:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 26,
+            "id": "d4d2581b",
+            "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
+            "outputs": [],
+            "source": [
+                "nlp = spacy.load(\"en_core_web_sm\")\n",
+                "nlp.add_pipe(\"biasedtextrank\");"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 27,
+            "id": "a83d4003",
+            "metadata": {
+                "pycharm": {
+                    "name": "#%%\n"
+                },
+                "scrolled": true
+            },
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "ic| phrase: Phrase(text='Leicester', chunks=[Leicester, Leicester], count=2, rank=0.26184834028994514)\n",
+                        "ic| phrase: Phrase(text='Saturday', chunks=[Saturday, Saturday], count=2, rank=0.13938186779355857)\n",
+                        "ic| phrase: Phrase(text='the last 13 Premier League matches', chunks=[the last 13 Premier League matches], count=1, rank=0.12502820319236171)\n",
+                        "ic| phrase: Phrase(text='none', chunks=[none], count=1, rank=1.9498221604845646e-07)\n",
+                        "ic| phrase: Phrase(text='Moussa Dembele', chunks=[Moussa Dembele, Moussa Dembele], count=2, rank=8.640024414329197e-08)\n",
+                        "ic| phrase: Phrase(text='Dries Mertens', chunks=[Dries Mertens, Dries Mertens], count=2, rank=5.152284728493906e-08)\n",
+                        "ic| phrase: Phrase(text='Edinson Cavani', chunks=[Edinson Cavani], count=1, rank=3.076049036231119e-08)\n",
+                        "ic| phrase: Phrase(text='a new centre', chunks=[a new centre], count=1, rank=2.7737546970070932e-08)\n",
+                        "ic| phrase: Phrase(text='deadline day', chunks=[deadline day, deadline day], count=2, rank=1.3752326412669907e-08)\n",
+                        "ic| phrase: Phrase(text='their long search', chunks=[their long search], count=1, rank=1.1267201943238505e-08)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "doc = nlp(text)\n",
+                "\n",
+                "focus = \"Leicester\"\n",
+                "doc._.textrank.change_focus(focus,bias=10.0,  default_bias=0.0)\n",
+                "\n",
+                "for phrase in doc._.phrases[:10]:\n",
+                "    ic(phrase)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
+            "source": [
+                "The top-ranked phrases from *Biased TextRank* are closely related to the \"focus\" item: `Leicester`"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
+            "source": [
+                "## Using PositionRank\n",
+                "\n",
+                "The *PositionRank* enhanced algorithm is simple to use in the `spaCy` pipeline and it supports the other features described above:"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "inner-acceptance",
             "metadata": {},
             "source": [
                 "## Using PositionRank\n",
                 "\n",
                 "The *PositionRank* enhanced algorithm is simple to use in the `spaCy` pipeline and it supports the other features described above:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 28,
             "id": "stock-millennium",
             "metadata": {},
             "outputs": [],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"positionrank\");"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 29,
             "id": "compact-retention",
             "metadata": {
                 "scrolled": true,
                 "tags": []
             },
             "outputs": [
                 {
@@ -2753,15 +2846,15 @@
                 "## Baseline\n",
                 "\n",
                 "Now let's re-run this pipeline with the baseline *TextRank* algorithm to compare results:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 30,
             "id": "unique-domestic",
             "metadata": {
                 "scrolled": true,
                 "tags": []
             },
             "outputs": [
                 {
@@ -2769,19 +2862,19 @@
                     "output_type": "stream",
                     "text": [
                         "ic| phrase: Phrase(text='Shanghai Shenhua striker Odion Ighalo', chunks=[Shanghai Shenhua striker Odion Ighalo], count=1, rank=0.11863090071749424)\n",
                         "ic| phrase: Phrase(text='Odion Ighalo', chunks=[Odion Ighalo], count=1, rank=0.10925286108900635)\n",
                         "ic| phrase: Phrase(text='none', chunks=[none], count=1, rank=0.09802416183300769)\n",
                         "ic| phrase: Phrase(text='Moussa Dembele', chunks=[Moussa Dembele, Moussa Dembele], count=2, rank=0.09341044332809736)\n",
                         "ic| phrase: Phrase(text='deadline day', chunks=[deadline day, deadline day], count=2, rank=0.09046182507994752)\n",
-                        "ic| phrase: Phrase(text='Dries Mertens', chunks=[Dries Mertens], count=1, rank=0.08919649435994934)\n",
-                        "ic| phrase: Phrase(text='Edinson Cavani', chunks=[Edinson Cavani, Edinson Cavani], count=2, rank=0.08418633972470349)\n",
+                        "ic| phrase: Phrase(text='Dries Mertens', chunks=[Dries Mertens, Dries Mertens], count=2, rank=0.08919649435994934)\n",
+                        "ic| phrase: Phrase(text='Edinson Cavani', chunks=[Edinson Cavani], count=1, rank=0.08418633972470349)\n",
+                        "ic| phrase: Phrase(text='Shanghai Shenhua', chunks=[Shanghai Shenhua], count=1, rank=0.08254442709505862)\n",
                         "ic| phrase: Phrase(text='Salomon Rond\u00f3n', chunks=[Salomon Rond\u00f3n, Salomon Rond\u00f3n], count=2, rank=0.08228367707127111)\n",
-                        "ic| phrase: Phrase(text='Salom\u00f3n Rond\u00f3n', chunks=[Salom\u00f3n Rond\u00f3n, Salom\u00f3n Rond\u00f3n], count=2, rank=0.08228367707127111)\n",
-                        "ic| phrase: Phrase(text='Premier League', chunks=[Premier League], count=1, rank=0.08198820712767878)\n"
+                        "ic| phrase: Phrase(text='Salom\u00f3n Rond\u00f3n', chunks=[Salom\u00f3n Rond\u00f3n, Salom\u00f3n Rond\u00f3n], count=2, rank=0.08228367707127111)\n"
                     ]
                 }
             ],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"textrank\")\n",
                 "doc = nlp(text)\n",
@@ -2811,13 +2904,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.9"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pytextrank-3.2.4/examples/explain_algo.ipynb` & `pytextrank-3.2.5/examples/explain_algo.ipynb`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/examples/explain_summ.ipynb` & `pytextrank-3.2.5/examples/explain_summ.ipynb`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/examples/sample.ipynb` & `pytextrank-3.2.5/examples/.ipynb_checkpoints/sample-checkpoint.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958003422579847%*

 * *Differences: {"'cells'": '{7: {\'outputs\': {1: {\'data\': {\'text/plain\': {insert: [(43, " \'attrs\': '*

 * *            '{\'token.ent_iob\': {\'assigns\': [\'ner\'], \'requires\': []},\\n"), (44, "  '*

 * *            '\'token.tag\': {\'assigns\': [\'tagger\'], \'requires\': []},\\n"), (45, "  '*

 * *            '\'doc.sents\': {\'assigns\': [\'parser\'], \'requires\': []},\\n"), (47, "  '*

 * *            '\'token.dep\': {\'assigns\': [\'parser\'], \'requires\': []},\\n"), (49, "  '*

 * *            '\'token.ent_type\': {\'assigns\': [\'ner […]*

```diff
@@ -169,24 +169,24 @@
                             " 'problems': {'tok2vec': [],\n",
                             "  'tagger': [],\n",
                             "  'parser': [],\n",
                             "  'attribute_ruler': [],\n",
                             "  'lemmatizer': [],\n",
                             "  'ner': [],\n",
                             "  'textrank': []},\n",
-                            " 'attrs': {'token.dep': {'assigns': ['parser'], 'requires': []},\n",
-                            "  'token.ent_type': {'assigns': ['ner'], 'requires': []},\n",
+                            " 'attrs': {'token.ent_iob': {'assigns': ['ner'], 'requires': []},\n",
+                            "  'token.tag': {'assigns': ['tagger'], 'requires': []},\n",
+                            "  'doc.sents': {'assigns': ['parser'], 'requires': []},\n",
                             "  'token.head': {'assigns': ['parser'], 'requires': []},\n",
-                            "  'token.is_sent_start': {'assigns': ['parser'], 'requires': []},\n",
-                            "  'token.ent_iob': {'assigns': ['ner'], 'requires': []},\n",
+                            "  'token.dep': {'assigns': ['parser'], 'requires': []},\n",
                             "  'doc.tensor': {'assigns': ['tok2vec'], 'requires': []},\n",
-                            "  'doc.ents': {'assigns': ['ner'], 'requires': []},\n",
-                            "  'doc.sents': {'assigns': ['parser'], 'requires': []},\n",
+                            "  'token.ent_type': {'assigns': ['ner'], 'requires': []},\n",
                             "  'token.lemma': {'assigns': ['lemmatizer'], 'requires': []},\n",
-                            "  'token.tag': {'assigns': ['tagger'], 'requires': []}}}"
+                            "  'token.is_sent_start': {'assigns': ['parser'], 'requires': []},\n",
+                            "  'doc.ents': {'assigns': ['ner'], 'requires': []}}}"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -272,15 +272,15 @@
             "id": "adaptive-paper",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| tr.elapsed_time: 7.581949234008789\n"
+                        "ic| tr.elapsed_time: 13.625860214233398\n"
                     ]
                 }
             ],
             "source": [
                 "tr = doc._.textrank\n",
                 "ic(tr.elapsed_time);"
             ]
@@ -302,107 +302,111 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase.rank: 0.18359439311764025\n",
+                        "ic| phrase.rank: 0.17054248030845812\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'mixed types'\n",
                         "ic| phrase.chunks: [mixed types]\n",
-                        "ic| phrase.rank: 0.1784796193107821\n",
-                        "    phrase.count: 3\n",
-                        "    phrase.text: 'systems'\n",
-                        "ic| phrase.chunks: [systems, systems, systems]\n",
-                        "ic| phrase.rank: 0.15037838042245094\n",
+                        "ic| phrase.rank: 0.15757771579579002\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'minimal generating sets'\n",
                         "ic| phrase.chunks: [minimal generating sets]\n",
-                        "ic| phrase.rank: 0.14740065982407313\n",
+                        "ic| phrase.rank: 0.1573942320091846\n",
+                        "    phrase.count: 3\n",
+                        "    phrase.text: 'systems'\n",
+                        "ic| phrase.chunks: [systems, systems, systems]\n",
+                        "ic| phrase.rank: 0.14894241299658317\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'nonstrict inequations'\n",
                         "ic| phrase.chunks: [nonstrict inequations]\n",
-                        "ic| phrase.rank: 0.13946027725597837\n",
+                        "ic| phrase.rank: 0.14039169904589088\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'strict inequations'\n",
                         "ic| phrase.chunks: [strict inequations]\n",
-                        "ic| phrase.rank: 0.1195023546245721\n",
-                        "    phrase.count: 1\n",
-                        "    phrase.text: 'linear Diophantine equations'\n",
-                        "ic| phrase.chunks: [linear Diophantine equations]\n",
-                        "ic| phrase.rank: 0.11450088293222845\n",
+                        "ic| phrase.rank: 0.11698198658021898\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'natural numbers'\n",
                         "ic| phrase.chunks: [natural numbers]\n",
-                        "ic| phrase.rank: 0.10780718173686318\n",
+                        "ic| phrase.rank: 0.11559770516796158\n",
+                        "    phrase.count: 1\n",
+                        "    phrase.text: 'linear Diophantine equations'\n",
+                        "ic| phrase.chunks: [linear Diophantine equations]\n",
+                        "ic| phrase.rank: 0.11407086615794945\n",
                         "    phrase.count: 3\n",
                         "    phrase.text: 'solutions'\n",
                         "ic| phrase.chunks: [solutions, solutions, solutions]\n",
-                        "ic| phrase.rank: 0.10529828014583348\n",
+                        "ic| phrase.rank: 0.10165710454752863\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'linear constraints'\n",
                         "ic| phrase.chunks: [linear constraints]\n",
-                        "ic| phrase.rank: 0.1036960590708142\n",
-                        "    phrase.count: 1\n",
-                        "    phrase.text: 'all the considered types systems'\n",
-                        "ic| phrase.chunks: [all the considered types systems]\n",
-                        "ic| phrase.rank: 0.08812713074893187\n",
+                        "ic| phrase.rank: 0.09237587396226833\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'a minimal supporting set'\n",
                         "ic| phrase.chunks: [a minimal supporting set]\n",
-                        "ic| phrase.rank: 0.08243620500315359\n",
+                        "ic| phrase.rank: 0.08845296671843554\n",
                         "    phrase.count: 1\n",
-                        "    phrase.text: 'a system'\n",
-                        "ic| phrase.chunks: [a system]\n",
-                        "ic| phrase.rank: 0.07944607954086784\n",
+                        "    phrase.text: 'all the considered types systems'\n",
+                        "ic| phrase.chunks: [all the considered types systems]\n",
+                        "ic| phrase.rank: 0.08294839224739124\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'a minimal set'\n",
                         "ic| phrase.chunks: [a minimal set]\n",
-                        "ic| phrase.rank: 0.0763527926213032\n",
+                        "ic| phrase.rank: 0.08107274369298882\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'algorithms'\n",
                         "ic| phrase.chunks: [algorithms]\n",
-                        "ic| phrase.rank: 0.07593126037016427\n",
+                        "ic| phrase.rank: 0.07429406639612553\n",
                         "    phrase.count: 1\n",
-                        "    phrase.text: 'all types'\n",
-                        "ic| phrase.chunks: [all types]\n",
-                        "ic| phrase.rank: 0.07309361902551355\n",
+                        "    phrase.text: 'construction'\n",
+                        "ic| phrase.chunks: [construction]\n",
+                        "ic| phrase.rank: 0.07269728177551771\n",
+                        "    phrase.count: 1\n",
+                        "    phrase.text: 'a system'\n",
+                        "ic| phrase.chunks: [a system]\n",
+                        "ic| phrase.rank: 0.07130948853545689\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'Diophantine'\n",
                         "ic| phrase.chunks: [Diophantine]\n",
-                        "ic| phrase.rank: 0.0702090100898443\n",
+                        "ic| phrase.rank: 0.07034880604533804\n",
                         "    phrase.count: 1\n",
-                        "    phrase.text: 'construction'\n",
-                        "ic| phrase.chunks: [construction]\n",
-                        "ic| phrase.rank: 0.05800111772673988\n",
+                        "    phrase.text: 'all types'\n",
+                        "ic| phrase.chunks: [all types]\n",
+                        "ic| phrase.rank: 0.06480303503167001\n",
+                        "    phrase.count: 1\n",
+                        "    phrase.text: 'Upper bounds'\n",
+                        "ic| phrase.chunks: [Upper bounds]\n",
+                        "ic| phrase.rank: 0.05969087234318076\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'the set'\n",
                         "ic| phrase.chunks: [the set]\n",
-                        "ic| phrase.rank: 0.054251394765316464\n",
+                        "ic| phrase.rank: 0.05837512270115124\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'components'\n",
                         "ic| phrase.chunks: [components]\n",
-                        "ic| phrase.rank: 0.04516904342912139\n",
+                        "ic| phrase.rank: 0.048602276273752514\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'Compatibility'\n",
                         "ic| phrase.chunks: [Compatibility]\n",
-                        "ic| phrase.rank: 0.04516904342912139\n",
+                        "ic| phrase.rank: 0.048602276273752514\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'compatibility'\n",
                         "ic| phrase.chunks: [compatibility]\n",
-                        "ic| phrase.rank: 0.04435648606848154\n",
+                        "ic| phrase.rank: 0.0472624878442175\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'the corresponding algorithms'\n",
                         "ic| phrase.chunks: [the corresponding algorithms]\n",
-                        "ic| phrase.rank: 0.042273783712246285\n",
+                        "ic| phrase.rank: 0.04548690742119631\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'Criteria'\n",
                         "ic| phrase.chunks: [Criteria]\n",
-                        "ic| phrase.rank: 0.01952542432474353\n",
+                        "ic| phrase.rank: 0.021009502595385022\n",
                         "    phrase.count: 1\n",
                         "    phrase.text: 'These criteria'\n",
                         "ic| phrase.chunks: [These criteria]\n"
                     ]
                 }
             ],
             "source": [
@@ -437,24 +441,24 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='words', chunks=[words, words], count=2, rank=0.16137018222637944)\n",
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.13367291641220508)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.1095023226326187)\n",
-                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.10745197034799042)\n",
-                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.10502825160040344)\n",
-                        "ic| phrase: Phrase(text='the remaining words', chunks=[the remaining words], count=1, rank=0.09559863808781449)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09162794519014893)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.08555365347028678)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.07894442579092492)\n",
-                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.07747520663125698)\n"
+                        "ic| phrase: Phrase(text='words', chunks=[words, words], count=2, rank=0.15746606699141763)\n",
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.12965916420829138)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.10571655249620954)\n",
+                        "ic| phrase: Phrase(text='the remaining words', chunks=[the remaining words], count=1, rank=0.09329379463860477)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.08981955768260336)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.0843351188899575)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.07936404910104827)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07400094270083186)\n",
+                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.07073416034725326)\n",
+                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.06710956557420322)\n"
                     ]
                 }
             ],
             "source": [
                 "text = pathlib.Path(\"../dat/gen.txt\").read_text()\n",
                 "doc = nlp(text)\n",
                 "\n",
@@ -480,24 +484,24 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.1490464677880926)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.117318519527749)\n",
-                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.11512161354108796)\n",
-                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.11252482346188267)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09816426515530181)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09165889278462461)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08457790386936588)\n",
-                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.08300479194058319)\n",
-                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.08179233228776425)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07919192237459494)\n"
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences], count=1, rank=0.14407775200046075)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.11286475216345385)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09589788430130489)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09004754289053603)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08473538778364878)\n",
+                        "ic| phrase: Phrase(text='every other sentence', chunks=[every other sentence], count=1, rank=0.07909136977858265)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07900911166567022)\n",
+                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07165073049436399)\n",
+                        "ic| phrase: Phrase(text='TextRank', chunks=[TextRank, TextRank, TextRank, TextRank], count=4, rank=0.06888311869751775)\n",
+                        "ic| phrase: Phrase(text='every sentence', chunks=[every sentence], count=1, rank=0.06654666312136172)\n"
                     ]
                 }
             ],
             "source": [
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "nlp.add_pipe(\"textrank\", config={ \"stopwords\": { \"word\": [\"NOUN\"] } })\n",
                 "\n",
@@ -523,44 +527,47 @@
                 "## Scrubber\n",
                 "\n",
                 "Observe how different variations of \"sentence\", like \"every sentence\" and \"every other sentence\", as well as variations of \"sentences\", occur in phrase list. You can omit such variations by passing a scrubber function in the config."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "id": "living-cholesterol",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "ic| phrase: Phrase(text='sentences', chunks=[sentences, the sentences], count=2, rank=0.1490464677880926)\n",
-                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.117318519527749)\n",
-                        "ic| phrase: Phrase(text='et al', chunks=[et al], count=1, rank=0.11512161354108796)\n",
-                        "ic| phrase: Phrase(text='Barrios et al', chunks=[Barrios et al], count=1, rank=0.11252482346188267)\n",
-                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09816426515530181)\n",
-                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09165889278462461)\n",
-                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08457790386936588)\n",
-                        "ic| phrase: Phrase(text='algorithm', chunks=[algorithm], count=1, rank=0.08300479194058319)\n",
-                        "ic| phrase: Phrase(text='sentence', chunks=[every sentence, every other sentence], count=2, rank=0.08179233228776425)\n",
-                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07919192237459494)\n"
+                        "ic| phrase: Phrase(text='sentences', chunks=[sentences, the two sentences, two sentences, the sentences], count=4, rank=0.14407775200046075)\n",
+                        "ic| phrase: Phrase(text='Mihalcea et al', chunks=[Mihalcea et al], count=1, rank=0.11286475216345385)\n",
+                        "ic| phrase: Phrase(text='gensim implements TextRank', chunks=[gensim implements TextRank], count=1, rank=0.09589788430130489)\n",
+                        "ic| phrase: Phrase(text='text summarization', chunks=[text summarization], count=1, rank=0.09004754289053603)\n",
+                        "ic| phrase: Phrase(text='ranking webpages', chunks=[ranking webpages], count=1, rank=0.08473538778364878)\n",
+                        "ic| phrase: Phrase(text='sentence', chunks=[every sentence, every other sentence], count=2, rank=0.07909136977858265)\n",
+                        "ic| phrase: Phrase(text='Okapi BM25 function', chunks=[Okapi BM25 function], count=1, rank=0.07900911166567022)\n",
+                        "ic| phrase: Phrase(text='original TextRank', chunks=[original TextRank], count=1, rank=0.07165073049436399)\n",
+                        "ic| phrase: Phrase(text='TextRank', chunks=[TextRank, TextRank, TextRank, TextRank], count=4, rank=0.06888311869751775)\n",
+                        "ic| phrase: Phrase(text='Olavur Mortensen', chunks=[Olavur Mortensen], count=1, rank=0.06451292345779545)\n"
                     ]
                 }
             ],
             "source": [
                 "from spacy.tokens import Span\n",
                 "nlp = spacy.load(\"en_core_web_sm\")\n",
                 "\n",
                 "\n",
+                "# \"every\", \"other\", \"the\", \"two\"\n",
+                "# \"a\", \"the\", \"their\", \"every\", \"other\"\n",
+                "\n",
                 "@spacy.registry.misc(\"prefix_scrubber\")\n",
                 "def prefix_scrubber():\n",
                 "\tdef scrubber_func(span: Span) -> str:\n",
-                "\t\twhile span[0].text in (\"a\", \"the\", \"their\", \"every\", \"other\"):\n",
+                "\t\twhile len(span) > 1 and span[0].text in (\"every\", \"other\", \"the\", \"two\"):\n",
                 "\t\t\tspan = span[1:]\n",
                 "\t\treturn span.text\n",
                 "\treturn scrubber_func\n",
                 "\n",
                 "nlp.add_pipe(\"textrank\", config={ \"stopwords\": { \"word\": [\"NOUN\"] }, \"scrubber\": {\"@misc\": \"prefix_scrubber\"}})\n",
                 "\n",
                 "doc = nlp(text)\n",
@@ -578,15 +585,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a123e0fa-c594-4b8c-9ca3-4d3205c2662a",
             "metadata": {},
             "source": [
-                "As the scrubber takes in `Spans`, we can also use `toekn.pos_` or any other spaCy `Token` or `Span` attribute in the scrubbing. The variations of \"sentences\" have different DETs (determiners), so we could achieve a similar result with the folowing scrubber."
+                "As the scrubber takes in `Spans`, we can also use `token.pos_` or any other spaCy `Token` or `Span` attribute in the scrubbing. The variations of \"sentences\" have different DETs (determiners), so we could achieve a similar result with the folowing scrubber."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "49bc498c-8bbe-4c41-8619-35f8f74ef608",
             "metadata": {},
@@ -721,15 +728,15 @@
             "id": "classical-fairy",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "-rw-rw-r-- 1 ankushchander ankushchander 17K Jun  4 11:56 lemma_graph.dot\r\n"
+                        "-rw-rw-r-- 1 ankushchander ankushchander 17K Jun  4 11:56 lemma_graph.dot\n"
                     ]
                 }
             ],
             "source": [
                 "!ls -lth lemma_graph.dot"
             ]
         },
@@ -741,15 +748,15 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: graphviz in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (0.19.1)\r\n"
+                        "Requirement already satisfied: graphviz in /home/ankushchander/workplace/.virtualenv/pytextrank/lib/python3.8/site-packages (0.19.1)\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install graphviz"
             ]
         },
@@ -2748,28 +2755,28 @@
                 "\n",
                 "for phrase in doc._.phrases[:10]:\n",
                 "    ic(phrase)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "28adba98",
             "metadata": {
-                "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "The top-ranked phrases from *Biased TextRank* are closely related to the \"focus\" item: `Leicester`"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "767be008",
             "metadata": {
-                "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "## Using PositionRank\n",
                 "\n",
@@ -2904,13 +2911,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.7.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pytextrank-3.2.4/lgtm.yml` & `pytextrank-3.2.5/lgtm.yml`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/meta.yaml` & `pytextrank-3.2.5/meta.yaml`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/mkdocs.yml` & `pytextrank-3.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pkg_doc.py` & `pytextrank-3.2.5/pkg_doc.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pyfixdoc.py` & `pytextrank-3.2.5/pyfixdoc.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pylintrc` & `pytextrank-3.2.5/pylintrc`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/__init__.py` & `pytextrank-3.2.5/pytextrank/__init__.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/base.py` & `pytextrank-3.2.5/pytextrank/base.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/biasedrank.py` & `pytextrank-3.2.5/pytextrank/biasedrank.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/positionrank.py` & `pytextrank-3.2.5/pytextrank/positionrank.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/topicrank.py` & `pytextrank-3.2.5/pytextrank/topicrank.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/util.py` & `pytextrank-3.2.5/pytextrank/util.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/pytextrank/version.py` & `pytextrank-3.2.5/pytextrank/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing
 
 
 ######################################################################
 ## Python version checking
 
 MIN_PY_VERSION: typing.Tuple = (3, 7,)
-__version__: str = "3.2.4"
+__version__: str = "3.2.5"
 
 
 def _versify (
     py_version_info: typing.Tuple
     ) -> str:
     """
 Semiprivate helper function to convert Python version to a point release (a string).
```

### Comparing `pytextrank-3.2.4/pytextrank.egg-info/SOURCES.txt` & `pytextrank-3.2.5/pytextrank.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 code_of_conduct.md
 environment.yml
 error.py
+foo.py
 lgtm.yml
 meta.yaml
 mkdocs.yml
 pkg_doc.py
 pyfixdoc.py
 pylintrc
 requirements-dev.txt
```

### Comparing `pytextrank-3.2.4/ru.py` & `pytextrank-3.2.5/ru.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/sample.py` & `pytextrank-3.2.5/sample.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/setup.py` & `pytextrank-3.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tests/conftest.py` & `pytextrank-3.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tests/test_base.py` & `pytextrank-3.2.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tests/test_biasedrank.py` & `pytextrank-3.2.5/tests/test_biasedrank.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tests/test_positionrank.py` & `pytextrank-3.2.5/tests/test_positionrank.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tests/test_topicrank.py` & `pytextrank-3.2.5/tests/test_topicrank.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tests/trace.py` & `pytextrank-3.2.5/tests/trace.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/tmp_api.py` & `pytextrank-3.2.5/tmp_api.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/udpipe.py` & `pytextrank-3.2.5/udpipe.py`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/wip/.ipynb_checkpoints/error-checkpoint.ipynb` & `pytextrank-3.2.5/wip/.ipynb_checkpoints/error-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pytextrank-3.2.4/wip/error.ipynb` & `pytextrank-3.2.5/wip/error.ipynb`

 * *Files identical despite different names*

