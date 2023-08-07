# Comparing `tmp/statute_utils-0.6.6.tar.gz` & `tmp/statute_utils-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.6.6.tar", max compression
+gzip compressed data, was "statute_utils-0.6.7.tar", max compression
```

## Comparing `statute_utils-0.6.6.tar` & `statute_utils-0.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.6/LICENSE
--rw-r--r--   0        0        0     2825 2023-07-31 16:21:33.481263 statute_utils-0.6.6/README.md
--rw-r--r--   0        0        0     1461 2023-07-31 17:00:13.670540 statute_utils-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.6/statute_utils/__init__.py
--rw-r--r--   0        0        0     3113 2023-07-30 00:42:26.232929 statute_utils-0.6.6/statute_utils/codification.py
--rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.6/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.6/statute_utils/components/branch.py
--rw-r--r--   0        0        0     9721 2023-07-30 10:35:07.925035 statute_utils-0.6.6/statute_utils/components/builder.py
--rw-r--r--   0        0        0    12717 2023-07-30 01:34:15.178955 statute_utils-0.6.6/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.6/statute_utils/components/short.py
--rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.6/statute_utils/components/utils.py
--rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.6/statute_utils/config.py
--rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.6/statute_utils/main.py
--rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.6/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.6/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.6/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.6/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.6/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.6/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.6/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.6/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6696 2023-07-30 01:34:59.725837 statute_utils-0.6.6/statute_utils/statute.py
--rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.6/statute_utils/templater.py
--rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.6/statute_utils/templates/crumbs.html
--rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.6/statute_utils/templates/paragraph.html
--rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.6/statute_utils/templates/subtree.html
--rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.6/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     3076 2023-07-31 17:02:13.294454 statute_utils-0.6.6/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 statute_utils-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2825 2023-07-31 16:21:33.481263 statute_utils-0.6.7/README.md
+-rw-r--r--   0        0        0     1461 2023-08-07 10:59:21.335892 statute_utils-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.7/statute_utils/__init__.py
+-rw-r--r--   0        0        0     3113 2023-07-30 00:42:26.232929 statute_utils-0.6.7/statute_utils/codification.py
+-rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.7/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.7/statute_utils/components/branch.py
+-rw-r--r--   0        0        0     9721 2023-07-30 10:35:07.925035 statute_utils-0.6.7/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    15560 2023-08-07 10:54:20.469809 statute_utils-0.6.7/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.7/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.7/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.7/statute_utils/config.py
+-rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.7/statute_utils/main.py
+-rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.7/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.7/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.7/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.7/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.7/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.7/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.7/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.7/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     7226 2023-08-07 10:53:38.924015 statute_utils-0.6.7/statute_utils/statute.py
+-rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.7/statute_utils/templater.py
+-rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.7/statute_utils/templates/crumbs.html
+-rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.7/statute_utils/templates/paragraph.html
+-rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.7/statute_utils/templates/subtree.html
+-rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.7/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     3043 2023-07-31 18:24:05.729977 statute_utils-0.6.7/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 statute_utils-0.6.7/PKG-INFO
```

### Comparing `statute_utils-0.6.6/LICENSE` & `statute_utils-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/README.md` & `statute_utils-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/pyproject.toml` & `statute_utils-0.6.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.6.6"
+version = "0.6.7"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.6.6/statute_utils/__init__.py` & `statute_utils-0.6.7/statute_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/codification.py` & `statute_utils-0.6.7/statute_utils/codification.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/components/__init__.py` & `statute_utils-0.6.7/statute_utils/components/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/components/branch.py` & `statute_utils-0.6.7/statute_utils/components/branch.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/components/builder.py` & `statute_utils-0.6.7/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/components/category.py` & `statute_utils-0.6.7/statute_utils/components/category.py`

 * *Files 26% similar despite different names*

```diff
@@ -210,38 +210,116 @@
                     )
 
             case _:
                 # no need to uppercase pure digits
                 target_digit = idx if idx.isdigit() else idx.upper()
                 return f"{uncamel(self)} No. {target_digit}"
 
-    def searchable(self, num: str) -> str:
+    def searchable(self, num: str) -> list[str]:
         """Given the value `<v>` of a category (lowercased, as saved in the database),
         use `StatuteSerialCategory(<v>)`. This will get the proper category. Use the
         category alongside the passed `num`.
 
         Examples:
             >>> civ = StatuteSerialCategory('ra')
             >>> civ.searchable('386')
-            'ra 386'
+            ['ra 386', 'rep act no. 386', 'r.a. no. 386', 'r.a. 386']
             >>> civ = StatuteSerialCategory('rule_am')
             >>> civ.searchable('00-2-03-sc')
-            'am 00-2-03-sc'
-        """
+            ['am 00-2-03-sc', 'a.m. no. 00-2-03-sc', 'a.m. 00-2-03-sc', 'admin matter no. 00-2-03-sc']
+        """  # noqa: E501
         match self:
+            case StatuteSerialCategory.RepublicAct:
+                return [
+                    f"ra {num}",
+                    f"rep act no. {num}",
+                    f"r.a. no. {num}",
+                    f"r.a. {num}",
+                ]
+            case StatuteSerialCategory.CommonwealthAct:
+                return [
+                    f"ca {num}",
+                    f"commonwealth act no. {num}",
+                    f"c.a. no. {num}",
+                    f"c.a. {num}",
+                ]
+            case StatuteSerialCategory.Act:
+                return [
+                    f"act of congress {num}",
+                ]
+            case StatuteSerialCategory.BatasPambansa:
+                return [
+                    f"bp {num}",
+                    f"b.p. no. {num}",
+                    f"b.p. blg. {num}",
+                    f"batas pambansa {num}",
+                    f"batas pambansa blg. {num}",
+                ]
+            case StatuteSerialCategory.ExecutiveOrder:
+                return [
+                    f"eo {num}",
+                    f"e.o. no. {num}",
+                    f"exec order {num}",
+                    f"exec. order no. {num}",
+                ]
+            case StatuteSerialCategory.PresidentialDecree:
+                return [
+                    f"pd {num}",
+                    f"p.d. no. {num}",
+                    f"pres decree {num}",
+                    f"pres. dec. {num}",
+                    f"pres. decree {num}",
+                ]
+            case StatuteSerialCategory.LetterOfInstruction:
+                return [
+                    f"loi {num}",
+                    f"l.o.i. {num}",
+                    f"l.o.i. no. {num}",
+                ]
+            case StatuteSerialCategory.Spain:
+                return [
+                    f"spanish {num}",
+                    f"old {num}",
+                ]
+            case StatuteSerialCategory.RulesOfCourt:
+                return [
+                    f"{num} roc",
+                ]
+            case StatuteSerialCategory.Constitution:
+                return [
+                    f"{num} const",
+                ]
             case StatuteSerialCategory.AdministrativeMatter:
-                return f"am {num}"
+                return [
+                    f"am {num}",
+                    f"a.m. no. {num}",
+                    f"a.m. {num}",
+                    f"admin matter no. {num}",
+                ]
             case StatuteSerialCategory.BarMatter:
-                return f"bm {num}"
+                return [
+                    f"bm {num}",
+                    f"b.m. no. {num}",
+                    f"b.m. {num}",
+                    f"bar matter no. {num}",
+                ]
             case StatuteSerialCategory.CircularOCA:
-                return f"oca cir {num}"
+                return [
+                    f"oca {num}",
+                    f"oca ipi {num}",
+                    f"oca ipi no. {num}",
+                ]
             case StatuteSerialCategory.CircularSC:
-                return f"sc cir {num}"
+                return [
+                    f"sc cir {num}",
+                    f"sc cir. no. {num}",
+                    f"sc cir. no. {num}",
+                ]
             case _:
-                return f"{self.value} {num}"
+                return [f"{self.value} {num}"]
 
     def cite(self, num: str) -> str | None:
         """Given the value `<v>` of a category (lowercased, as saved in the database),
         use `StatuteSerialCategory(<v>)`. This will get the proper category. Use the
         category alongside the passed `num`.
 
         Examples:
```

### Comparing `statute_utils-0.6.6/statute_utils/components/short.py` & `statute_utils-0.6.7/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/components/utils.py` & `statute_utils-0.6.7/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/config.py` & `statute_utils-0.6.7/statute_utils/config.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/main.py` & `statute_utils-0.6.7/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/models.py` & `statute_utils-0.6.7/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/models_names.py` & `statute_utils-0.6.7/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/models_serials.py` & `statute_utils-0.6.7/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/recipes/digits.py` & `statute_utils-0.6.7/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/recipes/spain.py` & `statute_utils-0.6.7/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/statute.py` & `statute_utils-0.6.7/statute_utils/statute.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,30 +51,40 @@
             yield {
                 "id": f"{self.slug}-{counter}",
                 "statute_id": self.slug,
                 "cat": title.category.name.lower(),
                 "text": title.text,
             }
 
+    def prepare_root(self):
+        """Adds material paths to each node in the tree with the root
+        node given special features: it's marked with a material path `id`
+        of `1.` and it's `content` will consist of the titles of the statute.
+        This will make it convenient to search for titles even if the table
+        being searched consists of material paths."""
+        set_node_ids(self.units)
+        titles = ", ".join([row["text"] for row in self.make_title_rows()])
+        root = {"id": "1.", "content": titles, "units": self.units}
+        return [root]
+
     def make_row(self) -> dict:
         """All nodes in the tree are marked by a material path.
 
         The units key is manipulated to add a root node. This is
         useful for repeals and other changes since affecting the root node, affects all nodes.
 
         The root node for every key should be `1.`
 
         A special `html` field exists for the purpose of performance. Since some units
         are overly large, this creates an unstyled html blob that semantically represents
         the tree object. The helper functions that were used to create the tree object
         can be re-used using the same function via filters.
         ```
         """  # noqa: E501
-        set_node_ids(self.units)
-        units = [{"id": "1.", "units": self.units}]
+        units = self.prepare_root()
         return {
             "id": self.slug,
             "cat": self.rule.cat.value,
             "num": self.rule.num,
             "date": self.date,
             "variant": self.variant,
             "units": units,
@@ -177,11 +187,11 @@
             units=data.get("units"),
             titles=list(
                 StatuteTitle.generate(
                     official=official,
                     serial=serial,
                     short=data.get("short"),
                     aliases=data.get("aliases"),
-                    searchables=[category.searchable(num)],
+                    searchables=category.searchable(num),
                 )
             ),
         )
```

### Comparing `statute_utils-0.6.6/statute_utils/templater.py` & `statute_utils-0.6.7/statute_utils/templater.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/templates/tree.css` & `statute_utils-0.6.7/statute_utils/templates/tree.css`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.6/statute_utils/templates/tree.html` & `statute_utils-0.6.7/statute_utils/templates/tree.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 {# BRANCHING #}
 
-{%- macro summarize(unit) -%}
-  {# The label class is added to style the combination of item + caption in styles.css #}
+{# The label class is added to style the heading consisting of an item and a caption #}
+{%- macro create_branch_heading(unit) -%}
   {%- set clean_item = unit.item|default('Container')|string -%}
   {%- if clean_item|is_hidden -%}
     {% if unit.caption -%}
       <a class="label" data-slug="{{unit.id|set_mp_slug}}">
         <strong >{{unit.caption}}</strong>
       </a>
     {%- endif %}
   {%- else -%}
     <a class="label" data-slug="{{unit.id|set_mp_slug}}">
       <strong>{{clean_item}}</strong>
       {% if unit.caption -%}
-        &nbsp;<em>{{unit.caption}}</em>{# Using literal &nbsp; (instead of adding a css style) makes converting from html to text easier. #}
+        &nbsp;<em>{{unit.caption}}</em>
       {%- endif %}
-    </a>
+    </a>{# Using literal &nbsp; (instead of adding a css style) makes converting from html to text easier. #}
   {%- endif -%}
 {%- endmacro -%}
 
 {%- macro create_branch(unit) -%}
-  {{ summarize(unit)}} {# Create the label based on <strong> and <em> tags #}
+  {{ create_branch_heading(unit)}}
   {% if unit.content -%}
     {{unit.content|trim|safe|md_to_html }} {# Needs to be safe since some unit content may have html #}
   {%- endif %}
   {% if unit|is_par -%}
     <a data-slug="{{unit.id|set_mp_slug}}" data-item="{{unit.item}}" class="par-branch"></a>
   {%- endif %}
 {%- endmacro -%}
```

### Comparing `statute_utils-0.6.6/PKG-INFO` & `statute_utils-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.6.6
+Version: 0.6.7
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

