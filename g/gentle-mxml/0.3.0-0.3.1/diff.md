# Comparing `tmp/gentle_mxml-0.3.0.tar.gz` & `tmp/gentle_mxml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentle_mxml-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gentle_mxml-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gentle_mxml-0.3.0.tar` & `gentle_mxml-0.3.1.tar`

### file list

```diff
@@ -1,119 +1,199 @@
--rw-r--r--   0        0        0      432 2023-06-09 12:39:00.288853 gentle_mxml-0.3.0/LICENSE
--rw-r--r--   0        0        0     2244 2023-06-25 12:11:00.893469 gentle_mxml-0.3.0/README.md
--rw-r--r--   0        0        0      162 2023-06-25 14:13:36.466085 gentle_mxml-0.3.0/gentle/__init__.py
--rw-r--r--   0        0        0     3716 2023-06-25 12:27:13.516179 gentle_mxml-0.3.0/gentle/__main__.py
--rw-r--r--   0        0        0      967 2023-06-24 19:59:23.234866 gentle_mxml-0.3.0/gentle/generators/__init__.py
--rw-r--r--   0        0        0     1628 2023-06-14 11:48:31.704149 gentle_mxml-0.3.0/gentle/generators/bower.py
--rw-r--r--   0        0        0     3061 2023-06-23 06:42:42.354791 gentle_mxml-0.3.0/gentle/generators/cargo.py
--rw-r--r--   0        0        0     2396 2023-06-11 14:01:29.545936 gentle_mxml-0.3.0/gentle/generators/composer.py
--rw-r--r--   0        0        0     2124 2023-06-25 12:08:57.131595 gentle_mxml-0.3.0/gentle/generators/doap.py
--rw-r--r--   0        0        0     2495 2023-06-21 22:59:00.769937 gentle_mxml-0.3.0/gentle/generators/hpack.py
--rw-r--r--   0        0        0     2672 2023-06-23 06:39:27.842866 gentle_mxml-0.3.0/gentle/generators/npm.py
--rw-r--r--   0        0        0     2602 2023-06-24 19:10:52.669001 gentle_mxml-0.3.0/gentle/generators/pkg_info.py
--rw-r--r--   0        0        0     2329 2023-06-23 06:42:35.538073 gentle_mxml-0.3.0/gentle/generators/pyproject.py
--rw-r--r--   0        0        0     1922 2023-06-11 14:05:23.291217 gentle_mxml-0.3.0/gentle/generators/shards.py
--rw-r--r--   0        0        0     7386 2023-06-23 06:37:52.366830 gentle_mxml-0.3.0/gentle/metadata/__init__.py
--rw-r--r--   0        0        0     3138 2023-06-25 12:04:41.903135 gentle_mxml-0.3.0/gentle/metadata/utils.py
--rw-r--r--   0        0        0        0 2023-06-23 06:33:13.040427 gentle_mxml-0.3.0/gentle/py.typed
--rw-r--r--   0        0        0     1701 2023-06-25 13:11:28.282190 gentle_mxml-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:04:35.028663 gentle_mxml-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:52:07.066278 gentle_mxml-0.3.0/tests/bower/__init__.py
--rw-r--r--   0        0        0      905 2023-06-14 11:52:52.204418 gentle_mxml-0.3.0/tests/bower/aurelia/bower.json
--rw-r--r--   0        0        0       93 2023-06-14 11:53:17.309384 gentle_mxml-0.3.0/tests/bower/aurelia/bower.json.license
--rw-r--r--   0        0        0      151 2023-06-14 11:53:43.708296 gentle_mxml-0.3.0/tests/bower/aurelia/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-14 11:52:46.348659 gentle_mxml-0.3.0/tests/bower/aurelia/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.0/tests/bower/pkg_empty/bower.json
--rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.0/tests/bower/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1111 2023-06-14 11:54:26.724524 gentle_mxml-0.3.0/tests/bower/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.159951 gentle_mxml-0.3.0/tests/cargo/__init__.py
--rw-r--r--   0        0        0     4750 2023-06-21 17:39:19.188683 gentle_mxml-0.3.0/tests/cargo/lemmy/Cargo.toml
--rw-r--r--   0        0        0       83 2023-06-21 17:54:17.087576 gentle_mxml-0.3.0/tests/cargo/lemmy/Cargo.toml.license
--rw-r--r--   0        0        0      163 2023-06-21 17:42:36.044548 gentle_mxml-0.3.0/tests/cargo/lemmy/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 17:39:09.494084 gentle_mxml-0.3.0/tests/cargo/lemmy/metadata.xml.license
--rw-r--r--   0        0        0     2581 2023-06-07 19:44:08.872681 gentle_mxml-0.3.0/tests/cargo/orjson/Cargo.toml
--rw-r--r--   0        0        0       95 2023-06-07 19:44:24.198957 gentle_mxml-0.3.0/tests/cargo/orjson/Cargo.toml.license
--rw-r--r--   0        0        0      189 2023-06-07 19:42:12.112203 gentle_mxml-0.3.0/tests/cargo/orjson/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 19:41:23.961480 gentle_mxml-0.3.0/tests/cargo/orjson/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.0/tests/cargo/pkg_empty/Cargo.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.0/tests/cargo/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1119 2023-06-21 17:46:02.450018 gentle_mxml-0.3.0/tests/cargo/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.862715 gentle_mxml-0.3.0/tests/composer/__init__.py
--rw-r--r--   0        0        0     3329 2023-06-11 13:56:25.593575 gentle_mxml-0.3.0/tests/composer/composer/composer.json
--rw-r--r--   0        0        0      161 2023-06-11 13:58:46.476717 gentle_mxml-0.3.0/tests/composer/composer/composer.json.license
--rw-r--r--   0        0        0      318 2023-06-11 14:01:02.564058 gentle_mxml-0.3.0/tests/composer/composer/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-11 13:57:30.625871 gentle_mxml-0.3.0/tests/composer/composer/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.0/tests/composer/pkg_empty/composer.json
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.0/tests/composer/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1127 2023-06-11 13:57:14.003562 gentle_mxml-0.3.0/tests/composer/test_generator.py
--rw-r--r--   0        0        0      290 2023-06-07 15:18:39.595705 gentle_mxml-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-25 11:57:38.439617 gentle_mxml-0.3.0/tests/doap/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-25 11:59:51.296133 gentle_mxml-0.3.0/tests/doap/gnome-calls/calls.doap
--rw-r--r--   0        0        0      193 2023-06-25 12:01:58.282890 gentle_mxml-0.3.0/tests/doap/gnome-calls/calls.doap.license
--rw-r--r--   0        0        0      329 2023-06-25 12:03:47.156396 gentle_mxml-0.3.0/tests/doap/gnome-calls/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-25 12:00:30.912497 gentle_mxml-0.3.0/tests/doap/gnome-calls/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-25 11:57:38.441617 gentle_mxml-0.3.0/tests/doap/pkg_empty/null.doap
--rw-r--r--   0        0        0        0 2023-06-25 11:58:21.257850 gentle_mxml-0.3.0/tests/doap/pkg_multiple/one.doap
--rw-r--r--   0        0        0        0 2023-06-25 11:58:24.041735 gentle_mxml-0.3.0/tests/doap/pkg_multiple/two.doap
--rw-r--r--   0        0        0        0 2023-06-25 11:57:38.444617 gentle_mxml-0.3.0/tests/doap/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1243 2023-06-25 11:59:31.351956 gentle_mxml-0.3.0/tests/doap/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-21 23:06:21.776769 gentle_mxml-0.3.0/tests/hpack/__init__.py
--rw-r--r--   0        0        0      197 2023-06-21 23:10:21.212904 gentle_mxml-0.3.0/tests/hpack/hpack/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 23:09:22.249333 gentle_mxml-0.3.0/tests/hpack/hpack/metadata.xml.license
--rw-r--r--   0        0        0     1398 2023-06-21 23:08:08.575369 gentle_mxml-0.3.0/tests/hpack/hpack/package.yaml
--rw-r--r--   0        0        0       90 2023-06-21 23:09:09.245869 gentle_mxml-0.3.0/tests/hpack/hpack/package.yaml.license
--rw-r--r--   0        0        0        0 2023-06-21 23:06:21.780768 gentle_mxml-0.3.0/tests/hpack/pkg_empty/package.yaml
--rw-r--r--   0        0        0        0 2023-06-21 23:06:21.783768 gentle_mxml-0.3.0/tests/hpack/pkg_none/.gitkeep
--rw-r--r--   0        0        0      117 2023-06-21 23:11:51.765173 gentle_mxml-0.3.0/tests/hpack/stack/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 23:10:32.554437 gentle_mxml-0.3.0/tests/hpack/stack/metadata.xml.license
--rw-r--r--   0        0        0    10727 2023-06-21 23:11:25.944237 gentle_mxml-0.3.0/tests/hpack/stack/package.yaml
--rw-r--r--   0        0        0       91 2023-06-21 23:16:13.343396 gentle_mxml-0.3.0/tests/hpack/stack/package.yaml.license
--rw-r--r--   0        0        0     1117 2023-06-21 23:07:37.239659 gentle_mxml-0.3.0/tests/hpack/test_generator.py
--rw-r--r--   0        0        0      168 2023-06-07 14:51:10.813952 gentle_mxml-0.3.0/tests/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 15:22:49.997859 gentle_mxml-0.3.0/tests/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.990442 gentle_mxml-0.3.0/tests/npm/__init__.py
--rw-r--r--   0        0        0      234 2023-06-08 00:13:02.172234 gentle_mxml-0.3.0/tests/npm/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-08 00:10:46.617642 gentle_mxml-0.3.0/tests/npm/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0     3382 2023-06-08 00:13:19.251427 gentle_mxml-0.3.0/tests/npm/mkdocs-material/package.json
--rw-r--r--   0        0        0      103 2023-06-08 00:10:46.616642 gentle_mxml-0.3.0/tests/npm/mkdocs-material/package.json.license
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.997442 gentle_mxml-0.3.0/tests/npm/pkg_empty/package.json
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.998442 gentle_mxml-0.3.0/tests/npm/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1109 2023-06-07 23:57:05.916436 gentle_mxml-0.3.0/tests/npm/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-24 18:59:44.866553 gentle_mxml-0.3.0/tests/pkg_info/__init__.py
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/PKG-INFO
--rw-r--r--   0        0        0      103 2023-06-24 18:59:44.869553 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/PKG-INFO.license
--rw-r--r--   0        0        0      303 2023-06-24 19:09:17.624922 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-24 18:59:44.869553 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.0/tests/pkg_info/pkg_empty/PKG-INFO
--rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.0/tests/pkg_info/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1883 2023-02-18 15:55:47.929912 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/PKG-INFO
--rw-r--r--   0        0        0       92 2023-06-24 18:59:44.868553 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/PKG-INFO.license
--rw-r--r--   0        0        0      214 2023-06-24 18:59:44.868553 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-24 18:59:44.868553 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/metadata.xml.license
--rw-r--r--   0        0        0     1142 2023-06-24 19:05:20.815692 gentle_mxml-0.3.0/tests/pkg_info/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.372752 gentle_mxml-0.3.0/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      330 2023-06-07 19:13:56.979345 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 19:07:24.968873 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0     2949 2023-06-07 19:07:42.936024 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/pyproject.toml
--rw-r--r--   0        0        0      103 2023-06-07 19:11:03.167560 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/pyproject.toml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.0/tests/pyproject/pkg_empty/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.0/tests/pyproject/pkg_none/.gitkeep
--rw-r--r--   0        0        0      214 2023-06-07 18:58:47.333338 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 18:59:06.048453 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/metadata.xml.license
--rw-r--r--   0        0        0     2549 2023-06-07 18:54:37.693136 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/pyproject.toml
--rw-r--r--   0        0        0       92 2023-06-07 18:56:45.335103 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/pyproject.toml.license
--rw-r--r--   0        0        0     1151 2023-06-07 19:38:35.578442 gentle_mxml-0.3.0/tests/pyproject/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:05:22.876399 gentle_mxml-0.3.0/tests/shards/__init__.py
--rw-r--r--   0        0        0      262 2023-06-07 16:08:13.258065 gentle_mxml-0.3.0/tests/shards/athena-spec/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 16:19:57.337776 gentle_mxml-0.3.0/tests/shards/athena-spec/metadata.xml.license
--rw-r--r--   0        0        0      287 2023-06-07 15:44:23.136690 gentle_mxml-0.3.0/tests/shards/athena-spec/shard.yml
--rw-r--r--   0        0        0       97 2023-06-07 16:19:15.122771 gentle_mxml-0.3.0/tests/shards/athena-spec/shard.yml.license
--rw-r--r--   0        0        0      254 2023-06-07 18:34:22.044597 gentle_mxml-0.3.0/tests/shards/exception_page/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 18:20:08.443939 gentle_mxml-0.3.0/tests/shards/exception_page/metadata.xml.license
--rw-r--r--   0        0        0      432 2023-06-07 18:17:35.813152 gentle_mxml-0.3.0/tests/shards/exception_page/shard.yml
--rw-r--r--   0        0        0      208 2023-06-07 18:19:13.172551 gentle_mxml-0.3.0/tests/shards/exception_page/shard.yml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:12:58.225856 gentle_mxml-0.3.0/tests/shards/pkg_empty/shard.yml
--rw-r--r--   0        0        0        0 2023-06-07 14:55:14.309353 gentle_mxml-0.3.0/tests/shards/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1137 2023-06-07 19:38:04.782898 gentle_mxml-0.3.0/tests/shards/test_generator.py
--rw-r--r--   0        0        0     1064 2023-06-23 06:29:53.471712 gentle_mxml-0.3.0/tests/test_metadata.py
--rw-r--r--   0        0        0      361 2023-06-07 16:03:33.900274 gentle_mxml-0.3.0/tests/utils.py
--rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 gentle_mxml-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      177 2023-07-01 23:16:33.075157 gentle_mxml-0.3.1/.bumpversion.cfg
+-rw-r--r--   0        0        0       85 2023-06-25 13:58:30.249547 gentle_mxml-0.3.1/.bumpversion.cfg.license
+-rw-r--r--   0        0        0      384 2023-06-26 18:36:20.326251 gentle_mxml-0.3.1/.drone.yml
+-rw-r--r--   0        0        0      153 2023-07-01 23:15:07.469678 gentle_mxml-0.3.1/.gitignore
+-rw-r--r--   0        0        0      432 2023-06-09 12:39:00.288853 gentle_mxml-0.3.1/LICENSE
+-rw-r--r--   0        0        0    34020 2023-06-21 17:54:08.857916 gentle_mxml-0.3.1/LICENSES/AGPL-3.0-only.txt
+-rw-r--r--   0        0        0    10280 2023-06-07 19:43:48.069665 gentle_mxml-0.3.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     1460 2023-06-21 23:16:06.355684 gentle_mxml-0.3.1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0     7048 2022-11-14 10:12:41.100101 gentle_mxml-0.3.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-06-25 12:08:33.459576 gentle_mxml-0.3.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-06-07 16:20:14.601959 gentle_mxml-0.3.1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      432 2022-11-14 10:12:40.671121 gentle_mxml-0.3.1/LICENSES/WTFPL.txt
+-rw-r--r--   0        0        0     2343 2023-06-26 18:30:42.288936 gentle_mxml-0.3.1/README.md
+-rw-r--r--   0        0        0      230 2023-06-25 13:09:13.402778 gentle_mxml-0.3.1/docs/_build/.buildinfo
+-rw-r--r--   0        0        0     9939 2023-06-25 13:09:12.274825 gentle_mxml-0.3.1/docs/_build/.doctrees/contributing.doctree
+-rw-r--r--   0        0        0   119130 2023-06-25 13:09:12.772805 gentle_mxml-0.3.1/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     4893 2023-06-25 13:09:12.284825 gentle_mxml-0.3.1/docs/_build/.doctrees/getting-started.doctree
+-rw-r--r--   0        0        0     5207 2023-06-25 13:09:12.293825 gentle_mxml-0.3.1/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0        0        0     6471 2023-06-25 13:09:12.307824 gentle_mxml-0.3.1/docs/_build/.doctrees/installation.doctree
+-rw-r--r--   0        0        0    43744 2023-06-25 13:09:12.755805 gentle_mxml-0.3.1/docs/_build/.doctrees/reference.doctree
+-rw-r--r--   0        0        0     4901 2023-06-25 13:09:12.765805 gentle_mxml-0.3.1/docs/_build/.doctrees/toc.doctree
+-rw-r--r--   0        0        0     8129 2023-06-25 13:09:13.319782 gentle_mxml-0.3.1/docs/_build/404.html
+-rw-r--r--   0        0        0     1458 2023-06-25 12:55:03.457995 gentle_mxml-0.3.1/docs/_build/_sources/contributing.rst.txt
+-rw-r--r--   0        0        0      450 2023-06-25 12:49:53.056856 gentle_mxml-0.3.1/docs/_build/_sources/getting-started.rst.txt
+-rw-r--r--   0        0        0      456 2023-06-25 12:43:37.704408 gentle_mxml-0.3.1/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0        0        0      619 2023-06-25 12:45:58.431577 gentle_mxml-0.3.1/docs/_build/_sources/installation.rst.txt
+-rw-r--r--   0        0        0      301 2023-06-25 13:09:09.222952 gentle_mxml-0.3.1/docs/_build/_sources/reference.rst.txt
+-rw-r--r--   0        0        0      321 2023-06-25 13:05:45.723384 gentle_mxml-0.3.1/docs/_build/_sources/toc.rst.txt
+-rw-r--r--   0        0        0    14813 2023-06-25 13:09:13.360780 gentle_mxml-0.3.1/docs/_build/_static/basic.css
+-rw-r--r--   0        0        0     4472 2023-06-20 06:40:23.406098 gentle_mxml-0.3.1/docs/_build/_static/doctools.js
+-rw-r--r--   0        0        0      417 2023-06-25 13:09:13.349781 gentle_mxml-0.3.1/docs/_build/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-20 06:40:23.406098 gentle_mxml-0.3.1/docs/_build/_static/file.png
+-rw-r--r--   0        0        0     1249 2023-06-25 13:09:13.379779 gentle_mxml-0.3.1/docs/_build/_static/insipid-sidebar-readthedocs.css
+-rw-r--r--   0        0        0    10567 2023-06-25 13:09:13.375780 gentle_mxml-0.3.1/docs/_build/_static/insipid-sidebar.js
+-rw-r--r--   0        0        0    22222 2023-06-25 13:09:13.401779 gentle_mxml-0.3.1/docs/_build/_static/insipid.css
+-rw-r--r--   0        0        0     5269 2023-05-08 04:53:11.827459 gentle_mxml-0.3.1/docs/_build/_static/insipid.js
+-rw-r--r--   0        0        0     4758 2023-06-25 13:09:13.354781 gentle_mxml-0.3.1/docs/_build/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-20 06:40:23.407098 gentle_mxml-0.3.1/docs/_build/_static/minus.png
+-rw-r--r--   0        0        0       90 2023-06-20 06:40:23.407098 gentle_mxml-0.3.1/docs/_build/_static/plus.png
+-rw-r--r--   0        0        0     4846 2023-06-25 13:09:13.343781 gentle_mxml-0.3.1/docs/_build/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-20 06:40:23.408098 gentle_mxml-0.3.1/docs/_build/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-20 06:40:23.408098 gentle_mxml-0.3.1/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    17289 2023-06-25 13:09:13.115790 gentle_mxml-0.3.1/docs/_build/contributing.html
+-rw-r--r--   0        0        0    12858 2023-06-25 13:09:13.286783 gentle_mxml-0.3.1/docs/_build/genindex.html
+-rw-r--r--   0        0        0    13806 2023-06-25 13:09:13.132790 gentle_mxml-0.3.1/docs/_build/getting-started.html
+-rw-r--r--   0        0        0    13514 2023-06-25 13:09:13.148789 gentle_mxml-0.3.1/docs/_build/index.html
+-rw-r--r--   0        0        0    14768 2023-06-25 13:09:13.164788 gentle_mxml-0.3.1/docs/_build/installation.html
+-rw-r--r--   0        0        0      508 2023-06-25 13:09:13.405779 gentle_mxml-0.3.1/docs/_build/objects.inv
+-rw-r--r--   0        0        0     8996 2023-06-25 13:09:13.312782 gentle_mxml-0.3.1/docs/_build/py-modindex.html
+-rw-r--r--   0        0        0    28930 2023-06-25 13:09:13.221786 gentle_mxml-0.3.1/docs/_build/reference.html
+-rw-r--r--   0        0        0     7918 2023-06-25 13:09:13.341781 gentle_mxml-0.3.1/docs/_build/search.html
+-rw-r--r--   0        0        0     7181 2023-06-25 13:09:13.404778 gentle_mxml-0.3.1/docs/_build/searchindex.js
+-rw-r--r--   0        0        0      702 2023-06-25 13:09:13.407778 gentle_mxml-0.3.1/docs/_build/sitemap.xml
+-rw-r--r--   0        0        0    15966 2023-06-25 13:09:13.248785 gentle_mxml-0.3.1/docs/_build/toc.html
+-rw-r--r--   0        0        0        0 2023-06-25 12:32:02.812195 gentle_mxml-0.3.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-25 12:32:06.444044 gentle_mxml-0.3.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      217 2023-06-26 13:39:30.085763 gentle_mxml-0.3.1/docs/api/gentle.generators.bower.rst
+-rw-r--r--   0        0        0      217 2023-06-26 13:39:30.096762 gentle_mxml-0.3.1/docs/api/gentle.generators.cargo.rst
+-rw-r--r--   0        0        0      229 2023-06-26 13:39:30.105762 gentle_mxml-0.3.1/docs/api/gentle.generators.composer.rst
+-rw-r--r--   0        0        0      213 2023-06-26 13:39:30.118761 gentle_mxml-0.3.1/docs/api/gentle.generators.doap.rst
+-rw-r--r--   0        0        0      217 2023-06-26 13:39:30.129761 gentle_mxml-0.3.1/docs/api/gentle.generators.hpack.rst
+-rw-r--r--   0        0        0      209 2023-06-26 13:39:30.139761 gentle_mxml-0.3.1/docs/api/gentle.generators.npm.rst
+-rw-r--r--   0        0        0      230 2023-06-26 13:39:30.149760 gentle_mxml-0.3.1/docs/api/gentle.generators.pkg_info.rst
+-rw-r--r--   0        0        0      233 2023-06-26 13:39:30.159760 gentle_mxml-0.3.1/docs/api/gentle.generators.pyproject.rst
+-rw-r--r--   0        0        0      521 2023-06-26 13:39:30.047764 gentle_mxml-0.3.1/docs/api/gentle.generators.rst
+-rw-r--r--   0        0        0      221 2023-06-26 13:39:30.170759 gentle_mxml-0.3.1/docs/api/gentle.generators.shards.rst
+-rw-r--r--   0        0        0      326 2023-06-26 13:39:30.059764 gentle_mxml-0.3.1/docs/api/gentle.metadata.rst
+-rw-r--r--   0        0        0      241 2023-06-26 13:39:30.178759 gentle_mxml-0.3.1/docs/api/gentle.metadata.utils.rst
+-rw-r--r--   0        0        0      204 2023-06-26 13:39:29.750777 gentle_mxml-0.3.1/docs/api/gentle.rst
+-rw-r--r--   0        0        0     1722 2023-07-01 23:16:33.074157 gentle_mxml-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0     1614 2023-06-26 18:32:13.013266 gentle_mxml-0.3.1/docs/contributing.rst
+-rw-r--r--   0        0        0      450 2023-06-25 12:49:53.056856 gentle_mxml-0.3.1/docs/getting-started.rst
+-rw-r--r--   0        0        0      456 2023-06-25 12:43:37.704408 gentle_mxml-0.3.1/docs/index.rst
+-rw-r--r--   0        0        0      546 2023-06-26 18:21:56.391213 gentle_mxml-0.3.1/docs/installation.rst
+-rw-r--r--   0        0        0      197 2023-06-26 13:35:46.178048 gentle_mxml-0.3.1/docs/reference.rst
+-rw-r--r--   0        0        0      305 2023-07-01 22:50:55.661323 gentle_mxml-0.3.1/docs/release-notes.rst
+-rw-r--r--   0        0        0      338 2023-07-01 22:51:29.247945 gentle_mxml-0.3.1/docs/toc.rst
+-rw-r--r--   0        0        0      162 2023-07-01 23:16:33.074157 gentle_mxml-0.3.1/gentle/__init__.py
+-rw-r--r--   0        0        0     2512 2023-07-01 22:40:42.721486 gentle_mxml-0.3.1/gentle/__main__.py
+-rw-r--r--   0        0        0      967 2023-06-28 15:28:10.118254 gentle_mxml-0.3.1/gentle/generators/__init__.py
+-rw-r--r--   0        0        0     1661 2023-06-28 22:07:13.223836 gentle_mxml-0.3.1/gentle/generators/bower.py
+-rw-r--r--   0        0        0     3061 2023-06-23 06:42:42.354791 gentle_mxml-0.3.1/gentle/generators/cargo.py
+-rw-r--r--   0        0        0     2429 2023-06-28 22:08:17.555203 gentle_mxml-0.3.1/gentle/generators/composer.py
+-rw-r--r--   0        0        0     2157 2023-06-28 22:08:38.229357 gentle_mxml-0.3.1/gentle/generators/doap.py
+-rw-r--r--   0        0        0     2528 2023-06-28 22:08:52.124788 gentle_mxml-0.3.1/gentle/generators/hpack.py
+-rw-r--r--   0        0        0     2705 2023-06-28 22:09:13.317921 gentle_mxml-0.3.1/gentle/generators/npm.py
+-rw-r--r--   0        0        0      376 2023-06-26 11:47:57.742065 gentle_mxml-0.3.1/gentle/generators/python/__init__.py
+-rw-r--r--   0        0        0     2625 2023-06-26 11:53:28.465383 gentle_mxml-0.3.1/gentle/generators/python/pkg_info.py
+-rw-r--r--   0        0        0     2385 2023-06-28 22:07:44.380561 gentle_mxml-0.3.1/gentle/generators/python/pyproject.py
+-rw-r--r--   0        0        0     1922 2023-06-11 14:05:23.291217 gentle_mxml-0.3.1/gentle/generators/shards.py
+-rw-r--r--   0        0        0     3642 2023-06-28 22:03:01.445140 gentle_mxml-0.3.1/gentle/metadata/__init__.py
+-rw-r--r--   0        0        0     1555 2023-06-28 21:25:57.964830 gentle_mxml-0.3.1/gentle/metadata/types.py
+-rw-r--r--   0        0        0     3206 2023-06-26 13:40:45.503635 gentle_mxml-0.3.1/gentle/metadata/utils.py
+-rw-r--r--   0        0        0        0 2023-07-01 22:18:06.920291 gentle_mxml-0.3.1/gentle/pms/__init__.py
+-rw-r--r--   0        0        0     3051 2023-07-01 22:16:34.191111 gentle_mxml-0.3.1/gentle/pms/portagepm.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:33:13.040427 gentle_mxml-0.3.1/gentle/py.typed
+-rw-r--r--   0        0        0     1762 2023-06-26 18:38:20.296348 gentle_mxml-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:04:35.028663 gentle_mxml-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:52:07.066278 gentle_mxml-0.3.1/tests/bower/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-14 11:52:52.204418 gentle_mxml-0.3.1/tests/bower/aurelia/bower.json
+-rw-r--r--   0        0        0       93 2023-06-14 11:53:17.309384 gentle_mxml-0.3.1/tests/bower/aurelia/bower.json.license
+-rw-r--r--   0        0        0      151 2023-06-14 11:53:43.708296 gentle_mxml-0.3.1/tests/bower/aurelia/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-14 11:52:46.348659 gentle_mxml-0.3.1/tests/bower/aurelia/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.1/tests/bower/pkg_empty/bower.json
+-rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.1/tests/bower/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1111 2023-06-14 11:54:26.724524 gentle_mxml-0.3.1/tests/bower/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.159951 gentle_mxml-0.3.1/tests/cargo/__init__.py
+-rw-r--r--   0        0        0     4750 2023-06-21 17:39:19.188683 gentle_mxml-0.3.1/tests/cargo/lemmy/Cargo.toml
+-rw-r--r--   0        0        0       83 2023-06-21 17:54:17.087576 gentle_mxml-0.3.1/tests/cargo/lemmy/Cargo.toml.license
+-rw-r--r--   0        0        0      163 2023-06-21 17:42:36.044548 gentle_mxml-0.3.1/tests/cargo/lemmy/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 17:39:09.494084 gentle_mxml-0.3.1/tests/cargo/lemmy/metadata.xml.license
+-rw-r--r--   0        0        0     2581 2023-06-07 19:44:08.872681 gentle_mxml-0.3.1/tests/cargo/orjson/Cargo.toml
+-rw-r--r--   0        0        0       95 2023-06-07 19:44:24.198957 gentle_mxml-0.3.1/tests/cargo/orjson/Cargo.toml.license
+-rw-r--r--   0        0        0      189 2023-06-07 19:42:12.112203 gentle_mxml-0.3.1/tests/cargo/orjson/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 19:41:23.961480 gentle_mxml-0.3.1/tests/cargo/orjson/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.1/tests/cargo/pkg_empty/Cargo.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.1/tests/cargo/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1119 2023-06-21 17:46:02.450018 gentle_mxml-0.3.1/tests/cargo/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.862715 gentle_mxml-0.3.1/tests/composer/__init__.py
+-rw-r--r--   0        0        0     3329 2023-06-11 13:56:25.593575 gentle_mxml-0.3.1/tests/composer/composer/composer.json
+-rw-r--r--   0        0        0      161 2023-06-11 13:58:46.476717 gentle_mxml-0.3.1/tests/composer/composer/composer.json.license
+-rw-r--r--   0        0        0      318 2023-06-11 14:01:02.564058 gentle_mxml-0.3.1/tests/composer/composer/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-11 13:57:30.625871 gentle_mxml-0.3.1/tests/composer/composer/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.1/tests/composer/pkg_empty/composer.json
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.1/tests/composer/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1127 2023-06-11 13:57:14.003562 gentle_mxml-0.3.1/tests/composer/test_generator.py
+-rw-r--r--   0        0        0      346 2023-06-28 22:01:32.014811 gentle_mxml-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.439617 gentle_mxml-0.3.1/tests/doap/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-25 11:59:51.296133 gentle_mxml-0.3.1/tests/doap/gnome-calls/calls.doap
+-rw-r--r--   0        0        0      193 2023-06-25 12:01:58.282890 gentle_mxml-0.3.1/tests/doap/gnome-calls/calls.doap.license
+-rw-r--r--   0        0        0      329 2023-06-25 12:03:47.156396 gentle_mxml-0.3.1/tests/doap/gnome-calls/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-25 12:00:30.912497 gentle_mxml-0.3.1/tests/doap/gnome-calls/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.441617 gentle_mxml-0.3.1/tests/doap/pkg_empty/null.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:21.257850 gentle_mxml-0.3.1/tests/doap/pkg_multiple/one.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:24.041735 gentle_mxml-0.3.1/tests/doap/pkg_multiple/two.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.444617 gentle_mxml-0.3.1/tests/doap/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1243 2023-06-25 11:59:31.351956 gentle_mxml-0.3.1/tests/doap/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.776769 gentle_mxml-0.3.1/tests/hpack/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-21 23:10:21.212904 gentle_mxml-0.3.1/tests/hpack/hpack/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 23:09:22.249333 gentle_mxml-0.3.1/tests/hpack/hpack/metadata.xml.license
+-rw-r--r--   0        0        0     1398 2023-06-21 23:08:08.575369 gentle_mxml-0.3.1/tests/hpack/hpack/package.yaml
+-rw-r--r--   0        0        0       90 2023-06-21 23:09:09.245869 gentle_mxml-0.3.1/tests/hpack/hpack/package.yaml.license
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.780768 gentle_mxml-0.3.1/tests/hpack/pkg_empty/package.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.783768 gentle_mxml-0.3.1/tests/hpack/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      117 2023-06-21 23:11:51.765173 gentle_mxml-0.3.1/tests/hpack/stack/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 23:10:32.554437 gentle_mxml-0.3.1/tests/hpack/stack/metadata.xml.license
+-rw-r--r--   0        0        0    10727 2023-06-21 23:11:25.944237 gentle_mxml-0.3.1/tests/hpack/stack/package.yaml
+-rw-r--r--   0        0        0       91 2023-06-21 23:16:13.343396 gentle_mxml-0.3.1/tests/hpack/stack/package.yaml.license
+-rw-r--r--   0        0        0     1117 2023-06-21 23:07:37.239659 gentle_mxml-0.3.1/tests/hpack/test_generator.py
+-rw-r--r--   0        0        0      168 2023-06-07 14:51:10.813952 gentle_mxml-0.3.1/tests/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 15:22:49.997859 gentle_mxml-0.3.1/tests/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.990442 gentle_mxml-0.3.1/tests/npm/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-08 00:13:02.172234 gentle_mxml-0.3.1/tests/npm/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-08 00:10:46.617642 gentle_mxml-0.3.1/tests/npm/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0     3382 2023-06-08 00:13:19.251427 gentle_mxml-0.3.1/tests/npm/mkdocs-material/package.json
+-rw-r--r--   0        0        0      103 2023-06-08 00:10:46.616642 gentle_mxml-0.3.1/tests/npm/mkdocs-material/package.json.license
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.997442 gentle_mxml-0.3.1/tests/npm/pkg_empty/package.json
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.998442 gentle_mxml-0.3.1/tests/npm/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1109 2023-06-07 23:57:05.916436 gentle_mxml-0.3.1/tests/npm/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.866553 gentle_mxml-0.3.1/tests/pkg_info/__init__.py
+-rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-06-24 18:59:44.869553 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/PKG-INFO.license
+-rw-r--r--   0        0        0      303 2023-06-24 19:09:17.624922 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-24 18:59:44.869553 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.1/tests/pkg_info/pkg_empty/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.1/tests/pkg_info/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1883 2023-02-18 15:55:47.929912 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/PKG-INFO
+-rw-r--r--   0        0        0       92 2023-06-24 18:59:44.868553 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/PKG-INFO.license
+-rw-r--r--   0        0        0      214 2023-06-24 18:59:44.868553 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-24 18:59:44.868553 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/metadata.xml.license
+-rw-r--r--   0        0        0     1149 2023-06-26 11:51:52.074371 gentle_mxml-0.3.1/tests/pkg_info/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.372752 gentle_mxml-0.3.1/tests/pyproject/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-07 19:13:56.979345 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 19:07:24.968873 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0     2949 2023-06-07 19:07:42.936024 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-06-07 19:11:03.167560 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/pyproject.toml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.1/tests/pyproject/pkg_empty/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.1/tests/pyproject/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      214 2023-06-07 18:58:47.333338 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 18:59:06.048453 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/metadata.xml.license
+-rw-r--r--   0        0        0     2549 2023-06-07 18:54:37.693136 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-06-07 18:56:45.335103 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/pyproject.toml.license
+-rw-r--r--   0        0        0     1158 2023-06-26 11:51:38.121948 gentle_mxml-0.3.1/tests/pyproject/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:05:22.876399 gentle_mxml-0.3.1/tests/shards/__init__.py
+-rw-r--r--   0        0        0      262 2023-06-07 16:08:13.258065 gentle_mxml-0.3.1/tests/shards/athena-spec/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 16:19:57.337776 gentle_mxml-0.3.1/tests/shards/athena-spec/metadata.xml.license
+-rw-r--r--   0        0        0      287 2023-06-07 15:44:23.136690 gentle_mxml-0.3.1/tests/shards/athena-spec/shard.yml
+-rw-r--r--   0        0        0       97 2023-06-07 16:19:15.122771 gentle_mxml-0.3.1/tests/shards/athena-spec/shard.yml.license
+-rw-r--r--   0        0        0      254 2023-06-07 18:34:22.044597 gentle_mxml-0.3.1/tests/shards/exception_page/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 18:20:08.443939 gentle_mxml-0.3.1/tests/shards/exception_page/metadata.xml.license
+-rw-r--r--   0        0        0      432 2023-06-07 18:17:35.813152 gentle_mxml-0.3.1/tests/shards/exception_page/shard.yml
+-rw-r--r--   0        0        0      208 2023-06-07 18:19:13.172551 gentle_mxml-0.3.1/tests/shards/exception_page/shard.yml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:12:58.225856 gentle_mxml-0.3.1/tests/shards/pkg_empty/shard.yml
+-rw-r--r--   0        0        0        0 2023-06-07 14:55:14.309353 gentle_mxml-0.3.1/tests/shards/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1137 2023-06-07 19:38:04.782898 gentle_mxml-0.3.1/tests/shards/test_generator.py
+-rw-r--r--   0        0        0     1239 2023-06-28 22:09:49.764429 gentle_mxml-0.3.1/tests/test_metadata.py
+-rw-r--r--   0        0        0      361 2023-06-07 16:03:33.900274 gentle_mxml-0.3.1/tests/utils.py
+-rw-r--r--   0        0        0      619 2023-06-26 18:38:06.720903 gentle_mxml-0.3.1/tox.ini
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 gentle_mxml-0.3.1/PKG-INFO
```

### Comparing `gentle_mxml-0.3.0/README.md` & `gentle_mxml-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 Installing
 ----------
 
 ### Gentoo
 
 ```sh
-eselect repository enable guru
 emerge app-portage/gentle
 ```
 
 ### Other systems
 
 `pip install gentle-mxml --user`
 
@@ -57,27 +56,31 @@
 
 Contributing
 ------------
 
 Patches and pull requests are welcome. Please use either [git-send-email(1)][1]
 or [git-request-pull(1)][2], addressed to <cyber@sysrq.in>.
 
+If you prefer GitHub-style workflow, use the [mirror repo][gh] to send pull
+requests.
+
 Your commit message should conform to the following standard:
 
 ```
 file/changed: Concice and complete statement of the purpose
 
 This is the body of the commit message.  The line above is the
 summary.  The summary should be no more than 72 chars long.  The
 body can be more freely formatted, but make it look nice.  Make
 sure to reference any bug reports and other contributors.  Make
 sure the correct authorship appears.
 ```
 
 [1]: https://git-send-email.io/
 [2]: https://git-scm.com/docs/git-request-pull
+[gh]: http://github.com/cybertailor/gentle
 
 
 License
 -------
 
 WTFPL
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/__init__.py` & `gentle_mxml-0.3.1/gentle/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/gentle/generators/bower.py` & `gentle_mxml-0.3.1/gentle/generators/bower.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 """
 
 import json
 import logging
 from pathlib import Path
 
 from gentle.generators import AbstractGenerator
-from gentle.metadata import Person, MetadataXML
+from gentle.metadata import MetadataXML
+from gentle.metadata.types import Person
 from gentle.metadata.utils import extract_name_email, extract_remote_id
 
 logger = logging.getLogger("bower")
 
 
 class BowerGenerator(AbstractGenerator):
     def __init__(self, srcdir: Path):
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/cargo.py` & `gentle_mxml-0.3.1/gentle/generators/cargo.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/gentle/generators/composer.py` & `gentle_mxml-0.3.1/gentle/generators/composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 """
 
 import json
 import logging
 from pathlib import Path
 
 from gentle.generators import AbstractGenerator
-from gentle.metadata import Person, MetadataXML
+from gentle.metadata import MetadataXML
+from gentle.metadata.types import Person
 from gentle.metadata.utils import extract_remote_id
 
 logger = logging.getLogger("composer")
 
 
 class ComposerGenerator(AbstractGenerator):
     def __init__(self, srcdir: Path):
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/doap.py` & `gentle_mxml-0.3.1/gentle/generators/doap.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 """
 
 import logging
 from pathlib import Path
 from xml.sax._exceptions import SAXException
 
 from gentle.generators import AbstractGenerator
-from gentle.metadata import MetadataXML, Person
+from gentle.metadata import MetadataXML
+from gentle.metadata.types import Person
 from gentle.metadata.utils import extract_remote_id
 
 try:
     from rdflib import Graph
     from rdflib.namespace import DOAP, FOAF
     _HAS_RDFLIB = True
 except ModuleNotFoundError:
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/hpack.py` & `gentle_mxml-0.3.1/gentle/generators/hpack.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 * Remote ID
 """
 
 import logging
 from pathlib import Path
 
 from gentle.generators import AbstractGenerator
-from gentle.metadata import MetadataXML, RemoteID
+from gentle.metadata import MetadataXML
+from gentle.metadata.types import RemoteID
 from gentle.metadata.utils import extract_name_email, extract_remote_id
 
 try:
     import yaml
     from yaml import CLoader
     _HAS_PYYAML = True
 except ModuleNotFoundError:
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/npm.py` & `gentle_mxml-0.3.1/gentle/generators/npm.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 """
 
 import json
 import logging
 from pathlib import Path
 
 from gentle.generators import AbstractGenerator
-from gentle.metadata import Person, RemoteID, MetadataXML
+from gentle.metadata import MetadataXML
+from gentle.metadata.types import Person, RemoteID
 from gentle.metadata.utils import extract_name_email, extract_remote_id
 
 logger = logging.getLogger("npm")
 
 
 class NpmGenerator(AbstractGenerator):
     def __init__(self, srcdir: Path):
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/pkg_info.py` & `gentle_mxml-0.3.1/gentle/generators/python/pkg_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 * Remote ID
 """
 
 import logging
 from pathlib import Path
 
 from gentle.generators import AbstractGenerator
+from gentle.generators.python import (
+    BUG_TRACKER_LABELS,
+    CHANGELOG_LABELS,
+    DOCS_LABELS,
+    HOME_REPO_LABELS
+)
 from gentle.metadata import MetadataXML
 from gentle.metadata.utils import extract_name_email, extract_remote_id
 
 try:
     import pkginfo
     _HAS_PKGINFO_LIB = True
 except ModuleNotFoundError:
@@ -58,21 +64,20 @@
             if (remote_id := extract_remote_id(package.home_page)) is not None:
                 mxml.add_upstream_remote_id(remote_id)
 
         for url in package.project_urls:
             name, value = [entry.strip()
                            for entry in url.split(",", maxsplit=1)]
             logger.info("Found %s: %s", name, value)
-            match name.lower():
-                case "bug tracker" | "bugtracker" | "bugs" | "issues":
-                    mxml.set_upstream_bugs_to(value)
-                case "changelog" | "changes":
-                    mxml.set_upstream_changelog(value)
-                case "doc" | "docs" | "documentation":
-                    mxml.set_upstream_doc(value)
-                case "source" | "repo" | "repository" | "home" | "homepage":
-                    if (remote_id := extract_remote_id(value)) is not None:
-                        mxml.add_upstream_remote_id(remote_id)
+            if name.lower() in BUG_TRACKER_LABELS:
+                mxml.set_upstream_bugs_to(value)
+            elif name.lower() in CHANGELOG_LABELS:
+                mxml.set_upstream_changelog(value)
+            elif name.lower() in DOCS_LABELS:
+                mxml.set_upstream_doc(value)
+            elif name.lower() in HOME_REPO_LABELS:
+                if (remote_id := extract_remote_id(value)) is not None:
+                    mxml.add_upstream_remote_id(remote_id)
 
     @property
     def active(self) -> bool:
         return _HAS_PKGINFO_LIB and self.pkg_info.is_file()
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/pyproject.py` & `gentle_mxml-0.3.1/gentle/generators/python/pyproject.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,22 @@
 * Remote ID
 """
 
 import logging
 from pathlib import Path
 
 from gentle.generators import AbstractGenerator
-from gentle.metadata import Person, MetadataXML
+from gentle.generators.python import (
+    BUG_TRACKER_LABELS,
+    CHANGELOG_LABELS,
+    DOCS_LABELS,
+    HOME_REPO_LABELS
+)
+from gentle.metadata import MetadataXML
+from gentle.metadata.types import Person
 from gentle.metadata.utils import extract_remote_id
 
 try:
     try:
         import tomllib
     except ModuleNotFoundError:
         import tomli as tomllib  # type: ignore
@@ -53,21 +60,20 @@
             logger.info("Found upstream maintainer: %s", person)
             if not person.name:
                 continue
             mxml.add_upstream_maintainer(person)
 
         for name, value in project.get("urls").items():
             logger.info("Found %s: %s", name, value)
-            match name.lower():
-                case "bug tracker" | "bugtracker" | "bugs" | "issues":
-                    mxml.set_upstream_bugs_to(value)
-                case "changelog" | "changes":
-                    mxml.set_upstream_changelog(value)
-                case "doc" | "docs" | "documentation":
-                    mxml.set_upstream_doc(value)
-                case "source" | "repo" | "repository" | "home" | "homepage":
-                    if (remote_id := extract_remote_id(value)) is not None:
-                        mxml.add_upstream_remote_id(remote_id)
+            if name.lower() in BUG_TRACKER_LABELS:
+                mxml.set_upstream_bugs_to(value)
+            elif name.lower() in CHANGELOG_LABELS:
+                mxml.set_upstream_changelog(value)
+            elif name.lower() in DOCS_LABELS:
+                mxml.set_upstream_doc(value)
+            elif name.lower() in HOME_REPO_LABELS:
+                if (remote_id := extract_remote_id(value)) is not None:
+                    mxml.add_upstream_remote_id(remote_id)
 
     @property
     def active(self) -> bool:
         return _HAS_TOMLLIB and self.pyproject_toml.is_file()
```

### Comparing `gentle_mxml-0.3.0/gentle/generators/shards.py` & `gentle_mxml-0.3.1/gentle/generators/shards.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/gentle/metadata/utils.py` & `gentle_mxml-0.3.1/gentle/metadata/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in>
 # No warranty
 
 """ Utilities for metadata generators """
 
 import re
-from typing import Optional
 
 from gentle.metadata import Person, RemoteID
 
 author_re = re.compile(r"(?P<name>.+?)\s*<(?P<email>.+?@.+?)>")
 
 remote_ids = {
     "bitbucket":
@@ -59,30 +58,34 @@
     "sourcehut":
         re.compile(r"https?://sr.ht/(?P<v>\S+/\S+)"),
     "vim":
         re.compile(r"https?://vim.org/scripts/script.php?script_id=(?P<v>\d+)")
 }
 
 
-def extract_name_email(author: str) -> Optional[Person]:
+def extract_name_email(author: str) -> Person | None:
     """
+    Make a :class:`Person` object from a string.
+
     :param author: string in the ``name <email>`` format
 
     >>> extract_name_email("Foo Bar <foobar@example.com>")
     Person(name='Foo Bar', email='foobar@example.com')
     >>> extract_name_email("Foo Bar") is None
     True
     """
     if (match := author_re.match(author)) is None:
         return None
     return Person(match.group("name"), match.group("email"))
 
 
-def extract_remote_id(url: str) -> Optional[RemoteID]:
+def extract_remote_id(url: str) -> RemoteID | None:
     """
+    Make a :class:`RemoteID` object from a string.
+
     :param url: project's source repository
 
     >>> extract_remote_id("https://pypi.org/project/foo-bar")
     RemoteID(attr='pypi', value='foo-bar')
     >>> extract_remote_id("https://example.com") is None
     True
     """
```

### Comparing `gentle_mxml-0.3.0/pyproject.toml` & `gentle_mxml-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 ]
 
 [project.optional-dependencies]
 # PKG-INFO
 pkginfo = ["pkginfo"]
 # DOAP
 rdf = ["rdflib"]
-# Cargo.toml, pyproject.toml, ...
+# Cargo.toml, pyproject.toml
 toml = ["tomli; python_version <= '3.11'"]
-# shard.yml
+# package.yaml, shard.yml
 yaml = ["PyYAML"]
 
 docs = [
     "insipid-sphinx-theme",
     "sphinx",
     "sphinx-prompt"
 ]
@@ -45,22 +45,26 @@
     "xmldiff"
 ]
 
 [project.scripts]
 gentle = "gentle.__main__:main"
 
 [project.urls]
+Home = "https://gentle.sysrq.in"
 Source = "https://git.sysrq.in/gentle"
 Issues = "https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=gentle"
 
 [tool.flit.module]
 name = "gentle"
 
 [tool.flit.sdist]
-include = ["tests/"]
+include = [
+    "docs/",
+    "tests/"
+]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
 [tool.mypy]
 disallow_untyped_defs = true
 no_implicit_optional = true
```

### Comparing `gentle_mxml-0.3.0/tests/bower/aurelia/bower.json` & `gentle_mxml-0.3.1/tests/bower/aurelia/bower.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/bower/test_generator.py` & `gentle_mxml-0.3.1/tests/bower/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/cargo/lemmy/Cargo.toml` & `gentle_mxml-0.3.1/tests/cargo/lemmy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/cargo/orjson/Cargo.toml` & `gentle_mxml-0.3.1/tests/cargo/orjson/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/cargo/test_generator.py` & `gentle_mxml-0.3.1/tests/cargo/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/composer/composer/composer.json` & `gentle_mxml-0.3.1/tests/composer/composer/composer.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/composer/test_generator.py` & `gentle_mxml-0.3.1/tests/composer/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/doap/gnome-calls/calls.doap` & `gentle_mxml-0.3.1/tests/doap/gnome-calls/calls.doap`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/doap/test_generator.py` & `gentle_mxml-0.3.1/tests/doap/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/hpack/hpack/package.yaml` & `gentle_mxml-0.3.1/tests/hpack/hpack/package.yaml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/hpack/stack/package.yaml` & `gentle_mxml-0.3.1/tests/hpack/stack/package.yaml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/hpack/test_generator.py` & `gentle_mxml-0.3.1/tests/hpack/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/npm/mkdocs-material/package.json` & `gentle_mxml-0.3.1/tests/npm/mkdocs-material/package.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/npm/test_generator.py` & `gentle_mxml-0.3.1/tests/npm/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/PKG-INFO` & `gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/PKG-INFO`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/PKG-INFO` & `gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/PKG-INFO`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/pkg_info/test_generator.py` & `gentle_mxml-0.3.1/tests/pkg_info/test_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # No warranty
 
 from copy import deepcopy
 from pathlib import Path
 
 import pytest
 
-from gentle.generators.pkg_info import PkgInfoGenerator
+from gentle.generators.python.pkg_info import PkgInfoGenerator
 from gentle.metadata import MetadataXML
 
 from tests.utils import compare_mxml
 
 
 def test_pkg_none(mxml: MetadataXML):
     gen = PkgInfoGenerator(Path(__file__).parent / "pkg_none")
```

### Comparing `gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/pyproject.toml` & `gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/pyproject/pkgcraft/pyproject.toml` & `gentle_mxml-0.3.1/tests/pyproject/pkgcraft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/tests/pyproject/test_generator.py` & `gentle_mxml-0.3.1/tests/pyproject/test_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # No warranty
 
 from copy import deepcopy
 from pathlib import Path
 
 import pytest
 
-from gentle.generators.pyproject import PyprojectGenerator
+from gentle.generators.python.pyproject import PyprojectGenerator
 from gentle.metadata import MetadataXML
 
 from tests.utils import compare_mxml
 
 
 def test_pkg_none(mxml: MetadataXML):
     gen = PyprojectGenerator(Path(__file__).parent / "pkg_none")
```

### Comparing `gentle_mxml-0.3.0/tests/shards/test_generator.py` & `gentle_mxml-0.3.1/tests/shards/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.0/PKG-INFO` & `gentle_mxml-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentle-mxml
-Version: 0.3.0
+Version: 0.3.1
 Summary: Gentoo Metadata XML generator 
 Author-email: Anna <cyber@sysrq.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,15 @@
 Requires-Dist: sphinx-prompt ; extra == "docs"
 Requires-Dist: pkginfo ; extra == "pkginfo"
 Requires-Dist: rdflib ; extra == "rdf"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: xmldiff ; extra == "test"
 Requires-Dist: tomli ; extra == "toml" and ( python_version <= '3.11')
 Requires-Dist: PyYAML ; extra == "yaml"
+Project-URL: Home, https://gentle.sysrq.in
 Project-URL: Issues, https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=gentle
 Project-URL: Source, https://git.sysrq.in/gentle
 Provides-Extra: docs
 Provides-Extra: pkginfo
 Provides-Extra: rdf
 Provides-Extra: test
 Provides-Extra: toml
@@ -67,15 +68,14 @@
 
 Installing
 ----------
 
 ### Gentoo
 
 ```sh
-eselect repository enable guru
 emerge app-portage/gentle
 ```
 
 ### Other systems
 
 `pip install gentle-mxml --user`
 
@@ -90,28 +90,32 @@
 
 Contributing
 ------------
 
 Patches and pull requests are welcome. Please use either [git-send-email(1)][1]
 or [git-request-pull(1)][2], addressed to <cyber@sysrq.in>.
 
+If you prefer GitHub-style workflow, use the [mirror repo][gh] to send pull
+requests.
+
 Your commit message should conform to the following standard:
 
 ```
 file/changed: Concice and complete statement of the purpose
 
 This is the body of the commit message.  The line above is the
 summary.  The summary should be no more than 72 chars long.  The
 body can be more freely formatted, but make it look nice.  Make
 sure to reference any bug reports and other contributors.  Make
 sure the correct authorship appears.
 ```
 
 [1]: https://git-send-email.io/
 [2]: https://git-scm.com/docs/git-request-pull
+[gh]: http://github.com/cybertailor/gentle
 
 
 License
 -------
 
 WTFPL
```

