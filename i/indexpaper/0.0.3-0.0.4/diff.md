# Comparing `tmp/indexpaper-0.0.3.tar.gz` & `tmp/indexpaper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexpaper-0.0.3.tar", last modified: Sun Aug  6 15:52:50 2023, max compression
+gzip compressed data, was "indexpaper-0.0.4.tar", last modified: Mon Aug  7 17:16:08 2023, max compression
```

## Comparing `indexpaper-0.0.3.tar` & `indexpaper-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-06 15:52:50.535092 indexpaper-0.0.3/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    11357 2023-07-29 22:10:33.000000 indexpaper-0.0.3/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5838 2023-08-06 15:52:50.535092 indexpaper-0.0.3/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5178 2023-08-06 15:21:25.000000 indexpaper-0.0.3/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-06 15:52:50.535092 indexpaper-0.0.3/indexpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5838 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      232 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       47 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      172 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-08-06 15:52:50.535092 indexpaper-0.0.3/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1538 2023-08-06 14:56:02.000000 indexpaper-0.0.3/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-07 17:16:08.893240 indexpaper-0.0.4/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    11357 2023-07-29 22:10:33.000000 indexpaper-0.0.4/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6777 2023-08-07 17:16:08.893240 indexpaper-0.0.4/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6117 2023-08-07 17:12:25.000000 indexpaper-0.0.4/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-07 17:16:08.893240 indexpaper-0.0.4/indexpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6777 2023-08-07 17:16:08.000000 indexpaper-0.0.4/indexpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      232 2023-08-07 17:16:08.000000 indexpaper-0.0.4/indexpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-07 17:16:08.000000 indexpaper-0.0.4/indexpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       47 2023-08-07 17:16:08.000000 indexpaper-0.0.4/indexpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      172 2023-08-07 17:16:08.000000 indexpaper-0.0.4/indexpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-07 17:16:08.000000 indexpaper-0.0.4/indexpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-08-07 17:16:08.893240 indexpaper-0.0.4/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1538 2023-08-07 17:03:33.000000 indexpaper-0.0.4/setup.py
```

### Comparing `indexpaper-0.0.3/LICENSE` & `indexpaper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indexpaper-0.0.3/PKG-INFO` & `indexpaper-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,76 @@
-Metadata-Version: 2.1
-Name: indexpaper
-Version: 0.0.3
-Summary: indexpaper - library to index papers with vector databases
-Author: antonkulaga (Anton Kulaga)
-Author-email: <antonkulaga@gmail.com>
-Keywords: python,utils,files,papers,download,index,vector databases
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # indexpaper
+
 The project devoted to indexing papers in vector databases
 
 It was originally part of getpaper but now has not dependencies on it
 
-We provide features to index the papers with openai or llama embeddings and save them in chromadb vector store.
+We provide features to index the papers as well as semantic-scholar paper datasets with openai, huggingface or llama embeddings and save them either chromadb or qdrant vector store.
+
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 
+# getting started
+
+Install the library with:
+```bash
+pip install getpaper
+```
+
+On linux systems you sometimes need to check that build--essential are installed:
+```bash
+sudo apt install build-essential
+```
+It is also recommended to use micromamba, conda, anaconda or other environments to avoid bloating system python with too many dependencies.
+Assuming you installed [micromamba](https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html), you will have to create an environment and enable the library locally
+```
+micromamba create -f environment.yaml
+micromabma activate indexpaper
+pip install -e .
+```
+The last command is optional. With conda/anaconda the commands will look the same but with another name of executable.
+
+## Running local Qdrant
+
+We provide docker-compose configuration to run local qdrant (you can also use qdrant cloud instead).
+To run local qdrant install docker compose (sometimes needs sudo) and run:
+```bash
+cd services
+docker compose up
+```
+Then you should be able to see  http://localhost:6333/dashboard
+
+# Additional requirements
+
+index.py has local dependencies on other modules, for this reason if you are running it inside indexpaper project folder consider having it installed locally:
+```bash
+pip install -e .
+```
+
+# indexing a dataset
+
+To index a dataset you can use either index.py dataset subcommand or you look how to do it in code in papers.ipynb example notebook
+For example, if we want to index "longevity-genie/tacutu_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "cuda" as device and with 10 papers in a slice.
+And we want to write it to the local version of qdrant located at http://localhost:6333 (see services for docker-compose file):
+```bash
+python indexpaper/index.py dataset --collection biolinkbert_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --url http://localhost:6333 --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
+```
+
+Another example. If we want to index "longevity-genie/moskalev_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "gpu" as device and with 10 papers in a slice.
+And we want to use our Qdrant cloud key (fill in QDRANT_KEY or put it to environment variable)
+```bash
+python indexpaper/index.py dataset --collection biolinkbert_512_moskalev_papers --dataset "longevity-genie/moskalev_papers" --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key QDRANT_KEY --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
+```
+Another example. Robi Tacutu papers with cpu using QDRANT_KEY, cluster url (put yours) and michiyasunaga/BioLinkBERT-large embeddings model:
+```
+python indexpaper/index.py dataset --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --collection biolord_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --key QDRANT_KEY --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cpu
+```
+If you want to recreate the collection from scretch you can also add --rewrite true
+
+# Indexing papers
+
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 indexpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 It is possible to use both Chroma and Qdrant. To use qdrant we provide docker-compose file to set it up:
 ```bash
@@ -67,43 +110,7 @@
 ```bash
 python example.py evaluate --model intfloat/multilingual-e5-large --dataset longevity-genie/tacutu_papers
 ```
 To measure time
 ```bash
 python example.py measure --model intfloat/multilingual-e5-large --dataset longevity-genie/tacutu_papers
 ```
-
-# indexing a dataset
-
-To index a dataset you can use either index.py dataset subcomment or you look how to do it in code in papers.ipynb example notebook
-For example, if we want to index "longevity-genie/tacutu_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "cuda" as device and with 10 papers in a slice.
-And we want to write it to the local version of qdrant located at http://localhost:6333 (see services for docker-compose file):
-```bash
-python indexpaper/index.py dataset --collection biolinkbert_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --url http://localhost:6333 --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
-```
-
-Another example. If we want to index "longevity-genie/moskalev_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "gpu" as device and with 10 papers in a slice.
-And we want to use our Qdrant cloud key (fill in QDRANT_KEY or put it to environment variable)
-```bash
-python indexpaper/index.py dataset --collection biolinkbert_512_moskalev_papers --dataset "longevity-genie/moskalev_papers" --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key QDRANT_KEY --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
-```
-Another example. Robi Tacutu papers with cpu using QDRANT_KEY, cluster url (put yours) and biolord embeddings model:
-```
-python indexpaper/index.py dataset --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io --collection biolord_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --key QDRANT_KEY --model FremyCompany/BioLORD-STAMB2-v1 --slice 10 --chunk_size 512 --device cpu
-```
-
-# Runnning local Qdrant
-
-We provide docker-compose configuration to run local qdrant (you can also use qdrant cloud instead).
-To run local qdrant install docker compose (sometimes needs sudo) and run:
-```bash
-cd services
-docker compose up
-```
-Then you should be able to see  http://localhost:6333/dashboard
-
-# Additional requirements
-
-index.py has local dependencies on other modules, for this reason if you are running it inside indexpaper project folder consider having it installed locally:
-```bash
-pip install -e .
-```
```

### Comparing `indexpaper-0.0.3/indexpaper.egg-info/PKG-INFO` & `indexpaper-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexpaper
-Version: 0.0.3
+Version: 0.0.4
 Summary: indexpaper - library to index papers with vector databases
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download,index,vector databases
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -13,21 +13,82 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # indexpaper
+
 The project devoted to indexing papers in vector databases
 
 It was originally part of getpaper but now has not dependencies on it
 
-We provide features to index the papers with openai or llama embeddings and save them in chromadb vector store.
+We provide features to index the papers as well as semantic-scholar paper datasets with openai, huggingface or llama embeddings and save them either chromadb or qdrant vector store.
+
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 
+# getting started
+
+Install the library with:
+```bash
+pip install getpaper
+```
+
+On linux systems you sometimes need to check that build--essential are installed:
+```bash
+sudo apt install build-essential
+```
+It is also recommended to use micromamba, conda, anaconda or other environments to avoid bloating system python with too many dependencies.
+Assuming you installed [micromamba](https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html), you will have to create an environment and enable the library locally
+```
+micromamba create -f environment.yaml
+micromabma activate indexpaper
+pip install -e .
+```
+The last command is optional. With conda/anaconda the commands will look the same but with another name of executable.
+
+## Running local Qdrant
+
+We provide docker-compose configuration to run local qdrant (you can also use qdrant cloud instead).
+To run local qdrant install docker compose (sometimes needs sudo) and run:
+```bash
+cd services
+docker compose up
+```
+Then you should be able to see  http://localhost:6333/dashboard
+
+# Additional requirements
+
+index.py has local dependencies on other modules, for this reason if you are running it inside indexpaper project folder consider having it installed locally:
+```bash
+pip install -e .
+```
+
+# indexing a dataset
+
+To index a dataset you can use either index.py dataset subcommand or you look how to do it in code in papers.ipynb example notebook
+For example, if we want to index "longevity-genie/tacutu_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "cuda" as device and with 10 papers in a slice.
+And we want to write it to the local version of qdrant located at http://localhost:6333 (see services for docker-compose file):
+```bash
+python indexpaper/index.py dataset --collection biolinkbert_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --url http://localhost:6333 --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
+```
+
+Another example. If we want to index "longevity-genie/moskalev_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "gpu" as device and with 10 papers in a slice.
+And we want to use our Qdrant cloud key (fill in QDRANT_KEY or put it to environment variable)
+```bash
+python indexpaper/index.py dataset --collection biolinkbert_512_moskalev_papers --dataset "longevity-genie/moskalev_papers" --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key QDRANT_KEY --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
+```
+Another example. Robi Tacutu papers with cpu using QDRANT_KEY, cluster url (put yours) and michiyasunaga/BioLinkBERT-large embeddings model:
+```
+python indexpaper/index.py dataset --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --collection biolord_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --key QDRANT_KEY --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cpu
+```
+If you want to recreate the collection from scretch you can also add --rewrite true
+
+# Indexing papers
+
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 indexpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 It is possible to use both Chroma and Qdrant. To use qdrant we provide docker-compose file to set it up:
 ```bash
@@ -67,43 +128,7 @@
 ```bash
 python example.py evaluate --model intfloat/multilingual-e5-large --dataset longevity-genie/tacutu_papers
 ```
 To measure time
 ```bash
 python example.py measure --model intfloat/multilingual-e5-large --dataset longevity-genie/tacutu_papers
 ```
-
-# indexing a dataset
-
-To index a dataset you can use either index.py dataset subcomment or you look how to do it in code in papers.ipynb example notebook
-For example, if we want to index "longevity-genie/tacutu_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "cuda" as device and with 10 papers in a slice.
-And we want to write it to the local version of qdrant located at http://localhost:6333 (see services for docker-compose file):
-```bash
-python indexpaper/index.py dataset --collection biolinkbert_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --url http://localhost:6333 --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
-```
-
-Another example. If we want to index "longevity-genie/moskalev_papers" huggingface dataset using "michiyasunaga/BioLinkBERT-large" hugging face embedding with "gpu" as device and with 10 papers in a slice.
-And we want to use our Qdrant cloud key (fill in QDRANT_KEY or put it to environment variable)
-```bash
-python indexpaper/index.py dataset --collection biolinkbert_512_moskalev_papers --dataset "longevity-genie/moskalev_papers" --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key QDRANT_KEY --model michiyasunaga/BioLinkBERT-large --slice 10 --chunk_size 512 --device cuda
-```
-Another example. Robi Tacutu papers with cpu using QDRANT_KEY, cluster url (put yours) and biolord embeddings model:
-```
-python indexpaper/index.py dataset --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io --collection biolord_512_tacutu_papers --dataset "longevity-genie/tacutu_papers" --key QDRANT_KEY --model FremyCompany/BioLORD-STAMB2-v1 --slice 10 --chunk_size 512 --device cpu
-```
-
-# Runnning local Qdrant
-
-We provide docker-compose configuration to run local qdrant (you can also use qdrant cloud instead).
-To run local qdrant install docker compose (sometimes needs sudo) and run:
-```bash
-cd services
-docker compose up
-```
-Then you should be able to see  http://localhost:6333/dashboard
-
-# Additional requirements
-
-index.py has local dependencies on other modules, for this reason if you are running it inside indexpaper project folder consider having it installed locally:
-```bash
-pip install -e .
-```
```

### Comparing `indexpaper-0.0.3/setup.py` & `indexpaper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'indexpaper - library to index papers with vector databases'
 LONG_DESCRIPTION = 'indexpaper - library to index papers with vector databases'
 
 # Setting up
 setup(
     name="indexpaper",
     version=VERSION,
```

