# Comparing `tmp/PySDM-2.8.tar.gz` & `tmp/PySDM-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySDM-2.8.tar", last modified: Wed May 18 16:46:56 2022, max compression
+gzip compressed data, was "PySDM-2.9.tar", last modified: Wed Jun  1 21:33:19 2022, max compression
```

## Comparing `PySDM-2.8.tar` & `PySDM-2.9.tar`

### file list

```diff
@@ -1,519 +1,517 @@
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.068786 PySDM-2.8/
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.988785 PySDM-2.8/.github/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       94 2021-09-14 23:03:26.000000 PySDM-2.8/.github/dependabot.yml
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.992786 PySDM-2.8/.github/workflows/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      283 2022-03-03 20:51:13.000000 PySDM-2.8/.github/workflows/cancel.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      587 2021-11-11 22:35:26.000000 PySDM-2.8/.github/workflows/codecov.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      519 2022-01-14 18:50:04.000000 PySDM-2.8/.github/workflows/joss.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1243 2022-05-18 16:46:20.000000 PySDM-2.8/.github/workflows/joss_paper.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      804 2022-04-24 06:49:33.000000 PySDM-2.8/.github/workflows/julia.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1170 2022-04-24 06:49:33.000000 PySDM-2.8/.github/workflows/main.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1155 2022-04-24 06:49:33.000000 PySDM-2.8/.github/workflows/matlab.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      820 2022-04-24 06:49:33.000000 PySDM-2.8/.github/workflows/pdoc.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      670 2022-04-24 06:49:33.000000 PySDM-2.8/.github/workflows/precommithooks.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      855 2022-05-03 21:31:02.000000 PySDM-2.8/.github/workflows/pylint.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      949 2022-04-24 06:49:33.000000 PySDM-2.8/.github/workflows/python.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      717 2021-09-18 19:34:20.000000 PySDM-2.8/.github/workflows/stale.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1870 2022-02-17 22:35:33.000000 PySDM-2.8/.gitignore
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      418 2022-05-03 21:31:02.000000 PySDM-2.8/.pre-commit-config.yaml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    35149 2021-09-14 23:03:26.000000 PySDM-2.8/LICENSE
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    37247 2022-05-18 16:46:56.068786 PySDM-2.8/PKG-INFO
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.992786 PySDM-2.8/PySDM/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1674 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.992786 PySDM-2.8/PySDM/attributes/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       55 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/attributes/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.992786 PySDM-2.8/PySDM/attributes/chemistry/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      272 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/chemistry/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1609 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/attributes/chemistry/acidity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      435 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/chemistry/concentration.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      437 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/chemistry/hydrogen_ion_concentration.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      409 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/chemistry/mole_amount.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.992786 PySDM-2.8/PySDM/attributes/ice/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      221 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/ice/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1127 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/ice/cooling_rate.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      321 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/ice/freezing_temperature.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      333 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/ice/immersed_surface_area.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.996785 PySDM-2.8/PySDM/attributes/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      395 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1048 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      402 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/base_attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      219 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/attributes/impl/cell_attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      843 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/derived_attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      559 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/dummy_attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      223 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/attributes/impl/extensive_attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      592 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/intensive_attribute.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3275 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/impl/mapper.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      390 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/attributes/impl/maximum_attribute.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.000786 PySDM-2.8/PySDM/attributes/numerics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      201 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/attributes/numerics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      260 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/numerics/cell_id.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      299 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/numerics/cell_origin.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      337 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/numerics/position_in_cell.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.000786 PySDM-2.8/PySDM/attributes/physics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      474 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      594 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/area.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1337 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/critical_supersaturation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1103 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/attributes/physics/critical_volume.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      516 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/dry_radius.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1526 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/dry_volume.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      291 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/heat.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      922 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/hygroscopicity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      345 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/multiplicities.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      542 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/radius.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      317 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/temperature.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      628 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/terminal_velocity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      366 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/attributes/physics/volume.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.000786 PySDM-2.8/PySDM/backends/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2195 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.004786 PySDM-2.8/PySDM/backends/impl_common/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       37 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_common/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      374 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_common/backend_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      519 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_common/freezing_attributes.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1764 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_common/index.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1722 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_common/indexed_storage.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      567 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_common/pair_indicator.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1135 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/backends/impl_common/pairwise_storage.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      240 2022-03-03 20:51:13.000000 PySDM-2.8/PySDM/backends/impl_common/random_common.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1875 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_common/storage_utils.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.004786 PySDM-2.8/PySDM/backends/impl_numba/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       36 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_numba/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4936 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/atomic_operations.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      504 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/conf.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.008786 PySDM-2.8/PySDM/backends/impl_numba/methods/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       42 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    15577 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/chemistry_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    23272 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/collisions_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    22442 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/condensation_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5935 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/displacement_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3591 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/freezing_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1161 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/index_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4935 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/moments_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4923 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/pair_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4257 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/physics_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2342 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/methods/terminal_velocity_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      513 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/random.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5497 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/storage.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1644 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/storage_impl.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.008786 PySDM-2.8/PySDM/backends/impl_numba/test_helpers/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       98 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_numba/test_helpers/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7008 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_numba/test_helpers/bdf.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6393 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/toms748.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      648 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_numba/warnings.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.008786 PySDM-2.8/PySDM/backends/impl_thrust_rtc/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       36 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1368 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/bisection.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1016 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/conf.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.012786 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       42 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    11303 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/collisions_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    14560 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/condensation_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4320 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/displacement_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2010 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/index_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6474 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/moments_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4515 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/pair_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4078 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/physics_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4170 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/terminal_velocity_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      768 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/thrust_rtc_backend_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      471 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/nice_thrust.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1213 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/random.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    14769 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/storage.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.012786 PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      145 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5486 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/cpp2python.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7553 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/fake_thrust_rtc.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      171 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/flag.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1947 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/numba.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2362 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/backends/thrust_rtc.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3883 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/builder.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.012786 PySDM-2.8/PySDM/dynamics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      572 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      283 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/ambient_thermodynamics.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4665 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/aqueous_chemistry.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.012786 PySDM-2.8/PySDM/dynamics/collisions/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      520 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.016786 PySDM-2.8/PySDM/dynamics/collisions/breakup_efficiencies/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       58 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_efficiencies/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      317 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_efficiencies/constEb.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.016786 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      182 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      719 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/always_n.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1488 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/exponential.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1570 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/feingold1988.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      900 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/gaussian.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      502 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/slams.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.016786 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      210 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      437 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/_gravitational.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      648 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/_parameterized.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      245 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/berry1967.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      293 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/constEc.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1559 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/schlottke2010.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      536 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/specified_eff.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    12164 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/collisions/collision.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.020786 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      480 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      296 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/constantK.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      414 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/electric.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      726 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/geometric.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1303 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/golovin.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      370 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/hydrodynamic.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.020786 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       55 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      483 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/impl/gravitational.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      972 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/impl/parameterized.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      445 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/linear.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      802 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/simple_geometric.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3823 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/condensation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5603 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/displacement.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      625 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/eulerian_advection.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2670 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/freezing.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.020786 PySDM-2.8/PySDM/dynamics/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       57 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/dynamics/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5015 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/impl/chemistry_utils.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1466 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/impl/random_generator_optimizer.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1059 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/dynamics/impl/random_generator_optimizer_nopair.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.020786 PySDM-2.8/PySDM/dynamics/terminal_velocity/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      189 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/dynamics/terminal_velocity/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5941 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/terminal_velocity/gunn_and_kinzer.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      990 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/dynamics/terminal_velocity/rogers_and_yau.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.020786 PySDM-2.8/PySDM/environments/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      207 2021-09-14 23:03:26.000000 PySDM-2.8/PySDM/environments/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      925 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/environments/box.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.024786 PySDM-2.8/PySDM/environments/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       68 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/environments/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2443 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/environments/impl/moist.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2513 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/environments/kinematic_1d.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3070 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/environments/kinematic_2d.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3938 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/environments/parcel.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.024786 PySDM-2.8/PySDM/exporters/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      167 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/exporters/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4189 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/exporters/netcdf_exporter.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5682 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/exporters/vtk_exporter.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     8758 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/formulae.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.024786 PySDM-2.8/PySDM/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       53 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      330 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/impl/arakawa_c.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1344 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/impl/mesh.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3319 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/impl/particle_attributes.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4516 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/impl/particle_attributes_factory.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      464 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/impl/wall_timer.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.024786 PySDM-2.8/PySDM/initialisation/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      220 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/initialisation/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.024786 PySDM-2.8/PySDM/initialisation/aerosol_composition/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      205 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/aerosol_composition/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4339 2022-05-18 16:46:20.000000 PySDM-2.8/PySDM/initialisation/aerosol_composition/dry_aerosol.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      776 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/discretise_multiplicities.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4297 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/initialisation/equilibrate_wet_radii.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.024786 PySDM-2.8/PySDM/initialisation/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      125 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/initialisation/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1138 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/impl/spectrum.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.028786 PySDM-2.8/PySDM/initialisation/sampling/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       42 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/initialisation/sampling/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      442 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/sampling/spatial_sampling.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3489 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/sampling/spectral_sampling.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2059 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/sampling/spectro_glacial_sampling.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.028786 PySDM-2.8/PySDM/initialisation/spectra/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      308 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      363 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/exponential.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      384 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/gamma.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      361 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/gaussian.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      924 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/lognormal.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1314 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/sum.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      562 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/initialisation/spectra/top_hat.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    14451 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/particulator.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.028786 PySDM-2.8/PySDM/physics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      648 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.032786 PySDM-2.8/PySDM/physics/condensation_coordinate/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      150 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/physics/condensation_coordinate/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      409 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/condensation_coordinate/volume.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      511 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/condensation_coordinate/volume_logarithm.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1040 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/constants.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4257 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/constants_defaults.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.032786 PySDM-2.8/PySDM/physics/diffusion_kinetics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      209 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/physics/diffusion_kinetics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1024 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/diffusion_kinetics/fuchs_sutugin.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      598 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/physics/diffusion_kinetics/lowe_et_al_2019.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      500 2022-01-14 18:50:04.000000 PySDM-2.8/PySDM/physics/diffusion_kinetics/neglect.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.032786 PySDM-2.8/PySDM/physics/diffusion_thermics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      226 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/diffusion_thermics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      435 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/physics/diffusion_thermics/lowe_et_al_2019.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      312 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/physics/diffusion_thermics/neglect.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      423 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/physics/diffusion_thermics/tracy_welch_porter.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      653 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/dimensional_analysis.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.032786 PySDM-2.8/PySDM/physics/drop_growth/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      107 2021-11-11 22:35:26.000000 PySDM-2.8/PySDM/physics/drop_growth/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      410 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/physics/drop_growth/maxwell_mason.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.032786 PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      201 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      741 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/bigg_1953.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1342 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/niemand_et_al_2012.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      225 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/null.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.036786 PySDM-2.8/PySDM/physics/heterogeneous_ice_nucleation_rate/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      136 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/heterogeneous_ice_nucleation_rate/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      407 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/heterogeneous_ice_nucleation_rate/abifm.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      266 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/heterogeneous_ice_nucleation_rate/constant.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      247 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/heterogeneous_ice_nucleation_rate/null.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.036786 PySDM-2.8/PySDM/physics/hydrostatics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       99 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/physics/hydrostatics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      850 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/physics/hydrostatics/default.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.036786 PySDM-2.8/PySDM/physics/hygroscopicity/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      209 2021-09-14 23:03:26.000000 PySDM-2.8/PySDM/physics/hygroscopicity/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      605 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/physics/hygroscopicity/kappa_koehler.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      711 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/physics/hygroscopicity/kappa_koehler_leading_terms.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.036786 PySDM-2.8/PySDM/physics/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      153 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1641 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/impl/fake_unit_registry.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      192 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/physics/impl/flag.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.036786 PySDM-2.8/PySDM/physics/latent_heat/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      184 2022-02-17 22:35:33.000000 PySDM-2.8/PySDM/physics/latent_heat/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      221 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/latent_heat/constant.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      342 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/latent_heat/kirchhoff.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      268 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/latent_heat/lowe2019.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.036786 PySDM-2.8/PySDM/physics/particle_advection/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      168 2021-09-14 23:03:26.000000 PySDM-2.8/PySDM/physics/particle_advection/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      218 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/particle_advection/explicit_in_space.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      277 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/particle_advection/implicit_in_space.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.040786 PySDM-2.8/PySDM/physics/saturation_vapour_pressure/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      279 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/saturation_vapour_pressure/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      559 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/saturation_vapour_pressure/august_roche_magnus.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1398 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/saturation_vapour_pressure/flatau_walko_cotton.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      925 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/saturation_vapour_pressure/lowe1977.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1188 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/saturation_vapour_pressure/murphy_koop_2005.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.040786 PySDM-2.8/PySDM/physics/state_variable_triplet/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       96 2021-09-14 23:03:26.000000 PySDM-2.8/PySDM/physics/state_variable_triplet/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1381 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/physics/state_variable_triplet/rhod_thd_qv.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.040786 PySDM-2.8/PySDM/physics/surface_tension/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      249 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/surface_tension/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1436 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/surface_tension/compressed_film_ovadnevaite.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3118 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/physics/surface_tension/compressed_film_ruehl.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      405 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/surface_tension/constant.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2186 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/surface_tension/szyszkowski_langmuir.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1850 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/physics/trivia.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.040786 PySDM-2.8/PySDM/physics/ventilation/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       70 2021-11-11 22:35:26.000000 PySDM-2.8/PySDM/physics/ventilation/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      143 2022-01-03 01:34:14.000000 PySDM-2.8/PySDM/physics/ventilation/neglect.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.040786 PySDM-2.8/PySDM/products/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      357 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.044786 PySDM-2.8/PySDM/products/ambient_thermodynamics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      476 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      287 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_dry_air_density.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      349 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_dry_air_potential_temperature.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      269 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_pressure.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      607 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_relative_humidity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      274 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_temperature.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      354 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_water_vapour_mixing_ratio.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.044786 PySDM-2.8/PySDM/products/aqueous_chemistry/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      353 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/aqueous_chemistry/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1530 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/aqueous_chemistry/acidity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2505 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/aqueous_chemistry/aqueous_mass_spectrum.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1166 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/aqueous_chemistry/aqueous_mole_fraction.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      859 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/aqueous_chemistry/gaseous_mole_fraction.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      800 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/aqueous_chemistry/total_dry_mass_mixing_ratio.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.044786 PySDM-2.8/PySDM/products/collision/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      380 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/collision/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1363 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/collision/collision_rates.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1254 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/collision/collision_timestep_mean.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      791 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/collision/collision_timestep_min.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.044786 PySDM-2.8/PySDM/products/condensation/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      345 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/condensation/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      890 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/condensation/activable_fraction.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1539 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/condensation/condensation_timestep.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1811 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/condensation/event_rates.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1110 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/condensation/peak_supersaturation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.044786 PySDM-2.8/PySDM/products/displacement/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      249 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/displacement/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1382 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/displacement/flow_velocity_component.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      954 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/displacement/max_courant_number.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1305 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/displacement/surface_precipitation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.048786 PySDM-2.8/PySDM/products/freezing/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      347 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/freezing/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      459 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/freezing/cooling_rate.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1551 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/freezing/freezable_specific_concentration.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1066 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/freezing/ice_water_content.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      743 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/freezing/total_unfrozen_immersed_surface_area.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.048786 PySDM-2.8/PySDM/products/housekeeping/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      334 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/housekeeping/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      642 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/housekeeping/dynamic_wall_time.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      652 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/housekeeping/parcel_displacement.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      518 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/housekeeping/super_droplet_count_per_gridbox.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      456 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/housekeeping/time.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1084 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/housekeeping/timers.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.048786 PySDM-2.8/PySDM/products/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      386 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      888 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/products/impl/moist_environment_product.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1474 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/impl/moment_product.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3411 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/impl/product.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      899 2021-12-14 15:28:00.000000 PySDM-2.8/PySDM/products/impl/rate_product.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1669 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/impl/spectrum_moment_product.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/PySDM/products/size_spectral/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      859 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/size_spectral/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1023 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/size_spectral/arbitrary_moment.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1473 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/effective_radius.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      480 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/mean_radius.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1421 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/size_spectral/number_size_spectrum.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1340 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/particle_concentration.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2617 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/particle_size_spectrum.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1708 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/size_spectral/particle_volume_versus_radius_logarithm_spectrum.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1357 2022-04-24 06:49:33.000000 PySDM-2.8/PySDM/products/size_spectral/radius_binned_number_averaged_terminal_velocity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      432 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/total_particle_concentration.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      596 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/total_particle_specific_concentration.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1300 2022-05-03 21:31:02.000000 PySDM-2.8/PySDM/products/size_spectral/water_mixing_ratio.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:55.992786 PySDM-2.8/PySDM.egg-info/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    37247 2022-05-18 16:46:55.000000 PySDM-2.8/PySDM.egg-info/PKG-INFO
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    19518 2022-05-18 16:46:55.000000 PySDM-2.8/PySDM.egg-info/SOURCES.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        1 2022-05-18 16:46:55.000000 PySDM-2.8/PySDM.egg-info/dependency_links.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       80 2022-05-18 16:46:55.000000 PySDM-2.8/PySDM.egg-info/requires.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        6 2022-05-18 16:46:55.000000 PySDM-2.8/PySDM.egg-info/top_level.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    36077 2022-05-03 21:31:02.000000 PySDM-2.8/README.md
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1020 2022-04-24 06:49:33.000000 PySDM-2.8/appveyor.yml
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/paper/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    19993 2022-05-18 16:46:20.000000 PySDM-2.8/paper/ARG_fig1.pdf
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    19572 2022-05-18 16:46:20.000000 PySDM-2.8/paper/Singer_fig1_kohler.pdf
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20126 2022-05-18 16:46:20.000000 PySDM-2.8/paper/deJong_fig1.pdf
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    13623 2022-05-18 16:46:20.000000 PySDM-2.8/paper/paper.bib
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    15147 2022-05-18 16:46:20.000000 PySDM-2.8/paper/paper.md
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20410 2022-05-18 16:46:20.000000 PySDM-2.8/paper/paperv1.md
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    23437 2022-01-14 18:50:04.000000 PySDM-2.8/paper/readme.pdf
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   135529 2022-01-14 18:50:04.000000 PySDM-2.8/paper/test.pdf
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       30 2022-04-24 06:49:33.000000 PySDM-2.8/pyproject.toml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       38 2022-05-18 16:46:56.068786 PySDM-2.8/setup.cfg
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2149 2022-05-18 16:46:32.000000 PySDM-2.8/setup.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      317 2022-05-18 16:46:20.000000 PySDM-2.8/test-time-requirements.txt
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/tests/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      235 2022-04-24 06:49:33.000000 PySDM-2.8/tests/backends_fixture.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/tests/devops_tests/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2502 2022-04-24 06:49:33.000000 PySDM-2.8/tests/devops_tests/test_todos_annotated.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/tests/smoke_tests/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/smoke_tests/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/tests/smoke_tests/abdul_razzak_ghan_2000/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/abdul_razzak_ghan_2000/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      459 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/abdul_razzak_ghan_2000/test_just_do_it.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4131 2022-05-03 21:31:02.000000 PySDM-2.8/tests/smoke_tests/abdul_razzak_ghan_2000/test_single_supersaturation_peak.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.052786 PySDM-2.8/tests/smoke_tests/alpert_and_knopf_2016/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/alpert_and_knopf_2016/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3153 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/alpert_and_knopf_2016/test_ak16_fig_1.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.056786 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2820 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_conservation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      724 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_displacement.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1238 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_event_rates.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2393 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_initialisation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1313 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_vs_bdf.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.056786 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      463 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/dummy_storage.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2556 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_adaptive_displacement.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      994 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_environment.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1445 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_export.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1787 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_freezing.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      688 2022-01-03 01:34:14.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_gui_settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3689 2022-05-03 21:31:02.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_initialisation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1735 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_spin_up.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.056786 PySDM-2.8/tests/smoke_tests/berry_1967/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/berry_1967/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3014 2022-05-03 21:31:02.000000 PySDM-2.8/tests/smoke_tests/berry_1967/test_coalescence.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.056786 PySDM-2.8/tests/smoke_tests/dejong_and_mackay_2022/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-02-17 22:35:33.000000 PySDM-2.8/tests/smoke_tests/dejong_and_mackay_2022/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1088 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/dejong_and_mackay_2022/test_collision.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.056786 PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3133 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_fig_1.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3581 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_ionic_strength.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1507 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_spectrum_at_t_0.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4093 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_table_3.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      558 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/constants.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3974 2022-05-18 16:46:20.000000 PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/test_fig_1.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2319 2022-05-03 21:31:02.000000 PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/test_fig_2.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    12390 2022-05-18 16:46:20.000000 PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/test_surface_tension_models.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/smoke_tests/niedermeier_et_al_2013/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-25 05:42:14.000000 PySDM-2.8/tests/smoke_tests/niedermeier_et_al_2013/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/smoke_tests/pyrcel/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-03-03 20:51:13.000000 PySDM-2.8/tests/smoke_tests/pyrcel/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2183 2022-05-03 21:31:02.000000 PySDM-2.8/tests/smoke_tests/pyrcel/test_parcel_example.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/smoke_tests/shima_et_al_2009/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/shima_et_al_2009/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2869 2022-05-03 21:31:02.000000 PySDM-2.8/tests/smoke_tests/shima_et_al_2009/test_coalescence.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2603 2022-05-18 16:46:20.000000 PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/test_few_steps.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2319 2022-05-18 16:46:20.000000 PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/test_initial_condition.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      952 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/test_settings.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/smoke_tests/yang_et_al_2018/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/smoke_tests/yang_et_al_2018/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      884 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/yang_et_al_2018/test_displacement.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2553 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/yang_et_al_2018/test_initialisation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1961 2022-04-24 06:49:33.000000 PySDM-2.8/tests/smoke_tests/yang_et_al_2018/test_just_do_it.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/unit_tests/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.060787 PySDM-2.8/tests/unit_tests/attributes/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/attributes/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5672 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/attributes/test_acidity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1452 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/attributes/test_area_radius.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1038 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/attributes/test_critical_supersaturation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1422 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/attributes/test_terminal_velocity.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/backends/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/backends/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/backends/storage/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/backends/storage/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1057 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/storage/test_index.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      500 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/storage/test_setitem.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5343 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/backends/test_collisions_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      708 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/test_ctor_defaults.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      456 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/test_fake_thrust.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4576 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/test_freezing_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1299 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/test_moments_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5882 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/test_oxidation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1104 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/backends/test_physics_methods.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1090 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/backends/test_toms748.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1856 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/dummy_environment.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      750 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dummy_particulator.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/dynamics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/dynamics/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/dynamics/collisions/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-02-17 22:35:33.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2437 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/__parametrisation__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1843 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/test_croupiers.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      659 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/test_defaults.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2760 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/test_kernels.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    16795 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/test_sdm_breakup.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1673 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/test_sdm_multi_cell.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    10110 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/dynamics/collisions/test_sdm_single_cell.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/dynamics/condensation/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3110 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/dynamics/condensation/test_diagnostics.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/dynamics/displacement/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/dynamics/displacement/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1623 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/displacement/displacement_settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5999 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/displacement/test_advection.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1677 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/displacement/test_courant_product.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1283 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/displacement/test_sedimentation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1232 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/dynamics/test_eulerian_advection.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.064787 PySDM-2.8/tests/unit_tests/impl/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.8/tests/unit_tests/impl/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4563 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/impl/test_moments.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    10696 2022-05-03 21:31:02.000000 PySDM-2.8/tests/unit_tests/impl/test_particle_attributes.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.068786 PySDM-2.8/tests/unit_tests/initialisation/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/initialisation/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1718 2022-05-18 16:46:20.000000 PySDM-2.8/tests/unit_tests/initialisation/test_aerosol_init.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2370 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/initialisation/test_r_wet_init.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1576 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/initialisation/test_spectral_discretisation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.068786 PySDM-2.8/tests/unit_tests/physics/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.8/tests/unit_tests/physics/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      945 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_accommodation_coefficients.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      959 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_constants.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1251 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_dimensional_analysis.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4773 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_formulae.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1684 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_freezing_temperature_spectra.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1179 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_latent_heat.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2566 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_saturation_vapour_pressure.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3039 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_spectra.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1899 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_spectra_top_hat.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1338 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/physics/test_thermal_conductivity.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:46:56.068786 PySDM-2.8/tests/unit_tests/products/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-02-24 19:37:37.000000 PySDM-2.8/tests/unit_tests/products/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1230 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/products/test_ambient_relative_humidity.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1694 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/products/test_cooling_rate.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3522 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/products/test_impl.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      898 2022-04-24 06:49:33.000000 PySDM-2.8/tests/unit_tests/test_particulator.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.196699 PySDM-2.9/
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.108700 PySDM-2.9/.github/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       94 2021-09-14 23:03:26.000000 PySDM-2.9/.github/dependabot.yml
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.112700 PySDM-2.9/.github/workflows/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      283 2022-03-03 20:51:13.000000 PySDM-2.9/.github/workflows/cancel.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      587 2021-11-11 22:35:26.000000 PySDM-2.9/.github/workflows/codecov.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      556 2022-06-01 21:32:52.000000 PySDM-2.9/.github/workflows/joss.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1243 2022-05-18 16:46:20.000000 PySDM-2.9/.github/workflows/joss_paper.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      804 2022-04-24 06:49:33.000000 PySDM-2.9/.github/workflows/julia.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1170 2022-04-24 06:49:33.000000 PySDM-2.9/.github/workflows/main.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1155 2022-04-24 06:49:33.000000 PySDM-2.9/.github/workflows/matlab.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      820 2022-04-24 06:49:33.000000 PySDM-2.9/.github/workflows/pdoc.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      670 2022-04-24 06:49:33.000000 PySDM-2.9/.github/workflows/precommithooks.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      876 2022-06-01 21:32:52.000000 PySDM-2.9/.github/workflows/pylint.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      949 2022-04-24 06:49:33.000000 PySDM-2.9/.github/workflows/python.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      717 2021-09-18 19:34:20.000000 PySDM-2.9/.github/workflows/stale.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1870 2022-02-17 22:35:33.000000 PySDM-2.9/.gitignore
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      418 2022-05-03 21:31:02.000000 PySDM-2.9/.pre-commit-config.yaml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    35149 2021-09-14 23:03:26.000000 PySDM-2.9/LICENSE
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    37247 2022-06-01 21:33:19.196699 PySDM-2.9/PKG-INFO
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.112700 PySDM-2.9/PySDM/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1674 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.112700 PySDM-2.9/PySDM/attributes/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       55 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/attributes/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.116700 PySDM-2.9/PySDM/attributes/chemistry/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      272 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/chemistry/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1609 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/attributes/chemistry/acidity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      435 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/chemistry/concentration.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      437 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/chemistry/hydrogen_ion_concentration.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      409 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/chemistry/mole_amount.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.116700 PySDM-2.9/PySDM/attributes/ice/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      221 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/ice/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1127 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/ice/cooling_rate.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      321 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/ice/freezing_temperature.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      333 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/ice/immersed_surface_area.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.120700 PySDM-2.9/PySDM/attributes/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      395 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1048 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      402 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/base_attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      219 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/attributes/impl/cell_attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      843 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/derived_attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      559 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/dummy_attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      223 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/attributes/impl/extensive_attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      592 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/intensive_attribute.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3275 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/impl/mapper.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      390 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/attributes/impl/maximum_attribute.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.120700 PySDM-2.9/PySDM/attributes/numerics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      201 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/attributes/numerics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      260 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/numerics/cell_id.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      299 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/numerics/cell_origin.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      337 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/numerics/position_in_cell.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.124699 PySDM-2.9/PySDM/attributes/physics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      474 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      594 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/area.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1337 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/critical_supersaturation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1103 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/attributes/physics/critical_volume.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      516 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/dry_radius.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1526 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/dry_volume.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      291 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/heat.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      922 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/hygroscopicity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      345 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/multiplicities.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      542 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/radius.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      317 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/temperature.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      628 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/terminal_velocity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      366 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/attributes/physics/volume.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.124699 PySDM-2.9/PySDM/backends/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2195 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.124699 PySDM-2.9/PySDM/backends/impl_common/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       37 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_common/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      374 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_common/backend_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      519 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_common/freezing_attributes.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1764 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_common/index.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1722 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_common/indexed_storage.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      567 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_common/pair_indicator.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1135 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/backends/impl_common/pairwise_storage.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      240 2022-03-03 20:51:13.000000 PySDM-2.9/PySDM/backends/impl_common/random_common.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1875 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_common/storage_utils.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.128699 PySDM-2.9/PySDM/backends/impl_numba/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       36 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_numba/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4936 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/atomic_operations.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      504 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/conf.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.128699 PySDM-2.9/PySDM/backends/impl_numba/methods/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       42 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    15577 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/chemistry_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    23272 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/collisions_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    22442 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/condensation_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5935 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/displacement_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3591 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/freezing_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1161 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/index_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4935 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/moments_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4923 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/pair_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4257 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/physics_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2342 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/methods/terminal_velocity_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      513 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/random.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5497 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/storage.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1644 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/storage_impl.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.128699 PySDM-2.9/PySDM/backends/impl_numba/test_helpers/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       98 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_numba/test_helpers/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7008 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_numba/test_helpers/bdf.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6393 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/toms748.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      648 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_numba/warnings.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.132699 PySDM-2.9/PySDM/backends/impl_thrust_rtc/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       36 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1368 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/bisection.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1016 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/conf.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.132699 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       42 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    11303 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/collisions_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    14560 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/condensation_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4320 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/displacement_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2010 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/index_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6474 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/moments_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4515 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/pair_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4078 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/physics_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4170 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/terminal_velocity_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      768 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/thrust_rtc_backend_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      471 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/nice_thrust.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1213 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/random.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    14769 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/storage.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.132699 PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      145 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5486 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/cpp2python.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7553 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/fake_thrust_rtc.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      171 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/flag.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1947 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/numba.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2362 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/backends/thrust_rtc.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3883 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/builder.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.136699 PySDM-2.9/PySDM/dynamics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      572 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      283 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/ambient_thermodynamics.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4665 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/aqueous_chemistry.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.136699 PySDM-2.9/PySDM/dynamics/collisions/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      520 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.136699 PySDM-2.9/PySDM/dynamics/collisions/breakup_efficiencies/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       58 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_efficiencies/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      317 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_efficiencies/constEb.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.136699 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      182 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      719 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/always_n.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1488 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/exponential.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1570 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/feingold1988.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      900 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/gaussian.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      502 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/slams.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.136699 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      210 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      437 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/_gravitational.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      648 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/_parameterized.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      245 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/berry1967.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      293 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/constEc.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1559 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/schlottke2010.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      536 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/specified_eff.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    12164 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/collisions/collision.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.140699 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      480 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      296 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/constantK.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      414 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/electric.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      726 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/geometric.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1303 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/golovin.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      370 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/hydrodynamic.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.140699 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       55 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      483 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/impl/gravitational.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      972 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/impl/parameterized.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      445 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/linear.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      802 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/simple_geometric.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4082 2022-06-01 21:32:52.000000 PySDM-2.9/PySDM/dynamics/condensation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5603 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/displacement.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      625 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/eulerian_advection.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2670 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/freezing.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.140699 PySDM-2.9/PySDM/dynamics/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       57 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/dynamics/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5015 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/impl/chemistry_utils.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1466 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/impl/random_generator_optimizer.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1059 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/dynamics/impl/random_generator_optimizer_nopair.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.140699 PySDM-2.9/PySDM/dynamics/terminal_velocity/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      189 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/dynamics/terminal_velocity/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5941 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/terminal_velocity/gunn_and_kinzer.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      990 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/dynamics/terminal_velocity/rogers_and_yau.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.144699 PySDM-2.9/PySDM/environments/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      207 2021-09-14 23:03:26.000000 PySDM-2.9/PySDM/environments/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      925 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/environments/box.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.144699 PySDM-2.9/PySDM/environments/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       68 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/environments/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2443 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/environments/impl/moist.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2513 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/environments/kinematic_1d.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3070 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/environments/kinematic_2d.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3938 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/environments/parcel.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.144699 PySDM-2.9/PySDM/exporters/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      167 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/exporters/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4189 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/exporters/netcdf_exporter.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5682 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/exporters/vtk_exporter.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     8758 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/formulae.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.144699 PySDM-2.9/PySDM/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       53 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      330 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/impl/arakawa_c.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1344 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/impl/mesh.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3319 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/impl/particle_attributes.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4516 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/impl/particle_attributes_factory.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      464 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/impl/wall_timer.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.144699 PySDM-2.9/PySDM/initialisation/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      220 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/initialisation/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.144699 PySDM-2.9/PySDM/initialisation/aerosol_composition/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      205 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/aerosol_composition/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4339 2022-05-18 16:46:20.000000 PySDM-2.9/PySDM/initialisation/aerosol_composition/dry_aerosol.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      776 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/discretise_multiplicities.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4297 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/initialisation/equilibrate_wet_radii.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.148699 PySDM-2.9/PySDM/initialisation/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      125 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/initialisation/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1138 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/impl/spectrum.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.148699 PySDM-2.9/PySDM/initialisation/sampling/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       42 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/initialisation/sampling/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      442 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/sampling/spatial_sampling.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3489 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/sampling/spectral_sampling.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2059 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/sampling/spectro_glacial_sampling.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.148699 PySDM-2.9/PySDM/initialisation/spectra/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      308 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      363 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/exponential.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      384 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/gamma.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      361 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/gaussian.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      924 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/lognormal.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1314 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/sum.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      562 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/initialisation/spectra/top_hat.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    14451 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/particulator.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.148699 PySDM-2.9/PySDM/physics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      648 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.152699 PySDM-2.9/PySDM/physics/condensation_coordinate/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      150 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/physics/condensation_coordinate/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      409 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/condensation_coordinate/volume.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      511 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/condensation_coordinate/volume_logarithm.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1040 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/constants.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4257 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/constants_defaults.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.152699 PySDM-2.9/PySDM/physics/diffusion_kinetics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      209 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/physics/diffusion_kinetics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1024 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/diffusion_kinetics/fuchs_sutugin.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      598 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/physics/diffusion_kinetics/lowe_et_al_2019.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      500 2022-01-14 18:50:04.000000 PySDM-2.9/PySDM/physics/diffusion_kinetics/neglect.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.152699 PySDM-2.9/PySDM/physics/diffusion_thermics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      226 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/diffusion_thermics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      435 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/physics/diffusion_thermics/lowe_et_al_2019.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      312 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/physics/diffusion_thermics/neglect.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      423 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/physics/diffusion_thermics/tracy_welch_porter.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      653 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/dimensional_analysis.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.152699 PySDM-2.9/PySDM/physics/drop_growth/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      107 2021-11-11 22:35:26.000000 PySDM-2.9/PySDM/physics/drop_growth/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      410 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/physics/drop_growth/maxwell_mason.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.152699 PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      201 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      741 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/bigg_1953.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1342 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/niemand_et_al_2012.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      225 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/null.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.156699 PySDM-2.9/PySDM/physics/heterogeneous_ice_nucleation_rate/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      136 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/heterogeneous_ice_nucleation_rate/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      407 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/heterogeneous_ice_nucleation_rate/abifm.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      266 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/heterogeneous_ice_nucleation_rate/constant.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      247 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/heterogeneous_ice_nucleation_rate/null.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.156699 PySDM-2.9/PySDM/physics/hydrostatics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       99 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/physics/hydrostatics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      850 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/physics/hydrostatics/default.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.156699 PySDM-2.9/PySDM/physics/hygroscopicity/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      209 2021-09-14 23:03:26.000000 PySDM-2.9/PySDM/physics/hygroscopicity/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      605 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/physics/hygroscopicity/kappa_koehler.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      711 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/physics/hygroscopicity/kappa_koehler_leading_terms.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.156699 PySDM-2.9/PySDM/physics/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      153 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1641 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/impl/fake_unit_registry.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      192 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/physics/impl/flag.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.156699 PySDM-2.9/PySDM/physics/latent_heat/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      184 2022-02-17 22:35:33.000000 PySDM-2.9/PySDM/physics/latent_heat/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      221 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/latent_heat/constant.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      342 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/latent_heat/kirchhoff.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      268 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/latent_heat/lowe2019.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.156699 PySDM-2.9/PySDM/physics/particle_advection/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      168 2021-09-14 23:03:26.000000 PySDM-2.9/PySDM/physics/particle_advection/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      218 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/particle_advection/explicit_in_space.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      277 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/particle_advection/implicit_in_space.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.160699 PySDM-2.9/PySDM/physics/saturation_vapour_pressure/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      279 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/saturation_vapour_pressure/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      559 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/saturation_vapour_pressure/august_roche_magnus.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1398 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/saturation_vapour_pressure/flatau_walko_cotton.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      925 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/saturation_vapour_pressure/lowe1977.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1188 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/saturation_vapour_pressure/murphy_koop_2005.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.160699 PySDM-2.9/PySDM/physics/state_variable_triplet/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       96 2021-09-14 23:03:26.000000 PySDM-2.9/PySDM/physics/state_variable_triplet/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1381 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/physics/state_variable_triplet/rhod_thd_qv.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.160699 PySDM-2.9/PySDM/physics/surface_tension/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      249 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/surface_tension/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1436 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/surface_tension/compressed_film_ovadnevaite.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3118 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/physics/surface_tension/compressed_film_ruehl.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      405 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/surface_tension/constant.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2186 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/surface_tension/szyszkowski_langmuir.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1850 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/physics/trivia.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.160699 PySDM-2.9/PySDM/physics/ventilation/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       70 2021-11-11 22:35:26.000000 PySDM-2.9/PySDM/physics/ventilation/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      143 2022-01-03 01:34:14.000000 PySDM-2.9/PySDM/physics/ventilation/neglect.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.160699 PySDM-2.9/PySDM/products/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      357 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.160699 PySDM-2.9/PySDM/products/ambient_thermodynamics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      476 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      287 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_dry_air_density.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      349 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_dry_air_potential_temperature.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      269 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_pressure.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      607 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_relative_humidity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      274 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_temperature.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      354 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_water_vapour_mixing_ratio.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.164699 PySDM-2.9/PySDM/products/aqueous_chemistry/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      353 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/aqueous_chemistry/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1530 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/aqueous_chemistry/acidity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2505 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/aqueous_chemistry/aqueous_mass_spectrum.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1166 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/aqueous_chemistry/aqueous_mole_fraction.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      859 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/aqueous_chemistry/gaseous_mole_fraction.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      800 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/aqueous_chemistry/total_dry_mass_mixing_ratio.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.164699 PySDM-2.9/PySDM/products/collision/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      380 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/collision/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1363 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/collision/collision_rates.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1254 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/collision/collision_timestep_mean.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      791 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/collision/collision_timestep_min.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.164699 PySDM-2.9/PySDM/products/condensation/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      345 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/condensation/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      890 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/condensation/activable_fraction.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1539 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/condensation/condensation_timestep.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1811 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/condensation/event_rates.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1110 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/condensation/peak_supersaturation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.164699 PySDM-2.9/PySDM/products/displacement/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      249 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/displacement/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1382 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/displacement/flow_velocity_component.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      954 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/displacement/max_courant_number.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1305 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/displacement/surface_precipitation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.168699 PySDM-2.9/PySDM/products/freezing/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      347 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/freezing/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      459 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/freezing/cooling_rate.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1551 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/freezing/freezable_specific_concentration.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1066 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/freezing/ice_water_content.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      743 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/freezing/total_unfrozen_immersed_surface_area.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.168699 PySDM-2.9/PySDM/products/housekeeping/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      334 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/housekeeping/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      642 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/housekeeping/dynamic_wall_time.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      652 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/housekeeping/parcel_displacement.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      518 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/housekeeping/super_droplet_count_per_gridbox.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      456 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/housekeeping/time.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1084 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/housekeeping/timers.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.168699 PySDM-2.9/PySDM/products/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      386 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      888 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/products/impl/moist_environment_product.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1474 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/impl/moment_product.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3411 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/impl/product.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      899 2021-12-14 15:28:00.000000 PySDM-2.9/PySDM/products/impl/rate_product.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1669 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/impl/spectrum_moment_product.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.172699 PySDM-2.9/PySDM/products/size_spectral/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      859 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/size_spectral/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1023 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/size_spectral/arbitrary_moment.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1473 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/effective_radius.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      480 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/mean_radius.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1421 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/size_spectral/number_size_spectrum.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1340 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/particle_concentration.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2617 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/particle_size_spectrum.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1708 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/size_spectral/particle_volume_versus_radius_logarithm_spectrum.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1357 2022-04-24 06:49:33.000000 PySDM-2.9/PySDM/products/size_spectral/radius_binned_number_averaged_terminal_velocity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      432 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/total_particle_concentration.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      596 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/total_particle_specific_concentration.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1300 2022-05-03 21:31:02.000000 PySDM-2.9/PySDM/products/size_spectral/water_mixing_ratio.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.112700 PySDM-2.9/PySDM.egg-info/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    37247 2022-06-01 21:33:18.000000 PySDM-2.9/PySDM.egg-info/PKG-INFO
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    19467 2022-06-01 21:33:19.000000 PySDM-2.9/PySDM.egg-info/SOURCES.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        1 2022-06-01 21:33:18.000000 PySDM-2.9/PySDM.egg-info/dependency_links.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       80 2022-06-01 21:33:18.000000 PySDM-2.9/PySDM.egg-info/requires.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        6 2022-06-01 21:33:18.000000 PySDM-2.9/PySDM.egg-info/top_level.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    36077 2022-05-03 21:31:02.000000 PySDM-2.9/README.md
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1020 2022-04-24 06:49:33.000000 PySDM-2.9/appveyor.yml
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.172699 PySDM-2.9/paper/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    19993 2022-05-18 16:46:20.000000 PySDM-2.9/paper/ARG_fig1.pdf
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    13151 2022-06-01 21:32:52.000000 PySDM-2.9/paper/paper.bib
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    15422 2022-06-01 21:32:52.000000 PySDM-2.9/paper/paper.md
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20410 2022-05-18 16:46:20.000000 PySDM-2.9/paper/paperv1.md
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    23437 2022-01-14 18:50:04.000000 PySDM-2.9/paper/readme.pdf
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   135529 2022-01-14 18:50:04.000000 PySDM-2.9/paper/test.pdf
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       30 2022-04-24 06:49:33.000000 PySDM-2.9/pyproject.toml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       38 2022-06-01 21:33:19.196699 PySDM-2.9/setup.cfg
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2149 2022-06-01 21:33:04.000000 PySDM-2.9/setup.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      310 2022-06-01 21:32:52.000000 PySDM-2.9/test-time-requirements.txt
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.176699 PySDM-2.9/tests/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      235 2022-04-24 06:49:33.000000 PySDM-2.9/tests/backends_fixture.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.176699 PySDM-2.9/tests/devops_tests/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2502 2022-04-24 06:49:33.000000 PySDM-2.9/tests/devops_tests/test_todos_annotated.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.176699 PySDM-2.9/tests/smoke_tests/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/smoke_tests/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.176699 PySDM-2.9/tests/smoke_tests/abdul_razzak_ghan_2000/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/abdul_razzak_ghan_2000/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      459 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/abdul_razzak_ghan_2000/test_just_do_it.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4131 2022-05-03 21:31:02.000000 PySDM-2.9/tests/smoke_tests/abdul_razzak_ghan_2000/test_single_supersaturation_peak.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.176699 PySDM-2.9/tests/smoke_tests/alpert_and_knopf_2016/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/alpert_and_knopf_2016/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3153 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/alpert_and_knopf_2016/test_ak16_fig_1.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.176699 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2820 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_conservation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      724 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_displacement.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1238 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_event_rates.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2393 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_initialisation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1313 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_vs_bdf.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      463 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/dummy_storage.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2556 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_adaptive_displacement.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      994 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_environment.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1445 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_export.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1787 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_freezing.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      688 2022-01-03 01:34:14.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_gui_settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3689 2022-05-03 21:31:02.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_initialisation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1735 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_spin_up.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/berry_1967/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/berry_1967/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3014 2022-05-03 21:31:02.000000 PySDM-2.9/tests/smoke_tests/berry_1967/test_coalescence.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/dejong_and_mackay_2022/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-02-17 22:35:33.000000 PySDM-2.9/tests/smoke_tests/dejong_and_mackay_2022/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1088 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/dejong_and_mackay_2022/test_collision.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3133 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_fig_1.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3581 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_ionic_strength.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1507 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_spectrum_at_t_0.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4093 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_table_3.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      558 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/constants.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3974 2022-05-18 16:46:20.000000 PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/test_fig_1.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2319 2022-05-03 21:31:02.000000 PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/test_fig_2.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    12390 2022-05-18 16:46:20.000000 PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/test_surface_tension_models.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/niedermeier_et_al_2013/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-25 05:42:14.000000 PySDM-2.9/tests/smoke_tests/niedermeier_et_al_2013/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/pyrcel/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-03-03 20:51:13.000000 PySDM-2.9/tests/smoke_tests/pyrcel/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2183 2022-05-03 21:31:02.000000 PySDM-2.9/tests/smoke_tests/pyrcel/test_parcel_example.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/shima_et_al_2009/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/shima_et_al_2009/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2869 2022-05-03 21:31:02.000000 PySDM-2.9/tests/smoke_tests/shima_et_al_2009/test_coalescence.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.180699 PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3933 2022-06-01 21:32:52.000000 PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/test_few_steps.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2319 2022-05-18 16:46:20.000000 PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/test_initial_condition.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      952 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/test_settings.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.184699 PySDM-2.9/tests/smoke_tests/yang_et_al_2018/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/smoke_tests/yang_et_al_2018/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      884 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/yang_et_al_2018/test_displacement.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2553 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/yang_et_al_2018/test_initialisation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1961 2022-04-24 06:49:33.000000 PySDM-2.9/tests/smoke_tests/yang_et_al_2018/test_just_do_it.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.184699 PySDM-2.9/tests/unit_tests/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.184699 PySDM-2.9/tests/unit_tests/attributes/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/attributes/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5672 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/attributes/test_acidity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1452 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/attributes/test_area_radius.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1038 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/attributes/test_critical_supersaturation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1422 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/attributes/test_terminal_velocity.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.188699 PySDM-2.9/tests/unit_tests/backends/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/backends/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.188699 PySDM-2.9/tests/unit_tests/backends/storage/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/backends/storage/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1057 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/storage/test_index.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      500 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/storage/test_setitem.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5343 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/backends/test_collisions_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      708 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/test_ctor_defaults.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      456 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/test_fake_thrust.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4576 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/test_freezing_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1299 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/test_moments_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5882 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/test_oxidation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1104 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/backends/test_physics_methods.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1090 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/backends/test_toms748.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1856 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/dummy_environment.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      750 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dummy_particulator.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.188699 PySDM-2.9/tests/unit_tests/dynamics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/dynamics/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.188699 PySDM-2.9/tests/unit_tests/dynamics/collisions/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-02-17 22:35:33.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2437 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/__parametrisation__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1843 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/test_croupiers.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      659 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/test_defaults.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2760 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/test_kernels.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    16795 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/test_sdm_breakup.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1673 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/test_sdm_multi_cell.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    10110 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/dynamics/collisions/test_sdm_single_cell.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.188699 PySDM-2.9/tests/unit_tests/dynamics/condensation/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3110 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/dynamics/condensation/test_diagnostics.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.192699 PySDM-2.9/tests/unit_tests/dynamics/displacement/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/dynamics/displacement/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1623 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/displacement/displacement_settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5999 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/displacement/test_advection.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1677 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/displacement/test_courant_product.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1283 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/displacement/test_sedimentation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1232 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/dynamics/test_eulerian_advection.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.192699 PySDM-2.9/tests/unit_tests/impl/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-11-11 22:35:26.000000 PySDM-2.9/tests/unit_tests/impl/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4563 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/impl/test_moments.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    10696 2022-05-03 21:31:02.000000 PySDM-2.9/tests/unit_tests/impl/test_particle_attributes.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.192699 PySDM-2.9/tests/unit_tests/initialisation/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/initialisation/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1718 2022-05-18 16:46:20.000000 PySDM-2.9/tests/unit_tests/initialisation/test_aerosol_init.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2370 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/initialisation/test_r_wet_init.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1576 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/initialisation/test_spectral_discretisation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.196699 PySDM-2.9/tests/unit_tests/physics/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2021-09-18 19:34:20.000000 PySDM-2.9/tests/unit_tests/physics/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      945 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_accommodation_coefficients.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      959 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_constants.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1251 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_dimensional_analysis.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4773 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_formulae.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1684 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_freezing_temperature_spectra.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1179 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_latent_heat.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2566 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_saturation_vapour_pressure.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3039 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_spectra.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1899 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_spectra_top_hat.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1338 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/physics/test_thermal_conductivity.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:33:19.196699 PySDM-2.9/tests/unit_tests/products/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        0 2022-02-24 19:37:37.000000 PySDM-2.9/tests/unit_tests/products/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1230 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/products/test_ambient_relative_humidity.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1694 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/products/test_cooling_rate.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3522 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/products/test_impl.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      898 2022-04-24 06:49:33.000000 PySDM-2.9/tests/unit_tests/test_particulator.py
```

### Comparing `PySDM-2.8/.github/workflows/codecov.yml` & `PySDM-2.9/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/joss_paper.yml` & `PySDM-2.9/.github/workflows/joss_paper.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/julia.yml` & `PySDM-2.9/.github/workflows/julia.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/main.yml` & `PySDM-2.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/matlab.yml` & `PySDM-2.9/.github/workflows/matlab.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/pdoc.yml` & `PySDM-2.9/.github/workflows/pdoc.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/precommithooks.yml` & `PySDM-2.9/.github/workflows/precommithooks.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/pylint.yml` & `PySDM-2.9/.github/workflows/pylint.yml`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
         python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install pylint
+        pip install pylint==2.13.9  # TODO #854
         python setup.py egg_info
         pip install -r *.egg-info/requires.txt
         pip install -r test-time-requirements.txt
     - name: Analysing the code with pylint
       run: |
         # TODO #682
         pylint --disable=fixme,invalid-name,missing-function-docstring,missing-class-docstring,too-many-locals,too-many-instance-attributes,too-few-public-methods,protected-access,too-many-statements,duplicate-code,C0330,C0326 $(git ls-files '*.py')
```

### Comparing `PySDM-2.8/.github/workflows/python.yml` & `PySDM-2.9/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.github/workflows/stale.yml` & `PySDM-2.9/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/.gitignore` & `PySDM-2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/LICENSE` & `PySDM-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PKG-INFO` & `PySDM-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySDM
-Version: 2.8
+Version: 2.9
 Summary: Pythonic particle-based (super-droplet) warm-rain/aqueous-chemistry cloud microphysics package with box, parcel & 1D/2D prescribed-flow examples in Python, Julia and Matlab
 Home-page: https://github.com/atmos-cloud-sim-uj/PySDM
 Author: https://github.com/atmos-cloud-sim-uj/PySDM/graphs/contributors
 Author-email: sylwester.arabas@uj.edu.pl
 License: GPL-3.0
 Keywords: physics-simulation,monte-carlo-simulation,gpu-computing,atmospheric-modelling,particle-system,numba,thrust,nvrtc,pint,atmospheric-physics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PySDM-2.8/PySDM/__init__.py` & `PySDM-2.9/PySDM/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/chemistry/acidity.py` & `PySDM-2.9/PySDM/attributes/chemistry/acidity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/ice/cooling_rate.py` & `PySDM-2.9/PySDM/attributes/ice/cooling_rate.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/impl/attribute.py` & `PySDM-2.9/PySDM/attributes/impl/attribute.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/impl/derived_attribute.py` & `PySDM-2.9/PySDM/attributes/impl/derived_attribute.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/impl/dummy_attribute.py` & `PySDM-2.9/PySDM/attributes/impl/dummy_attribute.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/impl/intensive_attribute.py` & `PySDM-2.9/PySDM/attributes/impl/intensive_attribute.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/impl/mapper.py` & `PySDM-2.9/PySDM/attributes/impl/mapper.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/area.py` & `PySDM-2.9/PySDM/attributes/physics/area.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/critical_supersaturation.py` & `PySDM-2.9/PySDM/attributes/physics/critical_supersaturation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/critical_volume.py` & `PySDM-2.9/PySDM/attributes/physics/critical_volume.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/dry_radius.py` & `PySDM-2.9/PySDM/attributes/physics/dry_radius.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/dry_volume.py` & `PySDM-2.9/PySDM/attributes/physics/dry_volume.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/hygroscopicity.py` & `PySDM-2.9/PySDM/attributes/physics/hygroscopicity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/radius.py` & `PySDM-2.9/PySDM/attributes/physics/radius.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/attributes/physics/terminal_velocity.py` & `PySDM-2.9/PySDM/attributes/physics/terminal_velocity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/__init__.py` & `PySDM-2.9/PySDM/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_common/freezing_attributes.py` & `PySDM-2.9/PySDM/backends/impl_common/freezing_attributes.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_common/index.py` & `PySDM-2.9/PySDM/backends/impl_common/index.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_common/indexed_storage.py` & `PySDM-2.9/PySDM/backends/impl_common/indexed_storage.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_common/pair_indicator.py` & `PySDM-2.9/PySDM/backends/impl_common/pair_indicator.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_common/pairwise_storage.py` & `PySDM-2.9/PySDM/backends/impl_common/pairwise_storage.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_common/storage_utils.py` & `PySDM-2.9/PySDM/backends/impl_common/storage_utils.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/atomic_operations.py` & `PySDM-2.9/PySDM/backends/impl_numba/atomic_operations.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/chemistry_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/chemistry_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/collisions_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/collisions_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/condensation_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/condensation_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/displacement_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/displacement_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/freezing_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/freezing_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/index_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/index_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/moments_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/moments_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/pair_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/pair_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/physics_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/physics_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/methods/terminal_velocity_methods.py` & `PySDM-2.9/PySDM/backends/impl_numba/methods/terminal_velocity_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/random.py` & `PySDM-2.9/PySDM/backends/impl_numba/random.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/storage.py` & `PySDM-2.9/PySDM/backends/impl_numba/storage.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/storage_impl.py` & `PySDM-2.9/PySDM/backends/impl_numba/storage_impl.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/test_helpers/bdf.py` & `PySDM-2.9/PySDM/backends/impl_numba/test_helpers/bdf.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/toms748.py` & `PySDM-2.9/PySDM/backends/impl_numba/toms748.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_numba/warnings.py` & `PySDM-2.9/PySDM/backends/impl_numba/warnings.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/bisection.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/bisection.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/conf.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/conf.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/collisions_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/collisions_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/condensation_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/condensation_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/displacement_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/displacement_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/index_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/index_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/moments_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/moments_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/pair_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/pair_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/physics_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/physics_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/terminal_velocity_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/terminal_velocity_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/methods/thrust_rtc_backend_methods.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/methods/thrust_rtc_backend_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/random.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/random.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/storage.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/storage.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/cpp2python.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/cpp2python.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/impl_thrust_rtc/test_helpers/fake_thrust_rtc.py` & `PySDM-2.9/PySDM/backends/impl_thrust_rtc/test_helpers/fake_thrust_rtc.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/numba.py` & `PySDM-2.9/PySDM/backends/numba.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/backends/thrust_rtc.py` & `PySDM-2.9/PySDM/backends/thrust_rtc.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/builder.py` & `PySDM-2.9/PySDM/builder.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/__init__.py` & `PySDM-2.9/PySDM/dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/aqueous_chemistry.py` & `PySDM-2.9/PySDM/dynamics/aqueous_chemistry.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/__init__.py` & `PySDM-2.9/PySDM/dynamics/collisions/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/always_n.py` & `PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/always_n.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/exponential.py` & `PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/exponential.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/feingold1988.py` & `PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/feingold1988.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/breakup_fragmentations/gaussian.py` & `PySDM-2.9/PySDM/dynamics/collisions/breakup_fragmentations/gaussian.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/_parameterized.py` & `PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/_parameterized.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/schlottke2010.py` & `PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/schlottke2010.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/coalescence_efficiencies/specified_eff.py` & `PySDM-2.9/PySDM/dynamics/collisions/coalescence_efficiencies/specified_eff.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/collision.py` & `PySDM-2.9/PySDM/dynamics/collisions/collision.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/geometric.py` & `PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/geometric.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/golovin.py` & `PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/golovin.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/impl/parameterized.py` & `PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/impl/parameterized.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/collisions/collision_kernels/simple_geometric.py` & `PySDM-2.9/PySDM/dynamics/collisions/collision_kernels/simple_geometric.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/condensation.py` & `PySDM-2.9/PySDM/dynamics/condensation.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         rtol_x=DEFAULTS.rtol_x,
         rtol_thd=DEFAULTS.rtol_thd,
         substeps: int = 1,
         adaptive: bool = True,
         dt_cond_range: tuple = DEFAULTS.cond_range,
         schedule: str = DEFAULTS.schedule,
         max_iters: int = 16,
+        update_thd: bool = True,
     ):
 
         self.particulator = None
         self.enable = True
 
         self.rtol_x = rtol_x
         self.rtol_thd = rtol_thd
@@ -43,14 +44,16 @@
         self.counters = {}
         self.dt_cond_range = dt_cond_range
         self.schedule = schedule
         self.max_iters = max_iters
 
         self.cell_order = None
 
+        self.update_thd = update_thd
+
     def register(self, builder):
         self.particulator = builder.particulator
 
         builder._set_condensation_parameters(
             dt_range=self.dt_cond_range,
             adaptive=self.adaptive,
             fuse=32,
@@ -96,14 +99,18 @@
                 counters=self.counters,
                 RH_max=self.rh_max,
                 success=self.success,
                 cell_order=self.cell_order,
             )
             if not self.success.all():
                 raise RuntimeError("Condensation failed")
+            if not self.update_thd:
+                self.particulator.environment.get_predicted("thd").ravel(
+                    self.particulator.environment.get_thd()
+                )
             # note: this makes order of dynamics matter
             #       (e.g., condensation after chemistry or before)
             self.particulator.update_TpRH()
 
             if self.adaptive:
                 self.counters["n_substeps"][:] = np.maximum(
                     self.counters["n_substeps"][:],
```

### Comparing `PySDM-2.8/PySDM/dynamics/displacement.py` & `PySDM-2.9/PySDM/dynamics/displacement.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/eulerian_advection.py` & `PySDM-2.9/PySDM/dynamics/eulerian_advection.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/freezing.py` & `PySDM-2.9/PySDM/dynamics/freezing.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/impl/chemistry_utils.py` & `PySDM-2.9/PySDM/dynamics/impl/chemistry_utils.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/impl/random_generator_optimizer.py` & `PySDM-2.9/PySDM/dynamics/impl/random_generator_optimizer.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/impl/random_generator_optimizer_nopair.py` & `PySDM-2.9/PySDM/dynamics/impl/random_generator_optimizer_nopair.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/terminal_velocity/gunn_and_kinzer.py` & `PySDM-2.9/PySDM/dynamics/terminal_velocity/gunn_and_kinzer.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/dynamics/terminal_velocity/rogers_and_yau.py` & `PySDM-2.9/PySDM/dynamics/terminal_velocity/rogers_and_yau.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/environments/box.py` & `PySDM-2.9/PySDM/environments/box.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/environments/impl/moist.py` & `PySDM-2.9/PySDM/environments/impl/moist.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/environments/kinematic_1d.py` & `PySDM-2.9/PySDM/environments/kinematic_1d.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/environments/kinematic_2d.py` & `PySDM-2.9/PySDM/environments/kinematic_2d.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/environments/parcel.py` & `PySDM-2.9/PySDM/environments/parcel.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/exporters/netcdf_exporter.py` & `PySDM-2.9/PySDM/exporters/netcdf_exporter.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/exporters/vtk_exporter.py` & `PySDM-2.9/PySDM/exporters/vtk_exporter.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/formulae.py` & `PySDM-2.9/PySDM/formulae.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/impl/mesh.py` & `PySDM-2.9/PySDM/impl/mesh.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/impl/particle_attributes.py` & `PySDM-2.9/PySDM/impl/particle_attributes.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/impl/particle_attributes_factory.py` & `PySDM-2.9/PySDM/impl/particle_attributes_factory.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/aerosol_composition/dry_aerosol.py` & `PySDM-2.9/PySDM/initialisation/aerosol_composition/dry_aerosol.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/discretise_multiplicities.py` & `PySDM-2.9/PySDM/initialisation/discretise_multiplicities.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/equilibrate_wet_radii.py` & `PySDM-2.9/PySDM/initialisation/equilibrate_wet_radii.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/impl/spectrum.py` & `PySDM-2.9/PySDM/initialisation/impl/spectrum.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/sampling/spectral_sampling.py` & `PySDM-2.9/PySDM/initialisation/sampling/spectral_sampling.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/sampling/spectro_glacial_sampling.py` & `PySDM-2.9/PySDM/initialisation/sampling/spectro_glacial_sampling.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/spectra/lognormal.py` & `PySDM-2.9/PySDM/initialisation/spectra/lognormal.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/spectra/sum.py` & `PySDM-2.9/PySDM/initialisation/spectra/sum.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/initialisation/spectra/top_hat.py` & `PySDM-2.9/PySDM/initialisation/spectra/top_hat.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/particulator.py` & `PySDM-2.9/PySDM/particulator.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/__init__.py` & `PySDM-2.9/PySDM/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/constants.py` & `PySDM-2.9/PySDM/physics/constants.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/constants_defaults.py` & `PySDM-2.9/PySDM/physics/constants_defaults.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/diffusion_kinetics/fuchs_sutugin.py` & `PySDM-2.9/PySDM/physics/diffusion_kinetics/fuchs_sutugin.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/diffusion_kinetics/lowe_et_al_2019.py` & `PySDM-2.9/PySDM/physics/diffusion_kinetics/lowe_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/dimensional_analysis.py` & `PySDM-2.9/PySDM/physics/dimensional_analysis.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/bigg_1953.py` & `PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/bigg_1953.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/freezing_temperature_spectrum/niemand_et_al_2012.py` & `PySDM-2.9/PySDM/physics/freezing_temperature_spectrum/niemand_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/hydrostatics/default.py` & `PySDM-2.9/PySDM/physics/hydrostatics/default.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/hygroscopicity/kappa_koehler.py` & `PySDM-2.9/PySDM/physics/hygroscopicity/kappa_koehler.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/hygroscopicity/kappa_koehler_leading_terms.py` & `PySDM-2.9/PySDM/physics/hygroscopicity/kappa_koehler_leading_terms.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/impl/fake_unit_registry.py` & `PySDM-2.9/PySDM/physics/impl/fake_unit_registry.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/saturation_vapour_pressure/august_roche_magnus.py` & `PySDM-2.9/PySDM/physics/saturation_vapour_pressure/august_roche_magnus.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/saturation_vapour_pressure/flatau_walko_cotton.py` & `PySDM-2.9/PySDM/physics/saturation_vapour_pressure/flatau_walko_cotton.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/saturation_vapour_pressure/lowe1977.py` & `PySDM-2.9/PySDM/physics/saturation_vapour_pressure/lowe1977.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/saturation_vapour_pressure/murphy_koop_2005.py` & `PySDM-2.9/PySDM/physics/saturation_vapour_pressure/murphy_koop_2005.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/state_variable_triplet/rhod_thd_qv.py` & `PySDM-2.9/PySDM/physics/state_variable_triplet/rhod_thd_qv.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/surface_tension/compressed_film_ovadnevaite.py` & `PySDM-2.9/PySDM/physics/surface_tension/compressed_film_ovadnevaite.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/surface_tension/compressed_film_ruehl.py` & `PySDM-2.9/PySDM/physics/surface_tension/compressed_film_ruehl.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/surface_tension/szyszkowski_langmuir.py` & `PySDM-2.9/PySDM/physics/surface_tension/szyszkowski_langmuir.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/physics/trivia.py` & `PySDM-2.9/PySDM/physics/trivia.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/ambient_thermodynamics/ambient_relative_humidity.py` & `PySDM-2.9/PySDM/products/ambient_thermodynamics/ambient_relative_humidity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/aqueous_chemistry/acidity.py` & `PySDM-2.9/PySDM/products/aqueous_chemistry/acidity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/aqueous_chemistry/aqueous_mass_spectrum.py` & `PySDM-2.9/PySDM/products/aqueous_chemistry/aqueous_mass_spectrum.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/aqueous_chemistry/aqueous_mole_fraction.py` & `PySDM-2.9/PySDM/products/aqueous_chemistry/aqueous_mole_fraction.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/aqueous_chemistry/gaseous_mole_fraction.py` & `PySDM-2.9/PySDM/products/aqueous_chemistry/gaseous_mole_fraction.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/aqueous_chemistry/total_dry_mass_mixing_ratio.py` & `PySDM-2.9/PySDM/products/aqueous_chemistry/total_dry_mass_mixing_ratio.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/collision/collision_rates.py` & `PySDM-2.9/PySDM/products/collision/collision_rates.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/collision/collision_timestep_mean.py` & `PySDM-2.9/PySDM/products/collision/collision_timestep_mean.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/collision/collision_timestep_min.py` & `PySDM-2.9/PySDM/products/collision/collision_timestep_min.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/condensation/activable_fraction.py` & `PySDM-2.9/PySDM/products/condensation/activable_fraction.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/condensation/condensation_timestep.py` & `PySDM-2.9/PySDM/products/condensation/condensation_timestep.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/condensation/event_rates.py` & `PySDM-2.9/PySDM/products/condensation/event_rates.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/condensation/peak_supersaturation.py` & `PySDM-2.9/PySDM/products/condensation/peak_supersaturation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/displacement/flow_velocity_component.py` & `PySDM-2.9/PySDM/products/displacement/flow_velocity_component.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/displacement/max_courant_number.py` & `PySDM-2.9/PySDM/products/displacement/max_courant_number.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/displacement/surface_precipitation.py` & `PySDM-2.9/PySDM/products/displacement/surface_precipitation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/freezing/freezable_specific_concentration.py` & `PySDM-2.9/PySDM/products/freezing/freezable_specific_concentration.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/freezing/ice_water_content.py` & `PySDM-2.9/PySDM/products/freezing/ice_water_content.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/freezing/total_unfrozen_immersed_surface_area.py` & `PySDM-2.9/PySDM/products/freezing/total_unfrozen_immersed_surface_area.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/housekeeping/dynamic_wall_time.py` & `PySDM-2.9/PySDM/products/housekeeping/dynamic_wall_time.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/housekeeping/parcel_displacement.py` & `PySDM-2.9/PySDM/products/housekeeping/parcel_displacement.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/housekeeping/super_droplet_count_per_gridbox.py` & `PySDM-2.9/PySDM/products/housekeeping/super_droplet_count_per_gridbox.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/housekeeping/timers.py` & `PySDM-2.9/PySDM/products/housekeeping/timers.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/impl/moist_environment_product.py` & `PySDM-2.9/PySDM/products/impl/moist_environment_product.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/impl/moment_product.py` & `PySDM-2.9/PySDM/products/impl/moment_product.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/impl/product.py` & `PySDM-2.9/PySDM/products/impl/product.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/impl/rate_product.py` & `PySDM-2.9/PySDM/products/impl/rate_product.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/impl/spectrum_moment_product.py` & `PySDM-2.9/PySDM/products/impl/spectrum_moment_product.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/__init__.py` & `PySDM-2.9/PySDM/products/size_spectral/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/arbitrary_moment.py` & `PySDM-2.9/PySDM/products/size_spectral/arbitrary_moment.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/effective_radius.py` & `PySDM-2.9/PySDM/products/size_spectral/effective_radius.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/number_size_spectrum.py` & `PySDM-2.9/PySDM/products/size_spectral/number_size_spectrum.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/particle_concentration.py` & `PySDM-2.9/PySDM/products/size_spectral/particle_concentration.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/particle_size_spectrum.py` & `PySDM-2.9/PySDM/products/size_spectral/particle_size_spectrum.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/particle_volume_versus_radius_logarithm_spectrum.py` & `PySDM-2.9/PySDM/products/size_spectral/particle_volume_versus_radius_logarithm_spectrum.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/radius_binned_number_averaged_terminal_velocity.py` & `PySDM-2.9/PySDM/products/size_spectral/radius_binned_number_averaged_terminal_velocity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/total_particle_specific_concentration.py` & `PySDM-2.9/PySDM/products/size_spectral/total_particle_specific_concentration.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM/products/size_spectral/water_mixing_ratio.py` & `PySDM-2.9/PySDM/products/size_spectral/water_mixing_ratio.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/PySDM.egg-info/PKG-INFO` & `PySDM-2.9/PySDM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySDM
-Version: 2.8
+Version: 2.9
 Summary: Pythonic particle-based (super-droplet) warm-rain/aqueous-chemistry cloud microphysics package with box, parcel & 1D/2D prescribed-flow examples in Python, Julia and Matlab
 Home-page: https://github.com/atmos-cloud-sim-uj/PySDM
 Author: https://github.com/atmos-cloud-sim-uj/PySDM/graphs/contributors
 Author-email: sylwester.arabas@uj.edu.pl
 License: GPL-3.0
 Keywords: physics-simulation,monte-carlo-simulation,gpu-computing,atmospheric-modelling,particle-system,numba,thrust,nvrtc,pint,atmospheric-physics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PySDM-2.8/PySDM.egg-info/SOURCES.txt` & `PySDM-2.9/PySDM.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -302,16 +302,14 @@
 PySDM/products/size_spectral/particle_size_spectrum.py
 PySDM/products/size_spectral/particle_volume_versus_radius_logarithm_spectrum.py
 PySDM/products/size_spectral/radius_binned_number_averaged_terminal_velocity.py
 PySDM/products/size_spectral/total_particle_concentration.py
 PySDM/products/size_spectral/total_particle_specific_concentration.py
 PySDM/products/size_spectral/water_mixing_ratio.py
 paper/ARG_fig1.pdf
-paper/Singer_fig1_kohler.pdf
-paper/deJong_fig1.pdf
 paper/paper.bib
 paper/paper.md
 paper/paperv1.md
 paper/readme.pdf
 paper/test.pdf
 tests/__init__.py
 tests/backends_fixture.py
```

### Comparing `PySDM-2.8/README.md` & `PySDM-2.9/README.md`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/appveyor.yml` & `PySDM-2.9/appveyor.yml`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/paper/ARG_fig1.pdf` & `PySDM-2.9/paper/ARG_fig1.pdf`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/paper/paper.bib` & `PySDM-2.9/paper/paper.bib`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 
 @article{Bartman_and_Arabas_2021,
   author = {Bartman, P. and Arabas, S.},
   title = {On the design of {M}onte-{C}arlo particle coagulation solver interface: a CPU/GPU Super-Droplet Method case study with PySDM},
   doi = {10.1007/978-3-030-77964-1_2},
   year = {2021},
   journal = {Lect. Notes Comput. Sci.},
-  volume = {12743}
 }
 
 @article{Shipway_and_Hill_2012,
   author = {Shipway, B.J. and Hill, A.A.},
   title = {Diagnosis of systematic differences between multiple parametrizations of warm rain microphysics using a kinematic framework},
   journal = {Q. J. Royal Meteorol. Soc.},
   year = {2012},
@@ -209,17 +208,17 @@
   year = {2022},
   doi = {10.21105/joss.03219}
 }
 
 @article{Bieli_et_al_2022,
   title = {An efficient Bayesian approach to learning droplet collision kernels: Proof of concept using "Cloudy", a new n-moment bulk microphysics scheme},
   author = {Bieli, M. and Dunbar, O.R.A. and De Jong, E.K. and Jaruga, A. and Schneider, T. and Bischoff, T.},
-  year = {2022},
   doi = {10.1002/essoar.10510248.1},
-  journal = {TODO}
+  journal = {J. Adv. Model. Earth Syst.},
+  year = {in review}
 }
 
 @article{Alpert_and_Knopf_2016,
   title = {Analysis of isothermal and cooling-rate-dependent immersion freezing by a unifying stochastic ice nucleation model},
   author = {Alpert, P.A. and Knopf, D.A.},
   year = {2016},
   doi = {10.5194/acp-16-2083-2016},
@@ -241,14 +240,15 @@
   journal = {J. Geophys. Res.},
   year = {2000}
 }
 
 @article{DeJong_et_al_2022,
   title = {Breakups are Complicated: Representing Collisional Droplet Breakup in the Superdroplet Method},
   author = {De Jong, E. and Mackay, J. B. and Jaruga, A.},
+  journal = {J. Adv. Model. Earth Syst.},
   year = {in preparation}
 }
 
 @article{Ovadnevaite_et_al_2017,
   author = {Ovadnevaite, J. and Zuend, A. and Laaksonen, A. and Sanchez, K.J. and Roberts, G. and Ceburnis, D. and Decesari, S. and Rinaldi, M. and Hodas, N. and Facchini, M.C. and Seinfeld, J.H. and O'Dowd, C.},
   doi = {10.1038/nature22806},
   year = {2017},
@@ -268,22 +268,14 @@
   title = {A stochastic, Lagrangian model of sinking biogenic aggregates in the ocean (SLAMS 1.0): model formulation, validation and sensitivity},
   author = {Jokulsdottir, T. and Archer, D.},
   year = {2016},
   journal = {Geosci. Model Dev.},
   doi = {10.5194/gmd-9-1455-2016}
 }
 
-@article{Howell_1949,
-  title = {The growth of cloud drops in uniformly cooled air},
-  author = {Howell, W.E.},
-  doi = {10.1175/1520-0469(1949)006%3C0134:TGOCDI%3E2.0.CO;2},
-  year = {1949},
-  journal = {J. Atmos. Sci.}
-}
-
 @article{Lange_1978,
   title = {ADPIC—A Three-Dimensional Particle-in-Cell Model for the Dispersal of Atmospheric Pollutants and its Comparison to Regional Tracer Studies},
   author = {Lange, R.},
   doi = {10.1175/1520-0450(1978)017<0320:ATDPIC>2.0.CO;2},
   year = {1978},
   journal = {J. Appl. Meteorol. Climatol.}
 }
@@ -312,18 +304,10 @@
   year = {2022}
 }
 
 @article{Knopf_and_Alpert_2013,
   title = {A water activity based model of heterogeneous ice nucleation kinetics for freezing of water and aqueous solution droplets},
   author = {Knopf, D.A. and Alpert, P.A.},
   journal = {Faraday Discuss.},
-  volume = {165},
   year = {2013},
   doi = {10.1039/c3fd00035d}
 }
-
-@article{Bartman_et_al_2022_adaptive,
-  title = {Adaptive time-stepping for particle-based cloud microphysics: super-droplet transport, collisions and condensational growth},
-  year = {2022},
-  author = {Bartman, P. and TODO and TODO and Arabas, S.},
-  note = {(n preparation}
-}
```

### Comparing `PySDM-2.8/paper/paper.md` & `PySDM-2.9/paper/paper.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,141 +1,142 @@
 ---
-title: 'New developments in PySDM and PySDM-examples v2: collisional breakup, immersion freezing, dry aerosol composition initialisation, and adaptive time-stepping'
-date: 17 May 2022
+title: 'New developments in PySDM and PySDM-examples v2: collisional breakup, immersion freezing, dry aerosol initialization, and adaptive time-stepping'
+date: 18 May 2022
 tags:
   - Python
   - physics-simulation 
   - monte-carlo-simulation 
-  - gpu-computing 
-  - atmospheric-modelling 
+  - atmospheric-modeling 
   - particle-system 
-  - numba 
-  - thrust 
-  - nvrtc 
-  - pint 
   - atmospheric-physics
-  - atmospheric-chemistry
 authors:
-  - name: Emily de Jong
+  - name: Emily K. de Jong
     affiliation: "1"
     orcid: 0000-0002-5310-4554
+  - name: Clare E. Singer
+    orcid: 0000-0002-1708-0997
+    affiliation: "2"
   - name: Sajjad Azimi
-    affiliation: "3"
+    affiliation: "2"
     orcid: 0000-0002-6329-7775
   - name: Piotr Bartman
     orcid: 0000-0003-0265-6428
-    affiliation: "2"
+    affiliation: "3"
   - name: Kacper Derlatka
-    affiliation: "2"
-  - name: Isabella Dula
     affiliation: "3"
+  - name: Isabella Dula
+    affiliation: "2"
   - name: Anna Jaruga
-    affiliation: "3"
+    affiliation: "2"
     orcid: 0000-0003-3194-6440
   - name: J. Ben Mackay
-    affiliation: "3"
+    affiliation: "2"
     orcid: 0000-0001-8677-3562
-  - name: Clare E. Singer
-    orcid: 0000-0002-1708-0997
-    affiliation: "3"
   - name: Ryan X. Ward
-    affiliation: "3"
+    affiliation: "2"
     orcid: 0000-0003-2317-3310
   - name: Sylwester Arabas
     orcid: 0000-0003-2361-0082
-    affiliation: "4,2"
+    affiliation: "4,3"
 affiliations:
  - name: Department of Mechanical and Civil Engineering, California Institute of Technology, Pasadena, CA, USA
    index: 1
- - name: Faculty of Mathematics and Computer Science, Jagiellonian University, Kraków, Poland
-   index: 2
  - name: Department of Environmental Science and Engineering, California Institute of Technology, Pasadena, CA, USA
+   index: 2
+ - name: Faculty of Mathematics and Computer Science, Jagiellonian University, Kraków, Poland
    index: 3
- - name: University of Illinois at Urbana-Champaign, Urbana, IL, USA
+ - name: Department of Atmospheric Sciences, University of Illinois at Urbana-Champaign, Urbana, IL, USA
    index: 4
 bibliography: paper.bib
 
 ---
 # Summary
 
 `PySDM` and the accompanying `PySDM-examples` packages are open-source modeling tools
-  for computational studies of atmospheric clouds, aerosols, and precipitation. The
-  project hinges on a particle-based modeling approach and Pythonic design and
-  implementation. 
+  for computational studies of atmospheric clouds, aerosols, and precipitation.
+The project hinges on the particle-based microphysics modeling approach and Pythonic code design.
 The eponymous `SDM` refers to the Super Droplet Method -- a 
   Monte-Carlo algorithm introduced in @Shima_et_al_2009 to represent the coagulation
-  of droplets in modelling frameworks such as Large-Eddy Simulations (LES) of atmospheric
+  of particles in modeling frameworks such as Large-Eddy Simulations (LES) of atmospheric
   flows. 
 Recent efforts have culminated
-  in a second release, which includes a variety of new processes for both liquid and ice-phase particles,
+  in the "v2" release line, which includes representation of a variety of new processes 
+  for both liquid and ice-phase particles,
   performance enhancements such as adaptive time-stepping, as well as a broadened suite of 
   examples which demonstrate, test, and motivate the use of the SDM for cloud modeling research.
 
 
 # Background and Statement of Need
+
 The key motivation behind development of `PySDM` has been to offer the community an approachable
   readily reusable software for users and developers who wish to contribute to the
   scientific progress of particle-based methods for simulating atmospheric clouds.
-To this end, we strive to maintain strict modularity of the PySDM building blocks, separation of
+To this end, we strive to maintain modularity of the `PySDM` building blocks, separation of
   functionality and examples, and extensive unit test coverage in the project.
 A user of the package can select top-level options such as the simulation
-  environment, particle processes, and output attributes without a detailed understanding
-  of the CPU and GPU implementations at the superparticle level.
+  environment, particle processes, and output attributes without a detailed grasp
+  of the CPU and GPU backend code.
 
-`PySDM` v1 featured representation of the following 
+`PySDM` "v1" featured representation of the following 
   processes: condensational growth/evaporation, collisional growth,
-  aqueous sulphur chemistry, as well as coupling of particle transport
-  and vapour/heat budget with grid-discretised fluid flow.
-This paper outlines these subsequent developments in the "v2" releases of `PySDM`
-  including three new processes (collisional breakup, immersion freezing, and surface-partitioning of organic aerosol components), 
-  initialisation framework for aerosol size and composition,
-  enhanced support for adaptive timestepping, and additional illustrative examples.
-
-In v2 of the companion `PySDM-examples` package, we continue to expand and maintain 
-  a set of examples demonstrating project features 
-  through reproduction of results from literature.
-The examples package has a fourfold role in the project.
-First, it serves to guide users and developers through the package features.
+  aqueous sulfur chemistry, and coupling of particle transport
+  and vapor/heat budget with grid-discretized fluid flow.
+This paper outlines subsequent developments in the "v2" releases of `PySDM`
+  including representation of three new processes (collisional breakup, immersion freezing, 
+  and surface-partitioning of organic aerosol components), 
+  initialization framework for aerosol size and composition,
+  enhanced support for adaptive time-stepping, and additional illustrative examples.
+
+In the companion `PySDM-examples` package, we continue to expand and maintain 
+  a set of examples demonstrating project features through automated reproduction of results from literature.
+The examples package serves multiple roles in the project.
+First, it guides users and developers through the package features.
 Second, `PySDM-examples` has been used as educational material, offering
   interactive Jupyter notebooks suitable for hands-on demonstrations of basic cloud-physics
   simulations.
 Third, inclusion of simulation scripts/notebooks pertaining to
-  new research papers is intended to streamline assessment of the
-  results by reviewers. Running simulations described in a paper can be done independently on a cloud-computing platform such as Google Colab.
-Finally, we require new examples include a set of "smoke tests" in `PySDM`,
+  new research papers can streamline assessment of the
+  results by reviewers.
+Running simulations described in a paper can be done independently on a cloud-computing platform 
+  such as Google Colab or mybinder.org.
+Finally, we require new examples introduced into `PySDM-examples` to be accompanied by 
+  a set of "smoke tests" in `PySDM`,
   which assert results against reference data to ensure that published results remain 
-  reproducible with future developments.
-
+  reproducible with future developments of `PySDM`.
 
 
 # Summary of new features and examples in v2
 
 For an example of running basic zero-dimensional
-  simulations with `PySDM`, we refer to the project README.md file and the
-  preceeding @Bartman_et_al_2022_JOSS JOSS paper.
-The following code snippets demonstrating new elements of `PySDM` API 
-  can be added or substituted into the v1 API description to run 
-  simulation using the new features.
+  simulations with `PySDM`, we refer to the project `README.md` file and @Bartman_et_al_2022_JOSS.
+The key building blocks of the `PySDM` API and class hierarchy are: "attributes", "backends", "dynamics",
+  "environments", "products" and physics "formulae".
+The following code snippets demonstrate new elements of `PySDM` API which
+  can be added or substituted into the "v1" API description to run 
+  simulations using the new features.
+Execution of code snippets from both the present "v2" and the previous "v1" papers
+  is included in the `PySDM` continuous integration workflow.
 
 ## Collisional Breakup
+
 The collisional breakup process represents the splitting of two colliding superdroplets
   into multiple fragments.
-It can be specified as an individual dynamic, as for coalescence in v1, or as a unified
-  `collision` dynamic, in which the probability of breakup versus coalescence is sampled.
+It can be specified as an individual `Breakup` "dynamic" or used within a unified
+  `Collision` "dynamic", in which the probability of breakup versus coalescence is sampled.
 The additional `PySDM` components used in the example below can be imported via:
 ```python
 from PySDM.dynamics.collisions import Collision
 from PySDM.dynamics.collisions.collision_kernels import Golovin
 from PySDM.dynamics.collisions.coalescence_efficiencies import ConstEc
 from PySDM.dynamics.collisions.breakup_efficiencies import ConstEb
 from PySDM.dynamics.collisions.breakup_fragmentations import ExponFrag
 ```
 The rate of superdroplet collisions are specified by a collision kernel, and the
-  breakup process requires two additional `dynamics` specifications: `coalescence_efficiencies`
-  (probability of coalescence occuring), `breakup_efficiencies` (probability of breakup occuring
+  breakup process requires three additional specifications: `coalescence_efficiencies`
+  (probability of coalescence occurring), `breakup_efficiencies` (probability of breakup occurring
   if not coalescence), and `breakup_fragmentations` (the number
   of fragments formed in the case of a breakup event). 
 
 ```python
 from PySDM import Builder
 from PySDM.backends import CPU
 from PySDM.environments import Box
@@ -147,49 +148,51 @@
   collision_kernel=Golovin(b=1.5e3 / si.s),
   coalescence_efficiency=ConstEc(Ec=0.9),
   breakup_efficiency=ConstEb(Eb=1.0),
   fragmentation_function=ExponFrag(scale=100*si.um**3)
 ))
 ```
 
-In `PySDM-examples`, we reproduce results from two forthcoming publications.
-In @Bieli_et_al_2022 (in review), `PySDM` results from collisional coalescence and breakup 
-  were used as a calibration tool 
-  for learning microphysics rate parameters.
-In @DeJong_et_al_2022, the physics and algorithm for superdroplet breakup are described,
-  and results demonstrating the impact of breakup on cloud properties in a box and 1D
-  environment (based on @Shipway_and_Hill_2012) are reproduced.
+In `PySDM-examples`, we introduced a set of notebooks reproducing figures from two forthcoming publications.
+In @Bieli_et_al_2022, `PySDM` results from collisional coalescence and breakup 
+  were used as a calibration tool for learning microphysical rate parameters.
+In @DeJong_et_al_2022, the physics of and algorithm for superdroplet breakup are described,
+  and the impact of breakup on cloud properties is demonstrated with box and single-column
+  simulations (the latter based on @Shipway_and_Hill_2012).
 
 ## Immersion Freezing
+
 This release of `PySDM` introduces representation of immersion freezing, 
   i.e. freezing contingent on the presence of insoluble ice nuclei immersed 
   in supercooled water droplets.
 There are two alternative models implemented: the singular approach presented in 
   @Shima_et_al_2020, and the time-dependent approach of @Alpert_and_Knopf_2016.
 For the time-dependent model, the water Activity Based Immersion Freezing Model (ABIFM)
   of @Knopf_and_Alpert_2013 is used.
-The dynamic is introduced by specifying whether a singular model is used, and additional particle
-  attributes must be initialised accordingly.
+The `Freezing` "dynamic" is introduced by specifying whether a singular model is used, 
+  and additional particle attributes (either freezing temperature or immersed surface area)
+  must be initialized accordingly.
 ```python
 from PySDM.dynamics import Freezing
 builder.add_dynamic(Freezing(singular=False))
 ```
 
 For validation of the the newly introduced immersion freezing models, a set of
   notebooks reproducing box-model simulations from @Alpert_and_Knopf_2016 was introduced
-  to the `PySDM-examples` package using the kinematic prescribed-flow environment 
-  introduced in `PySDM` v1.
-A comparison of the time-dependent and singular models using this setup is the focus of @Arabas_et_al_2022.
-
-## Initialisation of multi-component internally or externally mixed aerosols 
-The new aerosol initialisation framework allows flexible specification of multi-modal, multi-component
-  aerosol with arbitrary composition.
-The `DryAerosolMixture` class takes a list of compounds and dictionaries specifying their molar masses,
+  to the `PySDM-examples` package.
+A comparison of the time-dependent and singular models using 
+  a two-dimensional kinematic prescribed-flow framework was the focus of @Arabas_et_al_2022.
+
+## Initialization of multi-component internally or externally mixed aerosol
+
+The new aerosol initialization framework introduced in `PySDM` "v2" allows flexible specification 
+  of multi-modal, multi-component aerosol.
+The `DryAerosolMixture` class takes a tuple of compounds and dictionaries specifying their molar masses,
   densities, solubilities, and ionic dissociation numbers.
-The user must then specify the aerosol `modes` which are comprised of a `kappa` hygroscopicity value, 
+The user specifies the aerosol `modes` which are comprised of a `kappa` hygroscopicity value, 
   calculated from the molecular components and their associated `mass_fractions`,
   and a dry aerosol size `spectrum`.
 For example, a single-mode aerosol class (`SimpleAerosol`) can be defined as follows.
 ```python
 from PySDM.initialisation import spectra
 from PySDM.initialisation.aerosol_composition import DryAerosolMixture
 class SimpleAerosol(DryAerosolMixture):
@@ -204,84 +207,90 @@
             ionic_dissociation_phi={"(NH4)2SO4": 3, "NaCl": 2},
         )
         self.modes = (
             {
                 "kappa": self.kappa(
                   mass_fractions={"(NH4)2SO4": 0.7, "NaCl": 0.3}),
                 "spectrum": spectra.Lognormal(
-                    norm_factor=100.0 / si.cm**3,
-                    m_mode=50.0 * si.nm, s_geom=2.0
+                    norm_factor=100 / si.cm**3,
+                    m_mode=50 * si.nm, s_geom=2
                 ),
             },
         )
 ```
-The `aerosol` object can be used during initialisation to calculate the total number of 
+An aerosol object (instance of `DryAerosolMixture` subclass) is used during initialization to calculate the total number of 
   superdroplets given a prescribed number per mode, sample the size spectrum from the aerosol 
-  `spectrum` property, and initialise the `kappa times dry volume` attribute using the `aerosol` 
+  `spectrum` property, and initialize the `kappa times dry volume` attribute using the 
   hygroscopicity property `kappa`.
 The choice of `kappa times dry volume` as an extensive attribute ensures that, upon coalescence,
   the hygroscopicity of a resultant super-particle is the volume-weighted average of the hygroscopicity 
   of the coalescing super-particles.
-This new aerosol initialisation framework is used in the new example that reproduces results from 
-  @Abdul_Razzak_and_Ghan_2000, comparing these SDM results against the original bin implementation and a new 
-  cloud microphysics method, as shown in \autoref{fig:ARG}).
+The new aerosol initialization framework is used in several examples in `PySDM-examples` including a new 
+  example that reproduces results from @Abdul_Razzak_and_Ghan_2000, comparing `PySDM` 
+  simulations against data retrieved from the
+  publication as shown in \autoref{fig:ARG}).
 
-![Activated aerosol fraction in Mode 1 as a function of aerosol number concentration in Mode 2, reproducing results from @Abdul_Razzak_and_Ghan_2000. The figure shows the results from `PySDM` in color with two definitions of activated fraction based on the critical supersaturation threshold (Scrit) or the critical volume threshold (Vcrit) compared against the parameterization developed in @Abdul_Razzak_and_Ghan_2000, as implemented in their paper (solid line) and as implemented in a new Julia model (CloudMicrophysics.jl, dashed line), as well as the results from a bin scheme employed in @Abdul_Razzak_and_Ghan_2000 (black dots).](ARG_fig1.pdf){#fig:ARG width="100%"}
+![Activated aerosol fraction in Mode 1 as a function of aerosol number concentration in Mode 2, reproducing results from @Abdul_Razzak_and_Ghan_2000. The figure shows the results from `PySDM` in color with two definitions of activated fraction based on the critical supersaturation threshold (Scrit) or the critical volume threshold (Vcrit). For comparison, we include the parameterization developed in @Abdul_Razzak_and_Ghan_2000 as formulated in their paper (solid line) and as implemented in a new Julia model (`CloudMicrophysics.jl`, dashed line), as well as the results from simulations reported in @Abdul_Razzak_and_Ghan_2000 (black dots).](ARG_fig1.pdf){#fig:ARG width="100%"}
 
 ## Surface-partitioning of organics to modify surface tension of droplets
-`PySDM` v2 includes a new example demonstrating three new models for droplet surface tension.
-The four surface tension options included in `PySDM`, which define the droplet surface tension as a function of dry aerosol composition and wet radius, are `'Constant'`, `'CompressedFilmOvadnevaite'` (@Ovadnevaite_et_al_2017), `'CompressedFilmRuehl'` (@Ruehl_et_al_2016), and `'SzyszkowskiLangmuir'` following the Szyszkowski-Langmuir equation.
-Parameters for the three surface-partitioning models must be specified as shown in the example below, and a full comparison
-  of surface-partitioning options can be found in the `Singer_Ward` example.
+
+`PySDM` "v2" includes a new example demonstrating the available models for droplet surface tension.
+The four surface tension options included in `PySDM`, which define the droplet surface tension as 
+  a function of dry aerosol composition and wet radius, are: `'Constant'`, 
+  `'CompressedFilmOvadnevaite'` (@Ovadnevaite_et_al_2017), `'CompressedFilmRuehl'` (@Ruehl_et_al_2016), 
+  and `'SzyszkowskiLangmuir'` following the Szyszkowski-Langmuir equation.
+Parameters for the three surface-partitioning models must be specified as shown below.
+A full comparison of the four surface tension models can be found in the `Singer_Ward` example.
 ```python
 from PySDM import Formulae
 f = Formulae(
     surface_tension='CompressedFilmOvadnevaite',
     constants={
         'sgm_org': 35 * si.mN / si.m,
         'delta_min': 1.75 * si.nm
     }
 )
 ```
 
 ## Adaptive time-stepping
-In `PySDM` v2, the condensation, collision, and displacement dynamics 
+
+In `PySDM` "v2", the `Condensation`, `Collision`, and `Displacement` "dynamics"
   all support adaptive time-stepping logic,
-  which involves substepping within the user-specified time step used for coupling
-  with the environmental coupled-flow framework.
+  which involves sub-stepping within the user-specified time step used for coupling
+  with the "environment".
 Adaptivity is enabled by default and can be disabled by passing `False` as the value of optional `adaptive`
-  keyword to the given dynamic, i.e. `builder.add_dynamic(Dynamic(**kwargs, adaptive=False))`.
-The adaptive time-step controls are described in a forthcomming @Bartman_et_al_2022_adaptive 
-  publication and are bespoke developments introduced partialy in `PySDM` v1.
-The time-step adaptivity aims both to reduce computational errors where the specified time step is
-  longer than the timescale of the dynamic, as well as to reduce computational load by dynamically
-  changing the time-step. 
+  keyword to the given dynamic.
 This adaptive time-stepping applies separately in each grid box of a multidimensional environment,
-  and includes a load-balancing logic for the CPU backend and condensation example to simultaneously
-  handle grid cells with comparable substep count.
-The dynamic load-balancing across threads can be switched off by setting the `schedule` 
-  keyword parameter to a value of `"static"` when instantiating the `Condensation` dynamic
-  (the default value is `"dynamic"`).
-
+  and includes a load-balancing logic.
+In the case of collisions, the time-step adaptivity is aimed at eliminating errors
+  associated with multiple coalescence events within a timestep.
+In the case of condensation, the time-step adaptivity is aimed at reducing computational
+  load by coupling the time-step length choice with ambient supersaturation leading
+  to using longer time-steps in cloud-free regions and shorter time-steps in regions
+  where droplet [de]activation or rain evaporation occurs.
+In the case of displacement, the time-step adaptivity is aimed at obeying a given tolerance
+  in integration of the super-particle trajectories, and the error measure is constructed
+  by comparing implicit- and explicit-Euler solutions.
 
 # Author contributions
 
-EDJ led the formulation and implementation of the collisional breakup scheme with contributions from JBM.
-PB led the formulation and implementation of the adaptive time-stepping.
+EdJ led the formulation and implementation of the collisional breakup scheme with contributions from JBM.
+CES added the aerosol initialization framework.
+CES contributed the new surface tension models and relevant examples, in consultation with RXW.
+SAz contributed to extensions and enhancement of the one-dimensional kinematic framework environment.
+PB led the formulation and worked with SAr on implementation of the adaptive time-stepping schemes.
 KD contributed to setting up continuous integration workflows for the GPU backend. 
-CES contributed the aerosol initialisation framework.
-ID, CES, and AJ contributed to the CCN activation examples.
-CES contributed the representation of surface-partitioning by organic aerosol and the relevant examples in consultation with RXW.
-SA contributed to extensions and enhancement of the one-dimensional kinematic framework environment.
-The immersion freezing representation code was developed by SA who also carried out the maintenance of the project.
+ID, CES, and AJ contributed to the aerosol activation examples.
+The immersion freezing representation code was developed by SAr.
+Maintenance of the project have been carried out by SAr, CS, and EdJ.
 
-# Acknowledgements
+# Acknowledgments
 
 We thank Shin-ichiro Shima (University of Hyogo, Japan) for his continuous help and support in implementing SDM.
 Part of the outlined developments was supported by the generosity of Eric and Wendy Schmidt (by recommendation of Schmidt Futures).
 Development of ice-phase microphysics representation has been supported through 
-grant no. DE-SC0021034 by the Atmospheric System Research Program and 
-Atmospheric Radiation Measurement Program sponsored by the U.S. Department of Energy (DOE).
-EDJ's contributions were made possible by support from the Department of Energy Computational Sciences Graduate Research Fellowship.
+  grant no. DE-SC0021034 by the Atmospheric System Research Program and 
+  Atmospheric Radiation Measurement Program sponsored by the U.S. Department of Energy (DOE).
+EdJ's contributions were made possible by support from the Department of Energy Computational Sciences Graduate Research Fellowship.
 
 # References
```

### Comparing `PySDM-2.8/paper/paperv1.md` & `PySDM-2.9/paper/paperv1.md`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/paper/readme.pdf` & `PySDM-2.9/paper/readme.pdf`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/paper/test.pdf` & `PySDM-2.9/paper/test.pdf`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/setup.py` & `PySDM-2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 setup(
     name="PySDM",
     description="Pythonic particle-based (super-droplet) warm-rain/aqueous-chemistry"
     " cloud microphysics package with box, parcel & 1D/2D prescribed-flow"
     " examples in Python, Julia and Matlab",
-    version='2.8',
+    version='2.9',
     setup_requires=["setuptools_scm"],
     install_requires=[
         "ThrustRTC==0.3.19",
         "CURandRTC" + ("==0.1.6" if "CI" in os.environ else ">=0.1.2"),
-        "numba" + ("==0.55.1" if "CI" in os.environ else ">=0.51.2"),
+        "numba" + ("==0.55.2" if "CI" in os.environ else ">=0.51.2"),
         "numpy" + ("==1.21" if "CI" in os.environ else ""),
         "Pint" + ("==0.17" if "CI" in os.environ else ""),
         "chempy" + ("==0.7.10" if "CI" in os.environ else ""),
         "scipy" + ("==1.6.3" if "CI" in os.environ else ""),
         "pyevtk" + ("==1.2.0" if "CI" in os.environ else ""),
     ],
     author="https://github.com/atmos-cloud-sim-uj/PySDM/graphs/contributors",
```

### Comparing `PySDM-2.8/tests/devops_tests/test_todos_annotated.py` & `PySDM-2.9/tests/devops_tests/test_todos_annotated.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/abdul_razzak_ghan_2000/test_single_supersaturation_peak.py` & `PySDM-2.9/tests/smoke_tests/abdul_razzak_ghan_2000/test_single_supersaturation_peak.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/alpert_and_knopf_2016/test_ak16_fig_1.py` & `PySDM-2.9/tests/smoke_tests/alpert_and_knopf_2016/test_ak16_fig_1.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_conservation.py` & `PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_conservation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_displacement.py` & `PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_displacement.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_event_rates.py` & `PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_event_rates.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_initialisation.py` & `PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_initialisation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_and_shima_2017/test_vs_bdf.py` & `PySDM-2.9/tests/smoke_tests/arabas_and_shima_2017/test_vs_bdf.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_adaptive_displacement.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_adaptive_displacement.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_environment.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_environment.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_export.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_export.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_freezing.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_freezing.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_gui_settings.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_gui_settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_initialisation.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_initialisation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/arabas_et_al_2015/test_spin_up.py` & `PySDM-2.9/tests/smoke_tests/arabas_et_al_2015/test_spin_up.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/berry_1967/test_coalescence.py` & `PySDM-2.9/tests/smoke_tests/berry_1967/test_coalescence.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/dejong_and_mackay_2022/test_collision.py` & `PySDM-2.9/tests/smoke_tests/dejong_and_mackay_2022/test_collision.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_fig_1.py` & `PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_fig_1.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_ionic_strength.py` & `PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_ionic_strength.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_spectrum_at_t_0.py` & `PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_spectrum_at_t_0.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/kreidenweis_et_al_2003/test_table_3.py` & `PySDM-2.9/tests/smoke_tests/kreidenweis_et_al_2003/test_table_3.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/constants.py` & `PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/constants.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/test_fig_1.py` & `PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/test_fig_1.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/test_fig_2.py` & `PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/test_fig_2.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/lowe_et_al_2019/test_surface_tension_models.py` & `PySDM-2.9/tests/smoke_tests/lowe_et_al_2019/test_surface_tension_models.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/pyrcel/test_parcel_example.py` & `PySDM-2.9/tests/smoke_tests/pyrcel/test_parcel_example.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/shima_et_al_2009/test_coalescence.py` & `PySDM-2.9/tests/smoke_tests/shima_et_al_2009/test_coalescence.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/test_few_steps.py` & `PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/test_few_steps.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         dt=30 * si.s,
         dz=60 * si.m,
         precip=False,
         rho_times_w_1=2 * si.m / si.s * si.kg / si.m**3,
     )
     settings.particle_reservoir_depth = particle_reservoir_depth
     settings.t_max = 50 * settings.dt
+    settings.condensation_update_thd = True
     simulation = Simulation(settings)
 
     # Act
     output = simulation.run().products
 
     # Plot
     def mean_profile_over_last_steps(var, smooth=True):
@@ -76,7 +77,42 @@
     assert 0.01 < max(mean_profile_over_last_steps("peak supersaturation")) < 0.1
     assert min(mean_profile_over_last_steps("ql")) < 1e-10
     assert 0.15 < max(mean_profile_over_last_steps("ql")) < 0.25
     assert max(mean_profile_over_last_steps("activating rate")) == 0
 
     assert max(mean_profile_over_last_steps("ripening rate")) > 0
     assert max(mean_profile_over_last_steps("deactivating rate")) > 0
+
+
+def test_fixed_thd():
+    # Arrange
+    n_sd_per_gridbox = 128
+    settings = Settings(
+        n_sd_per_gridbox=n_sd_per_gridbox,
+        dt=30 * si.s,
+        dz=60 * si.m,
+        precip=False,
+        rho_times_w_1=2 * si.m / si.s * si.kg / si.m**3,
+    )
+    settings.t_max = 50 * settings.dt
+    settings.condensation_update_thd = False
+    simulation = Simulation(settings)
+
+    # Act
+    output = simulation.run().products
+
+    # Assert
+    mean_profile_over_last_steps = lambda var: np.mean(
+        output[var][output["z"] >= 0, -10:], axis=1
+    )
+    sd_prof = mean_profile_over_last_steps("super droplet count per gridbox")
+    assert 0.5 * n_sd_per_gridbox < min(sd_prof) < 1.5 * n_sd_per_gridbox
+    assert 0.5 * n_sd_per_gridbox < max(sd_prof) < 1.5 * n_sd_per_gridbox
+
+    assert 0.01 < max(mean_profile_over_last_steps("peak supersaturation")) < 0.1
+    assert min(mean_profile_over_last_steps("ql")) < 1e-10
+    assert 0.6 < max(mean_profile_over_last_steps("ql")) < 0.9
+    assert max(mean_profile_over_last_steps("activating rate")) == 0
+    assert max(mean_profile_over_last_steps("ripening rate")) == 0
+    assert max(mean_profile_over_last_steps("deactivating rate")) == 0
+
+    assert sum(np.amin(output["thd"], axis=1)) == sum(np.amax(output["thd"], axis=1))
```

### Comparing `PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/test_initial_condition.py` & `PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/test_initial_condition.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/shipway_and_hill_2012/test_settings.py` & `PySDM-2.9/tests/smoke_tests/shipway_and_hill_2012/test_settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/yang_et_al_2018/test_displacement.py` & `PySDM-2.9/tests/smoke_tests/yang_et_al_2018/test_displacement.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/yang_et_al_2018/test_initialisation.py` & `PySDM-2.9/tests/smoke_tests/yang_et_al_2018/test_initialisation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/smoke_tests/yang_et_al_2018/test_just_do_it.py` & `PySDM-2.9/tests/smoke_tests/yang_et_al_2018/test_just_do_it.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/attributes/test_acidity.py` & `PySDM-2.9/tests/unit_tests/attributes/test_acidity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/attributes/test_area_radius.py` & `PySDM-2.9/tests/unit_tests/attributes/test_area_radius.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/attributes/test_critical_supersaturation.py` & `PySDM-2.9/tests/unit_tests/attributes/test_critical_supersaturation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/attributes/test_terminal_velocity.py` & `PySDM-2.9/tests/unit_tests/attributes/test_terminal_velocity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/storage/test_index.py` & `PySDM-2.9/tests/unit_tests/backends/storage/test_index.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_collisions_methods.py` & `PySDM-2.9/tests/unit_tests/backends/test_collisions_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_ctor_defaults.py` & `PySDM-2.9/tests/unit_tests/backends/test_ctor_defaults.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_freezing_methods.py` & `PySDM-2.9/tests/unit_tests/backends/test_freezing_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_moments_methods.py` & `PySDM-2.9/tests/unit_tests/backends/test_moments_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_oxidation.py` & `PySDM-2.9/tests/unit_tests/backends/test_oxidation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_physics_methods.py` & `PySDM-2.9/tests/unit_tests/backends/test_physics_methods.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/backends/test_toms748.py` & `PySDM-2.9/tests/unit_tests/backends/test_toms748.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dummy_environment.py` & `PySDM-2.9/tests/unit_tests/dummy_environment.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dummy_particulator.py` & `PySDM-2.9/tests/unit_tests/dummy_particulator.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/__parametrisation__.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/__parametrisation__.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/test_croupiers.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/test_croupiers.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/test_defaults.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/test_defaults.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/test_kernels.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/test_kernels.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/test_sdm_breakup.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/test_sdm_breakup.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/test_sdm_multi_cell.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/test_sdm_multi_cell.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/collisions/test_sdm_single_cell.py` & `PySDM-2.9/tests/unit_tests/dynamics/collisions/test_sdm_single_cell.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/condensation/test_diagnostics.py` & `PySDM-2.9/tests/unit_tests/dynamics/condensation/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/displacement/displacement_settings.py` & `PySDM-2.9/tests/unit_tests/dynamics/displacement/displacement_settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/displacement/test_advection.py` & `PySDM-2.9/tests/unit_tests/dynamics/displacement/test_advection.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/displacement/test_courant_product.py` & `PySDM-2.9/tests/unit_tests/dynamics/displacement/test_courant_product.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/displacement/test_sedimentation.py` & `PySDM-2.9/tests/unit_tests/dynamics/displacement/test_sedimentation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/dynamics/test_eulerian_advection.py` & `PySDM-2.9/tests/unit_tests/dynamics/test_eulerian_advection.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/impl/test_moments.py` & `PySDM-2.9/tests/unit_tests/impl/test_moments.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/impl/test_particle_attributes.py` & `PySDM-2.9/tests/unit_tests/impl/test_particle_attributes.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/initialisation/test_aerosol_init.py` & `PySDM-2.9/tests/unit_tests/initialisation/test_aerosol_init.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/initialisation/test_r_wet_init.py` & `PySDM-2.9/tests/unit_tests/initialisation/test_r_wet_init.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/initialisation/test_spectral_discretisation.py` & `PySDM-2.9/tests/unit_tests/initialisation/test_spectral_discretisation.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_accommodation_coefficients.py` & `PySDM-2.9/tests/unit_tests/physics/test_accommodation_coefficients.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_constants.py` & `PySDM-2.9/tests/unit_tests/physics/test_constants.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_dimensional_analysis.py` & `PySDM-2.9/tests/unit_tests/physics/test_dimensional_analysis.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_formulae.py` & `PySDM-2.9/tests/unit_tests/physics/test_formulae.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_freezing_temperature_spectra.py` & `PySDM-2.9/tests/unit_tests/physics/test_freezing_temperature_spectra.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_latent_heat.py` & `PySDM-2.9/tests/unit_tests/physics/test_latent_heat.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_saturation_vapour_pressure.py` & `PySDM-2.9/tests/unit_tests/physics/test_saturation_vapour_pressure.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_spectra.py` & `PySDM-2.9/tests/unit_tests/physics/test_spectra.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_spectra_top_hat.py` & `PySDM-2.9/tests/unit_tests/physics/test_spectra_top_hat.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/physics/test_thermal_conductivity.py` & `PySDM-2.9/tests/unit_tests/physics/test_thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/products/test_ambient_relative_humidity.py` & `PySDM-2.9/tests/unit_tests/products/test_ambient_relative_humidity.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/products/test_cooling_rate.py` & `PySDM-2.9/tests/unit_tests/products/test_cooling_rate.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/products/test_impl.py` & `PySDM-2.9/tests/unit_tests/products/test_impl.py`

 * *Files identical despite different names*

### Comparing `PySDM-2.8/tests/unit_tests/test_particulator.py` & `PySDM-2.9/tests/unit_tests/test_particulator.py`

 * *Files identical despite different names*

