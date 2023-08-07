# Comparing `tmp/mbp-1.5.8.tar.gz` & `tmp/mbp-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbp-1.5.8.tar", last modified: Mon Nov  7 08:01:12 2022, max compression
+gzip compressed data, was "mbp-1.5.9.tar", last modified: Thu Dec  1 03:35:15 2022, max compression
```

## Comparing `mbp-1.5.8.tar` & `mbp-1.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 08:01:12.609263 mbp-1.5.8/
--rw-rw-rw-   0        0        0     1088 2022-07-22 16:45:56.000000 mbp-1.5.8/LICENSE
--rw-rw-rw-   0        0        0     1514 2022-11-07 08:01:12.609263 mbp-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2022-11-07 08:00:54.000000 mbp-1.5.8/README.md
--rw-rw-rw-   0        0        0      108 2022-07-22 18:32:41.000000 mbp-1.5.8/pyproject.toml
--rw-rw-rw-   0        0        0      688 2022-11-07 08:01:12.610296 mbp-1.5.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-07 08:01:12.601148 mbp-1.5.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-07 08:01:12.608266 mbp-1.5.8/src/mbp.egg-info/
--rw-rw-rw-   0        0        0     1514 2022-11-07 08:01:12.000000 mbp-1.5.8/src/mbp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2022-11-07 08:01:12.000000 mbp-1.5.8/src/mbp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 08:01:12.000000 mbp-1.5.8/src/mbp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-11-07 08:01:12.000000 mbp-1.5.8/src/mbp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-11-07 08:01:12.000000 mbp-1.5.8/src/mbp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    33120 2022-11-07 08:00:54.000000 mbp-1.5.8/src/mbp.py
+drwxrwxrwx   0        0        0        0 2022-12-01 03:35:15.786588 mbp-1.5.9/
+-rw-rw-rw-   0        0        0     1088 2022-07-22 16:45:56.000000 mbp-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0     1514 2022-12-01 03:35:15.786588 mbp-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2022-12-01 03:27:32.000000 mbp-1.5.9/README.md
+-rw-rw-rw-   0        0        0      108 2022-07-22 18:32:41.000000 mbp-1.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0      688 2022-12-01 03:35:15.790980 mbp-1.5.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-12-01 03:35:15.777353 mbp-1.5.9/src/
+drwxrwxrwx   0        0        0        0 2022-12-01 03:35:15.786588 mbp-1.5.9/src/mbp.egg-info/
+-rw-rw-rw-   0        0        0     1514 2022-12-01 03:35:15.000000 mbp-1.5.9/src/mbp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2022-12-01 03:35:15.000000 mbp-1.5.9/src/mbp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-01 03:35:15.000000 mbp-1.5.9/src/mbp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2022-12-01 03:35:15.000000 mbp-1.5.9/src/mbp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2022-12-01 03:35:15.000000 mbp-1.5.9/src/mbp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    33762 2022-12-01 03:34:16.000000 mbp-1.5.9/src/mbp.py
```

### Comparing `mbp-1.5.8/LICENSE` & `mbp-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mbp-1.5.8/PKG-INFO` & `mbp-1.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbp
-Version: 1.5.8
+Version: 1.5.9
 Summary: Make Python even more beautiful :) This package includes implementations that you wish were in the standard library..
 Home-page: https://github.com/sudongqi/MoreBeautifulPython.git
 Author: Dongqi Su
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -21,15 +21,15 @@
     
     > python -m mbp
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp.py
     cpu_count             16
-    version               1.5.8
+    version               1.5.9
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 * replacement for logging
```

### Comparing `mbp-1.5.8/README.md` & `mbp-1.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     
     > python -m mbp
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp.py
     cpu_count             16
-    version               1.5.8
+    version               1.5.9
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 * replacement for logging
```

### Comparing `mbp-1.5.8/setup.cfg` & `mbp-1.5.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6270 0d0a 7665 7273 696f 6e20   = mbp..version 
-00000020: 3d20 312e 352e 380d 0a61 7574 686f 7220  = 1.5.8..author 
+00000020: 3d20 312e 352e 390d 0a61 7574 686f 7220  = 1.5.9..author 
 00000030: 3d20 446f 6e67 7169 2053 750d 0a64 6573  = Dongqi Su..des
 00000040: 6372 6970 7469 6f6e 203d 204d 616b 6520  cription = Make 
 00000050: 5079 7468 6f6e 2065 7665 6e20 6d6f 7265  Python even more
 00000060: 2062 6561 7574 6966 756c 203a 2920 5468   beautiful :) Th
 00000070: 6973 2070 6163 6b61 6765 2069 6e63 6c75  is package inclu
 00000080: 6465 7320 696d 706c 656d 656e 7461 7469  des implementati
 00000090: 6f6e 7320 7468 6174 2079 6f75 2077 6973  ons that you wis
```

### Comparing `mbp-1.5.8/src/mbp.egg-info/PKG-INFO` & `mbp-1.5.9/src/mbp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbp
-Version: 1.5.8
+Version: 1.5.9
 Summary: Make Python even more beautiful :) This package includes implementations that you wish were in the standard library..
 Home-page: https://github.com/sudongqi/MoreBeautifulPython.git
 Author: Dongqi Su
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -21,15 +21,15 @@
     
     > python -m mbp
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp.py
     cpu_count             16
-    version               1.5.8
+    version               1.5.9
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 * replacement for logging
```

### Comparing `mbp-1.5.8/src/mbp.py` & `mbp-1.5.9/src/mbp.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 from io import StringIO
 from collections.abc import Iterator, Iterable
 from datetime import datetime, timezone
 from multiprocessing import Process, Queue, cpu_count
 from pathlib import Path
 from wcwidth import wcswidth
 
-VERSION = '1.5.8'
+VERSION = '1.5.9'
 
 __all__ = [
     # replacement for logging
     'log', 'logger', 'get_logger', 'set_global_logger', 'reset_global_logger', 'recorder',
     'NOTSET', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL', 'SILENT',
     # replacement for multiprocessing
     'Workers', 'work',
     # syntax sugar for common utilities
-    'try_f', 'type_in', 'get_range', 'get_items', 'join_path', 'exec_dir', 'lib_path',
+    'try_f', 'type_of', 'range_of', 'items_of', 'jp', 'join_path', 'run_dir', 'lib_path',
     # tools for file system & data handling
-    'make_dirs', 'make_files', 'make_dirs_for',
-    'traverse', 'this_dir', 'dir_of', 'get_only_file_if_dir', 'get_file_name', 'get_dir_name',
-    'load_txt', 'load_jsonl', 'load_json', 'save_json', 'save_jsonl',
-    'iterate', 'open_file', 'file_paths_under', 'open_files',
+    'load_txt', 'load_jsonl', 'load_json', 'save_json', 'save_jsonl', 'iterate', 'open_file',
+    'traverse', 'this_dir', 'dir_of', 'get_only_sub_path', 'file_basename', 'dir_basename',
+    'init_dirs', 'init_files', 'init_dirs_for', 'files_under', 'open_files',
     # tools for summarizations
     'print_line', 'enclose', 'enclose_timer', 'error_msg', 'prints', 'print_iter', 'print_table', 'debug',
     # tools for simple statistics
     'timer', 'curr_time', 'avg', 'min_max_avg', 'n_min_max_avg', 'CPU_COUNT'
 ]
 
 NOTSET, DEBUG, INFO, WARNING, ERROR, CRITICAL, SILENT = 0, 10, 20, 30, 40, 50, 60
@@ -60,15 +59,15 @@
 
 
 def open_files_for_logger(file):
     res = file if isinstance(file, list) else [file]
     for i in range(len(res)):
         f = res[i]
         if isinstance(f, str):
-            make_dirs_for(f)
+            init_dirs_for(f)
             res[i] = open(f, 'w', encoding='utf-8')
     return res
 
 
 class Logger:
     def __init__(self, name='', file=sys.stdout, level=INFO, meta_info=False, sep=' '):
         self.level = level
@@ -173,20 +172,20 @@
         else:
             if buffer_value:
                 buffer_value = buffer_value.rstrip().split('\n')
                 self.tape.extend(buffer_value)
         self.logger.__exit__(_type, value, _traceback)
 
 
-def error_msg(e, detailed=False, seperator='\n'):
+def error_msg(e, detailed=False, sep='\n'):
     if not detailed:
         return repr(e)
     else:
         res = traceback.format_exc()
-        return res.replace('\n', seperator)
+        return res.replace('\n', sep)
 
 
 class Worker(Process):
     def __init__(self, f, inp, out, worker_id=None, cached_inp=None, built_inp=None, detailed_error=True,
                  progress=True):
         super(Worker, self).__init__()
         self.worker_id = worker_id
@@ -338,26 +337,27 @@
         return gzip.open(path, 'rt', encoding=encoding)
     elif compression == 'bz2':
         return bz2.open(path, 'rb')
     else:
         assert False, '{} not supported'.format(compression)
 
 
-def file_paths_under(path, pattern=r".*"):
+def files_under(path, pattern=r".*"):
+    # return  iterator of (absolute_path, relative_path, file_name)
     _is_dir_if_exist(path)
     matcher = re.compile(pattern)
     for p, dirs, files in os.walk(path):
         for file_name in files:
             if matcher.fullmatch(file_name):
                 full_path = join_path(p, file_name)
-                yield full_path, full_path[len(path):], file_name
+                yield os.path.abspath(full_path), full_path[len(path):], file_name
 
 
 def open_files(path, encoding='utf-8', compression=None, pattern=r".*", progress=True):
-    for full_path, _, file_name in file_paths_under(path, pattern):
+    for full_path, _, file_name in files_under(path, pattern):
         try:
             yield open_file(full_path, encoding, compression)
             if progress:
                 log('found {} <== {}'.format(file_name, full_path))
         except PermissionError:
             if progress:
                 log('no permission to open {} <== {}'.format(file_name, full_path))
@@ -389,15 +389,15 @@
 
 def save_jsonl(data, path, encoding='utf-8'):
     with open(path, 'w', encoding=encoding) as f:
         for d in data:
             f.write(json.dumps(d, ensure_ascii=False) + '\n')
 
 
-def type_in(data, types):
+def type_of(data, types):
     assert isinstance(types, list), 'types must be a list'
     for idx, _type in enumerate(types):
         if isinstance(data, _type):
             return idx + 1
     return 0
 
 
@@ -406,17 +406,18 @@
     start = max(start, 0)
     step = max(step, 1)
     for idx, item in enumerate(data):
         if start <= idx < end and (idx - start) % step == 0:
             yield idx, item
 
 
-def get_range(data, start=0, end=None, step=1, reverse=False):
-    assert isinstance(data, Iterable), 'data should be an Iterable'
+def range_of(data, start=0, end=None, step=1, reverse=False):
+    # replace of ==> for i in range(data)
 
+    assert isinstance(data, Iterable), 'data should be an Iterable'
     if isinstance(data, Iterator):
         assert not reverse, 'cannot set reverse=True when data is an Iterator'
         for idx, _ in _range_iterate(data, start, end, step):
             yield idx
     else:
         step = max(step, 1)
         start = max(start, 0)
@@ -431,59 +432,59 @@
             for i in range(end - 1, start - 1, -step):
                 yield i
         else:
             for i in range(start, end, step):
                 yield i
 
 
-def get_items(data, start=0, end=None, step=1, reverse=False):
+def items_of(data, start=0, end=None, step=1, reverse=False):
     assert isinstance(data, Iterable), 'input should be an Iterable'
     if isinstance(data, Iterator):
         assert not reverse, 'cannot set reverse=True when data is an Iterator'
         for _, item in _range_iterate(data, start, end, step):
             yield item
 
-    for idx in get_range(data, start, end, step, reverse):
+    for idx in range_of(data, start, end, step, reverse):
         yield data[idx]
 
 
 COLLECTION_TYPES = [list, set, tuple, dict]
 
 
 def _build_table(rows, space=3, sub_table_space=1, filler=' '):
     space = max(space, 1)
 
-    rows_type = type_in(rows, COLLECTION_TYPES)
+    rows_type = type_of(rows, COLLECTION_TYPES)
     if not rows_type:
         return [str(rows)]
     elif rows_type == 4:
         _rows = []
         for k, v in rows.items():
             r = _build_table(v, sub_table_space, sub_table_space, filler)
             _rows.append([k, r])
         rows = _rows
 
     # calculate max column width
     num_col = -1
     _rows = []
     for row in rows:
-        row_type = type_in(row, COLLECTION_TYPES)
+        row_type = type_of(row, COLLECTION_TYPES)
         if not row_type:
             row = [row]
         num_col = max(num_col, len(row))
         _rows.append(row)
     rows = _rows
 
     data = []
     for row in rows:
         if len(row) != num_col:
             row += [''] * (num_col - len(row))
 
         row = [_build_table(item, sub_table_space, sub_table_space, filler)
-               if type_in(item, COLLECTION_TYPES) else [str(item)]
+               if type_of(item, COLLECTION_TYPES) else [str(item)]
                for item in row]
         max_height = max(len(r) for r in row)
         new_rows = [['' for _ in range(len(row))] for _ in range(max_height)]
         for j, items in enumerate(row):
             for i in range(len(items)):
                 new_rows[i][j] = items[i]
         data.extend(new_rows)
@@ -527,15 +528,15 @@
     sep_len = len(sep)
     kv_sep_len = len(kv_sep)
 
     # int, float, single-line str
     def is_short_data(_d):
         if _d is None:
             return True
-        r = type_in(_d, [int, float, str, bool])
+        r = type_of(_d, [int, float, str, bool])
         if r == 3:
             return not any(True for ch in _d if ch == '\n')
         return r
 
     def put_quote(string):
         return quote + string + quote if isinstance(string, str) else str(string)
 
@@ -546,15 +547,15 @@
 
     def print_cache(_tokens, _shift, _extra_indent):
         line = sep.join(_tokens)
         if _extra_indent is None:
             line = _shift * ' ' + line
         log_raw(line)
 
-    data_type = type_in(data, [list, tuple, set, dict, str])
+    data_type = type_of(data, [list, tuple, set, dict, str])
     if is_short_data(data):
         if extra_indent is None:
             log_raw(shift_str + put_quote(data))
         else:
             log_raw(put_quote(data))
     # collection
     elif data_type in {1, 2, 3}:
@@ -677,43 +678,52 @@
                 log(shift * ' ', end='')
                 log(item, level=level)
 
 
 VALID_REFERENCE_ARGUMENTS_PATTERN = r'\(([_a-zA-Z][_a-zA-Z0-9]*( *= *[_a-zA-Z0-9]+)?( *, *)?)+\)'
 
 
-def debug(*data, iter_data=False, stop=False, level=DEBUG, width=None, char='-'):
+def debug(*data, mode=print, stop=False, level=DEBUG, width=None, char='-'):
     if LOGGER.level <= level:
 
         stack = inspect.stack()
-        filename = get_file_name(stack[1][1])
+        filename = file_basename(stack[1][1])
         function_name = ' [{}]'.format(stack[1][3]) if stack[1][3] != '<module>' else ''
 
         code_str = stack[1].code_context[0].strip()
         r = re.search('debug' + VALID_REFERENCE_ARGUMENTS_PATTERN, code_str)
         assert len(data) >= 1, '{} ==> debug() need at least 1 argument'.format(code_str)
         assert r is not None, '{} ==> debug() can only take named arguments'.format(code_str)
         arguments = [s.strip() for s in code_str[r.start(): r.end()][len('debug') + 1:-1].split(',')]
 
         with enclose('{}{}: {}'.format(filename, function_name, code_str), width=width, char=char):
-            if iter_data:
+            if mode == log or mode == print:
+                if len(data) > 1:
+                    for k, v in zip(arguments, data):
+                        log(k, end=': ')
+                        log(v)
+                else:
+                    log(data)
+            elif mode == print_iter:
                 if len(data) > 1:
                     for k, v in zip(arguments, data):
                         log(k, end=': \n')
                         print_iter(v, shift=4)
                 else:
                     print_iter(data[0])
-            else:
+            elif mode == prints:
                 if len(data) > 1:
                     for k, v in zip(arguments, data):
                         log(k, end=': ')
                         prints(v, shift=len(k) + 2, extra_indent=0)
                 else:
                     data = data[0]
                     log(data) if isinstance(data, str) else prints(data)
+            else:
+                assert False, 'mode: {} not supported'.format(mode)
         assert not stop, "debug(stop=True)"
 
 
 def try_f(*args, **kwargs):
     res = {}
     try:
         f = args[0]
@@ -824,71 +834,75 @@
 
 class enclose_timer(enclose):
     def __init__(self, text_or_length='', width=None, max_width=80, char='=', top_margin=0, bottom_margin=1,
                  level=INFO):
         super().__init__(text_or_length, width, max_width, char, top_margin, bottom_margin, True, level)
 
 
+def jp(*args, **kwargs):
+    return os.path.join(*args, **kwargs)
+
+
 def join_path(*args, **kwargs):
     return os.path.join(*args, **kwargs)
 
 
 def lib_path():
     return str(Path(__file__).absolute())
 
 
-def exec_dir():
+def run_dir():
     return os.getcwd()
 
 
 def _is_file_if_exist(path):
     if os.path.exists(path):
         assert os.path.isfile(path), '{} ==> already exist but it\'s a directory'.format(path)
 
 
 def _is_dir_if_exist(path):
     if os.path.exists(path):
         assert os.path.isdir(path), '{} ==> already exist but it\'s a file'.format(path)
 
 
-def make_dirs(path, overwrite=False):
-    paths = path if isinstance(path, list) else [path]
+def init_dirs(path_or_paths, overwrite=False):
+    paths = path_or_paths if isinstance(path_or_paths, list) else [path_or_paths]
     for path in paths:
         path = Path(os.path.abspath(path))
         _is_dir_if_exist(path)
         if overwrite and os.path.exists(path):
             shutil.rmtree(path)
         os.makedirs(path, exist_ok=True)
 
 
-def make_files(path, overwrite=False):
-    paths = path if isinstance(path, list) else [path]
+def init_files(path_or_paths, overwrite=False):
+    paths = path_or_paths if isinstance(path_or_paths, list) else [path_or_paths]
     for path in paths:
         _is_file_if_exist(path)
         if overwrite and os.path.exists(path):
             os.remove(path)
-        make_dirs_for(path)
+        init_dirs_for(path)
         open(path, 'a').close()
 
 
-def make_dirs_for(path, overwrite=False):
-    paths = path if isinstance(path, list) else [path]
+def init_dirs_for(path_or_paths, overwrite=False):
+    paths = path_or_paths if isinstance(path_or_paths, list) else [path_or_paths]
     for path in paths:
         path = Path(os.path.abspath(path))
         _is_file_if_exist(path)
-        make_dirs(dir_of(path), overwrite)
+        init_dirs(dir_of(path), overwrite)
 
 
-def get_file_name(path):
+def file_basename(path):
     path = Path(os.path.abspath(path))
     _is_file_if_exist(path)
     return os.path.basename(path)
 
 
-def get_dir_name(path):
+def dir_basename(path):
     path = Path(os.path.abspath(path))
     _is_dir_if_exist(path)
     return os.path.basename(path)
 
 
 def traverse(path, go_up=0, go_to=None, should_exist=False):
     if isinstance(go_up, str):
@@ -918,27 +932,27 @@
         should_exist = go_to if isinstance(go_to, bool) else should_exist
         go_to = go_up
         go_up = 0
     caller_module = inspect.getmodule(inspect.stack()[1][0])
     return traverse(caller_module.__file__, go_up + 1, go_to, should_exist)
 
 
-def get_only_file_if_dir(dir_path):
+def get_only_sub_path(dir_path):
     if os.path.isdir(dir_path):
         sub_paths = os.listdir(dir_path)
         assert len(sub_paths) == 1, 'there are more than one files/dirs in {}'.format(dir_path)
         return join_path(dir_path, sub_paths[0])
     return dir_path
 
 
 def mbp_info():
     with enclose('More Beautiful Python'):
         rows = [
             ['examples', 'https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py'],
-            ['execution_directory', exec_dir()],
+            ['execution_directory', run_dir()],
             ['library_path', lib_path()],
             ['cpu_count', CPU_COUNT],
             ['version', VERSION]
         ]
         print_table(rows)
```

