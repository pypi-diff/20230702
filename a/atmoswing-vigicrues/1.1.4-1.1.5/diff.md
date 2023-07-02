# Comparing `tmp/atmoswing-vigicrues-1.1.4.tar.gz` & `tmp/atmoswing-vigicrues-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.1.4.tar", last modified: Thu Jun  8 20:28:56 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.1.5.tar", last modified: Sun Jul  2 21:21:55 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.1.4.tar` & `atmoswing-vigicrues-1.1.5.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.488468 atmoswing-vigicrues-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.488468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.488468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.1.4/LICENSE` & `atmoswing-vigicrues-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/PKG-INFO` & `atmoswing-vigicrues-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.4
+Version: 1.1.5
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -35,15 +35,15 @@
 Installation
 ------------
 
 Pour utiliser le module atmoswing-vigicrues, il faut installer :
 
 * Python >= 3.7
 * AtmoSwing Forecaster (de préférence la version serveur)
-* Le module atmoswing-vigicrues ("``pip install atmoswing-vigicrues``" ou l'image docker "``docker pull atmoswing/atmoswing-vigicrues``")
+* Le module atmoswing-vigicrues (``pip install atmoswing-vigicrues`` ou l'image docker ``docker pull atmoswing/atmoswing-vigicrues``)
 
 Utilisation
 -----------
 
 Le paquet est constitué de plusieurs modules qui peuvent être activés et configurés dans un fichier de configuration. Plusieurs flux de prévision peuvent être configurés sur un serveur / PC par la création de différents fichiers de configuration. Il n’y a pas de paramètres codés en dur dans le code. L’exécution d’un flux de prévision est effectuée par la commande :
 ``python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml``
 Le fichier de configuration définit :
```

### Comparing `atmoswing-vigicrues-1.1.4/README.md` & `atmoswing-vigicrues-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 Installation
 ------------
 
 Pour utiliser le module atmoswing-vigicrues, il faut installer :
 
 * Python >= 3.7
 * AtmoSwing Forecaster (de préférence la version serveur)
-* Le module atmoswing-vigicrues ("``pip install atmoswing-vigicrues``" ou l'image docker "``docker pull atmoswing/atmoswing-vigicrues``")
+* Le module atmoswing-vigicrues (``pip install atmoswing-vigicrues`` ou l'image docker ``docker pull atmoswing/atmoswing-vigicrues``)
 
 Utilisation
 -----------
 
 Le paquet est constitué de plusieurs modules qui peuvent être activés et configurés dans un fichier de configuration. Plusieurs flux de prévision peuvent être configurés sur un serveur / PC par la création de différents fichiers de configuration. Il n’y a pas de paramètres codés en dur dans le code. L’exécution d’un flux de prévision est effectuée par la commande :
 ``python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml``
 Le fichier de configuration définit :
```

### Comparing `atmoswing-vigicrues-1.1.4/pyproject.toml` & `atmoswing-vigicrues-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,44 @@
 import atmoswing_vigicrues as asv
 
 
 class Controller:
     """
     Classe principale pour la gestion des prévisions AtmoSwing pour le réseau Vigicrues.
 
+    Parameters
+    ----------
+    cli_options : retour de la fonction parse_args() de la classe
+                  argparse.ArgumentParser
+        Options passées en lignes de commandes à la fonction main()
+
     Attributes
     ----------
-    options : object
+    options : instance de la classe Options
         Options de la prévision combinant les arguments passés lors de l'utilisation en
         lignes de commandes et les options du fichier de configuration.
-    verbose : bool
-        Affichage verbose des messages d'erreurs (pas beaucoup utilisé)
+    time_increment : int
+        Incrément de temps en heures pour l'émission de la prévision
+        (par défaut 6 heures).
     date : datetime.datetime
         Date de la prévision.
+    existing_files : list
+        Liste des fichiers de prévision d'AtmoSwing Forecaster déjà existants pour
+        l'échéance en cours.
+    pre_actions : list
+        Liste des actions préalables à la prévision.
+    post_actions : list
+        Liste des actions postérieures à la prévision.
+    disseminations : list
+        Liste des actions de dissémination.
     """
 
     def __init__(self, cli_options):
         """
         Initialisation de l'instance Controller
-
-        Parameters
-        ----------
-        cli_options : object
-            Options passées en lignes de commandes à la fonction main()
         """
         self.options = asv.Options(cli_options)
         self.time_increment = 6
         self.date = datetime.datetime.utcnow()
         self.existing_files = []
         self.pre_actions = []
         self.post_actions = []
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 class Dissemination:
     """
     Classe de base pour les opérations de diffusion des résultats d'AtmoSwing.
+
+    Attributes
+    ----------
+    _file_paths : list
+        Chemins des fichiers à diffuser.
     """
 
     def __init__(self):
         self._file_paths = []
 
     def feed(self, file_paths):
         """
@@ -21,9 +26,14 @@
         """
         Exécution de la diffusion.
 
         Parameters
         ----------
         date : datetime.datetime
             Date de la prévision.
+
+        Returns
+        -------
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         raise NotImplementedError
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     """
     Transfer des résultats par SFTP.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * local_dir : str
             Répertoire local contenant les fichiers à exporter.
         * extension : str
             Extension des fichiers à exporter.
         * hostname : str
             Adresse du serveur pour la diffusion des résultats.
@@ -32,14 +32,39 @@
             Mot de passe de l'utilisateur sur le serveur.
         * proxy_host : str
             Adresse du proxy, si nécessaire.
         * proxy_port : int
             Port du proxy si nécessaire (par défaut: 1080).
         * remote_dir : str
             Chemin sur le serveur distant où enregistrer les fichiers.
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de l'action.
+    name : str
+        Le nom de l'action.
+    local_dir : str
+        Répertoire local contenant les fichiers à exporter.
+    extension : str
+        Extension des fichiers à exporter.
+    hostname : str
+        Adresse du serveur pour la diffusion des résultats.
+    port : int
+        Port du serveur distant.
+    username : str
+        Utilisateur ayant un accès au serveur.
+    password : str
+        Mot de passe de l'utilisateur sur le serveur.
+    proxy_host : str
+        Adresse du proxy, si nécessaire.
+    proxy_port : int
+        Port du proxy si nécessaire (par défaut: 1080).
+    remote_dir : str
+        Chemin sur le serveur distant où enregistrer les fichiers.
     """
 
     def __init__(self, name, options):
         """
         Initialisation de l'instance TransferSftp
         """
         self.type_name = "Transfert SFTP"
@@ -70,15 +95,16 @@
         Parameters
         ----------
         date : datetime.datetime
             Date de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
             print("  -> Aucun fichier à traiter")
             return False
 
         try:
             # Create a transport object for the SFTP connection
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/options.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 
 class Options:
     """
     Classe permettant de gérer les options passées en lignes de commande et définies
     dans le fichier config.
 
     ----------
-    cli_options : object
+    cli_options : retour de la fonction parse_args() de la classe
+                  argparse.ArgumentParser
         Options de la prévision généralement passées sous la forme d'arguments lors de
         l'utilisation en lignes de commandes.
     config : dict
         Configuration chargée du fichier défini par l'argument config_file.
     """
 
     def __init__(self, cli_options):
         """
         Initialisation de l'instance Options
 
         Parameters
         ----------
-        cli_options : object
+        cli_options : retour de la fonction parse_args() de la classe
+                      argparse.ArgumentParser
             Options passées en lignes de commandes à la fonction main()
         """
         self.cli_options = cli_options
         self.config = None
         self._check_options()
         self._load_config()
         self._override_options()
@@ -54,14 +56,15 @@
         Parameters
         ----------
         key
             Le nom de l'option.
 
         Returns
         -------
+        bool
             Vrai (True) si l'option existe, faux (False) sinon.
         """
         if key in self.config and self.config[key]:
             return True
         return False
 
     def get(self, key):
@@ -71,14 +74,15 @@
         Parameters
         ----------
         key
             Le nom de l'option.
 
         Returns
         -------
+        str|int|float
             La valeur de l'option.
         """
         if self.has(key):
             return self.config[key]
         raise asv.OptionError(key)
 
     def _check_options(self):
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,46 @@
     """
     Export des prévisions au format Json de la BdApBp.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
         * number_analogs : int
             Nombre d'analogues maximal à conserver (valeurs les plus élevées).
             -1 pour toutes les analogues.
         * only_relevant_stations : bool
             Exporter uniquement les stations pour lesquelles la méthode a été calibrée.
         * use_indentation : bool
             Ajouter une indentation aux fichiers produits.
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de post-action.
+    name : str
+        Le nom de l'action.
+    status : int
+        Le statut de l'action.
+    message : str
+        Un éventuel message d'erreur de l'action.
+    output_dir : str
+        Chemin cible pour l'enregistrement des fichiers.
+    number_analogs : int
+        Nombre d'analogues maximal à conserver (valeurs les plus élevées).
+        -1 pour toutes les analogues.
+    only_relevant_stations : bool
+        Exporter uniquement les stations pour lesquelles la méthode a été calibrée.
+    use_indentation : bool
+        Ajouter une indentation aux fichiers produits.
     """
 
     def __init__(self, name, options):
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
 
         self.type_name = "Export BdApBp"
@@ -70,19 +90,20 @@
 
         * 100 : Absence du fichier netcdf.
         * 110 : Fichier netcdf corrompu.
         * 200 : Erreur lors du traitement fichier netcdf.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
             print("  -> Aucun fichier à traiter")
-            return False
+            return True
 
         files_count = 0
         for file in self._file_paths:
             file = Path(file)
 
             # Nom du fichier
             file_path = self._build_file_path(file)
@@ -295,15 +316,18 @@
                 block_target_date[target_date_str] = block_analogs
             block[str(station_id)] = block_target_date
 
         return block
 
     @staticmethod
     def _get_time_format(target_dates):
-        time_step = target_dates[1] - target_dates[0]
+        assert len(target_dates) > 1
+        time_step = target_dates[1].astype(datetime.datetime) - \
+                    target_dates[0].astype(datetime.datetime)
+        time_step = time_step.total_seconds()
         show_hour = time_step < 24 * 3600
         time_format_target = "%Y%m%d"
         time_format_analogs = "%Y-%m-%d"
         if show_hour:
             time_format_target = "%Y%m%d%H"
             time_format_analogs = "%Y-%m-%d %H"
         return time_format_analogs, time_format_target
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,26 +12,42 @@
     """
     Export des prévisions au format PRV du logiciel Scores.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
         * date_format : str
             Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
         * frequencies : list
             Les fréquences à extraire.
             Par défaut : [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.95]
         * combine_stations_in_one_file : bool
             Combinaison des différentes stations (entités) dans un seul fichier.
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de l'action.
+    name : str
+        Le nom de l'action.
+    output_dir : str
+        Chemin cible pour l'enregistrement des fichiers.
+    date_format : str
+        Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
+    frequencies : list
+        Les fréquences à extraire.
+        Par défaut : [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.95]
+    combine_stations_in_one_file : bool
+        Combinaison des différentes stations (entités) dans un seul fichier.
     """
 
     def __init__(self, name, options):
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
 
         self.type_name = "Export PRV"
@@ -58,19 +74,20 @@
 
     def run(self) -> bool:
         """
         Exécution de la post-action.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
             print("  -> Aucun fichier à traiter")
-            return False
+            return True
 
         files_count = 0
         for file in self._file_paths:
             nc_file = asv.Dataset(file, 'r', format='NETCDF4')
             station_ids = self._extract_station_ids(nc_file)
             header_comments = self._create_header_comments(nc_file)
             if self.combine_stations_in_one_file:
@@ -213,13 +230,16 @@
     def _build_id_series(self, nc_file):
         ids = ""
         for freq in self.frequencies:
             ids += f"{nc_file.method_id}.{nc_file.specific_tag}.{int(100 * freq):03d};"
         return ids
 
     def _get_time_format(self, target_dates):
-        time_step = target_dates[1] - target_dates[0]
+        assert len(target_dates) > 1
+        time_step = target_dates[1].astype(datetime.datetime) - \
+                    target_dates[0].astype(datetime.datetime)
+        time_step = time_step.total_seconds()
         show_hour = time_step < 24 * 3600
         time_format_target = self.date_format
         if show_hour:
             time_format_target = self.date_format + " %H:%M"
         return time_format_target
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,43 +14,68 @@
     """
     Téléchargement des prévisions émises par GFS.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Répertoire cible pour l'enregistrement des fichiers.
         * lead_time_max : int
             Échéance maximale de la prévision en heures.
             Valeur par défaut : 168
         * variables : list
             Variables à télécharger.
             Valeur par défaut: ['hgt']
         * levels : list
             Niveaux de pression à télécharger.
             Valeur par défaut: [300, 400, 500, 600, 700, 850, 925, 1000]
         * domain : list
-            Domaine à télécharger.
+            Domaine à télécharger (coordonnées géographiques).
             Valeur par défaut: [-20, 30, 25, 65]
         * resolution : float
             Résolution spatiale des données.
             Options: 0.25, 0.50, 1
             Valeur par défaut : 0.25
         * proxy_host : str
             L'adresse du proxy (si nécessaire). Format : proxy_ip:proxy_port
         * proxy_user : str
             L'utilisateur et le mot de passe pour le proxy. Format : username:password
         * attempts_max_hours : int
             Décalage temporel autorisé pour rechercher d'anciens fichiers
         * attempts_step_hours : int
             Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de l'action
+    name : str
+        Le nom de l'action
+    output_dir : str
+        Répertoire cible pour l'enregistrement des fichiers.
+    lead_time_max : int
+        Échéance maximale de la prévision en heures.
+    variables : list
+        Variables à télécharger.
+    levels : list
+        Niveaux de pression à télécharger.
+    domain : list
+        Domaine à télécharger (coordonnées géographiques).
+    resolution : float
+        Résolution spatiale des données.
+    proxies : list
+        Les informations de connexion au proxy.
+    time_increment : int
+        Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
+    time_step_back : int
+        Nombre de pas de temps autorisé pour rechercher d'anciens fichiers
     """
 
     def __init__(self, name, options):
         self.type_name = "Téléchargement GFS"
         self.name = name
         self.output_dir = options['output_dir']
         asv.check_dir_exists(self.output_dir, True)
@@ -115,30 +140,32 @@
         Parameters
         ----------
         date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         return self.download(date)
 
     def download(self, date) -> bool:
         """
         Télécharge les prévisions de GFS pour une date d'émission de la prévision.
 
         Parameters
         ----------
         date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         subregion = self._build_subregion_request()
         levels = self._build_levels_request()
         resol = self.resolution
         sub_product = 'pgrb2'
         if resol == '0p50':
             sub_product = 'pgrb2full'
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/preaction.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/preaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,27 @@
     Classe de base pour les opérations nécessaires avant l'exécution des prévisions.
     """
 
     def __init__(self):
         pass
 
     def run(self, date) -> bool:
-        """ Exécution de la pre-action. """
+        """
+        Exécution de la pre-action.
+
+        Parameters
+        ----------
+        date : datetime.datetime
+            Date de la prévision.
+
+        Returns
+        -------
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
+        """
         raise NotImplementedError
 
     def _set_attempts_attributes(self, options):
         if 'attempts_max_hours' in options:
             self.attempts_max_hours = options['attempts_max_hours']
         else:
             self.attempts_max_hours = 24
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     """
     Récupération des prévisions des modèles météo par SFTP.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * local_dir : str
             Répertoire cible pour l'enregistrement des fichiers.
         * prefix : str
             Prefix des fichiers à importer.
         * variables : list (optionnel)
             Liste des variables météorologiques à importer.
@@ -41,14 +41,41 @@
             Port du proxy si nécessaire (par défaut: 1080).
         * remote_dir : str
             Chemin sur le serveur distant où se trouvent les fichiers.
         * attempts_max_hours : int
             Décalage temporel autorisé pour rechercher d'anciens fichiers
         * attempts_step_hours : int
             Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de l'action
+    name : str
+        Le nom de l'action
+    local_dir : str
+        Répertoire cible pour l'enregistrement des fichiers.
+    prefix : str
+        Prefix des fichiers à importer.
+    hostname : str
+        Adresse du serveur distant.
+    port : int
+        Port du serveur distant.
+    username : str
+        Utilisateur ayant un accès au serveur.
+    password : str
+        Mot de passe de l'utilisateur sur le serveur.
+    remote_dir : str
+        Chemin sur le serveur distant où se trouvent les fichiers.
+    variables : list
+        Liste des variables météorologiques à importer.
+    proxy_host : str
+        Adresse du proxy, si nécessaire.
+    proxy_port : int
+        Port du proxy si nécessaire (par défaut: 1080).
     """
 
     def __init__(self, name, options):
         """
         Initialisation de l'instance TransferSftp
         """
         self.type_name = "Transfert SFTP"
@@ -83,14 +110,19 @@
         """
         Exécution de la récupération par SFTP.
 
         Parameters
         ----------
         date : datetime.datetime
             Date de la prévision.
+
+        Returns
+        -------
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         try:
 
             # Check if files already in the local folder (only with defined variables)
             if self.variables is not None:
                 if self._files_already_present(date):
                     print("  -> Fichiers déjà présents localement.")
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,36 @@
     """
     Transforme les prévisions émises par le CEP en fichier netcdf.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
         * date_format : str
             Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
         * variables : list
             Les variables météorologiques à convertir.
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de l'action.
+    name : str
+        Le nom de l'action.
+    input_dir : str
+        Le chemin vers le répertoire contenant les fichiers à traiter.
+    output_dir : str
+        Le chemin vers le répertoire où seront enregistrés les fichiers.
+    variables : list
+        Les variables météorologiques à convertir.
     """
 
     def __init__(self, name, options):
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
         if not asv.has_eccodes:
             raise ImportError("Le paquet eccodes est requis pour cette action.")
@@ -50,38 +63,39 @@
         Parameters
         ----------
         date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         return self.transform(date)
 
     def transform(self, date) -> bool:
         """
         Transforme les prévisions de l'ECMWF pour une date d'émission de la prévision.
 
         Parameters
         ----------
         date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
 
         input_dir = self._get_input_dir(date)
         forecast_date, forecast_hour = self._format_forecast_date(date)
 
         for variable in self.variables:
-            file_name_pattern = f'{forecast_date}{forecast_hour}.ECMWF_IFS.' \
-                                f'{variable.lower()}.*.grib2'
+            file_name_pattern = f'CEP_{variable}_{forecast_date}{forecast_hour}00.grb'
             new_file_name = f'{forecast_date}{forecast_hour}.ECMWF_IFS.' \
                             f'{variable.lower()}.nc'
 
             input_files = sorted(input_dir.glob(file_name_pattern))
 
             if len(input_files) == 0:
                 return False
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,36 @@
     """
     Transforme les prévisions émises par GFS en fichier netcdf.
 
     Parameters
     ----------
     name: str
         Le nom de l'action
-    options: objet
-        L'instance contenant les options de l'action. Les champs possibles sont:
+    options: dict
+        Un dictionnaire contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
         * date_format : str
             Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
         * variables : list
             Les variables météorologiques à convertir.
+
+    Attributes
+    ----------
+    type_name : str
+        Le nom du type de l'action.
+    name : str
+        Le nom de l'action.
+    input_dir : str
+        Le chemin vers le répertoire contenant les fichiers à traiter.
+    output_dir : str
+        Le chemin vers le répertoire où seront enregistrés les fichiers.
+    variables : list
+        Les variables météorologiques à convertir.
     """
 
     def __init__(self, name, options):
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
         if not asv.has_eccodes:
             raise ImportError("Le paquet eccodes est requis pour cette action.")
@@ -50,30 +63,32 @@
         Parameters
         ----------
         date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
         return self.transform(date)
 
     def transform(self, date) -> bool:
         """
         Transforme les prévisions de GFS pour une date d'émission de la prévision.
 
         Parameters
         ----------
         date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
-        Vrai (True) en cas de succès, faux (False) autrement.
+        bool
+            Vrai (True) en cas de succès, faux (False) autrement.
         """
 
         input_dir = self._get_input_dir(date)
         forecast_date, forecast_hour = self._format_forecast_date(date)
 
         for variable in self.variables:
             file_name_pattern = f'{forecast_date}{forecast_hour}.NWS_GFS.' \
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/PKG-INFO` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.4
+Version: 1.1.5
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -35,15 +35,15 @@
 Installation
 ------------
 
 Pour utiliser le module atmoswing-vigicrues, il faut installer :
 
 * Python >= 3.7
 * AtmoSwing Forecaster (de préférence la version serveur)
-* Le module atmoswing-vigicrues ("``pip install atmoswing-vigicrues``" ou l'image docker "``docker pull atmoswing/atmoswing-vigicrues``")
+* Le module atmoswing-vigicrues (``pip install atmoswing-vigicrues`` ou l'image docker ``docker pull atmoswing/atmoswing-vigicrues``)
 
 Utilisation
 -----------
 
 Le paquet est constitué de plusieurs modules qui peuvent être activés et configurés dans un fichier de configuration. Plusieurs flux de prévision peuvent être configurés sur un serveur / PC par la création de différents fichiers de configuration. Il n’y a pas de paramètres codés en dur dans le code. L’exécution d’un flux de prévision est effectuée par la commande :
 ``python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml``
 Le fichier de configuration définit :
```

### Comparing `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 tests/test_exceptions.py
 tests/test_export_bdapbp.py
 tests/test_export_prv.py
 tests/test_main.py
 tests/test_options.py
 tests/test_transfer_sftp_in.py
 tests/test_transfer_sftp_out.py
+tests/test_transform_ecmwf.py
 tests/test_transform_gfs.py
 tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_controller.py` & `atmoswing-vigicrues-1.1.5/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.1.5/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_exceptions.py` & `atmoswing-vigicrues-1.1.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.1.5/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_export_prv.py` & `atmoswing-vigicrues-1.1.5/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_options.py` & `atmoswing-vigicrues-1.1.5/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_transform_gfs.py` & `atmoswing-vigicrues-1.1.5/tests/test_transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.4/tests/test_utils.py` & `atmoswing-vigicrues-1.1.5/tests/test_utils.py`

 * *Files identical despite different names*

