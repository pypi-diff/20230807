# Comparing `tmp/envisionriskraas-1.1.6.tar.gz` & `tmp/envisionriskraas-1.1.7.tar.gz`

## Comparing `envisionriskraas-1.1.6.tar` & `envisionriskraas-1.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0    86306 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/src/EnvisionRiskRaaS/core.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/LICENSE.txt
--rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 envisionriskraas-1.1.7/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0    89884 2020-02-02 00:00:00.000000 envisionriskraas-1.1.7/src/EnvisionRiskRaaS/core.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     8894 2020-02-02 00:00:00.000000 envisionriskraas-1.1.7/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 envisionriskraas-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9876 2020-02-02 00:00:00.000000 envisionriskraas-1.1.7/PKG-INFO
```

### Comparing `envisionriskraas-1.1.6/src/EnvisionRiskRaaS/core.py` & `envisionriskraas-1.1.7/src/EnvisionRiskRaaS/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1931,7 +1931,96 @@
                 },
                 "UnMappedSymbols": pd.DataFrame(out_raw["Output"]["UnmappedSymbols"])
             }
         else:
             return res_out
 
         return out
+
+
+def envrsk_decorate_portfolio_with_product_type(positions, simplify=True):
+    """
+    Function to enrich portfolio position data with additional information based on position ID.
+    
+    Parameters:
+    positions (pd.DataFrame): A list of positions to be enriched with additional information.
+    simplify (bool, optional): Logical, indicating whether to simplify the output.
+    
+    Returns:
+    pd.DataFrame or requests.Response: If the API call is successful, a dataframe containing the
+    enriched positions is returned. If the API call is unsuccessful,
+    the original API response is returned.
+    
+    Examples:
+    dt_positions_without_product_type = pd.DataFrame({
+    "symbol": ["AAPL.US", "DANSKE.CO", "CashUSD", "AGG.US"],
+    "quantity": [129, 768, 69000, 89]
+    })
+    dt_positions = envrsk_decorate_portfolio_with_product_type(positions=dt_positions_without_product_type)
+    """
+    if os.getenv("LOGGED_IN") != 'Yes':
+        return {"message": "Please login before using the functionality - use 'envrsk_auth_log_in()' or 'envrsk_auth_log_in_interactively()'"}
+    else:
+        end_point = "decorate-position-id"
+        api_url = get_api_url(end_point)
+        params = {
+            "simplify": simplify
+            }
+    
+        # Remove None values from params
+        params = {k: v for k, v in params.items() if v is not None}
+        positions_dict = pd.DataFrame(positions).to_dict('list')
+        res_out = envrsk_post(url=api_url, access_token=get_access_token(), params=params, body=positions_dict)
+    
+        if res_out["status_code"] == 200:
+            out = res_out["content"]
+    
+            if simplify:
+                return out["Output"]
+            else:
+                return out
+        else:
+            return res_out
+
+def envrsk_decorate_portfolio_with_uid(positions, simplify=True):
+    """
+    Uses the envrsk API to decorate a given portfolio with the respective ID.
+    
+    Parameters:
+    positions (pd.DataFrame): A list of positions to be enriched with additional information.
+    simplify (bool, optional): Logical, indicating whether to simplify the output.
+    
+    Returns:
+    pd.DataFrame or requests.Response: If the API call is successful, a dataframe containing the
+    enriched positions is returned. If the API call is unsuccessful,
+    the original API response is returned.
+    
+    Examples:
+    dt_positions_without_ids = pd.DataFrame({
+    "symbol": ["AAPL.US", "DANSKE.CO", "CashUSD", "AGG.US"],
+    "quantity": [129, 768, 69000, 89]
+    })
+    dt_positions = envrsk_decorate_portfolio_with_uid(positions=dt_positions_without_ids)
+    """
+    if os.getenv("LOGGED_IN") != 'Yes':
+        return {"message": "Please login before using the functionality - use 'envrsk_auth_log_in()' or 'envrsk_auth_log_in_interactively()'"}
+    else:
+        end_point = "decorate-table-id"
+        api_url = get_api_url(end_point)
+        params = {
+            "simplify": simplify
+            }
+    
+        # Remove None values from params
+        params = {k: v for k, v in params.items() if v is not None}
+        positions_dict = pd.DataFrame(positions).to_dict('list')
+        res_out = envrsk_post(url=api_url, access_token=get_access_token(), params=params, body=positions_dict)
+    
+        if res_out["status_code"] == 200:
+            out = res_out["content"]
+    
+            if simplify:
+                return out["Output"]
+            else:
+                return out
+        else:
+            return res_out
```

### Comparing `envisionriskraas-1.1.6/LICENSE.txt` & `envisionriskraas-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.6/README.md` & `envisionriskraas-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,40 +39,42 @@
 
 - <b>Stress Testing:</b> Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
 
 ```
 #Libraries
+#Libraries
 import EnvisionRiskRaaS as RaaS
 from datetime import date
 import matplotlib.pyplot as plt
 from scipy import stats
 import pandas as pd
 import numpy as np
 import queuelib
+import seaborn as sns
 
 #EnvisionRisk login
 RaaS.envrsk_auth_log_in("your username/email here", "your password here")
 
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
 # the stock. This implies that the analysis maintains the original currency 
 # perspective of the stock, allowing for more accurate and relevant 
 # insights. It enhances ease of comprehension and direct applicability, 
 # bringing us closer to the context of the actual trading environment.
 use_date = date.today()
 use_symbol = "AAPL.US"
-api_response = RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol)
+api_response = RaaS.envrsk_instrument_delta_vector_raw(use_date,use_symbol)
 
 # Leverage our sophisticated API to conduct an Expected-Shortfall computation, 
 # specified at a 97.5% confidence level across a single-day span, utilizing a 
 # point-in-time volatility scenario.
-api_response_es = RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols = use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
+api_response_es = RaaS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols = use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"][0]
 
 #manipulate the data for the density function
 data = api_response["Output"]["PnL"]
 
 #titles and captions
 subtitle = "Profit/Loss distribution (one day) for " + use_symbol + " as seen from the " + str(use_date)
@@ -85,15 +87,14 @@
 plt.axvline(x = expected_shortfall_estimate, color = "#57575F", label = 'axvline - full height')
 plt.text(expected_shortfall_estimate, 300, 'Expected-Shortfall (97.5%, 1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
 plt.xlabel("Profit/Loss (in $)")
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(5,-120, caption, ha='center', size=7)
 plt.show()
-
 ```
 
 <img height='600' style='border:0px;height:600px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
 
 <h2>API documentation</h2>
 <hr>
 You can locate our extensive API documentation <a href="https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/9ed9f79a31a4a-market-risk-as-a-service-api">here</a>. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
```

#### html2text {}

```diff
@@ -62,30 +62,30 @@
 requirements. - Stress Testing: Stress testing involves applying extreme but
 plausible hypothetical scenarios to the P/L distribution to assess the
 portfolioâs resilience. This helps managers prepare for unexpected market
 events and ensure that the portfolio can withstand adverse conditions.
 Therefore, P/L distribution serves as a key pillar of market risk management,
 providing insights into potential risks, informing decision-making, enabling
 portfolio optimization, and ensuring regulatory compliance. ``` #Libraries
-import EnvisionRiskRaaS as RaaS from datetime import date import
+#Libraries import EnvisionRiskRaaS as RaaS from datetime import date import
 matplotlib.pyplot as plt from scipy import stats import pandas as pd import
-numpy as np import queuelib #EnvisionRisk login RaaS.envrsk_auth_log_in("your
-username/email here", "your password here") #### Get the delta vector
-(simulated price change) #### # The term '_raw' within the function name is
-indicative of a key feature: # the simulated price changes are denominated in
-the same currency as # the stock. This implies that the analysis maintains the
-original currency # perspective of the stock, allowing for more accurate and
-relevant # insights. It enhances ease of comprehension and direct
+numpy as np import queuelib import seaborn as sns #EnvisionRisk login
+RaaS.envrsk_auth_log_in("your username/email here", "your password here") ####
+Get the delta vector (simulated price change) #### # The term '_raw' within the
+function name is indicative of a key feature: # the simulated price changes are
+denominated in the same currency as # the stock. This implies that the analysis
+maintains the original currency # perspective of the stock, allowing for more
+accurate and relevant # insights. It enhances ease of comprehension and direct
 applicability, # bringing us closer to the context of the actual trading
 environment. use_date = date.today() use_symbol = "AAPL.US" api_response =
-RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol) # Leverage our
+RaaS.envrsk_instrument_delta_vector_raw(use_date,use_symbol) # Leverage our
 sophisticated API to conduct an Expected-Shortfall computation, # specified at
 a 97.5% confidence level across a single-day span, utilizing a # point-in-time
 volatility scenario. api_response_es =
-RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols =
+RaaS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols =
 use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"]
 [0] #manipulate the data for the density function data = api_response["Output"]
 ["PnL"] #titles and captions subtitle = "Profit/Loss distribution (one day) for
 " + use_symbol + " as seen from the " + str(use_date) caption= "In the world of
 financial markets, price uncertainty is a key element that contributes to
 market risk - the risk of losses in positions arising \nfrom movements in
```

### Comparing `envisionriskraas-1.1.6/pyproject.toml` & `envisionriskraas-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.1.6"
+version = "1.1.7"
 authors = [{name="EnvisionRisk", email="support@envisionrisk.com" },{name="Coptolon",email="mark@brezina.dk"},]
 keywords = ["Risk-as-a-service","Market risk","Quantitative finance"]
 description = "EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `envisionriskraas-1.1.6/PKG-INFO` & `envisionriskraas-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.1.6
+Version: 1.1.7
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management
 Project-URL: Homepage, https://www.envisionrisk.com/
 Author-email: EnvisionRisk <support@envisionrisk.com>, Coptolon <mark@brezina.dk>
 License-File: LICENSE.txt
 Keywords: Market risk,Quantitative finance,Risk-as-a-service
 Classifier: License :: OSI Approved :: MIT License
@@ -59,40 +59,42 @@
 
 - <b>Stress Testing:</b> Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
 
 ```
 #Libraries
+#Libraries
 import EnvisionRiskRaaS as RaaS
 from datetime import date
 import matplotlib.pyplot as plt
 from scipy import stats
 import pandas as pd
 import numpy as np
 import queuelib
+import seaborn as sns
 
 #EnvisionRisk login
 RaaS.envrsk_auth_log_in("your username/email here", "your password here")
 
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
 # the stock. This implies that the analysis maintains the original currency 
 # perspective of the stock, allowing for more accurate and relevant 
 # insights. It enhances ease of comprehension and direct applicability, 
 # bringing us closer to the context of the actual trading environment.
 use_date = date.today()
 use_symbol = "AAPL.US"
-api_response = RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol)
+api_response = RaaS.envrsk_instrument_delta_vector_raw(use_date,use_symbol)
 
 # Leverage our sophisticated API to conduct an Expected-Shortfall computation, 
 # specified at a 97.5% confidence level across a single-day span, utilizing a 
 # point-in-time volatility scenario.
-api_response_es = RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols = use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
+api_response_es = RaaS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols = use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"][0]
 
 #manipulate the data for the density function
 data = api_response["Output"]["PnL"]
 
 #titles and captions
 subtitle = "Profit/Loss distribution (one day) for " + use_symbol + " as seen from the " + str(use_date)
@@ -105,15 +107,14 @@
 plt.axvline(x = expected_shortfall_estimate, color = "#57575F", label = 'axvline - full height')
 plt.text(expected_shortfall_estimate, 300, 'Expected-Shortfall (97.5%, 1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
 plt.xlabel("Profit/Loss (in $)")
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(5,-120, caption, ha='center', size=7)
 plt.show()
-
 ```
 
 <img height='600' style='border:0px;height:600px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
 
 <h2>API documentation</h2>
 <hr>
 You can locate our extensive API documentation <a href="https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/9ed9f79a31a4a-market-risk-as-a-service-api">here</a>. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.6 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.7 Summary:
 EnvisionRisk improves market risk management by providing predictive analytics
 for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-
 documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
 risk-management Project-URL: Homepage, https://www.envisionrisk.com/ Author-
 email: EnvisionRisk
 envisionrisk.com>, Coptolon
@@ -78,30 +78,30 @@
 requirements. - Stress Testing: Stress testing involves applying extreme but
 plausible hypothetical scenarios to the P/L distribution to assess the
 portfolioâs resilience. This helps managers prepare for unexpected market
 events and ensure that the portfolio can withstand adverse conditions.
 Therefore, P/L distribution serves as a key pillar of market risk management,
 providing insights into potential risks, informing decision-making, enabling
 portfolio optimization, and ensuring regulatory compliance. ``` #Libraries
-import EnvisionRiskRaaS as RaaS from datetime import date import
+#Libraries import EnvisionRiskRaaS as RaaS from datetime import date import
 matplotlib.pyplot as plt from scipy import stats import pandas as pd import
-numpy as np import queuelib #EnvisionRisk login RaaS.envrsk_auth_log_in("your
-username/email here", "your password here") #### Get the delta vector
-(simulated price change) #### # The term '_raw' within the function name is
-indicative of a key feature: # the simulated price changes are denominated in
-the same currency as # the stock. This implies that the analysis maintains the
-original currency # perspective of the stock, allowing for more accurate and
-relevant # insights. It enhances ease of comprehension and direct
+numpy as np import queuelib import seaborn as sns #EnvisionRisk login
+RaaS.envrsk_auth_log_in("your username/email here", "your password here") ####
+Get the delta vector (simulated price change) #### # The term '_raw' within the
+function name is indicative of a key feature: # the simulated price changes are
+denominated in the same currency as # the stock. This implies that the analysis
+maintains the original currency # perspective of the stock, allowing for more
+accurate and relevant # insights. It enhances ease of comprehension and direct
 applicability, # bringing us closer to the context of the actual trading
 environment. use_date = date.today() use_symbol = "AAPL.US" api_response =
-RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol) # Leverage our
+RaaS.envrsk_instrument_delta_vector_raw(use_date,use_symbol) # Leverage our
 sophisticated API to conduct an Expected-Shortfall computation, # specified at
 a 97.5% confidence level across a single-day span, utilizing a # point-in-time
 volatility scenario. api_response_es =
-RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols =
+RaaS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols =
 use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"]
 [0] #manipulate the data for the density function data = api_response["Output"]
 ["PnL"] #titles and captions subtitle = "Profit/Loss distribution (one day) for
 " + use_symbol + " as seen from the " + str(use_date) caption= "In the world of
 financial markets, price uncertainty is a key element that contributes to
 market risk - the risk of losses in positions arising \nfrom movements in
```

