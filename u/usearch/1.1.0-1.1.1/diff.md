# Comparing `tmp/usearch-1.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-1.1.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 211992 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 15:56 usearch/__init__.py
--rw-rw-rw-  2.0 fat     4241 b- defN 23-Aug-05 15:56 usearch/client.py
--rw-rw-rw-  2.0 fat   436736 b- defN 23-Aug-05 16:05 usearch/compiled.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    14953 b- defN 23-Aug-05 15:56 usearch/eval.py
--rw-rw-rw-  2.0 fat    34478 b- defN 23-Aug-05 15:56 usearch/index.py
--rw-rw-rw-  2.0 fat     3274 b- defN 23-Aug-05 15:56 usearch/io.py
--rw-rw-rw-  2.0 fat     4100 b- defN 23-Aug-05 15:56 usearch/numba.py
--rw-rw-rw-  2.0 fat     3858 b- defN 23-Aug-05 15:56 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-05 16:05 usearch-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    16401 b- defN 23-Aug-05 16:05 usearch-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-05 16:05 usearch-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-05 16:05 usearch-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      993 b- defN 23-Aug-05 16:05 usearch-1.1.0.dist-info/RECORD
-13 files, 530700 bytes uncompressed, 210368 bytes compressed:  60.4%
+Zip file size: 212787 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-07 13:09 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     4241 b- defN 23-Aug-07 13:09 usearch/client.py
+-rw-rw-rw-  2.0 fat   438272 b- defN 23-Aug-07 13:16 usearch/compiled.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    14953 b- defN 23-Aug-07 13:09 usearch/eval.py
+-rw-rw-rw-  2.0 fat    34478 b- defN 23-Aug-07 13:09 usearch/index.py
+-rw-rw-rw-  2.0 fat     3274 b- defN 23-Aug-07 13:09 usearch/io.py
+-rw-rw-rw-  2.0 fat     4100 b- defN 23-Aug-07 13:09 usearch/numba.py
+-rw-rw-rw-  2.0 fat     3858 b- defN 23-Aug-07 13:09 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-07 13:16 usearch-1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    18242 b- defN 23-Aug-07 13:16 usearch-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-07 13:16 usearch-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-07 13:16 usearch-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      993 b- defN 23-Aug-07 13:16 usearch-1.1.1.dist-info/RECORD
+13 files, 534077 bytes uncompressed, 211163 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: usearch/numba.py
 Comment: 
 
 Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-1.1.0.dist-info/LICENSE
+Filename: usearch-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-1.1.0.dist-info/METADATA
+Filename: usearch-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: usearch-1.1.0.dist-info/WHEEL
+Filename: usearch-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-1.1.0.dist-info/top_level.txt
+Filename: usearch-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-1.1.0.dist-info/RECORD
+Filename: usearch-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `usearch-1.1.0.dist-info/LICENSE` & `usearch-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usearch-1.1.0.dist-info/METADATA` & `usearch-1.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Smaller & Faster Single-File Vector Search Engine from Unum
 Author: Ash Vardanian
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -48,20 +48,20 @@
 &nbsp;&nbsp;&nbsp;
 <a href="https://github.com/unum-cloud/usearch"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/github.svg" alt="GitHub"></a>
 </p>
 
 <p align="center">
 Euclidean • Angular • Jaccard • Hamming • Haversine • User-Defined Metrics
 <br/>
-<a href="https://unum-cloud.github.io/usearch/cpp">C++11</a> •
-<a href="https://unum-cloud.github.io/usearch/python">Python</a> •
+<a href="https://unum-cloud.github.io/usearch/cpp">C++ 11</a> •
+<a href="https://unum-cloud.github.io/usearch/python">Python 3</a> •
 <a href="https://unum-cloud.github.io/usearch/javascript">JavaScript</a> •
 <a href="https://unum-cloud.github.io/usearch/java">Java</a> •
 <a href="https://unum-cloud.github.io/usearch/rust">Rust</a> •
-<a href="https://unum-cloud.github.io/usearch/c">C99</a> •
+<a href="https://unum-cloud.github.io/usearch/c">C 99</a> •
 <a href="https://unum-cloud.github.io/usearch/objective-c">Objective-C</a> •
 <a href="https://unum-cloud.github.io/usearch/swift">Swift</a> •
 <a href="https://unum-cloud.github.io/usearch/golang">GoLang</a> •
 <a href="https://unum-cloud.github.io/usearch/wolfram">Wolfram</a>
 <br/>
 Linux • MacOS • Windows • Docker • WebAssembly
 </p>
@@ -187,15 +187,54 @@
 loaded_copy = index.load("index.usearch")
 view = Index.restore("index.usearch", view=True)
 
 other_view = Index(ndim=..., metric=CompiledMetric(...))
 other_view.view("index.usearch")
 ```
 
-## Joins
+## Exact, Approximate, and Multi-Index Lookups
+
+Approximate search methods, such as HNSW, are predominantly used when an exact brute-force search becomes too resource-intensive.
+This typically occurs when you have millions of entries in a collection.
+For smaller collections, we offer a more direct approach with the `search` method.
+
+```py
+from usearch.index import search, MetricKind, Matches, BatchMatches
+import numpy as np
+
+# Generate 10'000 random vectors with 1024 dimensions
+vectors = np.random.rand(10_000, 1024).astype(np.float32)
+vector = np.random.rand(1024).astype(np.float32)
+
+one_in_many: Matches = search(vectors, vector, 50, MetricKind.L2sq, exact=True)
+many_in_many: BatchMatches = search(vectors, vectors, 50, MetricKind.L2sq, exact=True)
+```
+
+By passing the `exact=True` argument, the system bypasses indexing altogether and performs a brute-force search through the entire dataset using SIMD-optimized similarity metrics from [SimSIMD](https://github.com/ashvardanian/simsimd).
+When compared to FAISS's `IndexFlatL2` in Google Colab, **[USearch may offer up to a 20x performance improvement](https://github.com/unum-cloud/usearch/issues/176#issuecomment-1666650778)**:
+
+- `faiss.IndexFlatL2`: **55.3 ms**.
+- `usearch.index.search`: **2.54 ms**.
+
+For larger workloads targeting billions or even trillions of vectors, parallel multi-index lookups become invaluable.
+These lookups prevent the need to construct a single, massive index, allowing users to query multiple smaller ones instead.
+
+```py
+from usearch.index import Indexes
+
+multi_index = Indexes(
+    indexes: Iterable[usearch.index.Index] = [...],
+    paths: Iterable[os.PathLike] = [...],
+    view: bool = False,
+    threads: int = 0,
+)
+multi_index.search(...)
+```
+
+## Joins, One-to-One, One-to-Many, and Many-to-Many Mappings
 
 One of the big questions these days is how will AI change the world of databases and data management.
 Most databases are still struggling to implement high-quality fuzzy search, and the only kind of joins they know are deterministic.
 A `join` is different from searching for every entry, as it requires a one-to-one mapping, banning collisions among separate search results.
 
 | Exact Search | Fuzzy Search | Semantic Search ? |
 | :----------: | :----------: | :---------------: |
@@ -217,17 +256,17 @@
 By now, the core functionality is supported across all bindings.
 Broader functionality is ported per request.
 
 |                         | C++ 11 | Python 3 | C 99  | Java  | JavaScript | Rust  | GoLang | Swift |
 | :---------------------- | :----: | :------: | :---: | :---: | :--------: | :---: | :----: | :---: |
 | Add, search             |   ✅    |    ✅     |   ✅   |   ✅   |     ✅      |   ✅   |   ✅    |   ✅   |
 | Save, load, view        |   ✅    |    ✅     |   ✅   |   ✅   |     ✅      |   ✅   |   ✅    |   ✅   |
-| Join                    |   ✅    |    ✅     |   ✅   |   ❌   |     ❌      |   ❌   |   ❌    |   ❌   |
 | User-defined metrics    |   ✅    |    ✅     |   ✅   |   ❌   |     ❌      |   ❌   |   ❌    |   ❌   |
-| Variable-length vectors |   ✅    |    ✅     |   ❌   |   ❌   |     ❌      |   ❌   |   ❌    |   ❌   |
+| Joins                    |   ✅    |    ✅     |   ❌   |   ❌   |     ❌      |   ❌   |   ❌    |   ❌   |
+| Variable-length vectors |   ✅    |    ❌     |   ❌   |   ❌   |     ❌      |   ❌   |   ❌    |   ❌   |
 | 4B+ capacities          |   ✅    |    ❌     |   ❌   |   ❌   |     ❌      |   ❌   |   ❌    |   ❌   |
 
 ## Application Examples
 
 ### USearch + AI = Multi-Modal Semantic Search
 
 AI has a growing number of applications, but one of the coolest classic ideas is to use it for Semantic Search.
@@ -309,17 +348,17 @@
 [smiles]: https://en.wikipedia.org/wiki/Simplified_molecular-input_line-entry_system
 [rdkit-fingerprints]: https://www.rdkit.org/docs/RDKit_Book.html#additional-information-about-the-fingerprints
 
 
 ## Integrations
 
 - [x] GPT-Cache.
-- [ ] LangChain.
-- [ ] Microsoft Semantic Kernel.
+- [x] LangChain.
 - [ ] ClickHouse.
+- [ ] Microsoft Semantic Kernel.
 
 ## Citations
 
 ```txt
 @software{Vardanian_USearch_2022,
 doi = {10.5281/zenodo.7949416},
 author = {Vardanian, Ash},
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usearch Version: 1.1.0 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 1.1.1 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum Author: Ash Vardanian License:
 Apache-2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Natural Language :: English Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
@@ -19,16 +19,16 @@
                        **** Smaller & Faster Single-File
                              Vector Search Engine
                                       ****
 
         [Discord]     [LinkedIn]     [Twitter]     [Blog]     [GitHub]
  Euclidean â¢ Angular â¢ Jaccard â¢ Hamming â¢ Haversine â¢ User-Defined
                                    Metrics
- C++11 â¢ Python â¢ JavaScript â¢ Java â¢ Rust â¢ C99 â¢ Objective-C â¢
-                         Swift â¢ GoLang â¢ Wolfram
+ C++_11 â¢ Python_3 â¢ JavaScript â¢ Java â¢ Rust â¢ C_99 â¢ Objective-
+                      C â¢ Swift â¢ GoLang â¢ Wolfram
             Linux â¢ MacOS â¢ Windows â¢ Docker â¢ WebAssembly
 --- - â Benchmark-topping performance. - â Simple and extensible [single
 C++11 header][usearch-header] implementation. - â SIMD-optimized and [user-
 defined metrics](#user-defined-functions) with JIT compilation. - â Variable
 dimensionality vectors for unique applications, including search over
 compressed data. - â Bitwise Tanimoto and Sorensen coefficients for [Genomics
 and Chemistry applications](#usearch--rdkit--molecular-search). - â Hardware-
@@ -110,77 +110,100 @@
 hyper-parameters. [benchmarking]: https://github.com/unum-cloud/usearch/blob/
 main/docs/benchmarks.md ## Disk-based Indexes With USearch, you can serve
 indexes from external memory, enabling you to optimize your server choices for
 indexing speed and serving costs. This can result in **20x cost reduction** on
 AWS and other public clouds. ```py index.save("index.usearch") loaded_copy =
 index.load("index.usearch") view = Index.restore("index.usearch", view=True)
 other_view = Index(ndim=..., metric=CompiledMetric(...)) other_view.view
-("index.usearch") ``` ## Joins One of the big questions these days is how will
-AI change the world of databases and data management. Most databases are still
-struggling to implement high-quality fuzzy search, and the only kind of joins
-they know are deterministic. A `join` is different from searching for every
-entry, as it requires a one-to-one mapping, banning collisions among separate
-search results. | Exact Search | Fuzzy Search | Semantic Search ? | | :--------
---: | :----------: | :---------------: | | Exact Join | Fuzzy Join ? | Semantic
-Join ?? | Using USearch one can implement sub-quadratic complexity approximate,
-fuzzy, and semantic joins. This can come in handy in any fuzzy-matching tasks,
-common to Database Management Software. ```py men = Index(...) women = Index
-(...) pairs: dict = men.join(women, max_proposals=0, exact=False) ``` > Read
-more in post: [From Dating to Vector Search - "Stable Marriages" on a Planetary
-Scale ð©ââ¤ï¸âð¨](https://ashvardanian.com/posts/searching-stable-
-marriages) ## Functionality By now, the core functionality is supported across
-all bindings. Broader functionality is ported per request. | | C++ 11 | Python
-3 | C 99 | Java | JavaScript | Rust | GoLang | Swift | | :---------------------
-- | :----: | :------: | :---: | :---: | :--------: | :---: | :----: | :---: | |
-Add, search | â | â | â | â | â | â | â | â | | Save, load,
-view | â | â | â | â | â | â | â | â | | Join | â | â | â
-| â | â | â | â | â | | User-defined metrics | â | â | â | â
-| â | â | â | â | | Variable-length vectors | â | â | â | â |
-â | â | â | â | | 4B+ capacities | â | â | â | â | â | â |
-â | â | ## Application Examples ### USearch + AI = Multi-Modal Semantic
-Search AI has a growing number of applications, but one of the coolest classic
-ideas is to use it for Semantic Search. One can take an encoder model, like the
-multi-modal UForm, and a web-programming framework, like UCall, and build a
-text-to-image search platform in just 20 lines of Python. ```python import
-ucall import uform import usearch import numpy as np import PIL as pil server =
-ucall.Server() model = uform.get_model('unum-cloud/uform-vl-multilingual')
-index = usearch.index.Index(ndim=256) @server def add(key: int, photo:
-pil.Image.Image): image = model.preprocess_image(photo) vector =
-model.encode_image(image).detach().numpy() index.add(key, vector.flatten(),
-copy=True) @server def search(query: str) -> np.ndarray: tokens =
-model.preprocess_text(query) vector = model.encode_text(tokens).detach().numpy
-() matches = index.search(vector.flatten(), 3) return matches.keys server.run()
-``` We have pre-processed some commonly used datasets, cleaned the images,
-produced the vectors, and pre-built the index. | Dataset | Modalities | Images
-| Download | | :------------------------------------- | --------------------: |
------: | ------------------------------------: | | [Unsplash 25K][unsplash-25k-
-origin] | Images & Descriptions | 25 K | [HuggingFace / Unum][unsplash-25k-hf]
-| | [Conceptual Captions 3M][cc-3m-origin] | Images & Descriptions | 3 M |
-[HuggingFace / Unum][cc-3m-hf] | | [Arxiv 2M][arxiv-2m-origin] | Titles &
-Abstracts | 2 M | [HuggingFace / Unum][arxiv-2m-hf] | [unsplash-25k-origin]:
-https://github.com/unsplash/datasets [cc-3m-origin]: https://huggingface.co/
-datasets/conceptual_captions [arxiv-2m-origin]: https://www.kaggle.com/
-datasets/Cornell-University/arxiv [unsplash-25k-hf]: https://huggingface.co/
-datasets/unum-cloud/ann-unsplash-25k [cc-3m-hf]: https://huggingface.co/
-datasets/unum-cloud/ann-cc-3m [arxiv-2m-hf]: https://huggingface.co/datasets/
-unum-cloud/ann-arxiv-2m ### USearch + RDKit = Molecular Search Comparing
-molecule graphs and searching for similar structures is expensive and slow. It
-can be seen as a special case of the NP-Complete Subgraph Isomorphism problem.
-Luckily, domain-specific approximate methods exist. The one commonly used in
-Chemistry, is to generate structures from [SMILES][smiles], and later hash them
-into binary fingerprints. The latter are searchable with bitwise similarity
-metrics, like the Tanimoto coefficient. Below is an example using the RDKit
-package. ```python from usearch.index import Index, MetricKind from rdkit
-import Chem from rdkit.Chem import AllChem import numpy as np molecules =
-[Chem.MolFromSmiles('CCOC'), Chem.MolFromSmiles('CCO')] encoder =
-AllChem.GetRDKitFPGenerator() fingerprints = np.vstack([encoder.GetFingerprint
-(x) for x in molecules]) fingerprints = np.packbits(fingerprints, axis=1) index
-= Index(ndim=2048, metric=MetricKind.Tanimoto) keys = np.arange(len(molecules))
-index.add(keys, fingerprints) matches = index.search(fingerprints, 10) ```
-[smiles]: https://en.wikipedia.org/wiki/Simplified_molecular-input_line-
-entry_system [rdkit-fingerprints]: https://www.rdkit.org/docs/
-RDKit_Book.html#additional-information-about-the-fingerprints ## Integrations -
-[x] GPT-Cache. - [ ] LangChain. - [ ] Microsoft Semantic Kernel. - [ ]
-ClickHouse. ## Citations ```txt @software{Vardanian_USearch_2022, doi =
-{10.5281/zenodo.7949416}, author = {Vardanian, Ash}, title = {{USearch by Unum
-Cloud}}, url = {https://github.com/unum-cloud/usearch}, version = {0.13.0},
-year = {2022} month = jun, } ```
+("index.usearch") ``` ## Exact, Approximate, and Multi-Index Lookups
+Approximate search methods, such as HNSW, are predominantly used when an exact
+brute-force search becomes too resource-intensive. This typically occurs when
+you have millions of entries in a collection. For smaller collections, we offer
+a more direct approach with the `search` method. ```py from usearch.index
+import search, MetricKind, Matches, BatchMatches import numpy as np # Generate
+10'000 random vectors with 1024 dimensions vectors = np.random.rand(10_000,
+1024).astype(np.float32) vector = np.random.rand(1024).astype(np.float32)
+one_in_many: Matches = search(vectors, vector, 50, MetricKind.L2sq, exact=True)
+many_in_many: BatchMatches = search(vectors, vectors, 50, MetricKind.L2sq,
+exact=True) ``` By passing the `exact=True` argument, the system bypasses
+indexing altogether and performs a brute-force search through the entire
+dataset using SIMD-optimized similarity metrics from [SimSIMD](https://
+github.com/ashvardanian/simsimd). When compared to FAISS's `IndexFlatL2` in
+Google Colab, **[USearch may offer up to a 20x performance improvement](https:/
+/github.com/unum-cloud/usearch/issues/176#issuecomment-1666650778)**: -
+`faiss.IndexFlatL2`: **55.3 ms**. - `usearch.index.search`: **2.54 ms**. For
+larger workloads targeting billions or even trillions of vectors, parallel
+multi-index lookups become invaluable. These lookups prevent the need to
+construct a single, massive index, allowing users to query multiple smaller
+ones instead. ```py from usearch.index import Indexes multi_index = Indexes
+( indexes: Iterable[usearch.index.Index] = [...], paths: Iterable[os.PathLike]
+= [...], view: bool = False, threads: int = 0, ) multi_index.search(...) ``` ##
+Joins, One-to-One, One-to-Many, and Many-to-Many Mappings One of the big
+questions these days is how will AI change the world of databases and data
+management. Most databases are still struggling to implement high-quality fuzzy
+search, and the only kind of joins they know are deterministic. A `join` is
+different from searching for every entry, as it requires a one-to-one mapping,
+banning collisions among separate search results. | Exact Search | Fuzzy Search
+| Semantic Search ? | | :----------: | :----------: | :---------------: | |
+Exact Join | Fuzzy Join ? | Semantic Join ?? | Using USearch one can implement
+sub-quadratic complexity approximate, fuzzy, and semantic joins. This can come
+in handy in any fuzzy-matching tasks, common to Database Management Software.
+```py men = Index(...) women = Index(...) pairs: dict = men.join(women,
+max_proposals=0, exact=False) ``` > Read more in post: [From Dating to Vector
+Search - "Stable Marriages" on a Planetary Scale ð©ââ¤ï¸âð¨](https://
+ashvardanian.com/posts/searching-stable-marriages) ## Functionality By now, the
+core functionality is supported across all bindings. Broader functionality is
+ported per request. | | C++ 11 | Python 3 | C 99 | Java | JavaScript | Rust |
+GoLang | Swift | | :---------------------- | :----: | :------: | :---: | :---:
+| :--------: | :---: | :----: | :---: | | Add, search | â | â | â | â |
+â | â | â | â | | Save, load, view | â | â | â | â | â | â
+| â | â | | User-defined metrics | â | â | â | â | â | â | â
+| â | | Joins | â | â | â | â | â | â | â | â | | Variable-
+length vectors | â | â | â | â | â | â | â | â | | 4B+
+capacities | â | â | â | â | â | â | â | â | ## Application
+Examples ### USearch + AI = Multi-Modal Semantic Search AI has a growing number
+of applications, but one of the coolest classic ideas is to use it for Semantic
+Search. One can take an encoder model, like the multi-modal UForm, and a web-
+programming framework, like UCall, and build a text-to-image search platform in
+just 20 lines of Python. ```python import ucall import uform import usearch
+import numpy as np import PIL as pil server = ucall.Server() model =
+uform.get_model('unum-cloud/uform-vl-multilingual') index = usearch.index.Index
+(ndim=256) @server def add(key: int, photo: pil.Image.Image): image =
+model.preprocess_image(photo) vector = model.encode_image(image).detach().numpy
+() index.add(key, vector.flatten(), copy=True) @server def search(query: str) -
+> np.ndarray: tokens = model.preprocess_text(query) vector = model.encode_text
+(tokens).detach().numpy() matches = index.search(vector.flatten(), 3) return
+matches.keys server.run() ``` We have pre-processed some commonly used
+datasets, cleaned the images, produced the vectors, and pre-built the index. |
+Dataset | Modalities | Images | Download | | :---------------------------------
+---- | --------------------: | -----: | ------------------------------------: |
+| [Unsplash 25K][unsplash-25k-origin] | Images & Descriptions | 25 K |
+[HuggingFace / Unum][unsplash-25k-hf] | | [Conceptual Captions 3M][cc-3m-
+origin] | Images & Descriptions | 3 M | [HuggingFace / Unum][cc-3m-hf] | |
+[Arxiv 2M][arxiv-2m-origin] | Titles & Abstracts | 2 M | [HuggingFace / Unum]
+[arxiv-2m-hf] | [unsplash-25k-origin]: https://github.com/unsplash/datasets
+[cc-3m-origin]: https://huggingface.co/datasets/conceptual_captions [arxiv-2m-
+origin]: https://www.kaggle.com/datasets/Cornell-University/arxiv [unsplash-
+25k-hf]: https://huggingface.co/datasets/unum-cloud/ann-unsplash-25k [cc-3m-
+hf]: https://huggingface.co/datasets/unum-cloud/ann-cc-3m [arxiv-2m-hf]: https:
+//huggingface.co/datasets/unum-cloud/ann-arxiv-2m ### USearch + RDKit =
+Molecular Search Comparing molecule graphs and searching for similar structures
+is expensive and slow. It can be seen as a special case of the NP-Complete
+Subgraph Isomorphism problem. Luckily, domain-specific approximate methods
+exist. The one commonly used in Chemistry, is to generate structures from
+[SMILES][smiles], and later hash them into binary fingerprints. The latter are
+searchable with bitwise similarity metrics, like the Tanimoto coefficient.
+Below is an example using the RDKit package. ```python from usearch.index
+import Index, MetricKind from rdkit import Chem from rdkit.Chem import AllChem
+import numpy as np molecules = [Chem.MolFromSmiles('CCOC'), Chem.MolFromSmiles
+('CCO')] encoder = AllChem.GetRDKitFPGenerator() fingerprints = np.vstack(
+[encoder.GetFingerprint(x) for x in molecules]) fingerprints = np.packbits
+(fingerprints, axis=1) index = Index(ndim=2048, metric=MetricKind.Tanimoto)
+keys = np.arange(len(molecules)) index.add(keys, fingerprints) matches =
+index.search(fingerprints, 10) ``` [smiles]: https://en.wikipedia.org/wiki/
+Simplified_molecular-input_line-entry_system [rdkit-fingerprints]: https://
+www.rdkit.org/docs/RDKit_Book.html#additional-information-about-the-
+fingerprints ## Integrations - [x] GPT-Cache. - [x] LangChain. - [ ]
+ClickHouse. - [ ] Microsoft Semantic Kernel. ## Citations ```txt @software
+{Vardanian_USearch_2022, doi = {10.5281/zenodo.7949416}, author = {Vardanian,
+Ash}, title = {{USearch by Unum Cloud}}, url = {https://github.com/unum-cloud/
+usearch}, version = {0.13.0}, year = {2022} month = jun, } ```
```

## Comparing `usearch-1.1.0.dist-info/RECORD` & `usearch-1.1.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 usearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 usearch/client.py,sha256=DcqPCZi15fMPd4Y9jXWSoRCp1fbjiOcnFmOO3lFe8f4,4241
-usearch/compiled.cp39-win_amd64.pyd,sha256=swYGiwyWXePN36rlgW_XMvIC2N9shxAy9CBCfwcMrUA,436736
+usearch/compiled.cp39-win_amd64.pyd,sha256=FV1zMokoXCloV0TrnIQeahU0jrA3io2iFNy57MdvcJs,438272
 usearch/eval.py,sha256=rw4R7qPm_E85xSIijE8MsQElEZh-Xa7EoJBrdIx0TCY,14953
 usearch/index.py,sha256=PCPYYOCliBGv8rYB-Jx5neM042scwJ6fB0izCQCP5PI,34478
 usearch/io.py,sha256=dmx9xq04E691BDE8-kASLZ93iCi5rEdxhEk61BKm0gI,3274
 usearch/numba.py,sha256=qkdzziRfE1p7VPi7rxUcllli6iiyx2eR9krc3o3UTvY,4100
 usearch/server.py,sha256=RVl5pXZQXs80MzmYaTMU9Wg9pH0maWmh3tiF22pj4OI,3858
-usearch-1.1.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-usearch-1.1.0.dist-info/METADATA,sha256=0a6rjvO9RBxJEd5Y2ZSd0oxbvpiEGIYp8YrdJSpZnjE,16401
-usearch-1.1.0.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
-usearch-1.1.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
-usearch-1.1.0.dist-info/RECORD,,
+usearch-1.1.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+usearch-1.1.1.dist-info/METADATA,sha256=lxnrrVSI67B_wE0pv_-ZodYna_HOgPDXtJlh9aAf_nY,18242
+usearch-1.1.1.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
+usearch-1.1.1.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
+usearch-1.1.1.dist-info/RECORD,,
```

