# Comparing `tmp/mdxpy-1.3.1.tar.gz` & `tmp/mdxpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxpy-1.3.1.tar", last modified: Wed Apr 19 16:51:43 2023, max compression
+gzip compressed data, was "mdxpy-1.3.2.tar", last modified: Mon Aug  7 13:57:06 2023, max compression
```

## Comparing `mdxpy-1.3.1.tar` & `mdxpy-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/
--rw-rw-rw-   0        0        0       88 2020-05-07 19:15:45.000000 mdxpy-1.3.1/.gitignore
--rw-rw-rw-   0        0        0     1099 2020-04-25 16:07:06.000000 mdxpy-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     9294 2023-04-19 16:51:43.009164 mdxpy-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/images/
--rw-rw-rw-   0        0        0    65252 2020-05-07 21:01:00.000000 mdxpy-1.3.1/images/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/mdxpy/
--rw-rw-rw-   0        0        0      192 2022-10-09 19:46:22.000000 mdxpy-1.3.1/mdxpy/__init__.py
--rw-rw-rw-   0        0        0    49608 2023-04-19 16:49:06.000000 mdxpy-1.3.1/mdxpy/mdx.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/mdxpy.egg-info/
--rw-rw-rw-   0        0        0     9294 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-01-19 11:32:22.000000 mdxpy-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     8260 2022-10-10 13:17:58.000000 mdxpy-1.3.1/readme.md
--rw-rw-rw-   0        0        0       42 2023-04-19 16:51:43.009164 mdxpy-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-04-19 16:48:52.000000 mdxpy-1.3.1/setup.py
--rw-rw-rw-   0        0        0    47119 2023-04-19 16:48:43.000000 mdxpy-1.3.1/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:57:06.008938 mdxpy-1.3.2/
+-rw-rw-rw-   0        0        0       88 2020-05-07 19:15:45.000000 mdxpy-1.3.2/.gitignore
+-rw-rw-rw-   0        0        0     1099 2020-04-25 16:07:06.000000 mdxpy-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     9294 2023-08-07 13:57:06.008938 mdxpy-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 13:57:05.993311 mdxpy-1.3.2/images/
+-rw-rw-rw-   0        0        0    65252 2020-05-07 21:01:00.000000 mdxpy-1.3.2/images/logo.png
+drwxrwxrwx   0        0        0        0 2023-08-07 13:57:05.993311 mdxpy-1.3.2/mdxpy/
+-rw-rw-rw-   0        0        0      192 2022-10-09 19:46:22.000000 mdxpy-1.3.2/mdxpy/__init__.py
+-rw-rw-rw-   0        0        0    49855 2023-08-07 13:46:55.000000 mdxpy-1.3.2/mdxpy/mdx.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:57:06.008938 mdxpy-1.3.2/mdxpy.egg-info/
+-rw-rw-rw-   0        0        0     9294 2023-08-07 13:57:05.000000 mdxpy-1.3.2/mdxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-07 13:57:05.000000 mdxpy-1.3.2/mdxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 13:57:05.000000 mdxpy-1.3.2/mdxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 13:57:05.000000 mdxpy-1.3.2/mdxpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-01-19 11:32:22.000000 mdxpy-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     8260 2022-10-10 13:17:58.000000 mdxpy-1.3.2/readme.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 13:57:06.008938 mdxpy-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-08-07 13:50:31.000000 mdxpy-1.3.2/setup.py
+-rw-rw-rw-   0        0        0    47402 2023-08-07 13:46:55.000000 mdxpy-1.3.2/test.py
```

### Comparing `mdxpy-1.3.1/LICENSE` & `mdxpy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxpy-1.3.1/PKG-INFO` & `mdxpy-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple, yet elegant MDX library for TM1
 Home-page: https://github.com/cubewise-code/mdxpy
 Maintainer: Marius Wirtz
 Maintainer-email: MWirtz@cubewise.com
 License: MIT-LICENSE
 Keywords: MDX,TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Platform: any
```

### Comparing `mdxpy-1.3.1/images/logo.png` & `mdxpy-1.3.2/images/logo.png`

 * *Files identical despite different names*

### Comparing `mdxpy-1.3.1/mdxpy/mdx.py` & `mdxpy-1.3.2/mdxpy/mdx.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,18 +458,18 @@
     @staticmethod
     def ancestor(member: Union[str, Member], ancestor: int) -> 'MdxHierarchySet':
         if isinstance(member, str):
             member = Member.of(member)
         return AncestorHierarchySet(member, ancestor)
 
     @staticmethod
-    def drill_down_level(member: Union[str, Member]) -> 'MdxHierarchySet':
+    def drill_down_level(member: Union[str, Member], level: int) -> 'MdxHierarchySet':
         if isinstance(member, str):
             member = Member.of(member)
-        return DrillDownLevelHierarchySet(member)
+        return DrillDownLevelHierarchySet(member, level)
 
     @staticmethod
     def descendants(member: Union[str, Member], level_or_depth: Union[MdxLevelExpression, int] = None,
                     desc_flag: Union[str, Order] = None) -> 'MdxHierarchySet':
         if isinstance(member, str):
             member = Member.of(member)
         return DescendantsHierarchySet(member, level_or_depth, desc_flag)
@@ -696,20 +696,27 @@
 
     def to_mdx(self) -> str:
         return f"{{TM1DRILLDOWNMEMBER({self.underlying_hierarchy_set.to_mdx()}, {self.set2}{self.recursive})}}"
 
 
 class DrillDownLevelHierarchySet(MdxHierarchySet):
 
-    def __init__(self, member: Member):
+    def __init__(self, member: Member, level: int =1):
         super(DrillDownLevelHierarchySet, self).__init__(member.dimension, member.hierarchy)
         self.member = member
+        self.level = level
 
     def to_mdx(self) -> str:
-        return f"{{DRILLDOWNLEVEL({{{self.member.unique_name}}})}}"
+        startstring = ''
+        endstring = ''
+        for _ in range(self.level):
+            startstring += 'DRILLDOWNLEVEL('
+            endstring += ')'
+            
+        return f"{{{startstring}{{{self.member.unique_name}}}{endstring}}}"
 
 
 class DescendantsHierarchySet(MdxHierarchySet):
 
     def __init__(self, member: Member, level_or_depth: Union[int, MdxLevelExpression] = None,
                  description_flag: DescFlag = None):
         super(DescendantsHierarchySet, self).__init__(member.dimension, member.hierarchy)
```

### Comparing `mdxpy-1.3.1/mdxpy.egg-info/PKG-INFO` & `mdxpy-1.3.2/mdxpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple, yet elegant MDX library for TM1
 Home-page: https://github.com/cubewise-code/mdxpy
 Maintainer: Marius Wirtz
 Maintainer-email: MWirtz@cubewise.com
 License: MIT-LICENSE
 Keywords: MDX,TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Platform: any
```

### Comparing `mdxpy-1.3.1/readme.md` & `mdxpy-1.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `mdxpy-1.3.1/setup.py` & `mdxpy-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = open('readme.md').read()
 
 setup(
     name="mdxpy",
-    version='1.3.1',
+    version='1.3.2',
     maintainer='Marius Wirtz',
     maintainer_email='MWirtz@cubewise.com',
     license="MIT-LICENSE",
     url='https://github.com/cubewise-code/mdxpy',
     platforms=["any"],
     description="A simple, yet elegant MDX library for TM1",
     long_description=DESCRIPTION,
```

### Comparing `mdxpy-1.3.1/test.py` & `mdxpy-1.3.2/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,20 +269,27 @@
         hierarchy_set = MdxHierarchySet.ancestor(Member.of("Dimension", "Element"), 1)
 
         self.assertEqual(
             "{ANCESTOR([dimension].[dimension].[element],1)}",
             hierarchy_set.to_mdx())
 
     def test_mdx_hierarchy_set_drill_down_level(self):
-        hierarchy_set = MdxHierarchySet.drill_down_level(Member.of("Dimension", "Element"))
+        hierarchy_set = MdxHierarchySet.drill_down_level(Member.of("Dimension", "Element"), level=1)
 
         self.assertEqual(
             "{DRILLDOWNLEVEL({[dimension].[dimension].[element]})}",
             hierarchy_set.to_mdx())
 
+        hierarchy_set = MdxHierarchySet.drill_down_level(Member.of("Dimension", "Element"), level=3)
+
+        self.assertEqual(
+            "{DRILLDOWNLEVEL(DRILLDOWNLEVEL(DRILLDOWNLEVEL({[dimension].[dimension].[element]})))}",
+            hierarchy_set.to_mdx())
+
+
     def test_mdx_hierarchy_set_tm1_drill_down_member_all_recursive(self):
         hierarchy_set = MdxHierarchySet.members([Member.of("dimension", "element")]).tm1_drill_down_member(
             recursive=True)
 
         self.assertEqual(
             "{TM1DRILLDOWNMEMBER({[dimension].[dimension].[element]}, ALL, RECURSIVE)}",
             hierarchy_set.to_mdx())
```

