# Comparing `tmp/cxwidgets-0.8.tar.gz` & `tmp/cxwidgets-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cxwidgets-0.8.tar", last modified: Tue Mar 16 12:51:56 2021, max compression
+gzip compressed data, was "dist/cxwidgets-0.9.tar", last modified: Fri Mar 19 11:11:45 2021, max compression
```

## Comparing `cxwidgets-0.8.tar` & `cxwidgets-0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-16 12:51:56.053983 cxwidgets-0.8/
--rw-rw-r--   0 femanov   (1000) femanov   (1001)      305 2021-03-16 12:51:56.053983 cxwidgets-0.8/PKG-INFO
-drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-16 12:51:56.049983 cxwidgets-0.8/cxwidgets/
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1329 2021-03-15 03:50:39.000000 cxwidgets-0.8/cxwidgets/__init__.py
-drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-16 12:51:56.053983 cxwidgets-0.8/cxwidgets/aQt/
--rw-r--r--   0 femanov   (1000) femanov   (1001)      113 2018-12-02 18:58:00.000000 cxwidgets-0.8/cxwidgets/aQt/QtCore.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      123 2018-12-02 18:58:00.000000 cxwidgets-0.8/cxwidgets/aQt/QtDesigner.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      113 2018-12-02 18:58:00.000000 cxwidgets-0.8/cxwidgets/aQt/QtGui.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      117 2018-12-02 18:58:00.000000 cxwidgets-0.8/cxwidgets/aQt/QtWidgets.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      624 2018-11-16 19:36:00.000000 cxwidgets-0.8/cxwidgets/aQt/__init__.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      109 2018-12-02 18:58:00.000000 cxwidgets-0.8/cxwidgets/aQt/uic.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1663 2021-03-13 19:23:45.000000 cxwidgets-0.8/cxwidgets/auxwidgets.py
--rwxr-xr-x   0 femanov   (1000) femanov   (1001)     9113 2019-11-26 08:13:00.000000 cxwidgets-0.8/cxwidgets/cx_bpm_plot.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1277 2021-03-15 03:33:53.000000 cxwidgets-0.8/cxwidgets/cx_checkbox.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     3545 2020-03-05 05:02:00.000000 cxwidgets-0.8/cxwidgets/cx_combobox.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1959 2021-03-14 15:27:26.000000 cxwidgets-0.8/cxwidgets/cx_doublespinbox.py
--rwxr-xr-x   0 femanov   (1000) femanov   (1001)      433 2020-10-29 05:29:00.000000 cxwidgets-0.8/cxwidgets/cx_historyplot.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1029 2021-03-15 03:55:53.000000 cxwidgets-0.8/cxwidgets/cx_label.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1037 2021-03-14 15:27:26.000000 cxwidgets-0.8/cxwidgets/cx_lcdnumber.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1865 2021-03-15 03:33:53.000000 cxwidgets-0.8/cxwidgets/cx_led.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1388 2020-02-21 17:11:00.000000 cxwidgets-0.8/cxwidgets/cx_lineedit.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     6985 2020-11-06 18:08:00.000000 cxwidgets-0.8/cxwidgets/cx_plot.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1148 2021-03-15 03:33:53.000000 cxwidgets-0.8/cxwidgets/cx_progressbar.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1153 2021-03-16 12:48:40.000000 cxwidgets-0.8/cxwidgets/cx_pushbutton.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1911 2021-03-16 07:19:47.000000 cxwidgets-0.8/cxwidgets/cx_spinbox.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     2874 2021-03-15 03:33:53.000000 cxwidgets-0.8/cxwidgets/cx_switch.py
--rwxr-xr-x   0 femanov   (1000) femanov   (1001)      847 2019-11-26 08:13:00.000000 cxwidgets-0.8/cxwidgets/cxw_demo.py
-drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-16 12:51:56.053983 cxwidgets-0.8/cxwidgets/menus/
--rw-r--r--   0 femanov   (1000) femanov   (1001)        0 2019-11-28 05:36:00.000000 cxwidgets-0.8/cxwidgets/menus/__init__.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1347 2021-03-12 11:08:43.000000 cxwidgets-0.8/cxwidgets/menus/doublespinbox_cm.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     3146 2021-03-16 12:45:29.000000 cxwidgets-0.8/cxwidgets/menus/general_cm.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     2182 2021-03-16 07:20:42.000000 cxwidgets-0.8/cxwidgets/menus/spinbox_cm.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      428 2020-02-21 17:11:00.000000 cxwidgets-0.8/cxwidgets/pcheckbox.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      573 2020-02-21 17:13:00.000000 cxwidgets-0.8/cxwidgets/pcombobox.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1481 2021-02-20 06:07:51.000000 cxwidgets-0.8/cxwidgets/pdoublespinbox.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)      150 2020-02-21 17:13:00.000000 cxwidgets-0.8/cxwidgets/plcdnumber.py
--rw-rw-r--   0 femanov   (1000) femanov   (1001)     3500 2021-03-12 15:52:30.000000 cxwidgets-0.8/cxwidgets/pledwidget.py
--rwxr-xr-x   0 femanov   (1000) femanov   (1001)     3414 2019-11-26 08:13:00.000000 cxwidgets-0.8/cxwidgets/plt_text.py
-drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-16 12:51:56.053983 cxwidgets-0.8/cxwidgets/plugins/
--rw-r--r--   0 femanov   (1000) femanov   (1001)        0 2019-11-28 05:36:00.000000 cxwidgets-0.8/cxwidgets/plugins/__init__.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     4839 2021-03-15 03:48:43.000000 cxwidgets-0.8/cxwidgets/plugins/cx_plugin.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     2003 2019-11-28 07:01:00.000000 cxwidgets-0.8/cxwidgets/plugins/p_plugin.py
--rw-r--r--   0 femanov   (1000) femanov   (1001)     1340 2021-02-20 06:09:34.000000 cxwidgets-0.8/cxwidgets/pspinbox.py
--rwxr-xr-x   0 femanov   (1000) femanov   (1001)     1697 2020-02-10 09:58:00.000000 cxwidgets-0.8/cxwidgets/pswitch.py
--rwxr-xr-x   0 femanov   (1000) femanov   (1001)      290 2018-08-22 08:34:00.000000 cxwidgets-0.8/cxwidgets/pw_demo.py
-drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-16 12:51:56.049983 cxwidgets-0.8/cxwidgets.egg-info/
--rw-rw-r--   0 femanov   (1000) femanov   (1001)      305 2021-03-16 12:51:55.000000 cxwidgets-0.8/cxwidgets.egg-info/PKG-INFO
--rw-rw-r--   0 femanov   (1000) femanov   (1001)     1129 2021-03-16 12:51:55.000000 cxwidgets-0.8/cxwidgets.egg-info/SOURCES.txt
--rw-rw-r--   0 femanov   (1000) femanov   (1001)        1 2021-03-16 12:51:55.000000 cxwidgets-0.8/cxwidgets.egg-info/dependency_links.txt
--rw-rw-r--   0 femanov   (1000) femanov   (1001)       10 2021-03-16 12:51:55.000000 cxwidgets-0.8/cxwidgets.egg-info/top_level.txt
--rw-rw-r--   0 femanov   (1000) femanov   (1001)       38 2021-03-16 12:51:56.053983 cxwidgets-0.8/setup.cfg
--rw-r--r--   0 femanov   (1000) femanov   (1001)      351 2021-03-16 12:51:13.000000 cxwidgets-0.8/setup.py
+drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-19 11:11:45.223056 cxwidgets-0.9/
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)      305 2021-03-19 11:11:45.223056 cxwidgets-0.9/PKG-INFO
+drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-19 11:11:45.219056 cxwidgets-0.9/cxwidgets/
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1697 2021-03-19 02:20:08.000000 cxwidgets-0.9/cxwidgets/__init__.py
+drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-19 11:11:45.219056 cxwidgets-0.9/cxwidgets/aQt/
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      113 2018-12-02 18:58:00.000000 cxwidgets-0.9/cxwidgets/aQt/QtCore.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      123 2018-12-02 18:58:00.000000 cxwidgets-0.9/cxwidgets/aQt/QtDesigner.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      113 2018-12-02 18:58:00.000000 cxwidgets-0.9/cxwidgets/aQt/QtGui.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      117 2018-12-02 18:58:00.000000 cxwidgets-0.9/cxwidgets/aQt/QtWidgets.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      624 2018-11-16 19:36:00.000000 cxwidgets-0.9/cxwidgets/aQt/__init__.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      109 2018-12-02 18:58:00.000000 cxwidgets-0.9/cxwidgets/aQt/uic.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1365 2021-03-18 04:06:21.000000 cxwidgets-0.9/cxwidgets/auxwidgets.py
+-rwxr-xr-x   0 femanov   (1000) femanov   (1001)     9113 2019-11-26 08:13:00.000000 cxwidgets-0.9/cxwidgets/cx_bpm_plot.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1277 2021-03-15 03:33:53.000000 cxwidgets-0.9/cxwidgets/cx_checkbox.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     3545 2020-03-05 05:02:00.000000 cxwidgets-0.9/cxwidgets/cx_combobox.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     2418 2021-03-19 10:47:42.000000 cxwidgets-0.9/cxwidgets/cx_doublespinbox.py
+-rwxr-xr-x   0 femanov   (1000) femanov   (1001)      433 2020-10-29 05:29:00.000000 cxwidgets-0.9/cxwidgets/cx_historyplot.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     3113 2021-03-19 08:53:09.000000 cxwidgets-0.9/cxwidgets/cx_label.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1037 2021-03-14 15:27:26.000000 cxwidgets-0.9/cxwidgets/cx_lcdnumber.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1865 2021-03-15 03:33:53.000000 cxwidgets-0.9/cxwidgets/cx_led.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1599 2021-03-18 10:24:17.000000 cxwidgets-0.9/cxwidgets/cx_lineedit.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     6985 2020-11-06 18:08:00.000000 cxwidgets-0.9/cxwidgets/cx_plot.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1148 2021-03-15 03:33:53.000000 cxwidgets-0.9/cxwidgets/cx_progressbar.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1153 2021-03-16 12:48:40.000000 cxwidgets-0.9/cxwidgets/cx_pushbutton.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1912 2021-03-19 10:37:10.000000 cxwidgets-0.9/cxwidgets/cx_spinbox.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     2874 2021-03-15 03:33:53.000000 cxwidgets-0.9/cxwidgets/cx_switch.py
+-rwxr-xr-x   0 femanov   (1000) femanov   (1001)      847 2019-11-26 08:13:00.000000 cxwidgets-0.9/cxwidgets/cxw_demo.py
+drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-19 11:11:45.223056 cxwidgets-0.9/cxwidgets/menus/
+-rw-r--r--   0 femanov   (1000) femanov   (1001)        0 2019-11-28 05:36:00.000000 cxwidgets-0.9/cxwidgets/menus/__init__.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     2522 2021-03-19 10:59:56.000000 cxwidgets-0.9/cxwidgets/menus/doublespinbox_cm.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     3525 2021-03-19 06:35:40.000000 cxwidgets-0.9/cxwidgets/menus/general_cm.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     2492 2021-03-19 10:37:10.000000 cxwidgets-0.9/cxwidgets/menus/spinbox_cm.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      428 2020-02-21 17:11:00.000000 cxwidgets-0.9/cxwidgets/pcheckbox.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      573 2020-02-21 17:13:00.000000 cxwidgets-0.9/cxwidgets/pcombobox.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1481 2021-02-20 06:07:51.000000 cxwidgets-0.9/cxwidgets/pdoublespinbox.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      150 2020-02-21 17:13:00.000000 cxwidgets-0.9/cxwidgets/plcdnumber.py
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)     3500 2021-03-12 15:52:30.000000 cxwidgets-0.9/cxwidgets/pledwidget.py
+-rwxr-xr-x   0 femanov   (1000) femanov   (1001)     3414 2019-11-26 08:13:00.000000 cxwidgets-0.9/cxwidgets/plt_text.py
+drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-19 11:11:45.223056 cxwidgets-0.9/cxwidgets/plugins/
+-rw-r--r--   0 femanov   (1000) femanov   (1001)        0 2019-11-28 05:36:00.000000 cxwidgets-0.9/cxwidgets/plugins/__init__.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     5581 2021-03-19 02:24:18.000000 cxwidgets-0.9/cxwidgets/plugins/cx_plugin.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     2003 2019-11-28 07:01:00.000000 cxwidgets-0.9/cxwidgets/plugins/p_plugin.py
+-rw-r--r--   0 femanov   (1000) femanov   (1001)     1340 2021-02-20 06:09:34.000000 cxwidgets-0.9/cxwidgets/pspinbox.py
+-rwxr-xr-x   0 femanov   (1000) femanov   (1001)     1697 2020-02-10 09:58:00.000000 cxwidgets-0.9/cxwidgets/pswitch.py
+-rwxr-xr-x   0 femanov   (1000) femanov   (1001)      290 2018-08-22 08:34:00.000000 cxwidgets-0.9/cxwidgets/pw_demo.py
+drwxrwxr-x   0 femanov   (1000) femanov   (1001)        0 2021-03-19 11:11:45.219056 cxwidgets-0.9/cxwidgets.egg-info/
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)      305 2021-03-19 11:11:44.000000 cxwidgets-0.9/cxwidgets.egg-info/PKG-INFO
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)     1129 2021-03-19 11:11:45.000000 cxwidgets-0.9/cxwidgets.egg-info/SOURCES.txt
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)        1 2021-03-19 11:11:44.000000 cxwidgets-0.9/cxwidgets.egg-info/dependency_links.txt
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)       10 2021-03-19 11:11:44.000000 cxwidgets-0.9/cxwidgets.egg-info/top_level.txt
+-rw-rw-r--   0 femanov   (1000) femanov   (1001)       38 2021-03-19 11:11:45.223056 cxwidgets-0.9/setup.cfg
+-rw-r--r--   0 femanov   (1000) femanov   (1001)      351 2021-03-19 10:55:57.000000 cxwidgets-0.9/setup.py
```

### Comparing `cxwidgets-0.8/cxwidgets/aQt/__init__.py` & `cxwidgets-0.9/cxwidgets/aQt/__init__.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_bpm_plot.py` & `cxwidgets-0.9/cxwidgets/cx_bpm_plot.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_checkbox.py` & `cxwidgets-0.9/cxwidgets/cx_checkbox.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_combobox.py` & `cxwidgets-0.9/cxwidgets/cx_combobox.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_doublespinbox.py` & `cxwidgets-0.9/cxwidgets/cx_doublespinbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,22 @@
        When value set - it's send to CX (set considered by done signal of PDoubleSpinbox).
        When CX updates value - it's set to spinbox value.
 
        attributes:
            cname - cx channel name. When changed
 
     """
-
     def __init__(self, parent=None, **kwargs):
         super().__init__(parent, **kwargs)
         self._cname = kwargs.get('cname', None)
         self.chan = None
         self.cx_connect()
         self.done.connect(self.cs_send)
+        self._hardmin = 0
+        self._hardmax = 0
 
     def contextMenuEvent(self, event):
         self.context_menu = CXDoubleSpinboxCM(self)
         self.context_menu.popup(event.globalPos())
 
     def cx_connect(self):
         if self._cname is None or self._cname == '':
@@ -56,7 +57,25 @@
         self.cx_connect()
 
     def getCname(self):
         return self._cname
 
     cname = pyqtProperty(str, getCname, setCname)
 
+    @pyqtSlot(float)
+    def set_hardmin(self, value):
+        self._hardmin = value
+
+    def get_hardmin(self):
+        return self._hardmin
+
+    hardmin = pyqtProperty(float, get_hardmin, set_hardmin)
+
+    @pyqtSlot(float)
+    def set_hardmax(self, value):
+        self._hardmax = value
+
+    def get_hardmax(self):
+        return self._hardmax
+
+    hardmax = pyqtProperty(float, get_hardmax, set_hardmax)
+
```

### Comparing `cxwidgets-0.8/cxwidgets/cx_label.py` & `cxwidgets-0.9/cxwidgets/cx_lcdnumber.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from cxwidgets.aQt.QtWidgets import QLCDNumber
 from cxwidgets.aQt.QtCore import pyqtSlot, pyqtProperty
-from cxwidgets.aQt.QtWidgets import QLabel
 import pycx4.qcda as cda
 from .menus.general_cm import CXGeneralCM
 
-class CXLabel(QLabel):
+
+class CXLCDNumber(QLCDNumber):
     def __init__(self, parent=None, **kwargs):
         super().__init__(parent)
         self._cname = kwargs.get('cname', None)
         self.chan = None
         self.cx_connect()
 
         self.context_menu = None
@@ -19,15 +20,15 @@
     def cx_connect(self):
         if self._cname is None or self._cname == '':
             return
         self.chan = cda.DChan(self._cname, private=True)
         self.chan.valueChanged.connect(self.cs_update)
 
     def cs_update(self, chan):
-        self.setText(str(chan.val))
+        self.display(chan.val)
 
     @pyqtSlot(float)
     def setCname(self, cname):
         self._cname = cname
         self.cx_connect()
 
     def getCname(self):
```

### Comparing `cxwidgets-0.8/cxwidgets/cx_lcdnumber.py` & `cxwidgets-0.9/cxwidgets/cx_progressbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-from cxwidgets.aQt.QtWidgets import QLCDNumber
+from cxwidgets.aQt.QtWidgets import QProgressBar
 from cxwidgets.aQt.QtCore import pyqtSlot, pyqtProperty
 import pycx4.qcda as cda
 from .menus.general_cm import CXGeneralCM
 
 
-class CXLCDNumber(QLCDNumber):
-    def __init__(self, parent=None, **kwargs):
-        super().__init__(parent)
+class CXProgressBar(QProgressBar):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args)
         self._cname = kwargs.get('cname', None)
         self.chan = None
         self.cx_connect()
 
         self.context_menu = None
 
     def contextMenuEvent(self, event):
         self.context_menu = CXGeneralCM(self)
         self.context_menu.popup(event.globalPos())
 
     def cx_connect(self):
         if self._cname is None or self._cname == '':
             return
-        self.chan = cda.DChan(self._cname, private=True)
+        self.chan = cda.IChan(self._cname, private=True, on_update=True)
         self.chan.valueChanged.connect(self.cs_update)
 
     def cs_update(self, chan):
-        self.display(chan.val)
+        if self.value() != chan.val:
+            self.setValue(chan.val)
 
-    @pyqtSlot(float)
-    def setCname(self, cname):
+    @pyqtSlot(str)
+    def set_cname(self, cname):
+        if self._cname == cname:
+            return
         self._cname = cname
         self.cx_connect()
 
-    def getCname(self):
+    def get_cname(self):
         return self._cname
 
-    cname = pyqtProperty(str, getCname, setCname)
+    cname = pyqtProperty(str, get_cname, set_cname)
```

### Comparing `cxwidgets-0.8/cxwidgets/cx_led.py` & `cxwidgets-0.9/cxwidgets/cx_led.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_lineedit.py` & `cxwidgets-0.9/cxwidgets/cx_lineedit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from cxwidgets.aQt.QtWidgets import QLineEdit
 from cxwidgets.aQt.QtCore import pyqtSlot, pyqtProperty
 import pycx4.qcda as cda
-
+from .menus.general_cm import CXGeneralCM
 
 class CXLineEdit(QLineEdit):
     def __init__(self, *args, **kwargs):
         super().__init__(*args)
         self._cname = kwargs.get('cname', '')
         self._max_len = kwargs.get('max_len', 100)
         self.setReadOnly(bool(kwargs.get('readonly', False)))
         self.chan = None
         self.cx_connect()
+        self.context_menu = None
+
+    def contextMenuEvent(self, event):
+        self.context_menu = CXGeneralCM(self)
+        self.context_menu.popup(event.globalPos())
 
     def cx_connect(self):
         if self._cname == '':
             return
         self.chan = cda.StrChan(self._cname, max_nelems=self._max_len, private=True, on_update=True)
         self.chan.valueChanged.connect(self.cs_update)
```

### Comparing `cxwidgets-0.8/cxwidgets/cx_plot.py` & `cxwidgets-0.9/cxwidgets/cx_plot.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_progressbar.py` & `cxwidgets-0.9/cxwidgets/cx_spinbox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,74 @@
-from cxwidgets.aQt.QtWidgets import QProgressBar
 from cxwidgets.aQt.QtCore import pyqtSlot, pyqtProperty
 import pycx4.qcda as cda
-from .menus.general_cm import CXGeneralCM
+from .pspinbox import PSpinBox
+from .menus.spinbox_cm import CXSpinboxCM
 
 
-class CXProgressBar(QProgressBar):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args)
+class CXSpinBox(PSpinBox):
+    def __init__(self, parent=None, **kwargs):
+        super().__init__(parent, **kwargs)
         self._cname = kwargs.get('cname', None)
         self.chan = None
-        self.cx_connect()
 
+        self.cx_connect()
+        self.done.connect(self.cs_send)
         self.context_menu = None
 
+        self._hardmin = 0
+        self._hardmax = 0
+
     def contextMenuEvent(self, event):
-        self.context_menu = CXGeneralCM(self)
+        self.context_menu = CXSpinboxCM(self)
         self.context_menu.popup(event.globalPos())
 
     def cx_connect(self):
         if self._cname is None or self._cname == '':
             return
-        self.chan = cda.IChan(self._cname, private=True, on_update=True)
+        self.chan = cda.IChan(self._cname, private=True)
         self.chan.valueChanged.connect(self.cs_update)
 
+    @pyqtSlot(int)
+    def cs_send(self, value):
+        if self.chan is None:
+            return
+        if int(value) == self.chan.val:
+            return
+        self.chan.setValue(value)
+
     def cs_update(self, chan):
-        if self.value() != chan.val:
-            self.setValue(chan.val)
+        if int(self.value()) == chan.val:
+            return
+        self.setValue(chan.val)
+        if chan.rflags != 0:
+            print(chan.rflags_text())
+            pass
 
     @pyqtSlot(str)
     def set_cname(self, cname):
         if self._cname == cname:
             return
         self._cname = cname
         self.cx_connect()
 
     def get_cname(self):
         return self._cname
 
     cname = pyqtProperty(str, get_cname, set_cname)
+
+    @pyqtSlot(int)
+    def set_hardmin(self, value):
+        self._hardmin = value
+
+    def get_hardmin(self):
+        return self._hardmin
+
+    hardmin = pyqtProperty(int, get_hardmin, set_hardmin)
+
+    @pyqtSlot(int)
+    def set_hardmax(self, value):
+        self._hardmax = value
+
+    def get_hardmax(self):
+        return self._hardmax
+
+    hardmax = pyqtProperty(int, get_hardmax, set_hardmax)
```

### Comparing `cxwidgets-0.8/cxwidgets/cx_pushbutton.py` & `cxwidgets-0.9/cxwidgets/cx_pushbutton.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cx_spinbox.py` & `cxwidgets-0.9/cxwidgets/cx_label.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,108 @@
 from cxwidgets.aQt.QtCore import pyqtSlot, pyqtProperty
+from cxwidgets.aQt.QtWidgets import QLabel
 import pycx4.qcda as cda
-from .pspinbox import PSpinBox
-from .menus.spinbox_cm import CXSpinboxCM
+from .menus.general_cm import CXGeneralCM
 
 
-class CXSpinBox(PSpinBox):
+class CXIntLabel(QLabel):
     def __init__(self, parent=None, **kwargs):
-        super().__init__(parent, **kwargs)
+        super().__init__(parent)
         self._cname = kwargs.get('cname', None)
         self.chan = None
-
         self.cx_connect()
-        self.done.connect(self.cs_send)
         self.context_menu = None
-
-        self._hardmin = 0
-        self._hardmax = 0
+        if self.chan is None:
+            self.setText('No cname')
 
     def contextMenuEvent(self, event):
-        self.context_menu = CXSpinboxCM(self)
+        self.context_menu = CXGeneralCM(self)
         self.context_menu.popup(event.globalPos())
 
     def cx_connect(self):
         if self._cname is None or self._cname == '':
             return
         self.chan = cda.IChan(self._cname, private=True)
         self.chan.valueChanged.connect(self.cs_update)
 
-    @pyqtSlot(int)
-    def cs_send(self, value):
-        if self.chan is None:
-            return
-        if int(value) == self.chan.val:
-            return
-        self.chan.setValue(value)
-
     def cs_update(self, chan):
-        if int(self.value()) == chan.val:
-            return
-        self.setValue(chan.val)
-        if chan.rflags != 0:
-            print(chan.rflags_text())
-            pass
-
-    @pyqtSlot(str)
-    def set_cname(self, cname):
-        if self._cname == cname:
-            return
+        self.setText(str(chan.val))
+
+    @pyqtSlot(float)
+    def setCname(self, cname):
         self._cname = cname
         self.cx_connect()
 
-    def get_cname(self):
+    def getCname(self):
         return self._cname
 
-    cname = pyqtProperty(str, get_cname, set_cname)
+    cname = pyqtProperty(str, getCname, setCname)
+
 
-    @pyqtSlot(int)
-    def set_hardmin(self, value):
-        self._hardmin = value
+class CXDoubleLabel(CXIntLabel):
+    def __init__(self, parent=None, **kwargs):
+        super().__init__(parent, **kwargs)
+        self._decimals = 0 # init stored
+        self.decimals = 3 # default value
+
+    def cs_update(self, chan):
+        self.setText(format(chan.val, self.format_spec))
+
+    def cx_connect(self):
+        if self._cname is None or self._cname == '':
+            return
+        self.chan = cda.DChan(self._cname, private=True)
+        self.chan.valueChanged.connect(self.cs_update)
 
-    def get_hardmin(self):
-        return self._hardmin
+    def setDecimals(self, n: int):
+        self._decimals = n
+        self.format_spec = '.' + str(self._decimals) + 'f'
 
-    hardmin = pyqtProperty(int, get_hardmin, set_hardmin)
+    def getDecimals(self) -> int:
+        return self._decimals
 
-    @pyqtSlot(int)
-    def set_hardmax(self, value):
-        self._hardmax = value
+    decimals = pyqtProperty(int, getDecimals, setDecimals)
+
+
+class CXStrLabel(QLabel):
+    def __init__(self, parent=None, **kwargs):
+        super().__init__(parent)
+        self._cname = kwargs.get('cname', None)
+        self._max_len = kwargs.get('max_len', 100)
+        self.chan = None
+        self.cx_connect()
+        self.context_menu = None
+        if self.chan is None:
+            self.setText('No cname')
+
+    def contextMenuEvent(self, event):
+        self.context_menu = CXGeneralCM(self)
+        self.context_menu.popup(event.globalPos())
+
+    def cx_connect(self):
+        if self._cname is None or self._cname == '':
+            return
+        self.chan = cda.StrChan(self._cname, private=True, max_nelems=self._max_len, on_update=True)
+        self.chan.valueChanged.connect(self.cs_update)
+
+    def cs_update(self, chan):
+        self.setText(str(chan.val))
+
+    @pyqtSlot(float)
+    def setCname(self, cname):
+        self._cname = cname
+        self.cx_connect()
+
+    def getCname(self):
+        return self._cname
+
+    cname = pyqtProperty(str, getCname, setCname)
+
+    @pyqtSlot(float)
+    def set_max_len(self, max_len):
+        self._max_len = max_len
+        self.cx_connect()
 
-    def get_hardmax(self):
-        return self._hardmax
+    def get_max_len(self):
+        return self._max_len
 
-    hardmax = pyqtProperty(int, get_hardmax, set_hardmax)
+    max_len = pyqtProperty(int, get_max_len, set_max_len)
```

### Comparing `cxwidgets-0.8/cxwidgets/cx_switch.py` & `cxwidgets-0.9/cxwidgets/cx_switch.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/cxw_demo.py` & `cxwidgets-0.9/cxwidgets/cxw_demo.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/menus/general_cm.py` & `cxwidgets-0.9/cxwidgets/menus/spinbox_cm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,68 @@
-from cxwidgets import BaseGridW, PSpinBox, PCheckBox, LedWidget, HLine
-from cxwidgets.aQt.QtWidgets import QLabel, QLineEdit, QTextEdit, QMenu, QWidgetAction, QWidget, QHBoxLayout, QLayout
 from cxwidgets.aQt.QtCore import Qt
-from pycx4.qcda import rflags_meanings
+from cxwidgets import BaseGridW, PSpinBox
+from cxwidgets.aQt.QtWidgets import QLabel, QLineEdit, QWidgetAction
+from .general_cm import CXGeneralCM
 
 
-class LabeledLed(QWidget):
-    """LedWidget + label
-
-    attributes:
-        led - LedWidget
-        label - Qlabel
-    """
-    def __init__(self, parent=None, text='label'):
-        super().__init__()
-        self.layout = QHBoxLayout(self)
-        self.layout.setSpacing(0)
-        self.layout.setSizeConstraint(QLayout.SetFixedSize)
-        self.layout.setContentsMargins(0, 0, 0, 0)
-
-        self.led = LedWidget(self)
-        self.led.setDiameter(10)
-        self.layout.addWidget(self.led)
-        self.label = QLabel(text)
-        self.layout.addWidget(self.label)
-
-
-class CXGeneralCMW(BaseGridW):
-    """Widget for general CX channel information
-    """
-
-    def __init__(self, source_chan=None, parent=None):
+class CXSpinboxSettingsW(BaseGridW):
+    def __init__(self, source_w, parent=None):
         super().__init__(parent)
-        self.source_chan = source_chan
-        self.l_h1 = QLabel("channel info")
-        self.l_h1.setStyleSheet("")
-        self.grid.addWidget(self.l_h1, 0, 0, 1, 2, Qt.AlignHCenter)
-        self.grid.addWidget(HLine(), 1, 0, 1, 2, Qt.AlignHCenter)
-
-        self.grid.addWidget(QLabel("name:  "), 2, 0)
-        name_txt = 'n/a' if source_chan is None else source_chan.name
-        self.grid.addWidget(QLabel(name_txt), 2, 1)
-
-        self.grid.addWidget(QLabel("value:  "), 3, 0)
-        val_text = 'n/a' if source_chan is None else str(source_chan.val)
-        self.label_val = QLabel(val_text)
-        self.grid.addWidget(self.label_val, 3, 1)
-
-        self.grid.addWidget(QLabel("time:  "), 4, 0)
-        self.label_time = QLabel()
-
-
-class CXFlagsMenu(QMenu):
-    """QMenu to show CX rflags
-    """
-    def __init__(self, source_chan):
-        super().__init__()
-        self.source_chan = source_chan
-        self.setTitle('rflags')
-        self.items = {}
-        self.widgets = {}
-
-        for k in rflags_meanings.keys():
-            self.widgets[k] = LabeledLed(text=k)
-            self.items[k] = QWidgetAction(self)
-            self.items[k].setDefaultWidget(self.widgets[k])
-            self.addAction(self.items[k])
-
-        if source_chan is not None:
-            rflags_t = source_chan.rflags_text()
-            self.setFlags(rflags_t)
-
-    def setFlags(self, flags):
-        for k in self.widgets:
-            if k in flags:
-                self.widgets[k].led.setValue(1)
-            else:
-                self.widgets[k].led.setValue(0)
+        self.source_w = source_w
+        self.l_h1 = QLabel("knob settings")
+        self.l_h1.setStyleSheet("font-weight: bold; font-size: 12pt")
+        self.grid.addWidget(self.l_h1, 0, 0, 1, 4, Qt.AlignHCenter)
+
+        self.grid.addWidget(QLabel("step:"), 1, 0)
+        self.step_sb = PSpinBox()
+        self.grid.addWidget(self.step_sb, 1, 1)
+        self.step_sb.setValue(source_w.singleStep())
+        self.step_sb.done.connect(source_w.setSingleStep)
+
+        self.grid.addWidget(QLabel("range:"), 2, 0)
+        self.min_sb = PSpinBox()
+        self.grid.addWidget(self.min_sb, 2, 1)
+        self.min_sb.setValue(source_w.minimum())
+        self.min_sb.done.connect(source_w.setMinimum)
+
+        self.grid.addWidget(QLabel("-"), 2, 2)
+        self.max_sb = PSpinBox()
+        self.max_sb.setValue(source_w.maximum())
+        self.max_sb.done.connect(source_w.setMaximum)
+        self.grid.addWidget(self.max_sb, 2, 3)
+
+        if not (source_w.hardmin == 0 and source_w.hardmax == 0):
+            self.min_sb.setMinimum(source_w.hardmin)
+            self.min_sb.setMaximum(source_w.hardmax)
+            self.max_sb.setMinimum(source_w.hardmin)
+            self.max_sb.setMaximum(source_w.hardmax)
+
+        self.grid.addWidget(QLabel("max range:"), 3, 0)
+        self.grid.addWidget(QLabel(str(source_w.hardmin)), 3, 1, Qt.AlignHCenter)
+        self.grid.addWidget(QLabel("-"), 3, 2)
+        self.grid.addWidget(QLabel(str(source_w.hardmax)), 3, 3, Qt.AlignHCenter)
+
+        self.grid.setColumnMinimumWidth(1, 100)
+        self.grid.setColumnMinimumWidth(3, 100)
+
+        # ranges now working incorrectly - reported to Bolkhov
+        # if source_w.chan is not None:
+        #     source_w.chan.get_range()
+        #     source_w.chan.get_strings()
+        #     print(source_w.chan.quant)
+        #     print(source_w.chan.rng)
 
+    def validate_minmax(self):
+        pass
 
-class CXGeneralCM(QMenu):
-    """General context menu for most CX-connected widgets
 
-    """
+class CXSpinboxCM(CXGeneralCM):
     def __init__(self, source_w):
-        super().__init__()
-        self.source_w = source_w
+        super().__init__(source_w)
 
-        w = CXGeneralCMW(source_w.chan)
-        self.act_gen = QWidgetAction(self)
-        self.act_gen.setDefaultWidget(w)
-        self.addAction(self.act_gen)
+        self.addSeparator()
 
-        self.fl_menu = CXFlagsMenu(source_w.chan)
-        self.addMenu(self.fl_menu)
+        self.w1 = CXSpinboxSettingsW(source_w)
+        self.act_set = QWidgetAction(self)
+        self.act_set.setDefaultWidget(self.w1)
+        self.addAction(self.act_set)
 
-        # self.setAttribute(Qt.WA_DeleteOnClose) # this also works, but runs later
-        self.aboutToHide.connect(self.deleteLater)
```

### Comparing `cxwidgets-0.8/cxwidgets/menus/spinbox_cm.py` & `cxwidgets-0.9/cxwidgets/menus/doublespinbox_cm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,67 @@
-#from cxwidgets.aQt.QtCore import Qt
-from cxwidgets import BaseGridW, PSpinBox
-from cxwidgets.aQt.QtWidgets import QLabel, QLineEdit, QWidgetAction
+from cxwidgets.aQt.QtCore import Qt
+from cxwidgets import BaseGridW, PDoubleSpinBox
+from cxwidgets.aQt.QtWidgets import QLabel, QWidgetAction
 from .general_cm import CXGeneralCM
 
 
-class CXSpinboxSettingsW(BaseGridW):
+class CXDoubleSpinboxSettingsW(BaseGridW):
     def __init__(self, source_w, parent=None):
         super().__init__(parent)
         self.source_w = source_w
-
-        self.grid.addWidget(QLabel("step"), 0, 0)
-        self.step_sb = PSpinBox()
-        self.grid.addWidget(self.step_sb, 0, 1)
+        self.l_h1 = QLabel("knob settings")
+        self.l_h1.setStyleSheet("font-weight: bold; font-size: 12pt")
+        self.grid.addWidget(self.l_h1, 0, 0, 1, 4, Qt.AlignHCenter)
+
+        self.grid.addWidget(QLabel("step:"), 1, 0)
+        self.step_sb = PDoubleSpinBox()
+        self.grid.addWidget(self.step_sb, 1, 1)
         self.step_sb.setValue(source_w.singleStep())
         self.step_sb.done.connect(source_w.setSingleStep)
 
-        self.grid.addWidget(QLabel("min"), 1, 0)
-        self.min_sb = PSpinBox()
-        self.grid.addWidget(self.min_sb, 1, 1)
+        self.grid.addWidget(QLabel("range:"), 2, 0)
+        self.min_sb = PDoubleSpinBox()
+        self.grid.addWidget(self.min_sb, 2, 1)
         self.min_sb.setValue(source_w.minimum())
         self.min_sb.done.connect(source_w.setMinimum)
 
-        self.grid.addWidget(QLabel("max"), 2, 0)
-        self.max_sb = PSpinBox()
-        self.grid.addWidget(self.max_sb, 2, 1)
+        self.grid.addWidget(QLabel("-"), 2, 2)
+        self.max_sb = PDoubleSpinBox()
         self.max_sb.setValue(source_w.maximum())
         self.max_sb.done.connect(source_w.setMaximum)
+        self.grid.addWidget(self.max_sb, 2, 3)
 
         if not (source_w.hardmin == 0 and source_w.hardmax == 0):
             self.min_sb.setMinimum(source_w.hardmin)
             self.min_sb.setMaximum(source_w.hardmax)
             self.max_sb.setMinimum(source_w.hardmin)
             self.max_sb.setMaximum(source_w.hardmax)
 
-        self.grid.addWidget(QLabel("hardmin"), 3, 0)
-        self.grid.addWidget(QLabel(str(source_w.hardmin)), 3, 1)
+        self.grid.addWidget(QLabel("max range:"), 3, 0)
+        self.grid.addWidget(QLabel(str(source_w.hardmin)), 3, 1, Qt.AlignHCenter)
+        self.grid.addWidget(QLabel("-"), 3, 2)
+        self.grid.addWidget(QLabel(str(source_w.hardmax)), 3, 3, Qt.AlignHCenter)
 
-        self.grid.addWidget(QLabel("hardmax"), 4, 0)
-        self.grid.addWidget(QLabel(str(source_w.hardmax)), 4, 1)
+        self.grid.setColumnMinimumWidth(1, 100)
+        self.grid.setColumnMinimumWidth(3, 100)
 
         # ranges now working incorrectly - reported to Bolkhov
         # if source_w.chan is not None:
         #     source_w.chan.get_range()
         #     source_w.chan.get_strings()
         #     print(source_w.chan.quant)
         #     print(source_w.chan.rng)
+
     def validate_minmax(self):
         pass
 
 
-
-
-class CXSpinboxCM(CXGeneralCM):
+class CXDoubleSpinboxCM(CXGeneralCM):
     def __init__(self, source_w):
         super().__init__(source_w)
 
         self.addSeparator()
 
-        self.w1 = CXSpinboxSettingsW(source_w)
+        self.w1 = CXDoubleSpinboxSettingsW(source_w)
         self.act_set = QWidgetAction(self)
         self.act_set.setDefaultWidget(self.w1)
         self.addAction(self.act_set)
```

### Comparing `cxwidgets-0.8/cxwidgets/pcombobox.py` & `cxwidgets-0.9/cxwidgets/pcombobox.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/pdoublespinbox.py` & `cxwidgets-0.9/cxwidgets/pdoublespinbox.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/pledwidget.py` & `cxwidgets-0.9/cxwidgets/pledwidget.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/plt_text.py` & `cxwidgets-0.9/cxwidgets/plt_text.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/plugins/cx_plugin.py` & `cxwidgets-0.9/cxwidgets/plugins/cx_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cxwidgets.aQt.QtDesigner import QPyDesignerCustomWidgetPlugin
 from cxwidgets.aQt.QtGui import QIcon
 from cxwidgets import CXDoubleSpinBox, CXSpinBox, CXLCDNumber, CXCheckBox, CXTextComboBox
-from cxwidgets import CXPushButton, CXLineEdit, CXProgressBar, CXSwitch, CXDevSwitch, CXLabel
+from cxwidgets import CXPushButton, CXLineEdit, CXProgressBar, CXSwitch, CXDevSwitch, CXIntLabel, CXDoubleLabel, CXStrLabel
 from cxwidgets import CXEventLed, CXStateLed
 
 
 class CXDoubleSpinBoxWidgetPlugin(QPyDesignerCustomWidgetPlugin):
     def __init__(self, parent=None):
         super(CXDoubleSpinBoxWidgetPlugin, self).__init__(parent)
 
@@ -184,20 +184,48 @@
     def whatsThis(self):
         return 'StateLed connected to CX'
 
     def createWidget(self, parent):
         return CXStateLed(parent)
 
 
-class CXLabelWidgetPlugin(CXDoubleSpinBoxWidgetPlugin):
+class CXIntLabelWidgetPlugin(CXDoubleSpinBoxWidgetPlugin):
     def name(self):
-        return 'CXLabel'
+        return 'CXIntLabel'
 
     def toolTip(self):
-        return 'Label connected to CX'
+        return 'Label connected to CX int channel'
 
     def whatsThis(self):
-        return 'Label connected to CX'
+        return 'Label connected to CX int channel'
 
     def createWidget(self, parent):
-        return CXLabel(parent)
+        return CXIntLabel(parent)
+
+
+class CXDoubleLabelWidgetPlugin(CXDoubleSpinBoxWidgetPlugin):
+    def name(self):
+        return 'CXDoubleLabel'
+
+    def toolTip(self):
+        return 'Label connected to CX double channel'
+
+    def whatsThis(self):
+        return 'Label connected to CX double channel'
+
+    def createWidget(self, parent):
+        return CXDoubleLabel(parent)
+
+
+class CXStrLabelWidgetPlugin(CXDoubleSpinBoxWidgetPlugin):
+    def name(self):
+        return 'CXStrLabel'
+
+    def toolTip(self):
+        return 'Label connected to CX str channel'
+
+    def whatsThis(self):
+        return 'Label connected to CX str channel'
+
+    def createWidget(self, parent):
+        return CXStrLabel(parent)
```

### Comparing `cxwidgets-0.8/cxwidgets/plugins/p_plugin.py` & `cxwidgets-0.9/cxwidgets/plugins/p_plugin.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/pspinbox.py` & `cxwidgets-0.9/cxwidgets/pspinbox.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets/pswitch.py` & `cxwidgets-0.9/cxwidgets/pswitch.py`

 * *Files identical despite different names*

### Comparing `cxwidgets-0.8/cxwidgets.egg-info/SOURCES.txt` & `cxwidgets-0.9/cxwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

