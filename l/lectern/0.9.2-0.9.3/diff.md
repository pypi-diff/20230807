# Comparing `tmp/lectern-0.9.2.tar.gz` & `tmp/lectern-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lectern-0.9.2.tar", last modified: Sat Mar 27 11:50:19 2021, max compression
+gzip compressed data, was "lectern-0.9.3.tar", last modified: Fri Apr  2 12:09:17 2021, max compression
```

## Comparing `lectern-0.9.2.tar` & `lectern-0.9.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1073 2021-03-27 11:49:17.933461 lectern-0.9.2/LICENSE
--rw-r--r--   0        0        0    24213 2021-03-27 11:49:17.933461 lectern-0.9.2/README.md
--rw-r--r--   0        0        0      190 2021-03-27 11:50:15.729908 lectern-0.9.2/lectern/__init__.py
--rw-r--r--   0        0        0       37 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/__main__.py
--rw-r--r--   0        0        0     2534 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/cli.py
--rw-r--r--   0        0        0     6810 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/directive.py
--rw-r--r--   0        0        0     5281 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/document.py
--rw-r--r--   0        0        0    17672 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/extract.py
--rw-r--r--   0        0        0     3038 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/fragment.py
--rw-r--r--   0        0        0     1461 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/plugin.py
--rw-r--r--   0        0        0     2956 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/prefetch.py
--rw-r--r--   0        0        0        0 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/py.typed
--rw-r--r--   0        0        0     2180 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/pytest_plugin.py
--rw-r--r--   0        0        0     9400 2021-03-27 11:49:17.937461 lectern-0.9.2/lectern/serialize.py
--rw-r--r--   0        0        0     1445 2021-03-27 11:50:15.741908 lectern-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    25779 2021-03-27 11:50:19.308673 lectern-0.9.2/setup.py
--rw-r--r--   0        0        0    25054 2021-03-27 11:50:19.311001 lectern-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-04-02 12:08:25.440231 lectern-0.9.3/LICENSE
+-rw-r--r--   0        0        0    24213 2021-04-02 12:08:25.440231 lectern-0.9.3/README.md
+-rw-r--r--   0        0        0      190 2021-04-02 12:09:13.568572 lectern-0.9.3/lectern/__init__.py
+-rw-r--r--   0        0        0       37 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/__main__.py
+-rw-r--r--   0        0        0     2534 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/cli.py
+-rw-r--r--   0        0        0     6810 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/directive.py
+-rw-r--r--   0        0        0     5281 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/document.py
+-rw-r--r--   0        0        0    17672 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/extract.py
+-rw-r--r--   0        0        0     3038 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/fragment.py
+-rw-r--r--   0        0        0     1461 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/plugin.py
+-rw-r--r--   0        0        0     2956 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/prefetch.py
+-rw-r--r--   0        0        0        0 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/py.typed
+-rw-r--r--   0        0        0     2180 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/pytest_plugin.py
+-rw-r--r--   0        0        0     9400 2021-04-02 12:08:25.444232 lectern-0.9.3/lectern/serialize.py
+-rw-r--r--   0        0        0     1446 2021-04-02 12:09:13.576572 lectern-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    25771 2021-04-02 12:09:18.022228 lectern-0.9.3/setup.py
+-rw-r--r--   0        0        0    25046 2021-04-02 12:09:18.023928 lectern-0.9.3/PKG-INFO
```

### Comparing `lectern-0.9.2/LICENSE` & `lectern-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/README.md` & `lectern-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/cli.py` & `lectern-0.9.3/lectern/cli.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/directive.py` & `lectern-0.9.3/lectern/directive.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/document.py` & `lectern-0.9.3/lectern/document.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/extract.py` & `lectern-0.9.3/lectern/extract.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/fragment.py` & `lectern-0.9.3/lectern/fragment.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/plugin.py` & `lectern-0.9.3/lectern/plugin.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/prefetch.py` & `lectern-0.9.3/lectern/prefetch.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/pytest_plugin.py` & `lectern-0.9.3/lectern/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/lectern/serialize.py` & `lectern-0.9.3/lectern/serialize.py`

 * *Files identical despite different names*

### Comparing `lectern-0.9.2/pyproject.toml` & `lectern-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lectern"
-version = "0.9.2"
+version = "0.9.3"
 description = "Literate Minecraft data packs and resource packs."
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/lectern"
 repository = "https://github.com/mcbeet/lectern"
 documentation = "https://github.com/mcbeet/lectern"
@@ -21,24 +21,24 @@
 
 classifiers = ["Framework :: Pytest"]
 
 include = ["lectern/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-beet = "^0.18.0"
+beet = ">=0.19.1"
 markdown-it-py = "^0.6.2"
 click = "^7.1.2"
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 rope = "^0.18.0"
 pytest = "^6.2.2"
 isort = "^5.8.0"
-python-semantic-release = "^7.15.0"
+python-semantic-release = "^7.15.1"
 pytest-insta = "^0.1.6"
 
 [tool.poetry.scripts]
 lectern = "lectern.cli:main"
 
 [tool.poetry.plugins.pytest11]
 lectern = "lectern.pytest_plugin"
```

### Comparing `lectern-0.9.2/setup.py` & `lectern-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['lectern']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beet>=0.18.0,<0.19.0', 'click>=7.1.2,<8.0.0', 'markdown-it-py>=0.6.2,<0.7.0']
+['beet>=0.19.1', 'click>=7.1.2,<8.0.0', 'markdown-it-py>=0.6.2,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['lectern = lectern.cli:main'],
  'pytest11': ['lectern = lectern.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'lectern',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Literate Minecraft data packs and resource packs.',
     'long_description': '<img align="right" src="https://raw.githubusercontent.com/mcbeet/lectern/main/logo.png?sanitize=true" alt="logo" width="52">\n\n# Lectern\n\n[![GitHub Actions](https://github.com/mcbeet/lectern/workflows/CI/badge.svg)](https://github.com/mcbeet/lectern/actions)\n[![PyPI](https://img.shields.io/pypi/v/lectern.svg)](https://pypi.org/project/lectern/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lectern.svg)](https://pypi.org/project/lectern/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n> Literate Minecraft data packs and resource packs.\n\n`@function tutorial:greeting`\n\n```mcfunction\nsay Hello, world!\n```\n\n## Introduction\n\nThis markdown file is interspersed with code fragments describing the content of a Minecraft data pack. Using `lectern`, you can turn this single file into an actual data pack that can be loaded into the game.\n\n**Features**\n\n- Turn markdown files into data packs and resource packs\n- Merge resources from several markdown files\n- Convert data packs and resource packs into markdown snapshots\n- Can be used as a [`beet`](https://github.com/mcbeet/beet) plugin\n- Highly extensible with custom directives\n- Automatically integrates with [`pytest-insta`](https://github.com/vberlier/pytest-insta)\n\n**Hmmkay but why?**\n\n- Editing data packs involves a lot of jumping around between files, for simple use-cases a single file is a lot easier to work with\n- Minecraft packs aggregate various types of files that can have complex interactions with each other, a literate style allows you to document these interactions fluently\n- Human-readable, single-file data pack and resource pack snapshots can be really useful to diff and track regressions in Minecraft-related tooling\n\n## Installation\n\nThe package can be installed with `pip`.\n\n```bash\n$ pip install lectern\n```\n\n## Getting started\n\nThis is an example of a markdown file that can be turned into a data pack:\n\n    # Beginner tutorial\n\n    Let\'s start by creating a simple function:\n\n    `@function tutorial:greeting`\n\n    ```mcfunction\n    say Hello, world!\n    ```\n\n    And now we can make it run when the data pack is loaded!\n\n    `@function_tag minecraft:load`\n\n    ```json\n    {\n      "values": ["tutorial:greeting"]\n    }\n    ```\n\nYou can use the `lectern` command-line utility to turn the markdown file into a data pack.\n\n```bash\n$ lectern tutorial.md --data-pack path/to/tutorial_data_pack\n```\n\nIf you\'re using [`beet`](https://github.com/mcbeet/beet) you can use `lectern` as a plugin in your pipeline.\n\n```json\n{\n  "pipeline": ["lectern"],\n  "meta": {\n    "lectern": {\n      "load": ["*.md"]\n    }\n  }\n}\n```\n\n## Document formats\n\n`lectern` implements two closely-related document formats: markdown and plain text. The markdown format builds upon the plain text format.\n\nThe markdown format lets you present the various elements of your data pack or resource pack and how they fit together. It\'s a format that\'s meant to support [literate programming](https://en.wikipedia.org/wiki/Literate_programming). You can use it when your document is meant to be read by other people. It allows you to emphasize the important parts, explain tradeoffs and discuss alternatives, implementation details, etc...\n\n    `@function tutorial:greeting`\n\n    ```mcfunction\n    say Hello, world!\n    ```\n\nOn the other hand if you don\'t intend to produce literate documents you can use the plain text format to author data packs and resource packs as a single file without having to deal with markdown formatting.\n\n```\n@function tutorial:greeting\nsay Hello, world!\n```\n\n## Directives\n\nData pack and resource pack fragments are code blocks, links or images annotated with a special `lectern` directive. Directives are prefixed with the `@` symbol and can be followed by zero or more arguments.\n\n```\n@<directive_name> <arg1> <arg2> <arg3>...\n```\n\n`lectern` provides directives for including namespaced resources inside data packs and resource packs. These built-in directives all expect a single argument specifying the fully-qualified resource name.\n\n```\n@function tutorial:greeting\n@function_tag minecraft:load\n```\n\nHere is a reference of all the supported resources:\n\n| Data pack                       | Resource pack      |\n| ------------------------------- | ------------------ |\n| `@advancement`                  | `@blockstate`      |\n| `@function`                     | `@model`           |\n| `@loot_table`                   | `@language`        |\n| `@predicate`                    | `@font`            |\n| `@recipe`                       | `@glyph_sizes`     |\n| `@structure`                    | `@truetype_font`   |\n| `@block_tag`                    | `@shader_post`     |\n| `@entity_type_tag`              | `@shader`          |\n| `@fluid_tag`                    | `@fragment_shader` |\n| `@function_tag`                 | `@vertex_shader`   |\n| `@item_tag`                     | `@glsl_shader`     |\n| `@dimension_type`               | `@text`            |\n| `@dimension`                    | `@texture_mcmeta`  |\n| `@biome`                        | `@texture`         |\n| `@configured_carver`            |                    |\n| `@configured_feature`           |                    |\n| `@configured_structure_feature` |                    |\n| `@configured_surface_builder`   |                    |\n| `@noise_settings`               |                    |\n| `@processor_list`               |                    |\n| `@template_pool`                |                    |\n| `@item_modifier`                |                    |\n\nThere are also two built-in directives that can be used to include files using a path relative to the root of the data pack or the resource pack.\n\n```\n@data_pack pack.mcmeta\n@resource_pack pack.png\n@resource_pack assets/minecraft/textures/block/kelp_plant.png.mcmeta\n```\n\nThis is useful for adding files that aren\'t part of any particular namespace.\n\nIf you\'re using `lectern` as a `beet` plugin you will be able to require plugins dynamically wih the `@require` directive.\n\n```\n@require my_plugins.hello\n```\n\nFinally, the `@skip` directive is simply ignored and allows you to end a previous fragment in the plain text format.\n\n```\n@function tutorial:greeting\nsay Hello, world!\n\n@skip\nThis will not be included in the output.\n```\n\n## Code block fragments\n\nYou can include the content of a code block in a data pack or a resource pack by preceding it with a directive surrounded by backticks.\n\n`@function tutorial:greeting`\n\n```mcfunction\nsay Hello, world!\n```\n\nYou can put the directive in an html comment to make it invisible. Here the code block is annotated with the following comment:\n\n```html\n<!-- @function_tag minecraft:load -->\n```\n\n<!-- @function_tag minecraft:load -->\n\n```json\n{\n  "values": ["tutorial:greeting"]\n}\n```\n\nWhen using backticks you can surround the code block in a `<details>` element to make the code fragment foldable.\n\n`@function tutorial:greeting`\n\n<details>\n\n```mcfunction\nsay Hello, world!\n```\n\n</details>\n\nThe directive can also be embedded directly inside the code block. You can insert a directive preceded by either `#` or `//` and the following lines will be included in the specified file.\n\n```mcfunction\n# @function tutorial:obtained_dead_bush\nsay You obtained a dead bush!\n```\n\nEmbedded directives are stripped from the output. You can use multiple directives in a single code block.\n\n```json\n// @loot_table minecraft:blocks/diamond_ore\n{\n  "pools": [\n    {\n      "rolls": 1,\n      "entries": [\n        {\n          "type": "minecraft:item",\n          "name": "minecraft:dead_bush"\n        }\n      ]\n    }\n  ]\n}\n\n// @advancement tutorial:obtained_dead_bush\n{\n  "criteria": {\n    "dead_bush": {\n      "trigger": "minecraft:inventory_changed",\n      "conditions": {\n        "items": [\n          {\n            "item": "minecraft:dead_bush"\n          }\n        ]\n      }\n    }\n  },\n  "requirements": [\n    [\n      "dead_bush"\n    ]\n  ],\n  "rewards": {\n    "function": "tutorial:obtained_dead_bush"\n  }\n}\n```\n\n## Link fragments\n\nLink fragments make it possible to refer to external files, online assets, and to embed binary files in the markdown as data urls. You can create a link fragment by turning a directive surrounded by backticks into a markdown link.\n\n[`@loot_table minecraft:blocks/yellow_shulker_box`](examples/with_links/yellow_shulker_box.json)\n\nThe link itself can be a path to a local file or any url supported by the built-in [`urlopen`](https://docs.python.org/3/library/urllib.request.html#urllib.request.urlopen) function.\n\n## Image fragments\n\nYou can include inline markdown images in the output data pack or resource pack by preceding the image with a directive surrounded by backticks.\n\n`@data_pack pack.png`\n\n![](https://static.wikia.nocookie.net/minecraft_gamepedia/images/3/3a/Pack.png/revision/latest?cb=20210210114950)\n\nImage fragments support the same variations as code block fragments. You can put the directive in a comment or surround the image with a `<details>` element to make it foldable.\n\n## Hidden fragments\n\nYou can use html comments to add fragments that will be completely hidden in the rendered markdown.\n\n```html\n<!--\n@function tutorial:hidden\nsay This will not appear in the rendered markdown.\n\n@function tutorial:also_hidden\nsay This is also hidden.\n-->\n```\n\n<!--\n@function tutorial:hidden\nsay This will not appear in the rendered markdown.\n\n@function tutorial:also_hidden\nsay This is also hidden.\n-->\n\n## Modifiers\n\nThe behavior of particular directives can be adjusted with modifiers. A modifier is specified between parentheses right after the name of the directive.\n\n```\n@<directive_name>(<modifier>) <arg1> <arg2> <arg3>...\n```\n\nThe `append` modifier is implemented by all the text-based built-in namespaced resource directives and makes it possible to concatenate the content of the fragment to the already-existing content.\n\n`@function(append) tutorial:greeting`\n\n```mcfunction\nsay This is added afterwards.\n```\n\nThe `merge` modifier is similar but instead of concatenating the contents it uses the `beet` merging strategy to combine the fragment with the existing file.\n\n`@function_tag(merge) minecraft:load`\n\n```json\n{\n  "values": ["#tutorial:something_else"]\n}\n```\n\nThere are also modifiers that are applied to the content of the fragment directly. The `base64` modifier will decode the content of the code fragment as [base64](https://en.wikipedia.org/wiki/Base64).\n\n`@function_tag(base64) tutorial:something_else`\n\n```json\newogICJ2YWx1ZXMiOiBbInR1dG9yaWFsOnN0cmlwcGVkIl0KfQ==\n```\n\nFinally, there\'s a `strip_final_newline` modifier that removes the final newline at the end of code block fragments. It\'s mostly used to make sure that `lectern` snapshots can reconstruct the original content byte for byte in case the file wasn\'t terminated by a newline.\n\n`@function(strip_final_newline) tutorial:stripped`\n\n```mcfunction\nsay This function doesn\'t have a final newline.\n```\n\n## Command-line utility\n\n```bash\n$ lectern --help\nUsage: lectern [OPTIONS] [PATH]...\n\n  Literate Minecraft data packs and resource packs.\n\nOptions:\n  -d, --data-pack <path>       Extract data pack.\n  -r, --resource-pack <path>   Extract resource pack.\n  -e, --external-files <path>  Emit external files.\n  -p, --prefetch-urls <path>   Prefetch markdown links.\n  -v, --version                Show the version and exit.\n  -h, --help                   Show this message and exit.\n```\n\nYou can extract data packs from markdown files with the `-d/--data-pack` option. If the name ends with `.zip` the generated data pack will be zipped. Multiple markdown files can be merged together into a single data pack.\n\n```bash\n$ lectern demo.md --data-pack demo_data_pack\n$ lectern demo.md -d demo_data_pack\n$ lectern demo.md -d demo_data_pack.zip\n$ lectern foo.md bar.md -d demo_data_pack\n```\n\nThe `-r/--resource-pack` option lets you do exactly the same thing but with resource packs. The two options can be combined to extract a data packs and a resource pack at the same time.\n\n```bash\n$ lectern demo.md --resource-pack demo_resource_pack\n$ lectern demo.md -r demo_resource_pack\n$ lectern demo.md -d demo_data_pack -r demo_resource_pack\n```\n\nYou can also convert a combination of data packs and resource packs into a single markdown file.\n\n```bash\n$ lectern demo_data_pack demo.md\n$ lectern demo_data_pack.zip demo.md\n$ lectern demo_data_pack demo_resource_pack demo.md\n$ lectern foo_data_pack bar_data_pack demo.md\n```\n\nThe last argument is the name of the generated markdown file. By default, the `lectern` utility will bundle binary files into the markdown file as data urls. You can use the `-e/--external-files` option to dump the binary files in a given directory instead.\n\n```bash\n$ lectern demo_data_pack demo.md --external-files files\n$ lectern demo_data_pack demo.md -e files\n$ lectern demo_data_pack demo.md -e .\n```\n\nAll these commands also work with plain text files. `lectern` will only use the markdown document format when the filename ends with `.md`.\n\nFinally, you can also use the command-line utility to prefetch markdown urls. The `-p/--prefetch-urls` option can replace the urls in-place or in a copy.\n\n```bash\n$ lectern --prefetch-urls demo.md\n$ lectern --prefetch-urls demo.md demo_prefetched.md\n$ lectern -p demo.md demo_prefetched.md\n$ lectern -p demo.md\n```\n\nBy default, the remote files will be bundled as data urls but you can use the `-e/--external-files` option to dump everything in a given directory.\n\n```bash\n$ lectern --prefetch-urls demo.md --external-files files\n$ lectern --prefetch-urls demo.md demo_prefetched.md --external-files files\n$ lectern -p demo.md demo_prefetched.md -e files\n$ lectern -p demo.md -e .\n```\n\n## Python API\n\nThe API revolves around `Document` objects. A `lectern` document holds a `DataPack` and a `ResourcePack`, as well as a dictionary defining the usable directives. The extractors and serializers are also exposed on the document to make it possible to swap them out with custom ones if needed.\n\n```python\nfrom beet import DataPack, ResourcePack\nfrom lectern import Document\n\ndocument = Document()\nassert document.data == DataPack()\nassert document.assets == ResourcePack()\n```\n\nThe constructor makes it possible to provide existing `DataPack` and `ResourcePack` instances, some initial text or markdown content, or a path from which to load an existing `lectern` document.\n\n```python\nDocument(data=DataPack(), assets=ResourcePack())\nDocument(text=...)\nDocument(markdown=...)\nDocument(path="path/to/document.md")\n```\n\n`Document` instances will compare equal if the underlying data packs and resource packs also compare equal.\n\nYou can use the `load` method to read a markdown or a plain text file and update the internal data pack and resource pack with the extracted fragments.\n\n```python\ndocument.load("path/to/document.md")\n```\n\nIf you already have some text or markdown ready to go, you can use the `add_text` and `add_markdown` methods.\n\n```python\ndocument.add_text(...)\ndocument.add_markdown(...)\n```\n\nIf the markdown content refers to local files you can specify the directory from which the external files should be loaded from with the `external_files` argument.\n\n```python\ndocument.add_markdown(..., external_files="path/to/directory")\n```\n\nYou can use the `get_text` and `get_markdown` methods to serialize the entire content of the internal data pack and resource pack. By default the `get_markdown` method will produce markdown that embeds binary files as data urls. You can enable `emit_external_files` and optionally provide a path prefix to generate a dictionary of associated files instead.\n\n```python\ntext = document.get_text()\nmarkdown = document.get_markdown()\nmarkdown, external_files = document.get_markdown(emit_external_files=True)\nmarkdown, external_files = document.get_markdown(emit_external_files=True, prefix="path/to/directory")\n```\n\nFinally, the `save` method lets you serialize and write the document to a given path. If the filename ends with `.md` the generated markdown will bundle binary files as data urls by default. You can use the `external_files` argument to emit the binary files in the given directory instead.\n\n```python\ndocument.save("path/to/document.txt")\ndocument.save("path/to/document.md")\ndocument.save("path/to/document.md", external_files="path/to/files")\n```\n\n## Custom directives\n\nDirectives are simply callable objects that receive the document fragment, the resource pack, and the data pack as arguments.\n\n```python\nfrom beet import DataPack, ResourcePack, Function\nfrom lectern import Document, Fragment\n\ndef my_directive(fragment: Fragment, assets: ResourcePack, data: DataPack):\n    num1, num2 = fragment.expect("num1", "num2")\n    result = int(num1) + int(num2)\n    data["demo:output_result"] = Function([f"say {result}"])\n\ndocument = Document()\ndocument.directives["my_directive"] = my_directive\ndocument.add_text("@my_directive 32 10")\nassert document.data.functions["demo:output_result"] == Function(["say 42"])\n```\n\nThe `expect` method allows you to unpack the directive arguments and automatically raises an error if the user didn\'t specify the arguments properly. You can use the `as_file` method to get the content of the fragment as a specific type of file.\n\n```python\ndef repeated_function(fragment: Fragment, assets: ResourcePack, data: DataPack):\n    full_name, count = fragment.expect("full_name", "count")\n    function = fragment.as_file(Function)\n    function.lines *= int(count)\n    data[full_name] = function\n```\n\nThe `as_file` method will take care of reading the file or downloading it if the directive is used with a link fragment. It will also handle the `base64` and `strip_final_newline` modifiers.\n\nYou can handle custom modifiers by checking the content of the `modifier` attribute.\n\n## Beet plugin\n\nUsing `lectern` as a `beet` plugin makes it possible to combine your markdown files with arbitrary `beet` plugins for further processing. The plugin can load files using the plain text and markdown document formats and emit a snapshot of the `beet` context at the end of the build.\n\n```json\n{\n  "pipeline": ["lectern"],\n  "meta": {\n    "lectern": {\n      "load": ["*.md"],\n      "snapshot": "out/snapshot.md",\n      "external_files": "out"\n    }\n  }\n}\n```\n\nYou can require the plugin programmatically by using the `lectern` plugin factory.\n\n```python\nfrom beet import Context\nfrom lectern import lectern\n\ndef my_plugin(ctx: Context):\n    ctx.require(\n        lectern(\n            load=["*.md"],\n            snapshot="out/snapshot.md",\n            external_files="out",\n        )\n    )\n```\n\nAll the configuration is optional. The plugin is a no-op if the `load` or `snapshot` options are not specified.\n\nYou can retrieve the `Document` instance with the `inject` method. This is useful for adding custom directives.\n\n```python\nfrom beet import Context, DataPack, ResourcePack, Function\nfrom lectern import Document, Fragment\n\ndef hello_directive(ctx: Context):\n    """Plugin that defines the `@hello <name>` directive."""\n    document = ctx.inject(Document)\n    document.directives["hello"] = hello\n\ndef hello(fragment: Fragment, assets: ResourcePack, data: DataPack):\n    name = fragment.expect("name")\n    function = data.functions.setdefault("hello:greetings", Function([]))\n    function.lines.append(f"say Hello, {name}!")\n```\n\nIt\'s worth mentioning that `lectern` uses the `beet` cache to avoid downloading link fragments repeatedly and keeping your build snappy, especially in watch mode. If you need to re-download link fragments you can clear the `lectern` cache.\n\n```bash\n$ beet cache --clear lectern\n```\n\nYou can also use a plugin to configure a custom cache timeout if you want to make sure that your assets are re-downloaded periodically.\n\n```python\nfrom beet import Context\n\ndef download_every_day(ctx: Context):\n    ctx.cache["lectern"].timeout(hours=24)\n```\n\n## Lectern scripts\n\nThe text format is pretty well-suited for writing basic data pack and resource pack generators. You can very easily write scripts that produce lectern syntax that can then be turned into a data pack or a resource pack.\n\n```python\n# my_script.py\nprint("@function tutorial:count")\n\nfor i in range(10):\n    print(f"say {i}")\n```\n\n```bash\n$ python my_script.py > output.txt\n$ lectern output.txt -d my_data_pack\n```\n\nThe `beet` plugin supports this use-case natively and allows you to run lectern scripts within your pipeline.\n\n```json\n// beet.json\n{\n  "pipeline": ["lectern"],\n  "meta": {\n    "lectern": {\n      "scripts": [["python", "my_script.py"]]\n    }\n  }\n}\n```\n\nThe `scripts` option lets you specify the command-line arguments for your scripts. The scripts don\'t even have to be written in Python. As long as the command prints out valid `lectern` syntax you can use any language you want.\n\n## Snapshot testing\n\nA lot of Minecraft tooling involves generating data packs and resource packs. Writing tests for this kind of tooling takes time because you need to painstakingly compare everything that you care about with a reference value. This makes it hard to get good coverage, and then even harder to keep making changes to the code being tested afterwards. You\'re trading robustness and stability for a shackle that massively slows down development.\n\nThat\'s where snapshot testing comes into play. Snapshot testing allows you to record a reference value and then make sure that your code keeps producing the same results. It provides the necessary tools for reviewing snapshots and updating them as your project evolves.\n\n`lectern` documents are useful as snapshot formats because they represent entire data packs and resource packs in a single file that\'s human-readable and diff-friendly.\n\n[`pytest-insta`](https://github.com/vberlier/pytest-insta) is an extensible snapshot testing plugin for [`pytest`](https://docs.pytest.org/en/stable/). When it\'s installed, `lectern` defines three additional snapshot formats.\n\n| Extension                 | Format description                                               |\n| ------------------------- | ---------------------------------------------------------------- |\n| `.pack.txt`               | Plain text snapshot.                                             |\n| `.pack.md`                | Markdown snapshot with bundled binary files.                     |\n| `.pack.md_external_files` | Directory with a README.md that refers to external binary files. |\n\nYou can use these snapshot formats when comparing `Document` objects with the `snapshot` fixture.\n\n```python\ndef test_generate(snapshot):\n    data = generate_some_data_pack()\n    assert snapshot("pack.txt") == Document(data=data)\n```\n\nIf you\'re using the `beet` toolchain, keep in mind that you can get a `Document` instance bound to the context object by using the `inject` method.\n\n```python\ndef test_generate_with_beet(snapshot):\n    ctx = run_beet(...)\n    assert snapshot("pack.txt") == ctx.inject(Document)\n```\n\nThis will save the entire data pack and resource pack in the snapshot. For more details about working with the generated snapshots check out the [`pytest-insta` documentation](https://github.com/vberlier/pytest-insta#command-line-options).\n\n## Contributing\n\nContributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org).\n\n```bash\n$ poetry install\n```\n\nYou can run the tests with `poetry run pytest`.\n\n```bash\n$ poetry run pytest\n```\n\nThe project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you\'re using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.\n\n```bash\n$ npm run watch\n$ npm run check\n```\n\nThe code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).\n\n```bash\n$ poetry run isort lectern tests\n$ poetry run black lectern tests\n$ poetry run black --check lectern tests\n```\n\n---\n\nLicense - [MIT](https://github.com/mcbeet/lectern/blob/main/LICENSE)\n',
     'author': 'Valentin Berlier',
     'author_email': 'berlier.v@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mcbeet/lectern',
```

### Comparing `lectern-0.9.2/PKG-INFO` & `lectern-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: lectern
-Version: 0.9.2
+Version: 0.9.3
 Summary: Literate Minecraft data packs and resource packs.
 Home-page: https://github.com/mcbeet/lectern
 License: MIT
 Keywords: literate-programming,beet,resourcepack,minecraft,datapack
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: beet (>=0.18.0,<0.19.0)
+Requires-Dist: beet (>=0.19.1)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: markdown-it-py (>=0.6.2,<0.7.0)
 Project-URL: Documentation, https://github.com/mcbeet/lectern
 Project-URL: Repository, https://github.com/mcbeet/lectern
 Description-Content-Type: text/markdown
 
 <img align="right" src="https://raw.githubusercontent.com/mcbeet/lectern/main/logo.png?sanitize=true" alt="logo" width="52">
```

