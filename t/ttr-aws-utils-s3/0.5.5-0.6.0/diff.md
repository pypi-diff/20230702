# Comparing `tmp/ttr.aws.utils.s3-0.5.5.tar.gz` & `tmp/ttr_aws_utils_s3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttr.aws.utils.s3-0.5.5.tar", last modified: Fri Jun 30 20:46:24 2023, max compression
+gzip compressed data, was "ttr_aws_utils_s3-0.6.0.tar", last modified: Sat Jul  1 22:37:07 2023, max compression
```

## Comparing `ttr.aws.utils.s3-0.5.5.tar` & `ttr_aws_utils_s3-0.6.0.tar`

### file list

```diff
@@ -1,57 +1,9 @@
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.134949 ttr.aws.utils.s3-0.5.5/
--rw-r--r--   0 javl      (1000) javl      (1000)      830 2020-12-18 23:12:39.000000 ttr.aws.utils.s3-0.5.5/.proclamation.json
--rw-rw-r--   0 javl      (1000) javl      (1000)      436 2016-08-16 00:32:09.000000 ttr.aws.utils.s3-0.5.5/.pydevproject
--rw-rw-r--   0 javl      (1000) javl      (1000)     2134 2018-08-21 15:02:49.000000 ttr.aws.utils.s3-0.5.5/.s3lsversrc
--rw-rw-r--   0 javl      (1000) javl      (1000)      250 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/AUTHORS
--rw-r--r--   0 javl      (1000) javl      (1000)     4691 2023-06-30 20:25:11.000000 ttr.aws.utils.s3-0.5.5/CHANGELOG.md
--rw-rw-r--   0 javl      (1000) javl      (1000)     3296 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ChangeLog
--rw-rw-r--   0 javl      (1000) javl      (1000)      446 2020-12-18 23:40:39.000000 ttr.aws.utils.s3-0.5.5/HACKING.txt
--rw-rw-r--   0 javl      (1000) javl      (1000)     1590 2017-05-09 23:34:02.000000 ttr.aws.utils.s3-0.5.5/LICENSE.rst
--rw-r--r--   0 javl      (1000) javl      (1000)    10642 2023-06-30 20:46:24.138949 ttr.aws.utils.s3-0.5.5/PKG-INFO
--rw-rw-r--   0 javl      (1000) javl      (1000)     9634 2020-12-19 18:20:31.000000 ttr.aws.utils.s3-0.5.5/README.rst
--rw-rw-r--   0 javl      (1000) javl      (1000)      902 2016-08-16 00:32:49.000000 ttr.aws.utils.s3-0.5.5/TODO.rst
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.118949 ttr.aws.utils.s3-0.5.5/changes/
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.126949 ttr.aws.utils.s3-0.5.5/changes/bugfixes/
--rw-r--r--   0 javl      (1000) javl      (1000)       12 2020-12-19 00:10:24.000000 ttr.aws.utils.s3-0.5.5/changes/bugfixes/.gitignore
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.126949 ttr.aws.utils.s3-0.5.5/changes/docs/
--rw-r--r--   0 javl      (1000) javl      (1000)       12 2020-12-18 23:11:22.000000 ttr.aws.utils.s3-0.5.5/changes/docs/.gitignore
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.126949 ttr.aws.utils.s3-0.5.5/changes/features/
--rw-r--r--   0 javl      (1000) javl      (1000)       12 2020-12-18 23:11:16.000000 ttr.aws.utils.s3-0.5.5/changes/features/.gitignore
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.126949 ttr.aws.utils.s3-0.5.5/changes/internals/
--rw-r--r--   0 javl      (1000) javl      (1000)       12 2020-12-18 23:11:06.000000 ttr.aws.utils.s3-0.5.5/changes/internals/.gitignore
--rw-r--r--   0 javl      (1000) javl      (1000)    12505 2018-08-21 19:55:29.000000 ttr.aws.utils.s3-0.5.5/pylintrc
--rw-r--r--   0 javl      (1000) javl      (1000)       68 2023-06-30 20:18:03.000000 ttr.aws.utils.s3-0.5.5/requirements.txt
--rw-r--r--   0 javl      (1000) javl      (1000)     1153 2023-06-30 20:46:24.138949 ttr.aws.utils.s3-0.5.5/setup.cfg
--rw-rw-r--   0 javl      (1000) javl      (1000)      106 2017-05-09 23:34:02.000000 ttr.aws.utils.s3-0.5.5/setup.py
--rw-r--r--   0 javl      (1000) javl      (1000)       30 2023-06-30 20:18:03.000000 ttr.aws.utils.s3-0.5.5/test_requirements.txt
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.126949 ttr.aws.utils.s3-0.5.5/tests/
--rw-rw-r--   0 javl      (1000) javl      (1000)     1847 2020-06-23 18:04:12.000000 ttr.aws.utils.s3-0.5.5/tests/test_fname_factory.py
--rw-rw-r--   0 javl      (1000) javl      (1000)     1130 2019-02-27 19:42:31.000000 ttr.aws.utils.s3-0.5.5/tests/test_from_to.py
--rw-rw-r--   0 javl      (1000) javl      (1000)     1852 2017-05-09 23:34:02.000000 ttr.aws.utils.s3-0.5.5/tests/test_parsetime.py
--rw-r--r--   0 javl      (1000) javl      (1000)      379 2023-06-30 20:20:10.000000 ttr.aws.utils.s3-0.5.5/tox.ini
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.126949 ttr.aws.utils.s3-0.5.5/ttr/
--rw-r--r--   0 javl      (1000) javl      (1000)       56 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/__init__.py
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.134949 ttr.aws.utils.s3-0.5.5/ttr/aws/
--rw-r--r--   0 javl      (1000) javl      (1000)       56 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/__init__.py
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.134949 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/
--rw-r--r--   0 javl      (1000) javl      (1000)       56 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/__init__.py
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.134949 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/
--rw-rw-r--   0 javl      (1000) javl      (1000)        0 2017-05-09 23:34:02.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/__init__.py
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.134949 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/cli/
--rw-rw-r--   0 javl      (1000) javl      (1000)        0 2017-05-15 19:33:23.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/cli/__init__.py
--rw-rw-r--   0 javl      (1000) javl      (1000)     1733 2017-05-09 23:34:02.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/cli/chart.html
--rw-r--r--   0 javl      (1000) javl      (1000)     3568 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/cli/getvers.py
--rw-r--r--   0 javl      (1000) javl      (1000)     8353 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/cli/lsvers.py
--rw-r--r--   0 javl      (1000) javl      (1000)     3291 2023-06-30 19:47:14.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/cli/tmpgen.py
--rw-r--r--   0 javl      (1000) javl      (1000)     4925 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/saver.py
--rw-r--r--   0 javl      (1000) javl      (1000)     2021 2023-06-29 14:57:11.000000 ttr.aws.utils.s3-0.5.5/ttr/aws/utils/s3/utils.py
-drwxr-xr-x   0 javl      (1000) javl      (1000)        0 2023-06-30 20:46:24.134949 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/
--rw-r--r--   0 javl      (1000) javl      (1000)    10642 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/PKG-INFO
--rw-r--r--   0 javl      (1000) javl      (1000)     1044 2023-06-30 20:46:24.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/SOURCES.txt
--rw-r--r--   0 javl      (1000) javl      (1000)        1 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/dependency_links.txt
--rw-r--r--   0 javl      (1000) javl      (1000)      158 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/entry_points.txt
--rw-r--r--   0 javl      (1000) javl      (1000)       26 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/namespace_packages.txt
--rw-r--r--   0 javl      (1000) javl      (1000)        1 2020-12-19 21:08:02.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/not-zip-safe
--rw-r--r--   0 javl      (1000) javl      (1000)       46 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/pbr.json
--rw-r--r--   0 javl      (1000) javl      (1000)       68 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/requires.txt
--rw-r--r--   0 javl      (1000) javl      (1000)        4 2023-06-30 20:46:21.000000 ttr.aws.utils.s3-0.5.5/ttr.aws.utils.s3.egg-info/top_level.txt
+-rw-r--r--   0        0        0      250 2023-06-30 20:46:21.594945 ttr_aws_utils_s3-0.6.0/AUTHORS
+-rw-r--r--   0        0        0     1590 2017-05-09 23:34:02.826309 ttr_aws_utils_s3-0.6.0/LICENSE.rst
+-rw-r--r--   0        0        0     9640 2023-07-01 22:31:08.760778 ttr_aws_utils_s3-0.6.0/README.rst
+-rw-r--r--   0        0        0      283 2023-07-01 22:25:59.534302 ttr_aws_utils_s3-0.6.0/noxfile.py
+-rw-r--r--   0        0        0     1587 2023-07-01 22:37:07.163274 ttr_aws_utils_s3-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1847 2020-06-23 18:04:12.897439 ttr_aws_utils_s3-0.6.0/tests/test_fname_factory.py
+-rw-r--r--   0        0        0     1130 2019-02-27 19:42:31.563499 ttr_aws_utils_s3-0.6.0/tests/test_from_to.py
+-rw-r--r--   0        0        0     1852 2017-05-09 23:34:02.830309 ttr_aws_utils_s3-0.6.0/tests/test_parsetime.py
+-rw-r--r--   0        0        0    10370 1970-01-01 00:00:00.000000 ttr_aws_utils_s3-0.6.0/PKG-INFO
```

### Comparing `ttr.aws.utils.s3-0.5.5/LICENSE.rst` & `ttr_aws_utils_s3-0.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ttr.aws.utils.s3-0.5.5/PKG-INFO` & `ttr_aws_utils_s3-0.6.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,28 @@
-Metadata-Version: 2.1
-Name: ttr.aws.utils.s3
-Version: 0.5.5
-Summary: CLI to list and fetch objects from versioned S3 buckets. Plus get tmp url.
-Home-page: https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
-Author: Jan Vlcinsky
-Author-email: jan.vlcinsky@tamtamresearch.com
-License: BSD
-Keywords: aws,s3
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Communications :: File Sharing
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: System :: Archiving :: Backup
-Classifier: Topic :: System :: Recovery Tools
-Classifier: Topic :: Utilities
-License-File: LICENSE.rst
-License-File: AUTHORS
-
 ============
 AWS Utils S3
 ============
 
 Tools to list and fetch objects from versioned AWS_ S3_ bucket:
 
 * `s3lsvers`: List object versions, see versioning_
 * `s3getvers`: Fetch specified object versions
 * `s3tmpgen`: Generate temporary url links to objects
 
 .. contents:: Table of Contents
 
 Installation
 ============
-::
+Using `pip`::
 
   $ pip install ttr.aws.utils.s3
 
-Other methods (pipx, easy_install, setup.py) work too.
+Using `pipx`::
+
+  $ pipx install ttr.aws.utils.s3
     
 Quick start
 ===========
 We want to fetch versions of feed in bucket `mybucket` named `my/versioned/feed.xml`
 
 1. Configure AWSCLI credentials to allow access to your buckets and objects. E.g. using `AWS_DEFAULT_PROFILE`. See AWS_config_.
 
@@ -271,8 +247,7 @@
 If you configure profiles, you may use switch `-profile` when calling the commands.
 
 
 .. _AWS: http://aws.amazon.com/
 .. _S3: http://aws.amazon.com/s3/
 .. _versioning: http://aws.amazon.com/about-aws/whats-new/2010/02/08/versioning-feature-for-amazon-s3-now-available/
 .. _AWS_config: http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html
-
```

### Comparing `ttr.aws.utils.s3-0.5.5/README.rst` & `ttr_aws_utils_s3-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,49 @@
+Metadata-Version: 2.1
+Name: ttr.aws.utils.s3
+Version: 0.6.0
+Summary: CLI to list and fetch objects from versioned S3 buckets. Plus get tmp url.
+Keywords: aws s3
+Home-page: https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
+Author: Jan Vlcinsky
+Author-Email: Unknown <jan.vlcinsky@tamtamresearch.com>
+License: BSD
+Project-URL: Homepage, https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
+Requires-Python: >=3.8
+Requires-Dist: PyYAML==6.0
+Requires-Dist: boto3==1.26.165
+Requires-Dist: plac==1.3.5
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: pytz
+Requires-Dist: pendulum==2.1.2; extra == "test"
+Requires-Dist: pytest==7.4.0; extra == "test"
+Provides-Extra: test
+Description-Content-Type: text/x-rst
+
 ============
 AWS Utils S3
 ============
 
 Tools to list and fetch objects from versioned AWS_ S3_ bucket:
 
 * `s3lsvers`: List object versions, see versioning_
 * `s3getvers`: Fetch specified object versions
 * `s3tmpgen`: Generate temporary url links to objects
 
 .. contents:: Table of Contents
 
 Installation
 ============
-::
+Using `pip`::
 
   $ pip install ttr.aws.utils.s3
 
-Other methods (pipx, easy_install, setup.py) work too.
+Using `pipx`::
+
+  $ pipx install ttr.aws.utils.s3
     
 Quick start
 ===========
 We want to fetch versions of feed in bucket `mybucket` named `my/versioned/feed.xml`
 
 1. Configure AWSCLI credentials to allow access to your buckets and objects. E.g. using `AWS_DEFAULT_PROFILE`. See AWS_config_.
```

### Comparing `ttr.aws.utils.s3-0.5.5/tests/test_fname_factory.py` & `ttr_aws_utils_s3-0.6.0/tests/test_fname_factory.py`

 * *Files identical despite different names*

### Comparing `ttr.aws.utils.s3-0.5.5/tests/test_from_to.py` & `ttr_aws_utils_s3-0.6.0/tests/test_from_to.py`

 * *Files identical despite different names*

### Comparing `ttr.aws.utils.s3-0.5.5/tests/test_parsetime.py` & `ttr_aws_utils_s3-0.6.0/tests/test_parsetime.py`

 * *Files identical despite different names*

