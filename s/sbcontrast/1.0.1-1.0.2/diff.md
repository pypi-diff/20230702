# Comparing `tmp/sbcontrast-1.0.1.tar.gz` & `tmp/sbcontrast-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbcontrast-1.0.1.tar", last modified: Sat Jul 30 19:25:47 2022, max compression
+gzip compressed data, was "sbcontrast-1.0.2.tar", last modified: Sun Jul  2 12:52:57 2023, max compression
```

## Comparing `sbcontrast-1.0.1.tar` & `sbcontrast-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 michaelkeim   (501) staff       (20)        0 2022-07-30 19:25:47.474117 sbcontrast-1.0.1/
--rw-r--r--   0 michaelkeim   (501) staff       (20)     1108 2022-07-29 18:40:46.000000 sbcontrast-1.0.1/LICENSE.txt
--rw-r--r--   0 michaelkeim   (501) staff       (20)     2492 2022-07-30 19:25:47.474176 sbcontrast-1.0.1/PKG-INFO
--rw-r--r--   0 michaelkeim   (501) staff       (20)     1936 2022-07-30 19:17:02.000000 sbcontrast-1.0.1/README.txt
-drwxr-xr-x   0 michaelkeim   (501) staff       (20)        0 2022-07-30 19:25:47.473407 sbcontrast-1.0.1/sbcontrast/
--rw-r--r--   0 michaelkeim   (501) staff       (20)       34 2022-07-29 23:38:18.000000 sbcontrast-1.0.1/sbcontrast/__init__.py
--rw-r--r--   0 michaelkeim   (501) staff       (20)       57 2022-07-29 23:28:49.000000 sbcontrast-1.0.1/sbcontrast/__main__.py
--rw-r--r--   0 michaelkeim   (501) staff       (20)     9607 2022-07-30 19:21:58.000000 sbcontrast-1.0.1/sbcontrast/main.py
-drwxr-xr-x   0 michaelkeim   (501) staff       (20)        0 2022-07-30 19:25:47.474025 sbcontrast-1.0.1/sbcontrast.egg-info/
--rw-r--r--   0 michaelkeim   (501) staff       (20)     2492 2022-07-30 19:25:47.000000 sbcontrast-1.0.1/sbcontrast.egg-info/PKG-INFO
--rw-r--r--   0 michaelkeim   (501) staff       (20)      312 2022-07-30 19:25:47.000000 sbcontrast-1.0.1/sbcontrast.egg-info/SOURCES.txt
--rw-r--r--   0 michaelkeim   (501) staff       (20)        1 2022-07-30 19:25:47.000000 sbcontrast-1.0.1/sbcontrast.egg-info/dependency_links.txt
--rw-r--r--   0 michaelkeim   (501) staff       (20)       51 2022-07-30 19:25:47.000000 sbcontrast-1.0.1/sbcontrast.egg-info/entry_points.txt
--rw-r--r--   0 michaelkeim   (501) staff       (20)       14 2022-07-30 19:25:47.000000 sbcontrast-1.0.1/sbcontrast.egg-info/requires.txt
--rw-r--r--   0 michaelkeim   (501) staff       (20)       11 2022-07-30 19:25:47.000000 sbcontrast-1.0.1/sbcontrast.egg-info/top_level.txt
--rw-r--r--   0 michaelkeim   (501) staff       (20)       80 2022-07-30 19:25:47.474367 sbcontrast-1.0.1/setup.cfg
--rw-r--r--   0 michaelkeim   (501) staff       (20)      806 2022-07-30 19:25:39.000000 sbcontrast-1.0.1/setup.py
+drwxr-xr-x   0 michaelkeim   (501) staff       (20)        0 2023-07-02 12:52:57.091836 sbcontrast-1.0.2/
+-rw-r--r--   0 michaelkeim   (501) staff       (20)     1108 2022-07-29 18:40:46.000000 sbcontrast-1.0.2/LICENSE.txt
+-rw-r--r--   0 michaelkeim   (501) staff       (20)     2473 2023-07-02 12:52:57.091903 sbcontrast-1.0.2/PKG-INFO
+-rw-r--r--   0 michaelkeim   (501) staff       (20)     1936 2022-07-30 19:17:02.000000 sbcontrast-1.0.2/README.txt
+drwxr-xr-x   0 michaelkeim   (501) staff       (20)        0 2023-07-02 12:52:57.090968 sbcontrast-1.0.2/sbcontrast/
+-rw-r--r--   0 michaelkeim   (501) staff       (20)       34 2022-07-29 23:38:18.000000 sbcontrast-1.0.2/sbcontrast/__init__.py
+-rw-r--r--   0 michaelkeim   (501) staff       (20)       57 2022-07-29 23:28:49.000000 sbcontrast-1.0.2/sbcontrast/__main__.py
+-rw-r--r--   0 michaelkeim   (501) staff       (20)     9671 2023-07-02 12:45:14.000000 sbcontrast-1.0.2/sbcontrast/main.py
+drwxr-xr-x   0 michaelkeim   (501) staff       (20)        0 2023-07-02 12:52:57.091712 sbcontrast-1.0.2/sbcontrast.egg-info/
+-rw-r--r--   0 michaelkeim   (501) staff       (20)     2473 2023-07-02 12:52:57.000000 sbcontrast-1.0.2/sbcontrast.egg-info/PKG-INFO
+-rw-r--r--   0 michaelkeim   (501) staff       (20)      312 2023-07-02 12:52:57.000000 sbcontrast-1.0.2/sbcontrast.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelkeim   (501) staff       (20)        1 2023-07-02 12:52:57.000000 sbcontrast-1.0.2/sbcontrast.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelkeim   (501) staff       (20)       51 2023-07-02 12:52:57.000000 sbcontrast-1.0.2/sbcontrast.egg-info/entry_points.txt
+-rw-r--r--   0 michaelkeim   (501) staff       (20)       14 2023-07-02 12:52:57.000000 sbcontrast-1.0.2/sbcontrast.egg-info/requires.txt
+-rw-r--r--   0 michaelkeim   (501) staff       (20)       11 2023-07-02 12:52:57.000000 sbcontrast-1.0.2/sbcontrast.egg-info/top_level.txt
+-rw-r--r--   0 michaelkeim   (501) staff       (20)       80 2023-07-02 12:52:57.092106 sbcontrast-1.0.2/setup.cfg
+-rw-r--r--   0 michaelkeim   (501) staff       (20)      806 2023-07-02 12:40:33.000000 sbcontrast-1.0.2/setup.py
```

### Comparing `sbcontrast-1.0.1/LICENSE.txt` & `sbcontrast-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sbcontrast-1.0.1/PKG-INFO` & `sbcontrast-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sbcontrast
-Version: 1.0.1
+Version: 1.0.2
 Summary: Surface Brightness Limit Calculator
 Home-page: https://github.com/michaelkeim/sbcontrast/
 Download-URL: https://github.com/michaelkeim/sbcontrast/archive/master.tar.gz
 Author: Keim, M. A., van Dokkum, P., Li, J.
 Author-email: michael.keim@yale.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/plain
 License-File: LICENSE.txt
 
 Authors
@@ -53,8 +52,7 @@
 single pixel scale sbcontrast may diverge from the true rms due to
 correlations introduced by re-sampling.
 
 Citation
 --------
 We ask that users utilizing this tool please cite Keim et al. 2022
 (https://arxiv.org/pdf/2109.09778.pdf).
-
```

### Comparing `sbcontrast-1.0.1/README.txt` & `sbcontrast-1.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `sbcontrast-1.0.1/sbcontrast/main.py` & `sbcontrast-1.0.2/sbcontrast/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,27 +134,30 @@
 				bck_loc = np.delete(bck_loc.flatten(), 4)
 				im_fluct[j+1,i+1] = im_loc[j+1,i+1] - biweight_location(bck_loc, ignore_nan=True) \
 					if len(bck_loc[~np.isnan(bck_loc)]) > minback else np.nan
 
 	# Remove edge
 	im_fluct[:,[0,-1]] = im_fluct[[0,-1]] = np.nan
 
+	# Remove unreal image regions (e.g. unmasked edges)
+	im_fluct[im_fluct == 0] = np.nan
+
 	# Find limit
 	sig_adu = np.sqrt(biweight_midvariance(im_fluct, ignore_nan=True))*sigma/np.sqrt(1.125)
 
 	# For the standard deviation of standard deviation, see:
 	# https://stats.stackexchange.com/questions/631/standard-deviation-of-standard-deviation
 	dsig_adu = sig_adu / np.sqrt(2.*(im_fluct.size - 1.))
 
 	# Convert limit in ADU to magnitudes
 	sb_lim = zeropoint - 2.5*np.log10(sig_adu / pix_scale**2)
 	dsb_lim = 2.5*np.log10(1.+1./np.sqrt(im_fluct.size))
 
 	if verbose:
-			print('The {0:.1f}-sigma limit on {1} arcsec scales is {2:.4f} +- {3:.4f} mag/arcsec2.'.format(sigma, scale_arcsec, sb_lim, dsb_lim))
+			print('The {0:.1f}-sigma limit on {1} arcsec scales is {2:.4f} mag/arcsec2.'.format(sigma, scale_arcsec, sb_lim))
 
 	return (sb_lim, dsb_lim), (sig_adu, dsig_adu), [im_fluct, im_loc]
 
 # -----------------------------------------------------------------------------
 # Load Files and Run
 # -----------------------------------------------------------------------------
 
@@ -237,11 +240,7 @@
 	temp = sblimit(datai, datam, pix, zp, sigma=args.N, scale_arcsec=args.s)	
 
 	# Save Files
 	if args.fluctmap is not None:
 		np.save(args.fluctmap+'.npy', temp[2][0])
 	if args.binmap is not None:
 		np.save(args.binmap+'.npy', temp[2][1])
-
-
-
-
```

### Comparing `sbcontrast-1.0.1/sbcontrast.egg-info/PKG-INFO` & `sbcontrast-1.0.2/sbcontrast.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sbcontrast
-Version: 1.0.1
+Version: 1.0.2
 Summary: Surface Brightness Limit Calculator
 Home-page: https://github.com/michaelkeim/sbcontrast/
 Download-URL: https://github.com/michaelkeim/sbcontrast/archive/master.tar.gz
 Author: Keim, M. A., van Dokkum, P., Li, J.
 Author-email: michael.keim@yale.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/plain
 License-File: LICENSE.txt
 
 Authors
@@ -53,8 +52,7 @@
 single pixel scale sbcontrast may diverge from the true rms due to
 correlations introduced by re-sampling.
 
 Citation
 --------
 We ask that users utilizing this tool please cite Keim et al. 2022
 (https://arxiv.org/pdf/2109.09778.pdf).
-
```

### Comparing `sbcontrast-1.0.1/setup.py` & `sbcontrast-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.txt', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
 	name='sbcontrast',
 	packages=['sbcontrast'],
-	version='1.0.1',
+	version='1.0.2',
 	license='MIT',
 	description='Surface Brightness Limit Calculator',
 	long_description=long_description,
 	long_description_content_type="text/plain",
 	author='Keim, M. A., van Dokkum, P., Li, J.',
 	author_email='michael.keim@yale.edu',
 	entry_points={"console_scripts": ["sbcontrast = sbcontrast.main:sbc"]},
```

