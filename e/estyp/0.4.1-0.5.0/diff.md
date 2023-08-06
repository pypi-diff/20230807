# Comparing `tmp/estyp-0.4.1.tar.gz` & `tmp/estyp-0.5.0.tar.gz`

## Comparing `estyp-0.4.1.tar` & `estyp-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/__init__.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/linear_model/stepwise/__init__.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/linear_model/stepwise/__base/__init__.py
--rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/testing/__init__.py
--rw-r--r--   0        0        0    23090 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.4.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.4.1/LICENSE
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 estyp-0.4.1/README.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 estyp-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 estyp-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/__init__.py
+-rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/cluster/__init__.py
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/linear_model/stepwise/__init__.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/linear_model/stepwise/__base/__init__.py
+-rw-r--r--   0        0        0    26835 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/testing/__init__.py
+-rw-r--r--   0        0        0    31924 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 estyp-0.5.0/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 estyp-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 estyp-0.5.0/PKG-INFO
```

### Comparing `estyp-0.4.1/estyp/linear_model/__init__.py` & `estyp-0.5.0/estyp/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.1/estyp/linear_model/stepwise/__init__.py` & `estyp-0.5.0/estyp/linear_model/stepwise/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.1/estyp/linear_model/stepwise/__base/__init__.py` & `estyp-0.5.0/estyp/linear_model/stepwise/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.1/estyp/testing/__init__.py` & `estyp-0.5.0/estyp/testing/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from typing import List, Literal, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from pandas import Series
 from statsmodels.regression.linear_model import RegressionResultsWrapper
 
-from estyp.testing.__base import (TestResults, _CheckHomocedasticity,
-                                    _CheckIndependence,
-                                    _CheckMulticollinearity, _CheckNormality,
-                                    __nested_models_test, __prop_test, __t_test,
-                                    __var_test)
+from estyp.testing.__base import (
+    TestResults,
+    _CheckHomocedasticity,
+    _CheckIndependence,
+    _CheckMulticollinearity,
+    _CheckNormality,
+    __nested_models_test,
+    __prop_test,
+    __t_test,
+    __var_test,
+    __cor_test,
+    __chisq_test,
+)
+
 
 class CheckModel:
     """
     # Check Linear Regression Assumptions
 
     The `CheckModel` class provides methods to test the assumptions of the linear regression model.
     These assumptions are:
@@ -80,29 +89,29 @@
         pvals = normality.test(sign_level=alpha)
         if return_pvals:
             return pvals
 
     def check_homocedasticity(self, alpha=0.05, plot=True, return_pvals=False):
         """
         Checks the homoscedasticity assumption (equal variance of residuals) using several statistical tests.
-        
+
         Parameters
         ----------
         `alpha` : float, optional
             The significance level used by the statistical tests, by default 0.05.
         `plot` : bool, optional
             If `True`, a plot is shown for visual inspection of homoscedasticity, by default `True`.
         `return_pvals` : bool, optional
             If `True`, the p-values of the statistical tests are returned, by default `False`.
-        
+
         Returns
         -------
         dict
             A dictionary of p-values of the statistical tests if `return_pvals=True`.
-            
+
         Example
         -------
         >>> cm.check_homocedasticity()
         """
         homocedasticity = _CheckHomocedasticity(self.model)
         if plot:
             fig, ax = homocedasticity.plot()
@@ -110,29 +119,29 @@
         pvals = homocedasticity.test(sign_level=alpha)
         if return_pvals:
             return pvals
 
     def check_independence(self, alpha=0.05, plot=True, return_vals=False):
         """
         Checks the independence assumption of the residuals using several statistical tests.
-        
+
         Parameters
         ----------
         alpha : float, optional
             The significance level used by the statistical tests, by default 0.05.
         plot : bool, optional
             If `True`, a plot is shown for visual inspection of independence, by default `True`.
         return_pvals : bool, optional
             If `True`, the p-values of the statistical tests are returned, by default `False`.
-        
+
         Returns
         -------
         dict
             A dictionary of values of the statistical tests if `return_vals=True`.
-            
+
         Example
         -------
         >>> cm.check_independence()
         """
         independence = _CheckIndependence(self.model)
         if plot:
             fig, ax = independence.plot()
@@ -140,27 +149,27 @@
         vals = independence.test(sign_level=alpha)
         if return_vals:
             return vals
 
     def check_multicollinearity(self, plot=True, return_cm=False):
         """
         Checks the multicollinearity assumption among predictors using the variance inflation factor (VIF).
-        
+
         Parameters
         ----------
         `plot` : bool, optional
             If True, a plot is shown for visual inspection of multicollinearity, by default True.
         `return_cm` : bool, optional
             Returns the condition number of the model if True, by default False.
-            
+
         Returns
         -------
         float
             The condition number of the model if `return_cm=True`.
-        
+
         Example
         -------
         >>> cm.check_multicollinearity()
         """
         multicollinearity = _CheckMulticollinearity(self.model)
         if plot:
             fig, ax = multicollinearity.plot()
@@ -168,29 +177,29 @@
         pvals = multicollinearity.test()
         if return_cm:
             return pvals
 
     def check_all(self, alpha=0.05, plot=True, return_vals=False):
         """
         Checks all the assumptions of the linear regression model.
-        
+
         Parameters
         ----------
         `alpha` : float, optional
             The significance level used by the statistical tests, by default 0.05.
         `plot` : bool, optional
             If `True`, a plot is shown for visual inspection of each assumption, by default `True`.
         `return_vals` : bool, optional
             If `True`, the values of the statistical tests are returned, by default `False`.
-        
+
         Returns
         -------
         dict
             A dictionary of values of the statistical tests if `return_vals=True`.
-            
+
         Example
         -------
         >>> cm.check_all()
         """
         normality = _CheckNormality(self.model)
         homocedasticity = _CheckHomocedasticity(self.model)
         independence = _CheckIndependence(self.model)
@@ -222,15 +231,15 @@
         if return_vals:
             return dict(zip(names, tests))
 
 
 def var_test(
     x: Union[List, np.ndarray, Series],
     y: Union[List, np.ndarray, Series],
-    ratio: Union[float, int]=1,
+    ratio: Union[float, int] = 1,
     alternative: Literal["two-sided", "less", "greater"] = "two-sided",
     conf_level=0.95,
 ) -> TestResults:
     """
     # F Test to Compare Two Variances
     ## Description
     Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
@@ -504,7 +513,202 @@
     n = np.array([86, 93, 136, 82])
     result = prop_test(x, n)
     print(result)
     ```
     """
     return __prop_test(x, n, p, alternative, conf_level, correct)
 
+
+def cor_test(
+    x: Union[List, np.ndarray, Series],
+    y: Union[List, np.ndarray, Series],
+    method: Literal["pearson", "kendall", "spearman"] = "pearson",
+    alternative: Literal["two-sided", "less", "greater"] = "two-sided",
+    conf_level: float = 0.95,
+    continuity: bool = False,
+) -> TestResults:
+    """
+    # Test for Association/Correlation Between Paired Samples
+
+    Description
+    -----------
+    Test for association between paired samples, using one of Pearson's product moment correlation coefficient, Kendall's
+    tau or Spearman's rho.
+
+    Usage
+    -----
+    ```python
+    cor_test(x, y, ...)
+    cor_test(x, y, alternative="two-sided", method="pearson", conf_level=0.95, continuity=False)
+    ```
+
+    Arguments
+    ---------
+    `x`, `y` : array_like
+        Numeric one-dimensional `arrays`, `lists` or `pd.Series` of data values. `x` and `y` must have the same length.
+
+    `alternative` : str, optional
+        Indicates the alternative hypothesis and must be one of "two-sided", "greater" or "less".
+        "greater" corresponds to positive association, "less" to negative association.
+
+    `method` : str, optional
+        A string indicating which correlation coefficient is to be used for the test.
+        One of "pearson", "kendall", or "spearman".
+
+    `conf_level` : float, optional
+        Confidence level for the returned confidence interval. Currently only used for the
+        Pearson product moment correlation coefficient if there are at least 4 complete pairs of observations.
+
+    `continuity` : bool, optional
+        If `True`, a continuity correction is used for Kendall's tau.
+
+    Returns
+    -------
+    A `TestResults` instance containing the following atributes:
+        - `statistic`: the value of the test statistic.
+        - `df` (if applicable): the degrees of freedom of the test statistic.
+        - `p_value`: the p-value of the test.
+        - `estimate`: the estimated measure of association.
+        - `null_value`: the value of the association measure under the null hypothesis, always 0.
+        - `alternative`: a string describing the alternative hypothesis.
+        - `method`: a string indicating how the association was measured.
+        - `conf_int` (if applicable): a confidence interval for the measure of association.
+
+    Details
+    -------
+    The three methods each estimate the association between paired samples and compute a test of the value being zero.
+    They use different measures of association, all in the range [-1, 1] with 0 indicating no association.
+    These are sometimes referred to as tests of no correlation, but that term is often confined to the default method.
+
+    References
+    ----------
+    [1] D. J. Best & D. E. Roberts (1975). Algorithm AS 89: The Upper Tail Probabilities of Spearman's rho.
+        Applied Statistics, 24, 377--379. 10.2307/2347111.
+
+    [2] Myles Hollander & Douglas A. Wolfe (1973), Nonparametric Statistical Methods.
+        New York: John Wiley & Sons. Pages 185--194 (Kendall and Spearman tests).
+
+    Example
+    -------
+    Using the iris dataset to test the association between sepal length and petal length using Pearson's correlation:
+
+    ```python
+    from sklearn import datasets
+    iris = datasets.load_iris()
+
+    sepal_length = iris.data[:, 0]
+    petal_length = iris.data[:, 2]
+
+    result = cor_test(sepal_length, petal_length, method="pearson")
+    print(result)
+    """
+    return __cor_test(x, y, method, alternative, conf_level, continuity)
+
+
+def chisq_test(
+    x: Union[List, np.ndarray, Series],
+    y: Union[List, np.ndarray, Series, None] = None,
+    p: Union[List, np.ndarray, Series, None] = None,
+    correct: bool = True,
+    rescale_p: bool = False
+):
+    """
+# Pearson's Chi-squared Test for Count Data
+
+
+Description
+-----------
+`chisq_test()` performs chi-squared contingency table tests and goodness-of-fit tests.
+
+Usage
+------
+```python
+chisq_test(x, ...)
+chisq_test(x, y=None, correct=True, p=None, rescale_p=False)
+```
+
+Arguments
+---------
+`x`: arrat_like
+    A numeric list or 2D list (matrix). x and y can also both be lists.
+    
+`y`: array_like
+    A numeric data ; ignored if x is a matrix. If x is a list, y should be a list of the same length. The default is None.
+
+`p`: array_like
+    A list of probabilities of the same length as x. An error is raised if any entry of p is negative.
+
+`correct`: 
+    A boolean indicating whether to apply continuity correction when computing the test statistic for 2x2 tables: 
+    one half is subtracted from all |O-E| differences; however, the correction will not be bigger than the differences themselves. The default is True.
+
+`rescale_p`: boolean
+    A boolean; if True then p is rescaled (if necessary) to sum to 1. If rescale_p is False, and p does not sum to 1, an error is raised.
+
+Details
+-------
+    If x is a matrix with one row or column, or if x is a list and y is not given, then a goodness-of-fit test is performed 
+    (x is treated as a one-dimensional contingency table). The entries of x must be non-negative integers. In this case, the hypothesis 
+    tested is whether the population probabilities equal those in p, or are all equal if p is not given.
+
+    If x is a matrix with at least two rows and columns, it is taken as a two-dimensional contingency table: the entries of x must be 
+    non-negative integers. Otherwise, x and y must be lists of the same length; cases with None values are removed, the lists are 
+    treated as factors, and the contingency table is computed from these. Then Pearson's chi-squared test is performed of the null 
+    hypothesis that the joint distribution of the cell counts in a 2-dimensional contingency table is the product of the row and column marginals.
+
+    The p-value is computed from the asymptotic chi-squared distribution of the test statistic; continuity correction is only used in 
+    the 2-by-2 case (if correct is True, the default).
+
+Returns
+-------
+    A `TestResults` instance containing the following attributes:
+
+    `statistic`: 
+        The value of the chi-squared test statistic.
+
+    `df`: 
+        The degrees of freedom of the approximate chi-squared distribution of the test statistic.
+
+    `p_value`:
+        The p-value for the test.
+
+    `method`:
+        A string indicating the type of test performed, and whether continuity correction was used.
+
+    `expected`:
+        The expected counts under the null hypothesis.
+
+
+Examples
+--------
+```python
+## From Agresti(2007) p.39
+M = [[762, 327, 468], [484, 239, 477]]
+result1 = chisq_test(M)
+print(result1)
+
+## Effect of rescale_p
+x = [12, 5, 7, 7]
+p = [0.4, 0.4, 0.2, 0.2]
+result2 = chisq_test(x, p=p, rescale_p=True)
+print(result2)
+
+## Testing for population probabilities
+x = [20, 15, 25]
+result31 = chisq_test(x)
+print(result31)
+
+x = [89,37,30,28,2]
+p = [0.40,0.20,0.20,0.19,0.01]
+result32 = chisq_test(x, p=p)
+print(result32)
+
+
+# Goodness of fit
+x = [1, 2, 3, 4, 5, 6]
+y = [6, 1, 2, 3, 4, 5]
+result4 = chisq_test(x, y)
+print(result4)
+```
+    """
+
+    return __chisq_test(x, y, p, correct, rescale_p)
```

### Comparing `estyp-0.4.1/estyp/testing/__base/__init__.py` & `estyp-0.5.0/estyp/testing/__base/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import warnings
+
 import matplotlib.pyplot as plt
 import numpy as np
+import scipy.stats as stats
 import statsmodels.api as sm
-from pandas import DataFrame, Series
+from pandas import DataFrame, Series, crosstab
 from scipy.stats import chi2
 from scipy.stats import f as fisher
 from scipy.stats import (kstest, norm, probplot, shapiro, ttest_1samp,
                          ttest_ind, ttest_rel)
 from statsmodels.api import GLM, OLS
 from statsmodels.genmod.families.family import Gaussian
 from statsmodels.stats.diagnostic import (acorr_breusch_godfrey,
@@ -277,45 +280,51 @@
         # p-value
         p_value = self.p_value
         if p_value < 0.0001:
             p_value = "<0.0001"
         else:
             p_value = f"{p_value:0.4f}"
         # df
-        df = self.df
-        if isinstance(df, (float, int)):
-            if df == float(int(df)):
-                df = int(df)
-        elif isinstance(df, dict):
-            df = {k: f"{v:0.2f}" for k, v in df.items()}
-        elif isinstance(df, float):
-            df = f"{df:0.2f}"
+        if self.__dict__.get("df"):
+            df = self.df
+            if isinstance(df, (float, int)):
+                if df == float(int(df)):
+                    df = int(df)
+                else:
+                    df = f"{df:0.2f}"
+            elif isinstance(df, dict):
+                df = {k: round(v, 2) for k, v in df.items()}
+            elif isinstance(df, float):
+                df = f"{df:0.2f}"
+        else:
+            df = None
         # estimates
-        estimate = self.estimate
-        if isinstance(estimate, (list, np.ndarray)):
-            estimate = [float(f"{e:0.6f}") for e in estimate]
-        elif estimate == float(int(estimate)):
-            estimate = int(estimate)
-        elif isinstance(estimate, float):
-            estimate = f"{estimate:0.6f}"
+        if self.__dict__.get("estimate"):
+            estimate = self.estimate
+            if isinstance(estimate, (list, np.ndarray)):
+                estimate = [float(f"{e:0.6f}") for e in estimate]
+            elif estimate == float(int(estimate)):
+                estimate = int(estimate)
+            elif isinstance(estimate, float):
+                estimate = f"{estimate:0.6f}"
 
         string = f"""
-    {self.method}
-    {len(self.method) * "-"}
-    {self.__names['statistic']} = {self.statistic:0.4f} | df: {df} | p-value = {p_value}
+    {bcolors.BOLD + bcolors.UNDERLINE + self.method + bcolors.ENDC}
+    {self.__names['statistic']} = {self.statistic:0.4f} |{' df: ' + str(df) + ' |' if df is not None else ''} p-value = {p_value}
     alternative hypothesis: {self.__names["alternative"]}"""
         if self.__dict__.get("conf_int"):
             if self.conf_int is not None:
                 cl = self.conf_level * 100
                 if cl == float(int(cl)):
                     cl = int(cl)
                 string += f"""
-        {cl} percent confidence interval:
-        {" "}{self.conf_int[0]:0.6f} {self.conf_int[1]:0.6f}"""
-        string += f"""
+    {cl} percent confidence interval:
+    {" "}{self.conf_int[0]:0.6f} {self.conf_int[1]:0.6f}"""
+        if self.__dict__.get("estimate"):
+            string += f"""
     sample estimates:
     {" " * 2}{self.__names["estimate"]}: {estimate}
     """
         return string
 
 
 def __var_test(x, y, ratio, alternative, conf_level):
@@ -640,9 +649,247 @@
         "df": parameter,
         "p_value": p_value.item() if alternative != "two-sided" else p_value,
         "conf_int": conf_int,
         "null_value": p.item() if len(p.shape) != 0 and p.shape[0] == 1 else p,
         "conf_level": conf_level,
         "alternative": alternative,
     }
-    #return res
+    return TestResults(res, names)
+
+
+def __cor_test(x, y, method, alternative, conf_level, continuity):
+    
+    if not isinstance(x, (list, np.ndarray, Series)):
+        raise TypeError("'x' must be a list, numpy array, or pandas Series")
+    if isinstance(x, (Series, np.ndarray)):
+        if len(x.shape) != 1:
+            raise ValueError("'x' must be one-dimensional")
+    if isinstance(y, (Series, np.ndarray)):
+        if len(y.shape) != 1:
+            raise ValueError("'x' must be one-dimensional")
+    if len(x) != len(y):
+        raise ValueError("'x' and 'y' must have the same length")
+    
+    res = {
+        "conf_level": conf_level,
+        "alternative": alternative,
+        "null_value": 0
+    }
+
+    
+    direction = "not equal to" if alternative == "two-sided" else f"{alternative} than"
+    
+    n = len(x)
+    
+    if method == "pearson":
+        if n < 3:
+            raise ValueError("not enough finite observations")
+        
+        r = np.corrcoef(x, y)[0, 1]
+        df = n - 2
+        
+        t_statistic = np.sqrt(df) * r / np.sqrt(1 - r ** 2)
+        
+        # Confidence interval calculation following R's logic
+        if n > 3:
+            z = np.arctanh(r)
+            sigma = 1 / np.sqrt(n - 3)
+            
+            if alternative == "less":
+                lo_z, hi_z = -np.inf, z + sigma * stats.norm.ppf(conf_level)
+            elif alternative == "greater":
+                lo_z, hi_z = z - sigma * stats.norm.ppf(conf_level), np.inf
+            else:  # two-sided
+                z_crit = sigma * stats.norm.ppf((1 + conf_level) / 2)
+                lo_z, hi_z = z - z_crit, z + z_crit
+                
+            lo, hi = np.tanh((lo_z, hi_z))
+        else:
+            lo, hi = None, None
+        
+        # P-value
+        if alternative == "less":
+            p_value = stats.t.cdf(t_statistic, df)
+        elif alternative == "greater":
+            p_value = 1 - stats.t.cdf(t_statistic, df)
+        else:  # two-sided
+            p_value = 2 * min(stats.t.cdf(t_statistic, df), 1 - stats.t.cdf(t_statistic, df))
+        
+        
+        names = {
+            "statistic": "t",
+            "estimate": "cor",
+            "alternative": f"true correlation is {direction} 0"
+        }
+        
+        res.update({
+            "method": "Pearson's product-moment correlation",
+            "estimate": r,
+            "statistic": t_statistic,
+            "df": df,
+            "p_value": p_value,
+            "conf_int": (lo, hi)
+        })
+        
+        return TestResults(res, names)
+    
+    elif method == "spearman":
+        r, p_value = stats.spearmanr(x, y, alternative=alternative)
+        
+        # Calculate S statistic
+        S = (n ** 3 - n) * (1 - r)/6
+        
+        names = {
+            "statistic": "S",
+            "estimate": "rho",
+            "alternative": f"true rho is {direction} 0"
+        }
+        
+        res.update({
+            "method": "Spearman's rank correlation rho",
+            "estimate": r,
+            "statistic": S,
+            "p_value": p_value
+        })
+        
+        return TestResults(res, names)
+    
+    
+    elif method == "kendall":
+        tau, p_value = stats.kendalltau(x, y, alternative=alternative)
+        
+        xties = np.array([k for k in np.unique(x, return_counts=True)[1] if k > 1])
+        yties = np.array([k for k in np.unique(y, return_counts=True)[1] if k > 1])
+
+        T0 = n * (n - 1) / 2
+        T1 = sum(xties * (xties - 1)) / 2
+        T2 = sum(yties * (yties - 1)) / 2
+        S = tau * np.sqrt((T0 - T1) * (T0 - T2))
+        
+        v0 = n * (n - 1) * (2 * n + 5)
+        vt = sum(xties * (xties - 1) * (2 * xties + 5))
+        vu = sum(yties * (yties - 1) * (2 * yties + 5))
+        v1 = sum(xties * (xties - 1)) * sum(yties * (yties - 1))
+        v2 = sum(xties * (xties - 1) * (xties - 2)) * sum(yties * (yties - 1) * (yties - 2))
+        
+        var_S = (v0 - vt - vu) / 18 + v1 / (2 * n * (n - 1)) + v2 / (9 * n * (n - 1) * (n - 2))
+        
+        if continuity:
+            S = np.sign(S) * (np.abs(S) - 1)
+        
+        z_statistic = S / np.sqrt(var_S)
+        
+        names = {
+            "statistic": "z",
+            "estimate": "tau",
+            "alternative": f"true tau is {direction} 0"
+        }
+        
+        res.update({
+            "method": "Kendall's rank correlation tau",
+            "estimate": tau,
+            "statistic": z_statistic,
+            "p_value": p_value
+        })
+        
+        
+        return TestResults(res, names)
+
+    else:
+        raise ValueError("Invalid method")
+
+def __chisq_test(x, y, p, correct, rescale_p):
+        
+    names = {
+        "statistic": "X-squared",
+        "estimate": "expected frequencies",
+        "alternative": "true frequencies are not equal to expected frequencies"
+    }
+    
+    # Convert x to a numpy array if it's a list
+    if isinstance(x, list):
+        x = np.array(x)
+    if isinstance(x, Series):
+        x = x.values
+    
+    if not (isinstance(x, np.ndarray) and len(x.shape) == 2) and y is not None:
+        if len(x) != len(y):
+            raise ValueError("'x' and 'y' must have the same length")
+    # If x is a matrix
+    if isinstance(x, np.ndarray) and len(x.shape) == 2:
+        observed = x 
+    # If x and y are provided as vectors
+    elif y is not None:
+        observed = crosstab(np.array(x), np.array(y)).values
+    # If only x is provided (goodness-of-fit test)
+    elif y is None:
+        observed = np.array(x).reshape(-1)
+        method = "Chi-squared test for given probabilities"
+        if p is not None:
+            if rescale_p:
+                total_p = sum(p)
+                p = [prob/total_p for prob in p]
+            p = np.array(p)
+            if abs(p.sum() - 1) >= 1e-5:
+                raise ValueError("Elements of 'p' must sum to 1")
+            if np.any(p <= 0):
+                raise ValueError("Elements of 'p' must be positive")
+            expected = p * np.sum(observed)
+            chi2_statistic = np.sum((observed - expected)**2 / expected)
+            df = len(x) - 1
+            if np.any(expected < 5) and np.isfinite(df):
+                warnings.warn("Chi-squared approximation may be incorrect")
+            p_value = 1 - stats.chi2.cdf(chi2_statistic, df)
+            res = {
+                "method": method,
+                "statistic": chi2_statistic,
+                "df": df,
+                "expected": expected,
+                "p": p,
+                "p_value": p_value
+            }
+            
+            return TestResults(res, names)
+        else:
+            p = [1/len(x)] * len(x)
+            expected = np.array(p) * np.sum(observed)
+            chi2_statistic = np.sum((observed - expected)**2 / expected)
+            df = len(x) - 1
+            if np.any(expected < 5) and np.isfinite(df):
+                warnings.warn("Chi-squared approximation may be incorrect")
+            p_value = 1 - stats.chi2.cdf(chi2_statistic, df)
+            res = {
+                "method": method,
+                "statistic": chi2_statistic,
+                "df": df,
+                "expected": expected,
+                "p": p,
+                "p_value": p_value
+            }
+            
+            return TestResults(res, names)
+    else:
+        raise ValueError("Invalid input. Provide either a matrix or two vectors.")
+
+    n = np.sum(observed)
+    if observed.shape == (2, 2) and correct:
+        # Applying Yates' continuity correction for 2x2 table
+        expected = np.outer(np.sum(observed, axis=1), np.sum(observed, axis=0)) / n
+        chi2_statistic = np.sum((np.abs(observed - expected) - 0.5)**2 / expected)
+        add_correct = True
+    else:
+        add_correct = False
+        expected = np.outer(np.sum(observed, axis=1), np.sum(observed, axis=0)) / n
+        chi2_statistic = np.sum((observed - expected)**2 / expected)
+
+    df = (observed.shape[0] - 1) * (observed.shape[1] - 1)
+    p_value = 1 - stats.chi2.cdf(chi2_statistic, df)
+    
+    res = {
+        "method": "Pearson's Chi-squared test" + (" with Yates' continuity correction" if add_correct else ""),
+        "statistic": chi2_statistic,
+        "df": df,
+        "expected": expected,
+        "p_value": p_value
+    }
+    
     return TestResults(res, names)
```

### Comparing `estyp-0.4.1/.gitignore` & `estyp-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `estyp-0.4.1/LICENSE` & `estyp-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.4.1/README.md` & `estyp-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,19 +6,29 @@
 
 This library is a collection of statistical functions for Python.
 
 Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
 ## Changelog 
 
+### V0.5.0
+
+* Added `testing.chisq_test()` function to perform a chi-squared test.
+* Added `testing.cor_test()` function to perform a correlation test.
+* Added `cluster.NClusterSearch()` class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
+* Added `kmodes >= 0.12.2` as a depedency of the library.
+* Added `__version__` atribute to the library.
+* Changed method displaying in `TestResults` class.
+* Minor changes in README.
+
 ### V0.4.1
 
 * Bug fixes in `linear_model.LogisticRegression()` class.
 * Added downloads badge to README.
-* Changed `sklearn>=1.2.1` to `scipy>=1.3.0` as a depedency of the library.
+* Changed `sklearn>=1.2.1` to `sklearn>=1.3.0` as a depedency of the library.
 
 ### V0.4.0
 
 * Added `testing.prop_test()` function to perform a test of proportions.
 * Added `testing.CheckModel()` class to perform linear regression assumptions checking.
 * Added badges to README.
 * Minor changes in README.
@@ -37,23 +47,35 @@
 * Added `scipy>=1.11.1` as a depedency of the library.
 * New modularization of the functions in the `testing` module.
 * R like documentation in the `testing.var_test()` function.
 * Added `testing.t_test()` function to perform t-test like in software R.
 
 ## Features
 
-* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
-* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-* `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
+### `testing` module
+
 * `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
 * `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the R software.
 * `testing.prop_test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
+* `testing.chisq_test()`: Performs a chi-squared test of independence of variables in a contingency table. This function is inspired by the `chisq.test()` function of the R software.
+* `testing.cor_test()`: Performs a correlation test with Pearson, Spearman or Kendall method. This function is inspired by the `cor.test()` function of the R software.
 * `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
+### `linear_model` module
+
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
+* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
+* `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
+
+### `cluster` module
+
+* `cluster.NClusterSearch`: A helper class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
+
+
 ## Installation
 
 To install this library, you can use PyPI:
 
 ```bash
 pip install estyp
 ```
```

### Comparing `estyp-0.4.1/pyproject.toml` & `estyp-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.4.1"
+version = "0.5.0"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Extended Statistical Toolkit Yet Practical"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
@@ -19,13 +19,14 @@
 ]
 dependencies = [
     "numpy >= 1.22.3",
     "scikit-learn >= 1.3.0",
     "matplotlib >= 3.4.3",
     "patsy >= 0.5.3",
     "statsmodels >= 0.13.5",
-    "scipy >= 1.10.1"
+    "scipy >= 1.10.1",
+    "kmodes >= 0.12.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/estebanrucan/estyp"
 "Bug Tracker" = "https://github.com/estebanrucan/estyp/issues"
```

### Comparing `estyp-0.4.1/PKG-INFO` & `estyp-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.4.1
+Version: 0.5.0
 Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -27,14 +27,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9.12
+Requires-Dist: kmodes>=0.12.2
 Requires-Dist: matplotlib>=3.4.3
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: patsy>=0.5.3
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.5
 Description-Content-Type: text/markdown
@@ -47,19 +48,29 @@
 
 This library is a collection of statistical functions for Python.
 
 Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
 ## Changelog 
 
+### V0.5.0
+
+* Added `testing.chisq_test()` function to perform a chi-squared test.
+* Added `testing.cor_test()` function to perform a correlation test.
+* Added `cluster.NClusterSearch()` class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
+* Added `kmodes >= 0.12.2` as a depedency of the library.
+* Added `__version__` atribute to the library.
+* Changed method displaying in `TestResults` class.
+* Minor changes in README.
+
 ### V0.4.1
 
 * Bug fixes in `linear_model.LogisticRegression()` class.
 * Added downloads badge to README.
-* Changed `sklearn>=1.2.1` to `scipy>=1.3.0` as a depedency of the library.
+* Changed `sklearn>=1.2.1` to `sklearn>=1.3.0` as a depedency of the library.
 
 ### V0.4.0
 
 * Added `testing.prop_test()` function to perform a test of proportions.
 * Added `testing.CheckModel()` class to perform linear regression assumptions checking.
 * Added badges to README.
 * Minor changes in README.
@@ -78,23 +89,35 @@
 * Added `scipy>=1.11.1` as a depedency of the library.
 * New modularization of the functions in the `testing` module.
 * R like documentation in the `testing.var_test()` function.
 * Added `testing.t_test()` function to perform t-test like in software R.
 
 ## Features
 
-* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
-* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-* `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
+### `testing` module
+
 * `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
 * `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the R software.
 * `testing.prop_test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
+* `testing.chisq_test()`: Performs a chi-squared test of independence of variables in a contingency table. This function is inspired by the `chisq.test()` function of the R software.
+* `testing.cor_test()`: Performs a correlation test with Pearson, Spearman or Kendall method. This function is inspired by the `cor.test()` function of the R software.
 * `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
+### `linear_model` module
+
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
+* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
+* `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
+
+### `cluster` module
+
+* `cluster.NClusterSearch`: A helper class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
+
+
 ## Installation
 
 To install this library, you can use PyPI:
 
 ```bash
 pip install estyp
 ```
```

