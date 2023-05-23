# Comparing `tmp/geosyspy-0.1.2.tar.gz` & `tmp/geosyspy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosyspy-0.1.2.tar", last modified: Tue Apr 26 14:19:58 2022, max compression
+gzip compressed data, was "geosyspy-0.1.3.tar", last modified: Tue May 23 16:19:16 2023, max compression
```

## Comparing `geosyspy-0.1.2.tar` & `geosyspy-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:19:58.779505 geosyspy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11833 2022-04-26 14:19:58.779505 geosyspy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9462 2022-04-26 14:18:01.000000 geosyspy-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-26 14:18:01.000000 geosyspy-0.1.2/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:19:58.779505 geosyspy-0.1.2/geosyspy/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-26 14:18:01.000000 geosyspy-0.1.2/geosyspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-04-26 14:18:01.000000 geosyspy-0.1.2/geosyspy/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    33704 2022-04-26 14:18:01.000000 geosyspy-0.1.2/geosyspy/geosys.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-04-26 14:18:01.000000 geosyspy-0.1.2/geosyspy/image_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-04-26 14:18:01.000000 geosyspy-0.1.2/geosyspy/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:19:58.779505 geosyspy-0.1.2/geosyspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11833 2022-04-26 14:19:58.000000 geosyspy-0.1.2/geosyspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-04-26 14:19:58.000000 geosyspy-0.1.2/geosyspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 14:19:58.000000 geosyspy-0.1.2/geosyspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-26 14:19:58.000000 geosyspy-0.1.2/geosyspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-26 14:19:58.000000 geosyspy-0.1.2/geosyspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-26 14:19:58.783506 geosyspy-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-04-26 14:18:01.000000 geosyspy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:19:16.508660 geosyspy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-23 16:19:16.508660 geosyspy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-23 16:17:31.000000 geosyspy-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 16:17:31.000000 geosyspy-0.1.3/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:19:16.508660 geosyspy-0.1.3/geosyspy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 16:17:31.000000 geosyspy-0.1.3/geosyspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-05-23 16:17:31.000000 geosyspy-0.1.3/geosyspy/geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 16:17:31.000000 geosyspy-0.1.3/geosyspy/image_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:19:16.508660 geosyspy-0.1.3/geosyspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 16:19:16.508660 geosyspy-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-23 16:17:31.000000 geosyspy-0.1.3/setup.py
```

### Comparing `geosyspy-0.1.2/README.md` & `geosyspy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: geosyspy
+Version: 0.1.3
+Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
+Author: Geosys
+Description-Content-Type: text/markdown
+
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
 *** See the bottom of this document for the declaration of the reference variables
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
 
@@ -32,15 +39,15 @@
 
 <div align="center">
   
 [![LinkedIn][linkedin-shield]][linkedin-url]
 [![Twitter][twitter-shield]][twitter-url]
 [![Youtube][youtube-shield]][youtube-url]
 [![languages][language-python-shiedl]][issues-url]
-[![CITest][CITest-shield]][CITest-url]
+<!-- [![CITest][CITest-shield]][CITest-url]-->
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
   
 </div>
 
 
 <!--[![Stargazers][GitStars-shield]][GitStars-url]-->
@@ -77,15 +84,17 @@
 EarthDaily Agro is the agricultural analysis division of EartDaily Analytics. Learn more about Earth Daily at [EarthDaily Analytics | Satellite imagery & data for agriculture, insurance, surveillance](https://earthdaily.com/).  EarthDaily Agro uses satellite imaging to provide advanced analytics to mitigate risk and increase efficiencies – leading to more sustainable outcomes for the organizations and people who feed the planet.
 <p align="center">
   <a href="https://earthdailyagro.com/geosys/">
     <img src="https://earthdailyagro.com/wp-content/uploads/2022/01/new-logo.png" alt="Logo" width="400">
   </a>
 </p>
 
-Throught our <geosys/> platform, we make geospatial analytics easily accessible for you to be browsed or analyzed, within our cloud or within your own environment. We provide developers and data scientists both flexibility and extensibility with analytic ready data and digital agriculture ready development blocks. We empower your team to enrich your systems with information at the field, regional or continent level via our API or Apps.
+ <p align="left">
+Throught our &ltgeosys/&gt platform, we make geospatial analytics easily accessible for you to be browsed or analyzed, within our cloud or within your own environment. We provide developers and data scientists both flexibility and extensibility with analytic ready data and digital agriculture ready development blocks. We empower your team to enrich your systems with information at the field, regional or continent level via our API or Apps.
+</p>
 
 We have a team of experts around the world that understand local crops and ag industry, as well as advanced analytics to support your business.
 
 We have established a developer community to provide you with plug-ins and integrations to be able to discover, request and use aggregate imagery products based on Landsat, Sentinel, Modis and many other open and commercial satellite sensors.
 
 The `geosyspy` python package aims to provide an easy and ready to use library allowing any Python developers to quickly experience Earthdaily Agro capabilities.
 
@@ -96,23 +105,23 @@
 * Data sourcing:
      * Get aggregated NDVI/EVI normalized times series from Modis satellite imagery as pandas dataframe
      * Get aggregated historical and forecast weather data (precipitation, temperatures...) location based time series as pandas dataframe
      * Get SENTINEL 2, LANDSAT 8 and LANSAT 9 satellite images time series in [xarray](https://docs.xarray.dev/en/stable/) format
 * Analytic publication:
      * Save and retrieve custom data in Analytics Fabrik
 
-See [Examples](examples.ipynb) notebook for more information
+See [documentation](https://geosys.github.io/GeosysPy/) and [Examples](examples.ipynb) notebook for more information
 
 ## Getting started
 
 ### Prerequisites
 
 Make sure you have valid credentials. If you need to get trial access, please register [here](https://earthdailyagro.com/geosys-api/#get-started).
 
-This package has been tested on Python 3.9.7.
+This package has been tested on Python 3.10.11.
 
 
 ### Installing
 
 #### For Linux / Mac OS
 ```
 pip install geosyspy
@@ -163,55 +172,55 @@
 or, without .env file :
 
 `docker run -it -e API_CLIENT_ID='...' -e API_CLIENT_SECRET='...' -e API_USERNAME='...' -e API_PASSWORD='...' geosyspy`
 
 Then :
 
 ```python
->>> from geosyspy.geosys import Geosys
->>> from geosyspy.constants import Collection, Region, Env
+>>> from geosyspy import Geosys
+>>> from geosyspy.utils.constants import *
 >>> import os
 >>> client = Geosys(os.getenv('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv('API_USERNAME'), os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA)
 
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Usage
 
 Initialize client:
 
 ```python
-from geosyspy.geosys import Geosys
-from geosyspy.constants import Collection, Region, Env
+from geosyspy import Geosys
+from geosyspy.utils.constants import *
 
 client = Geosys("API_CLIENT_ID", "API_CLIENT_SECRET", "API_USERNAME", "API_PASSWORD", Env.PREPROD, Region.NA)
 
 ```
 
 Query data:
 
 ```python
 polygon = "POLYGON((...))"
 
 today = dt.date.today()
 year_ago = dt.date.today() + relativedelta(months=-12)
 
-dataframe = client.get_time_series(polygon, year_ago, today, collection=Collection.MODIS, indicators=["NDVI"])
+dataframe = client.get_time_series(polygon, year_ago, today, collection=SatelliteImageryCollection.MODIS, indicators=["NDVI"])
 ```
 
 See the Jupyter notebook [Examples](examples.ipynb) for a working example.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- RESOURCES -->
 ## Resources 
 The following links will provide access to more information:
 - [EarthDaily agro developer portal  ](https://developer.geosys.com/)
-- 
+- [Pypi package](https://pypi.org/project/geosyspy/)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
 ## Support development
 
 If this project has been useful, that it helped you or your business to save precious time, don't hesitate to give it a star.
@@ -242,23 +251,23 @@
 <!-- List of available shields https://simpleicons.org/ -->
 [contributors-shield]: https://img.shields.io/github/contributors/github_username/repo.svg?style=social
 [contributors-url]: https://github.com/github_username/repo/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/github_username/repo.svg?style=plastic&logo=appveyor
 [forks-url]: https://github.com/github_username/repo/network/members
 [stars-shield]: https://img.shields.io/github/stars/qgis-plugin/repo.svg?style=plastic&logo=appveyor
 [stars-url]: https://github.com/github_username/repo/stargazers
-[issues-shield]: https://img.shields.io/github/issues/GEOSYS/qgis-plugin/repo.svg?style=social
+[issues-shield]: https://img.shields.io/github/issues/GEOSYS/GeosysPy/repo.svg?style=social
 [issues-url]: https://github.com/github_username/repo/issues
 [license-shield]: https://img.shields.io/github/license/GEOSYS/qgis-plugin
 [license-url]: https://www.gnu.org/licenses/gpl-3.0.en.html
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=social&logo=linkedin
 [linkedin-url]: https://www.linkedin.com/company/earthdailyagro/mycompany/
 [twitter-shield]: https://img.shields.io/twitter/follow/EarthDailyAgro?style=social
 [twitter-url]: https://img.shields.io/twitter/follow/EarthDailyAgro?style=social
 [youtube-shield]: https://img.shields.io/youtube/channel/views/UCy4X-hM2xRK3oyC_xYKSG_g?style=social
 [youtube-url]: https://img.shields.io/youtube/channel/views/UCy4X-hM2xRK3oyC_xYKSG_g?style=social
 [language-python-shiedl]: https://img.shields.io/badge/python-3.9-green?logo=python
 [language-python-url]: https://pypi.org/ 
 [GitStars-shield]: https://img.shields.io/github/stars/GEOSYS?style=social
 [GitStars-url]: https://img.shields.io/github/stars/GEOSYS?style=social
-[CITest-shield]: https://img.shields.io/github/workflow/status/GEOSYS/qgis-plugin/Continous%20Integration
-[CITest-url]: https://img.shields.io/github/workflow/status/GEOSYS/qgis-plugin/Continous%20Integration
+[CITest-shield]: https://img.shields.io/github/workflow/status/GEOSYS/GeosysPy/Continous%20Integration
+[CITest-url]: https://img.shields.io/github/workflow/status/GEOSYS/GeosysPy/Continous%20Integration
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_6971yam2_/tmpx9jdbjn6_TarContainer/0/2.md", line 18, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_6971yam2_/tmpx9jdbjn6_TarContainer/0/2.md", line 18, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,19 +1,22 @@
+Metadata-Version: 2.1 Name: geosyspy Version: 0.1.3 Summary: Easy-to-use python
+wrapper for Geosys APIs (time series, imagery products) Author: Geosys
+Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
                                   Who_we_are
 
              Project_description Â· Report_Bug Â· Request_Feature
    [![LinkedIn][linkedin-shield]][linkedin-url] [![Twitter][twitter-shield]]
 [twitter-url] [![Youtube][youtube-shield]][youtube-url] [![languages][language-
- python-shiedl]][issues-url] [![CITest][CITest-shield]][CITest-url] [![Issues]
-  [issues-shield]][issues-url] [![MIT License][license-shield]][license-url]
+  python-shiedl]][issues-url]  [![Issues][issues-shield]][issues-url] [![MIT
+                    License][license-shield]][license-url]
      Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Prerequisites
           o Installation
    3. Usage
    4. Support_development
@@ -24,65 +27,68 @@
   ## About The Project EarthDaily Agro is the agricultural analysis division of
 EartDaily Analytics. Learn more about Earth Daily at [EarthDaily Analytics |
 Satellite imagery & data for agriculture, insurance, surveillance](https://
 earthdaily.com/). EarthDaily Agro uses satellite imaging to provide advanced
 analytics to mitigate risk and increase efficiencies â leading to more
 sustainable outcomes for the organizations and people who feed the planet.
                                     [Logo]
-Throught our  platform, we make geospatial analytics easily accessible for you
-to be browsed or analyzed, within our cloud or within your own environment. We
-provide developers and data scientists both flexibility and extensibility with
-analytic ready data and digital agriculture ready development blocks. We
-empower your team to enrich your systems with information at the field,
-regional or continent level via our API or Apps. We have a team of experts
-around the world that understand local crops and ag industry, as well as
-advanced analytics to support your business. We have established a developer
-community to provide you with plug-ins and integrations to be able to discover,
-request and use aggregate imagery products based on Landsat, Sentinel, Modis
-and many other open and commercial satellite sensors. The `geosyspy` python
-package aims to provide an easy and ready to use library allowing any Python
-developers to quickly experience Earthdaily Agro capabilities.
+Throught our &ltgeosys/> platform, we make geospatial analytics easily
+accessible for you to be browsed or analyzed, within our cloud or within your
+own environment. We provide developers and data scientists both flexibility and
+extensibility with analytic ready data and digital agriculture ready
+development blocks. We empower your team to enrich your systems with
+information at the field, regional or continent level via our API or Apps.
+We have a team of experts around the world that understand local crops and ag
+industry, as well as advanced analytics to support your business. We have
+established a developer community to provide you with plug-ins and integrations
+to be able to discover, request and use aggregate imagery products based on
+Landsat, Sentinel, Modis and many other open and commercial satellite sensors.
+The `geosyspy` python package aims to provide an easy and ready to use library
+allowing any Python developers to quickly experience Earthdaily Agro
+capabilities.
                                                                   (back_to_top)
 ## Features * Data sourcing: * Get aggregated NDVI/EVI normalized times series
 from Modis satellite imagery as pandas dataframe * Get aggregated historical
 and forecast weather data (precipitation, temperatures...) location based time
 series as pandas dataframe * Get SENTINEL 2, LANDSAT 8 and LANSAT 9 satellite
 images time series in [xarray](https://docs.xarray.dev/en/stable/) format *
 Analytic publication: * Save and retrieve custom data in Analytics Fabrik See
-[Examples](examples.ipynb) notebook for more information ## Getting started ###
+[documentation](https://geosys.github.io/GeosysPy/) and [Examples]
+(examples.ipynb) notebook for more information ## Getting started ###
 Prerequisites Make sure you have valid credentials. If you need to get trial
 access, please register [here](https://earthdailyagro.com/geosys-api/#get-
-started). This package has been tested on Python 3.9.7. ### Installing #### For
-Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer to
-the [install.md](install.md) file. ### Run the package from source 1. Install
-dependencies ``` conda config --add channels conda-forge conda install --file
-requirements.txt ``` or ``` pip install -r requirements.txt ``` 2. Create .env
-file You need a .env file with your credentials to run the [Examples]
-(examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID= API_CLIENT_SECRET=
-API_USERNAME= API_PASSWORD= ``` 3. Run the Jupyter notebook ### Run the package
-inside a Docker container Build the image locally : `docker build --tag
-geosyspy .` Run it : `docker run -it --env-file .env geosyspy` or, without .env
-file : `docker run -it -e API_CLIENT_ID='...' -e API_CLIENT_SECRET='...' -
-e API_USERNAME='...' -e API_PASSWORD='...' geosyspy` Then : ```python >>> from
-geosyspy.geosys import Geosys >>> from geosyspy.constants import Collection,
-Region, Env >>> import os >>> client = Geosys(os.getenv('API_CLIENT_ID'),
-os.getenv('API_CLIENT_SECRET'), os.getenv('API_USERNAME'), os.getenv
-('API_PASSWORD'), Env.PREPROD, Region.NA) ```
-                                                                  (back_to_top)
-## Usage Initialize client: ```python from geosyspy.geosys import Geosys from
-geosyspy.constants import Collection, Region, Env client = Geosys
-("API_CLIENT_ID", "API_CLIENT_SECRET", "API_USERNAME", "API_PASSWORD",
-Env.PREPROD, Region.NA) ``` Query data: ```python polygon = "POLYGON((...))"
-today = dt.date.today() year_ago = dt.date.today() + relativedelta(months=-12)
-dataframe = client.get_time_series(polygon, year_ago, today,
-collection=Collection.MODIS, indicators=["NDVI"]) ``` See the Jupyter notebook
-[Examples](examples.ipynb) for a working example.
+started). This package has been tested on Python 3.10.11. ### Installing ####
+For Linux / Mac OS ``` pip install geosyspy ``` #### For Windows Please refer
+to the [install.md](install.md) file. ### Run the package from source 1.
+Install dependencies ``` conda config --add channels conda-forge conda install
+--file requirements.txt ``` or ``` pip install -r requirements.txt ``` 2.
+Create .env file You need a .env file with your credentials to run the
+[Examples](examples.ipynb) Jupyter notebook. ``` API_CLIENT_ID=
+API_CLIENT_SECRET= API_USERNAME= API_PASSWORD= ``` 3. Run the Jupyter notebook
+### Run the package inside a Docker container Build the image locally : `docker
+build --tag geosyspy .` Run it : `docker run -it --env-file .env geosyspy` or,
+without .env file : `docker run -it -e API_CLIENT_ID='...' -
+e API_CLIENT_SECRET='...' -e API_USERNAME='...' -e API_PASSWORD='...' geosyspy`
+Then : ```python >>> from geosyspy import Geosys >>> from
+geosyspy.utils.constants import * >>> import os >>> client = Geosys(os.getenv
+('API_CLIENT_ID'), os.getenv('API_CLIENT_SECRET'), os.getenv('API_USERNAME'),
+os.getenv('API_PASSWORD'), Env.PREPROD, Region.NA) ```
+                                                                  (back_to_top)
+## Usage Initialize client: ```python from geosyspy import Geosys from
+geosyspy.utils.constants import * client = Geosys("API_CLIENT_ID",
+"API_CLIENT_SECRET", "API_USERNAME", "API_PASSWORD", Env.PREPROD, Region.NA)
+``` Query data: ```python polygon = "POLYGON((...))" today = dt.date.today()
+year_ago = dt.date.today() + relativedelta(months=-12) dataframe =
+client.get_time_series(polygon, year_ago, today,
+collection=SatelliteImageryCollection.MODIS, indicators=["NDVI"]) ``` See the
+Jupyter notebook [Examples](examples.ipynb) for a working example.
                                                                   (back_to_top)
  ## Resources The following links will provide access to more information: -
-[EarthDaily agro developer portal ](https://developer.geosys.com/) -
+[EarthDaily agro developer portal ](https://developer.geosys.com/) - [Pypi
+package](https://pypi.org/project/geosyspy/)
                                                                   (back_to_top)
  ## Support development If this project has been useful, that it helped you or
 your business to save precious time, don't hesitate to give it a star.
                                                                   (back_to_top)
 ## License Distributed under the [GPL 3.0 License](https://www.gnu.org/
 licenses/gpl-3.0.en.html).
                                                                   (back_to_top)
@@ -96,25 +102,24 @@
 github_username/repo.svg?style=social [contributors-url]: https://github.com/
 github_username/repo/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/github_username/
 repo.svg?style=plastic&logo=appveyor [forks-url]: https://github.com/
 github_username/repo/network/members [stars-shield]: https://img.shields.io/
 github/stars/qgis-plugin/repo.svg?style=plastic&logo=appveyor [stars-url]:
 https://github.com/github_username/repo/stargazers [issues-shield]: https://
-img.shields.io/github/issues/GEOSYS/qgis-plugin/repo.svg?style=social [issues-
+img.shields.io/github/issues/GEOSYS/GeosysPy/repo.svg?style=social [issues-
 url]: https://github.com/github_username/repo/issues [license-shield]: https://
 img.shields.io/github/license/GEOSYS/qgis-plugin [license-url]: https://
 www.gnu.org/licenses/gpl-3.0.en.html [linkedin-shield]: https://img.shields.io/
 badge/-LinkedIn-black.svg?style=social&logo=linkedin [linkedin-url]: https://
 www.linkedin.com/company/earthdailyagro/mycompany/ [twitter-shield]: https://
 img.shields.io/twitter/follow/EarthDailyAgro?style=social [twitter-url]: https:
 //img.shields.io/twitter/follow/EarthDailyAgro?style=social [youtube-shield]:
 https://img.shields.io/youtube/channel/views/UCy4X-
 hM2xRK3oyC_xYKSG_g?style=social [youtube-url]: https://img.shields.io/youtube/
 channel/views/UCy4X-hM2xRK3oyC_xYKSG_g?style=social [language-python-shiedl]:
 https://img.shields.io/badge/python-3.9-green?logo=python [language-python-
 url]: https://pypi.org/ [GitStars-shield]: https://img.shields.io/github/stars/
 GEOSYS?style=social [GitStars-url]: https://img.shields.io/github/stars/
 GEOSYS?style=social [CITest-shield]: https://img.shields.io/github/workflow/
-status/GEOSYS/qgis-plugin/Continous%20Integration [CITest-url]: https://
-img.shields.io/github/workflow/status/GEOSYS/qgis-plugin/
-Continous%20Integration
+status/GEOSYS/GeosysPy/Continous%20Integration [CITest-url]: https://
+img.shields.io/github/workflow/status/GEOSYS/GeosysPy/Continous%20Integration
```

### Comparing `geosyspy-0.1.2/geosyspy/geosys.py` & `geosyspy-0.1.3/geosyspy/geosys.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,198 +1,59 @@
-from oauthlib.oauth2 import LegacyApplicationClient
-from requests_oauthlib import OAuth2Session
-from oauthlib.oauth2 import TokenExpiredError
+from datetime import datetime
 import json
-import re
 from urllib.parse import urljoin
 import pandas as pd
-from . import platforms
 import logging
 import io
 import zipfile
 from rasterio.io import MemoryFile
+from requests import HTTPError
 from shapely import wkt
 from pathlib import Path
-from . import image_reference
+from geosyspy import image_reference
 import xarray as xr
 import rasterio
 import numpy as np
-from .constants import Collection
-
-
-def renew_access_token(func):
-    """Decorator used to wrap the Geosys class's http methods.
-
-    This decorator wraps the geosys http methods (get,post...) and checks
-    wether the used token is still valid or not. If not, it fetches a new token and
-    uses it to make another request.
-
-    """
-
-    def wrapper(self, *args, **kwargs):
-        try:
-            return func(self, *args, **kwargs)
-        except TokenExpiredError:
-            self._Geosys__refresh_token()
-            return func(self, *args, **kwargs)
-
-    return wrapper
 
+from geosyspy.utils.helper import *
+from geosyspy.utils.constants import *
+from geosyspy.utils.http_client import *
+from geosyspy.utils.geosys_platform_urls import *
 
 class Geosys:
-    """Geosys is the main client class to access all the Geosys APIs capabilities.
-
-    `client = Geosys(api_client_id, api_client_secret, api_username, api_password, env, region)`
-
-    Parameters:
-        str_api_client_id (str): The client id
-        str_api_client_secret (str): The client secret
-        str_api_username (str): The api username
-        str_api_password (str): The api user password
-        enum_env (enum): 'Env.PROD' or 'Env.PREPROD'
-        enum_region (enum): 'Region.NA' or 'Region.EU'
-        str_priority_queue (str): 'realtime' or 'bulk'
-    """
-
-    def __init__(
-        self,
-        str_api_client_id,
-        str_api_client_secret,
-        str_api_username,
-        str_api_password,
-        enum_env,
-        enum_region,
-        str_priority_queue="realtime",
-    ):
+    def __init__(self, client_id: str,
+                 client_secret: str,
+                 username: str,
+                 password: str,
+                 enum_env: Env,
+                 enum_region: Region,
+                 priority_queue: str = "realtime",
+                 ):
         """Initializes a Geosys instance with the required credentials
         to connect to the GEOSYS API.
         """
-        self.region = enum_region
-        self.env = enum_env
-        self.str_id_server_url = platforms.IDENTITY_URLS[enum_region.value][enum_env.value]
-        self.base_url = platforms.GEOSYS_API_URLS[enum_region.value][enum_env.value]
-        self.master_data_management_endpoint = "master-data-management/v6/seasonfields"
-        self.vts_endpoint = "vegetation-time-series/v1/season-fields"
-        self.vts_by_pixel_endpoint = "vegetation-time-series/v1/season-fields/pixels"
-        self.flm_catalog_imagery = (
-            "field-level-maps/v4/season-fields/{}/catalog-imagery"
-        )
-        self.flm_coverage = "field-level-maps/v4/season-fields/{}/coverage"
-        self.weather_endpoint = "Weather/v1/weather"
-        self.analytics_fabric_endpoint = "analytics/metrics"
-        self.analytics_fabric_schema_endpoint = "analytics/schemas"
-        self.str_api_client_id = str_api_client_id
-        self.str_api_client_secret = str_api_client_secret
-        self.str_api_username = str_api_username
-        self.str_api_password = str_api_password
-        self.token = None
-        self.priority_queue = str_priority_queue
-        self.priority_headers = {"bulk": "Geosys_API_Bulk", "realtime": ""}
-        self.list_collection_lr = [Collection.MODIS]
-        self.list_collection_mr = [Collection.LANDSAT_8, Collection.LANDSAT_9, Collection.SENTINEL_2]
-        self.list_collection_weather = [
-            Collection.WEATHER_FORECAST_DAILY,
-            Collection.WEATHER_FORECAST_HOURLY,
-            Collection.WEATHER_HISTORICAL_DAILY,
-        ]
-        self.__authenticate()
-
-    def __authenticate(self):
-        """Authenticates the client to the API.
-
-        This method connects the user to the API which generates a token that
-        will be valid for one hour. A refresh token is also generated, which
-        makes it possible for the http methods wrappers to get a new token
-        once the previous one is no more valid through the renew_access_token
-        decorator. This method is only run once when a Geosys object is instantiated.
-
-        """
-
-        try:
-            oauth = OAuth2Session(
-                client=LegacyApplicationClient(client_id=self.str_api_client_id)
-            )
-            self.token = oauth.fetch_token(
-                token_url=self.str_id_server_url,
-                username=self.str_api_username,
-                password=self.str_api_password,
-                client_id=self.str_api_client_id,
-                client_secret=self.str_api_client_secret,
-            )
-            self.token["refresh_token"] = oauth.cookies["refresh_token"]
-            logging.info("Authenticated")
-        except Exception as e:
-            logging.error(e)
-
-    def __refresh_token(self):
-        """Fetches a new token."""
-
-        client = OAuth2Session(self.str_api_client_id, token=self.token)
-        self.token = client.refresh_token(
-            self.str_id_server_url,
-            client_id=self.str_api_client_id,
-            client_secret=self.str_api_client_secret,
-        )
+        self.region: str = enum_region.value
+        self.env: str = enum_env.value
+        self.base_url: str = GEOSYS_API_URLS[enum_region.value][enum_env.value]
+        self.priority_queue: str = priority_queue
+        self.http_client: HttpClient = HttpClient(client_id, client_secret, username, password, enum_env.value,
+                                                  enum_region.value)
 
-    def __get_matched_str_from_pattern(self, pattern, text):
-        """Returns the first occurence of the matched pattern in text.
-
-        Args:
-            pattern : A string representing the regex pattern to look for.
-            text : The text to look into.
-
-        Returns:
-            A string representing the first occurence in text of the pattern.
-
-        """
-        p = re.compile(pattern)
-        return p.findall(text)[0]
-
-    @renew_access_token
-    def __get(self, url_endpoint, headers={}):
-        """Gets the url_endpopint.
-
-        Args:
-            url_endpoint : A string representing the url to get.
-
-        Returns:
-            A response object.
-        """
-        client = OAuth2Session(self.str_api_client_id, token=self.token)
-        return client.get(url_endpoint, headers=headers)
-
-    @renew_access_token
-    def __post(self, url_endpoint, payload, headers={}):
-        """Posts payload to the url_endpoint.
-
-        Args:
-            url_endpoint : A string representing the url to post paylaod to.
-            payload : A python dict representing the payload.
-
-        Returns:
-            A response object.
-        """
-        client = OAuth2Session(self.str_api_client_id, token=self.token)
-        return client.post(url_endpoint, json=payload, headers=headers)
+    """Geosys is the main client class to access all the Geosys APIs capabilities.
 
-    @renew_access_token
-    def __patch(self, url_endpoint, payload):
-        """Patchs payload to the url_endpoint.
+    `client = Geosys(api_client_id, api_client_secret, api_username, api_password, env, region)`
 
-        Args:
-            url_endpoint : A string representing the url to patch paylaod to.
-            payload : A python dict representing the payload.
+    Parameters:
+        enum_env: 'Env.PROD' or 'Env.PREPROD'
+        enum_region: 'Region.NA' or 'Region.EU'
+        priority_queue: 'realtime' or 'bulk'
+    """
 
-        Returns:
-            A response object.
-        """
-        client = OAuth2Session(self.str_api_client_id, token=self.token)
-        return client.patch(url_endpoint, json=payload)
 
-    def __create_season_field_id(self, polygon):
+    def __create_season_field_id(self, polygon: str) -> object:
         """Posts the payload below to the master data management endpoint.
 
         This method returns a season field id. The season field id is required
         to request other APIs endpoints.
 
         Args:
             polygon : A string representing a polygon.
@@ -202,19 +63,18 @@
 
         """
         payload = {
             "Geometry": polygon,
             "Crop": {"Id": "CORN"},
             "SowingDate": "2022-01-01",
         }
-        str_mdm_url = urljoin(self.base_url, self.master_data_management_endpoint)
-
-        return self.__post(str_mdm_url, payload)
+        mdm_url: str = urljoin(self.base_url, GeosysApiEndpoints.MASTER_DATA_MANAGEMENT_ENDPOINT.value)
+        return self.http_client.post(mdm_url, payload)
 
-    def __extract_season_field_id(self, polygon):
+    def __extract_season_field_id(self, polygon: str) -> str:
         """Extracts the season field id from the response object.
 
         Args:
             polygon : A string representing a polygon.
 
         Returns:
             A string rerpesenting the season field id.
@@ -223,95 +83,103 @@
             ValueError: The response status code is not as expected.
         """
 
         response = self.__create_season_field_id(polygon)
         dict_response = response.json()
 
         if (
-            response.status_code == 400
-            and "sowingDate" in dict_response["errors"]["body"]
+                response.status_code == 400
+                and "sowingDate" in dict_response["errors"]["body"]
         ):
-            pattern = r"\sId:\s(\w+),"
-            str_text = dict_response["errors"]["body"]["sowingDate"][0]["message"]
-            return self.__get_matched_str_from_pattern(pattern, str_text)
+
+            text: str = dict_response["errors"]["body"]["sowingDate"][0]["message"]
+            return Helper.get_matched_str_from_pattern(SEASON_FIELD_ID_REGEX, text)
 
         elif response.status_code == 201:
             return dict_response["id"]
         else:
             raise ValueError(
                 f"Cannot handle HTTP response : {str(response.status_code)} : {str(response.json())}"
             )
 
-    def get_time_series(self, polygon, start_date, end_date, collection, indicators):
+    def get_time_series(self, polygon: str,
+                        start_date: datetime,
+                        end_date: datetime,
+                        collection: enumerate,
+                        indicators: [str]) -> pd.DataFrame:
         """Retrieve a time series of the indicator for the aggregated polygon on the collection targeted.
 
         Args:
-            polygon (str): The polygon
-            start_date (datetime): The start date of the time series
-            end_date (datetime): The end date of the time series
-            collection (enum): The collection targeted
-            indicators (str list): The indicators to retrieve on the collection
+            polygon : The polygon
+            start_date : The start date of the time series
+            end_date : The end date of the time series
+            collection : The collection targeted
+            indicators : The indicators to retrieve on the collection
 
         Returns:
             (dataframe): A pandas dataframe for the time series
 
         Raises:
             ValueError: The collection doesn't exist
         """
-
-        if collection in self.list_collection_weather:
+        if collection in WeatherTypeCollection:
             return self.__get_weather(
                 polygon,
                 start_date,
                 end_date,
-                collection.value.split(".").pop(),
+                collection,
                 indicators,
             )
-        elif collection in self.list_collection_lr:
+        elif collection in LR_SATELLITE_COLLECTION:
             return self.__get_modis_time_series(
                 polygon, start_date, end_date, indicators[0]
             )
         else:
             raise ValueError(f"{collection} collection doesn't exist")
 
-    def get_satellite_image_time_series(
-        self, polygon, start_date, end_date, collections, indicators
-    ):
-        """Retrieve a pixel-by-pxel time series of the indicator on the collection targeted.
-
-        Args:
-            polygon (str): The polygon
-            start_date (datetime): The start date of the time series
-            end_date (datetime): The end date of the time series
-            collections (enum list): The collections targeted
-            indicators (str list): The indicators to retrieve on the collections
+    def get_satellite_image_time_series(self, polygon: str,
+                                        start_date: datetime,
+                                        end_date: datetime,
+                                        collections: list[SatelliteImageryCollection],
+                                        indicators: [str]
+                                        ):
+        """Retrieve a pixel-by-pixel time series of the indicator on the collection targeted.
+
+        Args:
+            polygon : The polygon
+            start_date : The start date of the time series
+            end_date : The end date of the time series
+            collections : The Satellite Imagery Collection targeted
+            indicators : The indicators to retrieve on the collections
 
         Returns:
-            ('dataframe or xarray'): Either a pandas dataframe or an xarray for the time series
+            ('dataframe or xarray'): Either a pandas dataframe or a xarray for the time series
         """
-
         if not collections:
             raise ValueError(
-                "The argument collections is empty. It must be a list of constants.Collection objects"
+                "The argument collections is empty. It must be a list of SatelliteImageryCollection objects"
             )
-        elif all([isinstance(elem, Collection) for elem in collections]):
-            if set(collections).issubset(set(self.list_collection_lr)):
+        elif all([isinstance(elem, SatelliteImageryCollection) for elem in collections]):
+            if set(collections).issubset(set(LR_SATELLITE_COLLECTION)):
                 return self.__get_time_series_by_pixel(
                     polygon, start_date, end_date, indicators[0]
                 )
-            elif set(collections).issubset(set(self.list_collection_mr)):
+            elif set(collections).issubset(set(MR_SATELLITE_COLLECTION)):
                 return self.__get_images_as_dataset(
-                    polygon, start_date, end_date, collections
+                    polygon, start_date, end_date, collections, indicators[0]
                 )
         else:
             raise TypeError(
-                f"Argument collections must be a list of constants.Collection objects"
+                f"Argument collections must be a list of SatelliteImageryCollection objects"
             )
 
-    def __get_modis_time_series(self, polygon, start_date, end_date, indicator):
+    def __get_modis_time_series(self, polygon: str,
+                                start_date: datetime,
+                                end_date: datetime,
+                                indicator: str) -> pd.DataFrame:
         """Returns a pandas DataFrame.
 
         This method returns a time series of 'indicator' within the range
         'start_date' -> 'end_date' as a pandas DataFrame :
 
                      | index     | value |
 
@@ -330,31 +198,33 @@
             indicator : A string representing the indicator whose time series the user wants.
 
         Returns:
             df : A Pandas DataFrame containing two columns : index and value, and an index called 'date'.
 
         """
         logging.info("Calling APIs for aggregated time series")
-        str_season_field_id = self.__extract_season_field_id(polygon)
-        str_start_date = start_date.strftime("%Y-%m-%d")
-        str_end_date = end_date.strftime("%Y-%m-%d")
-        parameters = f"/values?$offset=0&$limit=9999&$count=false&SeasonField.Id={str_season_field_id}&index={indicator}&$filter=Date >= '{str_start_date}' and Date <= '{str_end_date}'"
-        str_vts_url = urljoin(self.base_url, self.vts_endpoint + parameters)
-
-        response = self.__get(str_vts_url)
+        season_field_id: str = self.__extract_season_field_id(polygon)
+        start_date: str = start_date.strftime("%Y-%m-%d")
+        end_date: str = end_date.strftime("%Y-%m-%d")
+        parameters: str = f"/values?$offset=0&$limit=9999&$count=false&SeasonField.Id={season_field_id}&index={indicator}&$filter=Date >= '{start_date}' and Date <= '{end_date}'"
+        vts_url: str = urljoin(self.base_url, GeosysApiEndpoints.VTS_ENDPOINT.value + parameters)
+        response = self.http_client.get(vts_url)
 
         if response.status_code == 200:
             dict_response = response.json()
             df = pd.read_json(json.dumps(dict_response))
             df.set_index("date", inplace=True)
             return df
         else:
             logging.info(response.status_code)
 
-    def __get_time_series_by_pixel(self, polygon, start_date, end_date, indicator):
+    def __get_time_series_by_pixel(self, polygon: str,
+                                   start_date: datetime,
+                                   end_date: datetime,
+                                   indicator: str) -> pd.DataFrame:
         """Returns a pandas DataFrame.
 
         This method returns a time series of 'indicator' by pixel within the range 'start_date' -> 'end_date'
         as well as the pixel's coordinates X,Y in the MODIS's sinusoidal projection as a pandas DataFrame :
 
 
 
@@ -377,28 +247,28 @@
 
         Returns:
             df : A Pandas DataFrame containing five columns : index, value, pixel.id, X, Y and an index called 'date'.
 
         """
 
         logging.info("Calling APIs for time series by the pixel")
-        str_season_field_id = self.__extract_season_field_id(polygon)
-        str_start_date = start_date.strftime("%Y-%m-%d")
-        str_end_date = end_date.strftime("%Y-%m-%d")
-        parameters = f"/values?$offset=0&$limit=9999&$count=false&SeasonField.Id={str_season_field_id}&index={indicator}&$filter=Date >= '{str_start_date}' and Date <= '{str_end_date}'"
-        str_vts_url = urljoin(self.base_url, self.vts_by_pixel_endpoint + parameters)
+        season_field_id: str = self.__extract_season_field_id(polygon)
+        start_date: str = start_date.strftime("%Y-%m-%d")
+        end_date: str = end_date.strftime("%Y-%m-%d")
+        parameters: str = f"/values?$offset=0&$limit=9999&$count=false&SeasonField.Id={season_field_id}&index={indicator}&$filter=Date >= '{start_date}' and Date <= '{end_date}'"
+        vts_url: str = urljoin(self.base_url, GeosysApiEndpoints.VTS_BY_PIXEL_ENDPOINT.value + parameters)
         # PSX/PSY : size in meters of one pixel
         # MODIS_GRID_LENGTH : theoretical length of the modis grid in meters
-        # MOIS_GRID_HEIGHT : theoretical height of the modis grid in meters
+        # MODIS_GRID_HEIGHT : theoretical height of the modis grid in meters
         PSX = 231.65635826
         PSY = -231.65635826
         MODIS_GRID_LENGTH = 4800 * PSX * 36
         MODIS_GRID_HEIGHT = 4800 * PSY * 18
 
-        response = self.__get(str_vts_url)
+        response = self.http_client.get(vts_url)
 
         if response.status_code == 200:
             df = pd.json_normalize(response.json())
             df.set_index("date", inplace=True)
 
             # Extracts h, v, i and j from the pixel dataframe
             logging.info("Computing X and Y coordinates per pixel... ")
@@ -414,124 +284,155 @@
             df["X"] = df["i"] * PSX + df["XUL"]
             df["Y"] = df["j"] * PSY + df["YUL"]
             logging.info("Done ! ")
             return df[["index", "value", "pixel.id", "X", "Y"]]
         else:
             logging.info(response.status_code)
 
-    def get_satellite_coverage_image_references(
-        self, polygon, start_date, end_date, collections=[Collection.SENTINEL_2, Collection.LANDSAT_8]
-    ):
+    def get_satellite_coverage_image_references(self, polygon: str,
+                                                start_date: datetime,
+                                                end_date: datetime,
+                                                collections: list[SatelliteImageryCollection] = [
+                                                    SatelliteImageryCollection.SENTINEL_2,
+                                                    SatelliteImageryCollection.LANDSAT_8]
+                                                ) -> tuple:
         """Retrieves a list of images that covers a polygon on a specific date range.
-        The return is a tuple: a dataframe with all the images covering the polygon, and 
-                    an dictionary images_references. Key= a tuple (image_date, image_sensor).
+        The return is a tuple: a dataframe with all the images covering the polygon, and
+                    a dictionary images_references. Key= a tuple (image_date, image_sensor).
                     Value = an object image_reference, to use with the method `download_image()`
 
         Args:
-            polygon (str): The polygon
-            start_date (datetime): The start date of the time series
-            end_date (datetime): The end date of the time series
-            sensors (str list): The sensors to check the coverage on
+            polygon: The polygon
+            start_date: The start date of the time series
+            end_date: The end date of the time series
+            collections: The sensors to check the coverage on
 
         Returns:
             (tuple): images list and image references for downloading
         """
 
-        df = self.__get_satellite_coverage(polygon, start_date, end_date, collections)
+        df = self.__get_satellite_coverage(polygon, start_date, end_date, "", collections)
         images_references = {}
 
         for i, image in df.iterrows():
             images_references[
                 (image["image.date"], image["image.sensor"])
             ] = image_reference.ImageReference(
                 image["image.id"],
                 image["image.date"],
                 image["image.sensor"],
                 image["seasonField.id"],
             )
 
         return df, images_references
 
-    def __get_satellite_coverage(
-        self, polygon, start_date, end_date, sensors=[Collection.SENTINEL_2, Collection.LANDSAT_8]
-    ):
+    def __get_satellite_coverage(self, polygon: str,
+                                 start_date: datetime,
+                                 end_date: datetime,
+                                 indicator,
+                                 sensors_collection: list[SatelliteImageryCollection] = [
+                                     SatelliteImageryCollection.SENTINEL_2,
+                                     SatelliteImageryCollection.LANDSAT_8]
+                                 ):
         logging.info("Calling APIs for coverage")
-        str_season_field_id = self.__extract_season_field_id(polygon)
-        str_start_date = start_date.strftime("%Y-%m-%d")
-        str_end_date = end_date.strftime("%Y-%m-%d")
-        sensors = [elem.value for elem in sensors]
-        parameters = f"?maps.type=INSEASON_NDVI&Image.Sensor=$in:{'|'.join(sensors)}&CoverageType=CLEAR&$limit=9999&$filter=Image.Date >= '{str_start_date}' and Image.Date <= '{str_end_date}'"
+        season_field_id: str = self.__extract_season_field_id(polygon)
+        start_date: str = start_date.strftime("%Y-%m-%d")
+        end_date: str = end_date.strftime("%Y-%m-%d")
+        sensors: list[str] = [elem.value for elem in sensors_collection]
+
+        if indicator == "" or indicator.upper() == "REFLECTANCE" or indicator.upper() == "NDVI":
+            mapType = "INSEASON_NDVI"
+        else:
+            mapType = f"INSEASON_{indicator.upper()}"
+
+        parameters = f"?maps.type={mapType}&Image.Sensor=$in:{'|'.join(sensors)}&CoverageType=CLEAR&$limit=9999&$filter=Image.Date >= '{start_date}' and Image.Date <= '{end_date}'"
 
-        str_flm_url = urljoin(
+        flm_url: str = urljoin(
             self.base_url,
-            self.flm_catalog_imagery.format(str_season_field_id) + parameters,
+            GeosysApiEndpoints.FLM_CATALOG_IMAGERY.value.format(season_field_id) + parameters,
         )
-        response = self.__get(
-            str_flm_url,
-            {"X-Geosys-Task-Code": self.priority_headers[self.priority_queue]},
+        response = self.http_client.get(
+            flm_url,
+            {"X-Geosys-Task-Code": PRIORITY_HEADERS[self.priority_queue]},
         )
 
         if response.status_code == 200:
             df = pd.json_normalize(response.json())
             if df.empty:
                 return df
             else:
                 return df[
                     [
                         "coverageType",
+                        "maps",
                         "image.id",
                         "image.availableBands",
                         "image.sensor",
                         "image.soilMaterial",
                         "image.spatialResolution",
                         "image.weather",
                         "image.date",
                         "seasonField.id",
-                    ]       
+                    ]
                 ]
         else:
             logging.info(response.status_code)
 
-    def __get_zipped_tiff(self, field_id, image_id):
+    def __get_zipped_tiff(self, field_id: str,
+                          image_id: str,
+                          indicator: str = ""):
         parameters = f"/{image_id}/reflectance-map/TOC/image.tiff.zip"
-        download_tiff_url = urljoin(
-            self.base_url, self.flm_coverage.format(field_id) + parameters
+
+        if indicator != "" and indicator.upper() != "REFLECTANCE":
+            parameters = f"/{image_id}/base-reference-map/INSEASON_{indicator.upper()}/image.tiff.zip?resolution=Sensor"
+
+        download_tiff_url: str = urljoin(
+            self.base_url, GeosysApiEndpoints.FLM_COVERAGE.value.format(field_id) + parameters
         )
 
-        response_zipped_tiff = self.__get(
+        response_zipped_tiff = self.http_client.get(
             download_tiff_url,
-            {"X-Geosys-Task-Code": self.priority_headers[self.priority_queue]},
+            {"X-Geosys-Task-Code": PRIORITY_HEADERS[self.priority_queue]},
         )
+        if response_zipped_tiff.status_code != 200:
+            raise HTTPError("Unable to download tiff.zip file. Server error: " + str(response_zipped_tiff.status_code))
         return response_zipped_tiff
 
-    def download_image(self, image_reference, str_path=""):
+    def download_image(self, image_reference,
+                       path: str = ""):
         """Downloads a satellite image locally
 
         Args:
             image_reference (ImageReference): An ImageReference object representing the image to download
-            str_path (str): the path to download the image to
+            path (str): the path to download the image to
         """
+
         response_zipped_tiff = self.__get_zipped_tiff(
             image_reference.season_field_id, image_reference.image_id
         )
-        if str_path == "":
-            str_path = Path.cwd() / f"image_{image_reference.image_id}_tiff.zip"
-        with open(str_path, "wb") as f:
-            logging.info(f"writing to {str_path}")
+        if path == "":
+            path = Path.cwd() / f"image_{image_reference.image_id}_tiff.zip"
+        with open(path, "wb") as f:
+            logging.info(f"writing to {path}")
             f.write(response_zipped_tiff.content)
 
-    def __get_images_as_dataset(self, polygon, start_date, end_date, collections):
+    def __get_images_as_dataset(self, polygon: str,
+                                start_date: datetime,
+                                end_date: datetime,
+                                collections: list[SatelliteImageryCollection],
+                                indicator: str) -> 'np.ndarray[Any , np.dtype[np.float64]]':
         """Returns all the 'sensors_list' images covering 'polygon' between
-        'start_date' and 'end_date' as an xarray dataset.
+        'start_date' and 'end_date' as a xarray dataset.
 
         Args:
             polygon : A string representing the polygon that the images will be covering.
             start_date : The date from which the method will start looking for images.
-            end_date : The date at which the methd will stop looking images.
-            sensors_list : A list of the sensors' names as strings.
+            end_date : The date at which the method will stop looking images.
+            collections : A list of Satellite Imagery Collection.
+            indicator : A string representing the indicator whose time series the user wants.
 
         Returns:
             The image's numpy array.
 
         """
 
         def get_coordinates_by_pixel(raster):
@@ -550,15 +451,15 @@
             lst_lons = list(lons[0])
             return {"y": lst_lats, "x": lst_lons}
 
         # Selects the covering images in the provided date range
         # and sorts them by resolution, from the highest to the lowest.
         # Keeps only the first image if two are found on the same date.
         df_coverage = self.__get_satellite_coverage(
-            polygon, start_date, end_date, collections
+            polygon, start_date, end_date, indicator, collections
         )
 
         # Return empty dataset if no coverage on the polygon between start_date, end_date
         if df_coverage.empty:
             return xr.Dataset()
 
         df_coverage["image.date"] = pd.to_datetime(
@@ -568,79 +469,80 @@
             by=["image.spatialResolution", "image.date"], ascending=[True, True]
         ).drop_duplicates(subset="image.date", keep="first")
 
         # Creates a dictionary that contains a zip archive containing the tif file
         # for each image id and some additional data (bands, sensor...)
         dict_archives = {}
         for i, row in df_coverage.iterrows():
+            if indicator.upper() != "REFLECTANCE":
+                bands = [indicator]
+            else:
+                bands = row["image.availableBands"]
             dict_archives[row["image.id"]] = {
                 "byte_archive": self.__get_zipped_tiff(
-                    row["seasonField.id"], row["image.id"]
+                    row["seasonField.id"], row["image.id"], indicator
                 ).content,
-                "bands": row["image.availableBands"],
+                "bands": bands,
                 "date": row["image.date"],
                 "sensor": row["image.sensor"],
             }
 
         # Extracts the tif files from  the zip archives in memory
         # and transforms them into a list of xarray DataArrays.
         # A list of all the raster's crs is also created in order
         # to merge this data in the final xarray Dataset later on.
         list_xarr = []
         list_crs = []
         first_img_id = df_coverage.iloc[0]["image.id"]
         for img_id, dict_data in dict_archives.items():
             with zipfile.ZipFile(io.BytesIO(dict_data["byte_archive"]), "r") as archive:
-                list_files = archive.namelist()
-                for file in list_files:
-                    list_words = file.split(".")
-                    if list_words[-1] == "tif":
-                        img_in_bytes = archive.read(file)
-                        with MemoryFile(img_in_bytes) as memfile:
-                            with memfile.open() as raster:
-                                dict_coords = get_coordinates_by_pixel(raster)
-                                xarr = xr.DataArray(
-                                    raster.read(masked=True),
-                                    dims=["band", "y", "x"],
-                                    coords={
-                                        "band": dict_data["bands"],
-                                        "y": dict_coords["y"],
-                                        "x": dict_coords["x"],
-                                        "time": dict_data["date"],
-                                    },
+                images_in_bytes = [archive.read(file) for file in archive.namelist() if file.endswith('.tif')]
+                for image in images_in_bytes:
+                    with MemoryFile(image) as memfile:
+                        with memfile.open() as raster:
+                            dict_coords = get_coordinates_by_pixel(raster)
+                            xarr = xr.DataArray(
+                                raster.read(masked=True),
+                                dims=["band", "y", "x"],
+                                coords={
+                                    "band": dict_data["bands"],
+                                    "y": dict_coords["y"],
+                                    "x": dict_coords["x"],
+                                    "time": dict_data["date"],
+                                },
+                            )
+
+                            if img_id == first_img_id:
+                                len_y = len(dict_coords["y"])
+                                len_x = len(dict_coords["x"])
+                                print(
+                                    f"The highest resolution's image grid size is {(len_x, len_y)}"
                                 )
-
-                                if img_id == first_img_id:
-                                    len_y = len(dict_coords["y"])
-                                    len_x = len(dict_coords["x"])
-                                    print(
-                                        f"The highest resolution's image grid size is {(len_x, len_y)}"
-                                    )
-                                else:
-                                    logging.info(
-                                        f"interpolating {img_id} to {first_img_id}'s grid"
-                                    )
-                                    xarr = xarr.interp(
-                                        x=list_xarr[0].coords["x"].data,
-                                        y=list_xarr[0].coords["y"].data,
-                                        method="linear",
-                                    )
-                                list_xarr.append(xarr)
-                                list_crs.append(raster.crs.to_string())
+                            else:
+                                logging.info(
+                                    f"interpolating {img_id} to {first_img_id}'s grid"
+                                )
+                                xarr = xarr.interp(
+                                    x=list_xarr[0].coords["x"].data,
+                                    y=list_xarr[0].coords["y"].data,
+                                    method="linear",
+                                )
+                            list_xarr.append(xarr)
+                            list_crs.append(raster.crs.to_string())
 
         # Adds the img's raster's crs to the initial dataframe
         df_coverage["crs"] = list_crs
 
         # Concatenates all the DataArrays in list_xarr in order
         # to create one final DataArray with an additional dimension
         # 'time'. This final DataArray is then transformed into
-        # an xarray Dataset containing one data variable "reflectance".
+        # a xarray Dataset containing one data variable "reflectance".
 
         final_xarr = xr.concat(list_xarr, "time")
-        dataset = xr.Dataset(data_vars={"reflectance": final_xarr})
+        dataset = xr.Dataset(data_vars={indicator.lower(): final_xarr})
 
         # Adds additional metadata to the dataset.
         dataset = dataset.assign_coords(
             **{
                 k: ("time", np.array(v))
                 for k, v in df_coverage[
                     [
@@ -654,67 +556,67 @@
                 ]
                 .to_dict(orient="list")
                 .items()
             }
         )
         return dataset
 
-    def __get_weather(self, polygon, start_date, end_date, weather_type, fields):
+    def __get_weather(self, polygon: str,
+                      start_date: datetime,
+                      end_date: datetime,
+                      weather_type: WeatherTypeCollection,
+                      fields: [str]):
         """Returns the weather data as a pandas dataframe.
 
         Args:
             polygon : A string representing a polygon.
             start_date : A datetime object representing the start date of the date interval the user wants to filter on.
             end_date : A datetime object representing the final date of the date interval the user wants to filter on.
-            weather_type : A string representing the collection ["HISTORICAL_DAILY", "FORECAST_DAILY", "FORECAST_HOURLY"]
-            fields : An array of strings representings the fields to select (eg: Precipitation, Temperature)
+            weather_type : A list representing the weather type collection ["HISTORICAL_DAILY", "FORECAST_DAILY", "FORECAST_HOURLY"]
+            fields : A list of strings representing the fields to select (eg: Precipitation, Temperature)
 
         Returns:
             The image's numpy array.
 
         """
 
-        allowed_weather_types = [
-            "HISTORICAL_DAILY",
-            "FORECAST_DAILY",
-            "FORECAST_HOURLY",
-        ]
-        if weather_type not in allowed_weather_types:
-            raise ValueError(f"weather_type should be either {allowed_weather_types}")
-
+        if weather_type not in WeatherTypeCollection:
+            raise ValueError(f"weather_type should be either {[item.value for item in WeatherTypeCollection]}")
+        weather_type = weather_type.value
         if "Date" not in fields:
             fields.append("Date")
 
-        str_start_date = start_date.strftime("%Y-%m-%d")
-        str_end_date = end_date.strftime("%Y-%m-%d")
+        start_date: str = start_date.strftime("%Y-%m-%d")
+        end_date: str = end_date.strftime("%Y-%m-%d")
         polygon_wkt = wkt.loads(polygon)
-        str_weather_fields = ",".join(fields)
-        parameters = f"?%24offset=0&%24limit=9999&%24count=false&Location={polygon_wkt.centroid.wkt}&Date=%24between%3A{str_start_date}T00%3A00%3A00.0000000Z%7C{str_end_date}T00%3A00%3A00.0000000Z&Provider=GLOBAL1&WeatherType={weather_type}&$fields={str_weather_fields}"
-        str_weather_url = urljoin(self.base_url, self.weather_endpoint + parameters)
+        weather_fields: str = ",".join(fields)
+        parameters: str = f"?%24offset=0&%24limit=9999&%24count=false&Location={polygon_wkt.centroid.wkt}&Date=%24between%3A{start_date}T00%3A00%3A00.0000000Z%7C{end_date}T00%3A00%3A00.0000000Z&Provider=GLOBAL1&WeatherType={weather_type}&$fields={weather_fields}"
+        weather_url: str = urljoin(self.base_url, GeosysApiEndpoints.WEATHER_ENDPOINT.value + parameters)
 
-        response = self.__get(str_weather_url)
+        response = self.http_client.get(weather_url)
 
         if response.status_code == 200:
             df = pd.json_normalize(response.json())
             if df.empty:
                 return df
             else:
                 df.set_index("date", inplace=True)
                 df["Location"] = polygon_wkt.centroid.wkt
                 return df.sort_index()
         else:
             logging.error(response.status_code)
             raise ValueError(response.content)
 
-    def create_schema_id(self, schema_id, schema):
+    def create_schema_id(self, schema_id: str,
+                         schema: dict):
         """Create a schema in Analytics Fabrics
 
         Args:
-            schema_id (str): The schema id to create
-            schema (dict): Dict representing the schema {'property_name': 'property_type'}
+            schema_id: The schema id to create
+            schema: Dict representing the schema {'property_name': 'property_type'}
 
         Returns:
             A http response object.
         """
         properties = []
         for prop_name, datatype in schema.items():
             prop = {
@@ -727,86 +629,141 @@
             properties.append(prop)
 
         payload = {
             "Id": schema_id,
             "Properties": properties,
             "Metadata": {"OnAggregationCompleted": "Off"},
         }
-        str_af_url = urljoin(
+        af_url: str = urljoin(
             self.base_url,
-            self.analytics_fabric_schema_endpoint,
+            GeosysApiEndpoints.ANALYTICS_FABRIC_SCHEMA_ENDPOINT.value,
         )
-        response = self.__post(str_af_url, payload)
+        response = self.http_client.post(af_url, payload)
         if response.status_code == 201:
             return response.content
         else:
             logging.info(response.status_code)
 
-    def get_metrics(self, polygon, schema_id, start_date, end_date):
+    def _get_s3_path(self, task_id: str):
+
+        endpoint: str = GeosysApiEndpoints.MRTS_PROCESSOR_EVENTS_ENDPOINT.value + "/" + task_id
+        response = self.http_client.get(endpoint)
+        if response.ok:
+            dict_resp = json.loads(response.content)
+            customer_code: str = dict_resp["customerCode"].lower().replace("_", "-")
+            user_id: str = dict_resp["userId"]
+            task_id = dict_resp["taskId"]
+            return "s3://geosys-" + customer_code + "/" + user_id + "/mrts/" + task_id
+        else:
+            logging.info(response.status_code)
+
+    def get_mr_time_series(self, start_date: str, end_date: str, list_sensors, denoiser: bool, smoother: str, eoc: bool,
+                           func: str, index: str, raw_data: bool, polygon: str):
+        payload = {
+            "parametersProfile": {
+                "code": "mrts_default",
+                "version": 1
+            },
+            "parameters": {
+                "start_date": start_date,
+                "end_date": end_date,
+                "sensors": list_sensors,
+                "denoiser": denoiser,
+                "smoother": smoother,
+                "eoc": eoc,
+                "aggregation": func,
+                "index": index,
+                "raw_data": raw_data
+            },
+            "data": [
+                {"wkt": polygon}
+            ]
+        }
+
+        response = self.http_client.post(GeosysApiEndpoints.MRTS_PROCESSOR_ENDPOINT.value, payload)
+
+        if response.ok:
+            task_id = json.loads(response.content)["taskId"]
+            return self._get_s3_path(task_id)
+        else:
+            logging.info(response.status_code)
+
+    def get_metrics(self, polygon: str,
+                    schema_id: str,
+                    start_date: datetime,
+                    end_date: datetime):
         """Returns metrics from Analytics Fabrics in a pandas dataframe.
 
         Args:
-            polygon (str): A string representing a polygon.
-            start_date (datetime): A datetime object representing the start date of the date interval the user wants to filter on.
-            end_date (datetime): A datetime object representing the final date of the date interval the user wants to filter on.
-            schema_id (str): A string representing a schema existing in Analytics Fabrics
+            polygon : A string representing a polygon.
+            start_date : A datetime object representing the start date of the date interval the user wants to filter on.
+            end_date : A datetime object representing the final date of the date interval the user wants to filter on.
+            schema_id : A string representing a schema existing in Analytics Fabrics
 
         Returns:
-            df : A Pandas DataFrame containing severals columns with metrics
+            df : A Pandas DataFrame containing several's columns with metrics
 
         """
-        season_field_id = self.__extract_season_field_id(polygon)
+        season_field_id: str = self.__extract_season_field_id(polygon)
         logging.info("Calling APIs for metrics")
-        str_start_date = start_date.strftime("%Y-%m-%d")
-        str_end_date = end_date.strftime("%Y-%m-%d")
-        parameters = f'?%24limit=9999&Timestamp=$between:{str_start_date}|{str_end_date}&$filter=Entity.ExternalTypedIds.Contains("SeasonField:{season_field_id}@LEGACY_ID_{self.region.value.upper()}")&$filter=Schema.Id=={schema_id}'
-        str_af_url = urljoin(
+        start_date: str = start_date.strftime("%Y-%m-%d")
+        end_date: str = end_date.strftime("%Y-%m-%d")
+        parameters: str = f'?%24limit=9999&Timestamp=$between:{start_date}|{end_date}&$filter=Entity.ExternalTypedIds.Contains("SeasonField:{season_field_id}@LEGACY_ID_{self.region.upper()}")&$filter=Schema.Id=={schema_id}'
+        af_url: str = urljoin(
             self.base_url,
-            self.analytics_fabric_endpoint + parameters,
+            GeosysApiEndpoints.ANALYTICS_FABRIC_ENDPOINT.value + parameters,
         )
-        response = self.__get(str_af_url)
+        response = self.http_client.get(af_url)
 
         if response.status_code == 200:
             df = pd.json_normalize(response.json())
+            if df.empty:
+                logging.info(f"No metrics found in Analytic Fabric with "
+                             f"SchemaId: {schema_id}, "
+                             f"SeasonField:{season_field_id}@LEGACY_ID_{self.region.upper()} "
+                             f"between:{start_date} and{end_date} ")
+                return df
             df.drop("Entity.TypedId", inplace=True, axis=1)
             df.rename(
                 columns={"Timestamp": "date"},
                 inplace=True,
             )
             df = df.sort_values(by="date")
             df.set_index("date", inplace=True)
             return df
         else:
             logging.info(response.status_code)
 
-    def push_metrics(self, polygon, schema_id, values):
+    def push_metrics(self, polygon: str,
+                     schema_id: str,
+                     values: dict):
         """Push metrics in Analytics Fabrics
 
         Args:
             polygon : A string representing the polygon.
             schema_id : The schema on which to save
             values : Dict representing values to push
 
         Returns:
             A response object.
         """
-        season_field_id = self.__extract_season_field_id(polygon)
+        season_field_id: str = self.__extract_season_field_id(polygon)
         payload = []
         for value in values:
             prop = {
                 "Entity": {
-                    "TypedId": f"SeasonField:{season_field_id}@LEGACY_ID_{self.region.value.upper()}"
+                    "TypedId": f"SeasonField:{season_field_id}@LEGACY_ID_{self.region.upper()}"
                 },
                 "Schema": {"Id": schema_id, "Version": 1},
             }
             prop = dict(prop, **value)
             payload.append(prop)
 
-        str_af_url = urljoin(
+        af_url: str = urljoin(
             self.base_url,
-            self.analytics_fabric_endpoint,
+            GeosysApiEndpoints.ANALYTICS_FABRIC_SCHEMA_ENDPOINT.value,
         )
-        response = self.__patch(str_af_url, payload)
+        response = self.http_client.patch(af_url, payload)
         if response.status_code == 200:
             return response.status_code
         else:
             logging.info(response.status_code)
```

### Comparing `geosyspy-0.1.2/setup.py` & `geosyspy-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     description="Easy-to-use python wrapper for Geosys APIs (time series, imagery products)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Geosys",
     packages=["geosyspy"],
     include_package_data=True,
     data_files=[('', ['VERSION.txt'])],
-    install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray"]
+    install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray", "boto3"]
 )
```

