# Comparing `tmp/libmata-0.73.0.tar.gz` & `tmp/libmata-0.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.73.0.tar", last modified: Fri Jun 23 12:42:46 2023, max compression
+gzip compressed data, was "libmata-0.74.0.tar", last modified: Sun Jul  2 11:59:47 2023, max compression
```

## Comparing `libmata-0.73.0.tar` & `libmata-0.74.0.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-23 12:42:46.186757 libmata-0.73.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)  1893893 2023-06-23 12:39:33.032893 libmata-0.73.0/libmata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-23 12:38:19.064168 libmata-0.73.0/libmata.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    69672 2023-06-23 12:38:19.064168 libmata-0.73.0/libmata.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.158757 libmata-0.73.0/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.158757 libmata-0.73.0/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-06-23 12:38:19.004168 libmata-0.73.0/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-06-23 12:38:19.008168 libmata-0.73.0/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.158757 libmata-0.73.0/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.166757 libmata-0.73.0/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.178758 libmata-0.73.0/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-23 12:38:19.036168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-23 12:38:19.040168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.178758 libmata-0.73.0/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.178758 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-23 12:38:19.044168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-06-23 12:38:19.048168 libmata-0.73.0/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.150757 libmata-0.73.0/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.150757 libmata-0.73.0/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.166757 libmata-0.73.0/mata/3rdparty/cudd-min/
--rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/bnet.c
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/bnet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/chkMterm.c
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-23 12:38:19.012168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-23 12:38:19.016168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-23 12:38:19.020168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-23 12:38:19.024168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/dddmpUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/epdInt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.150757 libmata-0.73.0/mata/3rdparty/cudd-min/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.150757 libmata-0.73.0/mata/3rdparty/cudd-min/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.166757 libmata-0.73.0/mata/3rdparty/cudd-min/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/ntr.c
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/ntr.h
--rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/ntrBddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/ntrHeap.c
--rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-06-23 12:38:19.028168 libmata-0.73.0/mata/3rdparty/cudd-min/ntrMflow.c
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/ntrShort.c
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/ntrZddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/st.h
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testdddmp.c
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testmtr.c
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testobj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/testst.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-23 12:38:19.032168 libmata-0.73.0/mata/3rdparty/cudd-min/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.182757 libmata-0.73.0/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-06-23 12:38:19.052168 libmata-0.73.0/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.154757 libmata-0.73.0/mata/3rdparty/simlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.154757 libmata-0.73.0/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.154757 libmata-0.73.0/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-23 12:38:19.056168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-06-23 12:38:19.060168 libmata-0.73.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-23 12:42:46.014756 libmata-0.73.0/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-23 12:42:46.014756 libmata-0.73.0/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 12:42:46.014756 libmata-0.73.0/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.154757 libmata-0.73.0/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/include/mata/
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/alphabet.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/nfa-algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/nfa-plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/nfa-strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)    44896 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/re2parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/sparse-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/include/mata/util.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    38796 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/nfa/nfa-complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/nfa/nfa-inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-23 12:38:19.072168 libmata-0.73.0/mata/src/nfa/nfa-universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76372 2023-06-23 12:38:19.076168 libmata-0.73.0/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-23 12:38:19.076168 libmata-0.73.0/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31762 2023-06-23 12:38:19.076168 libmata-0.73.0/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:42:46.186757 libmata-0.73.0/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-23 12:38:19.076168 libmata-0.73.0/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-23 12:38:19.076168 libmata-0.73.0/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-23 12:38:19.076168 libmata-0.73.0/mata/src/strings/nfa-strings.cc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 12:38:19.064168 libmata-0.73.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-23 12:38:19.064168 libmata-0.73.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.346329 libmata-0.74.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-02 11:59:47.346329 libmata-0.74.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)  1893893 2023-07-02 11:57:24.423067 libmata-0.74.0/libmata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-07-02 11:56:37.023137 libmata-0.74.0/libmata.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    69672 2023-07-02 11:56:37.023137 libmata-0.74.0/libmata.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.330329 libmata-0.74.0/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.330329 libmata-0.74.0/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-02 11:56:36.975136 libmata-0.74.0/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-02 11:56:36.979136 libmata-0.74.0/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.330329 libmata-0.74.0/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.338329 libmata-0.74.0/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.338329 libmata-0.74.0/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-02 11:56:37.003136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-02 11:56:37.007136 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.338329 libmata-0.74.0/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-02 11:56:37.011137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-02 11:56:37.015137 libmata-0.74.0/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.338329 libmata-0.74.0/mata/3rdparty/cudd-min/
+-rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/bnet.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/bnet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/chkMterm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-02 11:56:36.983136 libmata-0.74.0/mata/3rdparty/cudd-min/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-02 11:56:36.987136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-02 11:56:36.991136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/dddmpUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-02 11:56:36.995136 libmata-0.74.0/mata/3rdparty/cudd-min/epdInt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/cudd-min/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/cudd-min/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.338329 libmata-0.74.0/mata/3rdparty/cudd-min/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntrBddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntrHeap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntrMflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntrShort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ntrZddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testdddmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testmtr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testobj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/testst.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-02 11:56:36.999136 libmata-0.74.0/mata/3rdparty/cudd-min/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/simlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-02 11:56:37.019137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-02 11:56:37.023137 libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.342329 libmata-0.74.0/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-02 11:56:37.023137 libmata-0.74.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-02 11:59:47.238333 libmata-0.74.0/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-02 11:59:47.238333 libmata-0.74.0/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 11:59:47.238333 libmata-0.74.0/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.326329 libmata-0.74.0/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.346329 libmata-0.74.0/mata/include/mata/
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/alphabet.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/nfa-algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/nfa-plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/nfa-strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    46004 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/re2parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/sparse-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-02 11:56:37.027137 libmata-0.74.0/mata/include/mata/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/include/mata/util.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.346329 libmata-0.74.0/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.346329 libmata-0.74.0/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    38796 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.346329 libmata-0.74.0/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/nfa/nfa-complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/nfa/nfa-concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/nfa/nfa-inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/nfa/nfa-intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/nfa/nfa-universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    78503 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31762 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:59:47.346329 libmata-0.74.0/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-02 11:56:37.031137 libmata-0.74.0/mata/src/strings/nfa-strings.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 11:56:37.023137 libmata-0.74.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-02 11:56:37.023137 libmata-0.74.0/setup.py
```

### Comparing `libmata-0.73.0/PKG-INFO` & `libmata-0.74.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.73.0
+Version: 0.74.0
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
```

### Comparing `libmata-0.73.0/libmata.cpp` & `libmata-0.74.0/libmata.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/libmata.pxd` & `libmata-0.74.0/libmata.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/libmata.pyx` & `libmata-0.74.0/libmata.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/args.hxx` & `libmata-0.74.0/mata/3rdparty/args.hxx`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/catch.hpp` & `libmata-0.74.0/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.74.0/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.74.0/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.74.0/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.74.0/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/LICENSE` & `libmata-0.74.0/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/README` & `libmata-0.74.0/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.74.0/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.74.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.74.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.74.0/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.74.0/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.74.0/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.74.0/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.74.0/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.74.0/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.74.0/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.74.0/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.74.0/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.74.0/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/groups.dox` & `libmata-0.74.0/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.74.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.74.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.74.0/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.74.0/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.74.0/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.74.0/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.74.0/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.74.0/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/st/st.c` & `libmata-0.74.0/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/st/st.h` & `libmata-0.74.0/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/st/testst.c` & `libmata-0.74.0/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.74.0/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.74.0/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd/util/util.h` & `libmata-0.74.0/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/bnet.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/bnet.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/bnet.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/bnet.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/chkMterm.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/chkMterm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/config.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/config.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cpu_stats.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cpu_time.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cstringstream.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cstringstream.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cudd.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAPI.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddAbs.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddApply.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddFind.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddInv.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddIte.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddNeg.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAddWalsh.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAndAbs.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddAnneal.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddApa.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddApprox.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddBddAbs.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddBddCorr.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddBddIte.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddBridge.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddCache.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddCheck.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddClip.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddCof.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddCompose.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddDecomp.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddEssent.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddExact.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddExport.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddGenCof.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddGenetic.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddGroup.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddHarwell.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddInit.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddInt.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddInteract.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddLCache.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddLevelQ.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddLinear.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddLiteral.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddMatMult.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddObj.cc` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddObj.hh` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddPriority.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddRead.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddRef.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddReorder.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSat.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSign.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSolve.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSplit.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSubsetHB.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSubsetSP.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddSymmetry.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddTable.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddUtil.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddWindow.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddCount.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddFuncs.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddGroup.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddIsop.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddLin.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddMisc.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddPort.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddReord.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddSetop.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddSymm.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/cuddZddUtil.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/datalimit.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmp.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpBinary.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpConvert.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpDbg.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpInt.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpLoad.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/dddmpUtil.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/epd.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/epd.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/epdInt.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh` & `libmata-0.74.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/main.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/main.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/mtr.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/mtrBasic.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/mtrGroup.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/mtrInt.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntr.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntr.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntrBddTest.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntrBddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntrHeap.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntrHeap.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntrMflow.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntrMflow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntrShort.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntrShort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ntrZddTest.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ntrZddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/pathsearch.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/pipefork.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/prtime.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/safe_mem.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/st.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/st.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/strsav.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testcudd.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testdddmp.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testextra.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testmtr.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testmulti.cc` & `libmata-0.74.0/mata/3rdparty/cudd-min/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testobj.cc` & `libmata-0.74.0/mata/3rdparty/cudd-min/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/testst.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/texpand.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/ucbqsort.c` & `libmata-0.74.0/mata/3rdparty/cudd-min/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/cudd-min/util.h` & `libmata-0.74.0/mata/3rdparty/cudd-min/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.74.0/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/LICENSE` & `libmata-0.74.0/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/prog.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/re2.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.74.0/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.74.0/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/util/logging.h` & `libmata-0.74.0/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/util/mutex.h` & `libmata-0.74.0/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/util/rune.cc` & `libmata-0.74.0/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.74.0/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/util/utf.h` & `libmata-0.74.0/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/re2/util/util.h` & `libmata-0.74.0/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.74.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.74.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/LICENSE` & `libmata-0.74.0/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/README.md` & `libmata-0.74.0/mata/README.md`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/afa.hh` & `libmata-0.74.0/mata/include/mata/afa.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/alphabet.hh` & `libmata-0.74.0/mata/include/mata/alphabet.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/closed-set.hh` & `libmata-0.74.0/mata/include/mata/closed-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/inter-aut.hh` & `libmata-0.74.0/mata/include/mata/inter-aut.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/mintermization.hh` & `libmata-0.74.0/mata/include/mata/mintermization.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/nfa-algorithms.hh` & `libmata-0.74.0/mata/include/mata/nfa-algorithms.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/nfa-plumbing.hh` & `libmata-0.74.0/mata/include/mata/nfa-plumbing.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/nfa-strings.hh` & `libmata-0.74.0/mata/include/mata/nfa-strings.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/nfa.hh` & `libmata-0.74.0/mata/include/mata/nfa.hh`

 * *Files 2% similar despite different names*

```diff
@@ -288,14 +288,46 @@
     /**
      * Check whether automaton contains no transitions.
      * @return True if there are no transitions in the automaton, false otherwise.
      */
     bool empty() const;
 
     /**
+     * @brief Append post vector to the delta.
+     * 
+     * @param post_vector Vector of posts to be appended.
+     */
+    void append(const std::vector<Post>& post_vector) {
+        for(const Post& pst : post_vector) {
+            this->posts.push_back(pst);
+        }
+    }
+
+    /**
+     * @brief Copy posts of delta and apply a lambda update function on each state from 
+     * targets. 
+     * 
+     * IMPORTANT: In order to work properly, the lambda function needs to be 
+     * monotonic. 
+     * 
+     * @param lambda Monotonic lambda function mapping states to different states
+     * @return std::vector<Post> Copied posts.
+     */
+    std::vector<Post> transform(const std::function<State(State)>& lambda) const;
+
+    /**
+     * @brief Add transitions to multiple destinations
+     * 
+     * @param state_from From
+     * @param symbol Symbol
+     * @param states Set of states to
+     */
+    void add(const State state_from, const Symbol symbol, const StateSet& states);
+
+    /**
      * Iterator over transitions. It iterates over triples (lhs, symbol, rhs) where lhs and rhs are states.
      */
     struct const_iterator {
     private:
         const std::vector<Post>& post;
         size_t current_state;
         Post::const_iterator post_iterator{};
@@ -523,14 +555,19 @@
 
     /**
      * Remove epsilon transitions from the automaton.
      */
     void remove_epsilon(Symbol epsilon = EPSILON);
 
     /**
+     * @brief In-place concatenation.
+     */
+    Mata::Nfa::Nfa& concatenate(const Mata::Nfa::Nfa& aut);
+
+    /**
      * @brief Get a number of transitions in the whole automaton.
      *
      * The operation has constant time complexity.
      */
     size_t get_num_of_trans() const { return static_cast<size_t>(std::distance(delta.begin(), delta.end())); }
 
     /**
```

### Comparing `libmata-0.73.0/mata/include/mata/number-predicate.hh` & `libmata-0.74.0/mata/include/mata/number-predicate.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/ord-vector.hh` & `libmata-0.74.0/mata/include/mata/ord-vector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,16 @@
 
         assert(vectorIsSorted());
     }
 
     virtual void insert(const OrdVector& vec) {
         assert(vectorIsSorted());
         assert(vec.vectorIsSorted());
+
+        // TODO: sometimes it is not efficient to copy both vectors to create a new one
         vec_ = OrdVector::Union(*this, vec).vec_;
         assert(vectorIsSorted());
     }
 
     inline void clear() { vec_.clear(); }
 
     virtual inline size_t size() const { return vec_.size(); }
```

### Comparing `libmata-0.73.0/mata/include/mata/parser.hh` & `libmata-0.74.0/mata/include/mata/parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/re2parser.hh` & `libmata-0.74.0/mata/include/mata/re2parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/sparse-set.hh` & `libmata-0.74.0/mata/include/mata/sparse-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/synchronized-iterator.hh` & `libmata-0.74.0/mata/include/mata/synchronized-iterator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/include/mata/util.hh` & `libmata-0.74.0/mata/include/mata/util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/afa/afa.cc` & `libmata-0.74.0/mata/src/afa/afa.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/alphabet.cc` & `libmata-0.74.0/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/inter-aut.cc` & `libmata-0.74.0/mata/src/inter-aut.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/mintermization.cc` & `libmata-0.74.0/mata/src/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/nfa/nfa-complement.cc` & `libmata-0.74.0/mata/src/nfa/nfa-complement.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/nfa/nfa-concatenation.cc` & `libmata-0.74.0/mata/src/nfa/nfa-concatenation.cc`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,51 @@
 namespace Mata::Nfa {
 
 Nfa concatenate(const Nfa& lhs, const Nfa& rhs, bool use_epsilon,
                 StateToStateMap* lhs_result_states_map, StateToStateMap* rhs_result_states_map) {
     return Algorithms::concatenate_eps(lhs, rhs, EPSILON, use_epsilon, lhs_result_states_map, rhs_result_states_map);
 }
 
+Nfa& Nfa::concatenate(const Nfa& aut) {
+    size_t n = this->size();
+    auto upd_fnc = [&](State st) {
+        return st + n;
+    };
+
+    this->delta.append(aut.delta.transform(upd_fnc));
+
+    // set accepting states
+    Util::SparseSet<State> new_fin{};
+    new_fin.reserve(n+aut.size());
+    for(const State& aut_fin : aut.final) {
+        new_fin.insert(upd_fnc(aut_fin));
+    }
+
+    // connect both parts
+    for(const State& ini : aut.initial) {
+        const Post& ini_post = this->delta[upd_fnc(ini)];
+        // is ini state also final?
+        bool is_final = aut.final[ini];
+        for(const State& fin : this->final) {
+            if(is_final) {
+                new_fin.insert(fin);
+            }
+            for(const Move& ini_mv : ini_post) {
+                // TODO: this should be done efficiently in a delta method
+                // TODO: in fact it is not efficient for now
+                for(const State& dest : ini_mv.targets) {
+                    this->delta.add(fin, ini_mv.symbol, dest);
+                }
+            }
+        }
+    }
+    this->final = new_fin;
+    return *this;
+}
+
 Nfa Algorithms::concatenate_eps(const Nfa& lhs, const Nfa& rhs, const Symbol& epsilon, bool use_epsilon,
                 StateToStateMap* lhs_result_states_map, StateToStateMap* rhs_result_states_map) {
     // Compute concatenation of given automata.
     // Concatenation will proceed in the order of the passed automata: Result is 'lhs . rhs'.
 
     if (lhs.size() == 0 || rhs.size() == 0 || lhs.initial.empty() || lhs.final.empty() ||
         rhs.initial.empty() || rhs.final.empty()) {
```

### Comparing `libmata-0.73.0/mata/src/nfa/nfa-inclusion.cc` & `libmata-0.74.0/mata/src/nfa/nfa-inclusion.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/nfa/nfa-intersection.cc` & `libmata-0.74.0/mata/src/nfa/nfa-intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/nfa/nfa-universal.cc` & `libmata-0.74.0/mata/src/nfa/nfa-universal.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/nfa/nfa.cc` & `libmata-0.74.0/mata/src/nfa/nfa.cc`

 * *Files 1% similar despite different names*

```diff
@@ -316,24 +316,55 @@
     if (state_transitions.empty()) {
         state_transitions.insert({ symbol, state_to });
     } else if (state_transitions.back().symbol < symbol) {
         state_transitions.insert({ symbol, state_to });
     } else {
         const auto symbol_transitions{ state_transitions.find(Move{ symbol }) };
         if (symbol_transitions != state_transitions.end()) {
-            // Add transition with symbolOnTransition already used on transitions from stateFrom.
+            // Add transition with symbol already used on transitions from state_from.
             symbol_transitions->insert(state_to);
         } else {
-            // Add transition to a new Move struct with symbolOnTransition yet unused on transitions from stateFrom.
+            // Add transition to a new Move struct with symbol yet unused on transitions from state_from.
             const Move new_symbol_transitions{ symbol, state_to };
             state_transitions.insert(new_symbol_transitions);
         }
     }
 }
 
+void Delta::add(const State state_from, const Symbol symbol, const StateSet& states) {
+    if(states.empty()) {
+        return;
+    }
+
+    const State max_state{ std::max(state_from, states.back()) };
+    if (max_state >= posts.size()) {
+        reserve_on_insert(posts, max_state + 1);
+        posts.resize(max_state + 1);
+    }
+
+    Post& state_transitions{ posts[state_from] };
+
+    if (state_transitions.empty()) {
+        state_transitions.insert({ symbol, states });
+    } else if (state_transitions.back().symbol < symbol) {
+        state_transitions.insert({ symbol, states });
+    } else {
+        const auto symbol_transitions{ state_transitions.find(symbol) };
+        if (symbol_transitions != state_transitions.end()) {
+            // Add transition with symbolOnTransition already used on transitions from state_from.
+            symbol_transitions->insert(states);
+
+        } else {
+            // Add transition to a new Move struct with symbol yet unused on transitions from state_from.
+            // Move new_symbol_transitions{ symbol, states };
+            state_transitions.insert(Move{symbol, states});
+        }
+    }
+}
+
 void Delta::remove(State src, Symbol symb, State tgt) {
     if (src >= posts.size()) {
         return;
     }
 
     Post& state_transitions{ posts[src] };
     if (state_transitions.empty()) {
@@ -468,14 +499,33 @@
                     max = m.targets.back();
         }
         src++;
     }
     return max;
 }
 
+std::vector<Post> Delta::transform(const std::function<State(State)>& lambda) const {
+    std::vector<Post> cp_post_vector;
+    cp_post_vector.reserve(num_of_states());
+    for(const Post& act_post: this->posts) {
+        Post cp_post;
+        cp_post.reserve(act_post.size());
+        for(const Move& mv : act_post) {
+            StateSet cp_dest;
+            cp_dest.reserve(mv.size());
+            for(const State& state : mv.targets) {
+                cp_dest.push_back(std::move(lambda(state)));
+            }
+            cp_post.push_back(std::move(Move(mv.symbol, cp_dest)));
+        }
+        cp_post_vector.emplace_back(cp_post);
+    }
+    return cp_post_vector;
+}
+
 Post& Delta::get_mutable_post(State q) {
     if (q >= posts.size()) {
         Util::reserve_on_insert(posts, q);
         const size_t new_size{ q + 1 };
         posts.resize(new_size);
     }
 
@@ -2234,16 +2284,23 @@
         symbol = rhs.symbol;
         targets = std::move(rhs.targets);
     }
     return *this;
 }
 
 void Move::insert(State s) {
-    if (targets.find(s) == targets.end()) {
-        targets.insert(s);
+    if(targets.empty() || targets.back() < s) {
+        targets.push_back(s);
+        return;
+    }
+    // Find the place where to put the element (if not present).
+    // insert to OrdVector without the searching of a proper position inside insert(const Key&x).
+    auto it = std::lower_bound(targets.begin(), targets.end(), s);
+    if (it == targets.end() || *it != s) {
+        targets.insert(it, s);
     }
 }
 
 void Move::insert(const StateSet& states) {
     for (State s : states) {
         insert(s);
     }
```

### Comparing `libmata-0.73.0/mata/src/parser.cc` & `libmata-0.74.0/mata/src/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/re2parser.cc` & `libmata-0.74.0/mata/src/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/strings/nfa-noodlification.cc` & `libmata-0.74.0/mata/src/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/strings/nfa-segmentation.cc` & `libmata-0.74.0/mata/src/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/mata/src/strings/nfa-strings.cc` & `libmata-0.74.0/mata/src/strings/nfa-strings.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.73.0/setup.py` & `libmata-0.74.0/setup.py`

 * *Files identical despite different names*

