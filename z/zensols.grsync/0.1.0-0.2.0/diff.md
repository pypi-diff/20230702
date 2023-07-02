# Comparing `tmp/zensols.grsync-0.1.0-py3-none-any.whl.zip` & `tmp/zensols.grsync-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 24448 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      226 b- defN 22-Sep-16 01:47 zensols/grsync/__init__.py
--rw-rw-r--  2.0 unx     2469 b- defN 22-Sep-16 01:47 zensols/grsync/bootstrap.py
--rw-rw-r--  2.0 unx     7063 b- defN 22-Sep-16 01:47 zensols/grsync/cli.py
--rw-rw-r--  2.0 unx     4207 b- defN 22-Sep-16 01:47 zensols/grsync/config.py
--rw-rw-r--  2.0 unx     5533 b- defN 22-Sep-16 01:47 zensols/grsync/distmng.py
--rw-rw-r--  2.0 unx     4233 b- defN 22-Sep-16 01:47 zensols/grsync/distribution.py
--rw-rw-r--  2.0 unx     6135 b- defN 22-Sep-16 01:47 zensols/grsync/domain.py
--rw-rw-r--  2.0 unx    14233 b- defN 22-Sep-16 01:47 zensols/grsync/freeze.py
--rw-rw-r--  2.0 unx     5110 b- defN 22-Sep-16 01:47 zensols/grsync/mover.py
--rw-rw-r--  2.0 unx     8860 b- defN 22-Sep-16 01:47 zensols/grsync/repospec.py
--rw-rw-r--  2.0 unx     6912 b- defN 22-Sep-16 01:47 zensols/grsync/thaw.py
--rw-rw-r--  2.0 unx     6106 b- defN 22-Sep-16 01:47 zensols.grsync-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-16 01:47 zensols.grsync-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       47 b- defN 22-Sep-16 01:47 zensols.grsync-0.1.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 22-Sep-16 01:47 zensols.grsync-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1327 b- defN 22-Sep-16 01:47 zensols.grsync-0.1.0.dist-info/RECORD
-16 files, 72568 bytes uncompressed, 22260 bytes compressed:  69.3%
+Zip file size: 25807 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx      245 b- defN 23-Jul-02 21:01 zensols/grsync/__init__.py
+-rw-rw-r--  2.0 unx     5874 b- defN 23-Jul-02 21:01 zensols/grsync/app.py
+-rw-rw-r--  2.0 unx     2374 b- defN 23-Jul-02 21:01 zensols/grsync/bootstrap.py
+-rw-rw-r--  2.0 unx      625 b- defN 23-Jul-02 21:01 zensols/grsync/cli.py
+-rw-rw-r--  2.0 unx     4317 b- defN 23-Jul-02 21:01 zensols/grsync/config.py
+-rw-rw-r--  2.0 unx     5660 b- defN 23-Jul-02 21:01 zensols/grsync/distmng.py
+-rw-rw-r--  2.0 unx     4231 b- defN 23-Jul-02 21:01 zensols/grsync/distribution.py
+-rw-rw-r--  2.0 unx     6228 b- defN 23-Jul-02 21:01 zensols/grsync/domain.py
+-rw-rw-r--  2.0 unx    14528 b- defN 23-Jul-02 21:01 zensols/grsync/freeze.py
+-rw-rw-r--  2.0 unx     5105 b- defN 23-Jul-02 21:01 zensols/grsync/mover.py
+-rw-rw-r--  2.0 unx     8844 b- defN 23-Jul-02 21:01 zensols/grsync/repospec.py
+-rw-rw-r--  2.0 unx     6912 b- defN 23-Jul-02 21:01 zensols/grsync/thaw.py
+-rw-rw-r--  2.0 unx     1093 b- defN 23-Jul-02 21:01 zensols/grsync/resources/app.conf
+-rw-rw-r--  2.0 unx     6326 b- defN 23-Jul-02 21:01 zensols.grsync-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-02 21:01 zensols.grsync-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       47 b- defN 23-Jul-02 21:01 zensols.grsync-0.2.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jul-02 21:01 zensols.grsync-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1494 b- defN 23-Jul-02 21:01 zensols.grsync-0.2.0.dist-info/RECORD
+18 files, 74010 bytes uncompressed, 23359 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: zensols/grsync/__init__.py
 Comment: 
 
+Filename: zensols/grsync/app.py
+Comment: 
+
 Filename: zensols/grsync/bootstrap.py
 Comment: 
 
 Filename: zensols/grsync/cli.py
 Comment: 
 
 Filename: zensols/grsync/config.py
@@ -27,23 +30,26 @@
 
 Filename: zensols/grsync/repospec.py
 Comment: 
 
 Filename: zensols/grsync/thaw.py
 Comment: 
 
-Filename: zensols.grsync-0.1.0.dist-info/METADATA
+Filename: zensols/grsync/resources/app.conf
+Comment: 
+
+Filename: zensols.grsync-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: zensols.grsync-0.1.0.dist-info/WHEEL
+Filename: zensols.grsync-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: zensols.grsync-0.1.0.dist-info/entry_points.txt
+Filename: zensols.grsync-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: zensols.grsync-0.1.0.dist-info/top_level.txt
+Filename: zensols.grsync-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zensols.grsync-0.1.0.dist-info/RECORD
+Filename: zensols.grsync-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zensols/grsync/__init__.py

```diff
@@ -3,8 +3,9 @@
 from .repospec import *
 from .bootstrap import *
 from .freeze import *
 from .distribution import *
 from .thaw import *
 from .mover import *
 from .distmng import *
+from .app import *
 from .cli import *
```

## zensols/grsync/bootstrap.py

```diff
@@ -1,18 +1,21 @@
+"""A utility class to create a bootstrapping script to install Python.
+
+"""
+__author__ = 'Paul Landes'
+
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class BootstrapGenerator(object):
-    """
-    Generate the script that creates the distribution on the target machine.
+    """Generate the script that creates the distribution on the target machine.
 
     """
-
     SCRIPT = """\
 #!/bin/sh
 
 if [ $# -eq 0 ] ; then
     echo "usage: $0 <python_dir> [grsync dir] [python<version>]"
     echo "where: python_dir is the bin directory where python is installed"
     echo "       grsync_dir is the distribution directory copied from the source"
@@ -32,43 +35,36 @@
     echo "setting python ver: $3"
     PYTHON_VER=$3
 else
     PYTHON_VER=$NATIVE_PYTHON_BIN_DIR
 fi
 
 PYTHON_DIR=${HOME}/opt/lib/python3
-PIP=${PYTHON_DIR}/bin/pip
-VIRTUAL_ENV=${NATIVE_PYTHON_BIN_DIR}/virtualenv
+PIP=${PYTHON_DIR}/bin/pip3
 PYTHON_PAR=`dirname $PYTHON_DIR`
 WHEELS_DIR=${GRSYNC_INST_DIR}/%(wheel_dir)s
 WHEELS=${WHEELS_DIR}/*.whl
 
 if [ -f ${PIP} ] ; then
     PIP=${PYTHON_DIR}/bin/pip3
 fi
 
 echo "GRSYNC_INST_DIR=${GRSYNC_INST_DIR}"
 echo "PYTHON_DIR=${PYTHON_DIR}"
 echo "PYTHON_VER=${PYTHON_VER}"
 echo "PIP=${PIP}"
-echo "VIRTUAL_ENV=${VIRTUAL_ENV}"
 echo "PYTHON_PAR=${PYTHON_PAR}"
 echo "WHEELS_DIR=${WHEELS_DIR}"
 echo "WHEELS=${WHEELS}"
 
-if [ ! -e "${VIRTUAL_ENV}" ] ; then
-    echo "virtual environment not installed: 'pip3 install virtualenv'"
-    exit 1
-fi
-
 echo "bootstrapping python env in ${PYTHON_DIR}, wheels: ${WHEELS}"
 
 rm -rf $PYTHON_PAR
 
-cmd="${VIRTUAL_ENV} -p ${PYTHON_VER} `basename ${PYTHON_DIR}`"
+cmd="${NATIVE_PYTHON_BIN_DIR}/bin/python3 -m venv --copies ${PYTHON_DIR}"
 
 echo "invoke $cmd"
 mkdir -p $PYTHON_PAR && \
     cd $PYTHON_PAR && \
     $cmd && \
     cd - || exit 1
```

## zensols/grsync/cli.py

```diff
@@ -1,167 +1,20 @@
-import logging
-from pathlib import Path
-from zensols.cli import OneConfPerActionOptionsCliEnv
-from zensols.grsync import (
-    AppConfig,
-    DistManager,
-    RepoSpec,
-)
-
-
-class InfoCli(object):
-    def __init__(self, config, fmt=None, repo_names=None, profiles=None):
-        self.config = config
-        self.fmt = fmt
-        if repo_names is not None:
-            self.repo_names = repo_names.split(',')
-        else:
-            self.repo_names = repo_names
-        self.profiles = profiles
-        self.dm = DistManager(self.config, profiles=self.profiles)
-
-    def info(self):
-        self.dm.discover_info()
-
-    def repos(self):
-        self.dm.print_repos(self.fmt)
-
-    def repo_info(self):
-        self.dm.print_repo_info(self.repo_names)
-
-
-class DistManagerCli(object):
-    def __init__(self, config=None, dist_dir=None, target_dir=None,
-                 move_dir=None, wheel_dependency='zensols.grsync',
-                 profiles=None, dir_reduce=False, repopref=None, dry_run=None):
-        self.dm = DistManager(config, dist_dir, target_dir,
-                              profiles=profiles, repo_preference=repopref,
-                              dry_run=dry_run)
-        self.wheel_dependency = wheel_dependency
-        self.dir_reduce = dir_reduce
-        if move_dir is None:
-            self.move_dir = None
-        else:
-            self.move_dir = Path(move_dir).expanduser().absolute()
-
-    def freeze(self):
-        self.dm.freeze(self.wheel_dependency)
-
-    def thaw(self):
-        self.dm.thaw()
-
-    def move(self):
-        self.dm.move(self.move_dir, self.dir_reduce)
-
-    def copy(self):
-        self.dm.copy()
-
-
-class ConfAppCommandLine(OneConfPerActionOptionsCliEnv):
-    """Command line entry point.
-
-    """
-    def __init__(self):
-        dist_dir_op = ['-d', '--distdir', False,
-                       {'dest': 'dist_dir',
-                        'metavar': 'DIRECTORY',
-                        'help': 'the location of build out distribution'}]
-        target_dir_op = ['-t', '--targetdir', False,
-                         {'dest': 'target_dir', 'metavar': 'DIRECTORY',
-                          'help': 'the location of build out target dir'}]
-        move_dir_op = ['-m', '--movedir', False,
-                       {'dest': 'move_dir', 'metavar': 'DIRECTORY',
-                        'help': 'the location of build out move dir'}]
-        wheel_dir_op = [None, '--wheeldep', False,
-                        {'dest': 'wheel_dependency',
-                         'default': 'zensols.grsync',
-                         'metavar': 'STRING',
-                         'help': 'used to create the wheel dep files'}]
-        rp_format_op = ['-f', '--format', False,
-                        {'dest': 'fmt',
-                         'default': '{path}',
-                         'metavar': 'STRING',
-                         'help':
-                         f'format string (i.e. {RepoSpec.DEFAULT_FORMAT})'}]
-        repo_name_op = ['-n', '--name', False,
-                        {'dest': 'repo_names',
-                         'metavar': 'STRING',
-                         'help': 'comma spearated list of repo names'}]
-        profile_op = ['-p', '--profiles', False,
-                      {'metavar': 'STRING',
-                       'help': 'comma spearated list of profiles in config'}]
-        repopref_op = ['-r', '--repopref', False,
-                       {'metavar': 'STRING',
-                        'help': 'the repository to make primary on thaw'}]
-        dry_run_op = [None, '--dryrun', False,
-                      {'dest': 'dry_run',
-                       'action': 'store_true', 'default': False,
-                       'help': 'do not do anything, just act like it'}]
-        dir_reduce_op = [None, '--reduce', False,
-                         {'dest': 'dir_reduce',
-                          'action': 'store_true', 'default': False,
-                          'help': 'remove empty directories'}]
-        cnf = {'executors':
-               [{'name': 'info',
-                 'executor': lambda params: InfoCli(**params),
-                 'actions': [{'name': 'info',
-                              'doc': 'pretty print discovery information'},
-                             {'name': 'repos',
-                              'doc': 'output all repository top level info',
-                              'opts': [rp_format_op, profile_op]},
-                             {'name': 'repoinfo',
-                              'meth': 'repo_info',
-                              'doc': 'get information on repositories',
-                              'opts': [repo_name_op, profile_op]}]},
-                {'name': 'dist',
-                 'executor': lambda params: DistManagerCli(**params),
-                 'actions': [{'name': 'freeze',
-                              'doc': 'create a distribution',
-                              'opts': [dist_dir_op, wheel_dir_op, repopref_op,
-                                       profile_op]},
-                             {'name': 'thaw',
-                              'doc': 'build out a distribution',
-                              'opts': [dist_dir_op, target_dir_op,
-                                       profile_op, dry_run_op]},
-                             {'name': 'copy',
-                              'doc': 'copy a distribution to a local file system',
-                              'opts': [dist_dir_op, repopref_op, target_dir_op,
-                                       profile_op, dry_run_op]},
-                             {'name': 'move',
-                              'doc': 'move a distribution to another root (easy to delete)',
-                              'opts': [dist_dir_op, target_dir_op,
-                                       move_dir_op, profile_op, dir_reduce_op,
-                                       dry_run_op]}]}],
-               'config_option': {'name': 'config',
-                                 'expect': False,
-                                 'opt': ['-c', '--config', False,
-                                         {'dest': 'config', 'metavar': 'FILE',
-                                          'help': 'configuration file'}]},
-               'whine': 1}
-        super(ConfAppCommandLine, self).__init__(
-            cnf, config_env_name='grsyncrc', config_type=AppConfig,
-            pkg_dist='zensols.grsync')
-
-    def _config_logging(self, level):
-        root = logging.getLogger()
-        tuple(map(root.removeHandler, root.handlers[:]))
-        if level == 0:
-            levelno = logging.ERROR
-        elif level == 1:
-            levelno = logging.WARNING
-        elif level == 2:
-            levelno = logging.INFO
-        elif level == 3:
-            levelno = logging.DEBUG
-        if level <= 2:
-            fmt = '%(message)s'
-        else:
-            fmt = '%(levelname)s:%(asctime)-15s %(name)s: %(message)s'
-        logging.basicConfig(format=fmt, level=levelno)
-
-    def _init_executor(self, executor, config, args):
-        executor.dm.app_version = self.version
-
-
-def main():
-    cl = ConfAppCommandLine()
-    cl.invoke()
+"""Command line entry point to the application.
+
+"""
+__author__ = 'Paul Landes'
+
+from typing import List, Any, Dict
+import sys
+from zensols.cli import ActionResult, CliHarness
+from zensols.cli import ApplicationFactory as CliApplicationFactory
+
+
+class ApplicationFactory(CliApplicationFactory):
+    def __init__(self, *args, **kwargs):
+        kwargs['package_resource'] = 'zensols.grsync'
+        super().__init__(*args, **kwargs)
+
+
+def main(args: List[str] = sys.argv, **kwargs: Dict[str, Any]) -> ActionResult:
+    harness: CliHarness = ApplicationFactory.create_harness(relocate=False)
+    harness.invoke(args, **kwargs)
```

## zensols/grsync/config.py

```diff
@@ -1,8 +1,13 @@
-from typing import Set
+"""Specialized application configuration.
+
+"""
+__author__ = 'Paul Landes'
+
+from typing import List, Union
 import logging
 from pathlib import Path
 import itertools as it
 import re
 from zensols.config import YamlConfig
 
 logger = logging.getLogger(__name__)
@@ -31,33 +36,32 @@
     def _find_profiles(self):
         if not self.has_option(self.PROFILES_PATH):
             opts = ()
         else:
             opts = self.get_options(self.PROFILES_PATH)
         return opts
 
-    @property
-    def all_profiles(self) -> Set[str]:
-        return set(self._find_profiles.keys())
-
     @staticmethod
-    def _split_profiles(profile_str):
+    def split_profiles(profile_str):
         return re.split(r'\s*,\s*', profile_str)
 
     @property
     def _default_profiles(self):
         strlist = self.get_option(f'{self.ROOT}.default_profiles')
         if strlist is not None:
-            return self._split_profiles(strlist)
+            return self.split_profiles(strlist)
 
-    def get_profiles(self, profile_overide_str):
-        if profile_overide_str is None:
+    def get_profiles(self, profile_overide: Union[str, List[str]] = None):
+        if profile_overide is None:
             profiles = self._default_profiles
         else:
-            profiles = self._split_profiles(profile_overide_str)
+            if isinstance(profile_overide, str):
+                profiles = self.split_profiles(profile_overide)
+            else:
+                profiles = profile_overide
         if profiles is None:
             profiles = self._find_profiles
         profiles = list(profiles)
         # protect user error
         if 'default' not in profiles:
             profiles = ['default'] + list(profiles)
         if 'nodefault' in profiles:
```

## zensols/grsync/distmng.py

```diff
@@ -1,7 +1,13 @@
+"""Distribution manager class.
+
+"""
+__author__ = 'Paul Landes'
+
+from typing import List
 import logging
 from pathlib import Path
 from zensols.config import YamlConfig
 from zensols.persist import persisted
 from zensols.grsync import (
     Discoverer,
     Distribution,
@@ -18,15 +24,15 @@
     """The main entry point that supports saving user home directory information
     (freezing) so that the data can later be restored (thawed).  It does this
     by finding git repositories and saving the remotes.  It also finds symbolic
     links, files and empty directories specified in the configuration.
 
     """
     def __init__(self, config: YamlConfig, dist_dir: Path = None,
-                 target_dir: Path = None, profiles: list = None,
+                 target_dir: Path = None, profiles: List[str] = None,
                  repo_preference: str = None, dry_run: bool = False):
         """Initialize.
 
         :param config: the app config
         :param dist_dir: the location of the frozen distribution
         :param target_dir: the location of the distrbution to freeze or where
                            to exapand (default to the user home)
@@ -108,15 +114,16 @@
 
     def freeze(self, wheel_dependency=None):
         """Freeze the current configuration and file set to the distribution zip.
 
         """
         fmng = FreezeManager(
             self.config, self.dist_file, self.defs_file, self.discoverer,
-            self.app_version)
+            self.app_version,
+            dry_run=self.dry_run)
         fmng.freeze(wheel_dependency)
 
     def thaw(self):
         """Expand the distribution zip on to the file system.
 
         """
         tmng = ThawManager(self.distribution, self.path_translator,
```

## zensols/grsync/distribution.py

```diff
@@ -1,14 +1,12 @@
-from __future__ import annotations
-
 """"Contains the class needed to thaw the distribution.
 
 """
+from __future__ import annotations
 __author__ = 'Paul Landes'
-
 from typing import Dict, Any, Iterable
 import logging
 from pathlib import Path
 import platform
 import zipfile
 import json
 from zensols.persist import persisted, PersistedWork
```

## zensols/grsync/domain.py

```diff
@@ -1,7 +1,12 @@
+"""Domain and container classes, mostly modeling Git repos.
+
+"""
+__author__ = 'Paul Landes'
+
 import logging
 from git import Remote
 from pathlib import Path
 from zensols.persist import persisted
 
 logger = logging.getLogger(__name__)
```

## zensols/grsync/freeze.py

```diff
@@ -82,15 +82,17 @@
 
     def get_discoverable_objects(self):
         """Find git repos, files, sym links and directories to reconstitute
         later.
 
         """
         paths = []
-        logger.info(f'finding objects to perist for {self.config}')
+        if logger.isEnabledFor(logging.INFO):
+            path: Path = {self.config.config_file}
+            logger.info(f'finding objects to perist defined in {path}')
         for fname in self.config.get_discoverable_objects(self.profiles):
             path = Path(fname).expanduser().absolute()
             logger.debug(f'file pattern {fname} -> {path}')
             bname = path.name
             dname = path.parent.expanduser()
             files = list(dname.glob(bname))
             logger.debug(f'expanding {path} -> {dname} / {bname}: {files}')
@@ -276,20 +278,22 @@
 
 class FreezeManager(object):
     """Invoked by a client to create *frozen* distribution .
 
     """
     CREATE_WHEEL = 'discover.wheel.create'
 
-    def __init__(self, config, dist_file, defs_file, discoverer, app_version):
+    def __init__(self, config, dist_file, defs_file, discoverer, app_version,
+                 dry_run: bool):
         self.config = config
         self.dist_file = dist_file
         self.defs_file = defs_file
         self.discoverer = discoverer
         self.app_version = app_version
+        self.dry_run = dry_run
 
     def _create_wheels(self, wheel_dependency):
         """Create wheel dependencies on this software so the host doesn't need Internet
         connectivity.  Currently the YAML dependency breaks this since only
         binary per host wheels are available for download and the wrong was is
         given of spanning platforms (i.e. OSX to Linux).
 
@@ -305,38 +309,40 @@
         main(pip_cmd.split())
 
     def _freeze_dist(self):
         """Freeze the distribution (see the class documentation).
 
         """
         dist_dir = self.dist_file.parent
-        if not dist_dir.exists():
+        if not self.dry_run and not dist_dir.exists():
             dist_dir.mkdir(parents=True, exist_ok=True)
         data = self.discoverer.freeze()
         data['app_version'] = self.app_version
-        with zipfile.ZipFile(self.dist_file, mode='w') as zf:
-            for finfo in data['files']:
-                fabs = finfo['abs']
-                frel = str(Path(finfo['rel']))
-                logger.debug(f'adding file: {fabs}')
-                zf.write(fabs, arcname=frel)
-                del finfo['abs']
-                finfo['rel'] = frel
-            logger.info(f'writing distribution defs to {self.defs_file}')
-            zf.writestr(self.defs_file, json.dumps(data, indent=2))
+        if not self.dry_run:
+            with zipfile.ZipFile(self.dist_file, mode='w') as zf:
+                for finfo in data['files']:
+                    fabs = finfo['abs']
+                    frel = str(Path(finfo['rel']))
+                    logger.debug(f'adding file: {fabs}')
+                    zf.write(fabs, arcname=frel)
+                    del finfo['abs']
+                    finfo['rel'] = frel
+                logger.info(f'writing distribution defs to {self.defs_file}')
+                zf.writestr(self.defs_file, json.dumps(data, indent=2))
         logger.info(f'created frozen distribution in {self.dist_file}')
 
     def freeze(self, wheel_dependency=None):
         """Freeze the distribution by saving creating a script to thaw along with all
         artifacts (i.e. repo definitions) in a zip file.
 
         """
         self._freeze_dist()
         script_file = self.config.bootstrap_script_file
-        bg = BootstrapGenerator(self.config)
-        bg.generate(script_file)
-        script_file.chmod(0o755)
+        if not self.dry_run:
+            bg = BootstrapGenerator(self.config)
+            bg.generate(script_file)
+            script_file.chmod(0o755)
         # wheel creation last since pip clobers/reconfigures logging
         if self.config.has_option(self.CREATE_WHEEL):
             create_wheel = self.config.get_option(self.CREATE_WHEEL)
             if create_wheel and wheel_dependency is not None:
                 self._create_wheels(wheel_dependency)
```

## zensols/grsync/mover.py

```diff
@@ -59,15 +59,15 @@
         for src, obj in self._get_paths():
             if not src.exists() and not src.is_symlink():
                 logger.warning(f'no longer exists: {src}')
             else:
                 if isinstance(obj, FrozenRepo):
                     try:
                         grepo = obj.repo_spec.repo
-                    except Exception as e:
+                    except Exception:
                         # git.exc.InvalidGitRepositoryError
                         logger.error(f'invalid repository: {obj}--skipping')
                         continue
                     if grepo.is_dirty():
                         name = obj.repo_spec.format(RepoSpec.SHORT_FORMAT)
                         if self.force_repo:
                             logger.warning(f'repo is dirty: {name}; moving anyway')
```

## zensols/grsync/repospec.py

```diff
@@ -5,19 +5,15 @@
 
 from typing import List, Dict, Any
 import logging
 import sys
 from pathlib import Path
 from git import Repo
 from zensols.persist import persisted
-from zensols.grsync import (
-    LinkEntry,
-    RemoteSpec,
-    PathTranslator
-)
+from zensols.grsync import LinkEntry, RemoteSpec, PathTranslator
 
 logger = logging.getLogger(__name__)
 MASTER_SECTION = 'branch "master"'
 
 
 class RepoSpec(object):
     """This class represents a git repository and all the symbolic links from the
```

## Comparing `zensols.grsync-0.1.0.dist-info/METADATA` & `zensols.grsync-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zensols.grsync
-Version: 0.1.0
+Version: 0.2.0
 Summary: Synchronize and manage multiple GitHub repositories
 Home-page: https://github.com/plandes/grsync
-Download-URL: https://github.com/plandes/grsync/releases/download/v0.1.0/zensols.grsync-0.1.0-py3-none-any.whl
+Download-URL: https://github.com/plandes/grsync/releases/download/v0.2.0/zensols.grsync-0.2.0-py3-none-any.whl
 Author: Paul Landes
 Author-email: landes@mailc.net
 Keywords: tooling,configuration
 Description-Content-Type: text/markdown
-Requires-Dist: zensols.util (~=1.11.0)
-Requires-Dist: gitpython (==2.1.11)
-Requires-Dist: gitdb2 (==2.0.3)
+Requires-Dist: zensols.util (~=1.12.0)
+Requires-Dist: GitPython (~=3.1.29)
+Requires-Dist: gitdb2 (~=2.0.3)
 
 # GRSync: Persist create build out environments
 
 [![PyPI][pypi-badge]][pypi-link]
 [![Python 3.9][python39-badge]][python39-link]
 [![Python 3.10][python310-badge]][python310-link]
 [![Build Status][build-badge]][build-link]
@@ -31,14 +31,17 @@
 on another system (see [overview](#overview)).  This is done by:
 1. Copying files, directories and git repos configuration.
 2. Creating a distribution compressed file.
 3. Uncompress on the destination system and create repos.
 
 A future release will also synchronize and manage multiple GitHub repositories.
 
+A [utility script] also provided to do operations on all configured local git
+repositories.
+
 
 ## Documentation
 
 See the [full documentation](https://plandes.github.io/grsync/index.html).  The
 [API reference](https://plandes.github.io/grsync/api.html) is also available.
 
 
@@ -83,15 +86,15 @@
 
 ## Usage
 
 The program has two phases: *freeze* and *thaw* (see [overview](#overview)).
 The command line program is used twice: first on the *freeze* on the source
 system and then *thaw* on the target machine.
 
-See [usage](doc/usage.md) for more information.
+See [usage](https://plandes.github.io/grsync/doc/usage.html) for more information.
 
 
 ## Configuration
 
 The configuration is used the *freeze* phase to create the distribution file.
 This fil contains all git repositories, files, empty directory paths on the
 current file system that is stored to be *thawed* on the target system.
@@ -113,15 +116,15 @@
 A future release might have a *follow symbolic links* type functionality that
 allows this.  However, for now, you must include both the link and the data it
 points to get this integrity.
 
 
 ## Requirements
 
-* At least [Python 3.7]
+* At least [Python 3.9]
 * A system that supports [PyYAML]
 
 
 ## Planned Future Features
 
 Preserve and restore file and directory timestamps.
 
@@ -131,30 +134,31 @@
 An extensive changelog is available [here](CHANGELOG.md).
 
 
 ## License
 
 [MIT License](LICENSE.md)
 
-Copyright (c) 2020 Paul Landes
+Copyright (c) 2020 - 2023 Paul Landes
 
 
 <!-- links -->
 [pypi]: https://pypi.org/project/zensols.grsync/
 [pypi-link]: https://pypi.python.org/pypi/zensols.grsync
 [pypi-badge]: https://img.shields.io/pypi/v/zensols.grsync.svg
 [python39-badge]: https://img.shields.io/badge/python-3.9-blue.svg
 [python39-link]: https://www.python.org/downloads/release/python-390
 [python310-badge]: https://img.shields.io/badge/python-3.10-blue.svg
 [python310-link]: https://www.python.org/downloads/release/python-3100
 [build-badge]: https://github.com/plandes/grsync/workflows/CI/badge.svg
 [build-link]: https://github.com/plandes/grsync/actions
 
-[Python 3.7]: https://www.python.org
+[Python 3.9]: https://www.python.org
 [PyYAML]: https://pyyaml.org
 [test configuration]: test-resources/grsync-test.yml
 
 [maven profiles]: https://maven.apache.org/guides/introduction/introduction-to-profiles.html
 [configuration file]: test-resources/midsize-test.yml#L29
 [configuration file profile entry]: test-resources/midsize-test.yml#L29
 [pip]: https://docs.python.org/3/installing/index.html
 [Puppet]: https://en.wikipedia.org/wiki/Puppet_(software)
+[utility script]: https://plandes.github.io/grsync/doc/usage.html#utility-git-script
```

## Comparing `zensols.grsync-0.1.0.dist-info/RECORD` & `zensols.grsync-0.2.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-zensols/grsync/__init__.py,sha256=zOZ5p5ByWS8SUY6j-VJM6h5lJsiEancNStRUsRGi1ok,226
-zensols/grsync/bootstrap.py,sha256=jRZumDeOvbuOzaBTTlYveMzeZf0vzt7CbMzm_KCZEdg,2469
-zensols/grsync/cli.py,sha256=iOOdsp7MVw5W8pbT9U-GHxg1W40EQ5UdVZrIZmSKCwM,7063
-zensols/grsync/config.py,sha256=doqCn5-S_Mj8KcQwpfu0j0mVQpQJtWx7YlXv3bMpvSo,4207
-zensols/grsync/distmng.py,sha256=ZdRfgqP9muFXk3-UdwNfC8bLvt0uBh-CK23hPMI8qdM,5533
-zensols/grsync/distribution.py,sha256=PER-9iT4aPpqTmsd7yB4s1fgs6z23QR3vyBHXuzR4UI,4233
-zensols/grsync/domain.py,sha256=9E49LVRRRHNRsLPm3yfkXI8q0CpGAG7P1xMBH4q6S2g,6135
-zensols/grsync/freeze.py,sha256=WbuAzIRMor3MYZ4znB0Z-hbPm29PFe6SgEWEbgG5RZs,14233
-zensols/grsync/mover.py,sha256=GdfU8d7aYjLjLdyJgU5i6QWf4q8VRrOfmoJDvtEpVzQ,5110
-zensols/grsync/repospec.py,sha256=97NJOObbrIp3PXJsjk8DFmWTIQxVEuV2mWL48G1Zyoo,8860
+zensols/grsync/__init__.py,sha256=Sbgv9DqcN_aoZSTEpBumQelGY0l1TyCn0Ndyt9qVxH8,245
+zensols/grsync/app.py,sha256=9sfO3dCCyVQzhLvsOjBet9wvhTEzgxl71P0fcvmpIkc,5874
+zensols/grsync/bootstrap.py,sha256=Upuypc8YN-bAm-BdZ2Yq_nDR_kq1KoepRQLy0GfPVko,2374
+zensols/grsync/cli.py,sha256=dv-Egc2aQpGmzgbwn37XZW-kw5yGTAh5YioNapfc4Gs,625
+zensols/grsync/config.py,sha256=YZ01a7sDGI57hheN_s-p6LGK7A4Uop0V6OgY2kL-vgE,4317
+zensols/grsync/distmng.py,sha256=TtIqzypIGIg0oi25BIij_GXlrM-OW8CTVQ8Dtmwb41c,5660
+zensols/grsync/distribution.py,sha256=UEownHsoOhjn25R5wnl7BxQTPA6ERmbeSj498hSLFFk,4231
+zensols/grsync/domain.py,sha256=jeNdh0wMQh3r6Mz4w1jmW52frqhCWjczTtb4Hc0NtEs,6228
+zensols/grsync/freeze.py,sha256=K-_pTsQos75vNO6zvLHVhLZGecSNl_OZAtveW3bDe1E,14528
+zensols/grsync/mover.py,sha256=a2fVEySYbsxAaKGZU5T98xQmdbtrXWkPCPEfcLkqsR4,5105
+zensols/grsync/repospec.py,sha256=jpToT9YCSbv-fh8DIUbPpCIXzR4RD_t7eKdoamidstA,8844
 zensols/grsync/thaw.py,sha256=-Ty-WyW8b4kjDf98RjUdt3dk4U6lZykssx_xXvjGPOE,6912
-zensols.grsync-0.1.0.dist-info/METADATA,sha256=UZyX2XpivhyBS-9Jool8m7DmumPxGItCTeEwRYLOM08,6106
-zensols.grsync-0.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-zensols.grsync-0.1.0.dist-info/entry_points.txt,sha256=o2LTq6DpSUAtALRA6JEmwE3_gycSN5WBJSKtIJPAJMQ,47
-zensols.grsync-0.1.0.dist-info/top_level.txt,sha256=OV7uMopmFj1gpEBb-dK5iJSY_08oHYRnurV6-djDIWM,15
-zensols.grsync-0.1.0.dist-info/RECORD,,
+zensols/grsync/resources/app.conf,sha256=Hog7pdOb-uqTWkXavA862LtajQeNoQGCIYiHLSSqO4s,1093
+zensols.grsync-0.2.0.dist-info/METADATA,sha256=r2dOQ3CmSzKgyPcCx1kHy2YRM_0vuUuPt1S-UGrUqIU,6326
+zensols.grsync-0.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+zensols.grsync-0.2.0.dist-info/entry_points.txt,sha256=o2LTq6DpSUAtALRA6JEmwE3_gycSN5WBJSKtIJPAJMQ,47
+zensols.grsync-0.2.0.dist-info/top_level.txt,sha256=OV7uMopmFj1gpEBb-dK5iJSY_08oHYRnurV6-djDIWM,15
+zensols.grsync-0.2.0.dist-info/RECORD,,
```

