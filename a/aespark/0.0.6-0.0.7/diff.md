# Comparing `tmp/aespark-0.0.6.tar.gz` & `tmp/aespark-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aespark-0.0.6.tar", last modified: Wed Aug  2 09:55:21 2023, max compression
+gzip compressed data, was "aespark-0.0.7.tar", last modified: Mon Aug  7 03:36:27 2023, max compression
```

## Comparing `aespark-0.0.6.tar` & `aespark-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.883252 aespark-0.0.6/
--rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1067 2023-08-02 09:55:21.883252 aespark-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-08-02 09:54:45.000000 aespark-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.755752 aespark-0.0.6/aespark/
--rw-rw-rw-   0        0        0    19784 2023-08-02 09:52:09.000000 aespark-0.0.6/aespark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.883252 aespark-0.0.6/aespark/static/
--rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.6/aespark/static/ip.txt
--rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.6/aespark/static/材料模板.docx
-drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.775774 aespark-0.0.6/aespark.egg-info/
--rw-rw-rw-   0        0        0     1067 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-08-02 01:31:36.000000 aespark-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 09:55:21.883252 aespark-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1595 2023-08-02 09:54:57.000000 aespark-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:36:27.403134 aespark-0.0.7/
+-rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1465 2023-08-07 03:36:27.403134 aespark-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-08-07 03:23:48.000000 aespark-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 03:36:27.262541 aespark-0.0.7/aespark/
+-rw-rw-rw-   0        0        0    22715 2023-08-07 03:22:55.000000 aespark-0.0.7/aespark/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:36:27.403134 aespark-0.0.7/aespark/static/
+-rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.7/aespark/static/ip.txt
+-rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.7/aespark/static/材料模板.docx
+-rw-rw-rw-   0        0        0   199772 2023-08-07 02:25:20.000000 aespark-0.0.7/aespark/static/银行卡BIN.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 03:36:27.278162 aespark-0.0.7/aespark.egg-info/
+-rw-rw-rw-   0        0        0     1465 2023-08-07 03:36:27.000000 aespark-0.0.7/aespark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-08-07 03:36:27.000000 aespark-0.0.7/aespark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 03:36:27.000000 aespark-0.0.7/aespark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 03:36:27.000000 aespark-0.0.7/aespark.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-08-07 03:36:27.000000 aespark-0.0.7/aespark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 03:36:27.000000 aespark-0.0.7/aespark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-08-02 01:31:36.000000 aespark-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 03:36:27.403134 aespark-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-08-07 03:24:47.000000 aespark-0.0.7/setup.py
```

### Comparing `aespark-0.0.6/aespark/__init__.py` & `aespark-0.0.7/aespark/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,33 @@
 
     def add_text(self, string: str = '未指定插入内容', level: int = -1):
         '''
         功能简介：
             在docx文档末尾增加新的内容，可以是标题或者段落
         参数解释：
             string    :     新增的内容
-            level     :     内容格式，默认为段落；其他正整数则为对于级别标题
+            level     :     内容格式，默认为段落，其余正整数为标题、对于标题等级
         '''
         if level == -1:
             self.doc.add_paragraph(string)
         else:
             self.doc.add_heading(string, level=level)
 
+    def add_picture(self, url:str, scale:float=1):
+        '''
+        功能简介：
+            在docx文档末尾插入图片
+        参数解释：
+            url 图片文件路径
+            scale   图片缩放比例，默认不缩放；例如 3：放大3倍，0.5：缩小50%
+        '''
+        picture = self.doc.add_picture(url)
+        picture.width = int(picture.width * scale)
+        picture.height = int(picture.height * scale)
+
     def add_table(self, df: pd.DataFrame, sty: str = 'Grid Table 5 Dark Accent 1', fontsize: int = 10):
         '''
         功能简介：
             在docx文档末尾插入新表格
         参数解释：
             df          :   需插入的表格
             sty         :   可选 表格风格
@@ -379,14 +391,39 @@
         if 'urlstr' not in locals():
             urlstr = i
         else:
             urlstr += '/'+i
         if os.path.exists(urlstr) is False:
             os.mkdir(urlstr)
 
+def DataClean_amontCleaning(df:pd.DataFrame, clo:str):
+    '''
+    功能简介：
+        交易金额清洗
+    阐述解释：
+        df  需要清洗的表
+        clo 需要清洗的列名
+    '''
+    try:
+        df[clo] = df[clo].astype('float')
+    except:
+        df.reset_index(drop=True, inplace=True)
+        count = 0
+        for i in df.index:
+            try:
+                float(df[clo][i])
+            except:
+                df[clo][i] = np.nan
+                count += 1
+
+        df[clo] = df[clo].astype('float')
+        print(f"金额清洗：共清洗错误金额{count}条，占比：{'{:.2%}'.format(count/len(df))}")
+    finally:
+        return df
+
 
 def DataClean_inOutCleaning(str: str):
     '''
     功能简介：
         统一借贷标志
     所需参数：
         需要清洗的字符，建议配合pandas.apply使用
@@ -514,24 +551,58 @@
         基于交易数据产出账户交易概况表
     参数解释：
         df  交易数据表
         collist 字段列表，顺序需要一致，[主端账户，交易金额，借贷标志，交易时间]
     调用示例：
         ddf = PivotTable_transView(df01,['用户ID', '金额(元)', '收/支', '创建时间'])
     '''
-    df[collist[1]] = df[collist[1]].astype('float')
+    df = df[[collist[0],collist[1], collist[2], collist[3]]]
+    df = DataClean_amontCleaning(df, collist[1])
     df[collist[2]] = df[collist[2]].apply(DataClean_inOutCleaning)
     df[collist[3]] = df[collist[3]].apply(DataClean_TimeConversion)
+    if '进' not in list(df[collist[2]].drop_duplicates()) or '出' not in list(df[collist[2]].drop_duplicates()):
+        df.loc[len(df)] = ['填充用账户', 0, '进', '1999.01.01 11:14:42']
+        df.loc[len(df)] = ['填充用账户', 0, '出', '1999.01.01 11:14:42']
     piv = df.pivot_table(index=collist[0], columns=collist[2], values=collist[1], aggfunc=['sum', 'count']).reset_index()
     piv.columns = [''.join([i[1],i[0]]).replace('sum', '金额').replace('count', '次数') for i in piv.columns]
+    if '填充用账户' in list(piv[collist[0]]):
+        piv.drop(piv[piv[collist[0]]=='填充用账户'].index, inplace=True)
     if len(piv.columns) == 7:
         piv = piv.take([0, 1, 4, 2, 5, 3, 6], axis=1)
     else:
         piv = piv.take([0, 1, 3, 2, 4], axis=1)
+    piv.fillna(0, inplace=True)
+    piv['总金额'] = piv['其他金额']+piv['出金额']+piv['进金额'] if len(piv.columns) == 7 else piv['出金额']+piv['进金额']
+    df[collist[3]] = pd.to_datetime(df[collist[3]])
     piv2 = df.pivot_table(index=collist[0], values=collist[3], aggfunc=['min', 'max']).reset_index()
     piv2.columns = [collist[0], '首次交易', '末次交易']
-    piv2['首次交易'] = piv2['首次交易'].apply(lambda x:str(x)[:str(x).index(' ')])
-    piv2['末次交易'] = piv2['末次交易'].apply(lambda x:str(x)[:str(x).index(' ')])
+    piv2['首次交易'] = piv2['首次交易'].apply(lambda x:str(x)[:str(x).index(' ')].replace('-','.'))
+    piv2['末次交易'] = piv2['末次交易'].apply(lambda x:str(x)[:str(x).index(' ')].replace('-','.'))
 
     piv = pd.merge(left=piv, right=piv2, how='left', on=collist[0])
+    for i in piv.columns:
+        if '金额' in i:
+            piv[i] = piv[i].apply(lambda x: '%.2f'%x)
+        elif '次数' in i:
+            piv[i] = piv[i].astype('int')
+    piv.sort_values(by=['总金额', '末次交易', '首次交易'], ascending=[False, False, True], inplace=True)
+
+    return piv
 
-    return piv
+class BANK():
+
+    def __init__(self):
+        dist = pkg_resources.get_distribution("aespark")
+        self.df = pd.read_table(f'{dist.location}/aespark/static/银行卡BIN.txt', keep_default_na='')
+
+    def Parse_bankNumber(self, card: str):
+        '''
+        功能简介：
+            银行卡归属行查询
+        return：
+            返回一个字典，查询状态、卡类型、归属行
+        '''
+        lins = self.df[self.df['长度']==len(card)]
+        for i in lins.index:
+            if card[:lins['BIN长度'][i]] == str(lins['卡头'][i]):
+                return {'statu':'success','lex':lins['卡类型'][i],'bank':lins['银行'][i]}
+        return {'statu':'fail','lex':'','bank':''}
```

### Comparing `aespark-0.0.6/aespark/static/ip.txt` & `aespark-0.0.7/aespark/static/ip.txt`

 * *Files identical despite different names*

### Comparing `aespark-0.0.6/aespark/static/材料模板.docx` & `aespark-0.0.7/aespark/static/材料模板.docx`

 * *Files identical despite different names*

### Comparing `aespark-0.0.6/setup.py` & `aespark-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name='aespark', version='0.0.6',
+setuptools.setup(name='aespark', version='0.0.7',  # 2023.08.07 11.24
                  description='Generate a QR code that can adapt to the cylinder',
                  long_description=open(
                      'README.md', 'r', encoding='utf-8').read(),
                  author='wtianxin',
                  author_email='1007582510@qq.com',
                  url='https://pypi.org/project/aespark/',
                  license='MIT',  # 与之前你选用的许可证类型有关系
```

