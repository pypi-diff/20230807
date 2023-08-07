# Comparing `tmp/jhrtools-1.2.0-py3-none-any.whl.zip` & `tmp/jhrtools-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15533 bytes, number of entries: 9
+Zip file size: 14443 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      276 b- defN 22-Mar-16 06:33 jhrtools/__init__.py
--rw-rw-rw-  2.0 fat    16582 b- defN 22-Aug-12 07:47 jhrtools/data_source.py
--rw-rw-rw-  2.0 fat     3817 b- defN 22-Mar-16 06:52 jhrtools/rtdb.py
--rw-rw-rw-  2.0 fat     8790 b- defN 22-Mar-16 06:37 jhrtools/rule_base.py
+-rw-rw-rw-  2.0 fat    14627 b- defN 23-Aug-07 07:37 jhrtools/data_source.py
+-rw-rw-rw-  2.0 fat     4886 b- defN 23-Aug-07 08:12 jhrtools/rtdb.py
+-rw-rw-rw-  2.0 fat     6764 b- defN 23-Aug-07 07:18 jhrtools/rule_base.py
 -rw-rw-rw-  2.0 fat    14091 b- defN 22-Mar-16 06:37 jhrtools/tools.py
--rw-rw-rw-  2.0 fat      530 b- defN 22-Aug-12 07:52 jhrtools-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-12 07:52 jhrtools-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Aug-12 07:52 jhrtools-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      683 b- defN 22-Aug-12 07:52 jhrtools-1.2.0.dist-info/RECORD
-9 files, 44870 bytes uncompressed, 14369 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat      521 b- defN 23-Aug-07 08:12 jhrtools-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 08:12 jhrtools-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Aug-07 08:12 jhrtools-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      683 b- defN 23-Aug-07 08:12 jhrtools-1.2.1.dist-info/RECORD
+9 files, 41949 bytes uncompressed, 13279 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: jhrtools/rule_base.py
 Comment: 
 
 Filename: jhrtools/tools.py
 Comment: 
 
-Filename: jhrtools-1.2.0.dist-info/METADATA
+Filename: jhrtools-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: jhrtools-1.2.0.dist-info/WHEEL
+Filename: jhrtools-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: jhrtools-1.2.0.dist-info/top_level.txt
+Filename: jhrtools-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jhrtools-1.2.0.dist-info/RECORD
+Filename: jhrtools-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jhrtools/data_source.py

```diff
@@ -13,39 +13,38 @@
 from typing import Union, Iterable
 import pandas as pd
 from pandas import DataFrame
 import numpy as np
 import simplejson as json
 import requests
 import sqlalchemy
-from kafka import KafkaProducer, KafkaConsumer, KafkaClient
 from tqdm import tqdm
 import warnings
 from functools import reduce
 
 warnings.filterwarnings('ignore')
 pd.set_option('display.max_columns', 100)
 pd.set_option('display.width', 1000)
 
 """
 数据源模块，操作mysql,rtdb实时库，kafka消息队列等不同数据源。
 """
-__all__ = ['Mysql', 'Rtdb', 'Kafka']
+__all__ = ['Mysql', 'Rtdb']
 
 
 class Mysql(Jet):
     """
     MySQL数据库操作，读取，写入
     """
 
     def __init__(self,
                  host: str = 'localhost',
                  port: Union[int, str] = 3306,
                  user: str = 'root',
-                 pw: str = '',
+                 pw: str = 'jizhongjieneng9-28',
                  name: str = ''):
         """
 
         :param host: mysql数据库地址，默认localhost,ip地址格式：'x.x.x.x'，例如'192.168.1.240'
         :param port: mysql数据库端口
         :param user: 用户名
         :param pw: 密码
@@ -405,71 +404,7 @@
         r = requests.post(self.delete_url, body_json, headers=self._headers)
         raw_dict = json.loads(r.content)
         if raw_dict.get('opResult') == 'SUCCESS':
             print(self.success, f'(points:{len(point)},point name:{list(point)[0]}...)')
         else:
             raise ValueError(self.fail)
 
-
-class Kafka:
-
-    def __init__(self, host: str = 'localhost', port: Union[str, int] = 9092):
-        """
-
-        :param host: kafka主机，默认localhost,ip地址格式：'x.x.x.x'，例如'192.168.1.240'
-        :param port: kafka端口
-        """
-        self.host = host
-        self.port = int(port)
-
-    @property
-    def server(self):
-        return f'{self.host}:{self.port}'
-
-    @property
-    def is_available(self):
-        # 消息队列服务是否可用
-        try:
-            kc = KafkaClient(bootstrap_servers=self.server)
-            if kc.bootstrap_connected():
-                return True
-            else:
-                return False
-        except:
-            return False
-
-    @staticmethod
-    def _value_serializer(obj):
-        """kafka消息序列化器"""
-        return json.dumps(obj, cls=JetEncoder).encode('ascii')
-
-    @staticmethod
-    def _key_serializer(obj: str):
-        return bytes(obj, encoding='utf-8')
-
-    def produce(self, key: str, value, topic: str):
-        """消息队列生产
-
-        :param key: 消息key
-        :param value: 消息
-        :param topic: 消息队列主题
-        """
-        try:
-            # 生产者
-            producer = KafkaProducer(bootstrap_servers=self.server,
-                                     key_serializer=self._key_serializer,
-                                     value_serializer=self._value_serializer)
-            # 发送数据
-            producer.send(topic=topic, value=value, key=key)
-            # 关闭生产者
-            producer.close()
-        except Exception as e:
-            raise e
-
-    def consume(self, *topics: str):
-        """消息队列消费
-
-        :param topics: 主题
-        """
-        consumer = KafkaConsumer(*topics, bootstrap_servers=self.server)
-        for msg in consumer:
-            print(msg)
```

## jhrtools/rtdb.py

```diff
@@ -13,15 +13,35 @@
 from typing import List
 from .data_source import Mysql
 from functools import reduce
 
 """
 rtdb-v10 标准实时库相关操作
 """
-__all__ = ['RTDBPointTable', ]
+__all__ = ['RTDBPointTable', 'PointTable']
+
+
+class PointTable(Mysql):
+
+    def point_table(self):
+        # 实时库系列表
+        tb_tenant, tb_project, tb_meter, tb_point = self.read(["tb_tenant", "tb_project", "tb_meter", "tb_point"])
+        # 实时库表选择列
+        tenant = tb_tenant[['tenant_id', 'tenant_name']]
+        project = tb_project[['tenant_id', 'project_id', 'project_name']]
+        meter = tb_meter[['tenant_id', 'project_id', 'meter_id', 'meter_name']]
+        point = tb_point[['tenant_id', 'project_id', 'meter_id', 'point_id', 'point_name']]
+        # 合并
+        df = reduce(lambda x, y: pd.merge(x, y, how='left'), [point, meter, project, tenant])
+        # 增加点位id和点位名列
+        id_col = ['tenant_id', 'project_id', 'meter_id', 'point_id']
+        df['rtdb_id'] = df[id_col].apply(lambda x: f'{x[0]}.{x[1]}.{x[2]}.{x[3]}', axis=1)
+        name_col = ['tenant_name', 'project_name', 'meter_name', 'point_name']
+        df['rtdb_name'] = df[name_col].apply(lambda x: f'{x[0]}.{x[1]}.{x[2]}.{x[3]}', axis=1)
+        return df
 
 
 class RTDBPointTable:
     """
     RTDB_V10 点位表
     """
```

## jhrtools/rule_base.py

```diff
@@ -10,21 +10,21 @@
 """
 import json
 import re
 import pandas as pd
 from typing import List
 from itertools import product
 import requests
-from .data_source import JetTimeStamp, Rtdb, Kafka
+from .data_source import JetTimeStamp, Rtdb
 
 """
 jet标准规则库相关操作
 """
 
-__all__ = ['Rule', 'RuleMatch', 'run_task']
+__all__ = ['Rule', 'RuleMatch']
 
 
 class Rule:
     def __init__(self, rb_host: str = 'http://192.168.1.97:9991', rb_url='/static/data/api.json'):
         """
 
         :param rb_url: jet规则库配置文件
@@ -183,60 +183,7 @@
         :param rule: 规则
         """
         result = {}
         for sys_equip in self.find_equips(rule):
             d = self._create_job_conf(rule, sys_equip)
             result.update(d)
         return result
-
-
-def run_task(**job):
-    """运行单个任务
-    任务配置文件->获取对应实时库数据->调用规则接口计算（数据+参数）-> 结果发送到kafka
-
-    :param job:
-    :type job:
-    :return:
-    :rtype:
-    """
-    meta_tags = {
-        'group_id': job.get('tenant_id'),
-        'site_id': job.get('project_id'),
-        'equip_sys_type_id': job.get('sys'),
-        'equip_sys_id': job.get('equip_sys_id'),
-        'equip_id': [i.get('equip_id') for i in job.get('equip')],
-        'job_id': job.get('task_id'),
-    }
-    tenant_id = job.get('tenant_id')
-    project_id = job.get('project_id')
-    rule_url = job.get('rule_url')
-    # 获取实时库数据
-    api_body_data = []
-    for i in job.get('equip'):
-        if i.get('use_all'):  # 全部设备
-            pass
-        else:
-            # 测点
-            points = [f'{tenant_id}.{project_id}.{i.get("equip_id")}.{j}' for j in i.get('point_id')]
-            # 查询数据
-            df = Rtdb(points, start_time=i.get('start'), end_time=i.get('end')).query_history()
-            # 格式变换为接口输入
-            df.index = df.index.map(lambda x: JetTimeStamp(x).ms)
-            data = {k: v.reset_index().rename(columns={k: 'value'}).to_dict('list') for k, v in
-                    df.to_dict('series').items()}
-            api_body_data.append(data)
-    # 计算
-    if job.get('rule_para') is not None:
-        api_body_paras = {}
-        for i in job.get('rule_para'):
-            api_body_paras.update({i.get("key"): i.get("value")})
-    else:
-        api_body_paras = None
-    # 请求数据
-    api_body = {'data': api_body_data[0], 'paras': api_body_paras}
-    body_json = json.dumps(api_body)
-    r = requests.post(rule_url, body_json, headers={"Content-Type": "application/json"})
-    # 发送kafka
-    if r.ok:
-        api_result = json.loads(r.content)
-        kafka_value = dict(id=meta_tags, **api_result)
-        Kafka().produce(kafka_value)
```

## Comparing `jhrtools-1.2.0.dist-info/METADATA` & `jhrtools-1.2.1.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: jhrtools
-Version: 1.2.0
-Summary: jet tools
-Author: jihaoran
+Version: 1.2.1
+Summary: jet database tools
+Home-page: UNKNOWN
+Author: Haoran Ji
 Author-email: 944816903@qq.com
 License: MIT
 Platform: UNKNOWN
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: typeguard (==2.13.3)
 Requires-Dist: pandas (==1.4.1)
 Requires-Dist: pathos (==0.2.8)
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: simplejson (==3.17.6)
 Requires-Dist: SQLAlchemy (==1.4.32)
 Requires-Dist: pymysql (==1.0.2)
-Requires-Dist: kafka-python (==2.0.2)
 Requires-Dist: tqdm (==4.63.0)
 Requires-Dist: netifaces (==0.11.0)
 
 UNKNOWN
```

