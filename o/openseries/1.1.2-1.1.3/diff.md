# Comparing `tmp/openseries-1.1.2-py3-none-any.whl.zip` & `tmp/openseries-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 54640 bytes, number of entries: 15
+Zip file size: 54431 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 openseries/__init__.py
 -rw-r--r--  2.0 unx    10224 b- defN 80-Jan-01 00:00 openseries/datefixer.py
--rw-r--r--  2.0 unx   115475 b- defN 80-Jan-01 00:00 openseries/frame.py
+-rw-r--r--  2.0 unx   115855 b- defN 80-Jan-01 00:00 openseries/frame.py
 -rw-r--r--  2.0 unx     1180 b- defN 80-Jan-01 00:00 openseries/load_plotly.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 openseries/plotly_captor_logo.json
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 openseries/plotly_layouts.json
--rw-r--r--  2.0 unx     4275 b- defN 80-Jan-01 00:00 openseries/risk.py
--rw-r--r--  2.0 unx    84635 b- defN 80-Jan-01 00:00 openseries/series.py
--rw-r--r--  2.0 unx    15567 b- defN 80-Jan-01 00:00 openseries/sim_price.py
--rw-r--r--  2.0 unx    14719 b- defN 80-Jan-01 00:00 openseries/stoch_processes.py
--rw-r--r--  2.0 unx     7082 b- defN 80-Jan-01 00:00 openseries/types.py
--rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.1.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    47925 b- defN 80-Jan-01 00:00 openseries-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1201 b- defN 16-Jan-01 00:00 openseries-1.1.2.dist-info/RECORD
-15 files, 305499 bytes uncompressed, 52680 bytes compressed:  82.8%
+-rw-r--r--  2.0 unx     4456 b- defN 80-Jan-01 00:00 openseries/risk.py
+-rw-r--r--  2.0 unx    84732 b- defN 80-Jan-01 00:00 openseries/series.py
+-rw-r--r--  2.0 unx    37004 b- defN 80-Jan-01 00:00 openseries/simulation.py
+-rw-r--r--  2.0 unx     5128 b- defN 80-Jan-01 00:00 openseries/types.py
+-rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.1.3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    47610 b- defN 80-Jan-01 00:00 openseries-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1115 b- defN 16-Jan-01 00:00 openseries-1.1.3.dist-info/RECORD
+14 files, 310520 bytes uncompressed, 52603 bytes compressed:  83.1%
```

## zipnote {}

```diff
@@ -18,29 +18,26 @@
 
 Filename: openseries/risk.py
 Comment: 
 
 Filename: openseries/series.py
 Comment: 
 
-Filename: openseries/sim_price.py
-Comment: 
-
-Filename: openseries/stoch_processes.py
+Filename: openseries/simulation.py
 Comment: 
 
 Filename: openseries/types.py
 Comment: 
 
-Filename: openseries-1.1.2.dist-info/LICENSE.md
+Filename: openseries-1.1.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: openseries-1.1.2.dist-info/METADATA
+Filename: openseries-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: openseries-1.1.2.dist-info/WHEEL
+Filename: openseries-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: openseries-1.1.2.dist-info/RECORD
+Filename: openseries-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openseries/frame.py

```diff
@@ -1269,39 +1269,42 @@
         )
 
     def max_drawdown_func(
         self: "OpenFrame",
         months_from_last: Optional[int] = None,
         from_date: Optional[dt.date] = None,
         to_date: Optional[dt.date] = None,
+        min_periods: int = 1,
     ) -> Series:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
             Specific to date
+        min_periods: int, default: 1
+            Smallest number of observations to use to find the maximum drawdown
 
         Returns
         -------
         Pandas.Series
             Maximum drawdown without any limit on date range
         """
 
         earlier, later = self.calc_range(months_from_last, from_date, to_date)
         return Series(
             data=(
                 self.tsdf.loc[cast(int, earlier) : cast(int, later)]
                 / self.tsdf.loc[cast(int, earlier) : cast(int, later)]
-                .expanding(min_periods=1)
+                .expanding(min_periods=min_periods)
                 .max()
             ).min()
             - 1,
             name="Subset Max drawdown",
             dtype="float64",
         )
 
@@ -2028,28 +2031,34 @@
             An OpenFrame object
         """
 
         for serie in self.tsdf:
             self.tsdf.loc[:, serie] = drawdown_series(self.tsdf.loc[:, serie])
         return self
 
-    def drawdown_details(self: "OpenFrame") -> DataFrame:
-        """
+    def drawdown_details(self: "OpenFrame", min_periods: int = 1) -> DataFrame:
+        """Calculates 'Max Drawdown', 'Start of drawdown', 'Date of bottom',
+        'Days from start to bottom', & 'Average fall per day'
+
+        Parameters
+        ----------
+        min_periods: int, default: 1
+            Smallest number of observations to use to find the maximum drawdown
+
         Returns
         -------
         Pandas.DataFrame
-            Calculates 'Max Drawdown', 'Start of drawdown', 'Date of bottom',
-            'Days from start to bottom', & 'Average fall per day'
+            Drawdown details
         """
 
         mxdwndf = DataFrame()
         for i in self.constituents:
             tmpdf = i.tsdf.copy()
             tmpdf.index = DatetimeIndex(tmpdf.index)
-            ddown = drawdown_details(tmpdf)
+            ddown = drawdown_details(prices=tmpdf, min_periods=min_periods)
             ddown.name = i.label
             mxdwndf = concat([mxdwndf, ddown], axis="columns")
         return mxdwndf
 
     def ewma_risk(
         self: "OpenFrame",
         lmbda: float = 0.94,
```

## openseries/risk.py

```diff
@@ -102,35 +102,41 @@
     drawdown = drawdown.fillna(method="ffill")
     drawdown[isnan(drawdown)] = -Inf
     roll_max = maximum.accumulate(drawdown)
     drawdown = drawdown / roll_max - 1.0
     return drawdown
 
 
-def drawdown_details(prices: Union[DataFrame, Series]) -> Series:
+def drawdown_details(prices: Union[DataFrame, Series], min_periods: int = 1) -> Series:
     """Details of the maximum drawdown
 
     Parameters
     ----------
     prices: DataFrame | Series
         A timeserie of dates and values
+    min_periods: int, default: 1
+        Smallest number of observations to use to find the maximum drawdown
 
     Returns
     -------
     Series
         Max Drawdown
         Start of drawdown
         Date of bottom
         Days from start to bottom
         Average fall per day
     """
 
-    mdd_date = (prices / prices.expanding(min_periods=1).max()).idxmin().values[0]
+    mdd_date = (
+        (prices / prices.expanding(min_periods=min_periods).max()).idxmin().values[0]
+    )
     mdate = dt.datetime.strptime(str(mdd_date)[:10], "%Y-%m-%d").date()
-    maxdown = ((prices / prices.expanding(min_periods=1).max()).min() - 1).iloc[0]
+    maxdown = (
+        (prices / prices.expanding(min_periods=min_periods).max()).min() - 1
+    ).iloc[0]
     ddata = prices.copy()
     drwdwn = drawdown_series(ddata).loc[: cast(int, mdate)]
     drwdwn.sort_index(ascending=False, inplace=True)
     sdate = drwdwn[drwdwn == 0.0].idxmax().values[0]
     sdate = dt.datetime.strptime(str(sdate)[:10], "%Y-%m-%d").date()
     duration = (mdate - sdate).days
     ret_per_day = maxdown / duration
```

## openseries/series.py

```diff
@@ -284,15 +284,15 @@
         valuetype : ValueType, default: ValueType.PRICE
             Identifies if the series is a series of values or returns
         timeseries_id : str
             Database identifier of the timeseries
         instrument_id: str
             Database identifier of the instrument associated with the timeseries
         baseccy : str, default: "SEK"
-            The currency of the timeseries
+            ISO 4217 currency code of the timeseries
         local_ccy: bool, default: True
             Boolean flag indicating if timeseries is in local currency
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
@@ -332,15 +332,15 @@
         dframe: DataFrame | Series
             Pandas DataFrame or Series
         column_nmbr : int, default: 0
             Using iloc[:, column_nmbr] to pick column
         valuetype : ValueType, default: ValueType.PRICE
             Identifies if the series is a series of values or returns
         baseccy : str, default: "SEK"
-            The currency of the timeseries
+            ISO 4217 currency code of the timeseries
         local_ccy: bool, default: True
             Boolean flag indicating if timeseries is in local currency
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
@@ -1304,41 +1304,43 @@
         return dt.datetime.strptime(str(mdd_date)[:10], "%Y-%m-%d").date()
 
     def max_drawdown_func(
         self: "OpenTimeSeries",
         months_from_last: Optional[int] = None,
         from_date: Optional[dt.date] = None,
         to_date: Optional[dt.date] = None,
+        min_periods: int = 1,
     ) -> float:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
             Specific to date
+        min_periods: int, default: 1
 
         Returns
         -------
         float
             Maximum drawdown without any limit on date range
         """
 
         earlier, later = self.calc_range(months_from_last, from_date, to_date)
         return cast(
             float,
             (
                 (
                     self.tsdf.loc[cast(int, earlier) : cast(int, later)]
                     / self.tsdf.loc[cast(int, earlier) : cast(int, later)]
-                    .expanding(min_periods=1)
+                    .expanding(min_periods=min_periods)
                     .max()
                 ).min()
                 - 1
             ).iloc[0],
         )
 
     @property
```

## openseries/types.py

```diff
@@ -1,12 +1,12 @@
 """
 Declaring types used throughout the project
 """
 from typing import Literal, List, Union
-from pydantic import BaseModel, conlist, constr
+from pydantic import conlist, constr
 
 
 CountryStringType = constr(
     pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
 )
 CountriesType = Union[conlist(CountryStringType, min_length=1), CountryStringType]
 
@@ -198,67 +198,7 @@
             if item not in self.allowed_strings:
                 raise ValueError(
                     f"Invalid string: {item}. Allowed strings: {self.allowed_strings}"
                 )
             if item in seen:
                 raise ValueError(f"Duplicate string: {item}")
             seen.add(item)
-
-
-class ModelParameters(BaseModel):
-    """Object of the class ModelParameters. Subclass of the Pydantic BaseModel
-
-    Parameters
-    ----------
-    all_s0: float
-        Starting asset value
-    all_time: float
-        Amount of time to simulate for
-    all_delta: float
-        Delta, the rate of time e.g. 1/252 = daily, 1/12 = monthly
-    all_sigma: float
-        Volatility of the stochastic processes
-    all_r0: float, default: 0.0
-        Starting interest rate value
-    gbm_mu: float
-        Annual drift factor for geometric brownian motion
-    jumps_lamda: float, default: 0.0
-        Probability of a jump happening at each point in time
-    jumps_sigma: float, default: 0.0
-        Volatility of the jump size
-    jumps_mu: float, default: 0.0
-        Average jump size
-    cir_a: float, default: 0.0
-        Rate of mean reversion for Cox Ingersoll Ross
-    cir_mu: float, default: 0.0
-        Long run average interest rate for Cox Ingersoll Ross
-    cir_rho: float, default: 0.0
-        Correlation between the wiener processes of the Heston model
-    ou_a: float, default: 0.0
-        Rate of mean reversion for Ornstein Uhlenbeck
-    ou_mu: float, default: 0.0
-        Long run average interest rate for Ornstein Uhlenbeck
-    heston_a: float, default: 0.0
-        Rate of mean reversion for volatility in the Heston model
-    heston_mu: float, default: 0.0
-        Long run average volatility for the Heston model
-    heston_vol0: float, default: 0.0
-        Starting volatility value for the Heston vol model
-    """
-
-    all_s0: float
-    all_time: int
-    all_delta: float
-    all_sigma: float
-    gbm_mu: float
-    jumps_lamda: float = 0.0
-    jumps_sigma: float = 0.0
-    jumps_mu: float = 0.0
-    cir_a: float = 0.0
-    cir_mu: float = 0.0
-    all_r0: float = 0.0
-    cir_rho: float = 0.0
-    ou_a: float = 0.0
-    ou_mu: float = 0.0
-    heston_a: float = 0.0
-    heston_mu: float = 0.0
-    heston_vol0: float = 0.0
```

## Comparing `openseries-1.1.2.dist-info/LICENSE.md` & `openseries-1.1.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `openseries-1.1.2.dist-info/METADATA` & `openseries-1.1.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package for simple financial time series analysis.
 Home-page: https://github.com/CaptorAB/OpenSeries
 License: BSD-3-Clause
 Keywords: python,python3,plotly,pandas,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.9,<3.12
@@ -200,16 +200,15 @@
 | [series.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py)                             | Defines the class _OpenTimeSeries_ for managing and analyzing a single timeseries. The module also defines a function `timeseries_chain` that can be used to chain two timeseries objects together. |
 | [frame.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py)                               | Defines the class _OpenFrame_ for managing a group of timeseries, and e.g. calculate a portfolio timeseries from a rebalancing strategy between timeseries.                                         |
 | [datefixer.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/datefixer.py)                       | Date utilities. Please read the docstring of each function for its description.                                                                                                                     |
 | [load_plotly.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/load_plotly.py)                   | Functions to load [Plotly](https://plotly.com/python/) default layout and configuration from local json file.                                                                                       |
 | [plotly_layouts.json](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/plotly_layouts.json)         | [Plotly](https://plotly.com/python/) defaults used in the `plot_bars` and `plot_series` methods.                                                                                                    |
 | [plotly_captor_logo.json](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/plotly_captor_logo.json) | JSON with a link to the Captor logo used in the `plot_bars` and `plot_series` methods.                                                                                                              |
 | [risk.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/risk.py)                                 | Functions used to calculate VaR, CVaR and drawdowns.                                                                                                                                                |
-| [sim_price.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/sim_price.py)                       | Simulates OpenTimeSeries from different stochastic processes.                                                                                                                                       |
-| [stoch_processes.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/stoch_processes.py)           | Generates stochastic processes used in the `sim_price.py` module.                                                                                                                                   |
+| [simulation.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/simulation.py)                     | Simulates OpenTimeSeries from different stochastic processes.                                                                                                                                       |
 | [types.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/types.py)                               | Contains all bespoke typing.                                                                                                                                                                        |
 
 ### Class methods used to construct objects.
 
 | Method            | Applies to                    | Description                                                                                        |
 |:------------------|:------------------------------|:---------------------------------------------------------------------------------------------------|
 | `from_arrays`     | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a list of date strings and a list of values.  |
```

## Comparing `openseries-1.1.2.dist-info/RECORD` & `openseries-1.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 openseries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openseries/datefixer.py,sha256=oNDIIQgm2vYxLIVS2kow1SMPn1KcZTjgwgVJfPcccTU,10224
-openseries/frame.py,sha256=x3qMiYUhQ3CRhlUo3QOF-WbL0bmdM_B7s6qjcfqoONA,115475
+openseries/frame.py,sha256=BeXEiQhERTkOiv1PnXG1igfyNskAeuDdtoqjuQqnJ9c,115855
 openseries/load_plotly.py,sha256=DSeLRNjMAlLYrYjD7zXCcKr0ilJLrmUqpPyqywqbbbU,1180
 openseries/plotly_captor_logo.json,sha256=pGMuPVu4cEO3ZsCH1wU03hxqbIQkHFNoJUs1k1WK89Y,178
 openseries/plotly_layouts.json,sha256=xhrMOqW8LXb4QMtPiNBGdkPX518OHThiIJ68jpQk524,1429
-openseries/risk.py,sha256=1BD3edR1Xmgd9dT21Vsb1NjV2nCSTd41-H2eomzsJoQ,4275
-openseries/series.py,sha256=p2aOhYx4tSmNmLwZd1A1bIa7AB16XcKyhlO7za1dkTw,84635
-openseries/sim_price.py,sha256=KbTVe3B_d_Bl4-qtBkKK1a1AxuUbyiMB3oJxcSAwU8U,15567
-openseries/stoch_processes.py,sha256=0s8W-jPaUMkRau7InmSkRgqyoKIbvL4CgoJajPJoQ30,14719
-openseries/types.py,sha256=gK7drITAZu-tvosEIlojqMs5WmT8I81hs9wOf2F_Zk8,7082
-openseries-1.1.2.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
-openseries-1.1.2.dist-info/METADATA,sha256=QUBcEaDPsfQyr5U8_4ucT3CeiFBcIO_wk4lbQgFFGRQ,47925
-openseries-1.1.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-openseries-1.1.2.dist-info/RECORD,,
+openseries/risk.py,sha256=T678SgRCuxKh49pF38DlivtQfXjG1NZ8fR2ff5PrLZw,4456
+openseries/series.py,sha256=zghPVcZPhJoU1N5sjtyJeqmDXT4Nkw51YK7l8GbMJNo,84732
+openseries/simulation.py,sha256=tpaa4ThBDiMgH9eNlHX48xIIBlix9Ueq59f2XiXvBas,37004
+openseries/types.py,sha256=lOWwTcwUjEPAjsNLeNIRMwm8yLaEi-U_ttB3mlMqAKI,5128
+openseries-1.1.3.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
+openseries-1.1.3.dist-info/METADATA,sha256=zY4oDfb-8o_OzfQw1HYGsP4x3JPD52_WKp8WH3pv9b8,47610
+openseries-1.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+openseries-1.1.3.dist-info/RECORD,,
```

