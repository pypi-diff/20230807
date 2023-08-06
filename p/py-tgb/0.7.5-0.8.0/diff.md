# Comparing `tmp/py_tgb-0.7.5.tar.gz` & `tmp/py_tgb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tgb-0.7.5.tar", max compression
+gzip compressed data, was "py_tgb-0.8.0.tar", max compression
```

## Comparing `py_tgb-0.7.5.tar` & `py_tgb-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     4653 2023-07-27 18:19:30.184342 py_tgb-0.7.5/README.md
--rw-r--r--   0        0        0      748 2023-07-27 18:19:30.184342 py_tgb-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      177 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/MAG/mag.py
--rw-r--r--   0        0        0      820 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py
--rw-r--r--   0        0        0     4740 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin.py
--rw-r--r--   0        0        0     2497 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py
--rw-r--r--   0        0        0     6912 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment.py
--rw-r--r--   0        0        0     2499 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py
--rw-r--r--   0        0        0     7781 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight.py
--rw-r--r--   0        0        0     2499 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py
--rw-r--r--   0        0        0     4777 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review.py
--rw-r--r--   0        0        0     2503 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py
--rw-r--r--   0        0        0     2543 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py
--rw-r--r--   0        0        0    19780 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-genre.py
--rw-r--r--   0        0        0    11859 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-reddit.py
--rw-r--r--   0        0        0     5927 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-trade.py
--rw-r--r--   0        0        0      539 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/tgbn-arxiv/process_arxiv.py
--rw-r--r--   0        0        0     5290 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/token_network/token.py
--rw-r--r--   0        0        0    15644 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/dataset.py
--rw-r--r--   0        0        0     7532 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5869 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/evaluate.py
--rw-r--r--   0        0        0    14146 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/negative_generator.py
--rw-r--r--   0        0        0     5123 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/negative_sampler.py
--rw-r--r--   0        0        0    17517 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/nodeproppred/dataset.py
--rw-r--r--   0        0        0     7205 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/nodeproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5336 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/nodeproppred/evaluate.py
--rw-r--r--   0        0        0     8691 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/dataset_stats.py
--rw-r--r--   0        0        0     2185 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/info.py
--rw-r--r--   0        0        0    27787 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/pre_process.py
--rw-r--r--   0        0        0     2747 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/stats.py
--rw-r--r--   0        0        0     2974 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/utils.py
--rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 py_tgb-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     5209 2023-08-06 22:32:29.529394 py_tgb-0.8.0/README.md
+-rw-r--r--   0        0        0      748 2023-08-06 22:32:29.529394 py_tgb-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/MAG/mag.py
+-rw-r--r--   0        0        0      820 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py
+-rw-r--r--   0        0        0     4740 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-coin.py
+-rw-r--r--   0        0        0     2497 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py
+-rw-r--r--   0        0        0     6912 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-comment.py
+-rw-r--r--   0        0        0     2499 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py
+-rw-r--r--   0        0        0     7781 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-flight.py
+-rw-r--r--   0        0        0     2499 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py
+-rw-r--r--   0        0        0     4777 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-review.py
+-rw-r--r--   0        0        0     2503 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py
+-rw-r--r--   0        0        0     2543 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py
+-rw-r--r--   0        0        0    19780 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-genre.py
+-rw-r--r--   0        0        0    11859 2023-08-06 22:32:29.529394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-reddit.py
+-rw-r--r--   0        0        0    17005 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-token.py
+-rw-r--r--   0        0        0     5927 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-trade.py
+-rw-r--r--   0        0        0      539 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/datasets/tgbn-arxiv/process_arxiv.py
+-rw-r--r--   0        0        0    15500 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/linkproppred/dataset.py
+-rw-r--r--   0        0        0     7532 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/linkproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5869 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/linkproppred/evaluate.py
+-rw-r--r--   0        0        0    14146 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/linkproppred/negative_generator.py
+-rw-r--r--   0        0        0     5123 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/linkproppred/negative_sampler.py
+-rw-r--r--   0        0        0    18456 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/nodeproppred/dataset.py
+-rw-r--r--   0        0        0     7240 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/nodeproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5336 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/nodeproppred/evaluate.py
+-rw-r--r--   0        0        0     8691 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/utils/dataset_stats.py
+-rw-r--r--   0        0        0     2348 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/utils/info.py
+-rw-r--r--   0        0        0    28590 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/utils/pre_process.py
+-rw-r--r--   0        0        0     2747 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/utils/stats.py
+-rw-r--r--   0        0        0     2974 2023-08-06 22:32:29.533394 py_tgb-0.8.0/tgb/utils/utils.py
+-rw-r--r--   0        0        0     5893 1970-01-01 00:00:00.000000 py_tgb-0.8.0/PKG-INFO
```

### Comparing `py_tgb-0.7.5/README.md` & `py_tgb-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,29 @@
 - TGB includes large-scale and realistic datasets from five different domains with both dynamic link prediction and node property prediction tasks
 - TGB automatically downloads datasets and processes them into `numpy`, `PyTorch` and `PyG compatible TemporalData` formats. 
 - Novel TG models can be easily evaluated on TGB datasets via reproducible and realistic evaluation protocols. 
 - TGB provides public and online leaderboards to track recent developments in temporal graph learning domain
 
 ![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
 
+**To submit to [TGB leaderboard](https://tgb.complexdatalab.com/), please fill in this [google form](https://forms.gle/SEsXvN1QHo9tSFwx9)**
+
+**See all version differences and update notes [here](https://tgb.complexdatalab.com/docs/update/)**
+
 ### Annoucements
 
-**Please update to version `0.7.5`**
+**Please update to version `0.8.0`**
+
+#### version `0.8.0`
+
+fixing metric computation issue in node property prediction task, `tgbn` leaderboards results are updated to reflect the changes.
+Please refer to `examples/nodeproppred/` example folders to how to compute the metric correctly. No changes for `linkproppred` datasets.
+
+
+#### version `0.7.5`
 
 the negative samples for the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of the dataset would be needed (will be prompted automatically in this version when you use the dataloader)
 
 
 ### Pip Install
 
 You can install TGB via [pip](https://pypi.org/project/py-tgb/)
```

#### html2text {}

```diff
@@ -7,20 +7,27 @@
 realistic datasets from five different domains with both dynamic link
 prediction and node property prediction tasks - TGB automatically downloads
 datasets and processes them into `numpy`, `PyTorch` and `PyG compatible
 TemporalData` formats. - Novel TG models can be easily evaluated on TGB
 datasets via reproducible and realistic evaluation protocols. - TGB provides
 public and online leaderboards to track recent developments in temporal graph
 learning domain ![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
-### Annoucements **Please update to version `0.7.5`** the negative samples for
-the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of
-the dataset would be needed (will be prompted automatically in this version
-when you use the dataloader) ### Pip Install You can install TGB via [pip]
-(https://pypi.org/project/py-tgb/) ``` pip install py-tgb ``` ### Links and
-Datasets The project website can be found [here](https://
+**To submit to [TGB leaderboard](https://tgb.complexdatalab.com/), please fill
+in this [google form](https://forms.gle/SEsXvN1QHo9tSFwx9)** **See all version
+differences and update notes [here](https://tgb.complexdatalab.com/docs/update/
+)** ### Annoucements **Please update to version `0.8.0`** #### version `0.8.0`
+fixing metric computation issue in node property prediction task, `tgbn`
+leaderboards results are updated to reflect the changes. Please refer to
+`examples/nodeproppred/` example folders to how to compute the metric
+correctly. No changes for `linkproppred` datasets. #### version `0.7.5` the
+negative samples for the `tgbl-wiki` and `tgbl-review` dataset has been updated
+and redownload of the dataset would be needed (will be prompted automatically
+in this version when you use the dataloader) ### Pip Install You can install
+TGB via [pip](https://pypi.org/project/py-tgb/) ``` pip install py-tgb ``` ###
+Links and Datasets The project website can be found [here](https://
 tgb.complexdatalab.com/). The API documentations can be found [here](https://
 shenyanghuang.github.io/TGB/). all dataset download links can be found at
 [info.py](https://github.com/shenyangHuang/TGB/blob/main/tgb/utils/info.py) TGB
 dataloader will also automatically download the dataset as well as the negative
 samples for the link property prediction datasets. ### Running Example Methods
 - For the dynamic link property prediction task, see the [`examples/
 linkproppred`](https://github.com/shenyangHuang/TGB/tree/main/examples/
```

### Comparing `py_tgb-0.7.5/pyproject.toml` & `py_tgb-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-tgb"
-version = "0.7.5"
+version = "0.8.0"
 description = "Temporal Graph Benchmark project repo"
 authors = ["shenyang Huang <shenyang.huang@mail.mcgill.ca>", "Farimah Poursafaei", "Emanuele Rossi <emanuele.rossi1909@gmail.com>", "Jacob Danovitch <jacob.danovitch@mila.quebec>"]
 readme = "README.md"
 packages = [{include = "tgb"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-coin.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-comment.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-flight.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-review.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-genre.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-genre.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-reddit.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-reddit.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-trade.py` & `py_tgb-0.8.0/tgb/datasets/dataset_scripts/tgbn-trade.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/datasets/tgbn-arxiv/process_arxiv.py` & `py_tgb-0.8.0/tgb/datasets/tgbn-arxiv/process_arxiv.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/linkproppred/dataset.py` & `py_tgb-0.8.0/tgb/linkproppred/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     def download(self):
         """
         downloads this dataset from url
         check if files are already downloaded
         """
         # check if the file already exists
         if osp.exists(self.meta_dict["fname"]):
-            print("file found, skipping download")
+            print("raw file found, skipping download")
             return
 
         inp = input(
             "Will you download the dataset(s) now? (y/N)\n"
         ).lower()  # ask if the user wants to download the dataset
 
         if inp == "y":
@@ -244,17 +244,14 @@
         sources = np.array(df["u"])
         destinations = np.array(df["i"])
         timestamps = np.array(df["ts"])
         edge_idxs = np.array(df["idx"])
         weights = np.array(df["w"])
 
         edge_label = np.ones(len(df))  # should be 1 for all pos edges
-        # self._edge_feat = edge_feat + weights.reshape(
-        #     -1, 1
-        # )  # reshape weights as feature if available #! to remove
         self._edge_feat = edge_feat
         self._node_feat = node_feat
 
         full_data = {
             "sources": sources,
             "destinations": destinations,
             "timestamps": timestamps,
```

### Comparing `py_tgb-0.7.5/tgb/linkproppred/dataset_pyg.py` & `py_tgb-0.8.0/tgb/linkproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/linkproppred/evaluate.py` & `py_tgb-0.8.0/tgb/linkproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/linkproppred/negative_generator.py` & `py_tgb-0.8.0/tgb/linkproppred/negative_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/linkproppred/negative_sampler.py` & `py_tgb-0.8.0/tgb/linkproppred/negative_sampler.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/nodeproppred/dataset.py` & `py_tgb-0.8.0/tgb/nodeproppred/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     DATA_EVAL_METRIC_DICT,
     BColors,
 )
 from tgb.utils.utils import save_pkl, load_pkl
 from tgb.utils.pre_process import (
     load_label_dict,
     load_edgelist_sr,
+    load_edgelist_token,
     load_edgelist_datetime,
     load_trade_label_dict,
     load_edgelist_trade,
 )
 
 
 class NodePropPredDataset(object):
@@ -130,15 +131,15 @@
         Returns:
             None
         """
         # check if the file already exists
         if osp.exists(self.meta_dict["fname"]) and osp.exists(
             self.meta_dict["nodefile"]
         ):
-            print("file found, skipping download")
+            print("raw file found, skipping download")
             return
 
         else:
             inp = input(
                 "Will you download the dataset(s) now? (y/N)\n"
             ).lower()  # ask if the user wants to download the dataset
             if inp == "y":
@@ -188,85 +189,98 @@
         Returns:
             df: pandas data frame storing the temporal edge list
             node_label_dict: dictionary with key as timestamp and item as dictionary of node labels
         """
         OUT_DF = self.root + "/" + "ml_{}.pkl".format(self.name)
         OUT_NODE_DF = self.root + "/" + "ml_{}_node.pkl".format(self.name)
         OUT_LABEL_DF = self.root + "/" + "ml_{}_label.pkl".format(self.name)
+        OUT_EDGE_FEAT = self.root + "/" + "ml_{}.pkl".format(self.name + "_edge")
 
-        # * logic for tgbl-reddit, as node label file is too big to store on disc
-        if self.name == "tgbn-reddit":
-            if osp.exists(OUT_DF) and osp.exists(OUT_NODE_DF):
+        # * logic for large datasets, as node label file is too big to store on disc
+        if self.name == "tgbn-reddit" or self.name == "tgbn-token":
+            if osp.exists(OUT_DF) and osp.exists(OUT_NODE_DF) and osp.exists(OUT_EDGE_FEAT):
                 df = pd.read_pickle(OUT_DF)
+                edge_feat = load_pkl(OUT_EDGE_FEAT)
+                if (self.name == "tgbn-token"):
+                    #! taking log normalization for numerical stability
+                    print ("applying log normalization for weights in tgbn-token")
+                    edge_feat[:,0] = np.log(edge_feat[:,0])
                 node_ids = load_pkl(OUT_NODE_DF)
                 labels_dict = load_pkl(OUT_LABEL_DF)
                 node_label_dict = load_label_dict(
                     self.meta_dict["nodefile"], node_ids, labels_dict
                 )
-                return df, node_label_dict
+                return df, node_label_dict, edge_feat
 
         # * load the preprocessed file if possible
-        if osp.exists(OUT_DF) and osp.exists(OUT_NODE_DF):
+        if osp.exists(OUT_DF) and osp.exists(OUT_NODE_DF) and osp.exists(OUT_EDGE_FEAT):
             print("loading processed file")
             df = pd.read_pickle(OUT_DF)
             node_label_dict = load_pkl(OUT_NODE_DF)
+            edge_feat = load_pkl(OUT_EDGE_FEAT)
         else:  # * process the file
             print("file not processed, generating processed file")
             if self.name == "tgbn-reddit":
                 df, edge_feat, node_ids, labels_dict = load_edgelist_sr(
                     self.meta_dict["fname"], label_size=self._num_classes
                 )
+            elif self.name == "tgbn-token":
+                df, edge_feat, node_ids, labels_dict = load_edgelist_token(
+                    self.meta_dict["fname"], label_size=self._num_classes
+                )
             elif self.name == "tgbn-genre":
                 df, edge_feat, node_ids, labels_dict = load_edgelist_datetime(
                     self.meta_dict["fname"], label_size=self._num_classes
                 )
             elif self.name == "tgbn-trade":
                 df, edge_feat, node_ids = load_edgelist_trade(
                     self.meta_dict["fname"], label_size=self._num_classes
                 )
 
             df.to_pickle(OUT_DF)
+            save_pkl(edge_feat, OUT_EDGE_FEAT)
 
             if self.name == "tgbn-trade":
                 node_label_dict = load_trade_label_dict(
                     self.meta_dict["nodefile"], node_ids
                 )
             else:
                 node_label_dict = load_label_dict(
                     self.meta_dict["nodefile"], node_ids, labels_dict
                 )
 
             if (
-                self.name != "tgbn-reddit"
+                self.name != "tgbn-reddit" and self.name != "tgbn-token"
             ):  # don't save subreddits on disc, the node label file is too big
                 save_pkl(node_label_dict, OUT_NODE_DF)
             else:
                 save_pkl(node_ids, OUT_NODE_DF)
                 save_pkl(labels_dict, OUT_LABEL_DF)
             
             print("file processed and saved")
-        return df, node_label_dict
+        return df, node_label_dict, edge_feat
 
     def pre_process(self) -> None:
         """
         Pre-process the dataset and generates the splits, must be run before dataset properties can be accessed
         Returns:
             None
         """
         # first check if all files exist
         if ("fname" not in self.meta_dict) or ("nodefile" not in self.meta_dict):
             raise Exception("meta_dict does not contain all required filenames")
 
-        df, node_label_dict = self.generate_processed_files()
+        df, node_label_dict, edge_feat = self.generate_processed_files()
         sources = np.array(df["u"])
         destinations = np.array(df["i"])
         timestamps = np.array(df["ts"])
         edge_idxs = np.array(df["idx"])
         edge_label = np.ones(sources.shape[0])
-        self._edge_feat = np.array(df["w"])
+        #self._edge_feat = np.array(df["w"])
+        self._edge_feat = edge_feat
 
         full_data = {
             "sources": sources,
             "destinations": destinations,
             "timestamps": timestamps,
             "edge_idxs": edge_idxs,
             "edge_feat": self._edge_feat,
```

### Comparing `py_tgb-0.7.5/tgb/nodeproppred/dataset_pyg.py` & `py_tgb-0.8.0/tgb/nodeproppred/dataset_pyg.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,18 +141,18 @@
         """
         convert data to pytorch tensors
         """
         src = torch.from_numpy(self.dataset.full_data["sources"])
         dst = torch.from_numpy(self.dataset.full_data["destinations"])
         t = torch.from_numpy(self.dataset.full_data["timestamps"])
         edge_label = torch.from_numpy(self.dataset.full_data["edge_label"])
-        msg = torch.from_numpy(self.dataset.full_data["edge_feat"]).reshape(
-            [-1, 1]
-        )  # use edge features here if available
-
+        msg = torch.from_numpy(self.dataset.full_data["edge_feat"])
+        # msg = torch.from_numpy(self.dataset.full_data["edge_feat"]).reshape(
+        #     [-1, 1]
+        # ) 
         # * check typing
         if src.dtype != torch.int64:
             src = src.long()
 
         if dst.dtype != torch.int64:
             dst = dst.long()
```

### Comparing `py_tgb-0.7.5/tgb/nodeproppred/evaluate.py` & `py_tgb-0.8.0/tgb/nodeproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/utils/dataset_stats.py` & `py_tgb-0.8.0/tgb/utils/dataset_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/utils/info.py` & `py_tgb-0.8.0/tgb/utils/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,40 +27,44 @@
     "tgbl-review": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-review-v2.zip", #"https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-review.zip", #v1
     "tgbl-coin": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-coin.zip",
     "tgbl-flight": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-flight.zip",
     "tgbl-comment": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-comment.zip",
     "tgbn-trade": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-trade.zip",
     "tgbn-genre": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-genre.zip",
     "tgbn-reddit": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-reddit.zip",
+    "tgbn-token": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-token.zip",
 }
 
 DATA_VERSION_DICT = {
-    "tgbl-wiki": 2,
+    "tgbl-wiki": 2,  
     "tgbl-review": 2,
     "tgbl-coin": 1,
     "tgbl-comment": 1,
     "tgbl-flight": 1,
     "tgbn-trade": 1,
     "tgbn-genre": 1,
     "tgbn-reddit": 1,
+    "tgbn-token": 1,
 }
 
 #"https://object-arbutus.cloud.computecanada.ca/tgb/wiki_neg.zip" #for all negative samples of the wiki dataset
 #"https://object-arbutus.cloud.computecanada.ca/tgb/review_ns100.zip" #for 100 ns samples in review
 
 DATA_EVAL_METRIC_DICT = {
     "tgbl-wiki": "mrr",
     "tgbl-review": "mrr",
     "tgbl-coin": "mrr",
     "tgbl-comment": "mrr",
     "tgbl-flight": "mrr",
     "tgbn-trade": "ndcg",
     "tgbn-genre": "ndcg",
     "tgbn-reddit": "ndcg",
+    "tgbn-token": "ndcg",
 }
 
 
 DATA_NUM_CLASSES = {
     "tgbn-trade": 255,
     "tgbn-genre": 513,
     "tgbn-reddit": 698,
+    "tgbn-token": 1001,
 }
```

### Comparing `py_tgb-0.7.5/tgb/utils/pre_process.py` & `py_tgb-0.8.0/tgb/utils/pre_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,21 +76,20 @@
 
                 if v not in node_ids:
                     node_ids[v] = node_uid
                     node_uid += 1
 
                 u = node_ids[u]
                 i = node_ids[v]
-                feat = np.array([w])
                 u_list[idx - 1] = u
                 i_list[idx - 1] = i
                 ts_list[idx - 1] = ts
                 idx_list[idx - 1] = idx
                 w_list[idx - 1] = w
-                feat_l[idx - 1] = feat
+                feat_l[idx - 1] = np.array([w])
                 idx += 1
 
     return (
         pd.DataFrame(
             {"u": u_list, "i": i_list, "ts": ts_list, "idx": idx_list, "w": w_list}
         ),
         feat_l,
@@ -139,14 +138,113 @@
 
                 node_label_dict[ts][u][v] = weight
                 idx += 1
         return node_label_dict
 
 
 """
+functions for tgbn-token
+---------------------------------------
+"""
+
+def load_edgelist_token(
+    fname: str,
+    label_size: int = 1001,
+) -> pd.DataFrame:
+    """
+    load the edgelist into pandas dataframe
+    also outputs index for the user nodes and genre nodes
+    Parameters:
+        fname: str, name of the input file
+        label_size: int, number of genres
+    Returns:
+        df: a pandas dataframe containing the edgelist data
+    """
+    feat_size = 2
+    num_lines = sum(1 for line in open(fname)) - 1
+    #print("number of lines counted", num_lines)
+    print("there are ", num_lines, " lines in the raw data")
+    u_list = np.zeros(num_lines)
+    i_list = np.zeros(num_lines)
+    ts_list = np.zeros(num_lines)
+    label_list = np.zeros(num_lines)
+    feat_l = np.zeros((num_lines, feat_size))
+    idx_list = np.zeros(num_lines)
+    w_list = np.zeros(num_lines)
+
+    node_ids = {}
+    rd_dict = {}
+    node_uid = label_size  # node ids start after all the genres
+    sr_uid = 0
+
+    with open(fname, "r") as csv_file:
+        csv_reader = csv.reader(csv_file, delimiter=",")
+        idx = 0
+        # [timestamp,user_address,token_address,value,IsSender]
+        for row in tqdm(csv_reader):
+            if idx == 0:
+                idx += 1
+            else:
+                ts = row[0]
+                src = row[1]
+                token = row[2]
+                w = float(row[3])
+                attr = float(row[4])
+                if src not in node_ids:
+                    node_ids[src] = node_uid
+                    node_uid += 1
+                if token not in rd_dict:
+                    rd_dict[token] = sr_uid
+                    sr_uid += 1
+                u = node_ids[src]
+                i = rd_dict[token]
+                u_list[idx - 1] = u
+                i_list[idx - 1] = i
+                ts_list[idx - 1] = ts
+                idx_list[idx - 1] = idx
+                w_list[idx - 1] = w
+                feat_l[idx - 1] = np.array([w,attr])
+                idx += 1
+
+        return (
+            pd.DataFrame(
+                {
+                    "u": u_list,
+                    "i": i_list,
+                    "ts": ts_list,
+                    "label": label_list,
+                    "idx": idx_list,
+                    "w": w_list,
+                }
+            ),
+            feat_l,
+            node_ids,
+            rd_dict,
+        )
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+"""
 functions for subreddits dataset
 ---------------------------------------
 """
 
 
 def load_edgelist_sr(
     fname: str,
@@ -157,15 +255,15 @@
     also outputs index for the user nodes and genre nodes
     Parameters:
         fname: str, name of the input file
         label_size: int, number of genres
     Returns:
         df: a pandas dataframe containing the edgelist data
     """
-    feat_size = 2
+    feat_size = 1 #2
     num_lines = sum(1 for line in open(fname)) - 1
     #print("number of lines counted", num_lines)
     print("there are ", num_lines, " lines in the raw data")
     u_list = np.zeros(num_lines)
     i_list = np.zeros(num_lines)
     ts_list = np.zeros(num_lines)
     label_list = np.zeros(num_lines)
@@ -185,15 +283,15 @@
         for row in tqdm(csv_reader):
             if idx == 0:
                 idx += 1
             else:
                 ts = row[0]
                 src = row[1]
                 subreddit = row[2]
-                num_words = int(row[3])
+                #num_words = int(row[3])
                 score = int(row[4])
                 if src not in node_ids:
                     node_ids[src] = node_uid
                     node_uid += 1
                 if subreddit not in rd_dict:
                     rd_dict[subreddit] = sr_uid
                     sr_uid += 1
@@ -201,15 +299,15 @@
                 u = node_ids[src]
                 i = rd_dict[subreddit]
                 u_list[idx - 1] = u
                 i_list[idx - 1] = i
                 ts_list[idx - 1] = ts
                 idx_list[idx - 1] = idx
                 w_list[idx - 1] = w
-                feat_l[idx - 1] = np.array([num_words, score])
+                feat_l[idx - 1] = np.array([w])
                 idx += 1
 
         return (
             pd.DataFrame(
                 {
                     "u": u_list,
                     "i": i_list,
@@ -228,15 +326,14 @@
 def load_labels_sr(
     fname,
     node_ids,
     rd_dict,
 ):
     """
     load the node labels for subreddit dataset
-    #TODO can be further optimized when using numpy and not appending
     """
     if not osp.exists(fname):
         raise FileNotFoundError(f"File not found at {fname}")
 
     # day, user_idx, label_vec
     label_size = len(rd_dict)
     label_vec = np.zeros(label_size)
@@ -790,21 +887,20 @@
                     label_ids[genre] = label_uid
                     if label_uid >= label_size:
                         print("id overlap, terminate")
                     label_uid += 1
 
                 u = node_ids[user_id]
                 i = label_ids[genre]
-                feat = np.zeros((1))
                 u_list[idx - 1] = u
                 i_list[idx - 1] = i
                 ts_list[idx - 1] = ts
                 idx_list[idx - 1] = idx
                 w_list[idx - 1] = w
-                feat_l[idx - 1] = feat
+                feat_l[idx - 1] = np.asarray([w])
                 idx += 1
 
     return (
         pd.DataFrame(
             {"u": u_list, "i": i_list, "ts": ts_list, "idx": idx_list, "w": w_list}
         ),
         feat_l,
@@ -838,74 +934,14 @@
 
 
 """
 functions for wikipedia and un_trade
 -------------------------------------------
 """
 
-
-def _to_pd_data(
-    fname: str,
-):
-    r"""
-    convert the raw .csv data to pandas dataframe and numpy array
-    input .csv file format should be: timestamp, node u, node v, weight w,
-    Args:
-        fname: the path to the raw data
-    """
-    u_list, i_list, ts_list, label_list = [], [], [], []
-    feat_l = []
-    idx_list = []
-    w_list = []
-
-    with open(fname) as f:
-        s = next(f)
-        node_ids = {}
-        unique_id = 0
-        for idx, line in enumerate(f):
-            e = line.strip().split(",")
-            if len(e) > 4:
-                print(e)
-            # convert to integer node id
-            ts = float(e[0])
-
-            if e[1] not in node_ids:
-                node_ids[e[1]] = unique_id
-                unique_id += 1
-            if e[2] not in node_ids:
-                node_ids[e[2]] = unique_id
-                unique_id += 1
-
-            u = node_ids[e[1]]
-            i = node_ids[e[2]]
-            w = float(e[3])
-
-            label = 0
-            feat = np.zeros((1))
-
-            u_list.append(u)
-            i_list.append(i)
-            ts_list.append(ts)
-            label_list.append(label)
-            idx_list.append(idx)
-            feat_l.append(feat)
-            w_list.append(w)
-
-    return pd.DataFrame(
-        {
-            "u": u_list,
-            "i": i_list,
-            "ts": ts_list,
-            "label": label_list,
-            "idx": idx_list,
-            "w": w_list,
-        }
-    ), np.array(feat_l)
-
-
 def reindex(
     df: pd.DataFrame,
     bipartite: Optional[bool] = False,
 ):
     r"""
     reindex the nodes especially if the node ids are not integers
     Args:
```

### Comparing `py_tgb-0.7.5/tgb/utils/stats.py` & `py_tgb-0.8.0/tgb/utils/stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/tgb/utils/utils.py` & `py_tgb-0.8.0/tgb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.5/PKG-INFO` & `py_tgb-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tgb
-Version: 0.7.5
+Version: 0.8.0
 Summary: Temporal Graph Benchmark project repo
 Author: shenyang Huang
 Author-email: shenyang.huang@mail.mcgill.ca
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -33,17 +33,29 @@
 - TGB includes large-scale and realistic datasets from five different domains with both dynamic link prediction and node property prediction tasks
 - TGB automatically downloads datasets and processes them into `numpy`, `PyTorch` and `PyG compatible TemporalData` formats. 
 - Novel TG models can be easily evaluated on TGB datasets via reproducible and realistic evaluation protocols. 
 - TGB provides public and online leaderboards to track recent developments in temporal graph learning domain
 
 ![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
 
+**To submit to [TGB leaderboard](https://tgb.complexdatalab.com/), please fill in this [google form](https://forms.gle/SEsXvN1QHo9tSFwx9)**
+
+**See all version differences and update notes [here](https://tgb.complexdatalab.com/docs/update/)**
+
 ### Annoucements
 
-**Please update to version `0.7.5`**
+**Please update to version `0.8.0`**
+
+#### version `0.8.0`
+
+fixing metric computation issue in node property prediction task, `tgbn` leaderboards results are updated to reflect the changes.
+Please refer to `examples/nodeproppred/` example folders to how to compute the metric correctly. No changes for `linkproppred` datasets.
+
+
+#### version `0.7.5`
 
 the negative samples for the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of the dataset would be needed (will be prompted automatically in this version when you use the dataloader)
 
 
 ### Pip Install
 
 You can install TGB via [pip](https://pypi.org/project/py-tgb/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-tgb Version: 0.7.5 Summary: Temporal Graph
+Metadata-Version: 2.1 Name: py-tgb Version: 0.8.0 Summary: Temporal Graph
 Benchmark project repo Author: shenyang Huang Author-email:
 shenyang.huang@mail.mcgill.ca Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: clint (>=0.5.1,<0.6.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) Requires-Dist:
@@ -16,20 +16,27 @@
 realistic datasets from five different domains with both dynamic link
 prediction and node property prediction tasks - TGB automatically downloads
 datasets and processes them into `numpy`, `PyTorch` and `PyG compatible
 TemporalData` formats. - Novel TG models can be easily evaluated on TGB
 datasets via reproducible and realistic evaluation protocols. - TGB provides
 public and online leaderboards to track recent developments in temporal graph
 learning domain ![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
-### Annoucements **Please update to version `0.7.5`** the negative samples for
-the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of
-the dataset would be needed (will be prompted automatically in this version
-when you use the dataloader) ### Pip Install You can install TGB via [pip]
-(https://pypi.org/project/py-tgb/) ``` pip install py-tgb ``` ### Links and
-Datasets The project website can be found [here](https://
+**To submit to [TGB leaderboard](https://tgb.complexdatalab.com/), please fill
+in this [google form](https://forms.gle/SEsXvN1QHo9tSFwx9)** **See all version
+differences and update notes [here](https://tgb.complexdatalab.com/docs/update/
+)** ### Annoucements **Please update to version `0.8.0`** #### version `0.8.0`
+fixing metric computation issue in node property prediction task, `tgbn`
+leaderboards results are updated to reflect the changes. Please refer to
+`examples/nodeproppred/` example folders to how to compute the metric
+correctly. No changes for `linkproppred` datasets. #### version `0.7.5` the
+negative samples for the `tgbl-wiki` and `tgbl-review` dataset has been updated
+and redownload of the dataset would be needed (will be prompted automatically
+in this version when you use the dataloader) ### Pip Install You can install
+TGB via [pip](https://pypi.org/project/py-tgb/) ``` pip install py-tgb ``` ###
+Links and Datasets The project website can be found [here](https://
 tgb.complexdatalab.com/). The API documentations can be found [here](https://
 shenyanghuang.github.io/TGB/). all dataset download links can be found at
 [info.py](https://github.com/shenyangHuang/TGB/blob/main/tgb/utils/info.py) TGB
 dataloader will also automatically download the dataset as well as the negative
 samples for the link property prediction datasets. ### Running Example Methods
 - For the dynamic link property prediction task, see the [`examples/
 linkproppred`](https://github.com/shenyangHuang/TGB/tree/main/examples/
```

