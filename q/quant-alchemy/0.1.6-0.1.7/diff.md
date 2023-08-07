# Comparing `tmp/quant-alchemy-0.1.6.tar.gz` & `tmp/quant-alchemy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant-alchemy-0.1.6.tar", last modified: Tue Aug  1 23:48:46 2023, max compression
+gzip compressed data, was "dist\quant-alchemy-0.1.7.tar", last modified: Mon Aug  7 05:59:21 2023, max compression
```

## Comparing `quant-alchemy-0.1.6.tar` & `quant-alchemy-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 23:48:46.854793 quant-alchemy-0.1.6/
--rw-rw-rw-   0        0        0      400 2023-08-01 23:48:46.853798 quant-alchemy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 23:48:46.847797 quant-alchemy-0.1.6/quant_alchemy/
--rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.6/quant_alchemy/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.6/quant_alchemy/portfolio.py
--rw-rw-rw-   0        0        0    16021 2023-08-01 23:45:46.000000 quant-alchemy-0.1.6/quant_alchemy/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:48:46.852797 quant-alchemy-0.1.6/quant_alchemy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 23:48:46.854793 quant-alchemy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-08-01 23:48:35.000000 quant-alchemy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/
+-rw-rw-rw-   0        0        0      400 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-07-07 18:15:04.000000 quant-alchemy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy/
+-rw-rw-rw-   0        0        0       94 2023-07-26 18:55:52.000000 quant-alchemy-0.1.7/quant_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:18.000000 quant-alchemy-0.1.7/quant_alchemy/portfolio.py
+-rw-rw-rw-   0        0        0    18195 2023-08-07 05:48:46.000000 quant-alchemy-0.1.7/quant_alchemy/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/quant_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 05:59:21.000000 quant-alchemy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-08-07 05:59:12.000000 quant-alchemy-0.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `quant-alchemy-0.1.6/quant_alchemy/portfolio.py` & `quant-alchemy-0.1.7/quant_alchemy/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.6/quant_alchemy/timeseries.py` & `quant-alchemy-0.1.7/quant_alchemy/timeseries.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,40 @@
         Constructs all the necessary attributes for the Timeseries object.
 
         Parameters
         ----------
         prices : pandas.Series or pandas.DataFrame
             The time series data of prices.
         """
-        self.prices = prices.copy()
+
+        self.prices = self.handle_input_data( prices.copy())
+
+    def handle_input_data(self, prices):
+        """
+        This method handles the input data by converting it to a DataFrame.
+
+        Parameters:
+            prices (pandas.Series or pandas.DataFrame): The time series data of prices.
+
+        Returns:
+            pandas.DataFrame: The time series data of prices.
+        """
+        # If the input is a Series, convert it to a DataFrame
+        if isinstance(prices, pd.Series):
+            prices = pd.DataFrame(prices)
+        
+        # If is an array, convert it to a DataFrame
+        if isinstance(prices, np.ndarray):
+            prices = pd.DataFrame(prices)
+
+        # If is a list, convert it to a DataFrame
+        if isinstance(prices, list):
+            prices = pd.DataFrame(prices)
+
+        return prices
 
     def returns(self):
         """
         Calculate the simple returns of the time series data.
 
         Returns
         -------
@@ -154,86 +179,102 @@
         This method calculates and returns the maximum drawdown of the time series data.
         
         The drawdown is the percentage loss from the highest point to the lowest point.
         
         Returns:
             float: The maximum drawdown of the time series data.
         """
-        drawdown = self.drawdown()
+        drawdown = self.drawdowns()
         max_drawdowns = {}
 
         for col, df in drawdown.items():
             max_drawdowns[col] = df['Drawdown'].min()
 
         return pd.Series(max_drawdowns)
     
-    def drawdown(self):
+    def drawdowns(self):
         """
         This method calculates and returns a DataFrame containing the return series,
         cumulative return series, previous peak in the cumulative returns, 
         and the drawdown series.
 
         The drawdown is the percentage loss from the highest point to the lowest point.
 
         Returns:
             dict: A dictionary where the keys are column names and the values are DataFrames containing the return series, cumulative return series, previous peak in the cumulative returns, and the drawdown series.
         """
         return_series = self.returns()
         cumulative_returns = (1 + return_series).cumprod()
         running_max = cumulative_returns.cummax()
-        running_max.iloc[0] = 1.0
         drawdown = (cumulative_returns) / running_max - 1.0
 
         return {
             col: pd.DataFrame({
                 'Returns': return_series[col],
                 'Cumulative Returns': cumulative_returns[col],
                 'Running Max': running_max[col],
-                'Drawdown': drawdown[col]
+                'Drawdowns': drawdown[col]
             })
             for col in return_series.columns
         }
 
     def skewness(self):
         """
         This method calculates and returns the skewness of the returns of the time series data.
 
         Skewness is a measure of the asymmetry of the probability distribution.
 
         Returns:
-            float: The skewness of the returns of the time series data.
+            pd.Series: The skewness of the returns of the time series data.
         """
         returns = self.returns()
-        return skew(returns)
+
+        # For each column, calculate the skewness
+        pd_series = {}
+        for col in returns.columns:
+            pd_series[col] = skew(returns[col])
+
+        return pd.Series(pd_series)
     
     def kurtosis(self):
         """
         This method calculates and returns the kurtosis of the returns of the time series data.
 
         Kurtosis is a statistical measure that defines how heavily the tails of a distribution differ from the tails of a normal distribution.
 
         Returns:
-            float: The kurtosis of the returns of the time series data.
+            pd.Series: The kurtosis of the returns of the time series data.
         """
         returns = self.returns()
-        return kurtosis(returns)
+
+        # For each column, calculate the kurtosis
+        pd_series = {}
+        for col in returns.columns:
+            pd_series[col] = kurtosis(returns[col])
+
+        return pd.Series(pd_series)
     
     def is_normal(self, level=0.01):
         """
         This method applies the Jarque-Bera test to determine if the returns are normally distributed.
 
         The Jarque-Bera test is a goodness-of-fit test of whether sample data have the skewness and kurtosis matching a normal distribution.
 
         Returns:
-            bool: True if the p-value of the test is greater than the significance level indicating that
-                the returns could be from a normal distribution, False otherwise.
+            pd.Series: The result of the Jarque-Bera test for each time series.
         """
+
         returns = self.returns()
-        _, p_value = jarque_bera(returns)
-        return p_value > level
+        pd_series = {}
+        for col in returns.columns:
+            _, p_value = jarque_bera(returns[col])
+            pd_series[col] = p_value > level
+
+        return pd.Series(pd_series)
+
     
     def sharpe_ratio(self, period='daily', risk_free_rate=0.0, trading_days=252, hours_per_day=8):
         """
         This method calculates and returns the Sharpe ratio of the time series data.
 
         The Sharpe ratio is a measure of risk-adjusted return.
 
@@ -287,21 +328,26 @@
             level: (float, optional)
                 The percentile level at which to calculate VaR. This is the level below which the returns would fall with the given level of probability. Defaults to 5.
 
         Raises:
             ValueError: If the given level is not a valid percentile (i.e., not between 0 and 100).
 
         Returns:
-            float: The historic VaR at the specified level. This is the return value such that 'level' percent of returns fall below this number and (100 - level) percent of returns fall above this number.
+            pd.Series: The historic VaR at the specified level. This is the return value such that 'level' percent of returns fall below this number.
         """
         if not 0 <= level <= 100:
             raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
         
         returns = self.returns()
-        return np.percentile(returns, level)
+        pd_series = {}
+
+        for col in returns.columns:
+            pd_series[col] = np.percentile(returns[col], level)
+
+        return pd.Series(pd_series)
 
     def cvar_historic(self, level=5):
         """
         Calculates the historic Conditional Value at Risk (CVaR), also known as Expected Shortfall (ES),
         at a specified level. CVaR quantifies the expected value of loss given that a certain level of 
         loss threshold (VaR) has been exceeded.
 
@@ -310,46 +356,59 @@
                 The percentile level at which to calculate CVaR. This is the level below which the returns would 
                 fall with the given level of probability. Defaults to 5.
 
         Raises:
             ValueError: If the given level is not a valid percentile (i.e., not between 0 and 100).
 
         Returns:
-            float: The historic CVaR at the specified level. This is the average return value such that 'level' 
+            pd.Series: The historic CVaR at the specified level. This is the average return value such that 'level' 
                 percent of returns fall below this number.
         """
         if not 0 <= level <= 100:
             raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
         
         returns = self.returns()
-        var = np.percentile(returns, level)
-        return returns[returns <= var].mean()
+
+        pd_series = {}
+        for col in returns.columns:
+            is_beyond = returns[col] <= -self.var_historic(level=level)[col]
+            pd_series[col] = returns[col][is_beyond].mean()
+
+        return pd.Series(pd_series)
 
     def var_gaussian(self, level=5):
         """
         Calculates the Gaussian Value at Risk (VaR) at a specified level.
 
         Parameters:
             level: (float, optional)
                 The percentile level at which to calculate VaR. This is the level below which the returns would 
                 fall with the given level of probability. Defaults to 5.
 
         Raises:
             ValueError: If the given level is not a valid percentile (i.e., not between 0 and 100).
 
         Returns:
-            float: The Gaussian VaR at the specified level. This is the return value such that 'level' percent of 
+            pd.Series: The Gaussian VaR at the specified level. This is the return value such that 'level' percent of 
                     returns fall below this number, assuming returns follow a Gaussian distribution.
         """
         if not 0 <= level <= 100:
             raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
         
         returns = self.returns()
-        return -norm.ppf(level/100, loc=returns.mean(), scale=returns.std(ddof=1))
-    
+        pd_series = {}
+
+        for col in returns.columns:
+            z = norm.ppf(level / 100)
+            mean = returns[col].mean()
+            var = returns[col].std(ddof=1)
+            pd_series[col] = mean + z * var
+
+        return pd.Series(pd_series)
+        
     def calculate_monthly_compound_return(self):
         """
         Calculates the monthly compounded return based on the closing prices.
 
         Parameters:
             df (pd.DataFrame): DataFrame with Date as the index and OHLC columns.
 
@@ -371,15 +430,29 @@
 
         result = {}
 
         returns = self.returns()
         returns["Year"] = returns.index.year
         returns["Month"] = returns.index.month
 
-        for col in returns.columns:
-            compound_return = returns.groupby(["Year", "Month"])["Close"].apply(calculate_compound_return).reset_index()
+        # -2 because we don't want to include the Year and Month columns
+        for col in returns.columns[:-2]:
+            compound_return = returns.groupby(["Year", "Month"])[col].apply(calculate_compound_return).reset_index()
             compound_return.columns = ["Year", "Month", "Compound Return"]
 
             result[col] = compound_return
 
         return result
+    
+    def correlation(self, use_log_returns=False):
+        """
+        Calculates the correlation between the returns of the time series data.
 
+        Parameters:
+            use_log_returns (bool, optional): 
+                If True, the correlation between the log returns is calculated.
+
+        Returns:
+            float: The correlation between the returns of the time series data.
+        """
+        returns = self.log_returns() if use_log_returns else self.returns()
+        return returns.corr()
```

### Comparing `quant-alchemy-0.1.6/setup.py` & `quant-alchemy-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="quant-alchemy",
-    version="0.1.6",
+    version="0.1.7",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="Package for quantitative finance.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/quant-alchemy",
     project_urls={
```

