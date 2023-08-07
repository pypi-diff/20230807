# Comparing `tmp/pymdfs-0.1.tar.gz` & `tmp/pymdfs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymdfs-0.1.tar", last modified: Tue Feb 28 01:13:43 2023, max compression
+gzip compressed data, was "dist\pymdfs-0.1.1.tar", last modified: Mon Aug  7 09:32:39 2023, max compression
```

## Comparing `pymdfs-0.1.tar` & `pymdfs-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 01:13:43.000000 pymdfs-0.1/
--rw-rw-rw-   0        0        0    35821 2020-07-23 14:20:29.000000 pymdfs-0.1/LICENSE
--rw-rw-rw-   0        0        0      218 2023-02-20 02:13:03.000000 pymdfs-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7412 2023-02-28 01:13:43.000000 pymdfs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7111 2023-02-28 01:12:37.000000 pymdfs-0.1/README.rst
--rw-rw-rw-   0        0        0     7058 2023-02-28 01:12:23.000000 pymdfs-0.1/README.zh_CN.rst
-drwxrwxrwx   0        0        0        0 2023-02-28 01:13:43.000000 pymdfs-0.1/pymdfs/
--rw-rw-rw-   0        0        0      164 2023-02-20 17:28:18.000000 pymdfs-0.1/pymdfs/__init__.py
--rw-rw-rw-   0        0        0    17134 2023-02-27 02:23:23.000000 pymdfs-0.1/pymdfs/client.py
--rw-rw-rw-   0        0        0     4844 2023-02-27 02:22:52.000000 pymdfs-0.1/pymdfs/client_dump.py
--rw-rw-rw-   0        0        0     1150 2023-02-27 02:22:33.000000 pymdfs-0.1/pymdfs/client_query.py
-drwxrwxrwx   0        0        0        0 2023-02-28 01:13:43.000000 pymdfs-0.1/pymdfs/config/
--rw-rw-rw-   0        0        0     5447 2023-02-15 01:52:11.000000 pymdfs-0.1/pymdfs/config/ElementNameDict.yml
-drwxrwxrwx   0        0        0        0 2023-02-28 01:13:43.000000 pymdfs-0.1/pymdfs/diamond/
--rw-rw-rw-   0        0        0      134 2023-02-20 16:54:02.000000 pymdfs-0.1/pymdfs/diamond/__init__.py
--rw-rw-rw-   0        0        0     8280 2023-02-16 09:27:22.000000 pymdfs-0.1/pymdfs/diamond/diamond1.py
--rw-rw-rw-   0        0        0     6884 2023-02-17 02:35:17.000000 pymdfs-0.1/pymdfs/diamond/diamond11.py
--rw-rw-rw-   0        0        0    21095 2023-02-16 09:13:21.000000 pymdfs-0.1/pymdfs/diamond/diamond14.py
--rw-rw-rw-   0        0        0     6586 2023-02-16 09:30:40.000000 pymdfs-0.1/pymdfs/diamond/diamond16.py
--rw-rw-rw-   0        0        0     7771 2023-02-16 09:27:30.000000 pymdfs-0.1/pymdfs/diamond/diamond2.py
--rw-rw-rw-   0        0        0     9037 2023-02-16 09:27:36.000000 pymdfs-0.1/pymdfs/diamond/diamond3.py
--rw-rw-rw-   0        0        0     8058 2023-02-16 09:32:46.000000 pymdfs-0.1/pymdfs/diamond/diamond31.py
--rw-rw-rw-   0        0        0     8133 2023-02-17 02:34:48.000000 pymdfs-0.1/pymdfs/diamond/diamond4.py
--rw-rw-rw-   0        0        0     8511 2023-02-16 09:23:25.000000 pymdfs-0.1/pymdfs/diamond/diamond41.py
--rw-rw-rw-   0        0        0     7481 2023-02-16 09:26:25.000000 pymdfs-0.1/pymdfs/diamond/diamond42.py
--rw-rw-rw-   0        0        0     8425 2023-02-20 16:46:47.000000 pymdfs-0.1/pymdfs/diamond/diamond5.py
--rw-rw-rw-   0        0        0     8238 2023-02-27 02:26:05.000000 pymdfs-0.1/pymdfs/diamond/diamond7.py
--rw-rw-rw-   0        0        0     7699 2023-02-16 09:29:12.000000 pymdfs-0.1/pymdfs/diamond/diamond8.py
--rw-rw-rw-   0        0        0     5223 2023-02-17 02:35:44.000000 pymdfs-0.1/pymdfs/latlon.py
-drwxrwxrwx   0        0        0        0 2023-02-28 01:13:43.000000 pymdfs-0.1/pymdfs/mdfs/
--rw-rw-rw-   0        0        0    13509 2023-02-15 01:52:11.000000 pymdfs-0.1/pymdfs/mdfs/DataBlock_pb2.py
--rw-rw-rw-   0        0        0      128 2023-02-20 16:58:56.000000 pymdfs-0.1/pymdfs/mdfs/__init__.py
--rw-rw-rw-   0        0        0     6415 2023-02-17 02:36:10.000000 pymdfs-0.1/pymdfs/mdfs/mdfs_grid_data.py
--rw-rw-rw-   0        0        0     6226 2023-02-20 02:21:58.000000 pymdfs-0.1/pymdfs/mdfs/mdfs_station_data.py
-drwxrwxrwx   0        0        0        0 2023-02-28 01:13:43.000000 pymdfs-0.1/pymdfs.egg-info/
--rw-rw-rw-   0        0        0     7412 2023-02-28 01:13:42.000000 pymdfs-0.1/pymdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-02-28 01:13:42.000000 pymdfs-0.1/pymdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 01:13:42.000000 pymdfs-0.1/pymdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-02-28 01:13:42.000000 pymdfs-0.1/pymdfs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-28 01:03:47.000000 pymdfs-0.1/pymdfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-02-28 01:13:42.000000 pymdfs-0.1/pymdfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-28 01:13:42.000000 pymdfs-0.1/pymdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-28 01:13:43.000000 pymdfs-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-02-27 08:18:40.000000 pymdfs-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:32:39.000000 pymdfs-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2023-08-07 08:37:00.000000 pymdfs-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      218 2023-08-07 08:37:00.000000 pymdfs-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8064 2023-08-07 09:32:39.000000 pymdfs-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7802 2023-08-07 08:44:53.000000 pymdfs-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs/
+-rw-rw-rw-   0        0        0      164 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/__init__.py
+-rw-rw-rw-   0        0        0    17134 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/client.py
+-rw-rw-rw-   0        0        0     4976 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/client_dump.py
+-rw-rw-rw-   0        0        0     1191 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/client_query.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs/config/
+-rw-rw-rw-   0        0        0     5447 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/config/ElementNameDict.yml
+drwxrwxrwx   0        0        0        0 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs/diamond/
+-rw-rw-rw-   0        0        0      134 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/__init__.py
+-rw-rw-rw-   0        0        0     8280 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond1.py
+-rw-rw-rw-   0        0        0     6801 2023-08-07 08:50:50.000000 pymdfs-0.1.1/pymdfs/diamond/diamond11.py
+-rw-rw-rw-   0        0        0    21047 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond14.py
+-rw-rw-rw-   0        0        0     6586 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond16.py
+-rw-rw-rw-   0        0        0     7771 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond2.py
+-rw-rw-rw-   0        0        0     9037 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond3.py
+-rw-rw-rw-   0        0        0     8058 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond31.py
+-rw-rw-rw-   0        0        0     8647 2023-08-07 08:50:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond4.py
+-rw-rw-rw-   0        0        0     8511 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond41.py
+-rw-rw-rw-   0        0        0     7481 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond42.py
+-rw-rw-rw-   0        0        0     8425 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond5.py
+-rw-rw-rw-   0        0        0     8238 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond7.py
+-rw-rw-rw-   0        0        0     7699 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/diamond/diamond8.py
+-rw-rw-rw-   0        0        0     5223 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/latlon.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs/mdfs/
+-rw-rw-rw-   0        0        0    13509 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/mdfs/DataBlock_pb2.py
+-rw-rw-rw-   0        0        0      128 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/mdfs/__init__.py
+-rw-rw-rw-   0        0        0     7561 2023-08-07 09:18:08.000000 pymdfs-0.1.1/pymdfs/mdfs/mdfs_grid_data.py
+-rw-rw-rw-   0        0        0     6226 2023-08-07 08:37:00.000000 pymdfs-0.1.1/pymdfs/mdfs/mdfs_station_data.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/
+-rw-rw-rw-   0        0        0     8064 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      882 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       97 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 09:32:39.000000 pymdfs-0.1.1/pymdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:32:39.000000 pymdfs-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2023-08-07 09:20:02.000000 pymdfs-0.1.1/setup.py
```

### Comparing `pymdfs-0.1/LICENSE` & `pymdfs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/README.zh_CN.rst` & `pymdfs-0.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #. 过滤站点和经纬度裁剪
 #. 主要的数据结构为`pandas.DataFrame <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html>`_
    和 `xarray.DataArray <https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html>`_
 
 README
 ^^^^^^
 
-- `English <https://github.com/zjobsdev/pymdfs/blob/master/README.rst>`_
+- `English <https://github.com/zjobsdev/pymdfs/blob/master/README.en.rst>`_
 
 安装方法
 ^^^^^^^^^^^^^^^
 
 使用 *pip* 可以直接安装
 
 .. code:: shell
@@ -61,14 +61,28 @@
     from pymdfs import MdfsClient
 
     gds = MdfsClient('xxx.xxx.xxx.xxx:xxxx')
     dar = gds.sel('ECMWF_HR', datetime(2023, 2, 20, 20), fh=24, varname='RH',
                   level=850, lat=slice(20, 40), lon=slice(110, 130))
     print(dar)
 
+以下程序，使用 **MdfsClient** 拉取2023年2月20日20时观测的24小时站点降水量，
+并过滤出北纬20-40度、东经110-130度范围的站点数据，数据结构为 pandas.DataFrame
+
+
+.. code:: python
+
+    from datetime import datetime
+    from pymdfs import MdfsClient
+
+    gds = MdfsClient('xxx.xxx.xxx.xxx:xxxx')
+    df = gds.sel('SURFACE', datetime(2023, 2, 20, 20), varname='RAIN24_ALL_STATION',
+                 lat=slice(20, 40), lon=slice(110, 130))
+    print(df)
+
 
 命令行程序
 ^^^^^^^^^^^^^^^^^^^^^^
 
 1. client_query
 ----------------
 
@@ -92,15 +106,15 @@
     +----------------------------------+---------------------------------+
 
 
 示例:
 
 .. code:: python
 
-    client_query ECMWF_HR
+    mdfs_query ECMWF_HR
 
 2. client_dump
 ----------------
 
 用法:
     mdfs_dump [-h] [-f FH] [-e OUTFILE] [-c COMPLEVEL] [-v VARNAME] [-x LON] [-y LAT] [-p LEVEL] [-t OFFSET_INITTIME] [--name_map NAME_MAP] [-s SERVER] [-o LOGLEVEL] datasource inittime
 
@@ -142,13 +156,16 @@
     | -s SERVER, --server SERVER                            | GDS server address                  |
     +-------------------------------------------------------+-------------------------------------+
     | -o LOGLEVEL, --loglevel LOGLEVEL                      | logger level in number              |
     +-------------------------------------------------------+-------------------------------------+
 
 示例:
 
+以下脚本使用 **client_dump** 命令行程序，拉取ECMWF 2023年2月19日20时起报的24小时预报时效，
+500hPa的相对湿度、U/V风场、温度场、高度场的数据，并存储为 ECMWF_HR.2023021920.nc 文件。
+
 .. code:: shell
 
-     client_dump ECMWF_HR 2023021920 -f 24 --level 500 -v RH,UGRD,VGRD,TMP,HGT -e ECMWF_HR.2023021920.nc
+     mdfs_dump ECMWF_HR 2023021920 -f 24 --level 500 -v RH,UGRD,VGRD,TMP,HGT -e ECMWF_HR.2023021920.nc
 
 
 更多细节和特征，请参与项目文档 `readthedocs <www.pymdfs.readthedocs.org>`_ .
```

### Comparing `pymdfs-0.1/pymdfs/client.py` & `pymdfs-0.1.1/pymdfs/client.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/client_dump.py` & `pymdfs-0.1.1/pymdfs/client_dump.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#!/usr/bin/env python
-
-# -*- coding: utf-8 -*-
-# @Author: wqshen
-# @Email: wqshen91@gmail.com
-# @Date: 2019/12/27 14:42
-# @Last Modified by: wqshen
-
-import os
-import sys
-import argparse
-import logzero
-import pandas as pd
-import xarray as xr
-from logzero import logger
-from datetime import datetime
-from pymdfs import MdfsClient
-
-
-def construct_slice(coord):
-    """construct point, slice, or step slice from list or tuple
-
-    Parameters
-    ----------
-    coord : list or tuple
-        (point,) or (start, stop) or (start, stop, step)
-
-    Returns
-    -------
-    s : float, slice
-        slice or point
-    """
-    if len(coord) == 1:
-        s = coord[0]
-    elif 1 < len(coord) < 3:
-        s = slice(*coord)
-    else:
-        raise Exception("length of coord must less than or equal 3")
-    return s
-
-
-def tpyecast(string):
-    """cast string into int/float/str"""
-    try:
-        return int(string)
-    except ValueError:
-        try:
-            return float(string)
-        except Exception:
-            return string
-
-
-def _main():
-    example_text = """Example:
-     client_dump ECMWF_HR 2023021920 -f 24 --level 500 -v RH,UGRD,VGRD,TMP,HGT -e ECMWF_HR.2023021920.nc
-     """
-
-    args_parser = lambda s: [tpyecast(item) for item in s.split(',')]
-    parser = argparse.ArgumentParser(description='MDFS Data Dumper', epilog=example_text,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('datasource', help='data source name')
-    parser.add_argument('inittime', help='model initial datetime or observation datetime')
-    parser.add_argument('-f', '--fh', help='model forecast hour', type=args_parser)
-    parser.add_argument('-e', '--outfile', type=str, help='output netcdf file name')
-    parser.add_argument('-c', '--complevel', type=str, help='output netcdf4 compress level',
-                        default=5)
-    parser.add_argument('-v', '--varname', help='model variable names', type=args_parser)
-    parser.add_argument('-x', '--lon', help='longitude point or range', type=args_parser)
-    parser.add_argument('-y', '--lat', help='latitude point or range', type=args_parser)
-    parser.add_argument('-p', '--level', help='pressure level point or range', type=args_parser)
-    parser.add_argument('-t', '--offset-inittime', help='offset inittime (hours) to variable',
-                        type=str)
-    parser.add_argument('--name_map', help='map variable name to new', type=args_parser)
-    parser.add_argument('-s', '--server', type=str, help='GDS server address',
-                        default='xxx.xxx.xxx.xxx')
-    parser.add_argument('-o', '--loglevel', type=int, help='logger level in number', default=20)
-
-    if len(sys.argv) == 1:
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-
-    args = parser.parse_args()
-    logzero.loglevel(args.loglevel)
-    logger.debug(args)
-
-    inittime = datetime.strptime(args.inittime, '%Y%m%d%H')
-    coord_kwargs = dict()
-    if args.lon is not None:
-        coord_kwargs['lon'] = construct_slice(args.lon)
-    if args.lat is not None:
-        coord_kwargs['lat'] = construct_slice(args.lat)
-    if args.level is not None:
-        coord_kwargs['level'] = construct_slice(args.level)
-
-    with MdfsClient(args.server) as mc:
-        dataset = mc.sel(args.datasource, inittime, args.fh, args.varname, **coord_kwargs)
-        logger.debug(dataset)
-        if isinstance(dataset, list):
-            if isinstance(dataset[0], xr.DataArray):
-                dataset = xr.merge(dataset)
-            elif isinstance(dataset[0], pd.DataFrame):
-                dataset = pd.concat(dataset)
-        elif isinstance(dataset, xr.DataArray):
-            dataset = dataset.to_dataset()
-        else:
-            raise TypeError(f"type of return ({type(dataset)}) not be understood.")
-
-        if args.offset_inittime is not None:
-            dataset['time'] = pd.to_datetime(dataset.time.values) + pd.to_timedelta(
-                args.offset_inittime)
-
-        if args.name_map is not None:
-            dataset = dataset.rename({args.name_map[0]: args.name_map[1]})
-
-    logger.info(dataset)
-    if args.outfile is not None:
-        _, file_extension = os.path.splitext(args.outfile)
-        if file_extension in ('.nc', '.nc4') and isinstance(dataset, xr.Dataset):
-            comp = dict(zlib=True, complevel=args.complevel)
-            encoding = {var: comp for var in dataset.data_vars}
-            dataset.to_netcdf(args.outfile, encoding=encoding)
-        elif file_extension in ('.txt', '.csv'):
-            if isinstance(dataset, xr.DataArray):
-                dataset.to_dataframe().to_csv(args.outfile)
-            else:
-                dataset.to_csv(args.outfile)
-        else:
-            raise NotImplementedError("Only support nc, nc4, txt, csv extentsion.")
-
-
-if __name__ == '__main__':
-    _main()
+#!/usr/bin/env python
+
+# -*- coding: utf-8 -*-
+# @Author: wqshen
+# @Email: wqshen91@gmail.com
+# @Date: 2019/12/27 14:42
+# @Last Modified by: wqshen
+
+import os
+import sys
+import argparse
+import logzero
+import pandas as pd
+import xarray as xr
+from logzero import logger
+from datetime import datetime
+from pymdfs import MdfsClient
+
+
+def construct_slice(coord):
+    """construct point, slice, or step slice from list or tuple
+
+    Parameters
+    ----------
+    coord : list or tuple
+        (point,) or (start, stop) or (start, stop, step)
+
+    Returns
+    -------
+    s : float, slice
+        slice or point
+    """
+    if len(coord) == 1:
+        s = coord[0]
+    elif 1 < len(coord) < 3:
+        s = slice(*coord)
+    else:
+        raise Exception("length of coord must less than or equal 3")
+    return s
+
+
+def tpyecast(string):
+    """cast string into int/float/str"""
+    try:
+        return int(string)
+    except ValueError:
+        try:
+            return float(string)
+        except Exception:
+            return string
+
+
+def _main():
+    example_text = """Example:
+     client_dump ECMWF_HR 2023021920 -f 24 --level 500 -v RH,UGRD,VGRD,TMP,HGT -e ECMWF_HR.2023021920.nc
+     """
+
+    args_parser = lambda s: [tpyecast(item) for item in s.split(',')]
+    parser = argparse.ArgumentParser(description='MDFS Data Dumper', epilog=example_text,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser.add_argument('datasource', help='data source name')
+    parser.add_argument('inittime', help='model initial datetime or observation datetime')
+    parser.add_argument('-f', '--fh', help='model forecast hour', type=args_parser)
+    parser.add_argument('-e', '--outfile', type=str, help='output netcdf file name')
+    parser.add_argument('-c', '--complevel', type=str, help='output netcdf4 compress level',
+                        default=5)
+    parser.add_argument('-v', '--varname', help='model variable names', type=args_parser)
+    parser.add_argument('-x', '--lon', help='longitude point or range', type=args_parser)
+    parser.add_argument('-y', '--lat', help='latitude point or range', type=args_parser)
+    parser.add_argument('-p', '--level', help='pressure level point or range', type=args_parser)
+    parser.add_argument('-t', '--offset-inittime', help='offset inittime (hours) to variable',
+                        type=str)
+    parser.add_argument('--name_map', help='map variable name to new', type=args_parser)
+    parser.add_argument('-s', '--server', type=str, help='GDS server address',
+                        default='xxx.xxx.xxx.xxx')
+    parser.add_argument('-o', '--loglevel', type=int, help='logger level in number', default=20)
+
+    if len(sys.argv) == 1:
+        parser.print_help(sys.stderr)
+        sys.exit(1)
+
+    args = parser.parse_args()
+    logzero.loglevel(args.loglevel)
+    logger.debug(args)
+
+    inittime = datetime.strptime(args.inittime, '%Y%m%d%H')
+    coord_kwargs = dict()
+    if args.lon is not None:
+        coord_kwargs['lon'] = construct_slice(args.lon)
+    if args.lat is not None:
+        coord_kwargs['lat'] = construct_slice(args.lat)
+    if args.level is not None:
+        coord_kwargs['level'] = construct_slice(args.level)
+
+    with MdfsClient(args.server) as mc:
+        dataset = mc.sel(args.datasource, inittime, args.fh, args.varname, **coord_kwargs)
+        logger.debug(dataset)
+        if isinstance(dataset, list):
+            if isinstance(dataset[0], xr.DataArray):
+                dataset = xr.merge(dataset)
+            elif isinstance(dataset[0], pd.DataFrame):
+                dataset = pd.concat(dataset)
+        elif isinstance(dataset, xr.DataArray):
+            dataset = dataset.to_dataset()
+        else:
+            raise TypeError(f"type of return ({type(dataset)}) not be understood.")
+
+        if args.offset_inittime is not None:
+            dataset['time'] = pd.to_datetime(dataset.time.values) + pd.to_timedelta(
+                args.offset_inittime)
+
+        if args.name_map is not None:
+            dataset = dataset.rename({args.name_map[0]: args.name_map[1]})
+
+    logger.info(dataset)
+    if args.outfile is not None:
+        _, file_extension = os.path.splitext(args.outfile)
+        if file_extension in ('.nc', '.nc4') and isinstance(dataset, xr.Dataset):
+            comp = dict(zlib=True, complevel=args.complevel)
+            encoding = {var: comp for var in dataset.data_vars}
+            dataset.to_netcdf(args.outfile, encoding=encoding)
+        elif file_extension in ('.txt', '.csv'):
+            if isinstance(dataset, xr.DataArray):
+                dataset.to_dataframe().to_csv(args.outfile)
+            else:
+                dataset.to_csv(args.outfile)
+        else:
+            raise NotImplementedError("Only support nc, nc4, txt, csv extentsion.")
+
+
+if __name__ == '__main__':
+    _main()
```

### Comparing `pymdfs-0.1/pymdfs/client_query.py` & `pymdfs-0.1.1/pymdfs/client_query.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-#!/usr/bin/env python
-
-# -*- coding: utf-8 -*-
-# @Author: wqshen
-# @Email: wqshen91@gmail.com
-# @Date: 2019/12/27 14:42
-# @Last Modified by: wqshen
-
-import sys
-import argparse
-import logzero
-from logzero import logger
-from pymdfs import MdfsClient
-
-
-def _main():
-    example_text = """Example: client_query ECMWF_HR"""
-
-    parser = argparse.ArgumentParser(description='MDFS Data Query',
-                                     epilog=example_text,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('datasource', help='data source name')
-    parser.add_argument('-s', '--server', type=str, help='GDS server address',
-                        default='xxx.xxx.xxx.xxx')
-    parser.add_argument('-o', '--loglevel', type=int, help='loglevel: 10, 20, 30, 40, 50',
-                        default=20)
-
-    if len(sys.argv) == 1:
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-
-    args = parser.parse_args()
-    logzero.loglevel(args.loglevel)
-    logger.debug(args)
-
-    mc = MdfsClient(args.server)
-    print(mc.list_vars(args.datasource))
-
-
-if __name__ == '__main__':
-    _main()
+#!/usr/bin/env python
+
+# -*- coding: utf-8 -*-
+# @Author: wqshen
+# @Email: wqshen91@gmail.com
+# @Date: 2019/12/27 14:42
+# @Last Modified by: wqshen
+
+import sys
+import argparse
+import logzero
+from logzero import logger
+from pymdfs import MdfsClient
+
+
+def _main():
+    example_text = """Example: client_query ECMWF_HR"""
+
+    parser = argparse.ArgumentParser(description='MDFS Data Query',
+                                     epilog=example_text,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser.add_argument('datasource', help='data source name')
+    parser.add_argument('-s', '--server', type=str, help='GDS server address',
+                        default='xxx.xxx.xxx.xxx')
+    parser.add_argument('-o', '--loglevel', type=int, help='loglevel: 10, 20, 30, 40, 50',
+                        default=20)
+
+    if len(sys.argv) == 1:
+        parser.print_help(sys.stderr)
+        sys.exit(1)
+
+    args = parser.parse_args()
+    logzero.loglevel(args.loglevel)
+    logger.debug(args)
+
+    mc = MdfsClient(args.server)
+    print(mc.list_vars(args.datasource))
+
+
+if __name__ == '__main__':
+    _main()
```

### Comparing `pymdfs-0.1/pymdfs/config/ElementNameDict.yml` & `pymdfs-0.1.1/pymdfs/config/ElementNameDict.yml`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond1.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond1.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond11.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond11.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,18 +173,17 @@
         # To mask potential missing values
         if self.missing_value is not None:
             var_x = var_x.where(var_x == self.missing_value)
             var_y = var_y.where(var_y == self.missing_value)
         # Append extra attributes to netcdf varibale
         var_x.attrs['description'] = self.head.description + "_" + name[0]
         var_y.attrs['description'] = self.head.description + "_" + name[1]
-        var_x.attrs['inittime'] = datetime(self.head.year, self.head.month, self.head.day,
-                                           self.head.hour)
-        var_y.attrs['inittime'] = datetime(self.head.year, self.head.month, self.head.day,
-                                           self.head.hour)
+        inittime = datetime(self.head.year, self.head.month, self.head.day, self.head.hour)
+        var_x.attrs['inittime'] = f"{inittime:%Y-%m-%d %H:%M}"
+        var_y.attrs['inittime'] = f"{inittime:%Y-%m-%d %H:%M}"
         var_x.attrs['fh'] = self.head.duration
         var_y.attrs['fh'] = self.head.duration
 
         if self.pathfile is not None:
             var_x.attrs['raw'] = self.pathfile
             var_y.attrs['raw'] = self.pathfile
         var = xr.merge([var_x, var_y])
```

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond14.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond14.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
                 # line xyz point number
                 xyz_num = int(data[idx])
                 line_xyz_num.append(xyz_num)
                 idx += 1
 
                 # line xyz
-                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(float)
                 xyz.shape = [xyz_num, 3]
                 line_xyz.append(xyz)
                 idx += xyz_num * 3
 
                 # line label
                 label = data[idx]
                 line_label.append(label)
@@ -164,15 +164,15 @@
                 label_num = int(data[idx])
                 line_label_num.append(label_num)
                 idx += 1
 
                 # label xyz
                 if label_num > 0:
                     label_xyz = np.array(
-                        data[idx:(idx + 3 * label_num)]).astype(np.float)
+                        data[idx:(idx + 3 * label_num)]).astype(float)
                     label_xyz.shape = [label_num, 3]
                     line_label_xyz.append(label_xyz)
                     idx += label_num * 3
                 else:
                     line_label_xyz.append([])
 
             # construct line data type
@@ -210,15 +210,15 @@
 
                 # line symbol xyz point number
                 xyz_num = int(data[idx])
                 linesym_xyz_num.append(xyz_num)
                 idx += 1
 
                 # line symbol xyz
-                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(float)
                 xyz.shape = [xyz_num, 3]
                 linesym_xyz.append(xyz)
                 idx += xyz_num * 3
 
                 # line symbol label
                 label = data[idx]
                 idx += 1
@@ -250,15 +250,15 @@
             for i in range(nlines):
                 # symbol code
                 code = int(data[idx])
                 symbol_code.append(code)
                 idx += 1
 
                 # symbol xyz
-                xyz = np.array(data[idx:(idx + 3)]).astype(np.float)
+                xyz = np.array(data[idx:(idx + 3)]).astype(float)
                 symbol_xyz.append(xyz)
                 idx += 3
 
                 # symbol value
                 value = data[idx]
                 symbol_value.append(value)
                 idx += 1
@@ -292,15 +292,15 @@
 
                 # line xyz point number
                 xyz_num = int(data[idx])
                 cn_xyz_num.append(xyz_num)
                 idx += 1
 
                 # line xyz
-                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(float)
                 xyz.shape = [xyz_num, 3]
                 cn_xyz.append(xyz)
                 idx += 3 * xyz_num
 
                 # line label
                 label = data[idx]
                 cn_label.append(label)
@@ -310,15 +310,15 @@
                 label_num = int(data[idx])
                 cn_label_num.append(label_num)
                 idx += 1
 
                 # label xyz
                 if label_num > 0:
                     label_xyz = np.array(
-                        data[idx:(idx + 3 * label_num)]).astype(np.float)
+                        data[idx:(idx + 3 * label_num)]).astype(float)
                     label_xyz.shape = [3, label_num]
                     cn_label_xyz.append(label_xyz)
                     idx += label_num * 3
                 else:
                     cn_label_xyz.append([])
 
             closed_contours = {
@@ -359,15 +359,15 @@
                 # region xyz point number
                 xyz_num = int(data[idx])
                 weather_region_xyz_num.append(xyz_num)
                 idx += 1
 
                 # region xyz point
                 xyz = np.array(
-                    data[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                    data[idx:(idx + 3 * xyz_num)]).astype(float)
                 xyz.shape = [xyz_num, 3]
                 weather_region_xyz.append(xyz)
                 idx += 3 * xyz_num
 
             weather_region = {
                 "weather_region_code": weather_region_code,
                 "weather_region_xyz_num": weather_region_xyz_num,
@@ -404,36 +404,36 @@
                 # xyz point number
                 xyz_num = int(data[idx])
                 fillarea_num.append(xyz_num)
                 idx += 1
 
                 # xyz point
                 xyz = np.array(
-                    data[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                    data[idx:(idx + 3 * xyz_num)]).astype(float)
                 xyz.shape = [xyz_num, 3]
                 fillarea_xyz.append(xyz)
                 idx += 3 * xyz_num
 
                 # fill type
                 ftype = int(data[idx])
                 fillarea_type.append(ftype)
                 idx += 1
 
                 # line color
-                color = np.array(data[idx:(idx + 4)]).astype(np.int)
+                color = np.array(data[idx:(idx + 4)]).astype(int)
                 fillarea_color.append(color)
                 idx += 4
 
                 # front color
-                front_color = np.array(data[idx:(idx + 4)]).astype(np.int)
+                front_color = np.array(data[idx:(idx + 4)]).astype(int)
                 fillarea_frontcolor.append(front_color)
                 idx += 4
 
                 # background color
-                back_color = np.array(data[idx:(idx + 4)]).astype(np.int)
+                back_color = np.array(data[idx:(idx + 4)]).astype(int)
                 fillarea_backcolor.append(back_color)
                 idx += 4
 
                 # color gradient angle
                 gradient_angle = float(data[idx])
                 fillarea_gradient_angle.append(gradient_angle)
                 idx += 1
@@ -483,15 +483,15 @@
             for i in range(nlines):
                 # code
                 code = int(data[idx])
                 nsymbol_code.append(code)
                 idx += 1
 
                 # xyz
-                xyz = np.array(data[idx:(idx + 3)]).astype(np.float)
+                xyz = np.array(data[idx:(idx + 3)]).astype(float)
                 nsymbol_xyz.append([xyz])
                 idx += 3
 
                 # character length
                 char_len = int(data[idx])
                 nsymbol_charLen.append(char_len)
                 idx += 1
@@ -523,15 +523,15 @@
 
                 # font type
                 font_type = data[idx]
                 nsymbol_fontType.append(font_type)
                 idx += 1
 
                 # color
-                color = np.array(data[idx:(idx + 4)]).astype(np.int)
+                color = np.array(data[idx:(idx + 4)]).astype(int)
                 nsymbol_color.append(color)
                 idx += 4
 
             notes_symbol = {
                 "nsymbol_code": nsymbol_code,
                 "nsymbol_xyz": nsymbol_xyz,
                 "nsymbol_charLen": nsymbol_charLen,
@@ -573,15 +573,15 @@
 
                 # line width
                 width = float(data[idx])
                 plinesym_width.append(width)
                 idx += 1
 
                 # line color
-                color = np.array(data[idx:(idx + 4)]).astype(np.int)
+                color = np.array(data[idx:(idx + 4)]).astype(int)
                 plinesym_color.append([color])
                 idx += 4
 
                 # line type
                 ltype = int(data[idx])
                 plinesym_type.append(ltype)
                 idx += 1
@@ -593,15 +593,15 @@
 
                 # line symbol xyz point nlines
                 xyz_num = int(data[idx])
                 plinesym_xyz_num.append(xyz_num)
                 idx += 1
 
                 # line symbol xyz
-                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(np.float)
+                xyz = np.array(data[idx:(idx + 3 * xyz_num)]).astype(float)
                 xyz.shape = [xyz_num, 3]
                 plinesym_xyz.append(xyz)
                 idx += 3 * xyz_num
 
                 # line symbol label
                 label = data[idx]
                 plinesym_label.append(label)
@@ -611,15 +611,15 @@
                 label_num = int(data[idx])
                 plinesym_label_num.append(label_num)
                 idx += 1
 
                 # label xyz
                 if label_num > 0:
                     label_xyz = np.array(
-                        data[idx:(idx + 3 * label_num)]).astype(np.float)
+                        data[idx:(idx + 3 * label_num)]).astype(float)
                     label_xyz.shape = [label_num, 3]
                     plinesym_label_xyz.append(label_xyz)
                     idx += label_num * 3
                 else:
                     plinesym_label_xyz.append([])
 
             plines_symbol = {
```

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond16.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond16.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond2.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond2.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond3.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond3.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond31.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond31.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond4.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond4.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,24 @@
         self._cast_fields_types()
 
     def _cast_fields_types(self):
         for field in fields(cast(dataclass, self)):
             field_value = getattr(self, field.name)
             setattr(self, field.name, field.type(field_value))
 
+    def __repr__(self):
+        _str = []
+        for field in fields(cast(dataclass, self)):
+            field_value = getattr(self, field.name)
+            if isinstance(field_value, float):
+                _str.append(f"{field_value:.5f}")
+            else:
+                _str.append(str(field_value))
+        return "\t".join(_str[:3]) + "\n" + "\t".join(_str[3:9]) + "\n" + "\t".join(_str[9:])
+
 
 @dataclass
 class Diamond4:
     """Micaps Diamond Data class
 
     From this class, one can read and write Micaps Diamond4 file
 
@@ -128,20 +138,16 @@
             path to file name
         encoding : str, Optional, default: 'GBK'
             encoding of output file
         fmt : Optional[str], default: '.5f'
             float format to save data
         """
         with open(pathfile, 'w', encoding=encoding) as f:
-            head = tuple(map(str, astuple(self.head)))
-            f.write("\t".join(head[:3]) + "\n")
-            f.write("\t".join(head[3:9]) + "\n")
-            f.write("\t".join(head[9:22]) + "\n")
-
-            np.savetxt(f, self.data, fmt=fmt, delimiter='\t')
+            f.write(self.head.__repr__() + "\n")
+            np.savetxt(f, self.data.squeeze(), fmt=fmt, delimiter='\t')
 
     def to_netcdf(self, pathfile: str, name: str, complevel: int = 5):
         """write data into NetCDF4 file
 
         Parameters
         ----------
         pathfile : str
@@ -157,27 +163,31 @@
         ds = data.to_dataset(name=name)
         encoding = {var: comp for var in ds.data_vars}
         ds.to_netcdf(pathfile, encoding=encoding)
 
     def from_xarray(self, darray: xr.DataArray):
         """convert xarray into Diamond4"""
         desc = getattr(darray, 'long_name', 'Unknown')
-        time = getattr(darray, 'time', datetime(1900, 1, 1, 0))
-        it = pd.to_datetime(time)
+        it = getattr(darray, 'time', datetime(1900, 1, 1, 0))
+        if not isinstance(it, datetime):
+            it = it.values
+            if isinstance(it, np.datetime64):
+                it = [it]
+            it = pd.to_datetime(it)[0]
         duration = getattr(darray, 'step', 0)
         level = getattr(darray, 'level', 0)
         xinterval = darray.lon[1] - darray.lon[0]
         yinterval = darray.lat[1] - darray.lat[0]
         startlon = darray.lon.min()
         startlat = darray.lat.min()
         endlon = darray.lon.max()
         endlat = darray.lat.max()
         xsize, ysize = darray.shape[-1], darray.shape[-2]
-        startvalue = darray.min().floor()
-        endvalue = darray.max().ceil()
+        startvalue = np.floor(darray.min().values)
+        endvalue = np.ceil(darray.max().values)
         lineinteravl = (endvalue - startvalue) / 20.
         self.head = Diamond4Head('diamond', 4, desc, it.year, it.month, it.day, it.hour, duration,
                                  level, xinterval, yinterval, startlon, endlon, startlat, endlat,
                                  xsize, ysize, lineinteravl, startvalue, endvalue, )
         self.data = darray.values
         self._ds = darray
 
@@ -204,18 +214,18 @@
         fh = self.head.duration
         leadtime = inittime + timedelta(hours=fh)
         data = xr.DataArray(self.data[None, ...], dims=('time', 'lat', 'lon'),
                             coords={'time': [leadtime], 'lat': lats, 'lon': lons},
                             name=name)
         # To mask potential missing values
         if self.missing_value is not None:
-            data = data.where(data == self.missing_value)
+            data = data.where(data != self.missing_value)
         # Append extra attributes to netcdf varibale
         data.attrs['description'] = self.head.description
-        data.attrs['inittime'] = inittime
+        data.attrs['inittime'] = f"{inittime:%Y-%m-%d %H:%M}"
         data.attrs['fh'] = fh
 
         if self.pathfile is not None:
             data.attrs['raw'] = self.pathfile
         return data
 
     def __enter__(self):
@@ -224,7 +234,11 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Close open dataset"""
         del self.pathfile, self.data, self.head, self._ds
 
     def __repr__(self):
         """print"""
         return self.head.__repr__()
+
+    @property
+    def values(self):
+        return self._ds
```

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond41.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond41.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond42.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond42.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond5.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond5.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond7.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond7.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/diamond/diamond8.py` & `pymdfs-0.1.1/pymdfs/diamond/diamond8.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/latlon.py` & `pymdfs-0.1.1/pymdfs/latlon.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/mdfs/DataBlock_pb2.py` & `pymdfs-0.1.1/pymdfs/mdfs/DataBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs/mdfs/mdfs_grid_data.py` & `pymdfs-0.1.1/pymdfs/mdfs/mdfs_grid_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,45 +77,67 @@
             if 'lat' in kwargs and isinstance(kwargs.get('lat'), slice):
                 lat = kwargs.get('lat')
                 kwargs['lat'] = slice(lat.stop, lat.start, lat.step)
         dar = self._ds.sel(**kwargs)
         return dar
 
     def read(self, path_or_bytes: Union[str, bytes]):
+        def read_block(bytes_arr, p: int = 0):
+            head_data = unpack('=4sh20s50s30sfiiiiiifffifffifff100s', bytes_arr[p:p + 278])
+            head = MdfsGridHead(*head_data)
+            n_points = head.latitudeGridNumber * head.longitudeGridNumber
+            body_data = np.frombuffer(bytes_arr[p + 278:p + 278 + n_points * 4],
+                                      '{}f'.format(n_points))
+            data = np.array(body_data).reshape(head.longitudeGridNumber,
+                                               head.latitudeGridNumber)
+            if head.dtype == 11:
+                p = 278 + data.size * 4
+                block_size = p + data.size * 4
+                body_data_angle = unpack('{}f'.format(data.size), bytes_array[p:block_size])
+                data_angle = np.array(body_data_angle).reshape(head.longitudeGridNumber,
+                                                               head.latitudeGridNumber)
+                data = {'magnitude': data, 'angle': data_angle}
+            return head, data
+
         if isinstance(path_or_bytes, str):
             with open(path_or_bytes, 'rb') as f:
                 bytes_array = f.read()
         else:
             bytes_array = path_or_bytes
-        head_data = unpack('=4sh20s50s30sfiiiiiifffifffifff100s', bytes_array[:278])
-        self.head = MdfsGridHead(*head_data)
-        n_points = self.head.latitudeGridNumber * self.head.longitudeGridNumber
-        body_data = np.frombuffer(bytes_array[278:278 + n_points * 4], '{}f'.format(n_points))
-        data = np.array(body_data).reshape(self.head.longitudeGridNumber,
-                                           self.head.latitudeGridNumber)
-        if self.head.dtype == 11:
-            self.data = {'magnitude': data}
-            p = 278 + n_points * 4
-            body_data_angle = unpack('{}f'.format(n_points), bytes_array[p:p + n_points * 4])
-            self.data['angle'] = np.array(body_data_angle).reshape(self.head.longitudeGridNumber,
-                                                                   self.head.latitudeGridNumber)
+        self.head, self.data = read_block(bytes_array)
+        nbytes = len(bytes_array)
+        size = self.head.latitudeGridNumber * self.head.longitudeGridNumber
+        block_size = 278 + size * 4 * (2 if self.head.dtype == 11 else 1)
+        if nbytes > block_size and nbytes % block_size == 0:
+            heads = [self.head]
+            datas = [self.data]
+            nblocks = int(nbytes / block_size)
+            _ds = [self.to_xarray(name=self.head.element)]
+            for i in range(1, nblocks):
+                self.head, self.data = read_block(bytes_array[block_size * i:block_size * (i + 1)])
+                heads.append(self.head)
+                datas.append(self.data)
+                _ds.append(self.to_xarray(name=self.head.element))
+            self.data = datas
+            self.head = heads
+            self._ds = xr.concat(_ds, dim=xr.DataArray(range(len(_ds)), dims='number')).transpose('time', ...)
         else:
-            self.data = data
-        self._ds = self.to_xarray(name=self.head.element)
+            self._ds = self.to_xarray(name=self.head.element)
+        return self.data
 
     def to_xarray(self, name=None):
         def set_mask_and_attrs(data):
             # To mask potential missing values
             if self.missing_value is not None:
                 data = data.where(data == self.missing_value)
 
             # Append extra attributes to netcdf varibale
             data.attrs['model'] = self.head.modelName
             data.attrs['description'] = self.head.description
-            data.attrs['inittime'] = inittime
+            data.attrs['inittime'] = f"{inittime:%Y-%m-%d %H:%M}"
             data.attrs['fh'] = fh
 
             if self.pathfile is not None:
                 data.attrs['raw'] = self.pathfile
             return data
 
         head = self.head
```

### Comparing `pymdfs-0.1/pymdfs/mdfs/mdfs_station_data.py` & `pymdfs-0.1.1/pymdfs/mdfs/mdfs_station_data.py`

 * *Files identical despite different names*

### Comparing `pymdfs-0.1/pymdfs.egg-info/SOURCES.txt` & `pymdfs-0.1.1/pymdfs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.rst
-README.zh_CN.rst
 setup.py
 pymdfs/__init__.py
 pymdfs/client.py
 pymdfs/client_dump.py
 pymdfs/client_query.py
 pymdfs/latlon.py
 pymdfs.egg-info/PKG-INFO
```

### Comparing `pymdfs-0.1/setup.py` & `pymdfs-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # @Author: wqshen
 # @Date: 2019/4/6 11:59
 # @Last Modified by: wqshen
 
 
 from setuptools import setup, find_packages
 
-version = "0.1"
+version = "0.1.1"
 name = "pymdfs"
 
 install_requires = [
     "awx",
     "numpy>=1.10",
     "xarray",
     "pandas",
     "logzero>=1.0",
     "pyyaml",
-    "protobuf",
+    "protobuf<=3.20",
     "retrying",
     "httplib2"
+    "netCDF4<=1.5.8",
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research/Operation",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

