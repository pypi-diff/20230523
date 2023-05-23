# Comparing `tmp/SpectroscopicBinarySystem-1.3.1.tar.gz` & `tmp/SpectroscopicBinarySystem-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.3.1.tar", last modified: Tue May 23 08:28:31 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.4.0.tar", last modified: Wed May 17 13:37:03 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.3.1.tar` & `SpectroscopicBinarySystem-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:31.297720 SpectroscopicBinarySystem-1.3.1/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     4710 2023-05-23 08:28:31.297720 SpectroscopicBinarySystem-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4319 2023-05-17 18:34:07.000000 SpectroscopicBinarySystem-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:31.289339 SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4710 2023-05-23 08:28:31.000000 SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-23 08:28:31.000000 SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:28:31.000000 SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-23 08:28:31.000000 SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-23 08:28:31.000000 SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-05-23 08:28:31.299228 SpectroscopicBinarySystem-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:31.289339 SpectroscopicBinarySystem-1.3.1/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    32906 2023-05-23 08:00:30.000000 SpectroscopicBinarySystem-1.3.1/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:37:03.836655 SpectroscopicBinarySystem-1.4.0/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4710 2023-05-17 13:37:03.836655 SpectroscopicBinarySystem-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4319 2023-05-15 22:27:13.000000 SpectroscopicBinarySystem-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:37:03.834642 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4710 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-05-17 13:37:03.843117 SpectroscopicBinarySystem-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 13:37:03.835651 SpectroscopicBinarySystem-1.4.0/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    34755 2023-05-17 13:34:14.000000 SpectroscopicBinarySystem-1.4.0/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.3.1/LICENSE` & `SpectroscopicBinarySystem-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.3.1/PKG-INFO` & `SpectroscopicBinarySystem-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.3.1/README.md` & `SpectroscopicBinarySystem-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.3.1/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.3.1/setup.cfg` & `SpectroscopicBinarySystem-1.4.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 332e 310d 0a61  rsion = 1.3.1..a
+00000030: 7273 696f 6e20 3d20 312e 342e 300d 0a61  rsion = 1.4.0..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.3.1/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.4.0/spectroscopicbinarysystem/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import os
-import csv
 import copy
 import math
 import warnings
+import pickle
+from hashlib import md5
 
 # numpy
 import numpy as np
 
 # astropy
 from astropy.io import fits
 from astropy.time import Time
@@ -243,14 +244,25 @@
                 fwhm = g_fit.fwhm
 
         self._debug_line_fitting = (spec1d_line, y_fit, extract_region(Spectrum1D(
             flux=spec1_gsmooth.flux, wcs=self.wcs), sr_w1))
         self._center_of_line = center.value
         self._line_fit_fwhm = fwhm.value
 
+    def asdict(self):
+        return {'jd': self.getJD(),
+                'date': self.getDate(),
+                'observer': self.getObserver(),
+                'instrument': self.getInstrument(),
+                'basename': self.getBaseName(),
+                'rv': self.getRV(),
+                'error': self.getError(),
+                'center': self.getCenterOfLine(),
+                'phase': self.getPhase()}
+
     def __str__(self):
         return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- snr: {self._snr}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n- error: {self.getError()}\n"
 
 #
 
 
 class SpectroscopicBinarySystem:
@@ -267,39 +279,46 @@
     :param t0: Allow to fix Periastron epoch T0 if known (julian date)
     :param period: If the period of the orbit is already known use this param (period in days).
     :param perdiod_guess: If the period is uncertain use this param (period in days).
     :param conf: Allow to customize additionnal parameters (see self._conf default value below)
     :param debug: Allow to activate log and some additional plots for debug purpose
     """
 
-    def __init__(self, object_name, spectra_path, t0=None, period=None, period_guess=None, conf=None, verbose=False, debug=False):
+    def __init__(self, object_name, spectra_path, t0=None, period=None, period_guess=None, conf=None, verbose=False, debug=False, nocache=False):
 
         self._conf = {"LAMBDA_REF": 6562.82,
                       "LINE_FIT_MODEL": "gaussian",
                       "LINE_FIT_FWHM": 3.0,
                       "LINE_FIT_GAUSS_SMOOTH_STD": 10,
                       "RV_CORR_TYPE": "barycentric",
                       "SB_TYPE": 1}
 
         self._sb_spectra = []
+        self._sb_spectra_dict = []
         self._spectra_filename = []
         self._orbital_solution = None
         self._spectra_path = spectra_path
         self._object_name = object_name
         self._type = type
+        self._nocache = nocache
         self._t0 = t0
         self._period = period
         self._period_guess = period_guess
         self._debug = debug
         self._verbose = verbose
         self._residuals = []
-        self._results_csv_filename = os.path.join(
-            self._spectra_path, 'sbss_results.csv')
-        self._bss_filename = os.path.join(
-            self._spectra_path, 'binarystarsolver_results.txt')
+        self._key = str(self._conf).encode()
+        for root, dirs, files in os.walk(self._spectra_path):
+            for file in files:
+                regex = re.compile('(.*).fit')
+                if (re.match(regex, file)):
+                    spectrum_filename = os.path.join(
+                        self._spectra_path, file)
+                    self._key += spectrum_filename.encode()
+        self._key = md5(self._key).hexdigest()
 
         # load user configuration or defaults
         if conf:
             self._conf.update(conf)
 
         print('** SpectroscopicBinarySystem **')
         self.__findObjectCoordinate()
@@ -311,28 +330,46 @@
         self._skycoord = None
         if result_table := Simbad.query_object(self._object_name):
             ra = result_table[0]['RA']
             dec = result_table[0]['DEC']
             self._skycoord = SkyCoord(f'{ra} {dec}', unit=(u.hourangle, u.deg))
 
     def __loadSpectra(self):
-        for root, dirs, files in os.walk(self._spectra_path):
-            for file in files:
-                regex = re.compile('(.*).fit')
-                if (re.match(regex, file)):
-                    spectrum_filename = os.path.join(self._spectra_path, file)
-                    sbSpec1D = SBSpectrum1D(
-                        spectrum_filename, self._skycoord, self._conf)
-                    self._sb_spectra.append(sbSpec1D)
-                    if self._verbose:
-                        print(sbSpec1D)
+        """
+        Load all spectra and create SBSpectrum1D objects
+        """
+        pickle_file = os.path.join(
+            self._spectra_path, f"{self._key}_spectra.pickle")
+        if os.path.exists(pickle_file) and not self._nocache:
+            with open(pickle_file, "rb") as infile:
+                self._sb_spectra_dict = pickle.load(infile)
+        else:
+            self._sb_spectra = []
+            self._sb_spectra_dict = []
+            for root, dirs, files in os.walk(self._spectra_path):
+                for file in files:
+                    regex = re.compile('(.*).fit')
+                    if (re.match(regex, file)):
+                        spectrum_filename = os.path.join(
+                            self._spectra_path, file)
+                        sbSpec1D = SBSpectrum1D(
+                            spectrum_filename, self._skycoord, self._conf)
+                        self._sb_spectra.append(sbSpec1D)
+                        self._sb_spectra_dict.append(sbSpec1D.asdict())
+                        if self._verbose:
+                            print(sbSpec1D)
+            if not self._nocache:
+                with open(pickle_file, "wb") as outfile:
+                    pickle.dump(self._sb_spectra_dict, outfile)
 
         if self._verbose:
-            print(f'{len(self._sb_spectra)} processed spectra')
-        if self._debug:
+            print(f'key : {self._key}')
+            print(f'{len(self._sb_spectra_dict)} processed spectra')
+
+        if self._debug and self._sb_spectra:
             plt.rcParams['font.size'] = '6'
             plt.rcParams['font.family'] = 'monospace'
 
             paginate_sb_spectra = [self._sb_spectra[i:i+16]
                                    for i in range(0, len(self._sb_spectra), 16)]
             for page, spectra in enumerate(paginate_sb_spectra):
                 fig, axs = plt.subplots(4, 4, figsize=(
@@ -370,15 +407,15 @@
 
     def getObservationCount(self):
         """
         Return the count of processed spectra
         :return: count
         :rtype: int
         """
-        return len(self._sb_spectra)
+        return len(self._sb_spectra_dict)
 
     def __getPhase(self, jd0, period, jd):
         """
         Compute the phase of a given JD
         :param jd0: JD of the first observation
         :param period: period of the orbit
         :param jd: JD to compute the phase
@@ -406,73 +443,76 @@
         f = utilities.true_anomaly_from_eccentric(e, E)
         return (K * (e * np.cos(w) + np.cos(w + f)) + v0)
 
     def __solveSystem(self):
         """
         Compute the orbital solution with BinaryStarSolver
         """
-        # write result file for BinaryStarSolver
-        with open(self._bss_filename, 'w') as f:
-            for s in self._sb_spectra:
-                error = 1 / s.getError() if s.getError() else 1
-                output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)} {error}"
-                f.write(output + '\n')
-
-        # [γ, K, ω, e, T0, P, a, f(M)]
-        try:
-            params, err, cov = StarSolve(
-                data_file=self._bss_filename,
-                star="primary",
-                Period=self._period,
-                Pguess=self._period_guess,
-                covariance=True,
-                graphs=False,
-            )
-        except:
-            print(
-                'An exception occurred : the calculation of the orbital solution failed')
-            exit()
-
-        self._orbital_solution = (params, err, cov)
+        pickle_file = os.path.join(
+            self._spectra_path, f"{self._key}_orbital.pickle")
+        if os.path.exists(pickle_file) and not self._nocache:
+            with open(pickle_file, "rb") as infile:
+                self._orbital_solution = pickle.load(infile)
+                params, err, cov = self._orbital_solution
+        else:
+            # write result file for BinaryStarSolver
+            with open(f'{self._spectra_path}/sbs_results.txt', 'w') as f:
+                for s in self._sb_spectra:
+                    error = 1 / s.getError() if s.getError() else 1
+                    output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)} {error}"
+                    f.write(output + '\n')
+
+            # [γ, K, ω, e, T0, P, a, f(M)]
+            try:
+                params, err, cov = StarSolve(
+                    data_file=f"{self._spectra_path}/sbs_results.txt",
+                    star="primary",
+                    Period=self._period,
+                    Pguess=self._period_guess,
+                    covariance=True,
+                    graphs=False,
+                )
+            except:
+                print(
+                    'An exception occurred : the calculation of the orbital solution failed')
+                exit()
+
+            self._orbital_solution = (params, err, cov)
+
+            if not self._nocache:
+                with open(pickle_file, "wb") as outfile:
+                    pickle.dump(self._orbital_solution, outfile)
 
         # If self._t0 compute phase delta between T0 of the model and the fixed value
         if self._t0:
             t0 = self._t0
             phase1 = self.__getPhase(
                 t0, self._orbital_solution[0][5], self._orbital_solution[0][4]+2400000)
             phase2 = 1.0
             self._v0 = phase1 - phase2
         # Else use t0 compute by the model
         else:
             self._t0 = self._orbital_solution[0][4] + 2400000
             self._v0 = 0
 
         period = self._orbital_solution[0][5]
-        for s in self._sb_spectra:
+        if self._sb_spectra:
+            for s in self._sb_spectra:
+                # compute phase of the sytem
+                s.setPhase(self.__getPhase(float(self._t0), period, s.getJD()))
+
+        for s in self._sb_spectra_dict:
             # compute phase of the sytem
-            jd = s.getJD()
-            phase = self.__getPhase(float(self._t0), period, jd)
-            s.setPhase(phase)
+            jd = s['jd']
+            s['phase'] = self.__getPhase(float(self._t0), period, jd)
             if self._verbose:
-                print(f"{s.getBaseName()} phase : {phase}")
-
-        # export all results
-        res = [['JD-OBS', 'DATE-OBS', 'OBSERVER',
-                'INSTRUMENT', 'PHASE', 'CENTER', 'RV', 'ERROR']]
-        for s in self._sb_spectra:
-            res.append([s.getJD(), s.getDate(), s.getObserver(), s.getInstrument(
-            ), s.getPhase(), s.getCenterOfLine(), s.getRV(), s.getError()])
-
-        with open(self._results_csv_filename, 'w') as f:
-            mywriter = csv.writer(
-                f, delimiter=',', quoting=csv.QUOTE_NONNUMERIC)
-            mywriter.writerows(res)
+                print(f"{s['basename']} phase : {s['phase']}")
 
         print(
-            f'{self._object_name} orbital solution with {len(self._sb_spectra)} spectra',
+            f'{self._object_name} orbital solution with {len(self._sb_spectra_dict)} spectra',
             f'- γ = {params[0]} ± {err[0]}',
             f'- K = {params[1]} ± {err[1]}',
             f'- ω = {params[2]} ± {err[2]}',
             f'- e = {params[3]} ± {err[3]}',
             f'- T0 = {params[4]} ± {err[4]}',
             f'- P = {params[5]} ± {err[5]}',
             f'- a = {params[6]} ± {err[6]}',
@@ -511,53 +551,53 @@
 
         # define colors (max 60 distinct observers)
         colors = cmap((np.arange(20)).astype(int), alpha=1)
         + cmap((np.arange(20)).astype(int), alpha=.75)
         + cmap((np.arange(20)).astype(int), alpha=.5)
 
         # sort sb spectra by observer name
-        self._sb_spectra.sort(key=lambda x: x.getObserver())
+        self._sb_spectra_dict.sort(key=lambda x: x['observer'])
 
-        for s in self._sb_spectra:
+        for s in self._sb_spectra_dict:
 
             # get the observer
-            obs = s.getObserver()
+            obs = s['observer']
             if (obs not in observers.keys()):
                 observers[obs] = colors[color_number]
                 color_number += 1
                 if not group_by_instruments:
-                    axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
+                    axs[0].errorbar(s['phase'], s['rv'], yerr=0,
                                     fmt='o', ecolor='k', label=obs, capsize=0, color=observers[obs], lw=.7, markersize=5)
             elif not group_by_instruments:
-                axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
+                axs[0].errorbar(s['phase'], s['rv'], yerr=0,
                                 fmt='o', ecolor='k', capsize=0, color=observers[obs], lw=.7, markersize=5)
             color = observers[obs]
 
             # get the instrument
             if (group_by_instruments):
-                label = f"{obs} - {s.getInstrument()[:30]}…"
+                label = f"{obs} - {s['instrument'][:30]}…"
                 if label not in instruments.keys():
                     if obs not in marker_index:
                         marker_index[obs] = 0
                     instruments[label] = markers_style[marker_index[obs]]
                     marker_index[obs] += 1
-                    axs[0].errorbar(s.getPhase(), s.getRV(
-                    ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
+                    axs[0].errorbar(s['phase'], s['rv'], yerr=0, label=label, ecolor='k',
+                                    capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
                 else:
-                    axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
+                    axs[0].errorbar(s['phase'], s['rv'], yerr=0,
                                     fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
-            xindex = self.__findNearest(self._model_x, s.getPhase())
-            delta = s.getRV() - self._model_y[xindex]
+            xindex = self.__findNearest(self._model_x, s['phase'])
+            delta = s['rv'] - self._model_y[xindex]
             self._residuals.append(delta)
             fmt = instruments[label] if group_by_instruments else 'o'
-            error = s.getError()
+            error = s['error']
             capsize = 3 if error else 0
-            axs[1].errorbar(s.getPhase(), delta,
-                            yerr=s.getError(), fmt=fmt, ecolor='k', capsize=capsize, color=color, lw=.7, markersize=5)
+            axs[1].errorbar(s['phase'], delta,
+                            yerr=s['error'], fmt=fmt, ecolor='k', capsize=capsize, color=color, lw=.7, markersize=5)
 
         print(
             f'- Residual standard deviation : {np.std(self._residuals)}')
 
     def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=None, savefig=False, dpi=150, font_family='monospace', font_size=9, group_by_instruments=False):
         if not self._orbital_solution:
             self.__solveSystem()
@@ -651,61 +691,56 @@
         colors = cmap((np.arange(20)).astype(int), alpha=1)
         + cmap((np.arange(20)).astype(int), alpha=.75)
         + cmap((np.arange(20)).astype(int), alpha=.5)
 
         markers_style = ['circle', 'square',
                          'diamond', 'triangle-up', 'triangle-down']
 
-        for s in self._sb_spectra:
-            # compute phase of the sytem
-            jd = s.getJD()
-            phase = self.__getPhase(float(self._t0), period, jd)
-            s.setPhase(phase)
-
+        for s in self._sb_spectra_dict:
             # get the observer
-            obs = s.getObserver()
+            obs = s['observer']
             if (obs not in observers.keys()):
                 rgb = colors[color_number][:3] * 255
                 str_rgb = ",".join([str(rgb[0]), str(rgb[1]), str(rgb[2])])
                 observers[obs] = f'rgba({str_rgb}, {colors[color_number][3]})'
                 color_number += 1
             color = observers[obs]
 
             if group_by_instrument:
                 # get the instrument
-                label = f"{obs} - {s.getInstrument()[:30]}…"
+                label = f"{obs} - {s['instrument'][:30]}…"
                 if label in instruments:
                     fig.add_trace(
-                        go.Scatter(x=[phase],
-                                   y=[s.getRV()],
+                        go.Scatter(x=[s['phase']],
+                                   y=[s['rv']],
                                    mode='markers',
                                    marker_symbol=instruments[label],
                                    marker=dict(color=color,
                                                size=8),
                                    showlegend=False))
                 else:
                     if obs not in marker_index:
                         marker_index[obs] = 0
                     instruments[label] = markers_style[marker_index[obs]]
                     marker_index[obs] += 1
                     fig.add_trace(
-                        go.Scatter(x=[phase],
-                                   y=[s.getRV()],
+                        go.Scatter(x=[s['phase']],
+                                   y=[s['rv']],
                                    mode='markers',
                                    name=label,
                                    marker_symbol=instruments[label],
                                    marker=dict(color=color,
                                                size=8),
                                    showlegend=True))
             else:  # no grouping
                 # set label to date
-                label = f"{obs} - {s.getDate()}"
+                label = f"{obs} - {s['date']}"
                 fig.add_trace(
-                    go.Scatter(x=[phase],
-                               y=[s.getRV()],
+                    go.Scatter(x=[s['phase']],
+                               y=[s['rv']],
                                mode='markers',
                                name=label,
                                marker_symbol='circle',
                                marker=dict(color=color,
                                            size=8),
                                showlegend=False))
 
@@ -773,15 +808,19 @@
         :param font_size:
         :param show:
         :return: fig
         """
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
 
-        if not self._orbital_solution:
+        self._nocache = True
+        if not self._sb_spectra:
+            self.__loadSpectra()
+            self.__solveSystem()
+        elif not self._orbital_solution:
             self.__solveSystem()
 
         # sort sb spectra by phase
         self._sb_spectra.sort(key=lambda x: x.getPhase())
 
         # create y axis range (phase)
         y_phase = np.arange(0, 1.01, 0.015)
```

