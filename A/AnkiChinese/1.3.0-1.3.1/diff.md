# Comparing `tmp/AnkiChinese-1.3.0.tar.gz` & `tmp/AnkiChinese-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnkiChinese-1.3.0.tar", last modified: Mon Aug  7 19:17:32 2023, max compression
+gzip compressed data, was "AnkiChinese-1.3.1.tar", last modified: Mon Aug  7 20:49:40 2023, max compression
```

## Comparing `AnkiChinese-1.3.0.tar` & `AnkiChinese-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.364717 AnkiChinese-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.364717 AnkiChinese-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.384719 AnkiChinese-1.3.0/card_template/
--rw-r--r--   0 runner    (1001) docker     (123) 17321876 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/CNstrokeorder-0.0.4.7.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/back.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/front.html
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/input.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.364717 AnkiChinese-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/src/scrape/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/src/scrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/src/scrape/scrape_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/src/scrape/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.816011 AnkiChinese-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.792011 AnkiChinese-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.796011 AnkiChinese-1.3.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.796011 AnkiChinese-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-08-07 20:49:40.816011 AnkiChinese-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.812011 AnkiChinese-1.3.1/card_template/
+-rw-r--r--   0 runner    (1001) docker     (123) 17321876 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/card_template/CNstrokeorder-0.0.4.7.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/card_template/back.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/card_template/front.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/card_template/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-07 20:49:40.816011 AnkiChinese-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.792011 AnkiChinese-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.816011 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-08-07 20:49:40.000000 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-07 20:49:40.000000 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:49:40.000000 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 20:49:40.000000 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 20:49:40.000000 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 20:49:40.000000 AnkiChinese-1.3.1/src/AnkiChinese.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:40.816011 AnkiChinese-1.3.1/src/scrape/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/src/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/src/scrape/scrape_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-08-07 20:49:30.000000 AnkiChinese-1.3.1/src/scrape/scraper.py
```

### Comparing `AnkiChinese-1.3.0/.github/workflows/python-publish.yml` & `AnkiChinese-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/.gitignore` & `AnkiChinese-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/LICENSE.txt` & `AnkiChinese-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/card_template/CNstrokeorder-0.0.4.7.ttf` & `AnkiChinese-1.3.1/card_template/CNstrokeorder-0.0.4.7.ttf`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/card_template/back.html` & `AnkiChinese-1.3.1/card_template/back.html`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/card_template/styles.css` & `AnkiChinese-1.3.1/card_template/styles.css`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/input.txt` & `AnkiChinese-1.3.1/input.txt`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/setup.cfg` & `AnkiChinese-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/src/AnkiChinese.egg-info/SOURCES.txt` & `AnkiChinese-1.3.1/src/AnkiChinese.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 LICENSE.txt
 README.md
 input.txt
 pyproject.toml
 setup.cfg
+.github/scripts/release.py
 .github/workflows/python-publish.yml
 card_template/CNstrokeorder-0.0.4.7.ttf
 card_template/back.html
 card_template/front.html
 card_template/styles.css
 src/AnkiChinese.egg-info/PKG-INFO
 src/AnkiChinese.egg-info/SOURCES.txt
```

### Comparing `AnkiChinese-1.3.0/src/scrape/scrape_audio.py` & `AnkiChinese-1.3.1/src/scrape/scrape_audio.py`

 * *Files identical despite different names*

### Comparing `AnkiChinese-1.3.0/src/scrape/scraper.py` & `AnkiChinese-1.3.1/src/scrape/scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,19 @@
     page = await context.new_page()
     await page.goto(
         f"https://www.archchinese.com/chinese_english_dictionary.html?find={hanzi}"
     )
     await page.wait_for_function("() => !!document.querySelector('#wordTable')")
     content = await page.content()
     await page.close()
-    return scrape_word(content, num_defs, num_examples, hanzi)
+    try:
+        return scrape_word(content, num_defs, num_examples, hanzi)
+    except Exception as e:
+        print(f"Error scraping {hanzi}: {e}")
+        return None
 
 
 async def main_csv(chars, num_defs, num_examples):
     async with async_playwright() as p:
         browser = await p.chromium.launch()
         context = await browser.new_context()
 
@@ -115,14 +119,16 @@
         async with aiometer.amap(
             functools.partial(fetch, context, num_defs, num_examples),
             chars,
             max_at_once=10,
             max_per_second=5,
         ) as results:
             async for data in results:
+                if data is None:
+                    continue
                 result_list.append(data)
                 pbar.update(1)
         await browser.close()
         pbar.close()
         return result_list
 
 
@@ -170,14 +176,16 @@
         async with aiometer.amap(
             functools.partial(fetch, context, num_defs, num_examples),
             chars,
             max_at_once=10,
             max_per_second=5,
         ) as results:
             async for data in results:
+                if data is None:
+                    continue
                 note = genanki.Note(
                     model=chinese_model,
                     fields=[
                         data["hanzi"],
                         data["definition"],
                         data["pinyin"],
                         data["pinyin2"],
@@ -195,36 +203,36 @@
 
 
 def cli():
     parser = argparse.ArgumentParser(
         description="Scrape ArchChinese for definitions and example words"
     )
     parser.add_argument(
+        "--type",
+        "-t",
+        type=str,
+        choices=["anki", "csv"],
+        default="anki",
+        help="Output file type (default: anki)",
+    )
+    parser.add_argument(
         "--input",
         "-i",
         type=str,
         default="input.txt",
         help="Input file with characters to scrape (default: input.txt)",
     )
     parser.add_argument(
         "--output",
         "-o",
         type=str,
         default="ankchinese_output",
         help="Name of output file (do not include extension) (default: ankichinese_output)",
     )
     parser.add_argument(
-        "--type",
-        "-t",
-        type=str,
-        choices=["anki", "csv"],
-        default="anki",
-        help="Output file type (default: anki)",
-    )
-    parser.add_argument(
         "--defs",
         "-d",
         type=int,
         default=5,
         help="Number of definitions to scrape per character (default: 5)",
     )
     parser.add_argument(
@@ -238,22 +246,23 @@
 
     hanzi_list = []  # unfinished list of characters to scrape
     with open(args.input, encoding="utf8", errors="replace", mode="r") as f:
         for line in f:
             for hanzi in line:
                 if not hanzi.isspace():
                     hanzi_list.append(hanzi)
+    hanzi_list = set(hanzi_list)  # remove duplicates
 
     if args.type == "csv":
-        results = asyncio.run(main_csv(hanzi_list, args.num_defs, args.num_examples))
+        results = asyncio.run(main_csv(hanzi_list, args.defs, args.examples))
 
         df = pd.DataFrame(results)
         df.to_csv(args.output + ".csv", index=False)
     elif args.type == "anki":
-        results = asyncio.run(main_anki(hanzi_list, args.num_defs, args.num_examples))
+        results = asyncio.run(main_anki(hanzi_list, args.defs, args.examples))
 
         package = genanki.Package(results)
         audio_files = os.listdir("ankichinese_audio")
         for file in audio_files:
             package.media_files.append("ankichinese_audio/" + file)
         package.media_files.append("card_template/CNstrokeorder-0.0.4.7.ttf")
         package.write_to_file(args.output + ".apkg")
```

