# Comparing `tmp/klujax-0.1.4.tar.gz` & `tmp/klujax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klujax-0.1.4.tar", last modified: Thu Jun  1 17:42:29 2023, max compression
+gzip compressed data, was "klujax-0.2.0.tar", last modified: Sun Jul  2 02:34:02 2023, max compression
```

## Comparing `klujax-0.1.4.tar` & `klujax-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:42:29.206645 klujax-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)    24478 2023-06-01 17:41:20.000000 klujax-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-01 17:42:29.206645 klujax-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-06-01 17:41:20.000000 klujax-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-06-01 17:41:20.000000 klujax-0.1.4/klujax.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 17:42:29.206645 klujax-0.1.4/klujax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-01 17:42:29.000000 klujax-0.1.4/klujax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12146 2023-06-01 17:41:20.000000 klujax-0.1.4/klujax.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-01 17:41:20.000000 klujax-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 17:42:29.206645 klujax-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-06-01 17:41:20.000000 klujax-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.437111 klujax-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    24478 2023-07-02 02:32:37.000000 klujax-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-02 02:32:37.000000 klujax-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-07-02 02:34:02.437111 klujax-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-02 02:32:37.000000 klujax-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-07-02 02:32:37.000000 klujax-0.2.0/klujax.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.425111 klujax-0.2.0/klujax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-07-02 02:34:02.000000 klujax-0.2.0/klujax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-07-02 02:34:02.000000 klujax-0.2.0/klujax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 02:34:02.000000 klujax-0.2.0/klujax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-02 02:34:02.000000 klujax-0.2.0/klujax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-02 02:34:02.000000 klujax-0.2.0/klujax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12146 2023-07-02 02:32:37.000000 klujax-0.2.0/klujax.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-02 02:32:37.000000 klujax-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-02 02:34:02.437111 klujax-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-07-02 02:32:37.000000 klujax-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.425111 klujax-0.2.0/suitesparse/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.421111 klujax-0.2.0/suitesparse/AMD/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.425111 klujax-0.2.0/suitesparse/AMD/Include/
+-rw-r--r--   0 runner    (1001) docker     (122)    16891 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Include/amd.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Include/amd_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.429111 klujax-0.2.0/suitesparse/AMD/Source/
+-rw-r--r--   0 runner    (1001) docker     (122)     5560 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_1.c
+-rw-r--r--   0 runner    (1001) docker     (122)    64602 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_2.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4703 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_aat.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_control.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4825 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_dump.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4129 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_info.c
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l1.c
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l2.c
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_aat.c
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_control.c
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_dump.c
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_info.c
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_order.c
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_post_tree.c
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_postorder.c
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_preprocess.c
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_l_valid.c
+-rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_order.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3543 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_post_tree.c
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_postorder.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_preprocess.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2829 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/AMD/Source/amd_valid.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.421111 klujax-0.2.0/suitesparse/BTF/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.429111 klujax-0.2.0/suitesparse/BTF/Include/
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Include/btf.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Include/btf_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.429111 klujax-0.2.0/suitesparse/BTF/Source/
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Source/btf_l_maxtrans.c
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Source/btf_l_order.c
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Source/btf_l_strongcomp.c
+-rw-r--r--   0 runner    (1001) docker     (122)    16012 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Source/btf_maxtrans.c
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Source/btf_order.c
+-rw-r--r--   0 runner    (1001) docker     (122)    24232 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/BTF/Source/btf_strongcomp.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.421111 klujax-0.2.0/suitesparse/COLAMD/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.429111 klujax-0.2.0/suitesparse/COLAMD/Include/
+-rw-r--r--   0 runner    (1001) docker     (122)     9315 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/COLAMD/Include/colamd.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.429111 klujax-0.2.0/suitesparse/COLAMD/Source/
+-rw-r--r--   0 runner    (1001) docker     (122)   107235 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/COLAMD/Source/colamd.c
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-02 02:33:38.000000 klujax-0.2.0/suitesparse/COLAMD/Source/colamd_l.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.421111 klujax-0.2.0/suitesparse/KLU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.433112 klujax-0.2.0/suitesparse/KLU/Include/
+-rw-r--r--   0 runner    (1001) docker     (122)    29300 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Include/klu.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6737 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Include/klu_internal.h
+-rw-r--r--   0 runner    (1001) docker     (122)    20029 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Include/klu_version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.437111 klujax-0.2.0/suitesparse/KLU/Source/
+-rw-r--r--   0 runner    (1001) docker     (122)    24595 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu.c
+-rw-r--r--   0 runner    (1001) docker     (122)    16949 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_analyze.c
+-rw-r--r--   0 runner    (1001) docker     (122)    11831 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_analyze_given.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (122)    16891 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_diagnostics.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4779 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_dump.c
+-rw-r--r--   0 runner    (1001) docker     (122)     8240 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_extract.c
+-rw-r--r--   0 runner    (1001) docker     (122)    18902 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_factor.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_free_numeric.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_free_symbolic.c
+-rw-r--r--   0 runner    (1001) docker     (122)    34399 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_kernel.c
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l.c
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_analyze.c
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_analyze_given.c
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_diagnostics.c
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_dump.c
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_extract.c
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_factor.c
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_free_numeric.c
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_free_symbolic.c
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_kernel.c
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_memory.c
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_refactor.c
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_scale.c
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_solve.c
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_sort.c
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_l_tsolve.c
+-rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_memory.c
+-rw-r--r--   0 runner    (1001) docker     (122)    17270 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_refactor.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4846 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_scale.c
+-rw-r--r--   0 runner    (1001) docker     (122)    13446 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_solve.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_sort.c
+-rw-r--r--   0 runner    (1001) docker     (122)    15880 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_tsolve.c
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z.c
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_diagnostics.c
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_dump.c
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_extract.c
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_factor.c
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_free_numeric.c
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_kernel.c
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_refactor.c
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_scale.c
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_solve.c
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_sort.c
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_z_tsolve.c
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl.c
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_diagnostics.c
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_dump.c
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_extract.c
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_factor.c
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_free_numeric.c
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_kernel.c
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_refactor.c
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_scale.c
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_solve.c
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_sort.c
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/KLU/Source/klu_zl_tsolve.c
+-rw-r--r--   0 runner    (1001) docker     (122)    53240 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 02:34:02.437111 klujax-0.2.0/suitesparse/SuiteSparse_config/
+-rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/SuiteSparse_config/SuiteSparse_config.c
+-rw-r--r--   0 runner    (1001) docker     (122)    58533 2023-07-02 02:33:39.000000 klujax-0.2.0/suitesparse/SuiteSparse_config/SuiteSparse_config.h
```

### Comparing `klujax-0.1.4/LICENSE` & `klujax-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klujax-0.1.4/PKG-INFO` & `klujax-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klujax
-Version: 0.1.4
+Version: 0.2.0
 Summary: a KLU solver for JAX
 Home-page: https://github.com/flaport/klujax
 Author: Floris Laporte
 Author-email: floris.laporte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
@@ -59,30 +59,32 @@
 ```
 [ True True True True True]
 [1. 2. 3. 4. 5.]
 ```
 
 ## Installation
 
-The library is dynamically linked to the SuiteSparse C++ library. The easiest way to
-install is as follows:
+The library is statically linked to the SuiteSparse C++ library. It can be installed on
+most platforms as follows:
 
 ```bash
-conda install pybind11 suitesparse
 pip install klujax
 ```
 
 **There exist pre-built wheels for Linux and Windows (python 3.8+).** If no compatible
 wheel is found, however, pip will attempt to install the library from source... make
 sure you have the necessary build dependencies installed.
 
 ### Linux
 
-On linux, having `gcc` and `g++` available in your path should be sufficient to be able
-to build the library from source.
+On linux, you'll need `gcc` and `g++`. Then just do a normal pip install:
+
+```sh
+pip install klujax
+```
 
 ### Windows
 
 On Windows, installing from source is a bit more involved as typically the build
 dependencies are not installed. To install those, download Visual Studio Community 2017
 from [here](https://my.visualstudio.com/Downloads?q=visual%20studio%202017&wt.mc_id=o~msft~vscom~older-downloads). During installation, go to Workloads and select the following workloads:
 
@@ -93,25 +95,31 @@
 
 - C++/CLI support
 - VC++ 2015.3 v14.00 (v140) toolset for desktop
 
 Then, download and install Microsoft Visual C++ Redistributable from [here](https://aka.ms/vs/16/release/vc_redist.x64.exe).
 
 After these installation steps, run the following commands inside a x64 Native Tools
-Command Prompt for VS 2017, after activating your conda environment:
+Command Prompt for VS 2017:
 
 ```
 set DISTUTILS_USE_SDK=1
-conda install pybind11 suitesparse
 pip install klujax
 ```
 
 ## License & Credits
 
 © Floris Laporte 2022, LGPL-2.1
 
 This library was partly based on:
 
 - [torch_sparse_solve](https://github.com/flaport/torch_sparse_solve), LGPL-2.1
 - [SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse), LGPL-2.1
 - [kagami-c/PyKLU](https://github.com/kagami-c/PyKLU), LGPL-2.1
 - [scipy.sparse](https://github.com/scipy/scipy/tree/master/scipy/sparse), BSD-3
+
+This library vendors an unmodified version of the
+[SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse) libraries in its source
+(.tar.gz) distribution to allow for static linking.
+This is in accordance with their
+[LGPL licence](https://github.com/DrTimothyAldenDavis/SuiteSparse/blob/dev/LICENSE.txt).
+
```

### Comparing `klujax-0.1.4/README.md` & `klujax-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -43,30 +43,32 @@
 ```
 [ True True True True True]
 [1. 2. 3. 4. 5.]
 ```
 
 ## Installation
 
-The library is dynamically linked to the SuiteSparse C++ library. The easiest way to
-install is as follows:
+The library is statically linked to the SuiteSparse C++ library. It can be installed on
+most platforms as follows:
 
 ```bash
-conda install pybind11 suitesparse
 pip install klujax
 ```
 
 **There exist pre-built wheels for Linux and Windows (python 3.8+).** If no compatible
 wheel is found, however, pip will attempt to install the library from source... make
 sure you have the necessary build dependencies installed.
 
 ### Linux
 
-On linux, having `gcc` and `g++` available in your path should be sufficient to be able
-to build the library from source.
+On linux, you'll need `gcc` and `g++`. Then just do a normal pip install:
+
+```sh
+pip install klujax
+```
 
 ### Windows
 
 On Windows, installing from source is a bit more involved as typically the build
 dependencies are not installed. To install those, download Visual Studio Community 2017
 from [here](https://my.visualstudio.com/Downloads?q=visual%20studio%202017&wt.mc_id=o~msft~vscom~older-downloads). During installation, go to Workloads and select the following workloads:
 
@@ -77,25 +79,31 @@
 
 - C++/CLI support
 - VC++ 2015.3 v14.00 (v140) toolset for desktop
 
 Then, download and install Microsoft Visual C++ Redistributable from [here](https://aka.ms/vs/16/release/vc_redist.x64.exe).
 
 After these installation steps, run the following commands inside a x64 Native Tools
-Command Prompt for VS 2017, after activating your conda environment:
+Command Prompt for VS 2017:
 
 ```
 set DISTUTILS_USE_SDK=1
-conda install pybind11 suitesparse
 pip install klujax
 ```
 
 ## License & Credits
 
 © Floris Laporte 2022, LGPL-2.1
 
 This library was partly based on:
 
 - [torch_sparse_solve](https://github.com/flaport/torch_sparse_solve), LGPL-2.1
 - [SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse), LGPL-2.1
 - [kagami-c/PyKLU](https://github.com/kagami-c/PyKLU), LGPL-2.1
 - [scipy.sparse](https://github.com/scipy/scipy/tree/master/scipy/sparse), BSD-3
+
+This library vendors an unmodified version of the
+[SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse) libraries in its source
+(.tar.gz) distribution to allow for static linking.
+This is in accordance with their
+[LGPL licence](https://github.com/DrTimothyAldenDavis/SuiteSparse/blob/dev/LICENSE.txt).
+
```

### Comparing `klujax-0.1.4/klujax.cpp` & `klujax-0.2.0/klujax.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// version: 0.1.4
+// version: 0.2.0
 // author: Floris Laporte
 
 #include <iostream>
 #include <vector>
 
 #include <klu.h>
 #include <pybind11/pybind11.h>
```

### Comparing `klujax-0.1.4/klujax.egg-info/PKG-INFO` & `klujax-0.2.0/klujax.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klujax
-Version: 0.1.4
+Version: 0.2.0
 Summary: a KLU solver for JAX
 Home-page: https://github.com/flaport/klujax
 Author: Floris Laporte
 Author-email: floris.laporte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
@@ -59,30 +59,32 @@
 ```
 [ True True True True True]
 [1. 2. 3. 4. 5.]
 ```
 
 ## Installation
 
-The library is dynamically linked to the SuiteSparse C++ library. The easiest way to
-install is as follows:
+The library is statically linked to the SuiteSparse C++ library. It can be installed on
+most platforms as follows:
 
 ```bash
-conda install pybind11 suitesparse
 pip install klujax
 ```
 
 **There exist pre-built wheels for Linux and Windows (python 3.8+).** If no compatible
 wheel is found, however, pip will attempt to install the library from source... make
 sure you have the necessary build dependencies installed.
 
 ### Linux
 
-On linux, having `gcc` and `g++` available in your path should be sufficient to be able
-to build the library from source.
+On linux, you'll need `gcc` and `g++`. Then just do a normal pip install:
+
+```sh
+pip install klujax
+```
 
 ### Windows
 
 On Windows, installing from source is a bit more involved as typically the build
 dependencies are not installed. To install those, download Visual Studio Community 2017
 from [here](https://my.visualstudio.com/Downloads?q=visual%20studio%202017&wt.mc_id=o~msft~vscom~older-downloads). During installation, go to Workloads and select the following workloads:
 
@@ -93,25 +95,31 @@
 
 - C++/CLI support
 - VC++ 2015.3 v14.00 (v140) toolset for desktop
 
 Then, download and install Microsoft Visual C++ Redistributable from [here](https://aka.ms/vs/16/release/vc_redist.x64.exe).
 
 After these installation steps, run the following commands inside a x64 Native Tools
-Command Prompt for VS 2017, after activating your conda environment:
+Command Prompt for VS 2017:
 
 ```
 set DISTUTILS_USE_SDK=1
-conda install pybind11 suitesparse
 pip install klujax
 ```
 
 ## License & Credits
 
 © Floris Laporte 2022, LGPL-2.1
 
 This library was partly based on:
 
 - [torch_sparse_solve](https://github.com/flaport/torch_sparse_solve), LGPL-2.1
 - [SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse), LGPL-2.1
 - [kagami-c/PyKLU](https://github.com/kagami-c/PyKLU), LGPL-2.1
 - [scipy.sparse](https://github.com/scipy/scipy/tree/master/scipy/sparse), BSD-3
+
+This library vendors an unmodified version of the
+[SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse) libraries in its source
+(.tar.gz) distribution to allow for static linking.
+This is in accordance with their
+[LGPL licence](https://github.com/DrTimothyAldenDavis/SuiteSparse/blob/dev/LICENSE.txt).
+
```

### Comparing `klujax-0.1.4/klujax.py` & `klujax-0.2.0/klujax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ klujax: a KLU solver for JAX """
 
-__version__ = "0.1.4"
+__version__ = "0.2.0"
 __author__ = "Floris Laporte"
 __all__ = ["solve", "coo_mul_vec"]
 
 
 # Imports =============================================================================
```

