# Comparing `tmp/db2text-0.1.3.tar.gz` & `tmp/db2text-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2text-0.1.3.tar", last modified: Sun Aug  6 04:10:50 2023, max compression
+gzip compressed data, was "db2text-0.1.4.tar", last modified: Mon Aug  7 11:39:49 2023, max compression
```

## Comparing `db2text-0.1.3.tar` & `db2text-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 04:10:50.000000 db2text-0.1.3/
--rwxr--r--   0 root         (0) root         (0)     1063 2021-03-12 13:21:32.000000 db2text-0.1.3/LICENSE
--rwxr--r--   0 root         (0) root         (0)       44 2021-06-03 14:29:28.000000 db2text-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      553 2023-08-06 04:10:50.000000 db2text-0.1.3/PKG-INFO
--rwxr--r--   0 root         (0) root         (0)      154 2021-03-14 10:39:32.000000 db2text-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 04:10:50.000000 db2text-0.1.3/bin/
--rwxr--r--   0 root         (0) root         (0)     1862 2021-07-28 13:44:51.000000 db2text-0.1.3/bin/dbt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 04:10:50.000000 db2text-0.1.3/database2text/
--rwxr--r--   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 db2text-0.1.3/database2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 04:10:50.000000 db2text-0.1.3/database2text/datafile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 04:10:50.000000 db2text-0.1.3/database2text/datafile/sample/
--rwxr--r--   0 root         (0) root         (0)      988 2021-07-12 14:11:19.000000 db2text-0.1.3/database2text/datafile/sample/dbt_oracle11.txt
--rwxr--r--   0 root         (0) root         (0)     4634 2021-07-29 02:21:47.000000 db2text-0.1.3/database2text/datafile/usermenual.md
--rwxr--r--   0 root         (0) root         (0)     1363 2022-03-25 06:10:04.000000 db2text-0.1.3/database2text/mysql.py
--rwxr--r--   0 root         (0) root         (0)     6017 2023-08-06 03:58:07.000000 db2text-0.1.3/database2text/oracle11.py
--rwxr--r--   0 root         (0) root         (0)     5915 2021-07-30 06:11:52.000000 db2text-0.1.3/database2text/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 04:10:50.000000 db2text-0.1.3/db2text.egg-info/
--rwxr--r--   0 root         (0) root         (0)      553 2023-08-06 04:10:50.000000 db2text-0.1.3/db2text.egg-info/PKG-INFO
--rwxr--r--   0 root         (0) root         (0)      381 2023-08-06 04:10:50.000000 db2text-0.1.3/db2text.egg-info/SOURCES.txt
--rwxr--r--   0 root         (0) root         (0)        1 2023-08-06 04:10:50.000000 db2text-0.1.3/db2text.egg-info/dependency_links.txt
--rwxr--r--   0 root         (0) root         (0)        1 2021-06-03 14:11:16.000000 db2text-0.1.3/db2text.egg-info/not-zip-safe
--rwxr--r--   0 root         (0) root         (0)       14 2023-08-06 04:10:50.000000 db2text-0.1.3/db2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 04:10:50.000000 db2text-0.1.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1910 2023-08-06 04:10:11.000000 db2text-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:49.000000 db2text-0.1.4/
+-rwxr--r--   0 root         (0) root         (0)     1063 2021-03-12 13:21:32.000000 db2text-0.1.4/LICENSE
+-rwxr--r--   0 root         (0) root         (0)       44 2021-06-03 14:29:28.000000 db2text-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      553 2023-08-07 11:39:49.000000 db2text-0.1.4/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      154 2021-03-14 10:39:32.000000 db2text-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:49.000000 db2text-0.1.4/bin/
+-rwxr--r--   0 root         (0) root         (0)     1862 2021-07-28 13:44:51.000000 db2text-0.1.4/bin/dbt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:49.000000 db2text-0.1.4/database2text/
+-rwxr--r--   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 db2text-0.1.4/database2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:49.000000 db2text-0.1.4/database2text/datafile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:49.000000 db2text-0.1.4/database2text/datafile/sample/
+-rwxr--r--   0 root         (0) root         (0)      988 2021-07-12 14:11:19.000000 db2text-0.1.4/database2text/datafile/sample/dbt_oracle11.txt
+-rwxr--r--   0 root         (0) root         (0)     4634 2021-07-29 02:21:47.000000 db2text-0.1.4/database2text/datafile/usermenual.md
+-rwxr--r--   0 root         (0) root         (0)     1363 2022-03-25 06:10:04.000000 db2text-0.1.4/database2text/mysql.py
+-rwxr--r--   0 root         (0) root         (0)     6198 2023-08-07 01:15:25.000000 db2text-0.1.4/database2text/oracle11.py
+-rwxr--r--   0 root         (0) root         (0)     5915 2021-07-30 06:11:52.000000 db2text-0.1.4/database2text/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:49.000000 db2text-0.1.4/db2text.egg-info/
+-rwxr--r--   0 root         (0) root         (0)      553 2023-08-07 11:39:49.000000 db2text-0.1.4/db2text.egg-info/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      381 2023-08-07 11:39:49.000000 db2text-0.1.4/db2text.egg-info/SOURCES.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2023-08-07 11:39:49.000000 db2text-0.1.4/db2text.egg-info/dependency_links.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2021-06-03 14:11:16.000000 db2text-0.1.4/db2text.egg-info/not-zip-safe
+-rwxr--r--   0 root         (0) root         (0)       14 2023-08-07 11:39:49.000000 db2text-0.1.4/db2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 11:39:49.000000 db2text-0.1.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1910 2023-08-06 04:10:53.000000 db2text-0.1.4/setup.py
```

### Comparing `db2text-0.1.3/LICENSE` & `db2text-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `db2text-0.1.3/PKG-INFO` & `db2text-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2text
-Version: 0.1.3
+Version: 0.1.4
 Summary: database to text
 Home-page: https://gitee.com/chenc224/dbt
 Author: Chen chuan
 Author-email: kcchen@139.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db2text-0.1.3/bin/dbt` & `db2text-0.1.4/bin/dbt`

 * *Files identical despite different names*

### Comparing `db2text-0.1.3/database2text/datafile/sample/dbt_oracle11.txt` & `db2text-0.1.4/database2text/datafile/sample/dbt_oracle11.txt`

 * *Files identical despite different names*

### Comparing `db2text-0.1.3/database2text/datafile/usermenual.md` & `db2text-0.1.4/database2text/datafile/usermenual.md`

 * *Files identical despite different names*

### Comparing `db2text-0.1.3/database2text/mysql.py` & `db2text-0.1.4/database2text/mysql.py`

 * *Files identical despite different names*

### Comparing `db2text-0.1.3/database2text/oracle11.py` & `db2text-0.1.4/database2text/oracle11.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
                 col["COLUMN_COMMENT"]=db.res1("select comments from user_col_comments where table_name=:n and column_name=:cn",n=oname,cn=col["COLUMN_NAME"])
                 if col["DATA_DEFAULT"]!=None:
                     col["DATA_DEFAULT"]=col["DATA_DEFAULT"].strip()
                 oridata.append(col)
             for column_name,data_type,char_length,data_precision,data_scale,nullable,default_length,data_default in db.exec("select column_name,data_type,char_length,data_precision,data_scale,nullable,default_length,data_default from all_tab_cols where owner='%s' and table_name='%s' order by column_id" %(owner,oname)):
                 odata=odata+"  %s%*s" %(column_name,maxcsize-len(column_name)+1," ")
                 ctype="char"
-                cns="%s[%d]" %(column_name,char_length+1)
                 desc=db.res1("select comments from user_col_comments where table_name=:n and column_name=:cn",n=oname,cn=column_name)
                 if not desc:desc=""
                 if data_type=="NUMBER":
                     if data_precision is not None and data_scale is not None:
                         if data_scale==0:
                             if data_precision<8:ctype="int"
                             else:ctype="long"
@@ -44,14 +43,15 @@
                         ctype="long"
                         odata=odata+"NUMBER"
                     else:
                         print("table %s column %s type %s length %s %s %s" %(oname,column_name,data_type,char_length,data_precision,data_scale))
                         sys.exit(-1)
                     cns=column_name
                 elif data_type in ("VARCHAR2","VARCHAR","CHAR","NVARCHAR2","NVARCHAR"):
+                    cns="%s[%d]" %(column_name,char_length+1)
                     odata=odata+"%s(%d)" %(data_type,char_length)
                 elif data_type.startswith("TIMESTAMP"):
                     cns="%s[20]" %(column_name)
                     odata=odata+"%s" %(data_type)
                 elif data_type in("DATE"):
                     cns="%s[20]" %(column_name)
                     odata=odata+"%s" %(data_type)
@@ -68,15 +68,18 @@
                     print("table %s column %s type %s length %s %s %s" %(oname,column_name,data_type,char_length,data_precision,data_scale))
                     sys.exit(-1)
                 if default_length:
                     odata=odata+" default %s" %(data_default.strip())
                 if nullable=="N":
                     odata=odata+" not null"
                 odata=odata+",\n"
-                coldata.append({"type":ctype,"name":column_name,"ns":cns,"desc":desc})
+                cns2=cns
+                if data_type in ("VARCHAR2","VARCHAR","CHAR","NVARCHAR2","NVARCHAR") and char_length==1:
+                    cns=column_name
+                coldata.append({"type":ctype,"name":column_name,"ns":cns,"ns2":cns2,"desc":desc})
             odata=odata[:-2]
             odata=odata+"\n);"
             dbdata["sql"]["TABLE"][oname]=odata
             dbdata["exp"]["TABLE"].append({"tname":oname,"tdesc":tdesc,"ori":oridata,"c":coldata})
 
     def ana_VIEW(otype):
         for oname, in db.exec("select object_name from user_objects where object_type=:ot",ot=otype):
```

### Comparing `db2text-0.1.3/database2text/tool.py` & `db2text-0.1.4/database2text/tool.py`

 * *Files identical despite different names*

### Comparing `db2text-0.1.3/db2text.egg-info/PKG-INFO` & `db2text-0.1.4/db2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2text
-Version: 0.1.3
+Version: 0.1.4
 Summary: database to text
 Home-page: https://gitee.com/chenc224/dbt
 Author: Chen chuan
 Author-email: kcchen@139.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db2text-0.1.3/setup.py` & `db2text-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             f.write(i)
         f.close()
         shutil.move("setup.py2","setup.py")
         os.system("chmod +x setup.py")
 
 setuptools.setup(
     name="db2text",
-    version="0.1.3",
+    version="0.1.4",
     author="Chen chuan",
     author_email="kcchen@139.com",
     description="database to text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/chenc224/dbt",
     packages=setuptools.find_packages(),
```

