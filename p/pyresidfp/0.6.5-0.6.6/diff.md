# Comparing `tmp/pyresidfp-0.6.5.tar.gz` & `tmp/pyresidfp-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.6.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyresidfp-0.6.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.6.5.tar` & `pyresidfp-0.6.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/.gitignore
--rw-r--r--   0        0        0     3914 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/COPYING
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/README.md
--rw-r--r--   0        0        0     2314 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/PythonSid.cpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/PythonSid.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/config.h.in
--rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/__init__.py
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/_version.py
--rw-r--r--   0        0        0     4147 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/musical_scale.py
--rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/registers.py
--rw-r--r--   0        0        0    10889 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/AUTHORS
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/COPYING
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Dac.cpp
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Dac.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/ExternalFilter.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/ExternalFilter.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter.cpp
--rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter6581.cpp
--rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter6581.h
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter8580.cpp
--rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter8580.h
--rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig.h
--rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator6581.cpp
--rw-r--r--   0        0        0     9200 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator6581.h
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator8580.cpp
--rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator8580.h
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/OpAmp.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/OpAmp.h
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Potentiometer.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/README
--rw-r--r--   0        0        0    13759 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/SID.cpp
--rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/SID.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Spline.cpp
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Spline.h
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Voice.h
--rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformCalculator.h
--rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformGenerator.h
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/array.h
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/Resampler.h
--rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/SincResampler.h
--rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/siddefs-fp.h.in
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/version.cc
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/sidcxx11.h
--rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/sidcxx14.h
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     3914 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/README.md
+-rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/PythonSid.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/config.h.in
+-rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0     8617 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/_pyresidfp/__init__.pyi
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/py.typed
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/COPYING
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9200 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/README
+-rw-r--r--   0        0        0    13759 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/Voice.h
+-rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/residfp/version.cc
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/sidcxx11.h
+-rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/src/sidcxx14.h
+-rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.6/PKG-INFO
```

### Comparing `pyresidfp-0.6.5/CMakeLists.txt` & `pyresidfp-0.6.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/COPYING` & `pyresidfp-0.6.6/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/README.md` & `pyresidfp-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/pyproject.toml` & `pyresidfp-0.6.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [tool.scikit-build]
 metadata.version.provider = "scikit_build_core.metadata.setuptools_scm"
-sdist.include = ["src/pyresidfp/_version.py"]
-sdist.exclude = [".github"]
+sdist.include = ["src/pyresidfp/_version.py", "src/pyresidfp/py.typed"]
+sdist.exclude = [".github", ".gitignore", "scripts"]
 wheel.packages = ["src/pyresidfp"]
 wheel.install-dir = "pyresidfp"
 minimum-version = "0.3"
 
 [tool.setuptools_scm]
 write_to = "src/pyresidfp/_version.py"
```

### Comparing `pyresidfp-0.6.5/src/PythonSid.cpp` & `pyresidfp-0.6.6/src/PythonSid.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/PythonSid.h` & `pyresidfp-0.6.6/src/PythonSid.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/pyresidfp/__init__.py` & `pyresidfp-0.6.6/src/pyresidfp/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,31 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from .musical_scale import Tone
-from .registers import AttackDecayBits, ControlBits, ModeVolBits, ReadableRegister, ResFiltBits, SustainReleaseBits, \
-    WritableRegister
+from .registers import (
+    AttackDecayBits,
+    ControlBits,
+    ModeVolBits,
+    ReadableRegister,
+    ResFiltBits,
+    SustainReleaseBits,
+    WritableRegister,
+)
 from .sound_interface_device import SoundInterfaceDevice, Voice, _VoiceRegister
 from ._version import version, version_tuple, __version__, __version_tuple__
 
 __all__ = [
-    "Tone", "AttackDecayBits", "ControlBits", "ModeVolBits", "ReadableRegister", "ResFiltBits", "SustainReleaseBits",
-    "WritableRegister", "SoundInterfaceDevice", "Voice",
+    "Tone",
+    "AttackDecayBits",
+    "ControlBits",
+    "ModeVolBits",
+    "ReadableRegister",
+    "ResFiltBits",
+    "SustainReleaseBits",
+    "WritableRegister",
+    "SoundInterfaceDevice",
+    "Voice",
 ]
```

### Comparing `pyresidfp-0.6.5/src/pyresidfp/registers.py` & `pyresidfp-0.6.6/src/pyresidfp/registers.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,64 +18,64 @@
 
 from enum import IntEnum, IntFlag
 
 
 class WritableRegister(IntEnum):
     """Writable registers on the MOS 6581"""
 
-    Voice1_Freq_Lo         = 0x00
-    Voice1_Freq_Hi         = 0x01
-    Voice1_Pw_Lo           = 0x02
-    Voice1_Pw_Hi           = 0x03
-    Voice1_Control_Reg     = 0x04
-    Voice1_Attack_Decay    = 0x05
+    Voice1_Freq_Lo = 0x00
+    Voice1_Freq_Hi = 0x01
+    Voice1_Pw_Lo = 0x02
+    Voice1_Pw_Hi = 0x03
+    Voice1_Control_Reg = 0x04
+    Voice1_Attack_Decay = 0x05
     Voice1_Sustain_Release = 0x06
 
-    Voice2_Freq_Lo         = 0x07
-    Voice2_Freq_Hi         = 0x08
-    Voice2_Pw_Lo           = 0x09
-    Voice2_Pw_Hi           = 0x0A
-    Voice2_Control_Reg     = 0x0B
-    Voice2_Attack_Decay    = 0x0C
+    Voice2_Freq_Lo = 0x07
+    Voice2_Freq_Hi = 0x08
+    Voice2_Pw_Lo = 0x09
+    Voice2_Pw_Hi = 0x0A
+    Voice2_Control_Reg = 0x0B
+    Voice2_Attack_Decay = 0x0C
     Voice2_Sustain_Release = 0x0D
 
-    Voice3_Freq_Lo         = 0x0E
-    Voice3_Freq_Hi         = 0x0F
-    Voice3_Pw_Lo           = 0x10
-    Voice3_Pw_Hi           = 0x11
-    Voice3_Control_Reg     = 0x12
-    Voice3_Attack_Decay    = 0x13
+    Voice3_Freq_Lo = 0x0E
+    Voice3_Freq_Hi = 0x0F
+    Voice3_Pw_Lo = 0x10
+    Voice3_Pw_Hi = 0x11
+    Voice3_Control_Reg = 0x12
+    Voice3_Attack_Decay = 0x13
     Voice3_Sustain_Release = 0x14
 
-    Filter_Fc_Lo           = 0x15
-    Filter_Fc_Hi           = 0x16
-    Filter_Res_Filt        = 0x17
-    Filter_Mode_Vol        = 0x18
+    Filter_Fc_Lo = 0x15
+    Filter_Fc_Hi = 0x16
+    Filter_Res_Filt = 0x17
+    Filter_Mode_Vol = 0x18
 
 
 class ReadableRegister(IntEnum):
     """Readable registers on the MOS 6581"""
 
-    Misc_Potx              = 0x19
-    Misc_Poty              = 0x1A
-    Misc_Osc3_Random       = 0x1B
-    Misc_Env3              = 0x1C
+    Misc_Potx = 0x19
+    Misc_Poty = 0x1A
+    Misc_Osc3_Random = 0x1B
+    Misc_Env3 = 0x1C
 
 
 class ControlBits(IntFlag):
     """Bits in control registers"""
 
-    GATE     = 2**0
-    SYNC     = 2**1
+    GATE = 2**0
+    SYNC = 2**1
     RING_MOD = 2**2
-    TEST     = 2**3
+    TEST = 2**3
     TRIANGLE = 2**4
     SAWTOOTH = 2**5
-    PULSE    = 2**6
-    NOISE    = 2**7
+    PULSE = 2**6
+    NOISE = 2**7
 
 
 class AttackDecayBits(IntFlag):
     """Bits in Attack/Decay registers"""
 
     DCY0 = 2**0
     DCY1 = 2**1
@@ -99,28 +99,28 @@
     STN2 = 2**6
     STN3 = 2**7
 
 
 class ResFiltBits(IntFlag):
     """Bits in Resonance/Filter register"""
 
-    Filt1  = 2**0
-    Filt2  = 2**1
-    Filt3  = 2**2
+    Filt1 = 2**0
+    Filt2 = 2**1
+    Filt3 = 2**2
     FiltEX = 2**3
-    RES0   = 2**4
-    RES1   = 2**5
-    RES2   = 2**6
-    RES3   = 2**7
+    RES0 = 2**4
+    RES1 = 2**5
+    RES2 = 2**6
+    RES3 = 2**7
 
 
 class ModeVolBits(IntFlag):
     """Bits in Mode/Volume register"""
 
-    VOL0      = 2**0
-    VOL1      = 2**1
-    VOL2      = 2**2
-    VOL3      = 2**3
-    LP        = 2**4
-    BP        = 2**5
-    HP        = 2**6
+    VOL0 = 2**0
+    VOL1 = 2**1
+    VOL2 = 2**2
+    VOL3 = 2**3
+    LP = 2**4
+    BP = 2**5
+    HP = 2**6
     THREE_OFF = 2**7
```

### Comparing `pyresidfp-0.6.5/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.6.6/src/pyresidfp/sound_interface_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ._pyresidfp import ChipModel, SID, SamplingMethod
 from .musical_scale import Tone
 from .registers import ReadableRegister, WritableRegister
 
 
 class Voice(Enum):
     """The three voices of an emulated MOS 6581 / MOS 8580"""
+
     ONE = 0
     TWO = 1
     THREE = 2
 
 
 class _VoiceRegister(Enum):
     """Voice-specific writable registers"""
@@ -54,26 +55,45 @@
         Returns:
             WritableRegister according to register type and voice
         """
         return WritableRegister(self.value + 7 * voice.value)
 
 
 class _Metaclass(type):
-    def __init__(cls, name: str, bases: t.Tuple[type, ...], attrs: t.Dict[str, t.Any]) -> None:
+    def __init__(
+        cls, name: str, bases: t.Tuple[type, ...], attrs: t.Dict[str, t.Any]
+    ) -> None:
         super(_Metaclass, cls).__init__(name, bases, attrs)
 
-        for register in WritableRegister:
-            setter = type(cls)._create_setter(register)
-            setattr(cls, register.name,
-                    property(fget=None, fset=setter, doc="int: Writable {0:s} 8-bit register".format(register.name)))
-
-        for register in ReadableRegister:
-            getter = type(cls)._create_getter(register)
-            setattr(cls, register.name,
-                    property(fget=getter, doc="int: Readable {0:s} 8-bit register".format(register.name)))
+        for writable_register in WritableRegister:
+            setter = type(cls)._create_setter(writable_register)
+            setattr(
+                cls,
+                writable_register.name,
+                property(
+                    fget=None,
+                    fset=setter,
+                    doc="int: Writable {0:s} 8-bit register".format(
+                        writable_register.name
+                    ),
+                ),
+            )
+
+        for readable_register in ReadableRegister:
+            getter = type(cls)._create_getter(readable_register)
+            setattr(
+                cls,
+                readable_register.name,
+                property(
+                    fget=getter,
+                    doc="int: Readable {0:s} 8-bit register".format(
+                        readable_register.name
+                    ),
+                ),
+            )
 
     @staticmethod
     def _create_setter(register: WritableRegister) -> t.Callable[[t.Any, int], None]:
         def setter(self, value: int) -> None:
             self.write_register(register, value)
 
         return setter
@@ -92,28 +112,32 @@
     PAL_CLOCK_FREQUENCY: float = 985248.0
     NTSC_CLOCK_FREQUENCY: float = 1022730.0
     DEFAULT_CLOCK_FREQUENCY: float = PAL_CLOCK_FREQUENCY
     DEFAULT_SAMPLING_RATE: float = 48000.0
     DEFAULT_SAMPLING_METHOD: SamplingMethod = SamplingMethod.RESAMPLE
     DEFAULT_CHIP_MODEL: ChipModel = ChipModel.MOS6581
 
-    def __init__(self,
-                 model: t.Optional[ChipModel] = None,
-                 sampling_method: t.Optional[SamplingMethod] = None,
-                 clock_frequency: t.Optional[int] = None,
-                 sampling_frequency: t.Optional[int] = None) -> None:
+    def __init__(
+        self,
+        model: t.Optional[ChipModel] = None,
+        sampling_method: t.Optional[SamplingMethod] = None,
+        clock_frequency: t.Optional[float] = None,
+        sampling_frequency: t.Optional[float] = None,
+    ) -> None:
         """Creates a new instance."""
         self._log = logging.getLogger(__name__)
         chip_model = model or type(self).DEFAULT_CHIP_MODEL
         sampling_method = sampling_method or type(self).DEFAULT_SAMPLING_METHOD
         clock_frequency = clock_frequency or type(self).DEFAULT_CLOCK_FREQUENCY
         sampling_frequency = sampling_frequency or type(self).DEFAULT_SAMPLING_RATE
         assert 0 < sampling_frequency <= clock_frequency
         assert 125.0 * clock_frequency / sampling_frequency < 16384.0
-        self._sid = SID(chip_model, sampling_method, clock_frequency, sampling_frequency)
+        self._sid = SID(
+            chip_model, sampling_method, clock_frequency, sampling_frequency
+        )
 
     @property
     def chip_model(self) -> ChipModel:
         """ChipModel: Chip model to emulate"""
         return self._sid.chip_model
 
     @chip_model.setter
@@ -246,16 +270,20 @@
 
         Returns:
             list of int containing the sampled output in -32768 to 32767 range
         """
         num_cycles = int(duration.total_seconds() * self.clock_frequency)
         num_samples = int(duration.total_seconds() * self.sampling_frequency)
 
-        self._log.debug("Clock for %f cycles (%f samples estimated) for an interval of %s",
-                        num_cycles, num_samples, duration)
+        self._log.debug(
+            "Clock for %f cycles (%f samples estimated) for an interval of %s",
+            num_cycles,
+            num_samples,
+            duration,
+        )
 
         # native sample format is signed 16-bit integers in host endianness
         result = self._sid.clock(num_cycles)
 
         self._log.debug("Retrieved %d samples", len(result))
 
         return result
@@ -288,31 +316,33 @@
 
         result = self._sid.read(register)
 
         self._log.debug("Read value %d from register %s", result, register)
 
         return result
 
-    def _write_voice_register(self, voice: Voice, register: _VoiceRegister, value: int) -> None:
-        register = register.voice_register(voice)
+    def _write_voice_register(
+        self, voice: Voice, register: _VoiceRegister, value: int
+    ) -> None:
+        writable_register = register.voice_register(voice)
 
-        self.write_register(register, value)
+        self.write_register(writable_register, value)
 
     @staticmethod
     def _split_filter_cutoff(filter_cutoff: int) -> tuple:
-        assert 0 <= filter_cutoff <= (2 ** 11 - 1)
+        assert 0 <= filter_cutoff <= (2**11 - 1)
 
         lo = filter_cutoff & 0x07
         hi = (filter_cutoff >> 3) & 0xFF
 
         return lo, hi
 
     @staticmethod
     def _split_pulse_width(pulse_width: int) -> tuple:
-        assert 0 <= pulse_width <= (2 ** 12 - 1)
+        assert 0 <= pulse_width <= (2**12 - 1)
 
         lo = pulse_width & 0xFF
         hi = (pulse_width >> 8) & 0x0F
 
         return lo, hi
 
     @staticmethod
```

### Comparing `pyresidfp-0.6.5/src/pyresidfp.cpp` & `pyresidfp-0.6.6/src/pyresidfp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/COPYING` & `pyresidfp-0.6.6/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Dac.cpp` & `pyresidfp-0.6.6/src/residfp/Dac.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Dac.h` & `pyresidfp-0.6.6/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.6.6/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.6.6/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/ExternalFilter.h` & `pyresidfp-0.6.6/src/residfp/ExternalFilter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Filter.cpp` & `pyresidfp-0.6.6/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Filter.h` & `pyresidfp-0.6.6/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Filter6581.cpp` & `pyresidfp-0.6.6/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Filter6581.h` & `pyresidfp-0.6.6/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Filter8580.cpp` & `pyresidfp-0.6.6/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Filter8580.h` & `pyresidfp-0.6.6/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.6.6/src/residfp/FilterModelConfig.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/FilterModelConfig.h` & `pyresidfp-0.6.6/src/residfp/FilterModelConfig.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.cpp` & `pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.6.6/src/residfp/FilterModelConfig6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.cpp` & `pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.6.6/src/residfp/FilterModelConfig8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Integrator6581.cpp` & `pyresidfp-0.6.6/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Integrator6581.h` & `pyresidfp-0.6.6/src/residfp/Integrator6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Integrator8580.cpp` & `pyresidfp-0.6.6/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Integrator8580.h` & `pyresidfp-0.6.6/src/residfp/Integrator8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/OpAmp.cpp` & `pyresidfp-0.6.6/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/OpAmp.h` & `pyresidfp-0.6.6/src/residfp/OpAmp.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Potentiometer.h` & `pyresidfp-0.6.6/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/README` & `pyresidfp-0.6.6/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/SID.cpp` & `pyresidfp-0.6.6/src/residfp/SID.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/SID.h` & `pyresidfp-0.6.6/src/residfp/SID.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Spline.cpp` & `pyresidfp-0.6.6/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Spline.h` & `pyresidfp-0.6.6/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/Voice.h` & `pyresidfp-0.6.6/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/WaveformCalculator.cpp` & `pyresidfp-0.6.6/src/residfp/WaveformCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/WaveformCalculator.h` & `pyresidfp-0.6.6/src/residfp/WaveformCalculator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.6.6/src/residfp/WaveformGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/WaveformGenerator.h` & `pyresidfp-0.6.6/src/residfp/WaveformGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/array.h` & `pyresidfp-0.6.6/src/residfp/array.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/resample/Resampler.h` & `pyresidfp-0.6.6/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.6.6/src/residfp/resample/SincResampler.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/resample/SincResampler.h` & `pyresidfp-0.6.6/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.6.6/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.6.6/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.6.6/src/residfp/siddefs-fp.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/residfp/version.cc` & `pyresidfp-0.6.6/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/sidcxx11.h` & `pyresidfp-0.6.6/src/sidcxx11.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/src/sidcxx14.h` & `pyresidfp-0.6.6/src/sidcxx14.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.5/PKG-INFO` & `pyresidfp-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.6.5
+Version: 0.6.6
 Summary: Emulates the SID sound-chip
 Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

