# Comparing `tmp/syntaxlight-0.1.3.tar.gz` & `tmp/syntaxlight-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.1.3.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.4.tar", max compression
```

## Comparing `syntaxlight-0.1.3.tar` & `syntaxlight-0.1.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.3/LICENSE
--rw-r--r--   0        0        0      463 2023-08-05 13:52:25.613007 syntaxlight-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.3/README.md
--rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.3/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.3/syntaxlight/ast.py
--rw-r--r--   0        0        0     2244 2023-07-30 03:01:17.999345 syntaxlight-0.1.3/syntaxlight/css/all.css
--rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.3/syntaxlight/css/asm.css
--rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.3/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.3/syntaxlight/css/c.css
--rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.3/syntaxlight/css/css.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.3/syntaxlight/css/index.css
--rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.3/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.3/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.3/syntaxlight/css/makefile.css
--rw-r--r--   0        0        0      876 2023-08-01 01:05:24.169127 syntaxlight-0.1.3/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     2907 2023-08-02 06:45:18.634086 syntaxlight-0.1.3/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.3/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.3/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.3/syntaxlight/error.py
--rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.3/syntaxlight/example.py
--rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.3/syntaxlight/export.py
--rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.3/syntaxlight/gdt.py
--rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.3/syntaxlight/language.py
--rw-r--r--   0        0        0      579 2023-08-05 06:18:01.794963 syntaxlight-0.1.3/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.3/syntaxlight/lexers/asm_lexer.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.3/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.3/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.3/syntaxlight/lexers/css_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.3/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.3/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.3/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.3/syntaxlight/lexers/makefile_lexer.py
--rw-r--r--   0        0        0     4457 2023-08-02 08:39:10.819146 syntaxlight-0.1.3/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.3/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.3/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.3/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.3/syntaxlight/parsers/asm_parser.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.3/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   106244 2023-08-05 13:51:29.921960 syntaxlight-0.1.3/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.3/syntaxlight/parsers/css_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.3/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.3/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.3/syntaxlight/parsers/makefile_parser.py
--rw-r--r--   0        0        0    13418 2023-08-05 02:43:25.809482 syntaxlight-0.1.3/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     4619 2023-08-02 08:26:36.227646 syntaxlight-0.1.3/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.3/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.3/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.3/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.3/syntaxlight/template.html
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.4/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-07 13:42:28.134353 syntaxlight-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.4/README.md
+-rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.4/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.4/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.4/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.4/syntaxlight/css/asm.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.4/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.4/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.4/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.4/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.4/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.4/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.4/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.4/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     3068 2023-08-07 13:38:06.334941 syntaxlight-0.1.4/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.4/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.4/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.4/syntaxlight/error.py
+-rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.4/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.4/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.4/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.4/syntaxlight/language.py
+-rw-r--r--   0        0        0      579 2023-08-05 06:18:01.794963 syntaxlight-0.1.4/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.4/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.4/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.4/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.4/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.4/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.4/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.4/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.4/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.4/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.4/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.4/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.4/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.4/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.4/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   106329 2023-08-05 13:55:32.850499 syntaxlight-0.1.4/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.4/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.4/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.4/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.4/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13418 2023-08-05 02:43:25.809482 syntaxlight-0.1.4/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.4/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.4/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.4/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.4/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.4/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.4/PKG-INFO
```

### Comparing `syntaxlight-0.1.3/LICENSE` & `syntaxlight-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/README.md` & `syntaxlight-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/ast.py` & `syntaxlight-0.1.4/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/all.css` & `syntaxlight-0.1.4/syntaxlight/css/all.css`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     color: #6A9955; /* @--comment */
     color: #DCDCAA; /* @--function int func() */
     color: #4EC9B0; /* @--struct class */
     color: #D7BA6E; /* @--controlchar \n\t */
     color: #4FC1FF; /* @--enum type */
     color: #88D6FE; /* @--format type */
     color: #9EB2BF; /* @--punctuator . ; :  */
-    color: #D4D4D4; /* @--operator +-*=  */
-    color: #969696;
+    color: #d4d4d4; /* @--operator +-*=  */
+    color: #10bd01;
 }
 
 .one-dark-pro {
     color: #23272E; /* @--background */
     color: #DA4D3E; /* @--variant a */
     color: #C678DD; /* @--type int */
     color: #C678DD; /* @--define include */
```

### Comparing `syntaxlight-0.1.3/syntaxlight/css/asm.css` & `syntaxlight-0.1.4/syntaxlight/css/asm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/bnf.css` & `syntaxlight-0.1.4/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/c.css` & `syntaxlight-0.1.4/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/css.css` & `syntaxlight-0.1.4/syntaxlight/css/css.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/index.css` & `syntaxlight-0.1.4/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/json.css` & `syntaxlight-0.1.4/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/lua.css` & `syntaxlight-0.1.4/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/makefile.css` & `syntaxlight-0.1.4/syntaxlight/css/makefile.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/css/shell.css` & `syntaxlight-0.1.4/syntaxlight/css/shell.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,8 @@
 
 .Token.HOST_NAME {
     color: --struct;
 }
 
 .Token.DIR_PATH {
     color: --type;
-}
+}
```

### Comparing `syntaxlight-0.1.3/syntaxlight/css/themes.json` & `syntaxlight-0.1.4/syntaxlight/css/themes.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222223%*

 * *Differences: {"'vscode'": "{'extension': {'shell': {'.Token.HOST_NAME': 'color: #00c867;', '.Token.Success': "*

 * *             "'color: #00c867;', '.Token.Fail': 'color: #d00101;'}}}"}*

```diff
@@ -79,15 +79,18 @@
             "json": {
                 ".Token.Keyword": "color: #327ED0;"
             },
             "makefile": {
                 ".Token.OPTION": "color: #b3b2b2;"
             },
             "shell": {
-                ".Token.OPTION": "color: #b3b2b2;"
+                ".Token.Fail": "color: #d00101;",
+                ".Token.HOST_NAME": "color: #00c867;",
+                ".Token.OPTION": "color: #b3b2b2;",
+                ".Token.Success": "color: #00c867;"
             },
             "toml": {
                 ".Token.Keyword": "color: #327ED0;"
             }
         }
     }
 }
```

### Comparing `syntaxlight-0.1.3/syntaxlight/css/toml.css` & `syntaxlight-0.1.4/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/error.py` & `syntaxlight-0.1.4/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/example.py` & `syntaxlight-0.1.4/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/export.py` & `syntaxlight-0.1.4/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/gdt.py` & `syntaxlight-0.1.4/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/language.py` & `syntaxlight-0.1.4/syntaxlight/language.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/__init__.py` & `syntaxlight-0.1.4/syntaxlight/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/asm_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/asm_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/css_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/css_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/makefile_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/makefile_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/shell_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     DIR_PATH = 'DirPath'
     TAG = 'Tag'
 
 
 class ShellLexer(Lexer):
     def __init__(self, text: str, LanguageTokenType: Enum = ShellTokenType):
         super().__init__(text, LanguageTokenType)
-        self.build_long_op_dict(['&&','>>','<<'])
+        self.build_long_op_dict(['&&','>>','<<','==','==='])
 
     def get_option(self):
         """
         长短选项
         -s --options
         """
         result = ""
@@ -71,15 +71,15 @@
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
             if self.current_char.isdigit():
-                return self.get_number(accept_bit=True, accept_hex=True)
+                return self.get_number(accept_bit=True, accept_hex=True, end_chars=['s'])
 
             if self.current_char.isalnum() or self.current_char in ('_','.','/'):
                 token = self.get_id(extend_chars=["_", "-", ".",'/',':','+','-','@','~'])
                 if bool(re.match(r'^\w+@[\w.-]+:[~\w/]+', token.value)):
                     if self.current_char in ('#', '$'):
                         token.value += self.current_char
                         token.column += 1
```

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.4/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/asm_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/asm_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/c_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1276,26 +1276,27 @@
 
         所以这里做了一个对于 <initializer-list> 的补充
         """
         node = CastExpression()
         type_names = []
         
         '''
-        @扩展文法
+        @特殊处理
         对于强制类型转换 (uint64)trampoline (见 test/c/40.c)
         '''
         while self.current_token.type == TokenType.LPAREN and (
             self.peek_next_token().type in self.cfirst_set.type_name or self._type_cast_check()
         ):
             if self.peek_next_token().type in self.cfirst_set.type_name:
                 node.register_token(self.eat(TokenType.LPAREN))
                 type_names.append(self.type_name())
                 node.register_token(self.eat(TokenType.RPAREN))
             else:
                 node.register_token(self.eat(TokenType.LPAREN))
+                # 对于未知符号强制类型的情况将其修改为 TYPEDEF_ID
                 self.current_token.type = CTokenType.TYPEDEF_ID
                 GDT.register_id(self.current_token.value, CSS.TYPEDEF)
                 type_names.append(self.type_name())
                 node.register_token(self.eat(TokenType.RPAREN))
         node.update(type_names=type_names)
         if self.current_token.type in self.cfirst_set.unary_expression:
             node.update(expr=self.unary_expression())
```

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/css_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/css_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/makefile_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/makefile_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/shell_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,32 @@
     KEYWORD = "Keyword"
     PROGRAM = "Program"
     VARIANT = "Variant"
     FUNCTION = "Function"
     URL = "Url"
     HOST_NAME = "HostName"
     DIR_PATH = "DirPath"
+    SUCCESS = 'Success'
+    FAIL = 'Fail'
 
 
 class ShellParser(Parser):
     def __init__(
         self, lexer, skip_invisible_characters=False, skip_space=True, display_warning=True
     ):
         super().__init__(lexer, skip_invisible_characters, skip_space, display_warning)
 
     def parse(self):
         """
         bash 的文法可变因素太多, 这里直接不使用 BNF 采取匹配的方式
         """
-        is_program_name = True
+        is_program_name = True        
+        success_words = ["ok", "passed", "pass", "success", "yes", "completed", "finished", "done", "good"]
+        fail_words = ["fail", "failed", "error", "warning", "bug", "no", "problem", "issue", "incorrect", "unsuccessful"]
+
         new_program_token_type = [TokenType.LF, TokenType.PIPE, TokenType.SEMI, TokenType.AND]
         while self.current_token.type != TokenType.EOF:
             if self.current_token.type == TokenType.BACK_SLASH and self.peek_next_token().type == TokenType.LF:
                 self.eat()
                 self.eat_lf()
                 continue
 
@@ -75,24 +80,30 @@
                         r"^https?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?(?:;[\w\-\.,@?^=%&:\/~\+#=]*)?$",
                         self.current_token.value,
                     )
                 ):
                     self.current_token.add_css(ShellCSS.URL)
                 elif self.is_valid_path(self.current_token.value):
                     self.current_token.type = ShellTokenType.PATH
+                elif re.match(r'\b(' + '|'.join(success_words) + r')\b', self.current_token.value.lower()):
+                    self.current_token.add_css(ShellCSS.SUCCESS)
+                elif re.match(r'\b(' + '|'.join(fail_words) + r')\b', self.current_token.value.lower()):
+                    self.current_token.add_css(ShellCSS.FAIL)
+
+
 
             if is_program_name:
                 if self.current_token.type in (TokenType.ID, ShellTokenType.PATH):
                     is_program_name = False
                     self.current_token.add_css(ShellCSS.PROGRAM)
             else:
                 if self.current_token.type in new_program_token_type:
                     is_program_name = True
 
-            if self.peek_next_token().type == TokenType.ASSIGN:
+            if self.peek_next_token().type in (TokenType.ASSIGN, TokenType.EQ):
                 self.current_token.add_css(ShellCSS.VARIANT)
 
             if self.current_token.type == TokenType.STRING:
                 self.string_inside_format(self.current_token)
                 continue
 
             self.eat()
```

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.4/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.4/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.3/PKG-INFO` & `syntaxlight-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.1.3
+Version: 0.1.4
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

