# Comparing `tmp/teal-ravenframework-0.3.tar.gz` & `tmp/teal-ravenframework-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cogljj/raven/packaging/teal_package/dist/tmpng8vzp6e/teal-ravenframework-0.3.tar", last modified: Wed Nov 16 17:51:05 2022, max compression
+gzip compressed data, was "teal-ravenframework-0.4.tar", last modified: Mon May 22 16:26:54 2023, max compression
```

## Comparing `teal-ravenframework-0.3.tar` & `teal-ravenframework-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 cogljj   (536925976) staff       (20)        0 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/
--rw-r--r--   0 cogljj   (536925976) staff       (20)       72 2022-11-16 17:45:04.000000 teal-ravenframework-0.3/MANIFEST.in
--rw-r--r--   0 cogljj   (536925976) staff       (20)     1297 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/PKG-INFO
-drwxr-xr-x   0 cogljj   (536925976) staff       (20)        0 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/TEAL/
--rw-r--r--   0 cogljj   (536925976) staff       (20)    11356 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/LICENSE.txt
--rw-r--r--   0 cogljj   (536925976) staff       (20)     1758 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/NOTICE.txt
--rw-r--r--   0 cogljj   (536925976) staff       (20)     1127 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/README.md
--rw-r--r--   0 cogljj   (536925976) staff       (20)      800 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/__init__.py
-drwxr-xr-x   0 cogljj   (536925976) staff       (20)        0 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/TEAL/src/
--rw-r--r--   0 cogljj   (536925976) staff       (20)     2271 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/Amortization.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)    10994 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/CashFlowPlot.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)     3498 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/CashFlowUser.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)     8325 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/CashFlow_ExtMod.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)    56753 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/CashFlows.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)      674 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/__init__.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)     1576 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/_utils.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)    33822 2022-11-16 17:46:01.000000 teal-ravenframework-0.3/TEAL/src/main.py
--rw-r--r--   0 cogljj   (536925976) staff       (20)       85 2022-11-16 17:45:04.000000 teal-ravenframework-0.3/pyproject.toml
--rw-r--r--   0 cogljj   (536925976) staff       (20)      396 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/setup.cfg
-drwxr-xr-x   0 cogljj   (536925976) staff       (20)        0 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/teal_ravenframework.egg-info/
--rw-r--r--   0 cogljj   (536925976) staff       (20)     1297 2022-11-16 17:51:04.000000 teal-ravenframework-0.3/teal_ravenframework.egg-info/PKG-INFO
--rw-r--r--   0 cogljj   (536925976) staff       (20)      497 2022-11-16 17:51:05.000000 teal-ravenframework-0.3/teal_ravenframework.egg-info/SOURCES.txt
--rw-r--r--   0 cogljj   (536925976) staff       (20)        1 2022-11-16 17:51:04.000000 teal-ravenframework-0.3/teal_ravenframework.egg-info/dependency_links.txt
--rw-r--r--   0 cogljj   (536925976) staff       (20)       45 2022-11-16 17:51:04.000000 teal-ravenframework-0.3/teal_ravenframework.egg-info/requires.txt
--rw-r--r--   0 cogljj   (536925976) staff       (20)       14 2022-11-16 17:51:04.000000 teal-ravenframework-0.3/teal_ravenframework.egg-info/top_level.txt
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 16:26:54.458829 teal-ravenframework-0.4/
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)       72 2022-05-23 16:43:56.000000 teal-ravenframework-0.4/MANIFEST.in
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1297 2023-05-22 16:26:54.458829 teal-ravenframework-0.4/PKG-INFO
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 16:26:54.455829 teal-ravenframework-0.4/TEAL/
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)    11356 2022-05-23 16:40:16.000000 teal-ravenframework-0.4/TEAL/LICENSE.txt
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)     1758 2022-05-23 16:40:16.000000 teal-ravenframework-0.4/TEAL/NOTICE.txt
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)     1127 2022-05-23 16:40:16.000000 teal-ravenframework-0.4/TEAL/README.md
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      800 2022-10-26 17:30:26.000000 teal-ravenframework-0.4/TEAL/__init__.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 16:26:54.457829 teal-ravenframework-0.4/TEAL/src/
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)     2271 2022-05-23 16:40:16.000000 teal-ravenframework-0.4/TEAL/src/Amortization.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    10994 2022-10-26 17:30:26.000000 teal-ravenframework-0.4/TEAL/src/CashFlowPlot.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3498 2022-10-26 17:30:26.000000 teal-ravenframework-0.4/TEAL/src/CashFlowUser.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     8286 2023-05-22 16:24:20.000000 teal-ravenframework-0.4/TEAL/src/CashFlow_ExtMod.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    58385 2023-05-22 16:24:20.000000 teal-ravenframework-0.4/TEAL/src/CashFlows.py
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)      674 2022-05-23 16:40:16.000000 teal-ravenframework-0.4/TEAL/src/__init__.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1576 2022-10-26 17:30:26.000000 teal-ravenframework-0.4/TEAL/src/_utils.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    33664 2023-05-22 16:24:20.000000 teal-ravenframework-0.4/TEAL/src/main.py
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)       85 2022-05-23 16:42:03.000000 teal-ravenframework-0.4/pyproject.toml
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      388 2023-05-22 16:26:54.459829 teal-ravenframework-0.4/setup.cfg
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 16:26:54.458829 teal-ravenframework-0.4/teal_ravenframework.egg-info/
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)     1297 2023-05-22 16:26:54.000000 teal-ravenframework-0.4/teal_ravenframework.egg-info/PKG-INFO
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)      497 2023-05-22 16:26:54.000000 teal-ravenframework-0.4/teal_ravenframework.egg-info/SOURCES.txt
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)        1 2023-05-22 16:26:54.000000 teal-ravenframework-0.4/teal_ravenframework.egg-info/dependency_links.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       37 2023-05-22 16:26:54.000000 teal-ravenframework-0.4/teal_ravenframework.egg-info/requires.txt
+-rw-rw-r--   0 jjc       (1000) jjc       (1000)       14 2023-05-22 16:26:54.000000 teal-ravenframework-0.4/teal_ravenframework.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `teal-ravenframework-0.3/PKG-INFO` & `teal-ravenframework-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: teal-ravenframework
-Version: 0.3
+Version: 0.4
 Summary: TEAL plugin for RAVEN framework
 Home-page: https://github.com/idaholab/TEAL
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 
 ![TEAL Logo](./logos/TEAL_LOGO_FULL.png)
 
 TEAL (Tool for Economic AnaLysis) is RAVEN plugin aimed to
 contain and deploy economic analysis for RAVEN workflows.
 
 It leverages the Uncertanty Quantification, Probabilistic Risk Assesment,
```

### Comparing `teal-ravenframework-0.3/TEAL/LICENSE.txt` & `teal-ravenframework-0.4/TEAL/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/NOTICE.txt` & `teal-ravenframework-0.4/TEAL/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/README.md` & `teal-ravenframework-0.4/TEAL/README.md`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/__init__.py` & `teal-ravenframework-0.4/TEAL/__init__.py`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/src/Amortization.py` & `teal-ravenframework-0.4/TEAL/src/Amortization.py`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/src/CashFlowPlot.py` & `teal-ravenframework-0.4/TEAL/src/CashFlowPlot.py`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/src/CashFlowUser.py` & `teal-ravenframework-0.4/TEAL/src/CashFlowUser.py`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/src/CashFlow_ExtMod.py` & `teal-ravenframework-0.4/TEAL/src/CashFlow_ExtMod.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,41 +81,39 @@
       @ Out, None
     """
     globalSettings = container._globalSettings
     components = container._components
     metrics = main.run(globalSettings, components, Inputs)
 
     projectLife = main.getProjectLength(globalSettings, components)
-    if metrics['outputType'] == True:
+    if metrics['outputType']:
       for k, v in metrics.items():
         if k == "all_data":
           for comp,cfs in v.items():
             for cf, data in cfs.items():
-              if cf.find('depreciate') >0 :
-                setattr(container, f'{comp}_Depreciate', data)
-              elif cf.find('amortize') > 0 :
-                setattr(container, f'{comp}_Amortize', data)
+              if cf.find('depreciation_tax_credit') > 0:
+                setattr(container, f'{comp}_depreciation_tax_credit', data)
+              elif cf.find('depreciation') > 0:
+                setattr(container, f'{comp}_depreciation', data)
               else:
                 setattr(container, f'{comp}_{cf}_CashFlow', data)
         else:
           blank = []
           blank.append(v)
           for x in range(projectLife-1):
             blank.append(0)
           blank = np.array(blank)
           setattr(container, f'{k}', blank)
     else:
-          for k, v in metrics.items():
-            if k == 'outputType':
-              nothing = 1
-            else:
-              setattr(container, k, v)
+      for k, v in metrics.items():
+        if k != 'outputType':
+          setattr(container, k, v)
 
 
-    container.cfYears = np.asarray(range(projectLife))
+    container.cfYears = np.arange(projectLife)
 
 
 
 
   # =====================================================================================================================
```

### Comparing `teal-ravenframework-0.3/TEAL/src/CashFlows.py` & `teal-ravenframework-0.4/TEAL/src/CashFlows.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,30 @@
     """
       Get output type
       @ In, None
       @ Out, self._outputType, Boolean, output type
     """
     return self._outputType
 
+  def getVerbosity(self):
+    """
+      Set verbosity level
+      @ In, v, float, Verbosity level between 0 and 100
+      @ Out, None
+    """
+    return self._verbosity
+
+  def setVerbosity(self, v):
+    """
+      Set verbosity level
+      @ In, v, float, Verbosity level between 0 and 100
+      @ Out, None
+    """
+    assert 0<=v<=100, "Verbosity level is not between 0 and 100"
+    self._verbosity = v
 
 class Component:
   """
     Just a holder for multiple cash flows, and methods for doing stuff with them
     Note the class can be constructed by reading from the XML (readInput) or directly TODO consistency
   """
   nodeVarMap = {'Life_time': '_lifetime',
@@ -557,37 +573,34 @@
       @ In, ocf, instant of CashFlow, instant of CashFlow object
       @ Out, depreciation, list, [pos, neg], list amortization and depreciation objects
     """
     # use the reference plant price
     amort = ocf.getAmortization()
     if amort is None:
       return []
-    print('DEBUGG amortizing cf:', ocf.name)
-    originalValue = ocf.getParam('alpha') * -1.0 #start with a positive value
     scheme, plan = amort
     alpha = Amortization.amortize(scheme, plan, 1.0, self._lifetime)
     # first cash flow is POSITIVE on the balance sheet, is not taxed, and is a percent of the target
-    pos = Amortizor(component=self.name, verbosity=self._verbosity)
-    params = {'name': '{}_{}_{}'.format(self.name, 'amortize', ocf.name),
+    # -> this is the tax credit from MACRS for component value loss
+    pos = Amortizor(credit=True, component=self.name, verbosity=self._verbosity, pos=True)
+    params = {'name': f'{self.name}_{ocf.name}_{"depreciation_tax_credit"}',
               'driver': '{}|{}'.format(self.name, ocf.name),
               'tax': False,
               'inflation': 'real',
               'alpha': alpha,
-              # TODO is this reference and X right????
-              'reference': 1.0, #ocf.getParam('reference'),
-              'X': 1.0, #ocf.getParam('scale')
+              'reference': 1.0,
+              'X': 1.0,
               }
     pos.setParams(params)
     # second cash flow is as the first, except negative and taxed
-    neg = Amortizor(component=self.name, verbosity=self._verbosity)
+    # -> this is the MACRS-based loss of value of the component
+    neg = Amortizor(credit=False, component=self.name, verbosity=self._verbosity)
     nalpha = np.zeros(len(alpha))
     nalpha[alpha != 0] = -1
-    print('DEBUGG amort alpha:', alpha)
-    print('DEBUGG depre alpha:', nalpha)
-    params = {'name': '{}_{}_{}'.format(self.name, 'depreciate', ocf.name),
+    params = {'name': f'{self.name}_{ocf.name}_{"depreciation"}',
               'driver': '{}|{}'.format(self.name, pos.name),
               'tax': True,
               'inflation': 'real',
               'alpha': nalpha,
               'reference': 1.0,
               'X': 1.0}
     neg.setParams(params)
@@ -701,15 +714,15 @@
   def readInput(self, item):
     """
       Sets settings from input file
       @ In, item, InputData.ParameterInput, parsed specs from user
       @ Out, None
     """
     self.name = item.parameterValues['name']
-    print(' ... ... loading cash flow "{}"'.format(self.name))
+    print(f' ... ... loading cash flow "{self.name}"')
     # driver and alpha are specific to cashflow types # self._driver = item.parameterValues['driver']
     for key, value in item.parameterValues.items():
       if key == 'tax':
         self._taxable = value
       elif key == 'inflation':
         self._inflatable = value in ['True', 'real']
       elif key == 'mult_target':
@@ -834,19 +847,19 @@
     # multi-entry or single-entry?
     if len(value) == 1:
       # single entry should be either a float (price) or string (raven variable)
       value = value[0]
       if mathUtils.isAString(value) or mathUtils.isAFloatOrInt(value):
         ret = value
       else:
-        raise IOError('Unrecognized alpha/driver type: "{}" with type "{}"'.format(value, type(value)))
+        raise IOError(f'Unrecognized alpha/driver type: "{value}" with type "{type(value)}"')
     else:
       # should be floats; InputData assures the entries are the same type already
       if not mathUtils.isAFloatOrInt(value[0]):
-        raise IOError('Multiple non-number entries for alpha/driver found, but require either a single variable name or multiple float entries: {}'.format(value))
+        raise IOError(f'Multiple non-number entries for alpha/driver found, but require either a single variable name or multiple float entries: {value}')
       ret = np.asarray(value)
     return ret
 
   def loadFromVariables(self, need, variables, cashflows, lifetime):
     """
       Load the values of parameters from variables
       @ In, need, dict, the dict of parameters
@@ -860,15 +873,15 @@
       if mathUtils.isAString(source):
         # as a string, this is either from the variables or other cashflows
         # look in variables first
         value = variables.get(source, None)
         if value is None:
           # since not found in variables, try among cashflows
           if '|' not in source:
-            raise KeyError('Looking for variable "{}" to fill "{}" but not found among variables or other cashflows!'.format(source, name))
+            raise KeyError(f'Looking for variable "{source}" to fill "{name}" but not found among variables or other cashflows!')
           comp, cf = source.split('|')
           value = cashflows[comp][cf][:]
         need[name] = np.atleast_1d(value)
     # now, each is already a float or an array, so in case they're a float expand them
     ## NOTE this expects the correct keys (namely alpha, driver) to expand, right?
     need = self.extendParameters(need, lifetime)
     return need
@@ -879,14 +892,54 @@
       @ In, need, dict, the dict of parameters that need to extend
       @ In, lifetime, int, the given life time
       @ Out, None
     """
     # should be overwritten in the inheriting classes!
     raise NotImplementedError
 
+  def getDriver(self):
+    """
+      Get the driver for this component
+      @ In, None
+      @ Out, _driver, float | pyomo.Expression, quantity produced or "D" in cashflow
+    """
+    return self._driver
+
+  def getAlpha(self):
+    """
+      Get the alpha for this component
+      @ In, None
+      @ Out, _alpha, float | pyomo.Expression, price per quantity produced or "a" in cashflow
+    """
+    return self._alpha
+
+  def getReference(self):
+    """
+      Get the reference driver for this component
+      @ In, None
+      @ Out, _reference, float | pyomo.Expression, reference driver or "Dp" in cashflow
+    """
+    return self._reference
+
+  def getScale(self):
+    """
+      Get the economy of scale for this component
+      @ In, None
+      @ Out, _scale, float | pyomo.Expression, economy of scale or "x" in cashflow
+    """
+    return self._scale
+
+  def getYearlyCashflow(self):
+    """
+      Get the scale driver for this component
+      @ In, None
+      @ Out, _yearlyCashflow, float | pyomo.Expression, economy of scale or "x" in cashflow
+    """
+    # should be overwritten in the inheriting classes!
+    raise NotImplementedError
 
 class Capex(CashFlow):
   """
     Particular cashflow for infrequent large single expenditures
   """
   @classmethod
   def getInputSpecs(specs):
@@ -925,15 +978,14 @@
     """
       Constructor
       @ In, kwargs, dict, general keyword arguments
       @ Out, None
     """
     CashFlow.__init__(self, **kwargs)
     # new variables
-    self.type = 'Capex'
     self._amortScheme = None # amortization scheme for depreciating this capex
     self._amortPlan = None   # if scheme is MACRS, this is the years to recovery. Otherwise, vector percentages.
     # set defaults different from base class
     self.type = 'Capex'
     self._taxable = False    # capital investments are not taxed by default
 
   def readInput(self, item):
@@ -983,16 +1035,15 @@
     """
       Get amortization
       @ In, None
       @ Out, amortization, None or tuple, (amortizationScheme, amortizationPlan)
     """
     if self._amortScheme is None:
       return None
-    else:
-      return self._amortScheme, self._amortPlan
+    return self._amortScheme, self._amortPlan
 
   def setAmortization(self, scheme, plan):
     """
       Set amortization
       @ In, scheme, str, 'MACRS' or 'custom'
       @ In, plan, list, list of amortization values
       @ Out, None
@@ -1010,27 +1061,27 @@
     # for capex, both the Driver and Alpha are nonzero in year 1 and zero thereafter
     for name, value in toExtend.items():
       if name.lower() in ['alpha', 'driver']:
         if mathUtils.isAFloatOrInt(value):
           new = np.zeros(t)
           new[0] = float(value)
           toExtend[name] = new
-        elif type(value) in [list, np.ndarray]:
+        elif isinstance(value, (list, np.ndarray)):
           if len(value) == 1:
             if mathUtils.isAFloatOrInt(value[0]):
               new = np.zeros(t)
               new[0] = float(value)
               toExtend[name] = new
-            elif type(value) is str:
+            elif isinstance(value, str):
               continue
             else:
               listArray = [0]*t
               listArray[0] = value
               toExtend[name] = np.array(listArray)
-        elif type(value) is str:
+        elif isinstance(value, str):
           continue
         else:
           # the else is for any object type data. if other types require distinction, add new 'elif'
           listArray = [0]*t
           listArray[0] = value
           toExtend[name] = np.array(listArray)
     return toExtend
@@ -1085,22 +1136,17 @@
     for param in ['alpha', 'driver']:
       val = self.getParam(param)
       # if a string, then it's probably a variable, so don't check it now
       if mathUtils.isAString(val):
         continue
       # if it's valued, then it better be the same length as the lifetime (which is comp lifetime + 1)
       elif len(val) != lifetime:
-        preMsg = 'Component "{comp}" '.format(compName) if compName is not None else ''
-        raise IOError((preMsg + 'cashflow "{cf}" node <{param}> should have {correct} '+\
-                       'entries (1 + lifetime), but only found {found}!')
-                       .format(cf=self.name,
-                               correct=lifetime,
-                               param=param,
-                               found=len(val)))
-
+        preMsg = f'Component "{compName}" ' if compName is not None else ''
+        raise IOError((preMsg + f'cashflow "{self.name}" node <{param}> should have {lifetime} '+\
+                       f'entries (1 + lifetime), but only found {len(val)}!'))
 
 class Recurring(CashFlow):
   """
     Particular cashflow for yearly-consistent repeating expenditures
   """
 
   @classmethod
@@ -1154,23 +1200,23 @@
     if mult is None:
       mult = 1.0
     elif mathUtils.isAString(mult):
       raise NotImplementedError
     try:
       self._yearlyCashflow[year] = mult * (alpha * driver).sum() # +1 is for initial construct year
     except ValueError as e:
-      print('Error while computing yearly cash flow! Check alpha shape ({}) and driver shape ({})'.format(alpha.shape, driver.shape))
+      print(f'Error while computing yearly cash flow! Check alpha shape ({alpha.shape}) and driver shape ({driver.shape})')
       raise e
 
   def computeYearlyCashflow(self, alpha, driver):
     """
       Computes the yearly summary of recurring interactions, and sets them to self._yearlyCashflow
       Use this when you need to collapse one-point-per-year alpha and one-point-per-year driver
       into one-point-per-year summaries
-      Note this is more for once-per-year recurring cashflows
+      NOTE: this is more for once-per-year recurring cashflows
       @ In, alpha, np.array, array of "prices" (one entry per YEAR)
       @ In, driver, np.array, array of "quantities sold" (one entry per YEAR)
       @ Out, None
     """
     mult = self.getMultiplier()
     if mult is None:
       mult = 1.0
@@ -1222,64 +1268,80 @@
     # FIXME: we're going to integrate alpha * D over time (not year time, intrayear time)
     for name, value in toExtend.items():
       if name.lower() in ['alpha', 'driver']:
         if mathUtils.isAFloatOrInt(value):
           new = np.ones(t) * float(value)
           new[0] = 0
           toExtend[name] = new
-        elif type(value) in [list, np.ndarray]:
+        elif isinstance(value, (list, np.ndarray)):
           if len(value) == 1:
             if mathUtils.isAFloatOrInt(value[0]):
               new = np.ones(t) * float(value)
               new[0] = 0
               toExtend[name] = new
-            elif type(value) is str:
+            elif isinstance(value, str):
               continue
             else:
-              listArray = [0]*t
-              for i in range(len(listArray)):
-                listArray[i] = value
+              listArray = [value]*t
               listArray[0] = 0
               toExtend[name] = np.array(listArray)
           # Checking for scenario where alpha or driver do not match project length
           # having mismatched alpha and driver will cause an operand error later in the workflow
           elif 1 < len(value) < t or len(value) > t:
             correctedCoefs = np.zeros(t)
             # cycling through driver/alpha array starting from 1 since recurring cfs are 0 in year 0
             cycledCoefs = it.cycle(value[1:])
             correctedCoefs[1:] = [next(cycledCoefs) for _ in correctedCoefs[1:]]
             toExtend[name] = correctedCoefs
-        elif type(value) is str:
+        elif isinstance(value, str):
           continue
         else:
           # the else is for any object type data. if other types require distinction, add new 'elif'
-          listArray = [0]*t
-          for i in range(len(listArray)):
-            listArray[i] = value
+          listArray = [value]*t
           listArray[0] = 0
           toExtend[name] = np.array(listArray)
     return toExtend
 
+  def getYearlyCashflow(self):
+    """
+      Get the scale driver for this component
+      @ In, None
+      @ Out, _yearlyCashflow, float | pyomo.Expression, economy of scale or "x" in cashflow
+    """
+    return self._yearlyCashflow
 
 class Amortizor(Capex):
   """
     Particular cashflow for depreciation of capital expenditures
   """
+  def __init__(self, **kwargs):
+    """
+      Constructor
+      @ In, kwargs, dict, general keyword arguments
+      @ Out, None
+    """
+    try:
+      self._is_credit = kwargs['credit']
+    except KeyError as e:
+      raise RuntimeError('ERROR setting up TEAL Amortizor CashFlow: requires "credit" keyword but not found!') from e
+    assert mathUtils.isABoolean(self._is_credit)
+    Capex.__init__(self, **kwargs)
+
   def extendParameters(self, toExtend, t):
     """
       Extend values of parameters to the length of lifetime t
       @ In, toExtend, dict, the dict of parameters that need to extend
       @ In, t, int, the given life time
       @ Out, None
     """
     # unlike normal capex, for amortization we expand the driver to all nonzero entries and keep alpha as is
     # TODO forced driver values for now
     driver = toExtend['driver']
     # how we treat the driver depends on if this is the amortizer or the depreciator
-    if self.name.split('_')[-2] == 'amortize':
+    if self._is_credit:
       if not mathUtils.isAString(driver):
         toExtend['driver'] = np.ones(t) * driver[0] * -1.0
         toExtend['driver'][0] = 0.0
       for name, value in toExtend.items():
         if name.lower() in ['driver']:
           if mathUtils.isAFloatOrInt(value) or (len(value) == 1 and mathUtils.isAFloatOrInt(value[0])):
             new = np.zeros(t)
```

### Comparing `teal-ravenframework-0.3/TEAL/src/__init__.py` & `teal-ravenframework-0.4/TEAL/src/__init__.py`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/src/_utils.py` & `teal-ravenframework-0.4/TEAL/src/_utils.py`

 * *Files identical despite different names*

### Comparing `teal-ravenframework-0.3/TEAL/src/main.py` & `teal-ravenframework-0.4/TEAL/src/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,36 +46,36 @@
   components = []
   econ = xml.find('Economics')
   verb = int(econ.attrib.get('verbosity', 100))
   for node in econ:
     if node.tag == 'Global':
       globalSettings = CashFlows.GlobalSettings(**attr)
       globalSettings.readInput(node)
-      globalSettings._verbosity = verb
+      globalSettings.setVerbosity(verb)
     elif node.tag == 'Component':
       new = CashFlows.Component(**attr)
       new.readInput(node)
       components.append(new)
     else:
-      raise IOError('Unrecognized node under <Economics>: {}'.format(node.tag))
+      raise IOError(f'Unrecognized node under <Economics>: {node.tag}')
   return globalSettings, components
 
 def checkRunSettings(settings, components):
   """
     Checks that basic settings between global and components are satisfied.
     Errors out if any problems are found.
     @ In, settings, CashFlows.GlobalSettings, global settings
     @ In, components, list, list of CashFlows.Component instances
     @ Out, None
   """
   compByName = dict((c.name, c) for c in components)
   # perform final checks for the global settings and components
   for find, find_cf in settings.getActiveComponents().items():
     if find not in compByName:
-      raise IOError('Requested active component "{}" but not found! Options are: {}'.format(find, list(compByName.keys())))
+      raise IOError(f'Requested active component "{find}" but not found! Options are: {list(compByName.keys())}')
     # check cash flow is in comp
   # check that StartTime/Repetitions triggers a ProjectTime node
   ## if projecttime is not given, then error if start time/repetitions given (otherwise answer is misleading)
   if settings.getProjectTime() is None:
     for comp in components:
       warn = 'TEAL: <{node}> given for component "{comp}" but no <ProjectTime> in global settings!'
       if comp.getStartTime() != 0:
@@ -121,21 +121,21 @@
     lifetime = comp.getLifetime()
     # find multiplier variables
     multipliers = comp.getMultipliers()
     for mult in multipliers:
       if mult is None:
         continue
       if mult not in variables.keys():
-        raise RuntimeError('CashFlow: multiplier "{}" required for Component "{}" but not found among variables!'.format(mult, comp.name))
+        raise RuntimeError(f'CashFlow: multiplier "{mult}" required for Component "{comp.name}" but not found among variables!')
     # find order in which to evaluate cash flow components
     for c, cf in enumerate(comp.getCashflows()):
       # keys for graph are drivers, cash flow names
       driver = cf.getParam('driver')
       # does the driver come from the variable list, or from another cashflow, or is it already evaluated?
-      cfn = '{}|{}'.format(comp.name, cf.name)
+      cfn = f'{comp.name}|{cf.name}'
       found = False
       if driver is None or mathUtils.isAFloatOrInt(driver) or isinstance(driver, np.ndarray) or pyomoVar:
         found = True
         # TODO assert it's already filled?
         evaluated.append(cfn)
         continue
       elif driver in variables:
@@ -192,15 +192,15 @@
     @ In, projectLife, int, length of project in years
     @ In, v, int, verbosity
     @ In, pyomoVar, boolean, if True, indicates that an expression will be constructed instead of a value calculated
     @ Out, lifeCashflow, np.array, array of cashflow values with length of component life
   """
   m = 'compLife'
   vprint(v, 1, m, "-"*75)
-  vprint(v, 1, m, 'Computing LIFETIME cash flow for Component "{}" CashFlow "{}" ...'.format(comp.name, cf.name))
+  vprint(v, 1, m, f'Computing LIFETIME cash flow for Component "{comp.name}" CashFlow "{cf.name}" ...')
   paramText = '... {:^10.10s}: {: 1.9e}'
   # do cashflow
   # necessary to handle recurring and capex with different timelines
   ### TODO consider scenario where rebuilds times comp life is less than project life
   if cf.type == 'Recurring':
     results = cf.calculateCashflow(variables, lifetimeCashflows, projectLife, v)
   else:
@@ -217,20 +217,20 @@
       else:
         orig = cf.getParam(item)
         if mathUtils.isSingleValued(orig):
           name = orig
         else:
           name = '(from input)'
         if not pyomoVar:
-          vprint(v, 1, m, '... {:^10.10s}: {}'.format(item, name))
-          vprint(v, 1, m, '...           mean: {: 1.9e}'.format(value.mean()))
-          vprint(v, 1, m, '...           std : {: 1.9e}'.format(value.std()))
-          vprint(v, 1, m, '...           min : {: 1.9e}'.format(value.min()))
-          vprint(v, 1, m, '...           max : {: 1.9e}'.format(value.max()))
-          vprint(v, 1, m, '...           nonz: {:d}'.format(np.count_nonzero(value)))
+          vprint(v, 1, m, f'... {item:^10.10s}: {name}')
+          vprint(v, 1, m, f'...           mean: {value.mean():1.9e}')
+          vprint(v, 1, m, f'...           std : {value.std():1.9e}')
+          vprint(v, 1, m, f'...           min : {value.min():1.9e}')
+          vprint(v, 1, m, f'...           max : {value.max():1.9e}')
+          vprint(v, 1, m, f'...           nonz: {np.count_nonzero(value):d}')
         else:
           continue
 
     yx = max(len(str(len(lifeCashflow))),4)
     vprint(v, 0, m, 'LIFETIME cash flow summary by year:')
     vprint(v, 0, m, '    {y:^{yx}.{yx}s}, {a:^10.10s}, {d:^10.10s}, {c:^15.15s}'.format(y='year',
                                                                                         yx=yx,
@@ -310,51 +310,51 @@
     @ In, projectLength, int, project years
     @ In, v, int, verbosity level
     @ In, pyomoVar, boolean, if True, indicates that an expression will be constructed instead of a value calculated
     @ Out, cashflows, dict, dictionary of cashflows for this component, taken to project life
   """
   m = 'proj comp'
   vprint(v, 1, m, "-"*75)
-  vprint(v, 1, m, 'Computing PROJECT cash flow for Component "{}" ...'.format(comp.name))
+  vprint(v, 1, m, f'Computing PROJECT cash flow for Component "{comp.name}" ...')
   cashflows = {}
   # what is the first project year this component will be in existence?
   compStart = comp.getStartTime()
   # how long does each build of this component last?
   compLife = comp.getLifetime()
   # what is the last project year this component will be in existence?
   ## TODO will this work properly if start time is negative? Initial tests say yes ...
   ## note that we use projectLength as the default END of the component's cashflow life, NOT a decomission year!
   compEnd = projectLength if comp.getRepetitions() == 0 else compStart + compLife * comp.getRepetitions()
-  vprint(v, 1, m, ' ... component start: {}'.format(compStart))
-  vprint(v, 1, m, ' ... component end:   {}'.format(compEnd))
+  vprint(v, 1, m, f' ... component start: {compStart}')
+  vprint(v, 1, m, f' ... component end:   {compEnd}')
   for cf in comp.getCashflows():
     if cf.isTaxable():
       taxMult = 1.0 - tax
     else:
       taxMult = 1.0
     if cf.isInflated():
       inflRate = inflation + 1.0
     else:
       inflRate = 1.0 # TODO nominal inflation rate?
-    vprint(v, 1, m, ' ... inflation rate: {}'.format(inflRate))
-    vprint(v, 1, m, ' ... tax rate: {}'.format(taxMult))
+    vprint(v, 1, m, f' ... inflation rate: {inflRate}')
+    vprint(v, 1, m, f' ... tax rate: {taxMult}')
     lifeCf = lifeCashflows[cf.name]
     # Recurring cashflows should only be handled on project lifetimes, not on component lifes
     if cf.type == 'Recurring':
       singleCashflow = projectRecurringCashflow(cf, compStart, compEnd, lifeCf, taxMult, inflRate, projectLength, v=v, pyomoVar=pyomoVar)
     else:
       singleCashflow = projectSingleCashflow(cf, compStart, compEnd, compLife, lifeCf, taxMult, inflRate, projectLength, v=v, pyomoVar=pyomoVar)
-    vprint(v, 0, m, 'Project Cashflow for Component "{}" CashFlow "{}":'.format(comp.name, cf.name))
+    vprint(v, 0, m, f'Project Cashflow for Component "{comp.name}" CashFlow "{cf.name}":')
     if v < 1:
       vprint(v, 0, m, 'Year, Time-Adjusted Value')
       for y, val in enumerate(singleCashflow):
         if not pyomoVar:
-          vprint(v, 0, m, '{:4d}: {: 1.9e}'.format(y, val))
+          vprint(v, 0, m, f'{y:4d}: {val: 1.9e}')
         else:
-          vprint(v, 0, m, '{:4d}: {:}'.format(y, type(val)))
+          vprint(v, 0, m, f'{y:4d}: {type(val):}')
     cashflows[cf.name] = singleCashflow
 
   return cashflows
 
 def projectRecurringCashflow(cf, start, end, lifeCf, taxMult, inflRate, projectLength, v=100, pyomoVar=False):
   """
     Handles recurring cashflows independent of component life times
@@ -367,28 +367,28 @@
     @ In, projectLength, int, total years of analysis
     @ In, v, int, verbosity
     @ In, pyomoVar, boolean, if True, indicates that an expression will be constructed instead of a value calculated
     @ Out, projCf, np.array, cashflow for project life of component
   """
   m = 'proj c_fl'
   vprint(v, 1, m, "-"*50)
-  vprint(v, 1, m, 'Computing PROJECT cash flow for CashFlow "{}" ...'.format(cf.name))
-  if pyomoVar == False:
+  vprint(v, 1, m, f'Computing PROJECT cash flow for CashFlow "{cf.name}" ...')
+  if not pyomoVar:
     projCf = np.zeros(projectLength)
   else:
     projCf = np.zeros(projectLength, dtype=object)
   years = np.arange(projectLength) # years in project time, year 0 is first year # TODO just indices, pandas?
   operatingMask = np.logical_and(years >= start, years < end)
   operatingYears = years[operatingMask]
   # This considers components that dont start operation until later in the project
   # It is neccessary to index lifeCf from 0 while still indexing projCf and years from current project year
   relativeStartupYear = operatingYears - start
-  for year in range(len(operatingYears)):
+  for o,opYear in enumerate(operatingYears):
     # Necessary to discount the cashflow with tax and inflation, for recurring inflRate is typically 1
-    projCf[operatingYears[year]] = lifeCf[relativeStartupYear[year]] * taxMult * np.power(inflRate, -1*years[operatingYears[year]])
+    projCf[opYear] = lifeCf[relativeStartupYear[o]] * taxMult * np.power(inflRate, -1*years[opYear])
   return projCf
 
 def projectSingleCashflow(cf, start, end, life, lifeCf, taxMult, inflRate, projectLength, v=100, pyomoVar=False):
   """
     does a single cashflow for the life of the project
     @ In, cf, CashFlows.CashFlow, cash flow to extend to full project life
     @ In, start, int, project year in which component begins operating
@@ -400,16 +400,16 @@
     @ In, projectLength, int, total years of analysis
     @ In, v, int, verbosity
     @ In, pyomoVar, boolean, if True, indicates that an expression will be constructed instead of a value calculated
     @ Out, projCf, np.array, cashflow for project life of component
   """
   m = 'proj c_fl'
   vprint(v, 1, m, "-"*50)
-  vprint(v, 1, m, 'Computing PROJECT cash flow for CashFlow "{}" ...'.format(cf.name))
-  if pyomoVar == False:
+  vprint(v, 1, m, f'Computing PROJECT cash flow for CashFlow "{cf.name}" ...')
+  if not pyomoVar:
     projCf = np.zeros(projectLength)
   else:
     projCf = np.zeros(projectLength, dtype=object)
   years = np.arange(projectLength) # years in project time, year 0 is first year # TODO just indices, pandas?
   # before the project starts, after it ends are zero; we want the working part
   # ALFOA: Modified following expression (see issue #20):
   #        from operatingMask = np.logical_and(years >= start, years <= end)
@@ -478,20 +478,20 @@
       discounted = np.sum(data/discountRates)
       if cf.isMultTarget():
         multiplied += discounted
       else:
         others += discounted
   targetVal = settings.getMetricTarget()
   mult = (targetVal - others)/multiplied # TODO div zero possible?
-  vprint(v, 0, m, '... NPV multiplier: {: 1.9e}'.format(mult))
+  vprint(v, 0, m, f'... NPV multiplier: {mult:1.9e}')
   # SANITY CHECL -> FCFF with the multiplier, re-calculate NPV
   if v < 1:
     npv = NPV(components, cashFlows, projectLength, settings.getDiscountRate(), mult=mult, v=v)
     if npv != targetVal:
-      vprint(v, 1, m, 'NPV mismatch warning! Calculated NPV with mult: {: 1.9e}, target: {: 1.9e}'.format(npv, targetVal))
+      vprint(v, 1, m, f'NPV mismatch warning! Calculated NPV with mult: {npv:1.9e}, target: {targetVal:1.9e}')
   return mult
 
 def FCFF(components, cashFlows, projectLength, mult=None, v=100, pyomoVar=False):
   """
     Calculates "free cash flow to the firm" (FCFF)
     @ In, settings, CashFlows.GlobalSettings, global settings
     @ In, cashFlows, dict, component: cashflow: np.array of annual economic values
@@ -506,26 +506,23 @@
   if not pyomoVar:
     fcff = np.zeros(projectLength)
   else:
     fcff = np.zeros(projectLength, dtype=object)
   for comp in components:
     for cf in comp.getCashflows():
       data = cashFlows[comp.name][cf.name]
-      for i in range(len(fcff)):
-        if mult is not None and cf.isMultTarget():
-          fcff[i] += data[i] * mult
-        else:
-          fcff[i] += data[i]
+      need_to_multiply = mult is not None and cf.isMultTarget()
+      fcff = [fcff[i] + data[i] * mult if need_to_multiply else fcff[i] + data[i] for i in range(len(fcff))]
   if not pyomoVar:
-    vprint(v, 1, m, 'FCFF yearly (not discounted):\n{}'.format(fcff))
+    vprint(v, 1, m, f'FCFF yearly (not discounted):\n{fcff}')
   else:
     vprint(v, 1, m, 'FCFF yearly (not discounted):')
     vprint(v, 1, m, 'year, FCFF')
     for year, value in zip(range(projectLength+1), fcff):
-      vprint(v, 1, m, '{:}: {:}'.format(year, type(value)))
+      vprint(v, 1, m, f'{year}: {type(value)}')
   return fcff
 
 def NPV(components, cashFlows, projectLength, discountRate, mult=None, v=100, pyomoVar=False, returnFcff=False):
   """
     Calculates net present value of cash flows
     @ In, components, list, list of CashFlows.Component instances
     @ In, cashFlows, dict, component: cashflow: np.array of annual economic values
@@ -538,35 +535,34 @@
     @ Out, npv, float, net-present value of system
     @ Out, fcff, float, optional, free cash flow to the firm for same system
   """
   m = 'NPV'
   fcff = FCFF(components, cashFlows, projectLength, mult=mult, v=v, pyomoVar=pyomoVar)
   npv = npf.npv(discountRate, fcff)
   if not pyomoVar:
-    vprint(v, 0, m, '... NPV: {: 1.9e}'.format(npv))
+    vprint(v, 0, m, f'... NPV: {npv:1.9e}')
   else:
-    vprint(v, 0, m, '... NPV: {:}'.format(type(npv)))
+    vprint(v, 0, m, f'... NPV: {type(npv)}')
   if not returnFcff:
     return npv
-  else:
-    return npv, fcff
+  return npv, fcff
 
 def IRR(components, cashFlows, projectLength, v=100):
   """
     Calculates internal rate of return for system of cash flows
     @ In, components, list, list of CashFlows.Component instances
     @ In, cashFlows, dict, component: cashflow: np.array of annual economic values
     @ In, projectLength, int, project years
     @ In, v, int, verbosity level
     @ Out, irr, float, internal rate of return
   """
   m = 'IRR'
   fcff = FCFF(components, cashFlows, projectLength, mult=None, v=v) # TODO mult is none always?
   irr = npf.irr(fcff)
-  vprint(v, 1, m, '... IRR: {: 1.9e}'.format(irr))
+  vprint(v, 1, m, f'... IRR: {irr:1.9e}')
   return irr
 
 def PI(components, cashFlows, projectLength, discountRate, mult=None, v=100):
   """
     Calculates the profitability index for system
     @ In, components, list, list of CashFlows.Component instances
     @ In, cashFlows, dict, component: cash flow: np.array of annual economic values
@@ -575,15 +571,15 @@
     @ In, mult, float, optional, if provided then scale target cash flow by value
     @ In, v, int, verbosity level
     @ Out, pi, float, profitability index
   """
   m = 'PI'
   npv, fcff = NPV(components, cashFlows, projectLength, discountRate, mult=mult, v=v, returnFcff=True)
   pi = -1.0 * npv / fcff[0] # yes, really! This seems strange, but it also seems to be right.
-  vprint(v, 1, m, '... PI: {: 1.9e}'.format(pi))
+  vprint(v, 1, m, f'... PI: {pi:1.9e}')
   return pi
 
 def gcd(a, b):
   """
     Find greatest common denominator
     @ In, a, int, first value
     @ In, b, int, sescond value
@@ -619,15 +615,15 @@
     @ In, components, list, list of CashFlows.Component instances
     @ In, variables, dict, variables from RAVEN
     @ In, pyomoVar, boolean, if True, indicates that an expression will be constructed instead of a value calculated
     @ Out, results, dict, economic metric results
   """
   # make a dictionary mapping component names to components
   compsByName = dict((c.name, c) for c in components)
-  v = settings._verbosity
+  v = settings.getVerbosity()
   m = 'run'
   vprint(v, 0, m, 'Starting CashFlow Run ...')
   # check mapping of drivers and determine order in which they should be evaluated
   vprint(v, 0, m, '... Checking if all drivers present ...')
   ordered = checkDrivers(settings, components, variables, v=v, pyomoVar=pyomoVar)
 
   # compute project cashflows
@@ -656,15 +652,15 @@
     lifeCf = componentLifeCashflow(comp, cf, variables, lifetimeCashflows, projectLife, v=0, pyomoVar=pyomoVar)
     lifetimeCashflows[compName][cfName] = lifeCf
   vprint(v, 0, m, '='*90)
   vprint(v, 0, m, 'Project Lifetime Cashflow Calculations')
   vprint(v, 0, m, '='*90)
   # determine how the project life is calculated.
   projectLength = getProjectLength(settings, components, v=v)
-  vprint(v, 0, m, ' ... project length: {} years'.format(projectLength))
+  vprint(v, 0, m, f' ... project length: {projectLength} years')
   projectCashflows = projectLifeCashflows(settings, components, lifetimeCashflows, projectLength, v=v, pyomoVar=pyomoVar)
   # preserve cashflows by component so they're reportable as outputs
 
   vprint(v, 0, m, '='*90)
   vprint(v, 0, m, 'Economic Indicator Calculations')
   vprint(v, 0, m, '='*90)
   indicators = settings.getIndicators()
@@ -681,16 +677,20 @@
     metric = IRR(components, projectCashflows, projectLength, v=v)
     results['IRR'] = metric
   if 'PI' in indicators:
     metric = PI(components, projectCashflows, projectLength, settings.getDiscountRate(), v=v)
     results['PI'] = metric
   results['outputType'] = outputType
 
-  if outputType is True:
+  if outputType:
     results["all_data"] = projectCashflows
+    print('DEBUGG all data:')
+    for comp, cval in projectCashflows.items():
+      for cf, cfval in cval.items():
+        print('DEBUGG ...in CF', cf, len(cfval))
 
   return results
 
 
 #=====================
 # PRINTING STUFF
 #=====================
@@ -700,8 +700,8 @@
     @ In, threshold, int, cutoff verbosity
     @ In, desired, int, requested message verbosity level
     @ In, method, str, name of method raising print
     @ In, msg, list(str), messages to print
     @ Out, None
   """
   if desired >= threshold:
-    print('CashFlow INFO ({}):'.format(method), *msg)
+    print(f'CashFlow INFO ({method}):', *msg)
```

### Comparing `teal-ravenframework-0.3/teal_ravenframework.egg-info/PKG-INFO` & `teal-ravenframework-0.4/teal_ravenframework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: teal-ravenframework
-Version: 0.3
+Version: 0.4
 Summary: TEAL plugin for RAVEN framework
 Home-page: https://github.com/idaholab/TEAL
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 
 ![TEAL Logo](./logos/TEAL_LOGO_FULL.png)
 
 TEAL (Tool for Economic AnaLysis) is RAVEN plugin aimed to
 contain and deploy economic analysis for RAVEN workflows.
 
 It leverages the Uncertanty Quantification, Probabilistic Risk Assesment,
```

