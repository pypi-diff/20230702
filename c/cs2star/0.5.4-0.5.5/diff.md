# Comparing `tmp/cs2star-0.5.4.tar.gz` & `tmp/cs2star-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2star-0.5.4.tar", last modified: Wed Mar 29 12:17:44 2023, max compression
+gzip compressed data, was "cs2star-0.5.5.tar", last modified: Sun Jul  2 08:26:12 2023, max compression
```

## Comparing `cs2star-0.5.4.tar` & `cs2star-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-03-29 12:17:44.594378 cs2star-0.5.4/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.5.4/.gitignore
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.5.4/LICENSE
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-03-29 12:17:44.594378 cs2star-0.5.4/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.5.4/README.md
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-03-29 12:17:44.594378 cs2star-0.5.4/cs2star/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.5.4/cs2star/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star/_version.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    10631 2022-12-20 12:49:19.000000 cs2star-0.5.4/cs2star/cs2star.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.5.4/cs2star/job_parser.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-03-29 12:17:44.594378 cs2star-0.5.4/cs2star.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star.egg-info/entry_points.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-03-29 12:17:44.000000 cs2star-0.5.4/cs2star.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2022-12-12 16:09:00.000000 cs2star-0.5.4/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-03-29 12:17:44.594378 cs2star-0.5.4/setup.cfg
+drwxr-xr-x   0 brisvag   (1000) brisvag   (1000)        0 2023-07-02 08:26:12.132649 cs2star-0.5.5/
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)       12 2023-07-01 16:41:09.000000 cs2star-0.5.5/.gitignore
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)    35149 2023-07-01 16:41:09.000000 cs2star-0.5.5/LICENSE
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)     2692 2023-07-02 08:26:12.129315 cs2star-0.5.5/PKG-INFO
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)     2167 2023-07-01 16:41:09.000000 cs2star-0.5.5/README.md
+drwxr-xr-x   0 brisvag   (1000) brisvag   (1000)        0 2023-07-02 08:26:12.129315 cs2star-0.5.5/cs2star/
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)        0 2023-07-01 16:41:09.000000 cs2star-0.5.5/cs2star/__init__.py
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)      160 2023-07-02 08:26:11.000000 cs2star-0.5.5/cs2star/_version.py
+-rwxr-xr-x   0 brisvag   (1000) brisvag   (1000)    11036 2023-07-02 08:22:29.000000 cs2star-0.5.5/cs2star/cs2star.py
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)     3422 2023-07-01 16:41:09.000000 cs2star-0.5.5/cs2star/job_parser.py
+drwxr-xr-x   0 brisvag   (1000) brisvag   (1000)        0 2023-07-02 08:26:12.129315 cs2star-0.5.5/cs2star.egg-info/
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)     2692 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/PKG-INFO
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)      312 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/SOURCES.txt
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)        1 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/dependency_links.txt
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)       49 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/entry_points.txt
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)       24 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/requires.txt
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)        8 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/top_level.txt
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)      841 2023-07-01 16:41:09.000000 cs2star-0.5.5/pyproject.toml
+-rw-r--r--   0 brisvag   (1000) brisvag   (1000)       38 2023-07-02 08:26:12.132649 cs2star-0.5.5/setup.cfg
```

### Comparing `cs2star-0.5.4/LICENSE` & `cs2star-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2star-0.5.4/PKG-INFO` & `cs2star-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.5.4
+Version: 0.5.5
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.5.4/README.md` & `cs2star-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `cs2star-0.5.4/cs2star/cs2star.py` & `cs2star-0.5.5/cs2star/cs2star.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,24 +120,36 @@
             logfile.write(cleandoc(f'''
                 # this directory was converted from cryosparc with cs2star.py. Command:
                 cs2star {" ".join(sys.argv[1:])}
             ''') + '\n')
             logfile.write(log)
 
     if len(particles) != len(particles_passthrough):
-        if len(particles_passthrough) == 1:
+        if len(particles_passthrough) == 0:
+            pass
+        elif len(particles_passthrough) == 1:
             particles_passthrough = particles_passthrough * len(particles)
         else:
-            raise ValueError('Number of passthrough files and particle files is incompatible')
+            raise ValueError(
+                'Number of passthrough files and particle files is incompatible:\n'
+                f'particles: {particles}\n'
+                f'passthroughs: {particles_passthrough}'
+            )
 
     if len(micrographs) != len(micrographs_passthrough):
-        if len(micrographs_passthrough) == 1:
+        if len(micrographs_passthrough) == 0:
+            pass
+        elif len(micrographs_passthrough) == 1:
             micrographs_passthrough = micrographs_passthrough * len(micrographs)
         else:
-            raise ValueError('Number of passthrough files and particle files is incompatible')
+            raise ValueError(
+                'Number of passthrough files and micrographs files is incompatible:\n'
+                f'micrographs: {micrographs}\n'
+                f'passthroughs: {micrographs_passthrough}'
+            )
 
     if dest_star.is_file() and overwrite == 0:
         raise click.UsageError('particle file already exists. To overwrite, use -f')
     if dest_star.is_file() and overwrite == 0:
         raise click.UsageError('micrographs file already exists. To overwrite, use -f')
 
     with Progress() as progress:
```

### Comparing `cs2star-0.5.4/cs2star/job_parser.py` & `cs2star-0.5.5/cs2star/job_parser.py`

 * *Files identical despite different names*

### Comparing `cs2star-0.5.4/cs2star.egg-info/PKG-INFO` & `cs2star-0.5.5/cs2star.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.5.4
+Version: 0.5.5
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.5.4/pyproject.toml` & `cs2star-0.5.5/pyproject.toml`

 * *Files identical despite different names*

