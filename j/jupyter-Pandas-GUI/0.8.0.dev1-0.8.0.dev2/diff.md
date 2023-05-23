# Comparing `tmp/jupyter_Pandas_GUI-0.8.0.dev1.tar.gz` & `tmp/jupyter_Pandas_GUI-0.8.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev1.tar", last modified: Tue May 23 00:47:05 2023, max compression
+gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev2.tar", last modified: Tue May 23 15:11:05 2023, max compression
```

## Comparing `jupyter_Pandas_GUI-0.8.0.dev1.tar` & `jupyter_Pandas_GUI-0.8.0.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev1/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8312 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev1/README.md
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 00:47:05.625321 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/top_level.txt
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49764 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/fit_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/new_pandas_column_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/plot_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14289 2023-05-23 00:40:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1325 2023-05-23 00:46:37.000000 jupyter_Pandas_GUI-0.8.0.dev1/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 15:11:05.915628 jupyter_Pandas_GUI-0.8.0.dev2/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev2/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 15:11:05.915628 jupyter_Pandas_GUI-0.8.0.dev2/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8312 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev2/README.md
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 15:11:05.915628 jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 15:11:05.000000 jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-23 15:11:05.000000 jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-23 15:11:05.000000 jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-23 15:11:05.000000 jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-23 15:11:05.000000 jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 15:11:05.915628 jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49923 2023-05-23 14:11:00.000000 jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/fit_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/new_pandas_column_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/plot_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14308 2023-05-23 14:40:09.000000 jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-23 15:11:05.915628 jupyter_Pandas_GUI-0.8.0.dev2/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1325 2023-05-23 15:10:49.000000 jupyter_Pandas_GUI-0.8.0.dev2/setup.py
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/LICENSE` & `jupyter_Pandas_GUI-0.8.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_Pandas_GUI
-Version: 0.8.0.dev1
+Version: 0.8.0.dev2
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/README.md` & `jupyter_Pandas_GUI-0.8.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev2/jupyter_Pandas_GUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-Pandas-GUI
-Version: 0.8.0.dev1
+Version: 0.8.0.dev2
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/__init__.py` & `jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/fit_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/fit_Pandas_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                      r'where $\color{red}{A}$ = ' \
                      r'amplitude, $\color{red}{f}$ = frequency, '\
                      r'$\color{red}{\phi}$ = shift'
     }
 
     def polymodelresultstr(resultname):
         template = '' \
-          'fitstr = \'$fit = \'\n' \
+          'fitstr = r\'$fit = \'\n' \
           'termcount = 0\n' \
           'for k in %result.params.keys():\n' \
           '    pwr = int(str(k)[-1:])\n' \
           '    if %result.params[k].vary:\n' \
           '        if termcount > 0:\n' \
           '            fitstr += \' + \'\n' \
           '        fitstr += \'(\\\color{red}{\'+rue.latex_rndwitherr(' \
@@ -151,17 +151,18 @@
                                          '%result.params[k].value)+\'})\'\n' \
           '            termcount +=1\n' \
           '            if pwr == 1:\n' \
           '                fitstr += \'x\'\n' \
           '            if pwr > 1:\n' \
           '                fitstr += \'x^\'+str(pwr)\n' \
           'fitstr+=\'$\'\n' \
-          'captionstr=\'<p>Use the command <code>%result</code> as the ' \
+          'captionstr=r\'<p>Use the command <code>%result</code> as the ' \
           'last line of a code cell for more details.</p>\'\n' \
-          'display(HTML(fitstr+captionstr))'
+          'display(Math(fitstr))\n' \
+          'display(HTML(captionstr))'
         return template.replace('%result', str(resultname))
 
     def linmodelresultstr(resultname):
         template = '' \
        'slopestr = ''\'\'\n' \
        'interceptstr = ''\'\'\n' \
        'for k in %results.params.keys():\n' \
@@ -175,18 +176,19 @@
                    'k].value,' \
                    '\n' \
        '                                       )+\'}\'\n' \
        '    if k == \'slope\':\n' \
        '        slopestr = paramstr\n' \
        '    if k == \'intercept\' and %results.params[k].value != 0:\n' \
        '        interceptstr = \' + \' + paramstr\n' \
-       'fitstr = \'$fit = \'+slopestr + \'x\' + interceptstr + \'$\'\n' \
-       'captionstr = \'<p>Use the command <code>%results</code> as the ' \
+       'fitstr = r\'$fit = \'+slopestr + \'x\' + interceptstr + \'$\'\n' \
+       'captionstr = r\'<p>Use the command <code>%results</code> as the ' \
        'last line of a code cell for more details.</p>\'\n' \
-       'display(HTML(fitstr+captionstr))'
+       'display(Math(fitstr))\n' \
+       'display(HTML(captionstr))'
         return template.replace('%results', resultname)
 
     def expmodelresultstr(resultname):
         template = '' \
         'ampstr = ''\'\'\n' \
         'decaystr = ''\'\'\n' \
         'for k in %results.params.keys():\n' \
@@ -201,17 +203,18 @@
         '                                       )+\'}\'\n' \
         '    if k == \'amplitude\':\n' \
         '        ampstr = paramstr\n' \
         '    if k == \'decay\':\n' \
         '        decaystr = paramstr\n' \
         'fitstr = r\'$$fit = \'+ampstr+r\'%EXP %LEFT( %FRAC{-x}' \
                         '{\'+decaystr+r\'}%RIGHT)$$\'\n' \
-        'captionstr = \'<p>Use the command <code>%results</code> as the ' \
+        'captionstr = r\'<p>Use the command <code>%results</code> as the ' \
         'last line of a code cell for more details.</p>\'\n' \
-        'display(HTML(fitstr+captionstr))'
+        'display(Math(fitstr))\n' \
+        'display(HTML(captionstr))'
         return template.replace('%results',resultname)
 
     def gausmodelresultstr(resultname):
         # TODO
         template = '' \
         'ampstr = ''\'\'\n' \
         'centstr = ''\'\'\n' \
@@ -232,17 +235,18 @@
         '        centstr = paramstr\n' \
         '    if k == \'sigma\':\n' \
         '        sigmastr = paramstr\n' \
         'fitstr = r\'$$fit = %FRAC{\'+ampstr+\'}{' \
                    '\'+sigmastr+r\'%SQRT{2%PI}}%EXP %LEFT( %FRAC{' \
                    '-%LEFT[x-\'+centstr+r\'%RIGHT]^2}' \
                    '{2\'+sigmastr+r\'^2}%RIGHT)$$\'\n' \
-        'captionstr = \'<p>Use the command <code>%results</code> as the ' \
+        'captionstr = r\'<p>Use the command <code>%results</code> as the ' \
         'last line of a code cell for more details.</p>\'\n' \
-        'display(HTML(fitstr+captionstr))'
+        'display(Math(fitstr))\n' \
+        'display(HTML(captionstr))'
         return template.replace('%results',resultname)
 
     def sinmodelresultstr(resultname):
         template = '' \
        'ampstr = \'\'\n' \
        'freqstr = \'\'\n' \
        'shiftstr = \'\'\n' \
@@ -257,18 +261,19 @@
                    ')+\'}\'\n' \
        '    if k == \'amplitude\':\n' \
        '        ampstr = paramstr\n' \
        '    if k == \'frequency\':\n' \
        '        freqstr = paramstr\n' \
        '    if k == \'shift\' and %results.params[k].value != 0:\n' \
        '        shiftstr = \' + \' + paramstr\n' \
-       'fitstr = \'$fit = \'+ampstr + \'sin[\' + freqstr + \'x\' + shiftstr + \']$\'\n' \
-       'captionstr = \'<p>Use the command <code>%results</code> as the ' \
+       'fitstr = r\'$fit = \'+ampstr + \'sin[\' + freqstr + \'x\' + shiftstr + \']$\'\n' \
+       'captionstr = r\'<p>Use the command <code>%results</code> as the ' \
        'last line of a code cell for more details.</p>\'\n' \
-       'display(HTML(fitstr+captionstr))'
+       'display(Math(fitstr))\n' \
+       'display(HTML(captionstr))'
         return template.replace('%results', resultname)
 
     fitresultstrs = {
     'LinearModel': linmodelresultstr,
     'PolynomialModel': polymodelresultstr,
     'ExponentialModel': expmodelresultstr,
     'GaussianModel': gausmodelresultstr,
@@ -279,15 +284,15 @@
                 'https://jupyterphysscilab.github.io/jupyter_Pandas_GUI.\n' \
                 '# Imports (no effect if already imported)\n' \
                 'import numpy as np\n' \
                 'import lmfit as lmfit\n' \
                 'import round_using_error as rue\n' \
                 'import copy as copy\n' \
                 'from plotly import graph_objects as go\n' \
-                'from IPython.display import HTML\n\n'
+                'from IPython.display import HTML, Math\n\n'
     step1str = ''
     step2str = ''
     step3str = ''
     step4str = ''
     step5str = ''
     step6str = ''
     range_chosen = False
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/new_pandas_column_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/new_pandas_column_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/plot_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/plot_Pandas_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/utils.py` & `jupyter_Pandas_GUI-0.8.0.dev2/pandas_GUI/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,17 +352,18 @@
             shell = get_ipython()
             output_elem.clear_output()
             with output_elem:
                 display(HTML(
                 '<details><summary style="cursor:pointer;"><span style="font-weight:bold;"><a>' \
                 'Code that was run</a></span>(click to toggle visibility)</summary>' \
                 '<div style="background:#eff0f1;white-space:pre-line;white-space:pre-wrap;">' \
-                '<pre>' + self.sniptext.value + '</pre></div></details>'))
+                '<code><xmp>' + self.sniptext.value
+                +'</xmp></code></div></details>'))
                 display(HTML('<h3>Result<h3>'))
-                display(exec(str(self.sniptext.value), shell.user_ns))
+                exec(str(self.sniptext.value), shell.user_ns)
             pass
 
         self.dobutton.on_click(onRunCode)
 
         super(build_run_snip_widget, self).__init__([self.sniptext,
                                              self.dobox],
                                             layout=Layout(
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev1/setup.py` & `jupyter_Pandas_GUI-0.8.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="jupyter_Pandas_GUI",
-    version="0.8.0dev1",
+    version="0.8.0dev2",
     description="Pandas expression composers using Jupyter widgets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="fitting, data-analysis, plotting, learning to code",
```

