# Comparing `tmp/musicntwrk-2.2.8.tar.gz` & `tmp/musicntwrk-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/musicntwrk-2.2.8.tar", last modified: Fri Nov 19 22:22:56 2021, max compression
+gzip compressed data, was "dist/musicntwrk-2.2.9.tar", last modified: Mon Nov 22 17:40:00 2021, max compression
```

## Comparing `musicntwrk-2.2.8.tar` & `musicntwrk-2.2.9.tar`

### file list

```diff
@@ -1,158 +1,160 @@
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.772536 musicntwrk-2.2.8/
--rw-r--r--   0 marco      (502) staff       (20)     8042 2021-11-19 22:22:56.772185 musicntwrk-2.2.8/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     6875 2021-08-07 16:52:58.000000 musicntwrk-2.2.8/README.md
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.673531 musicntwrk-2.2.8/musicntwrk.egg-info/
--rw-r--r--   0 marco      (502) staff       (20)     8042 2021-11-19 22:22:56.000000 musicntwrk-2.2.8/musicntwrk.egg-info/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     4093 2021-11-19 22:22:56.000000 musicntwrk-2.2.8/musicntwrk.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (502) staff       (20)        1 2021-11-19 22:22:56.000000 musicntwrk-2.2.8/musicntwrk.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (502) staff       (20)      159 2021-11-19 22:22:56.000000 musicntwrk-2.2.8/musicntwrk.egg-info/requires.txt
--rw-r--r--   0 marco      (502) staff       (20)       11 2021-11-19 22:22:56.000000 musicntwrk-2.2.8/musicntwrk.egg-info/top_level.txt
--rw-r--r--   0 marco      (502) staff       (20)       38 2021-11-19 22:22:56.772662 musicntwrk-2.2.8/setup.cfg
--rw-r--r--   0 marco      (502) staff       (20)     1398 2021-11-19 22:21:40.000000 musicntwrk-2.2.8/setup.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.674546 musicntwrk-2.2.8/src/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/__init__.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.676848 musicntwrk-2.2.8/src/comptools/
--rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.2.8/src/comptools/MidiFile.py
--rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.2.8/src/comptools/genmidi.py
--rw-r--r--   0 marco      (502) staff       (20)     7760 2021-09-26 20:51:51.000000 musicntwrk-2.2.8/src/comptools/music.py
--rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.2.8/src/comptools/notation.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.687606 musicntwrk-2.2.8/src/data/
--rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/MIDImap.py
--rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/MIDImidi.py
--rw-r--r--   0 marco      (502) staff       (20)      915 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/MIDIscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/WRITEscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/WRITEscoreNoTime.py
--rw-r--r--   0 marco      (502) staff       (20)     1985 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/WRITEscoreOps.py
--rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.2.8/src/data/WRITEscoreOpsMIDI.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2919 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/analyzeSound.py
--rw-r--r--   0 marco      (502) staff       (20)     3947 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/analyzeTimbre.py
--rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/ctcsound.py
--rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/i_spectral.py
--rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/i_spectral2.py
--rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/i_spectral_pure.py
--rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/i_spectral_pyo.py
--rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/i_time_series.py
--rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/r_1Ddata.py
--rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/data/scaleMapping.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.705788 musicntwrk-2.2.8/src/harmony/
--rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/applyOps.py
--rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/changePoint.py
--rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/chinese_postman.py
--rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/enharmonicDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/getRN.py
--rw-r--r--   0 marco      (502) staff       (20)     4084 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/harmonicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     2364 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/keySections.py
--rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/lookupOps.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/lookupProgr.py
--rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/lookupWrapper.py
--rw-r--r--   0 marco      (502) staff       (20)     2348 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/networkHarmonyGen.py
--rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/plotHarmonicTable.py
--rw-r--r--   0 marco      (502) staff       (20)     2752 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/rhythmicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/scoreAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/scoreDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/scoreFilter.py
--rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/shortHands.py
--rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/showAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     4352 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/spiralChordSpace.py
--rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/tonalAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     7684 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/tonalHarmonyCalculator.py
--rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/tonalHarmonyModels.py
--rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/tonalPartition.py
--rw-r--r--   0 marco      (502) staff       (20)     2411 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/harmony/tonnentz.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.712547 musicntwrk-2.2.8/src/ml_utils/
--rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2690 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/checkRun.py
--rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/modelDump.py
--rw-r--r--   0 marco      (502) staff       (20)     1473 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/modelLoad.py
--rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/multiModelPredictor.py
--rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/prepareDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     2014 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/readModels.py
--rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/scaleDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     3227 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/trainCNNmodel.py
--rw-r--r--   0 marco      (502) staff       (20)     2213 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/ml_utils/trainNNmodel.py
--rw-r--r--   0 marco      (502) staff       (20)    68768 2021-11-15 16:16:23.000000 musicntwrk-2.2.8/src/musicntwrk.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.728701 musicntwrk-2.2.8/src/networks/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2577 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/orchestralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2375 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/orchestralVector.py
--rw-r--r--   0 marco      (502) staff       (20)     1636 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/orchestralVectorColor.py
--rw-r--r--   0 marco      (502) staff       (20)     4780 2021-11-11 23:43:00.000000 musicntwrk-2.2.8/src/networks/pcsDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5760 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/pcsEgoNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4822 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/pcsNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2920 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/rLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/readScore.py
--rw-r--r--   0 marco      (502) staff       (20)     3321 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/rhythmDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     4253 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/rhythmNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4186 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/rhythmPDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/scoreDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/scoreMIDIDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5142 2021-11-19 01:24:07.000000 musicntwrk-2.2.8/src/networks/scoreNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     5367 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/scoreSubNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     3680 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/timbralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4033 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/vLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4553 2021-11-19 16:56:36.000000 musicntwrk-2.2.8/src/networks/vLeadNetworkByName.py
--rw-r--r--   0 marco      (502) staff       (20)     2890 2021-11-12 19:23:59.000000 musicntwrk-2.2.8/src/networks/vLeadNetworkByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)     2588 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/networks/vLeadNetworkVec.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.735170 musicntwrk-2.2.8/src/plotting/
--rw-r--r--   0 marco      (502) staff       (20)     1061 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/barplot.py
--rw-r--r--   0 marco      (502) staff       (20)    25524 2021-10-28 22:26:22.000000 musicntwrk-2.2.8/src/plotting/chordspace.py
--rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/drawMultiLayerNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2811 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/drawNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/drawNetworkX.py
--rw-r--r--   0 marco      (502) staff       (20)      890 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/plotCC.py
--rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/plotCurveXY.py
--rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/plotCurveY.py
--rw-r--r--   0 marco      (502) staff       (20)     1864 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/plotting/plotOpsHistogram.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.745867 musicntwrk-2.2.8/src/timbre/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1550 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeCompMPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1661 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2646 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeModifiedASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computePSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2261 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeStandardizedMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1769 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeStandardizedMFPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1928 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/computeStandardizedPSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/mfccSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/mfccSoundDecayOptimal.py
--rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/mfccSoundDecayPiecewise.py
--rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/minimizeBKPT.py
--rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/normSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/timbre/normSoundDecay2.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-19 22:22:56.771358 musicntwrk-2.2.8/src/utils/
--rw-r--r--   0 marco      (502) staff       (20)      737 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/Remove.py
--rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/SegmentedLinearReg.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/Sublists.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/communications.py
--rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/diffusionEntropyAnalyis.py
--rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/diffusionEntropyAnalyisNew.py
--rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/entropyKLdiv.py
--rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/extractByString.py
--rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/fetchWaves.py
--rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/findLengthMax.py
--rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/flatten.py
--rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/floatize.py
--rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/generalizedOpsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1541 2021-11-19 01:21:35.000000 musicntwrk-2.2.8/src/utils/generalizedOpsName.py
--rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/init_list_of_objects.py
--rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/load_balancing.py
--rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/minimalDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/minimalDistanceVec.py
--rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/minimalNoBijDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.2.8/src/utils/opsCheckByName.py
--rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/opsCheckByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/opsDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/opsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:47.000000 musicntwrk-2.2.8/src/utils/opsName.py
--rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.2.8/src/utils/opsNameFull.py
--rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/opsNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/play_with_simpleaudio.py
--rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/powerFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/rhythmDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.2.8/src/utils/scaleFreeFit.py
--rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/str2float.py
--rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/str2frac.py
--rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.2.8/src/utils/vectorDistance.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.494081 musicntwrk-2.2.9/
+-rw-r--r--   0 marco      (502) staff       (20)     8042 2021-11-22 17:40:00.493583 musicntwrk-2.2.9/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     6875 2021-08-07 16:52:58.000000 musicntwrk-2.2.9/README.md
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.398421 musicntwrk-2.2.9/musicntwrk.egg-info/
+-rw-r--r--   0 marco      (502) staff       (20)     8042 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     4149 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (502) staff       (20)        1 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (502) staff       (20)      159 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/requires.txt
+-rw-r--r--   0 marco      (502) staff       (20)       11 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/top_level.txt
+-rw-r--r--   0 marco      (502) staff       (20)       38 2021-11-22 17:40:00.494254 musicntwrk-2.2.9/setup.cfg
+-rw-r--r--   0 marco      (502) staff       (20)     1398 2021-11-22 17:38:55.000000 musicntwrk-2.2.9/setup.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.399381 musicntwrk-2.2.9/src/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/__init__.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.402073 musicntwrk-2.2.9/src/comptools/
+-rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.2.9/src/comptools/MidiFile.py
+-rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.2.9/src/comptools/genmidi.py
+-rw-r--r--   0 marco      (502) staff       (20)     7760 2021-09-26 20:51:51.000000 musicntwrk-2.2.9/src/comptools/music.py
+-rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.2.9/src/comptools/notation.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.413246 musicntwrk-2.2.9/src/data/
+-rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/MIDImap.py
+-rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/MIDImidi.py
+-rw-r--r--   0 marco      (502) staff       (20)      915 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/MIDIscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/WRITEscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/WRITEscoreNoTime.py
+-rw-r--r--   0 marco      (502) staff       (20)     1985 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/WRITEscoreOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.2.9/src/data/WRITEscoreOpsMIDI.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2919 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/analyzeSound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3947 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/analyzeTimbre.py
+-rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/ctcsound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral.py
+-rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral2.py
+-rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral_pure.py
+-rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral_pyo.py
+-rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_time_series.py
+-rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/r_1Ddata.py
+-rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/scaleMapping.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.428003 musicntwrk-2.2.9/src/harmony/
+-rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/applyOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/changePoint.py
+-rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/chinese_postman.py
+-rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/enharmonicDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/getRN.py
+-rw-r--r--   0 marco      (502) staff       (20)     4084 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/harmonicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     2364 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/keySections.py
+-rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/lookupOps.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/lookupProgr.py
+-rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/lookupWrapper.py
+-rw-r--r--   0 marco      (502) staff       (20)     2348 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/networkHarmonyGen.py
+-rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/plotHarmonicTable.py
+-rw-r--r--   0 marco      (502) staff       (20)     2752 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/rhythmicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/scoreAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/scoreDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/scoreFilter.py
+-rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/shortHands.py
+-rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/showAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     4352 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/spiralChordSpace.py
+-rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     7684 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalHarmonyCalculator.py
+-rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalHarmonyModels.py
+-rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalPartition.py
+-rw-r--r--   0 marco      (502) staff       (20)     2411 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonnentz.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.433596 musicntwrk-2.2.9/src/ml_utils/
+-rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2690 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/checkRun.py
+-rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/modelDump.py
+-rw-r--r--   0 marco      (502) staff       (20)     1473 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/modelLoad.py
+-rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/multiModelPredictor.py
+-rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/prepareDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     2014 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/readModels.py
+-rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/scaleDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     3227 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/trainCNNmodel.py
+-rw-r--r--   0 marco      (502) staff       (20)     2213 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/trainNNmodel.py
+-rw-r--r--   0 marco      (502) staff       (20)    68768 2021-11-15 16:16:23.000000 musicntwrk-2.2.9/src/musicntwrk.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.451282 musicntwrk-2.2.9/src/networks/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2577 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/orchestralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2375 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/orchestralVector.py
+-rw-r--r--   0 marco      (502) staff       (20)     1636 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/orchestralVectorColor.py
+-rw-r--r--   0 marco      (502) staff       (20)     4780 2021-11-11 23:43:00.000000 musicntwrk-2.2.9/src/networks/pcsDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5760 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/pcsEgoNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4822 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/pcsNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2920 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/readScore.py
+-rw-r--r--   0 marco      (502) staff       (20)     3321 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rhythmDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     4253 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rhythmNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4186 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rhythmPDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/scoreDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/scoreMIDIDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5142 2021-11-19 01:24:07.000000 musicntwrk-2.2.9/src/networks/scoreNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     5367 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/scoreSubNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     3680 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/timbralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4033 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/vLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4553 2021-11-19 16:56:36.000000 musicntwrk-2.2.9/src/networks/vLeadNetworkByName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2890 2021-11-12 19:23:59.000000 musicntwrk-2.2.9/src/networks/vLeadNetworkByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     2588 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/vLeadNetworkVec.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.458930 musicntwrk-2.2.9/src/plotting/
+-rw-r--r--   0 marco      (502) staff       (20)     1061 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/barplot.py
+-rw-r--r--   0 marco      (502) staff       (20)    25524 2021-10-28 22:26:22.000000 musicntwrk-2.2.9/src/plotting/chordspace.py
+-rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/drawMultiLayerNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2811 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/drawNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2222 2021-11-22 17:29:08.000000 musicntwrk-2.2.9/src/plotting/drawNetworkViz.py
+-rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/drawNetworkX.py
+-rw-r--r--   0 marco      (502) staff       (20)      890 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotCC.py
+-rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotCurveXY.py
+-rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotCurveY.py
+-rw-r--r--   0 marco      (502) staff       (20)     1864 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotOpsHistogram.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.468108 musicntwrk-2.2.9/src/timbre/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1550 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeCompMPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1661 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2646 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeModifiedASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computePSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2261 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeStandardizedMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1769 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeStandardizedMFPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1928 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeStandardizedPSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/mfccSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/mfccSoundDecayOptimal.py
+-rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/mfccSoundDecayPiecewise.py
+-rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/minimizeBKPT.py
+-rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/normSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/normSoundDecay2.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.492662 musicntwrk-2.2.9/src/utils/
+-rw-r--r--   0 marco      (502) staff       (20)      737 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/Remove.py
+-rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/SegmentedLinearReg.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/Sublists.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/communications.py
+-rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyis.py
+-rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyisNew.py
+-rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/entropyKLdiv.py
+-rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/extractByString.py
+-rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/fetchWaves.py
+-rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/findLengthMax.py
+-rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/flatten.py
+-rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/floatize.py
+-rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/generalizedOpsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1541 2021-11-19 01:21:35.000000 musicntwrk-2.2.9/src/utils/generalizedOpsName.py
+-rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/init_list_of_objects.py
+-rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/load_balancing.py
+-rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/minimalDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/minimalDistanceVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/minimalNoBijDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.2.9/src/utils/opsCheckByName.py
+-rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsCheckByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:47.000000 musicntwrk-2.2.9/src/utils/opsName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.2.9/src/utils/opsNameFull.py
+-rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/play_with_simpleaudio.py
+-rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/powerFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/rhythmDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.2.9/src/utils/scaleFreeFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1130 2021-11-22 17:37:40.000000 musicntwrk-2.2.9/src/utils/score2vLead.py
+-rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/str2float.py
+-rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/str2frac.py
+-rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/vectorDistance.py
```

### Comparing `musicntwrk-2.2.8/PKG-INFO` & `musicntwrk-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicntwrk
-Version: 2.2.8
+Version: 2.2.9
 Summary: music as data, data as music
 Home-page: https://www.musicntwrk.com
 Author: Marco Buongiorno Nardelli
 Author-email: mbn@unt.edu
 License: UNKNOWN
 Description: <p></p>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.2.8 Summary: music as data,
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.2.9 Summary: music as data,
 data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
 Nardelli Author-email: mbn@unt.edu License: UNKNOWN Description:
                                [musicntwrk_logo]
                     **** music as data, data as music ****
        unleashing data tools for music theory, analysis and composition
 
 A python library for pitch class set and rhythmic sequences classification and
```

### Comparing `musicntwrk-2.2.8/README.md` & `musicntwrk-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/musicntwrk.egg-info/PKG-INFO` & `musicntwrk-2.2.9/musicntwrk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicntwrk
-Version: 2.2.8
+Version: 2.2.9
 Summary: music as data, data as music
 Home-page: https://www.musicntwrk.com
 Author: Marco Buongiorno Nardelli
 Author-email: mbn@unt.edu
 License: UNKNOWN
 Description: <p></p>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.2.8 Summary: music as data,
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.2.9 Summary: music as data,
 data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
 Nardelli Author-email: mbn@unt.edu License: UNKNOWN Description:
                                [musicntwrk_logo]
                     **** music as data, data as music ****
        unleashing data tools for music theory, analysis and composition
 
 A python library for pitch class set and rhythmic sequences classification and
```

### Comparing `musicntwrk-2.2.8/musicntwrk.egg-info/SOURCES.txt` & `musicntwrk-2.2.9/musicntwrk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 src/networks/vLeadNetworkByName.py
 src/networks/vLeadNetworkByNameVec.py
 src/networks/vLeadNetworkVec.py
 src/plotting/barplot.py
 src/plotting/chordspace.py
 src/plotting/drawMultiLayerNetwork.py
 src/plotting/drawNetwork.py
+src/plotting/drawNetworkViz.py
 src/plotting/drawNetworkX.py
 src/plotting/plotCC.py
 src/plotting/plotCurveXY.py
 src/plotting/plotCurveY.py
 src/plotting/plotOpsHistogram.py
 src/timbre/__init__.py
 src/timbre/computeASCBW.py
@@ -136,10 +137,11 @@
 src/utils/opsName.py
 src/utils/opsNameFull.py
 src/utils/opsNameVec.py
 src/utils/play_with_simpleaudio.py
 src/utils/powerFit.py
 src/utils/rhythmDistance.py
 src/utils/scaleFreeFit.py
+src/utils/score2vLead.py
 src/utils/str2float.py
 src/utils/str2frac.py
 src/utils/vectorDistance.py
```

### Comparing `musicntwrk-2.2.8/setup.py` & `musicntwrk-2.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 this_directory = './'
 #with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 with open(path.join(this_directory, 'README.md')) as f:
 	long_description = f.read()
 
 
 setup(name='musicntwrk',
-	version='2.2.8',
+	version='2.2.9',
 	description='music as data, data as music',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Marco Buongiorno Nardelli',
 	author_email='mbn@unt.edu',
 	platforms='OS independent',
 	url='https://www.musicntwrk.com',
```

### Comparing `musicntwrk-2.2.8/src/comptools/MidiFile.py` & `musicntwrk-2.2.9/src/comptools/MidiFile.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/comptools/genmidi.py` & `musicntwrk-2.2.9/src/comptools/genmidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/comptools/music.py` & `musicntwrk-2.2.9/src/comptools/music.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/comptools/notation.py` & `musicntwrk-2.2.9/src/comptools/notation.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/MIDImap.py` & `musicntwrk-2.2.9/src/data/MIDImap.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/MIDImidi.py` & `musicntwrk-2.2.9/src/data/MIDImidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/MIDIscore.py` & `musicntwrk-2.2.9/src/data/MIDIscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/WRITEscore.py` & `musicntwrk-2.2.9/src/data/WRITEscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/WRITEscoreNoTime.py` & `musicntwrk-2.2.9/src/data/WRITEscoreNoTime.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/WRITEscoreOps.py` & `musicntwrk-2.2.9/src/data/WRITEscoreOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/WRITEscoreOpsMIDI.py` & `musicntwrk-2.2.9/src/data/WRITEscoreOpsMIDI.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/analyzeSound.py` & `musicntwrk-2.2.9/src/data/analyzeSound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/analyzeTimbre.py` & `musicntwrk-2.2.9/src/data/analyzeTimbre.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/ctcsound.py` & `musicntwrk-2.2.9/src/data/ctcsound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/i_spectral.py` & `musicntwrk-2.2.9/src/data/i_spectral.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/i_spectral2.py` & `musicntwrk-2.2.9/src/data/i_spectral2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/i_spectral_pure.py` & `musicntwrk-2.2.9/src/data/i_spectral_pure.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/i_spectral_pyo.py` & `musicntwrk-2.2.9/src/data/i_spectral_pyo.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/i_time_series.py` & `musicntwrk-2.2.9/src/data/i_time_series.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/r_1Ddata.py` & `musicntwrk-2.2.9/src/data/r_1Ddata.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/data/scaleMapping.py` & `musicntwrk-2.2.9/src/data/scaleMapping.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/applyOps.py` & `musicntwrk-2.2.9/src/harmony/applyOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/changePoint.py` & `musicntwrk-2.2.9/src/harmony/changePoint.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/chinese_postman.py` & `musicntwrk-2.2.9/src/harmony/chinese_postman.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/enharmonicDictionary.py` & `musicntwrk-2.2.9/src/harmony/enharmonicDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/getRN.py` & `musicntwrk-2.2.9/src/harmony/getRN.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/harmonicDesign.py` & `musicntwrk-2.2.9/src/harmony/harmonicDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/keySections.py` & `musicntwrk-2.2.9/src/harmony/keySections.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/lookupOps.py` & `musicntwrk-2.2.9/src/harmony/lookupOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/lookupProgr.py` & `musicntwrk-2.2.9/src/harmony/lookupProgr.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/lookupWrapper.py` & `musicntwrk-2.2.9/src/harmony/lookupWrapper.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/networkHarmonyGen.py` & `musicntwrk-2.2.9/src/harmony/networkHarmonyGen.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/plotHarmonicTable.py` & `musicntwrk-2.2.9/src/harmony/plotHarmonicTable.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/rhythmicDesign.py` & `musicntwrk-2.2.9/src/harmony/rhythmicDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/scoreAnalysis.py` & `musicntwrk-2.2.9/src/harmony/scoreAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/scoreDesign.py` & `musicntwrk-2.2.9/src/harmony/scoreDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/scoreFilter.py` & `musicntwrk-2.2.9/src/harmony/scoreFilter.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/shortHands.py` & `musicntwrk-2.2.9/src/harmony/shortHands.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/showAnalysis.py` & `musicntwrk-2.2.9/src/harmony/showAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/spiralChordSpace.py` & `musicntwrk-2.2.9/src/harmony/spiralChordSpace.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/tonalAnalysis.py` & `musicntwrk-2.2.9/src/harmony/tonalAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/tonalHarmonyCalculator.py` & `musicntwrk-2.2.9/src/harmony/tonalHarmonyCalculator.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/tonalHarmonyModels.py` & `musicntwrk-2.2.9/src/harmony/tonalHarmonyModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/tonalPartition.py` & `musicntwrk-2.2.9/src/harmony/tonalPartition.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/harmony/tonnentz.py` & `musicntwrk-2.2.9/src/harmony/tonnentz.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/checkRun.py` & `musicntwrk-2.2.9/src/ml_utils/checkRun.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/modelDump.py` & `musicntwrk-2.2.9/src/ml_utils/modelDump.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/modelLoad.py` & `musicntwrk-2.2.9/src/ml_utils/modelLoad.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/multiModelPredictor.py` & `musicntwrk-2.2.9/src/ml_utils/multiModelPredictor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/prepareDataSet.py` & `musicntwrk-2.2.9/src/ml_utils/prepareDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/readModels.py` & `musicntwrk-2.2.9/src/ml_utils/readModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/scaleDataSet.py` & `musicntwrk-2.2.9/src/ml_utils/scaleDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/trainCNNmodel.py` & `musicntwrk-2.2.9/src/ml_utils/trainCNNmodel.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/ml_utils/trainNNmodel.py` & `musicntwrk-2.2.9/src/ml_utils/trainNNmodel.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/musicntwrk.py` & `musicntwrk-2.2.9/src/musicntwrk.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/orchestralNetwork.py` & `musicntwrk-2.2.9/src/networks/orchestralNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/orchestralVector.py` & `musicntwrk-2.2.9/src/networks/orchestralVector.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/orchestralVectorColor.py` & `musicntwrk-2.2.9/src/networks/orchestralVectorColor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/pcsDictionary.py` & `musicntwrk-2.2.9/src/networks/pcsDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/pcsEgoNetwork.py` & `musicntwrk-2.2.9/src/networks/pcsEgoNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/pcsNetwork.py` & `musicntwrk-2.2.9/src/networks/pcsNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/rLeadNetwork.py` & `musicntwrk-2.2.9/src/networks/rLeadNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/readScore.py` & `musicntwrk-2.2.9/src/networks/readScore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/rhythmDictionary.py` & `musicntwrk-2.2.9/src/networks/rhythmDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/rhythmNetwork.py` & `musicntwrk-2.2.9/src/networks/rhythmNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/rhythmPDictionary.py` & `musicntwrk-2.2.9/src/networks/rhythmPDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/scoreDictionary.py` & `musicntwrk-2.2.9/src/networks/scoreDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/scoreMIDIDictionary.py` & `musicntwrk-2.2.9/src/networks/scoreMIDIDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/scoreNetwork.py` & `musicntwrk-2.2.9/src/networks/scoreNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/scoreSubNetwork.py` & `musicntwrk-2.2.9/src/networks/scoreSubNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/timbralNetwork.py` & `musicntwrk-2.2.9/src/networks/timbralNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/vLeadNetwork.py` & `musicntwrk-2.2.9/src/networks/vLeadNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/vLeadNetworkByName.py` & `musicntwrk-2.2.9/src/networks/vLeadNetworkByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/vLeadNetworkByNameVec.py` & `musicntwrk-2.2.9/src/networks/vLeadNetworkByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/networks/vLeadNetworkVec.py` & `musicntwrk-2.2.9/src/networks/vLeadNetworkVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/barplot.py` & `musicntwrk-2.2.9/src/plotting/barplot.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/chordspace.py` & `musicntwrk-2.2.9/src/plotting/chordspace.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/drawMultiLayerNetwork.py` & `musicntwrk-2.2.9/src/plotting/drawMultiLayerNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/drawNetwork.py` & `musicntwrk-2.2.9/src/plotting/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/drawNetworkX.py` & `musicntwrk-2.2.9/src/plotting/drawNetworkX.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/plotCC.py` & `musicntwrk-2.2.9/src/plotting/plotCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/plotCurveXY.py` & `musicntwrk-2.2.9/src/plotting/plotCurveXY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/plotCurveY.py` & `musicntwrk-2.2.9/src/plotting/plotCurveY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/plotting/plotOpsHistogram.py` & `musicntwrk-2.2.9/src/plotting/plotOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeASCBW.py` & `musicntwrk-2.2.9/src/timbre/computeASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeCompMPS.py` & `musicntwrk-2.2.9/src/timbre/computeCompMPS.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeMFCC.py` & `musicntwrk-2.2.9/src/timbre/computeMFCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeModifiedASCBW.py` & `musicntwrk-2.2.9/src/timbre/computeModifiedASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computePSCC.py` & `musicntwrk-2.2.9/src/timbre/computePSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeStandardizedMFCC.py` & `musicntwrk-2.2.9/src/timbre/computeStandardizedMFCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeStandardizedMFPS.py` & `musicntwrk-2.2.9/src/timbre/computeStandardizedMFPS.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/computeStandardizedPSCC.py` & `musicntwrk-2.2.9/src/timbre/computeStandardizedPSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/mfccSoundDecay.py` & `musicntwrk-2.2.9/src/timbre/mfccSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/mfccSoundDecayOptimal.py` & `musicntwrk-2.2.9/src/timbre/mfccSoundDecayOptimal.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/mfccSoundDecayPiecewise.py` & `musicntwrk-2.2.9/src/timbre/mfccSoundDecayPiecewise.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/minimizeBKPT.py` & `musicntwrk-2.2.9/src/timbre/minimizeBKPT.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/normSoundDecay.py` & `musicntwrk-2.2.9/src/timbre/normSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/timbre/normSoundDecay2.py` & `musicntwrk-2.2.9/src/timbre/normSoundDecay2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/Remove.py` & `musicntwrk-2.2.9/src/utils/Remove.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/SegmentedLinearReg.py` & `musicntwrk-2.2.9/src/utils/SegmentedLinearReg.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/Sublists.py` & `musicntwrk-2.2.9/src/utils/Sublists.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/communications.py` & `musicntwrk-2.2.9/src/utils/communications.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/diffusionEntropyAnalyis.py` & `musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/diffusionEntropyAnalyisNew.py` & `musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyisNew.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/entropyKLdiv.py` & `musicntwrk-2.2.9/src/utils/entropyKLdiv.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/extractByString.py` & `musicntwrk-2.2.9/src/utils/extractByString.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/fetchWaves.py` & `musicntwrk-2.2.9/src/utils/fetchWaves.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/findLengthMax.py` & `musicntwrk-2.2.9/src/utils/findLengthMax.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/flatten.py` & `musicntwrk-2.2.9/src/utils/flatten.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/floatize.py` & `musicntwrk-2.2.9/src/utils/floatize.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/generalizedOpsHistogram.py` & `musicntwrk-2.2.9/src/utils/generalizedOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/generalizedOpsName.py` & `musicntwrk-2.2.9/src/utils/generalizedOpsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/init_list_of_objects.py` & `musicntwrk-2.2.9/src/utils/init_list_of_objects.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/load_balancing.py` & `musicntwrk-2.2.9/src/utils/load_balancing.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/minimalDistance.py` & `musicntwrk-2.2.9/src/utils/minimalDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/minimalDistanceVec.py` & `musicntwrk-2.2.9/src/utils/minimalDistanceVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/minimalNoBijDistance.py` & `musicntwrk-2.2.9/src/utils/minimalNoBijDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsCheckByName.py` & `musicntwrk-2.2.9/src/utils/opsCheckByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsCheckByNameVec.py` & `musicntwrk-2.2.9/src/utils/opsCheckByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsDistance.py` & `musicntwrk-2.2.9/src/utils/opsDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsHistogram.py` & `musicntwrk-2.2.9/src/utils/opsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsName.py` & `musicntwrk-2.2.9/src/utils/opsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsNameFull.py` & `musicntwrk-2.2.9/src/utils/opsNameFull.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/opsNameVec.py` & `musicntwrk-2.2.9/src/utils/opsNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/play_with_simpleaudio.py` & `musicntwrk-2.2.9/src/utils/play_with_simpleaudio.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/powerFit.py` & `musicntwrk-2.2.9/src/utils/powerFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/rhythmDistance.py` & `musicntwrk-2.2.9/src/utils/rhythmDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/scaleFreeFit.py` & `musicntwrk-2.2.9/src/utils/scaleFreeFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/str2float.py` & `musicntwrk-2.2.9/src/utils/str2float.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/str2frac.py` & `musicntwrk-2.2.9/src/utils/str2frac.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.8/src/utils/vectorDistance.py` & `musicntwrk-2.2.9/src/utils/vectorDistance.py`

 * *Files identical despite different names*

