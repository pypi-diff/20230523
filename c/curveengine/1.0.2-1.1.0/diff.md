# Comparing `tmp/curveengine-1.0.2-py3-none-any.whl.zip` & `tmp/curveengine-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 10195 bytes, number of entries: 10
--rw-r--r--  2.0 unx     6770 b- defN 23-Apr-18 01:53 curveengine.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 23:51 parsing/__init__.py
--rw-r--r--  2.0 unx      454 b- defN 23-Apr-13 14:34 parsing/enums.py
--rw-r--r--  2.0 unx     4557 b- defN 23-Apr-18 01:18 parsing/others.py
--rw-r--r--  2.0 unx    14342 b- defN 23-Apr-18 01:49 parsing/parsers.py
--rw-r--r--  2.0 unx    17797 b- defN 23-Apr-14 23:47 parsing/ratehelpers.py
--rw-r--r--  2.0 unx      532 b- defN 23-Apr-18 02:06 curveengine-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 02:06 curveengine-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-18 02:06 curveengine-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 23-Apr-18 02:06 curveengine-1.0.2.dist-info/RECORD
-10 files, 45323 bytes uncompressed, 8913 bytes compressed:  80.3%
+Zip file size: 14635 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      803 b- defN 23-May-23 01:29 curveengine/__init__.py
+-rw-r--r--  2.0 unx     7755 b- defN 23-May-23 01:06 curveengine/engine.py
+-rw-r--r--  2.0 unx      266 b- defN 23-May-23 01:18 curveengine/parsing/__init__.py
+-rw-r--r--  2.0 unx    32971 b- defN 23-May-23 02:53 curveengine/parsing/checks.py
+-rw-r--r--  2.0 unx     3462 b- defN 23-May-22 02:32 curveengine/parsing/enums.py
+-rw-r--r--  2.0 unx     4115 b- defN 23-May-23 01:00 curveengine/parsing/others.py
+-rw-r--r--  2.0 unx     7673 b- defN 23-May-23 01:01 curveengine/parsing/parsers.py
+-rw-r--r--  2.0 unx    13513 b- defN 23-May-23 03:29 curveengine/parsing/ratehelpers.py
+-rw-r--r--  2.0 unx      532 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      994 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/RECORD
+12 files, 72188 bytes uncompressed, 12963 bytes compressed:  82.0%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
-Filename: curveengine.py
+Filename: curveengine/__init__.py
 Comment: 
 
-Filename: parsing/__init__.py
+Filename: curveengine/engine.py
 Comment: 
 
-Filename: parsing/enums.py
+Filename: curveengine/parsing/__init__.py
 Comment: 
 
-Filename: parsing/others.py
+Filename: curveengine/parsing/checks.py
 Comment: 
 
-Filename: parsing/parsers.py
+Filename: curveengine/parsing/enums.py
 Comment: 
 
-Filename: parsing/ratehelpers.py
+Filename: curveengine/parsing/others.py
 Comment: 
 
-Filename: curveengine-1.0.2.dist-info/METADATA
+Filename: curveengine/parsing/parsers.py
 Comment: 
 
-Filename: curveengine-1.0.2.dist-info/WHEEL
+Filename: curveengine/parsing/ratehelpers.py
 Comment: 
 
-Filename: curveengine-1.0.2.dist-info/top_level.txt
+Filename: curveengine-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: curveengine-1.0.2.dist-info/RECORD
+Filename: curveengine-1.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: curveengine-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: curveengine-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `curveengine.py` & `curveengine/engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,87 @@
-from parsing.parsers import *
-from parsing.enums import *
-from parsing.others import *
-from parsing.ratehelpers import *
+from .parsing.parsers import *
+from .parsing.enums import *
+from .parsing.others import *
+from .parsing.ratehelpers import *
+from .parsing.checks import *
 
 
 class CurveEngine:
+    '''
+    Class for building curves and indexes from a JSON configuration file.
+
+    Parameters
+    ----------
+    data : dict
+        The JSON configuration file as a dictionary.
+    curves : dict, optional
+        A dictionary of curves to be populated by the engine. The default is {}.
+    indexes : dict, optional
+        A dictionary of indexes to be populated by the engine. The default is {}.
+
+    Returns
+    -------
+    None
+    '''
+
     def __init__(self, data, curves={}, indexes={}):
         self.curveHandles = {None: ore.RelinkableYieldTermStructureHandle()}
         self.curves = curves
         self.indexes = indexes
         localData = data.copy()
-        self.initialize(localData)
+        checkConfiguration(localData)
+        self.__initialize(localData)
+
+    '''
+    Get a curve by name.
+
+    Parameters
+    ----------
+    curveName : str
+        The name of the curve to get.
+
+    Returns
+    -------
+    ore.YieldTermStructure
+        The curve with the given name.
+    '''
 
     def getCurve(self, curveName):
         return self.curves[curveName]
 
+    '''
+    Get an index by name.
+
+    Parameters
+    ----------
+    indexName : str
+        The name of the index to get.
+
+    Returns
+    -------
+    ore.IborIndex or ore.OvernightIndex
+        The index with the given name.
+    '''
+
     def getIndex(self, indexName):
         return self.indexes[indexName]
 
-    def initialize(self, data):
+    def __initialize(self, data):
         refDate = parseDate(data['refDate'])
         ore.Settings.instance().evaluationDate = refDate
 
         tmpData = {}
         for curve in data['curves']:
             curveName = curve['curveName']
             tmpData[curveName] = curve
 
         dependencies = getDependencyList(data)
         sortedList = topologicalSort(dependencies)
         for curveName in sortedList:
-            parsed = parse(level=curveName,**tmpData[curveName])
+            parsed = parse(**tmpData[curveName])
             if curveName not in self.indexes.keys():
                 self.__buildIndexes(parsed)
             if curveName not in self.curves.keys():
                 self.__buildCurve(parsed)
 
     def __buildIndexes(self, data):
         name = data['curveName']
@@ -85,30 +132,30 @@
                 elif helperType == HelperType.OIS:
                     helper = createOISRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.Swap:
                     helper = createSwapRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.TenorBasis:
-                    helper = createTenorBasisSwap(
+                    helper = createTenorBasisSwapRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.Xccy:
-                    helper = createCrossCcyFixFloatSwapHelper(
+                    helper = createCrossCcyFixFloatSwapRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.FxSwap:
                     helper = createFxSwapRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.SofrFuture:
                     helper = createSofrFutureRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.XccyBasis:
-                    helper = createCrossCcyBasisSwapHelper(
+                    helper = createCrossCcyBasisSwapRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 elif helperType == HelperType.Bond:
-                    helper = createFixedRateBondHelper(
+                    helper = createFixedRateBondRateHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 else:
                     raise Exception(
                         'Unknown rate helper type: {}'.format(helperType))
             except KeyError as e:
                 raise KeyError('Failed to create rate helper {helper}/{i} at curve {curveName}: Key not found: {error} '.format(
                     helper=helperType, curveName=data['curveName'], error=e, i=i))
```

## Comparing `parsing/others.py` & `curveengine/parsing/others.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from parsing.parsers import *
-from parsing.enums import *
+from .parsers import *
+from .enums import *
 from collections import deque
 
 
 def createOvernightIndex(name: str, indexConfig: dict, handle: ore.YieldTermStructureHandle):
     """
     Create an overnight index
 
@@ -81,46 +81,34 @@
     curve depends on.
     """
     # Possible curve related keys
     pc = ['discountCurve', 'collateralCurve']
     # Possible index related keys
     pi = ['index', 'shortIndex', 'longIndex']
 
-    checkDictKeys(data, ['curves'], level='')
-
     dependencies = {}
     for curve in data['curves']:
-        checkDictKeys(curve, ['curveName', 'curveConfig'], level='curves')
-
         curveName = curve['curveName']
         if curveName not in dependencies.keys():
             dependencies[curveName] = set()
 
         curveConfig = curve['curveConfig']
-        checkDictKeys(curveConfig, ['curveType',
-                      'rateHelpers'], level=r'{curve}\curves'.format(curve=curveName))
-
         curveType = CurveType(curveConfig['curveType'])
         if curveType == CurveType.Piecewise:
             for rateHelper in curveConfig['rateHelpers']:
-                checkDictKeys(rateHelper, ['helperType', 'helperConfig'],
-                              level=r'{curve}\curves\rateHelpers'.format(curve=curveName))
                 helperConfig = rateHelper['helperConfig']
                 for key in pc:
                     if key in helperConfig:
                         dependencies[curveName].add(helperConfig[key])
                     for key in pi:
                         if key in helperConfig:
                             dependencies[curveName].add(helperConfig[key])
     return dependencies
 
 
-
-
-
 def topologicalSort(dependencies):
     """
     Sort the dependency list topologically
 
     Parameters
     ----------
     dependencies : dict
```

## Comparing `parsing/ratehelpers.py` & `curveengine/parsing/ratehelpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,49 @@
-from parsing.parsers import *
-from parsing.others import *
+from .parsers import *
+from .others import *
 
 
 def createOISRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
     """
     Create an OIS rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - tenor : str
-            The tenor of the helper
-        - calendar : str
-            The calendar
-        - convention : str
-            The business day convention
-        - settlementDays : int
-            The number of settlement days
-        - endOfMonth : bool
-            Whether the end of month rule is applied
-        - paymentLag : int
-            The payment lag
-        - fixedLegFrequency : str
-            The frequency of the fixed leg
-        - fwdStart : str
-            The forward start
-        - index : str
-            The index
+
     marketConfig : dict
         The market configuration for the helper
-        - rate : float
-            The rate
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.OISRateHelper
         The rate helper
+
+    See Also
+    ----------
+    checkOISRateHelper
     """
     tenor = helperConfig['tenor']
     calendar = helperConfig['calendar']
     businessDayConvention = helperConfig['convention']
 
     settlementDays = helperConfig['settlementDays']
     endOfMonth = helperConfig['endOfMonth']
     paymentLag = helperConfig['paymentLag']
     fixedLegFrequency = helperConfig['fixedLegFrequency']
     fwdStart = helperConfig['fwdStart']
     index = indexes[helperConfig['index']]
 
-    rate = marketConfig['rate']
+    rate = marketConfig['rate']['value']
     discountCurve = curves[helperConfig['discountCurve']]
 
     rate = ore.QuoteHandle(ore.SimpleQuote(rate))
     helper = ore.OISRateHelper(settlementDays, tenor, rate, index, discountCurve, endOfMonth,
                                paymentLag, businessDayConvention, fixedLegFrequency, calendar, fwdStart)
     return helper
 
@@ -67,96 +52,71 @@
     """
     Create a deposit rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - tenor : str
-            The tenor of the helper
-        - calendar : str
-            The calendar
-        - convention : str
-            The business day convention
-        - settlementDays : int
-            The number of settlement days
-        - endOfMonth : bool
-            Whether the end of month rule is applied
-        - dayCounter : str
-            The day counter
+       
     marketConfig : dict
         The market configuration for the helper
-        - rate : float
-            The rate
-
+       
     Returns
     -------
     ore.DepositRateHelper
         The rate helper
+
+    See Also
+    ----------
+    checkDepositRateHelper
     """
     tenor = helperConfig['tenor']
     settlementDays = helperConfig['settlementDays']
     calendar = helperConfig['calendar']
     convention = helperConfig['convention']
     endOfMonth = helperConfig['endOfMonth']
     dayCounter = helperConfig['dayCounter']
 
-    rate = ore.QuoteHandle(ore.SimpleQuote(marketConfig['rate']))
+    rate = ore.QuoteHandle(ore.SimpleQuote(marketConfig['rate']['value']))
     helper = ore.DepositRateHelper(rate, tenor, settlementDays, calendar,
                                    convention, endOfMonth, dayCounter)
     return helper
 
 
-def createFixedRateBondHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createFixedRateBondRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
     """
     Create a fixed rate bond helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - calendar : str
-            The calendar
-        - convention : str
-            The business day convention
-        - settlementDays : int
-            The number of settlement days
-        - couponDayCounter : str
-            The day counter for the coupon
-        - frequency : str
-            The frequency of the coupon
-        - tenor: str
-            The tenor of the helper
-            Optional, if not provided, startDate and endDate must be provided
-        - startDate : str
-            The start date of the helper
-        - endDate : str
-            The end date of the helper
+
     marketConfig : dict
         The market configuration for the helper
-        - couponRate : float
-            The coupon rate
-        - rate : float or ore.InterestRate
-            The rate
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.BondHelper
         The rate helper
+
+    See Also
+    ----------
+    checkFixedRateBondRateHelper
     """
     calendar = helperConfig['calendar']
     businessDayConvention = helperConfig['convention']
     settlementDays = helperConfig['settlementDays']
     couponDayCounter = helperConfig['couponDayCounter']
-    couponRate = marketConfig['couponRate']
+    couponRate = helperConfig['couponRate']
     frequency = helperConfig['frequency']
 
     if 'tenor' in helperConfig.keys():
         tenor = helperConfig['tenor']
         startDate = ore.Settings.instance().evaluationDate()
         maturityDate = startDate + ore.Period(tenor)
     else:
@@ -171,15 +131,15 @@
         calendar,
         businessDayConvention,
         businessDayConvention,
         ore.DateGeneration.Backward,
         False
     )
 
-    rate = marketConfig['rate']
+    rate = marketConfig['rate']['value']
     if isinstance(rate, float):
         rateDayCounter = ore.Actual365Fixed()
         rateCompounding = ore.Compounded
         rateFrequency = ore.Annual
     elif isinstance(rate, ore.InterestRate):
         rateDayCounter = rate.dayCounter()
         rateCompounding = rate.compounding()
@@ -216,57 +176,42 @@
     """
     Create a swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - tenor : str
-            The tenor of the helper
-        - calendar : str
-            The calendar
-        - convention : str
-            The business day convention
-        - fixedLegFrequency : str
-            The frequency of the fixed leg
-        - dayCounter : str
-            The day counter
-        - index : str
-            The index
-        - discountCurve : str
-            The discounting curve
-        - fwdStart : int
-            The number of days for the forward start
+
     marketConfig : dict
-        The market configuration for the helper
-        - rate : float
-            The rate
-        - spread : float
-            The spread
+        The market configuration for the helper      
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.SwapRateHelper
         The rate helper
+
+    See Also
+    ----------
+    checkSwapRateHelper
     """
     tenor = helperConfig['tenor']
     calendar = helperConfig['calendar']
     convention = helperConfig['convention']
     fixedLegFrequency = helperConfig['fixedLegFrequency']
     dayCounter = helperConfig['dayCounter']
     fwdStart = helperConfig['fwdStart']
 
     # QuoteHandle
-    rate = marketConfig['rate']
-    spread = marketConfig['spread']
+    rate = marketConfig['rate']['value']
+    spread = marketConfig['spread']['value']
     rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # Index
     index = indexes[helperConfig['index']]
 
     # Discounting curve
@@ -283,51 +228,34 @@
     """
     Create a fx swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - fixingDays : int
-            The number of fixing days
-        - calendar : str
-            The calendar
-        - convention : str
-            The business day convention
-        - endOfMonth : bool
-            Whether the end of month rule applies
-        - baseCurrencyAsCollateral : bool
-            Whether the base currency is used as collateral
-        - tenor : str
-            The tenor of the helper
-            Optional, if not provided, endDate must be provided
-        - endDate : str
-            The end date of the helper
-        - discountCurve : str
-            The discounting curve
 
     marketConfig : dict
         The market configuration for the helper
-        - fxPoints : float
-            The fx points
-        - fxSpot : float
-            The fx spot
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.FxSwapRateHelper
         The rate helper
+
+    See Also
+    ----------
+    checkFxSwapRateHelper
     """
-    fxPoints = marketConfig['fxPoints']
-    spotFx = marketConfig['fxSpot']
+    fxPoints = marketConfig['fxPoints']['value']
+    spotFx = marketConfig['fxSpot']['value']
 
     fixingDays = helperConfig['fixingDays']
     calendar = helperConfig['calendar']
     convention = helperConfig['convention']
     endOfMonth = helperConfig['endOfMonth']
     baseCurrencyAsCollateral = helperConfig['baseCurrencyAsCollateral']
 
@@ -366,36 +294,31 @@
     """
     Create a sofr future rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - month : int
-            The month of the helper
-        - year : int
-            The year of the helper
-        - frequency : str
-            The frequency of the helper
+
     marketConfig : dict
         The market configuration for the helper
-        - price : float
-            The price
-        - convexity : float
-            The convexity
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.SofrFutureRateHelper
         The rate helper
+
+    See Also
+    ----------
+    TODO: checkSofrFutureRateHelper
     """
     month = helperConfig['month']
     year = helperConfig['year']
     frequency = helperConfig['frequency']
     # QuoteHandle
     price = marketConfig['price']
     convexity = marketConfig['convexity']
@@ -409,57 +332,49 @@
         year,
         frequency,
         convexityQuote
     )
     return sofrFutureRateHelper
 
 
-def createTenorBasisSwap(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createTenorBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
     """
     Create a tenor basis swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - tenor : str
-            The tenor of the helper
-        - spreadOnShort : bool
-            Whether the spread is on the short leg
-        - longIndex : str
-            The long index
-        - shortIndex : str
-            The short index
-        - discountCurve : str
-            The discounting curve
 
     marketConfig : dict
         The market configuration for the helper
-        - spread : float
-            The spread
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.TenorBasisSwapHelper
         The rate helper
+
+    See Also
+    ----------
+    checkTenorBasisRateHelper
     """
     tenor = helperConfig['tenor']
     spreadOnShort = helperConfig['spreadOnShort']
 
     # Index
     longIndex = indexes[helperConfig['longIndex']]
     shortIndex = indexes[helperConfig['shortIndex']]
 
     # QuoteHandle
-    spread = marketConfig['spread']
+    spread = marketConfig['spread']['value']
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # Discounting curve
     discountCurve = curves[helperConfig['discountCurve']]
 
     # TenorBasisSwapHelper
     tenorBasisSwapHelper = ore.TenorBasisSwapHelper(
@@ -472,75 +387,53 @@
         spreadOnShort,
         True
     )
 
     return tenorBasisSwapHelper
 
 
-def createCrossCcyFixFloatSwapHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createCrossCcyFixFloatSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
     """
     Create a cross currency fix float swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
-        The configuration for the helper
-        - tenor : str
-            The tenor of the helper
-        - dayCounter : str
-            The day counter
-        - settlementDays : int
-            The number of settlement days
-        - endOfMonth : bool
-            Whether the end of month rule applies
-        - convention : str
-            The business day convention
-        - fixedLegFrequency : str
-            The frequency of the fixed leg
-        - fixedLegCurrency : str
-            The currency of the fixed leg
-        - calendar : str
-            The calendar
-        - index : str
-            The index
-        - discountCurve : str
-            The discounting curve
+        The configuration for the helper        
 
     marketConfig : dict
         The market configuration for the helper
-        - rate : float
-            The rate
-        - fxSpot : float
-            The fx spot
-        - spread : float
-            The spread
 
     curves : dict
         The curves
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.CrossCcyFixFloatSwapHelper
         The rate helper
+
+    See Also
+    ----------
+    checkCrossCcyFixFloatSwapRateHelper
     """
     tenor = helperConfig['tenor']
     dayCounter = helperConfig['dayCounter']
     settlementDays = helperConfig['settlementDays']
     endOfMonth = helperConfig['endOfMonth']
     convention = helperConfig['convention']
     fixedLegFrequency = helperConfig['fixedLegFrequency']
     fixedLegCurrency = helperConfig['fixedLegCurrency']
     calendar = helperConfig['calendar']
 
     # QuoteHandle
-    rate = marketConfig['rate']
-    spotFx = marketConfig['fxSpot']
-    spread = marketConfig['spread']
+    rate = marketConfig['rate']['value']
+    spotFx = marketConfig['fxSpot']['value']
+    spread = marketConfig['spread']['value']
 
     rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
     spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # Index
     index = indexes[helperConfig['index']]
@@ -564,38 +457,22 @@
         discountCurve,
         spreadQuote,
         endOfMonth
     )
     return crossCcyFixFloatSwapHelper
 
 
-def createCrossCcyBasisSwapHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createCrossCcyBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
     """
     Create a cross currency basis swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
-        - tenor : str
-            The tenor of the helper
-        - calendar : str
-            The calendar
-        - settlementDays : int
-            The number of settlement days
-        - endOfMonth : bool
-            Whether the end of month rule applies
-        - convention : str
-            The business day convention
-        - flatIndex : str
-            The flat index
-        - spreadIndex : str
-            The spread index
-        - discountCurve : str
-            The discounting curve
 
     marketConfig : dict
         The market configuration for the helper
         - spread : float
             The spread
 
     curves : dict
@@ -603,14 +480,18 @@
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.CrossCcyBasisSwapHelper
         The rate helper
+
+    See Also
+    ----------
+    checkCrossCcyBasisSwapRateHelper
     """
     tenor = helperConfig['tenor']
     calendar = helperConfig['calendar']
     settlementDays = helperConfig['settlementDays']
     endOfMonth = helperConfig['endOfMonth']
     convention = helperConfig['convention']
 
@@ -619,15 +500,15 @@
     spreadDiscountCurve = curves[helperConfig['discountCurve']]
 
     # Index
     flatIndex = indexes[helperConfig['flatIndex']]
     spreadIndex = indexes[helperConfig['spreadIndex']]
 
     # QuoteHandle
-    spread = marketConfig['spread']
+    spread = marketConfig['spread']['value']
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # CrossCcyBasisSwapHelper
     crossCcyBasisSwapHelper = ore.CrossCcyBasisSwapHelper(
         spreadQuote,
         tenor,
         calendar,
```

## Comparing `curveengine-1.0.2.dist-info/METADATA` & `curveengine-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curveengine
-Version: 1.0.2
+Version: 1.1.0
 Summary: A simple curve bootstraping tool based on ORE/QuantLib
 Author: Jose Melo
 Author-email: jmelo@live.cl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Requires-Dist: open-source-risk-engine
```

