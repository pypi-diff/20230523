# Comparing `tmp/pybigdft-1.0.5.tar.gz` & `tmp/pybigdft-1.0.6.tar.gz`

## Comparing `pybigdft-1.0.5.tar` & `pybigdft-1.0.6.tar`

### file list

```diff
@@ -1,543 +1,519 @@
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pybigdft-1.0.5/.gitrepo
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT_log.yaml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pybigdft-1.0.5/MANIFEST.in
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Makefile-sphinxbuild
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pybigdft-1.0.5/conftest.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pybigdft-1.0.5/setup.cfg
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pybigdft-1.0.5/setup.py
--rw-r--r--   0        0        0    11320 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/AiidaCalculator.py
--rw-r--r--   0        0        0    21263 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Atoms.py
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/BZ.py
--rw-r--r--   0        0        0   131061 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/BioQM.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/CDFT.py
--rw-r--r--   0        0        0    30528 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Calculators.py
--rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Datasets.py
--rw-r--r--   0        0        0    23903 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/DoS.py
--rw-r--r--   0        0        0    23268 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Fragments.py
--rw-r--r--   0        0        0    25941 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/IO.py
--rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/InputActions.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Inputfiles.py
--rw-r--r--   0        0        0    28150 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/LRTDDFT.py
--rwxr-xr-x   0        0        0     6227 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/LogUtils.py
--rw-r--r--   0        0        0    33524 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Logfiles.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/PointParticles.py
--rw-r--r--   0        0        0    50104 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/PostProcessing.py
--rw-r--r--   0        0        0    43833 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/RemoteRunnerUtils.py
--rwxr-xr-x   0        0        0    49020 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/RemoteRunners.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Spillage.py
--rw-r--r--   0        0        0    22494 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Stats.py
--rw-r--r--   0        0        0    48093 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Systems.py
--rw-r--r--   0        0        0    37079 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/URL.py
--rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/UnitCells.py
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Visualization.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/YamlDict.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/check_examples.py
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/wahba.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/__init__.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/postprocess.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/AlF.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Ar.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BF.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BH2.xyz
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BH2Cl.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BH2F.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BH3.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BHF2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BN.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BO.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BS.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Be.xyz
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BeH.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/BeH2.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/C2H.xyz
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/C2H2.xyz
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/C2H3.xyz
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/C2H4.xyz
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/C2H6O.xyz
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/C9H12.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH2-t.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH2.xyz
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH2BH.xyz
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH2F.xyz
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH2NH.xyz
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH2PH.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3.xyz
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3BH2.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3Cl.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3F.xyz
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3NH2.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3O.xyz
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3OH.xyz
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH3SH.xyz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CH4.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CN.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CO.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CO2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CS.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/CSO.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Cl2.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/ClCN.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/ClF.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/F2.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/FCN.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/FCO.xyz
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/FH-OH.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/FNO.xyz
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/H.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/H2.xyz
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/H2CN.xyz
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/H2O-Li.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/H2O.xyz
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HBO.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HBS.xyz
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCCCl.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCCF.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCHO.xyz
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCHS.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCN.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCO.xyz
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCONH2.xyz
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCOOH.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCP.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HCl.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HF.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HNC.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HNO.xyz
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HNS.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HO2.xyz
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HOCl.xyz
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HOF.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/HOOH.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/He.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Li.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Li2.xyz
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/LiBH4.xyz
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/LiCN.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/LiCl.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/LiH.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Mg.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Mg2.xyz
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/N.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/N2.xyz
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/N2H2.xyz
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/N2H4.xyz
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NCO.xyz
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH2.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH2Cl.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH2F.xyz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH2OH.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH3.xyz
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NH3O.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NO.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NOCl.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NP.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Na.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Na2.xyz
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NaCN.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NaCl.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NaH.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/NaLi.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Ne.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/O2.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/O3.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/OCl.xyz
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/OCl2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/OF.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/OF2.xyz
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/OH.xyz
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/P.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/P2.xyz
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/P2H4.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/PH.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/PH2.xyz
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/PH2OH.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/PH3.xyz
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/PH3O.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/PS.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/S2.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/S2H2.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SCl.xyz
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SCl2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SF.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SF2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SH.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SH2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SO-trip.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SO.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SO2.xyz
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/Si4.xyz
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SiH3.xyz
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SiH3Cl.xyz
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SiH3F.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SiH4.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/XYZs/SiO.xyz
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/__init__.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/archer2.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/fugaku.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/hokusai.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/irene.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/localhost.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/spring.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/summer.py
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/uclouvain.py
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/computers/vega.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.H.yaml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.He.yaml
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Be.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.H.yaml
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.He.yaml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Li.yaml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ag.yaml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Al.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.B.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Be.yaml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.C.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ca.yaml
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Cd.yaml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Cl.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.F.yaml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.H.yaml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.He.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.K.yaml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Li.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Mg.yaml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Mo.yaml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.N.yaml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Nb.yaml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ne.yaml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.O.yaml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.P.yaml
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Pd.yaml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Rh.yaml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ru.yaml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Sc.yaml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Si.yaml
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Sr.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Tc.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ti.yaml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.V.yaml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Y.yaml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Zr.yaml
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/ASEInterop.py
--rw-r--r--   0        0        0    18050 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/BabelInterop.py
--rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/DFTBInterop.py
--rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/DNAviewerInterop.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/DispersionInterop.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/MRChemInterop.py
--rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/OpenMMInterop.py
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/PSI4Interop.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/PolarisInterop.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/RDKitInterop.py
--rw-r--r--   0        0        0    16874 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/XTBInterop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/Interop/__init__.py
--rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/DeltaTest.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/InputGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/__init__.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ag.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Al.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ar.cif
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/As.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Au.cif
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/B.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ba.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Be.cif
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Bi.cif
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Br.cif
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/C.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ca.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Cd.cif
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Cl.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Co.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Cr.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Cs.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Cu.cif
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/F.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Fe.cif
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ga.cif
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ge.cif
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/H.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/He.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Hf.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Hg.cif
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/I.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/In.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ir.cif
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/K.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Kr.cif
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Li.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Lu.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Mg.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Mn.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Mo.cif
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/N.cif
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Na.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Nb.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ne.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ni.cif
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/O.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Os.cif
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/P.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Pb.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Pd.cif
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Po.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Pt.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Rb.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Re.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Rh.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Rn.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ru.cif
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/S.cif
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Sb.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Sc.cif
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Se.cif
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Si.cif
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Sn.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Sr.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ta.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Tc.cif
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Te.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Ti.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Tl.cif
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/V.cif
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/W.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Xe.cif
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Y.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Zn.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/CIFs/Zr.cif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ag
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Al
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.B
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Be
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.C
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ca
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Cd
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Cl
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.F
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.H
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.He
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.K
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Li
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Mg
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Mo
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.N
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Nb
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ne
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.O
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.P
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Pd
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Rh
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ru
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Sc
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Si
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Sr
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Tc
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ti
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.V
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Y
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Zr
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Tests/test_CallableAttrDict.ipynb
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Tests/test_RemoteDataset.ipynb
--rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Tests/test_RemoteRunners.ipynb
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Tests/test_URL.ipynb
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Tests/test_YamlDict.ipynb
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 pybigdft-1.0.5/Tests/test_flags.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/BigDFT_log.yaml
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/conf.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/coverage_log.yaml
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/docGeneration.rst
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/index.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/requirements.txt
--rw-r--r--   0        0        0   334081 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/BandStructure.ipynb
--rw-r--r--   0        0        0   280632 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/BandStructure.pdf
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/BandStructure.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/CH4_posinp.xyz
--rw-r--r--   0        0        0    21304 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/FragmentStudio.ipynb
--rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/GeometryOptimization.ipynb
--rw-r--r--   0        0        0    51537 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/LinearCubicComparison.ipynb
--rw-r--r--   0        0        0    18637 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/Link with Fortran and BigDFT in Notebooks.ipynb
--rw-r--r--   0        0        0   159640 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/Logfile-basics.pdf
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/Logfile-basics.py
--rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/QMMM-Fragments.ipynb
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/QMMM-Fragments.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/README
--rw-r--r--   0        0        0   291676 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/Spin-Polarization.ipynb
--rw-r--r--   0        0        0    45853 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/Tutorial-N2.ipynb
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/posinp.xyz
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/0004.xyz
--rw-r--r--   0        0        0   379025 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/BigCase.xyz
--rw-r--r--   0        0        0   234946 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/GEOPT-all_sqnmbiomode.out.ref.yaml
--rw-r--r--   0        0        0   495823 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/log-Graphene.yaml
--rw-r--r--   0        0        0    71825 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/log-HBDMI.yaml
--rw-r--r--   0        0        0  1963112 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/log-K.yaml
--rw-r--r--   0        0        0  4801577 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/log-snap02000-fullQM.yaml
--rw-r--r--   0        0        0   300521 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/newbig-rigid.xyz
--rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/newcenters2.xyz
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/psppar.N
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/three.xyz
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/notebooks/testfiles/two.xyz
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/sphinx_static/bigdft-logo-reduced.svg
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/sphinx_static/custom.css
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/sphinx_static/logo-bigdft-white.svg
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/sphinx_static/logo_header.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pybigdft-1.0.5/source/templates/module.rst_t
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 pybigdft-1.0.5/.gitignore
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 pybigdft-1.0.5/COPYING
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pybigdft-1.0.5/ReadMe.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 pybigdft-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pybigdft-1.0.6/.gitrepo
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pybigdft-1.0.6/MANIFEST.in
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.6/Makefile-sphinxbuild
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pybigdft-1.0.6/conftest.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pybigdft-1.0.6/setup.cfg
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pybigdft-1.0.6/setup.py
+-rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Atoms.py
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/BZ.py
+-rw-r--r--   0        0        0   131061 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/BioQM.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/CDFT.py
+-rw-r--r--   0        0        0    30528 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Calculators.py
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Datasets.py
+-rw-r--r--   0        0        0    23903 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/DoS.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Fragments.py
+-rw-r--r--   0        0        0    25983 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/IO.py
+-rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/InputActions.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Inputfiles.py
+-rw-r--r--   0        0        0    28150 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/LRTDDFT.py
+-rwxr-xr-x   0        0        0     6227 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/LogUtils.py
+-rw-r--r--   0        0        0    33462 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Logfiles.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/PointParticles.py
+-rw-r--r--   0        0        0    50145 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/PostProcessing.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Spillage.py
+-rw-r--r--   0        0        0    22494 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Stats.py
+-rw-r--r--   0        0        0    49326 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Systems.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/UnitCells.py
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Visualization.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/check_examples.py
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/wahba.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/__init__.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/postprocess.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/AlF.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Ar.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BF.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH2.xyz
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH2Cl.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH2F.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH3.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BHF2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BN.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BO.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BS.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Be.xyz
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BeH.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BeH2.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H.xyz
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H2.xyz
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H3.xyz
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H4.xyz
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H6O.xyz
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C9H12.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2-t.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2.xyz
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2BH.xyz
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2F.xyz
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2NH.xyz
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2PH.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3.xyz
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3BH2.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3Cl.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3F.xyz
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3NH2.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3O.xyz
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3OH.xyz
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3SH.xyz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH4.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CN.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CO.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CO2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CS.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CSO.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Cl2.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/ClCN.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/ClF.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/F2.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FCN.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FCO.xyz
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FH-OH.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FNO.xyz
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2.xyz
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2CN.xyz
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2O-Li.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2O.xyz
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HBO.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HBS.xyz
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCCCl.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCCF.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCHO.xyz
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCHS.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCN.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCO.xyz
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCONH2.xyz
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCOOH.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCP.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCl.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HF.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HNC.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HNO.xyz
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HNS.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HO2.xyz
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HOCl.xyz
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HOF.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HOOH.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/He.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Li.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Li2.xyz
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiBH4.xyz
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiCN.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiCl.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiH.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Mg.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Mg2.xyz
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N2.xyz
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N2H2.xyz
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N2H4.xyz
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NCO.xyz
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2Cl.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2F.xyz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2OH.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH3.xyz
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH3O.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NO.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NOCl.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NP.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Na.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Na2.xyz
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaCN.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaCl.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaH.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaLi.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Ne.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/O2.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/O3.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OCl.xyz
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OCl2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OF.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OF2.xyz
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OH.xyz
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/P.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/P2.xyz
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/P2H4.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH2.xyz
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH2OH.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH3.xyz
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH3O.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PS.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/S2.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/S2H2.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SCl.xyz
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SCl2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SF.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SF2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SH.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SH2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SO-trip.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SO.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SO2.xyz
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Si4.xyz
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH3.xyz
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH3Cl.xyz
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH3F.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH4.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiO.xyz
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.H.yaml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.He.yaml
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Be.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.H.yaml
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.He.yaml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Li.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ag.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Al.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.B.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Be.yaml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.C.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ca.yaml
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cd.yaml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cl.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.F.yaml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.H.yaml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.He.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.K.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Li.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mg.yaml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mo.yaml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.N.yaml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Nb.yaml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ne.yaml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.O.yaml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.P.yaml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Pd.yaml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Rh.yaml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ru.yaml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sc.yaml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Si.yaml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sr.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Tc.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ti.yaml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.V.yaml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Y.yaml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Zr.yaml
+-rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/ASEInterop.py
+-rw-r--r--   0        0        0    18050 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/BabelInterop.py
+-rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/DFTBInterop.py
+-rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/DNAviewerInterop.py
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/DispersionInterop.py
+-rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/MRChemInterop.py
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/OpenMMInterop.py
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/PSI4Interop.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/PolarisInterop.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/RDKitInterop.py
+-rw-r--r--   0        0        0    16874 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/XTBInterop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/__init__.py
+-rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/DeltaTest.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/InputGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/__init__.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ag.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Al.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ar.cif
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/As.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Au.cif
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/B.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ba.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Be.cif
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Bi.cif
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Br.cif
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/C.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ca.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cd.cif
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cl.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Co.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cr.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cs.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cu.cif
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/F.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Fe.cif
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ga.cif
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ge.cif
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/H.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/He.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Hf.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Hg.cif
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/I.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/In.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ir.cif
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/K.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Kr.cif
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Li.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Lu.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Mg.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Mn.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Mo.cif
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/N.cif
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Na.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Nb.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ne.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ni.cif
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/O.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Os.cif
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/P.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Pb.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Pd.cif
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Po.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Pt.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Rb.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Re.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Rh.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Rn.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ru.cif
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/S.cif
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sb.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sc.cif
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Se.cif
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Si.cif
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sn.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sr.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ta.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Tc.cif
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Te.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ti.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Tl.cif
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/V.cif
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/W.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Xe.cif
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Y.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Zn.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Zr.cif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ag
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Al
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.B
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Be
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.C
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ca
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cd
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cl
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.F
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.H
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.He
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.K
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Li
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mg
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mo
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.N
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Nb
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ne
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.O
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.P
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Pd
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Rh
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ru
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sc
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Si
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sr
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Tc
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ti
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.V
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Y
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Zr
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/conf.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/docGeneration.rst
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/index.rst
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/requirements.txt
+-rw-r--r--   0        0        0   334081 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/BandStructure.ipynb
+-rw-r--r--   0        0        0   280632 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/BandStructure.pdf
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/BandStructure.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/CH4_posinp.xyz
+-rw-r--r--   0        0        0    21304 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/FragmentStudio.ipynb
+-rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/GeometryOptimization.ipynb
+-rw-r--r--   0        0        0    51537 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/LinearCubicComparison.ipynb
+-rw-r--r--   0        0        0    18637 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Link with Fortran and BigDFT in Notebooks.ipynb
+-rw-r--r--   0        0        0   159640 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Logfile-basics.pdf
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Logfile-basics.py
+-rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/QMMM-Fragments.ipynb
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/QMMM-Fragments.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/README
+-rw-r--r--   0        0        0   291676 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Spin-Polarization.ipynb
+-rw-r--r--   0        0        0    45853 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Tutorial-N2.ipynb
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/posinp.xyz
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/0004.xyz
+-rw-r--r--   0        0        0   379025 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/BigCase.xyz
+-rw-r--r--   0        0        0   234946 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/GEOPT-all_sqnmbiomode.out.ref.yaml
+-rw-r--r--   0        0        0   495823 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-Graphene.yaml
+-rw-r--r--   0        0        0    71825 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-HBDMI.yaml
+-rw-r--r--   0        0        0  1963112 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-K.yaml
+-rw-r--r--   0        0        0  4801577 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-snap02000-fullQM.yaml
+-rw-r--r--   0        0        0   300521 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/newbig-rigid.xyz
+-rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/newcenters2.xyz
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/psppar.N
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/three.xyz
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/two.xyz
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/bigdft-logo-reduced.svg
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/custom.css
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/logo-bigdft-white.svg
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/logo_header.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/templates/module.rst_t
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 pybigdft-1.0.6/.gitignore
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 pybigdft-1.0.6/COPYING
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pybigdft-1.0.6/ReadMe.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 pybigdft-1.0.6/PKG-INFO
```

### Comparing `pybigdft-1.0.5/Makefile-sphinxbuild` & `pybigdft-1.0.6/Makefile-sphinxbuild`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/conftest.py` & `pybigdft-1.0.6/conftest.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/setup.py` & `pybigdft-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Atoms.py` & `pybigdft-1.0.6/BigDFT/Atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,15 @@
 
 
 def IsReduced(units):
     """
     Checks if a string or atom has reduced as its units.
 
     Args:
-      units: either a string or a (BigDFT.Atoms.Atom)
+      units(BigDFT.Atoms.Atom, str): either a string or a Atom.
     """
     if hasattr(units, 'store'):
         check = units.store.get("units")
         if not check:
             return False
     else:
         check = units
```

### Comparing `pybigdft-1.0.5/BigDFT/BZ.py` & `pybigdft-1.0.6/BigDFT/BZ.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/BioQM.py` & `pybigdft-1.0.6/BigDFT/BioQM.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/CDFT.py` & `pybigdft-1.0.6/BigDFT/CDFT.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Calculators.py` & `pybigdft-1.0.6/BigDFT/Calculators.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Datasets.py` & `pybigdft-1.0.6/BigDFT/Datasets.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/DoS.py` & `pybigdft-1.0.6/BigDFT/DoS.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Fragments.py` & `pybigdft-1.0.6/BigDFT/Fragments.py`

 * *Files 3% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         Args:
             cell (BigDFT.UnitCells.UnitCell): the cell this fragment is
               contained in. Minimum image convention will be enforced.
             units (str): units of the centroid to be returned.
         """
         from numpy import mean, ravel
         pos = [at.get_position(units=units, cell=cell) for at in self]
-        return ravel(mean(pos, axis=0))
+        return ravel(mean(pos, axis=0)).tolist()
 
     def center_of_charge(self):  # , zion):
         """
         The charge center which depends both on the position and net charge
         of each atom.
         """
         from numpy import array
@@ -588,15 +588,15 @@
             yval = y
             zval = z
         else:
             raise ValueError("Units must be degrees or radians")
 
         # Translate back to the origin.
         centroid = self.centroid
-        self.translate(-1.0 * centroid)
+        self.translate([-1.0 * x for x in centroid])
 
         # Build the rotation
         rot = identity(3)
         if x:
             rx = mat([
                 [1.0,        0.0,       0.0],
                 [0.0,        cos(xval), -sin(xval)],
@@ -671,50 +671,14 @@
         Calculate the Reduced Mean Square displacement with a reference
         fragment.
         """
         R = RotoTranslation(reference, self)
         return R.J
 
 
-class Lattice():
-    """
-    Defines the fundamental objects to deal with periodic systems
-    """
-
-    def __init__(self, vectors):
-        self.vectors = vectors
-
-    def grid(self, origin=[0.0, 0.0, 0.0], extremes=None, radius=None):
-        """
-        Produces a set of translation vectors from a given origin
-        """
-        import numpy as np
-        transl = []
-        g = [[], [], []]  # the grid of discrete translations
-        if extremes is not None:
-            # print extremes
-            for i, d in enumerate(extremes):
-                for k in range(d[0], d[1] + 1):
-                    g[i].append(k)
-            # print g
-            for i in g[0]:
-                arri = np.array(self.vectors[0]) * i
-                for j in g[1]:
-                    arrj = np.array(self.vectors[1]) * j + arri
-                    for k in g[2]:
-                        arrk = np.array(self.vectors[2]) * k + arrj
-                        vect = np.array(origin) + arrk
-                        app = True
-                        if radius is not None:
-                            app = np.linalg.norm(arrk) < radius
-                        if app:
-                            transl.append(vect)
-        return transl
-
-
 def _example():
     """Example of using fragments"""
     from BigDFT.IO import XYZReader, XYZWriter
     from copy import deepcopy
 
     safe_print("Read in an xyz file and build from a list.")
     atom_list = []
```

### Comparing `pybigdft-1.0.5/BigDFT/IO.py` & `pybigdft-1.0.6/BigDFT/IO.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,15 +359,16 @@
     from BigDFT.UnitCells import UnitCell
     from warnings import warn
 
     sys = System()
 
     # Just go ahead and read the whole file into a string.
     lines = [x for x in ifile]
-
+    if len(lines) == 0:
+        return sys
     # First pass, read in the number of atoms.
     for start, line in enumerate(lines):
         if ("@<TRIPOS>MOLECULE" in line):
             break
     start += 1
 
     split = lines[start+1].split()
```

### Comparing `pybigdft-1.0.5/BigDFT/InputActions.py` & `pybigdft-1.0.6/BigDFT/InputActions.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Inputfiles.py` & `pybigdft-1.0.6/BigDFT/Inputfiles.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/LRTDDFT.py` & `pybigdft-1.0.6/BigDFT/LRTDDFT.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/LogUtils.py` & `pybigdft-1.0.6/BigDFT/LogUtils.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Logfiles.py` & `pybigdft-1.0.6/BigDFT/Logfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         ax.axvline(it, color='k', linestyle='dashdot')
     ax.xaxis.set_major_locator(MaxNLocator(integer=True))
     ax.set_xlabel('WFN Iterations')
     ax.set_ylabel('Norm of WFN Residue')
     return ax
 
 
-class Logfile():
+class Logfile:
     """
     Import a Logfile from a filename in yaml format, a list of filenames,
     an archive (compressed tar file), a dictionary or a list of dictionaries.
 
     Args:
         *args: sequence of logfiles to be parsed. If it is longer than
             one item, the logfiles are considered as belonging to the same run.
@@ -438,36 +438,32 @@
             ens = [(ll.energy if hasattr(ll, 'energy') else 1.e100)
                    for ll in self._instances]
             #: Position in the logfile items of the run associated to lower
             #  energy
             self.reference_log = numpy.argmin(ens)
             # print 'Energies',ens
             self._initialize_class(dicts[self.reference_log])
-    #
 
     def __getitem__(self, index):
         if hasattr(self, '_instances'):
             return self._instances[index]
         else:
             # print('index not available')
             raise ValueError(
                 'This instance of Logfile has no multiple instances')
-    #
 
     def __str__(self):
         """Display short information about the logfile"""
         return self._print_information()
-    #
 
     def __len__(self):
         if hasattr(self, '_instances'):
             return len(self._instances)
         else:
             return 0  # single point run
-    #
 
     def __toType(self, val, tp=None):
         from futile.Utils import floatify
         if tp == FLOAT_SCALAR:
             return floatify(val)
         elif tp == MIXED_SCALAR:
             try:
@@ -544,15 +540,14 @@
         self.memory = {}
         for key in ['memory_run', 'memory_quantities', 'memory_peak']:
             if hasattr(self, key):
                 title = BUILTIN[key][PATH][0][0]
                 self.memory[title] = getattr(self, key)
                 if key != 'memory_peak':
                     delattr(self, key)
-    #
 
     def _fermi_level_from_evals(self, evals):
         import numpy
         # this works when the representation of the evals is only with
         # occupied states
         # write('evals',self.evals)
         fl = None
@@ -569,15 +564,14 @@
                 fl = e if not isinstance(
                     e, list) else numpy.max(numpy.array(e))
             e = ev.get('e_vrt', ev.get('e_virt'))
             if e is not None:
                 break
         #: Chemical potential of the system
         self.fermi_level = fl
-    #
 
     def _sdos_line_to_orbitals_old(self, sorbs):
         from BigDFT import BZ
         evals = []
         iorb = 1
         # renorm=len(xs)
         # iterate on k-points
@@ -595,15 +589,14 @@
                                's': 1-2*ispin, 'k': i+1})
                     # ev.append({'e':np.sum([ so[iorb+iorbk] for so in sd]),
                     #            's':1-2*ispin,'k':i+1})
                 iorb += norb
             evals.append(BZ.BandArray(
                 ev, ikpt=i+1, kpt=kp['Rc'], kwgt=kp['Wgt']))
         return evals
-    #
 
     def _sdos_line_to_orbitals(self, sorbs):
         import numpy as np
         iorb = 1
         sdos = [[], []]
         for ikpt, band in enumerate(self.evals):
             sdoskpt = [[], []]
@@ -612,15 +605,14 @@
                     continue
                 for i in range(norb):
                     val = sorbs[iorb]
                     iorb += 1
                     sdoskpt[ispin].append(val)
                 sdos[ispin].append(np.array(sdoskpt[ispin]))
         return sdos
-    #
 
     def _get_bz(self, ev, kpts):
         """Get the Brillouin Zone."""
         evals = []
         from BigDFT import BZ
         for i, kp in enumerate(kpts):
             evals.append(BZ.BandArray(
@@ -664,27 +656,25 @@
         mesh = self.kpt_mesh  # : K-points grid
         if isinstance(mesh, int):
             mesh = [mesh, ]*3
         if self.astruct['cell'][1] == float('inf'):
             mesh[1] = 1
         return BZ.BrillouinZone(self.astruct, mesh, self.evals,
                                 self.fermi_level)
-    #
 
     def SCF_convergence(self, ax=None):
         """
         Plot the wavefunction convergence.
         :Example:
            >>> tt=Logfile('log-with-wfn-optimization.yaml',label='a label')
            >>> tt.wfn_plot()
         """
         wfn_it = find_iterations(self.log)
         return plot_wfn_convergence(wfn_it, self.gnrm_cv, label=self.label,
                                     ax=ax)
-    #
 
     def geopt_plot(self, ax=None):
         """
         For a set of logfiles construct the convergence plot if available.
         Plot the Maximum value of the forces against the difference between
         the minimum value of the energy and the energy of the iteration.
         Also an errorbar is given indicating the noise on the forces for a
```

### Comparing `pybigdft-1.0.5/BigDFT/PointParticles.py` & `pybigdft-1.0.6/BigDFT/PointParticles.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/PostProcessing.py` & `pybigdft-1.0.6/BigDFT/PostProcessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1298,15 +1298,15 @@
         return keys, values
 
     from_scratch = False
     if ax is None:
         fig, ax = plt.subplots()
         from_scratch = True
     else:
-        from_scratch = not reuse_ticks
+        from_scratch = not reuse_ticks or (not ax.lines and not ax.collections)
     keys, values = get_keys_and_values(ax, system_dict, from_scratch)
     ret = ax.violinplot(values, **kwargs)
     ax.set_xticks(range(1, len(keys)+1))
     ax.set_xticklabels(keys, rotation=90)
     return ax, ret
```

### Comparing `pybigdft-1.0.5/BigDFT/Spillage.py` & `pybigdft-1.0.6/BigDFT/Spillage.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Stats.py` & `pybigdft-1.0.6/BigDFT/Stats.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Systems.py` & `pybigdft-1.0.6/BigDFT/Systems.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @property
     def centroid(self):
         """
         Center of mass of the system
         """
         from numpy import mean
-        return mean([frag.centroid for frag in self.values()], axis=0)
+        return mean([frag.centroid for frag in self.values()], axis=0).tolist()
 
     @property
     def central_fragment(self):
         """
         Returns the fragment whose center of mass is closest to the centroid
 
         Returns:
@@ -241,20 +241,21 @@
         pos = []
         nokey = ['r', 'frag', 'Frozen', 'sym', 'units']
         if order is None:
             order = list(self)
         for fragid in order:
             frag = self[fragid]
             for at in frag:
-                atdict = {at.sym: at.get_position(units, self.cell)}
+                atdict = {}
                 atdict["frag"] = list(GetFragTuple(fragid))
                 if frag.frozen:
                     atdict["Frozen"] = frag.frozen
                 atdict.update({k: v for k, v in at.store.items()
                                if k not in nokey})
+                atdict.update({at.sym: at.get_position(units, self.cell)})
                 pos.append(atdict)
 
         result = {}
         result["positions"] = pos
         if IsReduced(units):
             result["units"] = "angstroem"
             result["cell"] = self.cell.get_posinp("angstroem")
@@ -362,14 +363,36 @@
             else:
                 frag_slicing = atom_slicing(sl, [frag])
                 dist_restricted = dist[:, frag_slicing]
                 val = min(dist_restricted.flatten())
             alldist[frag] = val
         return alldist
 
+    def to_file(self, filename, **kwargs):
+        """Dump the System instance into a file.
+
+        Write the system information in the file system, according to the
+        file extension
+
+        Args:
+            filename (str): path of the filename to write into. Automatically
+                determine the format according to the file extension
+            **kwargs: further kwyword arguments to be passed to the writing
+                routine
+        """
+        from BigDFT import IO
+
+        extension = filename.split('.')[-1].lower()
+
+        with open(filename, 'w') as ofile:
+            if extension == 'pdb':
+                IO.write_pdb(system=self, ofile=ofile)
+            if extension == 'xyz':
+                IO.write_xyz(system=self, ofile=ofile)
+
     @property
     def PointParticles(self):
         """
         Transform the system into a `py:class:~PointParticles.PointParticles`
         object
         """
         from BigDFT.PointParticles import PointParticles as PP
@@ -1110,41 +1133,48 @@
     logfile. If the logfile contains information about fragmentation and atomic
     multipoles, then the system is created accordingly.
     Otherwise, the fragmentation scheme is determined by the fragmentation
     variable.
 
     Args:
        log (Logfile): the logfile of the QM run. In general the execution
-           should be performed with Linear Scaling formalism.
+           should be performed with Linear Scaling formalism, but
+           also other executions are possible (dry_run for instance).
        fragmentation (str): the scheme to be used for the fragmentation in the
            case if not provided internally by the logfile.
            The possible values are ``atomic`` and ``full``, in which case the
            system as as many fragments as the number of atoms, or only one
            fragment, respectively.
     Returns:
         (BigDFT.Systems.System): The instance of the class containing
         fragments.
     """
     from BigDFT.Fragments import Fragment
+    from BigDFT.UnitCells import UnitCell
     name = log.log.get('run_name', 'FULL') + ':0'
 
     full_system = System()
     posinp = log.log.get('posinp')
     if posinp is not None and not isinstance(posinp, str):
         full_system[name] = Fragment(posinp=posinp)
+        cell = UnitCell(cell=posinp.get('cell'),
+                        units=posinp.get('units', 'angstroem'))
     else:
         full_system[name] = Fragment(astruct=log.astruct)
+        cell = UnitCell(cell=log.astruct.get('cell'),
+                        units=log.astruct.get('units', 'angstroem'))
 
     full_system.set_logfile_info(log)
 
     # now we may defragment the system according to the provided scheme
     if fragmentation == 'full':
         return full_system
     elif fragmentation == 'atomic' or 'posinp' not in log.log:
         atomic_system = System()
+        atomic_system.cell = cell
         for iat, at in enumerate(full_system[name]):
             atomic_system['ATOM:' + str(iat)] = Fragment([at])
         return atomic_system
     else:
         posinp = log.log['posinp']
         frag_dict = {}
         for iat, tupl in enumerate(zip(posinp['positions'],
@@ -1154,14 +1184,15 @@
             if isinstance(fragid, list):
                 fragid = ':'.join(map(str, fragid))
             if fragid not in frag_dict:
                 frag_dict[fragid] = [obj]
             else:
                 frag_dict[fragid].append(obj)
         frag_system = System()
+        frag_system.cell = cell
         for fragid in frag_dict:
             frag_system[fragid] = Fragment(frag_dict[fragid])
         return frag_system
 
 
 def system_from_df(df):
     """System instance from system dataframe.
```

### Comparing `pybigdft-1.0.5/BigDFT/UnitCells.py` & `pybigdft-1.0.6/BigDFT/UnitCells.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,23 +145,23 @@
             (list): the position in cartesian coordinates.
         """
         from numpy import array
         return array(self.cell).dot(pos)
 
     def to_reduced(self, pos):
         """
-        Convert a vector which is in reduced units to cartesian units.
+        Convert a vector which is in cartesian units to reduced units.
 
         Returns:
             (list): the position in reduced coordinates.
         """
-        from numpy import array
+        from numpy import array, round
         from numpy.linalg import solve
 
-        return solve(array(self.cell), pos)
+        return round(solve(array(self.cell), pos), 6)
 
     def mirror_point(self, pos):
         """
         Given a point in space, this returns a list of points replicated
         across all periodic boundaries.
 
         Args:
```

### Comparing `pybigdft-1.0.5/BigDFT/Visualization.py` & `pybigdft-1.0.6/BigDFT/Visualization.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/check_examples.py` & `pybigdft-1.0.6/BigDFT/check_examples.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/wahba.py` & `pybigdft-1.0.6/BigDFT/wahba.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/postprocess.yaml` & `pybigdft-1.0.6/BigDFT/Database/postprocess.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/XYZs/C9H12.xyz` & `pybigdft-1.0.6/BigDFT/Database/XYZs/C9H12.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ag.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ag.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Al.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Al.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.B.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.B.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Be.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Be.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.C.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.C.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ca.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ca.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Cd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Cl.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.F.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.F.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.K.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Li.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Li.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Mg.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Mo.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mo.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.N.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.N.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Nb.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Nb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ne.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ne.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.O.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.O.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.P.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.P.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Pd.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Pd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Rh.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Rh.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ru.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ru.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Sc.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Si.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Si.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Sr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Tc.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Tc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Ti.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ti.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.V.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.V.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Y.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Y.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Database/psppar/SS/psppar.Zr.yaml` & `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Zr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/ASEInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/ASEInterop.py`

 * *Files 13% similar despite different names*

```diff
@@ -192,59 +192,14 @@
 
     def _run_calculation(self):
         self.log = self.code.run(input=self.parameters,
                                  posinp=self._get_posinp(),
                                  name=self.label, run_dir=self.rundir)
 
 
-class RemoteBigDFTASECalculator(BigASECalculator):
-    """
-    This calculator can be used by ASE to run remote BigDFT calculations.
-
-    Args:
-      parameters (BigDFT.Inputfiles.Inputfile): the input parameters to use.
-      calc (BigDFT.Calculators.SystemCalculator): the calculator to use.
-      runner_args (dict): the arguments that are passed to a remote runner
-        when it is created.
-      directory (str): the directory to run the calculation in.
-      label (str): a label for this particular calculation.
-      atoms (ase.Atoms): an ase collection of atoms to compute.
-    """
-    def __init__(self, parameters, calc, runner_args, restart=None,
-                 ignore_bad_restart_file=False, directory=".", label=None,
-                 atoms=None, **kwargs):
-        # Call the Super Method
-        BigASECalculator.__init__(self, parameters=parameters, calc=calc, restart=restart,
-                 ignore_bad_restart_file=ignore_bad_restart_file,
-                 directory=directory, label=label,
-                 atoms=atoms, **kwargs)
-
-        # Internal data.
-        self.runner_args = runner_args
-
-    def _run_calculation(self):
-        import BigDFT.RemoteRunners as R
-        from time import sleep
-
-        def single_point(sys, inp, code, label, run_dir):
-            return code.run(input=inp, posinp=sys.get_posinp(),
-                            name=label, run_dir=run_dir)
-
-        fargs = {"sys": self._create_system(), "inp": self.parameters, "code": self.code,
-                 "label": self.label, "run_dir": self.rundir}
-
-        runner = R.RemoteRunner(single_point, arguments=fargs,
-                                name=self.label, **self.runner_args)
-        runner.run(asynchronous=True, skip=False)
-
-        while not runner.is_finished(verbose=False, anyfile=False):
-            sleep(1)
-        self.log = runner.fetch_result()
-
-
 def _example():
     """Example of using ASE interoperability"""
     from BigDFT.IO import XYZReader
     from BigDFT.Inputfiles import Inputfile
     from BigDFT.Calculators import SystemCalculator
     from BigDFT.Fragments import Fragment
     from BigDFT.Systems import System
```

### Comparing `pybigdft-1.0.5/BigDFT/Interop/BabelInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/BabelInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/DFTBInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/DFTBInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/DNAviewerInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/DNAviewerInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/DispersionInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/DispersionInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/MRChemInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/MRChemInterop.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,19 @@
         if "output" not in self:
             raise ValueError("Calculation data not there")
 
 
 class MRChemCalculator(Runner):
     """
     A calculator that drives MRChem calculations through the command line.
+
+    This calculator will look in the environment for the following variables:
+    * OMP_NUM_THREADS : number of threads to use
+    * MRCHEM_MPIRUN : the mpi command you want to launch mrchem with
+    * MRCHEM_ROOT : the directoy that contains the mrchem executable.
     """
     import os
 
     def __init__(self, omp=os.environ.get('OMP_NUM_THREADS', '1'),
                  mpi_run=os.environ.get('MRCHEM_MPIRUN', ''),
                  dry_run=False, skip=False, verbose=True):
         from os.path import join
@@ -140,24 +145,33 @@
 
         return ostr
 
     def _get_logname(self):
         return self.run_options.get("name", "mrchem") + ".json"
 
     def _get_command(self):
+        from os import environ
+        from os.path import join
+
         if self._check_skip():
             return '''echo "skip"'''
 
-        iname = self.run_options.get("name", "mrchem")
-        oname = iname + ".json"
+        iname = self.run_options.get("name", "mrchem") + ".inp"
+        oname = self.run_options.get("name", "mrchem") + ".json"
 
-        cmd = "cd " + self.run_dir + "; mrchem"
-        cmd += " --json " + iname
+        cmd = "cd " + self.run_dir + "; "
+        if "MRCHEM_ROOT" in environ:
+            cmd += join(environ["MRCHEM_ROOT"], "mrchem")
+        else:
+            cmd += "mrchem"
+        cmd += " --json " + iname + " "
         if "mpi_run" in self.run_options:
-            cmd += ' --launcher "' + self.run_options["mpi_run"] + '"'
+            cmd += '--launcher="' + self.run_options["mpi_run"] + '" '
+        if "MRCHEM_ROOT" in environ:
+            cmd += "--executable=" + join(environ["MRCHEM_ROOT"], "mrchem.x")
         cmd += " > " + oname
 
         return cmd
 
     def _check_skip(self):
         from json import JSONDecodeError
         from os.path import join
```

### Comparing `pybigdft-1.0.5/BigDFT/Interop/OpenMMInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/OpenMMInterop.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     def write(self, ofile):
         from openmm import app
         app.PDBFile.writeFile(self.OMMsimulation.topology, self.OMMposition,
                               open(ofile, 'w'))
 
     def optimize(self, iters):
-        self.OMMsimulation.minimizeEnergy(maxIterations=iters)
+        return self.OMMsimulation.minimizeEnergy(maxIterations=iters)
 
     @property
     def forcegroups(self):
         forcegroups = {}
         for i in range(self.OMMsystem.getNumForces()):
             force = self.OMMsystem.getForce(i)
             force.setForceGroup(i)
@@ -296,15 +296,18 @@
         add_missing_residues (bool): include missing residues if true.
         keepIds (bool): If True, keep the residue and chain IDs specified
             in the Topology rather than generating new ones.
         convert_from_charmm_format (bool): Accept the PDB format which is
             usually provided as the output of charmm-gui.
             The chain id is provided as the last letter of each line.
         variants (dict): dictionary of ``chain_id,res_id: name`` of the
-            variants which have to be imposed for the protonation state
+            variants which have to be imposed for the protonation state.
+            Allowed names are ASH, ASP, CYS, CYX, GLH, GLU, HID, HIE, HIP,
+            HIN, LYN, LYS, with obvious meaning of the names
+            (see OpenMM documentation).
 
     Warning:
         (From OpenMM documentation)
         When keepIds=True, it is up to the caller to make sure these are
         valid IDs that satisfy the requirements of the PDB format.
         Otherwise, the output file will be invalid.
```

### Comparing `pybigdft-1.0.5/BigDFT/Interop/PSI4Interop.py` & `pybigdft-1.0.6/BigDFT/Interop/PSI4Interop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/PolarisInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/PolarisInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/RDKitInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/RDKitInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/Interop/XTBInterop.py` & `pybigdft-1.0.6/BigDFT/Interop/XTBInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/DeltaTest.py` & `pybigdft-1.0.6/BigDFT/scripts/DeltaTest.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/InputGenerator.py` & `pybigdft-1.0.6/BigDFT/scripts/InputGenerator.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ag.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ag.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Al.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Al.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ar.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ar.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/As.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/As.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Au.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Au.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/B.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/B.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ba.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ba.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Be.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Be.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Bi.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Bi.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Br.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Br.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/C.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/C.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ca.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ca.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Cd.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cd.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Cl.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cl.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Co.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Co.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Cr.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Cs.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cs.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Cu.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cu.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/F.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/F.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Fe.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Fe.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ga.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ga.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ge.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ge.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/H.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/H.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/He.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/He.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Hf.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Hf.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Hg.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Hg.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/I.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/I.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/In.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/In.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ir.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ir.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/K.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/K.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Kr.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Kr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Li.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Li.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Lu.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Lu.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Mg.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Mg.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Mn.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Mn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Mo.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Mo.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/N.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/N.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Na.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Na.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Nb.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Nb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ne.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ne.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ni.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ni.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/O.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/O.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Os.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Os.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/P.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/P.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Pb.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Pb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Pd.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Pd.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Po.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Po.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Pt.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Pt.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Rb.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Rb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Re.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Re.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Rh.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Rh.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Rn.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Rn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ru.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ru.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/S.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/S.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Sb.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Sc.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sc.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Se.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Se.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Si.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Si.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Sn.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Sr.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ta.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ta.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Tc.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Tc.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Te.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Te.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Ti.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ti.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Tl.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Tl.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/V.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/V.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/W.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/W.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Xe.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Xe.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Y.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Y.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Zn.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Zn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/CIFs/Zr.cif` & `pybigdft-1.0.6/BigDFT/scripts/CIFs/Zr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ag` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ag`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Al` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Al`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ca` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ca`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Cd` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cd`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Cl` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cl`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.K` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.K`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Mg` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mg`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Mo` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mo`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Nb` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Nb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.P` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.P`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Pd` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Pd`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Rh` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Rh`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ru` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ru`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Sc` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sc`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Si` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Si`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Sr` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sr`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Tc` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Tc`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Ti` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ti`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.V` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.V`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Y` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Y`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/BigDFT/scripts/psppar/psppar.Zr` & `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Zr`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/conf.py` & `pybigdft-1.0.6/source/conf.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/docGeneration.rst` & `pybigdft-1.0.6/source/docGeneration.rst`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/index.rst` & `pybigdft-1.0.6/source/index.rst`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/BandStructure.ipynb` & `pybigdft-1.0.6/source/notebooks/BandStructure.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/BandStructure.pdf` & `pybigdft-1.0.6/source/notebooks/BandStructure.pdf`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/BandStructure.py` & `pybigdft-1.0.6/source/notebooks/BandStructure.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/FragmentStudio.ipynb` & `pybigdft-1.0.6/source/notebooks/FragmentStudio.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/GeometryOptimization.ipynb` & `pybigdft-1.0.6/source/notebooks/GeometryOptimization.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/LinearCubicComparison.ipynb` & `pybigdft-1.0.6/source/notebooks/LinearCubicComparison.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/Link with Fortran and BigDFT in Notebooks.ipynb` & `pybigdft-1.0.6/source/notebooks/Link with Fortran and BigDFT in Notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/Logfile-basics.pdf` & `pybigdft-1.0.6/source/notebooks/Logfile-basics.pdf`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/Logfile-basics.py` & `pybigdft-1.0.6/source/notebooks/Logfile-basics.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/QMMM-Fragments.ipynb` & `pybigdft-1.0.6/source/notebooks/QMMM-Fragments.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/QMMM-Fragments.py` & `pybigdft-1.0.6/source/notebooks/QMMM-Fragments.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/Spin-Polarization.ipynb` & `pybigdft-1.0.6/source/notebooks/Spin-Polarization.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/Tutorial-N2.ipynb` & `pybigdft-1.0.6/source/notebooks/Tutorial-N2.ipynb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/0004.xyz` & `pybigdft-1.0.6/source/notebooks/testfiles/0004.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/BigCase.xyz` & `pybigdft-1.0.6/source/notebooks/testfiles/BigCase.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/GEOPT-all_sqnmbiomode.out.ref.yaml` & `pybigdft-1.0.6/source/notebooks/testfiles/GEOPT-all_sqnmbiomode.out.ref.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/log-Graphene.yaml` & `pybigdft-1.0.6/source/notebooks/testfiles/log-Graphene.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/log-HBDMI.yaml` & `pybigdft-1.0.6/source/notebooks/testfiles/log-HBDMI.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/log-K.yaml` & `pybigdft-1.0.6/source/notebooks/testfiles/log-K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/log-snap02000-fullQM.yaml` & `pybigdft-1.0.6/source/notebooks/testfiles/log-snap02000-fullQM.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/newbig-rigid.xyz` & `pybigdft-1.0.6/source/notebooks/testfiles/newbig-rigid.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/newcenters2.xyz` & `pybigdft-1.0.6/source/notebooks/testfiles/newcenters2.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/three.xyz` & `pybigdft-1.0.6/source/notebooks/testfiles/three.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/notebooks/testfiles/two.xyz` & `pybigdft-1.0.6/source/notebooks/testfiles/two.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/sphinx_static/bigdft-logo-reduced.svg` & `pybigdft-1.0.6/source/sphinx_static/bigdft-logo-reduced.svg`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/sphinx_static/logo-bigdft-white.svg` & `pybigdft-1.0.6/source/sphinx_static/logo-bigdft-white.svg`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/source/sphinx_static/logo_header.png` & `pybigdft-1.0.6/source/sphinx_static/logo_header.png`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/.gitignore` & `pybigdft-1.0.6/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,14 @@
 *~
 v1.12.2.tar.gz
 ntpoly*
 openbabel-3-0-0.tar.gz
 simgrid-dev
 swig-*
 PyBigDFT/source/tutorials/runs
-boost
 rdkit*
 biopython*
 ase*
 mpi4py*
 bigpoly*
 pdbfixer*
 openmm*
```

### Comparing `pybigdft-1.0.5/COPYING` & `pybigdft-1.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.5/pyproject.toml` & `pybigdft-1.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyBigDFT"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="William Dawson", email="william.dawson@riken.jp"},
   { name="Damien Caliste", email="Damien.Caliste@cea.fr"},
   { name="Luigi Genovese", email="Luigi.Genovese@cea.fr"},
 ]
 
 description="Python utilities for BigDFT"
```

### Comparing `pybigdft-1.0.5/PKG-INFO` & `pybigdft-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBigDFT
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python utilities for BigDFT
 Project-URL: Homepage, https://bigdft.org
 Project-URL: Bug Tracker, https://gitlab.com/l_sim/bigdft-suite/-/issues
 Author-email: William Dawson <william.dawson@riken.jp>, Damien Caliste <Damien.Caliste@cea.fr>, Luigi Genovese <Luigi.Genovese@cea.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

