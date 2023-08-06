# Comparing `tmp/bactopia-1.0.4.tar.gz` & `tmp/bactopia-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bactopia-1.0.4.tar", max compression
+gzip compressed data, was "bactopia-1.0.5.tar", max compression
```

## Comparing `bactopia-1.0.4.tar` & `bactopia-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1065 2023-07-01 00:24:13.088709 bactopia-1.0.4/LICENSE
--rw-r--r--   0        0        0    27493 2023-07-01 00:24:13.088709 bactopia-1.0.4/README.md
--rw-r--r--   0        0        0      113 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/__init__.py
--rw-r--r--   0        0        0     2667 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/citations.py
--rw-r--r--   0        0        0     5118 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/datasets.py
--rw-r--r--   0        0        0    19341 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/download.py
--rw-r--r--   0        0        0     2416 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/jsonify.py
--rw-r--r--   0        0        0    16397 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/prepare.py
--rw-r--r--   0        0        0    20125 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/search.py
--rw-r--r--   0        0        0    15455 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/summary.py
--rw-r--r--   0        0        0     1388 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parse.py
--rw-r--r--   0        0        0      267 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/__init__.py
--rw-r--r--   0        0        0      484 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/amrfinderplus.py
--rw-r--r--   0        0        0     1000 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/annotator.py
--rw-r--r--   0        0        0     2783 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/ariba.py
--rw-r--r--   0        0        0      664 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/assembler.py
--rw-r--r--   0        0        0     4673 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/blast.py
--rw-r--r--   0        0        0     1365 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/error.py
--rw-r--r--   0        0        0      372 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/gather.py
--rw-r--r--   0        0        0     1492 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/generic.py
--rw-r--r--   0        0        0     2683 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/mapping.py
--rw-r--r--   0        0        0      640 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/mlst.py
--rw-r--r--   0        0        0     1500 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/parsables.py
--rw-r--r--   0        0        0     3093 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/qc.py
--rw-r--r--   0        0        0     5014 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/sketcher.py
--rw-r--r--   0        0        0     2574 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/variants.py
--rw-r--r--   0        0        0      874 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/versions.py
--rw-r--r--   0        0        0     5292 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/summary.py
--rw-r--r--   0        0        0     4496 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/utils.py
--rw-r--r--   0        0        0     1034 2023-07-01 00:24:13.092709 bactopia-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    29064 1970-01-01 00:00:00.000000 bactopia-1.0.4/setup.py
--rw-r--r--   0        0        0    28407 1970-01-01 00:00:00.000000 bactopia-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-06 22:48:25.742203 bactopia-1.0.5/LICENSE
+-rw-r--r--   0        0        0    27493 2023-08-06 22:48:25.742203 bactopia-1.0.5/README.md
+-rw-r--r--   0        0        0      113 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/__init__.py
+-rw-r--r--   0        0        0     2667 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/citations.py
+-rw-r--r--   0        0        0     5118 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/datasets.py
+-rw-r--r--   0        0        0    19587 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/download.py
+-rw-r--r--   0        0        0     2416 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/jsonify.py
+-rw-r--r--   0        0        0    16397 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/prepare.py
+-rw-r--r--   0        0        0    20125 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/search.py
+-rw-r--r--   0        0        0    16184 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/summary.py
+-rw-r--r--   0        0        0     5682 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/cli/update.py
+-rw-r--r--   0        0        0     1388 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parse.py
+-rw-r--r--   0        0        0      267 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/__init__.py
+-rw-r--r--   0        0        0      484 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/amrfinderplus.py
+-rw-r--r--   0        0        0     1000 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/annotator.py
+-rw-r--r--   0        0        0     2783 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/ariba.py
+-rw-r--r--   0        0        0      664 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/assembler.py
+-rw-r--r--   0        0        0     4673 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/blast.py
+-rw-r--r--   0        0        0     1365 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/error.py
+-rw-r--r--   0        0        0      372 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/gather.py
+-rw-r--r--   0        0        0     1492 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/generic.py
+-rw-r--r--   0        0        0     2683 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/mapping.py
+-rw-r--r--   0        0        0      640 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/mlst.py
+-rw-r--r--   0        0        0     1883 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/parsables.py
+-rw-r--r--   0        0        0     3093 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/qc.py
+-rw-r--r--   0        0        0     5014 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/sketcher.py
+-rw-r--r--   0        0        0     2574 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/variants.py
+-rw-r--r--   0        0        0      874 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/parsers/versions.py
+-rw-r--r--   0        0        0     5292 2023-08-06 22:48:25.742203 bactopia-1.0.5/bactopia/summary.py
+-rw-r--r--   0        0        0     4496 2023-08-06 22:48:25.746203 bactopia-1.0.5/bactopia/utils.py
+-rw-r--r--   0        0        0     1079 2023-08-06 22:48:25.746203 bactopia-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    29131 1970-01-01 00:00:00.000000 bactopia-1.0.5/setup.py
+-rw-r--r--   0        0        0    28407 1970-01-01 00:00:00.000000 bactopia-1.0.5/PKG-INFO
```

### Comparing `bactopia-1.0.4/LICENSE` & `bactopia-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/README.md` & `bactopia-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/cli/citations.py` & `bactopia-1.0.5/bactopia/cli/citations.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/cli/datasets.py` & `bactopia-1.0.5/bactopia/cli/datasets.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/cli/download.py` & `bactopia-1.0.5/bactopia/cli/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,17 +135,23 @@
                         modules[module] = True
         if "modules" in workflows[wf]:
             for module in workflows[wf]["modules"]:
                 modules[module] = True
         if "path" in workflows[wf]:
             modules[wf] = True
 
-        if include_merlin and wf == "bactopia":
-            for module in workflows["merlin"]["modules"]:
+        if wf == "bactopia" or wf == "staphopia":
+            # Build Prokka and Bakta
+            modules["prokka"] = True
+            for module in workflows["bakta"]["modules"]:
                 modules[module] = True
+            # Install Merlin tools
+            if include_merlin:
+                for module in workflows["merlin"]["modules"]:
+                    modules[module] = True
 
         for module in modules:
             final_workflows[wf][module] = parse_module(
                 f'{bactopia_path}/{workflows[module]["path"]}/main.nf'
             )
 
         final_workflows[wf]["custom_dumpsoftwareversions"] = parse_module(
```

### Comparing `bactopia-1.0.4/bactopia/cli/jsonify.py` & `bactopia-1.0.5/bactopia/cli/jsonify.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/cli/prepare.py` & `bactopia-1.0.5/bactopia/cli/prepare.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/cli/search.py` & `bactopia-1.0.5/bactopia/cli/search.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/cli/summary.py` & `bactopia-1.0.5/bactopia/cli/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,43 +365,54 @@
                 errors = parse_errors(sample["path"], sample["id"])
                 if errors:
                     # Sample has errors, skip parsing
                     process_errors(sample["id"], errors)
                 else:
                     # Get list of files to parse
                     df = pd.DataFrame()
-                    for path, parser in get_parsable_files(
+                    is_complete, parsable_files = get_parsable_files(
                         sample["path"], sample["id"]
-                    ).items():
-                        if Path(path).exists() or parser == "qc":
-                            logging.debug(f"\tParsing {path} ({parser})")
-                            if df.empty:
-                                df = pd.DataFrame(
-                                    [getattr(parsers, parser).parse(path, sample["id"])]
-                                )
-                            else:
-                                df = pd.merge(
-                                    df,
-                                    pd.DataFrame(
+                    )
+                    if is_complete:
+                        for path, parser in parsable_files.items():
+                            if Path(path).exists() or parser == "qc":
+                                logging.debug(f"\tParsing {path} ({parser})")
+                                if df.empty:
+                                    df = pd.DataFrame(
                                         [
                                             getattr(parsers, parser).parse(
                                                 path, sample["id"]
                                             )
                                         ]
-                                    ),
-                                    on="sample",
-                                    how="inner",
-                                )
-                    rank, reason = process_sample(df, RANK_CUTOFF)
-                    processed_samples[sample["id"]] = True
-                    df["rank"] = rank
-                    df["reason"] = reason
-                    dfs.append(df)
-                    logging.debug(f"\tRank: {rank} ({reason})")
-
+                                    )
+                                else:
+                                    df = pd.merge(
+                                        df,
+                                        pd.DataFrame(
+                                            [
+                                                getattr(parsers, parser).parse(
+                                                    path, sample["id"]
+                                                )
+                                            ]
+                                        ),
+                                        on="sample",
+                                        how="inner",
+                                    )
+                        rank, reason = process_sample(df, RANK_CUTOFF)
+                        processed_samples[sample["id"]] = True
+                        df["rank"] = rank
+                        df["reason"] = reason
+                        dfs.append(df)
+                        logging.debug(f"\tRank: {rank} ({reason})")
+                    else:
+                        missing_files = ";".join(parsable_files)
+                        logging.debug(
+                            f"Skipping {sample['id']} ({sample['path']}) due to missing files: {missing_files}"
+                        )
+                        increment_and_append("ignore-unknown", sample["id"])
             else:
                 logging.debug(
                     f"Skipping {sample['id']} ({sample['path']}), incomplete or not a Bactopia directory"
                 )
                 increment_and_append("ignore-unknown", sample["id"])
     final_df = pd.concat(dfs)
     for col in EXCLUDE_COLUMNS:
```

### Comparing `bactopia-1.0.4/bactopia/parse.py` & `bactopia-1.0.5/bactopia/parse.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/annotator.py` & `bactopia-1.0.5/bactopia/parsers/annotator.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/ariba.py` & `bactopia-1.0.5/bactopia/parsers/ariba.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/assembler.py` & `bactopia-1.0.5/bactopia/parsers/assembler.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/blast.py` & `bactopia-1.0.5/bactopia/parsers/blast.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/error.py` & `bactopia-1.0.5/bactopia/parsers/error.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/generic.py` & `bactopia-1.0.5/bactopia/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/mapping.py` & `bactopia-1.0.5/bactopia/parsers/mapping.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/mlst.py` & `bactopia-1.0.5/bactopia/parsers/mlst.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/parsables.py` & `bactopia-1.0.5/bactopia/parsers/parsables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A list of files that can be parsed by Bactopia
 """
+from pathlib import Path
 
 EXCLUDE_COLUMNS = [
     "qc_final_per_base_quality",
     "qc_final_r1_per_base_quality",
     "qc_final_r2_per_base_quality",
     "qc_final_read_lengths",
     "qc_final_r1_read_lengths",
@@ -18,15 +19,15 @@
     "qc_original_r2_read_lengths",
     "amrfinderplus_genes_hits",
     "amrfinderplus_proteins_hits",
 ]
 
 
 def get_parsable_files(path: str, name: str) -> list:
-    return {
+    parsable_files = {
         # main
         # annotator
         f"{path}/main/annotator/prokka/{name}.txt": "annotator",
         # assembler
         f"{path}/main/assembler/{name}.tsv": "assembler",
         # gather
         f"{path}/main/gather/{name}-meta.tsv": "gather",
@@ -39,7 +40,19 @@
         # bactopia-tools
         # amrfinderplus
         f"{path}/tools/amrfinderplus/{name}-genes.tsv": "amrfinderplus",
         f"{path}/tools/amrfinderplus/{name}-proteins.tsv": "amrfinderplus",
         # mlst
         f"{path}/tools/mlst/{name}.tsv": "mlst",
     }
+
+    is_complete = True
+    missing_files = []
+    for output_file, output_type in parsable_files.items():
+        if not Path(output_file).exists():
+            is_complete = False
+            missing_files.append(output_file)
+
+    if is_complete:
+        return [is_complete, parsable_files]
+    else:
+        return [is_complete, missing_files]
```

### Comparing `bactopia-1.0.4/bactopia/parsers/qc.py` & `bactopia-1.0.5/bactopia/parsers/qc.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/sketcher.py` & `bactopia-1.0.5/bactopia/parsers/sketcher.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/variants.py` & `bactopia-1.0.5/bactopia/parsers/variants.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/parsers/versions.py` & `bactopia-1.0.5/bactopia/parsers/versions.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/summary.py` & `bactopia-1.0.5/bactopia/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/bactopia/utils.py` & `bactopia-1.0.5/bactopia/utils.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.4/pyproject.toml` & `bactopia-1.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bactopia"
-version = "1.0.4"
+version = "1.0.5"
 description = "A Python package for working with Bactopia"
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://bactopia.github.io/"
@@ -14,14 +14,15 @@
 [tool.poetry.scripts]
 bactopia-citations = "bactopia.cli.citations:main"
 bactopia-datasets = "bactopia.cli.datasets:main"
 bactopia-download = "bactopia.cli.download:main"
 bactopia-prepare = "bactopia.cli.prepare:main"
 bactopia-search = "bactopia.cli.search:main"
 bactopia-summary = "bactopia.cli.summary:main"
+bactopia-update = "bactopia.cli.update:main"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 requests = "^2.28.2"
 rich-click = "^1.6.1"
 executor = "^23.2"
 rich = "^13.3.1"
```

### Comparing `bactopia-1.0.4/setup.py` & `bactopia-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 entry_points = \
 {'console_scripts': ['bactopia-citations = bactopia.cli.citations:main',
                      'bactopia-datasets = bactopia.cli.datasets:main',
                      'bactopia-download = bactopia.cli.download:main',
                      'bactopia-prepare = bactopia.cli.prepare:main',
                      'bactopia-search = bactopia.cli.search:main',
-                     'bactopia-summary = bactopia.cli.summary:main']}
+                     'bactopia-summary = bactopia.cli.summary:main',
+                     'bactopia-update = bactopia.cli.update:main']}
 
 setup_kwargs = {
     'name': 'bactopia',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'A Python package for working with Bactopia',
     'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version        -V        Show the version and exit.                             │\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │\n│                               [required]                                             │\n│    --name           -n  TEXT  Only print citation matching a given name              │\n│    --plain-text     -p        Disable rich formatting                                │\n│    --help                     Show this message and exit.                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-datasets`\n\n```{bash}\n Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...\n\n Download optional datasets to supplement your analyses with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Download Related Options ───────────────────────────────────────────────────────────╮\n│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │\n│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │\n│                              will be created)                                        │\n│                              [default: ${HOME}/.bactopia]                 │\n│ --force                      Force overwrite of existing pre-built environments.     │\n│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │\n│                              (Default: 3)                                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bactopia.github.io/',
```

### Comparing `bactopia-1.0.4/PKG-INFO` & `bactopia-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bactopia
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package for working with Bactopia
 Home-page: https://bactopia.github.io/
 License: MIT
 Keywords: bioinformatics,bacteria,bactopia,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

