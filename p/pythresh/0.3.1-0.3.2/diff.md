# Comparing `tmp/pythresh-0.3.1.tar.gz` & `tmp/pythresh-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythresh-0.3.1.tar", last modified: Wed May  3 17:06:44 2023, max compression
+gzip compressed data, was "pythresh-0.3.2.tar", last modified: Sun Jul  2 07:18:36 2023, max compression
```

## Comparing `pythresh-0.3.1.tar` & `pythresh-0.3.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.131144 pythresh-0.3.1/
--rw-r--r--   0 denmark   (1000) denmark   (1000)     1317 2022-06-16 06:55:08.000000 pythresh-0.3.1/LICENSE
--rw-r--r--   0 denmark   (1000) denmark   (1000)      269 2023-03-20 18:17:50.000000 pythresh-0.3.1/MANIFEST.in
--rw-r--r--   0 denmark   (1000) denmark   (1000)    28480 2023-05-03 17:06:44.131144 pythresh-0.3.1/PKG-INFO
--rw-r--r--   0 denmark   (1000) denmark   (1000)    27334 2023-05-03 17:00:01.000000 pythresh-0.3.1/README.rst
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.107810 pythresh-0.3.1/pythresh/
--rw-r--r--   0 denmark   (1000) denmark   (1000)       89 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/__init__.py
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.111144 pythresh-0.3.1/pythresh/models/
--rw-r--r--   0 denmark   (1000) denmark   (1000)   141564 2022-11-06 09:53:23.000000 pythresh-0.3.1/pythresh/models/meta_model_GNB.pkl
--rw-r--r--   0 denmark   (1000) denmark   (1000)   141284 2022-12-31 13:15:02.000000 pythresh-0.3.1/pythresh/models/meta_model_GNBC.pkl
--rw-r--r--   0 denmark   (1000) denmark   (1000)   165531 2023-03-16 17:01:32.000000 pythresh-0.3.1/pythresh/models/meta_model_GNBM.pkl
--rw-r--r--   0 denmark   (1000) denmark   (1000)  3181480 2022-11-06 09:53:21.000000 pythresh-0.3.1/pythresh/models/meta_model_LIN.pkl
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.131144 pythresh-0.3.1/pythresh/thresholds/
--rw-r--r--   0 denmark   (1000) denmark   (1000)        0 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/__init__.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3320 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/aucp.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     1008 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/base.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3378 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/boot.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3499 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/chau.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2905 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/clf.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)    10087 2023-04-23 15:04:42.000000 pythresh-0.3.1/pythresh/thresholds/clust.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4293 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/comb.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2782 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/cpd.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3996 2023-04-27 08:02:52.000000 pythresh-0.3.1/pythresh/thresholds/decomp.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)    10503 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/dsn.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3427 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/eb.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2512 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/fgd.py
--rwxr-xr-x   0 denmark   (1000) denmark   (1000)     4900 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/filter.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2316 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/fwfm.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4104 2023-04-13 18:25:50.000000 pythresh-0.3.1/pythresh/thresholds/gesd.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     9327 2023-04-15 13:25:28.000000 pythresh-0.3.1/pythresh/thresholds/hist.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2323 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/iqr.py
--rwxr-xr-x   0 denmark   (1000) denmark   (1000)     3516 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/karch.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2110 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/mad.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4938 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/mcst.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     5266 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/meta.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4721 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/moll.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     5518 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/mtt.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     7163 2023-04-15 13:29:48.000000 pythresh-0.3.1/pythresh/thresholds/ocsvm.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3928 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/qmcd.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3476 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/regr.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)      806 2023-04-13 17:36:34.000000 pythresh-0.3.1/pythresh/thresholds/thresh_utility.py
--rwxr-xr-x   0 denmark   (1000) denmark   (1000)    10067 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/vae.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4774 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/wind.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3253 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/yj.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2067 2023-05-02 19:25:21.000000 pythresh-0.3.1/pythresh/thresholds/zscore.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)      171 2023-05-03 16:02:26.000000 pythresh-0.3.1/pythresh/version.py
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.111144 pythresh-0.3.1/pythresh.egg-info/
--rw-r--r--   0 denmark   (1000) denmark   (1000)    28480 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/PKG-INFO
--rw-r--r--   0 denmark   (1000) denmark   (1000)     1315 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/SOURCES.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)        1 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/dependency_links.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)       66 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/requires.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)        9 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/top_level.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)       66 2023-05-02 18:44:48.000000 pythresh-0.3.1/requirements.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)       80 2023-05-03 17:06:44.131144 pythresh-0.3.1/setup.cfg
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2266 2023-05-02 17:41:56.000000 pythresh-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.580541 pythresh-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-02 07:18:20.000000 pythresh-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-02 07:18:20.000000 pythresh-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28627 2023-07-02 07:18:36.580541 pythresh-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-07-02 07:18:20.000000 pythresh-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.564540 pythresh-0.3.2/pythresh/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.568540 pythresh-0.3.2/pythresh/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   141564 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_GNB.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   141284 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_GNBC.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   165531 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_GNBM.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  3181480 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_LIN.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.580541 pythresh-0.3.2/pythresh/thresholds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/aucp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/chau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/clf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/clust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/comb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/cpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/dsn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/eb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/fgd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/fwfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/gesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/iqr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3447 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/karch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/mad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/mcst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/moll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/mtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/ocsvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/qmcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/thresh_utility.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10061 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/yj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/zscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-02 07:18:21.000000 pythresh-0.3.2/pythresh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.568540 pythresh-0.3.2/pythresh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28627 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-02 07:18:20.000000 pythresh-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 07:18:36.580541 pythresh-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-02 07:18:20.000000 pythresh-0.3.2/setup.py
```

### Comparing `pythresh-0.3.1/LICENSE` & `pythresh-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/PKG-INFO` & `pythresh-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pythresh
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Toolbox for Outlier Detection Thresholding
 Home-page: https://github.com/KulikDM/pythresh
-Author: D Kulik
-License: UNKNOWN
 Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
+Author: D Kulik
 Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
 Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
@@ -46,14 +44,18 @@
    :target: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml
    :alt: testing
 
 .. image:: https://codecov.io/gh/KulikDM/pythresh/branch/main/graph/badge.svg?token=8ZAPXTLW9Y
    :target: https://codecov.io/gh/KulikDM/pythresh
    :alt: Codecov
 
+.. image:: https://api.codeclimate.com/v1/badges/3e2de42b48701c731ef6/maintainability
+   :target: https://codeclimate.com/github/KulikDM/pythresh/maintainability
+   :alt: Maintainability
+
 .. image:: https://img.shields.io/github/stars/KulikDM/pythresh.svg?logo=github&logoColor=white
    :target: https://github.com/KulikDM/pythresh/stargazers
    :alt: GitHub stars
 
 .. image:: https://pepy.tech/badge/pythresh?
    :target: https://pepy.tech/project/pythresh
    :alt: Downloads
@@ -107,24 +109,24 @@
 
 **Outlier Detection Thresholding with 7 Lines of Code**:
 
 .. code:: python
 
    # train the KNN detector
    from pyod.models.knn import KNN
-   from pythresh.thresholds.clust import CLUST
+   from pythresh.thresholds.filter import FILTER
 
    clf = KNN()
    clf.fit(X_train)
 
    # get outlier scores
    decision_scores = clf.decision_scores_  # raw outlier scores on the train data
 
    # get outlier labels
-   thres = CLUST()
+   thres = FILTER()
    labels = thres.eval(decision_scores)
 
 **************
  Installation
 **************
 
 It is recommended to use **pip** or **conda** for installation:
@@ -156,15 +158,14 @@
 **Required Dependencies**:
 
 -  matplotlib
 -  numpy>=1.13
 -  pyod
 -  scipy>=1.3.1
 -  scikit_learn>=0.20.0
--  six
 
 **Optional Dependencies**:
 
 -  pyclustering (used in the CLUST thresholder)
 -  ruptures (used in the CPD thresholder)
 -  geomstats (used in the KARCH thresholder)
 -  scikit-lego (used in the META thresholder)
@@ -489,9 +490,7 @@
    `Transforming variables to central normality
    <https://arxiv.org/abs/2005.07946>`_
 
 .. [#zscore1]
 
    `Multiple outlier detection tests for parametric models
    <https://arxiv.org/abs/1910.10426>`_
-
-
```

### Comparing `pythresh-0.3.1/README.rst` & `pythresh-0.3.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,18 @@
    :target: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml
    :alt: testing
 
 .. image:: https://codecov.io/gh/KulikDM/pythresh/branch/main/graph/badge.svg?token=8ZAPXTLW9Y
    :target: https://codecov.io/gh/KulikDM/pythresh
    :alt: Codecov
 
+.. image:: https://api.codeclimate.com/v1/badges/3e2de42b48701c731ef6/maintainability
+   :target: https://codeclimate.com/github/KulikDM/pythresh/maintainability
+   :alt: Maintainability
+
 .. image:: https://img.shields.io/github/stars/KulikDM/pythresh.svg?logo=github&logoColor=white
    :target: https://github.com/KulikDM/pythresh/stargazers
    :alt: GitHub stars
 
 .. image:: https://pepy.tech/badge/pythresh?
    :target: https://pepy.tech/project/pythresh
    :alt: Downloads
@@ -81,24 +85,24 @@
 
 **Outlier Detection Thresholding with 7 Lines of Code**:
 
 .. code:: python
 
    # train the KNN detector
    from pyod.models.knn import KNN
-   from pythresh.thresholds.clust import CLUST
+   from pythresh.thresholds.filter import FILTER
 
    clf = KNN()
    clf.fit(X_train)
 
    # get outlier scores
    decision_scores = clf.decision_scores_  # raw outlier scores on the train data
 
    # get outlier labels
-   thres = CLUST()
+   thres = FILTER()
    labels = thres.eval(decision_scores)
 
 **************
  Installation
 **************
 
 It is recommended to use **pip** or **conda** for installation:
@@ -130,15 +134,14 @@
 **Required Dependencies**:
 
 -  matplotlib
 -  numpy>=1.13
 -  pyod
 -  scipy>=1.3.1
 -  scikit_learn>=0.20.0
--  six
 
 **Optional Dependencies**:
 
 -  pyclustering (used in the CLUST thresholder)
 -  ruptures (used in the CPD thresholder)
 -  geomstats (used in the KARCH thresholder)
 -  scikit-lego (used in the META thresholder)
```

### Comparing `pythresh-0.3.1/pythresh/models/meta_model_GNB.pkl` & `pythresh-0.3.2/pythresh/models/meta_model_GNB.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/models/meta_model_GNBC.pkl` & `pythresh-0.3.2/pythresh/models/meta_model_GNBC.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/models/meta_model_GNBM.pkl` & `pythresh-0.3.2/pythresh/models/meta_model_GNBM.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/models/meta_model_LIN.pkl` & `pythresh-0.3.2/pythresh/models/meta_model_LIN.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/aucp.py` & `pythresh-0.3.2/pythresh/thresholds/aucp.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/base.py` & `pythresh-0.3.2/pythresh/thresholds/base.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/boot.py` & `pythresh-0.3.2/pythresh/thresholds/boot.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/chau.py` & `pythresh-0.3.2/pythresh/thresholds/chau.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/clf.py` & `pythresh-0.3.2/pythresh/thresholds/clf.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/clust.py` & `pythresh-0.3.2/pythresh/thresholds/clust.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/comb.py` & `pythresh-0.3.2/pythresh/thresholds/comb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import numpy as np
 import scipy.stats as stats
+from sklearn.base import BaseEstimator, ClassifierMixin
+from sklearn.ensemble import BaggingClassifier, StackingClassifier
+from sklearn.linear_model import RidgeClassifier
 from sklearn.utils import check_array
 
 from .base import BaseThresholder
 from .thresh_utility import cut, normalize
 
 
 class COMB(BaseThresholder):
@@ -14,47 +17,53 @@
        are set to any value beyond the (mean, median, or mode) of the
        contamination from the selected combination of thresholders.
 
        Parameters
        ----------
 
        thresholders : list, optional (default='default')
-            List of instantiated thresholders, e.g. [DSN(), FILTER()]
+            List of instantiated thresholders, e.g. [DSN(), FILTER()].
+            Default is [DSN(random_state=self.random_state), FILTER(),
+            OCSVM(random_state=self.random_state)]
 
        max_contam : float, optional (default=0.5)
             Maximum contamination allowed for each threshold output. Thresholded scores
             above the maximum contamination will not be included in the final combined
             threshold
 
-       method : {'mean', 'median', 'mode'}, optional (default='mean')
-           statistic to apply to contamination levels
+       method : {'mean', 'median', 'mode', 'bagged', 'stacked}, optional (default='stacked')
+           evaluation method to apply to contamination levels
 
-           - 'mean':   calculate the mean combined threshold
-           - 'median': calculate the median combined threshold
-           - 'mode':  calculate the majority vote or mode of the thresholded labels
+           - 'mean':    calculate the mean combined threshold
+           - 'median':  calculate the median combined threshold
+           - 'mode':    calculate the majority vote or mode of the thresholded labels
+           - 'bagged':  use a bagged LaplaceGaussianNB to solve the combined threshold
+           - 'stacked': use a stacked Ridge, and LaplaceGaussianNB classifier combined method
 
        random_state : int, optional (default=1234)
             Random seed for the random number generators of the thresholders. Can also
             be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        confidence_interval_ : lower and upper confidence interval of the contamination level
     """
 
-    def __init__(self, thresholders='default', max_contam=0.5, method='mean', random_state=1234):
+    def __init__(self, thresholders='default', max_contam=0.5, method='stacked', random_state=1234):
 
         self.thresholders = thresholders
         self.max_contam = max_contam
-        stat = {'mean': np.mean, 'median': np.median, 'mode': stats.mode}
+        func = {'mean': np.mean, 'median': np.median,
+                'mode': stats.mode, 'bagged': BaggingClassifier,
+                'stacked': StackingClassifier}
         self.method = method
-        self.method_func = stat[method]
+        self.method_func = func[method]
         self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
@@ -68,15 +77,15 @@
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
         decision = check_array(decision, ensure_2d=False)
 
-        decision = np.sort(normalize(decision))
+        decision = normalize(decision)
 
         # Initialize thresholders
         if self.thresholders == 'default':
             from .dsn import DSN
             from .filter import FILTER
             from .ocsvm import OCSVM
 
@@ -103,25 +112,92 @@
 
         # Get lower and upper confidence interval
         low, high = stats.bootstrap(ratio.reshape(1, -1),
                                     np.mean, paired=True,
                                     random_state=self.random_state).confidence_interval
         self.confidence_interval_ = [low, high]
 
-        # Get [mean, median, or mode] of inliers
-        if self.method == 'mode':
+        # Get [mean, median, mode, bagged, or stacked] of inliers
+        if (self.method == 'bagged') or (self.method == 'stacked'):
+
+            X = np.tile(decision, len(contam))
+            y = np.hstack(contam)
+
+            if (self.method == 'bagged'):
+                model = self.method_func(LaplaceGaussianNB(),
+                                         n_estimators=12,
+                                         random_state=self.random_state)
+            else:
+                model = self.method_func([('Ridge', RidgeClassifier()),
+                                          ('GNB', LaplaceGaussianNB())])
+
+            model.fit(X.reshape(-1, 1), y)
+            lbls = model.predict(decision.reshape(-1, 1))
+
+            self.thresh_ = None
+
+            return lbls
+
+        elif self.method == 'mode':
 
             self.thresh_ = None
             lbls = self.method_func(contam, axis=0)
 
             return np.squeeze(lbls[0])
 
         else:
 
             contam = np.sum(contam, axis=1)/contam.shape[1]
             inlier_ratio = 1-self.method_func(contam)
 
             idx = int(counts*inlier_ratio)
-            limit = decision[idx] if idx < counts else 1.0
+            ordered = np.sort(decision)
+            limit = ordered[idx] if idx < counts else 1.0
             self.thresh_ = limit
 
             return cut(decision, limit)
+
+
+class LaplaceGaussianNB(BaseEstimator, ClassifierMixin):
+
+    def __init__(self):
+
+        pass
+
+    def fit(self, X, y):
+
+        X = X.squeeze()
+
+        self.models = []
+        self.priors = []
+        self.classes_ = [0, 1]
+        dist = [stats.laplace, stats.norm]
+
+        for c in self.classes_:
+
+            subset_x = X[y == c]
+
+            self.models.append(dist[c](subset_x.mean(),
+                                       subset_x.std()))
+
+            self.priors.append(len(subset_x)/len(X))
+
+        return self
+
+    def predict(self, X):
+
+        likelihoods = self.predict_proba(X)
+
+        return likelihoods.argmax(axis=1)
+
+    def predict_proba(self, X):
+
+        X = X.squeeze()
+
+        likelihoods = []
+
+        for c in self.classes_:
+
+            probs = self.priors[c] * self.models[c].pdf(X)
+            likelihoods.append(probs)
+
+        return np.vstack(likelihoods).T
```

### Comparing `pythresh-0.3.1/pythresh/thresholds/cpd.py` & `pythresh-0.3.2/pythresh/thresholds/cpd.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/decomp.py` & `pythresh-0.3.2/pythresh/thresholds/decomp.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/dsn.py` & `pythresh-0.3.2/pythresh/thresholds/dsn.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/eb.py` & `pythresh-0.3.2/pythresh/thresholds/eb.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/fgd.py` & `pythresh-0.3.2/pythresh/thresholds/fgd.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/filter.py` & `pythresh-0.3.2/pythresh/thresholds/filter.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/fwfm.py` & `pythresh-0.3.2/pythresh/thresholds/fwfm.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/gesd.py` & `pythresh-0.3.2/pythresh/thresholds/gesd.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/hist.py` & `pythresh-0.3.2/pythresh/thresholds/hist.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/iqr.py` & `pythresh-0.3.2/pythresh/thresholds/iqr.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/karch.py` & `pythresh-0.3.2/pythresh/thresholds/karch.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,21 +86,19 @@
             val_data = val_data.reshape(-1, 1)
             val_norm = np.sort(decision).reshape(1, -1)
 
             try:
                 # find kde and score dot product and solve the
                 vals = np.dot(val_data, val_norm)
                 estimator.fit(vals)
-                kmean = np.mean(estimator.estimate_)+np.std(decision)
 
             except ValueError:
-                kmean = 1.0
+                estimator.fit(decision.reshape(1, -1))
         else:
             estimator.fit(decision.reshape(1, -1))
-            kmean = np.mean(estimator.estimate_) + np.std(decision)
 
         # Get the mean of each dimension's Karcher mean
-        limit = kmean
+        limit = np.mean(estimator.estimate_) + np.std(decision)
 
         self.thresh_ = limit
 
         return cut(decision, limit)
```

### Comparing `pythresh-0.3.1/pythresh/thresholds/mad.py` & `pythresh-0.3.2/pythresh/thresholds/mad.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
         decision = check_array(decision, ensure_2d=False)
 
         decision = normalize(decision)
 
-        # Set limit equal to 3 median abolute deviations
+        # Set limit
         mean = np.mean(decision)
         limit = mean + \
             stats.median_abs_deviation(decision, scale=np.std(decision))
 
         self.thresh_ = limit
 
         return cut(decision, limit)
```

### Comparing `pythresh-0.3.1/pythresh/thresholds/mcst.py` & `pythresh-0.3.2/pythresh/thresholds/mcst.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/meta.py` & `pythresh-0.3.2/pythresh/thresholds/meta.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/moll.py` & `pythresh-0.3.2/pythresh/thresholds/moll.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,15 @@
         p = np.abs((s - (s[0]+s[-1])/2.0)/width)
         r = np.zeros_like(s)
         q = p[p < 1.0]
         r[p < 1.0] = np.exp(1.0/(q**2-1.0))
         rho = (norm_const/width)*r
 
         # Perform convolution to make smooth reconstruction
-        if s.shape[0] > 500:
-            smooth = signal.fftconvolve(ds*position_interp, rho, mode='same')
-        else:
-            smooth = np.convolve(ds*position_interp, rho, mode='same')
+        conv_func = signal.fftconvolve if s.shape[0] > 500 else np.convolve
+        smooth = conv_func(ds*position_interp, rho, mode='same')
 
         # remove padding
         s = s[left_pad_num:-right_pad_num]
         smooth = smooth[left_pad_num:-(right_pad_num)]
 
         return np.asarray(smooth)
```

### Comparing `pythresh-0.3.1/pythresh/thresholds/ocsvm.py` & `pythresh-0.3.2/pythresh/thresholds/ocsvm.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/qmcd.py` & `pythresh-0.3.2/pythresh/thresholds/qmcd.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/regr.py` & `pythresh-0.3.2/pythresh/thresholds/regr.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/thresh_utility.py` & `pythresh-0.3.2/pythresh/thresholds/thresh_utility.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/vae.py` & `pythresh-0.3.2/pythresh/thresholds/vae.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,15 @@
         self.device = device
         self.latent_dims = latent_dims
         self.dist = Normal
         self.epochs = epochs
         self.loss = loss
         self.batch_size = batch_size
         self.random_state = random_state
-        if random_state:
-            torch.manual_seed(random_state)
+        torch.manual_seed(random_state) if random_state else None
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
@@ -197,16 +196,15 @@
         self.input_size = input_size
         self.latent_size = latent_size
         self.encoder = self.data_encoder(input_size, latent_size)
         self.decoder = self.data_decoder(latent_size, input_size)
         self.dist = dist
         self.loss = loss
 
-        if random_state:
-            torch.manual_seed(random_state)
+        torch.manual_seed(random_state) if random_state else None
 
         self.prior = self.dist(0, 1)
 
     def data_encoder(self, input_size, latent_size):
 
         return nn.Sequential(
             nn.Linear(input_size, 128),
```

### Comparing `pythresh-0.3.1/pythresh/thresholds/wind.py` & `pythresh-0.3.2/pythresh/thresholds/wind.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/yj.py` & `pythresh-0.3.2/pythresh/thresholds/yj.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh/thresholds/zscore.py` & `pythresh-0.3.2/pythresh/thresholds/zscore.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/pythresh.egg-info/PKG-INFO` & `pythresh-0.3.2/pythresh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pythresh
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Toolbox for Outlier Detection Thresholding
 Home-page: https://github.com/KulikDM/pythresh
-Author: D Kulik
-License: UNKNOWN
 Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
+Author: D Kulik
 Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
 Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
@@ -46,14 +44,18 @@
    :target: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml
    :alt: testing
 
 .. image:: https://codecov.io/gh/KulikDM/pythresh/branch/main/graph/badge.svg?token=8ZAPXTLW9Y
    :target: https://codecov.io/gh/KulikDM/pythresh
    :alt: Codecov
 
+.. image:: https://api.codeclimate.com/v1/badges/3e2de42b48701c731ef6/maintainability
+   :target: https://codeclimate.com/github/KulikDM/pythresh/maintainability
+   :alt: Maintainability
+
 .. image:: https://img.shields.io/github/stars/KulikDM/pythresh.svg?logo=github&logoColor=white
    :target: https://github.com/KulikDM/pythresh/stargazers
    :alt: GitHub stars
 
 .. image:: https://pepy.tech/badge/pythresh?
    :target: https://pepy.tech/project/pythresh
    :alt: Downloads
@@ -107,24 +109,24 @@
 
 **Outlier Detection Thresholding with 7 Lines of Code**:
 
 .. code:: python
 
    # train the KNN detector
    from pyod.models.knn import KNN
-   from pythresh.thresholds.clust import CLUST
+   from pythresh.thresholds.filter import FILTER
 
    clf = KNN()
    clf.fit(X_train)
 
    # get outlier scores
    decision_scores = clf.decision_scores_  # raw outlier scores on the train data
 
    # get outlier labels
-   thres = CLUST()
+   thres = FILTER()
    labels = thres.eval(decision_scores)
 
 **************
  Installation
 **************
 
 It is recommended to use **pip** or **conda** for installation:
@@ -156,15 +158,14 @@
 **Required Dependencies**:
 
 -  matplotlib
 -  numpy>=1.13
 -  pyod
 -  scipy>=1.3.1
 -  scikit_learn>=0.20.0
--  six
 
 **Optional Dependencies**:
 
 -  pyclustering (used in the CLUST thresholder)
 -  ruptures (used in the CPD thresholder)
 -  geomstats (used in the KARCH thresholder)
 -  scikit-lego (used in the META thresholder)
@@ -489,9 +490,7 @@
    `Transforming variables to central normality
    <https://arxiv.org/abs/2005.07946>`_
 
 .. [#zscore1]
 
    `Multiple outlier detection tests for parametric models
    <https://arxiv.org/abs/1910.10426>`_
-
-
```

### Comparing `pythresh-0.3.1/pythresh.egg-info/SOURCES.txt` & `pythresh-0.3.2/pythresh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.1/setup.py` & `pythresh-0.3.2/setup.py`

 * *Files identical despite different names*

