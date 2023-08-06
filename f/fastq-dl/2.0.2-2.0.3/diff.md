# Comparing `tmp/fastq_dl-2.0.2.tar.gz` & `tmp/fastq_dl-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastq_dl-2.0.2.tar", max compression
+gzip compressed data, was "fastq_dl-2.0.3.tar", max compression
```

## Comparing `fastq_dl-2.0.2.tar` & `fastq_dl-2.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/LICENSE
--rw-r--r--   0        0        0    10364 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/fastq_dl/__init__.py
--rwxr-xr-x   0        0        0    25349 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/fastq_dl/fastq_dl.py
--rw-r--r--   0        0        0      917 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    11469 1970-01-01 00:00:00.000000 fastq_dl-2.0.2/setup.py
--rw-r--r--   0        0        0    11324 1970-01-01 00:00:00.000000 fastq_dl-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-06 22:20:45.948744 fastq_dl-2.0.3/LICENSE
+-rw-r--r--   0        0        0    11707 2023-08-06 22:20:45.948744 fastq_dl-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 22:20:45.948744 fastq_dl-2.0.3/fastq_dl/__init__.py
+-rwxr-xr-x   0        0        0    29156 2023-08-06 22:20:45.948744 fastq_dl-2.0.3/fastq_dl/fastq_dl.py
+-rw-r--r--   0        0        0      917 2023-08-06 22:20:45.952744 fastq_dl-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    12827 1970-01-01 00:00:00.000000 fastq_dl-2.0.3/setup.py
+-rw-r--r--   0        0        0    12667 1970-01-01 00:00:00.000000 fastq_dl-2.0.3/PKG-INFO
```

### Comparing `fastq_dl-2.0.2/LICENSE` & `fastq_dl-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq_dl-2.0.2/README.md` & `fastq_dl-2.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,36 @@
-[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/bactopia/rpetit3/fastq-dl)
+Metadata-Version: 2.1
+Name: fastq-dl
+Version: 2.0.3
+Summary: Download FASTQ files from SRA or ENA repositories.
+Home-page: https://github.com/rpetit3/fastq-dl
+License: MIT
+Keywords: bioinformatics,fastq,download,SRA,ENA
+Author: Robert A. Petit III
+Author-email: robbie.petit@gmail.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: executor (>=23.2,<24.0)
+Requires-Dist: markdown-it-py (==2.2.0)
+Requires-Dist: pysradb (>=1.4,<2.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Project-URL: Repository, https://github.com/rpetit3/fastq-dl
+Description-Content-Type: text/markdown
+
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/rpetit3/fastq-dl/releases)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/rpetit3/fastq-dl)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8051230.svg)](https://doi.org/10.5281/zenodo.8051230)
 
 # fastq-dl
 
 Download FASTQ files from the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) or the
 [Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) repositories.
 
 ## Introduction
@@ -26,41 +52,47 @@
 conda activate fastq-dl 
 ```
 
 ## Usage
 
 ```{bash}
 fastq-dl --help
-                                                                                          
- Usage: fastq-dl [OPTIONS]                                                                
-                                                                                          
- Download FASTQ files from ENA or SRA.                                                    
-                                                                                          
-╭─ Required Options ─────────────────────────────────────────────────────────────────────╮
-│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run  │
-│                           accession) [required]                                        │
-╰────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Additional Options ───────────────────────────────────────────────────────────────────╮
-│ --provider                 [ena|sra]  Specify which provider (ENA or SRA) to use.      │
-│                                       [default: ena]                                   │
-│ --group-by-experiment                 Group Runs by experiment accession.              │
-│ --group-by-sample                     Group Runs by sample accession.                  │
-│ --outdir               -o  TEXT       Directory to output downloads to. [default: ./]  │
-│ --prefix                   TEXT       Prefix to use for naming log files.              │
-│                                       [default: fastq]                                 │
-│ --cpus                     INTEGER    Total cpus used for downloading from SRA.        │
-│                                       [default: 1]                                     │
-│ --max-attempts         -m  INTEGER    Maximum number of download attempts.             │
-│                                       [default: 10]                                    │
-│ --only-provider        -F             Only attempt download from specified provider.   │
-│ --silent                              Only critical errors will be printed.            │
-│ --version              -V             Show the version and exit.                       │
-│ --verbose              -v             Print debug related text.                        │
-│ --help                 -h             Show this message and exit.                      │
-╰────────────────────────────────────────────────────────────────────────────────────────╯
+
+ Usage: fastq-dl [OPTIONS]                                                                        
+                                                                                                  
+ Download FASTQ files from ENA or SRA.                                                            
+                                                                                                  
+╭─ Required Options ─────────────────────────────────────────────────────────────────────────────╮
+│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run          │
+│                           accession)                                                           │
+│                           [required]                                                           │
+╰────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Additional Options ───────────────────────────────────────────────────────────────────────────╮
+│ --provider                    [ena|sra]  Specify which provider (ENA or SRA) to use.           │
+│                                          [default: ena]                                        │
+│ --group-by-experiment                    Group Runs by experiment accession.                   │
+│ --group-by-sample                        Group Runs by sample accession.                       │
+│ --outdir                  -o  TEXT       Directory to output downloads to. [default: ./]       │
+│ --prefix                      TEXT       Prefix to use for naming log files. [default: fastq]  │
+│ --cpus                        INTEGER    Total cpus used for downloading from SRA.             │
+│                                          [default: 1]                                          │
+│ --max-attempts            -m  INTEGER    Maximum number of download attempts. [default: 10]    │
+│ --force                                  Overwrite existing files if their MD5 checksums do    │
+│                                          not match.                                            │
+│ --sra-lite                               Set preference to SRA Lite                            │
+│ --only-provider                          Only attempt download from specified provider.        │
+│ --only-download-metadata                 Skip FASTQ downloads, and retrieve only the metadata. │
+│ --silent                                 Only critical errors will be printed.                 │
+│ --sleep                   -s  INTEGER    Minimum amount of time to sleep between retries (API  │
+│                                          query and download)                                   │
+│                                          [default: 10]                                         │
+│ --version                 -V             Show the version and exit.                            │
+│ --verbose                 -v             Print debug related text.                             │
+│ --help                    -h             Show this message and exit.                           │
+╰────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 *fastq-dl* requires a single ENA/SRA Study, Sample, Experiment, or Run accession and FASTQs
 for all Runs that fall under the given accession will be downloaded. For example, if a Study
 accession is given all Runs under that studies umbrella will be downloaded. By default, 
 `fastq-dl` will try to download from ENA first, then SRA.
 
@@ -98,14 +130,22 @@
 
 ### --group-by-experiment & --group-by-sample
 
 There maybe times you might want to group Run accessions based on a Experiment or Sample
 accessions. This will merge FASTQs associated with a Run accession based its associated
 Experiment accession (`--group-by-experiment`) or Sample accession (`--group-by-sample`).
 
+### --sra-lite
+
+Downloads from SRA are provided in [SRA Normalized and SRA Lite](https://www.ncbi.nlm.nih.gov/sra/docs/sra-data-formats/) formats.
+SRA Normalized is the original format with full base quality scores and SRA Lite are smaller
+due to simplifying the quality scores to a uniform Q30. By default the preference will be
+set to SRA Normalized, if you prefer SRA Lite you can use `--sra-lite` to set the
+preference to SRA Lite.
+
 ## Output Files
 
 | Extension          | Description                                                                              |
 |--------------------|------------------------------------------------------------------------------------------|
 | `-run-info.tsv`    | Tab-delimited file containing metadata for each Run downloaded                           |
 | `-run-mergers.tsv` | Tab-delimited file merge information from `--group-by-experiment` or `--group-by-sample` |
 | `.fastq.gz`        | FASTQ files downloaded from ENA or SRA                                                   |
@@ -174,7 +214,8 @@
 line (1-to-1 relationship), so you will always get the expected Run.
 
 ## Alternatives
 `fastq-dl`, is a spin-off of [ena-dl](https://github.com/rpetit3/ena-dl), that has been developed for
 usage with [Bactopia](https://github.com/bactopia/bactopia). With this in mind, EBI/NCBI and provide
 their own tools ([enaBrowserTools](https://github.com/enasequence/enaBrowserTools) and
 [SRA Toolkit](https://github.com/ncbi/sra-tools)) that offer more extensive access to their databases.
+
```

### Comparing `fastq_dl-2.0.2/fastq_dl/fastq_dl.py` & `fastq_dl-2.0.3/fastq_dl/fastq_dl.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,19 @@
                 "--group-by-experiment",
                 "--group-by-sample",
                 "--outdir",
                 "--prefix",
                 "--cpus",
                 "--max-attempts",
                 "--force",
+                "--sra-lite",
                 "--only-provider",
                 "--only-download-metadata",
                 "--silent",
+                "--sleep",
                 "--version",
                 "--verbose",
                 "--help",
             ],
         },
     ]
 }
@@ -53,25 +55,27 @@
     cmd: str,
     directory: str = str(Path.cwd()),
     capture_stdout: bool = False,
     stdout_file: str = None,
     stderr_file: str = None,
     max_attempts: int = 1,
     is_sra: bool = False,
+    sleep: int = 10,
 ) -> str:
     """A simple wrapper around executor.
 
     Args:
         cmd (str): A command to execute.
         directory (str, optional): Set the working directory for command. Defaults to str(Path.cwd()).
         capture_stdout (bool, optional): Capture and return the STDOUT of a command. Defaults to False.
         stdout_file (str, optional): File to write STDOUT to. Defaults to None.
         stderr_file (str, optional): File to write STDERR to. Defaults to None.
         max_attempts (int, optional): Maximum times to attempt command execution. Defaults to 1.
         is_sra (bool, optional): The command is from SRA. Defaults to False.
+        sleep (int): Minimum amount of time to sleep before retry
 
     Raises:
         error: An unexpected error occurred.
 
     Returns:
         str: Exit code, accepted error message, or STDOUT of command.
     """
@@ -103,36 +107,41 @@
                 # The FASTQ isn't on SRA for some reason, try to download from ENA
                 error_msg = command.decoded_stderr.split("\n")[0]
                 logging.error(error_msg)
                 return SRA_FAILED
 
             if attempt < max_attempts:
                 logging.error(f"Retry execution ({attempt} of {max_attempts})")
-                time.sleep(10)
+                time.sleep(sleep)
             else:
                 if is_sra:
                     return SRA_FAILED
                 else:
                     return ENA_FAILED
 
 
 def sra_download(
     accession: str,
     outdir: str,
     cpus: int = 1,
     max_attempts: int = 10,
     force: bool = False,
+    sleep: int = 10,
+    sra_lite: bool = False,
 ) -> dict:
     """Download FASTQs from SRA using fasterq-dump.
 
     Args:
         accession (str): The accession to download associated FASTQs.
         outdir (str): Directory to write FASTQs to.
         cpus (int, optional): Number of CPUs to use. Defaults to 1.
         max_attempts (int, optional): Maximum number of download attempts. Defaults to 10.
+        force (bool, optional): Force overwrite of existing files
+        sleep (int, default = 10): Amount of seconds to sleep in between attempts
+        sra_lite (bool, optional): If True, prefer SRA Lite downloads
 
     Returns:
         dict: A dictionary of the FASTQs and their paired status.
     """
     fastqs = {"r1": "", "r2": "", "single_end": True}
     se = f"{outdir}/{accession}.fastq.gz"
     pe1 = f"{outdir}/{accession}_1.fastq.gz"
@@ -148,30 +157,41 @@
         Path(pe2).unlink()
         logging.warning(f"Overwriting existing file: {pe1}")
         logging.warning(f"Overwriting existing file: {pe2}")
 
     if not Path(se).exists() and not (Path(pe1).exists() and Path(pe2).exists()):
         Path(outdir).mkdir(parents=True, exist_ok=True)
 
+        if sra_lite:
+            # Prefer SRA Lite
+            logging.debug("Setting preference to SRA Lite")
+            execute("vdb-config --simplified-quality-scores yes")
+        else:
+            # Prefer SRA Normalized
+            logging.debug("Setting preference to SRA Normalized")
+            execute("vdb-config --simplified-quality-scores no")
+
         # TODO: add check of read count as a proxy for checksum?
         outcome = execute(
             f"prefetch {accession} --max-size 10T -o {accession}.sra",
             max_attempts=max_attempts,
             directory=outdir,
             is_sra=True,
+            sleep=sleep,
         )
 
         if outcome == SRA_FAILED:
             return outcome
         else:
             outcome = execute(
                 f"fasterq-dump {accession} --split-3 --mem 1G --threads {cpus}",
                 max_attempts=max_attempts,
                 directory=outdir,
                 is_sra=True,
+                sleep=sleep,
             )
 
         if outcome == SRA_FAILED:
             return outcome
         else:
             execute(f"pigz --force -p {cpus} -n {accession}*.fastq", directory=outdir)
             Path(f"{outdir}/{accession}.sra").unlink()
@@ -193,23 +213,24 @@
     else:
         fastqs["r1"] = f"{outdir}/{accession}.fastq.gz"
 
     return fastqs
 
 
 def ena_download(
-    run: str, outdir: str, max_attempts: int = 10, force: bool = False
+    run: str, outdir: str, max_attempts: int = 10, force: bool = False, sleep: int = 10
 ) -> dict:
     """Download FASTQs from ENA FTP using wget.
 
     Args:
         accession (str): The accession to download associated FASTQs.
         outdir (str): Directory to write FASTQs to.
         max_attempts (int, optional): Maximum number of download attempts. Defaults to 10.
         force: (bool, optional): Whether to overwrite existing files if the MD5's do not match
+        sleep (int): Minimum amount of time to sleep before retry
 
     Returns:
         dict: A dictionary of the FASTQs and their paired status.
     """
     fastqs = {"r1": "", "r2": "", "single_end": True}
     ftp = run["fastq_ftp"]
     if not ftp:
@@ -237,15 +258,20 @@
                 exp_fq = f'{run["run_accession"]}.fastq.gz'
                 if len(ftp) != 1 and obs_fq != exp_fq:
                     continue
 
         # Download Run
         if md5[i]:
             fastq = download_ena_fastq(
-                ftp[i], outdir, md5[i], max_attempts=max_attempts, force=force
+                ftp[i],
+                outdir,
+                md5[i],
+                max_attempts=max_attempts,
+                force=force,
+                sleep=sleep,
             )
             if fastq == ENA_FAILED:
                 return ENA_FAILED
 
             if is_r2:
                 fastqs["r2"] = fastq
                 fastqs["single_end"] = False
@@ -281,23 +307,25 @@
 
 def download_ena_fastq(
     ftp: str,
     outdir: str,
     md5: str,
     max_attempts: int = 10,
     force: bool = False,
+    sleep: int = 10,
 ) -> str:
     """Download FASTQs from ENA using FTP.
 
     Args:
         ftp (str): The FTP address of the FASTQ file.
         outdir (str): Directory to download the FASTQ to.
         md5 (str): Expected MD5 checksum of the FASTQ.
         max_attempts (int, optional): Maximum number of download attempts. Defaults to 10.
         force: (bool, optional): Whether to overwrite existing files if the MD5's do not match
+        sleep (int): Minimum amount of time to sleep before retry
 
     Returns:
         str: Path to the downloaded FASTQ.
     """
     success = False
     attempt = 0
     fastq = f"{outdir}/{Path(ftp).name}"
@@ -308,15 +336,17 @@
 
     if not Path(fastq).exists():
         Path(outdir).mkdir(parents=True, exist_ok=True)
 
         while not success:
             logging.info(f"\t\t{Path(ftp).name} FTP download attempt {attempt + 1}")
             outcome = execute(
-                f"wget --quiet -O {fastq} ftp://{ftp}", max_attempts=max_attempts
+                f"wget --quiet -O {fastq} ftp://{ftp}",
+                max_attempts=max_attempts,
+                sleep=sleep,
             )
             if outcome == ENA_FAILED:
                 return ENA_FAILED
 
             if force:
                 logging.debug(f"--force used, skipping MD5sum check for {fastq}")
                 success = True
@@ -329,17 +359,14 @@
                         Path(fastq).unlink()
                     if attempt > max_attempts:
                         logging.error(
                             f"Download failed after {max_attempts} attempts. "
                             "Please try again later or manually from SRA/ENA."
                         )
                         sys.exit(1)
-
-                    # Hiccup? Wait a bit before trying again.
-                    time.sleep(10)
                 else:
                     success = True
     else:
         logging.debug(f"Skipping re-download of existing file: {fastq}")
 
     return fastq
 
@@ -398,71 +425,117 @@
         for line in r.text.split("\n"):
             cols = line.rstrip().split("\t")
             if line:
                 if col_names:
                     data.append(dict(zip(col_names, cols)))
                 else:
                     col_names = cols
-        return [True, data]
+        if data:
+            return [True, data]
+        else:
+            return [
+                False,
+                [r.status_code, "Query was successful, but received an empty response"],
+            ]
     else:
         return [False, [r.status_code, r.text]]
 
 
 def get_run_info(
-    accession: str, query: str, provider: str, only_provider: bool
+    accession: str,
+    query: str,
+    provider: str,
+    only_provider: bool,
+    max_attempts: int = 10,
+    sleep: int = 10,
 ) -> tuple:
     """Retrieve a list of samples available from ENA.
 
     The first attempt will be against ENA, and if that fails, SRA will be queried. This should
     capture those samples not yet synced between ENA and SRA.
 
     Args:
         accession (str): The accession to search for.
         query (str): A formatted query for ENA searches.
         provider (str): Limit queries only to the specified provider (requires only_provider be true)
         only_provider (bool): If true, limit queries to the specified provider
+        max_attempts (int, optional): Maximum number of download attempts
+        sleep (int): Minimum amount of time to sleep before retry
 
     Returns:
         tuple: Records associated with the accession.
     """
+    # Attempt for when "--only-provider" used, others to allow multiple attempts on fallback
+    attempt = 1
+    sra_attempt = 1
+    ena_attempt = 1
+    while True:
+        if only_provider:
+            logging.debug(
+                f"Querying for metadata (Attempt {attempt} of {max_attempts})"
+            )
+            logging.debug(f"--only-provider supplied, limiting queries to {provider}")
+            if provider.lower() == "ena":
+                success, ena_data = get_ena_metadata(query)
+                if success:
+                    return ENA, ena_data
+                elif attempt >= max_attempts:
+                    logging.error("There was an issue querying ENA, exiting...")
+                    logging.error(f"STATUS: {ena_data[0]}")
+                    logging.error(f"TEXT: {ena_data[1]}")
+                    sys.exit(1)
+            else:
+                success, sra_data = get_sra_metadata(accession)
+                if success:
+                    return SRA, sra_data
+                elif attempt >= max_attempts:
+                    logging.error("There was an issue querying SRA, exiting...")
+                    sys.exit(1)
+            attempt += 1
+            logging.warning(
+                f"Querying {provider.lower()} was unsuccessful, retrying after ({sleep} seconds)"
+            )
+            time.sleep(sleep)
+        else:
+            if ena_attempt < max_attempts:
+                logging.debug(
+                    f"Querying ENA for metadata (Attempt {ena_attempt} of {max_attempts})"
+                )
+            else:
+                logging.debug(
+                    f"Querying SRA for metadata (Attempt {sra_attempt} of {max_attempts})"
+                )
 
-    logging.debug("Querying ENA for metadata...")
-
-    if only_provider:
-        logging.debug(f"--only-provider supplied, limiting queries to {provider}")
-        if provider.lower() == "ena":
             success, ena_data = get_ena_metadata(query)
             if success:
                 return ENA, ena_data
+            elif ena_attempt >= max_attempts:
+                if ena_attempt == max_attempts:
+                    ena_attempt += 1
+                    logging.debug("Failed to get metadata from ENA. Trying SRA...")
+                success, sra_data = get_sra_metadata(accession)
+                if success:
+                    return SRA, sra_data
+                elif sra_attempt >= max_attempts:
+                    logging.error("There was an issue querying ENA and SRA, exiting...")
+                    logging.error(f"STATUS: {ena_data[0]}")
+                    logging.error(f"TEXT: {ena_data[1]}")
+                    sys.exit(1)
+                else:
+                    sra_attempt += 1
+                    logging.warning(
+                        f"Querying SRA was unsuccessful, retrying after ({sleep} seconds)"
+                    )
+                    time.sleep(sleep)
             else:
-                logging.error("There was an issue querying ENA, exiting...")
-                logging.error(f"STATUS: {ena_data[0]}")
-                logging.error(f"TEXT: {ena_data[1]}")
-                sys.exit(1)
-        else:
-            success, sra_data = get_sra_metadata(accession)
-            if success:
-                return SRA, sra_data
-            else:
-                logging.error("There was an issue querying SRA, exiting...")
-                sys.exit(1)
-    else:
-        success, ena_data = get_ena_metadata(query)
-        if success:
-            return ENA, ena_data
-        else:
-            logging.debug("Failed to get metadata from ENA. Trying SRA...")
-            success, sra_data = get_sra_metadata(accession)
-            if not success:
-                logging.error("There was an issue querying ENA and SRA, exiting...")
-                logging.error(f"STATUS: {ena_data[0]}")
-                logging.error(f"TEXT: {ena_data[1]}")
-                sys.exit(1)
-            else:
-                return SRA, sra_data
+                ena_attempt += 1
+                logging.warning(
+                    f"Querying ENA was unsuccessful, retrying after ({sleep} seconds)"
+                )
+                time.sleep(sleep)
 
 
 def write_tsv(data: dict, output: str) -> None:
     """Write a TSV file.
 
     Args:
         data (dict): Data to be written to TSV.
@@ -567,19 +640,31 @@
     "--max-attempts",
     "-m",
     default=10,
     show_default=True,
     help="Maximum number of download attempts.",
 )
 @click.option(
+    "--sleep",
+    "-s",
+    default=10,
+    show_default=True,
+    help="Minimum amount of time to sleep between retries (API query and download)",
+)
+@click.option(
     "--force",
     is_flag=True,
     help="Overwrite existing files if their MD5 checksums do not match.",
 )
 @click.option(
+    "--sra-lite",
+    is_flag=True,
+    help="Set preference to SRA Lite",
+)
+@click.option(
     "--only-provider",
     is_flag=True,
     help="Only attempt download from specified provider.",
 )
 @click.option(
     "--only-download-metadata",
     is_flag=True,
@@ -598,15 +683,17 @@
     accession,
     provider,
     group_by_experiment,
     group_by_sample,
     outdir,
     prefix,
     max_attempts,
+    sleep,
     force,
+    sra_lite,
     only_provider,
     only_download_metadata,
     cpus,
     silent,
     verbose,
 ):
     """Download FASTQ files from ENA or SRA."""
@@ -620,15 +707,22 @@
     )
 
     logging.getLogger().setLevel(
         logging.ERROR if silent else logging.DEBUG if verbose else logging.INFO
     )
     # Start Download Process
     query = validate_query(accession)
-    data_from, ena_data = get_run_info(accession, query, provider, only_provider)
+    data_from, ena_data = get_run_info(
+        accession,
+        query,
+        provider,
+        only_provider,
+        max_attempts=max_attempts,
+        sleep=sleep,
+    )
 
     logging.info(f"Query: {accession}")
     logging.info(f"Archive: {provider}")
     if only_download_metadata:
         logging.info(f"Total Runs Found: {len(ena_data)}")
         logging.debug("--only-download-metadata used, skipping FASTQ downloads")
     else:
@@ -651,15 +745,19 @@
                     f"Duplicate run {run_acc} found, skipping re-download..."
                 )
                 continue
             logging.info(f"\tWorking on run {run_acc}...")
             fastqs = None
             if provider.lower() == "ena" and data_from == ENA:
                 fastqs = ena_download(
-                    run_info, outdir, max_attempts=max_attempts, force=force
+                    run_info,
+                    outdir,
+                    max_attempts=max_attempts,
+                    force=force,
+                    sleep=sleep,
                 )
 
                 if fastqs == ENA_FAILED:
                     if only_provider:
                         logging.error(f"\tNo fastqs found in ENA for {run_acc}")
                         ena_data[i]["error"] = ENA_FAILED
                         fastqs = None
@@ -668,37 +766,44 @@
                         logging.info(f"\t{run_acc} not found on ENA, retrying from SRA")
 
                         fastqs = sra_download(
                             run_acc,
                             outdir,
                             cpus=cpus,
                             max_attempts=max_attempts,
+                            sleep=sleep,
+                            sra_lite=sra_lite,
                         )
                         if fastqs == SRA_FAILED:
                             logging.error(f"\t{run_acc} not found on SRA")
                             ena_data[i]["error"] = f"{ENA_FAILED}&{SRA_FAILED}"
                             fastqs = None
-
             else:
                 fastqs = sra_download(
                     run_acc,
                     outdir,
                     cpus=cpus,
                     max_attempts=max_attempts,
+                    sleep=sleep,
+                    sra_lite=sra_lite,
                 )
                 if fastqs == SRA_FAILED:
                     if only_provider or data_from == SRA:
                         logging.error(f"\t{run_acc} not found on SRA or ENA")
                         ena_data[i]["error"] = SRA_FAILED
                         fastqs = None
                     else:
                         # Retry download from ENA
                         logging.info(f"\t{run_acc} not found on SRA, retrying from ENA")
                         fastqs = ena_download(
-                            run_info, outdir, max_attempts=max_attempts, force=force
+                            run_info,
+                            outdir,
+                            max_attempts=max_attempts,
+                            force=force,
+                            sleep=sleep,
                         )
                         if fastqs == ENA_FAILED:
                             logging.error(f"\tNo fastqs found in ENA for {run_acc}")
                             ena_data[i]["error"] = f"{SRA_FAILED}&{ENA_FAILED}"
                             fastqs = None
 
             # Add the download results
@@ -737,12 +842,15 @@
             )
             write_tsv(runs, f"{outdir}/{prefix}-run-mergers.tsv")
         logging.info(f"Writing metadata to {outdir}/{prefix}-run-info.tsv")
         write_tsv(ena_data, f"{outdir}/{prefix}-run-info.tsv")
 
 
 def main():
-    fastqdl()
+    if len(sys.argv) == 1:
+        fastqdl(["--help"])
+    else:
+        fastqdl()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fastq_dl-2.0.2/pyproject.toml` & `fastq_dl-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastq-dl"
-version = "2.0.2"
+version = "2.0.3"
 description = "Download FASTQ files from SRA or ENA repositories."
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
     "Michael B. Hall <michael@mbh.sh>",
     "Gerry Tonkin-Hill",
     "Jie Zhu",
     "Timothy D. Read"
```

### Comparing `fastq_dl-2.0.2/setup.py` & `fastq_dl-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['fastq-dl = fastq_dl.fastq_dl:main']}
 
 setup_kwargs = {
     'name': 'fastq-dl',
-    'version': '2.0.2',
+    'version': '2.0.3',
     'description': 'Download FASTQ files from SRA or ENA repositories.',
-    'long_description': "[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/bactopia/rpetit3/fastq-dl)\n[![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)\n[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/rpetit3/fastq-dl)\n\n# fastq-dl\n\nDownload FASTQ files from the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) or the\n[Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) repositories.\n\n## Introduction\n\n`fastq-dl` takes an ENA/SRA accession (Study, Sample, Experiment, or Run) and queries ENA (via\n[Data Warehouse API](https://www.ebi.ac.uk/ena/browse/search-rest)) to determine the associated\nmetadata. It then downloads FASTQ files for each Run. For Samples or Experiments with multiple\nRuns, users can optionally merge the runs.\n\n## Installation\n\n### Bioconda\n\n`fastq-dl` is available from [Bioconda](https://bioconda.github.io/) and I highly recommend you\ngo this route to for installation.\n\n```{bash}\nconda create -n fastq-dl -c conda-forge -c bioconda fastq-dl\nconda activate fastq-dl \n```\n\n## Usage\n\n```{bash}\nfastq-dl --help\n                                                                                          \n Usage: fastq-dl [OPTIONS]                                                                \n                                                                                          \n Download FASTQ files from ENA or SRA.                                                    \n                                                                                          \n╭─ Required Options ─────────────────────────────────────────────────────────────────────╮\n│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run  │\n│                           accession) [required]                                        │\n╰────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ───────────────────────────────────────────────────────────────────╮\n│ --provider                 [ena|sra]  Specify which provider (ENA or SRA) to use.      │\n│                                       [default: ena]                                   │\n│ --group-by-experiment                 Group Runs by experiment accession.              │\n│ --group-by-sample                     Group Runs by sample accession.                  │\n│ --outdir               -o  TEXT       Directory to output downloads to. [default: ./]  │\n│ --prefix                   TEXT       Prefix to use for naming log files.              │\n│                                       [default: fastq]                                 │\n│ --cpus                     INTEGER    Total cpus used for downloading from SRA.        │\n│                                       [default: 1]                                     │\n│ --max-attempts         -m  INTEGER    Maximum number of download attempts.             │\n│                                       [default: 10]                                    │\n│ --only-provider        -F             Only attempt download from specified provider.   │\n│ --silent                              Only critical errors will be printed.            │\n│ --version              -V             Show the version and exit.                       │\n│ --verbose              -v             Print debug related text.                        │\n│ --help                 -h             Show this message and exit.                      │\n╰────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n*fastq-dl* requires a single ENA/SRA Study, Sample, Experiment, or Run accession and FASTQs\nfor all Runs that fall under the given accession will be downloaded. For example, if a Study\naccession is given all Runs under that studies umbrella will be downloaded. By default, \n`fastq-dl` will try to download from ENA first, then SRA.\n\n### --accession\n\nThe accession you would like to download associated FASTQS for. Currently the following types\nof accessions are accepted.\n\n| Accession Type | Prefixes            | Example                                  |\n|----------------|---------------------|------------------------------------------|\n| BioProject     | PRJEB, PRJNA, PRJDB | PRJEB42779, PRJNA480016, PRJDB14838      |\n| Study          | ERP, DRP, SRP       | ERP126685, DRP009283, SRP158268          |\n| BioSample      | SAMD, SAME, SAMN    | SAMD00258402, SAMEA7997453, SAMN06479985 |\n| Sample         | ERS, DRS, SRS       | ERS5684710, DRS259711, SRS2024210        |\n| Experiment     | ERX, DRX, SRX       | ERX5050800, DRX406443, SRX4563689        |\n| Run            | ERR, DRR, SRR       | ERR5260405, DRR421224, SRR7706354        |\n\nThe accessions are using regular expressions from the [ENA Training Modules - Accession Numbers](https://ena-docs.readthedocs.io/en/latest/submit/general-guide/accessions.html#accession-numbers) section.\n\n### --provider\n\n`fastq-dl` gives you the option to download from ENA or SRA. the `--provider` option will\nspecify which provider you would like to attempt downloads from first. If a download fails\nfrom the first provider, additional attempts will be made using the other provider.\n\nENA was selected as the default provider because the FASTQs are available directly without\nthe need for conversion.\n\n### --only-provider\n\nBy default, `fastq-dl` will fallback on a secondary provider to attempt downloads. There\nmay be cases where you would prefer to disable this feature, and that is exactly the\npurpose of `--only-provider`. When provided, if a FASTQ cannot be downloaded from the\noriginal provider, no additional attempts will be made.\n\n### --group-by-experiment & --group-by-sample\n\nThere maybe times you might want to group Run accessions based on a Experiment or Sample\naccessions. This will merge FASTQs associated with a Run accession based its associated\nExperiment accession (`--group-by-experiment`) or Sample accession (`--group-by-sample`).\n\n## Output Files\n\n| Extension          | Description                                                                              |\n|--------------------|------------------------------------------------------------------------------------------|\n| `-run-info.tsv`    | Tab-delimited file containing metadata for each Run downloaded                           |\n| `-run-mergers.tsv` | Tab-delimited file merge information from `--group-by-experiment` or `--group-by-sample` |\n| `.fastq.gz`        | FASTQ files downloaded from ENA or SRA                                                   |\n\n## Example Usage\n\n#### Download FASTQs associated with a Study\n\nSometimes you might be reading a paper and they very kindly provided a Bioproject of all\nthe samples they sequenced. So, you decide you want to download FASTQs for all the samples\nasscociated with the Bioproject. `fastq-dl` can help you with that! \n\n```{bash}\nfastq-dl --accession PRJNA248678 --provider SRA\nfastq-dl --accession PRJNA248678\n```\n\nThe above commands will download the 3 Runs that fall under Study accession [PRJNA248678](https://www.ebi.ac.uk/ena/browser/view/PRJNA248678)\nfrom either SRA (`--provider SRA`) or ENA (without `--provider`).\n\n#### Download FASTQs associated with an Experiment\n\nLet's say instead of the whole Bioproject you just want a single Experiment. You can do\nthat as well.\n\n```{bash}\nfastq-dl --accession SRX477044\n```\n\nThe above command would download the Run accessions from ENA that fall under Experiment SRX477044.\n\nThe relationship of Experiment to Run is a 1-to-many relationship, or there can be many Run accessions\nassociated with a single Experiment Accession (e.g. re-sequencing the same sample). Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-experiment` to merge multiple runs\nassociated with an Experiment accession into a single FASTQ file.\n\n#### Download FASTQs associated with an Sample\n\nOk, this time you just want a single Sample, or Biosample.\n\n```{bash}\nfastq-dl --accession SRS1904245 --provider SRA\n```\n\nThe above command would download the Run accessions from SRA that fall under Sample SRS1904245.\n\nSimilar to Experiment accessions, the relationship of Sample to Run is a 1-to-many relationship,\nor there can be many Run accessions associated with a single Sample Accession. Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-sample` to merge multiple runs\nassociated with an Sample accession into a single FASTQ file.\n\n_Warning! For some type strains (e.g. S. aureus USA300) a Biosample accession might be associated with\n100s or 1000s of Run accessions. These Runs are likely associated with many different conditions and\nreally should not fall under a single BioSample accession. Please consider this when using\n`--group-by-sample`.\n\n#### Download FASTQs associated with a Run\n\nLet's keep it super simple and just download a Run.\n\n```\nfastq-dl --accession SRR1178105 --provider SRA\n```\n\nThe above command would download the Run SRR1178105 from SRA. Run accessions are the end of the\nline (1-to-1 relationship), so you will always get the expected Run.\n\n## Alternatives\n`fastq-dl`, is a spin-off of [ena-dl](https://github.com/rpetit3/ena-dl), that has been developed for\nusage with [Bactopia](https://github.com/bactopia/bactopia). With this in mind, EBI/NCBI and provide\ntheir own tools ([enaBrowserTools](https://github.com/enasequence/enaBrowserTools) and\n[SRA Toolkit](https://github.com/ncbi/sra-tools)) that offer more extensive access to their databases.\n",
+    'long_description': "[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/rpetit3/fastq-dl/releases)\n[![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)\n[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/rpetit3/fastq-dl)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8051230.svg)](https://doi.org/10.5281/zenodo.8051230)\n\n# fastq-dl\n\nDownload FASTQ files from the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) or the\n[Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) repositories.\n\n## Introduction\n\n`fastq-dl` takes an ENA/SRA accession (Study, Sample, Experiment, or Run) and queries ENA (via\n[Data Warehouse API](https://www.ebi.ac.uk/ena/browse/search-rest)) to determine the associated\nmetadata. It then downloads FASTQ files for each Run. For Samples or Experiments with multiple\nRuns, users can optionally merge the runs.\n\n## Installation\n\n### Bioconda\n\n`fastq-dl` is available from [Bioconda](https://bioconda.github.io/) and I highly recommend you\ngo this route to for installation.\n\n```{bash}\nconda create -n fastq-dl -c conda-forge -c bioconda fastq-dl\nconda activate fastq-dl \n```\n\n## Usage\n\n```{bash}\nfastq-dl --help\n\n Usage: fastq-dl [OPTIONS]                                                                        \n                                                                                                  \n Download FASTQ files from ENA or SRA.                                                            \n                                                                                                  \n╭─ Required Options ─────────────────────────────────────────────────────────────────────────────╮\n│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run          │\n│                           accession)                                                           │\n│                           [required]                                                           │\n╰────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ───────────────────────────────────────────────────────────────────────────╮\n│ --provider                    [ena|sra]  Specify which provider (ENA or SRA) to use.           │\n│                                          [default: ena]                                        │\n│ --group-by-experiment                    Group Runs by experiment accession.                   │\n│ --group-by-sample                        Group Runs by sample accession.                       │\n│ --outdir                  -o  TEXT       Directory to output downloads to. [default: ./]       │\n│ --prefix                      TEXT       Prefix to use for naming log files. [default: fastq]  │\n│ --cpus                        INTEGER    Total cpus used for downloading from SRA.             │\n│                                          [default: 1]                                          │\n│ --max-attempts            -m  INTEGER    Maximum number of download attempts. [default: 10]    │\n│ --force                                  Overwrite existing files if their MD5 checksums do    │\n│                                          not match.                                            │\n│ --sra-lite                               Set preference to SRA Lite                            │\n│ --only-provider                          Only attempt download from specified provider.        │\n│ --only-download-metadata                 Skip FASTQ downloads, and retrieve only the metadata. │\n│ --silent                                 Only critical errors will be printed.                 │\n│ --sleep                   -s  INTEGER    Minimum amount of time to sleep between retries (API  │\n│                                          query and download)                                   │\n│                                          [default: 10]                                         │\n│ --version                 -V             Show the version and exit.                            │\n│ --verbose                 -v             Print debug related text.                             │\n│ --help                    -h             Show this message and exit.                           │\n╰────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n*fastq-dl* requires a single ENA/SRA Study, Sample, Experiment, or Run accession and FASTQs\nfor all Runs that fall under the given accession will be downloaded. For example, if a Study\naccession is given all Runs under that studies umbrella will be downloaded. By default, \n`fastq-dl` will try to download from ENA first, then SRA.\n\n### --accession\n\nThe accession you would like to download associated FASTQS for. Currently the following types\nof accessions are accepted.\n\n| Accession Type | Prefixes            | Example                                  |\n|----------------|---------------------|------------------------------------------|\n| BioProject     | PRJEB, PRJNA, PRJDB | PRJEB42779, PRJNA480016, PRJDB14838      |\n| Study          | ERP, DRP, SRP       | ERP126685, DRP009283, SRP158268          |\n| BioSample      | SAMD, SAME, SAMN    | SAMD00258402, SAMEA7997453, SAMN06479985 |\n| Sample         | ERS, DRS, SRS       | ERS5684710, DRS259711, SRS2024210        |\n| Experiment     | ERX, DRX, SRX       | ERX5050800, DRX406443, SRX4563689        |\n| Run            | ERR, DRR, SRR       | ERR5260405, DRR421224, SRR7706354        |\n\nThe accessions are using regular expressions from the [ENA Training Modules - Accession Numbers](https://ena-docs.readthedocs.io/en/latest/submit/general-guide/accessions.html#accession-numbers) section.\n\n### --provider\n\n`fastq-dl` gives you the option to download from ENA or SRA. the `--provider` option will\nspecify which provider you would like to attempt downloads from first. If a download fails\nfrom the first provider, additional attempts will be made using the other provider.\n\nENA was selected as the default provider because the FASTQs are available directly without\nthe need for conversion.\n\n### --only-provider\n\nBy default, `fastq-dl` will fallback on a secondary provider to attempt downloads. There\nmay be cases where you would prefer to disable this feature, and that is exactly the\npurpose of `--only-provider`. When provided, if a FASTQ cannot be downloaded from the\noriginal provider, no additional attempts will be made.\n\n### --group-by-experiment & --group-by-sample\n\nThere maybe times you might want to group Run accessions based on a Experiment or Sample\naccessions. This will merge FASTQs associated with a Run accession based its associated\nExperiment accession (`--group-by-experiment`) or Sample accession (`--group-by-sample`).\n\n### --sra-lite\n\nDownloads from SRA are provided in [SRA Normalized and SRA Lite](https://www.ncbi.nlm.nih.gov/sra/docs/sra-data-formats/) formats.\nSRA Normalized is the original format with full base quality scores and SRA Lite are smaller\ndue to simplifying the quality scores to a uniform Q30. By default the preference will be\nset to SRA Normalized, if you prefer SRA Lite you can use `--sra-lite` to set the\npreference to SRA Lite.\n\n## Output Files\n\n| Extension          | Description                                                                              |\n|--------------------|------------------------------------------------------------------------------------------|\n| `-run-info.tsv`    | Tab-delimited file containing metadata for each Run downloaded                           |\n| `-run-mergers.tsv` | Tab-delimited file merge information from `--group-by-experiment` or `--group-by-sample` |\n| `.fastq.gz`        | FASTQ files downloaded from ENA or SRA                                                   |\n\n## Example Usage\n\n#### Download FASTQs associated with a Study\n\nSometimes you might be reading a paper and they very kindly provided a Bioproject of all\nthe samples they sequenced. So, you decide you want to download FASTQs for all the samples\nasscociated with the Bioproject. `fastq-dl` can help you with that! \n\n```{bash}\nfastq-dl --accession PRJNA248678 --provider SRA\nfastq-dl --accession PRJNA248678\n```\n\nThe above commands will download the 3 Runs that fall under Study accession [PRJNA248678](https://www.ebi.ac.uk/ena/browser/view/PRJNA248678)\nfrom either SRA (`--provider SRA`) or ENA (without `--provider`).\n\n#### Download FASTQs associated with an Experiment\n\nLet's say instead of the whole Bioproject you just want a single Experiment. You can do\nthat as well.\n\n```{bash}\nfastq-dl --accession SRX477044\n```\n\nThe above command would download the Run accessions from ENA that fall under Experiment SRX477044.\n\nThe relationship of Experiment to Run is a 1-to-many relationship, or there can be many Run accessions\nassociated with a single Experiment Accession (e.g. re-sequencing the same sample). Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-experiment` to merge multiple runs\nassociated with an Experiment accession into a single FASTQ file.\n\n#### Download FASTQs associated with an Sample\n\nOk, this time you just want a single Sample, or Biosample.\n\n```{bash}\nfastq-dl --accession SRS1904245 --provider SRA\n```\n\nThe above command would download the Run accessions from SRA that fall under Sample SRS1904245.\n\nSimilar to Experiment accessions, the relationship of Sample to Run is a 1-to-many relationship,\nor there can be many Run accessions associated with a single Sample Accession. Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-sample` to merge multiple runs\nassociated with an Sample accession into a single FASTQ file.\n\n_Warning! For some type strains (e.g. S. aureus USA300) a Biosample accession might be associated with\n100s or 1000s of Run accessions. These Runs are likely associated with many different conditions and\nreally should not fall under a single BioSample accession. Please consider this when using\n`--group-by-sample`.\n\n#### Download FASTQs associated with a Run\n\nLet's keep it super simple and just download a Run.\n\n```\nfastq-dl --accession SRR1178105 --provider SRA\n```\n\nThe above command would download the Run SRR1178105 from SRA. Run accessions are the end of the\nline (1-to-1 relationship), so you will always get the expected Run.\n\n## Alternatives\n`fastq-dl`, is a spin-off of [ena-dl](https://github.com/rpetit3/ena-dl), that has been developed for\nusage with [Bactopia](https://github.com/bactopia/bactopia). With this in mind, EBI/NCBI and provide\ntheir own tools ([enaBrowserTools](https://github.com/enasequence/enaBrowserTools) and\n[SRA Toolkit](https://github.com/ncbi/sra-tools)) that offer more extensive access to their databases.\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rpetit3/fastq-dl',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastq_dl-2.0.2/PKG-INFO` & `fastq_dl-2.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,11 @@
-Metadata-Version: 2.1
-Name: fastq-dl
-Version: 2.0.2
-Summary: Download FASTQ files from SRA or ENA repositories.
-Home-page: https://github.com/rpetit3/fastq-dl
-License: MIT
-Keywords: bioinformatics,fastq,download,SRA,ENA
-Author: Robert A. Petit III
-Author-email: robbie.petit@gmail.com
-Requires-Python: >=3.7.1,<4.0.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: executor (>=23.2,<24.0)
-Requires-Dist: markdown-it-py (==2.2.0)
-Requires-Dist: pysradb (>=1.4,<2.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
-Requires-Dist: rich-click (>=1.6.1,<2.0.0)
-Project-URL: Repository, https://github.com/rpetit3/fastq-dl
-Description-Content-Type: text/markdown
-
-[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/bactopia/rpetit3/fastq-dl)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/rpetit3/fastq-dl/releases)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/rpetit3/fastq-dl)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8051230.svg)](https://doi.org/10.5281/zenodo.8051230)
 
 # fastq-dl
 
 Download FASTQ files from the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) or the
 [Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) repositories.
 
 ## Introduction
@@ -51,41 +27,47 @@
 conda activate fastq-dl 
 ```
 
 ## Usage
 
 ```{bash}
 fastq-dl --help
-                                                                                          
- Usage: fastq-dl [OPTIONS]                                                                
-                                                                                          
- Download FASTQ files from ENA or SRA.                                                    
-                                                                                          
-╭─ Required Options ─────────────────────────────────────────────────────────────────────╮
-│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run  │
-│                           accession) [required]                                        │
-╰────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Additional Options ───────────────────────────────────────────────────────────────────╮
-│ --provider                 [ena|sra]  Specify which provider (ENA or SRA) to use.      │
-│                                       [default: ena]                                   │
-│ --group-by-experiment                 Group Runs by experiment accession.              │
-│ --group-by-sample                     Group Runs by sample accession.                  │
-│ --outdir               -o  TEXT       Directory to output downloads to. [default: ./]  │
-│ --prefix                   TEXT       Prefix to use for naming log files.              │
-│                                       [default: fastq]                                 │
-│ --cpus                     INTEGER    Total cpus used for downloading from SRA.        │
-│                                       [default: 1]                                     │
-│ --max-attempts         -m  INTEGER    Maximum number of download attempts.             │
-│                                       [default: 10]                                    │
-│ --only-provider        -F             Only attempt download from specified provider.   │
-│ --silent                              Only critical errors will be printed.            │
-│ --version              -V             Show the version and exit.                       │
-│ --verbose              -v             Print debug related text.                        │
-│ --help                 -h             Show this message and exit.                      │
-╰────────────────────────────────────────────────────────────────────────────────────────╯
+
+ Usage: fastq-dl [OPTIONS]                                                                        
+                                                                                                  
+ Download FASTQ files from ENA or SRA.                                                            
+                                                                                                  
+╭─ Required Options ─────────────────────────────────────────────────────────────────────────────╮
+│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run          │
+│                           accession)                                                           │
+│                           [required]                                                           │
+╰────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Additional Options ───────────────────────────────────────────────────────────────────────────╮
+│ --provider                    [ena|sra]  Specify which provider (ENA or SRA) to use.           │
+│                                          [default: ena]                                        │
+│ --group-by-experiment                    Group Runs by experiment accession.                   │
+│ --group-by-sample                        Group Runs by sample accession.                       │
+│ --outdir                  -o  TEXT       Directory to output downloads to. [default: ./]       │
+│ --prefix                      TEXT       Prefix to use for naming log files. [default: fastq]  │
+│ --cpus                        INTEGER    Total cpus used for downloading from SRA.             │
+│                                          [default: 1]                                          │
+│ --max-attempts            -m  INTEGER    Maximum number of download attempts. [default: 10]    │
+│ --force                                  Overwrite existing files if their MD5 checksums do    │
+│                                          not match.                                            │
+│ --sra-lite                               Set preference to SRA Lite                            │
+│ --only-provider                          Only attempt download from specified provider.        │
+│ --only-download-metadata                 Skip FASTQ downloads, and retrieve only the metadata. │
+│ --silent                                 Only critical errors will be printed.                 │
+│ --sleep                   -s  INTEGER    Minimum amount of time to sleep between retries (API  │
+│                                          query and download)                                   │
+│                                          [default: 10]                                         │
+│ --version                 -V             Show the version and exit.                            │
+│ --verbose                 -v             Print debug related text.                             │
+│ --help                    -h             Show this message and exit.                           │
+╰────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 *fastq-dl* requires a single ENA/SRA Study, Sample, Experiment, or Run accession and FASTQs
 for all Runs that fall under the given accession will be downloaded. For example, if a Study
 accession is given all Runs under that studies umbrella will be downloaded. By default, 
 `fastq-dl` will try to download from ENA first, then SRA.
 
@@ -123,14 +105,22 @@
 
 ### --group-by-experiment & --group-by-sample
 
 There maybe times you might want to group Run accessions based on a Experiment or Sample
 accessions. This will merge FASTQs associated with a Run accession based its associated
 Experiment accession (`--group-by-experiment`) or Sample accession (`--group-by-sample`).
 
+### --sra-lite
+
+Downloads from SRA are provided in [SRA Normalized and SRA Lite](https://www.ncbi.nlm.nih.gov/sra/docs/sra-data-formats/) formats.
+SRA Normalized is the original format with full base quality scores and SRA Lite are smaller
+due to simplifying the quality scores to a uniform Q30. By default the preference will be
+set to SRA Normalized, if you prefer SRA Lite you can use `--sra-lite` to set the
+preference to SRA Lite.
+
 ## Output Files
 
 | Extension          | Description                                                                              |
 |--------------------|------------------------------------------------------------------------------------------|
 | `-run-info.tsv`    | Tab-delimited file containing metadata for each Run downloaded                           |
 | `-run-mergers.tsv` | Tab-delimited file merge information from `--group-by-experiment` or `--group-by-sample` |
 | `.fastq.gz`        | FASTQ files downloaded from ENA or SRA                                                   |
@@ -199,8 +189,7 @@
 line (1-to-1 relationship), so you will always get the expected Run.
 
 ## Alternatives
 `fastq-dl`, is a spin-off of [ena-dl](https://github.com/rpetit3/ena-dl), that has been developed for
 usage with [Bactopia](https://github.com/bactopia/bactopia). With this in mind, EBI/NCBI and provide
 their own tools ([enaBrowserTools](https://github.com/enasequence/enaBrowserTools) and
 [SRA Toolkit](https://github.com/ncbi/sra-tools)) that offer more extensive access to their databases.
-
```

