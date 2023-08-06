# Comparing `tmp/metafid_data-0.1.0-py3-none-any.whl.zip` & `tmp/metafid_data-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 8226 bytes, number of entries: 15
+Zip file size: 8960 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mf_data/__init__.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 mf_data/ise/__init__.py
--rw-r--r--  2.0 unx     3701 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc.py
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 mf_data/ise/utils/__init__.py
--rw-r--r--  2.0 unx     3626 b- defN 80-Jan-01 00:00 mf_data/ise/utils/clean_and_extend_data.py
--rw-r--r--  2.0 unx     3763 b- defN 80-Jan-01 00:00 mf_data/ise/utils/columns.py
--rw-r--r--  2.0 unx     2707 b- defN 80-Jan-01 00:00 mf_data/ise/utils/constants.py
+-rw-r--r--  2.0 unx      723 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard.py
+-rw-r--r--  2.0 unx     3776 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc.py
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 mf_data/ise/utils/__init__.py
+-rw-r--r--  2.0 unx     4032 b- defN 80-Jan-01 00:00 mf_data/ise/utils/clean_and_extend_data.py
+-rw-r--r--  2.0 unx     3781 b- defN 80-Jan-01 00:00 mf_data/ise/utils/columns.py
+-rw-r--r--  2.0 unx     3016 b- defN 80-Jan-01 00:00 mf_data/ise/utils/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mf_data/tgju/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mf_data/tgju/tgju.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 mf_data/utils/__init__.py
 -rw-r--r--  2.0 unx      992 b- defN 80-Jan-01 00:00 mf_data/utils/async_.py
 -rw-r--r--  2.0 unx      278 b- defN 80-Jan-01 00:00 mf_data/utils/get.py
--rw-r--r--  2.0 unx      833 b- defN 80-Jan-01 00:00 metafid_data-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 metafid_data-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1191 b- defN 16-Jan-01 00:00 metafid_data-0.1.0.dist-info/RECORD
-15 files, 17319 bytes uncompressed, 6244 bytes compressed:  63.9%
+-rw-r--r--  2.0 unx      838 b- defN 80-Jan-01 00:00 metafid_data-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 metafid_data-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1271 b- defN 16-Jan-01 00:00 metafid_data-0.1.1.dist-info/RECORD
+16 files, 18975 bytes uncompressed, 6856 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: mf_data/__init__.py
 Comment: 
 
 Filename: mf_data/ise/__init__.py
 Comment: 
 
+Filename: mf_data/ise/rahavard.py
+Comment: 
+
 Filename: mf_data/ise/tsetmc.py
 Comment: 
 
 Filename: mf_data/ise/utils/__init__.py
 Comment: 
 
 Filename: mf_data/ise/utils/clean_and_extend_data.py
@@ -30,17 +33,17 @@
 
 Filename: mf_data/utils/async_.py
 Comment: 
 
 Filename: mf_data/utils/get.py
 Comment: 
 
-Filename: metafid_data-0.1.0.dist-info/METADATA
+Filename: metafid_data-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: metafid_data-0.1.0.dist-info/WHEEL
+Filename: metafid_data-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: metafid_data-0.1.0.dist-info/RECORD
+Filename: metafid_data-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mf_data/ise/tsetmc.py

```diff
@@ -1,56 +1,56 @@
 from urllib.parse import urlencode
 import pandas as pd
 from ..utils import get
-from .utils import cols, URL, ced
+from .utils import cols, TsetmcURL, tsetmc_ced
 
 
 class TSETMC:
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.url = URL()
+        self.url = TsetmcURL()
 
     def market_watch(self, **kwargs):
         main = get(self.url.mw(**kwargs)).json()["marketwatch"]
         df = pd.json_normalize(
             main, "blDs", list(cols.mw.rename.keys()), record_prefix="ob_"
         )
-        return ced.mw(df)
+        return tsetmc_ced.mw(df)
 
     def option_market_watch(self):
         # option df
         option = self.market_watch(option=True).drop(cols.omw.drop, axis=1)
         # underlying asset
         ua = self.market_watch(stock=True, etf=True).drop(cols.omw.drop, axis=1)
         ua = ua[(ua["ins_id"].str.endswith("1"))].add_prefix("ua_")
         ua = ua[ua.ua_quote.astype(int) == 1]
         ua.drop_duplicates(inplace=True)
         ua.drop(["ua_name_far"], axis=1, inplace=True)
         # marge option with ua df and clean and extend data
-        df = ced.omw(option=option, ua=ua)
+        df = tsetmc_ced.omw(option=option, ua=ua)
         return df.rename(columns=cols.omw.rename)
 
     def search_instrument_code(self, symbol_far: str):
         data = get(self.url.search_ins_code(symbol_far)).json()["instrumentSearch"]
         for i in data:
-            if (ced.arabic_char(i["lVal18AFC"]) == ced.arabic_char(symbol_far)) and (
+            if (tsetmc_ced.arabic_char(i["lVal18AFC"]) == tsetmc_ced.arabic_char(symbol_far)) and (
                 i["lastDate"] == 1
             ):
                 return i["insCode"]
 
     def instrument_info(self, ins_codes: list):
         """
         take instrument info
         :param ins_codes: list of instrument code
         :return: pandas data-frame
         """
         ins_info = []
         for ins_code in ins_codes:
             ins_info.append(
-                ced.ins_info(get(self.url.ins_info(ins_code)).json()["instrumentInfo"])
+                tsetmc_ced.ins_info(get(self.url.ins_info(ins_code)).json()["instrumentInfo"])
             )
         return pd.DataFrame.from_records(ins_info)
 
     def option_info(self):
         return self.instrument_info(
             self.market_watch(option=True)["instrument_code"].values
         )[cols.option_info.rep].rename(columns={"symbol": "ua"})
@@ -77,34 +77,34 @@
         :return: pandas data-frame
         """
 
         main = get(self.url.hist_price(ins_code)).json()["closingPriceDaily"]
         df = pd.DataFrame(main).rename(columns=cols.hist_price.rename)[
             cols.hist_price.rep
         ]
-        return ced.date(df)
+        return tsetmc_ced.date(df)
 
     def adj_hist_price(self, ins_code):
         """
         take adjusted price history.
         :param ins_code: int or str, instrument code.
         :return: pandas data-frame
         """
-        return ced.adj_price(self.hist_price(ins_code))
+        return tsetmc_ced.adj_price(self.hist_price(ins_code))
 
     def client_type(self, ins_code):
         """
         take Individual and Institutional trade data
         :param ins_code: int or str, instrument code.
         :return: pandas data-frame
         """
 
         main = get(self.url.client_type(ins_code)).json()["clientType"]
         df = pd.DataFrame(main)
         df = df.rename(columns=cols.client_type.rename)[cols.client_type.rep]
-        return ced.date(df).applymap(int)
+        return tsetmc_ced.date(df).applymap(int)
 
     @staticmethod
     def share_change(ins_code):
         url = (
             f"http://cdn.tsetmc.com/api/Instrument/GetInstrumentShareChange/{ins_code}"
         )
```

## mf_data/ise/utils/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .columns import cols
-from .constants import URL
-from .clean_and_extend_data import ced
+from .constants import TsetmcURL, RahavardURL
+from .clean_and_extend_data import tsetmc_ced, rahavard_ced
```

## mf_data/ise/utils/clean_and_extend_data.py

```diff
@@ -1,14 +1,16 @@
 import jdatetime
 from collections import namedtuple
 import re
+import json
 import pandas as pd
 from .columns import cols
 
-Ced = namedtuple("Ced", ["mw", "omw", "arabic_char", "ins_info", "date", "adj_price"])
+TsetmcCed = namedtuple("TsetmcCed", ["mw", "omw", "arabic_char", "ins_info", "date", "adj_price"])
+RahavardCed = namedtuple("RahavardCed", ["parser", "balance_sheet"])
 
 
 def mw(df):
     """
     :param df:
     :return:
     """
@@ -101,8 +103,19 @@
         "base_vol": instrument_info["baseVol"],
         "eps": instrument_info["eps"]["estimatedEPS"],
         "float_shares_pct": instrument_info["kAjCapValCpsIdx"],
         "contract_size": instrument_info["contractSize"],
     }
 
 
-ced = Ced(mw=mw, omw=omw, arabic_char=arabic_char, ins_info=ins_info, date=date, adj_price= adj_price)
+# ------------ Rahavard 356 -------------
+def rahavard_parser(t):
+    t = t.split("var layoutModel =")[1].split(";")[0].strip()
+    return json.loads(t)
+
+
+def balance_sheet(data: json):
+    df = pd.json_normalize(data)
+
+
+tsetmc_ced = TsetmcCed(mw=mw, omw=omw, arabic_char=arabic_char, ins_info=ins_info, date=date, adj_price=adj_price)
+rahavard_ced = RahavardCed(parser=rahavard_parser, balance_sheet=balance_sheet)
```

## mf_data/ise/utils/columns.py

```diff
@@ -1,12 +1,12 @@
 from collections import namedtuple
 
 
-Cols = namedtuple(
-    "Cols", ["mw", "mw_ob", "omw", "hist_price", "option_info", "client_type"]
+TsetmcCols = namedtuple(
+    "TsetmcCols", ["mw", "mw_ob", "omw", "hist_price", "option_info", "client_type"]
 )
 Property = namedtuple("Property", ["rename", "drop", "rep"])
 
 _mw = {
     "rename": {
         "insCode": "ins_code",
         "insID": "ins_id",
@@ -147,15 +147,15 @@
 )
 client_type = Property(
     rename=_client_type.get("rename"),
     drop=_client_type.get("drop"),
     rep=_client_type.get("rep"),
 )
 
-cols = Cols(
+cols = TsetmcCols(
     mw=mw,
     mw_ob=mw_ob,
     omw=omw,
     hist_price=hist_price,
     option_info=option_info,
     client_type=client_type,
 )
```

## mf_data/ise/utils/constants.py

```diff
@@ -1,25 +1,25 @@
 from urllib.parse import urlencode
 
 
-class URL:
+class TsetmcURL:
     def __init__(self, base_url="http://cdn.tsetmc.com/api/"):
         self.base_url = base_url
 
     def mw(
-        self,
-        stock: bool = False,
-        ifb_paye: bool = False,
-        mortgage: bool = False,
-        cum_right: bool = False,
-        bond: bool = False,
-        option: bool = False,
-        futures: bool = False,
-        etf: bool = False,
-        commodity: bool = False,
+            self,
+            stock: bool = False,
+            ifb_paye: bool = False,
+            mortgage: bool = False,
+            cum_right: bool = False,
+            bond: bool = False,
+            option: bool = False,
+            futures: bool = False,
+            etf: bool = False,
+            commodity: bool = False,
     ):
         """
         ترتیبَ ورودی‌ها مهم است، پس دقت کن!
         :param stock: bool, if True add stock data, default is False
         :param ifb_paye: bool, if True add ifb_pay data, default is False (فرابورس-پایه)
         :param mortgage: bool, if True add mortgage data, default is False
         :param cum_right: bool, if True add cum_right data, default is False
@@ -46,14 +46,15 @@
                 "etf": 8,
                 "commodity": 9,
             }
             return {
                 f"paperTypes[{i}]": paper_type_.get(k)
                 for i, k in enumerate(l_kwargs.keys())
             }
+
         param = {
             "market": 0,
             "industrialGroup": "",
             **paper_type(),
             "showTraded": "false",
             "withBestLimits": "true",
         }
@@ -69,7 +70,18 @@
         return f"{self.base_url}ClosingPrice/GetClosingPriceDailyList/{ins_code}/0"
 
     def client_type(self, ins_code):
         f"{self.base_url}ClientType/GetClientTypeHistory/{ins_code}"
 
     def share_change(self, ins_code):
         return f"{self.base_url}Instrument/GetInstrumentShareChange/{ins_code}"
+
+
+class RahavardURL:
+    def __init__(self):
+        self.base_url = "https://rahavard365.com/"
+
+    def stock(self):
+        return f"{self.base_url}stock"
+
+    def balance_sheet(self, symbol_id):
+        return f"{self.base_url}asset/{symbol_id}/balancesheet"
```

## mf_data/utils/get.py

```diff
@@ -1,9 +1,9 @@
 import requests
 
 headers = {
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
 }
 
 
-def get(url, timeout=(1, 2), verify=False):
+def get(url, timeout=(1, 3), verify=False):
     return requests.get(url, headers=headers, timeout=timeout, verify=verify)
```

## Comparing `metafid_data-0.1.0.dist-info/METADATA` & `metafid_data-0.1.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: metafid-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Yaghoub Ghadri
 Author-email: y.ghaderi@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jdatetime (>=4.1.1,<5.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # metafid
 
 ## install 
 ```bash
-python3 -m pip install mf-data
+python3 -m pip install metafid-data
 ```
 
 ## data
 ### ise (Iran Stock Exchange)
 #### TSETMC (tsetmc.com)
 ```python
 from mf_data.ise import TSETMC
```

## Comparing `metafid_data-0.1.0.dist-info/RECORD` & `metafid_data-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 mf_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mf_data/ise/__init__.py,sha256=m0SCvU84bfRZcmbE4LJKpS3dr6lKF52Ke8encoRGZVc,26
-mf_data/ise/tsetmc.py,sha256=I5Xbdot1TVofq3cWbWSIQDwChxrmAhADjDkmFKAfyvA,3701
-mf_data/ise/utils/__init__.py,sha256=vri0krxq9eq_tP_096O9-JOe3ptNCcEr1HyYZLAIZuk,92
-mf_data/ise/utils/clean_and_extend_data.py,sha256=Zj1JL6hBqkJdHKVOrXqmWGPVzzURBB_73UsjqzQ_qko,3626
-mf_data/ise/utils/columns.py,sha256=9jdSysgvTwiTH7rTUmKs_goJ4xf9p_PFKOX98Z93s00,3763
-mf_data/ise/utils/constants.py,sha256=VjaScaZK8brw1Y2FI0UQsM2YArIzjn8jR-lxGsqfNWA,2707
+mf_data/ise/rahavard.py,sha256=alfxnaawa3MaZkCVHcvfrFo7kTuHD8Sdowk-D67Kj00,723
+mf_data/ise/tsetmc.py,sha256=FE4i290efPZ5G09dEiwKpCB8GQjuWau177SCg40YvtI,3776
+mf_data/ise/utils/__init__.py,sha256=L24Q781XGf_ZiiCV0dqXNsWtjBjEo1XswPH9dXrgos4,132
+mf_data/ise/utils/clean_and_extend_data.py,sha256=col--kkVai7wODKoCuQ_cK_tpHmC6xVfbmVWfZh_s1A,4032
+mf_data/ise/utils/columns.py,sha256=63MkKbJDOReLs5XVwYhqgmIHa5OIrNEE7_q2U3W8w04,3781
+mf_data/ise/utils/constants.py,sha256=ko2bIcSXfiSMfwUxIlTu_vh3YFatMXIoXCW368Bkx6I,3016
 mf_data/tgju/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mf_data/tgju/tgju.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mf_data/utils/__init__.py,sha256=330lCAUgletamq5raTXT_T13HIW3ZwkLqpKWzTxeJV4,22
 mf_data/utils/async_.py,sha256=njUD2EBWlQRL5zC3vQ9N6qpR971itrdpAHz67B9bScM,992
-mf_data/utils/get.py,sha256=0RVTkHflpNRr0KmpAEilp7v1IapY0EShQ2FfMXhY6L8,278
-metafid_data-0.1.0.dist-info/METADATA,sha256=hTkrom5lkuAOWqQcZEz0Fol9Z00ktIMpQwV8Kd3O02c,833
-metafid_data-0.1.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-metafid_data-0.1.0.dist-info/RECORD,,
+mf_data/utils/get.py,sha256=mAWgtcIpEOa_EhzGbC--FTm4r-r9r-nDl7nEW8Tt3AE,278
+metafid_data-0.1.1.dist-info/METADATA,sha256=W_0CpjjLkG8nlDkFd4PLJVazgX7e3lGUhlUuNHbh-j0,838
+metafid_data-0.1.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+metafid_data-0.1.1.dist-info/RECORD,,
```

