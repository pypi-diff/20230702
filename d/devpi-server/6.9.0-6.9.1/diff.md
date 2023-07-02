# Comparing `tmp/devpi-server-6.9.0.tar.gz` & `tmp/devpi-server-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-server-6.9.0.tar", last modified: Tue May 23 14:32:20 2023, max compression
+gzip compressed data, was "devpi-server-6.9.1.tar", last modified: Sun Jul  2 12:02:56 2023, max compression
```

## Comparing `devpi-server-6.9.0.tar` & `devpi-server-6.9.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.454745 devpi-server-6.9.0/
--rw-r--r--   0 fschulze   (501) staff       (20)      138 2023-05-23 14:32:14.000000 devpi-server-6.9.0/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    70739 2023-05-23 14:32:14.000000 devpi-server-6.9.0/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-05-23 14:32:14.000000 devpi-server-6.9.0/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      188 2023-05-23 14:32:14.000000 devpi-server-6.9.0/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     6946 2023-05-23 14:32:20.454864 devpi-server-6.9.0/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     2033 2023-05-23 14:32:14.000000 devpi-server-6.9.0/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.419010 devpi-server-6.9.0/devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       82 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/__main__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7260 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1195 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/auth_basic.py
--rw-r--r--   0 fschulze   (501) staff       (20)      958 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/auth_devpi.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.426238 devpi-server-6.9.0/devpi_server/cfg/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)      213 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/crontab.template
--rw-r--r--   0 fschulze   (501) staff       (20)      430 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/devpi.service.template
--rw-r--r--   0 fschulze   (501) staff       (20)      455 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/launchd-macos.txt.template
--rw-r--r--   0 fschulze   (501) staff       (20)      619 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-http.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      237 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-location.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      330 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      341 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-server.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)     2065 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      140 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/supervisor-devpi.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      283 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/supervisord.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)     1694 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/windows-service.txt.template
--rw-r--r--   0 fschulze   (501) staff       (20)    36715 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/config.py
--rw-r--r--   0 fschulze   (501) staff       (20)      643 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/exceptions.py
--rw-r--r--   0 fschulze   (501) staff       (20)    10069 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/filestore.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8841 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/fileutil.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3579 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/fsck.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6962 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/genconfig.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8555 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    28123 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/importexport.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1926 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/init.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5921 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/interfaces.py
--rw-r--r--   0 fschulze   (501) staff       (20)    30064 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    24238 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs_sqlite.py
--rw-r--r--   0 fschulze   (501) staff       (20)    11289 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs_sqlite_fs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2865 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs_types.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3751 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/log.py
--rw-r--r--   0 fschulze   (501) staff       (20)    26268 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)      952 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/middleware.py
--rw-r--r--   0 fschulze   (501) staff       (20)    39630 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/mirror.py
--rw-r--r--   0 fschulze   (501) staff       (20)    74949 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/model.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3668 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/mythread.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1642 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/passwd.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7018 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/readonly.py
--rw-r--r--   0 fschulze   (501) staff       (20)    52077 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1589 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/sizeof.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.426654 devpi-server-6.9.0/devpi_server/vendor/
--rw-r--r--   0 fschulze   (501) staff       (20)     5030 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/vendor/_pip.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9110 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/view_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)    75198 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/views.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.421715 devpi-server-6.9.0/devpi_server.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     6946 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     4838 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)     1007 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)      235 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       51 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      549 2023-05-23 14:32:14.000000 devpi-server-6.9.0/pyproject.toml
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.427025 devpi-server-6.9.0/pytest_devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)      863 2023-05-23 14:32:14.000000 devpi-server-6.9.0/pytest_devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-05-23 14:32:20.455296 devpi-server-6.9.0/setup.cfg
--rwxr-xr-x   0 fschulze   (501) staff       (20)     4518 2023-05-23 14:32:14.000000 devpi-server-6.9.0/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.445440 devpi-server-6.9.0/test_devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    46442 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)      504 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/example.py
--rw-r--r--   0 fschulze   (501) staff       (20)    21873 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/functional.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.398379 devpi-server-6.9.0/test_devpi_server/importexportdata/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.445852 devpi-server-6.9.0/test_devpi_server/importexportdata/badindexname/
--rw-r--r--   0 fschulze   (501) staff       (20)      698 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/badindexname/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.446250 devpi-server-6.9.0/test_devpi_server/importexportdata/badusername/
--rw-r--r--   0 fschulze   (501) staff       (20)      719 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/badusername/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.446622 devpi-server-6.9.0/test_devpi_server/importexportdata/basescycle/
--rw-r--r--   0 fschulze   (501) staff       (20)      659 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/basescycle/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.447031 devpi-server-6.9.0/test_devpi_server/importexportdata/createdmodified/
--rw-r--r--   0 fschulze   (501) staff       (20)      423 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/createdmodified/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.447440 devpi-server-6.9.0/test_devpi_server/importexportdata/deletedbase/
--rw-r--r--   0 fschulze   (501) staff       (20)     1603 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/deletedbase/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.448023 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/
--rw-r--r--   0 fschulze   (501) staff       (20)     1413 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.394524 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.394646 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.394766 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.448575 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/
--rw-r--r--   0 fschulze   (501) staff       (20)      780 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.448954 devpi-server-6.9.0/test_devpi_server/importexportdata/modifiedpypi/
--rw-r--r--   0 fschulze   (501) staff       (20)      648 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/modifiedpypi/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.449333 devpi-server-6.9.0/test_devpi_server/importexportdata/nocreatedmodified/
--rw-r--r--   0 fschulze   (501) staff       (20)      485 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/nocreatedmodified/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.449707 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/
--rw-r--r--   0 fschulze   (501) staff       (20)     1610 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.395564 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.395680 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.450095 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.450472 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/
--rw-r--r--   0 fschulze   (501) staff       (20)     2299 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.396145 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.396426 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.450854 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/hello.pkg-1.1.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.451235 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.451609 devpi-server-6.9.0/test_devpi_server/importexportdata/norootpypi/
--rw-r--r--   0 fschulze   (501) staff       (20)      340 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/norootpypi/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.451982 devpi-server-6.9.0/test_devpi_server/importexportdata/nouser/
--rw-r--r--   0 fschulze   (501) staff       (20)      198 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/nouser/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.452346 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/
--rw-r--r--   0 fschulze   (501) staff       (20)     1581 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397219 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397335 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.452725 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.453086 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/
--rw-r--r--   0 fschulze   (501) staff       (20)     1538 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397796 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397911 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.398213 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.453472 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/hello-0.9.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.454054 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/
--rw-r--r--   0 fschulze   (501) staff       (20)        2 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/hello-0.9.tar.gz.toxresult0
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.454428 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_upload_default/
--rw-r--r--   0 fschulze   (501) staff       (20)      650 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json
--rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/simpypi.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9275 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2401 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_authcheck.py
--rw-r--r--   0 fschulze   (501) staff       (20)    17566 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_config.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1064 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16223 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_filestore.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4355 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_fileutil.py
--rw-r--r--   0 fschulze   (501) staff       (20)      623 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_genconfig.py
--rw-r--r--   0 fschulze   (501) staff       (20)    47791 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_importexport.py
--rw-r--r--   0 fschulze   (501) staff       (20)    31905 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_keyfs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2877 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_keyfs_sqlite_fs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3965 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_log.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13794 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)    51665 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_mirror.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8945 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_mirror_no_project_list.py
--rw-r--r--   0 fschulze   (501) staff       (20)    81466 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_model.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1711 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_mythread.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3112 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1210 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_nginx_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9617 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_permissions.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4527 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_readonly.py
--rw-r--r--   0 fschulze   (501) staff       (20)    56091 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3305 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_replica_functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1790 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16607 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_stage_customizer.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5214 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming.py
--rw-r--r--   0 fschulze   (501) staff       (20)      664 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)      669 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)      681 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming_replica_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4932 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_view_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)   105730 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3101 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views_patch.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9465 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views_push_external.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8899 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views_status.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1514 2023-05-23 14:32:14.000000 devpi-server-6.9.0/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.395679 devpi-server-6.9.1/
+-rw-r--r--   0 fschulze   (501) staff       (20)      138 2023-07-02 12:02:49.000000 devpi-server-6.9.1/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    70990 2023-07-02 12:02:49.000000 devpi-server-6.9.1/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-07-02 12:02:49.000000 devpi-server-6.9.1/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      188 2023-07-02 12:02:49.000000 devpi-server-6.9.1/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     6008 2023-07-02 12:02:56.395806 devpi-server-6.9.1/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     2033 2023-07-02 12:02:49.000000 devpi-server-6.9.1/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.355997 devpi-server-6.9.1/devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       82 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/__main__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7260 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1195 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/auth_basic.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      958 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/auth_devpi.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.362956 devpi-server-6.9.1/devpi_server/cfg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      213 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/crontab.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      430 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/devpi.service.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      455 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/launchd-macos.txt.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      619 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-http.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      237 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-location.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      330 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      341 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-server.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)     2065 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      140 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/supervisor-devpi.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      283 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/supervisord.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)     1694 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/windows-service.txt.template
+-rw-r--r--   0 fschulze   (501) staff       (20)    36622 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      643 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/exceptions.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    10069 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/filestore.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8841 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/fileutil.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3579 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/fsck.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6962 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/genconfig.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8555 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    28123 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/importexport.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1926 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/init.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5921 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/interfaces.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    30210 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    24464 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs_sqlite.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    11289 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs_sqlite_fs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2865 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs_types.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3751 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/log.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    26268 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      952 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/middleware.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    39630 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/mirror.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    74949 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/model.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3668 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/mythread.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1642 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/passwd.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7018 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/readonly.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    52150 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1589 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/sizeof.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.363385 devpi-server-6.9.1/devpi_server/vendor/
+-rw-r--r--   0 fschulze   (501) staff       (20)     5030 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/vendor/_pip.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9110 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/view_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    75592 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/views.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.358514 devpi-server-6.9.1/devpi_server.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     6008 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     4838 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1007 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)      235 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       51 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      549 2023-07-02 12:02:49.000000 devpi-server-6.9.1/pyproject.toml
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.364895 devpi-server-6.9.1/pytest_devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)      863 2023-07-02 12:02:49.000000 devpi-server-6.9.1/pytest_devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-07-02 12:02:56.396309 devpi-server-6.9.1/setup.cfg
+-rwxr-xr-x   0 fschulze   (501) staff       (20)     4518 2023-07-02 12:02:49.000000 devpi-server-6.9.1/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.386576 devpi-server-6.9.1/test_devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    46442 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      504 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/example.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    21873 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/functional.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.336688 devpi-server-6.9.1/test_devpi_server/importexportdata/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.386986 devpi-server-6.9.1/test_devpi_server/importexportdata/badindexname/
+-rw-r--r--   0 fschulze   (501) staff       (20)      698 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/badindexname/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.387385 devpi-server-6.9.1/test_devpi_server/importexportdata/badusername/
+-rw-r--r--   0 fschulze   (501) staff       (20)      719 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/badusername/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.387773 devpi-server-6.9.1/test_devpi_server/importexportdata/basescycle/
+-rw-r--r--   0 fschulze   (501) staff       (20)      659 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/basescycle/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.388155 devpi-server-6.9.1/test_devpi_server/importexportdata/createdmodified/
+-rw-r--r--   0 fschulze   (501) staff       (20)      423 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/createdmodified/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.388530 devpi-server-6.9.1/test_devpi_server/importexportdata/deletedbase/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1603 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/deletedbase/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.388903 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1413 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.328259 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.328394 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.328514 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.389292 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/
+-rw-r--r--   0 fschulze   (501) staff       (20)      780 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.389682 devpi-server-6.9.1/test_devpi_server/importexportdata/modifiedpypi/
+-rw-r--r--   0 fschulze   (501) staff       (20)      648 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/modifiedpypi/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.390067 devpi-server-6.9.1/test_devpi_server/importexportdata/nocreatedmodified/
+-rw-r--r--   0 fschulze   (501) staff       (20)      485 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/nocreatedmodified/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.390443 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1610 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.329341 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.329468 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.390826 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.391214 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/
+-rw-r--r--   0 fschulze   (501) staff       (20)     2299 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.329986 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.330742 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.391621 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/hello.pkg-1.1.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.392004 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.392385 devpi-server-6.9.1/test_devpi_server/importexportdata/norootpypi/
+-rw-r--r--   0 fschulze   (501) staff       (20)      340 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/norootpypi/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.392767 devpi-server-6.9.1/test_devpi_server/importexportdata/nouser/
+-rw-r--r--   0 fschulze   (501) staff       (20)      198 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/nouser/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.393201 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1581 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.334502 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.334731 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.393662 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.394066 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1538 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.335657 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.335869 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.336478 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.394471 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/hello-0.9.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.394926 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/
+-rw-r--r--   0 fschulze   (501) staff       (20)        2 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/hello-0.9.tar.gz.toxresult0
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.395343 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_upload_default/
+-rw-r--r--   0 fschulze   (501) staff       (20)      650 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json
+-rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/simpypi.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9275 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2401 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_authcheck.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    17566 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1064 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    16223 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_filestore.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4355 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_fileutil.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      623 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_genconfig.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    47791 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_importexport.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    31905 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_keyfs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2877 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_keyfs_sqlite_fs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3965 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_log.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    13794 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    51665 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_mirror.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8945 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_mirror_no_project_list.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    81466 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_model.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1711 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_mythread.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3112 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1210 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_nginx_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9617 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_permissions.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4527 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_readonly.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    56091 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3305 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_replica_functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1790 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    16607 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_stage_customizer.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5214 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      664 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      669 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      681 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming_replica_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4932 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_view_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)   105730 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3101 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views_patch.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9465 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views_push_external.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8899 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views_status.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1514 2023-07-02 12:02:50.000000 devpi-server-6.9.1/tox.ini
```

### Comparing `devpi-server-6.9.0/CHANGELOG` & `devpi-server-6.9.1/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 
 
 .. towncrier release notes start
 
+6.9.1 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Prevent error in find_pre_existing_file in case of incomplete metadata.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 6.9.0 (2023-05-23)
 ==================
 
 Features
 --------
 
 - Support export directory layout for ``--replica-file-search-path`` option.
```

### Comparing `devpi-server-6.9.0/LICENSE` & `devpi-server-6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/PKG-INFO` & `devpi-server-6.9.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-server
-Version: 6.9.0
+Version: 6.9.1
 Summary: devpi-server: reliable private and pypi.org caching server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/server/CHANGELOG
@@ -98,14 +98,25 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.9.1 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Prevent error in find_pre_existing_file in case of incomplete metadata.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 6.9.0 (2023-05-23)
 ==================
 
 Features
 --------
 
 - Support export directory layout for ``--replica-file-search-path`` option.
@@ -175,36 +186,7 @@
 
 - Removed preservation of original server uuid during import. Imported state is different from the original server. Replicas could not detect the change and get into an inconsistent state.
 
 - Prevent cache trashing when updating simple links on mirrors for projects with huge number of releases.
 
 - Preserve toxresult filenames during import to keep them being accessible on the same URLs after the fix for #686 in 5.2.0.
 
-
-6.6.0 (2022-08-16)
-==================
-
-Features
---------
-
-- Fix #592: return dict from ``list_projects_perstage`` of mirrors where the values contain the un-normalized project name. This allows support in devpi-web 4.1.0 to index them correctly.
-
-- Check name in project list instead of fetching project page for mirrors. This improves response times and avoids leaking typos of private package names upstream.
-
-- Use ETag header if provided by mirror to reduce bandwidth usage and latency.
-
-- Prevent concurrent updates of simple links on mirrors with a short lived lock.
-
-- Support `PEP-691 <https://peps.python.org/pep-0691/>`_ conformant fetching for mirrors, and requests with JSON result for installers. Proxy servers should add compression support for the ``application/vnd.pypi.simple.v1+json`` content type (``gzip_types`` for nginx).
-
-
-Bug Fixes
----------
-
-- Fix #743: support PEP427 escaped wheels with local version, where the + is replaced by _.
-
-- Fix #895: store and return content of data-yanked.
-
-- Fix #908: include basic auth from ``mirror_url`` when fetching packages.
-
-- Fix #914: switch to write transaction as late as possible when streaming a file from a mirror.
-
```

### Comparing `devpi-server-6.9.0/README.rst` & `devpi-server-6.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/auth.py` & `devpi-server-6.9.1/devpi_server/auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/auth_basic.py` & `devpi-server-6.9.1/devpi_server/auth_basic.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/auth_devpi.py` & `devpi-server-6.9.1/devpi_server/auth_devpi.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-http.conf.template` & `devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-http.conf.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/cfg/nginx-devpi.conf.template` & `devpi-server-6.9.1/devpi_server/cfg/nginx-devpi.conf.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/cfg/windows-service.txt.template` & `devpi-server-6.9.1/devpi_server/cfg/windows-service.txt.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/config.py` & `devpi-server-6.9.1/devpi_server/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,14 @@
         return False
     else:
         raise ValueError(f"invalid truth value {val!r}")
 
 
 def get_pluginmanager(load_entrypoints=True):
     pm = PluginManager("devpiserver")
-    # support old plugins, but emit deprecation warnings
-    pm._implprefix = "devpiserver_"
     pm.add_hookspecs(hookspecs)
     # XXX load internal plugins here
     if load_entrypoints:
         pm.load_setuptools_entrypoints("devpi_server")
     pm.check_pending()
     return pm
```

### Comparing `devpi-server-6.9.0/devpi_server/exceptions.py` & `devpi-server-6.9.1/devpi_server/exceptions.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/filestore.py` & `devpi-server-6.9.1/devpi_server/filestore.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/fileutil.py` & `devpi-server-6.9.1/devpi_server/fileutil.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/fsck.py` & `devpi-server-6.9.1/devpi_server/fsck.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/genconfig.py` & `devpi-server-6.9.1/devpi_server/genconfig.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/hookspecs.py` & `devpi-server-6.9.1/devpi_server/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/importexport.py` & `devpi-server-6.9.1/devpi_server/importexport.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/init.py` & `devpi-server-6.9.1/devpi_server/init.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/interfaces.py` & `devpi-server-6.9.1/devpi_server/interfaces.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/keyfs.py` & `devpi-server-6.9.1/devpi_server/keyfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
 from devpi_common.types import cached_property
 
 
 absent = object()
 
 
+class KeyfsTimeoutError(TimeoutError):
+    pass
+
+
 class MissingFileException(Exception):
     def __init__(self, relpath, serial):
         msg = "missing file '%s' at serial %s" % (relpath, serial)
         super(MissingFileException, self).__init__(msg)
         self.relpath = relpath
         self.serial = serial
 
@@ -757,15 +761,19 @@
 
     def restart(self, write=False):
         self.commit()
         threadlog.debug(
             "restarting %s transaction afresh as %s transaction",
             "write" if self.write else "read",
             "write" if write else "read")
-        newtx = self.__class__(self.keyfs, write=write)
+        try:
+            newtx = self.__class__(self.keyfs, write=write)
+        except BaseException:
+            self.doomed = True
+            raise
         self.__dict__ = newtx.__dict__
 
     def doom(self):
         """ mark as doomed to automatically rollback any changes """
         self.doomed = True
```

### Comparing `devpi-server-6.9.0/devpi_server/keyfs_sqlite.py` & `devpi-server-6.9.1/devpi_server/keyfs_sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from devpi_common.types import cached_property
 from .config import hookimpl
 from .fileutil import dumps, loads
 from .interfaces import IStorageConnection2
+from .keyfs import KeyfsTimeoutError
 from .keyfs import RelpathInfo
 from .keyfs import get_relpath_at
 from .log import threadlog, thread_push_log, thread_pop_log
 from .mythread import current_thread
 from .readonly import ReadonlyView
 from .readonly import ensure_deeply_readonly, get_mutable_deepcopy
 from .sizeof import gettotalsizeof
@@ -111,15 +112,19 @@
     def close(self):
         self._sqlconn.close()
 
     def commit(self):
         self._sqlconn.commit()
 
     def rollback(self):
-        self._sqlconn.rollback()
+        try:
+            self._sqlconn.rollback()
+        except sqlite3.ProgrammingError as e:
+            if not e.args or 'closed database' not in e.args[0]:
+                raise
 
     @cached_property
     def last_changelog_serial(self):
         return self.db_read_last_changelog_serial()
 
     def db_read_last_changelog_serial(self):
         q = 'SELECT MAX(_ROWID_) FROM "changelog" LIMIT 1'
@@ -437,15 +442,16 @@
                     # another thread may be writing, give it a chance to finish
                     time.sleep(0.1)
                     if hasattr(thread, "exit_if_shutdown"):
                         thread.exit_if_shutdown()
                     elapsed = time.monotonic() - start_time
                     if elapsed > timeout:
                         # if it takes this long, something is wrong
-                        raise TimeoutError(f"Timeout after {elapsed} seconds.") from e
+                        raise KeyfsTimeoutError(
+                            f"Timeout after {int(elapsed)} seconds.") from e
         conn = self.Connection(sqlconn, self.basedir, self)
         if closing:
             return contextlib.closing(conn)
         return conn
 
     def _reflect_schema(self):
         result = {}
```

### Comparing `devpi-server-6.9.0/devpi_server/keyfs_sqlite_fs.py` & `devpi-server-6.9.1/devpi_server/keyfs_sqlite_fs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/keyfs_types.py` & `devpi-server-6.9.1/devpi_server/keyfs_types.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/log.py` & `devpi-server-6.9.1/devpi_server/log.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/main.py` & `devpi-server-6.9.1/devpi_server/main.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/middleware.py` & `devpi-server-6.9.1/devpi_server/middleware.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/mirror.py` & `devpi-server-6.9.1/devpi_server/mirror.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/model.py` & `devpi-server-6.9.1/devpi_server/model.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/mythread.py` & `devpi-server-6.9.1/devpi_server/mythread.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/passwd.py` & `devpi-server-6.9.1/devpi_server/passwd.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/readonly.py` & `devpi-server-6.9.1/devpi_server/readonly.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/replica.py` & `devpi-server-6.9.1/devpi_server/replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,19 +851,20 @@
 
     def find_pre_existing_file(self, entry):
         if self.file_search_path is None:
             return
         path = os.path.join(self.file_search_path, entry.relpath)
         if not os.path.exists(path):
             # look for file in export layout
-            path = os.path.join(
-                self.file_search_path,
+            parts = (
                 entry.user, entry.index,
                 entry.project, entry.version,
                 entry.basename)
+            if all(part is not None for part in parts):
+                path = os.path.join(self.file_search_path, *parts)
         if not os.path.exists(path):
             threadlog.debug("path for existing file not found: %s", path)
             return
         threadlog.debug("checking existing file: %s", path)
         f = open(path, "rb")
         hexdigest = get_file_hash(f, entry.hash_type)
         if hexdigest != entry.hash_value:
```

### Comparing `devpi-server-6.9.0/devpi_server/sizeof.py` & `devpi-server-6.9.1/devpi_server/sizeof.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/vendor/_pip.py` & `devpi-server-6.9.1/devpi_server/vendor/_pip.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/view_auth.py` & `devpi-server-6.9.1/devpi_server/view_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server/views.py` & `devpi-server-6.9.1/devpi_server/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pluggy import HookimplMarker
 from pyramid.authentication import b64encode
 from pyramid.interfaces import IRequestExtensions
 from pyramid.interfaces import IRootFactory
 from pyramid.interfaces import IRoutesMapper
 from pyramid.httpexceptions import HTTPException, HTTPFound, HTTPSuccessful
 from pyramid.httpexceptions import HTTPForbidden
+from pyramid.httpexceptions import HTTPInternalServerError
 from pyramid.httpexceptions import HTTPOk
 from pyramid.httpexceptions import HTTPUnauthorized
 from pyramid.httpexceptions import exception_response
 from pyramid.request import Request
 from pyramid.request import apply_request_extensions
 from pyramid.response import FileIter
 from pyramid.response import Response
@@ -32,17 +33,19 @@
 from urllib3.exceptions import IncompleteRead
 import itertools
 import json
 from devpi_common.request import new_requests_session
 from devpi_common.validation import normalize_name, is_valid_archive_name
 
 from .config import hookimpl
+from .exceptions import lazy_format_exception_only
 from .filestore import BadGateway
 from .filestore import get_checksum_error
 from .fileutil import buffered_iterator
+from .keyfs import KeyfsTimeoutError
 from .model import InvalidIndex, InvalidIndexconfig, InvalidUser, InvalidUserconfig
 from .model import ReadonlyIndex
 from .model import RemoveValue
 from .readonly import get_mutable_deepcopy
 from .log import thread_push_log, thread_pop_log, threadlog
 
 from .auth import Auth
@@ -219,15 +222,21 @@
     keyfs = registry["xom"].keyfs
     is_replica = registry["xom"].is_replica()
 
     def request_tx_handler(request):
         write = is_mutating_http_method(request.method) and not is_replica
         with keyfs.transaction(write=write) as tx:
             threadlog.debug("in-transaction %s", tx.at_serial)
-            response = handler(request)
+            try:
+                response = handler(request)
+            except KeyfsTimeoutError as e:
+                msg = lazy_format_exception_only(e)
+                threadlog.error(
+                    "Keyfs timeout: %s", msg)
+                return HTTPInternalServerError(msg)
         set_header_devpi_serial(response, tx)
         return response
     return request_tx_handler
 
 
 def set_header_devpi_serial(response, tx):
     if "X-DEVPI-SERIAL" in response.headers:
```

### Comparing `devpi-server-6.9.0/devpi_server.egg-info/PKG-INFO` & `devpi-server-6.9.1/devpi_server.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-server
-Version: 6.9.0
+Version: 6.9.1
 Summary: devpi-server: reliable private and pypi.org caching server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/server/CHANGELOG
@@ -98,14 +98,25 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.9.1 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Prevent error in find_pre_existing_file in case of incomplete metadata.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 6.9.0 (2023-05-23)
 ==================
 
 Features
 --------
 
 - Support export directory layout for ``--replica-file-search-path`` option.
@@ -175,36 +186,7 @@
 
 - Removed preservation of original server uuid during import. Imported state is different from the original server. Replicas could not detect the change and get into an inconsistent state.
 
 - Prevent cache trashing when updating simple links on mirrors for projects with huge number of releases.
 
 - Preserve toxresult filenames during import to keep them being accessible on the same URLs after the fix for #686 in 5.2.0.
 
-
-6.6.0 (2022-08-16)
-==================
-
-Features
---------
-
-- Fix #592: return dict from ``list_projects_perstage`` of mirrors where the values contain the un-normalized project name. This allows support in devpi-web 4.1.0 to index them correctly.
-
-- Check name in project list instead of fetching project page for mirrors. This improves response times and avoids leaking typos of private package names upstream.
-
-- Use ETag header if provided by mirror to reduce bandwidth usage and latency.
-
-- Prevent concurrent updates of simple links on mirrors with a short lived lock.
-
-- Support `PEP-691 <https://peps.python.org/pep-0691/>`_ conformant fetching for mirrors, and requests with JSON result for installers. Proxy servers should add compression support for the ``application/vnd.pypi.simple.v1+json`` content type (``gzip_types`` for nginx).
-
-
-Bug Fixes
----------
-
-- Fix #743: support PEP427 escaped wheels with local version, where the + is replaced by _.
-
-- Fix #895: store and return content of data-yanked.
-
-- Fix #908: include basic auth from ``mirror_url`` when fetching packages.
-
-- Fix #914: switch to write transaction as late as possible when streaming a file from a mirror.
-
```

### Comparing `devpi-server-6.9.0/devpi_server.egg-info/SOURCES.txt` & `devpi-server-6.9.1/devpi_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/devpi_server.egg-info/entry_points.txt` & `devpi-server-6.9.1/devpi_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/pyproject.toml` & `devpi-server-6.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/pytest_devpi_server/__init__.py` & `devpi-server-6.9.1/pytest_devpi_server/__init__.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/setup.py` & `devpi-server-6.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
       url="https://devpi.net",
       project_urls={
         'Bug Tracker': 'https://github.com/devpi/devpi/issues',
         'Changelog': 'https://github.com/devpi/devpi/blob/main/server/CHANGELOG',
         'Documentation': 'https://doc.devpi.net',
         'Source Code': 'https://github.com/devpi/devpi'
       },
-      version='6.9.0',
+      version='6.9.1',
       maintainer="Florian Schulze",
       maintainer_email="mail@pyfidelity.com",
       packages=[
         'devpi_server',
         'devpi_server.cfg',
         'devpi_server.vendor',
         'pytest_devpi_server',
```

### Comparing `devpi-server-6.9.0/test_devpi_server/conftest.py` & `devpi-server-6.9.1/test_devpi_server/conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/functional.py` & `devpi-server-6.9.1/test_devpi_server/functional.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/badindexname/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/badindexname/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/badusername/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/badusername/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/basescycle/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/basescycle/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/deletedbase/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/deletedbase/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz` & `devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/modifiedpypi/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/modifiedpypi/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json` & `devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/reqmock.py` & `devpi-server-6.9.1/test_devpi_server/reqmock.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/simpypi.py` & `devpi-server-6.9.1/test_devpi_server/simpypi.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_auth.py` & `devpi-server-6.9.1/test_devpi_server/test_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_authcheck.py` & `devpi-server-6.9.1/test_devpi_server/test_authcheck.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_config.py` & `devpi-server-6.9.1/test_devpi_server/test_config.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_conftest.py` & `devpi-server-6.9.1/test_devpi_server/test_conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_filestore.py` & `devpi-server-6.9.1/test_devpi_server/test_filestore.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_fileutil.py` & `devpi-server-6.9.1/test_devpi_server/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_genconfig.py` & `devpi-server-6.9.1/test_devpi_server/test_genconfig.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_importexport.py` & `devpi-server-6.9.1/test_devpi_server/test_importexport.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_keyfs.py` & `devpi-server-6.9.1/test_devpi_server/test_keyfs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_keyfs_sqlite_fs.py` & `devpi-server-6.9.1/test_devpi_server/test_keyfs_sqlite_fs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_log.py` & `devpi-server-6.9.1/test_devpi_server/test_log.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_main.py` & `devpi-server-6.9.1/test_devpi_server/test_main.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_mirror.py` & `devpi-server-6.9.1/test_devpi_server/test_mirror.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_mirror_no_project_list.py` & `devpi-server-6.9.1/test_devpi_server/test_mirror_no_project_list.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_model.py` & `devpi-server-6.9.1/test_devpi_server/test_model.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_mythread.py` & `devpi-server-6.9.1/test_devpi_server/test_mythread.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_nginx.py` & `devpi-server-6.9.1/test_devpi_server/test_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_nginx_replica.py` & `devpi-server-6.9.1/test_devpi_server/test_nginx_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_permissions.py` & `devpi-server-6.9.1/test_devpi_server/test_permissions.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_readonly.py` & `devpi-server-6.9.1/test_devpi_server/test_readonly.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_replica.py` & `devpi-server-6.9.1/test_devpi_server/test_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_replica_functional.py` & `devpi-server-6.9.1/test_devpi_server/test_replica_functional.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_reqmock.py` & `devpi-server-6.9.1/test_devpi_server/test_reqmock.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_stage_customizer.py` & `devpi-server-6.9.1/test_devpi_server/test_stage_customizer.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_streaming.py` & `devpi-server-6.9.1/test_devpi_server/test_streaming.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_streaming_nginx.py` & `devpi-server-6.9.1/test_devpi_server/test_streaming_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_streaming_replica.py` & `devpi-server-6.9.1/test_devpi_server/test_streaming_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_streaming_replica_nginx.py` & `devpi-server-6.9.1/test_devpi_server/test_streaming_replica_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_view_auth.py` & `devpi-server-6.9.1/test_devpi_server/test_view_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_views.py` & `devpi-server-6.9.1/test_devpi_server/test_views.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_views_patch.py` & `devpi-server-6.9.1/test_devpi_server/test_views_patch.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_views_push_external.py` & `devpi-server-6.9.1/test_devpi_server/test_views_push_external.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/test_devpi_server/test_views_status.py` & `devpi-server-6.9.1/test_devpi_server/test_views_status.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.0/tox.ini` & `devpi-server-6.9.1/tox.ini`

 * *Files identical despite different names*

