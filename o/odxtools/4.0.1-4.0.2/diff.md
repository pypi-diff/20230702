# Comparing `tmp/odxtools-4.0.1.tar.gz` & `tmp/odxtools-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odxtools-4.0.1.tar", last modified: Wed Jun 28 12:36:24 2023, max compression
+gzip compressed data, was "odxtools-4.0.2.tar", last modified: Sun Jul  2 11:28:37 2023, max compression
```

## Comparing `odxtools-4.0.1.tar` & `odxtools-4.0.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.980317 odxtools-4.0.1/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.0.1/LICENSE
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-06-28 12:36:24.976317 odxtools-4.0.1/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.0.1/README.md
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.956316 odxtools-4.0.1/examples/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.0.1/examples/__init__.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.0.1/examples/isotp_send.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.0.1/examples/mksomersaultpdx.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.0.1/examples/pdxcopy.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    81924 2023-06-28 12:35:57.000000 odxtools-4.0.1/examples/somersaultecu.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-4.0.1/examples/somersaultlazy.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.968317 odxtools-4.0.1/odxtools/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.0.1/odxtools/__main__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/admindata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/audience.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.968317 odxtools-4.0.1/odxtools/cli/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.0.1/odxtools/cli/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/cli/_parser_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/cli/_print_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/cli/browse.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/cli/dummy_sub_parser.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/cli/find.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7317 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/cli/list.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/cli/main.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/cli/snoop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/communicationparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8581 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/companydata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/comparam_subset.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.972317 odxtools-4.0.1/odxtools/compumethods/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/compumethodbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/compurationalcoeffs.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/compuscale.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7485 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/createanycompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/identicalcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/limit.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/linearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/scalelinearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/tabintpcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/compumethods/texttablecompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/database.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15371 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/dataobjectproperty.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/decodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27425 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/diagcodedtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6643 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/diagdatadictionaryspec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    39660 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/diaglayer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/diaglayercontainer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11411 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/diaglayerraw.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/diaglayertype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6969 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/ecu_variant_matcher.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/encodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7285 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/endofpdufield.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/envdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/envdatadesc.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/exceptions.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/functionalclass.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/globals.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/isotp_state_machine.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/load_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/load_odx_d_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/load_pdx_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/message.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12896 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/multiplexer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4185 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/nameditemlist.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/obd.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/odxlink.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameter_info.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.976317 odxtools-4.0.1/odxtools/parameters/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/codedconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/createanyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/dynamicparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/lengthkeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3011 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/parameters/matchingrequestparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/nrcconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7208 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/parameters/parameterbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4108 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/parameters/parameterwithdop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/physicalconstantparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/reservedparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/systemparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/tableentryparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2565 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/parameters/tablekeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/tablestructparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/parameters/valueparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/parentref.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/physicaltype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13655 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/service.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16374 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/specialdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/state.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/statechart.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/statetransition.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24316 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/structures.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8058 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/table.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/uds.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/units.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.0.1/odxtools/utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-06-28 12:35:57.000000 odxtools-4.0.1/odxtools/version.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.0.1/odxtools/write_pdx_file.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.968317 odxtools-4.0.1/odxtools.egg-info/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-06-28 12:36:24.000000 odxtools-4.0.1/odxtools.egg-info/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3342 2023-06-28 12:36:24.000000 odxtools-4.0.1/odxtools.egg-info/SOURCES.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-06-28 12:36:24.000000 odxtools-4.0.1/odxtools.egg-info/dependency_links.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-06-28 12:36:24.000000 odxtools-4.0.1/odxtools.egg-info/entry_points.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-06-28 12:36:24.000000 odxtools-4.0.1/odxtools.egg-info/requires.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-06-28 12:36:24.000000 odxtools-4.0.1/odxtools.egg-info/top_level.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.0.1/pyproject.toml
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-06-28 12:36:24.980317 odxtools-4.0.1/setup.cfg
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.0.1/setup.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-28 12:36:24.976317 odxtools-4.0.1/tests/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10427 2023-01-27 13:39:15.000000 odxtools-4.0.1/tests/test_compu_methods.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51695 2023-06-28 12:35:57.000000 odxtools-4.0.1/tests/test_decoding.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36363 2023-06-21 06:52:15.000000 odxtools-4.0.1/tests/test_diag_coded_types.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9192 2023-06-21 06:52:15.000000 odxtools-4.0.1/tests/test_diag_data_dictionary_spec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14065 2023-06-21 06:52:15.000000 odxtools-4.0.1/tests/test_ecu_variant_matching.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.0.1/tests/test_ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.0.1/tests/test_encoding.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.0.1/tests/test_odxtools.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.0.1/tests/test_odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.0.1/tests/test_readparameters.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.0.1/tests/test_singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11866 2023-06-28 12:35:57.000000 odxtools-4.0.1/tests/test_somersault.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.0.1/tests/test_unit_spec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.0.1/tests/test_utils.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.375399 odxtools-4.0.2/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.0.2/LICENSE
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-02 11:28:37.375399 odxtools-4.0.2/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.0.2/README.md
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.339398 odxtools-4.0.2/examples/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.0.2/examples/__init__.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.0.2/examples/isotp_send.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.0.2/examples/mksomersaultpdx.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.0.2/examples/pdxcopy.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    81924 2023-07-02 11:28:36.000000 odxtools-4.0.2/examples/somersaultecu.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-4.0.2/examples/somersaultlazy.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.355399 odxtools-4.0.2/odxtools/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.0.2/odxtools/__main__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/admindata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/audience.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.359399 odxtools-4.0.2/odxtools/cli/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.0.2/odxtools/cli/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/cli/_parser_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/cli/_print_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/cli/browse.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/cli/dummy_sub_parser.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/cli/find.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7317 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/cli/list.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/cli/main.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/cli/snoop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/communicationparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8581 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/companydata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/comparam_subset.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.367399 odxtools-4.0.2/odxtools/compumethods/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/compumethodbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/compurationalcoeffs.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/compuscale.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7662 2023-07-02 11:28:36.000000 odxtools-4.0.2/odxtools/compumethods/createanycompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/identicalcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/limit.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/linearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/scalelinearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/tabintpcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/compumethods/texttablecompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/database.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15371 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/dataobjectproperty.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/decodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27425 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/diagcodedtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6643 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/diagdatadictionaryspec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    39660 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/diaglayer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/diaglayercontainer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11411 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/diaglayerraw.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/diaglayertype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6969 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/ecu_variant_matcher.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/encodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7285 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/endofpdufield.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/envdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/envdatadesc.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/exceptions.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/functionalclass.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/globals.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/isotp_state_machine.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/load_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/load_odx_d_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/load_pdx_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/message.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12896 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/multiplexer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4185 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/nameditemlist.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/obd.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/odxlink.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameter_info.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.371399 odxtools-4.0.2/odxtools/parameters/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/codedconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/createanyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/dynamicparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/lengthkeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3011 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/parameters/matchingrequestparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/nrcconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7208 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/parameters/parameterbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4108 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/parameters/parameterwithdop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/physicalconstantparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/reservedparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/systemparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/tableentryparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2484 2023-07-02 11:28:36.000000 odxtools-4.0.2/odxtools/parameters/tablekeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/tablestructparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/parameters/valueparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/parentref.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/physicaltype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13655 2023-06-28 12:35:57.000000 odxtools-4.0.2/odxtools/service.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16374 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/specialdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/state.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/statechart.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/statetransition.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24316 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/structures.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8058 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/table.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/uds.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/units.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.0.2/odxtools/utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-07-02 11:28:36.000000 odxtools-4.0.2/odxtools/version.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.0.2/odxtools/write_pdx_file.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.359399 odxtools-4.0.2/odxtools.egg-info/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-02 11:28:37.000000 odxtools-4.0.2/odxtools.egg-info/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3342 2023-07-02 11:28:37.000000 odxtools-4.0.2/odxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-07-02 11:28:37.000000 odxtools-4.0.2/odxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-07-02 11:28:37.000000 odxtools-4.0.2/odxtools.egg-info/entry_points.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-07-02 11:28:37.000000 odxtools-4.0.2/odxtools.egg-info/requires.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-07-02 11:28:37.000000 odxtools-4.0.2/odxtools.egg-info/top_level.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.0.2/pyproject.toml
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-07-02 11:28:37.375399 odxtools-4.0.2/setup.cfg
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.0.2/setup.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-02 11:28:37.375399 odxtools-4.0.2/tests/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14195 2023-07-02 11:28:36.000000 odxtools-4.0.2/tests/test_compu_methods.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51695 2023-06-28 12:35:57.000000 odxtools-4.0.2/tests/test_decoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36363 2023-06-21 06:52:15.000000 odxtools-4.0.2/tests/test_diag_coded_types.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9192 2023-06-21 06:52:15.000000 odxtools-4.0.2/tests/test_diag_data_dictionary_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14065 2023-06-21 06:52:15.000000 odxtools-4.0.2/tests/test_ecu_variant_matching.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.0.2/tests/test_ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.0.2/tests/test_encoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.0.2/tests/test_odxtools.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.0.2/tests/test_odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.0.2/tests/test_readparameters.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.0.2/tests/test_singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11866 2023-06-28 12:35:57.000000 odxtools-4.0.2/tests/test_somersault.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.0.2/tests/test_unit_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.0.2/tests/test_utils.py
```

### Comparing `odxtools-4.0.1/LICENSE` & `odxtools-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/PKG-INFO` & `odxtools-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 4.0.1
+Version: 4.0.2
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-4.0.1/README.md` & `odxtools-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/examples/isotp_send.py` & `odxtools-4.0.2/examples/isotp_send.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/examples/mksomersaultpdx.py` & `odxtools-4.0.2/examples/mksomersaultpdx.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/examples/pdxcopy.py` & `odxtools-4.0.2/examples/pdxcopy.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/examples/somersaultecu.py` & `odxtools-4.0.2/examples/somersaultecu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -503,434 +503,14 @@
             compu_method=somersault_compumethods["boolean"],
             unit_ref=None,
             is_visible_raw=None,
             sdgs=[],
         ),
 }
 
-# tables
-somersault_tables = {
-    "flip_quality":
-        Table(
-            odx_id=OdxLinkId("somersault.table.flip_quality", doc_frags),
-            short_name="flip_quality",
-            long_name="Flip Quality",
-            description="<p>The quality the flip (average, good or best)</p>",
-            semantic="QUALITY",
-            key_dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-            table_rows=[
-                TableRow(
-                    odx_id=OdxLinkId("somersault.table.flip_quality.average", doc_frags),
-                    short_name="average",
-                    long_name="Average",
-                    key=3,
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                    description="<p>The quality of the flip is average</p>",
-                    semantic="QUALITY-KEY",
-                    dop_ref=None,
-                    sdgs=[],
-                ),
-                TableRow(
-                    odx_id=OdxLinkId("somersault.table.flip_quality.good", doc_frags),
-                    short_name="good",
-                    long_name="Good",
-                    description=None,
-                    semantic=None,
-                    key=5,
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                    dop_ref=None,
-                    sdgs=[],
-                ),
-                TableRow(
-                    odx_id=OdxLinkId("somersault.table.flip_quality.best", doc_frags),
-                    short_name="best",
-                    long_name="Best",
-                    description=None,
-                    semantic=None,
-                    key=10,
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                    dop_ref=None,
-                    sdgs=[],
-                ),
-            ],
-            table_row_refs=[],
-            sdgs=[],
-        )
-}
-
-# muxs
-somersault_muxs = {
-    "flip_preference":
-        Multiplexer(
-            odx_id=OdxLinkId("somersault.multiplexer.flip_preference", doc_frags),
-            short_name="flip_preference",
-            long_name="Flip Preference",
-            description=None,
-            is_visible_raw=None,
-            sdgs=[],
-            byte_position=0,
-            switch_key=MultiplexerSwitchKey(
-                byte_position=0,
-                bit_position=0,
-                dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-            ),
-            default_case=MultiplexerDefaultCase(
-                short_name="default_case",
-                long_name="Default Case",
-                structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-            ),
-            cases=[
-                MultiplexerCase(
-                    short_name="forward_flip",
-                    long_name="Forward Flip",
-                    lower_limit="1",
-                    upper_limit="3",
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                ),
-                MultiplexerCase(
-                    short_name="backward_flip",
-                    long_name="Backward Flip",
-                    lower_limit="1",
-                    upper_limit="3",
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                ),
-            ],
-        )
-}
-
-# env-data
-somersault_env_datas = {
-    "flip_env_data":
-        EnvironmentData(
-            odx_id=OdxLinkId("somersault.env_data.flip_env_data", doc_frags),
-            short_name="flip_env_data",
-            long_name="Flip Env Data",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            byte_size=None,
-            dtc_values=[],
-            parameters=[
-                ValueParameter(
-                    short_name="flip_speed",
-                    long_name="Flip Speed",
-                    description=None,
-                    physical_default_value_raw=None,
-                    byte_position=0,
-                    semantic="DATA",
-                    dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                    dop_snref=None,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                PhysicalConstantParameter(
-                    short_name="flip_direction",
-                    long_name="Flip Direction",
-                    description=None,
-                    byte_position=1,
-                    semantic="DATA",
-                    physical_constant_value="1",
-                    dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                    dop_snref=None,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-        )
-}
-
-# env-data-desc
-somersault_env_data_descs = {
-    "flip_env_data_desc":
-        EnvironmentDataDescription(
-            odx_id=OdxLinkId("somersault.env_data_desc.flip_env_data_desc", doc_frags),
-            short_name="flip_env_data_desc",
-            long_name="Flip Env Data Desc",
-            description=None,
-            param_snref="flip_speed",
-            param_snpathref=None,
-            is_visible_raw=None,
-            env_datas=[],
-            env_data_refs=[OdxLinkRef("somersault.env_data.flip_env_data", doc_frags)],
-            sdgs=[],
-        )
-}
-
-# requests
-somersault_requests = {
-    "start_session":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.start_session", doc_frags),
-            short_name="start_session",
-            long_name="Start the diagnostic session & do some mischief",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.DiagnosticSessionControl.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                CodedConstParameter(
-                    short_name="odx_id",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=1,
-                    coded_value=0x0,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-    "stop_session":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.stop_session", doc_frags),
-            short_name="stop_session",
-            long_name="Terminate the current diagnostic session",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.DiagnosticSessionControl.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                CodedConstParameter(
-                    short_name="odx_id",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=1,
-                    coded_value=0x1,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-    "tester_present":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.tester_present", doc_frags),
-            short_name="tester_present",
-            long_name="Prevent the current diagnostic session from timing out",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.TesterPresent.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                CodedConstParameter(
-                    short_name="odx_id",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=1,
-                    coded_value=0x0,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-    "set_operation_params":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.set_operation_params", doc_frags),
-            short_name="set_operation_params",
-            long_name="Specify the mode of operation for the ECU; e.g. if rings "
-            "of fire ought to be used for maximum effect",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.ForwardFlipCondition.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                ValueParameter(
-                    short_name="use_fire_ring",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    physical_default_value_raw=None,
-                    byte_position=1,
-                    dop_ref=OdxLinkRef("somersault.DOP.boolean", doc_frags),
-                    dop_snref=None,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-    "forward_flips":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.do_forward_flips", doc_frags),
-            short_name="do_forward_flips",
-            long_name="Do forward somersaults & some other mischief",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.ForwardFlip.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                ValueParameter(
-                    short_name="forward_soberness_check",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    physical_default_value_raw=None,
-                    dop_ref=OdxLinkRef("somersault.DOP.soberness_check", doc_frags),
-                    dop_snref=None,
-                    byte_position=1,
-                    # value must be 0x12 for the request to be accepted
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                ValueParameter(
-                    short_name="num_flips",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    physical_default_value_raw=None,
-                    byte_position=2,
-                    dop_ref=OdxLinkRef("somersault.DOP.num_flips", doc_frags),
-                    dop_snref=None,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-    "backward_flips":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.do_backward_flips", doc_frags),
-            short_name="do_backward_flips",
-            long_name="Do a backward somersault & some other mischief",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.BackwardFlip.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                ValueParameter(
-                    short_name="backward_soberness_check",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    physical_default_value_raw=None,
-                    dop_ref=OdxLinkRef("somersault.DOP.soberness_check", doc_frags),
-                    dop_snref=None,
-                    byte_position=1,
-                    # value must be 0x21 for the request to be accepted
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                ValueParameter(
-                    short_name="num_flips",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    physical_default_value_raw=None,
-                    byte_position=2,
-                    dop_ref=OdxLinkRef("somersault.DOP.num_flips", doc_frags),
-                    dop_snref=None,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-    "report_status":
-        Request(
-            odx_id=OdxLinkId("somersault.RQ.report_status", doc_frags),
-            short_name="report_status",
-            long_name="Report back the current level of dizzy- & happiness.",
-            description=None,
-            sdgs=[],
-            is_visible_raw=None,
-            parameters=[
-                CodedConstParameter(
-                    short_name="sid",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=0,
-                    coded_value=SID.ReadDataByIdentifier.value,  # type: ignore
-                    bit_position=None,
-                    sdgs=[],
-                ),
-                CodedConstParameter(
-                    short_name="odx_id",
-                    long_name=None,
-                    semantic=None,
-                    description=None,
-                    diag_coded_type=somersault_diagcodedtypes["uint8"],
-                    byte_position=1,
-                    coded_value=0x0,
-                    bit_position=None,
-                    sdgs=[],
-                ),
-            ],
-            byte_size=None,
-        ),
-}
-
 # positive responses
 somersault_positive_responses = {
     "session":
         Response(
             odx_id=OdxLinkId("somersault.PR.session_start", doc_frags),
             short_name="session",
             long_name=None,
@@ -1441,14 +1021,434 @@
                     ),
                 ],
             ),
             byte_size=None,
         )
 }
 
+# tables
+somersault_tables = {
+    "flip_quality":
+        Table(
+            odx_id=OdxLinkId("somersault.table.flip_quality", doc_frags),
+            short_name="flip_quality",
+            long_name="Flip Quality",
+            description="<p>The quality the flip (average, good or best)</p>",
+            semantic="QUALITY",
+            key_dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+            table_rows=[
+                TableRow(
+                    odx_id=OdxLinkId("somersault.table.flip_quality.average", doc_frags),
+                    short_name="average",
+                    long_name="Average",
+                    key=3,
+                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    description="<p>The quality of the flip is average</p>",
+                    semantic="QUALITY-KEY",
+                    dop_ref=None,
+                    sdgs=[],
+                ),
+                TableRow(
+                    odx_id=OdxLinkId("somersault.table.flip_quality.good", doc_frags),
+                    short_name="good",
+                    long_name="Good",
+                    description=None,
+                    semantic=None,
+                    key=5,
+                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    dop_ref=None,
+                    sdgs=[],
+                ),
+                TableRow(
+                    odx_id=OdxLinkId("somersault.table.flip_quality.best", doc_frags),
+                    short_name="best",
+                    long_name="Best",
+                    description=None,
+                    semantic=None,
+                    key=10,
+                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    dop_ref=None,
+                    sdgs=[],
+                ),
+            ],
+            table_row_refs=[],
+            sdgs=[],
+        )
+}
+
+# muxs
+somersault_muxs = {
+    "flip_preference":
+        Multiplexer(
+            odx_id=OdxLinkId("somersault.multiplexer.flip_preference", doc_frags),
+            short_name="flip_preference",
+            long_name="Flip Preference",
+            description=None,
+            is_visible_raw=None,
+            sdgs=[],
+            byte_position=0,
+            switch_key=MultiplexerSwitchKey(
+                byte_position=0,
+                bit_position=0,
+                dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+            ),
+            default_case=MultiplexerDefaultCase(
+                short_name="default_case",
+                long_name="Default Case",
+                structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+            ),
+            cases=[
+                MultiplexerCase(
+                    short_name="forward_flip",
+                    long_name="Forward Flip",
+                    lower_limit="1",
+                    upper_limit="3",
+                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                ),
+                MultiplexerCase(
+                    short_name="backward_flip",
+                    long_name="Backward Flip",
+                    lower_limit="1",
+                    upper_limit="3",
+                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                ),
+            ],
+        )
+}
+
+# env-data
+somersault_env_datas = {
+    "flip_env_data":
+        EnvironmentData(
+            odx_id=OdxLinkId("somersault.env_data.flip_env_data", doc_frags),
+            short_name="flip_env_data",
+            long_name="Flip Env Data",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            byte_size=None,
+            dtc_values=[],
+            parameters=[
+                ValueParameter(
+                    short_name="flip_speed",
+                    long_name="Flip Speed",
+                    description=None,
+                    physical_default_value_raw=None,
+                    byte_position=0,
+                    semantic="DATA",
+                    dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    dop_snref=None,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                PhysicalConstantParameter(
+                    short_name="flip_direction",
+                    long_name="Flip Direction",
+                    description=None,
+                    byte_position=1,
+                    semantic="DATA",
+                    physical_constant_value="1",
+                    dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    dop_snref=None,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+        )
+}
+
+# env-data-desc
+somersault_env_data_descs = {
+    "flip_env_data_desc":
+        EnvironmentDataDescription(
+            odx_id=OdxLinkId("somersault.env_data_desc.flip_env_data_desc", doc_frags),
+            short_name="flip_env_data_desc",
+            long_name="Flip Env Data Desc",
+            description=None,
+            param_snref="flip_speed",
+            param_snpathref=None,
+            is_visible_raw=None,
+            env_datas=[],
+            env_data_refs=[OdxLinkRef("somersault.env_data.flip_env_data", doc_frags)],
+            sdgs=[],
+        )
+}
+
+# requests
+somersault_requests = {
+    "start_session":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.start_session", doc_frags),
+            short_name="start_session",
+            long_name="Start the diagnostic session & do some mischief",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.DiagnosticSessionControl.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                CodedConstParameter(
+                    short_name="odx_id",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=1,
+                    coded_value=0x0,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+    "stop_session":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.stop_session", doc_frags),
+            short_name="stop_session",
+            long_name="Terminate the current diagnostic session",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.DiagnosticSessionControl.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                CodedConstParameter(
+                    short_name="odx_id",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=1,
+                    coded_value=0x1,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+    "tester_present":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.tester_present", doc_frags),
+            short_name="tester_present",
+            long_name="Prevent the current diagnostic session from timing out",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.TesterPresent.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                CodedConstParameter(
+                    short_name="odx_id",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=1,
+                    coded_value=0x0,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+    "set_operation_params":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.set_operation_params", doc_frags),
+            short_name="set_operation_params",
+            long_name="Specify the mode of operation for the ECU; e.g. if rings "
+            "of fire ought to be used for maximum effect",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.ForwardFlipCondition.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                ValueParameter(
+                    short_name="use_fire_ring",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    physical_default_value_raw=None,
+                    byte_position=1,
+                    dop_ref=OdxLinkRef("somersault.DOP.boolean", doc_frags),
+                    dop_snref=None,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+    "forward_flips":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.do_forward_flips", doc_frags),
+            short_name="do_forward_flips",
+            long_name="Do forward somersaults & some other mischief",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.ForwardFlip.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                ValueParameter(
+                    short_name="forward_soberness_check",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    physical_default_value_raw=None,
+                    dop_ref=OdxLinkRef("somersault.DOP.soberness_check", doc_frags),
+                    dop_snref=None,
+                    byte_position=1,
+                    # value must be 0x12 for the request to be accepted
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                ValueParameter(
+                    short_name="num_flips",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    physical_default_value_raw=None,
+                    byte_position=2,
+                    dop_ref=OdxLinkRef("somersault.DOP.num_flips", doc_frags),
+                    dop_snref=None,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+    "backward_flips":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.do_backward_flips", doc_frags),
+            short_name="do_backward_flips",
+            long_name="Do a backward somersault & some other mischief",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.BackwardFlip.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                ValueParameter(
+                    short_name="backward_soberness_check",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    physical_default_value_raw=None,
+                    dop_ref=OdxLinkRef("somersault.DOP.soberness_check", doc_frags),
+                    dop_snref=None,
+                    byte_position=1,
+                    # value must be 0x21 for the request to be accepted
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                ValueParameter(
+                    short_name="num_flips",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    physical_default_value_raw=None,
+                    byte_position=2,
+                    dop_ref=OdxLinkRef("somersault.DOP.num_flips", doc_frags),
+                    dop_snref=None,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+    "report_status":
+        Request(
+            odx_id=OdxLinkId("somersault.RQ.report_status", doc_frags),
+            short_name="report_status",
+            long_name="Report back the current level of dizzy- & happiness.",
+            description=None,
+            sdgs=[],
+            is_visible_raw=None,
+            parameters=[
+                CodedConstParameter(
+                    short_name="sid",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=0,
+                    coded_value=SID.ReadDataByIdentifier.value,  # type: ignore
+                    bit_position=None,
+                    sdgs=[],
+                ),
+                CodedConstParameter(
+                    short_name="odx_id",
+                    long_name=None,
+                    semantic=None,
+                    description=None,
+                    diag_coded_type=somersault_diagcodedtypes["uint8"],
+                    byte_position=1,
+                    coded_value=0x0,
+                    bit_position=None,
+                    sdgs=[],
+                ),
+            ],
+            byte_size=None,
+        ),
+}
+
 # services
 somersault_services = {
     "start_session":
         DiagService(
             odx_id=OdxLinkId("somersault.service.session_start", doc_frags),
             short_name="session_start",
             long_name=None,
```

### Comparing `odxtools-4.0.1/examples/somersaultlazy.py` & `odxtools-4.0.2/examples/somersaultlazy.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/__init__.py` & `odxtools-4.0.2/odxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/admindata.py` & `odxtools-4.0.2/odxtools/admindata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/audience.py` & `odxtools-4.0.2/odxtools/audience.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/_parser_utils.py` & `odxtools-4.0.2/odxtools/cli/_parser_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/_print_utils.py` & `odxtools-4.0.2/odxtools/cli/_print_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/browse.py` & `odxtools-4.0.2/odxtools/cli/browse.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/dummy_sub_parser.py` & `odxtools-4.0.2/odxtools/cli/dummy_sub_parser.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/find.py` & `odxtools-4.0.2/odxtools/cli/find.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/list.py` & `odxtools-4.0.2/odxtools/cli/list.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/main.py` & `odxtools-4.0.2/odxtools/cli/main.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/cli/snoop.py` & `odxtools-4.0.2/odxtools/cli/snoop.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/communicationparameter.py` & `odxtools-4.0.2/odxtools/communicationparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/companydata.py` & `odxtools-4.0.2/odxtools/companydata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/comparam_subset.py` & `odxtools-4.0.2/odxtools/comparam_subset.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/__init__.py` & `odxtools-4.0.2/odxtools/compumethods/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/compumethodbase.py` & `odxtools-4.0.2/odxtools/compumethods/compumethodbase.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/compuscale.py` & `odxtools-4.0.2/odxtools/compumethods/compuscale.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/createanycompumethod.py` & `odxtools-4.0.2/odxtools/compumethods/createanycompumethod.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
+import warnings
 from typing import Any, Dict, List, Optional, Type, Union
 
+from ..exceptions import OdxWarning
 from ..globals import logger
 from ..odxlink import OdxDocFragment
 from ..odxtypes import DataType
 from ..utils import create_description_from_et
 from .compumethodbase import CompuMethod
 from .compuscale import CompuScale
 from .identicalcompumethod import IdenticalCompuMethod
@@ -48,18 +50,20 @@
 
     coeffs = scale_element.find("COMPU-RATIONAL-COEFFS")
     nums = coeffs.iterfind("COMPU-NUMERATOR/V")
 
     offset = computation_python_type(next(nums).text)
     factor_el = next(nums, None)
     factor = computation_python_type(factor_el.text if factor_el is not None else "0")
-    if coeffs.find("COMPU-DENOMINATOR/V") is not None:
-        kwargs["denominator"] = float(coeffs.findtext("COMPU-DENOMINATOR/V"))
-        assert kwargs["denominator"] > 0
-
+    denominator = 1.0
+    if (string := coeffs.findtext("COMPU-DENOMINATOR/V")) is not None:
+        denominator = float(string)
+        if denominator == 0:
+            warnings.warn("CompuMethod: A denominator of zero will lead to divisions by zero.",
+                          OdxWarning)
     # Read lower limit
     internal_lower_limit = Limit.from_et(
         scale_element.find("LOWER-LIMIT"),
         internal_type=internal_type,
     )
     if internal_lower_limit is None:
         internal_lower_limit = Limit(float("-inf"), IntervalType.INFINITE)
@@ -75,15 +79,15 @@
             internal_upper_limit = Limit(float("inf"), IntervalType.INFINITE)
         else:
             assert (internal_lower_limit is not None and
                     internal_lower_limit.interval_type == IntervalType.CLOSED)
             logger.info("Scale linear without UPPER-LIMIT")
             internal_upper_limit = internal_lower_limit
     kwargs["internal_upper_limit"] = internal_upper_limit
-    kwargs["denominator"] = 1.0
+    kwargs["denominator"] = denominator
     kwargs["factor"] = factor
     kwargs["offset"] = offset
 
     return LinearCompuMethod(**kwargs)
 
 
 def create_any_compu_method_from_et(et_element, doc_frags: List[OdxDocFragment],
```

### Comparing `odxtools-4.0.1/odxtools/compumethods/identicalcompumethod.py` & `odxtools-4.0.2/odxtools/compumethods/identicalcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/limit.py` & `odxtools-4.0.2/odxtools/compumethods/limit.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/linearcompumethod.py` & `odxtools-4.0.2/odxtools/compumethods/linearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/scalelinearcompumethod.py` & `odxtools-4.0.2/odxtools/compumethods/scalelinearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/tabintpcompumethod.py` & `odxtools-4.0.2/odxtools/compumethods/tabintpcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/compumethods/texttablecompumethod.py` & `odxtools-4.0.2/odxtools/compumethods/texttablecompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/database.py` & `odxtools-4.0.2/odxtools/database.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/dataobjectproperty.py` & `odxtools-4.0.2/odxtools/dataobjectproperty.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/decodestate.py` & `odxtools-4.0.2/odxtools/decodestate.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/diagcodedtypes.py` & `odxtools-4.0.2/odxtools/diagcodedtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/diagdatadictionaryspec.py` & `odxtools-4.0.2/odxtools/diagdatadictionaryspec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/diaglayer.py` & `odxtools-4.0.2/odxtools/diaglayer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/diaglayercontainer.py` & `odxtools-4.0.2/odxtools/diaglayercontainer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/diaglayerraw.py` & `odxtools-4.0.2/odxtools/diaglayerraw.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/diaglayertype.py` & `odxtools-4.0.2/odxtools/diaglayertype.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/ecu_variant_matcher.py` & `odxtools-4.0.2/odxtools/ecu_variant_matcher.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/ecu_variant_patterns.py` & `odxtools-4.0.2/odxtools/ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/encodestate.py` & `odxtools-4.0.2/odxtools/encodestate.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/endofpdufield.py` & `odxtools-4.0.2/odxtools/endofpdufield.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/envdata.py` & `odxtools-4.0.2/odxtools/envdata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/envdatadesc.py` & `odxtools-4.0.2/odxtools/envdatadesc.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/exceptions.py` & `odxtools-4.0.2/odxtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/functionalclass.py` & `odxtools-4.0.2/odxtools/functionalclass.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/isotp_state_machine.py` & `odxtools-4.0.2/odxtools/isotp_state_machine.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/message.py` & `odxtools-4.0.2/odxtools/message.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/multiplexer.py` & `odxtools-4.0.2/odxtools/multiplexer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/nameditemlist.py` & `odxtools-4.0.2/odxtools/nameditemlist.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/obd.py` & `odxtools-4.0.2/odxtools/obd.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/odxlink.py` & `odxtools-4.0.2/odxtools/odxlink.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/odxtypes.py` & `odxtools-4.0.2/odxtools/odxtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameter_info.py` & `odxtools-4.0.2/odxtools/parameter_info.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/__init__.py` & `odxtools-4.0.2/odxtools/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/codedconstparameter.py` & `odxtools-4.0.2/odxtools/parameters/codedconstparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/createanyparameter.py` & `odxtools-4.0.2/odxtools/parameters/createanyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/dynamicparameter.py` & `odxtools-4.0.2/odxtools/parameters/dynamicparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/lengthkeyparameter.py` & `odxtools-4.0.2/odxtools/parameters/lengthkeyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/matchingrequestparameter.py` & `odxtools-4.0.2/odxtools/parameters/matchingrequestparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/nrcconstparameter.py` & `odxtools-4.0.2/odxtools/parameters/nrcconstparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/parameterbase.py` & `odxtools-4.0.2/odxtools/parameters/parameterbase.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/parameterwithdop.py` & `odxtools-4.0.2/odxtools/parameters/parameterwithdop.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/physicalconstantparameter.py` & `odxtools-4.0.2/odxtools/parameters/physicalconstantparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/reservedparameter.py` & `odxtools-4.0.2/odxtools/parameters/reservedparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/systemparameter.py` & `odxtools-4.0.2/odxtools/parameters/systemparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/tableentryparameter.py` & `odxtools-4.0.2/odxtools/parameters/tableentryparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/tablekeyparameter.py` & `odxtools-4.0.2/odxtools/parameters/tablekeyparameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,17 @@
         if self.table_row_ref:
             self._table_row = odxlinks.resolve(self.table_row_ref)
 
     def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         super()._resolve_snrefs(diag_layer)
 
         if self.table_snref:
-            self._table = diag_layer.local_diag_data_dictionary_spec.tables[self.table_snref]
+            self._table = diag_layer.tables[self.table_snref]
         if self.table_row_snref:
-            self._table_row = diag_layer.local_diag_data_dictionary_spec.tables[
-                self.table_row_snref]
+            self._table_row = diag_layer.tables[self.table_row_snref]
 
     @property
     def table(self) -> "Table":
         return self._table
 
     @property
     def table_row(self) -> "TableRow":
```

### Comparing `odxtools-4.0.1/odxtools/parameters/tablestructparameter.py` & `odxtools-4.0.2/odxtools/parameters/tablestructparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parameters/valueparameter.py` & `odxtools-4.0.2/odxtools/parameters/valueparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/parentref.py` & `odxtools-4.0.2/odxtools/parentref.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/physicaltype.py` & `odxtools-4.0.2/odxtools/physicaltype.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/service.py` & `odxtools-4.0.2/odxtools/service.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/singleecujob.py` & `odxtools-4.0.2/odxtools/singleecujob.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/specialdata.py` & `odxtools-4.0.2/odxtools/specialdata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/state.py` & `odxtools-4.0.2/odxtools/state.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/statechart.py` & `odxtools-4.0.2/odxtools/statechart.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/statetransition.py` & `odxtools-4.0.2/odxtools/statetransition.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/structures.py` & `odxtools-4.0.2/odxtools/structures.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/table.py` & `odxtools-4.0.2/odxtools/table.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/uds.py` & `odxtools-4.0.2/odxtools/uds.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/units.py` & `odxtools-4.0.2/odxtools/units.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/utils.py` & `odxtools-4.0.2/odxtools/utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools/write_pdx_file.py` & `odxtools-4.0.2/odxtools/write_pdx_file.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/odxtools.egg-info/PKG-INFO` & `odxtools-4.0.2/odxtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 4.0.1
+Version: 4.0.2
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-4.0.1/odxtools.egg-info/SOURCES.txt` & `odxtools-4.0.2/odxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/setup.py` & `odxtools-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_decoding.py` & `odxtools-4.0.2/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_diag_coded_types.py` & `odxtools-4.0.2/tests/test_diag_coded_types.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_diag_data_dictionary_spec.py` & `odxtools-4.0.2/tests/test_diag_data_dictionary_spec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_ecu_variant_matching.py` & `odxtools-4.0.2/tests/test_ecu_variant_matching.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_ecu_variant_patterns.py` & `odxtools-4.0.2/tests/test_ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_encoding.py` & `odxtools-4.0.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_odxtools.py` & `odxtools-4.0.2/tests/test_odxtools.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_odxtypes.py` & `odxtools-4.0.2/tests/test_odxtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_readparameters.py` & `odxtools-4.0.2/tests/test_readparameters.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_singleecujob.py` & `odxtools-4.0.2/tests/test_singleecujob.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_somersault.py` & `odxtools-4.0.2/tests/test_somersault.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_unit_spec.py` & `odxtools-4.0.2/tests/test_unit_spec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.1/tests/test_utils.py` & `odxtools-4.0.2/tests/test_utils.py`

 * *Files identical despite different names*

