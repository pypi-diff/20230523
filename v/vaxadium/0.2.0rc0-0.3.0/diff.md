# Comparing `tmp/vaxadium-0.2.0rc0.tar.gz` & `tmp/vaxadium-0.3.0.tar.gz`

## Comparing `vaxadium-0.2.0rc0.tar` & `vaxadium-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/_version.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/axes.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_density.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_dls.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_macros.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_vaxadium.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/configuration.py
--rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/constants.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/data_descriptors.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/defaults.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/experiment.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/logging_setup.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/physics.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/processors.py
--rw-r--r--   0        0        0    12554 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/runner.py
--rw-r--r--   0        0        0    14340 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/scaler.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/basechecker.py
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/calibration.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/convergence.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/data.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/extractor.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/sample.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/axis_generators.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/detector.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/form_factors.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/fourier.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/units.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/fitting.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/macro_maker.py
--rw-r--r--   0        0        0    11483 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/macros.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/simulation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/__init__.py
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/nexus_reader.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/outputs.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/serializer_factory.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/serializers.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/__init__.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/attenuator.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/beam.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz_runner.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/direction.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz_runner.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/scatterer.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/transmission_map.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/yz_generator.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/.gitignore
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/AUTHORS.rst
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/LICENSE
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/README.rst
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/_version.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/axes.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/cli_density.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/cli_dls.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/cli_macros.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/cli_vaxadium.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/configuration.py
+-rw-r--r--   0        0        0    20665 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/constants.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/data_descriptors.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/defaults.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/experiment.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/logging_setup.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/physics.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/processors.py
+-rw-r--r--   0        0        0    13558 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/runner.py
+-rw-r--r--   0        0        0    14370 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/scaler.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/basechecker.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/calibration.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/convergence.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/data.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/extractor.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/checks/sample.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/core/axis_generators.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/core/detector.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/core/form_factors.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/core/fourier.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/core/units.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/g4diffsim/fitting.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/g4diffsim/macro_maker.py
+-rw-r--r--   0        0        0    11483 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/g4diffsim/macros.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/g4diffsim/simulation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/io/__init__.py
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/io/nexus_reader.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/io/outputs.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/io/serializer_factory.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/io/serializers.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/io/utils.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/__init__.py
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/attenuator.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/beam.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/cylinder_yz.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/cylinder_yz_runner.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/direction.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/illuminated_yz.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/illuminated_yz_runner.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/scatterer.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/transmission_map.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 vaxadium-0.3.0/vaxadium/transmission/yz_generator.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 vaxadium-0.3.0/.gitignore
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 vaxadium-0.3.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 vaxadium-0.3.0/LICENSE
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 vaxadium-0.3.0/README.rst
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 vaxadium-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 vaxadium-0.3.0/PKG-INFO
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/cli_density.py` & `vaxadium-0.3.0/vaxadium/cli_density.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/cli_dls.py` & `vaxadium-0.3.0/vaxadium/cli_dls.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/cli_macros.py` & `vaxadium-0.3.0/vaxadium/cli_macros.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/cli_vaxadium.py` & `vaxadium-0.3.0/vaxadium/cli_vaxadium.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/configuration.py` & `vaxadium-0.3.0/vaxadium/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     POLARIZATION = "polarization"
     LORCH_WIDTH = "lorch_width"
     TOPHAT_WIDTH = "tophat_width"
     RMINFT = "rmin_ft"
     RMAX = "rmax"
     RSTEP = "rstep"
     FSQUARED = "form_factor_normalisation"
+    MASK = "mask"
 
 
 class FORMFACTORKEYS:
     SUMOFSQUARES = "sum_of_squares"
     SQUAREOFSUMS = "square_of_sums"
 
 
@@ -99,7 +100,8 @@
 defaultconfig[CONFIGKEYS.POLARIZATION] = 0.9
 defaultconfig[CONFIGKEYS.LORCH_WIDTH] = 0.001
 defaultconfig[CONFIGKEYS.TOPHAT_WIDTH] = 4
 defaultconfig[CONFIGKEYS.RMINFT] = 0.025
 defaultconfig[CONFIGKEYS.RMAX] = 25
 defaultconfig[CONFIGKEYS.RSTEP] = 0.025
 defaultconfig[CONFIGKEYS.FSQUARED] = FORMFACTORKEYS.SUMOFSQUARES
+defaultconfig[CONFIGKEYS.MASK] = None
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/constants.py` & `vaxadium-0.3.0/vaxadium/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,7 +468,11 @@
     )
     PRIMARY_BEAM_DIRECTION = lambda x: [0, 0, 1]
     PRIMARY_BEAM_ELLIPTICAL = lambda x: False
 
 
 class NEWNXXPDFNEXUSKEYSBKGARC(NEWNXXPDFNEXUSKEYSARC):
     DATA = NexKey("/entry/pe2AD/data")
+
+
+class MASKKEYS(NexusKeyGroup):
+    MASK = NexKey("/entry/mask/mask/")
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/data_descriptors.py` & `vaxadium-0.3.0/vaxadium/data_descriptors.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/experiment.py` & `vaxadium-0.3.0/vaxadium/experiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import time
 from copy import deepcopy
 
 import numpy as np
+from pyFAI import units as pyFAIunits
 
+from vaxadium.configuration import CONFIGKEYS
 from vaxadium.constants import PHYSICAL
+from vaxadium.core.axis_generators import get_ai_params
 from vaxadium.g4diffsim import fitting
 from vaxadium.physics import atom_number_density
 from vaxadium.transmission.transmission_map import TransmissionMap
 
 logger = logging.getLogger(__name__)
 
 
@@ -33,14 +36,15 @@
     def __init__(
         self,
         components,
         data_collections,
         simulations,
         background,
         transmission_maps=None,
+        mask=None,
     ):
         """the zeroth component is the  innermost. therfore a sample with no container
         will be :
             components = [powder]
             data_collections = [sample]
         and with 1:
             components = [powder, capillary
@@ -57,14 +61,15 @@
         self.transmission_maps = transmission_maps
         self.tmaps_sims = None
         self.tmaps_exps = None
         self.simulated_result = None
         self.experimental_result = None
         self._gain = 0  # these are just stored for the checker
         self._delta = 0  # these are just stored for the checker
+        self.mask = mask
         logging.info("Experiment object created")
 
     @classmethod
     def from_config(cls, json_file_path):
         # return cls()
         pass
 
@@ -229,7 +234,38 @@
         )
         logger.debug(
             "interpolating and scaling to length = {}, rho = {}".format(
                 sample_length_m, sample_rho
             )
         )
         return scaled.reshape(self.detector_shape)
+
+    def validate_qmax_inst_against_mask(self, configuration):
+        """Check that the mask does not leave us with empty histogram bins
+        return None for no change or a new QMAX_INST if nexessary"""
+
+        dummy_data = np.ones(self.dc.pyfai.detector.max_shape)
+        q, ai_range, ai_npts = get_ai_params(
+            configuration[CONFIGKEYS.QMIN],
+            configuration[CONFIGKEYS.QMAX_INST],
+            configuration[CONFIGKEYS.QSTEP],
+        )
+        r = self.dc.pyfai.integrate1d(
+            dummy_data,
+            ai_npts,
+            radial_range=ai_range,
+            unit=pyFAIunits.Q_A,
+            mask=self.mask,
+            correctSolidAngle=False,
+        )
+        last_nonempty_bin_reversed_idx = np.nonzero(r.count[::-1])[0][0]
+        if last_nonempty_bin_reversed_idx == 0:
+            # then there's no zeros at the end and we're good to go
+            return None
+        else:
+            first_empty_bin_idx = ai_npts - last_nonempty_bin_reversed_idx - 1
+            # find the q matching the mask limit
+            new_qmax_inst = q[first_empty_bin_idx - 1]
+            logger.info(
+                "setting qmax_inst to {} to match mask limits".format(new_qmax_inst)
+            )
+            return new_qmax_inst
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/logging_setup.py` & `vaxadium-0.3.0/vaxadium/logging_setup.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/physics.py` & `vaxadium-0.3.0/vaxadium/physics.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/processors.py` & `vaxadium-0.3.0/vaxadium/processors.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/runner.py` & `vaxadium-0.3.0/vaxadium/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import json
 import logging
 from pathlib import Path
 
 import h5py
+import numpy as np
 from swmr_tools import DataSource
 
 from vaxadium.checks import run_diagnostics_checks
-from vaxadium.configuration import CKEYS, VaxadiumConfigurationError, defaultconfig
+from vaxadium.configuration import (
+    CKEYS,
+    CONFIGKEYS,
+    VaxadiumConfigurationError,
+    defaultconfig,
+)
 from vaxadium.constants import NEWG4NEXUSKEYS, NEWNXXPDFNEXUSKEYS, NEWNXXPDFNEXUSKEYSBKG
 from vaxadium.experiment import Experiment
 from vaxadium.io.nexus_reader import NexusReaderPyFAI, NexusReaderPyFAISample
 from vaxadium.io.outputs import default_outputs
 from vaxadium.io.serializer_factory import SERIALIZERS, nexus_serializer
+from vaxadium.io.utils import get_mask_from_mask_file
 from vaxadium.processors import FourierTransformer, TopHatter
 from vaxadium.scaler import ScaledResultsCollection, scale_experiment
 
 logger = logging.getLogger(__name__)
 
 
 def get_config_from_file(filepath):
@@ -51,14 +58,22 @@
         self.experiment = None
         self._output_filepath = None
         self._outputs = default_outputs
         self._diagnostics_filepath = ""
         self._diagnostics_results = list()
         self.n_pixels_for_tmaps = 20
         self.n_voxels_for_tmaps = 64
+        self.mask_file = self.configuration.get(CONFIGKEYS.MASK)
+        if self.mask_file:
+            try:
+                self.mask = get_mask_from_mask_file(self.mask_file)
+            except Exception:
+                logger.exception(
+                    "could not load mask from file {}".format(self.mask_file)
+                )
 
     @classmethod
     def from_configuration_dictionary(cls, config):
         logger.debug("configuration: {}".format(config))
         # check there are no erronious empty file paths in the config
         if config.get("background") == "":
             raise VaxadiumConfigurationError(
@@ -110,14 +125,15 @@
     def construct_experiment(self):
         self.experiment = Experiment(
             self.components,
             self.data_collections,
             self.simulations,
             self.background,
             None,
+            self.mask,
         )
         self._preprocessed = False
 
     def set_output_file(self, filepath):
         """output filepath will be a nxs file in which everything will be saved."""
         self._output_filepath = Path(filepath)
 
@@ -257,14 +273,19 @@
             n_voxels=self.n_voxels_for_tmaps,
             falsify=False,
         )
         self.experiment.do_simulation_preprocess()
         self.experiment.do_simulation_container_subtraction(force=force)
         self.experiment.do_simulation_extraction()
         self.experiment.do_background_preprocess()
+        new_qmax_inst = self.experiment.validate_qmax_inst_against_mask(
+            self.configuration
+        )
+        if new_qmax_inst:
+            self.configuration[CONFIGKEYS.QMAX_INST] = new_qmax_inst
         self._preprocessed = True
 
     def run(self):
         logger.info("running...")
         # check the background is present
 
         if self.experiment is None:
@@ -284,28 +305,37 @@
         else:
             save_as_we_go = False
 
         key_locations = [self.nxs.nodes.UNIQUE_KEYS.address]
         axes_locations = self.nxs.get_axes_locations()
         data_location = self.nxs.get_data_locations()
         with h5py.File(self.nxs.filename, "r", swmr=True) as f:
-            datasets = {data_location: f[data_location]} | {
-                k: f[v] for k, v in axes_locations.items()
-            }
+            datasets = {data_location: f[data_location]}
             keys = [f[k] for k in key_locations]
             ds = DataSource(keys, datasets)
+            axis_names = axes_locations.keys()
             for data_map in ds:
                 data = data_map[data_location]
+                # manually assemble the axes into a list
+                raw_axes = [f[k][()] for k in axes_locations.values()]
+
+                # mesh the axes to make something slicable
+                axes = np.meshgrid(*raw_axes, indexing="ij")
+                axis_values = [a[data_map.slice_metadata] for a in axes]
+                axis = {k: v for k, v in zip(axis_names, axis_values)}
+
+                logger.info(axis)
+
                 self.experiment.data_collections[0].set_raw_data(data)
+
                 scaled_experiment = scale_experiment(
                     self.experiment, self.configuration
                 )
                 [x(scaled_experiment) for x in self.procs]
 
-                axis = {k: data_map[k] for k in axes_locations.keys()}
                 scaled_results.add_scaled_experiment(
                     axis, scaled_experiment, save_as_we_go
                 )
                 scaled_results.process()
 
         logger.info("running complete.")
         if self._diagnostics_filepath != "":
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/scaler.py` & `vaxadium-0.3.0/vaxadium/scaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,14 +438,15 @@
     iterated_result = experiment.dc.pyfai.integrate1d(
         subtracted.squeeze(),
         pyfai_inst_npts,
         correctSolidAngle=False,
         unit=pyFAIunits.Q_A,
         radial_range=pyfai_inst_range,
         polarization_factor=configuration[CONFIGKEYS.POLARIZATION],
+        mask=experiment.mask,
     )
     #    qsq integral
     numerator = iterated_result[1]
     qsq_integral = np.trapz(numerator * q**2, x=q)
 
     #    correct the previous scale factor
     gain = gain + 10 * (qsq_integral - k_m)
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/__init__.py` & `vaxadium-0.3.0/vaxadium/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/basechecker.py` & `vaxadium-0.3.0/vaxadium/checks/basechecker.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/calibration.py` & `vaxadium-0.3.0/vaxadium/checks/calibration.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/convergence.py` & `vaxadium-0.3.0/vaxadium/checks/convergence.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/data.py` & `vaxadium-0.3.0/vaxadium/checks/data.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/extractor.py` & `vaxadium-0.3.0/vaxadium/checks/extractor.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/checks/sample.py` & `vaxadium-0.3.0/vaxadium/checks/sample.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/core/detector.py` & `vaxadium-0.3.0/vaxadium/core/detector.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/core/form_factors.py` & `vaxadium-0.3.0/vaxadium/core/form_factors.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/core/fourier.py` & `vaxadium-0.3.0/vaxadium/core/fourier.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/g4diffsim/fitting.py` & `vaxadium-0.3.0/vaxadium/g4diffsim/fitting.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/g4diffsim/macros.py` & `vaxadium-0.3.0/vaxadium/g4diffsim/macros.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/io/nexus_reader.py` & `vaxadium-0.3.0/vaxadium/io/nexus_reader.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/io/outputs.py` & `vaxadium-0.3.0/vaxadium/io/outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,26 +51,26 @@
 
         # add the axis
         nxaxis = nxdata.create_dataset(self.axis_name, data=self.axis)
         nxaxis.attrs["units"] = self.axis_unit
 
         # set the dataset
         self.nxdata = nxdata.create_dataset(
-            self.data_name, shape=(self.dim0, 0), maxshape=(self.dim0, MAX_NXS_SHAPE)
+            self.data_name, shape=(0, self.dim0), maxshape=(MAX_NXS_SHAPE, self.dim0)
         )
 
         # TODO sort this mess out
         self.nxdata.attrs["units"] = "counts"
 
     def _partial_write(self, scaled_result):
         logger.debug("_partial write called for {}".format(self.data_name))
-        new_shape = (self.dim0, self.n + 1)
+        new_shape = (self.n + 1, self.dim0)
         self.nxdata.resize(new_shape)
         data = getattr(scaled_result, self.data_name)
-        self.nxdata[:, -1] = data
+        self.nxdata[-1, :] = data
         self.nxdata.flush()
 
         if self.also_txt:
             self._write_txt_file(data)
 
         self.n += 1
```

### Comparing `vaxadium-0.2.0rc0/vaxadium/io/serializer_factory.py` & `vaxadium-0.3.0/vaxadium/io/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/io/serializers.py` & `vaxadium-0.3.0/vaxadium/io/serializers.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/attenuator.py` & `vaxadium-0.3.0/vaxadium/transmission/attenuator.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/beam.py` & `vaxadium-0.3.0/vaxadium/transmission/beam.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz.py` & `vaxadium-0.3.0/vaxadium/transmission/cylinder_yz.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz_runner.py` & `vaxadium-0.3.0/vaxadium/transmission/cylinder_yz_runner.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/direction.py` & `vaxadium-0.3.0/vaxadium/transmission/direction.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz.py` & `vaxadium-0.3.0/vaxadium/transmission/illuminated_yz.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz_runner.py` & `vaxadium-0.3.0/vaxadium/transmission/illuminated_yz_runner.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/scatterer.py` & `vaxadium-0.3.0/vaxadium/transmission/scatterer.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/transmission_map.py` & `vaxadium-0.3.0/vaxadium/transmission/transmission_map.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/vaxadium/transmission/yz_generator.py` & `vaxadium-0.3.0/vaxadium/transmission/yz_generator.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/.gitignore` & `vaxadium-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/LICENSE` & `vaxadium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/README.rst` & `vaxadium-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/pyproject.toml` & `vaxadium-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0rc0/PKG-INFO` & `vaxadium-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaxadium
-Version: 0.2.0rc0
+Version: 0.3.0
 Summary: Processes total scattering data using Monte Carlo simulations
 Project-URL: Homepage, https://github.com/DiamondLightSource/vaxadium
 Project-URL: Issues, https://github.com/DiamondLightSource/vaxadium/issues
 Author-email: Dean Keeble <dean.keeble@diamond.ac.uk>
 License-Expression: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
```

