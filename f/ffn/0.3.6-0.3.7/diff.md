# Comparing `tmp/ffn-0.3.6.tar.gz` & `tmp/ffn-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffn-0.3.6.tar", last modified: Wed Apr 21 02:47:20 2021, max compression
+gzip compressed data, was "ffn-0.3.7.tar", last modified: Tue May 23 20:32:17 2023, max compression
```

## Comparing `ffn-0.3.6.tar` & `ffn-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 02:47:20.000000 ffn-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2021-04-21 02:46:36.000000 ffn-0.3.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2021-04-21 02:47:20.000000 ffn-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-04-21 02:47:20.000000 ffn-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-04-21 02:46:36.000000 ffn-0.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-04-21 02:46:36.000000 ffn-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-04-21 02:46:36.000000 ffn-0.3.6/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 02:47:20.000000 ffn-0.3.6/ffn/
--rw-r--r--   0 runner    (1001) docker     (121)    78997 2021-04-21 02:46:36.000000 ffn-0.3.6/ffn/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2021-04-21 02:46:36.000000 ffn-0.3.6/ffn/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2021-04-21 02:46:36.000000 ffn-0.3.6/ffn/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-04-21 02:46:36.000000 ffn-0.3.6/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-04-21 02:46:36.000000 ffn-0.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:32:17.169293 ffn-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-23 20:31:35.000000 ffn-0.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 20:31:35.000000 ffn-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-23 20:32:17.169293 ffn-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-23 20:31:35.000000 ffn-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:32:17.169293 ffn-0.3.7/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 20:31:35.000000 ffn-0.3.7/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82021 2023-05-23 20:31:35.000000 ffn-0.3.7/ffn/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-23 20:31:35.000000 ffn-0.3.7/ffn/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-23 20:31:35.000000 ffn-0.3.7/ffn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:32:17.169293 ffn-0.3.7/ffn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-23 20:32:17.000000 ffn-0.3.7/ffn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 20:32:17.000000 ffn-0.3.7/ffn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:32:17.000000 ffn-0.3.7/ffn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-23 20:32:17.000000 ffn-0.3.7/ffn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 20:32:17.000000 ffn-0.3.7/ffn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 20:31:35.000000 ffn-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 20:32:17.173294 ffn-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-23 20:31:35.000000 ffn-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:32:17.169293 ffn-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26710 2023-05-23 20:31:35.000000 ffn-0.3.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-23 20:31:35.000000 ffn-0.3.7/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ffn-0.3.6/setup.py` & `ffn-0.3.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,36 +19,35 @@
     author_email="morissette.philippe@gmail.com",
     description="Financial functions for Python",
     keywords="python finance quant functions",
     url="https://github.com/pmorissette/ffn",
     license="MIT",
     install_requires=[
         "decorator>=4",
-        "future>=0.15",
         "matplotlib>=1",
         "numpy>=1.5",
         "pandas>=0.19",
         "pandas-datareader>=0.2",
         "scikit-learn>=0.15",
         "scipy>=0.15",
         "tabulate>=0.7.5",
+        "yfinance>=0.2",
     ],
     extras_require={
         "dev": [
-            "black>=20.8b1",
+            "black>=22",
             "codecov",
-            "coverage",
             "flake8",
             "flake8-black",
-            "future",
-            "mock",
-            "nose",
+            "pytest",
+            "pytest-cov",
         ],
     },
     packages=["ffn"],
     long_description=description,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python",
     ],
+    python_requires=">=3.7",
 )
```

### Comparing `ffn-0.3.6/LICENSE.txt` & `ffn-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ffn-0.3.6/README.rst` & `ffn-0.3.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 .. image:: https://github.com/pmorissette/ffn/workflows/Build%20Status/badge.svg
     :target: https://github.com/pmorissette/ffn/actions/
 
 .. image:: https://codecov.io/gh/pmorissette/ffn/branch/master/graph/badge.svg
     :target: https://codecov.io/pmorissette/ffn
 
+.. image:: https://img.shields.io/pypi/v/ffn
+    :alt: PyPI
+    :target: https://pypi.org/project/ffn/
+
+.. image:: https://img.shields.io/pypi/l/ffn
+    :alt: PyPI - License
+    :target: https://pypi.org/project/ffn/
+
 ffn - Financial Functions for Python
 ====================================
 
 Alpha release - please let me know if you find any bugs!
 
 If you are looking for a full backtesting framework, please check out `bt
 <https://github.com/pmorissette/bt>`_. bt is built atop ffn and makes it easy
@@ -53,19 +61,7 @@
 Documentation
 -------------
 
 Read the docs at http://pmorissette.github.io/ffn
 
 - `Quickstart <http://pmorissette.github.io/ffn/quick.html>`__
 - `Full API <http://pmorissette.github.io/ffn/ffn.html>`__
-
-Special Thanks
---------------
-
-A special thanks to the following contributors for their involvement with the project:
-
-* Jordan Platts `@JordanPlatts <https://github.com/JordanPlatts>`_ 
-
-License
--------
-
-MIT
```

### Comparing `ffn-0.3.6/ffn/core.py` & `ffn-0.3.7/ffn/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from __future__ import print_function
 
 import random
 
+import matplotlib
 import numpy as np
 import pandas as pd
 import scipy.stats
 import sklearn.cluster
 import sklearn.covariance
 import sklearn.manifold
-from future.utils import iteritems, listvalues
+from matplotlib import pyplot as plt  # noqa
+from packaging.version import Version
 from pandas.core.base import PandasObject
 from scipy.optimize import minimize
 from scipy.stats import t
 from sklearn.utils import resample
 from tabulate import tabulate
 
 from . import utils
 from .utils import fmtn, fmtp, fmtpn, get_freq_name
 
 try:
-    import prettyplotlib  # NOQA
+    import seaborn as sns
+
+    sns.set(style="ticks", palette="Set2")
 except ImportError:
     pass
 
-# avoid pyplot import failure in headless environment
-import os
+_PANDAS_TWO = Version(pd.__version__) >= Version("2")
 
-import matplotlib
-
-if "DISPLAY" not in os.environ:
-    if matplotlib.__version__ > "2.":
-        matplotlib.use("agg", force=False)
-    else:
-        matplotlib.use("agg", warn=False)
-
-from matplotlib import pyplot as plt  # noqa
+# module level variable, can be different for non traditional markets (eg. crypto - 360)
+TRADING_DAYS_PER_YEAR = 252
 
 
 class PerformanceStats(object):
     """
     PerformanceStats is a convenience class used for the performance
     evaluation of a price series. It contains various helper functions
     to help with plotting and contains a large amount of descriptive
@@ -53,30 +49,31 @@
     Attributes:
         * name (str): Name, derived from price series name
         * return_table (DataFrame): A table of monthly returns with
             YTD figures as well.
         * lookback_returns (Series): Returns for different
             lookback periods (1m, 3m, 6m, ytd...)
         * stats (Series): A series that contains all the stats
+        * annualization_factor (float): `Annualization factor` used in various calculations; aka `nperiods`, `252`
 
     """
 
-    def __init__(self, prices, rf=0.0):
+    def __init__(self, prices, rf=0.0, annualization_factor=TRADING_DAYS_PER_YEAR):
         super(PerformanceStats, self).__init__()
         self.prices = prices
         self.name = self.prices.name
         self._start = self.prices.index[0]
         self._end = self.prices.index[-1]
 
         self.rf = rf
+        self.annualization_factor = annualization_factor
 
         self._update(self.prices)
 
     def set_riskfree_rate(self, rf):
-
         """
         Set annual risk-free rate property and calculate properly annualized
         monthly and daily rates. Then performance stats are recalculated.
         Affects only this instance of the PerformanceStats.
 
         Args:
             * rf (float): Annual `risk-free rate <https://www.investopedia.com/terms/r/risk-freerate.asp>`_
@@ -219,29 +216,32 @@
 
         if len(r) < 2:
             return
 
         # Will calculate daily figures only if the input data has at least daily frequency or higher (e.g hourly)
         # Rather < 2 days than <= 1 days in case of data taken at different hours of the days
         if r.index.to_series().diff().min() < pd.Timedelta("2 days"):
-            self.daily_mean = r.mean() * 252
-            self.daily_vol = np.std(r, ddof=1) * np.sqrt(252)
+            self.daily_mean = r.mean() * self.annualization_factor
+            self.daily_vol = np.std(r, ddof=1) * np.sqrt(self.annualization_factor)
 
-            # if type(self.rf) is float:
             if isinstance(self.rf, float):
-                self.daily_sharpe = r.calc_sharpe(rf=self.rf, nperiods=252)
-                self.daily_sortino = calc_sortino_ratio(r, rf=self.rf, nperiods=252)
+                self.daily_sharpe = r.calc_sharpe(
+                    rf=self.rf, nperiods=self.annualization_factor
+                )
+                self.daily_sortino = calc_sortino_ratio(
+                    r, rf=self.rf, nperiods=self.annualization_factor
+                )
             # rf is a price series
             else:
                 _rf_daily_price_returns = self.rf.to_returns()
                 self.daily_sharpe = r.calc_sharpe(
-                    rf=_rf_daily_price_returns, nperiods=252
+                    rf=_rf_daily_price_returns, nperiods=self.annualization_factor
                 )
                 self.daily_sortino = calc_sortino_ratio(
-                    r, rf=_rf_daily_price_returns, nperiods=252
+                    r, rf=_rf_daily_price_returns, nperiods=self.annualization_factor
                 )
 
             self.best_day = r.max()
             self.worst_day = r.min()
 
         self.total_return = obj[-1] / obj[0] - 1
 
@@ -251,15 +251,16 @@
         self.drawdown = dp.to_drawdown_series()
         self.max_drawdown = self.drawdown.min()
         self.drawdown_details = drawdown_details(self.drawdown)
         if self.drawdown_details is not None:
             self.avg_drawdown = self.drawdown_details["drawdown"].mean()
             self.avg_drawdown_days = self.drawdown_details["Length"].mean()
 
-        self.calmar = np.divide(self.cagr, np.abs(self.max_drawdown))
+        with np.errstate(invalid="ignore", divide="ignore"):
+            self.calmar = np.divide(self.cagr, np.abs(self.max_drawdown))
 
         if len(r) < 4:
             return
 
         if r.index.to_series().diff().min() <= pd.Timedelta("2 days"):
             self.daily_skew = r.skew()
 
@@ -323,15 +324,15 @@
             fidx = mr.index[0]
             try:
                 self.return_table[fidx.year][fidx.month] = float(mp[0]) / dp[0] - 1
             except ZeroDivisionError:
                 self.return_table[fidx.year][fidx.month] = 0
             # calculate the YTD values
             for idx in self.return_table:
-                arr = np.array(listvalues(self.return_table[idx]))
+                arr = np.array(list(self.return_table[idx].values()))
                 self.return_table[idx][13] = np.prod(arr + 1) - 1
 
         if r.index.to_series().diff().min() < pd.Timedelta("93 days"):
             if len(mr) < 3:
                 return
 
             denom = dp[: dp.index[-1] - pd.DateOffset(months=3)]
@@ -924,15 +925,14 @@
     def _get_default_plot_title(self, freq, kind):
         if freq is None:
             return "%s" % kind
         else:
             return "%s %s" % (get_freq_name(freq), kind)
 
     def set_riskfree_rate(self, rf):
-
         """
         Set annual `risk-free rate <https://www.investopedia.com/terms/r/risk-freerate.asp>`_ property and calculate properly annualized
         monthly and daily rates. Then performance stats are recalculated.
         Affects only those instances of PerformanceStats that are children of
         this GroupStats object.
 
         Args:
@@ -1038,15 +1038,18 @@
 
         """
         if title is None:
             title = self._get_default_plot_title(freq, "Return Scatter Matrix")
 
         plt.figure()
         ser = self._get_series(freq).to_returns().dropna()
-        pd.scatter_matrix(ser, figsize=figsize, **kwargs)
+        if hasattr(pd, "scatter_matrix"):
+            pd.scatter_matrix(ser, figsize=figsize, **kwargs)
+        else:
+            pd.plotting.scatter_matrix(ser, figsize=figsize, **kwargs)
         return plt.suptitle(title)
 
     def plot_histograms(self, freq=None, title=None, figsize=(10, 10), **kwargs):
         """
         Wrapper around pandas' hist.
 
         Args:
@@ -1395,28 +1398,30 @@
     Args:
         * returns (Series, DataFrame): Input return series
         * rf (float, Series): `Risk-free rate <https://www.investopedia.com/terms/r/risk-freerate.asp>`_ expressed as a yearly (annualized) return or return series
         * nperiods (int): Frequency of returns (252 for daily, 12 for monthly,
             etc.)
 
     """
-    # if type(rf) is float and rf != 0 and nperiods is None:
+    if nperiods is None:
+        nperiods = infer_freq(returns)
+
     if isinstance(rf, float) and rf != 0 and nperiods is None:
         raise Exception("Must provide nperiods if rf != 0")
 
     er = returns.to_excess_returns(rf, nperiods=nperiods)
     std = np.std(er, ddof=1)
-    res = np.divide(er.mean(), std)
+    with np.errstate(invalid="ignore", divide="ignore"):
+        res = np.divide(er.mean(), std)
 
     if annualize:
         if nperiods is None:
             nperiods = 1
         return res * np.sqrt(nperiods)
-    else:
-        return res
+    return res
 
 
 def calc_information_ratio(returns, benchmark_returns):
     """
     Calculates the `Information ratio <https://www.investopedia.com/terms/i/informationratio.asp>`_ (or `from Wikipedia <http://en.wikipedia.org/wiki/Information_ratio>`_).
     """
     diff_rets = returns - benchmark_returns
@@ -1720,15 +1725,14 @@
     n = len(x0)
     x = x0.copy()
     var = np.diagonal(cov)
     ctr = cov.dot(x)
     sigma_x = np.sqrt(x.T.dot(ctr))
 
     for iteration in range(maximum_iterations):
-
         for i in range(n):
             alpha = var[i]
             beta = ctr[i] - x[i] * alpha
             gamma = -b[i] * sigma_x
 
             x_tilde = (-beta + np.sqrt(beta * beta - 4 * alpha * gamma)) / (2 * alpha)
             x_i = x[i]
@@ -1818,15 +1822,17 @@
     else:
         raise NotImplementedError("risk_parity_method not implemented")
 
     # return erc weights vector
     return pd.Series(erc_weights, index=returns.columns, name="erc")
 
 
-def get_num_days_required(offset, period="d", perc_required=0.90):
+def get_num_days_required(
+    offset, period="d", perc_required=0.90, annualization_factor=252
+):
     """
     Estimates the number of days required to assume that data is OK.
 
     Helper function used to determine if there are enough "good" data
     days over a given period.
 
     Args:
@@ -1842,15 +1848,15 @@
     days = delta.days * 0.69
 
     if period == "d":
         req = days * perc_required
     elif period == "m":
         req = (days / 20) * perc_required
     elif period == "y":
-        req = (days / 252) * perc_required
+        req = (days / annualization_factor) * perc_required
     else:
         raise NotImplementedError("period not supported. Supported periods are d, m, y")
 
     return req
 
 
 def calc_clusters(returns, n=None, plot=False):
@@ -1917,15 +1923,15 @@
         for i, txt in enumerate(returns.columns):
             ax.annotate(txt, (xy[i, 0], xy[i, 1]), size=14)
 
     # sanitize return value
     tmp = result[0]
     # map as such {cluster: [list of tickers], cluster2: [...]}
     inv_map = {}
-    for k, v in iteritems(tmp):
+    for k, v in tmp.items():
         inv_map[v] = inv_map.get(v, [])
         inv_map[v].append(k)
 
     return inv_map
 
 
 def calc_ftca(returns, threshold=0.5):
@@ -2269,38 +2275,100 @@
 
     Args:
         * returns (float, Series, DataFrame): Return(s)
         * nperiods (int): Target basis, typically 252 for daily, 12 for
             monthly, etc.
 
     """
+    if nperiods is None:
+        nperiods = infer_freq(returns)
     return np.power(1 + returns, 1.0 / nperiods) - 1.0
 
 
+def infer_freq(data):
+    """
+        Infer the most likely frequency given the input index. If the frequency is
+    uncertain or index is not DateTime like, just return None
+        Args:
+            * data (DataFrame, Series): Any timeseries dataframe or series
+    """
+    try:
+        if _PANDAS_TWO:
+            return pd.infer_freq(data.index)
+        else:
+            return pd.infer_freq(data.index, warn=False)
+    except Exception:
+        return None
+
+
+def _whole_periods_str_to_nperiods(freq, annualization_factor=TRADING_DAYS_PER_YEAR):
+    if freq == "Y" or freq == "A":
+        return 1
+    if freq == "M":
+        return 12
+    if freq == "D":
+        return annualization_factor
+    if freq == "H":
+        return annualization_factor * 24
+    if freq == "T":
+        return annualization_factor * 24 * 60
+    if freq == "S":
+        return annualization_factor * 24 * 60 * 60
+    return None
+
+
+def infer_nperiods(data, annualization_factor=TRADING_DAYS_PER_YEAR):
+    annualization_factor = annualization_factor or TRADING_DAYS_PER_YEAR
+    freq = infer_freq(data)
+
+    if freq is None:
+        return None
+
+    if len(freq) == 1:
+        return _whole_periods_str_to_nperiods(freq, annualization_factor)
+    try:
+        if freq.startswith("A"):
+            return 1
+        else:
+            whole_periods_str = freq[-1]
+            num_str = freq[:-1]
+            num = int(num_str)
+            return num * _whole_periods_str_to_nperiods(
+                whole_periods_str, annualization_factor
+            )
+    except KeyboardInterrupt:
+        raise
+    except BaseException:
+        return None
+
+
 def calc_sortino_ratio(returns, rf=0.0, nperiods=None, annualize=True):
     """
     Calculates the `Sortino ratio <https://www.investopedia.com/terms/s/sortinoratio.asp>`_ given a series of returns
     (see `Sharpe vs. Sortino <https://www.investopedia.com/ask/answers/010815/what-difference-between-sharpe-ratio-and-sortino-ratio.asp>`_).
 
     Args:
         * returns (Series or DataFrame): Returns
         * rf (float, Series): `Risk-free rate <https://www.investopedia.com/terms/r/risk-freerate.asp>`_ expressed in yearly (annualized) terms or return series.
         * nperiods (int): Number of periods used for annualization. Must be
             provided if rf is non-zero and rf is not a price series
 
     """
-    # if type(rf) is float and rf != 0 and nperiods is None:
     if isinstance(rf, float) and rf != 0 and nperiods is None:
         raise Exception("nperiods must be set if rf != 0 and rf is not a price series")
 
+    if nperiods is None:
+        nperiods = infer_freq(returns)
+
     er = returns.to_excess_returns(rf, nperiods=nperiods)
 
     negative_returns = np.minimum(er[1:], 0.0)
     std = np.std(negative_returns, ddof=1)
-    res = np.divide(er.mean(), std)
+    with np.errstate(invalid="ignore", divide="ignore"):
+        res = np.divide(er.mean(), std)
 
     if annualize:
         if nperiods is None:
             nperiods = 1
         return res * np.sqrt(nperiods)
 
     return res
@@ -2315,17 +2383,18 @@
         * rf (float, Series): `Risk-Free rate(s) <https://www.investopedia.com/terms/r/risk-freerate.asp>`_ expressed in annualized term or return series
         * nperiods (int): Optional. If provided, will convert rf to different
             frequency using deannualize only if rf is a float
     Returns:
         * excess_returns (Series, DataFrame): Returns - rf
 
     """
-    # if type(rf) is float and nperiods is not None:
-    if isinstance(rf, float) and nperiods is not None:
+    if nperiods is None:
+        nperiods = infer_freq(returns)
 
+    if isinstance(rf, float) and nperiods is not None:
         _rf = deannualize(rf, nperiods)
     else:
         _rf = rf
 
     return returns - _rf
 
 
@@ -2338,24 +2407,42 @@
 
     """
     return np.divide(prices.calc_cagr(), abs(prices.calc_max_drawdown()))
 
 
 def to_ulcer_index(prices):
     """
+    Calculates the Ulcer Index for a series of investment returns.
+
     Converts from prices -> `Ulcer index <https://www.investopedia.com/terms/u/ulcerindex.asp>`_
 
     See https://en.wikipedia.org/wiki/Ulcer_index
 
     Args:
-        * prices (Series, DataFrame): Prices
+        prices (pandas.Series or numpy.ndarray): A series of investment returns.
 
+    Returns:
+        float: The Ulcer Index.
     """
-    dd = prices.to_drawdown_series()
-    return np.divide(np.sqrt(np.sum(np.power(dd, 2))), dd.count())
+
+    # calculate the maximum value seen so far at each point in time
+    max_values = np.maximum.accumulate(prices)
+
+    # calculate the drawdowns relative to the maximum values
+    drawdowns = ((prices - max_values) / max_values) * 100
+
+    # calculate the squared drawdowns
+    squared_drawdowns = np.square(drawdowns)
+
+    # calculate the average of the squared drawdowns
+    avg_squared_drawdowns = np.mean(squared_drawdowns)
+
+    # calculate the square root of the average squared drawdowns
+    ulcer_index = np.sqrt(avg_squared_drawdowns)
+    return ulcer_index
 
 
 def to_ulcer_performance_index(prices, rf=0.0, nperiods=None):
     """
     Converts from prices -> `ulcer performance index <https://www.investopedia.com/terms/u/ulcerindex.asp>`_.
 
     See https://en.wikipedia.org/wiki/Ulcer_index
@@ -2363,15 +2450,17 @@
     Args:
         * prices (Series, DataFrame): Prices
         * rf (float, Series): `Risk-free rate of return <https://www.investopedia.com/terms/r/risk-freerate.asp>`_. Assumed to be expressed in
             yearly (annualized) terms or return series
         * nperiods (int): Used to deannualize rf if rf is provided (non-zero)
 
     """
-    # if type(rf) is float and rf != 0 and nperiods is None:
+    if nperiods is None:
+        nperiods = infer_freq(prices)
+
     if isinstance(rf, float) and rf != 0 and nperiods is None:
         raise Exception("nperiods must be set if rf != 0 and rf is not a price series")
 
     er = prices.to_returns().to_excess_returns(rf, nperiods=nperiods)
 
     return np.divide(er.mean(), prices.to_ulcer_index())
```

### Comparing `ffn-0.3.6/ffn/data.py` & `ffn-0.3.7/ffn/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from distutils.version import LooseVersion
-
-import pandas as pd
-
 import ffn
+import pandas as pd
+import yfinance
+from packaging.version import Version
+from pandas_datareader import data as pdata
 
 # import ffn.utils as utils
 from . import utils
 
 # This is a temporary fix until pandas_datareader 0.7 is released.
 # pandas 0.23 has moved is_list_like from common to api.types, hence the monkey patch
-if LooseVersion(pd.__version__) > LooseVersion("0.23.0"):
+if Version(pd.__version__) > Version("0.23.0"):
     pd.core.common.is_list_like = pd.api.types.is_list_like
 
-from pandas_datareader import data as pdata
-
 
 @utils.memoize
 def get(
     tickers,
     provider=None,
     common_dates=True,
     forward_fill=False,
@@ -133,14 +131,16 @@
 
 
 @utils.memoize
 def yf(ticker, field, start=None, end=None, mrefresh=False):
     if field is None:
         field = "Adj Close"
 
+    yfinance.pdr_override()
+
     tmp = pdata.get_data_yahoo(ticker, start=start, end=end)
 
     if tmp is None:
         raise ValueError("failed to retrieve data for %s:%s" % (ticker, field))
 
     if field:
         return tmp[field]
```

### Comparing `ffn-0.3.6/ffn/utils.py` & `ffn-0.3.7/ffn/utils.py`

 * *Files identical despite different names*

