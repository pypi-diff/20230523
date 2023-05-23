# Comparing `tmp/pyMSVC-0.4.0.tar.gz` & `tmp/pyMSVC-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMSVC-0.4.0.tar", last modified: Mon Aug  1 06:26:30 2022, max compression
+gzip compressed data, was "pyMSVC-0.5.1.tar", last modified: Tue May 23 03:44:16 2023, max compression
```

## Comparing `pyMSVC-0.4.0.tar` & `pyMSVC-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 06:26:30.277370 pyMSVC-0.4.0/
--rw-rw-rw-   0        0        0     1265 2022-08-01 05:24:54.000000 pyMSVC-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      405 2022-08-01 06:26:30.276369 pyMSVC-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     7168 2022-08-01 05:24:54.000000 pyMSVC-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-01 06:26:30.253348 pyMSVC-0.4.0/pyMSVC/
--rw-rw-rw-   0        0        0   118470 2022-08-01 05:24:54.000000 pyMSVC-0.4.0/pyMSVC/__init__.py
--rw-rw-rw-   0        0        0    40884 2022-08-01 05:40:38.000000 pyMSVC-0.4.0/pyMSVC/vswhere.py
-drwxrwxrwx   0        0        0        0 2022-08-01 06:26:30.275368 pyMSVC-0.4.0/pyMSVC.egg-info/
--rw-rw-rw-   0        0        0      405 2022-08-01 06:26:30.000000 pyMSVC-0.4.0/pyMSVC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-08-01 06:26:30.000000 pyMSVC-0.4.0/pyMSVC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       78 2022-08-01 06:26:30.000000 pyMSVC-0.4.0/pyMSVC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-08-01 06:26:30.000000 pyMSVC-0.4.0/pyMSVC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-01 06:26:30.000000 pyMSVC-0.4.0/pyMSVC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-01 06:26:30.277370 pyMSVC-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      713 2022-08-01 05:34:48.000000 pyMSVC-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:44:16.202447 pyMSVC-0.5.1/
+-rw-rw-rw-   0        0        0     1265 2022-08-01 05:24:54.000000 pyMSVC-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-05-23 03:44:16.201447 pyMSVC-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8235 2022-08-02 05:12:16.000000 pyMSVC-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 03:44:16.184936 pyMSVC-0.5.1/pyMSVC/
+-rw-rw-rw-   0        0        0   127906 2023-05-23 03:35:27.000000 pyMSVC-0.5.1/pyMSVC/__init__.py
+-rw-rw-rw-   0        0        0    43493 2022-10-20 23:05:10.000000 pyMSVC-0.5.1/pyMSVC/vswhere.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:44:16.200448 pyMSVC-0.5.1/pyMSVC.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 03:44:16.000000 pyMSVC-0.5.1/pyMSVC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-05-23 03:40:23.000000 pyMSVC-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 03:44:16.202447 pyMSVC-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      590 2023-05-23 03:35:27.000000 pyMSVC-0.5.1/setup.py
```

### Comparing `pyMSVC-0.4.0/LICENSE` & `pyMSVC-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.4.0/README.md` & `pyMSVC-0.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pyMSVC
 
-A fairly stupid proof build environment setup for compiling c extensions using pythons distutils or setup tools.
+A fairly stupid proof build environment setup for compiling c extensions using pythons distutils or setuptools.
 
 I created this module because distutils does not do a good job at setting up a Windows build environment.
 Distutils relies on static paths for the MSVC compiler It does not detect Visual Studio Build tools installations. And 
 the largest problem with it is that it uses the vcvars*.bat files included with the compiler. It runs a subprocess 
 takes a snapshot of the computer's environment then runs vcvarsall and takes another snapshot of the environment. It 
 then compares the before and after and stores the differences between the 2. Now this would be a fantastic approach if
 Microsoft had made the vcvars*.bat files in a manner that would et up a correct build environment. There have been known issues
@@ -28,14 +28,15 @@
 
 * 10.0 Visual Studio 2010
 * 11.0 Visual Studio 2012
 * 12.0 Visual Studio 2013
 * 14.0 Visual Studio 2015
 * 14.1x Visual Studio 2017
 * 14.2x Visual Studio 2019
+* 14.3x Visual Studio 2022
 
 Python recommends that any extensions that are compiled on Windows should be compiled with the same MSVC version
 that was used to compile Python. This is due to incompatibilities in the common runtime language between the 
 compiler versions. You may or may not experience any issues if you do not use the same compiler version. Your extension 
 would have to use that portion of the CLR in order to have an issue. This is why it is a recommendation.
 
 
@@ -149,9 +150,38 @@
 * ***architecture***: x86 or x64
 * ***version***: Python version
 * ***dependency***: library name.. Python27.lib
 * ***includes***: include paths
 * ***libraries***: library paths
 
 
-Visual Studio 2019 has a whole new system for package installation. It no longer stores the information in the registry 
-for installed packages.
+Starting with Visual Studio 2017 Microsoft has added a COM interface that I am able to use
+to collect information about the installed versions of Visual Studio. 
+
+In order to collect pyMSVC to be able to use it in your build system you will 
+need to create a pyproject.toml file. In that file you need to have the following lines.
+
+    [build-system]
+    requires=["setuptools", "wheel", "pyMSVC;sys_platform=='win32'"]
+    build-backend="setuptools.build_meta"
+
+This will instruct pip to collect pyMSVC if the OS is Windows.
+In your setup.py file you want this at the top
+
+    import sys
+
+    if sys.platform.startswith('win'):
+        import pyMSVC
+        environment = pyMSVC.setup_environment()
+        print(environment)
+
+    import setuptools
+
+    # rest of setup code here
+
+The code above does everything for you. you do not need to create the 
+environment using `os.environ` and you do not have to pass any versions. 
+It will locate the compiler needed automatically if it is instaleld.  
+
+It's really that easy to use. You really don't have know the inner working of
+this library in order for it to be able to set up a proper build environment.
+
```

### Comparing `pyMSVC-0.4.0/pyMSVC/__init__.py` & `pyMSVC-0.5.1/pyMSVC/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,19 +34,38 @@
 # prone. It does not make an identical build environment.
 
 import os
 import sys
 import ctypes
 import subprocess
 import winreg
-import distutils.log
+import logging
 from typing import Optional, Union
+__version__ = '0.5.1'
 
 _IS_WIN = sys.platform.startswith('win')
 
+logger = logging.getLogger(__name__)
+
+
+def _setup_logging():
+    logger.setLevel(logging.DEBUG)
+    formatter = logging.Formatter('%(levelname)s: %(name)s: %(message)s')
+    logger_handler = logging.StreamHandler()
+    logger_handler.setFormatter(formatter)
+    logger.addHandler(logger_handler)
+
+
+for item in sys.argv:
+    if item.startswith('-v') or item == '--verbose':
+        _setup_logging()
+        break
+
+
+
 if _IS_WIN:
     try:
         from . import vswhere
     except ImportError:
         import vswhere
 
 _HRESULT = ctypes.c_long
@@ -112,17 +131,17 @@
     def _get_file_version(filename):
         dw_len = _GetFileVersionInfoSize(filename, None)
         if not dw_len:
             raise ctypes.WinError()
 
         lp_data = (_CHAR * dw_len)()
         if not _GetFileVersionInfo(
-            filename,
-            0,
-            ctypes.sizeof(lp_data), lp_data
+                filename,
+                0,
+                ctypes.sizeof(lp_data), lp_data
         ):
             raise ctypes.WinError()
 
         u_len = _UINT()
         lpffi = _POINTER(_VS_FIXEDFILEINFO)()
         lplp_buffer = ctypes.cast(ctypes.pointer(lpffi), _POINTER(_LPVOID))
         if not _VerQueryValue(lp_data, "\\", lplp_buffer, ctypes.byref(u_len)):
@@ -338,195 +357,14 @@
         )
 
     ver = '.'.join(str(item) for item in ver)
 
     return ver
 
 
-class Environment(object):
-
-    def __init__(
-        self,
-        minimum_c_version: Optional[Union[int, float]] = None,
-        strict_c_version: Optional[Union[int, float]] = None,
-        minimum_toolkit_version: Optional[int] = None,
-        strict_toolkit_version: Optional[int] = None,
-        minimum_sdk_version: Optional[str] = None,
-        strict_sdk_version: Optional[str] = None,
-        minimum_net_version: Optional[str] = None,
-        strict_net_version: Optional[str] = None,
-        vs_version: Optional[Union[str, int]] = None
-    ):
-        self.python = PythonInfo()
-
-        self.visual_c = VisualCInfo(
-            self,
-            minimum_c_version,
-            strict_c_version,
-            minimum_toolkit_version,
-            strict_toolkit_version,
-            vs_version
-        )
-
-        self.visual_studio = VisualStudioInfo(
-            self,
-            self.visual_c
-        )
-
-        self.windows_sdk = WindowsSDKInfo(
-            self,
-            self.visual_c,
-            minimum_sdk_version,
-            strict_sdk_version
-        )
-
-        self.dot_net = NETInfo(
-            self,
-            self.visual_c,
-            self.windows_sdk.version,
-            minimum_net_version,
-            strict_net_version
-        )
-
-    @property
-    def machine_architecture(self):
-        import platform
-        return 'x64' if '64' in platform.machine() else 'x86'
-
-    @property
-    def platform(self):
-        """
-        :return: x86 or x64
-        """
-        import platform
-
-        win_64 = self.machine_architecture == 'x64'
-        python_64 = platform.architecture()[0] == '64bit' and win_64
-
-        return 'x64' if python_64 else 'x86'
-
-    @property
-    def configuration(self):
-        """
-        Build configuration
-        :return: one of ReleaseDLL, DebugDLL
-        """
-
-        if os.path.splitext(sys.executable)[0].endswith('_d'):
-            config = 'Debug'
-        else:
-            config = 'Release'
-
-        return config
-
-    def __iter__(self):
-        for item in self.build_environment.items():
-            yield item
-
-    @property
-    def build_environment(self):
-        """
-        This would be the work horse. This is where all of the gathered
-        information is put into a single container and returned.
-        The information is then added to os.environ in order to allow the
-        build process to run properly.
-
-        List of environment variables generated:
-        PATH
-        LIBPATH
-        LIB
-        INCLUDE
-        Platform
-        FrameworkDir
-        FrameworkVersion
-        FrameworkDIR32
-        FrameworkVersion32
-        FrameworkDIR64
-        FrameworkVersion64
-        VCToolsRedistDir
-        VCINSTALLDIR
-        VCToolsInstallDir
-        VCToolsVersion
-        WindowsLibPath
-        WindowsSdkDir
-        WindowsSDKVersion
-        WindowsSdkBinPath
-        WindowsSdkVerBinPath
-        WindowsSDKLibVersion
-        __DOTNET_ADD_32BIT
-        __DOTNET_ADD_64BIT
-        __DOTNET_PREFERRED_BITNESS
-        Framework{framework version}Version
-        NETFXSDKDir
-        UniversalCRTSdkDir
-        UCRTVersion
-        ExtensionSdkDir
-
-        These last 2 are set to ensure that distuils uses these environment
-        variables when compiling libopenzwave.pyd
-        MSSDK
-        DISTUTILS_USE_SDK
-
-        :return: dict of environment variables
-        """
-        path = os.environ.get('Path', '')
-
-        env = dict(
-            __VSCMD_PREINIT_PATH=path,
-            Platform=self.platform,
-            VSCMD_ARG_app_plat='Desktop',
-            VSCMD_ARG_HOST_ARCH=self.platform,
-            VSCMD_ARG_TGT_ARCH=self.platform,
-            __VSCMD_script_err_count='0'
-        )
-
-        env_path = set()
-
-        def update_env(cls):
-            for key, value in cls:
-                if key == 'Path':
-                    for item in value.split(';'):
-                        env_path.add(item)
-                    continue
-
-                if key in env:
-                    env[key] += ';' + value
-                else:
-                    env[key] = value
-
-        update_env(self.visual_c)
-        update_env(self.visual_studio)
-        update_env(self.windows_sdk)
-        update_env(self.dot_net)
-
-        env['Path'] = (';'.join(env_path)) + ';' + path
-
-        return env
-
-    def __str__(self):
-        template = (
-            'Machine architecture: {machine_architecture}\n'
-            'Build architecture: {architecture}\n'
-        )
-
-        res = [
-            template.format(
-                machine_architecture=self.machine_architecture,
-                architecture=self.platform
-            ),
-            str(self.python),
-            str(self.visual_studio),
-            str(self.visual_c),
-            str(self.windows_sdk),
-            str(self.dot_net),
-        ]
-
-        return '\n'.join(res)
-
-
 # I have separated the environment into several classes
 # Environment - the main environment class.
 # the environment class is what is going to get used. this handles all of the
 # non specific bits of the environment. all of the rest of the classes are
 # brought together in the environment to form a complete build environment.
 
 # NETInfo - Any .NET related environment settings
@@ -538,47 +376,80 @@
 # VisualCInfo - Any VisualC environment settings
 
 # PythonInfo - This class really isnt for environment settings as such.
 # It is more of a convenience class. it will get things like a list of the
 # includes specific to the python build. the architecture of the version of
 # python that is running stuff along those lines.
 class PythonInfo(object):
+    """
+    Build information for the version of Python that is running.
+    """
 
     @property
     def architecture(self):
+        """
+        System "bitness"
+        :rtype: str
+        :return: "x64" or "x86"
+        """
         return 'x64' if sys.maxsize > 2 ** 32 else 'x86'
 
     @property
     def version(self):
+        """
+        Python version
+
+        :rtype: str
+        :return: Python version as a str
+        """
         return '.'.join(str(ver) for ver in sys.version_info)
 
     @property
     def dependency(self):
+        """
+        Python lib file
+
+        :rtype: str
+        """
         return 'Python%d%d.lib' % sys.version_info[:2]
 
     @property
     def includes(self):
+        """
+        Python include paths
+
+        :rtype: list
+        :return: list of str
+        """
         python_path = os.path.dirname(sys.executable)
         python_include = os.path.join(python_path, 'include')
 
         python_includes = [python_include]
         for root, dirs, files in os.walk(python_include):
             for d in dirs:
-                python_includes += [os.path.join(root, d)]
+                python_includes.append(os.path.join(root, d))
+
         return python_includes
 
     @property
     def libraries(self):
+        """
+        Python library files
+
+        :rtype: list
+        :return: list of str
+        """
         python_path = os.path.dirname(sys.executable)
         python_lib = os.path.join(python_path, 'libs')
 
         python_libs = [python_lib]
         for root, dirs, files in os.walk(python_lib):
             for d in dirs:
                 python_libs += [os.path.join(root, d)]
+
         return python_libs
 
     def __str__(self):
         template = (
             '== Python =====================================================\n'
             '  version: {py_version}\n'
             '  architecture: {py_architecture}\n'
@@ -592,23 +463,26 @@
             py_dependency=self.dependency,
             py_libraries=self.libraries,
             py_includes=self.includes
         )
 
 
 class VisualCInfo(object):
+    """
+    Information about the Visual C or Visual Studio installation.
+    """
 
     def __init__(
-        self,
-        environ: Environment,
-        minimum_c_version: Optional[Union[int, float]] = None,
-        strict_c_version: Optional[Union[int, float]] = None,
-        minimum_toolkit_version: Optional[int] = None,
-        strict_toolkit_version: Optional[int] = None,
-        vs_version: Optional[Union[str, int]] = None
+            self,
+            environ: "Environment",
+            minimum_c_version: Optional[Union[int, float]] = None,
+            strict_c_version: Optional[Union[int, float]] = None,
+            minimum_toolkit_version: Optional[int] = None,
+            strict_toolkit_version: Optional[int] = None,
+            vs_version: Optional[Union[str, int]] = None
     ):
         self.environment = environ
         self.platform = environ.platform
         self.strict_c_version = strict_c_version
         self.__installed_versions = None
         self._cpp_installation = None
         self._ide_install_directory = None
@@ -622,21 +496,24 @@
         self._msbuild_version = None
         self._msbuild_path = None
         self._product_semantic_version = None
         self._devinit_path = None
 
         self._strict_toolkit_version = strict_toolkit_version
         self._minimum_toolkit_version = minimum_toolkit_version
+
         py_version = sys.version_info[:2]
         if py_version in ((3, 4),):
             min_visual_c_version = 10.0
         elif py_version in ((3, 5), (3, 6), (3, 7), (3, 8)):
             min_visual_c_version = 14.0
         elif py_version in ((3, 9), (3, 10)):
             min_visual_c_version = 14.2
+        elif py_version in ((3, 11), (3, 12)):
+            min_visual_c_version = 14.3
         else:
             raise RuntimeError(
                 'This library does not support '
                 'python version %d.%d' % py_version
             )
 
         if (
@@ -658,14 +535,16 @@
             minimum_toolkit_version = str(minimum_toolkit_version / 10.0)
 
         self.minimum_c_version = minimum_c_version
         self._strict_toolkit_version = strict_toolkit_version
         self._minimum_toolkit_version = minimum_toolkit_version
 
         if _vswhere is not None:
+            logger.debug('\n' + str(_vswhere))
+
             cpp_id = 'Microsoft.VisualCpp.Tools.Host{0}.Target{1}'.format(
                 environ.machine_architecture.upper(),
                 environ.python.architecture.upper()
             )
 
             tools_id = (
                 'Microsoft.VisualCpp.Premium.Tools.'
@@ -675,27 +554,24 @@
                 environ.python.architecture.upper()
             )
 
             cpp_version = None
             cpp_installation = None
 
             for installation in _vswhere:
-
-                distutils.log.debug(str(installation) + '\n\n')
-
                 if vs_version is not None:
                     try:
                         if isinstance(vs_version, str):
                             display_version = str(
                                 installation.catalog.product_display_version
                             )
 
                             if (
-                                installation.version != vs_version and
-                                display_version != vs_version
+                                    installation.version != vs_version and
+                                    display_version != vs_version
                             ):
                                 continue
                         else:
                             product_line_version = int(
                                 installation.catalog.product_line_version
                             )
 
@@ -704,22 +580,22 @@
 
                     except:  # NOQA
                         continue
 
                 for package in installation.packages.vsix:
                     if package.id == cpp_id:
                         if (
-                            self.strict_c_version is not None and
-                            package != self.strict_c_version
+                                self.strict_c_version is not None and
+                                package != self.strict_c_version
                         ):
                             continue
 
                         if (
-                            self.minimum_c_version is not None and
-                            package < self.minimum_c_version
+                                self.minimum_c_version is not None and
+                                package < self.minimum_c_version
                         ):
                             continue
 
                         if cpp_version is None:
                             cpp_version = package
                             cpp_installation = installation
                         elif package > cpp_version:
@@ -737,15 +613,15 @@
                     'Tools',
                     'MSVC'
                 )
 
                 for package in cpp_installation.packages.vsix:
                     if package.id == tools_id:
                         if not os.path.exists(
-                            os.path.join(tools_path, package.version)
+                                os.path.join(tools_path, package.version)
                         ):
                             continue
 
                         if strict_toolkit_version is not None:
                             if package == strict_toolkit_version:
                                 tools_version = package
                                 break
@@ -779,16 +655,16 @@
 
                 else:
                     tools_version = tools_version.version
 
                 if tools_version is not None:
                     tools_version = tools_version.split('.')
                     self._toolset_version = (
-                        'v' + tools_version[0] +
-                        tools_version[1][0]
+                            'v' + tools_version[0] +
+                            tools_version[1][0]
                     )
                     self._tools_version = '.'.join(tools_version)
 
                     self._tools_install_directory = os.path.join(
                         tools_path, self._tools_version
                     )
 
@@ -797,15 +673,15 @@
                             'Tools',
                             'Redist'
                         )
                     )
 
                     if os.path.exists(tools_redist_directory):
                         self._tools_redist_directory = (
-                            tools_redist_directory + '\\'
+                                tools_redist_directory + '\\'
                         )
 
                         msvc_dll_path = os.path.join(
                             tools_redist_directory,
                             environ.python.architecture,
                             'Microsoft.VC{0}.CRT'.format(
                                 self._toolset_version[1:]
@@ -860,44 +736,101 @@
                     'devinit',
                     'devinit.exe'
                 )
                 if os.path.exists(devinit_path):
                     self._devinit_path = devinit_path
 
     @property
+    def has_ninja(self) -> bool:
+        """
+        Is Ninja installed.
+
+        :rtype: bool
+        :return: `True`/`False`
+        """
+        ide_path = os.path.split(self.ide_install_directory)[0]
+        ninja_path = os.path.join(
+            ide_path,
+            'CommonExtensions',
+            'Microsoft',
+            'CMake',
+            'Ninja',
+            'ninja.exe'
+        )
+        return os.path.exists(ninja_path)
+
+    @property
+    def has_cmake(self) -> bool:
+        """
+        Is CMAKE installed.
+
+        :rtype: bool
+        :return: `True`/`False`
+        """
+        ide_path = os.path.split(self.ide_install_directory)[0]
+
+        cmake_path = os.path.join(
+            ide_path,
+            'CommonExtensions',
+            'Microsoft',
+            'CMake',
+            'CMake',
+            'bin',
+            'cmake.exe'
+        )
+        return os.path.exists(cmake_path)
+
+    @property
     def cmake_paths(self) -> list:
+        """
+        Paths to CMAKE
+
+        Gets added to the PATH environment variable.
+
+        :rtype: list
+        :return: `list` of `str`
+        """
         paths = []
         ide_path = os.path.split(self.ide_install_directory)[0]
 
         cmake_path = os.path.join(
             ide_path,
             'CommonExtensions',
             'Microsoft',
             'CMake'
         )
 
         if os.path.exists(cmake_path):
             bin_path = os.path.join(cmake_path, 'CMake', 'bin')
             ninja_path = os.path.join(cmake_path, 'Ninja')
             if os.path.exists(bin_path):
-                paths += [bin_path]
+                paths.append(bin_path)
 
             if os.path.exists(ninja_path):
-                paths += [ninja_path]
+                paths.append(ninja_path)
 
         return paths
 
     @property
     def cpp_installation(
-        self
+            self
     ) -> Union[vswhere.ISetupInstance, vswhere.ISetupInstance2]:
         return self._cpp_installation
 
     @property
     def f_sharp_path(self) -> Optional[str]:
+        """
+        Path to F#
+
+        Gets set to the FSHARPINSTALLDIR envioronment variable.
+        Gets added to the PATH environment variable.
+
+        :rtype: Optional, str
+        :return: path to F# or `None`
+        """
         version = float(int(self.version.split('.')[0]))
 
         reg_path = (
             winreg.HKEY_LOCAL_MACHINE,
             r'SOFTWARE\Microsoft\VisualStudio'
             r'\{0:.1f}\Setup\F#'.format(version)
         )
@@ -943,14 +876,21 @@
             'Tools'
         )
         if os.path.exists(f_sharp_path):
             return f_sharp_path
 
     @property
     def ide_install_directory(self) -> str:
+        """
+        IDE (Visual Studio) installation path
+
+        Gets set as the VCIDEInstallDir environment variable.
+
+        :rtype: str
+        """
         if self._ide_install_directory is None:
             directory = self.install_directory
             ide_directory = os.path.abspath(
                 os.path.join(directory, '..')
             )
 
             ide_directory = os.path.join(
@@ -964,15 +904,19 @@
 
         return self._ide_install_directory
 
     @property
     def install_directory(self) -> str:
         """
         Visual C path
-        :return: Visual C path
+
+        Gets set as the VCINSTALLDIR environment variable.
+        Gets added to the PATH environment variable.
+
+        :rtype: str
         """
         if self._install_directory is None:
             self._install_directory = (
                 self._installed_c_paths[self.version]['base']
             )
 
         return self._install_directory
@@ -1094,18 +1038,18 @@
                     version = float(key)
                 except ValueError:
                     continue
 
                 path = _get_reg_value(reg_path, key)
 
                 if (
-                    (
-                        os.path.exists(path) and
-                        version not in self.__installed_versions
-                    ) or version == 15.0
+                        (
+                                os.path.exists(path) and
+                                version not in self.__installed_versions
+                        ) or version == 15.0
                 ):
 
                     if version == 15.0:
                         version = 14.0
 
                     if not os.path.split(path)[1] == 'VC':
                         path = os.path.join(path, 'VC')
@@ -1130,14 +1074,15 @@
         that was used to compile Python has to also be used to compile an
         extension. I have this system set so it will automatically pick the
         most recent compiler installation. this can be overridden in 2 ways.
         The first way being that the compiler version that built Python has to
         be used. The second way is you can set a minimum compiler version to
         use.
 
+        :rtype: str
         :return: found Visual C version
         """
         if self._cpp_version is None:
             if self.strict_c_version is not None:
                 if self.strict_c_version not in self._installed_c_paths:
                     raise RuntimeError(
                         'No Compatible Visual C version found.'
@@ -1164,87 +1109,77 @@
 
             self._cpp_version = str(match)
 
         return self._cpp_version
 
     @property
     def tools_version(self) -> str:
+        """
+        Build tools version
+
+        Gets set into the VCToolsVersion environment variable.
+
+        :rtype: str
+        """
         if self._tools_version is None:
             version = os.path.split(self.tools_install_directory)[1]
             if not version.split('.')[-1].isdigit():
                 version = str(self.version)
 
             self._tools_version = version
 
         return self._tools_version
 
     @property
     def toolset_version(self) -> str:
         """
         The platform toolset gets written to the solution file. this instructs
         the compiler to use the matching MSVCPxxx.dll file.
+
+        :rtype: str
         """
 
         if self._toolset_version is None:
             tools_version = self.tools_version.split('.')
 
             self._toolset_version = (
-                'v' +
-                tools_version[0] +
-                tools_version[1][:1]
-            )
-            #
-            #
-            # tool_path = self.tools_redist_directory
-            # x64 = self.platform == 'x64'
-            #
-            # dirs = os.listdir(self.tools_redist_directory)
-            #
-            #
-            # if x64:
-            #     if 'amd64' in dirs:
-            #         tool_path = os.path.join(tool_path, 'amd64')
-            #     else:
-            #         tool_path = os.path.join(tool_path, 'x64')
-            #
-            # else:
-            #     tool_path = os.path.join(tool_path, 'x86')
-            #
-            # if os.path.exists(tool_path):
-            #     max_ver = 0
-            #
-            #     for f in os.listdir(tool_path):
-            #         if not f.endswith('CRT'):
-            #             continue
-            #         try:
-            #             ver = int(f.split('.')[1].lstrip('VC'))
-            #             max_ver = max(max_ver, ver)
-            #         except:
-            #             continue
-            #
-            #     if max_ver != 0:
-            #         self._toolset_version = 'v' + str(max_ver)
+                    'v' +
+                    tools_version[0] +
+                    tools_version[1][:1]
+            )
 
         return self._toolset_version
 
     @property
     def msvc_dll_version(self) -> Optional[str]:
+        """
+        The Version of the MSVC DLL file that was found
+
+        :rtype: Optional, str
+        :return: `str` version of the DLL or `None`
+        """
         msvc_dll_path = self.msvc_dll_path
         if not msvc_dll_path:
             return
 
         for f in os.listdir(msvc_dll_path):
             if f.endswith('dll'):
                 version = _get_file_version(
                     os.path.join(msvc_dll_path, f)
                 )
                 return '.'.join(str(ver) for ver in version)
 
     @property
     def msvc_dll_path(self) -> Optional[str]:
+        """
+        Path to the MSVC DLL if found
+
+        :rtype: Optional, str
+        :return: path to DLL or `None`
+        """
         if self._msvc_dll_path is None:
             x64 = self.platform == 'x64'
 
             toolset_version = self.toolset_version
 
             if toolset_version is None:
                 return None
@@ -1270,39 +1205,47 @@
                         if x64 and ('amd64' in root or 'x64' in root):
                             self._msvc_dll_path = os.path.join(
                                 root,
                                 folder_name
                             )
                             break
                         elif (
-                            not x64 and
-                            'amd64' not in root
-                            and 'x64' not in root
+                                not x64 and
+                                'amd64' not in root
+                                and 'x64' not in root
                         ):
                             self._msvc_dll_path = os.path.join(
                                 root,
                                 folder_name
                             )
                             break
 
         return self._msvc_dll_path
 
     @property
     def tools_redist_directory(self) -> Optional[str]:
+        """
+        Path to the tools redistributable directory.
+
+        Gets set into the VCToolsRedistDir environment variable.
+
+        :rtype: Optional, str
+        :return: path or `None`
+        """
         if self._tools_redist_directory is None:
             tools_install_path = self.tools_install_directory
 
             if 'MSVC' in tools_install_path:
                 redist_path = tools_install_path.replace(
                     'Tools',
                     'Redist'
                 )
                 if (
-                    not os.path.exists(redist_path) and
-                    'BuildTools' in tools_install_path
+                        not os.path.exists(redist_path) and
+                        'BuildTools' in tools_install_path
                 ):
                     redist_path = redist_path.replace(
                         'BuildRedist', 'BuildTools'
                     )
             else:
                 redist_path = os.path.join(
                     tools_install_path,
@@ -1311,15 +1254,15 @@
 
             if not os.path.exists(redist_path):
                 redist_path = os.path.split(redist_path)[0]
                 tools_version = None
 
                 for version in os.listdir(redist_path):
                     if not os.path.isdir(
-                        os.path.join(redist_path, version)
+                            os.path.join(redist_path, version)
                     ):
                         continue
 
                     if version.startswith('v'):
                         continue
 
                     if self._strict_toolkit_version is not None:
@@ -1349,26 +1292,31 @@
                 else:
                     self._tools_redist_directory = ''
 
             else:
                 self._tools_redist_directory = redist_path
 
             if (
-                self._tools_redist_directory and
-                not self._tools_redist_directory.endswith('\\')
+                    self._tools_redist_directory and
+                    not self._tools_redist_directory.endswith('\\')
             ):
                 self._tools_redist_directory += '\\'
 
         return self._tools_redist_directory
 
     @property
     def tools_install_directory(self) -> Optional[str]:
         """
         Visual C compiler tools path.
-        :return: Path to the compiler tools
+
+        Gets set to the VCToolsInstallDir environment variable.
+        Gets added to the INCLUDE, LIBPATH, LIB and PATH environment variables.
+
+        :rtype: Optional, str
+        :return: Path to the compiler tools or `None`
         """
         if self._tools_install_directory is None:
 
             vc_version = float(int(self.version.split('.')[0]))
             if vc_version >= 14.0:
                 vc_tools_path = self._installed_c_paths[vc_version]['root']
             else:
@@ -1416,29 +1364,40 @@
 
         return self._tools_install_directory
 
     @property
     def msbuild_version(self) -> Optional[str]:
         """
         MSBuild versions are specific to the Visual C version
-        :return: MSBuild version, 3.5, 4.0, 12, 14, 15
+
+        :rtype: Optional, str
+        :return: MSBuild version, `"3.5"`, `"4.0"`, `"12"`, `"14"`,
+          `"15"` or `None`
         """
         if self._msbuild_version is None:
             vc_version = str(float(int(self.version.split('.')[0])))
 
             if vc_version == 9.0:
                 self._msbuild_version = '3.5'
             elif vc_version in (10.0, 11.0):
                 self._msbuild_version = '4.0'
             else:
                 self._msbuild_version = vc_version
         return self._msbuild_version
 
     @property
     def msbuild_path(self) -> Optional[str]:
+        """
+        Path to MSBuild
+
+        Gets added to the PATH environment variable.
+
+        :rtype: Optional, str
+        :return: path to MSBuild or `None`
+        """
         if self._msbuild_path is not None:
             program_files = os.environ.get(
                 'ProgramFiles(x86)',
                 'C:\\Program Files (x86)'
             )
 
             version = float(int(self.version.split('.')[0]))
@@ -1462,32 +1421,45 @@
             if os.path.exists(ms_build_path):
                 self._msbuild_path = ms_build_path
 
         return self._msbuild_path
 
     @property
     def html_help_path(self) -> Optional[str]:
+        """
+        Path to HTMLHelp
 
+        Gets set to the HTMLHelpDir environment variable.
+
+        :rtype: Optional, str
+        :return: path to HTMLHelp or `None`
+        """
         reg_path = (
             winreg.HKEY_LOCAL_MACHINE,
             r'SOFTWARE\Wow6432Node\Microsoft\Windows'
             r'\CurrentVersion\App Paths\hhw.exe'
         )
 
         html_help_path = _get_reg_value(reg_path, 'Path')
         if html_help_path and os.path.exists(html_help_path):
             return html_help_path
 
         if os.path.exists(
-            r'C:\Program Files (x86)\HTML Help Workshop'
+                r'C:\Program Files (x86)\HTML Help Workshop'
         ):
             return r'C:\Program Files (x86)\HTML Help Workshop'
 
     @property
     def path(self) -> list:
+        """
+        Locations that need to be added to the "PATH" environment variable
+
+        :rtype: list
+        :return: `list` of `str`
+        """
         tools_path = self.tools_install_directory
         base_path = os.path.join(tools_path, 'bin')
 
         path = []
 
         f_sharp_path = self.f_sharp_path
         msbuild_path = self.msbuild_path
@@ -1614,34 +1586,21 @@
             path += [bin_path]
 
         path += self.cmake_paths
 
         return path
 
     @property
-    def atlmfc_lib_path(self) -> Optional[str]:
-        atlmfc_path = self.atlmfc_path
-        if not atlmfc_path:
-            return
-
-        atlmfc = os.path.join(atlmfc_path, 'lib')
-        if self.platform == 'x64':
-            atlmfc_path = os.path.join(atlmfc, 'x64')
-            if not os.path.exists(atlmfc_path):
-                atlmfc_path = os.path.join(atlmfc, 'amd64')
-        else:
-            atlmfc_path = os.path.join(atlmfc, 'x86')
-            if not os.path.exists(atlmfc_path):
-                atlmfc_path = atlmfc
-
-        if os.path.exists(atlmfc_path):
-            return atlmfc_path
-
-    @property
     def lib(self) -> list:
+        """
+        Gets added to the LIB environment variable.
+
+        :rtype: list
+        :return: list of str
+        """
         tools_path = self.tools_install_directory
         path = os.path.join(tools_path, 'lib')
 
         if self.platform == 'x64':
             lib_path = os.path.join(path, 'x64')
             if not os.path.exists(lib_path):
                 lib_path = os.path.join(path, 'amd64')
@@ -1660,14 +1619,20 @@
         if atlmfc_path is not None:
             lib += [atlmfc_path]
 
         return lib
 
     @property
     def lib_path(self) -> list:
+        """
+        Gets added to the LIBPATH environment variable.
+
+        :rtype: list
+        :return: list of str
+        """
         tools_path = self.tools_install_directory
         path = os.path.join(tools_path, 'lib')
 
         if self.platform == 'x64':
             lib = os.path.join(path, 'x64')
             if not os.path.exists(lib):
                 lib = os.path.join(path, 'amd64')
@@ -1689,40 +1654,88 @@
         atlmfc_path = self.atlmfc_lib_path
 
         if atlmfc_path is not None:
             lib_path += [atlmfc_path]
 
         if os.path.exists(references_path):
             lib_path += [references_path]
+        else:
+            references_path = os.path.join(path, 'x86', 'store', 'references')
+            if os.path.exists(references_path):
+                lib_path += [references_path]
 
         return lib_path
 
     @property
+    def atlmfc_lib_path(self) -> Optional[str]:
+
+        """
+        Gets added to the LIBPATH and LIB environment variables
+
+        :rtype: Optional, str
+        :return: str or `None`
+        """
+        atlmfc_path = self.atlmfc_path
+        if not atlmfc_path:
+            return
+
+        atlmfc = os.path.join(atlmfc_path, 'lib')
+        if self.platform == 'x64':
+            atlmfc_path = os.path.join(atlmfc, 'x64')
+            if not os.path.exists(atlmfc_path):
+                atlmfc_path = os.path.join(atlmfc, 'amd64')
+        else:
+            atlmfc_path = os.path.join(atlmfc, 'x86')
+            if not os.path.exists(atlmfc_path):
+                atlmfc_path = atlmfc
+
+        if os.path.exists(atlmfc_path):
+            return atlmfc_path
+
+    @property
     def atlmfc_path(self) -> Optional[str]:
+        """
+        Path to atlmfc directory
+
+        :rtype: Optional, str
+        :return: str o `None`
+        """
         tools_path = self.tools_install_directory
         atlmfc_path = os.path.join(tools_path, 'ATLMFC')
 
         if os.path.exists(atlmfc_path):
             return atlmfc_path
 
     @property
     def atlmfc_include_path(self) -> Optional[str]:
+        """
+        Gets added to the INCLUDE environment variable.
+
+        :rtype: Optional str
+        :return: str or `None`
+        """
         atlmfc_path = self.atlmfc_path
         if atlmfc_path is None:
             return
 
         atlmfc_include_path = os.path.join(
             atlmfc_path,
             'include'
         )
         if os.path.exists(atlmfc_include_path):
             return atlmfc_include_path
 
     @property
     def include(self) -> list:
+        """
+        Gets set to the INCLUDE environment variable.
+
+        :rtype: list
+        :return: list of str
+        """
         tools_path = self.tools_install_directory
         include_path = os.path.join(tools_path, 'include')
         atlmfc_path = self.atlmfc_include_path
 
         include = []
         if os.path.exists(include_path):
             include += [include_path]
@@ -1749,19 +1762,24 @@
             VCIDEInstallDir=ide_install_directory,
             VCToolsVersion=self.tools_version,
             VCToolsInstallDir=tools_install_directory,
             VCINSTALLDIR=install_directory,
             VCToolsRedistDir=self.tools_redist_directory,
             Path=self.path,
             LIB=self.lib,
-            Include=self.include,
+            INCLUDE=self.include,
             LIBPATH=self.lib_path,
             FSHARPINSTALLDIR=self.f_sharp_path
         )
 
+        html_help = self.html_help_path
+
+        if html_help is not None:
+            env['HTMLHelpDir'] = html_help
+
         if self._product_semantic_version is not None:
             env['VSCMD_VER'] = self._product_semantic_version
 
         if self._devinit_path is not None:
             env['__devinit_path'] = self._devinit_path
 
         for key, value in env.items():
@@ -1769,16 +1787,18 @@
                 if isinstance(value, list):
                     value = os.pathsep.join(value)
                 yield key, str(value)
 
     def __str__(self):
         template = (
             '== Visual C ===================================================\n'
-            '   version: {visual_c_version}\n'
-            '   path:    {visual_c_path}\n'
+            '   version:   {visual_c_version}\n'
+            '   path:      {visual_c_path}\n'
+            '   has cmake: {has_cmake}\n'
+            '   has ninja: {has_ninja}\n'
             '\n'
             '   -- Tools ---------------------------------------------------\n'
             '      version:     {tools_version}\n'
             '      path:        {tools_install_path}\n'
             '      redist path: {vc_tools_redist_path}\n'
             '   -- F# ------------------------------------------------------\n'
             '      path: {f_sharp_path}\n'
@@ -1798,14 +1818,16 @@
             '   include path: {atlmfc_include_path}\n'
             '   lib path:     {atlmfc_lib_path}\n'
         )
 
         return template.format(
             visual_c_version=self.version,
             visual_c_path=self.install_directory,
+            has_cmake=self.has_cmake,
+            has_ninja=self.has_ninja,
             tools_version=self.tools_version,
             tools_install_path=self.tools_install_directory,
             vc_tools_redist_path=self.tools_redist_directory,
             platform_toolset=self.toolset_version,
             msvc_dll_version=self.msvc_dll_version,
             msvc_dll_path=self.msvc_dll_path,
             msbuild_version=self.msbuild_version,
@@ -1817,17 +1839,17 @@
             atlmfc_path=self.atlmfc_path,
         )
 
 
 class VisualStudioInfo(object):
 
     def __init__(
-        self,
-        environ: Environment,
-        c_info: VisualCInfo
+            self,
+            environ: "Environment",
+            c_info: VisualCInfo
     ):
         self.environment = environ
         self.__devenv_version = None
         self.c_info = c_info
         self._install_directory = None
         self._dev_env_directory = None
         self._common_tools = None
@@ -1845,51 +1867,68 @@
                 installation.version
             )
 
             install_directory = installation.path
             if os.path.exists(install_directory):
                 self._install_directory = install_directory
 
-                dev_env_directory = os.path.split(installation.product_path)[0]
-
+                dev_env_directory = os.path.join(
+                    install_directory,
+                    os.path.split(installation.product_path)[0]
+                )
                 if os.path.exists(dev_env_directory):
                     self._dev_env_directory = dev_env_directory
 
                 common_tools = os.path.join(
                     install_directory, 'Common7', 'Tools'
                 )
                 if os.path.exists(common_tools):
                     self._common_tools = common_tools + '\\'
 
     @property
     def install_directory(self) -> str:
+        """
+        Visual Studio installation directory.
+
+        :rtype: str
+        """
         if self._install_directory is None:
             install_dir = os.path.join(
                 self.c_info.install_directory,
                 '..'
             )
 
             self._install_directory = (
                 os.path.abspath(install_dir)
             )
         return self._install_directory
 
     @property
     def dev_env_directory(self) -> str:
+        """
+        Directory that devenv.exe is located.
+
+        :rtype: str
+        """
         if self._dev_env_directory is None:
             self._dev_env_directory = os.path.join(
                 self.install_directory,
                 'Common7',
                 'IDE'
             )
 
         return self._dev_env_directory
 
     @property
     def common_tools(self) -> str:
+        """
+        CommonTools path.
+
+        :rtype: str
+        """
         if self._common_tools is None:
 
             common_tools = os.path.join(
                 self.install_directory,
                 'Common7',
                 'Tools'
             )
@@ -1898,14 +1937,20 @@
             else:
                 self._common_tools = ''
 
         return self._common_tools
 
     @property
     def path(self) -> list:
+        """
+        Gets added to the PATH environment variable.
+
+        :rtype: list
+        :return: list of str
+        """
         path = []
 
         dev_env_directory = self.dev_env_directory
         if dev_env_directory:
             path.append(dev_env_directory)
 
         common_tools = self.common_tools
@@ -1914,16 +1959,16 @@
             path.append(common_tools[:-1])
 
         collection_tools_dir = _get_reg_value(
             'VisualStudio\\VSPerf',
             'CollectionToolsDir'
         )
         if (
-            collection_tools_dir and
-            os.path.exists(collection_tools_dir)
+                collection_tools_dir and
+                os.path.exists(collection_tools_dir)
         ):
             path.append(collection_tools_dir)
 
         vs_ide_path = self.dev_env_directory
 
         test_window_path = os.path.join(
             vs_ide_path,
@@ -1948,21 +1993,19 @@
 
     @property
     def __version(self):
         if not isinstance(self.__devenv_version, tuple):
             dev_env_dir = self.dev_env_directory
 
             if dev_env_dir is not None:
-                command = ''.join(
-                    [
-                        '"',
-                        os.path.join(dev_env_dir, 'devenv'),
-                        '" /?\n'
-                    ]
-                )
+                command = ''.join([
+                    '"',
+                    os.path.join(dev_env_dir, 'devenv'),
+                    '" /?\n'
+                ])
 
                 proc = subprocess.Popen(
                     'cmd',
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     stdin=subprocess.PIPE,
                     shell=True
@@ -1994,22 +2037,52 @@
             else:
                 self.__devenv_version = (None, None)
 
         return self.__devenv_version
 
     @property
     def common_version(self) -> Optional[str]:
+        """
+        Visual Studio version
+
+        Example
+        "Microsoft Visual Studio 2022 Version 17.0.5"
+        the common version is "2022"
+
+        :rtype: Optional, str
+        :return: str or `None`
+        """
         return self.__version[0]
 
     @property
     def uncommon_version(self) -> Optional[str]:
+        """
+        Visual Studio version
+
+        Example
+        "Microsoft Visual Studio 2022 Version 17.0.5"
+        the uncommon version is "17.0.5"
+
+        :rtype: Optional, str
+        :return: str or `None`
+        """
         return self.__version[1]
 
     @property
     def version(self) -> Optional[float]:
+        """
+        Visual Studio version
+
+        Example
+        "Microsoft Visual Studio 2022 Version 17.0.5"
+        the version is 17.0
+
+        :rtype: Optional, float
+        :return: float or `None`
+        """
         version = self.uncommon_version
 
         if version is not None:
             return float(int(version.split('.')[0]))
 
     def __iter__(self):
         install_directory = self.install_directory
@@ -2031,15 +2104,15 @@
         toolsets = {
             'v142': '160',
             'v141': '150',
             'v140': '140',
             'v120': '120',
             'v110': '110',
             'v100': '100',
-            'v90' : '90'
+            'v90': '90'
         }
 
         toolset_version = self.c_info.toolset_version
 
         if toolset_version in toolsets:
             comn_tools = 'VS{0}COMNTOOLS'.format(
                 toolsets[toolset_version]
@@ -2055,16 +2128,17 @@
     def __str__(self):
         installation = self.c_info.cpp_installation
 
         if installation is None:
             return ''
 
         template = (
-            '== {name}==============================================\n'
+            '== {name} \n'
             '   description:        {description}\n'
+            '   install date:       {install_date}\n'
             '   version:            {version}\n'
             '   version (friendly): {product_line_version}\n'
             '   display version:    {product_display_version}\n'
             '   path:               {path}\n'
             '   executable:         {product_path}\n'
             '   is complete:        {is_complete}\n'
             '   is prerelease:      {is_prerelease}\n'
@@ -2072,70 +2146,76 @@
             '   state:              {state}\n'
         )
 
         name = installation.display_name
 
         if name is None:
             if self.__name__ == 'VisualStudioInfo':
-                name = 'Visual Studio '
+                name = 'Visual Studio'
             else:
-                name = 'Build Tools =='
+                name = 'Build Tools'
 
         description = installation.description
         path = installation.path
+        install_date = installation.install_date.strftime('%c')
         version = installation.version
         is_complete = installation.is_complete
         is_prerelease = installation.is_prerelease
         is_launchable = installation.is_launchable
         state = ', '.join(installation.state)
-        product_path = installation.product_path
+        product_path = os.path.join(path, installation.product_path)
 
         catalog = installation.catalog
         product_display_version = catalog.product_display_version
         product_line_version = catalog.product_line_version
 
-        return template.format(
+        res = template.format(
             name=name,
             description=description,
+            install_date=install_date,
             path=path,
             version=version,
             is_complete=is_complete,
             is_prerelease=is_prerelease,
             is_launchable=is_launchable,
             product_path=product_path,
             product_display_version=product_display_version,
             product_line_version=product_line_version,
             state=state
         )
 
+        res = res.split('\n', 1)
+        res[0] += '=' * (63 - len(res[0]))
+        return '\n'.join(res)
+
 
 class WindowsSDKInfo(object):
 
     def __init__(
-        self,
-        environ: Environment,
-        c_info: VisualCInfo,
-        minimum_sdk_version: Optional[str] = None,
-        strict_sdk_version: Optional[str] = None
+            self,
+            environ: "Environment",
+            c_info: VisualCInfo,
+            minimum_sdk_version: Optional[str] = None,
+            strict_sdk_version: Optional[str] = None
     ):
         self.environment = environ
         self.c_info = c_info
         self.platform = environ.platform
         self.vc_version = c_info.version
 
         if (
-            strict_sdk_version is not None and
-            strict_sdk_version.startswith('10.0')
+                strict_sdk_version is not None and
+                strict_sdk_version.startswith('10.0')
         ):
             if strict_sdk_version.count('.') == 2:
                 strict_sdk_version += '.0'
 
         if (
-            minimum_sdk_version is not None and
-            minimum_sdk_version.startswith('10.0')
+                minimum_sdk_version is not None and
+                minimum_sdk_version.startswith('10.0')
         ):
             if minimum_sdk_version.count('.') == 2:
                 minimum_sdk_version += '.0'
 
         self._minimum_sdk_version = minimum_sdk_version
         self._strict_sdk_version = strict_sdk_version
 
@@ -2533,15 +2613,17 @@
 
         return lib_path
 
     @property
     def windows_sdks(self) -> list:
         """
         Windows SDK versions that are compatible with Visual C
-        :return: compatible Windows SDK versions
+
+        :rtype: list
+        :return: list of compatible Windows SDK versions
         """
         ver = int(self.vc_version.split('.')[0])
 
         sdk_versions = []
         if ver >= 14:
             sdk_versions.extend(['v10.0'])
         if ver >= 12:
@@ -2550,30 +2632,31 @@
             sdk_versions.extend(['v8.0a', 'v8.0'])
         if ver >= 10:
             sdk_versions.extend(['v7.1a', 'v7.1', 'v7.0a'])
 
         sdk_versions.extend(['v7.0', 'v6.1', 'v6.0a'])
 
         if (
-            self._minimum_sdk_version is not None and
-            self._minimum_sdk_version in sdk_versions
+                self._minimum_sdk_version is not None and
+                self._minimum_sdk_version in sdk_versions
         ):
             index = sdk_versions.index(self._minimum_sdk_version)
             sdk_versions = sdk_versions[:index + 1]
 
         return sdk_versions
 
     @property
     def version(self) -> str:
         """
         This is used in the solution file to tell the compiler what SDK to use.
         We obtain a list of compatible Windows SDK versions for the
         Visual C version. We check and see if any  of the compatible SDK's are
         installed and if so we return that version.
 
+        :rtype: str
         :return: Installed Windows SDK version
         """
 
         if self._version is None:
             sdk_versions = _read_reg_keys('Microsoft SDKs\\Windows', True)
             if self._strict_sdk_version is not None:
                 if self._strict_sdk_version.startswith('10.0'):
@@ -2636,14 +2719,15 @@
 
     @property
     def sdk_version(self) -> str:
         """
         This is almost identical to target_platform. Except it returns the
         actual version of the Windows SDK not the truncated version.
 
+        :rtype: str
         :return: actual Windows SDK version
         """
 
         if self._sdk_version is None:
             version = self.version
 
             if self._strict_sdk_version is None:
@@ -2693,15 +2777,17 @@
 
         return self._sdk_version
 
     @property
     def directory(self) -> Optional[str]:
         """
         Path to the Windows SDK version that has been found.
-        :return: Windows SDK path
+
+        :rtype: Optional, str
+        :return: Windows SDK path or `None`
         """
 
         if self._directory is None:
             version = self.version
 
             if self._strict_sdk_version is None:
                 self._directory = _get_reg_value(
@@ -2746,15 +2832,14 @@
                     )
 
                     return self._directory
 
         return self._directory
 
     def __iter__(self):
-
         ver_bin_path = self.ver_bin_path
         directory = self.directory
 
         if ver_bin_path:
             ver_bin_path += '\\'
 
         if directory and not directory.endswith('\\'):
@@ -2768,15 +2853,15 @@
         if not sdk_version.endswith('\\'):
             sdk_version += '\\'
 
         env = dict(
             LIB=self.lib,
             Path=self.path,
             LIBPATH=self.lib_path,
-            Include=self.include,
+            INCLUDE=self.include,
             UniversalCRTSdkDir=self.ucrt_sdk_directory,
             ExtensionSdkDir=self.extension_sdk_directory,
             WindowsSdkVerBinPath=ver_bin_path,
             UCRTVersion=self.ucrt_version,
             WindowsSDKLibVersion=lib_version,
             WindowsSDKVersion=sdk_version,
             WindowsSdkDir=directory,
@@ -2824,20 +2909,20 @@
             type_script_path=self.type_script_path,
         )
 
 
 class NETInfo(object):
 
     def __init__(
-        self,
-        environ: Environment,
-        c_info: VisualCInfo,
-        sdk_version: str,
-        minimum_net_version: Optional[str] = None,
-        strict_net_version: Optional[str] = None
+            self,
+            environ: "Environment",
+            c_info: VisualCInfo,
+            sdk_version: str,
+            minimum_net_version: Optional[str] = None,
+            strict_net_version: Optional[str] = None
     ):
 
         self.environment = environ
         self.platform = environ.platform
         self.c_info = c_info
         self.vc_version = c_info.version
         self.sdk_version = sdk_version
@@ -2846,36 +2931,40 @@
         self._version_32 = None
         self._version_64 = None
 
     @property
     def version(self) -> str:
         """
         .NET Version
+
+        :rtype: str
         :return: returns the version associated with the architecture
         """
         if self.platform == 'x64':
             return self.version_64
         else:
             return self.version_32
 
     @property
     def version_32(self) -> str:
         """
         .NET 32bit framework version
+
+        :rtype: str
         :return: x86 .NET framework version
         """
         if self._version_32 is None:
             target_framework = None
             installation = self.c_info.cpp_installation
 
             if installation is not None:
                 for package in installation.packages.msi:
                     if (
-                        package.id.startswith('Microsoft.Net') and
-                        package.id.endswith('TargetingPack')
+                            package.id.startswith('Microsoft.Net') and
+                            package.id.endswith('TargetingPack')
                     ):
 
                         if self._strict_net_version is not None:
                             if self._strict_net_version == package:
                                 self._version_32 = 'v' + package.version
                                 return self._version_32
                             else:
@@ -2954,16 +3043,16 @@
                     raise RuntimeError(
                         'Unable to locate .NET version ' +
                         self._strict_net_version
                     )
 
                 for version in versions:
                     if (
-                        self._minimum_net_version is not None and
-                        version < self._minimum_net_version
+                            self._minimum_net_version is not None and
+                            version < self._minimum_net_version
                     ):
                         continue
 
                     if target_framework is None:
                         target_framework = version
                     elif target_framework < version:
                         target_framework = version
@@ -2989,26 +3078,28 @@
 
         return self._version_32
 
     @property
     def version_64(self) -> str:
         """
         .NET 64bit framework version
+
+        :rtype: str
         :return: x64 .NET framework version
         """
 
         if self._version_64 is None:
             target_framework = None
             installation = self.c_info.cpp_installation
 
             if installation is not None:
                 for package in installation.packages.msi:
                     if (
-                        package.id.startswith('Microsoft.Net') and
-                        package.id.endswith('TargetingPack')
+                            package.id.startswith('Microsoft.Net') and
+                            package.id.endswith('TargetingPack')
                     ):
 
                         if self._strict_net_version is not None:
                             if self._strict_net_version == package:
                                 self._version_64 = 'v' + package.version
                                 return self._version_64
                             else:
@@ -3089,16 +3180,16 @@
                     raise RuntimeError(
                         'Unable to locate .NET version ' +
                         self._strict_net_version
                     )
 
                 for version in versions:
                     if (
-                        self._minimum_net_version is not None and
-                        version < self._minimum_net_version
+                            self._minimum_net_version is not None and
+                            version < self._minimum_net_version
                     ):
                         continue
 
                     if target_framework is None:
                         target_framework = version
                     elif target_framework < version:
                         target_framework = version
@@ -3122,23 +3213,31 @@
 
             self._version_64 = ''
 
         return self._version_64
 
     @property
     def directory(self) -> str:
+        """
+        .NET directory
+
+        :rtype: str
+        :return: path to .NET
+        """
         if self.platform == 'x64':
             return self.directory_64
         else:
             return self.directory_32
 
     @property
     def directory_32(self) -> str:
         """
         .NET 32bit path
+
+        :rtype: str
         :return: path to x86 .NET
         """
         directory = _get_reg_value(
             'VisualStudio\\SxS\\VC7\\',
             'FrameworkDir32'
         )
         if not directory:
@@ -3156,14 +3255,16 @@
 
         return ''
 
     @property
     def directory_64(self) -> str:
         """
         .NET 64bit path
+
+        :rtype: str
         :return: path to x64 .NET
         """
 
         directory = _get_reg_value(
             'VisualStudio\\SxS\\VC7\\',
             'FrameworkDir64'
         )
@@ -3180,88 +3281,99 @@
         if os.path.exists(directory):
             return directory
 
         return ''
 
     @property
     def preferred_bitness(self) -> str:
+        """
+        .NET bitness
+
+        :rtype: str
+        :return:  either `"32"` or `"64"`
+        """
         return '32' if self.platform == 'x86' else '64'
 
     @property
-    def _net_fx_versions(self):
-        import fnmatch
+    def netfx_sdk_directory(self) -> Optional[str]:
+        """
+        Directory where NETFX is located.
+
+        :rtype: Optional, str
+        :return: path or `None`
+        """
+        framework = '.'.join(self.version[1:].split('.')[:2])
+        ver = float(int(self.vc_version.split('.')[0]))
+
+        if ver in (9.0, 10.0, 11.0, 12.0):
+            key = 'Microsoft SDKs\\Windows\\v{0}\\'.format(self.sdk_version)
+        else:
+            key = 'Microsoft SDKs\\NETFXSDK\\{0}\\'.format(framework)
 
+        net_fx_path = _get_reg_value(
+            key,
+            'KitsInstallationFolder',
+            wow6432=True
+        )
+
+        if net_fx_path and os.path.exists(net_fx_path):
+            return net_fx_path
+
+    @property
+    def net_fx_tools_directory(self) -> Optional[str]:
+        """
+        Directory where NETFX tools are located.
+
+        :rtype: Optional, str
+        :return: path or `None`
+        """
         framework = self.version[1:].split('.')[:2]
+
+        if framework[0] == '4':
+            net_framework = '40'
+        else:
+            net_framework = ''.join(framework)
+
         net_fx_key = (
             'WinSDK-NetFx{framework}Tools-{platform}'
         ).format(
-            framework=''.join(framework),
+            framework=''.join(net_framework),
             platform=self.platform
         )
+
+        framework = '.'.join(framework)
         ver = float(int(self.vc_version.split('.')[0]))
 
         if ver in (9.0, 10.0, 11.0, 12.0):
-            key = 'Microsoft SDKs\\Windows\\v{0}\\{1}'.format(
+            key = 'Microsoft SDKs\\Windows\\v{0}\\{1}\\'.format(
                 self.sdk_version,
                 net_fx_key
             )
 
             if self.sdk_version in ('6.0A', '6.1'):
                 key = key.replace(net_fx_key, 'WinSDKNetFxTools')
 
-            keys = (key,)
+            net_fx_path = _get_reg_value(
+                key,
+                'InstallationFolder',
+                wow6432=True
+            )
         else:
-            keys = (
-                'Microsoft SDKs\\NETFXSDK\\3.5*\\' + net_fx_key,
-                'Microsoft SDKs\\NETFXSDK\\4.0*\\' + net_fx_key,
-                'Microsoft SDKs\\NETFXSDK\\4.5*\\' + net_fx_key,
-                'Microsoft SDKs\\NETFXSDK\\4.6*\\' + net_fx_key,
-                'Microsoft SDKs\\NETFXSDK\\4.7*\\' + net_fx_key,
-                'Microsoft SDKs\\NETFXSDK\\4.8*\\' + net_fx_key,
-                'Microsoft SDKs\\NETFXSDK\\4.6*\\' + net_fx_key,
-                'Microsoft SDKs\\Windows\\v8.1\\' + net_fx_key,
-                'Microsoft SDKs\\Windows\\v10.0\\' + net_fx_key,
-            )
-
-        for key in keys:
-            if '*' in key:
-                for fx_ver in _read_reg_keys('Microsoft SDKs\\NETFXSDK'):
-                    fx_ver = 'Microsoft SDKs\\NETFXSDK\\{0}\\{1}'.format(
-                        fx_ver,
-                        net_fx_key
-                    )
-
-                    if fnmatch.fnmatch(fx_ver, key):
-                        yield fx_ver
-            else:
-                val = _get_reg_value(
-                    key + '\\',
-                    'InstallationFolder'
-                )
-                if val:
-                    yield val
-
-    @property
-    def netfx_sdk_directory(self) -> Optional[str]:
-        for key in self._net_fx_versions:
+            key = 'Microsoft SDKs\\NETFXSDK\\{0}\\{1}\\'.format(
+                framework,
+                net_fx_key
+            )
             net_fx_path = _get_reg_value(
-                key.rsplit('\\', 1)[0],
-                'KitsInstallationFolder'
+                key,
+                'InstallationFolder',
+                wow6432=True
             )
 
-            if net_fx_path and os.path.exists(net_fx_path):
-                return net_fx_path
-
-    @property
-    def net_fx_tools_directory(self) -> Optional[str]:
-        for key in self._net_fx_versions:
-            net_fx_path = _get_reg_value(key, 'InstallationFolder')
-
-            if net_fx_path and os.path.exists(net_fx_path):
-                return net_fx_path
+        if net_fx_path and os.path.exists(net_fx_path):
+            return net_fx_path
 
     @property
     def add(self) -> str:
         return '__DOTNET_ADD_{0}BIT'.format(self.preferred_bitness)
 
     @property
     def net_tools(self) -> list:
@@ -3305,15 +3417,16 @@
         tools_directory = self.net_fx_tools_directory
         if not tools_directory:
             return
 
         if 'NETFX' in tools_directory:
             if 'x64' in tools_directory:
                 return (
-                    os.path.split(os.path.split(tools_directory)[0])[0] + '\\'
+                        os.path.split(os.path.split(tools_directory)[0])[
+                            0] + '\\'
                 )
             else:
                 return tools_directory
         return None
 
     @property
     def lib(self) -> list:
@@ -3409,63 +3522,111 @@
                 )
                 path += [pth]
 
         return path
 
     @property
     def include(self) -> list:
-        net_fx_tools = self.net_fx_tools_directory
+        sdk_directory = self.netfx_sdk_directory
 
-        if net_fx_tools:
-            net_fx_tools = os.path.join(
-                net_fx_tools,
-                'include',
-                'um'
-            )
-            if os.path.exists(net_fx_tools):
-                return [net_fx_tools]
+        if sdk_directory:
+            include_dir = os.path.join(sdk_directory, 'include', 'um')
+
+            if os.path.exists(include_dir):
+                return [include_dir]
 
         return []
 
     def __iter__(self):
         directory = self.directory
         if directory:
             directory += '\\'
 
         env = dict(
             WindowsSDK_ExecutablePath_x64=self.executable_path_x64,
             WindowsSDK_ExecutablePath_x86=self.executable_path_x86,
             LIB=self.lib,
             Path=self.path,
             LIBPATH=self.lib_path,
-            Include=self.include,
+            INCLUDE=self.include,
             __DOTNET_PREFERRED_BITNESS=self.preferred_bitness,
             FrameworkDir=directory,
-            FrameworkVersion=self.version,
             NETFXSDKDir=self.netfx_sdk_directory,
         )
 
+        version = self.version[1:].split('.')
+        if version[0] == '4':
+            version = ['4', '0']
+        else:
+            version = version[:2]
+
+        net_p = 'v' + ('.'.join(version))
+
         env[self.add] = '1'
         if self.platform == 'x64':
             directory_64 = self.directory_64
 
             if directory_64:
+                loc = os.path.join(directory_64, net_p)
+
+                if os.path.exists(loc):
+                    version_64 = loc
+                else:
+                    for p in os.listdir(directory_64):
+                        if not os.path.isdir(os.path.join(directory_64, p)):
+                            continue
+
+                        if p[1:] < net_p[1:]:
+                            continue
+
+                        version_64 = p
+                        break
+                    else:
+                        version_64 = self.version_64
+
                 directory_64 += '\\'
+            else:
+                version_64 = None
 
             env['FrameworkDir64'] = directory_64
-            env['FrameworkVersion64'] = self.version_64
+            env['FrameworkVersion64'] = version_64
+            env['FrameworkVersion'] = version_64
+
         else:
             directory_32 = self.directory_32
+
             if directory_32:
+                loc = os.path.join(directory_32, net_p)
+
+                if not os.path.exists(loc):
+                    for p in os.listdir(directory_32):
+                        if not os.path.isdir(os.path.join(directory_32, p)):
+                            continue
+
+                        if p[1:] < net_p[1:]:
+                            continue
+
+                        version_32 = p
+                        break
+                    else:
+                        version_32 = self.version_64
+
+                else:
+                    version_32 = loc
+
                 directory_32 += '\\'
+            else:
+                version_32 = None
 
             env['FrameworkDir32'] = directory_32
-            env['FrameworkVersion32'] = self.version_32
+            env['FrameworkVersion32'] = version_32
+            env['FrameworkVersion'] = version_32
 
         framework = env['FrameworkVersion'][1:].split('.')[:2]
+
         framework_version_key = (
             'Framework{framework}Version'.format(framework=''.join(framework))
         )
         env[framework_version_key] = 'v' + '.'.join(framework)
 
         for key, value in env.items():
             if value is not None and value:
@@ -3497,28 +3658,229 @@
             framework_dir_64=self.directory_64,
             net_fx_tools_directory=self.net_fx_tools_directory,
             executable_path_x64=self.executable_path_x64,
             executable_path_x86=self.executable_path_x86,
         )
 
 
+class Environment(object):
+    _original_environment = {k_: v_ for k_, v_ in os.environ.items()}
+
+    def __init__(
+            self,
+            minimum_c_version: Optional[Union[int, float]] = None,
+            strict_c_version: Optional[Union[int, float]] = None,
+            minimum_toolkit_version: Optional[int] = None,
+            strict_toolkit_version: Optional[int] = None,
+            minimum_sdk_version: Optional[str] = None,
+            strict_sdk_version: Optional[str] = None,
+            minimum_net_version: Optional[str] = None,
+            strict_net_version: Optional[str] = None,
+            vs_version: Optional[Union[str, int]] = None
+    ):
+        self.python = PythonInfo()
+
+        self.visual_c = VisualCInfo(
+            self,
+            minimum_c_version,
+            strict_c_version,
+            minimum_toolkit_version,
+            strict_toolkit_version,
+            vs_version
+        )
+
+        self.visual_studio = VisualStudioInfo(
+            self,
+            self.visual_c
+        )
+
+        self.windows_sdk = WindowsSDKInfo(
+            self,
+            self.visual_c,
+            minimum_sdk_version,
+            strict_sdk_version
+        )
+
+        self.dot_net = NETInfo(
+            self,
+            self.visual_c,
+            self.windows_sdk.version,
+            minimum_net_version,
+            strict_net_version
+        )
+
+    def reset_environment(self):
+        for key in list(os.environ.keys())[:]:
+            if key not in self._original_environment:
+                del os.environ[key]
+
+        os.environ.update(self._original_environment)
+
+    @property
+    def machine_architecture(self):
+        import platform
+        return 'x64' if '64' in platform.machine() else 'x86'
+
+    @property
+    def platform(self):
+        """
+        :return: x86 or x64
+        """
+        import platform
+
+        win_64 = self.machine_architecture == 'x64'
+        python_64 = platform.architecture()[0] == '64bit' and win_64
+
+        return 'x64' if python_64 else 'x86'
+
+    @property
+    def configuration(self) -> str:
+        """
+        Build configuration
+
+        :rtype: str
+        :return: `"ReleaseDLL"` or `"DebugDLL"`
+        """
+
+        if os.path.splitext(sys.executable)[0].endswith('_d'):
+            config = 'Debug'
+        else:
+            config = 'Release'
+
+        return config
+
+    def __iter__(self):
+        for item in self.build_environment.items():
+            yield item
+
+    @property
+    def build_environment(self):
+        """
+        This would be the work horse. This is where all of the gathered
+        information is put into a single container and returned.
+        The information is then added to os.environ in order to allow the
+        build process to run properly.
+
+        List of environment variables generated:
+        PATH
+        LIBPATH
+        LIB
+        INCLUDE
+        Platform
+        FrameworkDir
+        FrameworkVersion
+        FrameworkDIR32
+        FrameworkVersion32
+        FrameworkDIR64
+        FrameworkVersion64
+        VCToolsRedistDir
+        VCINSTALLDIR
+        VCToolsInstallDir
+        VCToolsVersion
+        WindowsLibPath
+        WindowsSdkDir
+        WindowsSDKVersion
+        WindowsSdkBinPath
+        WindowsSdkVerBinPath
+        WindowsSDKLibVersion
+        __DOTNET_ADD_32BIT
+        __DOTNET_ADD_64BIT
+        __DOTNET_PREFERRED_BITNESS
+        Framework{framework version}Version
+        NETFXSDKDir
+        UniversalCRTSdkDir
+        UCRTVersion
+        ExtensionSdkDir
+
+        These last 2 are set to ensure that distuils uses these environment
+        variables when compiling libopenzwave.pyd
+        MSSDK
+        DISTUTILS_USE_SDK
+
+        :return: dict of environment variables
+        """
+        path = os.environ.get('Path', '')
+
+        env = dict(
+            __VSCMD_PREINIT_PATH=path,
+            Platform=self.platform,
+            VSCMD_ARG_app_plat='Desktop',
+            VSCMD_ARG_HOST_ARCH=self.platform,
+            VSCMD_ARG_TGT_ARCH=self.platform,
+            __VSCMD_script_err_count='0'
+        )
+
+        env_path = set()
+
+        def update_env(cls):
+            for key, value in cls:
+                if key == 'Path':
+                    for item in value.split(os.pathsep):
+                        env_path.add(item)
+                    continue
+
+                if key in env:
+                    env[key] += os.pathsep + value
+                else:
+                    env[key] = value
+
+        update_env(self.visual_c)
+        update_env(self.visual_studio)
+        update_env(self.windows_sdk)
+        update_env(self.dot_net)
+
+        env_path = os.pathsep.join(item for item in env_path)
+        env['Path'] = env_path
+
+        return env
+
+    def __str__(self):
+        template = (
+            'Machine architecture: {machine_architecture}\n'
+            'Build architecture: {architecture}\n'
+        )
+
+        res = [
+            template.format(
+                machine_architecture=self.machine_architecture,
+                architecture=self.platform
+            ),
+            str(self.python),
+            str(self.visual_studio),
+            str(self.visual_c),
+            str(self.windows_sdk),
+            str(self.dot_net),
+        ]
+
+        return '\n'.join(res)
+
+
 def setup_environment(
-    minimum_c_version: Optional[Union[int, float]] = None,
-    strict_c_version: Optional[Union[int, float]] = None,
-    minimum_toolkit_version: Optional[int] = None,
-    strict_toolkit_version: Optional[int] = None,
-    minimum_sdk_version: Optional[str] = None,
-    strict_sdk_version: Optional[str] = None,
-    minimum_net_version: Optional[str] = None,
-    strict_net_version: Optional[str] = None,
-    vs_version: Optional[Union[str, int]] = None
+        minimum_c_version: Optional[Union[int, float]] = None,
+        strict_c_version: Optional[Union[int, float]] = None,
+        minimum_toolkit_version: Optional[int] = None,
+        strict_toolkit_version: Optional[int] = None,
+        minimum_sdk_version: Optional[str] = None,
+        strict_sdk_version: Optional[str] = None,
+        minimum_net_version: Optional[str] = None,
+        strict_net_version: Optional[str] = None,
+        vs_version: Optional[Union[str, int]] = None
 ):
     """
     Main entry point.
 
+    There was some forwward thinking done when distutils was written. We are
+    able to set up a build environment without ever having to monkey patch any
+    part of distutils. There is an environment variable that I can set that will
+    tell distutils to use the existing environment for the build. This is
+    how I am able to set up a build environent and then let distutils do what
+    it does. The only portion of distutils that does not seem to function
+    properly 100% of the time is the MSVC detection. That is what gets fixed
+    with this library.
+
     :param minimum_c_version: The lowest MSVC compiler version to allow.
     :type minimum_c_version: optional - int, float
 
     :param strict_c_version: The MSVC compiler version that MUST be used.
       ie 14.0, 14.2
     :type strict_c_version: optional - int or float
 
@@ -3558,26 +3920,31 @@
       a specific installation  in this case then use the version or
       display version options.
     :type vs_version: optional - str, int
 
     :return: Environment instance
     :rtype: Environment
     """
+
     if not _IS_WIN:
         raise RuntimeError(
             'This script will only work with a Windows opperating system.'
         )
 
-    distutils.log.debug(
+    logger.debug(
         'Setting up Windows build environment, please wait.....'
     )
 
     python_version = sys.version_info[:2]
     if minimum_c_version is None:
-        if python_version == (3, 10):
+        if python_version == (3, 12):
+            minimum_c_version = 14.3
+        elif python_version == (3, 11):
+            minimum_c_version = 14.3
+        elif python_version == (3, 10):
             minimum_c_version = 14.2
         elif python_version == (3, 9):
             minimum_c_version = 14.2
         elif python_version == (3, 8):
             minimum_c_version = 14.0
         elif python_version == (3, 7):
             minimum_c_version = 14.0
@@ -3585,50 +3952,57 @@
             minimum_c_version = 14.0
         elif python_version == (3, 5):
             minimum_c_version = 12.0
         elif python_version == (3, 4):
             minimum_c_version = 12.0
         else:
             raise RuntimeError(
-                'ozw does not support this version of python'
+                'Python version not supported'
             )
 
     environment = Environment(
         minimum_c_version,
         strict_c_version,
         minimum_toolkit_version,
         strict_toolkit_version,
         minimum_sdk_version,
         strict_sdk_version,
         minimum_net_version,
         strict_net_version,
         vs_version
     )
 
-    distutils.log.debug('\n' + str(environment))
+    logger.debug('\n' + str(environment) + '\n\n')
+    logger.debug('SET ENVIRONMENT VARIABLES')
+    logger.debug('------------------------------------------------')
+    logger.debug('\n')
 
     for key, value in environment.build_environment.items():
+        old_val = os.environ.get(key, value)
+        if old_val != value:
+            if os.pathsep in old_val or os.pathsep in value:
+                value = [item for item in set(value.split(os.pathsep))]
+                old_val = [
+                    item for item in set(old_val.split(os.pathsep))
+                    if item not in value
+                ]
+
+                value.extend(old_val)
+                value = os.pathsep.join(
+                    item.strip() for item in value if item.strip()
+                )
+
+        logger.debug(key + '=' + value)
         os.environ[key] = value
 
+    logger.debug('\n\n')
+
     return environment
 
 
 if __name__ == '__main__':
-    distutils.log.set_threshold(distutils.log.DEBUG)
+    _setup_logging()
 
     # build tools   2019 '16.10.31515.178'  '16.10.4'
     # visual studio 2019 '16.11.31729.503'  '16.11.5'
 
     envr = setup_environment()  # vs_version='16.10.4')
-    print()
-    print()
-    print('SET ENVIRONMENT VARIABLES')
-    print('------------------------------------------------')
-    print()
-    for k, v in envr:
-        if os.pathsep in v:
-            v = v.split(';')
-            if not v[-1]:
-                v = v[:-1]
-
-        print(k + ':', v)
-        print()
```

### Comparing `pyMSVC-0.4.0/pyMSVC/vswhere.py` & `pyMSVC-0.5.1/pyMSVC/vswhere.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 # #############################################################################
 
 try:
     import comtypes
 except ImportError:
     raise RuntimeError('the comtypes library is needed to run this script')
 
-import os
 import weakref
 import ctypes
+import datetime
 from ctypes.wintypes import (
-    LPFILETIME,
+    WORD,
+    DWORD,
+    BOOL,
     LPCOLESTR,
     ULONG,
     LPCWSTR,
     LPVOID,
     LCID
 )
 
@@ -51,16 +53,16 @@
     POINTER,
     IUnknown,
     HRESULT
 )
 from comtypes._safearray import (  # NOQA
     SAFEARRAY,
     VARIANT_BOOL,
-    SafeArrayLock,
-    SafeArrayUnlock
+    SafeArrayLock as _SafeArrayLock,
+    SafeArrayUnlock as _SafeArrayUnlock
 )
 
 LPVARIANT = POINTER(tagVARIANT)
 VARIANT = tagVARIANT
 ENUM = ctypes.c_uint
 IID = GUID
 CLSID = GUID
@@ -82,14 +84,94 @@
 ERROR_FILE_NOT_FOUND = 0x00000002
 ERROR_NOT_FOUND = 0x00000490
 
 # Constants
 E_NOTFOUND = HRESULT_FROM_WIN32(ERROR_NOT_FOUND)
 E_FILENOTFOUND = HRESULT_FROM_WIN32(ERROR_FILE_NOT_FOUND)
 
+_kernel32 = ctypes.windll.kernel32
+
+_FileTimeToSystemTime = _kernel32.FileTimeToSystemTime
+_FileTimeToSystemTime.restype = BOOL
+
+_SystemTimeToFileTime = _kernel32.SystemTimeToFileTime
+_SystemTimeToFileTime.restype = BOOL
+
+
+class _FILETIME(ctypes.Structure):
+    _fields_ = [
+        ('dwLowDateTime', DWORD),
+        ('dwHighDateTime', DWORD)
+    ]
+
+    @property
+    def value(self):
+        system_time = SYSTEMTIME()
+        _FileTimeToSystemTime(ctypes.byref(self), ctypes.byref(system_time))
+        return system_time.value
+
+    @value.setter
+    def value(self, dt):
+        system_time = SYSTEMTIME()
+        system_time.value = dt
+        _SystemTimeToFileTime(ctypes.byref(system_time), ctypes.byref(self))
+
+
+FILETIME = _FILETIME
+LPFILETIME = POINTER(FILETIME)
+
+
+class _SYSTEMTIME(ctypes.Structure):
+    _fields_ = [
+        ('wYear', WORD),
+        ('wMonth', WORD),
+        ('wDayOfWeek', WORD),
+        ('wDay', WORD),
+        ('wHour', WORD),
+        ('wMinute', WORD),
+        ('wSecond', WORD),
+        ('wMilliseconds', WORD),
+    ]
+
+    @property
+    def value(self):
+        dt = datetime.datetime(
+            year=self.wYear,
+            month=self.wMonth,
+            day=self.wDay,
+            hour=self.wHour,
+            minute=self.wMinute,
+            second=self.wSecond,
+            microsecond=self.wMilliseconds * 1000
+        )
+
+        return dt
+
+    # noinspection PyAttributeOutsideInit
+    @value.setter
+    def value(self, dt):
+        if isinstance(dt, (int, float)):
+            dt = datetime.datetime.fromtimestamp(dt)
+
+        weekday = dt.weekday() + 1
+        if weekday == 7:
+            weekday = 0
+
+        self.wYear = dt.year
+        self.wMonth = dt.month
+        self.wDayOfWeek = weekday
+        self.wDay = dt.day
+        self.wHour = dt.hour
+        self.wMinute = dt.minute
+        self.wSecond = dt.second
+        self.wMilliseconds = int(dt.microsecond / 1000)
+
+
+SYSTEMTIME = _SYSTEMTIME
+
 
 # Enumerations
 # The state of an instance.
 class InstanceState(ENUM):
     # The instance state has not been determined.
     eNone = 0
     # The instance installation path exists.
@@ -414,15 +496,15 @@
     def id(self):
         # noinspection PyUnresolvedReferences
         return self.GetInstanceId()
 
     @property
     def install_date(self):
         # noinspection PyUnresolvedReferences
-        return self.GetInstallDate()
+        return self.GetInstallDate().value
 
     @property
     def name(self):
         # noinspection PyUnresolvedReferences
         return self.GetInstallationName()
 
     @property
@@ -453,23 +535,28 @@
         try:
             # noinspection PyUnresolvedReferences
             return self.GetDescription(_GetUserDefaultLCID())
         except (OSError, ValueError, comtypes.COMError):
             pass
 
     def __str__(self):
+        title_bar = '-- ' + str(self.display_name) + ' '
+        title_bar += '-' * (63 - len(title_bar))
         res = [
+            title_bar,
+            'description: ' + str(self.description),
+            'version: ' + str(self.version),
             'id: ' + str(self.id),
             'name: ' + str(self.name),
             'display name: ' + str(self.display_name),
             'description: ' + str(self.description),
             'path: ' + str(self.path),
             'version: ' + str(self.version),
             'full version: ' + str(self.full_version),
-            'install date: ' + str(self.install_date)
+            'install date: ' + self.install_date.strftime('%c')
         ]
         return '\n'.join(res)
 
 
 IID_ISetupInstance2 = IID("{89143C9A-05AF-49B0-B717-72E218A2185C}")
 
 
@@ -478,55 +565,62 @@
     _iid_ = IID_ISetupInstance2
 
     @property
     def packages(self) -> Packages:
         # noinspection PyUnresolvedReferences
         safearray = self.GetPackages()
 
-        SafeArrayLock(safearray)
+        _SafeArrayLock(safearray)
 
         # noinspection PyTypeChecker
         packs = ctypes.cast(
             safearray.contents.pvData,
             POINTER(POINTER(ISetupPackageReference))
         )
 
         cPackages = safearray.contents.rgsabound[0].cElements
 
         res = []
         for i in range(cPackages):
             p = packs[i]
             res.append(p)
 
-        SafeArrayUnlock(safearray)
+        _SafeArrayUnlock(safearray)
         res = Packages(res)
         return res
 
     @property
     def properties(self):
         # noinspection PyUnresolvedReferences
         return self.GetProperties()
 
     @property
     def product(self):
+        """
+        version
+        chip
+        language
+        branch
+        type
+        unique_id
+        is_extension
+        """
         if 'registered' in self.state:
             # noinspection PyUnresolvedReferences
             return self.GetProduct()
 
     @property
     def state(self):
         # noinspection PyUnresolvedReferences
         return self.GetState().value
 
     @property
     def product_path(self):
-        path = self.path
         # noinspection PyUnresolvedReferences
-        product_path = self.GetProductPath()
-        return os.path.join(path, product_path)
+        return self.GetProductPath()
 
     @property
     def errors(self):
         # noinspection PyUnresolvedReferences
         errors = self.GetErrors()
         try:
             return errors.QueryInterface(ISetupErrorState2)
@@ -542,15 +636,15 @@
     def is_complete(self):
         # noinspection PyUnresolvedReferences
         return self.IsComplete()
 
     @property
     def is_prerelease(self):
         catalog = self.QueryInterface(ISetupInstanceCatalog)
-        return catalog.IsPrerelease()
+        return catalog.IsPrerelease()  # NOQA
 
     @property
     def catalog(self):
         return self.QueryInterface(ISetupInstanceCatalog)
 
     @property
     def engine_path(self):
@@ -575,15 +669,16 @@
             'product: ',
             '{product}',
             'packages:',
             '{packages}',
             'properties:',
             '{properties}',
             'catalog:',
-            '{catalog}'
+            '{catalog}',
+            '-' * 63
         ]
 
         res = '\n'.join(res)
 
         return res.format(
             errors='\n'.join(
                 '    ' + line
@@ -747,28 +842,35 @@
 # Gets information about product instances set up on the machine.
 class ISetupConfiguration(IUnknown):
     _iid_ = IID_ISetupConfiguration
 
     def __call__(self):
         try:
             return self.QueryInterface(ISetupConfiguration2)
-        except ValueError:
+        except (ValueError, OSError, comtypes.COMError):
             return self
 
     def __iter__(self):
         # noinspection PyUnresolvedReferences
         setup_enum = self.EnumInstances()
         helper = self.QueryInterface(ISetupHelper)
 
         for si in setup_enum:
             if not si:
                 break
 
             yield si(helper)
 
+    def __str__(self):
+        res = []
+        for instance_config in self:
+            res += [str(instance_config)]
+
+        return '\n\n\n'.join(res)
+
 
 IID_ISetupConfiguration2 = IID("{26AAB78C-4A60-49D6-AF3B-3C35BC93365D}")
 
 
 # Gets information about product instances.
 class ISetupConfiguration2(ISetupConfiguration):
     _iid_ = IID_ISetupConfiguration2
@@ -803,15 +905,15 @@
     def failed_packages(self) -> Packages:
         try:
             # noinspection PyUnresolvedReferences
             safearray = self.GetFailedPackages()
         except ValueError:
             return Packages([])
 
-        SafeArrayLock(safearray)
+        _SafeArrayLock(safearray)
 
         # noinspection PyTypeChecker
         packs = ctypes.cast(
             safearray.contents.pvData,
             POINTER(POINTER(ISetupFailedPackageReference))
         )
 
@@ -819,27 +921,27 @@
 
         res = []
         for i in range(cPackages):
             p = packs[i]
             p = p.QueryInterface(ISetupFailedPackageReference2)
             res.append(p)
 
-        SafeArrayUnlock(safearray)
+        _SafeArrayUnlock(safearray)
         res = Packages(res)
         return res
 
     @property
     def skipped_packages(self) -> Packages:
         try:
             # noinspection PyUnresolvedReferences
             safearray = self.GetSkippedPackages()
         except ValueError:
             return Packages([])
 
-        SafeArrayLock(safearray)
+        _SafeArrayLock(safearray)
 
         # noinspection PyTypeChecker
         packs = ctypes.cast(
             safearray.contents.pvData,
             POINTER(POINTER(ISetupFailedPackageReference))
         )
 
@@ -847,15 +949,15 @@
 
         res = []
         for i in range(cPackages):
             p = packs[i]
             p = p.QueryInterface(ISetupFailedPackageReference2)
             res.append(p)
 
-        SafeArrayUnlock(safearray)
+        _SafeArrayUnlock(safearray)
         res = Packages(res)
         return res
 
     def __str__(self):
         res = ['failed packages: ']
         res.extend([
             '    ' + line for line in
@@ -893,27 +995,27 @@
             'error log file path: ' + self.error_log_file_path,
             'log file path: ' + self.log_file_path,
             ISetupErrorState.__str__(self)
         ]
         return '\n'.join(res)
 
 
-IID_ISetupFailedPackageReference = (
-    IID("{E73559CD-7003-4022-B134-27DC650B280F}")
-)
+IID_ISetupFailedPackageReference = IID(
+    "{E73559CD-7003-4022-B134-27DC650B280F}"
+    )
 
 
 # A reference to a failed package.
 class ISetupFailedPackageReference(ISetupPackageReference):
     _iid_ = IID_ISetupFailedPackageReference
 
 
-IID_ISetupFailedPackageReference2 = (
-    IID("{0FAD873E-E874-42E3-B268-4FE2F096B9CA}")
-)
+IID_ISetupFailedPackageReference2 = IID(
+    "{0FAD873E-E874-42E3-B268-4FE2F096B9CA}"
+    )
 
 
 # A reference to a failed package.
 class ISetupFailedPackageReference2(ISetupFailedPackageReference):
     _iid_ = IID_ISetupFailedPackageReference2
 
 
@@ -943,74 +1045,77 @@
     _iid_ = IID_ISetupPropertyStore
 
     @property
     def names(self):
         # noinspection PyUnresolvedReferences
         safearray = self.GetNames()
 
-        SafeArrayLock(safearray)
+        _SafeArrayLock(safearray)
 
         names = ctypes.cast(safearray.contents.pvData, POINTER(BSTR))
         cPackages = safearray.contents.rgsabound[0].cElements
 
         res = []
         for i in range(cPackages):
             res.append(names[i])
 
-        SafeArrayUnlock(safearray)
+        _SafeArrayUnlock(safearray)
 
         return res
 
     def __iter__(self):
         for n in self.names:
-            v = VARIANT()
             # noinspection PyUnresolvedReferences
-            self.GetValue(n, ctypes.byref(v))
+            v = VARIANT()
+
+            self.GetValue(n, ctypes.byref(v))  # NOQA
 
             v = v.value
             if isinstance(v, BSTR):
                 v = v.value
 
             yield Property(n, v)
 
     def __str__(self):
         return '\n'.join(str(prop) for prop in self)
 
 
-IID_ISetupLocalizedPropertyStore = (
-    IID("{5BB53126-E0D5-43DF-80F1-6B161E5C6F6C}")
-)
+IID_ISetupLocalizedPropertyStore = IID(
+    "{5BB53126-E0D5-43DF-80F1-6B161E5C6F6C}"
+    )
+
 
 # Provides localized named properties.
 class ISetupLocalizedPropertyStore(IUnknown):
     _iid_ = IID_ISetupLocalizedPropertyStore
 
     @property
     def names(self):
         # noinspection PyUnresolvedReferences
         safearray = self.GetNames()
 
-        SafeArrayLock(safearray)
+        _SafeArrayLock(safearray)
 
         names = ctypes.cast(safearray.contents.pvData, POINTER(BSTR))
         cPackages = safearray.contents.rgsabound[0].cElements
 
         res = []
         for i in range(cPackages):
             res.append(names[i])
 
-        SafeArrayUnlock(safearray)
+        _SafeArrayUnlock(safearray)
 
         return res
 
     def __iter__(self):
         for n in self.names:
-            v = VARIANT()
             # noinspection PyUnresolvedReferences
-            self.GetValue(n, ctypes.byref(v))
+            v = VARIANT()
+
+            self.GetValue(n, ctypes.byref(v))  # NOQA
 
             v = v.value
             if isinstance(v, BSTR):
                 v = v.value
 
             yield Property(n.value, v)
 
@@ -1515,9 +1620,8 @@
             instance = cls._instance_()
 
         return instance
 
 
 if __name__ == '__main__':
     setup_config = SetupConfiguration.GetSetupConfiguration()
-    for instance_config in setup_config:
-        print(instance_config)
+    print(setup_config)
```

### Comparing `pyMSVC-0.4.0/setup.py` & `pyMSVC-0.5.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 
 from setuptools import setup
 
 
 setup(
     name='pyMSVC',
-    version='0.4.0',
+    version='0.5.1',
     url='https://github.com/kdschlosser/python_msvc',
     packages=['pyMSVC'],
     author='Kevin Schlosser',
     description='Simple to use MSVC build environment setup tool.',
     long_description=(
         'Distutils and setup tools not working properly to compile on Windows?\n'
         'Tired of having a new visual studio version break your setup program?\n'
-        'This  library is the solution.'
+        'This library is the solution.'
     ),
     install_requires=[
         'comtypes==1.1.11',
     ],
-    dependency_links=[
-        'https://github.com/kdschlosser/comtypes/tarball/bstr_type#egg=comtypes-1.1.10',
-    ],
     license='MIT',
 )
```

