# Comparing `tmp/yambs-1.9.1.tar.gz` & `tmp/yambs-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.9.1.tar", last modified: Sat Jul  1 05:50:13 2023, max compression
+gzip compressed data, was "yambs-1.9.2.tar", last modified: Sat Jul  1 07:07:08 2023, max compression
```

## Comparing `yambs-1.9.1.tar` & `yambs-1.9.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.114201 yambs-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 05:47:55.000000 yambs-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-01 05:50:13.114201 yambs-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-07-01 05:47:55.000000 yambs-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 05:47:55.000000 yambs-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:50:13.114201 yambs-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 05:47:55.000000 yambs-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.102201 yambs-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-01 05:47:55.000000 yambs-1.9.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-01 05:47:55.000000 yambs-1.9.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.110201 yambs-1.9.1/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/targets_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.110201 yambs-1.9.1/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.110201 yambs-1.9.1/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.114201 yambs-1.9.1/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.114201 yambs-1.9.1/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/generate/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.114201 yambs-1.9.1/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.114201 yambs-1.9.1/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-01 05:47:55.000000 yambs-1.9.1/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:50:13.106202 yambs-1.9.1/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-01 05:50:13.000000 yambs-1.9.1/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-01 05:50:13.000000 yambs-1.9.1/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:50:13.000000 yambs-1.9.1/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 05:50:13.000000 yambs-1.9.1/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-01 05:50:13.000000 yambs-1.9.1/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 05:50:13.000000 yambs-1.9.1/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.455123 yambs-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 07:05:50.000000 yambs-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-01 07:07:08.451123 yambs-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-07-01 07:05:50.000000 yambs-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 07:05:50.000000 yambs-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:07:08.455123 yambs-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 07:05:50.000000 yambs-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.443123 yambs-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-01 07:05:50.000000 yambs-1.9.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-01 07:05:50.000000 yambs-1.9.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/targets_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.9.1/LICENSE` & `yambs-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/PKG-INFO` & `yambs-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=b699d78240c583717f3333f89773a15d
+    hash=9a21bcfc475707c132005e45f897b988
     =====================================
 -->
 
-# yambs ([1.9.1](https://pypi.org/project/yambs/))
+# yambs ([1.9.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.9.1/README.md` & `yambs-1.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=b699d78240c583717f3333f89773a15d
+    hash=9a21bcfc475707c132005e45f897b988
     =====================================
 -->
 
-# yambs ([1.9.1](https://pypi.org/project/yambs/))
+# yambs ([1.9.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.9.1/pyproject.toml` & `yambs-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.9.1"
+version = "1.9.2"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.9.1/setup.py` & `yambs-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/tests/test_entry.py` & `yambs-1.9.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/aggregation/__init__.py` & `yambs-1.9.2/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/app.py` & `yambs-1.9.2/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/commands/all.py` & `yambs-1.9.2/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/commands/common.py` & `yambs-1.9.2/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/commands/gen.py` & `yambs-1.9.2/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/commands/native.py` & `yambs-1.9.2/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/commands/uf2conv.py` & `yambs-1.9.2/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/config/__init__.py` & `yambs-1.9.2/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/config/board.py` & `yambs-1.9.2/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/config/common.py` & `yambs-1.9.2/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/includes/chips.yaml` & `yambs-1.9.2/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/includes/infineon.yaml` & `yambs-1.9.2/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/includes/microchip.yaml` & `yambs-1.9.2/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/schemas/Chip.yaml` & `yambs-1.9.2/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/schemas/Config.yaml` & `yambs-1.9.2/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/schemas/Native.yaml` & `yambs-1.9.2/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/templates/rules.ninja.j2` & `yambs-1.9.2/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/data/uf2families.json` & `yambs-1.9.2/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/entry.py` & `yambs-1.9.2/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/environment/__init__.py` & `yambs-1.9.2/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/environment/native.py` & `yambs-1.9.2/yambs/environment/native.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/__init__.py` & `yambs-1.9.2/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/architectures.py` & `yambs-1.9.2/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/boards.py` & `yambs-1.9.2/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/chips.py` & `yambs-1.9.2/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/common.py` & `yambs-1.9.2/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/ninja/__init__.py` & `yambs-1.9.2/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/ninja/format.py` & `yambs-1.9.2/yambs/generate/ninja/format.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,23 +26,30 @@
 
 def write_format_target(stream: TextIO, paths: Iterable[Path]) -> None:
     """
     Write rules and targets for running clang-format on first-party sources
     and headers.
     """
 
+    # Actually formats sources.
     stream.write("rule clang-format" + linesep)
     stream.write("  command = clang-format -i $in" + linesep + linesep)
 
+    # Just checks formatting.
+    stream.write("rule clang-format-check" + linesep)
+    stream.write("  command = clang-format -n --Werror $in" + linesep)
+
     paths = list(paths)
     if paths:
-        line = "build format: clang-format "
-        offset = " " * len(line)
-
-        stream.write(line)
-        stream.write(str(paths[0]))
-
-        for source in paths[1:]:
-            write_continuation(stream, offset)
-            stream.write(str(source))
+        for suffix in ["", "-check"]:
+            stream.write(linesep)
+            line = f"build format{suffix}: clang-format{suffix} "
+            offset = " " * len(line)
+
+            stream.write(line)
+            stream.write(str(paths[0]))
+
+            for source in paths[1:]:
+                write_continuation(stream, offset)
+                stream.write(str(source))
 
-        stream.write(linesep)
+            stream.write(linesep)
```

### Comparing `yambs-1.9.1/yambs/generate/toolchains.py` & `yambs-1.9.2/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/generate/variants.py` & `yambs-1.9.2/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/schemas.py` & `yambs-1.9.2/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/translation/__init__.py` & `yambs-1.9.2/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs/uf2/__init__.py` & `yambs-1.9.2/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.1/yambs.egg-info/PKG-INFO` & `yambs-1.9.2/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=b699d78240c583717f3333f89773a15d
+    hash=9a21bcfc475707c132005e45f897b988
     =====================================
 -->
 
-# yambs ([1.9.1](https://pypi.org/project/yambs/))
+# yambs ([1.9.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.9.1/yambs.egg-info/SOURCES.txt` & `yambs-1.9.2/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

