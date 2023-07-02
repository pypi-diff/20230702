# Comparing `tmp/c4p-2023.7.1.tar.gz` & `tmp/c4p-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4p-2023.7.1.tar", last modified: Sun Jul  2 04:25:58 2023, max compression
+gzip compressed data, was "c4p-2023.7.2.tar", last modified: Sun Jul  2 04:56:38 2023, max compression
```

## Comparing `c4p-2023.7.1.tar` & `c4p-2023.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:25:58.919653 c4p-2023.7.1/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.1/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-02 04:25:58.918940 c4p-2023.7.1/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.1/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:25:58.913683 c4p-2023.7.1/c4p/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.1/c4p/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1074 2023-07-02 04:08:18.000000 c4p-2023.7.1/c4p/case.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7925 2023-07-02 04:13:46.000000 c4p-2023.7.1/c4p/runoff.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1718 2023-07-02 02:31:49.000000 c4p-2023.7.1/c4p/utils.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:25:58.918122 c4p-2023.7.1/c4p.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-02 04:25:58.914490 c4p-2023.7.1/c4p.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      241 2023-07-02 04:25:58.915197 c4p-2023.7.1/c4p.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-02 04:25:58.915862 c4p-2023.7.1/c4p.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.1/c4p.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-02 04:25:58.917504 c4p-2023.7.1/c4p.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-02 04:25:58.918227 c4p-2023.7.1/c4p.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-02 04:25:58.919775 c4p-2023.7.1/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      880 2023-07-02 03:43:35.000000 c4p-2023.7.1/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:56:38.756313 c4p-2023.7.2/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.2/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-02 04:56:38.755565 c4p-2023.7.2/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.2/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:56:38.750680 c4p-2023.7.2/c4p/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.2/c4p/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1074 2023-07-02 04:08:18.000000 c4p-2023.7.2/c4p/case.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7947 2023-07-02 04:54:01.000000 c4p-2023.7.2/c4p/runoff.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1718 2023-07-02 02:31:49.000000 c4p-2023.7.2/c4p/utils.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:56:38.754830 c4p-2023.7.2/c4p.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-02 04:56:38.751490 c4p-2023.7.2/c4p.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      241 2023-07-02 04:56:38.752111 c4p-2023.7.2/c4p.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-02 04:56:38.752814 c4p-2023.7.2/c4p.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.2/c4p.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-02 04:56:38.754207 c4p-2023.7.2/c4p.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-02 04:56:38.754930 c4p-2023.7.2/c4p.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-02 04:56:38.756438 c4p-2023.7.2/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      880 2023-07-02 04:40:45.000000 c4p-2023.7.2/setup.py
```

### Comparing `c4p-2023.7.1/LICENSE` & `c4p-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1/PKG-INFO` & `c4p-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4p
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: c4p: CESM for Paleo
 Home-page: https://github.com/fzhu2e/cesm4paleo
 Author: Feng Zhu, Jiang Zhu
 Author-email: fengzhu@ucar.edu, jiangzhu@ucar.edu
 License: MIT
 Keywords: CESM,paleoclimate
 Classifier: Natural Language :: English
```

### Comparing `c4p-2023.7.1/c4p/case.py` & `c4p-2023.7.2/c4p/case.py`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1/c4p/runoff.py` & `c4p-2023.7.2/c4p/runoff.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 
 class Runoff:
     def __init__(self, grids_dirpath=None, path_create_ESMF_map_sh=None, **kwargs):
         for k, v in kwargs.items():
             self.__dict__[k] = v
 
         self.grids_dirpath='/glade/p/cesmdata/inputdata/share/scripgrids' if grids_dirpath is None else grids_dirpath
-        self.path_create_ESMF_map_sh=os.path.join(cwd, '../src/rof/create_ESMF_map.sh') if path_create_ESMF_map_sh is None else path_create_ESMF_map_sh
+        self.path_create_ESMF_map_sh=os.path.join(cwd, './src/rof/create_ESMF_map.sh') if path_create_ESMF_map_sh is None else path_create_ESMF_map_sh
 
         for k, v in self.__dict__.items():
             utils.p_success(f'>>> Runoff.{k}: {v}')
         
-    def prep_topo(self, topo_path, path_create_topo_ncl=os.path.join(cwd, '../src/rof/create-topo_1x1deg.ncl')):
+    def prep_topo(self, topo_path, path_create_topo_ncl=os.path.join(cwd, './src/rof/create-topo_1x1deg.ncl')):
         # Step 19
         utils.p_header('>>> Prep topo file at proper resolution ...')
         fpath = utils.copy(path_create_topo_ncl)
         utils.replace_str(
             fpath,
             {
                 '<casename>': self.casename,
                 '<input_topo-bath_filename>': topo_path,
             },
         )
         utils.run_shell(f'source $LMOD_ROOT/lmod/init/zsh && module load ncl && ncl {fpath}', timeout=3)
 
     def gen_runoff(self,
-            path_rdirc_template_csh=os.path.join(cwd, '../src/rof/rdirc_template.csh'),
-            path_topo2rdirc_sed_f90=os.path.join(cwd, '../src/rof/topo2rdirc_sed.F90'),
-            path_Makefile=os.path.join(cwd, '../src/rof/Makefile'),
+            path_rdirc_template_csh=os.path.join(cwd, './src/rof/rdirc_template.csh'),
+            path_topo2rdirc_sed_f90=os.path.join(cwd, './src/rof/topo2rdirc_sed.F90'),
+            path_Makefile=os.path.join(cwd, './src/rof/Makefile'),
         ):
         # Step 20
         utils.p_header('>>> Generate runoff data from topo inputs ...')
         fpath_new = utils.copy(path_rdirc_template_csh, f'./rdirc_{self.casename}.csh')
         utils.replace_str(
             fpath_new,
             {
@@ -63,28 +63,29 @@
                 'LIB_NETCDF = -L/glade/apps/opt/netcdf/4.2/intel/default/lib -lnetcdf': f'LIB_NETCDF = -L{self.lib_netcdf} -lnetcdff',
                 'INC_NETCDF = -I/glade/apps/opt/netcdf/4.2/intel/default/include': f'INC_NETCDF = -I{self.inc_netcdf}',
             },
         )
         utils.exec_script(fpath_new)
 
     def plot_runoff(self, topo_path,
-            path_plotrdirc_csh=os.path.join(cwd, '../src/rof/plotrdirc.csh'),
-            path_plotrdirc_ncl=os.path.join(cwd, '../src/rof/plot_rdirc.ncl'),
+            path_plotrdirc_csh=os.path.join(cwd, './src/rof/plotrdirc.csh'),
+            path_plotrdirc_ncl=os.path.join(cwd, './src/rof/plot_rdirc.ncl'),
         ):
         # Step 21
         utils.p_header('>>> Plot runoff ...')
         fpath = utils.copy(path_plotrdirc_csh)
         utils.replace_str(
             fpath,
             {
                 '<casename>': self.casename,
                 '<topography-bathymetry_file>': os.path.basename(topo_path),
             },
         )
         utils.copy(path_plotrdirc_ncl)
+        utils.run_shell(f'chmod +x {fpath}')
         utils.run_shell(f'source $LMOD_ROOT/lmod/init/zsh && module load ncl && ./{fpath}', timeout=3)
         display(
             Image('./rdirc_miocene_topo_pollard_antscape_dolan_0.5x0.5.nc.png')
         )
 
     def runoff2nc(self, input=None, output=None, res='1x1',
                   meta_user='Feng Zhu', meta_date=date.today().strftime('%Y%m%d')):
@@ -137,16 +138,16 @@
         ds.attrs['history'] = f'created by {meta_user} {meta_date}'
         ds.attrs['source'] = input
 
         # Save dataset to netCDF file
         ds.to_netcdf(output)
 
     def runoff2ocn_p1(self, ocn_scrp_path,
-            path_runoff_map=os.path.join(cwd, '../src/rof/runoff_map_1deg'),
-            path_runoff_map_template_nml=os.path.join(cwd, '../src/rof/runoff_map.1x1.template.nml'),
+            path_runoff_map=os.path.join(cwd, './src/rof/runoff_map_1deg'),
+            path_runoff_map_template_nml=os.path.join(cwd, './src/rof/runoff_map.1x1.template.nml'),
             meta_date=date.today().strftime('%Y%m%d'),
             ocnres=None,
         ):
         # Step 25
         utils.p_header('>>> Create runoff to ocean mapping file (part 1) ...')
         os.environ['ESMFBIN_PATH'] = self.esmfbin_path
         ocnres = f'gx1{self.casename}' if ocnres is None else ocnres
@@ -159,35 +160,33 @@
                 './<SCRIP_mapping_file>': ocn_scrp_path,
                 '<ocnres>': ocnres,
                 '<date>': meta_date,
             },
         )
         utils.run_shell(f'ln -s {fpath_new} ./runoff_map.nml')
         utils.exec_script(fpath)
+        self.ocn_scrp_path = ocn_scrp_path
 
-    def runoff2ocn_p2(self, ocn_scrp_path,
-            grids_dirpath='/glade/p/cesmdata/inputdata/share/scripgrids',
-            path_create_ESMF_map_sh=os.path.join(cwd, '../src/rof/create_ESMF_map.sh'),
-        ):
+    def runoff2ocn_p2(self, fsrc_fname='1x1d.nc'):
         # Step 26
         utils.p_header('>>> Create runoff to ocean mapping file (part 2) ...')
-        fpath = utils.copy(path_create_ESMF_map_sh)
+        fpath = utils.copy(self.path_create_ESMF_map_sh)
         ocnres = f'gx1{self.casename}'
-        fsrc = os.path.join(grids_dirpath, '1x1d.nc')
-        fdst = ocn_scrp_path
+        fsrc = os.path.join(self.grids_dirpath, fsrc_fname)
+        fdst = self.ocn_scrp_path
         utils.exec_script(fpath, args=f'-fsrc {fsrc} -nsrc r1_nomask -fdst {fdst} -ndst {ocnres} -map aave')
 
-    def runoff2land(self):
+    def runoff2land(self, fsrc_fname='fv1.9x2.5_141008.nc', fdst_fname='1x1d_lonshift.nc'):
         # Step 27
         utils.p_header('>>> Create runoff to land mapping files - needed if rof at 1deg rather than 0.5 deg ...')
         fpath = utils.copy(self.path_create_ESMF_map_sh)
-        fsrc = os.path.join(self.grids_dirpath, 'fv1.9x2.5_141008.nc')
-        fdst = os.path.join(self.grids_dirpath, '1x1d_lonshift.nc')
+        fsrc = os.path.join(self.grids_dirpath, fsrc_fname)
+        fdst = os.path.join(self.grids_dirpath, fdst_fname)
         utils.exec_script(fpath, args=f'-fsrc {fsrc} -nsrc r19_nomask -fdst {fdst} -ndst r1x1 -map aave')
 
-    def land2runoff(self):
+    def land2runoff(self, fsrc_fname='1x1d_lonshift.nc', fdst_fname='fv1.9x2.5_141008.nc'):
         # Step 27
         utils.p_header('>>> Create land to runoff mapping files - needed if rof at 1deg rather than 0.5 deg ...')
         fpath = utils.copy(self.path_create_ESMF_map_sh)
-        fsrc = os.path.join(self.grids_dirpath, '1x1d_lonshift.nc')
-        fdst = os.path.join(self.grids_dirpath, 'fv1.9x2.5_141008.nc')
+        fsrc = os.path.join(self.grids_dirpath, fsrc_fname)
+        fdst = os.path.join(self.grids_dirpath, fdst_fname)
         utils.exec_script(fpath, args=f'-fsrc {fsrc} -nsrc r19_nomask -fdst {fdst} -ndst r1x1 -map aave')
```

### Comparing `c4p-2023.7.1/c4p/utils.py` & `c4p-2023.7.2/c4p/utils.py`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1/c4p.egg-info/PKG-INFO` & `c4p-2023.7.2/c4p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4p
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: c4p: CESM for Paleo
 Home-page: https://github.com/fzhu2e/cesm4paleo
 Author: Feng Zhu, Jiang Zhu
 Author-email: fengzhu@ucar.edu, jiangzhu@ucar.edu
 License: MIT
 Keywords: CESM,paleoclimate
 Classifier: Natural Language :: English
```

### Comparing `c4p-2023.7.1/setup.py` & `c4p-2023.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='c4p',  # required
-    version='2023.7.1',
+    version='2023.7.2',
     description='c4p: CESM for Paleo',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Jiang Zhu',
     author_email='fengzhu@ucar.edu, jiangzhu@ucar.edu',
     url='https://github.com/fzhu2e/cesm4paleo',
     packages=find_packages(),
```

