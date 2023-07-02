# Comparing `tmp/adao-9.8.0.2.tar.gz` & `tmp/adao-9.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adao-9.8.0.2.tar", last modified: Sat Dec 11 09:42:23 2021, max compression
+gzip compressed data, was "adao-9.9.0.1.tar", last modified: Wed Jun  1 14:11:32 2022, max compression
```

## Comparing `adao-9.8.0.2.tar` & `adao-9.9.0.1.tar`

### file list

```diff
@@ -1,117 +1,140 @@
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.895354 adao-9.8.0.2/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    26430 2021-12-12 11:12:12.000000 adao-9.8.0.2/COPYING.txt
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)       95 2021-12-12 11:12:12.000000 adao-9.8.0.2/MANIFEST.in
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     6408 2021-12-11 09:42:23.895354 adao-9.8.0.2/PKG-INFO
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5158 2021-12-12 11:12:12.000000 adao-9.8.0.2/README.txt
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.887354 adao-9.8.0.2/adao/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5746 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2425 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/adaoBuilder.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.887354 adao-9.8.0.2/adao/daAlgorithms/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     8487 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/3DVAR.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5814 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/4DVAR.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     7529 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/AdjointTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    11204 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/Blue.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    22568 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/DerivativeFreeOptimization.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    13327 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/DifferentialEvolution.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5586 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/EnsembleBlue.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     9776 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/EnsembleKalmanFilter.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    11372 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/ExtendedBlue.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4896 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/ExtendedKalmanFilter.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     9678 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/FunctionTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    16610 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/GradientTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5758 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/InputValuesTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3763 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/KalmanFilter.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     6044 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/LinearLeastSquares.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    17223 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/LinearityTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4120 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/LocalSensitivityTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    16141 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/NonLinearLeastSquares.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3919 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/ObserverTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     9597 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/ParallelFunctionTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    13642 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/ParticleSwarmOptimization.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     8434 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/QuantileRegression.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    10483 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/SamplingTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    12765 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/TabuSearch.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     8915 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/TangentTest.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5740 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/UnscentedKalmanFilter.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      900 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    17142 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daAlgorithms/lbfgsbhlt.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daCore/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    37646 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/Aidsm.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     1455 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/AssimilationStudy.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)   126958 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/BasicObjects.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     6808 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/ExtendedLogging.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    62883 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/Interfaces.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)   215430 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/NumericObjects.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    37862 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/Persistence.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    18109 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/PlatformInfo.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     8788 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/Reporting.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    17248 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/Templates.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      900 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     1202 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daCore/version.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daEficas/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)   162906 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/ADAO_Cata_V0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      927 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2531 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/configuration_ADAO.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     1375 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/convert_adao.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    24659 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/generator_adao.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     1007 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/prefs.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2868 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/prefs_ADAO.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4036 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV7_4_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4036 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV7_5_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4036 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV7_5_1ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV7_6_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV7_7_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV7_8_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV8_1_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV8_2_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV8_3_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV8_4_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV8_5_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV8_6_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV9_2_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV9_3_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV9_4_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV9_5_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV9_6_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2969 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOV9_7_0ToV9_8_0.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4035 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficas/traduitADAOsansToV9_8_0.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daEficasWrapper/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      927 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficasWrapper/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     6416 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daEficasWrapper/adaoEficasWrapper.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daGUI/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     2050 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGUI/ADAO.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3740 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGUI/ADAOGUI.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      900 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGUI/__init__.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daGuiImpl/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5239 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/ADAOGUI_impl.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      927 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     6641 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/adaoCase.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4300 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/adaoGuiHelper.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    18905 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/adaoGuiManager.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     5535 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/adaoModuleHelper.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4036 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daGuiImpl/adaoStudyEditor.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daNumerics/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      900 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daNumerics/__init__.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.891354 adao-9.8.0.2/adao/daUtils/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      927 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daUtils/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3324 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daUtils/adaoEficasEvent.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     1968 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daUtils/adaoLogger.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     4588 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daUtils/enumerate.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.895354 adao-9.8.0.2/adao/daYacsIntegration/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      958 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsIntegration/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    19169 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsIntegration/daOptimizerLoop.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    12323 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsIntegration/daStudy.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.895354 adao-9.8.0.2/adao/daYacsSchemaCreator/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      926 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsSchemaCreator/__init__.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    10592 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsSchemaCreator/help_methods.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    11487 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsSchemaCreator/infos_daComposant.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)    64816 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsSchemaCreator/methods.py
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3000 2021-12-12 11:12:12.000000 adao-9.8.0.2/adao/daYacsSchemaCreator/run.py
-drwxr-xr-x   0 ahbhhjp  (62034) rdusers  (61000)        0 2021-12-11 09:42:23.887354 adao-9.8.0.2/adao.egg-info/
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     6408 2021-12-11 09:42:23.000000 adao-9.8.0.2/adao.egg-info/PKG-INFO
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3380 2021-12-11 09:42:23.000000 adao-9.8.0.2/adao.egg-info/SOURCES.txt
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)        1 2021-12-11 09:42:23.000000 adao-9.8.0.2/adao.egg-info/dependency_links.txt
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)       12 2021-12-11 09:42:23.000000 adao-9.8.0.2/adao.egg-info/requires.txt
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)      173 2021-12-11 09:42:23.000000 adao-9.8.0.2/adao.egg-info/top_level.txt
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)       38 2021-12-11 09:42:23.895354 adao-9.8.0.2/setup.cfg
--rw-r--r--   0 ahbhhjp  (62034) rdusers  (61000)     3120 2021-12-12 11:12:12.000000 adao-9.8.0.2/setup.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    26430 2022-05-02 10:12:12.000000 adao-9.9.0.1/COPYING.txt
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)       95 2022-05-02 10:12:12.000000 adao-9.9.0.1/MANIFEST.in
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     6409 2022-06-01 14:11:32.468037 adao-9.9.0.1/PKG-INFO
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5179 2022-05-02 10:12:12.000000 adao-9.9.0.1/README.txt
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.460037 adao-9.9.0.1/adao/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5759 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     2442 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/adaoBuilder.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.460037 adao-9.9.0.1/adao/daAlgorithms/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     8674 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/3DVAR.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5843 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/4DVAR.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     7085 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/AdjointTest.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.464037 adao-9.9.0.1/adao/daAlgorithms/Atoms/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      900 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13559 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/c2ukf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12596 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/cekf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     9149 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/ecwblue.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     9286 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/ecwexblue.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4454 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/ecwlls.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12131 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/ecwnlls.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     7243 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/ecwstdkf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     7894 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/enks.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    19031 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/etkf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    11837 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/exkf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13310 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/ienkf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    14431 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/incr3dvar.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    17859 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/lbfgsbhlt.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13650 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/mlef.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4478 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/mmqr.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12805 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/psas3dvar.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13676 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/senkf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13013 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/std3dvar.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12014 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/std4dvar.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12056 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/uskf.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13532 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Atoms/van3dvar.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5890 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/Blue.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    22299 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/DerivativeFreeOptimization.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13043 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/DifferentialEvolution.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5571 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/EnsembleBlue.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    10267 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/EnsembleKalmanFilter.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5935 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/ExtendedBlue.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4887 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/ExtendedKalmanFilter.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     9620 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/FunctionTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    16297 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/GradientTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5738 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/InputValuesTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4521 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/KalmanFilter.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4176 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/LinearLeastSquares.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    16246 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/LinearityTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4087 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/LocalSensitivityTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     6350 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/NonLinearLeastSquares.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3904 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/ObserverTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     9541 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/ParallelFunctionTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    13396 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/ParticleSwarmOptimization.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     7583 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/QuantileRegression.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    10429 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/SamplingTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12501 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/TabuSearch.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     8468 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/TangentTest.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5691 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/UnscentedKalmanFilter.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      900 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daAlgorithms/__init__.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.464037 adao-9.9.0.1/adao/daCore/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    37655 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/Aidsm.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     1456 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/AssimilationStudy.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)   123928 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/BasicObjects.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     6809 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/ExtendedLogging.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    64158 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/Interfaces.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    48959 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/NumericObjects.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    42872 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/Persistence.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    18651 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/PlatformInfo.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     8842 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/Reporting.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    17161 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/Templates.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      900 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     1215 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daCore/version.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daEficas/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)   164941 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/ADAO_Cata_V0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      927 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     2490 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/configuration_ADAO.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     1375 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/convert_adao.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    24661 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/generator_adao.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     1007 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/prefs.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     2868 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/prefs_ADAO.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4162 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV7_4_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4162 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV7_5_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4162 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV7_5_1ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV7_6_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV7_7_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV7_8_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV8_1_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV8_2_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV8_3_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV8_4_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV8_5_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV8_6_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_2_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_3_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_4_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_5_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_6_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_7_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3095 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOV9_8_0ToV9_9_0.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4162 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficas/traduitADAOsansToV9_9_0.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daEficasWrapper/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      927 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficasWrapper/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     6416 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daEficasWrapper/adaoEficasWrapper.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daGUI/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     2336 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGUI/ADAO.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3740 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGUI/ADAOGUI.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      900 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGUI/__init__.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daGuiImpl/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     5239 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/ADAOGUI_impl.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      927 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     6843 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/adaoCase.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4300 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/adaoGuiHelper.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    18905 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/adaoGuiManager.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4951 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/adaoModuleHelper.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4036 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daGuiImpl/adaoStudyEditor.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daNumerics/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      900 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daNumerics/__init__.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daUtils/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      927 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daUtils/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3324 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daUtils/adaoEficasEvent.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     1968 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daUtils/adaoLogger.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4611 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daUtils/enumerate.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daYacsIntegration/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      958 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsIntegration/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    19169 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsIntegration/daOptimizerLoop.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    12323 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsIntegration/daStudy.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.468037 adao-9.9.0.1/adao/daYacsSchemaCreator/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      926 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsSchemaCreator/__init__.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    10592 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsSchemaCreator/help_methods.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    11487 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsSchemaCreator/infos_daComposant.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)    64816 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsSchemaCreator/methods.py
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3034 2022-05-02 10:12:12.000000 adao-9.9.0.1/adao/daYacsSchemaCreator/run.py
+drwxr-xr-x   0 D18530   (62034) rdusers  (61000)        0 2022-06-01 14:11:32.460037 adao-9.9.0.1/adao.egg-info/
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     6409 2022-06-01 14:11:32.000000 adao-9.9.0.1/adao.egg-info/PKG-INFO
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     4147 2022-06-01 14:11:32.000000 adao-9.9.0.1/adao.egg-info/SOURCES.txt
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)        1 2022-06-01 14:11:32.000000 adao-9.9.0.1/adao.egg-info/dependency_links.txt
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)       12 2022-06-01 14:11:32.000000 adao-9.9.0.1/adao.egg-info/requires.txt
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)      197 2022-06-01 14:11:32.000000 adao-9.9.0.1/adao.egg-info/top_level.txt
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)       38 2022-06-01 14:11:32.468037 adao-9.9.0.1/setup.cfg
+-rw-r--r--   0 D18530   (62034) rdusers  (61000)     3155 2022-05-02 10:12:12.000000 adao-9.9.0.1/setup.py
```

### Comparing `adao-9.8.0.2/COPYING.txt` & `adao-9.9.0.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `adao-9.8.0.2/PKG-INFO` & `adao-9.9.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: adao
-Version: 9.8.0.2
+Version: 9.9.0.1
 Summary: A module for Data Assimilation and Optimization
 Home-page: http://www.salome-platform.org/
 Author: Jean-Philippe Argaud
 Author-email: jean-philippe.argaud@edf.fr
 License: GNU Library or Lesser General Public License (LGPL)
 Keywords: optimization,data assimilation,calibration,interpolation,inverse problem,tunning,minimization,black-box,checking,3D-Var,4D-Var,Filtering,Kalman,Ensemble,EnKF,UKF,BLUE,Regression,Quantile,V&V,Tabu Search,DFO,Derivative Free Optimization,PSO,Particle Swarm Optimization,Swarm,Gradient Test,Adjoint Test
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: COPYING.txt
 
 =====================================================
 ADAO: A module for Data Assimilation and Optimization
 =====================================================
 
@@ -36,20 +35,20 @@
 information coming from experimental measurements or observations, and from
 numerical *a priori* models, including information about their errors. Parts of
 the framework are also known under the names of *calibration*, *adjustment*,
 *state estimation*, *parameter estimation*, *parameter adjustment*, *inverse
 problems*, *Bayesian estimation*, *optimal interpolation*, *mathematical
 regularization*, *meta-heuristics for optimization*, *model reduction*, *data
 smoothing*, etc. More details can be found in the full ADAO documentation (see
-https://www.salome-platform.org/).
+https://www.salome-platform.org/ User Documentation dedicated section).
 
 Only the use of ADAO text programming interface (API/TUI) is introduced
 here. This interface gives ability to create a calculation object in a
 similar way than the case building obtained through the graphical
-interface (GUI). When one wants to elaborate "by hand" the TUI
+interface (GUI). When one wants to elaborate directly the TUI
 calculation case, it is recommended to extensively use all the ADAO
 module documentation, and to go back if necessary to the graphical
 interface (GUI), to get all the elements allowing to correctly set the
 commands.
 
 A simple setup example of an ADAO TUI calculation case
 ------------------------------------------------------
@@ -93,15 +92,15 @@
 ------------------------
 
 The license for this module is the GNU Lesser General Public License
 (Lesser GPL), as stated here and in the source files::
 
     <ADAO, a module for Data Assimilation and Optimization>
 
-    Copyright (C) 2008-2021 EDF R&D
+    Copyright (C) 2008-2022 EDF R&D
 
     This library is free software; you can redistribute it and/or
     modify it under the terms of the GNU Lesser General Public
     License as published by the Free Software Foundation; either
     version 2.1 of the License, or (at your option) any later version.
 
     This library is distributed in the hope that it will be useful,
@@ -111,25 +110,22 @@
 
     You should have received a copy of the GNU Lesser General Public
     License along with this library; if not, write to the Free Software
     Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
     See http://www.salome-platform.org/
 
-In addition, it is requested that any publication or presentation describing
+In addition, it is requested that any publication or presentation, describing
 work using this module, or any commercial or non-commercial product using it,
-cite at least one of at least one of the references below with the current year
-added:
+cite at least one of the references below with the current year added:
 
     * *ADAO, a module for Data Assimilation and Optimization*,
       http://www.salome-platform.org/
 
     * *ADAO, un module pour l'Assimilation de Données et l'Aide à
       l'Optimisation*, http://www.salome-platform.org/
 
     * *SALOME The Open Source Integration Platform for Numerical Simulation*,
       http://www.salome-platform.org/
 
 The documentation of the module is also covered by the license and the
 requirement of quoting.
-
-
```

### Comparing `adao-9.8.0.2/README.txt` & `adao-9.9.0.1/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 information coming from experimental measurements or observations, and from
 numerical *a priori* models, including information about their errors. Parts of
 the framework are also known under the names of *calibration*, *adjustment*,
 *state estimation*, *parameter estimation*, *parameter adjustment*, *inverse
 problems*, *Bayesian estimation*, *optimal interpolation*, *mathematical
 regularization*, *meta-heuristics for optimization*, *model reduction*, *data
 smoothing*, etc. More details can be found in the full ADAO documentation (see
-https://www.salome-platform.org/).
+https://www.salome-platform.org/ User Documentation dedicated section).
 
 Only the use of ADAO text programming interface (API/TUI) is introduced
 here. This interface gives ability to create a calculation object in a
 similar way than the case building obtained through the graphical
-interface (GUI). When one wants to elaborate "by hand" the TUI
+interface (GUI). When one wants to elaborate directly the TUI
 calculation case, it is recommended to extensively use all the ADAO
 module documentation, and to go back if necessary to the graphical
 interface (GUI), to get all the elements allowing to correctly set the
 commands.
 
 A simple setup example of an ADAO TUI calculation case
 ------------------------------------------------------
@@ -69,15 +69,15 @@
 ------------------------
 
 The license for this module is the GNU Lesser General Public License
 (Lesser GPL), as stated here and in the source files::
 
     <ADAO, a module for Data Assimilation and Optimization>
 
-    Copyright (C) 2008-2021 EDF R&D
+    Copyright (C) 2008-2022 EDF R&D
 
     This library is free software; you can redistribute it and/or
     modify it under the terms of the GNU Lesser General Public
     License as published by the Free Software Foundation; either
     version 2.1 of the License, or (at your option) any later version.
 
     This library is distributed in the hope that it will be useful,
@@ -87,18 +87,17 @@
 
     You should have received a copy of the GNU Lesser General Public
     License along with this library; if not, write to the Free Software
     Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
     See http://www.salome-platform.org/
 
-In addition, it is requested that any publication or presentation describing
+In addition, it is requested that any publication or presentation, describing
 work using this module, or any commercial or non-commercial product using it,
-cite at least one of at least one of the references below with the current year
-added:
+cite at least one of the references below with the current year added:
 
     * *ADAO, a module for Data Assimilation and Optimization*,
       http://www.salome-platform.org/
 
     * *ADAO, un module pour l'Assimilation de Données et l'Aide à
       l'Optimisation*, http://www.salome-platform.org/
```

### Comparing `adao-9.8.0.2/adao/__init__.py` & `adao-9.9.0.1/adao/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -87,15 +87,15 @@
 ------------------------
 
 The license for this module is the GNU Lesser General Public License
 (Lesser GPL), as stated here and in the source files::
 
     <ADAO, a module for Data Assimilation and Optimization>
 
-    Copyright (C) 2008-2021 EDF R&D
+    Copyright (C) 2008-2022 EDF R&D
 
     This library is free software; you can redistribute it and/or
     modify it under the terms of the GNU Lesser General Public
     License as published by the Free Software Foundation; either
     version 2.1 of the License, or (at your option) any later version.
 
     This library is distributed in the hope that it will be useful,
@@ -123,12 +123,12 @@
 requirement of quoting.
 """
 
 import os, sys, logging
 adao_py_dir = os.path.abspath(os.path.dirname(__file__))
 sys.path.insert(0, adao_py_dir)
 
-from daCore.version import name, version, year, date
+from daCore.version import name, version, year, date, __version__
 try:
     from daYacsIntegration.daOptimizerLoop import *
 except:
     logging.debug("INIT Pas de chargement initial de daOptimizerLoop")
```

### Comparing `adao-9.8.0.2/adao/adaoBuilder.py` & `adao-9.9.0.1/adao/adaoBuilder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -44,23 +44,23 @@
 
         See associated up-to-date documentation for details of commands.
 """
 __author__ = "Jean-Philippe ARGAUD"
 __all__ = ["New"]
 
 from daCore.Aidsm import Aidsm as _Aidsm
-from daCore.version import name, version, year, date
+from daCore.version import name, version, year, date, __version__
 
 # ==============================================================================
 class New(_Aidsm):
     """
     Generic ADAO TUI builder
     """
-    def __init__(self, name = ""):
-        _Aidsm.__init__(self, name)
+    def __init__(self, __name = ""):
+        _Aidsm.__init__(self, __name)
 
 class Gui(object):
     """
     Generic ADAO GUI builder
     """
     def __init__(self):
         from daCore.Interfaces import EficasGUI
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/3DVAR.py` & `adao-9.9.0.1/adao/daAlgorithms/3DVAR.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,64 +16,66 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging, numpy
+import numpy
 from daCore import BasicObjects, NumericObjects
+from daAlgorithms.Atoms import std3dvar, van3dvar, incr3dvar, psas3dvar
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "3DVAR")
         self.defineRequiredParameter(
-            name     = "Minimizer",
-            default  = "LBFGSB",
-            typecast = str,
-            message  = "Minimiseur utilisé",
-            listval  = [
-                "LBFGSB",
-                "TNC",
-                "CG",
-                "NCG",
-                "BFGS",
-                ],
-            )
-        self.defineRequiredParameter(
             name     = "Variant",
             default  = "3DVAR",
             typecast = str,
             message  = "Variant ou formulation de la méthode",
             listval  = [
                 "3DVAR",
                 "3DVAR-VAN",
                 "3DVAR-Incr",
                 "3DVAR-PSAS",
                 ],
             listadv  = [
+                "OneCorrection",
                 "3DVAR-Std",
                 "Incr3DVAR",
-                "OneCycle3DVAR-Std",
+                ],
+            )
+        self.defineRequiredParameter(
+            name     = "Minimizer",
+            default  = "LBFGSB",
+            typecast = str,
+            message  = "Minimiseur utilisé",
+            listval  = [
+                "LBFGSB",
+                "TNC",
+                "CG",
+                "NCG",
+                "BFGS",
                 ],
             )
         self.defineRequiredParameter(
             name     = "EstimationOf",
             default  = "Parameters",
             typecast = str,
             message  = "Estimation d'état ou de paramètres",
             listval  = ["State", "Parameters"],
             )
         self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
+            name     = "MaximumNumberOfIterations",
             default  = 15000,
             typecast = int,
             message  = "Nombre maximal de pas d'optimisation",
             minval   = -1,
+            oldname  = "MaximumNumberOfSteps",
             )
         self.defineRequiredParameter(
             name     = "CostDecrementTolerance",
             default  = 1.e-7,
             typecast = float,
             message  = "Diminution relative minimale du coût lors de l'arrêt",
             minval   = 0.,
@@ -115,17 +117,19 @@
                 "CostFunctionJb",
                 "CostFunctionJbAtCurrentOptimum",
                 "CostFunctionJo",
                 "CostFunctionJoAtCurrentOptimum",
                 "CurrentIterationNumber",
                 "CurrentOptimum",
                 "CurrentState",
+                "CurrentStepNumber",
                 "ForecastState",
                 "IndexOfOptimum",
                 "Innovation",
+                "InnovationAtCurrentAnalysis",
                 "InnovationAtCurrentState",
                 "JacobianMatrixAtBackground",
                 "JacobianMatrixAtOptimum",
                 "KalmanGainAtOptimum",
                 "MahalanobisConsistency",
                 "OMA",
                 "OMB",
@@ -176,41 +180,41 @@
         self.defineRequiredParameter(
             name     = "InitializationPoint",
             typecast = numpy.ravel,
             message  = "État initial imposé (par défaut, c'est l'ébauche si None)",
             )
         self.requireInputArguments(
             mandatory= ("Xb", "Y", "HO", "R", "B" ),
+            optional = ("U", "EM", "CM", "Q"),
             )
         self.setAttributes(tags=(
             "DataAssimilation",
             "NonLinear",
             "Variational",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
-        # Default 3DVAR
         if   self._parameters["Variant"] in ["3DVAR", "3DVAR-Std"]:
-            NumericObjects.multi3dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q, NumericObjects.std3dvar)
+            NumericObjects.multiXOsteps(self, Xb, Y, U, HO, EM, CM, R, B, Q, std3dvar.std3dvar)
         #
         elif self._parameters["Variant"] == "3DVAR-VAN":
-            NumericObjects.multi3dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q, NumericObjects.van3dvar)
+            NumericObjects.multiXOsteps(self, Xb, Y, U, HO, EM, CM, R, B, Q, van3dvar.van3dvar)
         #
         elif self._parameters["Variant"] in ["3DVAR-Incr", "Incr3DVAR"]:
-            NumericObjects.multi3dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q, NumericObjects.incr3dvar)
+            NumericObjects.multiXOsteps(self, Xb, Y, U, HO, EM, CM, R, B, Q, incr3dvar.incr3dvar)
         #
         elif self._parameters["Variant"] == "3DVAR-PSAS":
-            NumericObjects.multi3dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q, NumericObjects.psas3dvar)
+            NumericObjects.multiXOsteps(self, Xb, Y, U, HO, EM, CM, R, B, Q, psas3dvar.psas3dvar)
         #
         #--------------------------
-        elif self._parameters["Variant"] == "OneCycle3DVAR-Std":
-            NumericObjects.std3dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+        elif self._parameters["Variant"] == "OneCorrection":
+            std3dvar.std3dvar(self, Xb, Y, U, HO, CM, R, B)
         #
         #--------------------------
         else:
             raise ValueError("Error in Variant name: %s"%self._parameters["Variant"])
         #
         self._post_run(HO)
         return 0
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/4DVAR.py` & `adao-9.9.0.1/adao/daAlgorithms/4DVAR.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
-import numpy, scipy.optimize, scipy.version
+import numpy
+from daCore import BasicObjects
+from daAlgorithms.Atoms import std4dvar
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "4DVAR")
         self.defineRequiredParameter(
             name     = "ConstrainedBy",
@@ -58,19 +58,20 @@
             name     = "Minimizer",
             default  = "LBFGSB",
             typecast = str,
             message  = "Minimiseur utilisé",
             listval  = ["LBFGSB","TNC", "CG", "NCG", "BFGS"],
             )
         self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
+            name     = "MaximumNumberOfIterations",
             default  = 15000,
             typecast = int,
             message  = "Nombre maximal de pas d'optimisation",
             minval   = -1,
+            oldname  = "MaximumNumberOfSteps",
             )
         self.defineRequiredParameter(
             name     = "CostDecrementTolerance",
             default  = 1.e-7,
             typecast = float,
             message  = "Diminution relative minimale du coût lors de l'arrêt",
             minval   = 0.,
@@ -122,30 +123,30 @@
         self.defineRequiredParameter(
             name     = "InitializationPoint",
             typecast = numpy.ravel,
             message  = "État initial imposé (par défaut, c'est l'ébauche si None)",
             )
         self.requireInputArguments(
             mandatory= ("Xb", "Y", "HO", "EM", "R", "B" ),
-            optional = ("U", "CM"),
+            optional = ("U", "CM", "Q"),
             )
         self.setAttributes(tags=(
             "DataAssimilation",
             "NonLinear",
             "Variational",
             "Dynamic",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         # Default 4DVAR
         if   self._parameters["Variant"] in ["4DVAR", "4DVAR-Std"]:
-            NumericObjects.std4dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+            std4dvar.std4dvar(self, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         else:
             raise ValueError("Error in Variant name: %s"%self._parameters["Variant"])
         #
         self._post_run(HO)
         return 0
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/AdjointTest.py` & `adao-9.9.0.1/adao/daAlgorithms/AdjointTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,20 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
-from daCore import BasicObjects, PlatformInfo
 import numpy
+from daCore import BasicObjects, NumericObjects, PlatformInfo
 mpr = PlatformInfo.PlatformInfo().MachinePrecision()
-if sys.version_info.major > 2:
-    unicode = str
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "ADJOINTTEST")
         self.defineRequiredParameter(
             name     = "ResiduFormula",
@@ -91,40 +88,34 @@
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         Hm = HO["Direct"].appliedTo
         Ht = HO["Tangent"].appliedInXTo
         Ha = HO["Adjoint"].appliedInXTo
         #
-        # ----------
         Perturbations = [ 10**i for i in range(self._parameters["EpsilonMinimumExponent"],1) ]
         Perturbations.reverse()
         #
-        X       = numpy.asmatrix(numpy.ravel( Xb )).T
-        NormeX  = numpy.linalg.norm( X )
+        Xn       = numpy.ravel( Xb ).reshape((-1,1))
+        NormeX  = numpy.linalg.norm( Xn )
         if Y is None:
-            Y = numpy.asmatrix(numpy.ravel( Hm( X ) )).T
-        Y = numpy.asmatrix(numpy.ravel( Y )).T
-        NormeY = numpy.linalg.norm( Y )
+            Yn = numpy.ravel( Hm( Xn ) ).reshape((-1,1))
+        else:
+            Yn = numpy.ravel( Y ).reshape((-1,1))
+        NormeY = numpy.linalg.norm( Yn )
         if self._toStore("CurrentState"):
-            self.StoredVariables["CurrentState"].store( numpy.ravel(X) )
+            self.StoredVariables["CurrentState"].store( Xn )
         if self._toStore("SimulatedObservationAtCurrentState"):
-            self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(Y) )
-        #
-        if len(self._parameters["InitialDirection"]) == 0:
-            dX0 = []
-            for v in X.A1:
-                if abs(v) > 1.e-8:
-                    dX0.append( numpy.random.normal(0.,abs(v)) )
-                else:
-                    dX0.append( numpy.random.normal(0.,X.mean()) )
-        else:
-            dX0 = numpy.asmatrix(numpy.ravel( self._parameters["InitialDirection"] ))
+            self.StoredVariables["SimulatedObservationAtCurrentState"].store( Yn )
         #
-        dX0 = float(self._parameters["AmplitudeOfInitialDirection"]) * numpy.matrix( dX0 ).T
+        dX0 = NumericObjects.SetInitialDirection(
+            self._parameters["InitialDirection"],
+            self._parameters["AmplitudeOfInitialDirection"],
+            Xn,
+            )
         #
         # Entete des resultats
         # --------------------
         __marge =  12*u" "
         __precision = u"""
             Remarque : les nombres inferieurs a %.0e (environ) representent un zero
                        a la precision machine.\n"""%mpr
@@ -136,39 +127,37 @@
               R(Alpha) = | < TangentF_X(dX) , Y > - < dX , AdjointF_X(Y) > |
 
             qui doit rester constamment egal a zero a la precision du calcul.
             On prend dX0 = Normal(0,X) et dX = Alpha*dX0. F est le code de calcul.
             Y doit etre dans l'image de F. S'il n'est pas donne, on prend Y = F(X).\n""" + __precision
         #
         if len(self._parameters["ResultTitle"]) > 0:
-            __rt = unicode(self._parameters["ResultTitle"])
+            __rt = str(self._parameters["ResultTitle"])
             msgs  = u"\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
             msgs += __marge + "    " + __rt + "\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
         else:
             msgs  = u""
         msgs += __msgdoc
         #
         __nbtirets = len(__entete) + 2
         msgs += "\n" + __marge + "-"*__nbtirets
         msgs += "\n" + __marge + __entete
         msgs += "\n" + __marge + "-"*__nbtirets
         #
-        Normalisation= -1
-        #
         # ----------
         for i,amplitude in enumerate(Perturbations):
             dX          = amplitude * dX0
             NormedX     = numpy.linalg.norm( dX )
             #
-            TangentFXdX = numpy.asmatrix( Ht( (X,dX) ) )
-            AdjointFXY  = numpy.asmatrix( Ha( (X,Y)  ) )
+            TangentFXdX = numpy.ravel( Ht( (Xn,dX) ) )
+            AdjointFXY  = numpy.ravel( Ha( (Xn,Yn)  ) )
             #
-            Residu = abs(float(numpy.dot( TangentFXdX.A1 , Y.A1 ) - numpy.dot( dX.A1 , AdjointFXY.A1 )))
+            Residu = abs(float(numpy.dot( TangentFXdX, Yn ) - numpy.dot( dX, AdjointFXY )))
             #
             msg = "  %2i  %5.0e   %9.3e   %9.3e   %9.3e   |  %9.3e"%(i,amplitude,NormeX,NormeY,NormedX,Residu)
             msgs += "\n" + __marge + msg
             #
             self.StoredVariables["Residu"].store( Residu )
         #
         msgs += "\n" + __marge + "-"*__nbtirets
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/Blue.py` & `adao-9.9.0.1/adao/daAlgorithms/DifferentialEvolution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,215 +16,271 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
-import numpy
+import numpy, logging, scipy.optimize
+from daCore import BasicObjects
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
-        BasicObjects.Algorithm.__init__(self, "BLUE")
+        BasicObjects.Algorithm.__init__(self, "DIFFERENTIALEVOLUTION")
+        self.defineRequiredParameter(
+            name     = "Minimizer",
+            default  = "BEST1BIN",
+            typecast = str,
+            message  = "Stratégie de minimisation utilisée",
+            listval  = [
+                "BEST1BIN",
+                "BEST1EXP",
+                "BEST2BIN",
+                "BEST2EXP",
+                "RAND1BIN",
+                "RAND1EXP",
+                "RAND2BIN",
+                "RAND2EXP",
+                "RANDTOBEST1BIN",
+                "RANDTOBEST1EXP",
+                ],
+            listadv  = [
+                "CURRENTTOBEST1EXP",
+                "CURRENTTOBEST1BIN",
+                ],
+            )
+        self.defineRequiredParameter(
+            name     = "MaximumNumberOfIterations",
+            default  = 15000,
+            typecast = int,
+            message  = "Nombre maximal de générations",
+            minval   = 0,
+            oldname  = "MaximumNumberOfSteps",
+            )
+        self.defineRequiredParameter(
+            name     = "MaximumNumberOfFunctionEvaluations",
+            default  = 15000,
+            typecast = int,
+            message  = "Nombre maximal d'évaluations de la fonction",
+            minval   = -1,
+            )
+        self.defineRequiredParameter(
+            name     = "SetSeed",
+            typecast = numpy.random.seed,
+            message  = "Graine fixée pour le générateur aléatoire",
+            )
+        self.defineRequiredParameter(
+            name     = "PopulationSize",
+            default  = 100,
+            typecast = int,
+            message  = "Taille approximative de la population à chaque génération",
+            minval   = 1,
+            )
+        self.defineRequiredParameter(
+            name     = "MutationDifferentialWeight_F",
+            default  = (0.5, 1),
+            typecast = tuple,
+            message  = "Poids différentiel de mutation, constant ou aléatoire dans l'intervalle, noté F",
+            minval   = 0.,
+            maxval   = 2.,
+            )
+        self.defineRequiredParameter(
+            name     = "CrossOverProbability_CR",
+            default  = 0.7,
+            typecast = float,
+            message  = "Probabilité de recombinaison ou de croisement, notée CR",
+            minval   = 0.,
+            maxval   = 1.,
+            )
+        self.defineRequiredParameter(
+            name     = "QualityCriterion",
+            default  = "AugmentedWeightedLeastSquares",
+            typecast = str,
+            message  = "Critère de qualité utilisé",
+            listval  = [
+                "AugmentedWeightedLeastSquares", "AWLS", "DA",
+                "WeightedLeastSquares", "WLS",
+                "LeastSquares", "LS", "L2",
+                "AbsoluteValue", "L1",
+                "MaximumError", "ME",
+                ],
+            )
         self.defineRequiredParameter(
             name     = "StoreInternalVariables",
             default  = False,
             typecast = bool,
             message  = "Stockage des variables internes ou intermédiaires du calcul",
             )
         self.defineRequiredParameter(
             name     = "StoreSupplementaryCalculations",
             default  = [],
             typecast = tuple,
             message  = "Liste de calculs supplémentaires à stocker et/ou effectuer",
             listval  = [
                 "Analysis",
-                "APosterioriCorrelations",
-                "APosterioriCovariance",
-                "APosterioriStandardDeviations",
-                "APosterioriVariances",
                 "BMA",
                 "CostFunctionJ",
-                "CostFunctionJAtCurrentOptimum",
                 "CostFunctionJb",
-                "CostFunctionJbAtCurrentOptimum",
                 "CostFunctionJo",
+                "CostFunctionJAtCurrentOptimum",
+                "CostFunctionJbAtCurrentOptimum",
                 "CostFunctionJoAtCurrentOptimum",
+                "CurrentIterationNumber",
                 "CurrentOptimum",
                 "CurrentState",
+                "IndexOfOptimum",
                 "Innovation",
-                "MahalanobisConsistency",
+                "InnovationAtCurrentState",
                 "OMA",
                 "OMB",
-                "SampledStateForQuantiles",
-                "SigmaBck2",
-                "SigmaObs2",
                 "SimulatedObservationAtBackground",
                 "SimulatedObservationAtCurrentOptimum",
                 "SimulatedObservationAtCurrentState",
                 "SimulatedObservationAtOptimum",
-                "SimulationQuantiles",
                 ]
             )
-        self.defineRequiredParameter(
-            name     = "Quantiles",
-            default  = [],
-            typecast = tuple,
-            message  = "Liste des valeurs de quantiles",
-            minval   = 0.,
-            maxval   = 1.,
-            )
-        self.defineRequiredParameter(
-            name     = "SetSeed",
-            typecast = numpy.random.seed,
-            message  = "Graine fixée pour le générateur aléatoire",
-            )
-        self.defineRequiredParameter(
-            name     = "NumberOfSamplesForQuantiles",
-            default  = 100,
-            typecast = int,
-            message  = "Nombre d'échantillons simulés pour le calcul des quantiles",
-            minval   = 1,
-            )
-        self.defineRequiredParameter(
-            name     = "SimulationForQuantiles",
-            default  = "Linear",
-            typecast = str,
-            message  = "Type de simulation en estimation des quantiles",
-            listval  = ["Linear", "NonLinear"]
-            )
         self.defineRequiredParameter( # Pas de type
-            name     = "StateBoundsForQuantiles",
-            message  = "Liste des paires de bornes pour les états utilisés en estimation des quantiles",
+            name     = "Bounds",
+            message  = "Liste des valeurs de bornes",
             )
         self.requireInputArguments(
             mandatory= ("Xb", "Y", "HO", "R", "B"),
             )
         self.setAttributes(tags=(
-            "DataAssimilation",
-            "Linear",
-            "Filter",
+            "Optimization",
+            "NonLinear",
+            "MetaHeuristic",
+            "Population",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
-        Hm = HO["Tangent"].asMatrix(Xb)
-        Hm = Hm.reshape(Y.size,Xb.size) # ADAO & check shape
-        Ha = HO["Adjoint"].asMatrix(Xb)
-        Ha = Ha.reshape(Xb.size,Y.size) # ADAO & check shape
-        #
-        if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
-            HXb = HO["AppliedInX"]["HXb"]
-        else:
-            HXb = Hm @ Xb
-        HXb = HXb.reshape((-1,1))
-        if Y.size != HXb.size:
-            raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
-        if max(Y.shape) != max(HXb.shape):
-            raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
+        len_X = numpy.asarray(Xb).size
+        popsize = round(self._parameters["PopulationSize"]/len_X)
+        maxiter = min(self._parameters["MaximumNumberOfIterations"],round(self._parameters["MaximumNumberOfFunctionEvaluations"]/(popsize*len_X) - 1))
+        logging.debug("%s Nombre maximal de générations = %i, taille de la population à chaque génération = %i"%(self._name, maxiter, popsize*len_X))
+        #
+        Hm = HO["Direct"].appliedTo
         #
         BI = B.getI()
         RI = R.getI()
         #
-        Innovation  = Y - HXb
-        #
-        # Calcul de la matrice de gain et de l'analyse
-        # --------------------------------------------
-        if Y.size <= Xb.size:
-            _A = R + numpy.dot(Hm, B * Ha)
-            _u = numpy.linalg.solve( _A , Innovation )
-            Xa = Xb + B * Ha * _u
-        else:
-            _A = BI + numpy.dot(Ha, RI * Hm)
-            _u = numpy.linalg.solve( _A , numpy.dot(Ha, RI * Innovation) )
-            Xa = Xb + _u
-        self.StoredVariables["Analysis"].store( Xa )
-        #
-        # Calcul de la fonction coût
-        # --------------------------
-        if self._parameters["StoreInternalVariables"] or \
-            self._toStore("CostFunctionJ")  or self._toStore("CostFunctionJAtCurrentOptimum") or \
-            self._toStore("CostFunctionJb") or self._toStore("CostFunctionJbAtCurrentOptimum") or \
-            self._toStore("CostFunctionJo") or self._toStore("CostFunctionJoAtCurrentOptimum") or \
-            self._toStore("OMA") or \
-            self._toStore("SigmaObs2") or \
-            self._toStore("MahalanobisConsistency") or \
-            self._toStore("SimulatedObservationAtCurrentOptimum") or \
-            self._toStore("SimulatedObservationAtCurrentState") or \
-            self._toStore("SimulatedObservationAtOptimum") or \
-            self._toStore("SimulationQuantiles"):
-            HXa = Hm @ Xa
-            oma = Y - HXa
-        if self._parameters["StoreInternalVariables"] or \
-            self._toStore("CostFunctionJ")  or self._toStore("CostFunctionJAtCurrentOptimum") or \
-            self._toStore("CostFunctionJb") or self._toStore("CostFunctionJbAtCurrentOptimum") or \
-            self._toStore("CostFunctionJo") or self._toStore("CostFunctionJoAtCurrentOptimum") or \
-            self._toStore("MahalanobisConsistency"):
-            Jb  = float( 0.5 * (Xa - Xb).T * (BI * (Xa - Xb)) )
-            Jo  = float( 0.5 * oma.T * (RI * oma) )
-            J   = Jb + Jo
+        def CostFunction(x, QualityMeasure="AugmentedWeightedLeastSquares"):
+            _X  = numpy.ravel( x ).reshape((-1,1))
+            _HX = numpy.ravel( Hm( _X ) ).reshape((-1,1))
+            _Innovation = Y - _HX
+            self.StoredVariables["CurrentState"].store( _X )
+            if self._toStore("SimulatedObservationAtCurrentState") or \
+                self._toStore("SimulatedObservationAtCurrentOptimum"):
+                self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
+            if self._toStore("InnovationAtCurrentState"):
+                self.StoredVariables["InnovationAtCurrentState"].store( _Innovation )
+            #
+            if QualityMeasure in ["AugmentedWeightedLeastSquares","AWLS","DA"]:
+                if BI is None or RI is None:
+                    raise ValueError("Background and Observation error covariance matrices has to be properly defined!")
+                Jb  = 0.5 * (_X - Xb).T @ (BI @ (_X - Xb))
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
+            elif QualityMeasure in ["WeightedLeastSquares","WLS"]:
+                if RI is None:
+                    raise ValueError("Observation error covariance matrix has to be properly defined!")
+                Jb  = 0.
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
+            elif QualityMeasure in ["LeastSquares","LS","L2"]:
+                Jb  = 0.
+                Jo  = 0.5 * _Innovation.T @ _Innovation
+            elif QualityMeasure in ["AbsoluteValue","L1"]:
+                Jb  = 0.
+                Jo  = numpy.sum( numpy.abs(_Innovation) )
+            elif QualityMeasure in ["MaximumError","ME"]:
+                Jb  = 0.
+                Jo  = numpy.max( numpy.abs(_Innovation) )
+            #
+            J   = float( Jb ) + float( Jo )
+            #
+            self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
             self.StoredVariables["CostFunctionJb"].store( Jb )
             self.StoredVariables["CostFunctionJo"].store( Jo )
             self.StoredVariables["CostFunctionJ" ].store( J )
-            self.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( Jb )
-            self.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( Jo )
-            self.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( J )
-        #
-        # Calcul de la covariance d'analyse
-        # ---------------------------------
-        if self._toStore("APosterioriCovariance") or \
-            self._toStore("SimulationQuantiles"):
-            if   (Y.size <= Xb.size): K  = B * Ha * (R + numpy.dot(Hm, B * Ha)).I
-            elif (Y.size >  Xb.size): K = (BI + numpy.dot(Ha, RI * Hm)).I * Ha * RI
-            A = B - K * Hm * B
-            if min(A.shape) != max(A.shape):
-                raise ValueError("The %s a posteriori covariance matrix A is of shape %s, despites it has to be a squared matrix. There is an error in the observation operator, please check it."%(self._name,str(A.shape)))
-            if (numpy.diag(A) < 0).any():
-                raise ValueError("The %s a posteriori covariance matrix A has at least one negative value on its diagonal. There is an error in the observation operator, please check it."%(self._name,))
-            if logging.getLogger().level < logging.WARNING: # La verification n'a lieu qu'en debug
-                try:
-                    L = numpy.linalg.cholesky( A )
-                except:
-                    raise ValueError("The %s a posteriori covariance matrix A is not symmetric positive-definite. Please check your a priori covariances and your observation operator."%(self._name,))
-            self.StoredVariables["APosterioriCovariance"].store( A )
+            if self._toStore("IndexOfOptimum") or \
+                self._toStore("CurrentOptimum") or \
+                self._toStore("CostFunctionJAtCurrentOptimum") or \
+                self._toStore("CostFunctionJbAtCurrentOptimum") or \
+                self._toStore("CostFunctionJoAtCurrentOptimum") or \
+                self._toStore("SimulatedObservationAtCurrentOptimum"):
+                IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+            if self._toStore("IndexOfOptimum"):
+                self.StoredVariables["IndexOfOptimum"].store( IndexMin )
+            if self._toStore("CurrentOptimum"):
+                self.StoredVariables["CurrentOptimum"].store( self.StoredVariables["CurrentState"][IndexMin] )
+            if self._toStore("SimulatedObservationAtCurrentOptimum"):
+                self.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin] )
+            if self._toStore("CostFunctionJAtCurrentOptimum"):
+                self.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( self.StoredVariables["CostFunctionJ" ][IndexMin] )
+            if self._toStore("CostFunctionJbAtCurrentOptimum"):
+                self.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJb"][IndexMin] )
+            if self._toStore("CostFunctionJoAtCurrentOptimum"):
+                self.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJo"][IndexMin] )
+            return J
+        #
+        Xini = numpy.ravel(Xb)
+        #
+        # Minimisation de la fonctionnelle
+        # --------------------------------
+        nbPreviousSteps = self.StoredVariables["CostFunctionJ"].stepnumber()
+        #
+        optResults = scipy.optimize.differential_evolution(
+            CostFunction,
+            self._parameters["Bounds"],
+            strategy      = str(self._parameters["Minimizer"]).lower(),
+            maxiter       = maxiter,
+            popsize       = popsize,
+            mutation      = self._parameters["MutationDifferentialWeight_F"],
+            recombination = self._parameters["CrossOverProbability_CR"],
+            disp          = self._parameters["optdisp"],
+            )
+        #
+        IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+        MinJ     = self.StoredVariables["CostFunctionJ"][IndexMin]
+        Minimum  = self.StoredVariables["CurrentState"][IndexMin]
+        #
+        # Obtention de l'analyse
+        # ----------------------
+        Xa = Minimum
+        #
+        self.StoredVariables["Analysis"].store( Xa )
         #
         # Calculs et/ou stockages supplémentaires
         # ---------------------------------------
-        if self._parameters["StoreInternalVariables"] or self._toStore("CurrentState"):
-            self.StoredVariables["CurrentState"].store( Xa )
-        if self._toStore("CurrentOptimum"):
-            self.StoredVariables["CurrentOptimum"].store( Xa )
+        if self._toStore("OMA") or \
+            self._toStore("SimulatedObservationAtOptimum"):
+            if self._toStore("SimulatedObservationAtCurrentState"):
+                HXa = self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin]
+            elif self._toStore("SimulatedObservationAtCurrentOptimum"):
+                HXa = self.StoredVariables["SimulatedObservationAtCurrentOptimum"][-1]
+            else:
+                HXa = Hm(Xa)
+            HXa = HXa.reshape((-1,1))
+        if self._toStore("Innovation") or \
+            self._toStore("OMB") or \
+            self._toStore("SimulatedObservationAtBackground"):
+            HXb = Hm(Xb).reshape((-1,1))
+            Innovation = Y - HXb
         if self._toStore("Innovation"):
             self.StoredVariables["Innovation"].store( Innovation )
+        if self._toStore("OMB"):
+            self.StoredVariables["OMB"].store( Innovation )
         if self._toStore("BMA"):
             self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
         if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( oma )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( Innovation )
-        if self._toStore("SigmaObs2"):
-            TraceR = R.trace(Y.size)
-            self.StoredVariables["SigmaObs2"].store( float( Innovation.T @ oma ) / TraceR )
-        if self._toStore("SigmaBck2"):
-            self.StoredVariables["SigmaBck2"].store( float( (Innovation.T @ (Hm @ (Xa - Xb)))/(Hm * (B * Hm.T)).trace() ) )
-        if self._toStore("MahalanobisConsistency"):
-            self.StoredVariables["MahalanobisConsistency"].store( float( 2.*J/Innovation.size ) )
-        if self._toStore("SimulationQuantiles"):
-            H  = HO["Direct"].appliedTo
-            NumericObjects.QuantilesEstimations(self, A, Xa, HXa, H, Hm)
+            self.StoredVariables["OMA"].store( Y - HXa )
         if self._toStore("SimulatedObservationAtBackground"):
             self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
-        if self._toStore("SimulatedObservationAtCurrentState"):
-            self.StoredVariables["SimulatedObservationAtCurrentState"].store( HXa )
-        if self._toStore("SimulatedObservationAtCurrentOptimum"):
-            self.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( HXa )
         if self._toStore("SimulatedObservationAtOptimum"):
             self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
         #
         self._post_run(HO)
         return 0
 
 # ==============================================================================
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/DerivativeFreeOptimization.py` & `adao-9.9.0.1/adao/daAlgorithms/DerivativeFreeOptimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,16 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
+import numpy, logging, scipy.optimize
 from daCore import BasicObjects, PlatformInfo
-import numpy, scipy.optimize
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "DERIVATIVEFREEOPTIMIZATION")
         self.defineRequiredParameter(
             name     = "Minimizer",
@@ -39,19 +38,20 @@
                 "NEWUOA",
                 "POWELL",
                 "SIMPLEX",
                 "SUBPLEX",
                 ],
             )
         self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
+            name     = "MaximumNumberOfIterations",
             default  = 15000,
             typecast = int,
             message  = "Nombre maximal de pas d'optimisation",
             minval   = -1,
+            oldname  = "MaximumNumberOfSteps",
             )
         self.defineRequiredParameter(
             name     = "MaximumNumberOfFunctionEvaluations",
             default  = 15000,
             typecast = int,
             message  = "Nombre maximal d'évaluations de la fonction",
             minval   = -1,
@@ -70,19 +70,19 @@
             )
         self.defineRequiredParameter(
             name     = "QualityCriterion",
             default  = "AugmentedWeightedLeastSquares",
             typecast = str,
             message  = "Critère de qualité utilisé",
             listval  = [
-                "AugmentedWeightedLeastSquares","AWLS","DA",
-                "WeightedLeastSquares","WLS",
-                "LeastSquares","LS","L2",
-                "AbsoluteValue","L1",
-                "MaximumError","ME",
+                "AugmentedWeightedLeastSquares", "AWLS", "DA",
+                "WeightedLeastSquares", "WLS",
+                "LeastSquares", "LS", "L2",
+                "AbsoluteValue", "L1",
+                "MaximumError", "ME",
                 ],
             )
         self.defineRequiredParameter(
             name     = "StoreInternalVariables",
             default  = False,
             typecast = bool,
             message  = "Stockage des variables internes ou intermédiaires du calcul",
@@ -116,65 +116,58 @@
                 ]
             )
         self.defineRequiredParameter( # Pas de type
             name     = "Bounds",
             message  = "Liste des valeurs de bornes",
             )
         self.requireInputArguments(
-            mandatory= ("Xb", "Y", "HO", "R", "B" ),
+            mandatory= ("Xb", "Y", "HO", "R", "B"),
             )
         self.setAttributes(tags=(
             "Optimization",
             "NonLinear",
             "MetaHeuristic",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         if not PlatformInfo.has_nlopt and not self._parameters["Minimizer"] in ["COBYLA", "POWELL", "SIMPLEX"]:
             logging.warning("%s Minimization by SIMPLEX is forced because %s is unavailable (COBYLA, POWELL are also available)"%(self._name,self._parameters["Minimizer"]))
             self._parameters["Minimizer"] = "SIMPLEX"
         #
-        # Opérateurs
-        # ----------
         Hm = HO["Direct"].appliedTo
         #
-        # Précalcul des inversions de B et R
-        # ----------------------------------
         BI = B.getI()
         RI = R.getI()
         #
-        # Définition de la fonction-coût
-        # ------------------------------
         def CostFunction(x, QualityMeasure="AugmentedWeightedLeastSquares"):
-            _X  = numpy.asmatrix(numpy.ravel( x )).T
-            self.StoredVariables["CurrentState"].store( _X )
-            _HX = Hm( _X )
-            _HX = numpy.asmatrix(numpy.ravel( _HX )).T
+            _X  = numpy.ravel( x ).reshape((-1,1))
+            _HX = numpy.ravel( Hm( _X ) ).reshape((-1,1))
             _Innovation = Y - _HX
+            self.StoredVariables["CurrentState"].store( _X )
             if self._toStore("SimulatedObservationAtCurrentState") or \
                 self._toStore("SimulatedObservationAtCurrentOptimum"):
                 self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
             if self._toStore("InnovationAtCurrentState"):
                 self.StoredVariables["InnovationAtCurrentState"].store( _Innovation )
             #
             if QualityMeasure in ["AugmentedWeightedLeastSquares","AWLS","DA"]:
                 if BI is None or RI is None:
-                    raise ValueError("Background and Observation error covariance matrix has to be properly defined!")
-                Jb  = 0.5 * (_X - Xb).T * (BI * (_X - Xb))
-                Jo  = 0.5 * _Innovation.T * (RI * _Innovation)
+                    raise ValueError("Background and Observation error covariance matrices has to be properly defined!")
+                Jb  = 0.5 * (_X - Xb).T @ (BI @ (_X - Xb))
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
             elif QualityMeasure in ["WeightedLeastSquares","WLS"]:
                 if RI is None:
                     raise ValueError("Observation error covariance matrix has to be properly defined!")
                 Jb  = 0.
-                Jo  = 0.5 * (_Innovation).T * RI * (_Innovation)
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
             elif QualityMeasure in ["LeastSquares","LS","L2"]:
                 Jb  = 0.
-                Jo  = 0.5 * (_Innovation).T * (_Innovation)
+                Jo  = 0.5 * _Innovation.T @ _Innovation
             elif QualityMeasure in ["AbsoluteValue","L1"]:
                 Jb  = 0.
                 Jo  = numpy.sum( numpy.abs(_Innovation) )
             elif QualityMeasure in ["MaximumError","ME"]:
                 Jb  = 0.
                 Jo  = numpy.max( numpy.abs(_Innovation) )
             #
@@ -201,30 +194,28 @@
                 self.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( self.StoredVariables["CostFunctionJ" ][IndexMin] )
             if self._toStore("CostFunctionJbAtCurrentOptimum"):
                 self.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJb"][IndexMin] )
             if self._toStore("CostFunctionJoAtCurrentOptimum"):
                 self.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJo"][IndexMin] )
             return J
         #
-        # Point de démarrage de l'optimisation : Xini = Xb
-        # ------------------------------------
         Xini = numpy.ravel(Xb)
         if len(Xini) < 2 and self._parameters["Minimizer"] == "NEWUOA":
             raise ValueError("The minimizer %s can not be used when the optimisation state dimension is 1. Please choose another minimizer."%self._parameters["Minimizer"])
         #
         # Minimisation de la fonctionnelle
         # --------------------------------
         nbPreviousSteps = self.StoredVariables["CostFunctionJ"].stepnumber()
         #
         if self._parameters["Minimizer"] == "POWELL":
             Minimum, J_optimal, direc, niter, nfeval, rc = scipy.optimize.fmin_powell(
                 func        = CostFunction,
                 x0          = Xini,
                 args        = (self._parameters["QualityCriterion"],),
-                maxiter     = self._parameters["MaximumNumberOfSteps"]-1,
+                maxiter     = self._parameters["MaximumNumberOfIterations"]-1,
                 maxfun      = self._parameters["MaximumNumberOfFunctionEvaluations"],
                 xtol        = self._parameters["StateVariationTolerance"],
                 ftol        = self._parameters["CostDecrementTolerance"],
                 full_output = True,
                 disp        = self._parameters["optdisp"],
                 )
         elif self._parameters["Minimizer"] == "COBYLA" and not PlatformInfo.has_nlopt:
@@ -274,15 +265,15 @@
                 print("%s: minimum of J: %s"%(opt.get_algorithm_name(),opt.last_optimum_value()))
                 print("%s: return code: %i"%(opt.get_algorithm_name(),opt.last_optimize_result()))
         elif self._parameters["Minimizer"] == "SIMPLEX" and not PlatformInfo.has_nlopt:
             Minimum, J_optimal, niter, nfeval, rc = scipy.optimize.fmin(
                 func        = CostFunction,
                 x0          = Xini,
                 args        = (self._parameters["QualityCriterion"],),
-                maxiter     = self._parameters["MaximumNumberOfSteps"]-1,
+                maxiter     = self._parameters["MaximumNumberOfIterations"]-1,
                 maxfun      = self._parameters["MaximumNumberOfFunctionEvaluations"],
                 xtol        = self._parameters["StateVariationTolerance"],
                 ftol        = self._parameters["CostDecrementTolerance"],
                 full_output = True,
                 disp        = self._parameters["optdisp"],
                 )
         elif self._parameters["Minimizer"] == "SIMPLEX" and PlatformInfo.has_nlopt:
@@ -378,53 +369,54 @@
             opt.set_maxeval(self._parameters["MaximumNumberOfFunctionEvaluations"])
             Minimum = opt.optimize( Xini )
             if self._parameters["optdisp"]:
                 print("%s: optimal state: %s"%(opt.get_algorithm_name(),Minimum))
                 print("%s: minimum of J: %s"%(opt.get_algorithm_name(),opt.last_optimum_value()))
                 print("%s: return code: %i"%(opt.get_algorithm_name(),opt.last_optimize_result()))
         else:
-            raise ValueError("Error in Minimizer name: %s"%self._parameters["Minimizer"])
+            raise ValueError("Error in minimizer name: %s is unkown"%self._parameters["Minimizer"])
         #
         IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
         MinJ     = self.StoredVariables["CostFunctionJ"][IndexMin]
         Minimum  = self.StoredVariables["CurrentState"][IndexMin]
         #
         # Obtention de l'analyse
         # ----------------------
-        Xa = numpy.ravel( Minimum )
+        Xa = Minimum
         #
         self.StoredVariables["Analysis"].store( Xa )
         #
         # Calculs et/ou stockages supplémentaires
         # ---------------------------------------
         if self._toStore("OMA") or \
             self._toStore("SimulatedObservationAtOptimum"):
             if self._toStore("SimulatedObservationAtCurrentState"):
                 HXa = self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin]
             elif self._toStore("SimulatedObservationAtCurrentOptimum"):
                 HXa = self.StoredVariables["SimulatedObservationAtCurrentOptimum"][-1]
             else:
                 HXa = Hm(Xa)
+            HXa = HXa.reshape((-1,1))
         if self._toStore("Innovation") or \
             self._toStore("OMB") or \
             self._toStore("SimulatedObservationAtBackground"):
-            HXb = Hm(Xb)
-            Innovation  = Y - HXb
+            HXb = Hm(Xb).reshape((-1,1))
+            Innovation = Y - HXb
         if self._toStore("Innovation"):
             self.StoredVariables["Innovation"].store( Innovation )
         if self._toStore("OMB"):
             self.StoredVariables["OMB"].store( Innovation )
         if self._toStore("BMA"):
             self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
         if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( numpy.ravel(Y) - numpy.ravel(HXa) )
+            self.StoredVariables["OMA"].store( Y - HXa )
         if self._toStore("SimulatedObservationAtBackground"):
             self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
         if self._toStore("SimulatedObservationAtOptimum"):
             self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
         #
-        self._post_run()
+        self._post_run(HO)
         return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/DifferentialEvolution.py` & `adao-9.9.0.1/adao/daAlgorithms/Atoms/ecwnlls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,281 +16,245 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects
-import numpy, scipy.optimize
+__doc__ = """
+    Non Linear Least Squares
+"""
+__author__ = "Jean-Philippe ARGAUD"
 
-# ==============================================================================
-class ElementaryAlgorithm(BasicObjects.Algorithm):
-    def __init__(self):
-        BasicObjects.Algorithm.__init__(self, "DIFFERENTIALEVOLUTION")
-        self.defineRequiredParameter(
-            name     = "Minimizer",
-            default  = "BEST1BIN",
-            typecast = str,
-            message  = "Stratégie de minimisation utilisée",
-            listval  = [
-                "BEST1BIN",
-                "BEST1EXP",
-                "BEST2BIN",
-                "BEST2EXP",
-                "RAND1BIN",
-                "RAND1EXP",
-                "RAND2BIN",
-                "RAND2EXP",
-                "RANDTOBEST1BIN",
-                "RANDTOBEST1EXP",
-                ],
-            listadv  = [
-                "CURRENTTOBEST1EXP",
-                "CURRENTTOBEST1BIN",
-                ],
-            )
-        self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
-            default  = 15000,
-            typecast = int,
-            message  = "Nombre maximal de générations",
-            minval   = 0,
-            )
-        self.defineRequiredParameter(
-            name     = "MaximumNumberOfFunctionEvaluations",
-            default  = 15000,
-            typecast = int,
-            message  = "Nombre maximal d'évaluations de la fonction",
-            minval   = -1,
-            )
-        self.defineRequiredParameter(
-            name     = "PopulationSize",
-            default  = 100,
-            typecast = int,
-            message  = "Taille approximative de la population à chaque génération",
-            minval   = 1,
-            )
-        self.defineRequiredParameter(
-            name     = "MutationDifferentialWeight_F",
-            default  = (0.5, 1),
-            typecast = tuple,
-            message  = "Poids différentiel de mutation, constant ou aléatoire dans l'intervalle, noté F",
-            minval   = 0.,
-            maxval   = 2.,
-            )
-        self.defineRequiredParameter(
-            name     = "CrossOverProbability_CR",
-            default  = 0.7,
-            typecast = float,
-            message  = "Probabilité de recombinaison ou de croisement, notée CR",
-            minval   = 0.,
-            maxval   = 1.,
-            )
-        self.defineRequiredParameter(
-            name     = "QualityCriterion",
-            default  = "AugmentedWeightedLeastSquares",
-            typecast = str,
-            message  = "Critère de qualité utilisé",
-            listval  = [
-                "AugmentedWeightedLeastSquares","AWLS","DA",
-                "WeightedLeastSquares","WLS",
-                "LeastSquares","LS","L2",
-                "AbsoluteValue","L1",
-                "MaximumError","ME",
-                ],
-            )
-        self.defineRequiredParameter(
-            name     = "StoreInternalVariables",
-            default  = False,
-            typecast = bool,
-            message  = "Stockage des variables internes ou intermédiaires du calcul",
-            )
-        self.defineRequiredParameter(
-            name     = "StoreSupplementaryCalculations",
-            default  = [],
-            typecast = tuple,
-            message  = "Liste de calculs supplémentaires à stocker et/ou effectuer",
-            listval  = [
-                "Analysis",
-                "BMA",
-                "CostFunctionJ",
-                "CostFunctionJb",
-                "CostFunctionJo",
-                "CostFunctionJAtCurrentOptimum",
-                "CostFunctionJbAtCurrentOptimum",
-                "CostFunctionJoAtCurrentOptimum",
-                "CurrentIterationNumber",
-                "CurrentOptimum",
-                "CurrentState",
-                "IndexOfOptimum",
-                "Innovation",
-                "InnovationAtCurrentState",
-                "OMA",
-                "OMB",
-                "SimulatedObservationAtBackground",
-                "SimulatedObservationAtCurrentOptimum",
-                "SimulatedObservationAtCurrentState",
-                "SimulatedObservationAtOptimum",
-                ]
-            )
-        self.defineRequiredParameter(
-            name     = "SetSeed",
-            typecast = numpy.random.seed,
-            message  = "Graine fixée pour le générateur aléatoire",
-            )
-        self.defineRequiredParameter( # Pas de type
-            name     = "Bounds",
-            message  = "Liste des valeurs de bornes",
-            )
-        self.requireInputArguments(
-            mandatory= ("Xb", "Y", "HO", "R", "B" ),
-            )
-        self.setAttributes(tags=(
-            "Optimization",
-            "NonLinear",
-            "MetaHeuristic",
-            "Population",
-            ))
+import numpy, scipy, scipy.optimize, scipy.version
 
-    def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
-        self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
-        #
-        len_X = numpy.asarray(Xb).size
-        popsize = round(self._parameters["PopulationSize"]/len_X)
-        maxiter = min(self._parameters["MaximumNumberOfSteps"],round(self._parameters["MaximumNumberOfFunctionEvaluations"]/(popsize*len_X) - 1))
-        logging.debug("%s Nombre maximal de générations = %i, taille de la population à chaque génération = %i"%(self._name, maxiter, popsize*len_X))
-        #
-        # Opérateurs
-        # ----------
-        Hm = HO["Direct"].appliedTo
-        #
-        # Précalcul des inversions de B et R
-        # ----------------------------------
-        BI = B.getI()
-        RI = R.getI()
-        #
-        # Définition de la fonction-coût
-        # ------------------------------
-        def CostFunction(x, QualityMeasure="AugmentedWeightedLeastSquares"):
-            _X  = numpy.asmatrix(numpy.ravel( x )).T
-            self.StoredVariables["CurrentState"].store( _X )
-            _HX = Hm( _X )
-            _HX = numpy.asmatrix(numpy.ravel( _HX )).T
-            _Innovation = Y - _HX
-            if self._toStore("SimulatedObservationAtCurrentState") or \
-                self._toStore("SimulatedObservationAtCurrentOptimum"):
-                self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
-            if self._toStore("InnovationAtCurrentState"):
-                self.StoredVariables["InnovationAtCurrentState"].store( _Innovation )
-            #
-            if QualityMeasure in ["AugmentedWeightedLeastSquares","AWLS","DA"]:
-                if BI is None or RI is None:
-                    raise ValueError("Background and Observation error covariance matrix has to be properly defined!")
-                Jb  = 0.5 * (_X - Xb).T * (BI * (_X - Xb))
-                Jo  = 0.5 * _Innovation.T * (RI * _Innovation)
-            elif QualityMeasure in ["WeightedLeastSquares","WLS"]:
-                if RI is None:
-                    raise ValueError("Observation error covariance matrix has to be properly defined!")
-                Jb  = 0.
-                Jo  = 0.5 * (_Innovation).T * RI * (_Innovation)
-            elif QualityMeasure in ["LeastSquares","LS","L2"]:
-                Jb  = 0.
-                Jo  = 0.5 * (_Innovation).T * (_Innovation)
-            elif QualityMeasure in ["AbsoluteValue","L1"]:
-                Jb  = 0.
-                Jo  = numpy.sum( numpy.abs(_Innovation) )
-            elif QualityMeasure in ["MaximumError","ME"]:
-                Jb  = 0.
-                Jo  = numpy.max( numpy.abs(_Innovation) )
-            #
-            J   = float( Jb ) + float( Jo )
-            #
-            self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
-            self.StoredVariables["CostFunctionJb"].store( Jb )
-            self.StoredVariables["CostFunctionJo"].store( Jo )
-            self.StoredVariables["CostFunctionJ" ].store( J )
-            if self._toStore("IndexOfOptimum") or \
-                self._toStore("CurrentOptimum") or \
-                self._toStore("CostFunctionJAtCurrentOptimum") or \
-                self._toStore("CostFunctionJbAtCurrentOptimum") or \
-                self._toStore("CostFunctionJoAtCurrentOptimum") or \
-                self._toStore("SimulatedObservationAtCurrentOptimum"):
-                IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
-            if self._toStore("IndexOfOptimum"):
-                self.StoredVariables["IndexOfOptimum"].store( IndexMin )
-            if self._toStore("CurrentOptimum"):
-                self.StoredVariables["CurrentOptimum"].store( self.StoredVariables["CurrentState"][IndexMin] )
-            if self._toStore("SimulatedObservationAtCurrentOptimum"):
-                self.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin] )
-            if self._toStore("CostFunctionJAtCurrentOptimum"):
-                self.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( self.StoredVariables["CostFunctionJ" ][IndexMin] )
-            if self._toStore("CostFunctionJbAtCurrentOptimum"):
-                self.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJb"][IndexMin] )
-            if self._toStore("CostFunctionJoAtCurrentOptimum"):
-                self.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJo"][IndexMin] )
-            return J
-        #
-        # Point de démarrage de l'optimisation : Xini = Xb
-        # ------------------------------------
-        Xini = numpy.ravel(Xb)
-        #
-        # Minimisation de la fonctionnelle
-        # --------------------------------
-        nbPreviousSteps = self.StoredVariables["CostFunctionJ"].stepnumber()
-        #
-        optResults = scipy.optimize.differential_evolution(
-            CostFunction,
-            self._parameters["Bounds"],
-            strategy      = str(self._parameters["Minimizer"]).lower(),
-            maxiter       = maxiter,
-            popsize       = popsize,
-            mutation      = self._parameters["MutationDifferentialWeight_F"],
-            recombination = self._parameters["CrossOverProbability_CR"],
-            disp          = self._parameters["optdisp"],
-            )
-        #
-        IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
-        MinJ     = self.StoredVariables["CostFunctionJ"][IndexMin]
-        Minimum  = self.StoredVariables["CurrentState"][IndexMin]
-        #
-        # Obtention de l'analyse
-        # ----------------------
-        Xa = numpy.ravel( Minimum )
-        #
-        self.StoredVariables["Analysis"].store( Xa )
-        #
-        # Calculs et/ou stockages supplémentaires
-        # ---------------------------------------
-        if self._toStore("OMA") or \
-            self._toStore("SimulatedObservationAtOptimum"):
-            if self._toStore("SimulatedObservationAtCurrentState"):
-                HXa = self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin]
-            elif self._toStore("SimulatedObservationAtCurrentOptimum"):
-                HXa = self.StoredVariables["SimulatedObservationAtCurrentOptimum"][-1]
-            else:
-                HXa = Hm(Xa)
-        if self._toStore("Innovation") or \
-            self._toStore("OMB") or \
-            self._toStore("SimulatedObservationAtBackground"):
-            HXb = Hm(Xb)
-            Innovation  = Y - HXb
-        if self._toStore("Innovation"):
-            self.StoredVariables["Innovation"].store( Innovation )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( Innovation )
-        if self._toStore("BMA"):
-            self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
-        if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( numpy.ravel(Y) - numpy.ravel(HXa) )
-        if self._toStore("SimulatedObservationAtBackground"):
-            self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
-        if self._toStore("SimulatedObservationAtOptimum"):
-            self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
-        #
-        self._post_run()
-        return 0
+# ==============================================================================
+def ecwnlls(selfA, Xb, Y, U, HO, CM, R, B, __storeState = False):
+    """
+    Correction
+    """
+    #
+    # Initialisations
+    # ---------------
+    Hm = HO["Direct"].appliedTo
+    Ha = HO["Adjoint"].appliedInXTo
+    #
+    if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
+        HXb = numpy.asarray(Hm( Xb, HO["AppliedInX"]["HXb"] ))
+    else:
+        HXb = numpy.asarray(Hm( Xb ))
+    HXb = HXb.reshape((-1,1))
+    if Y.size != HXb.size:
+        raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
+    if max(Y.shape) != max(HXb.shape):
+        raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
+    #
+    RI = R.getI()
+    if selfA._parameters["Minimizer"] == "LM":
+        RdemiI = R.choleskyI()
+    #
+    Xini = selfA._parameters["InitializationPoint"]
+    #
+    # Définition de la fonction-coût
+    # ------------------------------
+    def CostFunction(x):
+        _X  = numpy.asarray(x).reshape((-1,1))
+        if selfA._parameters["StoreInternalVariables"] or \
+            selfA._toStore("CurrentState") or \
+            selfA._toStore("CurrentOptimum"):
+            selfA.StoredVariables["CurrentState"].store( _X )
+        _HX = numpy.asarray(Hm( _X )).reshape((-1,1))
+        _Innovation = Y - _HX
+        if selfA._toStore("SimulatedObservationAtCurrentState") or \
+            selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            selfA.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
+        if selfA._toStore("InnovationAtCurrentState"):
+            selfA.StoredVariables["InnovationAtCurrentState"].store( _Innovation )
+        #
+        Jb  = 0.
+        Jo  = float( 0.5 * _Innovation.T * (RI * _Innovation) )
+        J   = Jb + Jo
+        #
+        selfA.StoredVariables["CurrentIterationNumber"].store( len(selfA.StoredVariables["CostFunctionJ"]) )
+        selfA.StoredVariables["CostFunctionJb"].store( Jb )
+        selfA.StoredVariables["CostFunctionJo"].store( Jo )
+        selfA.StoredVariables["CostFunctionJ" ].store( J )
+        if selfA._toStore("IndexOfOptimum") or \
+            selfA._toStore("CurrentOptimum") or \
+            selfA._toStore("CostFunctionJAtCurrentOptimum") or \
+            selfA._toStore("CostFunctionJbAtCurrentOptimum") or \
+            selfA._toStore("CostFunctionJoAtCurrentOptimum") or \
+            selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            IndexMin = numpy.argmin( selfA.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+        if selfA._toStore("IndexOfOptimum"):
+            selfA.StoredVariables["IndexOfOptimum"].store( IndexMin )
+        if selfA._toStore("CurrentOptimum"):
+            selfA.StoredVariables["CurrentOptimum"].store( selfA.StoredVariables["CurrentState"][IndexMin] )
+        if selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            selfA.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( selfA.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin] )
+        if selfA._toStore("CostFunctionJbAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( selfA.StoredVariables["CostFunctionJb"][IndexMin] )
+        if selfA._toStore("CostFunctionJoAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( selfA.StoredVariables["CostFunctionJo"][IndexMin] )
+        if selfA._toStore("CostFunctionJAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( selfA.StoredVariables["CostFunctionJ" ][IndexMin] )
+        return J
+    #
+    def GradientOfCostFunction(x):
+        _X      = numpy.asarray(x).reshape((-1,1))
+        _HX     = numpy.asarray(Hm( _X )).reshape((-1,1))
+        GradJb  = 0.
+        GradJo  = - Ha( (_X, RI * (Y - _HX)) )
+        GradJ   = numpy.ravel( GradJb ) + numpy.ravel( GradJo )
+        return GradJ
+    #
+    def CostFunctionLM(x):
+        _X  = numpy.ravel( x ).reshape((-1,1))
+        _HX = Hm( _X ).reshape((-1,1))
+        _Innovation = Y - _HX
+        Jb  = 0.
+        Jo  = float( 0.5 * _Innovation.T * (RI * _Innovation) )
+        J   = Jb + Jo
+        if selfA._parameters["StoreInternalVariables"] or \
+            selfA._toStore("CurrentState"):
+            selfA.StoredVariables["CurrentState"].store( _X )
+        selfA.StoredVariables["CostFunctionJb"].store( Jb )
+        selfA.StoredVariables["CostFunctionJo"].store( Jo )
+        selfA.StoredVariables["CostFunctionJ" ].store( J )
+        #
+        return numpy.ravel( RdemiI*_Innovation )
+    #
+    def GradientOfCostFunctionLM(x):
+        _X      = x.reshape((-1,1))
+        return - RdemiI*HO["Tangent"].asMatrix( _X )
+    #
+    # Minimisation de la fonctionnelle
+    # --------------------------------
+    nbPreviousSteps = selfA.StoredVariables["CostFunctionJ"].stepnumber()
+    #
+    if selfA._parameters["Minimizer"] == "LBFGSB":
+        if "0.19" <= scipy.version.version <= "1.4.1":
+            import daAlgorithms.Atoms.lbfgsbhlt as optimiseur
+        else:
+            import scipy.optimize as optimiseur
+        Minimum, J_optimal, Informations = optimiseur.fmin_l_bfgs_b(
+            func        = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            bounds      = selfA._parameters["Bounds"],
+            maxfun      = selfA._parameters["MaximumNumberOfIterations"]-1,
+            factr       = selfA._parameters["CostDecrementTolerance"]*1.e14,
+            pgtol       = selfA._parameters["ProjectedGradientTolerance"],
+            iprint      = selfA._parameters["optiprint"],
+            )
+        # nfeval = Informations['funcalls']
+        # rc     = Informations['warnflag']
+    elif selfA._parameters["Minimizer"] == "TNC":
+        Minimum, nfeval, rc = scipy.optimize.fmin_tnc(
+            func        = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            bounds      = selfA._parameters["Bounds"],
+            maxfun      = selfA._parameters["MaximumNumberOfIterations"],
+            pgtol       = selfA._parameters["ProjectedGradientTolerance"],
+            ftol        = selfA._parameters["CostDecrementTolerance"],
+            messages    = selfA._parameters["optmessages"],
+            )
+    elif selfA._parameters["Minimizer"] == "CG":
+        Minimum, fopt, nfeval, grad_calls, rc = scipy.optimize.fmin_cg(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
+            )
+    elif selfA._parameters["Minimizer"] == "NCG":
+        Minimum, fopt, nfeval, grad_calls, hcalls, rc = scipy.optimize.fmin_ncg(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            avextol     = selfA._parameters["CostDecrementTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
+            )
+    elif selfA._parameters["Minimizer"] == "BFGS":
+        Minimum, fopt, gopt, Hopt, nfeval, grad_calls, rc = scipy.optimize.fmin_bfgs(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
+            )
+    elif selfA._parameters["Minimizer"] == "LM":
+        Minimum, cov_x, infodict, mesg, rc = scipy.optimize.leastsq(
+            func        = CostFunctionLM,
+            x0          = Xini,
+            Dfun        = GradientOfCostFunctionLM,
+            args        = (),
+            ftol        = selfA._parameters["CostDecrementTolerance"],
+            maxfev      = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            full_output = True,
+            )
+        # nfeval = infodict['nfev']
+    else:
+        raise ValueError("Error in minimizer name: %s is unkown"%selfA._parameters["Minimizer"])
+    #
+    IndexMin = numpy.argmin( selfA.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+    #
+    # Correction pour pallier a un bug de TNC sur le retour du Minimum
+    # ----------------------------------------------------------------
+    if selfA._parameters["StoreInternalVariables"] or selfA._toStore("CurrentState"):
+        Minimum = selfA.StoredVariables["CurrentState"][IndexMin]
+    #
+    Xa = Minimum
+    if __storeState: selfA._setInternalState("Xn", Xa)
+    #--------------------------
+    #
+    selfA.StoredVariables["Analysis"].store( Xa )
+    #
+    if selfA._toStore("OMA") or \
+        selfA._toStore("InnovationAtCurrentAnalysis") or \
+        selfA._toStore("SimulatedObservationAtOptimum"):
+        if selfA._toStore("SimulatedObservationAtCurrentState"):
+            HXa = selfA.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin]
+        elif selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            HXa = selfA.StoredVariables["SimulatedObservationAtCurrentOptimum"][-1]
+        else:
+            HXa = Hm( Xa )
+        oma = Y - HXa.reshape((-1,1))
+    #
+    # Calculs et/ou stockages supplémentaires
+    # ---------------------------------------
+    if selfA._toStore("Innovation") or \
+        selfA._toStore("OMB"):
+        Innovation  = Y - HXb
+    if selfA._toStore("Innovation"):
+        selfA.StoredVariables["Innovation"].store( Innovation )
+    if selfA._toStore("BMA"):
+        selfA.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
+    if selfA._toStore("OMA"):
+        selfA.StoredVariables["OMA"].store( oma )
+    if selfA._toStore("InnovationAtCurrentAnalysis"):
+        selfA.StoredVariables["InnovationAtCurrentAnalysis"].store( oma )
+    if selfA._toStore("OMB"):
+        selfA.StoredVariables["OMB"].store( Innovation )
+    if selfA._toStore("SimulatedObservationAtBackground"):
+        selfA.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
+    if selfA._toStore("SimulatedObservationAtOptimum"):
+        selfA.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
+    #
+    return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/EnsembleBlue.py` & `adao-9.9.0.1/adao/daAlgorithms/EnsembleBlue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,16 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects
 import numpy
+from daCore import BasicObjects
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "ENSEMBLEBLUE")
         self.defineRequiredParameter(
             name     = "StoreInternalVariables",
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/EnsembleKalmanFilter.py` & `adao-9.9.0.1/adao/daAlgorithms/EnsembleKalmanFilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
 import numpy
+from daCore import BasicObjects
+from daAlgorithms.Atoms import enks, etkf, ienkf, mlef, senkf
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "ENSEMBLEKALMANFILTER")
         self.defineRequiredParameter(
             name     = "Variant",
@@ -108,19 +108,33 @@
             message  = "Nombre d'intervalles de temps de lissage dans le passé",
             minval   = 0,
             )
         self.defineRequiredParameter(
             name     = "HybridCovarianceEquilibrium",
             default  = 0.5,
             typecast = float,
-            message  = "Facteur d'équilibre entre la covariance statique et la covariance d'ensemble",
+            message  = "Facteur d'équilibre entre la covariance statique et la covariance d'ensemble en hybride variationnel",
             minval   = 0.,
             maxval   = 1.,
             )
         self.defineRequiredParameter(
+            name     = "HybridMaximumNumberOfIterations",
+            default  = 15000,
+            typecast = int,
+            message  = "Nombre maximal de pas d'optimisation en hybride variationnel",
+            minval   = -1,
+            )
+        self.defineRequiredParameter(
+            name     = "HybridCostDecrementTolerance",
+            default  = 1.e-7,
+            typecast = float,
+            message  = "Diminution relative minimale du coût lors de l'arrêt en hybride variationnel",
+            minval   = 0.,
+            )
+        self.defineRequiredParameter(
             name     = "SetSeed",
             typecast = numpy.random.seed,
             message  = "Graine fixée pour le générateur aléatoire",
             )
         self.defineRequiredParameter(
             name     = "StoreInternalVariables",
             default  = False,
@@ -175,69 +189,69 @@
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         # Default EnKF = EnKF-16 = StochasticEnKF
         if   self._parameters["Variant"] == "EnKF-05":
-            NumericObjects.senkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="KalmanFilterFormula05")
+            senkf.senkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="KalmanFilterFormula05")
         #
         elif self._parameters["Variant"] in ["EnKF-16", "StochasticEnKF", "EnKF"]:
-            NumericObjects.senkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="KalmanFilterFormula16")
+            senkf.senkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="KalmanFilterFormula16")
         #
         #--------------------------
         # Default ETKF = ETKF-KFF
         elif self._parameters["Variant"] in ["ETKF-KFF", "ETKF"]:
-            NumericObjects.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="KalmanFilterFormula")
+            etkf.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="KalmanFilterFormula")
         #
         elif self._parameters["Variant"] == "ETKF-VAR":
-            NumericObjects.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="Variational")
+            etkf.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="Variational")
         #
         #--------------------------
         # Default ETKF-N = ETKF-N-16
         elif self._parameters["Variant"] == "ETKF-N-11":
-            NumericObjects.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="FiniteSize11")
+            etkf.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="FiniteSize11")
         #
         elif self._parameters["Variant"] == "ETKF-N-15":
-            NumericObjects.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="FiniteSize15")
+            etkf.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="FiniteSize15")
         #
         elif self._parameters["Variant"] in ["ETKF-N-16", "ETKF-N"]:
-            NumericObjects.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="FiniteSize16")
+            etkf.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="FiniteSize16")
         #
         #--------------------------
         # Default MLEF = MLEF-T
         elif self._parameters["Variant"] in ["MLEF-T", "MLEF"]:
-            NumericObjects.mlef(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=False)
+            mlef.mlef(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=False)
         #
         elif self._parameters["Variant"] == "MLEF-B":
-            NumericObjects.mlef(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=True)
+            mlef.mlef(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=True)
         #
         #--------------------------
         # Default IEnKF = IEnKF-T
         elif self._parameters["Variant"] in ["IEnKF-T", "IEnKF"]:
-            NumericObjects.ienkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=False)
+            ienkf.ienkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=False)
         #
         elif self._parameters["Variant"] in ["IEnKF-B", "IEKF"]:
-            NumericObjects.ienkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=True)
+            ienkf.ienkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, BnotT=True)
         #
         #--------------------------
         # Default EnKS = EnKS-KFF
         elif self._parameters["Variant"] in ["EnKS-KFF", "EnKS"]:
-            NumericObjects.enks(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="EnKS16-KalmanFilterFormula")
+            enks.enks(self, Xb, Y, U, HO, EM, CM, R, B, Q, VariantM="EnKS16-KalmanFilterFormula")
         #
         #--------------------------
-        # Default E3DVAR = E3DVAR-EnKF
-        elif self._parameters["Variant"] in ["E3DVAR-EnKF", "E3DVAR"]:
-            NumericObjects.senkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, Hybrid="E3DVAR")
+        # Default E3DVAR = E3DVAR-ETKF
+        elif self._parameters["Variant"] == "E3DVAR-EnKF":
+            senkf.senkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, Hybrid="E3DVAR")
         #
-        elif self._parameters["Variant"] == "E3DVAR-ETKF":
-            NumericObjects.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, Hybrid="E3DVAR")
+        elif self._parameters["Variant"] in ["E3DVAR-ETKF", "E3DVAR"]:
+            etkf.etkf(self, Xb, Y, U, HO, EM, CM, R, B, Q, Hybrid="E3DVAR")
         #
         elif self._parameters["Variant"] == "E3DVAR-MLEF":
-            NumericObjects.mlef(self, Xb, Y, U, HO, EM, CM, R, B, Q, Hybrid="E3DVAR")
+            mlef.mlef(self, Xb, Y, U, HO, EM, CM, R, B, Q, Hybrid="E3DVAR")
         #
         #--------------------------
         else:
             raise ValueError("Error in Variant name: %s"%self._parameters["Variant"])
         #
         self._post_run(HO)
         return 0
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/ExtendedBlue.py` & `adao-9.9.0.1/adao/daAlgorithms/Atoms/std4dvar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,219 +16,253 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
-import numpy
+__doc__ = """
+    4DVAR
+"""
+__author__ = "Jean-Philippe ARGAUD"
+
+import numpy, scipy, scipy.optimize, scipy.version
+from daCore.NumericObjects import ForceNumericBounds, ApplyBounds
+from daCore.PlatformInfo import PlatformInfo
+mpr = PlatformInfo().MachinePrecision()
+mfp = PlatformInfo().MaximumPrecision()
 
 # ==============================================================================
-class ElementaryAlgorithm(BasicObjects.Algorithm):
-    def __init__(self):
-        BasicObjects.Algorithm.__init__(self, "EXTENDEDBLUE")
-        self.defineRequiredParameter(
-            name     = "StoreInternalVariables",
-            default  = False,
-            typecast = bool,
-            message  = "Stockage des variables internes ou intermédiaires du calcul",
-            )
-        self.defineRequiredParameter(
-            name     = "StoreSupplementaryCalculations",
-            default  = [],
-            typecast = tuple,
-            message  = "Liste de calculs supplémentaires à stocker et/ou effectuer",
-            listval  = [
-                "Analysis",
-                "APosterioriCorrelations",
-                "APosterioriCovariance",
-                "APosterioriStandardDeviations",
-                "APosterioriVariances",
-                "BMA",
-                "CostFunctionJ",
-                "CostFunctionJAtCurrentOptimum",
-                "CostFunctionJb",
-                "CostFunctionJbAtCurrentOptimum",
-                "CostFunctionJo",
-                "CostFunctionJoAtCurrentOptimum",
-                "CurrentOptimum",
-                "CurrentState",
-                "Innovation",
-                "MahalanobisConsistency",
-                "OMA",
-                "OMB",
-                "SampledStateForQuantiles",
-                "SigmaBck2",
-                "SigmaObs2",
-                "SimulatedObservationAtBackground",
-                "SimulatedObservationAtCurrentOptimum",
-                "SimulatedObservationAtCurrentState",
-                "SimulatedObservationAtOptimum",
-                "SimulationQuantiles",
-                ]
-            )
-        self.defineRequiredParameter(
-            name     = "Quantiles",
-            default  = [],
-            typecast = tuple,
-            message  = "Liste des valeurs de quantiles",
-            minval   = 0.,
-            maxval   = 1.,
-            )
-        self.defineRequiredParameter(
-            name     = "SetSeed",
-            typecast = numpy.random.seed,
-            message  = "Graine fixée pour le générateur aléatoire",
+def std4dvar(selfA, Xb, Y, U, HO, EM, CM, R, B, Q):
+    """
+    Correction
+    """
+    #
+    # Initialisations
+    # ---------------
+    #
+    # Opérateurs
+    Hm = HO["Direct"].appliedControledFormTo
+    Mm = EM["Direct"].appliedControledFormTo
+    #
+    if CM is not None and "Tangent" in CM and U is not None:
+        Cm = CM["Tangent"].asMatrix(Xb)
+    else:
+        Cm = None
+    #
+    def Un(_step):
+        if U is not None:
+            if hasattr(U,"store") and 1<=_step<len(U) :
+                _Un = numpy.ravel( U[_step] ).reshape((-1,1))
+            elif hasattr(U,"store") and len(U)==1:
+                _Un = numpy.ravel( U[0] ).reshape((-1,1))
+            else:
+                _Un = numpy.ravel( U ).reshape((-1,1))
+        else:
+            _Un = None
+        return _Un
+    def CmUn(_xn,_un):
+        if Cm is not None and _un is not None: # Attention : si Cm est aussi dans M, doublon !
+            _Cm   = Cm.reshape(_xn.size,_un.size) # ADAO & check shape
+            _CmUn = (_Cm @ _un).reshape((-1,1))
+        else:
+            _CmUn = 0.
+        return _CmUn
+    #
+    # Remarque : les observations sont exploitées à partir du pas de temps
+    # numéro 1, et sont utilisées dans Yo comme rangées selon ces indices.
+    # Donc le pas 0 n'est pas utilisé puisque la première étape commence
+    # avec l'observation du pas 1.
+    #
+    # Nombre de pas identique au nombre de pas d'observations
+    if hasattr(Y,"stepnumber"):
+        duration = Y.stepnumber()
+    else:
+        duration = 2
+    #
+    # Précalcul des inversions de B et R
+    BI = B.getI()
+    RI = R.getI()
+    #
+    # Point de démarrage de l'optimisation
+    Xini = selfA._parameters["InitializationPoint"]
+    #
+    # Définition de la fonction-coût
+    # ------------------------------
+    selfA.DirectCalculation = [None,] # Le pas 0 n'est pas observé
+    selfA.DirectInnovation  = [None,] # Le pas 0 n'est pas observé
+    def CostFunction(x):
+        _X  = numpy.asarray(x).reshape((-1,1))
+        if selfA._parameters["StoreInternalVariables"] or \
+            selfA._toStore("CurrentState") or \
+            selfA._toStore("CurrentOptimum"):
+            selfA.StoredVariables["CurrentState"].store( _X )
+        Jb  = float( 0.5 * (_X - Xb).T * (BI * (_X - Xb)) )
+        selfA.DirectCalculation = [None,]
+        selfA.DirectInnovation  = [None,]
+        Jo  = 0.
+        _Xn = _X
+        for step in range(0,duration-1):
+            if hasattr(Y,"store"):
+                _Ynpu = numpy.ravel( Y[step+1] ).reshape((-1,1))
+            else:
+                _Ynpu = numpy.ravel( Y ).reshape((-1,1))
+            _Un = Un(step)
+            #
+            # Etape d'évolution
+            if selfA._parameters["EstimationOf"] == "State":
+                _Xn = Mm( (_Xn, _Un) ).reshape((-1,1)) + CmUn(_Xn, _Un)
+            elif selfA._parameters["EstimationOf"] == "Parameters":
+                pass
+            #
+            if selfA._parameters["Bounds"] is not None and selfA._parameters["ConstrainedBy"] == "EstimateProjection":
+                _Xn = ApplyBounds( _Xn, ForceNumericBounds(selfA._parameters["Bounds"]) )
+            #
+            # Etape de différence aux observations
+            if selfA._parameters["EstimationOf"] == "State":
+                _YmHMX = _Ynpu - numpy.ravel( Hm( (_Xn, None) ) ).reshape((-1,1))
+            elif selfA._parameters["EstimationOf"] == "Parameters":
+                _YmHMX = _Ynpu - numpy.ravel( Hm( (_Xn, _Un) ) ).reshape((-1,1)) - CmUn(_Xn, _Un)
+            #
+            # Stockage de l'état
+            selfA.DirectCalculation.append( _Xn )
+            selfA.DirectInnovation.append( _YmHMX )
+            #
+            # Ajout dans la fonctionnelle d'observation
+            Jo = Jo + 0.5 * float( _YmHMX.T * (RI * _YmHMX) )
+        J = Jb + Jo
+        #
+        selfA.StoredVariables["CurrentIterationNumber"].store( len(selfA.StoredVariables["CostFunctionJ"]) )
+        selfA.StoredVariables["CostFunctionJb"].store( Jb )
+        selfA.StoredVariables["CostFunctionJo"].store( Jo )
+        selfA.StoredVariables["CostFunctionJ" ].store( J )
+        if selfA._toStore("IndexOfOptimum") or \
+            selfA._toStore("CurrentOptimum") or \
+            selfA._toStore("CostFunctionJAtCurrentOptimum") or \
+            selfA._toStore("CostFunctionJbAtCurrentOptimum") or \
+            selfA._toStore("CostFunctionJoAtCurrentOptimum"):
+            IndexMin = numpy.argmin( selfA.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+        if selfA._toStore("IndexOfOptimum"):
+            selfA.StoredVariables["IndexOfOptimum"].store( IndexMin )
+        if selfA._toStore("CurrentOptimum"):
+            selfA.StoredVariables["CurrentOptimum"].store( selfA.StoredVariables["CurrentState"][IndexMin] )
+        if selfA._toStore("CostFunctionJAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( selfA.StoredVariables["CostFunctionJ" ][IndexMin] )
+        if selfA._toStore("CostFunctionJbAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( selfA.StoredVariables["CostFunctionJb"][IndexMin] )
+        if selfA._toStore("CostFunctionJoAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( selfA.StoredVariables["CostFunctionJo"][IndexMin] )
+        return J
+    #
+    def GradientOfCostFunction(x):
+        _X      = numpy.asarray(x).reshape((-1,1))
+        GradJb  = BI * (_X - Xb)
+        GradJo  = 0.
+        for step in range(duration-1,0,-1):
+            # Étape de récupération du dernier stockage de l'évolution
+            _Xn = selfA.DirectCalculation.pop()
+            # Étape de récupération du dernier stockage de l'innovation
+            _YmHMX = selfA.DirectInnovation.pop()
+            # Calcul des adjoints
+            Ha = HO["Adjoint"].asMatrix(ValueForMethodForm = _Xn)
+            Ha = Ha.reshape(_Xn.size,_YmHMX.size) # ADAO & check shape
+            Ma = EM["Adjoint"].asMatrix(ValueForMethodForm = _Xn)
+            Ma = Ma.reshape(_Xn.size,_Xn.size) # ADAO & check shape
+            # Calcul du gradient par état adjoint
+            GradJo = GradJo + Ha * (RI * _YmHMX) # Équivaut pour Ha linéaire à : Ha( (_Xn, RI * _YmHMX) )
+            GradJo = Ma * GradJo                 # Équivaut pour Ma linéaire à : Ma( (_Xn, GradJo) )
+        GradJ = numpy.ravel( GradJb ) - numpy.ravel( GradJo )
+        return GradJ
+    #
+    # Minimisation de la fonctionnelle
+    # --------------------------------
+    nbPreviousSteps = selfA.StoredVariables["CostFunctionJ"].stepnumber()
+    #
+    if selfA._parameters["Minimizer"] == "LBFGSB":
+        if "0.19" <= scipy.version.version <= "1.4.1":
+            import daAlgorithms.Atoms.lbfgsbhlt as optimiseur
+        else:
+            import scipy.optimize as optimiseur
+        Minimum, J_optimal, Informations = optimiseur.fmin_l_bfgs_b(
+            func        = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            bounds      = selfA._parameters["Bounds"],
+            maxfun      = selfA._parameters["MaximumNumberOfIterations"]-1,
+            factr       = selfA._parameters["CostDecrementTolerance"]*1.e14,
+            pgtol       = selfA._parameters["ProjectedGradientTolerance"],
+            iprint      = selfA._parameters["optiprint"],
             )
-        self.defineRequiredParameter(
-            name     = "NumberOfSamplesForQuantiles",
-            default  = 100,
-            typecast = int,
-            message  = "Nombre d'échantillons simulés pour le calcul des quantiles",
-            minval   = 1,
+        # nfeval = Informations['funcalls']
+        # rc     = Informations['warnflag']
+    elif selfA._parameters["Minimizer"] == "TNC":
+        Minimum, nfeval, rc = scipy.optimize.fmin_tnc(
+            func        = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            bounds      = selfA._parameters["Bounds"],
+            maxfun      = selfA._parameters["MaximumNumberOfIterations"],
+            pgtol       = selfA._parameters["ProjectedGradientTolerance"],
+            ftol        = selfA._parameters["CostDecrementTolerance"],
+            messages    = selfA._parameters["optmessages"],
             )
-        self.defineRequiredParameter(
-            name     = "SimulationForQuantiles",
-            default  = "Linear",
-            typecast = str,
-            message  = "Type de simulation en estimation des quantiles",
-            listval  = ["Linear", "NonLinear"]
+    elif selfA._parameters["Minimizer"] == "CG":
+        Minimum, fopt, nfeval, grad_calls, rc = scipy.optimize.fmin_cg(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
             )
-        self.defineRequiredParameter( # Pas de type
-            name     = "StateBoundsForQuantiles",
-            message  = "Liste des paires de bornes pour les états utilisés en estimation des quantiles",
+    elif selfA._parameters["Minimizer"] == "NCG":
+        Minimum, fopt, nfeval, grad_calls, hcalls, rc = scipy.optimize.fmin_ncg(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            avextol     = selfA._parameters["CostDecrementTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
             )
-        self.requireInputArguments(
-            mandatory= ("Xb", "Y", "HO", "R", "B"),
+    elif selfA._parameters["Minimizer"] == "BFGS":
+        Minimum, fopt, gopt, Hopt, nfeval, grad_calls, rc = scipy.optimize.fmin_bfgs(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
             )
-        self.setAttributes(tags=(
-            "DataAssimilation",
-            "NonLinear",
-            "Filter",
-            ))
-
-    def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
-        self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
-        #
-        Hm = HO["Tangent"].asMatrix(Xb)
-        Hm = Hm.reshape(Y.size,Xb.size) # ADAO & check shape
-        Ha = HO["Adjoint"].asMatrix(Xb)
-        Ha = Ha.reshape(Xb.size,Y.size) # ADAO & check shape
-        H  = HO["Direct"].appliedTo
-        #
-        if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
-            HXb = H( Xb, HO["AppliedInX"]["HXb"])
-        else:
-            HXb = H( Xb )
-        HXb = HXb.reshape((-1,1))
-        if Y.size != HXb.size:
-            raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
-        if max(Y.shape) != max(HXb.shape):
-            raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
-        #
-        BI = B.getI()
-        RI = R.getI()
-        #
-        Innovation  = Y - HXb
-        #
-        # Calcul de la matrice de gain et de l'analyse
-        # --------------------------------------------
-        if Y.size <= Xb.size:
-            _A = R + numpy.dot(Hm, B * Ha)
-            _u = numpy.linalg.solve( _A , Innovation )
-            Xa = Xb + B * Ha * _u
-        else:
-            _A = BI + numpy.dot(Ha, RI * Hm)
-            _u = numpy.linalg.solve( _A , numpy.dot(Ha, RI * Innovation) )
-            Xa = Xb + _u
-        self.StoredVariables["Analysis"].store( Xa )
-        #
-        # Calcul de la fonction coût
-        # --------------------------
-        if self._parameters["StoreInternalVariables"] or \
-            self._toStore("CostFunctionJ")  or self._toStore("CostFunctionJAtCurrentOptimum") or \
-            self._toStore("CostFunctionJb") or self._toStore("CostFunctionJbAtCurrentOptimum") or \
-            self._toStore("CostFunctionJo") or self._toStore("CostFunctionJoAtCurrentOptimum") or \
-            self._toStore("OMA") or \
-            self._toStore("SigmaObs2") or \
-            self._toStore("MahalanobisConsistency") or \
-            self._toStore("SimulatedObservationAtCurrentOptimum") or \
-            self._toStore("SimulatedObservationAtCurrentState") or \
-            self._toStore("SimulatedObservationAtOptimum") or \
-            self._toStore("SimulationQuantiles"):
-            HXa  = H( Xa ).reshape((-1,1))
-            oma = Y - HXa
-        if self._parameters["StoreInternalVariables"] or \
-            self._toStore("CostFunctionJ")  or self._toStore("CostFunctionJAtCurrentOptimum") or \
-            self._toStore("CostFunctionJb") or self._toStore("CostFunctionJbAtCurrentOptimum") or \
-            self._toStore("CostFunctionJo") or self._toStore("CostFunctionJoAtCurrentOptimum") or \
-            self._toStore("MahalanobisConsistency"):
-            Jb  = float( 0.5 * (Xa - Xb).T * (BI * (Xa - Xb)) )
-            Jo  = float( 0.5 * oma.T * (RI * oma) )
-            J   = Jb + Jo
-            self.StoredVariables["CostFunctionJb"].store( Jb )
-            self.StoredVariables["CostFunctionJo"].store( Jo )
-            self.StoredVariables["CostFunctionJ" ].store( J )
-            self.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( Jb )
-            self.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( Jo )
-            self.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( J )
-        #
-        # Calcul de la covariance d'analyse
-        # ---------------------------------
-        if self._toStore("APosterioriCovariance") or \
-            self._toStore("SimulationQuantiles"):
-            if   (Y.size <= Xb.size): K  = B * Ha * (R + numpy.dot(Hm, B * Ha)).I
-            elif (Y.size >  Xb.size): K = (BI + numpy.dot(Ha, RI * Hm)).I * Ha * RI
-            A = B - K * Hm * B
-            if min(A.shape) != max(A.shape):
-                raise ValueError("The %s a posteriori covariance matrix A is of shape %s, despites it has to be a squared matrix. There is an error in the observation operator, please check it."%(self._name,str(A.shape)))
-            if (numpy.diag(A) < 0).any():
-                raise ValueError("The %s a posteriori covariance matrix A has at least one negative value on its diagonal. There is an error in the observation operator, please check it."%(self._name,))
-            if logging.getLogger().level < logging.WARNING: # La verification n'a lieu qu'en debug
-                try:
-                    L = numpy.linalg.cholesky( A )
-                except:
-                    raise ValueError("The %s a posteriori covariance matrix A is not symmetric positive-definite. Please check your a priori covariances and your observation operator."%(self._name,))
-            self.StoredVariables["APosterioriCovariance"].store( A )
-        #
-        # Calculs et/ou stockages supplémentaires
-        # ---------------------------------------
-        if self._parameters["StoreInternalVariables"] or self._toStore("CurrentState"):
-            self.StoredVariables["CurrentState"].store( Xa )
-        if self._toStore("CurrentOptimum"):
-            self.StoredVariables["CurrentOptimum"].store( Xa )
-        if self._toStore("Innovation"):
-            self.StoredVariables["Innovation"].store( Innovation )
-        if self._toStore("BMA"):
-            self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
-        if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( oma )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( Innovation )
-        if self._toStore("SigmaObs2"):
-            TraceR = R.trace(Y.size)
-            self.StoredVariables["SigmaObs2"].store( float( Innovation.T @ oma ) / TraceR )
-        if self._toStore("SigmaBck2"):
-            self.StoredVariables["SigmaBck2"].store( float( (Innovation.T @ (Hm @ (Xa - Xb)))/(Hm * (B * Hm.T)).trace() ) )
-        if self._toStore("MahalanobisConsistency"):
-            self.StoredVariables["MahalanobisConsistency"].store( float( 2.*J/Innovation.size ) )
-        if self._toStore("SimulationQuantiles"):
-            HtM  = HO["Tangent"].asMatrix(ValueForMethodForm = Xa)
-            HtM  = HtM.reshape(Y.size,Xa.size) # ADAO & check shape
-            NumericObjects.QuantilesEstimations(self, A, Xa, HXa, H, HtM)
-        if self._toStore("SimulatedObservationAtBackground"):
-            self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
-        if self._toStore("SimulatedObservationAtCurrentState"):
-            self.StoredVariables["SimulatedObservationAtCurrentState"].store( HXa )
-        if self._toStore("SimulatedObservationAtCurrentOptimum"):
-            self.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( HXa )
-        if self._toStore("SimulatedObservationAtOptimum"):
-            self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
-        #
-        self._post_run(HO)
-        return 0
+    else:
+        raise ValueError("Error in minimizer name: %s is unkown"%selfA._parameters["Minimizer"])
+    #
+    IndexMin = numpy.argmin( selfA.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+    #
+    # Correction pour pallier a un bug de TNC sur le retour du Minimum
+    # ----------------------------------------------------------------
+    if selfA._parameters["StoreInternalVariables"] or selfA._toStore("CurrentState"):
+        Minimum = selfA.StoredVariables["CurrentState"][IndexMin]
+    #
+    # Obtention de l'analyse
+    # ----------------------
+    Xa = Minimum
+    #
+    selfA.StoredVariables["Analysis"].store( Xa )
+    #
+    # Calculs et/ou stockages supplémentaires
+    # ---------------------------------------
+    if selfA._toStore("BMA"):
+        selfA.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
+    #
+    return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/ExtendedKalmanFilter.py` & `adao-9.9.0.1/adao/daAlgorithms/ExtendedKalmanFilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,16 +16,16 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
+from daCore import BasicObjects
+from daAlgorithms.Atoms import cekf, exkf
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "EXTENDEDKALMANFILTER")
         self.defineRequiredParameter(
             name     = "Variant",
@@ -106,20 +106,20 @@
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         # Default EKF
         #--------------------------
         if   self._parameters["Variant"] == "EKF":
-            NumericObjects.exkf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+            exkf.exkf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         # Default CEKF
         elif self._parameters["Variant"] == "CEKF":
-            NumericObjects.cekf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+            cekf.cekf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         else:
             raise ValueError("Error in Variant name: %s"%self._parameters["Variant"])
         #
         self._post_run(HO)
         return 0
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/FunctionTest.py` & `adao-9.9.0.1/adao/daAlgorithms/FunctionTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,21 +16,19 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
+import logging
 from daCore import BasicObjects, PlatformInfo
 import numpy, copy
 mpr = PlatformInfo.PlatformInfo().MachinePrecision()
 mfp = PlatformInfo.PlatformInfo().MaximumPrecision()
-if sys.version_info.major > 2:
-    unicode = str
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "FUNCTIONTEST")
         self.defineRequiredParameter(
             name     = "NumberOfPrintedDigits",
@@ -82,15 +80,15 @@
         #
         Xn = copy.copy( Xb )
         #
         # ----------
         __marge =  5*u" "
         _p = self._parameters["NumberOfPrintedDigits"]
         if len(self._parameters["ResultTitle"]) > 0:
-            __rt = unicode(self._parameters["ResultTitle"])
+            __rt = str(self._parameters["ResultTitle"])
             msgs  = u"\n"
             msgs +=  __marge + "====" + "="*len(__rt) + "====\n"
             msgs +=  __marge + "    " + __rt + "\n"
             msgs +=  __marge + "====" + "="*len(__rt) + "====\n"
             print("%s"%msgs)
         #
         msgs  = ("===> Information before launching:\n")
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/GradientTest.py` & `adao-9.9.0.1/adao/daAlgorithms/GradientTest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,20 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
-from daCore import BasicObjects, PlatformInfo
-import numpy, math
+import math, numpy
+from daCore import BasicObjects, NumericObjects, PlatformInfo
 mpr = PlatformInfo.PlatformInfo().MachinePrecision()
-if sys.version_info.major > 2:
-    unicode = str
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "GRADIENTTEST")
         self.defineRequiredParameter(
             name     = "ResiduFormula",
@@ -120,39 +117,34 @@
         if self._parameters["ResiduFormula"] in ["Taylor", "TaylorOnNorm"]:
             Ht = HO["Tangent"].appliedInXTo
         #
         # ----------
         Perturbations = [ 10**i for i in range(self._parameters["EpsilonMinimumExponent"],1) ]
         Perturbations.reverse()
         #
-        X       = numpy.asmatrix(numpy.ravel(    Xb   )).T
-        FX      = numpy.asmatrix(numpy.ravel( Hm( X ) )).T
+        X       = numpy.ravel(    Xb   ).reshape((-1,1))
+        FX      = numpy.ravel( Hm( X ) ).reshape((-1,1))
         NormeX  = numpy.linalg.norm( X )
         NormeFX = numpy.linalg.norm( FX )
+        if NormeFX < mpr: NormeFX = mpr
         if self._toStore("CurrentState"):
-            self.StoredVariables["CurrentState"].store( numpy.ravel(Xn) )
+            self.StoredVariables["CurrentState"].store( X )
         if self._toStore("SimulatedObservationAtCurrentState"):
-            self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX) )
+            self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX )
         #
-        if len(self._parameters["InitialDirection"]) == 0:
-            dX0 = []
-            for v in X.A1:
-                if abs(v) > 1.e-8:
-                    dX0.append( numpy.random.normal(0.,abs(v)) )
-                else:
-                    dX0.append( numpy.random.normal(0.,X.mean()) )
-        else:
-            dX0 = numpy.ravel( self._parameters["InitialDirection"] )
-        #
-        dX0 = float(self._parameters["AmplitudeOfInitialDirection"]) * numpy.matrix( dX0 ).T
+        dX0 = NumericObjects.SetInitialDirection(
+            self._parameters["InitialDirection"],
+            self._parameters["AmplitudeOfInitialDirection"],
+            X,
+            )
         #
         if self._parameters["ResiduFormula"] in ["Taylor", "TaylorOnNorm"]:
-            dX1      = float(self._parameters["AmplitudeOfTangentPerturbation"]) * dX0
+            dX1      = float(self._parameters["AmplitudeOfTangentPerturbation"]) * dX0.reshape((-1,1))
             GradFxdX = Ht( (X, dX1) )
-            GradFxdX = numpy.asmatrix(numpy.ravel( GradFxdX )).T
+            GradFxdX = numpy.ravel( GradFxdX ).reshape((-1,1))
             GradFxdX = float(1./self._parameters["AmplitudeOfTangentPerturbation"]) * GradFxdX
         #
         # Entete des resultats
         # --------------------
         __marge =  12*u" "
         __precision = u"""
             Remarque : les nombres inferieurs a %.0e (environ) representent un zero
@@ -211,15 +203,15 @@
                                     Alpha
 
             qui doit rester constant jusqu'a ce que l'on atteigne la precision du calcul.
 
             On prend dX0 = Normal(0,X) et dX = Alpha*dX0. F est le code de calcul.\n""" + __precision
         #
         if len(self._parameters["ResultTitle"]) > 0:
-            __rt = unicode(self._parameters["ResultTitle"])
+            __rt = str(self._parameters["ResultTitle"])
             msgs  = u"\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
             msgs += __marge + "    " + __rt + "\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
         else:
             msgs  = u""
         msgs += __msgdoc
@@ -235,18 +227,18 @@
         NormesFXdX   = []
         NormesdFX    = []
         NormesdFXsdX = []
         NormesdFXsAm = []
         NormesdFXGdX = []
         #
         for i,amplitude in enumerate(Perturbations):
-            dX      = amplitude * dX0
+            dX      = amplitude * dX0.reshape((-1,1))
             #
             FX_plus_dX = Hm( X + dX )
-            FX_plus_dX = numpy.asmatrix(numpy.ravel( FX_plus_dX )).T
+            FX_plus_dX = numpy.ravel( FX_plus_dX ).reshape((-1,1))
             #
             if self._toStore("CurrentState"):
                 self.StoredVariables["CurrentState"].store( numpy.ravel(X + dX) )
             if self._toStore("SimulatedObservationAtCurrentState"):
                 self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_plus_dX) )
             #
             NormedX     = numpy.linalg.norm( dX )
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/InputValuesTest.py` & `adao-9.9.0.1/adao/daAlgorithms/InputValuesTest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,15 +16,14 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
 import numpy
 from daCore import BasicObjects
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "INPUTVALUESTEST")
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/KalmanFilter.py` & `adao-9.9.0.1/adao/daAlgorithms/LinearLeastSquares.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,27 +16,38 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
 from daCore import BasicObjects, NumericObjects
-import numpy
+from daAlgorithms.Atoms import ecwlls
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
-        BasicObjects.Algorithm.__init__(self, "KALMANFILTER")
+        BasicObjects.Algorithm.__init__(self, "LINEARLEASTSQUARES")
+        self.defineRequiredParameter(
+            name     = "Variant",
+            default  = "LinearLeastSquares",
+            typecast = str,
+            message  = "Variant ou formulation de la méthode",
+            listval  = [
+                "LinearLeastSquares",
+                ],
+            listadv  = [
+                "OneCorrection",
+                ],
+            )
         self.defineRequiredParameter(
             name     = "EstimationOf",
-            default  = "State",
+            default  = "Parameters",
             typecast = str,
-            message  = "Estimation d'etat ou de parametres",
+            message  = "Estimation d'état ou de paramètres",
             listval  = ["State", "Parameters"],
             )
         self.defineRequiredParameter(
             name     = "StoreInternalVariables",
             default  = False,
             typecast = bool,
             message  = "Stockage des variables internes ou intermédiaires du calcul",
@@ -44,55 +55,55 @@
         self.defineRequiredParameter(
             name     = "StoreSupplementaryCalculations",
             default  = [],
             typecast = tuple,
             message  = "Liste de calculs supplémentaires à stocker et/ou effectuer",
             listval  = [
                 "Analysis",
-                "APosterioriCorrelations",
-                "APosterioriCovariance",
-                "APosterioriStandardDeviations",
-                "APosterioriVariances",
-                "BMA",
                 "CostFunctionJ",
                 "CostFunctionJAtCurrentOptimum",
                 "CostFunctionJb",
                 "CostFunctionJbAtCurrentOptimum",
                 "CostFunctionJo",
                 "CostFunctionJoAtCurrentOptimum",
-                "CurrentIterationNumber",
                 "CurrentOptimum",
                 "CurrentState",
-                "ForecastCovariance",
+                "CurrentStepNumber",
                 "ForecastState",
-                "IndexOfOptimum",
                 "InnovationAtCurrentAnalysis",
-                "InnovationAtCurrentState",
-                "SimulatedObservationAtCurrentAnalysis",
+                "OMA",
                 "SimulatedObservationAtCurrentOptimum",
                 "SimulatedObservationAtCurrentState",
+                "SimulatedObservationAtOptimum",
                 ]
             )
         self.requireInputArguments(
-            mandatory= ("Xb", "Y", "HO", "R", "B"),
-            optional = ("U", "EM", "CM", "Q"),
+            mandatory= ("Y", "HO"),
+            optional = ("R"),
             )
         self.setAttributes(tags=(
-            "DataAssimilation",
+            "Optimization",
             "Linear",
-            "Filter",
-            "Dynamic",
+            "Variational",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
-        NumericObjects.stdkf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+        if   self._parameters["Variant"] == "LinearLeastSquares":
+            NumericObjects.multiXOsteps(self, Xb, Y, U, HO, EM, CM, R, B, Q, ecwlls.ecwlls)
+        #
+        #--------------------------
+        elif self._parameters["Variant"] == "OneCorrection":
+            ecwlls.ecwlls(self, Xb, Y, U, HO, CM, R, B)
+        #
         #--------------------------
+        else:
+            raise ValueError("Error in Variant name: %s"%self._parameters["Variant"])
         #
         self._post_run(HO)
         return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/LinearityTest.py` & `adao-9.9.0.1/adao/daAlgorithms/LinearityTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,20 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
-from daCore import BasicObjects, PlatformInfo
-import numpy, math
+import math, numpy
+from daCore import BasicObjects, NumericObjects, PlatformInfo
 mpr = PlatformInfo.PlatformInfo().MachinePrecision()
-if sys.version_info.major > 2:
-    unicode = str
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "LINEARITYTEST")
         self.defineRequiredParameter(
             name     = "ResiduFormula",
@@ -98,56 +95,41 @@
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         def RMS(V1, V2):
             import math
             return math.sqrt( ((numpy.ravel(V2) - numpy.ravel(V1))**2).sum() / float(numpy.ravel(V1).size) )
         #
-        # Operateurs
-        # ----------
         Hm = HO["Direct"].appliedTo
         if self._parameters["ResiduFormula"] in ["Taylor", "NominalTaylor", "NominalTaylorRMS"]:
             Ht = HO["Tangent"].appliedInXTo
         #
-        # Construction des perturbations
-        # ------------------------------
         Perturbations = [ 10**i for i in range(self._parameters["EpsilonMinimumExponent"],1) ]
         Perturbations.reverse()
         #
-        # Calcul du point courant
-        # -----------------------
-        Xn      = numpy.asmatrix(numpy.ravel( Xb )).T
-        FX      = numpy.asmatrix(numpy.ravel( Hm( Xn ) )).T
+        Xn      = numpy.ravel(     Xb   ).reshape((-1,1))
+        FX      = numpy.ravel( Hm( Xn ) ).reshape((-1,1))
         NormeX  = numpy.linalg.norm( Xn )
         NormeFX = numpy.linalg.norm( FX )
+        if NormeFX < mpr: NormeFX = mpr
         if self._toStore("CurrentState"):
             self.StoredVariables["CurrentState"].store( numpy.ravel(Xn) )
         if self._toStore("SimulatedObservationAtCurrentState"):
             self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX) )
         #
-        # Fabrication de la direction de l'increment dX
-        # ---------------------------------------------
-        if len(self._parameters["InitialDirection"]) == 0:
-            dX0 = []
-            for v in Xn.A1:
-                if abs(v) > 1.e-8:
-                    dX0.append( numpy.random.normal(0.,abs(v)) )
-                else:
-                    dX0.append( numpy.random.normal(0.,Xn.mean()) )
-        else:
-            dX0 = numpy.ravel( self._parameters["InitialDirection"] )
-        #
-        dX0 = float(self._parameters["AmplitudeOfInitialDirection"]) * numpy.matrix( dX0 ).T
+        dX0 = NumericObjects.SetInitialDirection(
+            self._parameters["InitialDirection"],
+            self._parameters["AmplitudeOfInitialDirection"],
+            Xn,
+            )
         #
-        # Calcul du gradient au point courant X pour l'increment dX
-        # ---------------------------------------------------------
         if self._parameters["ResiduFormula"] in ["Taylor", "NominalTaylor", "NominalTaylorRMS"]:
             dX1      = float(self._parameters["AmplitudeOfTangentPerturbation"]) * dX0
             GradFxdX = Ht( (Xn, dX1) )
-            GradFxdX = numpy.asmatrix(numpy.ravel( GradFxdX )).T
+            GradFxdX = numpy.ravel( GradFxdX ).reshape((-1,1))
             GradFxdX = float(1./self._parameters["AmplitudeOfTangentPerturbation"]) * GradFxdX
         #
         # Entete des resultats
         # --------------------
         __marge =  12*u" "
         __precision = u"""
             Remarque : les nombres inferieurs a %.0e (environ) representent un zero
@@ -234,15 +216,15 @@
             S'il est egal a 0 sur une partie seulement du domaine de variation de
             l'increment Alpha, c'est sur cette partie que l'hypothese de linearite de F
             est verifiee.
 
             On prend dX0 = Normal(0,X) et dX = Alpha*dX0. F est le code de calcul.\n""" + __precision
         #
         if len(self._parameters["ResultTitle"]) > 0:
-            __rt = unicode(self._parameters["ResultTitle"])
+            __rt = str(self._parameters["ResultTitle"])
             msgs  = u"\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
             msgs += __marge + "    " + __rt + "\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
         else:
             msgs  = u""
         msgs += __msgdoc
@@ -251,87 +233,87 @@
         msgs += "\n" + __marge + "-"*__nbtirets
         msgs += "\n" + __marge + __entete
         msgs += "\n" + __marge + "-"*__nbtirets
         #
         # Boucle sur les perturbations
         # ----------------------------
         for i,amplitude in enumerate(Perturbations):
-            dX      = amplitude * dX0
+            dX      = amplitude * dX0.reshape((-1,1))
             #
             if self._parameters["ResiduFormula"] == "CenteredDL":
                 if self._toStore("CurrentState"):
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn + dX) )
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn - dX) )
+                    self.StoredVariables["CurrentState"].store( Xn + dX )
+                    self.StoredVariables["CurrentState"].store( Xn - dX )
                 #
-                FX_plus_dX  = numpy.asmatrix(numpy.ravel( Hm( Xn + dX ) )).T
-                FX_moins_dX = numpy.asmatrix(numpy.ravel( Hm( Xn - dX ) )).T
+                FX_plus_dX  = numpy.ravel( Hm( Xn + dX ) ).reshape((-1,1))
+                FX_moins_dX = numpy.ravel( Hm( Xn - dX ) ).reshape((-1,1))
                 #
                 if self._toStore("SimulatedObservationAtCurrentState"):
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_plus_dX) )
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_moins_dX) )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_plus_dX )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_moins_dX )
                 #
                 Residu = numpy.linalg.norm( FX_plus_dX + FX_moins_dX - 2 * FX ) / NormeFX
                 #
                 self.StoredVariables["Residu"].store( Residu )
                 msg = "  %2i  %5.0e   %9.3e   %9.3e   |   %9.3e   %4.0f"%(i,amplitude,NormeX,NormeFX,Residu,math.log10(max(1.e-99,Residu)))
                 msgs += "\n" + __marge + msg
             #
             if self._parameters["ResiduFormula"] == "Taylor":
                 if self._toStore("CurrentState"):
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn + dX) )
+                    self.StoredVariables["CurrentState"].store( Xn + dX )
                 #
-                FX_plus_dX  = numpy.asmatrix(numpy.ravel( Hm( Xn + dX ) )).T
+                FX_plus_dX  = numpy.ravel( Hm( Xn + dX ) ).reshape((-1,1))
                 #
                 if self._toStore("SimulatedObservationAtCurrentState"):
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_plus_dX) )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_plus_dX )
                 #
                 Residu = numpy.linalg.norm( FX_plus_dX - FX - amplitude * GradFxdX ) / NormeFX
                 #
                 self.StoredVariables["Residu"].store( Residu )
                 msg = "  %2i  %5.0e   %9.3e   %9.3e   |   %9.3e   %4.0f"%(i,amplitude,NormeX,NormeFX,Residu,math.log10(max(1.e-99,Residu)))
                 msgs += "\n" + __marge + msg
             #
             if self._parameters["ResiduFormula"] == "NominalTaylor":
                 if self._toStore("CurrentState"):
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn + dX) )
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn - dX) )
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(dX) )
-                #
-                FX_plus_dX  = numpy.asmatrix(numpy.ravel( Hm( Xn + dX ) )).T
-                FX_moins_dX = numpy.asmatrix(numpy.ravel( Hm( Xn - dX ) )).T
-                FdX         = numpy.asmatrix(numpy.ravel( Hm( dX ) )).T
+                    self.StoredVariables["CurrentState"].store( Xn + dX )
+                    self.StoredVariables["CurrentState"].store( Xn - dX )
+                    self.StoredVariables["CurrentState"].store( dX )
+                #
+                FX_plus_dX  = numpy.ravel( Hm( Xn + dX ) ).reshape((-1,1))
+                FX_moins_dX = numpy.ravel( Hm( Xn - dX ) ).reshape((-1,1))
+                FdX         = numpy.ravel( Hm( dX )      ).reshape((-1,1))
                 #
                 if self._toStore("SimulatedObservationAtCurrentState"):
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_plus_dX) )
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_moins_dX) )
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FdX) )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_plus_dX )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_moins_dX )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FdX )
                 #
                 Residu = max(
                     numpy.linalg.norm( FX_plus_dX  - amplitude * FdX ) / NormeFX,
                     numpy.linalg.norm( FX_moins_dX + amplitude * FdX ) / NormeFX,
                     )
                 #
                 self.StoredVariables["Residu"].store( Residu )
                 msg = "  %2i  %5.0e   %9.3e   %9.3e   |   %9.3e   %5i %s"%(i,amplitude,NormeX,NormeFX,Residu,100.*abs(Residu-1.),"%")
                 msgs += "\n" + __marge + msg
             #
             if self._parameters["ResiduFormula"] == "NominalTaylorRMS":
                 if self._toStore("CurrentState"):
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn + dX) )
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(Xn - dX) )
-                    self.StoredVariables["CurrentState"].store( numpy.ravel(dX) )
-                #
-                FX_plus_dX  = numpy.asmatrix(numpy.ravel( Hm( Xn + dX ) )).T
-                FX_moins_dX = numpy.asmatrix(numpy.ravel( Hm( Xn - dX ) )).T
-                FdX         = numpy.asmatrix(numpy.ravel( Hm( dX ) )).T
+                    self.StoredVariables["CurrentState"].store( Xn + dX )
+                    self.StoredVariables["CurrentState"].store( Xn - dX )
+                    self.StoredVariables["CurrentState"].store( dX )
+                #
+                FX_plus_dX  = numpy.ravel( Hm( Xn + dX ) ).reshape((-1,1))
+                FX_moins_dX = numpy.ravel( Hm( Xn - dX ) ).reshape((-1,1))
+                FdX         = numpy.ravel( Hm( dX )      ).reshape((-1,1))
                 #
                 if self._toStore("SimulatedObservationAtCurrentState"):
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_plus_dX) )
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX_moins_dX) )
-                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FdX) )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_plus_dX )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX_moins_dX )
+                    self.StoredVariables["SimulatedObservationAtCurrentState"].store( FdX )
                 #
                 Residu = max(
                     RMS( FX, FX_plus_dX   - amplitude * FdX ) / NormeFX,
                     RMS( FX, FX_moins_dX  + amplitude * FdX ) / NormeFX,
                     )
                 #
                 self.StoredVariables["Residu"].store( Residu )
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/LocalSensitivityTest.py` & `adao-9.9.0.1/adao/daAlgorithms/LocalSensitivityTest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,16 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
-from daCore import BasicObjects, PlatformInfo
-import numpy, copy
+import logging, numpy
+from daCore import BasicObjects
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "LOCALSENSITIVITYTEST")
         self.defineRequiredParameter(
             name     = "SetDebug",
@@ -76,15 +75,15 @@
         if self._toStore("JacobianMatrixAtCurrentState"):
             self.StoredVariables["JacobianMatrixAtCurrentState"].store( Ht )
         if self._toStore("SimulatedObservationAtCurrentState"):
             if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
                 HXb = HO["AppliedInX"]["HXb"]
             else:
                 HXb = Ht @ Xb
-            HXb = numpy.asmatrix(numpy.ravel( HXb )).T
+            HXb = numpy.ravel( HXb ).reshape((-1,1))
             if Y.size != HXb.size:
                 raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
             if max(Y.shape) != max(HXb.shape):
                 raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
             self.StoredVariables["SimulatedObservationAtCurrentState"].store( HXb )
         #
         self._post_run(HO)
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/NonLinearLeastSquares.py` & `adao-9.9.0.1/adao/daAlgorithms/Atoms/van3dvar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,334 +16,265 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects
-import numpy, scipy.optimize, scipy.version
+__doc__ = """
+    3DVAR variational analysis with no inversion of B
+"""
+__author__ = "Jean-Philippe ARGAUD"
+
+import numpy, scipy, scipy.optimize, scipy.version
+from daCore.NumericObjects import HessienneEstimation, QuantilesEstimations
+from daCore.NumericObjects import RecentredBounds
+from daCore.PlatformInfo import PlatformInfo
+mpr = PlatformInfo().MachinePrecision()
 
 # ==============================================================================
-class ElementaryAlgorithm(BasicObjects.Algorithm):
-    def __init__(self):
-        BasicObjects.Algorithm.__init__(self, "NONLINEARLEASTSQUARES")
-        self.defineRequiredParameter(
-            name     = "Minimizer",
-            default  = "LBFGSB",
-            typecast = str,
-            message  = "Minimiseur utilisé",
-            listval  = [
-                "LBFGSB",
-                "TNC",
-                "CG",
-                "NCG",
-                "BFGS",
-                "LM",
-                ],
-            )
-        self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
-            default  = 15000,
-            typecast = int,
-            message  = "Nombre maximal de pas d'optimisation",
-            minval   = -1,
-            )
-        self.defineRequiredParameter(
-            name     = "CostDecrementTolerance",
-            default  = 1.e-7,
-            typecast = float,
-            message  = "Diminution relative minimale du coût lors de l'arrêt",
-            minval   = 0.,
-            )
-        self.defineRequiredParameter(
-            name     = "ProjectedGradientTolerance",
-            default  = -1,
-            typecast = float,
-            message  = "Maximum des composantes du gradient projeté lors de l'arrêt",
-            minval   = -1,
-            )
-        self.defineRequiredParameter(
-            name     = "GradientNormTolerance",
-            default  = 1.e-05,
-            typecast = float,
-            message  = "Maximum des composantes du gradient lors de l'arrêt",
-            minval   = 0.,
-            )
-        self.defineRequiredParameter(
-            name     = "StoreInternalVariables",
-            default  = False,
-            typecast = bool,
-            message  = "Stockage des variables internes ou intermédiaires du calcul",
+def van3dvar(selfA, Xb, Y, U, HO, CM, R, B, __storeState = False):
+    """
+    Correction
+    """
+    #
+    # Initialisations
+    # ---------------
+    Hm = HO["Direct"].appliedTo
+    Ha = HO["Adjoint"].appliedInXTo
+    #
+    if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
+        HXb = numpy.asarray(Hm( Xb, HO["AppliedInX"]["HXb"] ))
+    else:
+        HXb = numpy.asarray(Hm( Xb ))
+    HXb = HXb.reshape((-1,1))
+    if Y.size != HXb.size:
+        raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
+    if max(Y.shape) != max(HXb.shape):
+        raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
+    #
+    if selfA._toStore("JacobianMatrixAtBackground"):
+        HtMb = HO["Tangent"].asMatrix(ValueForMethodForm = Xb)
+        HtMb = HtMb.reshape(Y.size,Xb.size) # ADAO & check shape
+        selfA.StoredVariables["JacobianMatrixAtBackground"].store( HtMb )
+    #
+    BT = B.getT()
+    RI = R.getI()
+    if ("Bounds" in selfA._parameters) and selfA._parameters["Bounds"] is not None:
+        BI = B.getI()
+    else:
+        BI = None
+    #
+    Xini = numpy.zeros(Xb.size)
+    #
+    # Définition de la fonction-coût
+    # ------------------------------
+    def CostFunction(v):
+        _V = numpy.asarray(v).reshape((-1,1))
+        _X = Xb + (B @ _V).reshape((-1,1))
+        if selfA._parameters["StoreInternalVariables"] or \
+            selfA._toStore("CurrentState") or \
+            selfA._toStore("CurrentOptimum"):
+            selfA.StoredVariables["CurrentState"].store( _X )
+        _HX = numpy.asarray(Hm( _X )).reshape((-1,1))
+        _Innovation = Y - _HX
+        if selfA._toStore("SimulatedObservationAtCurrentState") or \
+            selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            selfA.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
+        if selfA._toStore("InnovationAtCurrentState"):
+            selfA.StoredVariables["InnovationAtCurrentState"].store( _Innovation )
+        #
+        Jb  = float( 0.5 * _V.T * (BT * _V) )
+        Jo  = float( 0.5 * _Innovation.T * (RI * _Innovation) )
+        J   = Jb + Jo
+        #
+        selfA.StoredVariables["CurrentIterationNumber"].store( len(selfA.StoredVariables["CostFunctionJ"]) )
+        selfA.StoredVariables["CostFunctionJb"].store( Jb )
+        selfA.StoredVariables["CostFunctionJo"].store( Jo )
+        selfA.StoredVariables["CostFunctionJ" ].store( J )
+        if selfA._toStore("IndexOfOptimum") or \
+            selfA._toStore("CurrentOptimum") or \
+            selfA._toStore("CostFunctionJAtCurrentOptimum") or \
+            selfA._toStore("CostFunctionJbAtCurrentOptimum") or \
+            selfA._toStore("CostFunctionJoAtCurrentOptimum") or \
+            selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            IndexMin = numpy.argmin( selfA.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+        if selfA._toStore("IndexOfOptimum"):
+            selfA.StoredVariables["IndexOfOptimum"].store( IndexMin )
+        if selfA._toStore("CurrentOptimum"):
+            selfA.StoredVariables["CurrentOptimum"].store( selfA.StoredVariables["CurrentState"][IndexMin] )
+        if selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            selfA.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( selfA.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin] )
+        if selfA._toStore("CostFunctionJbAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( selfA.StoredVariables["CostFunctionJb"][IndexMin] )
+        if selfA._toStore("CostFunctionJoAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( selfA.StoredVariables["CostFunctionJo"][IndexMin] )
+        if selfA._toStore("CostFunctionJAtCurrentOptimum"):
+            selfA.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( selfA.StoredVariables["CostFunctionJ" ][IndexMin] )
+        return J
+    #
+    def GradientOfCostFunction(v):
+        _V = numpy.asarray(v).reshape((-1,1))
+        _X = Xb + (B @ _V).reshape((-1,1))
+        _HX     = numpy.asarray(Hm( _X )).reshape((-1,1))
+        GradJb  = BT * _V
+        GradJo  = - BT * Ha( (_X, RI * (Y - _HX)) )
+        GradJ   = numpy.ravel( GradJb ) + numpy.ravel( GradJo )
+        return GradJ
+    #
+    # Minimisation de la fonctionnelle
+    # --------------------------------
+    nbPreviousSteps = selfA.StoredVariables["CostFunctionJ"].stepnumber()
+    #
+    if selfA._parameters["Minimizer"] == "LBFGSB":
+        if "0.19" <= scipy.version.version <= "1.4.1":
+            import daAlgorithms.Atoms.lbfgsbhlt as optimiseur
+        else:
+            import scipy.optimize as optimiseur
+        Minimum, J_optimal, Informations = optimiseur.fmin_l_bfgs_b(
+            func        = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            bounds      = RecentredBounds(selfA._parameters["Bounds"], Xb, BI),
+            maxfun      = selfA._parameters["MaximumNumberOfIterations"]-1,
+            factr       = selfA._parameters["CostDecrementTolerance"]*1.e14,
+            pgtol       = selfA._parameters["ProjectedGradientTolerance"],
+            iprint      = selfA._parameters["optiprint"],
             )
-        self.defineRequiredParameter(
-            name     = "StoreSupplementaryCalculations",
-            default  = [],
-            typecast = tuple,
-            message  = "Liste de calculs supplémentaires à stocker et/ou effectuer",
-            listval  = [
-                "Analysis",
-                "BMA",
-                "CostFunctionJ",
-                "CostFunctionJAtCurrentOptimum",
-                "CostFunctionJb",
-                "CostFunctionJbAtCurrentOptimum",
-                "CostFunctionJo",
-                "CostFunctionJoAtCurrentOptimum",
-                "CurrentIterationNumber",
-                "CurrentOptimum",
-                "CurrentState",
-                "IndexOfOptimum",
-                "Innovation",
-                "InnovationAtCurrentState",
-                "OMA",
-                "OMB",
-                "SimulatedObservationAtBackground",
-                "SimulatedObservationAtCurrentOptimum",
-                "SimulatedObservationAtCurrentState",
-                "SimulatedObservationAtOptimum",
-                ]
+        # nfeval = Informations['funcalls']
+        # rc     = Informations['warnflag']
+    elif selfA._parameters["Minimizer"] == "TNC":
+        Minimum, nfeval, rc = scipy.optimize.fmin_tnc(
+            func        = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            bounds      = RecentredBounds(selfA._parameters["Bounds"], Xb, BI),
+            maxfun      = selfA._parameters["MaximumNumberOfIterations"],
+            pgtol       = selfA._parameters["ProjectedGradientTolerance"],
+            ftol        = selfA._parameters["CostDecrementTolerance"],
+            messages    = selfA._parameters["optmessages"],
             )
-        self.defineRequiredParameter( # Pas de type
-            name     = "Bounds",
-            message  = "Liste des paires de bornes",
+    elif selfA._parameters["Minimizer"] == "CG":
+        Minimum, fopt, nfeval, grad_calls, rc = scipy.optimize.fmin_cg(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
             )
-        self.defineRequiredParameter(
-            name     = "InitializationPoint",
-            typecast = numpy.ravel,
-            message  = "État initial imposé (par défaut, c'est l'ébauche si None)",
+    elif selfA._parameters["Minimizer"] == "NCG":
+        Minimum, fopt, nfeval, grad_calls, hcalls, rc = scipy.optimize.fmin_ncg(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            avextol     = selfA._parameters["CostDecrementTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
             )
-        self.requireInputArguments(
-            mandatory= ("Xb", "Y", "HO", "R"),
+    elif selfA._parameters["Minimizer"] == "BFGS":
+        Minimum, fopt, gopt, Hopt, nfeval, grad_calls, rc = scipy.optimize.fmin_bfgs(
+            f           = CostFunction,
+            x0          = Xini,
+            fprime      = GradientOfCostFunction,
+            args        = (),
+            maxiter     = selfA._parameters["MaximumNumberOfIterations"],
+            gtol        = selfA._parameters["GradientNormTolerance"],
+            disp        = selfA._parameters["optdisp"],
+            full_output = True,
             )
-        self.setAttributes(tags=(
-            "Optimization",
-            "NonLinear",
-            "Variational",
-            ))
-
-    def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
-        self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
-        #
-        # Initialisations
-        # ---------------
-        Hm = HO["Direct"].appliedTo
-        Ha = HO["Adjoint"].appliedInXTo
-        #
-        if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
-            HXb = Hm( Xb, HO["AppliedInX"]["HXb"] )
-        else:
-            HXb = Hm( Xb )
-        HXb = HXb.reshape((-1,1))
-        if Y.size != HXb.size:
-            raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
-        if max(Y.shape) != max(HXb.shape):
-            raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
-        #
-        RI = R.getI()
-        if self._parameters["Minimizer"] == "LM":
-            RdemiI = R.choleskyI()
-        #
-        Xini = self._parameters["InitializationPoint"]
-        #
-        # Définition de la fonction-coût
-        # ------------------------------
-        def CostFunction(x):
-            _X  = numpy.ravel( x ).reshape((-1,1))
-            if self._parameters["StoreInternalVariables"] or \
-                self._toStore("CurrentState") or \
-                self._toStore("CurrentOptimum"):
-                self.StoredVariables["CurrentState"].store( _X )
-            _HX = Hm( _X ).reshape((-1,1))
-            _Innovation = Y - _HX
-            if self._toStore("SimulatedObservationAtCurrentState") or \
-                self._toStore("SimulatedObservationAtCurrentOptimum"):
-                self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
-            if self._toStore("InnovationAtCurrentState"):
-                self.StoredVariables["InnovationAtCurrentState"].store( _Innovation )
-            #
-            Jb  = 0.
-            Jo  = float( 0.5 * _Innovation.T * (RI * _Innovation) )
-            J   = Jb + Jo
-            #
-            self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
-            self.StoredVariables["CostFunctionJb"].store( Jb )
-            self.StoredVariables["CostFunctionJo"].store( Jo )
-            self.StoredVariables["CostFunctionJ" ].store( J )
-            if self._toStore("IndexOfOptimum") or \
-                self._toStore("CurrentOptimum") or \
-                self._toStore("CostFunctionJAtCurrentOptimum") or \
-                self._toStore("CostFunctionJbAtCurrentOptimum") or \
-                self._toStore("CostFunctionJoAtCurrentOptimum") or \
-                self._toStore("SimulatedObservationAtCurrentOptimum"):
-                IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
-            if self._toStore("IndexOfOptimum"):
-                self.StoredVariables["IndexOfOptimum"].store( IndexMin )
-            if self._toStore("CurrentOptimum"):
-                self.StoredVariables["CurrentOptimum"].store( self.StoredVariables["CurrentState"][IndexMin] )
-            if self._toStore("SimulatedObservationAtCurrentOptimum"):
-                self.StoredVariables["SimulatedObservationAtCurrentOptimum"].store( self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin] )
-            if self._toStore("CostFunctionJbAtCurrentOptimum"):
-                self.StoredVariables["CostFunctionJbAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJb"][IndexMin] )
-            if self._toStore("CostFunctionJoAtCurrentOptimum"):
-                self.StoredVariables["CostFunctionJoAtCurrentOptimum"].store( self.StoredVariables["CostFunctionJo"][IndexMin] )
-            if self._toStore("CostFunctionJAtCurrentOptimum"):
-                self.StoredVariables["CostFunctionJAtCurrentOptimum" ].store( self.StoredVariables["CostFunctionJ" ][IndexMin] )
-            return J
-        #
-        def GradientOfCostFunction(x):
-            _X      = x.reshape((-1,1))
-            _HX     = Hm( _X ).reshape((-1,1))
-            GradJb  = 0.
-            GradJo  = - Ha( (_X, RI * (Y - _HX)) )
-            GradJ   = numpy.ravel( GradJb ) + numpy.ravel( GradJo )
-            return GradJ
-        #
-        def CostFunctionLM(x):
-            _X  = numpy.ravel( x ).reshape((-1,1))
-            _HX = Hm( _X ).reshape((-1,1))
-            _Innovation = Y - _HX
-            Jb  = 0.
-            Jo  = float( 0.5 * _Innovation.T * (RI * _Innovation) )
-            J   = Jb + Jo
-            if self._parameters["StoreInternalVariables"] or \
-                self._toStore("CurrentState"):
-                self.StoredVariables["CurrentState"].store( _X )
-            self.StoredVariables["CostFunctionJb"].store( Jb )
-            self.StoredVariables["CostFunctionJo"].store( Jo )
-            self.StoredVariables["CostFunctionJ" ].store( J )
-            #
-            return numpy.ravel( RdemiI*_Innovation )
-        #
-        def GradientOfCostFunctionLM(x):
-            _X      = x.reshape((-1,1))
-            return - RdemiI*HO["Tangent"].asMatrix( _X )
-        #
-        # Minimisation de la fonctionnelle
-        # --------------------------------
-        nbPreviousSteps = self.StoredVariables["CostFunctionJ"].stepnumber()
-        #
-        if self._parameters["Minimizer"] == "LBFGSB":
-            if "0.19" <= scipy.version.version <= "1.1.0":
-                import lbfgsbhlt as optimiseur
-            else:
-                import scipy.optimize as optimiseur
-            Minimum, J_optimal, Informations = optimiseur.fmin_l_bfgs_b(
-                func        = CostFunction,
-                x0          = Xini,
-                fprime      = GradientOfCostFunction,
-                args        = (),
-                bounds      = self._parameters["Bounds"],
-                maxfun      = self._parameters["MaximumNumberOfSteps"]-1,
-                factr       = self._parameters["CostDecrementTolerance"]*1.e14,
-                pgtol       = self._parameters["ProjectedGradientTolerance"],
-                iprint      = self._parameters["optiprint"],
-                )
-            nfeval = Informations['funcalls']
-            rc     = Informations['warnflag']
-        elif self._parameters["Minimizer"] == "TNC":
-            Minimum, nfeval, rc = scipy.optimize.fmin_tnc(
-                func        = CostFunction,
-                x0          = Xini,
-                fprime      = GradientOfCostFunction,
-                args        = (),
-                bounds      = self._parameters["Bounds"],
-                maxfun      = self._parameters["MaximumNumberOfSteps"],
-                pgtol       = self._parameters["ProjectedGradientTolerance"],
-                ftol        = self._parameters["CostDecrementTolerance"],
-                messages    = self._parameters["optmessages"],
-                )
-        elif self._parameters["Minimizer"] == "CG":
-            Minimum, fopt, nfeval, grad_calls, rc = scipy.optimize.fmin_cg(
-                f           = CostFunction,
-                x0          = Xini,
-                fprime      = GradientOfCostFunction,
-                args        = (),
-                maxiter     = self._parameters["MaximumNumberOfSteps"],
-                gtol        = self._parameters["GradientNormTolerance"],
-                disp        = self._parameters["optdisp"],
-                full_output = True,
-                )
-        elif self._parameters["Minimizer"] == "NCG":
-            Minimum, fopt, nfeval, grad_calls, hcalls, rc = scipy.optimize.fmin_ncg(
-                f           = CostFunction,
-                x0          = Xini,
-                fprime      = GradientOfCostFunction,
-                args        = (),
-                maxiter     = self._parameters["MaximumNumberOfSteps"],
-                avextol     = self._parameters["CostDecrementTolerance"],
-                disp        = self._parameters["optdisp"],
-                full_output = True,
-                )
-        elif self._parameters["Minimizer"] == "BFGS":
-            Minimum, fopt, gopt, Hopt, nfeval, grad_calls, rc = scipy.optimize.fmin_bfgs(
-                f           = CostFunction,
-                x0          = Xini,
-                fprime      = GradientOfCostFunction,
-                args        = (),
-                maxiter     = self._parameters["MaximumNumberOfSteps"],
-                gtol        = self._parameters["GradientNormTolerance"],
-                disp        = self._parameters["optdisp"],
-                full_output = True,
-                )
-        elif self._parameters["Minimizer"] == "LM":
-            Minimum, cov_x, infodict, mesg, rc = scipy.optimize.leastsq(
-                func        = CostFunctionLM,
-                x0          = Xini,
-                Dfun        = GradientOfCostFunctionLM,
-                args        = (),
-                ftol        = self._parameters["CostDecrementTolerance"],
-                maxfev      = self._parameters["MaximumNumberOfSteps"],
-                gtol        = self._parameters["GradientNormTolerance"],
-                full_output = True,
-                )
-            nfeval = infodict['nfev']
+    else:
+        raise ValueError("Error in minimizer name: %s is unkown"%selfA._parameters["Minimizer"])
+    #
+    IndexMin = numpy.argmin( selfA.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
+    MinJ     = selfA.StoredVariables["CostFunctionJ"][IndexMin]
+    #
+    # Correction pour pallier a un bug de TNC sur le retour du Minimum
+    # ----------------------------------------------------------------
+    if selfA._parameters["StoreInternalVariables"] or selfA._toStore("CurrentState"):
+        Minimum = selfA.StoredVariables["CurrentState"][IndexMin]
+    else:
+        Minimum = Xb + B * Minimum.reshape((-1,1)) # Pas @
+    #
+    Xa = Minimum
+    if __storeState: selfA._setInternalState("Xn", Xa)
+    #--------------------------
+    #
+    selfA.StoredVariables["Analysis"].store( Xa )
+    #
+    if selfA._toStore("OMA") or \
+        selfA._toStore("InnovationAtCurrentAnalysis") or \
+        selfA._toStore("SigmaObs2") or \
+        selfA._toStore("SimulationQuantiles") or \
+        selfA._toStore("SimulatedObservationAtOptimum"):
+        if selfA._toStore("SimulatedObservationAtCurrentState"):
+            HXa = selfA.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin]
+        elif selfA._toStore("SimulatedObservationAtCurrentOptimum"):
+            HXa = selfA.StoredVariables["SimulatedObservationAtCurrentOptimum"][-1]
         else:
-            raise ValueError("Error in Minimizer name: %s"%self._parameters["Minimizer"])
-        #
-        IndexMin = numpy.argmin( self.StoredVariables["CostFunctionJ"][nbPreviousSteps:] ) + nbPreviousSteps
-        MinJ     = self.StoredVariables["CostFunctionJ"][IndexMin]
-        #
-        # Correction pour pallier a un bug de TNC sur le retour du Minimum
-        # ----------------------------------------------------------------
-        if self._parameters["StoreInternalVariables"] or self._toStore("CurrentState"):
-            Minimum = self.StoredVariables["CurrentState"][IndexMin]
-        #
-        Xa = Minimum
-        #--------------------------
-        #
-        self.StoredVariables["Analysis"].store( Xa )
-        #
-        if self._toStore("OMA") or \
-            self._toStore("SimulatedObservationAtOptimum"):
-            if self._toStore("SimulatedObservationAtCurrentState"):
-                HXa = self.StoredVariables["SimulatedObservationAtCurrentState"][IndexMin]
-            elif self._toStore("SimulatedObservationAtCurrentOptimum"):
-                HXa = self.StoredVariables["SimulatedObservationAtCurrentOptimum"][-1]
-            else:
-                HXa = Hm( Xa )
-        #
-        # Calculs et/ou stockages supplémentaires
-        # ---------------------------------------
-        if self._toStore("Innovation") or \
-            self._toStore("OMB"):
-            Innovation  = Y - HXb
-        if self._toStore("Innovation"):
-            self.StoredVariables["Innovation"].store( Innovation )
-        if self._toStore("BMA"):
-            self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
-        if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( numpy.ravel(Y) - numpy.ravel(HXa) )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( Innovation )
-        if self._toStore("SimulatedObservationAtBackground"):
-            self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
-        if self._toStore("SimulatedObservationAtOptimum"):
-            self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
-        #
-        self._post_run(HO)
-        return 0
+            HXa = Hm( Xa )
+        oma = Y - HXa.reshape((-1,1))
+    #
+    if selfA._toStore("APosterioriCovariance") or \
+        selfA._toStore("SimulationQuantiles") or \
+        selfA._toStore("JacobianMatrixAtOptimum") or \
+        selfA._toStore("KalmanGainAtOptimum"):
+        HtM = HO["Tangent"].asMatrix(ValueForMethodForm = Xa)
+        HtM = HtM.reshape(Y.size,Xa.size) # ADAO & check shape
+    if selfA._toStore("APosterioriCovariance") or \
+        selfA._toStore("SimulationQuantiles") or \
+        selfA._toStore("KalmanGainAtOptimum"):
+        HaM = HO["Adjoint"].asMatrix(ValueForMethodForm = Xa)
+        HaM = HaM.reshape(Xa.size,Y.size) # ADAO & check shape
+    if selfA._toStore("APosterioriCovariance") or \
+        selfA._toStore("SimulationQuantiles"):
+        BI = B.getI()
+        A = HessienneEstimation(selfA, Xa.size, HaM, HtM, BI, RI)
+    if selfA._toStore("APosterioriCovariance"):
+        selfA.StoredVariables["APosterioriCovariance"].store( A )
+    if selfA._toStore("JacobianMatrixAtOptimum"):
+        selfA.StoredVariables["JacobianMatrixAtOptimum"].store( HtM )
+    if selfA._toStore("KalmanGainAtOptimum"):
+        if   (Y.size <= Xb.size): KG  = B * HaM * (R + numpy.dot(HtM, B * HaM)).I
+        elif (Y.size >  Xb.size): KG = (BI + numpy.dot(HaM, RI * HtM)).I * HaM * RI
+        selfA.StoredVariables["KalmanGainAtOptimum"].store( KG )
+    #
+    # Calculs et/ou stockages supplémentaires
+    # ---------------------------------------
+    if selfA._toStore("Innovation") or \
+        selfA._toStore("SigmaObs2") or \
+        selfA._toStore("MahalanobisConsistency") or \
+        selfA._toStore("OMB"):
+        Innovation  = Y - HXb
+    if selfA._toStore("Innovation"):
+        selfA.StoredVariables["Innovation"].store( Innovation )
+    if selfA._toStore("BMA"):
+        selfA.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
+    if selfA._toStore("OMA"):
+        selfA.StoredVariables["OMA"].store( oma )
+    if selfA._toStore("InnovationAtCurrentAnalysis"):
+        selfA.StoredVariables["InnovationAtCurrentAnalysis"].store( oma )
+    if selfA._toStore("OMB"):
+        selfA.StoredVariables["OMB"].store( Innovation )
+    if selfA._toStore("SigmaObs2"):
+        TraceR = R.trace(Y.size)
+        selfA.StoredVariables["SigmaObs2"].store( float( (Innovation.T @ oma) ) / TraceR )
+    if selfA._toStore("MahalanobisConsistency"):
+        selfA.StoredVariables["MahalanobisConsistency"].store( float( 2.*MinJ/Innovation.size ) )
+    if selfA._toStore("SimulationQuantiles"):
+        QuantilesEstimations(selfA, A, Xa, HXa, Hm, HtM)
+    if selfA._toStore("SimulatedObservationAtBackground"):
+        selfA.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
+    if selfA._toStore("SimulatedObservationAtOptimum"):
+        selfA.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
+    #
+    return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/ObserverTest.py` & `adao-9.9.0.1/adao/daAlgorithms/ObserverTest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,16 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects
 import numpy
+from daCore import BasicObjects
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "OBSERVERTEST")
         self.setAttributes(tags=(
             "Checking",
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/ParallelFunctionTest.py` & `adao-9.9.0.1/adao/daAlgorithms/ParallelFunctionTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,21 +16,19 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
+import logging
 from daCore import BasicObjects, PlatformInfo
 import numpy, copy
 mpr = PlatformInfo.PlatformInfo().MachinePrecision()
 mfp = PlatformInfo.PlatformInfo().MaximumPrecision()
-if sys.version_info.major > 2:
-    unicode = str
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "PARALLELFUNCTIONTEST")
         self.defineRequiredParameter(
             name     = "NumberOfPrintedDigits",
@@ -82,26 +80,26 @@
         #
         Xn = copy.copy( Xb )
         #
         # ----------
         __marge =  5*u" "
         _p = self._parameters["NumberOfPrintedDigits"]
         if len(self._parameters["ResultTitle"]) > 0:
-            __rt = unicode(self._parameters["ResultTitle"])
+            __rt = str(self._parameters["ResultTitle"])
             msgs  = u"\n"
             msgs +=  __marge + "====" + "="*len(__rt) + "====\n"
             msgs +=  __marge + "    " + __rt + "\n"
             msgs +=  __marge + "====" + "="*len(__rt) + "====\n"
             print("%s"%msgs)
         #
         msgs  = ("===> Information before launching:\n")
         msgs += ("     -----------------------------\n")
         msgs += ("     Characteristics of input vector X, internally converted:\n")
         msgs += ("       Type...............: %s\n")%type( Xn )
-        msgs += ("       Lenght of vector...: %i\n")%max(numpy.matrix( Xn ).shape)
+        msgs += ("       Lenght of vector...: %i\n")%max(numpy.asarray( Xn ).shape)
         msgs += ("       Minimum value......: %."+str(_p)+"e\n")%numpy.min( Xn )
         msgs += ("       Maximum value......: %."+str(_p)+"e\n")%numpy.max( Xn )
         msgs += ("       Mean of vector.....: %."+str(_p)+"e\n")%numpy.mean( Xn, dtype=mfp )
         msgs += ("       Standard error.....: %."+str(_p)+"e\n")%numpy.std( Xn, dtype=mfp )
         msgs += ("       L2 norm of vector..: %."+str(_p)+"e\n")%numpy.linalg.norm( Xn )
         print(msgs)
         #
@@ -140,15 +138,15 @@
             if self._parameters["NumberOfRepetition"] > 1:
                 print("===> Repetition step number %i on a total of %i\n"%(i+1,self._parameters["NumberOfRepetition"]))
             #
             Yn = Ys[i]
             msgs  = ("===> Information after evaluation:\n")
             msgs += ("\n     Characteristics of simulated output vector Y=H(X), to compare to others:\n")
             msgs += ("       Type...............: %s\n")%type( Yn )
-            msgs += ("       Lenght of vector...: %i\n")%max(numpy.matrix( Yn ).shape)
+            msgs += ("       Lenght of vector...: %i\n")%max(numpy.asarray( Yn ).shape)
             msgs += ("       Minimum value......: %."+str(_p)+"e\n")%numpy.min( Yn )
             msgs += ("       Maximum value......: %."+str(_p)+"e\n")%numpy.max( Yn )
             msgs += ("       Mean of vector.....: %."+str(_p)+"e\n")%numpy.mean( Yn, dtype=mfp )
             msgs += ("       Standard error.....: %."+str(_p)+"e\n")%numpy.std( Yn, dtype=mfp )
             msgs += ("       L2 norm of vector..: %."+str(_p)+"e\n")%numpy.linalg.norm( Yn )
             print(msgs)
             if self._toStore("SimulatedObservationAtCurrentState"):
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/ParticleSwarmOptimization.py` & `adao-9.9.0.1/adao/daAlgorithms/ParticleSwarmOptimization.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,28 +16,28 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
+import numpy, logging, copy
 from daCore import BasicObjects
-import numpy, copy
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "PARTICLESWARMOPTIMIZATION")
         self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
+            name     = "MaximumNumberOfIterations",
             default  = 50,
             typecast = int,
             message  = "Nombre maximal de pas d'optimisation",
             minval   = 0,
+            oldname  = "MaximumNumberOfSteps",
             )
         self.defineRequiredParameter(
             name     = "MaximumNumberOfFunctionEvaluations",
             default  = 15000,
             typecast = int,
             message  = "Nombre maximal d'évaluations de la fonction",
             minval   = -1,
@@ -71,25 +71,20 @@
             )
         self.defineRequiredParameter(
             name     = "QualityCriterion",
             default  = "AugmentedWeightedLeastSquares",
             typecast = str,
             message  = "Critère de qualité utilisé",
             listval  = [
-                "DA",
-                "AugmentedWeightedLeastSquares", "AWLS",
+                "AugmentedWeightedLeastSquares", "AWLS", "DA",
                 "WeightedLeastSquares", "WLS",
                 "LeastSquares", "LS", "L2",
                 "AbsoluteValue", "L1",
                 "MaximumError", "ME",
                 ],
-            listadv  = [
-                "AugmentedPonderatedLeastSquares","APLS",
-                "PonderatedLeastSquares","PLS",
-                ]
             )
         self.defineRequiredParameter(
             name     = "StoreInternalVariables",
             default  = False,
             typecast = bool,
             message  = "Stockage des variables internes ou intermédiaires du calcul",
             )
@@ -120,14 +115,15 @@
             )
         self.requireInputArguments(
             mandatory= ("Xb", "Y", "HO", "R", "B"),
             )
         self.setAttributes(tags=(
             "Optimization",
             "NonLinear",
+            "MetaHeuristic",
             "Population",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         if ("BoxBounds" in self._parameters) and isinstance(self._parameters["BoxBounds"], (list, tuple)) and (len(self._parameters["BoxBounds"]) > 0):
@@ -144,40 +140,38 @@
         logging.debug("%s Taux de rappel au meilleur insecte du groupe (entre 0 et 1) = %s et à la meilleure position précédente (son complémentaire à 1) = %s"%(self._name, str(Phig), str(Phip)))
         #
         Hm = HO["Direct"].appliedTo
         #
         BI = B.getI()
         RI = R.getI()
         #
-        # Définition de la fonction-coût
-        # ------------------------------
         def CostFunction(x, QualityMeasure="AugmentedWeightedLeastSquares"):
-            _X  = numpy.asmatrix(numpy.ravel( x )).T
-            _HX = Hm( _X )
-            _HX = numpy.asmatrix(numpy.ravel( _HX )).T
+            _X  = numpy.ravel( x ).reshape((-1,1))
+            _HX = numpy.ravel( Hm( _X ) ).reshape((-1,1))
+            _Innovation = Y - _HX
             #
-            if QualityMeasure in ["AugmentedWeightedLeastSquares","AWLS","AugmentedPonderatedLeastSquares","APLS","DA"]:
+            if QualityMeasure in ["AugmentedWeightedLeastSquares","AWLS","DA"]:
                 if BI is None or RI is None:
-                    raise ValueError("Background and Observation error covariance matrix has to be properly defined!")
-                Jb  = 0.5 * (_X - Xb).T * BI * (_X - Xb)
-                Jo  = 0.5 * (Y - _HX).T * RI * (Y - _HX)
-            elif QualityMeasure in ["WeightedLeastSquares","WLS","PonderatedLeastSquares","PLS"]:
+                    raise ValueError("Background and Observation error covariance matrices has to be properly defined!")
+                Jb  = 0.5 * (_X - Xb).T @ (BI @ (_X - Xb))
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
+            elif QualityMeasure in ["WeightedLeastSquares","WLS"]:
                 if RI is None:
                     raise ValueError("Observation error covariance matrix has to be properly defined!")
                 Jb  = 0.
-                Jo  = 0.5 * (Y - _HX).T * RI * (Y - _HX)
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
             elif QualityMeasure in ["LeastSquares","LS","L2"]:
                 Jb  = 0.
-                Jo  = 0.5 * (Y - _HX).T * (Y - _HX)
+                Jo  = 0.5 * _Innovation.T @ _Innovation
             elif QualityMeasure in ["AbsoluteValue","L1"]:
                 Jb  = 0.
-                Jo  = numpy.sum( numpy.abs(Y - _HX) )
+                Jo  = numpy.sum( numpy.abs(_Innovation) )
             elif QualityMeasure in ["MaximumError","ME"]:
                 Jb  = 0.
-                Jo  = numpy.max( numpy.abs(Y - _HX) )
+                Jo  = numpy.max( numpy.abs(_Innovation) )
             #
             J   = float( Jb ) + float( Jo )
             #
             return J
         #
         if Xb is not None:
             Xini = numpy.ravel(Xb)
@@ -194,99 +188,97 @@
         LimitVelocity = numpy.abs(SpaceUp-SpaceLow)
         #
         PosInsect = []
         VelocityInsect = []
         for i in range(nbparam) :
             PosInsect.append(numpy.random.uniform(low=SpaceLow[i], high=SpaceUp[i], size=self._parameters["NumberOfInsects"]))
             VelocityInsect.append(numpy.random.uniform(low=-LimitVelocity[i], high=LimitVelocity[i], size=self._parameters["NumberOfInsects"]))
-        VelocityInsect = numpy.matrix(VelocityInsect)
-        PosInsect = numpy.matrix(PosInsect)
+        VelocityInsect = numpy.array(VelocityInsect)
+        PosInsect = numpy.array(PosInsect)
         #
         BestPosInsect = numpy.array(PosInsect)
         qBestPosInsect = []
-        Best = copy.copy(SpaceLow)
-        qBest = CostFunction(Best,self._parameters["QualityCriterion"])
+        _Best = copy.copy(SpaceLow)
+        _qualityBest = CostFunction(_Best,self._parameters["QualityCriterion"])
         NumberOfFunctionEvaluations += 1
         #
         for i in range(self._parameters["NumberOfInsects"]):
             insect  = numpy.ravel(PosInsect[:,i])
             quality = CostFunction(insect,self._parameters["QualityCriterion"])
             NumberOfFunctionEvaluations += 1
             qBestPosInsect.append(quality)
-            if quality < qBest:
-                Best  = copy.copy( insect )
-                qBest = copy.copy( quality )
-        logging.debug("%s Initialisation, Insecte = %s, Qualité = %s"%(self._name, str(Best), str(qBest)))
+            if quality < _qualityBest:
+                _Best  = copy.copy( insect )
+                _qualityBest = copy.copy( quality )
+        logging.debug("%s Initialisation, Insecte = %s, Qualité = %s"%(self._name, str(_Best), str(_qualityBest)))
         #
         self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
         if self._parameters["StoreInternalVariables"] or self._toStore("CurrentState"):
-            self.StoredVariables["CurrentState"].store( Best )
+            self.StoredVariables["CurrentState"].store( _Best )
         self.StoredVariables["CostFunctionJb"].store( 0. )
         self.StoredVariables["CostFunctionJo"].store( 0. )
-        self.StoredVariables["CostFunctionJ" ].store( qBest )
+        self.StoredVariables["CostFunctionJ" ].store( _qualityBest )
         #
         # Minimisation de la fonctionnelle
         # --------------------------------
-        for n in range(self._parameters["MaximumNumberOfSteps"]):
+        for n in range(self._parameters["MaximumNumberOfIterations"]):
             for i in range(self._parameters["NumberOfInsects"]) :
                 insect  = numpy.ravel(PosInsect[:,i])
                 rp = numpy.random.uniform(size=nbparam)
                 rg = numpy.random.uniform(size=nbparam)
                 for j in range(nbparam) :
-                    VelocityInsect[j,i] = self._parameters["SwarmVelocity"]*VelocityInsect[j,i] +  Phip*rp[j]*(BestPosInsect[j,i]-PosInsect[j,i]) +  Phig*rg[j]*(Best[j]-PosInsect[j,i])
+                    VelocityInsect[j,i] = self._parameters["SwarmVelocity"]*VelocityInsect[j,i] +  Phip*rp[j]*(BestPosInsect[j,i]-PosInsect[j,i]) +  Phig*rg[j]*(_Best[j]-PosInsect[j,i])
                     PosInsect[j,i] = PosInsect[j,i]+VelocityInsect[j,i]
                 quality = CostFunction(insect,self._parameters["QualityCriterion"])
                 NumberOfFunctionEvaluations += 1
                 if quality < qBestPosInsect[i]:
                     BestPosInsect[:,i] = copy.copy( insect )
                     qBestPosInsect[i]  = copy.copy( quality )
-                    if quality < qBest :
-                        Best  = copy.copy( insect )
-                        qBest = copy.copy( quality )
-            logging.debug("%s Etape %i, Insecte = %s, Qualité = %s"%(self._name, n, str(Best), str(qBest)))
+                    if quality < _qualityBest :
+                        _Best  = copy.copy( insect )
+                        _qualityBest = copy.copy( quality )
+            logging.debug("%s Etape %i, Insecte = %s, Qualité = %s"%(self._name, n, str(_Best), str(_qualityBest)))
             #
             self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
             if self._parameters["StoreInternalVariables"] or self._toStore("CurrentState"):
-                self.StoredVariables["CurrentState"].store( Best )
+                self.StoredVariables["CurrentState"].store( _Best )
             if self._toStore("SimulatedObservationAtCurrentState"):
-                _HmX = Hm( numpy.asmatrix(numpy.ravel( Best )).T )
-                _HmX = numpy.asmatrix(numpy.ravel( _HmX )).T
+                _HmX = Hm( _Best )
                 self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HmX )
             self.StoredVariables["CostFunctionJb"].store( 0. )
             self.StoredVariables["CostFunctionJo"].store( 0. )
-            self.StoredVariables["CostFunctionJ" ].store( qBest )
+            self.StoredVariables["CostFunctionJ" ].store( _qualityBest )
             if NumberOfFunctionEvaluations > self._parameters["MaximumNumberOfFunctionEvaluations"]:
                 logging.debug("%s Stopping search because the number %i of function evaluations is exceeding the maximum %i."%(self._name, NumberOfFunctionEvaluations, self._parameters["MaximumNumberOfFunctionEvaluations"]))
                 break
         #
         # Obtention de l'analyse
         # ----------------------
-        Xa = numpy.asmatrix(numpy.ravel( Best )).T
+        Xa = _Best
         #
-        self.StoredVariables["Analysis"].store( Xa.A1 )
+        self.StoredVariables["Analysis"].store( Xa )
         #
+        # Calculs et/ou stockages supplémentaires
+        # ---------------------------------------
+        if self._toStore("OMA") or \
+            self._toStore("SimulatedObservationAtOptimum"):
+            HXa = Hm(Xa)
         if self._toStore("Innovation") or \
             self._toStore("OMB") or \
             self._toStore("SimulatedObservationAtBackground"):
             HXb = Hm(Xb)
-            d = Y - HXb
-        if self._toStore("OMA") or \
-            self._toStore("SimulatedObservationAtOptimum"):
-            HXa = Hm(Xa)
-        #
-        # Calculs et/ou stockages supplémentaires
-        # ---------------------------------------
+            Innovation = Y - HXb
         if self._toStore("Innovation"):
-            self.StoredVariables["Innovation"].store( d )
+            self.StoredVariables["Innovation"].store( Innovation )
+        if self._toStore("OMB"):
+            self.StoredVariables["OMB"].store( Innovation )
         if self._toStore("BMA"):
             self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
         if self._toStore("OMA"):
             self.StoredVariables["OMA"].store( numpy.ravel(Y) - numpy.ravel(HXa) )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( d )
         if self._toStore("SimulatedObservationAtBackground"):
             self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
         if self._toStore("SimulatedObservationAtOptimum"):
             self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
         #
         self._post_run(HO)
         return 0
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/QuantileRegression.py` & `adao-9.9.0.1/adao/daAlgorithms/QuantileRegression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,17 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
 import numpy
+from daCore import BasicObjects, NumericObjects
+from daAlgorithms.Atoms import mmqr
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "QUANTILEREGRESSION")
         self.defineRequiredParameter(
             name     = "Quantile",
@@ -40,19 +40,20 @@
             name     = "Minimizer",
             default  = "MMQR",
             typecast = str,
             message  = "Minimiseur utilisé",
             listval  = ["MMQR",],
             )
         self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
+            name     = "MaximumNumberOfIterations",
             default  = 15000,
             typecast = int,
             message  = "Nombre maximal de pas d'optimisation",
             minval   = 1,
+            oldname  = "MaximumNumberOfSteps",
             )
         self.defineRequiredParameter(
             name     = "CostDecrementTolerance",
             default  = 1.e-6,
             typecast = float,
             message  = "Maximum de variation de la fonction d'estimation lors de l'arrêt",
             )
@@ -103,99 +104,83 @@
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         self._parameters["Bounds"] = NumericObjects.ForceNumericBounds( self._parameters["Bounds"] )
         #
         Hm = HO["Direct"].appliedTo
         #
-        # Utilisation éventuelle d'un vecteur H(Xb) précalculé
-        # ----------------------------------------------------
-        if HO["AppliedInX"] is not None and "HXb" in HO["AppliedInX"]:
-            HXb = Hm( Xb, HO["AppliedInX"]["HXb"] )
-        else:
-            HXb = Hm( Xb )
-        HXb = numpy.asmatrix(numpy.ravel( HXb )).T
-        if Y.size != HXb.size:
-            raise ValueError("The size %i of observations Y and %i of observed calculation H(X) are different, they have to be identical."%(Y.size,HXb.size))
-        if max(Y.shape) != max(HXb.shape):
-            raise ValueError("The shapes %s of observations Y and %s of observed calculation H(X) are different, they have to be identical."%(Y.shape,HXb.shape))
-        d  = Y - HXb
-        #
-        # Définition de la fonction-coût
-        # ------------------------------
         def CostFunction(x):
-            _X  = numpy.asmatrix(numpy.ravel( x )).T
+            _X = numpy.asarray(x).reshape((-1,1))
             if self._parameters["StoreInternalVariables"] or \
                 self._toStore("CurrentState"):
                 self.StoredVariables["CurrentState"].store( _X )
-            _HX = Hm( _X )
-            _HX = numpy.asmatrix(numpy.ravel( _HX )).T
+            _HX = numpy.asarray(Hm( _X )).reshape((-1,1))
             if self._toStore("SimulatedObservationAtCurrentState"):
                 self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HX )
             Jb  = 0.
             Jo  = 0.
             J   = Jb + Jo
             #
             self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
             self.StoredVariables["CostFunctionJb"].store( Jb )
             self.StoredVariables["CostFunctionJo"].store( Jo )
             self.StoredVariables["CostFunctionJ" ].store( J )
             return _HX
         #
         def GradientOfCostFunction(x):
-            _X      = numpy.asmatrix(numpy.ravel( x )).T
+            _X = numpy.asarray(x).reshape((-1,1))
             Hg = HO["Tangent"].asMatrix( _X )
             return Hg
         #
-        # Point de démarrage de l'optimisation
-        # ------------------------------------
         Xini = self._parameters["InitializationPoint"]
         #
         # Minimisation de la fonctionnelle
         # --------------------------------
         if self._parameters["Minimizer"] == "MMQR":
-            Minimum, J_optimal, Informations = NumericObjects.mmqr(
+            Minimum, J_optimal, Informations = mmqr.mmqr(
                 func        = CostFunction,
                 x0          = Xini,
                 fprime      = GradientOfCostFunction,
                 bounds      = self._parameters["Bounds"],
                 quantile    = self._parameters["Quantile"],
-                maxfun      = self._parameters["MaximumNumberOfSteps"],
+                maxfun      = self._parameters["MaximumNumberOfIterations"],
                 toler       = self._parameters["CostDecrementTolerance"],
                 y           = Y,
                 )
-            nfeval = Informations[2]
-            rc     = Informations[4]
         else:
-            raise ValueError("Error in Minimizer name: %s"%self._parameters["Minimizer"])
+            raise ValueError("Error in minimizer name: %s is unkown"%self._parameters["Minimizer"])
         #
         # Obtention de l'analyse
         # ----------------------
-        Xa = numpy.asmatrix(numpy.ravel( Minimum )).T
+        Xa = Minimum
         #
-        self.StoredVariables["Analysis"].store( Xa.A1 )
-        #
-        if self._toStore("OMA") or \
-            self._toStore("SimulatedObservationAtOptimum"):
-            HXa = Hm( Xa )
+        self.StoredVariables["Analysis"].store( Xa )
         #
         # Calculs et/ou stockages supplémentaires
         # ---------------------------------------
+        if self._toStore("OMA") or \
+            self._toStore("SimulatedObservationAtOptimum"):
+            HXa = Hm(Xa).reshape((-1,1))
+        if self._toStore("Innovation") or \
+            self._toStore("OMB") or \
+            self._toStore("SimulatedObservationAtBackground"):
+            HXb = Hm(Xb).reshape((-1,1))
+            Innovation = Y - HXb
         if self._toStore("Innovation"):
-            self.StoredVariables["Innovation"].store( numpy.ravel(d) )
+            self.StoredVariables["Innovation"].store( Innovation )
+        if self._toStore("OMB"):
+            self.StoredVariables["OMB"].store( Innovation )
         if self._toStore("BMA"):
             self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
         if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( numpy.ravel(Y) - numpy.ravel(HXa) )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( numpy.ravel(d) )
+            self.StoredVariables["OMA"].store( Y - HXa )
         if self._toStore("SimulatedObservationAtBackground"):
-            self.StoredVariables["SimulatedObservationAtBackground"].store( numpy.ravel(HXb) )
+            self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
         if self._toStore("SimulatedObservationAtOptimum"):
-            self.StoredVariables["SimulatedObservationAtOptimum"].store( numpy.ravel(HXa) )
+            self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
         #
         self._post_run(HO)
         return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/SamplingTest.py` & `adao-9.9.0.1/adao/daAlgorithms/SamplingTest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,16 +16,15 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import copy, logging, itertools
-import numpy
+import numpy, logging, itertools
 from daCore import BasicObjects
 from daCore.PlatformInfo import PlatformInfo
 mfp = PlatformInfo().MaximumPrecision()
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
@@ -133,15 +132,14 @@
             for i,dim in enumerate(self._parameters["SampleAsIndependantRandomVariables"]):
                 if len(dim) != 3:
                     raise ValueError("For dimension %i, the variable definition \"%s\" is incorrect, it should be ('distribution',(parameters),length) with distribution in ['normal'(mean,std),'lognormal'(mean,sigma),'uniform'(low,high),'weibull'(shape)]."%(i,dim))
                 elif not( str(dim[0]) in ['normal','lognormal','uniform','weibull'] and hasattr(numpy.random,dim[0]) ):
                     raise ValueError("For dimension %i, the distribution name \"%s\" is not allowed, please choose in ['normal'(mean,std),'lognormal'(mean,sigma),'uniform'(low,high),'weibull'(shape)]"%(i,dim[0]))
                 else:
                     distribution = getattr(numpy.random,str(dim[0]),'normal')
-                    parameters   = dim[1]
                     coordinatesList.append(distribution(*dim[1], size=max(1,int(dim[2]))))
             sampleList = itertools.product(*coordinatesList)
         else:
             sampleList = iter([X0,])
         # ----------
         BI = B.getI()
         RI = R.getI()
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/TabuSearch.py` & `adao-9.9.0.1/adao/daAlgorithms/TabuSearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,28 +16,28 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects
 import numpy
+from daCore import BasicObjects
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "TABUSEARCH")
         self.defineRequiredParameter(
-            name     = "MaximumNumberOfSteps",
+            name     = "MaximumNumberOfIterations",
             default  = 50,
             typecast = int,
             message  = "Nombre maximal de pas d'optimisation",
             minval   = 1,
+            oldname  = "MaximumNumberOfSteps",
             )
         self.defineRequiredParameter(
             name     = "SetSeed",
             typecast = numpy.random.seed,
             message  = "Graine fixée pour le générateur aléatoire",
             )
         self.defineRequiredParameter(
@@ -62,30 +62,32 @@
             listval  = ["Gaussian","Uniform"],
             )
         self.defineRequiredParameter(
             name     = "QualityCriterion",
             default  = "AugmentedWeightedLeastSquares",
             typecast = str,
             message  = "Critère de qualité utilisé",
-            listval  = ["AugmentedWeightedLeastSquares","AWLS","DA",
-                        "WeightedLeastSquares","WLS",
-                        "LeastSquares","LS","L2",
-                        "AbsoluteValue","L1",
-                        "MaximumError","ME"],
+            listval  = [
+                "AugmentedWeightedLeastSquares", "AWLS", "DA",
+                "WeightedLeastSquares", "WLS",
+                "LeastSquares", "LS", "L2",
+                "AbsoluteValue", "L1",
+                "MaximumError", "ME",
+                ],
             )
         self.defineRequiredParameter(
             name     = "NoiseHalfRange",
             default  = [],
-            typecast = numpy.matrix,
+            typecast = numpy.ravel,
             message  = "Demi-amplitude des perturbations uniformes centrées d'état pour chaque composante de l'état",
             )
         self.defineRequiredParameter(
             name     = "StandardDeviation",
             default  = [],
-            typecast = numpy.matrix,
+            typecast = numpy.ravel,
             message  = "Ecart-type des perturbations gaussiennes d'état pour chaque composante de l'état",
             )
         self.defineRequiredParameter(
             name     = "NoiseAddingProbability",
             default  = 1.,
             typecast = float,
             message  = "Probabilité de perturbation d'une composante de l'état",
@@ -132,35 +134,29 @@
             "MetaHeuristic",
             ))
 
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         if self._parameters["NoiseDistribution"] == "Uniform":
-            nrange = numpy.ravel(self._parameters["NoiseHalfRange"]) # Vecteur
+            nrange = self._parameters["NoiseHalfRange"] # Vecteur
             if nrange.size != Xb.size:
                 raise ValueError("Noise generation by Uniform distribution requires range for all variable increments. The actual noise half range vector is:\n%s"%nrange)
         elif self._parameters["NoiseDistribution"] == "Gaussian":
             sigma = numpy.ravel(self._parameters["StandardDeviation"]) # Vecteur
             if sigma.size != Xb.size:
                 raise ValueError("Noise generation by Gaussian distribution requires standard deviation for all variable increments. The actual standard deviation vector is:\n%s"%sigma)
         #
-        # Opérateur d'observation
-        # -----------------------
         Hm = HO["Direct"].appliedTo
         #
-        # Précalcul des inversions de B et R
-        # ----------------------------------
         BI = B.getI()
         RI = R.getI()
         #
-        # Définition de la fonction de deplacement
-        # ----------------------------------------
         def Tweak( x, NoiseDistribution, NoiseAddingProbability ):
-            _X  = numpy.matrix(numpy.ravel( x )).T
+            _X  = numpy.array( x, dtype=float, copy=True ).ravel().reshape((-1,1))
             if NoiseDistribution == "Uniform":
                 for i in range(_X.size):
                     if NoiseAddingProbability >= numpy.random.uniform():
                         _increment = numpy.random.uniform(low=-nrange[i], high=nrange[i])
                         # On ne traite pas encore le dépassement des bornes ici
                         _X[i] += _increment
             elif NoiseDistribution == "Gaussian":
@@ -168,124 +164,115 @@
                     if NoiseAddingProbability >= numpy.random.uniform():
                         _increment = numpy.random.normal(loc=0., scale=sigma[i])
                         # On ne traite pas encore le dépassement des bornes ici
                         _X[i] += _increment
             #
             return _X
         #
-        def StateInList( x, TL ):
+        def StateInList( x, _TL ):
             _X  = numpy.ravel( x )
             _xInList = False
-            for state in TL:
+            for state in _TL:
                 if numpy.all(numpy.abs( _X - numpy.ravel(state) ) <= 1e-16*numpy.abs(_X)):
                     _xInList = True
             # if _xInList: import sys ; sys.exit()
             return _xInList
         #
+        def CostFunction(x, QualityMeasure="AugmentedWeightedLeastSquares"):
+            _X  = numpy.ravel( x ).reshape((-1,1))
+            _HX = numpy.ravel( Hm( _X ) ).reshape((-1,1))
+            _Innovation = Y - _HX
+            #
+            if QualityMeasure in ["AugmentedWeightedLeastSquares","AWLS","DA"]:
+                if BI is None or RI is None:
+                    raise ValueError("Background and Observation error covariance matrices has to be properly defined!")
+                Jb  = 0.5 * (_X - Xb).T @ (BI @ (_X - Xb))
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
+            elif QualityMeasure in ["WeightedLeastSquares","WLS"]:
+                if RI is None:
+                    raise ValueError("Observation error covariance matrix has to be properly defined!")
+                Jb  = 0.
+                Jo  = 0.5 * _Innovation.T @ (RI @ _Innovation)
+            elif QualityMeasure in ["LeastSquares","LS","L2"]:
+                Jb  = 0.
+                Jo  = 0.5 * _Innovation.T @ _Innovation
+            elif QualityMeasure in ["AbsoluteValue","L1"]:
+                Jb  = 0.
+                Jo  = numpy.sum( numpy.abs(_Innovation) )
+            elif QualityMeasure in ["MaximumError","ME"]:
+                Jb  = 0.
+                Jo  = numpy.max( numpy.abs(_Innovation) )
+            #
+            J   = float( Jb ) + float( Jo )
+            #
+            return J
+        #
         # Minimisation de la fonctionnelle
         # --------------------------------
         _n = 0
         _S = Xb
-        # _qualityS = CostFunction( _S, self._parameters["QualityCriterion"] )
-        _qualityS = BasicObjects.CostFunction3D(
-                   _S,
-            _Hm  = Hm,
-            _BI  = BI,
-            _RI  = RI,
-            _Xb  = Xb,
-            _Y   = Y,
-            _SSC = self._parameters["StoreSupplementaryCalculations"],
-            _QM  = self._parameters["QualityCriterion"],
-            _SSV = self.StoredVariables,
-            _sSc = False,
-            )
+        _qualityS = CostFunction( _S, self._parameters["QualityCriterion"] )
         _Best, _qualityBest   =   _S, _qualityS
         _TabuList = []
         _TabuList.append( _S )
-        while _n < self._parameters["MaximumNumberOfSteps"]:
+        while _n < self._parameters["MaximumNumberOfIterations"]:
             _n += 1
             if len(_TabuList) > self._parameters["LengthOfTabuList"]:
                 _TabuList.pop(0)
             _R = Tweak( _S, self._parameters["NoiseDistribution"], self._parameters["NoiseAddingProbability"] )
-            # _qualityR = CostFunction( _R, self._parameters["QualityCriterion"] )
-            _qualityR = BasicObjects.CostFunction3D(
-                       _R,
-                _Hm  = Hm,
-                _BI  = BI,
-                _RI  = RI,
-                _Xb  = Xb,
-                _Y   = Y,
-                _SSC = self._parameters["StoreSupplementaryCalculations"],
-                _QM  = self._parameters["QualityCriterion"],
-                _SSV = self.StoredVariables,
-                _sSc = False,
-                )
+            _qualityR = CostFunction( _R, self._parameters["QualityCriterion"] )
             for nbt in range(self._parameters["NumberOfElementaryPerturbations"]-1):
                 _W = Tweak( _S, self._parameters["NoiseDistribution"], self._parameters["NoiseAddingProbability"] )
-                # _qualityW = CostFunction( _W, self._parameters["QualityCriterion"] )
-                _qualityW = BasicObjects.CostFunction3D(
-                           _W,
-                    _Hm  = Hm,
-                    _BI  = BI,
-                    _RI  = RI,
-                    _Xb  = Xb,
-                    _Y   = Y,
-                    _SSC = self._parameters["StoreSupplementaryCalculations"],
-                    _QM  = self._parameters["QualityCriterion"],
-                    _SSV = self.StoredVariables,
-                    _sSc = False,
-                    )
+                _qualityW = CostFunction( _W, self._parameters["QualityCriterion"] )
                 if (not StateInList(_W, _TabuList)) and ( (_qualityW < _qualityR) or StateInList(_R,_TabuList) ):
                     _R, _qualityR   =   _W, _qualityW
             if (not StateInList( _R, _TabuList )) and (_qualityR < _qualityS):
                 _S, _qualityS   =   _R, _qualityR
                 _TabuList.append( _S )
             if _qualityS < _qualityBest:
                 _Best, _qualityBest   =   _S, _qualityS
             #
+            self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
             if self._parameters["StoreInternalVariables"] or self._toStore("CurrentState"):
                 self.StoredVariables["CurrentState"].store( _Best )
             if self._toStore("SimulatedObservationAtCurrentState"):
-                _HmX = Hm( numpy.asmatrix(numpy.ravel( _Best )).T )
-                _HmX = numpy.asmatrix(numpy.ravel( _HmX )).T
+                _HmX = Hm( _Best )
                 self.StoredVariables["SimulatedObservationAtCurrentState"].store( _HmX )
-            self.StoredVariables["CurrentIterationNumber"].store( len(self.StoredVariables["CostFunctionJ"]) )
             self.StoredVariables["CostFunctionJb"].store( 0. )
             self.StoredVariables["CostFunctionJo"].store( 0. )
             self.StoredVariables["CostFunctionJ" ].store( _qualityBest )
         #
         # Obtention de l'analyse
         # ----------------------
-        Xa = numpy.asmatrix(numpy.ravel( _Best )).T
+        Xa = _Best
         #
-        self.StoredVariables["Analysis"].store( Xa.A1 )
+        self.StoredVariables["Analysis"].store( Xa )
         #
+        # Calculs et/ou stockages supplémentaires
+        # ---------------------------------------
+        if self._toStore("OMA") or \
+            self._toStore("SimulatedObservationAtOptimum"):
+            HXa = Hm(Xa).reshape((-1,1))
         if self._toStore("Innovation") or \
             self._toStore("OMB") or \
             self._toStore("SimulatedObservationAtBackground"):
-            HXb = Hm(Xb)
-            d = Y - HXb
-        if self._toStore("OMA") or \
-           self._toStore("SimulatedObservationAtOptimum"):
-            HXa = Hm(Xa)
-        #
-        # Calculs et/ou stockages supplémentaires
-        # ---------------------------------------
+            HXb = Hm(Xb).reshape((-1,1))
+            Innovation = Y - HXb
         if self._toStore("Innovation"):
-            self.StoredVariables["Innovation"].store( numpy.ravel(d) )
+            self.StoredVariables["Innovation"].store( Innovation )
+        if self._toStore("OMB"):
+            self.StoredVariables["OMB"].store( Innovation )
         if self._toStore("BMA"):
             self.StoredVariables["BMA"].store( numpy.ravel(Xb) - numpy.ravel(Xa) )
         if self._toStore("OMA"):
-            self.StoredVariables["OMA"].store( numpy.ravel(Y) - numpy.ravel(HXa) )
-        if self._toStore("OMB"):
-            self.StoredVariables["OMB"].store( numpy.ravel(d) )
+            self.StoredVariables["OMA"].store( Y - HXa )
         if self._toStore("SimulatedObservationAtBackground"):
-            self.StoredVariables["SimulatedObservationAtBackground"].store( numpy.ravel(HXb) )
+            self.StoredVariables["SimulatedObservationAtBackground"].store( HXb )
         if self._toStore("SimulatedObservationAtOptimum"):
-            self.StoredVariables["SimulatedObservationAtOptimum"].store( numpy.ravel(HXa) )
+            self.StoredVariables["SimulatedObservationAtOptimum"].store( HXa )
         #
         self._post_run(HO)
         return 0
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/TangentTest.py` & `adao-9.9.0.1/adao/daAlgorithms/TangentTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,20 +16,17 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import sys, logging
-from daCore import BasicObjects, PlatformInfo
-import numpy, math
+import numpy
+from daCore import BasicObjects, NumericObjects, PlatformInfo
 mpr = PlatformInfo.PlatformInfo().MachinePrecision()
-if sys.version_info.major > 2:
-    unicode = str
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "TANGENTTEST")
         self.defineRequiredParameter(
             name     = "ResiduFormula",
@@ -104,45 +101,38 @@
         # Construction des perturbations
         # ------------------------------
         Perturbations = [ 10**i for i in range(self._parameters["EpsilonMinimumExponent"],1) ]
         Perturbations.reverse()
         #
         # Calcul du point courant
         # -----------------------
-        Xn      = numpy.asmatrix(numpy.ravel( Xb )).T
-        FX      = numpy.asmatrix(numpy.ravel( Hm( Xn ) )).T
+        Xn      = numpy.ravel( Xb ).reshape((-1,1))
+        FX      = numpy.ravel( Hm( Xn ) ).reshape((-1,1))
         NormeX  = numpy.linalg.norm( Xn )
         NormeFX = numpy.linalg.norm( FX )
         if self._toStore("CurrentState"):
-            self.StoredVariables["CurrentState"].store( numpy.ravel(Xn) )
+            self.StoredVariables["CurrentState"].store( Xn )
         if self._toStore("SimulatedObservationAtCurrentState"):
-            self.StoredVariables["SimulatedObservationAtCurrentState"].store( numpy.ravel(FX) )
+            self.StoredVariables["SimulatedObservationAtCurrentState"].store( FX )
         #
-        # Fabrication de la direction de l'increment dX
-        # ---------------------------------------------
-        if len(self._parameters["InitialDirection"]) == 0:
-            dX0 = []
-            for v in Xn.A1:
-                if abs(v) > 1.e-8:
-                    dX0.append( numpy.random.normal(0.,abs(v)) )
-                else:
-                    dX0.append( numpy.random.normal(0.,Xn.mean()) )
-        else:
-            dX0 = numpy.ravel( self._parameters["InitialDirection"] )
-        #
-        dX0 = float(self._parameters["AmplitudeOfInitialDirection"]) * numpy.matrix( dX0 ).T
+        dX0 = NumericObjects.SetInitialDirection(
+            self._parameters["InitialDirection"],
+            self._parameters["AmplitudeOfInitialDirection"],
+            Xn,
+            )
         #
         # Calcul du gradient au point courant X pour l'increment dX
         # qui est le tangent en X multiplie par dX
         # ---------------------------------------------------------
         dX1      = float(self._parameters["AmplitudeOfTangentPerturbation"]) * dX0
         GradFxdX = Ht( (Xn, dX1) )
-        GradFxdX = numpy.asmatrix(numpy.ravel( GradFxdX )).T
+        GradFxdX = numpy.ravel( GradFxdX ).reshape((-1,1))
         GradFxdX = float(1./self._parameters["AmplitudeOfTangentPerturbation"]) * GradFxdX
         NormeGX  = numpy.linalg.norm( GradFxdX )
+        if NormeGX < mpr: NormeGX = mpr
         #
         # Entete des resultats
         # --------------------
         __marge =  12*u" "
         __precision = u"""
             Remarque : les nombres inferieurs a %.0e (environ) representent un zero
                        a la precision machine.\n"""%mpr
@@ -166,15 +156,15 @@
             Si |R-1|/Alpha est tres faible, le code F est vraisemblablement
             lineaire ou quasi-lineaire, et le tangent est valide jusqu'a ce que
             l'on atteigne la precision du calcul.
 
             On prend dX0 = Normal(0,X) et dX = Alpha*dX0. F est le code de calcul.\n""" + __precision
         #
         if len(self._parameters["ResultTitle"]) > 0:
-            __rt = unicode(self._parameters["ResultTitle"])
+            __rt = str(self._parameters["ResultTitle"])
             msgs  = u"\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
             msgs += __marge + "    " + __rt + "\n"
             msgs += __marge + "====" + "="*len(__rt) + "====\n"
         else:
             msgs  = u""
         msgs += __msgdoc
@@ -183,18 +173,18 @@
         msgs += "\n" + __marge + "-"*__nbtirets
         msgs += "\n" + __marge + __entete
         msgs += "\n" + __marge + "-"*__nbtirets
         #
         # Boucle sur les perturbations
         # ----------------------------
         for i,amplitude in enumerate(Perturbations):
-            dX      = amplitude * dX0
+            dX      = amplitude * dX0.reshape((-1,1))
             #
             if self._parameters["ResiduFormula"] == "Taylor":
-                FX_plus_dX  = numpy.asmatrix(numpy.ravel( Hm( Xn + dX ) )).T
+                FX_plus_dX  = numpy.ravel( Hm( Xn + dX ) ).reshape((-1,1))
                 #
                 Residu = numpy.linalg.norm( FX_plus_dX - FX ) / (amplitude * NormeGX)
                 #
                 self.StoredVariables["Residu"].store( Residu )
                 msg = "  %2i  %5.0e   %9.3e   %9.3e   |   %11.5e    %5.1e"%(i,amplitude,NormeX,NormeFX,Residu,abs(Residu-1.)/amplitude)
                 msgs += "\n" + __marge + msg
         #
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/UnscentedKalmanFilter.py` & `adao-9.9.0.1/adao/daAlgorithms/UnscentedKalmanFilter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -16,16 +16,16 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import logging
-from daCore import BasicObjects, NumericObjects
+from daCore import BasicObjects
+from daAlgorithms.Atoms import c2ukf, uskf
 
 # ==============================================================================
 class ElementaryAlgorithm(BasicObjects.Algorithm):
     def __init__(self):
         BasicObjects.Algorithm.__init__(self, "UNSCENTEDKALMANFILTER")
         self.defineRequiredParameter(
             name     = "Variant",
@@ -34,28 +34,28 @@
             message  = "Variant ou formulation de la méthode",
             listval  = [
                 "UKF",
                 "2UKF",
                 ],
             )
         self.defineRequiredParameter(
-            name     = "ConstrainedBy",
-            default  = "EstimateProjection",
-            typecast = str,
-            message  = "Prise en compte des contraintes",
-            listval  = ["EstimateProjection"],
-            )
-        self.defineRequiredParameter(
             name     = "EstimationOf",
             default  = "State",
             typecast = str,
             message  = "Estimation d'etat ou de parametres",
             listval  = ["State", "Parameters"],
             )
         self.defineRequiredParameter(
+            name     = "ConstrainedBy",
+            default  = "EstimateProjection",
+            typecast = str,
+            message  = "Prise en compte des contraintes",
+            listval  = ["EstimateProjection"],
+            )
+        self.defineRequiredParameter(
             name     = "Alpha",
             default  = 1.,
             typecast = float,
             message  = "",
             minval   = 1.e-4,
             maxval   = 1.,
             )
@@ -100,15 +100,14 @@
                 "BMA",
                 "CostFunctionJ",
                 "CostFunctionJAtCurrentOptimum",
                 "CostFunctionJb",
                 "CostFunctionJbAtCurrentOptimum",
                 "CostFunctionJo",
                 "CostFunctionJoAtCurrentOptimum",
-                "CurrentIterationNumber",
                 "CurrentOptimum",
                 "CurrentState",
                 "ForecastCovariance",
                 "ForecastState",
                 "IndexOfOptimum",
                 "InnovationAtCurrentAnalysis",
                 "InnovationAtCurrentState",
@@ -136,20 +135,20 @@
     def run(self, Xb=None, Y=None, U=None, HO=None, EM=None, CM=None, R=None, B=None, Q=None, Parameters=None):
         self._pre_run(Parameters, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         # Default UKF
         #--------------------------
         if   self._parameters["Variant"] == "UKF":
-            NumericObjects.uskf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+            uskf.uskf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         # Default 2UKF
         elif self._parameters["Variant"] == "2UKF":
-            NumericObjects.c2ukf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
+            c2ukf.c2ukf(self, Xb, Y, U, HO, EM, CM, R, B, Q)
         #
         #--------------------------
         else:
             raise ValueError("Error in Variant name: %s"%self._parameters["Variant"])
         #
         self._post_run(HO)
         return 0
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/__init__.py` & `adao-9.9.0.1/adao/daAlgorithms/Atoms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
```

### Comparing `adao-9.8.0.2/adao/daAlgorithms/lbfgsbhlt.py` & `adao-9.9.0.1/adao/daAlgorithms/Atoms/lbfgsbhlt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Modification de la version 1.1.0
+# Modification de la version 1.4.1
 """
 Functions
 ---------
 .. autosummary::
    :toctree: generated/
 
     fmin_l_bfgs_b
@@ -35,15 +35,15 @@
 ## Modifications by Travis Oliphant and Enthought, Inc. for inclusion in SciPy
 
 from __future__ import division, print_function, absolute_import
 
 import numpy as np
 from numpy import array, asarray, float64, int32, zeros
 from scipy.optimize import _lbfgsb
-from scipy.optimize.optimize import (approx_fprime, MemoizeJac, OptimizeResult,
+from scipy.optimize.optimize import (MemoizeJac, OptimizeResult,
                        _check_unknown_options, wrap_function,
                        _approx_fprime_helper)
 from scipy.sparse.linalg import LinearOperator
 
 __all__ = ['fmin_l_bfgs_b', 'LbfgsInvHessProduct']
 
 
@@ -215,36 +215,46 @@
                      iprint=-1, callback=None, maxls=20, **unknown_options):
     """
     Minimize a scalar function of one or more variables using the L-BFGS-B
     algorithm.
 
     Options
     -------
-    disp : bool
-       Set to True to print convergence messages.
+    disp : None or int
+        If `disp is None` (the default), then the supplied version of `iprint`
+        is used. If `disp is not None`, then it overrides the supplied version
+        of `iprint` with the behaviour you outlined.
     maxcor : int
         The maximum number of variable metric corrections used to
         define the limited memory matrix. (The limited memory BFGS
         method does not store the full hessian but uses this many terms
         in an approximation to it.)
     ftol : float
         The iteration stops when ``(f^k -
         f^{k+1})/max{|f^k|,|f^{k+1}|,1} <= ftol``.
     gtol : float
         The iteration will stop when ``max{|proj g_i | i = 1, ..., n}
         <= gtol`` where ``pg_i`` is the i-th component of the
         projected gradient.
     eps : float
         Step size used for numerical approximation of the jacobian.
-    disp : int
-        Set to True to print convergence messages.
     maxfun : int
         Maximum number of function evaluations.
     maxiter : int
         Maximum number of iterations.
+    iprint : int, optional
+        Controls the frequency of output. ``iprint < 0`` means no output;
+        ``iprint = 0``    print only one line at the last iteration;
+        ``0 < iprint < 99`` print also f and ``|proj g|`` every iprint iterations;
+        ``iprint = 99``   print details of every iteration except n-vectors;
+        ``iprint = 100``  print also the changes of active set and final x;
+        ``iprint > 100``  print details of every iteration including x and g.
+    callback : callable, optional
+        Called after each iteration, as ``callback(xk)``, where ``xk`` is the
+        current parameter vector.
     maxls : int, optional
         Maximum number of line search steps (per iteration). Default is 20.
 
     Notes
     -----
     The option `ftol` is exposed via the `scipy.optimize.minimize` interface,
     but calling `scipy.optimize.fmin_l_bfgs_b` directly exposes `factr`. The
```

### Comparing `adao-9.8.0.2/adao/daCore/Aidsm.py` & `adao-9.9.0.1/adao/daCore/Aidsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -162,18 +162,18 @@
                 commande(
                     Matrix, OneFunction, ThreeFunctions,
                     Parameters, Script, Scheduler, ExtraArguments,
                     Stored, PerformanceProfile, InputFunctionAsMulti, Checked )
             else:
                 raise ValueError("the variable named '%s' is not allowed."%str(Concept))
         except Exception as e:
-            if isinstance(e, SyntaxError): msg = "at %s: %s"%(e.offset, e.text)
+            if isinstance(e, SyntaxError): msg = " at %s: %s"%(e.offset, e.text)
             else: msg = ""
             raise ValueError(("during settings, the following error occurs:\n"+\
-                              "\n%s %s\n\nSee also the potential messages, "+\
+                              "\n%s%s\n\nSee also the potential messages, "+\
                               "which can show the origin of the above error, "+\
                               "in the launching terminal.")%(str(e),msg))
 
     # -----------------------------------------------------------
 
     def setBackground(self,
             Vector         = None,
@@ -672,15 +672,15 @@
             allvariables.update( self.__StoredInputs )
             allvariables.pop('Observer', None)
             allvariables.pop('UserPostAnalysis', None)
             return allvariables
 
     # -----------------------------------------------------------
 
-    def get_available_variables(self):
+    def __get_available_variables(self):
         """
         Renvoie les variables potentiellement utilisables pour l'étude,
         initialement stockées comme données d'entrées ou dans les algorithmes,
         identifiés par les chaînes de caractères. L'algorithme doit avoir été
         préalablement choisi sinon la méthode renvoie "None".
         """
         if len(list(self.__adaoObject["AlgorithmParameters"].keys())) == 0 and \
@@ -696,15 +696,15 @@
             if len(list(self.__StoredInputs.keys())) > 0:
                 variables.extend( list(self.__StoredInputs.keys()) )
             variables.remove('Observer')
             variables.remove('UserPostAnalysis')
             variables.sort()
             return variables
 
-    def get_available_algorithms(self):
+    def __get_available_algorithms(self):
         """
         Renvoie la liste des algorithmes potentiellement utilisables, identifiés
         par les chaînes de caractères.
         """
         files = []
         for directory in sys.path:
             trypath = os.path.join(directory,"daAlgorithms")
@@ -716,21 +716,21 @@
                         with open(os.path.join(trypath,fname)) as fc:
                             iselal = bool("class ElementaryAlgorithm" in fc.read())
                             if iselal and ext == '.py' and root != '__init__':
                                 files.append(root)
         files.sort()
         return files
 
-    def get_algorithms_main_path(self):
+    def __get_algorithms_main_path(self):
         """
         Renvoie le chemin pour le répertoire principal contenant les algorithmes
         """
         return self.__parent
 
-    def add_algorithms_path(self, Path=None):
+    def __add_algorithms_path(self, Path=None):
         """
         Ajoute au chemin de recherche des algorithmes un répertoire dans lequel
         se trouve un sous-répertoire "daAlgorithms"
         """
         if not os.path.isdir(Path):
             raise ValueError("The given "+Path+" argument must exist as a directory")
         if not os.path.isdir(os.path.join(Path,"daAlgorithms")):
@@ -860,10 +860,11 @@
             del self.__adaoObject # Because it breaks pickle in Python 2. Not required for Python 3
             del self.__case       # Because it breaks pickle in Python 2. Not required for Python 3
         if sys.version_info.major < 3:
             return 0
         else:
             return self.__StoredInputs
 
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/AssimilationStudy.py` & `adao-9.9.0.1/adao/daCore/AssimilationStudy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -32,10 +32,11 @@
 class AssimilationStudy(_Aidsm):
     """
     Generic ADAO TUI builder
     """
     def __init__(self, name = ""):
         _Aidsm.__init__(self, name)
 
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/BasicObjects.py` & `adao-9.9.0.1/adao/daCore/BasicObjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -28,14 +28,15 @@
 
 import os
 import sys
 import logging
 import copy
 import time
 import numpy
+import warnings
 from functools import partial
 from daCore import Persistence, PlatformInfo, Interfaces
 from daCore import Templates
 
 # ==============================================================================
 class CacheManager(object):
     """
@@ -242,15 +243,19 @@
             #
             if len(_xserie)>0 and self.__Matrix is None:
                 if self.__extraArgs is None:
                     _hserie = self.__Method( _xserie ) # Calcul MF
                 else:
                     _hserie = self.__Method( _xserie, self.__extraArgs ) # Calcul MF
                 if not hasattr(_hserie, "pop"):
-                    raise TypeError("The user input multi-function doesn't seem to return sequence results, behaving like a mono-function. It has to be checked.")
+                    raise TypeError(
+                        "The user input multi-function doesn't seem to return a"+\
+                        " result sequence, behaving like a mono-function. It has"+\
+                        " to be checked."
+                        )
                 for i in _hindex:
                     _xv = _xserie.pop(0)
                     _hv = _hserie.pop(0)
                     _HxValue[i] = _hv
                     if self.__avoidRC:
                         Operator.CM.storeValueInX(_xv,_hv,self.__name)
         #
@@ -491,27 +496,24 @@
                    (("useApproximatedDerivatives" not in asThreeFunctions) or not bool(asThreeFunctions["useApproximatedDerivatives"])):
                     __Function = asThreeFunctions
                 elif isinstance(asThreeFunctions, dict) and \
                    ("Direct" in asThreeFunctions) and (asThreeFunctions["Direct"] is not None):
                     __Function = asThreeFunctions
                     __Function.update({"useApproximatedDerivatives":True})
                 else:
-                    raise ValueError("The functions has to be given in a dictionnary which have either 1 key (\"Direct\") or 3 keys (\"Direct\" (optionnal), \"Tangent\" and \"Adjoint\")")
+                    raise ValueError(
+                        "The functions has to be given in a dictionnary which have either"+\
+                        " 1 key (\"Direct\") or"+\
+                        " 3 keys (\"Direct\" (optionnal), \"Tangent\" and \"Adjoint\")")
                 if "Direct"  not in asThreeFunctions:
                     __Function["Direct"] = asThreeFunctions["Tangent"]
                 __Function.update(__Parameters)
             else:
                 __Function = None
         #
-        # if sys.version_info[0] < 3 and isinstance(__Function, dict):
-        #     for k in ("Direct", "Tangent", "Adjoint"):
-        #         if k in __Function and hasattr(__Function[k],"__class__"):
-        #             if type(__Function[k]) is type(self.__init__):
-        #                 raise TypeError("can't use a class method (%s) as a function for the \"%s\" operator. Use a real function instead."%(type(__Function[k]),k))
-        #
         if   appliedInX is not None and isinstance(appliedInX, dict):
             __appliedInX = appliedInX
         elif appliedInX is not None:
             __appliedInX = {"HXb":appliedInX}
         else:
             __appliedInX = None
         #
@@ -542,45 +544,98 @@
                 avoidingRedundancy    = __Function["withAvoidingRedundancy"],
                 toleranceInRedundancy = __Function["withToleranceInRedundancy"],
                 lenghtOfRedundancy    = __Function["withLenghtOfRedundancy"],
                 mpEnabled             = __Function["EnableMultiProcessingInDerivatives"],
                 mpWorkers             = __Function["NumberOfProcesses"],
                 mfEnabled             = __Function["withmfEnabled"],
                 )
-            self.__FO["Direct"]  = Operator( name = self.__name,           fromMethod = FDA.DirectOperator,  reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, extraArguments = self.__extraArgs, enableMultiProcess = __Parameters["EnableMultiProcessingInEvaluation"] )
-            self.__FO["Tangent"] = Operator( name = self.__name+"Tangent", fromMethod = FDA.TangentOperator, reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, extraArguments = self.__extraArgs )
-            self.__FO["Adjoint"] = Operator( name = self.__name+"Adjoint", fromMethod = FDA.AdjointOperator, reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, extraArguments = self.__extraArgs )
+            self.__FO["Direct"]  = Operator(
+                name = self.__name,
+                fromMethod = FDA.DirectOperator,
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                extraArguments = self.__extraArgs,
+                enableMultiProcess = __Parameters["EnableMultiProcessingInEvaluation"] )
+            self.__FO["Tangent"] = Operator(
+                name = self.__name+"Tangent",
+                fromMethod = FDA.TangentOperator,
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                extraArguments = self.__extraArgs )
+            self.__FO["Adjoint"] = Operator(
+                name = self.__name+"Adjoint",
+                fromMethod = FDA.AdjointOperator,
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                extraArguments = self.__extraArgs )
         elif isinstance(__Function, dict) and \
                 ("Direct" in __Function) and ("Tangent" in __Function) and ("Adjoint" in __Function) and \
                 (__Function["Direct"] is not None) and (__Function["Tangent"] is not None) and (__Function["Adjoint"] is not None):
-            self.__FO["Direct"]  = Operator( name = self.__name,           fromMethod = __Function["Direct"],  reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, extraArguments = self.__extraArgs, enableMultiProcess = __Parameters["EnableMultiProcessingInEvaluation"] )
-            self.__FO["Tangent"] = Operator( name = self.__name+"Tangent", fromMethod = __Function["Tangent"], reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, extraArguments = self.__extraArgs )
-            self.__FO["Adjoint"] = Operator( name = self.__name+"Adjoint", fromMethod = __Function["Adjoint"], reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, extraArguments = self.__extraArgs )
+            self.__FO["Direct"]  = Operator(
+                name = self.__name,
+                fromMethod = __Function["Direct"],
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                extraArguments = self.__extraArgs,
+                enableMultiProcess = __Parameters["EnableMultiProcessingInEvaluation"] )
+            self.__FO["Tangent"] = Operator(
+                name = self.__name+"Tangent",
+                fromMethod = __Function["Tangent"],
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                extraArguments = self.__extraArgs )
+            self.__FO["Adjoint"] = Operator(
+                name = self.__name+"Adjoint",
+                fromMethod = __Function["Adjoint"],
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                extraArguments = self.__extraArgs )
         elif asMatrix is not None:
             if isinstance(__Matrix, str):
                 __Matrix = PlatformInfo.strmatrix2liststr( __Matrix )
             __matrice = numpy.asarray( __Matrix, dtype=float )
-            self.__FO["Direct"]  = Operator( name = self.__name,           fromMatrix = __matrice,   reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF, enableMultiProcess = __Parameters["EnableMultiProcessingInEvaluation"] )
-            self.__FO["Tangent"] = Operator( name = self.__name+"Tangent", fromMatrix = __matrice,   reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF )
-            self.__FO["Adjoint"] = Operator( name = self.__name+"Adjoint", fromMatrix = __matrice.T, reducingMemoryUse = __reduceM, avoidingRedundancy = __avoidRC, inputAsMultiFunction = inputAsMF )
+            self.__FO["Direct"]  = Operator(
+                name = self.__name,
+                fromMatrix = __matrice,
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF,
+                enableMultiProcess = __Parameters["EnableMultiProcessingInEvaluation"] )
+            self.__FO["Tangent"] = Operator(
+                name = self.__name+"Tangent",
+                fromMatrix = __matrice,
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF )
+            self.__FO["Adjoint"] = Operator(
+                name = self.__name+"Adjoint",
+                fromMatrix = __matrice.T,
+                reducingMemoryUse = __reduceM,
+                avoidingRedundancy = __avoidRC,
+                inputAsMultiFunction = inputAsMF )
             del __matrice
         else:
-            raise ValueError("The %s object is improperly defined or undefined, it requires at minima either a matrix, a Direct operator for approximate derivatives or a Tangent/Adjoint operators pair. Please check your operator input."%self.__name)
+            raise ValueError(
+                "The %s object is improperly defined or undefined,"%self.__name+\
+                " it requires at minima either a matrix, a Direct operator for"+\
+                " approximate derivatives or a Tangent/Adjoint operators pair."+\
+                " Please check your operator input.")
         #
         if __appliedInX is not None:
             self.__FO["AppliedInX"] = {}
-            for key in list(__appliedInX.keys()):
-                if type( __appliedInX[key] ) is type( numpy.matrix([]) ):
-                    # Pour le cas où l'on a une vraie matrice
-                    self.__FO["AppliedInX"][key] = numpy.matrix( __appliedInX[key].A1, numpy.float ).T
-                elif type( __appliedInX[key] ) is type( numpy.array([]) ) and len(__appliedInX[key].shape) > 1:
-                    # Pour le cas où l'on a un vecteur représenté en array avec 2 dimensions
-                    self.__FO["AppliedInX"][key] = numpy.matrix( __appliedInX[key].reshape(len(__appliedInX[key]),), numpy.float ).T
-                else:
-                    self.__FO["AppliedInX"][key] = numpy.matrix( __appliedInX[key],    numpy.float ).T
+            for key in __appliedInX:
+                if isinstance(__appliedInX[key], str):
+                    __appliedInX[key] = PlatformInfo.strvect2liststr( __appliedInX[key] )
+                self.__FO["AppliedInX"][key] = numpy.ravel( __appliedInX[key] ).reshape((-1,1))
         else:
             self.__FO["AppliedInX"] = None
 
     def getO(self):
         return self.__FO
 
     def __repr__(self):
@@ -621,14 +676,15 @@
             - CostFunctionJb : partie ébauche ou background de la fonction-coût : Jb
             - CostFunctionJbAtCurrentOptimum : partie ébauche à l'état optimal courant lors d'itérations
             - CostFunctionJo : partie observations de la fonction-coût : Jo
             - CostFunctionJoAtCurrentOptimum : partie observations à l'état optimal courant lors d'itérations
             - CurrentIterationNumber : numéro courant d'itération dans les algorithmes itératifs, à partir de 0
             - CurrentOptimum : état optimal courant lors d'itérations
             - CurrentState : état courant lors d'itérations
+            - CurrentStepNumber : pas courant d'avancement dans les algorithmes en évolution, à partir de 0
             - GradientOfCostFunctionJ  : gradient de la fonction-coût globale
             - GradientOfCostFunctionJb : gradient de la partie ébauche de la fonction-coût
             - GradientOfCostFunctionJo : gradient de la partie observations de la fonction-coût
             - IndexOfOptimum : index de l'état optimal courant lors d'itérations
             - Innovation : l'innovation : d = Y - H(X)
             - InnovationAtCurrentState : l'innovation à l'état courant : dn = Y - H(Xn)
             - JacobianMatrixAtBackground : matrice jacobienne à l'état d'ébauche
@@ -662,14 +718,15 @@
         self.__required_inputs = {
             "RequiredInputValues":{"mandatory":(), "optional":()},
             "ClassificationTags":[],
             }
         self.__variable_names_not_public = {"nextStep":False} # Duplication dans AlgorithmAndParameters
         self.__canonical_parameter_name = {} # Correspondance "lower"->"correct"
         self.__canonical_stored_name = {}    # Correspondance "lower"->"correct"
+        self.__replace_by_the_new_name = {}  # Nouveau nom à partir d'un nom ancien
         #
         self.StoredVariables = {}
         self.StoredVariables["APosterioriCorrelations"]              = Persistence.OneMatrix(name = "APosterioriCorrelations")
         self.StoredVariables["APosterioriCovariance"]                = Persistence.OneMatrix(name = "APosterioriCovariance")
         self.StoredVariables["APosterioriStandardDeviations"]        = Persistence.OneVector(name = "APosterioriStandardDeviations")
         self.StoredVariables["APosterioriVariances"]                 = Persistence.OneVector(name = "APosterioriVariances")
         self.StoredVariables["Analysis"]                             = Persistence.OneVector(name = "Analysis")
@@ -680,14 +737,15 @@
         self.StoredVariables["CostFunctionJbAtCurrentOptimum"]       = Persistence.OneScalar(name = "CostFunctionJbAtCurrentOptimum")
         self.StoredVariables["CostFunctionJo"]                       = Persistence.OneScalar(name = "CostFunctionJo")
         self.StoredVariables["CostFunctionJoAtCurrentOptimum"]       = Persistence.OneScalar(name = "CostFunctionJoAtCurrentOptimum")
         self.StoredVariables["CurrentEnsembleState"]                 = Persistence.OneMatrix(name = "CurrentEnsembleState")
         self.StoredVariables["CurrentIterationNumber"]               = Persistence.OneIndex(name  = "CurrentIterationNumber")
         self.StoredVariables["CurrentOptimum"]                       = Persistence.OneVector(name = "CurrentOptimum")
         self.StoredVariables["CurrentState"]                         = Persistence.OneVector(name = "CurrentState")
+        self.StoredVariables["CurrentStepNumber"]                    = Persistence.OneIndex(name  = "CurrentStepNumber")
         self.StoredVariables["ForecastCovariance"]                   = Persistence.OneMatrix(name = "ForecastCovariance")
         self.StoredVariables["ForecastState"]                        = Persistence.OneVector(name = "ForecastState")
         self.StoredVariables["GradientOfCostFunctionJ"]              = Persistence.OneVector(name = "GradientOfCostFunctionJ")
         self.StoredVariables["GradientOfCostFunctionJb"]             = Persistence.OneVector(name = "GradientOfCostFunctionJb")
         self.StoredVariables["GradientOfCostFunctionJo"]             = Persistence.OneVector(name = "GradientOfCostFunctionJo")
         self.StoredVariables["IndexOfOptimum"]                       = Persistence.OneIndex(name  = "IndexOfOptimum")
         self.StoredVariables["Innovation"]                           = Persistence.OneVector(name = "Innovation")
@@ -726,15 +784,15 @@
         self._getTimeState(reset=True)
         #
         # Mise a jour des paramètres internes avec le contenu de Parameters, en
         # reprenant les valeurs par défauts pour toutes celles non définies
         self.__setParameters(Parameters, reset=True)
         for k, v in self.__variable_names_not_public.items():
             if k not in self._parameters:  self.__setParameters( {k:v} )
-        #
+
         # Corrections et compléments des vecteurs
         def __test_vvalue(argument, variable, argname, symbol=None):
             if symbol is None: symbol = variable
             if argument is None:
                 if variable in self.__required_inputs["RequiredInputValues"]["mandatory"]:
                     raise ValueError("%s %s vector %s is not set and has to be properly defined!"%(self._name,argname,symbol))
                 elif variable in self.__required_inputs["RequiredInputValues"]["optional"]:
@@ -743,20 +801,22 @@
                     logging.debug("%s %s vector %s is not set, but is not required."%(self._name,argname,symbol))
             else:
                 if variable in self.__required_inputs["RequiredInputValues"]["mandatory"]:
                     logging.debug("%s %s vector %s is required and set, and its size is %i."%(self._name,argname,symbol,numpy.array(argument).size))
                 elif variable in self.__required_inputs["RequiredInputValues"]["optional"]:
                     logging.debug("%s %s vector %s is optional and set, and its size is %i."%(self._name,argname,symbol,numpy.array(argument).size))
                 else:
-                    logging.debug("%s %s vector %s is set although neither required nor optional, and its size is %i."%(self._name,argname,symbol,numpy.array(argument).size))
+                    logging.debug(
+                        "%s %s vector %s is set although neither required nor optional, and its size is %i."%(
+                        self._name,argname,symbol,numpy.array(argument).size))
             return 0
         __test_vvalue( Xb, "Xb", "Background or initial state" )
         __test_vvalue( Y,  "Y",  "Observation" )
         __test_vvalue( U,  "U",  "Control" )
-        #
+
         # Corrections et compléments des covariances
         def __test_cvalue(argument, variable, argname, symbol=None):
             if symbol is None: symbol = variable
             if argument is None:
                 if variable in self.__required_inputs["RequiredInputValues"]["mandatory"]:
                     raise ValueError("%s %s error covariance matrix %s is not set and has to be properly defined!"%(self._name,argname,symbol))
                 elif variable in self.__required_inputs["RequiredInputValues"]["optional"]:
@@ -770,15 +830,15 @@
                     logging.debug("%s %s error covariance matrix %s is optional and set."%(self._name,argname,symbol))
                 else:
                     logging.debug("%s %s error covariance matrix %s is set although neither required nor optional."%(self._name,argname,symbol))
             return 0
         __test_cvalue( B, "B", "Background" )
         __test_cvalue( R, "R", "Observation" )
         __test_cvalue( Q, "Q", "Evolution" )
-        #
+
         # Corrections et compléments des opérateurs
         def __test_ovalue(argument, variable, argname, symbol=None):
             if symbol is None: symbol = variable
             if argument is None or (isinstance(argument,dict) and len(argument)==0):
                 if variable in self.__required_inputs["RequiredInputValues"]["mandatory"]:
                     raise ValueError("%s %s operator %s is not set and has to be properly defined!"%(self._name,argname,symbol))
                 elif variable in self.__required_inputs["RequiredInputValues"]["optional"]:
@@ -798,15 +858,17 @@
         __test_ovalue( CM, "CM", "Control Model", "C" )
         #
         # Corrections et compléments des bornes
         if ("Bounds" in self._parameters) and isinstance(self._parameters["Bounds"], (list, tuple)) and (len(self._parameters["Bounds"]) > 0):
             logging.debug("%s Bounds taken into account"%(self._name,))
         else:
             self._parameters["Bounds"] = None
-        if ("StateBoundsForQuantiles" in self._parameters) and isinstance(self._parameters["StateBoundsForQuantiles"], (list, tuple)) and (len(self._parameters["StateBoundsForQuantiles"]) > 0):
+        if ("StateBoundsForQuantiles" in self._parameters) \
+            and isinstance(self._parameters["StateBoundsForQuantiles"], (list, tuple)) \
+            and (len(self._parameters["StateBoundsForQuantiles"]) > 0):
             logging.debug("%s Bounds for quantiles states taken into account"%(self._name,))
             # Attention : contrairement à Bounds, pas de défaut à None, sinon on ne peut pas être sans bornes
         #
         # Corrections et compléments de l'initialisation en X
         if  "InitializationPoint" in self._parameters:
             if Xb is not None:
                 if self._parameters["InitializationPoint"] is not None and hasattr(self._parameters["InitializationPoint"],'size'):
@@ -823,26 +885,18 @@
         # Correction pour pallier a un bug de TNC sur le retour du Minimum
         if "Minimizer" in self._parameters and self._parameters["Minimizer"] == "TNC":
             self.setParameterValue("StoreInternalVariables",True)
         #
         # Verbosité et logging
         if logging.getLogger().level < logging.WARNING:
             self._parameters["optiprint"], self._parameters["optdisp"] = 1, 1
-            if PlatformInfo.has_scipy:
-                import scipy.optimize
-                self._parameters["optmessages"] = scipy.optimize.tnc.MSG_ALL
-            else:
-                self._parameters["optmessages"] = 15
+            self._parameters["optmessages"] = 15
         else:
             self._parameters["optiprint"], self._parameters["optdisp"] = -1, 0
-            if PlatformInfo.has_scipy:
-                import scipy.optimize
-                self._parameters["optmessages"] = scipy.optimize.tnc.MSG_NONE
-            else:
-                self._parameters["optmessages"] = 15
+            self._parameters["optmessages"] = 0
         #
         return 0
 
     def _post_run(self,_oH=None):
         "Post-calcul"
         if ("StoreSupplementaryCalculations" in self._parameters) and \
             "APosterioriCovariance" in self._parameters["StoreSupplementaryCalculations"]:
@@ -852,16 +906,20 @@
                 if "APosterioriStandardDeviations" in self._parameters["StoreSupplementaryCalculations"]:
                     self.StoredVariables["APosterioriStandardDeviations"].store( numpy.sqrt(numpy.diag(_A)) )
                 if "APosterioriCorrelations" in self._parameters["StoreSupplementaryCalculations"]:
                     _EI = numpy.diag(1./numpy.sqrt(numpy.diag(_A)))
                     _C = numpy.dot(_EI, numpy.dot(_A, _EI))
                     self.StoredVariables["APosterioriCorrelations"].store( _C )
         if _oH is not None and "Direct" in _oH and "Tangent" in _oH and "Adjoint" in _oH:
-            logging.debug("%s Nombre d'évaluation(s) de l'opérateur d'observation direct/tangent/adjoint.: %i/%i/%i", self._name, _oH["Direct"].nbcalls(0),_oH["Tangent"].nbcalls(0),_oH["Adjoint"].nbcalls(0))
-            logging.debug("%s Nombre d'appels au cache d'opérateur d'observation direct/tangent/adjoint..: %i/%i/%i", self._name, _oH["Direct"].nbcalls(3),_oH["Tangent"].nbcalls(3),_oH["Adjoint"].nbcalls(3))
+            logging.debug(
+                "%s Nombre d'évaluation(s) de l'opérateur d'observation direct/tangent/adjoint.: %i/%i/%i",
+                self._name, _oH["Direct"].nbcalls(0),_oH["Tangent"].nbcalls(0),_oH["Adjoint"].nbcalls(0))
+            logging.debug(
+                "%s Nombre d'appels au cache d'opérateur d'observation direct/tangent/adjoint..: %i/%i/%i",
+                self._name, _oH["Direct"].nbcalls(3),_oH["Tangent"].nbcalls(3),_oH["Adjoint"].nbcalls(3))
         logging.debug("%s Taille mémoire utilisée de %.0f Mio", self._name, self._m.getUsedMemory("Mio"))
         logging.debug("%s Durées d'utilisation CPU de %.1fs et elapsed de %.1fs", self._name, self._getTimeState()[0], self._getTimeState()[1])
         logging.debug("%s Terminé", self._name)
         return 0
 
     def _toStore(self, key):
         "True if in StoreSupplementaryCalculations, else False"
@@ -897,30 +955,40 @@
     def pop(self, k, d):
         "D.pop(k[,d]) -> v, remove specified key and return the corresponding value"
         if hasattr(self, "StoredVariables") and k.lower() in self.__canonical_stored_name:
             return self.StoredVariables.pop(self.__canonical_stored_name[k.lower()], d)
         else:
             try:
                 msg = "'%s'"%k
-            except:
+            except Exception:
                 raise TypeError("pop expected at least 1 arguments, got 0")
             "If key is not found, d is returned if given, otherwise KeyError is raised"
             try:
                 return d
-            except:
+            except Exception:
                 raise KeyError(msg)
 
     def run(self, Xb=None, Y=None, H=None, M=None, R=None, B=None, Q=None, Parameters=None):
         """
         Doit implémenter l'opération élémentaire de calcul d'assimilation sous
         sa forme mathématique la plus naturelle possible.
         """
         raise NotImplementedError("Mathematical assimilation calculation has not been implemented!")
 
-    def defineRequiredParameter(self, name = None, default = None, typecast = None, message = None, minval = None, maxval = None, listval = None, listadv = None):
+    def defineRequiredParameter(self,
+        name     = None,
+        default  = None,
+        typecast = None,
+        message  = None,
+        minval   = None,
+        maxval   = None,
+        listval  = None,
+        listadv  = None,
+        oldname  = None,
+        ):
         """
         Permet de définir dans l'algorithme des paramètres requis et leurs
         caractéristiques par défaut.
         """
         if name is None:
             raise ValueError("A name is mandatory to define a required parameter.")
         #
@@ -928,16 +996,20 @@
             "default"  : default,
             "typecast" : typecast,
             "minval"   : minval,
             "maxval"   : maxval,
             "listval"  : listval,
             "listadv"  : listadv,
             "message"  : message,
+            "oldname"  : oldname,
             }
         self.__canonical_parameter_name[name.lower()] = name
+        if oldname is not None:
+            self.__canonical_parameter_name[oldname.lower()] = name # Conversion
+            self.__replace_by_the_new_name[oldname.lower()] = name
         logging.debug("%s %s (valeur par défaut = %s)", self._name, message, self.setParameterValue(name))
 
     def getRequiredParameters(self, noDetails=True):
         """
         Renvoie la liste des noms de paramètres requis ou directement le
         dictionnaire des paramètres requis.
         """
@@ -964,15 +1036,15 @@
             if typecast is None: __val = default
             else:                __val = typecast( default )
         else:
             if typecast is None: __val = value
             else:
                 try:
                     __val = typecast( value )
-                except:
+                except Exception:
                     raise ValueError("The value '%s' for the parameter named '%s' can not be correctly evaluated with type '%s'."%(value, __k, typecast))
         #
         if minval is not None and (numpy.array(__val, float) < minval).any():
             raise ValueError("The parameter named '%s' of value '%s' can not be less than %s."%(__k, __val, minval))
         if maxval is not None and (numpy.array(__val, float) > maxval).any():
             raise ValueError("The parameter named '%s' of value '%s' can not be greater than %s."%(__k, __val, maxval))
         if listval is not None or listadv is not None:
@@ -1015,14 +1087,22 @@
         self._parameters.update( fromDico )
         __inverse_fromDico_keys = {}
         for k in fromDico.keys():
             if k.lower() in self.__canonical_parameter_name:
                 __inverse_fromDico_keys[self.__canonical_parameter_name[k.lower()]] = k
         #~ __inverse_fromDico_keys = dict([(self.__canonical_parameter_name[k.lower()],k) for k in fromDico.keys()])
         __canonic_fromDico_keys = __inverse_fromDico_keys.keys()
+        #
+        for k in __inverse_fromDico_keys.values():
+            if k.lower() in self.__replace_by_the_new_name:
+                __newk = self.__replace_by_the_new_name[k.lower()]
+                __msg  = "the parameter \"%s\" used in \"%s\" algorithm case is deprecated and has to be replaced by \"%s\"."%(k,self._name,__newk)
+                __msg += " Please update your code."
+                warnings.warn(__msg, FutureWarning, stacklevel=50)
+        #
         for k in self.__required_parameters.keys():
             if k in __canonic_fromDico_keys:
                 self._parameters[k] = self.setParameterValue(k,fromDico[__inverse_fromDico_keys[k]])
             elif reset:
                 self._parameters[k] = self.setParameterValue(k)
             else:
                 pass
@@ -1090,14 +1170,15 @@
         #
         self.StoredVariables = {}
         self.StoredVariables["Analysis"]                             = Persistence.OneVector(name = "Analysis")
         self.StoredVariables["CostFunctionJ"]                        = Persistence.OneScalar(name = "CostFunctionJ")
         self.StoredVariables["CostFunctionJb"]                       = Persistence.OneScalar(name = "CostFunctionJb")
         self.StoredVariables["CostFunctionJo"]                       = Persistence.OneScalar(name = "CostFunctionJo")
         self.StoredVariables["CurrentIterationNumber"]               = Persistence.OneIndex(name  = "CurrentIterationNumber")
+        self.StoredVariables["CurrentStepNumber"]                    = Persistence.OneIndex(name  = "CurrentStepNumber")
         #
         self.__canonical_stored_name = {}
         for k in self.StoredVariables:
             self.__canonical_stored_name[k.lower()] = k
 
     def _toStore(self, key):
         "True if in StoreSupplementaryCalculations, else False"
@@ -1225,15 +1306,15 @@
 
         r = pilot.getRuntime()
         xmlLoader = loader.YACSLoader()
         xmlLoader.registerProcCataLoader()
         try:
             catalogAd = r.loadCatalog("proc", __file)
             r.addCatalog(catalogAd)
-        except:
+        except Exception:
             pass
 
         try:
             p = xmlLoader.load(__file)
         except IOError as ex:
             print("The YACS XML schema file can not be loaded: %s"%(ex,))
 
@@ -1355,27 +1436,29 @@
         # Recherche explicitement le fichier complet
         # ------------------------------------------
         module_path = None
         for directory in sys.path:
             if os.path.isfile(os.path.join(directory, daDirectory, str(choice)+'.py')):
                 module_path = os.path.abspath(os.path.join(directory, daDirectory))
         if module_path is None:
-            raise ImportError("No algorithm module named \"%s\" has been found in the search path.\n             The search path is %s"%(choice, sys.path))
+            raise ImportError(
+                "No algorithm module named \"%s\" has been found in the search path.\n             The search path is %s"%(choice, sys.path))
         #
         # Importe le fichier complet comme un module
         # ------------------------------------------
         try:
             sys_path_tmp = sys.path ; sys.path.insert(0,module_path)
             self.__algorithmFile = __import__(str(choice), globals(), locals(), [])
             if not hasattr(self.__algorithmFile, "ElementaryAlgorithm"):
                 raise ImportError("this module does not define a valid elementary algorithm.")
             self.__algorithmName = str(choice)
             sys.path = sys_path_tmp ; del sys_path_tmp
         except ImportError as e:
-            raise ImportError("The module named \"%s\" was found, but is incorrect at the import stage.\n             The import error message is: %s"%(choice,e))
+            raise ImportError(
+                "The module named \"%s\" was found, but is incorrect at the import stage.\n             The import error message is: %s"%(choice,e))
         #
         # Instancie un objet du type élémentaire du fichier
         # -------------------------------------------------
         self.__algorithm = self.__algorithmFile.ElementaryAlgorithm()
         return 0
 
     def __shape_validate(self):
@@ -1456,40 +1539,56 @@
             raise ValueError("Shape characteristic of observation errors covariance matrix (R) is incorrect: \"%s\"."%(__R_shape,))
         if not( min(__Q_shape) == max(__Q_shape) ):
             raise ValueError("Shape characteristic of evolution errors covariance matrix (Q) is incorrect: \"%s\"."%(__Q_shape,))
         if not( min(__EM_shape) == max(__EM_shape) ):
             raise ValueError("Shape characteristic of evolution operator (EM) is incorrect: \"%s\"."%(__EM_shape,))
         #
         if len(self.__HO) > 0 and not isinstance(self.__HO, dict) and not( __HO_shape[1] == max(__Xb_shape) ):
-            raise ValueError("Shape characteristic of observation operator (H) \"%s\" and state (X) \"%s\" are incompatible."%(__HO_shape,__Xb_shape))
+            raise ValueError(
+                "Shape characteristic of observation operator (H)"+\
+                " \"%s\" and state (X) \"%s\" are incompatible."%(__HO_shape,__Xb_shape))
         if len(self.__HO) > 0 and not isinstance(self.__HO, dict) and not( __HO_shape[0] == max(__Y_shape) ):
-            raise ValueError("Shape characteristic of observation operator (H) \"%s\" and observation (Y) \"%s\" are incompatible."%(__HO_shape,__Y_shape))
+            raise ValueError(
+                "Shape characteristic of observation operator (H)"+\
+                " \"%s\" and observation (Y) \"%s\" are incompatible."%(__HO_shape,__Y_shape))
         if len(self.__HO) > 0 and not isinstance(self.__HO, dict) and len(self.__B) > 0 and not( __HO_shape[1] == __B_shape[0] ):
-            raise ValueError("Shape characteristic of observation operator (H) \"%s\" and a priori errors covariance matrix (B) \"%s\" are incompatible."%(__HO_shape,__B_shape))
+            raise ValueError(
+                "Shape characteristic of observation operator (H)"+\
+                " \"%s\" and a priori errors covariance matrix (B) \"%s\" are incompatible."%(__HO_shape,__B_shape))
         if len(self.__HO) > 0 and not isinstance(self.__HO, dict) and len(self.__R) > 0 and not( __HO_shape[0] == __R_shape[1] ):
-            raise ValueError("Shape characteristic of observation operator (H) \"%s\" and observation errors covariance matrix (R) \"%s\" are incompatible."%(__HO_shape,__R_shape))
+            raise ValueError(
+                "Shape characteristic of observation operator (H)"+\
+                " \"%s\" and observation errors covariance matrix (R) \"%s\" are incompatible."%(__HO_shape,__R_shape))
         #
         if self.__B is not None and len(self.__B) > 0 and not( __B_shape[1] == max(__Xb_shape) ):
             if self.__algorithmName in ["EnsembleBlue",]:
                 asPersistentVector = self.__Xb.reshape((-1,min(__B_shape)))
                 self.__Xb = Persistence.OneVector("Background")
                 for member in asPersistentVector:
                     self.__Xb.store( numpy.asarray(member, dtype=float) )
                 __Xb_shape = min(__B_shape)
             else:
-                raise ValueError("Shape characteristic of a priori errors covariance matrix (B) \"%s\" and background (Xb) \"%s\" are incompatible."%(__B_shape,__Xb_shape))
+                raise ValueError(
+                    "Shape characteristic of a priori errors covariance matrix (B)"+\
+                    " \"%s\" and background vector (Xb) \"%s\" are incompatible."%(__B_shape,__Xb_shape))
         #
         if self.__R is not None and len(self.__R) > 0 and not( __R_shape[1] == max(__Y_shape) ):
-            raise ValueError("Shape characteristic of observation errors covariance matrix (R) \"%s\" and observation (Y) \"%s\" are incompatible."%(__R_shape,__Y_shape))
+            raise ValueError(
+                "Shape characteristic of observation errors covariance matrix (R)"+\
+                " \"%s\" and observation vector (Y) \"%s\" are incompatible."%(__R_shape,__Y_shape))
         #
         if self.__EM is not None and len(self.__EM) > 0 and not isinstance(self.__EM, dict) and not( __EM_shape[1] == max(__Xb_shape) ):
-            raise ValueError("Shape characteristic of evolution model (EM) \"%s\" and state (X) \"%s\" are incompatible."%(__EM_shape,__Xb_shape))
+            raise ValueError(
+                "Shape characteristic of evolution model (EM)"+\
+                " \"%s\" and state (X) \"%s\" are incompatible."%(__EM_shape,__Xb_shape))
         #
         if self.__CM is not None and len(self.__CM) > 0 and not isinstance(self.__CM, dict) and not( __CM_shape[1] == max(__U_shape) ):
-            raise ValueError("Shape characteristic of control model (CM) \"%s\" and control (U) \"%s\" are incompatible."%(__CM_shape,__U_shape))
+            raise ValueError(
+                "Shape characteristic of control model (CM)"+\
+                " \"%s\" and control (U) \"%s\" are incompatible."%(__CM_shape,__U_shape))
         #
         if ("Bounds" in self.__P) \
             and (isinstance(self.__P["Bounds"], list) or isinstance(self.__P["Bounds"], tuple)) \
             and (len(self.__P["Bounds"]) != max(__Xb_shape)):
             raise ValueError("The number \"%s\" of bound pairs for the state (X) components is different of the size \"%s\" of the state itself." \
                 %(len(self.__P["Bounds"]),max(__Xb_shape)))
         #
@@ -1765,15 +1864,14 @@
                __Vector = PlatformInfo.strvect2liststr( __Vector )
             self.__V         = numpy.ravel(numpy.asarray( __Vector, dtype=float )).reshape((-1,1))
             self.shape       = self.__V.shape
             self.size        = self.__V.size
         elif __Series is not None:
             self.__is_series  = True
             if isinstance(__Series, (tuple, list, numpy.ndarray, numpy.matrix, str)):
-                #~ self.__V = Persistence.OneVector(self.__name, basetype=numpy.matrix)
                 self.__V = Persistence.OneVector(self.__name)
                 if isinstance(__Series, str):
                     __Series = PlatformInfo.strmatrix2liststr(__Series)
                 for member in __Series:
                     if isinstance(member, str):
                         member = PlatformInfo.strvect2liststr( member )
                     self.__V.store(numpy.asarray( member, dtype=float ))
@@ -1783,15 +1881,18 @@
                 self.shape       = self.__V.shape
             else:
                 self.shape       = self.__V.shape()
             if len(self.shape) == 1:
                 self.shape       = (self.shape[0],1)
             self.size        = self.shape[0] * self.shape[1]
         else:
-            raise ValueError("The %s object is improperly defined or undefined, it requires at minima either a vector, a list/tuple of vectors or a persistent object. Please check your vector input."%self.__name)
+            raise ValueError(
+                "The %s object is improperly defined or undefined,"%self.__name+\
+                " it requires at minima either a vector, a list/tuple of"+\
+                " vectors or a persistent object. Please check your vector input.")
         #
         if scheduledBy is not None:
             self.__T = scheduledBy
 
     def getO(self, withScheduler=False):
         if withScheduler:
             return self.__V, self.__T
@@ -1870,15 +1971,18 @@
             __Matrix, __Scalar, __Vector, __Object = asCovariance, asEyeByScalar, asEyeByVector, asCovObject
         #
         if __Scalar is not None:
             if isinstance(__Scalar, str):
                 __Scalar = PlatformInfo.strvect2liststr( __Scalar )
                 if len(__Scalar) > 0: __Scalar = __Scalar[0]
             if numpy.array(__Scalar).size != 1:
-                raise ValueError('  The diagonal multiplier given to define a sparse matrix is not a unique scalar value.\n  Its actual measured size is %i. Please check your scalar input.'%numpy.array(__Scalar).size)
+                raise ValueError(
+                    "  The diagonal multiplier given to define a sparse matrix is"+\
+                    " not a unique scalar value.\n  Its actual measured size is"+\
+                    " %i. Please check your scalar input."%numpy.array(__Scalar).size)
             self.__is_scalar = True
             self.__C         = numpy.abs( float(__Scalar) )
             self.shape       = (0,0)
             self.size        = 0
         elif __Vector is not None:
             if isinstance(__Vector, str):
                 __Vector = PlatformInfo.strvect2liststr( __Vector )
@@ -1903,15 +2007,14 @@
                 self.shape       = (0,0)
             if hasattr(self.__C,"size"):
                 self.size        = self.__C.size
             else:
                 self.size        = 0
         else:
             pass
-            # raise ValueError("The %s covariance matrix has to be specified either as a matrix, a vector for its diagonal or a scalar multiplying an identity matrix."%self.__name)
         #
         self.__validate()
 
     def __validate(self):
         "Validation"
         if self.__C is None:
             raise UnboundLocalError("%s covariance matrix value has not been set!"%(self.__name,))
@@ -1921,21 +2024,21 @@
             raise ValueError("The matrix given for \"%s\" is not a square one, its shape is %s. Please check your object input."%(self.__name,self.shape))
         if self.isscalar() and self.__C <= 0:
             raise ValueError("The \"%s\" covariance matrix is not positive-definite. Please check your scalar input %s."%(self.__name,self.__C))
         if self.isvector() and (self.__C <= 0).any():
             raise ValueError("The \"%s\" covariance matrix is not positive-definite. Please check your vector input."%(self.__name,))
         if self.ismatrix() and (self.__check or logging.getLogger().level < logging.WARNING):
             try:
-                L = numpy.linalg.cholesky( self.__C )
-            except:
+                numpy.linalg.cholesky( self.__C )
+            except Exception:
                 raise ValueError("The %s covariance matrix is not symmetric positive-definite. Please check your matrix input."%(self.__name,))
         if self.isobject() and (self.__check or logging.getLogger().level < logging.WARNING):
             try:
-                L = self.__C.cholesky()
-            except:
+                self.__C.cholesky()
+            except Exception:
                 raise ValueError("The %s covariance object is not symmetric positive-definite. Please check your matrix input."%(self.__name,))
 
     def isscalar(self):
         "Vérification du type interne"
         return self.__is_scalar
 
     def isvector(self):
@@ -2095,15 +2198,18 @@
 
     def __add__(self, other):
         "x.__add__(y) <==> x+y"
         if   self.ismatrix() or self.isobject():
             return self.__C + numpy.asmatrix(other)
         elif self.isvector() or self.isscalar():
             _A = numpy.asarray(other)
-            _A.reshape(_A.size)[::_A.shape[1]+1] += self.__C
+            if len(_A.shape) == 1:
+                _A.reshape((-1,1))[::2] += self.__C
+            else:
+                _A.reshape(_A.size)[::_A.shape[1]+1] += self.__C
             return numpy.asmatrix(_A)
 
     def __radd__(self, other):
         "x.__radd__(y) <==> y+x"
         raise NotImplementedError("%s covariance matrix __radd__ method not available for %s type!"%(self.__name,type(other)))
 
     def __sub__(self, other):
@@ -2159,85 +2265,94 @@
             return self.__C * other
         elif self.ismatrix() and isinstance(other, (list, numpy.ndarray, tuple)):
             if numpy.ravel(other).size == self.shape[1]: # Vecteur
                 return self.__C * numpy.asmatrix(numpy.ravel(other)).T
             elif numpy.asmatrix(other).shape[0] == self.shape[1]: # Matrice
                 return self.__C * numpy.asmatrix(other)
             else:
-                raise ValueError("operands could not be broadcast together with shapes %s %s in %s matrix"%(self.shape,numpy.asmatrix(other).shape,self.__name))
+                raise ValueError(
+                    "operands could not be broadcast together with shapes %s %s in %s matrix"%(self.shape,numpy.asmatrix(other).shape,self.__name))
         elif self.isvector() and isinstance(other, (list, numpy.matrix, numpy.ndarray, tuple)):
             if numpy.ravel(other).size == self.shape[1]: # Vecteur
                 return numpy.asmatrix(self.__C * numpy.ravel(other)).T
             elif numpy.asmatrix(other).shape[0] == self.shape[1]: # Matrice
                 return numpy.asmatrix((self.__C * (numpy.asarray(other).transpose())).transpose())
             else:
-                raise ValueError("operands could not be broadcast together with shapes %s %s in %s matrix"%(self.shape,numpy.ravel(other).shape,self.__name))
+                raise ValueError(
+                    "operands could not be broadcast together with shapes %s %s in %s matrix"%(self.shape,numpy.ravel(other).shape,self.__name))
         elif self.isscalar() and isinstance(other,numpy.matrix):
             return self.__C * other
         elif self.isscalar() and isinstance(other, (list, numpy.ndarray, tuple)):
             if len(numpy.asarray(other).shape) == 1 or numpy.asarray(other).shape[1] == 1 or numpy.asarray(other).shape[0] == 1:
                 return self.__C * numpy.asmatrix(numpy.ravel(other)).T
             else:
                 return self.__C * numpy.asmatrix(other)
         elif self.isobject():
             return self.__C.__mul__(other)
         else:
-            raise NotImplementedError("%s covariance matrix __mul__ method not available for %s type!"%(self.__name,type(other)))
+            raise NotImplementedError(
+                "%s covariance matrix __mul__ method not available for %s type!"%(self.__name,type(other)))
 
     def __rmatmul__(self, other):
         "x.__rmul__(y) <==> y@x"
         if self.ismatrix() and isinstance(other, (int, numpy.matrix, float)):
             return other * self.__C
         elif self.ismatrix() and isinstance(other, (list, numpy.ndarray, tuple)):
             if numpy.ravel(other).size == self.shape[1]: # Vecteur
                 return numpy.asmatrix(numpy.ravel(other)) * self.__C
             elif numpy.asmatrix(other).shape[0] == self.shape[1]: # Matrice
                 return numpy.asmatrix(other) * self.__C
             else:
-                raise ValueError("operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.asmatrix(other).shape,self.shape,self.__name))
+                raise ValueError(
+                    "operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.asmatrix(other).shape,self.shape,self.__name))
         elif self.isvector() and isinstance(other,numpy.matrix):
             if numpy.ravel(other).size == self.shape[0]: # Vecteur
                 return numpy.asmatrix(numpy.ravel(other) * self.__C)
             elif numpy.asmatrix(other).shape[1] == self.shape[0]: # Matrice
                 return numpy.asmatrix(numpy.array(other) * self.__C)
             else:
-                raise ValueError("operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.ravel(other).shape,self.shape,self.__name))
+                raise ValueError(
+                    "operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.ravel(other).shape,self.shape,self.__name))
         elif self.isscalar() and isinstance(other,numpy.matrix):
             return other * self.__C
         elif self.isobject():
             return self.__C.__rmatmul__(other)
         else:
-            raise NotImplementedError("%s covariance matrix __rmatmul__ method not available for %s type!"%(self.__name,type(other)))
+            raise NotImplementedError(
+                "%s covariance matrix __rmatmul__ method not available for %s type!"%(self.__name,type(other)))
 
     def __rmul__(self, other):
         "x.__rmul__(y) <==> y*x"
         if self.ismatrix() and isinstance(other, (int, numpy.matrix, float)):
             return other * self.__C
         elif self.ismatrix() and isinstance(other, (list, numpy.ndarray, tuple)):
             if numpy.ravel(other).size == self.shape[1]: # Vecteur
                 return numpy.asmatrix(numpy.ravel(other)) * self.__C
             elif numpy.asmatrix(other).shape[0] == self.shape[1]: # Matrice
                 return numpy.asmatrix(other) * self.__C
             else:
-                raise ValueError("operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.asmatrix(other).shape,self.shape,self.__name))
+                raise ValueError(
+                    "operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.asmatrix(other).shape,self.shape,self.__name))
         elif self.isvector() and isinstance(other,numpy.matrix):
             if numpy.ravel(other).size == self.shape[0]: # Vecteur
                 return numpy.asmatrix(numpy.ravel(other) * self.__C)
             elif numpy.asmatrix(other).shape[1] == self.shape[0]: # Matrice
                 return numpy.asmatrix(numpy.array(other) * self.__C)
             else:
-                raise ValueError("operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.ravel(other).shape,self.shape,self.__name))
+                raise ValueError(
+                    "operands could not be broadcast together with shapes %s %s in %s matrix"%(numpy.ravel(other).shape,self.shape,self.__name))
         elif self.isscalar() and isinstance(other,numpy.matrix):
             return other * self.__C
         elif self.isscalar() and isinstance(other,float):
             return other * self.__C
         elif self.isobject():
             return self.__C.__rmul__(other)
         else:
-            raise NotImplementedError("%s covariance matrix __rmul__ method not available for %s type!"%(self.__name,type(other)))
+            raise NotImplementedError(
+                "%s covariance matrix __rmul__ method not available for %s type!"%(self.__name,type(other)))
 
     def __len__(self):
         "x.__len__() <==> len(x)"
         return self.shape[0]
 
 # ==============================================================================
 class Observer2Func(object):
@@ -2336,15 +2451,14 @@
         __mpEnabled = False
         __mpWorkers = None
     #
     # Calculs effectifs
     if __mpEnabled:
         _jobs = __xserie
         # logging.debug("MULTF Internal multiprocessing calculations begin : evaluation of %i point(s)"%(len(_jobs),))
-        import multiprocessing
         with multiprocessing.Pool(__mpWorkers) as pool:
             __multiHX = pool.map( _sFunction, _jobs )
             pool.close()
             pool.join()
         # logging.debug("MULTF Internal multiprocessing calculation end")
     else:
         # logging.debug("MULTF Internal monoprocessing calculation begin")
@@ -2361,125 +2475,11 @@
         else:
             raise TypeError("MultiFonction extra arguments unkown input type: %s"%(type(_extraArguments),))
         # logging.debug("MULTF Internal monoprocessing calculation end")
     #
     # logging.debug("MULTF Internal multifonction calculations end")
     return __multiHX
 
-# ==============================================================================
-def CostFunction3D(_x,
-                   _Hm  = None,  # Pour simuler Hm(x) : HO["Direct"].appliedTo
-                   _HmX = None,  # Simulation déjà faite de Hm(x)
-                   _arg = None,  # Arguments supplementaires pour Hm, sous la forme d'un tuple
-                   _BI  = None,
-                   _RI  = None,
-                   _Xb  = None,
-                   _Y   = None,
-                   _SIV = False, # A résorber pour la 8.0
-                   _SSC = [],    # self._parameters["StoreSupplementaryCalculations"]
-                   _nPS = 0,     # nbPreviousSteps
-                   _QM  = "DA",  # QualityMeasure
-                   _SSV = {},    # Entrée et/ou sortie : self.StoredVariables
-                   _fRt = False, # Restitue ou pas la sortie étendue
-                   _sSc = True,  # Stocke ou pas les SSC
-                  ):
-    """
-    Fonction-coût générale utile pour les algorithmes statiques/3D : 3DVAR, BLUE
-    et dérivés, Kalman et dérivés, LeastSquares, SamplingTest, PSO, SA, Tabu,
-    DFO, QuantileRegression
-    """
-    if not _sSc:
-        _SIV = False
-        _SSC = {}
-    else:
-        for k in ["CostFunctionJ",
-                  "CostFunctionJb",
-                  "CostFunctionJo",
-                  "CurrentOptimum",
-                  "CurrentState",
-                  "IndexOfOptimum",
-                  "SimulatedObservationAtCurrentOptimum",
-                  "SimulatedObservationAtCurrentState",
-                 ]:
-            if k not in _SSV:
-                _SSV[k] = []
-            if hasattr(_SSV[k],"store"):
-                _SSV[k].append = _SSV[k].store # Pour utiliser "append" au lieu de "store"
-    #
-    _X  = numpy.asmatrix(numpy.ravel( _x )).T
-    if _SIV or "CurrentState" in _SSC or "CurrentOptimum" in _SSC:
-        _SSV["CurrentState"].append( _X )
-    #
-    if _HmX is not None:
-        _HX = _HmX
-    else:
-        if _Hm is None:
-            raise ValueError("COSTFUNCTION3D Operator has to be defined.")
-        if _arg is None:
-            _HX = _Hm( _X )
-        else:
-            _HX = _Hm( _X, *_arg )
-    _HX = numpy.asmatrix(numpy.ravel( _HX )).T
-    #
-    if "SimulatedObservationAtCurrentState" in _SSC or \
-       "SimulatedObservationAtCurrentOptimum" in _SSC:
-        _SSV["SimulatedObservationAtCurrentState"].append( _HX )
-    #
-    if numpy.any(numpy.isnan(_HX)):
-        Jb, Jo, J = numpy.nan, numpy.nan, numpy.nan
-    else:
-        _Y   = numpy.asmatrix(numpy.ravel( _Y )).T
-        if _QM in ["AugmentedWeightedLeastSquares", "AWLS", "AugmentedPonderatedLeastSquares", "APLS", "DA"]:
-            if _BI is None or _RI is None:
-                raise ValueError("Background and Observation error covariance matrix has to be properly defined!")
-            _Xb  = numpy.asmatrix(numpy.ravel( _Xb )).T
-            Jb  = 0.5 * (_X - _Xb).T * _BI * (_X - _Xb)
-            Jo  = 0.5 * (_Y - _HX).T * _RI * (_Y - _HX)
-        elif _QM in ["WeightedLeastSquares", "WLS", "PonderatedLeastSquares", "PLS"]:
-            if _RI is None:
-                raise ValueError("Observation error covariance matrix has to be properly defined!")
-            Jb  = 0.
-            Jo  = 0.5 * (_Y - _HX).T * _RI * (_Y - _HX)
-        elif _QM in ["LeastSquares", "LS", "L2"]:
-            Jb  = 0.
-            Jo  = 0.5 * (_Y - _HX).T * (_Y - _HX)
-        elif _QM in ["AbsoluteValue", "L1"]:
-            Jb  = 0.
-            Jo  = numpy.sum( numpy.abs(_Y - _HX) )
-        elif _QM in ["MaximumError", "ME"]:
-            Jb  = 0.
-            Jo  = numpy.max( numpy.abs(_Y - _HX) )
-        elif _QM in ["QR", "Null"]:
-            Jb  = 0.
-            Jo  = 0.
-        else:
-            raise ValueError("Unknown asked quality measure!")
-        #
-        J   = float( Jb ) + float( Jo )
-    #
-    if _sSc:
-        _SSV["CostFunctionJb"].append( Jb )
-        _SSV["CostFunctionJo"].append( Jo )
-        _SSV["CostFunctionJ" ].append( J )
-    #
-    if "IndexOfOptimum" in _SSC or \
-       "CurrentOptimum" in _SSC or \
-       "SimulatedObservationAtCurrentOptimum" in _SSC:
-        IndexMin = numpy.argmin( _SSV["CostFunctionJ"][_nPS:] ) + _nPS
-    if "IndexOfOptimum" in _SSC:
-        _SSV["IndexOfOptimum"].append( IndexMin )
-    if "CurrentOptimum" in _SSC:
-        _SSV["CurrentOptimum"].append( _SSV["CurrentState"][IndexMin] )
-    if "SimulatedObservationAtCurrentOptimum" in _SSC:
-        _SSV["SimulatedObservationAtCurrentOptimum"].append( _SSV["SimulatedObservationAtCurrentState"][IndexMin] )
-    #
-    if _fRt:
-        return _SSV
-    else:
-        if _QM in ["QR"]: # Pour le QuantileRegression
-            return _HX
-        else:
-            return J
 
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/ExtendedLogging.py` & `adao-9.9.0.1/adao/daCore/ExtendedLogging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -154,10 +154,11 @@
         result = f(*args, **kwargs)
         end    = time.clock() # time.time()
         msg    = 'TIMER Durée elapsed de la fonction utilisateur "{}": {:.3f}s'
         logging.debug(msg.format(f.__name__, end-start))
         return result
     return wrapper
 
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/Interfaces.py` & `adao-9.9.0.1/adao/daCore/Interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -48,25 +48,39 @@
         self._objname      = str(__objname)
         self._lineSerie    = []
         self._switchoff    = False
         self._numobservers = 2
         self._content      = __content
         self._object       = __object
         self._missing = """raise ValueError("This case requires beforehand to import or define the variable named <%s>. When corrected, remove this command, correct and uncomment the following one.")\n# """
+    #------------------------
     def _append(self, *args):
         "Transformation d'une commande individuelle en un enregistrement"
         raise NotImplementedError()
     def _extract(self, *args):
         "Transformation d'enregistrement(s) en commande(s) individuelle(s)"
         raise NotImplementedError()
+    #------------------------------
+    def _initialize(self, __multilines):
+        "Permet des pré-conversions automatiques simples de commandes ou clés"
+        __translation = {
+            "Study_name"          :"StudyName",
+            "Study_repertory"     :"StudyRepertory",
+            "MaximumNumberOfSteps":"MaximumNumberOfIterations",
+            "FunctionDict"        :"ScriptWithSwitch",
+            "FUNCTIONDICT_FILE"   :"SCRIPTWITHSWITCH_FILE",
+        }
+        for k,v in __translation.items():
+            __multilines = __multilines.replace(k,v)
+        return __multilines
     def _finalize(self, __upa=None):
         "Enregistrement du final"
         __hasNotExecute = True
-        for l in self._lineSerie:
-            if "%s.execute"%(self._objname,) in l: __hasNotExecute = False
+        for __l in self._lineSerie:
+            if "%s.execute"%(self._objname,) in __l: __hasNotExecute = False
         if __hasNotExecute:
             self._lineSerie.append("%s.execute()"%(self._objname,))
         if __upa is not None and len(__upa)>0:
             __upa = __upa.replace("ADD",str(self._objname))
             self._lineSerie.append(__upa)
     def _addLine(self, line=""):
         "Ajoute un enregistrement individuel"
@@ -84,16 +98,17 @@
             __fid.write(__text)
             __fid.close()
         return __text
     def load(self, __filename=None, __content=None, __object=None):
         "Chargement normalisé des commandes"
         if __filename is not None and os.path.exists(__filename):
             self._content = open(__filename, 'r').read()
+            self._content = self._initialize(self._content)
         elif __content is not None and type(__content) is str:
-            self._content = __content
+            self._content = self._initialize(__content)
         elif __object is not None and type(__object) is dict:
             self._object = copy.deepcopy(__object)
         else:
             pass # use "self._content" from initialization
         __commands = self._extract(self._content, self._object)
         return __commands
 
@@ -234,15 +249,15 @@
             elif __command == "UserPostAnalysis" and type(r) is dict:
                 if 'STRING' in r:
                     __UserPostAnalysis = r['STRING'].replace("ADD",str(self._objname))
                     __commands.append( "set( Concept='UserPostAnalysis', String=\"\"\"%s\"\"\" )"%(__UserPostAnalysis,) )
                 elif 'SCRIPT_FILE' in r and os.path.exists(r['SCRIPT_FILE']):
                     __UserPostAnalysis = open(r['SCRIPT_FILE'],'r').read()
                     __commands.append( "set( Concept='UserPostAnalysis', Script='%s' )"%(r['SCRIPT_FILE'],) )
-                elif 'Template' in r and not 'ValueTemplate' in r:
+                elif 'Template' in r and 'ValueTemplate' not in r:
                     # AnalysisPrinter...
                     if r['Template'] not in Templates.UserPostAnalysisTemplates:
                         raise ValueError("User post-analysis template \"%s\" does not exist."%(r['Template'],))
                     else:
                         __UserPostAnalysis = Templates.UserPostAnalysisTemplates[r['Template']]
                     __commands.append( "set( Concept='UserPostAnalysis', Template='%s' )"%(r['Template'],) )
                 elif 'Template' in r and 'ValueTemplate' in r:
@@ -434,16 +449,18 @@
             __vectorIsScript = False
             for __k,__v in __local.items():
                 if __v is None: __to_be_removed.append(__k)
             for __k in __to_be_removed:
                 __local.pop(__k)
             for __k,__v in __local.items():
                 if __k == "Concept": continue
-                if __k in ['ScalarSparseMatrix','DiagonalSparseMatrix','Matrix','OneFunction','ThreeFunctions'] and 'Script' in __local and __local['Script'] is not None: continue
-                if __k in ['Vector','VectorSerie'] and 'DataFile' in __local and __local['DataFile'] is not None: continue
+                if __k in ['ScalarSparseMatrix','DiagonalSparseMatrix','Matrix','OneFunction','ThreeFunctions'] \
+                    and 'Script' in __local and __local['Script'] is not None: continue
+                if __k in ['Vector','VectorSerie'] \
+                    and 'DataFile' in __local and __local['DataFile'] is not None: continue
                 if __k == 'Parameters' and not (__command in ['AlgorithmParameters','SupplementaryParameters']): continue
                 if __k == 'Algorithm':
                     __text += "study_config['Algorithm'] = %s\n"%(repr(__v))
                 elif __k == 'DataFile':
                     __k = 'Vector'
                     __f = 'DataFile'
                     __v = "'"+repr(__v)+"'"
@@ -588,15 +605,15 @@
             __file    = os.path.abspath(__filename)
             if os.path.isfile(__file) or os.path.islink(__file):
                 os.remove(__file)
         # -----
         if not PlatformInfo.has_salome or \
             not PlatformInfo.has_adao:
             raise ImportError(
-                "Unable to get SALOME or ADAO environnement for YACS conversion.\n"+\
+                "Unable to get SALOME (%s) or ADAO (%s) environnement for YACS conversion.\n"%(PlatformInfo.has_salome,PlatformInfo.has_adao)+\
                 "Please load the right SALOME environnement before trying to use it.")
         else:
             from daYacsSchemaCreator.run import create_schema_from_content
         # -----
         self.__internalSCD._finalize(__upa)
         __SCDdump = self.__internalSCD.dump()
         create_schema_from_content(__SCDdump, __file)
@@ -648,15 +665,15 @@
                 if   k == "nextStep"             and not __v: continue
                 if   k == "PerformanceProfile"   and     __v: continue
                 if   k == "noDetails":                        continue
                 if   k == "Concept":                          continue
                 if   k == "self":                             continue
                 if isinstance(__v,Persistence.Persistence): __v = __v.values()
                 numpy.set_printoptions(precision=15,threshold=1000000,linewidth=1000*15)
-                __ktext += "\n        %s = %s, "%(k,repr(__v))
+                __ktext += "\n        %s = %s,"%(k,repr(__v))
                 numpy.set_printoptions(precision=8,threshold=1000,linewidth=75)
             if len(__ktext) > 0:
                 __text += " with values:" + __ktext
             __text = __text.rstrip(", ")
             self._r.append(__text, "uli")
     def _finalize(self, __upa=None):
         "Enregistrement du final"
@@ -690,15 +707,17 @@
     """
     __slots__ = ("__basename", "__filenspace", "__filestring")
     def __init__(self, __filename=None):
         "Verifie l'existence et importe le script"
         if __filename is None:
             raise ValueError("The name of the file, containing the variable to be read, has to be specified.")
         if not os.path.isfile(__filename):
-            raise ValueError("The file containing the variable to be imported doesn't seem to exist. Please check the file. The given file name is:\n  \"%s\""%str(__filename))
+            raise ValueError(
+                "The file containing the variable to be imported doesn't seem to"+\
+                " exist. Please check the file. The given file name is:\n  \"%s\""%str(__filename))
         if os.path.dirname(__filename) != '':
             sys.path.insert(0, os.path.dirname(__filename))
             __basename = os.path.basename(__filename).rstrip(".py")
         else:
             __basename = __filename.rstrip(".py")
         PlatformInfo.checkFileNameImportability( __basename+".py" )
         self.__basename = __basename
@@ -710,17 +729,23 @@
             self.__filestring = fid.read()
     def getvalue(self, __varname=None, __synonym=None ):
         "Renvoie la variable demandee par son nom ou son synonyme"
         if __varname is None:
             raise ValueError("The name of the variable to be read has to be specified. Please check the content of the file and the syntax.")
         if not hasattr(self.__filenspace, __varname):
             if __synonym is None:
-                raise ValueError("The imported script file \"%s\" doesn't contain the mandatory variable \"%s\" to be read. Please check the content of the file and the syntax."%(str(self.__basename)+".py",__varname))
+                raise ValueError(
+                    "The imported script file \"%s\""%(str(self.__basename)+".py",)+\
+                    " doesn't contain the mandatory variable \"%s\""%(__varname,)+\
+                    " to be read. Please check the content of the file and the syntax.")
             elif not hasattr(self.__filenspace, __synonym):
-                raise ValueError("The imported script file \"%s\" doesn't contain the mandatory variable \"%s\" to be read. Please check the content of the file and the syntax."%(str(self.__basename)+".py",__synonym))
+                raise ValueError(
+                    "The imported script file \"%s\""%(str(self.__basename)+".py",)+\
+                    " doesn't contain the mandatory variable \"%s\""%(__synonym,)+\
+                    " to be read. Please check the content of the file and the syntax.")
             else:
                 return getattr(self.__filenspace, __synonym)
         else:
             return getattr(self.__filenspace, __varname)
     def getstring(self):
         "Renvoie le script complet"
         return self.__filestring
@@ -728,16 +753,18 @@
 # ==============================================================================
 class ImportDetector(object):
     """
     Détection des caractéristiques de fichiers ou objets en entrée
     """
     __slots__ = (
         "__url", "__usr", "__root", "__end")
-    def __enter__(self): return self
-    def __exit__(self, exc_type, exc_val, exc_tb): return False
+    def __enter__(self):
+        return self
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        return False
     #
     def __init__(self, __url, UserMime=""):
         if __url is None:
             raise ValueError("The name or url of the file object has to be specified.")
         if __url is bytes:
             self.__url = __url.decode()
         else:
@@ -760,38 +787,32 @@
     # ------------------
     def is_local_file(self):
         if os.path.isfile(os.path.realpath(self.__url)):
             return True
         else:
             return False
     def is_not_local_file(self):
-        if not os.path.isfile(os.path.realpath(self.__url)):
-            return True
-        else:
-            return False
+        return not self.is_local_file()
     def raise_error_if_not_local_file(self):
-        if not os.path.isfile(os.path.realpath(self.__url)):
+        if self.is_not_local_file():
             raise ValueError("The name or the url of the file object doesn't seem to exist. The given name is:\n  \"%s\""%str(self.__url))
         else:
             return False
     #
     # Directory related tests
     # -----------------------
     def is_local_dir(self):
         if os.path.isdir(self.__url):
             return True
         else:
             return False
     def is_not_local_dir(self):
-        if not os.path.isdir(self.__url):
-            return True
-        else:
-            return False
+        return not self.is_local_dir()
     def raise_error_if_not_local_dir(self):
-        if not os.path.isdir(self.__url):
+        if self.is_not_local_dir():
             raise ValueError("The name or the url of the directory object doesn't seem to exist. The given name is:\n  \"%s\""%str(self.__url))
         else:
             return False
     #
     # Mime related functions
     # ------------------------
     def get_standard_mime(self):
@@ -831,16 +852,18 @@
     textes doivent présenter en première ligne (hors commentaire ou ligne vide)
     les noms des variables de colonnes. Les commentaires commencent par un "#".
     """
     __slots__ = (
         "_filename", "_colnames", "_colindex", "_varsline", "_format",
         "_delimiter", "_skiprows", "__url", "__filestring", "__header",
         "__allowvoid", "__binaryformats", "__supportedformats")
-    def __enter__(self): return self
-    def __exit__(self, exc_type, exc_val, exc_tb): return False
+    def __enter__(self):
+        return self
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        return False
     #
     def __init__(self, Filename=None, ColNames=None, ColIndex=None, Format="Guess", AllowVoidNameList=True):
         """
         Verifie l'existence et les informations de définition du fichier. Les
         noms de colonnes ou de variables sont ignorées si le format ne permet
         pas de les indiquer.
         Arguments :
@@ -898,15 +921,15 @@
         else:
             with open(self._filename,'r') as fid:
                 __line = fid.readline().strip()
                 while "#" in __line or len(__line) < 1:
                     __header.append(__line)
                     __skiprows += 1
                     __line = fid.readline().strip()
-                __varsline = __line
+                __varsline = __line # Ligne de labels par convention
                 for i in range(max(0,__nblines)):
                     __header.append(fid.readline())
         return (__header, __varsline, __skiprows)
 
     def __getindices(self, __colnames, __colindex, __delimiter=None ):
         "Indices de colonnes correspondants à l'index et aux variables"
         if __delimiter is None:
@@ -946,15 +969,15 @@
         self.__supportedformats["text/tab-separated-values"] = True
         self.__supportedformats["application/numpy.npy"]     = True
         self.__supportedformats["application/numpy.npz"]     = True
         self.__supportedformats["application/dymola.sdf"]    = PlatformInfo.has_sdf
         return self.__supportedformats
 
     def getvalue(self, ColNames=None, ColIndex=None ):
-        "Renvoie la ou les variables demandees par la liste de leurs noms"
+        "Renvoie la ou les variables demandées par la liste de leurs noms"
         # Uniquement si mise à jour
         if ColNames is not None: self._colnames = tuple(ColNames)
         if ColIndex is not None: self._colindex = str(ColIndex)
         #
         __index = None
         if self._format == "application/numpy.npy":
             __columns = numpy.load(self._filename)
@@ -1016,15 +1039,15 @@
             if __useindex is not None:
                 __index = numpy.loadtxt(self._filename, dtype = bytes, usecols = (__useindex,), delimiter = self._delimiter, skiprows=self._skiprows)
             if __usecols is None: # Si une variable demandée n'existe pas
                 self._colnames = None
         else:
             raise ValueError("Unkown file format \"%s\" or no reader available"%self._format)
         if __columns is None: __columns = ()
-        #
+
         def toString(value):
             try:
                 return value.decode()
             except ValueError:
                 return value
         if __index is not None:
             __index = tuple([toString(v) for v in __index])
@@ -1048,35 +1071,39 @@
     fichier comporte soit 2, soit 4 colonnes, obligatoirement nommées "Name",
     "Value", "Minimum", "Maximum" si les noms sont précisés. Sur chaque ligne
     est indiqué le nom, la valeur, et éventuelement deux bornes min et max (ou
     None si nécessaire pour une borne).
 
     Seule la méthode "getvalue" est changée.
     """
-    def __enter__(self): return self
-    def __exit__(self, exc_type, exc_val, exc_tb): return False
+    def __enter__(self):
+        return self
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        return False
     #
     def __init__(self, Filename=None, ColNames=None, ColIndex=None, Format="Guess"):
         ImportFromFile.__init__(self, Filename, ColNames, ColIndex, Format)
         if self._format not in ["text/plain", "text/csv", "text/tab-separated-values"]:
             raise ValueError("Unkown file format \"%s\""%self._format)
     #
     def getvalue(self, VarNames = None, HeaderNames=()):
-        "Renvoie la ou les variables demandees par la liste de leurs noms"
+        "Renvoie la ou les variables demandées par la liste de leurs noms"
         if VarNames is not None: __varnames = tuple(VarNames)
         else:                    __varnames = None
         #
         if "Name" in self._varsline and "Value" in self._varsline and "Minimum" in self._varsline and "Maximum" in self._varsline:
             __ftype = "NamValMinMax"
             __dtypes   = {'names'  : ('Name', 'Value', 'Minimum', 'Maximum'),
                           'formats': ('S128', 'g', 'g', 'g')}
             __usecols  = (0, 1, 2, 3)
+
             def __replaceNoneN( s ):
                 if s.strip() == b'None': return numpy.NINF
                 else:                    return s
+
             def __replaceNoneP( s ):
                 if s.strip() == b'None': return numpy.PINF
                 else:                    return s
             __converters = {2: __replaceNoneN, 3: __replaceNoneP}
         elif "Name" in self._varsline and "Value" in self._varsline and ("Minimum" not in self._varsline or "Maximum" not in self._varsline):
             __ftype = "NamVal"
             __dtypes   = {'names'  : ('Name', 'Value'),
@@ -1084,27 +1111,41 @@
             __converters = None
             __usecols  = (0, 1)
         elif len(HeaderNames)>0 and numpy.all([kw in self._varsline for kw in HeaderNames]):
             __ftype = "NamLotOfVals"
             __dtypes   = {'names'  : HeaderNames,
                           'formats': tuple(['S128',]+['g']*(len(HeaderNames)-1))}
             __usecols  = tuple(range(len(HeaderNames)))
+
             def __replaceNone( s ):
                 if s.strip() == b'None': return numpy.NAN
                 else:                    return s
             __converters = dict()
             for i in range(1,len(HeaderNames)):
                 __converters[i] = __replaceNone
         else:
-            raise ValueError("Can not find names of columns for initial values. Wrong first line is:\n            \"%s\""%__firstline)
+            raise ValueError("Can not find names of columns for initial values. Wrong first line is:\n            \"%s\""%self._varsline)
         #
         if self._format == "text/plain":
-            __content = numpy.loadtxt(self._filename, dtype = __dtypes, usecols = __usecols, skiprows = self._skiprows, converters = __converters)
+            __content = numpy.loadtxt(
+                self._filename,
+                dtype      = __dtypes,
+                usecols    = __usecols,
+                skiprows   = self._skiprows,
+                converters = __converters,
+                )
         elif self._format in ["text/csv", "text/tab-separated-values"]:
-            __content = numpy.loadtxt(self._filename, dtype = __dtypes, usecols = __usecols, skiprows = self._skiprows, converters = __converters, delimiter = self._delimiter)
+            __content = numpy.loadtxt(
+                self._filename,
+                dtype      = __dtypes,
+                usecols    = __usecols,
+                skiprows   = self._skiprows,
+                converters = __converters,
+                delimiter  = self._delimiter,
+                )
         else:
             raise ValueError("Unkown file format \"%s\""%self._format)
         #
         __names, __thevalue, __bounds = [], [], []
         for sub in __content:
             if len(__usecols) == 4:
                 na, va, mi, ma = sub
@@ -1144,14 +1185,17 @@
         # Chemin pour l'installation (ordre important)
         self.__msg = ""
         self.__path_settings_ok = False
         #----------------
         if "EFICAS_ROOT" in os.environ:
             __EFICAS_ROOT = os.environ["EFICAS_ROOT"]
             __path_ok = True
+        elif "EFICAS_NOUVEAU_ROOT" in os.environ:
+            __EFICAS_ROOT = os.environ["EFICAS_NOUVEAU_ROOT"]
+            __path_ok = True
         else:
             self.__msg += "\nKeyError:\n"+\
                 "  the required environment variable EFICAS_ROOT is unknown.\n"+\
                 "  You have either to be in SALOME environment, or to set\n"+\
                 "  this variable in your environment to the right path \"<...>\"\n"+\
                 "  to find an installed EFICAS application. For example:\n"+\
                 "      EFICAS_ROOT=\"<...>\" command\n"
@@ -1208,10 +1252,11 @@
             logging.debug("Launching standalone EFICAS/ADAO interface...")
             from daEficas import prefs
             from InterfaceQT4 import eficas_go
             eficas_go.lanceEficas(code=prefs.code)
         else:
             logging.debug("Can not launch standalone EFICAS/ADAO interface for path errors.")
 
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/Persistence.py` & `adao-9.9.0.1/adao/daCore/Persistence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -17,41 +17,33 @@
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
 """
-    Définit des outils de persistence et d'enregistrement de séries de valeurs
+    Définit des outils de persistance et d'enregistrement de séries de valeurs
     pour analyse ultérieure ou utilisation de calcul.
 """
 __author__ = "Jean-Philippe ARGAUD"
 __all__ = []
 
-import os, sys, numpy, copy
-import gzip, bz2
+import os, numpy, copy, math
+import gzip, bz2, pickle
 
 from daCore.PlatformInfo import PathManagement ; PathManagement()
 from daCore.PlatformInfo import has_gnuplot, PlatformInfo
 mfp = PlatformInfo().MaximumPrecision()
 if has_gnuplot:
     import Gnuplot
 
-if sys.version_info.major < 3:
-    range = xrange
-    iLong = long
-    import cPickle as pickle
-else:
-    iLong = int
-    import pickle
-
 # ==============================================================================
 class Persistence(object):
     """
-    Classe générale de persistence définissant les accesseurs nécessaires
+    Classe générale de persistance définissant les accesseurs nécessaires
     (Template)
     """
     def __init__(self, name="", unit="", basetype=str):
         """
         name : nom courant
         unit : unité
         basetype : type de base de l'objet stocké à chaque pas
@@ -101,15 +93,15 @@
         __step = len(self.__values) - 1
         for hook, parameters, scheduler in self.__dataobservers:
             if __step in scheduler:
                 hook( self, parameters )
 
     def pop(self, item=None):
         """
-        Retire une valeur enregistree par son index de stockage. Sans argument,
+        Retire une valeur enregistrée par son index de stockage. Sans argument,
         retire le dernier objet enregistre.
         """
         if item is not None:
             __index = int(item)
             self.__values.pop(__index)
             self.__tags.pop(__index)
         else:
@@ -251,41 +243,41 @@
                 allTags = {}
                 for index in __indexOfFilteredItems:
                     allTags.update( self.__tags[index] )
                 allKeys = sorted(allTags.keys())
                 return allKeys
 
     # ---------------------------------------------------------
-    # Pour compatibilite
+    # Pour compatibilité
     def stepnumber(self):
         "Nombre de pas"
         return len(self.__values)
 
-    # Pour compatibilite
+    # Pour compatibilité
     def stepserie(self, **kwargs):
         "Nombre de pas filtrés"
         __indexOfFilteredItems = self.__filteredIndexes(**kwargs)
         return __indexOfFilteredItems
 
-    # Pour compatibilite
+    # Pour compatibilité
     def steplist(self, **kwargs):
         "Nombre de pas filtrés"
         __indexOfFilteredItems = self.__filteredIndexes(**kwargs)
         return list(__indexOfFilteredItems)
 
     # ---------------------------------------------------------
     def means(self):
         """
         Renvoie la série, contenant à chaque pas, la valeur moyenne des données
         au pas. Il faut que le type de base soit compatible avec les types
         élémentaires numpy.
         """
         try:
             return [numpy.mean(item, dtype=mfp).astype('float') for item in self.__values]
-        except:
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def stds(self, ddof=0):
         """
         Renvoie la série, contenant à chaque pas, l'écart-type des données
         au pas. Il faut que le type de base soit compatible avec les types
         élémentaires numpy.
@@ -294,50 +286,152 @@
                l'écart-type, qui est dans le diviseur. Inutile avant Numpy 1.1
         """
         try:
             if numpy.version.version >= '1.1.0':
                 return [numpy.array(item).std(ddof=ddof, dtype=mfp).astype('float') for item in self.__values]
             else:
                 return [numpy.array(item).std(dtype=mfp).astype('float') for item in self.__values]
-        except:
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def sums(self):
         """
         Renvoie la série, contenant à chaque pas, la somme des données au pas.
         Il faut que le type de base soit compatible avec les types élémentaires
         numpy.
         """
         try:
             return [numpy.array(item).sum() for item in self.__values]
-        except:
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def mins(self):
         """
         Renvoie la série, contenant à chaque pas, le minimum des données au pas.
         Il faut que le type de base soit compatible avec les types élémentaires
         numpy.
         """
         try:
             return [numpy.array(item).min() for item in self.__values]
-        except:
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def maxs(self):
         """
         Renvoie la série, contenant à chaque pas, la maximum des données au pas.
         Il faut que le type de base soit compatible avec les types élémentaires
         numpy.
         """
         try:
             return [numpy.array(item).max() for item in self.__values]
-        except:
+        except Exception:
+            raise TypeError("Base type is incompatible with numpy")
+
+    def norms(self, _ord=None):
+        """
+        Norm (_ord : voir numpy.linalg.norm)
+
+        Renvoie la série, contenant à chaque pas, la norme des données au pas.
+        Il faut que le type de base soit compatible avec les types élémentaires
+        numpy.
+        """
+        try:
+            return [numpy.linalg.norm(item, _ord) for item in self.__values]
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
+    def maes(self, _predictor=None):
+        """
+        Mean Absolute Error (MAE)
+        mae(dX) = 1/n sum(dX_i)
+
+        Renvoie la série, contenant à chaque pas, la MAE des données au pas.
+        Il faut que le type de base soit compatible avec les types élémentaires
+        numpy. C'est réservé aux variables d'écarts ou d'incréments si le
+        prédicteur est None, sinon c'est appliqué à l'écart entre les données
+        au pas et le prédicteur au même pas.
+        """
+        if _predictor is None:
+            try:
+                return [numpy.mean(numpy.abs(item)) for item in self.__values]
+            except Exception:
+                raise TypeError("Base type is incompatible with numpy")
+        else:
+            if len(_predictor) != len(self.__values):
+                raise ValueError("Predictor number of steps is incompatible with the values")
+            for i, item in enumerate(self.__values):
+                if numpy.asarray(_predictor[i]).size != numpy.asarray(item).size:
+                    raise ValueError("Predictor size at step %i is incompatible with the values"%i)
+            try:
+                return [numpy.mean(numpy.abs(numpy.ravel(item) - numpy.ravel(_predictor[i]))) for i, item in enumerate(self.__values)]
+            except Exception:
+                raise TypeError("Base type is incompatible with numpy")
+
+    def mses(self, _predictor=None):
+        """
+        Mean-Square Error (MSE) ou Mean-Square Deviation (MSD)
+        mse(dX) = 1/n sum(dX_i**2)
+
+        Renvoie la série, contenant à chaque pas, la MSE des données au pas. Il
+        faut que le type de base soit compatible avec les types élémentaires
+        numpy. C'est réservé aux variables d'écarts ou d'incréments si le
+        prédicteur est None, sinon c'est appliqué à l'écart entre les données
+        au pas et le prédicteur au même pas.
+        """
+        if _predictor is None:
+            try:
+                __n = self.shape()[0]
+                return [(numpy.linalg.norm(item)**2 / __n) for item in self.__values]
+            except Exception:
+                raise TypeError("Base type is incompatible with numpy")
+        else:
+            if len(_predictor) != len(self.__values):
+                raise ValueError("Predictor number of steps is incompatible with the values")
+            for i, item in enumerate(self.__values):
+                if numpy.asarray(_predictor[i]).size != numpy.asarray(item).size:
+                    raise ValueError("Predictor size at step %i is incompatible with the values"%i)
+            try:
+                __n = self.shape()[0]
+                return [(numpy.linalg.norm(numpy.ravel(item) - numpy.ravel(_predictor[i]))**2 / __n) for i, item in enumerate(self.__values)]
+            except Exception:
+                raise TypeError("Base type is incompatible with numpy")
+
+    msds=mses # Mean-Square Deviation (MSD=MSE)
+
+    def rmses(self, _predictor=None):
+        """
+        Root-Mean-Square Error (RMSE) ou Root-Mean-Square Deviation (RMSD)
+        rmse(dX) = sqrt( 1/n sum(dX_i**2) ) = sqrt( mse(dX) )
+
+        Renvoie la série, contenant à chaque pas, la RMSE des données au pas.
+        Il faut que le type de base soit compatible avec les types élémentaires
+        numpy. C'est réservé aux variables d'écarts ou d'incréments si le
+        prédicteur est None, sinon c'est appliqué à l'écart entre les données
+        au pas et le prédicteur au même pas.
+        """
+        if _predictor is None:
+            try:
+                __n = self.shape()[0]
+                return [(numpy.linalg.norm(item) / math.sqrt(__n)) for item in self.__values]
+            except Exception:
+                raise TypeError("Base type is incompatible with numpy")
+        else:
+            if len(_predictor) != len(self.__values):
+                raise ValueError("Predictor number of steps is incompatible with the values")
+            for i, item in enumerate(self.__values):
+                if numpy.asarray(_predictor[i]).size != numpy.asarray(item).size:
+                    raise ValueError("Predictor size at step %i is incompatible with the values"%i)
+            try:
+                __n = self.shape()[0]
+                return [(numpy.linalg.norm(numpy.ravel(item) - numpy.ravel(_predictor[i])) / math.sqrt(__n)) for i, item in enumerate(self.__values)]
+            except Exception:
+                raise TypeError("Base type is incompatible with numpy")
+
+    rmsds = rmses # Root-Mean-Square Deviation (RMSD=RMSE)
+
     def __preplots(self,
                    title    = "",
                    xlabel   = "",
                    ylabel   = "",
                    ltitle   = None,
                    geometry = "600x400",
                    persist  = False,
@@ -469,76 +563,76 @@
         """
         Renvoie la moyenne sur toutes les valeurs sans tenir compte de la
         longueur des pas. Il faut que le type de base soit compatible avec
         les types élémentaires numpy.
         """
         try:
             return numpy.mean(self.__values, axis=0, dtype=mfp).astype('float')
-        except:
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def std(self, ddof=0):
         """
         Renvoie l'écart-type de toutes les valeurs sans tenir compte de la
         longueur des pas. Il faut que le type de base soit compatible avec
         les types élémentaires numpy.
 
         ddof : c'est le nombre de degrés de liberté pour le calcul de
                l'écart-type, qui est dans le diviseur. Inutile avant Numpy 1.1
         """
         try:
             if numpy.version.version >= '1.1.0':
-                return numpy.array(self.__values).std(ddof=ddof,axis=0).astype('float')
+                return numpy.asarray(self.__values).std(ddof=ddof,axis=0).astype('float')
             else:
-                return numpy.array(self.__values).std(axis=0).astype('float')
-        except:
+                return numpy.asarray(self.__values).std(axis=0).astype('float')
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def sum(self):
         """
         Renvoie la somme de toutes les valeurs sans tenir compte de la
         longueur des pas. Il faut que le type de base soit compatible avec
         les types élémentaires numpy.
         """
         try:
-            return numpy.array(self.__values).sum(axis=0)
-        except:
+            return numpy.asarray(self.__values).sum(axis=0)
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def min(self):
         """
         Renvoie le minimum de toutes les valeurs sans tenir compte de la
         longueur des pas. Il faut que le type de base soit compatible avec
         les types élémentaires numpy.
         """
         try:
-            return numpy.array(self.__values).min(axis=0)
-        except:
+            return numpy.asarray(self.__values).min(axis=0)
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def max(self):
         """
         Renvoie le maximum de toutes les valeurs sans tenir compte de la
         longueur des pas. Il faut que le type de base soit compatible avec
         les types élémentaires numpy.
         """
         try:
-            return numpy.array(self.__values).max(axis=0)
-        except:
+            return numpy.asarray(self.__values).max(axis=0)
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def cumsum(self):
         """
         Renvoie la somme cumulée de toutes les valeurs sans tenir compte de la
         longueur des pas. Il faut que le type de base soit compatible avec
         les types élémentaires numpy.
         """
         try:
-            return numpy.array(self.__values).cumsum(axis=0)
-        except:
+            return numpy.asarray(self.__values).cumsum(axis=0)
+        except Exception:
             raise TypeError("Base type is incompatible with numpy")
 
     def plot(self,
              steps    = None,
              title    = "",
              xlabel   = "",
              ylabel   = "",
@@ -623,15 +717,15 @@
         # -------------------------
         maxiter = int( 1e9 )
         if isinstance(Scheduler,int):      # Considéré comme une fréquence à partir de 0
             Schedulers = range( 0, maxiter, int(Scheduler) )
         elif isinstance(Scheduler,range):  # Considéré comme un itérateur
             Schedulers = Scheduler
         elif isinstance(Scheduler,(list,tuple)):   # Considéré comme des index explicites
-            Schedulers = [iLong(i) for i in Scheduler] # map( long, Scheduler )
+            Schedulers = [int(i) for i in Scheduler] # map( long, Scheduler )
         else:                              # Dans tous les autres cas, activé par défaut
             Schedulers = range( 0, maxiter )
         #
         # Stockage interne de l'observer dans la variable
         # -----------------------------------------------
         self.__dataobservers.append( [HookFunction, HookParameters, Schedulers] )
 
@@ -919,10 +1013,11 @@
             for k in output.keys():
                 self[k] = output[k]
         else:
             raise ValueError("Load mode '%s' unknown. Choose another one."%mode)
         #
         return filename
 
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/PlatformInfo.py` & `adao-9.9.0.1/adao/daCore/PlatformInfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -94,21 +94,26 @@
             if hasattr(platform, 'linux_distribution'):
                 __msg += "\n%s%30s : %s" %(__prefix,
                     "platform.linux_distribution",str(platform.linux_distribution()))
             elif hasattr(platform, 'dist'):
                 __msg += "\n%s%30s : %s" %(__prefix,"platform.dist",str(platform.dist()))
         elif sys.platform.startswith('darwin'):
             if hasattr(platform, 'mac_ver'):
-                __macosxv = {'5': 'Leopard',       '6': 'Snow Leopard', '7': 'Lion',
-                             '8': 'Mountain Lion', '9': 'Mavericks',   '10': 'Yosemite',
-                             '11': 'El Capitan',  '12': 'Sierra'}
+                __macosxv = {
+                    '0' : 'Cheetah',      '1' : 'Puma',        '2' : 'Jaguar',
+                    '3' : 'Panther',      '4' : 'Tiger',       '5' : 'Leopard',
+                    '6' : 'Snow Leopard', '7' : 'Lion',        '8' : 'Mountain Lion',
+                    '9' : 'Mavericks',    '10': 'Yosemite',    '11': 'El Capitan',
+                    '12': 'Sierra',       '13': 'High Sierra', '14': 'Mojave',
+                    '15': 'Catalina',     '16': 'Big Sur',     '17': 'Monterey',
+                    }
                 for key in __macosxv:
                     if (platform.mac_ver()[0].split('.')[1] == key):
                         __msg += "\n%s%30s : %s" %(__prefix,
-                            "platform.mac_ver",str(platform.mac_ver()[0]+"(" + macosx_dict[key]+")"))
+                            "platform.mac_ver",str(platform.mac_ver()[0]+"(" + __macosxv[key]+")"))
             elif hasattr(platform, 'dist'):
                 __msg += "\n%s%30s : %s" %(__prefix,"platform.dist",str(platform.dist()))
         elif os.name == 'nt':
             __msg += "\n%s%30s : %s" %(__prefix,"platform.win32_ver",platform.win32_ver()[1])
         #
         __msg += "\n"
         __msg += "\n%s%30s : %s" %(__prefix,"platform.python_implementation",platform.python_implementation())
@@ -176,14 +181,22 @@
                 nlopt.version_minor(),
                 nlopt.version_bugfix(),
                 )
         else:
             __version = "0.0.0"
         return __version
 
+    def getSdfVersion(self):
+        "Retourne la version de sdf disponible"
+        if has_sdf:
+            __version = sdf.__version__
+        else:
+            __version = "0.0.0"
+        return __version
+
     def getCurrentMemorySize(self):
         "Retourne la taille mémoire courante utilisée"
         return 1
 
     def MaximumPrecision(self):
         "Retourne la precision maximale flottante pour Numpy"
         import numpy
@@ -202,14 +215,15 @@
         #     eps = (1.0 + eps/2) - 1.0
         return sys.float_info.epsilon
 
     def __str__(self):
         import daCore.version as dav
         return "%s %s (%s)"%(dav.name,dav.version,dav.date)
 
+
 # ==============================================================================
 try:
     import scipy
     import scipy.version
     import scipy.optimize
     has_scipy = True
 except ImportError:
@@ -241,17 +255,17 @@
 
 try:
     import sdf
     has_sdf = True
 except ImportError:
     has_sdf = False
 
-has_salome = bool( "ROOT_SALOME"   in os.environ )
-has_yacs   = bool( "YACS_ROOT_DIR" in os.environ )
-has_adao   = bool( "ADAO_ROOT_DIR" in os.environ )
+has_salome = bool( "SALOME_ROOT_DIR" in os.environ )
+has_yacs   = bool(   "YACS_ROOT_DIR" in os.environ )
+has_adao   = bool(   "ADAO_ROOT_DIR" in os.environ )
 has_eficas = bool( "EFICAS_ROOT_DIR" in os.environ )
 
 # ==============================================================================
 def uniq( __sequence ):
     """
     Fonction pour rendre unique chaque élément d'une liste, en préservant l'ordre
     """
@@ -313,17 +327,17 @@
     représentation de flottants
     """
     for s in ("array", "matrix", "list", "tuple", "[", "(", "'", '"'):
         __strvect = __strvect.replace(s,"")  # Rien
     __strvect = __strvect.replace(","," ") # Blanc
     for s in ("]", ")"):
         __strvect = __strvect.replace(s,";") # "]" et ")" par ";"
-    __strvect = re.sub(';\s*;',';',__strvect)
+    __strvect = re.sub(r';\s*;',r';',__strvect)
     __strvect = __strvect.rstrip(";") # Après ^ et avant v
-    __strmat = [l.split() for l in __strvect.split(";")]
+    __strmat = [__l.split() for __l in __strvect.split(";")]
     return __strmat
 
 def checkFileNameConformity( __filename, __warnInsteadOfPrint=True ):
     if sys.platform.startswith("win") and len(__filename) > 256:
         __conform = False
         __msg = (" For some shared or older file systems on Windows, a file "+\
             "name longer than 256 characters can lead to access problems."+\
@@ -364,15 +378,15 @@
     def __init__(self):
         "Déclaration des répertoires statiques"
         parent = os.path.abspath(os.path.join(os.path.dirname(__file__),".."))
         self.__paths = {}
         self.__paths["daNumerics"]  = os.path.join(parent,"daNumerics")
         #
         for v in self.__paths.values():
-            sys.path.insert(0, v )
+            if os.path.isdir(v): sys.path.insert(0, v )
         #
         # Conserve en unique exemplaire chaque chemin
         sys.path = uniq( sys.path )
         del parent
 
     def getpaths(self):
         """
@@ -476,10 +490,11 @@
         "Renvoie la mémoire résidente maximale mesurée"
         return self._VmB('VmHWM:', unit)
     #
     def getMaxVirtualMemory(self, unit="o"):
         "Renvoie la mémoire totale maximale mesurée"
         return self._VmB('VmPeak:', unit)
 
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/Reporting.py` & `adao-9.9.0.1/adao/daCore/Reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -125,19 +125,17 @@
         return self.get()
 
     def close(self):
         del self.c
         return 0
 
 # ==============================================================================
-# Classes d'interface utilisateur : ReportStorage, ReportViewIn*
+# Classes d'interface utilisateur : ReportViewIn*, ReportStorage
 # Tags de structure : (title, h1, h2, h3, p, uli, oli, <b></b>, <i></i>)
 
-ReportStorage = __ReportC__
-
 class ReportViewInHtml(__ReportV__):
     """
     Report in HTML
     """
 
     default_filename="report.html"
     tags = {
@@ -291,10 +289,14 @@
                 if s in self.titles.keys():
                     pg += "\n%s\n%s\n%s"%(self.titles[s][0]*len(c),c,self.titles[s][1]*len(c))
                 elif s in self.tags.keys():
                     pg += "\n%s%s%s"%(self.tags[s][0],c,self.tags[s][1])
             pg += "\n"
         return pg
 
+
+# Interface utilisateur de stockage des informations
+ReportStorage = __ReportC__
+
 # ==============================================================================
 if __name__ == "__main__":
     print('\n AUTODIAGNOSTIC\n')
```

### Comparing `adao-9.8.0.2/adao/daCore/Templates.py` & `adao-9.9.0.1/adao/daCore/Templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -106,120 +106,120 @@
     content = """print(str(info)+" "+str(var[:]))""",
     fr_FR   = "Imprime sur la sortie standard la série des valeurs de la variable",
     en_EN   = "Print on standard output the value series of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueSaver",
-    content = """import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
+    content = """import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
     fr_FR   = "Enregistre la valeur courante de la variable dans un fichier du répertoire '/tmp' nommé 'value...txt' selon le nom de la variable et l'étape d'enregistrement",
     en_EN   = "Save the current value of the variable in a file of the '/tmp' directory named 'value...txt' from the variable name and the saving step",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueSerieSaver",
-    content = """import numpy, re\nv=numpy.array(var[:],  ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
+    content = """import numpy, re\nv=numpy.array(var[:], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
     fr_FR   = "Enregistre la série des valeurs de la variable dans un fichier du répertoire '/tmp' nommé 'value...txt' selon le nom de la variable et l'étape",
     en_EN   = "Save the value series of the variable in a file of the '/tmp' directory named 'value...txt' from the variable name and the saving step",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValuePrinterAndSaver",
-    content = """import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+" "+str(v))\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
+    content = """import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+" "+str(v))\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps enregistre dans un fichier du répertoire '/tmp', la valeur courante de la variable",
     en_EN   = "Print on standard output and, in the same time save in a file of the '/tmp' directory, the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueIndexPrinterAndSaver",
-    content = """import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+(" index %i:"%(len(var)-1))+" "+str(v))\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
+    content = """import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+(" index %i:"%(len(var)-1))+" "+str(v))\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps enregistre dans un fichier du répertoire '/tmp', la valeur courante de la variable, en ajoutant son index",
     en_EN   = "Print on standard output and, in the same time save in a file of the '/tmp' directory, the current value of the variable, adding its index",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueSeriePrinterAndSaver",
-    content = """import numpy, re\nv=numpy.array(var[:],  ndmin=1)\nprint(str(info)+" "+str(v))\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
+    content = """import numpy, re\nv=numpy.array(var[:], ndmin=1)\nprint(str(info)+" "+str(v))\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp', la série des valeurs de la variable",
     en_EN   = "Print on standard output and, in the same time, save in a file of the '/tmp' directory, the value series of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueGnuPlotter",
-    content = """import numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig, gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
+    content = """import numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig, gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
     fr_FR   = "Affiche graphiquement avec Gnuplot la valeur courante de la variable",
     en_EN   = "Graphically plot with Gnuplot the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueSerieGnuPlotter",
-    content = """import numpy, Gnuplot\nv=numpy.array(var[:],  ndmin=1)\nglobal ifig, gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
+    content = """import numpy, Gnuplot\nv=numpy.array(var[:], ndmin=1)\nglobal ifig, gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
     fr_FR   = "Affiche graphiquement avec Gnuplot la série des valeurs de la variable",
     en_EN   = "Graphically plot with Gnuplot the value series of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValuePrinterAndGnuPlotter",
-    content = """print(str(info)+" "+str(var[-1]))\nimport numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
+    content = """print(str(info)+' '+str(var[-1]))\nimport numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps, affiche graphiquement avec Gnuplot la valeur courante de la variable",
     en_EN   = "Print on standard output and, in the same time, graphically plot with Gnuplot the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueSeriePrinterAndGnuPlotter",
-    content = """print(str(info)+" "+str(var[:]))\nimport numpy, Gnuplot\nv=numpy.array(var[:],  ndmin=1)\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
+    content = """print(str(info)+' '+str(var[:]))\nimport numpy, Gnuplot\nv=numpy.array(var[:], ndmin=1)\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps, affiche graphiquement avec Gnuplot la série des valeurs de la variable",
     en_EN   = "Print on standard output and, in the same time, graphically plot with Gnuplot the value series of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValuePrinterSaverAndGnuPlotter",
-    content = """print(str(info)+" "+str(var[-1]))\nimport numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
+    content = """print(str(info)+' '+str(var[-1]))\nimport numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp' et affiche graphiquement la valeur courante de la variable",
     en_EN   = "Print on standard output and, in the same, time save in a file of the '/tmp' directory and graphically plot the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueSeriePrinterSaverAndGnuPlotter",
-    content = """print(str(info)+" "+str(var[:]))\nimport numpy, re\nv=numpy.array(var[:],  ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
+    content = """print(str(info)+' '+str(var[:]))\nimport numpy, re\nv=numpy.array(var[:], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )""",
     fr_FR   = "Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp' et affiche graphiquement la série des valeurs de la variable",
     en_EN   = "Print on standard output and, in the same, time save in a file of the '/tmp' directory and graphically plot the value series of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueMean",
-    content = """import numpy\nprint(str(info)+" "+str(numpy.nanmean(var[-1])))""",
+    content = """import numpy\nprint(str(info)+' '+str(numpy.nanmean(var[-1])))""",
     fr_FR   = "Imprime sur la sortie standard la moyenne de la valeur courante de la variable",
     en_EN   = "Print on standard output the mean of the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueStandardError",
-    content = """import numpy\nprint(str(info)+" "+str(numpy.nanstd(var[-1])))""",
+    content = """import numpy\nprint(str(info)+' '+str(numpy.nanstd(var[-1])))""",
     fr_FR   = "Imprime sur la sortie standard l'écart-type de la valeur courante de la variable",
     en_EN   = "Print on standard output the standard error of the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueVariance",
-    content = """import numpy\nprint(str(info)+" "+str(numpy.nanvar(var[-1])))""",
+    content = """import numpy\nprint(str(info)+' '+str(numpy.nanvar(var[-1])))""",
     fr_FR   = "Imprime sur la sortie standard la variance de la valeur courante de la variable",
     en_EN   = "Print on standard output the variance of the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueL2Norm",
-    content = """import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+" "+str(float( numpy.linalg.norm(v) )))""",
+    content = """import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+' '+str(float( numpy.linalg.norm(v) )))""",
     fr_FR   = "Imprime sur la sortie standard la norme L2 de la valeur courante de la variable",
     en_EN   = "Print on standard output the L2 norm of the current value of the variable",
     order   = "next",
     )
 ObserverTemplates.store(
     name    = "ValueRMS",
-    content = """import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+" "+str(float( numpy.sqrt((1./v.size)*numpy.dot(v,v)) )))""",
+    content = """import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+' '+str(float( numpy.sqrt((1./v.size)*numpy.dot(v,v)) )))""",
     fr_FR   = "Imprime sur la sortie standard la racine de la moyenne des carrés (RMS), ou moyenne quadratique, de la valeur courante de la variable",
     en_EN   = "Print on standard output the root mean square (RMS), or quadratic mean, of the current value of the variable",
     order   = "next",
     )
 
 # ==============================================================================
 UserPostAnalysisTemplates = TemplateStorage()
```

### Comparing `adao-9.8.0.2/adao/daCore/__init__.py` & `adao-9.9.0.1/adao/daAlgorithms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
```

### Comparing `adao-9.8.0.2/adao/daCore/version.py` & `adao-9.9.0.1/adao/daCore/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
@@ -23,13 +23,14 @@
 """
     Version
 """
 __author__ = "Jean-Philippe ARGAUD"
 __all__ = []
 
 name     = "ADAO"
-version  = "9.8.0.2"
-year     = "2021"
-date     = "dimanche 12 décembre 2021, 12:12:12 (UTC+0100)"
+version  = "9.9.0.1"
+year     = "2022"
+date     = "lundi 02 mai 2022, 12:12:12 (UTC+0100)"
 
 longname = name + ", a module for Data Assimilation and Optimization"
 cata     = "V" + version.replace(".","_")
+__version__ = version
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `adao-9.8.0.2/adao/daEficas/ADAO_Cata_V0.py` & `adao-9.9.0.1/adao/daEficas/ADAO_Cata_V0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -19,27 +19,27 @@
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
 # --------------------------------------------------------
-# Generated by AdaoCatalogGenerator on 2021-12-01 18:11:46
+# Generated by AdaoCatalogGenerator on 2022-05-30 21:42:45
 # --------------------------------------------------------
 
 import os, re
 import Accas
 from Accas import *
 
 JdC = JDC_CATA (
     code = 'ADAO',
     execmodul = None,
     regles = ( AU_MOINS_UN ('ASSIMILATION_STUDY','OPTIMIZATION_STUDY','REDUCTION_STUDY','CHECKING_STUDY'), AU_PLUS_UN ('ASSIMILATION_STUDY','OPTIMIZATION_STUDY','REDUCTION_STUDY','CHECKING_STUDY')),
     )
-VERSION_CATALOGUE='V9_8_0'
+VERSION_CATALOGUE='V9_9_0'
 
 def NoCheckInNS(filename):
     return 1
 NoCheckInNS.info = u""
 def DirectOperatorInNS(filename):
     if os.path.isfile(filename):
         fc = open(filename, 'r').readlines()
@@ -716,60 +716,60 @@
                 ValueAndIndexPrinter = BLOC (condition = " Template == 'ValueAndIndexPrinter' ",
                     ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+(\" index %i:\"%(len(var)-1))+\" \"+str(var[-1]))", fr="Imprime sur la sortie standard la valeur courante de la variable, en ajoutant son index", ang="Print on standard output the current value of the variable, adding its index" ),
                     ),
                 ValueSeriePrinter = BLOC (condition = " Template == 'ValueSeriePrinter' ",
                     ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+\" \"+str(var[:]))", fr="Imprime sur la sortie standard la série des valeurs de la variable", ang="Print on standard output the value series of the variable" ),
                     ),
                 ValueSaver = BLOC (condition = " Template == 'ValueSaver' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Enregistre la valeur courante de la variable dans un fichier du répertoire '/tmp' nommé 'value...txt' selon le nom de la variable et l'étape d'enregistrement", ang="Save the current value of the variable in a file of the '/tmp' directory named 'value...txt' from the variable name and the saving step" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Enregistre la valeur courante de la variable dans un fichier du répertoire '/tmp' nommé 'value...txt' selon le nom de la variable et l'étape d'enregistrement", ang="Save the current value of the variable in a file of the '/tmp' directory named 'value...txt' from the variable name and the saving step" ),
                     ),
                 ValueSerieSaver = BLOC (condition = " Template == 'ValueSerieSaver' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[:],  ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Enregistre la série des valeurs de la variable dans un fichier du répertoire '/tmp' nommé 'value...txt' selon le nom de la variable et l'étape", ang="Save the value series of the variable in a file of the '/tmp' directory named 'value...txt' from the variable name and the saving step" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[:], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Enregistre la série des valeurs de la variable dans un fichier du répertoire '/tmp' nommé 'value...txt' selon le nom de la variable et l'étape", ang="Save the value series of the variable in a file of the '/tmp' directory named 'value...txt' from the variable name and the saving step" ),
                     ),
                 ValuePrinterAndSaver = BLOC (condition = " Template == 'ValuePrinterAndSaver' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+\" \"+str(v))\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Imprime sur la sortie standard et, en même temps enregistre dans un fichier du répertoire '/tmp', la valeur courante de la variable", ang="Print on standard output and, in the same time save in a file of the '/tmp' directory, the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+\" \"+str(v))\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Imprime sur la sortie standard et, en même temps enregistre dans un fichier du répertoire '/tmp', la valeur courante de la variable", ang="Print on standard output and, in the same time save in a file of the '/tmp' directory, the current value of the variable" ),
                     ),
                 ValueIndexPrinterAndSaver = BLOC (condition = " Template == 'ValueIndexPrinterAndSaver' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+(\" index %i:\"%(len(var)-1))+\" \"+str(v))\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Imprime sur la sortie standard et, en même temps enregistre dans un fichier du répertoire '/tmp', la valeur courante de la variable, en ajoutant son index", ang="Print on standard output and, in the same time save in a file of the '/tmp' directory, the current value of the variable, adding its index" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[-1], ndmin=1)\nprint(str(info)+(\" index %i:\"%(len(var)-1))+\" \"+str(v))\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Imprime sur la sortie standard et, en même temps enregistre dans un fichier du répertoire '/tmp', la valeur courante de la variable, en ajoutant son index", ang="Print on standard output and, in the same time save in a file of the '/tmp' directory, the current value of the variable, adding its index" ),
                     ),
                 ValueSeriePrinterAndSaver = BLOC (condition = " Template == 'ValueSeriePrinterAndSaver' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[:],  ndmin=1)\nprint(str(info)+\" \"+str(v))\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp', la série des valeurs de la variable", ang="Print on standard output and, in the same time, save in a file of the '/tmp' directory, the value series of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, re\nv=numpy.array(var[:], ndmin=1)\nprint(str(info)+\" \"+str(v))\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)", fr="Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp', la série des valeurs de la variable", ang="Print on standard output and, in the same time, save in a file of the '/tmp' directory, the value series of the variable" ),
                     ),
                 ValueGnuPlotter = BLOC (condition = " Template == 'ValueGnuPlotter' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig, gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Affiche graphiquement avec Gnuplot la valeur courante de la variable", ang="Graphically plot with Gnuplot the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig, gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Affiche graphiquement avec Gnuplot la valeur courante de la variable", ang="Graphically plot with Gnuplot the current value of the variable" ),
                     ),
                 ValueSerieGnuPlotter = BLOC (condition = " Template == 'ValueSerieGnuPlotter' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, Gnuplot\nv=numpy.array(var[:],  ndmin=1)\nglobal ifig, gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Affiche graphiquement avec Gnuplot la série des valeurs de la variable", ang="Graphically plot with Gnuplot the value series of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy, Gnuplot\nv=numpy.array(var[:], ndmin=1)\nglobal ifig, gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Affiche graphiquement avec Gnuplot la série des valeurs de la variable", ang="Graphically plot with Gnuplot the value series of the variable" ),
                     ),
                 ValuePrinterAndGnuPlotter = BLOC (condition = " Template == 'ValuePrinterAndGnuPlotter' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+\" \"+str(var[-1]))\nimport numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, affiche graphiquement avec Gnuplot la valeur courante de la variable", ang="Print on standard output and, in the same time, graphically plot with Gnuplot the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+' '+str(var[-1]))\nimport numpy, Gnuplot\nv=numpy.array(var[-1], ndmin=1)\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, affiche graphiquement avec Gnuplot la valeur courante de la variable", ang="Print on standard output and, in the same time, graphically plot with Gnuplot the current value of the variable" ),
                     ),
                 ValueSeriePrinterAndGnuPlotter = BLOC (condition = " Template == 'ValueSeriePrinterAndGnuPlotter' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+\" \"+str(var[:]))\nimport numpy, Gnuplot\nv=numpy.array(var[:],  ndmin=1)\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, affiche graphiquement avec Gnuplot la série des valeurs de la variable", ang="Print on standard output and, in the same time, graphically plot with Gnuplot the value series of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+' '+str(var[:]))\nimport numpy, Gnuplot\nv=numpy.array(var[:], ndmin=1)\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, affiche graphiquement avec Gnuplot la série des valeurs de la variable", ang="Print on standard output and, in the same time, graphically plot with Gnuplot the value series of the variable" ),
                     ),
                 ValuePrinterSaverAndGnuPlotter = BLOC (condition = " Template == 'ValuePrinterSaverAndGnuPlotter' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+\" \"+str(var[-1]))\nimport numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp' et affiche graphiquement la valeur courante de la variable", ang="Print on standard output and, in the same, time save in a file of the '/tmp' directory and graphically plot the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+' '+str(var[-1]))\nimport numpy, re\nv=numpy.array(var[-1], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp' et affiche graphiquement la valeur courante de la variable", ang="Print on standard output and, in the same, time save in a file of the '/tmp' directory and graphically plot the current value of the variable" ),
                     ),
                 ValueSeriePrinterSaverAndGnuPlotter = BLOC (condition = " Template == 'ValueSeriePrinterSaverAndGnuPlotter' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+\" \"+str(var[:]))\nimport numpy, re\nv=numpy.array(var[:],  ndmin=1)\nglobal istep\ntry:\n    istep += 1\nexcept:\n    istep = 0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig += 1\n    gp(' set style data lines')\nexcept:\n    ifig = 0\n    gp = Gnuplot.Gnuplot(persist=1)\n    gp(' set style data lines')\ngp('set title  \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp' et affiche graphiquement la série des valeurs de la variable", ang="Print on standard output and, in the same, time save in a file of the '/tmp' directory and graphically plot the value series of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "print(str(info)+' '+str(var[:]))\nimport numpy, re\nv=numpy.array(var[:], ndmin=1)\nglobal istep\ntry:\n    istep+=1\nexcept:\n    istep=0\nf='/tmp/value_%s_%05i.txt'%(info,istep)\nf=re.sub('\s','_',f)\nprint('Value saved in \"%s\"'%f)\nnumpy.savetxt(f,v)\nimport Gnuplot\nglobal ifig,gp\ntry:\n    ifig+=1\n    gp('set style data lines')\nexcept:\n    ifig=0\n    gp=Gnuplot.Gnuplot(persist=1)\n    gp('set style data lines')\ngp('set title \"%s (Figure %i)\"'%(info,ifig))\ngp.plot( Gnuplot.Data( v, with_='lines lw 2' ) )", fr="Imprime sur la sortie standard et, en même temps, enregistre dans un fichier du répertoire '/tmp' et affiche graphiquement la série des valeurs de la variable", ang="Print on standard output and, in the same, time save in a file of the '/tmp' directory and graphically plot the value series of the variable" ),
                     ),
                 ValueMean = BLOC (condition = " Template == 'ValueMean' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nprint(str(info)+\" \"+str(numpy.nanmean(var[-1])))", fr="Imprime sur la sortie standard la moyenne de la valeur courante de la variable", ang="Print on standard output the mean of the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nprint(str(info)+' '+str(numpy.nanmean(var[-1])))", fr="Imprime sur la sortie standard la moyenne de la valeur courante de la variable", ang="Print on standard output the mean of the current value of the variable" ),
                     ),
                 ValueStandardError = BLOC (condition = " Template == 'ValueStandardError' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nprint(str(info)+\" \"+str(numpy.nanstd(var[-1])))", fr="Imprime sur la sortie standard l'écart-type de la valeur courante de la variable", ang="Print on standard output the standard error of the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nprint(str(info)+' '+str(numpy.nanstd(var[-1])))", fr="Imprime sur la sortie standard l'écart-type de la valeur courante de la variable", ang="Print on standard output the standard error of the current value of the variable" ),
                     ),
                 ValueVariance = BLOC (condition = " Template == 'ValueVariance' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nprint(str(info)+\" \"+str(numpy.nanvar(var[-1])))", fr="Imprime sur la sortie standard la variance de la valeur courante de la variable", ang="Print on standard output the variance of the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nprint(str(info)+' '+str(numpy.nanvar(var[-1])))", fr="Imprime sur la sortie standard la variance de la valeur courante de la variable", ang="Print on standard output the variance of the current value of the variable" ),
                     ),
                 ValueL2Norm = BLOC (condition = " Template == 'ValueL2Norm' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+\" \"+str(float( numpy.linalg.norm(v) )))", fr="Imprime sur la sortie standard la norme L2 de la valeur courante de la variable", ang="Print on standard output the L2 norm of the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+' '+str(float( numpy.linalg.norm(v) )))", fr="Imprime sur la sortie standard la norme L2 de la valeur courante de la variable", ang="Print on standard output the L2 norm of the current value of the variable" ),
                     ),
                 ValueRMS = BLOC (condition = " Template == 'ValueRMS' ",
-                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+\" \"+str(float( numpy.sqrt((1./v.size)*numpy.dot(v,v)) )))", fr="Imprime sur la sortie standard la racine de la moyenne des carrés (RMS), ou moyenne quadratique, de la valeur courante de la variable", ang="Print on standard output the root mean square (RMS), or quadratic mean, of the current value of the variable" ),
+                    ValueTemplate = SIMP(statut = "o", typ = "TXM", min=1, max=1, defaut = "import numpy\nv = numpy.ravel( var[-1] )\nprint(str(info)+' '+str(float( numpy.sqrt((1./v.size)*numpy.dot(v,v)) )))", fr="Imprime sur la sortie standard la racine de la moyenne des carrés (RMS), ou moyenne quadratique, de la valeur courante de la variable", ang="Print on standard output the root mean square (RMS), or quadratic mean, of the current value of the variable" ),
                     ),
                 )
 
 def F_Observers(statut) : return FACT(
     statut=statut,
     SELECTION = SIMP(statut="o", defaut=[], typ="TXM", min=0, max="**", homo="SansOrdreNiDoublon", validators=NoRepeat(), into=(['Analysis', 'Innovation', 'InnovationAtCurrentState', 'CurrentState', 'CurrentOptimum', 'IndexOfOptimum', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulatedObservationAtCurrentOptimum', 'BMA', 'OMA', 'OMB', 'CostFunctionJ', 'CostFunctionJb', 'CostFunctionJo', 'GradientOfCostFunctionJ', 'GradientOfCostFunctionJb', 'GradientOfCostFunctionJo', 'SigmaObs2', 'SigmaBck2', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'Residu'])),
     Analysis = BLOC (condition=" 'Analysis' in set(SELECTION) ",
@@ -1157,34 +1157,34 @@
     Parameters3DVAR = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == '3DVAR') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des paires de bornes"),
         CostDecrementTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-07, fr="Diminution relative minimale du coût lors de l'arrêt"),
         EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Parameters", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
         GradientNormTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-05, fr="Maximum des composantes du gradient lors de l'arrêt"),
         InitializationPoint = SIMP(statut="f", typ="TXM", fr="État initial imposé (par défaut, c'est l'ébauche si None)"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
         Minimizer = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="LBFGSB", into=['LBFGSB', 'TNC', 'CG', 'NCG', 'BFGS'], fr="Minimiseur utilisé"),
         NumberOfSamplesForQuantiles = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=100, fr="Nombre d'échantillons simulés pour le calcul des quantiles"),
         ProjectedGradientTolerance = SIMP(statut="f", typ="R", val_min=-1, min=1, max=1, defaut=-1.0, fr="Maximum des composantes du gradient projeté lors de l'arrêt"),
         Quantiles = SIMP(statut="f", typ="TXM", max="**", into=None, fr="Liste des valeurs de quantiles"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         SimulationForQuantiles = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Linear", into=['Linear', 'NonLinear'], fr="Type de simulation en estimation des quantiles"),
         StateBoundsForQuantiles = SIMP(statut="f", typ="TXM", fr="Liste des paires de bornes pour les états utilisés en estimation des quantiles"),
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'ForecastState', 'IndexOfOptimum', 'Innovation', 'InnovationAtCurrentState', 'JacobianMatrixAtBackground', 'JacobianMatrixAtOptimum', 'KalmanGainAtOptimum', 'MahalanobisConsistency', 'OMA', 'OMB', 'SampledStateForQuantiles', 'SigmaObs2', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulationQuantiles'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'CurrentStepNumber', 'ForecastState', 'IndexOfOptimum', 'Innovation', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'JacobianMatrixAtBackground', 'JacobianMatrixAtOptimum', 'KalmanGainAtOptimum', 'MahalanobisConsistency', 'OMA', 'OMB', 'SampledStateForQuantiles', 'SigmaObs2', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulationQuantiles'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="3DVAR", into=['3DVAR', '3DVAR-VAN', '3DVAR-Incr', '3DVAR-PSAS'], fr="Variant ou formulation de la méthode"),
         ),
     Parameters4DVAR = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == '4DVAR') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         ConstrainedBy = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="EstimateProjection", into=['EstimateProjection'], fr="Prise en compte des contraintes"),
         CostDecrementTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-07, fr="Diminution relative minimale du coût lors de l'arrêt"),
         EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="State", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
         GradientNormTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-05, fr="Maximum des composantes du gradient lors de l'arrêt"),
         InitializationPoint = SIMP(statut="f", typ="TXM", fr="État initial imposé (par défaut, c'est l'ébauche si None)"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
         Minimizer = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="LBFGSB", into=['LBFGSB', 'TNC', 'CG', 'NCG', 'BFGS'], fr="Minimiseur utilisé"),
         ProjectedGradientTolerance = SIMP(statut="f", typ="R", val_min=-1, min=1, max=1, defaut=-1.0, fr="Maximum des composantes du gradient projeté lors de l'arrêt"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'IndexOfOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="4DVAR", into=['4DVAR'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersAdjointTest = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'AdjointTest') ",
         statut="f",
@@ -1193,38 +1193,40 @@
         InitialDirection = SIMP(statut="f", typ="TXM", fr="Direction initiale de la dérivée directionnelle autour du point nominal"),
         ResiduFormula = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="ScalarProduct", into=['ScalarProduct'], fr="Formule de résidu utilisée"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['CurrentState', 'Residu', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersBlue = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'Blue') ",
         statut="f",
+        EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Parameters", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
         NumberOfSamplesForQuantiles = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=100, fr="Nombre d'échantillons simulés pour le calcul des quantiles"),
         Quantiles = SIMP(statut="f", typ="TXM", max="**", into=None, fr="Liste des valeurs de quantiles"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         SimulationForQuantiles = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Linear", into=['Linear', 'NonLinear'], fr="Type de simulation en estimation des quantiles"),
         StateBoundsForQuantiles = SIMP(statut="f", typ="TXM", fr="Liste des paires de bornes pour les états utilisés en estimation des quantiles"),
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'Innovation', 'MahalanobisConsistency', 'OMA', 'OMB', 'SampledStateForQuantiles', 'SigmaBck2', 'SigmaObs2', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulationQuantiles'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'CurrentStepNumber', 'ForecastState', 'Innovation', 'InnovationAtCurrentAnalysis', 'MahalanobisConsistency', 'OMA', 'OMB', 'SampledStateForQuantiles', 'SigmaBck2', 'SigmaObs2', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulationQuantiles'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Blue", into=['Blue'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersDerivativeFreeOptimization = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'DerivativeFreeOptimization') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         CostDecrementTolerance = SIMP(statut="f", typ="R", min=1, max=1, defaut=1e-07, fr="Diminution relative minimale du cout lors de l'arrêt"),
         MaximumNumberOfFunctionEvaluations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal d'évaluations de la fonction"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
         Minimizer = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="BOBYQA", into=['BOBYQA', 'COBYLA', 'NEWUOA', 'POWELL', 'SIMPLEX', 'SUBPLEX'], fr="Minimiseur utilisé"),
         QualityCriterion = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="AugmentedWeightedLeastSquares", into=['AugmentedWeightedLeastSquares', 'AWLS', 'DA', 'WeightedLeastSquares', 'WLS', 'LeastSquares', 'LS', 'L2', 'AbsoluteValue', 'L1', 'MaximumError', 'ME'], fr="Critère de qualité utilisé"),
         StateVariationTolerance = SIMP(statut="f", typ="R", min=1, max=1, defaut=0.0001, fr="Variation relative maximale de l'état lors de l'arrêt"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJb', 'CostFunctionJo', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'IndexOfOptimum', 'Innovation', 'InnovationAtCurrentState', 'OMA', 'OMB', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersDifferentialEvolution = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'DifferentialEvolution') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         CrossOverProbability_CR = SIMP(statut="f", typ="R", val_min=0.0, val_max=1.0, min=1, max=1, defaut=0.7, fr="Probabilité de recombinaison ou de croisement, notée CR"),
         MaximumNumberOfFunctionEvaluations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal d'évaluations de la fonction"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=15000, fr="Nombre maximal de générations"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=15000, fr="Nombre maximal de générations"),
         Minimizer = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="BEST1BIN", into=['BEST1BIN', 'BEST1EXP', 'BEST2BIN', 'BEST2EXP', 'RAND1BIN', 'RAND1EXP', 'RAND2BIN', 'RAND2EXP', 'RANDTOBEST1BIN', 'RANDTOBEST1EXP'], fr="Stratégie de minimisation utilisée"),
         MutationDifferentialWeight_F = SIMP(statut="f", typ="TXM", max="**", into=None, fr="Poids différentiel de mutation, constant ou aléatoire dans l'intervalle, noté F"),
         PopulationSize = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=100, fr="Taille approximative de la population à chaque génération"),
         QualityCriterion = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="AugmentedWeightedLeastSquares", into=['AugmentedWeightedLeastSquares', 'AWLS', 'DA', 'WeightedLeastSquares', 'WLS', 'LeastSquares', 'LS', 'L2', 'AbsoluteValue', 'L1', 'MaximumError', 'ME'], fr="Critère de qualité utilisé"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJb', 'CostFunctionJo', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'IndexOfOptimum', 'Innovation', 'InnovationAtCurrentState', 'OMA', 'OMB', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
@@ -1232,31 +1234,35 @@
         statut="f",
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'CurrentOptimum', 'CurrentState', 'Innovation', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersEnsembleKalmanFilter = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'EnsembleKalmanFilter') ",
         statut="f",
         EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="State", into=['State', 'Parameters'], fr="Estimation d'etat ou de parametres"),
-        HybridCovarianceEquilibrium = SIMP(statut="f", typ="R", val_min=0.0, val_max=1.0, min=1, max=1, defaut=0.5, fr="Facteur d'équilibre entre la covariance statique et la covariance d'ensemble"),
+        HybridCostDecrementTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-07, fr="Diminution relative minimale du coût lors de l'arrêt en hybride variationnel"),
+        HybridCovarianceEquilibrium = SIMP(statut="f", typ="R", val_min=0.0, val_max=1.0, min=1, max=1, defaut=0.5, fr="Facteur d'équilibre entre la covariance statique et la covariance d'ensemble en hybride variationnel"),
+        HybridMaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation en hybride variationnel"),
         InflationFactor = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1.0, fr="Facteur d'inflation"),
         InflationType = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="MultiplicativeOnAnalysisAnomalies", into=['MultiplicativeOnAnalysisAnomalies', 'MultiplicativeOnBackgroundAnomalies'], fr="Méthode d'inflation d'ensemble"),
         NumberOfMembers = SIMP(statut="f", typ="I", val_min=2, min=1, max=1, defaut=100, fr="Nombre de membres dans l'ensemble"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         SmootherLagL = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=0, fr="Nombre d'intervalles de temps de lissage dans le passé"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'ForecastCovariance', 'ForecastState', 'IndexOfOptimum', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentAnalysis', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="EnKF", into=['EnKF', 'ETKF', 'ETKF-N', 'MLEF', 'IEnKF', 'EnKS'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersExtendedBlue = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'ExtendedBlue') ",
         statut="f",
+        EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Parameters", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
         NumberOfSamplesForQuantiles = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=100, fr="Nombre d'échantillons simulés pour le calcul des quantiles"),
         Quantiles = SIMP(statut="f", typ="TXM", max="**", into=None, fr="Liste des valeurs de quantiles"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         SimulationForQuantiles = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Linear", into=['Linear', 'NonLinear'], fr="Type de simulation en estimation des quantiles"),
         StateBoundsForQuantiles = SIMP(statut="f", typ="TXM", fr="Liste des paires de bornes pour les états utilisés en estimation des quantiles"),
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'Innovation', 'MahalanobisConsistency', 'OMA', 'OMB', 'SampledStateForQuantiles', 'SigmaBck2', 'SigmaObs2', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulationQuantiles'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'CurrentStepNumber', 'ForecastState', 'Innovation', 'InnovationAtCurrentAnalysis', 'MahalanobisConsistency', 'OMA', 'OMB', 'SampledStateForQuantiles', 'SigmaBck2', 'SigmaObs2', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum', 'SimulationQuantiles'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="ExtendedBlue", into=['ExtendedBlue'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersExtendedKalmanFilter = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'ExtendedKalmanFilter') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         ConstrainedBy = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="EstimateProjection", into=['EstimateProjection'], fr="Prise en compte des contraintes"),
         EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="State", into=['State', 'Parameters'], fr="Estimation d'etat ou de parametres"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'ForecastCovariance', 'ForecastState', 'IndexOfOptimum', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentAnalysis', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
@@ -1284,20 +1290,23 @@
         NumberOfPrintedDigits = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=5, fr="Nombre de chiffres affichés pour les impressions de réels"),
         PrintAllValuesFor = SIMP(statut="f", typ="TXM", max="**", into=['Background', 'CheckingPoint', 'Observation'], fr="Liste de noms de vecteurs dont les valeurs détaillées sont à imprimer"),
         SetDebug = SIMP(statut="f", typ="I", into=(0, 1), min=1, max=1, defaut=0, fr="Activation du mode debug lors de l'exécution"),
         ShowInformationOnlyFor = SIMP(statut="f", typ="TXM", max="**", into=['Background', 'CheckingPoint', 'Observation'], fr="Liste de noms de vecteurs dont les informations synthétiques sont à imprimer"),
         ),
     ParametersKalmanFilter = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'KalmanFilter') ",
         statut="f",
-        EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="State", into=['State', 'Parameters'], fr="Estimation d'etat ou de parametres"),
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'ForecastCovariance', 'ForecastState', 'IndexOfOptimum', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentAnalysis', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="State", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'CurrentStepNumber', 'ForecastCovariance', 'ForecastState', 'IndexOfOptimum', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentAnalysis', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="KalmanFilter", into=['KalmanFilter'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersLinearLeastSquares = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'LinearLeastSquares') ",
         statut="f",
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'OMA', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Parameters", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'CurrentStepNumber', 'ForecastState', 'InnovationAtCurrentAnalysis', 'OMA', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="LinearLeastSquares", into=['LinearLeastSquares'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersLinearityTest = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'LinearityTest') ",
         statut="f",
         AmplitudeOfInitialDirection = SIMP(statut="f", typ="R", min=1, max=1, defaut=1.0, fr="Amplitude de la direction initiale de la dérivée directionnelle autour du point nominal"),
         AmplitudeOfTangentPerturbation = SIMP(statut="f", typ="R", val_min=1e-10, val_max=1.0, min=1, max=1, defaut=0.01, fr="Amplitude de la perturbation pour le calcul de la forme tangente"),
         EpsilonMinimumExponent = SIMP(statut="f", typ="I", val_min=-20, val_max=0, min=1, max=1, defaut=-8, fr="Exposant minimal en puissance de 10 pour le multiplicateur d'incrément"),
         InitialDirection = SIMP(statut="f", typ="TXM", fr="Direction initiale de la dérivée directionnelle autour du point nominal"),
@@ -1310,46 +1319,48 @@
         SetDebug = SIMP(statut="f", typ="I", into=(0, 1), min=1, max=1, defaut=0, fr="Activation du mode debug lors de l'exécution"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['CurrentState', 'JacobianMatrixAtCurrentState', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersNonLinearLeastSquares = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'NonLinearLeastSquares') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des paires de bornes"),
         CostDecrementTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-07, fr="Diminution relative minimale du coût lors de l'arrêt"),
+        EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Parameters", into=['State', 'Parameters'], fr="Estimation d'état ou de paramètres"),
         GradientNormTolerance = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1e-05, fr="Maximum des composantes du gradient lors de l'arrêt"),
         InitializationPoint = SIMP(statut="f", typ="TXM", fr="État initial imposé (par défaut, c'est l'ébauche si None)"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
         Minimizer = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="LBFGSB", into=['LBFGSB', 'TNC', 'CG', 'NCG', 'BFGS', 'LM'], fr="Minimiseur utilisé"),
         ProjectedGradientTolerance = SIMP(statut="f", typ="R", val_min=-1, min=1, max=1, defaut=-1.0, fr="Maximum des composantes du gradient projeté lors de l'arrêt"),
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'IndexOfOptimum', 'Innovation', 'InnovationAtCurrentState', 'OMA', 'OMB', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'CurrentStepNumber', 'ForecastState', 'IndexOfOptimum', 'Innovation', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'OMA', 'OMB', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="NonLinearLeastSquares", into=['NonLinearLeastSquares'], fr="Variant ou formulation de la méthode"),
         ),
     ParametersParallelFunctionTest = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'ParallelFunctionTest') ",
         statut="f",
         NumberOfPrintedDigits = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=5, fr="Nombre de chiffres affichés pour les impressions de réels"),
         NumberOfRepetition = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=1, fr="Nombre de fois où l'exécution de la fonction est répétée"),
         SetDebug = SIMP(statut="f", typ="I", into=(0, 1), min=1, max=1, defaut=0, fr="Activation du mode debug lors de l'exécution"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['CurrentState', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersParticleSwarmOptimization = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'ParticleSwarmOptimization') ",
         statut="f",
         BoxBounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes d'incréments de paramètres"),
         GroupRecallRate = SIMP(statut="f", typ="R", val_min=0.0, val_max=1.0, min=1, max=1, defaut=0.5, fr="Taux de rappel au meilleur insecte du groupe (entre 0 et 1)"),
         MaximumNumberOfFunctionEvaluations = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=15000, fr="Nombre maximal d'évaluations de la fonction"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=50, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=0, min=1, max=1, defaut=50, fr="Nombre maximal de pas d'optimisation"),
         NumberOfInsects = SIMP(statut="f", typ="I", val_min=-1, min=1, max=1, defaut=100, fr="Nombre d'insectes dans l'essaim"),
-        QualityCriterion = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="AugmentedWeightedLeastSquares", into=['DA', 'AugmentedWeightedLeastSquares', 'AWLS', 'WeightedLeastSquares', 'WLS', 'LeastSquares', 'LS', 'L2', 'AbsoluteValue', 'L1', 'MaximumError', 'ME'], fr="Critère de qualité utilisé"),
+        QualityCriterion = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="AugmentedWeightedLeastSquares", into=['AugmentedWeightedLeastSquares', 'AWLS', 'DA', 'WeightedLeastSquares', 'WLS', 'LeastSquares', 'LS', 'L2', 'AbsoluteValue', 'L1', 'MaximumError', 'ME'], fr="Critère de qualité utilisé"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJb', 'CostFunctionJo', 'CurrentIterationNumber', 'CurrentState', 'Innovation', 'OMA', 'OMB', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         SwarmVelocity = SIMP(statut="f", typ="R", val_min=0.0, min=1, max=1, defaut=1.0, fr="Vitesse de groupe imposée par l'essaim"),
         ),
     ParametersQuantileRegression = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'QuantileRegression') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         CostDecrementTolerance = SIMP(statut="f", typ="R", min=1, max=1, defaut=1e-06, fr="Maximum de variation de la fonction d'estimation lors de l'arrêt"),
         InitializationPoint = SIMP(statut="f", typ="TXM", fr="État initial imposé (par défaut, c'est l'ébauche si None)"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=15000, fr="Nombre maximal de pas d'optimisation"),
         Minimizer = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="MMQR", into=['MMQR'], fr="Minimiseur utilisé"),
         Quantile = SIMP(statut="f", typ="R", val_min=0.0, val_max=1.0, min=1, max=1, defaut=0.5, fr="Quantile pour la regression de quantile"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'BMA', 'CostFunctionJ', 'CostFunctionJb', 'CostFunctionJo', 'CurrentIterationNumber', 'CurrentState', 'Innovation', 'OMA', 'OMB', 'SimulatedObservationAtBackground', 'SimulatedObservationAtCurrentState', 'SimulatedObservationAtOptimum'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersSamplingTest = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'SamplingTest') ",
         statut="f",
         QualityCriterion = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="AugmentedWeightedLeastSquares", into=['DA', 'AugmentedWeightedLeastSquares', 'AWLS', 'WeightedLeastSquares', 'WLS', 'LeastSquares', 'LS', 'L2', 'AbsoluteValue', 'L1', 'MaximumError', 'ME'], fr="Critère de qualité utilisé"),
@@ -1361,15 +1372,15 @@
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['CostFunctionJ', 'CostFunctionJb', 'CostFunctionJo', 'CurrentState', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         ),
     ParametersTabuSearch = BLOC (condition = " (Parameters == 'Defaults') and (Algorithm == 'TabuSearch') ",
         statut="f",
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         LengthOfTabuList = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=50, fr="Longueur de la liste tabou"),
-        MaximumNumberOfSteps = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=50, fr="Nombre maximal de pas d'optimisation"),
+        MaximumNumberOfIterations = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=50, fr="Nombre maximal de pas d'optimisation"),
         NoiseAddingProbability = SIMP(statut="f", typ="R", val_min=0.0, val_max=1.0, min=1, max=1, defaut=1.0, fr="Probabilité de perturbation d'une composante de l'état"),
         NoiseDistribution = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="Uniform", into=['Gaussian', 'Uniform'], fr="Distribution pour générer les perturbations d'état"),
         NoiseHalfRange = SIMP(statut="f", typ="TXM", fr="Demi-amplitude des perturbations uniformes centrées d'état pour chaque composante de l'état"),
         NumberOfElementaryPerturbations = SIMP(statut="f", typ="I", val_min=1, min=1, max=1, defaut=1, fr="Nombre de perturbations élémentaires pour choisir une perturbation d'état"),
         QualityCriterion = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="AugmentedWeightedLeastSquares", into=['AugmentedWeightedLeastSquares', 'AWLS', 'DA', 'WeightedLeastSquares', 'WLS', 'LeastSquares', 'LS', 'L2', 'AbsoluteValue', 'L1', 'MaximumError', 'ME'], fr="Critère de qualité utilisé"),
         SetSeed = SIMP(statut="f", typ="TXM", fr="Graine fixée pour le générateur aléatoire"),
         StandardDeviation = SIMP(statut="f", typ="TXM", fr="Ecart-type des perturbations gaussiennes d'état pour chaque composante de l'état"),
@@ -1390,15 +1401,15 @@
         Alpha = SIMP(statut="f", typ="R", val_min=0.0001, val_max=1.0, min=1, max=1, defaut=1.0, fr=""),
         Beta = SIMP(statut="f", typ="R", min=1, max=1, defaut=2.0, fr=""),
         Bounds = SIMP(statut="f", typ="TXM", fr="Liste des valeurs de bornes"),
         ConstrainedBy = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="EstimateProjection", into=['EstimateProjection'], fr="Prise en compte des contraintes"),
         EstimationOf = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="State", into=['State', 'Parameters'], fr="Estimation d'etat ou de parametres"),
         Kappa = SIMP(statut="f", typ="I", val_max=2, min=1, max=1, defaut=0, fr=""),
         Reconditioner = SIMP(statut="f", typ="R", val_min=0.001, val_max=10.0, min=1, max=1, defaut=1.0, fr=""),
-        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentIterationNumber', 'CurrentOptimum', 'CurrentState', 'ForecastCovariance', 'ForecastState', 'IndexOfOptimum', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentAnalysis', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
+        StoreSupplementaryCalculations = SIMP(statut="f", typ="TXM", max="**", into=['Analysis', 'APosterioriCorrelations', 'APosterioriCovariance', 'APosterioriStandardDeviations', 'APosterioriVariances', 'BMA', 'CostFunctionJ', 'CostFunctionJAtCurrentOptimum', 'CostFunctionJb', 'CostFunctionJbAtCurrentOptimum', 'CostFunctionJo', 'CostFunctionJoAtCurrentOptimum', 'CurrentOptimum', 'CurrentState', 'ForecastCovariance', 'ForecastState', 'IndexOfOptimum', 'InnovationAtCurrentAnalysis', 'InnovationAtCurrentState', 'SimulatedObservationAtCurrentAnalysis', 'SimulatedObservationAtCurrentOptimum', 'SimulatedObservationAtCurrentState'], fr="Liste de calculs supplémentaires à stocker et/ou effectuer"),
         Variant = SIMP(statut="f", typ="TXM", min=1, max=1, defaut="2UKF", into=['UKF', '2UKF'], fr="Variant ou formulation de la méthode"),
         ),
     )
 
 def F_variables(statut) : return FACT(
     statut=statut,
     regles = ( MEME_NOMBRE ('NAMES', 'SIZES')),
```

### Comparing `adao-9.8.0.2/adao/daEficas/__init__.py` & `adao-9.9.0.1/adao/daEficas/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daEficas/configuration_ADAO.py` & `adao-9.9.0.1/adao/daEficas/configuration_ADAO.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -23,16 +23,15 @@
 # Author: André Ribes, andre.ribes@edf.fr, EDF R&D
 
 """
     Ce module sert pour charger les paramètres de configuration d'EFICAS
 """
 # Modules Python
 # print "passage dans la surcharge de configuration pour Adao"
-import os, sys, string, types, re
-import traceback
+import os
 from PyQt5.QtGui  import *
 
 # Modules Eficas
 from InterfaceQT4 import configuration
 
 # Classe de base permettant de lire, afficher
 # et sauvegarder les fichiers utilisateurs
```

### Comparing `adao-9.8.0.2/adao/daEficas/convert_adao.py` & `adao-9.9.0.1/adao/daEficas/convert_adao.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daEficas/generator_adao.py` & `adao-9.9.0.1/adao/daEficas/generator_adao.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -19,15 +19,14 @@
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: André Ribes, andre.ribes@edf.fr, EDF R&D
 
 from generator.generator_python import PythonGenerator
-import traceback
 import logging
 
 def entryPoint():
    """
       Retourne les informations necessaires pour le chargeur de plugins
 
       Ces informations sont retournees dans un dictionnaire
@@ -65,15 +64,15 @@
       self.text_da_status = False
       self.generate_da()
       self.text_da_status = True
     except:
       self.logger.debug("EFICAS case is not valid, python command file for YACS schema generation cannot be created")
       self.logger.debug(self.text_da)
       self.dictMCVal = {}
-      # traceback.print_exc()
+      # import traceback ; traceback.print_exc()
     return self.text_comm
 
   def writeDefault(self, fn):
     if self.text_da_status:
       self.logger.debug("write adao python command file")
       filename = fn[:fn.rfind(".")] + '.py'
       #~ f = open( str(filename), 'wb')
```

### Comparing `adao-9.8.0.2/adao/daEficas/prefs.py` & `adao-9.9.0.1/adao/daEficas/prefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daEficas/prefs_ADAO.py` & `adao-9.9.0.1/adao/daEficas/prefs_ADAO.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV7_4_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV7_4_0ToV9_9_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -58,15 +58,15 @@
     elif texte is not None:
         jdc  = getJDCFromTexte(texte,atraiter)
     else:
         raise ValueError("Traduction du JDC impossible")
 
     #Parse les mocles des commandes
     parseKeywords(jdc.root)
-    GenereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
+    genereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
     # ==========================================================================
 
     for command in atraiter:
         # Insere le MC s'il n'existe pas
         chercheOperInsereFacteurSiRegle(jdc, command, "AlgorithmParameters",((("AlgorithmParameters",),"nexistepasMCFParmi"),))
         # Deplace le MC
         moveMotClefInOperToFact(jdc, command, "Algorithm", "AlgorithmParameters", plusieursFois=False)
@@ -74,14 +74,15 @@
         renameMotCleInFact(jdc, command, "AlgorithmParameters", "INPUT_TYPE", "Parameters")
         # Renomme le MC
         renameMotCle(jdc, command, "Study_name", "StudyName")
         renameMotCle(jdc, command, "Study_repertory", "StudyRepertory")
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "FunctionDict", "ScriptWithSwitch", fsrc )
     fsrc = re.sub( "FUNCTIONDICT_FILE", "SCRIPTWITHSWITCH_FILE", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV7_5_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV7_5_0ToV9_9_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -58,15 +58,15 @@
     elif texte is not None:
         jdc  = getJDCFromTexte(texte,atraiter)
     else:
         raise ValueError("Traduction du JDC impossible")
 
     #Parse les mocles des commandes
     parseKeywords(jdc.root)
-    GenereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
+    genereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
     # ==========================================================================
 
     for command in atraiter:
         # Insere le MC s'il n'existe pas
         chercheOperInsereFacteurSiRegle(jdc, command, "AlgorithmParameters",((("AlgorithmParameters",),"nexistepasMCFParmi"),))
         # Deplace le MC
         moveMotClefInOperToFact(jdc, command, "Algorithm", "AlgorithmParameters", plusieursFois=False)
@@ -74,14 +74,15 @@
         renameMotCleInFact(jdc, command, "AlgorithmParameters", "INPUT_TYPE", "Parameters")
         # Renomme le MC
         renameMotCle(jdc, command, "Study_name", "StudyName")
         renameMotCle(jdc, command, "Study_repertory", "StudyRepertory")
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "FunctionDict", "ScriptWithSwitch", fsrc )
     fsrc = re.sub( "FUNCTIONDICT_FILE", "SCRIPTWITHSWITCH_FILE", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV7_5_1ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV7_5_1ToV9_9_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -58,15 +58,15 @@
     elif texte is not None:
         jdc  = getJDCFromTexte(texte,atraiter)
     else:
         raise ValueError("Traduction du JDC impossible")
 
     #Parse les mocles des commandes
     parseKeywords(jdc.root)
-    GenereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
+    genereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
     # ==========================================================================
 
     for command in atraiter:
         # Insere le MC s'il n'existe pas
         chercheOperInsereFacteurSiRegle(jdc, command, "AlgorithmParameters",((("AlgorithmParameters",),"nexistepasMCFParmi"),))
         # Deplace le MC
         moveMotClefInOperToFact(jdc, command, "Algorithm", "AlgorithmParameters", plusieursFois=False)
@@ -74,14 +74,15 @@
         renameMotCleInFact(jdc, command, "AlgorithmParameters", "INPUT_TYPE", "Parameters")
         # Renomme le MC
         renameMotCle(jdc, command, "Study_name", "StudyName")
         renameMotCle(jdc, command, "Study_repertory", "StudyRepertory")
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "FunctionDict", "ScriptWithSwitch", fsrc )
     fsrc = re.sub( "FUNCTIONDICT_FILE", "SCRIPTWITHSWITCH_FILE", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV7_6_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV7_6_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV7_7_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV7_7_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV7_8_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV7_8_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV8_1_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV8_1_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV8_2_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV8_2_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV8_3_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV8_3_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV8_4_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV8_4_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV8_5_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV8_5_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV8_6_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV8_6_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV9_2_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV9_2_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV9_3_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV9_3_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV9_4_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV9_4_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV9_5_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV9_5_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV9_6_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV9_6_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOV9_7_0ToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOV9_7_0ToV9_9_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -56,14 +56,15 @@
     else:
         raise ValueError("Traduction du JDC impossible")
     # ==========================================================================
 
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
         with open(outfile,'w') as f:
             f.write( fsrc )
```

### Comparing `adao-9.8.0.2/adao/daEficas/traduitADAOsansToV9_8_0.py` & `adao-9.9.0.1/adao/daEficas/traduitADAOsansToV9_9_0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#-*- coding: utf-8 -*-
+# -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2018 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -16,27 +16,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
 #
 # Author: Jean-Philippe Argaud, jean-philippe.argaud@edf.fr, EDF R&D
 
-import argparse
+import argparse # optparse deprecated since Python version 3.2
 import sys
 import re
 
 import Traducteur.log as log
 from Traducteur.load         import getJDC, getJDCFromTexte
 from Traducteur.mocles       import parseKeywords
-from Traducteur.dictErreurs  import GenereErreurPourCommande
+from Traducteur.dictErreurs  import genereErreurPourCommande
 from Traducteur.inseremocle  import *
 from Traducteur.movemocle    import *
 from Traducteur.renamemocle  import *
 
-version_out = "V9_8_0"
+version_out = "V9_9_0"
 
 usage="""Usage: python %(prog)s [args]
 
 Typical use is:
   python %(prog)s --infile=xxxx.comm --outfile=yyyy.comm"""
 
 atraiter = (
@@ -58,15 +58,15 @@
     elif texte is not None:
         jdc  = getJDCFromTexte(texte,atraiter)
     else:
         raise ValueError("Traduction du JDC impossible")
 
     #Parse les mocles des commandes
     parseKeywords(jdc.root)
-    GenereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
+    genereErreurPourCommande(jdc,('Algorithm','AlgorithmParameters','FunctionDict'))
     # ==========================================================================
 
     for command in atraiter:
         # Insere le MC s'il n'existe pas
         chercheOperInsereFacteurSiRegle(jdc, command, "AlgorithmParameters",((("AlgorithmParameters",),"nexistepasMCFParmi"),))
         # Deplace le MC
         moveMotClefInOperToFact(jdc, command, "Algorithm", "AlgorithmParameters", plusieursFois=False)
@@ -74,14 +74,15 @@
         renameMotCleInFact(jdc, command, "AlgorithmParameters", "INPUT_TYPE", "Parameters")
         # Renomme le MC
         renameMotCle(jdc, command, "Study_name", "StudyName")
         renameMotCle(jdc, command, "Study_repertory", "StudyRepertory")
 
     # ==========================================================================
     fsrc = jdc.getSource()
+    fsrc = re.sub( "MaximumNumberOfSteps", "MaximumNumberOfIterations", fsrc )
     fsrc = re.sub( "FunctionDict", "ScriptWithSwitch", fsrc )
     fsrc = re.sub( "FUNCTIONDICT_FILE", "SCRIPTWITHSWITCH_FILE", fsrc )
     fsrc = re.sub( "#VERSION_CATALOGUE:.*:FIN VERSION_CATALOGUE", "#VERSION_CATALOGUE:%s:FIN VERSION_CATALOGUE"%version_out, fsrc)
     fsrc = re.sub( "#CHECKSUM.*FIN CHECKSUM", "", fsrc )
     #
     log.ferme(hdlr)
     if outfile is not None:
```

### Comparing `adao-9.8.0.2/adao/daEficasWrapper/__init__.py` & `adao-9.9.0.1/adao/daEficasWrapper/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daEficasWrapper/adaoEficasWrapper.py` & `adao-9.9.0.1/adao/daEficasWrapper/adaoEficasWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daGUI/ADAO.py` & `adao-9.9.0.1/adao/daGUI/ADAO.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -21,14 +21,15 @@
 # See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 # Author: André Ribes, andre.ribes@edf.fr, EDF R&D
 
 import ADAO_COMPONENT__POA
 import SALOME_ComponentPy
 import SALOME_DriverPy
+import SALOME_Embedded_NamingService_ClientPy
 
 from daUtils.adaoLogger import *
 
 class ADAO(ADAO_COMPONENT__POA.ADAO_ENGINE,
            SALOME_ComponentPy.SALOME_ComponentPy_i,
            SALOME_DriverPy.SALOME_DriverPy_i):
   """
@@ -42,11 +43,18 @@
       interfaceName ):
     debug("Creating ADAO component instance", "ENGINE")
     SALOME_ComponentPy.SALOME_ComponentPy_i.__init__(self, orb, poa,
         contID, containerName, instanceName, interfaceName)
     SALOME_DriverPy.SALOME_DriverPy_i.__init__(self, interfaceName)
 
     # On stocke dans l'attribut _naming_service, une ref sur le Naming Service
-    self._naming_service = SALOME_ComponentPy.SALOME_NamingServicePy_i( self._orb )
+    #
+    emb_ns = self._contId.get_embedded_NS_if_ssl()
+    import CORBA
+    if CORBA.is_nil(emb_ns):
+        self._naming_service = SALOME_ComponentPy.SALOME_NamingServicePy_i( self._orb )
+    else:
+        self._naming_service = SALOME_Embedded_NamingService_ClientPy.SALOME_Embedded_NamingService_ClientPy(emb_ns)
+    #
 
   def print_ping():
     info("ADAO ENGINE Ping", "ENGINE")
```

### Comparing `adao-9.8.0.2/adao/daGUI/ADAOGUI.py` & `adao-9.9.0.1/adao/daGUI/ADAOGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daGUI/__init__.py` & `adao-9.9.0.1/adao/daCore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/ADAOGUI_impl.py` & `adao-9.9.0.1/adao/daGuiImpl/ADAOGUI_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/__init__.py` & `adao-9.9.0.1/adao/daGuiImpl/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/adaoCase.py` & `adao-9.9.0.1/adao/daGuiImpl/adaoCase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -71,14 +71,16 @@
         rtn = ""
         if (self.filename == "" or self.filename == "not yet defined"):
             return "You need to save your case before exporting it."
 
         self.yacs_filename = self.filename[:self.filename.rfind(".")] + '.xml'
         yacs_filename_backup = self.filename[:self.filename.rfind(".")] + '.xml.back'
         if os.path.exists(self.yacs_filename):
+            if os.path.exists(yacs_filename_backup):
+                os.unlink(yacs_filename_backup)
             os.rename(self.yacs_filename, yacs_filename_backup)
 
         self.eficas_editor.modified = True
         self.eficas_editor.saveFile()
         filename = self.filename[:self.filename.rfind(".")] + '.py'
         retry = 0
         while (not os.path.exists(filename) and retry < 30):
@@ -108,15 +110,17 @@
     def exportTUIFile(self):
         if (self.filename == "" or self.filename == "not yet defined"):
           return "You need to save your case before exporting it."
 
         self.tui_filename = self.filename[:self.filename.rfind(".")] + '_TUI.py'
         tui_filename_backup = self.filename[:self.filename.rfind(".")] + '_TUI.py.back'
         if os.path.exists(self.tui_filename):
-          os.rename(self.tui_filename, tui_filename_backup)
+            if os.path.exists(tui_filename_backup):
+                os.unlink(tui_filename_backup)
+            os.rename(self.tui_filename, tui_filename_backup)
 
         self.eficas_editor.modified = True
         self.eficas_editor.saveFile()
         #
         import adaoBuilder
         fullcase = adaoBuilder.New()
         rtn = fullcase.convert(FileNameFrom=self.filename, FormaterFrom="COM",
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/adaoGuiHelper.py` & `adao-9.9.0.1/adao/daGuiImpl/adaoGuiHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/adaoGuiManager.py` & `adao-9.9.0.1/adao/daGuiImpl/adaoGuiManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/adaoModuleHelper.py` & `adao-9.9.0.1/adao/daGuiImpl/adaoModuleHelper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # -*- coding: utf-8 -*-
+#
+# Copyright (C) 2008-2022 EDF R&D
+#
 # Copyright (C) 2007-2008  CEA/DEN, EDF R&D, OPEN CASCADE
 #
 # Copyright (C) 2003-2007  OPEN CASCADE, EADS/CCR, LIP6, CEA/DEN,
 # CEDRAT, EDF R&D, LEG, PRINCIPIA R&D, BUREAU VERITAS
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
@@ -25,26 +28,27 @@
     "moduleID",
     "objectID",
     "unknownID",
     "componentName",
     "modulePixmap",
     "verbose",
     "getORB",
-    "getNS",
     "getLCC",
     "getStudyManager",
     "getEngine",
     "getEngineIOR",
     "findOrCreateComponent",
     "getObjectID",
     ]
 
+import os
 from omniORB import CORBA
 from SALOME_NamingServicePy import SALOME_NamingServicePy_i
 from LifeCycleCORBA import LifeCycleCORBA
+import salome
 import SALOMEDS
 import SALOMEDS_Attributes_idl
 from salome.kernel.studyedit import getStudyEditor
 
 #import OMA_ORB
 
 ###
@@ -115,55 +119,31 @@
             pass
         pass
     return __verbose__
 
 ###
 # Get ORB reference
 ###
-__orb__ = None
 def getORB():
-    global __orb__
-    if __orb__ is None:
-        __orb__ = CORBA.ORB_init( [''], CORBA.ORB_ID )
-        pass
-    return __orb__
-
-###
-# Get naming service instance
-###
-__naming_service__ = None
-def getNS():
-    global __naming_service__
-    if __naming_service__ is None:
-        __naming_service__ = SALOME_NamingServicePy_i( getORB() )
-        pass
-    return __naming_service__
+    salome.salome_init()
+    return salome.orb
 
 ##
 # Get life cycle CORBA instance
 ##
-__lcc__ = None
 def getLCC():
-    global __lcc__
-    if __lcc__ is None:
-        __lcc__ = LifeCycleCORBA( getORB() )
-        pass
-    return __lcc__
+    salome.salome_init()
+    return salome.lcc
 
 ##
 # Get study manager
 ###
-__study_manager__ = None
 def getStudyManager():
-    global __study_manager__
-    if __study_manager__ is None:
-        obj = getNS().Resolve( '/myStudyManager' )
-        __study_manager__ = obj._narrow( SALOMEDS.StudyManager )
-        pass
-    return __study_manager__
+    salome.salome_init()
+    return salome.myStudy
 
 ###
 # Get OMA engine
 ###
 __engine__ = None
 def getEngine():
     global __engine__
```

### Comparing `adao-9.8.0.2/adao/daGuiImpl/adaoStudyEditor.py` & `adao-9.9.0.1/adao/daGuiImpl/adaoStudyEditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daNumerics/__init__.py` & `adao-9.9.0.1/adao/daGUI/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
 #
 # This library is distributed in the hope that it will be useful,
```

### Comparing `adao-9.8.0.2/adao/daUtils/__init__.py` & `adao-9.9.0.1/adao/daUtils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daUtils/adaoEficasEvent.py` & `adao-9.9.0.1/adao/daUtils/adaoEficasEvent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daUtils/adaoLogger.py` & `adao-9.9.0.1/adao/daUtils/adaoLogger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daUtils/enumerate.py` & `adao-9.9.0.1/adao/daUtils/enumerate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2007-2008  CEA/DEN, EDF R&D, OPEN CASCADE
 #
-#  Copyright (C) 2003-2007  OPEN CASCADE, EADS/CCR, LIP6, CEA/DEN,
-#  CEDRAT, EDF R&D, LEG, PRINCIPIA R&D, BUREAU VERITAS
+# Copyright (C) 2008-2022 EDF R&D
 #
-#  This library is free software; you can redistribute it and/or
-#  modify it under the terms of the GNU Lesser General Public
-#  License as published by the Free Software Foundation; either
-#  version 2.1 of the License.
-#
-#  This library is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public
-#  License along with this library; if not, write to the Free Software
-#  Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
+# Copyright (C) 2007-2008  CEA/DEN, EDF R&D, OPEN CASCADE
 #
-#  See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
+# Copyright (C) 2003-2007  OPEN CASCADE, EADS/CCR, LIP6, CEA/DEN,
+# CEDRAT, EDF R&D, LEG, PRINCIPIA R&D, BUREAU VERITAS
+#
+# This library is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 2.1 of the License.
+#
+# This library is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307 USA
+#
+# See http://www.salome-platform.org/ or email : webmaster.salome@opencascade.com
 #
 
 __author__ = "gboulant"
 __date__ = "$1 avr. 2010 09:08:02$"
 
 class Enumerate(object):
     """
```

### Comparing `adao-9.8.0.2/adao/daYacsIntegration/__init__.py` & `adao-9.9.0.1/adao/daYacsIntegration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsIntegration/daOptimizerLoop.py` & `adao-9.9.0.1/adao/daYacsIntegration/daOptimizerLoop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*-coding:utf-8-*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsIntegration/daStudy.py` & `adao-9.9.0.1/adao/daYacsIntegration/daStudy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*-coding:utf-8-*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsSchemaCreator/__init__.py` & `adao-9.9.0.1/adao/daYacsSchemaCreator/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsSchemaCreator/help_methods.py` & `adao-9.9.0.1/adao/daYacsSchemaCreator/help_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsSchemaCreator/infos_daComposant.py` & `adao-9.9.0.1/adao/daYacsSchemaCreator/infos_daComposant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsSchemaCreator/methods.py` & `adao-9.9.0.1/adao/daYacsSchemaCreator/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
```

### Comparing `adao-9.8.0.2/adao/daYacsSchemaCreator/run.py` & `adao-9.9.0.1/adao/daYacsSchemaCreator/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Copyright (C) 2008-2021 EDF R&D
+# Copyright (C) 2008-2022 EDF R&D
 #
 # This file is part of SALOME ADAO module
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License.
@@ -32,15 +32,16 @@
 
 def create_schema(config_file, config_content, yacs_schema_filename):
 
     if config_file is not None and config_content is None:
       # Import config_file
       try:
         (fd, filename) = tempfile.mkstemp()
-        exec(compile(open(config_file).read(), filename, 'exec'))
+        with open(config_file, 'r') as fid:
+            exec(compile(fid.read(), filename, 'exec'))
       except Exception as e:
         if isinstance(e, SyntaxError): msg = "at %s: %s"%(e.offset, e.text)
         else: msg = ""
         raise ValueError("\n\nexception in loading %s\n\nThe following error occurs:\n\n%s %s\n\nSee also the potential messages, which can show the origin of the above error, in the launching terminal.\n"%(config_file,str(e),msg))
     elif config_file is None and config_content is not None:
       # Import config_content
       try:
```

### Comparing `adao-9.8.0.2/adao.egg-info/PKG-INFO` & `adao-9.9.0.1/adao.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: adao
-Version: 9.8.0.2
+Version: 9.9.0.1
 Summary: A module for Data Assimilation and Optimization
 Home-page: http://www.salome-platform.org/
 Author: Jean-Philippe Argaud
 Author-email: jean-philippe.argaud@edf.fr
 License: GNU Library or Lesser General Public License (LGPL)
 Keywords: optimization,data assimilation,calibration,interpolation,inverse problem,tunning,minimization,black-box,checking,3D-Var,4D-Var,Filtering,Kalman,Ensemble,EnKF,UKF,BLUE,Regression,Quantile,V&V,Tabu Search,DFO,Derivative Free Optimization,PSO,Particle Swarm Optimization,Swarm,Gradient Test,Adjoint Test
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: COPYING.txt
 
 =====================================================
 ADAO: A module for Data Assimilation and Optimization
 =====================================================
 
@@ -36,20 +35,20 @@
 information coming from experimental measurements or observations, and from
 numerical *a priori* models, including information about their errors. Parts of
 the framework are also known under the names of *calibration*, *adjustment*,
 *state estimation*, *parameter estimation*, *parameter adjustment*, *inverse
 problems*, *Bayesian estimation*, *optimal interpolation*, *mathematical
 regularization*, *meta-heuristics for optimization*, *model reduction*, *data
 smoothing*, etc. More details can be found in the full ADAO documentation (see
-https://www.salome-platform.org/).
+https://www.salome-platform.org/ User Documentation dedicated section).
 
 Only the use of ADAO text programming interface (API/TUI) is introduced
 here. This interface gives ability to create a calculation object in a
 similar way than the case building obtained through the graphical
-interface (GUI). When one wants to elaborate "by hand" the TUI
+interface (GUI). When one wants to elaborate directly the TUI
 calculation case, it is recommended to extensively use all the ADAO
 module documentation, and to go back if necessary to the graphical
 interface (GUI), to get all the elements allowing to correctly set the
 commands.
 
 A simple setup example of an ADAO TUI calculation case
 ------------------------------------------------------
@@ -93,15 +92,15 @@
 ------------------------
 
 The license for this module is the GNU Lesser General Public License
 (Lesser GPL), as stated here and in the source files::
 
     <ADAO, a module for Data Assimilation and Optimization>
 
-    Copyright (C) 2008-2021 EDF R&D
+    Copyright (C) 2008-2022 EDF R&D
 
     This library is free software; you can redistribute it and/or
     modify it under the terms of the GNU Lesser General Public
     License as published by the Free Software Foundation; either
     version 2.1 of the License, or (at your option) any later version.
 
     This library is distributed in the hope that it will be useful,
@@ -111,25 +110,22 @@
 
     You should have received a copy of the GNU Lesser General Public
     License along with this library; if not, write to the Free Software
     Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
     See http://www.salome-platform.org/
 
-In addition, it is requested that any publication or presentation describing
+In addition, it is requested that any publication or presentation, describing
 work using this module, or any commercial or non-commercial product using it,
-cite at least one of at least one of the references below with the current year
-added:
+cite at least one of the references below with the current year added:
 
     * *ADAO, a module for Data Assimilation and Optimization*,
       http://www.salome-platform.org/
 
     * *ADAO, un module pour l'Assimilation de Données et l'Aide à
       l'Optimisation*, http://www.salome-platform.org/
 
     * *SALOME The Open Source Integration Platform for Numerical Simulation*,
       http://www.salome-platform.org/
 
 The documentation of the module is also covered by the license and the
 requirement of quoting.
-
-
```

### Comparing `adao-9.8.0.2/adao.egg-info/SOURCES.txt` & `adao-9.9.0.1/adao.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -32,15 +32,36 @@
 adao/daAlgorithms/ParticleSwarmOptimization.py
 adao/daAlgorithms/QuantileRegression.py
 adao/daAlgorithms/SamplingTest.py
 adao/daAlgorithms/TabuSearch.py
 adao/daAlgorithms/TangentTest.py
 adao/daAlgorithms/UnscentedKalmanFilter.py
 adao/daAlgorithms/__init__.py
-adao/daAlgorithms/lbfgsbhlt.py
+adao/daAlgorithms/Atoms/__init__.py
+adao/daAlgorithms/Atoms/c2ukf.py
+adao/daAlgorithms/Atoms/cekf.py
+adao/daAlgorithms/Atoms/ecwblue.py
+adao/daAlgorithms/Atoms/ecwexblue.py
+adao/daAlgorithms/Atoms/ecwlls.py
+adao/daAlgorithms/Atoms/ecwnlls.py
+adao/daAlgorithms/Atoms/ecwstdkf.py
+adao/daAlgorithms/Atoms/enks.py
+adao/daAlgorithms/Atoms/etkf.py
+adao/daAlgorithms/Atoms/exkf.py
+adao/daAlgorithms/Atoms/ienkf.py
+adao/daAlgorithms/Atoms/incr3dvar.py
+adao/daAlgorithms/Atoms/lbfgsbhlt.py
+adao/daAlgorithms/Atoms/mlef.py
+adao/daAlgorithms/Atoms/mmqr.py
+adao/daAlgorithms/Atoms/psas3dvar.py
+adao/daAlgorithms/Atoms/senkf.py
+adao/daAlgorithms/Atoms/std3dvar.py
+adao/daAlgorithms/Atoms/std4dvar.py
+adao/daAlgorithms/Atoms/uskf.py
+adao/daAlgorithms/Atoms/van3dvar.py
 adao/daCore/Aidsm.py
 adao/daCore/AssimilationStudy.py
 adao/daCore/BasicObjects.py
 adao/daCore/ExtendedLogging.py
 adao/daCore/Interfaces.py
 adao/daCore/NumericObjects.py
 adao/daCore/Persistence.py
@@ -52,33 +73,34 @@
 adao/daEficas/ADAO_Cata_V0.py
 adao/daEficas/__init__.py
 adao/daEficas/configuration_ADAO.py
 adao/daEficas/convert_adao.py
 adao/daEficas/generator_adao.py
 adao/daEficas/prefs.py
 adao/daEficas/prefs_ADAO.py
-adao/daEficas/traduitADAOV7_4_0ToV9_8_0.py
-adao/daEficas/traduitADAOV7_5_0ToV9_8_0.py
-adao/daEficas/traduitADAOV7_5_1ToV9_8_0.py
-adao/daEficas/traduitADAOV7_6_0ToV9_8_0.py
-adao/daEficas/traduitADAOV7_7_0ToV9_8_0.py
-adao/daEficas/traduitADAOV7_8_0ToV9_8_0.py
-adao/daEficas/traduitADAOV8_1_0ToV9_8_0.py
-adao/daEficas/traduitADAOV8_2_0ToV9_8_0.py
-adao/daEficas/traduitADAOV8_3_0ToV9_8_0.py
-adao/daEficas/traduitADAOV8_4_0ToV9_8_0.py
-adao/daEficas/traduitADAOV8_5_0ToV9_8_0.py
-adao/daEficas/traduitADAOV8_6_0ToV9_8_0.py
-adao/daEficas/traduitADAOV9_2_0ToV9_8_0.py
-adao/daEficas/traduitADAOV9_3_0ToV9_8_0.py
-adao/daEficas/traduitADAOV9_4_0ToV9_8_0.py
-adao/daEficas/traduitADAOV9_5_0ToV9_8_0.py
-adao/daEficas/traduitADAOV9_6_0ToV9_8_0.py
-adao/daEficas/traduitADAOV9_7_0ToV9_8_0.py
-adao/daEficas/traduitADAOsansToV9_8_0.py
+adao/daEficas/traduitADAOV7_4_0ToV9_9_0.py
+adao/daEficas/traduitADAOV7_5_0ToV9_9_0.py
+adao/daEficas/traduitADAOV7_5_1ToV9_9_0.py
+adao/daEficas/traduitADAOV7_6_0ToV9_9_0.py
+adao/daEficas/traduitADAOV7_7_0ToV9_9_0.py
+adao/daEficas/traduitADAOV7_8_0ToV9_9_0.py
+adao/daEficas/traduitADAOV8_1_0ToV9_9_0.py
+adao/daEficas/traduitADAOV8_2_0ToV9_9_0.py
+adao/daEficas/traduitADAOV8_3_0ToV9_9_0.py
+adao/daEficas/traduitADAOV8_4_0ToV9_9_0.py
+adao/daEficas/traduitADAOV8_5_0ToV9_9_0.py
+adao/daEficas/traduitADAOV8_6_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_2_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_3_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_4_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_5_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_6_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_7_0ToV9_9_0.py
+adao/daEficas/traduitADAOV9_8_0ToV9_9_0.py
+adao/daEficas/traduitADAOsansToV9_9_0.py
 adao/daEficasWrapper/__init__.py
 adao/daEficasWrapper/adaoEficasWrapper.py
 adao/daGUI/ADAO.py
 adao/daGUI/ADAOGUI.py
 adao/daGUI/__init__.py
 adao/daGuiImpl/ADAOGUI_impl.py
 adao/daGuiImpl/__init__.py
```

### Comparing `adao-9.8.0.2/setup.py` & `adao-9.9.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,27 @@
     long_description = f.read()
 
 setup(
     name = "adao",
     packages = [
         "adao",
         "adao/daAlgorithms",
+        "adao/daAlgorithms/Atoms",
         "adao/daCore",
         "adao/daEficas",
         "adao/daEficasWrapper",
         "adao/daGUI",
         "adao/daGuiImpl",
         "adao/daNumerics",
         "adao/daUtils",
         "adao/daYacsIntegration",
         "adao/daYacsSchemaCreator",
         ],
     install_requires=['numpy','scipy'],
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     version = version,
     description = "A module for Data Assimilation and Optimization",
     author = "Jean-Philippe Argaud",
     author_email = "jean-philippe.argaud@edf.fr",
     url = "http://www.salome-platform.org/",
     license = "GNU Library or Lesser General Public License (LGPL)",
     # download_url = "",
```

