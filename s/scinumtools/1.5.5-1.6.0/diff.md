# Comparing `tmp/scinumtools-1.5.5.tar.gz` & `tmp/scinumtools-1.6.0.tar.gz`

## Comparing `scinumtools-1.5.5.tar` & `scinumtools-1.6.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.5/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.5.5/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.5.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/BaseUnitsClass.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/DimensionsClass.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/FractionClass.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/UnitClass.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/cached_data.npy
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/pyproject.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/requirements.txt
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_stats.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_struct.py
--rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_units.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.5.5/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.5.5/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.5.5/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.6.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/BaseUnitsClass.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/DimensionsClass.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/FractionClass.py
+-rw-r--r--   0        0        0    13271 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/UnitClass.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.6.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/cached_data.npy
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/requirements.txt
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/test_stats.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/test_struct.py
+-rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/test_units.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.6.0/tests/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.6.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.6.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.6.0/PKG-INFO
```

### Comparing `scinumtools-1.5.5/.github/workflows/python-publish.yml` & `scinumtools-1.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/data/CachingClass.py` & `scinumtools-1.6.0/src/scinumtools/data/CachingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/data/ImageClass.py` & `scinumtools-1.6.0/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.6.0/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.6.0/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.6.0/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.6.0/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.6.0/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.6.0/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.6.0/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/BaseUnitsClass.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/BaseUnitsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/DimensionsClass.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/DimensionsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/FractionClass.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/FractionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/QuantityClass.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from ...math.solver import ExpressionSolver, AtomBase, OperatorPar, OperatorMul, OperatorTruediv
 from .UnitList import *
 from .UnitConverters import *
 from .DimensionsClass import Dimensions
 from .BaseUnitsClass import BaseUnits
 from .FractionClass import Fraction
 
+HANDLED_FUNCTIONS = {}
+
 class Quantity:
     prefixes: dict            # list of prefixes 
     unitlist: dict            # list of units
     
     magnitude: float          # quantity magnitude
     dimensions: Dimensions    # quantity dimensions
     baseunits: BaseUnits      # base units
@@ -72,17 +74,17 @@
             self.baseunits = BaseUnits()
 
     def _add(self, left, right):
         if not isinstance(left, Quantity):
             left = Quantity(left)
         if not isinstance(right, Quantity):
             right = Quantity(right)
-        magnitude = left.magnitude + right.magnitude
         if not left.dimensions == right.dimensions:
             raise Exception('Dimension does not match:', left.dimensions, right.dimensions)
+        magnitude = left.magnitude + right.to(left.baseunits).magnitude 
         dimensions = left.dimensions
         baseunits = left.baseunits
         return Quantity(magnitude, dimensions, baseunits)
 
     def __add__(self, other):
         return self._add(self, other)
     
@@ -90,17 +92,17 @@
         return self._add(other, self)
 
     def _sub(self, left, right):
         if not isinstance(left, Quantity):
             left = Quantity(left)
         if not isinstance(right, Quantity):
             right = Quantity(right)
-        magnitude = left.magnitude - right.magnitude
         if not left.dimensions == right.dimensions:
             raise Exception('Dimension does not match:', left.dimensions, right.dimensions)
+        magnitude = left.magnitude - right.to(left.baseunits).magnitude
         dimensions = left.dimensions
         baseunits = left.baseunits
         return Quantity(magnitude, dimensions, baseunits)
 
     def __sub__(self, other):
         return self._sub(self, other)
 
@@ -183,43 +185,50 @@
             magnitude = f"{magnitude:.03e}"
         baseunits = self.baseunits.expression()
         if baseunits:
             return f"Quantity({magnitude:s} {baseunits})"
         else:
             return f"Quantity({magnitude:s})"
 
+    def __getitem__(self, key):
+        return Quantity(self.magnitude[key], self.dimensions, self.baseunits)
+        
     def __array__(self):
         return np.array(self.magnitude)
     
     def __array_prepare__(self, array, context=None):
         if context:
             if context[0] in [np.sin, np.cos, np.tan]:
-                array = np.array(context[1][0].to('rad'))
+                return np.array(context[1][0].to('rad'))
         return array
     
     def __array_wrap__(self, out_arr, context=None):
         if out_arr.ndim==0:
             out_arr = float(out_arr)
         dimensions = self.dimensions
         baseunits = self.baseunits
         if context:
-            if context[0]==np.sqrt:
-                dimensions /= 2
-                baseunits /= 2
-            elif context[0]==np.cbrt:
-                dimensions /= 3
-                baseunits /= 3
-            elif context[0]==np.power:
-                dimensions *= context[1][1]
-                baseunits *= context[1][1]
-            elif context[0] in [np.sin, np.cos, np.tan]:
-                dimensions = Dimensions()
-                baseunits = BaseUnits()
+            fn = context[0]
+            if fn==np.sqrt:
+                return Quantity(out_arr, dimensions/2, baseunits/2)
+            elif fn==np.cbrt:
+                return Quantity(out_arr, dimensions/3, baseunits/3)
+            elif fn==np.power:
+                return Quantity(out_arr, dimensions*context[1][1], baseunits*context[1][1])
+            elif fn in [np.sin, np.cos, np.tan]:
+                return Quantity(out_arr)
+            elif fn in [np.arcsin, np.arccos, np.arctan]:
+                return Quantity(out_arr, 'rad')
         return Quantity(out_arr, dimensions, baseunits)
     
+    def __array_function__(self, func, types, args, kwargs):
+        if func not in HANDLED_FUNCTIONS:
+            raise NotImplementedError()
+        return HANDLED_FUNCTIONS[func](*args, **kwargs)
+
     def _atom_parser(self, string=None):
         # parse number
         m = re.match(r'^[-]?([0-9.]+)(e([0-9+-]+)|)$', str(string))
         if m:
             magnitude = float(string)
             return Quantity(magnitude)
         # parse unit
@@ -270,19 +279,18 @@
             dimensions = [dim*exp for dim in dimensions]
             baseunits = {unitid: exp}            
         else:
             baseunits = {unitid: 1}
         return Quantity(magnitude, dimensions, baseunits)
     
     def value(self, expression=None):
-        if not expression:
-            expression = self.baseunits.expression()
         if expression:
-            unit = self/Quantity(1,expression)
-            return unit.magnitude
+            return self.to(expression).value()
+        elif expr:=self.baseunits.expression():
+            return (self/Quantity(1, expr)).magnitude
         else:
             return self.magnitude
 
     def units(self):
         return self.baseunits.expression()
 
     def to(self, units: Union[str,list,np.ndarray,Dimensions,dict,BaseUnits]):
@@ -297,7 +305,37 @@
                 raise Exception("Converting units with different dimensions:",
                                 unit1.dimensions, unit2.dimensions)
         with TemperatureConverter(unit1.baseunits.value(), unit2.baseunits.value()) as tc:
             if tc.convertable:
                 unit2.magnitude = unit1.magnitude/tc.convert(unit1.magnitude, unit2.magnitude)
         unit = unit1/unit2
         return Quantity(unit.magnitude, units)
+
+def implements(np_function):
+    def decorator(func):
+        HANDLED_FUNCTIONS[np_function] = func
+        return func
+    return decorator
+
+@implements(np.linspace)
+def linspace(a, b, c, **kwargs):
+    if isinstance(a,Quantity):
+        b = b.to(a.baseunits) if isinstance(b,Quantity) else Quantity(b, a.baseunits)
+    else:
+        a = a.to(b.baseunits) if isinstance(a,Quantity) else Quantity(a, b.baseunits)
+    return Quantity(np.linspace(a.magnitude, b.magnitude, c, **kwargs), a.baseunits)
+
+@implements(np.logspace)
+def logspace(a, b, c, **kwargs):
+    if isinstance(a,Quantity):
+        b = b.to(a.baseunits) if isinstance(b,Quantity) else Quantity(b, a.baseunits)
+    else:
+        a = a.to(b.baseunits) if isinstance(a,Quantity) else Quantity(a, b.baseunits)
+    return Quantity(np.logspace(a.magnitude, b.magnitude, c, **kwargs), a.baseunits)
+
+@implements(np.absolute)
+def absolute(a, **kwargs):
+    return Quantity(np.absolute(a.magnitude, a.baseunits))
+
+@implements(np.abs)
+def abs(a, **kwargs):
+    return Quantity(np.abs(a.magnitude, a.baseunits))
```

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/UnitClass.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/UnitClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.6.0/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.6.0/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.6.0/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.6.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/cached_data.npy` & `scinumtools-1.6.0/tests/cached_data.npy`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/pyproject.toml` & `scinumtools-1.6.0/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/test_data.py` & `scinumtools-1.6.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/test_math.py` & `scinumtools-1.6.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/test_stats.py` & `scinumtools-1.6.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/test_struct.py` & `scinumtools-1.6.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/test_units.py` & `scinumtools-1.6.0/tests/test_units.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from scinumtools.phys.units import *
 
 def test_quantity():
     
     assert str(Quantity(123e2))         == "Quantity(1.230e+04)"
     q = Quantity(123e2, 'km/s')
     assert str(q) == "Quantity(1.230e+04 km*s-1)"
-    assert str(q.value()) == "12300.0"
-    assert str(q.value('m/s')) == "12300000.0"
-    assert str(q.units()) == "km*s-1"
+    assert str(q.value())               == "12300.0"
+    assert str(q.value('m/s'))          == "12300000.0"
+    assert str(q.value({'m':1,'s':-1})) == "12300000.0"
+    assert str(q.units())               == "km*s-1"
     
     result = "Quantity(1.230e+04 m*s2:3)"
     assert str(Quantity(123e2, [1,0,(2,3),0,0,0,0,0] ))    == result
     assert str(Quantity(123e2, Dimensions(m=1, s=(2,3)) )) == result
 
     result = "Quantity(1.230e+04 J2*kg2:3)"
     assert str(Quantity(123e2, {'J': 2, 'kg':(2,3)} )) == result
@@ -132,14 +133,19 @@
             continue
         q = Quantity(1, unit['definition'])
         assert isclose(q.magnitude,  unit['magnitude'], rel_tol=1e-07)
         assert q.dimensions.value() == unit['dimensions']
         
 def test_scalar_arithmetics():
 
+    # addition and substtraction
+    assert str(Quantity(1.1, 'km')-Quantity(100, 'm')) == "Quantity(1.000e+00 km)"
+    assert str(Quantity(1.0, 'km')+Quantity(100, 'm')) == "Quantity(1.100e+00 km)"
+
+    # multiplication, division and power
     q = Quantity(123e2, [3,3,0,0,1,0,0,0])
     assert str(q) == "Quantity(1.230e+04 m3*g3*C)"    
     q /= Quantity(123, 'C')
     assert str(q) == "Quantity(1.000e+02 m3*g3)"
     q *= Quantity(2, 's2')
     assert str(q) == "Quantity(2.000e+02 m3*g3*s2)"
     q = Quantity(123, "kg3*cm-2*s")
@@ -201,26 +207,40 @@
     assert str(q) == "Quantity([2. 3. 4.] m)"
     q = q ** 10
     assert str(q) == "Quantity([1.024e+03 5.905e+04 1.049e+06] m10)"
 
     # Test unit conversion on arrays
     assert str(Quantity([1,2,3], 'm').to('km')) == "Quantity([0.001 0.002 0.003] km)"
 
+    # Array slicing
+    q = Quantity([1,2,3], 'm')
+    assert str(q[:2]) == "Quantity([1. 2.] m)"
+    
 def test_numpy():
     
     # Test numpy functions
     assert str(np.sqrt(Quantity(4, 'm2')))             == "Quantity(2.000e+00 m)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm2')))    == "Quantity([2. 3. 4.] m)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm3')))    == "Quantity([2. 3. 4.] m3:2)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm-3')))   == "Quantity([2. 3. 4.] m-3:2)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm2:3')))  == "Quantity([2. 3. 4.] m1:3)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm2:3*g3:5*s5')))  == "Quantity([2. 3. 4.] m1:3*g3:10*s5:2)"
     assert str(np.cbrt(Quantity([8, 27, 64], 'm3')))   == "Quantity([2. 3. 4.] m)"
     assert str(np.power(Quantity([2, 3, 4], 'm'),3))   == "Quantity([ 8. 27. 64.] m3)"
     assert str(np.sin(Quantity([45, 60], "deg")))      == "Quantity([0.707 0.866])"
+    assert str(np.cos(Quantity([45, 60], "deg")))      == "Quantity([0.707 0.5  ])"
+    assert str(np.tan(Quantity([45, 60], "deg")))      == "Quantity([1.    1.732])"
+    assert str(np.arcsin(Quantity([0.3, -0.7])))       == "Quantity([ 0.305 -0.775] rad)"
+    assert str(np.arccos(Quantity([0.3, -0.7])))       == "Quantity([1.266 2.346] rad)"
+    assert str(np.arctan(Quantity([0.3, -0.7])))       == "Quantity([ 0.291 -0.611] rad)"
+    assert str(np.linspace(0,Quantity(20,'m'),3))      == "Quantity([ 0. 10. 20.] m)"
+    assert str(np.linspace(Quantity(10,'m'),Quantity(0.03,'km'),3))  == "Quantity([10. 20. 30.] m)"
+    assert str(np.logspace(1,Quantity(3,'m'),3))       == "Quantity([  10.  100. 1000.] m)"
+    assert str(np.absolute(Quantity(-3,'m')))          == "Quantity(3.000e+00 m)"
+    assert str(np.abs(Quantity(-3,'m')))               == "Quantity(3.000e+00 m)"
     
 def test_operation_sides():
     
     p = Quantity([2,3,4], 'm')
     q = Quantity([5,6,7], 'm')
     assert p+q == q+p
     assert p-q == -(q-p)
```

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/data/ImageClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.6.0/tests/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.6.0/tests/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/tests/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.6.0/tests/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/.gitignore` & `scinumtools-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.5/pyproject.toml` & `scinumtools-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.5.5"
+version = "1.6.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.5.5/PKG-INFO` & `scinumtools-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.5.5
+Version: 1.6.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

