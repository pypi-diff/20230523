# Comparing `tmp/integerbook-0.0.3.tar.gz` & `tmp/integerbook-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integerbook-0.0.3.tar", last modified: Sun Apr 23 23:25:48 2023, max compression
+gzip compressed data, was "integerbook-0.0.4.tar", last modified: Tue May 23 09:37:16 2023, max compression
```

## Comparing `integerbook-0.0.3.tar` & `integerbook-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.789423 integerbook-0.0.3/
--rw-r--r--   0 jvo        (501) staff       (20)    35149 2022-03-18 13:05:53.000000 integerbook-0.0.3/LICENSE
--rw-r--r--   0 jvo        (501) staff       (20)       84 2023-04-23 18:25:14.000000 integerbook-0.0.3/MANIFEST.in
--rw-r--r--   0 jvo        (501) staff       (20)    42511 2023-04-23 23:25:48.788907 integerbook-0.0.3/PKG-INFO
--rw-r--r--   0 jvo        (501) staff       (20)     1497 2023-04-23 18:25:14.000000 integerbook-0.0.3/README.md
--rw-r--r--   0 jvo        (501) staff       (20)      645 2023-04-23 23:24:26.000000 integerbook-0.0.3/pyproject.toml
--rw-r--r--   0 jvo        (501) staff       (20)       38 2023-04-23 23:25:48.789609 integerbook-0.0.3/setup.cfg
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.692858 integerbook-0.0.3/src/
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.710028 integerbook-0.0.3/src/integerbook/
--rw-r--r--   0 jvo        (501) staff       (20)     2475 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/CanvasCreator.py
--rw-r--r--   0 jvo        (501) staff       (20)     5918 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/LocationFinder.py
--rw-r--r--   0 jvo        (501) staff       (20)    10154 2023-04-23 23:09:59.000000 integerbook-0.0.3/src/integerbook/Settings.py
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)     1186 2023-04-23 18:31:12.000000 integerbook-0.0.3/src/integerbook/alternativeSymbols.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.723699 integerbook-0.0.3/src/integerbook/auxiliary_scripts/
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)      756 2023-04-23 22:57:26.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/changeNameMxl.py
--rw-r--r--   0 jvo        (501) staff       (20)     6139 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/chordTypes.py
--rw-r--r--   0 jvo        (501) staff       (20)      680 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/createBatchJson.py
--rw-r--r--   0 jvo        (501) staff       (20)      173 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/printSettings.py
--rw-r--r--   0 jvo        (501) staff       (20)     1619 2023-04-23 21:43:41.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/runMultiple.py
--rw-r--r--   0 jvo        (501) staff       (20)     3588 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/separateRealbook.py
--rw-r--r--   0 jvo        (501) staff       (20)      537 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/setMode.py
--rw-r--r--   0 jvo        (501) staff       (20)     1855 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/setModes.py
--rw-r--r--   0 jvo        (501) staff       (20)     1544 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/writeTexFile.py
--rw-r--r--   0 jvo        (501) staff       (20)      709 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/fontDimensions.json
--rw-r--r--   0 jvo        (501) staff       (20)     1485 2023-04-23 19:15:02.000000 integerbook-0.0.3/src/integerbook/fontSettings.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.724714 integerbook-0.0.3/src/integerbook/fonts/
--rw-r--r--   0 jvo        (501) staff       (20)     6148 2023-04-02 10:13:05.000000 integerbook-0.0.3/src/integerbook/fonts/.DS_Store
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.725621 integerbook-0.0.3/src/integerbook/fonts/Realbook/
--rw-r--r--   0 jvo        (501) staff       (20)    66232 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/fonts/Realbook/Realbook.ttf
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.728002 integerbook-0.0.3/src/integerbook/fonts/symbola/
--rw-r--r--   0 jvo        (501) staff       (20)  2240100 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/fonts/symbola/Symbola.ttf
--rw-r--r--   0 jvo        (501) staff       (20)     2093 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/main.py
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.782059 integerbook-0.0.3/src/integerbook/plotter/
--rw-r--r--   0 jvo        (501) staff       (20)    13336 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterBarLines.py
--rw-r--r--   0 jvo        (501) staff       (20)     1741 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterBase.py
--rw-r--r--   0 jvo        (501) staff       (20)    14571 2023-04-23 23:16:48.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterChords.py
--rw-r--r--   0 jvo        (501) staff       (20)     1367 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterMain.py
--rw-r--r--   0 jvo        (501) staff       (20)     3121 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterMetadata.py
--rw-r--r--   0 jvo        (501) staff       (20)    23638 2023-04-23 21:51:35.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterNotes.py
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)    10373 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/patches.py
--rw-r--r--   0 jvo        (501) staff       (20)    10593 2023-04-23 21:46:46.000000 integerbook-0.0.3/src/integerbook/runSingle.py
--rw-r--r--   0 jvo        (501) staff       (20)     1580 2023-04-23 23:09:59.000000 integerbook-0.0.3/src/integerbook/settings.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.713530 integerbook-0.0.3/src/integerbook.egg-info/
--rw-r--r--   0 jvo        (501) staff       (20)    42511 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/PKG-INFO
--rw-r--r--   0 jvo        (501) staff       (20)     1481 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/SOURCES.txt
--rw-r--r--   0 jvo        (501) staff       (20)        1 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/dependency_links.txt
--rw-r--r--   0 jvo        (501) staff       (20)       11 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/requires.txt
--rw-r--r--   0 jvo        (501) staff       (20)       12 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/top_level.txt
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.567088 integerbook-0.0.4/
+-rw-r--r--   0 jvo        (501) staff       (20)    35149 2022-03-18 13:05:53.000000 integerbook-0.0.4/LICENSE
+-rw-r--r--   0 jvo        (501) staff       (20)       84 2023-04-23 18:25:14.000000 integerbook-0.0.4/MANIFEST.in
+-rw-r--r--   0 jvo        (501) staff       (20)    42574 2023-05-23 09:37:16.566606 integerbook-0.0.4/PKG-INFO
+-rw-r--r--   0 jvo        (501) staff       (20)     1560 2023-04-25 14:48:32.000000 integerbook-0.0.4/README.md
+-rw-r--r--   0 jvo        (501) staff       (20)      645 2023-05-23 09:36:25.000000 integerbook-0.0.4/pyproject.toml
+-rw-r--r--   0 jvo        (501) staff       (20)       38 2023-05-23 09:37:16.567221 integerbook-0.0.4/setup.cfg
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.515746 integerbook-0.0.4/src/
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.526429 integerbook-0.0.4/src/integerbook/
+-rw-r--r--   0 jvo        (501) staff       (20)     2475 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/CanvasCreator.py
+-rw-r--r--   0 jvo        (501) staff       (20)     5918 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/LocationFinder.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10279 2023-04-29 18:03:24.000000 integerbook-0.0.4/src/integerbook/Settings.py
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1186 2023-04-23 18:31:12.000000 integerbook-0.0.4/src/integerbook/alternativeSymbols.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.539505 integerbook-0.0.4/src/integerbook/auxiliary_scripts/
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)      756 2023-04-23 22:57:26.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/changeNameMxl.py
+-rw-r--r--   0 jvo        (501) staff       (20)     6139 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/chordTypes.py
+-rw-r--r--   0 jvo        (501) staff       (20)      680 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/createBatchJson.py
+-rw-r--r--   0 jvo        (501) staff       (20)      173 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/printSettings.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1619 2023-04-23 21:43:41.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/runMultiple.py
+-rw-r--r--   0 jvo        (501) staff       (20)     3588 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/separateRealbook.py
+-rw-r--r--   0 jvo        (501) staff       (20)      537 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/setMode.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1855 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/setModes.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1544 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/auxiliary_scripts/writeTexFile.py
+-rw-r--r--   0 jvo        (501) staff       (20)      709 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/fontDimensions.json
+-rw-r--r--   0 jvo        (501) staff       (20)     1735 2023-04-29 18:11:08.000000 integerbook-0.0.4/src/integerbook/fontSettings.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.540311 integerbook-0.0.4/src/integerbook/fonts/
+-rw-r--r--   0 jvo        (501) staff       (20)     6148 2023-04-02 10:13:05.000000 integerbook-0.0.4/src/integerbook/fonts/.DS_Store
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.541276 integerbook-0.0.4/src/integerbook/fonts/Realbook/
+-rw-r--r--   0 jvo        (501) staff       (20)    66232 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/fonts/Realbook/Realbook.ttf
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.542904 integerbook-0.0.4/src/integerbook/fonts/symbola/
+-rw-r--r--   0 jvo        (501) staff       (20)  2240100 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/fonts/symbola/Symbola.ttf
+-rw-r--r--   0 jvo        (501) staff       (20)     2818 2023-05-22 13:36:25.000000 integerbook-0.0.4/src/integerbook/main.py
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.564925 integerbook-0.0.4/src/integerbook/plotter/
+-rw-r--r--   0 jvo        (501) staff       (20)    13336 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/plotter/PlotterBarLines.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1741 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/plotter/PlotterBase.py
+-rw-r--r--   0 jvo        (501) staff       (20)    14658 2023-04-29 17:50:17.000000 integerbook-0.0.4/src/integerbook/plotter/PlotterChords.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1367 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/plotter/PlotterMain.py
+-rw-r--r--   0 jvo        (501) staff       (20)     3121 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/plotter/PlotterMetadata.py
+-rw-r--r--   0 jvo        (501) staff       (20)    23638 2023-04-23 21:51:35.000000 integerbook-0.0.4/src/integerbook/plotter/PlotterNotes.py
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/plotter/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10373 2023-04-23 18:25:14.000000 integerbook-0.0.4/src/integerbook/plotter/patches.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10732 2023-05-22 13:44:16.000000 integerbook-0.0.4/src/integerbook/runSingle.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1580 2023-04-23 23:09:59.000000 integerbook-0.0.4/src/integerbook/settings.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 09:37:16.529335 integerbook-0.0.4/src/integerbook.egg-info/
+-rw-r--r--   0 jvo        (501) staff       (20)    42574 2023-05-23 09:37:16.000000 integerbook-0.0.4/src/integerbook.egg-info/PKG-INFO
+-rw-r--r--   0 jvo        (501) staff       (20)     1481 2023-05-23 09:37:16.000000 integerbook-0.0.4/src/integerbook.egg-info/SOURCES.txt
+-rw-r--r--   0 jvo        (501) staff       (20)        1 2023-05-23 09:37:16.000000 integerbook-0.0.4/src/integerbook.egg-info/dependency_links.txt
+-rw-r--r--   0 jvo        (501) staff       (20)       11 2023-05-23 09:37:16.000000 integerbook-0.0.4/src/integerbook.egg-info/requires.txt
+-rw-r--r--   0 jvo        (501) staff       (20)       12 2023-05-23 09:37:16.000000 integerbook-0.0.4/src/integerbook.egg-info/top_level.txt
```

### Comparing `integerbook-0.0.3/LICENSE` & `integerbook-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/PKG-INFO` & `integerbook-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integerbook
-Version: 0.0.3
+Version: 0.0.4
 Summary: sheet music converter
 Author-email: Jesse van Oostrum <integerbook@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,29 +691,29 @@
 
 This library converts sheet music in musicxml format to visualisations that refer to notes and chords with their relative position within the key of the song. More about how this notational system works [here](https://integerbook.com/about). 
 
 ### installation
 
 1. Download python
 2. install the [integerbook package](https://pypi.org/project/integerbook/0.0.2/) using pip: ``` $ pip install integerbook ```
-3. Download or copy the file ```run.py``` from the repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
+3. Download or copy the file ```run.py``` from the github repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
 
 
 ### running the code
-1. In the terminal, navigate to the folder where ```run.py``` is stored. 
+1. In the terminal, navigate to the folder where ```run.py``` is stored, e.g. ```~/Documents/music-visualisation```. 
 2. In the terminal, type: ``` $ python run.py -s <path-to-song>```  e.g.   
 ``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" ```
 
 This will convert the musicxml file you specified to a pdf and store it in the current folder. 
 
 Further options include:
 - -o set output directory  (without "/" at the end)
 - -b for bassline output
 - -l for printing lyrics
 - -c for colouring notes according to circle of fifths
 - -cn for printing chord notes
 - -cp for printing chord progressions (no melody, 8 measures per line)
-- -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See 'sample/settings.json' for the default settings.
+- -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See ```src/integerbok/settings.json``` for the default settings.
 
 
 ### example musicxml files
 In the folder example, there are some musicxml files that can be used to try out the program.
```

### Comparing `integerbook-0.0.3/README.md` & `integerbook-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 This library converts sheet music in musicxml format to visualisations that refer to notes and chords with their relative position within the key of the song. More about how this notational system works [here](https://integerbook.com/about). 
 
 ### installation
 
 1. Download python
 2. install the [integerbook package](https://pypi.org/project/integerbook/0.0.2/) using pip: ``` $ pip install integerbook ```
-3. Download or copy the file ```run.py``` from the repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
+3. Download or copy the file ```run.py``` from the github repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
 
 
 ### running the code
-1. In the terminal, navigate to the folder where ```run.py``` is stored. 
+1. In the terminal, navigate to the folder where ```run.py``` is stored, e.g. ```~/Documents/music-visualisation```. 
 2. In the terminal, type: ``` $ python run.py -s <path-to-song>```  e.g.   
 ``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" ```
 
 This will convert the musicxml file you specified to a pdf and store it in the current folder. 
 
 Further options include:
 - -o set output directory  (without "/" at the end)
 - -b for bassline output
 - -l for printing lyrics
 - -c for colouring notes according to circle of fifths
 - -cn for printing chord notes
 - -cp for printing chord progressions (no melody, 8 measures per line)
-- -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See 'sample/settings.json' for the default settings.
+- -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See ```src/integerbok/settings.json``` for the default settings.
 
 
 ### example musicxml files
 In the folder example, there are some musicxml files that can be used to try out the program.
```

### Comparing `integerbook-0.0.3/pyproject.toml` & `integerbook-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integerbook"
-version = "0.0.3"
+version = "0.0.4"
 description = "sheet music converter"
 readme = "README.md"
 authors = [{ name = "Jesse van Oostrum", email = "integerbook@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `integerbook-0.0.3/src/integerbook/CanvasCreator.py` & `integerbook-0.0.4/src/integerbook/CanvasCreator.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/LocationFinder.py` & `integerbook-0.0.4/src/integerbook/LocationFinder.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/Settings.py` & `integerbook-0.0.4/src/integerbook/Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,13 +234,15 @@
             fontSettings = fontSettings['DejaVu Sans']
             print("no fontsettings available")
 
 
         self.widthCharacter = fontSettings['widthCharacterRelative'] * fontSizeType
         self.widthMinus = fontSettings['widthMinusRelative'] * fontSizeType
         self.accidentalSpace = fontSettings['accidentalSpaceRelative'] * fontSizeType
-        self.accidentalSizeRelative = fontSettings["accidentalSizeRelativeRelative"] * fontSizeType
+        self.accidentalSizeRelative = fontSettings["accidentalSizeRelative"]
         self.widthDelta = fontSettings["widthDeltaRelative"] * fontSizeType
         self.widthCircle = fontSettings["widthCircleRelative"] * fontSizeType
         self.spaceAddSus = fontSettings["spaceAddSusRelative"] * fontSizeType
-        self.accidentalXPositionRelative = fontSettings["accidentalXPositionRelativeRelative"] * fontSizeType
+        self.accidentalXPositionRelative = fontSettings["accidentalXPositionRelative"]
         self.hDistanceChordAddition = fontSettings['hDistanceChordAdditionRelative'] * fontSizeType
+        self.positionSlashRelative = fontSettings["positionSlashRelative"]
+        self.widthAccidentalSlash = fontSettings["widthAccidentalSlashRelative"] * fontSizeType
```

### Comparing `integerbook-0.0.3/src/integerbook/alternativeSymbols.json` & `integerbook-0.0.4/src/integerbook/alternativeSymbols.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/changeNameMxl.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/changeNameMxl.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/chordTypes.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/chordTypes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/createBatchJson.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/createBatchJson.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/runMultiple.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/runMultiple.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/separateRealbook.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/separateRealbook.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/setMode.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/setMode.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/setModes.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/setModes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/auxiliary_scripts/writeTexFile.py` & `integerbook-0.0.4/src/integerbook/auxiliary_scripts/writeTexFile.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/fontDimensions.json` & `integerbook-0.0.4/src/integerbook/fontDimensions.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/fontSettings.json` & `integerbook-0.0.4/src/integerbook/fontSettings.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7800480769230769%*

 * *Differences: {"'DejaVu Sans'": "{'accidentalSizeRelative': 0.8, 'accidentalXPositionRelative': 0.13, "*

 * *                  "'positionSlashRelative': 1, 'widthAccidentalSlashRelative': 0.0004, delete: "*

 * *                  "['accidentalSizeRelativeRelative', 'accidentalXPositionRelativeRelative']}",*

 * * "'Humor Sans'": "{'accidentalSizeRelative': 1, 'accidentalXPositionRelative': 0.3, "*

 * *                 "'positionSlashRelative': 0.8, 'widthAccidentalSlashRelative': 0.00072, delete: "*

 * *                 "['accidentalSizeRelativeRe […]*

```diff
@@ -1,46 +1,54 @@
 {
     "DejaVu Sans": {
-        "accidentalSizeRelativeRelative": 0.1,
+        "accidentalSizeRelative": 0.8,
         "accidentalSpaceRelative": 0.0007,
-        "accidentalXPositionRelativeRelative": 0.02,
+        "accidentalXPositionRelative": 0.13,
         "hDistanceChordAdditionRelative": -0.0001,
+        "positionSlashRelative": 1,
         "spaceAddSusRelative": 0.0025,
+        "widthAccidentalSlashRelative": 0.0004,
         "widthCharacterRelative": 0.001,
         "widthCircleRelative": 0.001,
         "widthDeltaRelative": 0.0013,
         "widthMinusRelative": 0.0005
     },
     "Humor Sans": {
-        "accidentalSizeRelativeRelative": 0.1,
+        "accidentalSizeRelative": 1,
         "accidentalSpaceRelative": 0.0007,
-        "accidentalXPositionRelativeRelative": 0.03,
+        "accidentalXPositionRelative": 0.3,
         "hDistanceChordAdditionRelative": 0.0001,
+        "positionSlashRelative": 0.8,
         "spaceAddSusRelative": 0.0025,
+        "widthAccidentalSlashRelative": 0.00072,
         "widthCharacterRelative": 0.001,
         "widthCircleRelative": 0.001,
         "widthDeltaRelative": 0.0013,
         "widthMinusRelative": 0.0005
     },
     "Realbook": {
-        "accidentalSizeRelativeRelative": 0.1,
+        "accidentalSizeRelative": 1,
         "accidentalSpaceRelative": 0.0004,
-        "accidentalXPositionRelativeRelative": 0.01,
+        "accidentalXPositionRelative": 0.1,
         "hDistanceChordAdditionRelative": -6e-05,
+        "positionSlashRelative": 0.8,
         "spaceAddSusRelative": 0.002,
+        "widthAccidentalSlashRelative": 0.00072,
         "widthCharacterRelative": 0.0008,
         "widthCircleRelative": 0.001,
         "widthDeltaRelative": 0.0013,
         "widthMinusRelative": 0.0005
     },
     "Vulf Mono": {
-        "accidentalSizeRelativeRelative": 0.07,
+        "accidentalSizeRelative": 0.6,
         "accidentalSpaceRelative": 0.001,
-        "accidentalXPositionRelative": 0.03,
+        "accidentalXPositionRelative": 0.3,
         "hDistanceChordAdditionRelative": -0.0001,
+        "positionSlashRelative": 0.8,
         "spaceAddSusRelative": 0.003,
+        "widthAccidentalSlashRelative": 0.0006,
         "widthCharacterRelative": 0.001,
         "widthCircleRelative": 0.001,
         "widthDeltaRelative": 0.001,
         "widthMinusRelative": 0.001
     }
 }
```

### Comparing `integerbook-0.0.3/src/integerbook/fonts/.DS_Store` & `integerbook-0.0.4/src/integerbook/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/fonts/Realbook/Realbook.ttf` & `integerbook-0.0.4/src/integerbook/fonts/Realbook/Realbook.ttf`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/fonts/symbola/Symbola.ttf` & `integerbook-0.0.4/src/integerbook/fonts/symbola/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/main.py` & `integerbook-0.0.4/src/integerbook/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             else:
                 pathName = dirName + '/' + title + '.pdf'
             self.CanvasCreator.saveFig(pathName)
 
     def _preprocessStreamObj(self, streamObj):
 
         streamObj = self._removeBassStaff(streamObj)
+        streamObj = self._correctPickupMeasure(streamObj)
 
         return streamObj
 
     def _removeBassStaff(self, streamObj):
         staffs = streamObj[music21.stream.PartStaff]
         if staffs:
             if len(staffs) > 1:
@@ -58,13 +59,36 @@
         if parts:
             if len (parts) > 1:
                 streamObj.remove(parts[1:])
                 print("removed part(s)")
 
         return streamObj
 
+    def _correctPickupMeasure(self, streamObj):
+        measures = streamObj[music21.stream.Measure]
+        if measures[0].number == 1:
+            if measures[0].quarterLength < measures[1].quarterLength:
+                streamObj = self._renumberMeasures(streamObj)
+        return streamObj
+
+    def _renumberMeasures(self, streamObj):
+        measures = streamObj[music21.stream.Measure]
+        for i in range(len(measures)):
+            measures[i].number = i
+        return streamObj
+
 
 if __name__ == '__main__':
-    pathToSong = "../../example/All_Of_Me.mxl"
+    import tracemalloc
+    pathToSong = "../../example/All_Of_Me.musicxml"
+
+    tracemalloc.start()
 
     vis = Visualiser(pathToSong)
 
+    vis.saveFig("/Users/jvo/Downloads/outputIBApp")
+
+    print(tracemalloc.get_traced_memory())
+
+    tracemalloc.stop()
+
+
```

### Comparing `integerbook-0.0.3/src/integerbook/plotter/PlotterBarLines.py` & `integerbook-0.0.4/src/integerbook/plotter/PlotterBarLines.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/plotter/PlotterBase.py` & `integerbook-0.0.4/src/integerbook/plotter/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/plotter/PlotterChords.py` & `integerbook-0.0.4/src/integerbook/plotter/PlotterChords.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,25 +335,25 @@
 
                 key = self.Settings.getKey(chordSymbol.getOffsetInHierarchy(self.streamObj))
 
                 pitch = chordSymbol.bass()
                 number, accidental = key.getScaleDegreeAndAccidentalFromPitch(pitch)
 
                 # plot slash
-                xPosRightOfChord = xPos + 0.8 * self.Settings.widthNumberRelative * self.Settings.fontSizeChords
+                xPosRightOfChord = xPos + self.Settings.fontSettings.positionSlashRelative * self.Settings.widthNumberRelative * self.Settings.fontSizeChords
                 yPosSlash = yPos - .4 * fontSizeAddition * self.Settings.capsizeNumberRelative
 
                 self.axs[page].text(xPosRightOfChord, yPosSlash, '/', fontsize=fontSizeAddition,
                                     va='baseline', ha='left')
 
                 # plot number
                 xPosRightOfSlash = xPosRightOfChord + 0.8 * self.Settings.widthNumberRelative * fontSizeAddition
                 xPosBass = xPosRightOfSlash
                 if accidental:
-                    xPosBass += 0.006
+                    xPosBass += self.Settings.fontSettings.widthAccidentalSlash
 
                 yPosBass = yPosSlash - 0.25 * fontSizeAddition * self.Settings.capsizeNumberRelative
 
                 self.axs[page].text(xPosBass, yPosBass, number, fontsize=fontSizeAddition,
                                     va='baseline', ha='left')
 
                 # plot accidental
```

### Comparing `integerbook-0.0.3/src/integerbook/plotter/PlotterMain.py` & `integerbook-0.0.4/src/integerbook/plotter/PlotterMain.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/plotter/PlotterMetadata.py` & `integerbook-0.0.4/src/integerbook/plotter/PlotterMetadata.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/plotter/PlotterNotes.py` & `integerbook-0.0.4/src/integerbook/plotter/PlotterNotes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/plotter/patches.py` & `integerbook-0.0.4/src/integerbook/plotter/patches.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook/runSingle.py` & `integerbook-0.0.4/src/integerbook/runSingle.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 song3 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/wikifonia_edited/Burt Bacharach, Hal David - I Say A Little Prayer.mxl"
 song4 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/test-files/timeSignature-repeatExpression.mxl"
 song5 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/standards_musescore/I_Dont_Want_To_Set_The_World_On_Fire.mxl"
 song6 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/standards_musescore/I_Wish_You_Love.mxl"
 song7 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/bass_lines_SBL/Papa Was a Rollin' Stoneb.mxl"
 song8 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/easy songs/Silent_Night.mxl"
 song9 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/musescore/logo.mxl"
-song10 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/test-files/slash-chord.mxl"
+song10 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/test-files/slash-chords.musicxml"
 song11 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/bass_lines_SBL/December 1963.mxl"
 song12 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/easy songs/Twinkle_twinkle_little_star.mxl"
 song13 = "/usr/local/Caskroom/miniconda/base/envs/music/lib/python3.9/site-packages/music21/musicxml/lilypondTestSuite/24a-GraceNotes.xml"
 song14 = "/Users/jvo/Documents/music-visualisation/testfiles/gracenotes4.musicxml"
 song15 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/test-files/hammer-on2.musicxml"
 song16 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/standards_musescore/Bags_Groove.mxl"
 song17 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/pop/Yellow.mxl"
@@ -80,55 +80,58 @@
 song74 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/ultimate-guitar-top-100/2021 -- HALLELUJAH RJS mods.mscz"
 song75 = "/Users/jvo/Downloads/tempMxl/2021 -- HALLELUJAH RJS mods.musicxml"
 song76 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/musescore/Think_About_Things_-_Iceland_Eurovision_2020_-_Dai_Freyr-Part.mscz"
 song77 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/All_Of_Me.musicxml"
 song78 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/All_Of_Me-different-key.musicxml"
 song79 = "/Users/jvo/Downloads/favicon.musicxml"
 song80 = '/Users/jvo/Downloads/DickSchmittMxl/2020 --  Home, Sweet Home RJSReformat.musicxml'
+song81 = '/Users/jvo/Downloads/DickSchmittMxl/2022 -- Back Home Again in Indiana RJSMods.musicxml'
 
 settings = {}
-settings["measuresPerLine"] = 8
+settings["measuresPerLine"] = 4
 settings["subdivision"] = 0
+settings["fontSizeNotes"] = 10
 settings["setInMajorKey"] = True
 settings["lyrics"] = False
 settings['coloursVoices'] = False
 settings['coloursCircleOfFifths'] = False
 settings['thickBarlines'] = True
 settings['plotTimeSignature'] = True
 settings['printArranger'] = False
 settings['saveCropped'] = True
 settings['alpha'] = 0.2
 settings['xkcd'] = False
 
-settings['overlapFactor'] = 0
-settings["plotChordTones"] = True
-settings["plotMelody"] = False
+settings['overlapFactor'] = 0.5
+settings["plotChordTones"] = False
+settings["plotMelody"] = True
 
 # settings["usePlt"] = True
 
 # settings["alternativeSymbols"] = "SBJ"
 # settings["fontSizeNotes"] = 7
 
 
 # Settings['font'] = 'Sathu'
 # Settings['font'] = 'STIXGeneral'
 # Settings['fontStyle'] = 'italic'
 
+
 # settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Vulf Mono/Vulf Mono/Desktop"
 # settings['fontStyle'] = 'italic'
 # settings['fontWeight'] = 'light'
 # settings['font'] = 'Vulf Mono'
 
 # Settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Realbook"
 # Settings['font'] = 'Realbook'
 
 # settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Humor Sans"
 # settings['font'] = 'Humor Sans'
 
-song = song77
+song = song81
 
 if song[-5:] == ".mscz":
 
     dirSongsMxl = "/Users/jvo/Downloads/tempMxl"
     filename = os.path.basename(song).split("/")[-1]
     outputName = os.path.splitext(filename)[0] + '.musicxml'
```

### Comparing `integerbook-0.0.3/src/integerbook/settings.json` & `integerbook-0.0.4/src/integerbook/settings.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.3/src/integerbook.egg-info/PKG-INFO` & `integerbook-0.0.4/src/integerbook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integerbook
-Version: 0.0.3
+Version: 0.0.4
 Summary: sheet music converter
 Author-email: Jesse van Oostrum <integerbook@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,29 +691,29 @@
 
 This library converts sheet music in musicxml format to visualisations that refer to notes and chords with their relative position within the key of the song. More about how this notational system works [here](https://integerbook.com/about). 
 
 ### installation
 
 1. Download python
 2. install the [integerbook package](https://pypi.org/project/integerbook/0.0.2/) using pip: ``` $ pip install integerbook ```
-3. Download or copy the file ```run.py``` from the repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
+3. Download or copy the file ```run.py``` from the github repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
 
 
 ### running the code
-1. In the terminal, navigate to the folder where ```run.py``` is stored. 
+1. In the terminal, navigate to the folder where ```run.py``` is stored, e.g. ```~/Documents/music-visualisation```. 
 2. In the terminal, type: ``` $ python run.py -s <path-to-song>```  e.g.   
 ``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" ```
 
 This will convert the musicxml file you specified to a pdf and store it in the current folder. 
 
 Further options include:
 - -o set output directory  (without "/" at the end)
 - -b for bassline output
 - -l for printing lyrics
 - -c for colouring notes according to circle of fifths
 - -cn for printing chord notes
 - -cp for printing chord progressions (no melody, 8 measures per line)
-- -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See 'sample/settings.json' for the default settings.
+- -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See ```src/integerbok/settings.json``` for the default settings.
 
 
 ### example musicxml files
 In the folder example, there are some musicxml files that can be used to try out the program.
```

### Comparing `integerbook-0.0.3/src/integerbook.egg-info/SOURCES.txt` & `integerbook-0.0.4/src/integerbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

