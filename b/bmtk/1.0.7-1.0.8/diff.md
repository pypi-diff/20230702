# Comparing `tmp/bmtk-1.0.7.tar.gz` & `tmp/bmtk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtk-1.0.7.tar", last modified: Tue Oct 25 19:35:24 2022, max compression
+gzip compressed data, was "bmtk-1.0.8.tar", last modified: Sun Jul  2 17:52:21 2023, max compression
```

## Comparing `bmtk-1.0.7.tar` & `bmtk-1.0.8.tar`

### file list

```diff
@@ -1,411 +1,425 @@
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1482 2019-10-23 23:40:04.000000 bmtk-1.0.7/LICENSE.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)      113 2022-05-24 19:01:38.000000 bmtk-1.0.7/MANIFEST.in
--rw-rw-r--   0 kael      (1000) kael      (1000)     3215 2022-10-25 19:35:24.969249 bmtk-1.0.7/PKG-INFO
--rw-rw-r--   0 kael      (1000) kael      (1000)     2223 2022-10-25 18:55:38.000000 bmtk-1.0.7/README.md
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.937249 bmtk-1.0.7/bmtk/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1543 2022-10-25 19:31:22.000000 bmtk-1.0.7/bmtk/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.937249 bmtk-1.0.7/bmtk/analyzer/
--rw-rw-r--   0 kael      (1000) kael      (1000)     7934 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/analyzer/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4336 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/analyzer/cell_vars.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9180 2022-06-14 03:21:44.000000 bmtk-1.0.7/bmtk/analyzer/compartment.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3594 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/analyzer/ecp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3751 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/analyzer/firing_rates.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      391 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/analyzer/io_tools.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17922 2022-08-01 16:35:47.000000 bmtk-1.0.7/bmtk/analyzer/spike_trains.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4787 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/analyzer/spikes_analyzer.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3890 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/analyzer/spikes_loader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      211 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/analyzer/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.941249 bmtk-1.0.7/bmtk/builder/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1580 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.941249 bmtk-1.0.7/bmtk/builder/auxi/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1520 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/builder/auxi/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2515 2020-07-29 19:00:45.000000 bmtk-1.0.7/bmtk/builder/auxi/edge_connectors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4592 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/auxi/node_params.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.941249 bmtk-1.0.7/bmtk/builder/bionet/
--rw-rw-r--   0 kael      (1000) kael      (1000)      627 2022-08-09 16:24:04.000000 bmtk-1.0.7/bmtk/builder/bionet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    18567 2022-08-22 22:10:49.000000 bmtk-1.0.7/bmtk/builder/bionet/swc_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3958 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/builder_utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9061 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/connection_map.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1796 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/builder/connector.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3033 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/edge.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.941249 bmtk-1.0.7/bmtk/builder/edges_sorter/
--rw-rw-r--   0 kael      (1000) kael      (1000)      868 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/edges_sorter/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3912 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/edges_sorter/memory_sorter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    27427 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/builder/edges_sorter/merge_sorter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2504 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/builder/functor_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3089 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/id_generator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17386 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/index_builders.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5336 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/builder/iterator.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.941249 bmtk-1.0.7/bmtk/builder/network_adaptors/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1632 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    18987 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/dm_network.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    23846 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/dm_network_orig.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    11414 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/edge_props_table.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    20975 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/edges_collator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    32355 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/network.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3057 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/network_adaptors/nxnetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    29868 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/builder/network_builder.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      179 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/networks.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3055 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/node.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4202 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/builder/node_pool.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3077 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/builder/node_set.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.941249 bmtk-1.0.7/bmtk/simulator/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1521 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.945249 bmtk-1.0.7/bmtk/simulator/bionet/
--rw-rw-r--   0 kael      (1000) kael      (1000)      153 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/README.md
--rw-rw-r--   0 kael      (1000) kael      (1000)     1844 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    20932 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/bionet/biocell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17281 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/bionet/bionetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    22312 2022-07-23 20:09:37.000000 bmtk-1.0.7/bmtk/simulator/bionet/biosimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3883 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/cell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2367 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/config.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.945249 bmtk-1.0.7/bmtk/simulator/bionet/default_setters/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1606 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_setters/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17512 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_setters/cell_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6112 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_setters/synapse_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2449 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_setters/synaptic_weights.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.945249 bmtk-1.0.7/bmtk/simulator/bionet/default_templates/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1036 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      608 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_templates/Biophys1.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      239 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/default_templates/advance.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     1110 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/gids.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3126 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/iclamp.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.945249 bmtk-1.0.7/bmtk/simulator/bionet/import3d/
--rw-rw-r--   0 kael      (1000) kael      (1000)    28325 2022-01-20 23:00:55.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/import3d_gui.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    10086 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/import3d_sec.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     2038 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_morphml.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    16444 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_nlcda.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    27594 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_nlcda3.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     7697 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_nts.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    12318 2022-01-20 23:00:55.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_swc.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      335 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/import3d.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     1905 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.945249 bmtk-1.0.7/bmtk/simulator/bionet/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1785 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    12011 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/ecp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10116 2022-10-25 19:31:22.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/record_cellvars.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4732 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/record_clamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6338 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/record_netcons.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4740 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/record_spikes.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17785 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/save_synapses.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3356 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/sim_module.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6935 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/xstim.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4012 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/modules/xstim_waveforms.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    23379 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/bionet/morphology.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5482 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/nml_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3537 2022-08-22 22:07:50.000000 bmtk-1.0.7/bmtk/simulator/bionet/nrn.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6924 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/pointprocesscell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      371 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/pointsomacell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1679 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/pyfunction_cache.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.945249 bmtk-1.0.7/bmtk/simulator/bionet/schemas/
--rw-rw-r--   0 kael      (1000) kael      (1000)     3335 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/schemas/config_schema.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      536 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/schemas/csv_edge_types.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      170 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/schemas/csv_node_types_external.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      347 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/schemas/csv_node_types_internal.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      162 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/schemas/csv_nodes_external.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      456 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/schemas/csv_nodes_internal.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     2257 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/seclamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     8019 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4278 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/bionet/utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3217 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/bionet/virtualcell.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.949249 bmtk-1.0.7/bmtk/simulator/core/
--rw-rw-r--   0 kael      (1000) kael      (1000)        0 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/core/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      426 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/core/edge_population.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    15634 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/graph.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4506 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/io_tools.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1772 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/core/network_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      886 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/core/node_population.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1709 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/node_sets.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13708 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/core/pyfunction_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4610 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/simulation_config.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6008 2022-06-14 03:21:34.000000 bmtk-1.0.7/bmtk/simulator/core/simulation_config_validator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      203 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/simulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10573 2022-07-13 15:51:11.000000 bmtk-1.0.7/bmtk/simulator/core/simulator_network.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.949249 bmtk-1.0.7/bmtk/simulator/core/sonata_reader/
--rw-rw-r--   0 kael      (1000) kael      (1000)      159 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/core/sonata_reader/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7429 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/sonata_reader/edge_adaptor.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10541 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/sonata_reader/network_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7783 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/sonata_reader/node_adaptor.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.949249 bmtk-1.0.7/bmtk/simulator/core/sonata_schemas/
--rw-rw-r--   0 kael      (1000) kael      (1000)     4394 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/core/sonata_schemas/config_schema.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.949249 bmtk-1.0.7/bmtk/simulator/filternet/
--rw-rw-r--   0 kael      (1000) kael      (1000)      234 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1782 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/cell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)       57 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/cell_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      691 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/config.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.949249 bmtk-1.0.7/bmtk/simulator/filternet/default_setters/
--rw-rw-r--   0 kael      (1000) kael      (1000)       28 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/default_setters/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9248 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/filternet/default_setters/cell_loaders.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2046 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/filternetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      185 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/filters.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7288 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/filtersimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      756 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.953249 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/
--rw-rw-r--   0 kael      (1000) kael      (1000)      195 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.953249 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/
--rwxrwxr-x   0 kael      (1000) kael      (1000)    15615 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)    12437 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     4186 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     9904 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     1003 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     2783 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv
--rw-rw-r--   0 kael      (1000) kael      (1000)     6361 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cellmetrics.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6596 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cellmodel.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9019 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cursor.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3567 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/fitfuns.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    16117 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/kernel.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9140 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2111 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2567 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/linearfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3995 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/lnunit.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6022 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/make_cell_list.py
--rwxrwxr-x   0 kael      (1000) kael      (1000)    12157 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/movie.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2528 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/poissongeneration.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      263 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/singleunitcell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4618 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/spatialfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3730 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/temporalfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2268 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/transferfunction.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7390 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/util_fns.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3188 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/utilities.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.953249 bmtk-1.0.7/bmtk/simulator/filternet/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)       81 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      161 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/modules/base.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4587 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/modules/create_spikes.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5940 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/modules/record_rates.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4157 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/pyfunction_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9152 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)       64 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/filternet/transfer_functions.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      150 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/filternet/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.953249 bmtk-1.0.7/bmtk/simulator/pointnet/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1733 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/pointnet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2208 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/pointnet/config.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.953249 bmtk-1.0.7/bmtk/simulator/pointnet/default_setters/
--rw-rw-r--   0 kael      (1000) kael      (1000)       59 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/pointnet/default_setters/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      471 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/pointnet/default_setters/synapse_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      441 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/pointnet/default_setters/synaptic_weights.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2409 2022-07-14 00:17:59.000000 bmtk-1.0.7/bmtk/simulator/pointnet/gids.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    26368 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/pointnet/glif_utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2820 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/pointnet/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.953249 bmtk-1.0.7/bmtk/simulator/pointnet/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)       83 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/pointnet/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7014 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/pointnet/modules/multimeter_reporter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6298 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/pointnet/modules/record_spikes.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1751 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/simulator/pointnet/nest_utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10782 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/simulator/pointnet/pointnetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    11673 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/pointnet/pointsimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7611 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/pointnet/property_map.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1616 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/pointnet/pyfunction_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    14299 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/simulator/pointnet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6528 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/pointnet/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/simulator/popnet/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1622 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/popnet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1818 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/popnet/config.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3583 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/popnet/popedge.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17362 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/popnet/popnetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5797 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/popnet/popnode.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13400 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/popnet/popsimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      338 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/popnet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10509 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/popnet/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/simulator/utils/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1521 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/simulator/utils/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4728 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/utils/simulation_inputs.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    11771 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/simulator/utils/simulation_reports.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/utils/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1536 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/utils/compile_mechanisms/
--rw-rw-r--   0 kael      (1000) kael      (1000)       66 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/compile_mechanisms/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      884 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/compile_mechanisms/__main__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1030 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/compile_mechanisms/compile_mechanisms.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/utils/create_environment/
--rw-rw-r--   0 kael      (1000) kael      (1000)       50 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/create_environment/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6984 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/create_environment/__main__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4009 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/create_environment/create_environment.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    33814 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/create_environment/env_builder.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      417 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/hdf5_helper.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/utils/io/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1596 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/io/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    16033 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/utils/io/cell_vars.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      951 2022-07-13 17:53:48.000000 bmtk-1.0.7/bmtk/utils/io/firing_rates.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      917 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/io/ioutils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    15112 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/io/spike_trains.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/utils/reports/
--rw-rw-r--   0 kael      (1000) kael      (1000)       80 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.957249 bmtk-1.0.7/bmtk/utils/reports/compartment/
--rw-rw-r--   0 kael      (1000) kael      (1000)       49 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/compartment/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10723 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/utils/reports/compartment/compartment_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1062 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/compartment/compartment_report.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    20559 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/utils/reports/compartment/compartment_writer.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3841 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/compartment/core.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13144 2022-06-14 03:21:44.000000 bmtk-1.0.7/bmtk/utils/reports/compartment/plotting.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6459 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/current_writer.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/reports/spike_trains/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1735 2022-06-14 03:21:34.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3054 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/core.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    16732 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/plotting.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    35580 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_train_buffer.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    26814 2022-05-24 19:01:38.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_train_readers.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13590 2022-06-14 03:21:34.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_trains.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13831 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_trains_api.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6447 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/spikes_file_writers.py
--rw-rw-r--   0 kael      (1000) kael      (1000)       46 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/reports/spike_trains/stats.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/scripts/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/scripts/bionet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)     5738 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3563 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3383 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3348 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3566 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3558 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     2695 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      993 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/default_config.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.937249 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/
--rw-rw-r--   0 kael      (1000) kael      (1000)      704 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1211 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1069 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1005 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      859 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      761 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1161 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1031 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      705 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1394 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      631 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1413 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1267 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     4061 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1170 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      942 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      896 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.961249 bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/
--rw-rw-r--   0 kael      (1000) kael      (1000)    65973 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)    53043 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)    83820 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)    95135 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)   165301 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.965249 bmtk-1.0.7/bmtk/utils/scripts/bionet/point_neuron_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)       68 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_exc_1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       68 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_inh_1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      462 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/run_bionet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.965249 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)       80 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       80 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       84 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       83 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       55 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/instantaneousExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       56 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/synaptic_models/instantaneousInh.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.965249 bmtk-1.0.7/bmtk/utils/scripts/bionet/templates/
--rw-rw-r--   0 kael      (1000) kael      (1000)      437 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/templates/BioAllen_old.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     1035 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      626 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/bionet/templates/Biophys1.hoc
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.965249 bmtk-1.0.7/bmtk/utils/scripts/filternet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.965249 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      547 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/filternet/run_filternet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.965249 bmtk-1.0.7/bmtk/utils/scripts/pointnet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/472363762_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/472912177_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      118 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/473862421_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/473863035_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      118 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/473863510_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_exc_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      117 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_inh_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/point_neuron_models/filter_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      332 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/run_pointnet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/InhToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/InhToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousInh.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/scripts/popnet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/scripts/popnet/population_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      143 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/population_models/exc_model.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      143 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/population_models/inh_model.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      415 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/run_popnet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/InhToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/InhToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        3 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        3 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      545 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/scripts/sonata.circuit_config.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      450 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/scripts/sonata.simulation_config.json
--rw-rw-r--   0 kael      (1000) kael      (1000)    37691 2022-07-23 20:09:44.000000 bmtk-1.0.7/bmtk/utils/sim_setup.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/sonata/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1608 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/sonata/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3971 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/sonata/column_property.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.969249 bmtk-1.0.7/bmtk/utils/sonata/config/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1606 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/config/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4215 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/config/config_schema.json
--rw-rw-r--   0 kael      (1000) kael      (1000)    19237 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/config/sonata_config.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3453 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/sonata/edge.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5537 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/sonata/file.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13856 2019-10-23 23:40:04.000000 bmtk-1.0.7/bmtk/utils/sonata/file_root.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    19742 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/group.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4417 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/node.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    25155 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/population.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9090 2022-04-28 20:49:20.000000 bmtk-1.0.7/bmtk/utils/sonata/types_table.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4257 2022-07-18 16:28:21.000000 bmtk-1.0.7/bmtk/utils/sonata/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2022-10-25 19:35:24.937249 bmtk-1.0.7/bmtk.egg-info/
--rw-rw-r--   0 kael      (1000) kael      (1000)     3215 2022-10-25 19:35:24.000000 bmtk-1.0.7/bmtk.egg-info/PKG-INFO
--rw-rw-r--   0 kael      (1000) kael      (1000)    16172 2022-10-25 19:35:24.000000 bmtk-1.0.7/bmtk.egg-info/SOURCES.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)        1 2022-10-25 19:35:24.000000 bmtk-1.0.7/bmtk.egg-info/dependency_links.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)      174 2022-10-25 19:35:24.000000 bmtk-1.0.7/bmtk.egg-info/requires.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-10-25 19:35:24.000000 bmtk-1.0.7/bmtk.egg-info/top_level.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)      315 2022-10-25 19:35:24.969249 bmtk-1.0.7/setup.cfg
--rw-rw-r--   0 kael      (1000) kael      (1000)     2174 2022-04-28 20:49:20.000000 bmtk-1.0.7/setup.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.485474 bmtk-1.0.8/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1482 2019-10-23 23:40:04.000000 bmtk-1.0.8/LICENSE.txt
+-rw-rw-r--   0 kael      (1000) kael      (1000)      120 2023-06-21 19:55:18.000000 bmtk-1.0.8/MANIFEST.in
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3215 2023-07-02 17:52:21.485474 bmtk-1.0.8/PKG-INFO
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2223 2022-10-25 18:55:38.000000 bmtk-1.0.8/README.md
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.433472 bmtk-1.0.8/bmtk/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1543 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/__init__.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/analyzer/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7931 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/analyzer/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4336 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/cell_vars.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9180 2022-06-14 03:21:44.000000 bmtk-1.0.8/bmtk/analyzer/compartment.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3594 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/ecp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3751 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/firing_rates.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      391 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/io_tools.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17928 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/analyzer/spike_trains.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4787 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/analyzer/spikes_analyzer.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3890 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/analyzer/spikes_loader.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      211 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/analyzer/utils.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1580 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/__init__.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/auxi/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1520 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/builder/auxi/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2515 2020-07-29 19:00:45.000000 bmtk-1.0.8/bmtk/builder/auxi/edge_connectors.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    40569 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/builder/auxi/node_params.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/bionet/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      750 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/builder/bionet/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    19079 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/builder/bionet/swc_reader.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4784 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/builder/builder_utils.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9773 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/connection_map.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1796 2023-04-26 18:17:06.000000 bmtk-1.0.8/bmtk/builder/connector.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3033 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/edge.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/edges_sorter/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      962 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/edges_sorter/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4007 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/edges_sorter/memory_sorter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    27610 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/edges_sorter/merge_sorter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2504 2023-04-26 18:18:24.000000 bmtk-1.0.8/bmtk/builder/functor_cache.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3089 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/id_generator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17456 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/index_builders.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     5336 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/builder/iterator.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.441473 bmtk-1.0.8/bmtk/builder/network_adaptors/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1632 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    19870 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    23846 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network_orig.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    11489 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/edge_props_table.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    21380 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/edges_collator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    32560 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/network.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3057 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/nxnetwork.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    30657 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/network_builder.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      179 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/networks.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3055 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/node.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4202 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/node_pool.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3077 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/builder/node_set.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.441473 bmtk-1.0.8/bmtk/simulator/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1521 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/__init__.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.441473 bmtk-1.0.8/bmtk/simulator/bionet/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      153 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/README.md
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1844 2023-06-21 19:53:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    20932 2023-02-15 16:38:57.000000 bmtk-1.0.8/bmtk/simulator/bionet/biocell.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17281 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/simulator/bionet/bionetwork.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17779 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/biosimulator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3883 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/cell.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2367 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/config.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1606 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17512 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/cell_models.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6112 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synapse_models.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2449 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synaptic_weights.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1036 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)      608 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/Biophys1.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)      239 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/advance.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1110 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/gids.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3125 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/bionet/iclamp.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/import3d/
+-rw-rw-r--   0 kael      (1000) kael      (1000)    28325 2022-01-20 23:00:55.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_gui.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    10086 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_sec.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2038 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_morphml.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    16444 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    27594 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda3.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7697 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nts.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    12318 2022-01-20 23:00:55.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_swc.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)      335 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1905 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/io_tools.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/modules/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1895 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6515 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/comsol.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1434 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/ecephys_module.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    12928 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/ecp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     5867 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/iclamp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    13828 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_cellvars.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4732 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_clamp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9514 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_netcons.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4898 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_spikes.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17767 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/save_synapses.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3356 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/sim_module.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6994 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4012 2023-02-15 16:42:21.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim_waveforms.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    23657 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/morphology.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     5482 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/nml_reader.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3537 2022-08-22 22:07:50.000000 bmtk-1.0.8/bmtk/simulator/bionet/nrn.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6924 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/pointprocesscell.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      371 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/pointsomacell.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1679 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/pyfunction_cache.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/bionet/schemas/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3335 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/config_schema.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      536 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_edge_types.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      170 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_node_types_external.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      347 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_node_types_internal.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      162 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_nodes_external.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      456 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_nodes_internal.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2257 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/seclamp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     8019 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/sonata_adaptors.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4278 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/utils.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3596 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/virtualcell.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/
+-rw-rw-r--   0 kael      (1000) kael      (1000)        0 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      426 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/edge_population.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    15605 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/core/graph.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4666 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/io_tools.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/modules/
+-rw-rw-r--   0 kael      (1000) kael      (1000)        0 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/core/modules/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17106 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/modules/ecephys_module.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6954 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/core/modules/iclamp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3186 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/modules/ndx-aibs-ecephys.extension.yaml
+-rw-rw-r--   0 kael      (1000) kael      (1000)      250 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/modules/ndx-aibs-ecephys.namespace.yaml
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3355 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/core/modules/simulator_module.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1772 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/network_reader.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      886 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/node_population.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1928 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/node_sets.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    13708 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/core/pyfunction_cache.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4610 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/simulation_config.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6008 2022-06-14 03:21:34.000000 bmtk-1.0.8/bmtk/simulator/core/simulation_config_validator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      203 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/simulator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    10605 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/simulator/core/simulator_network.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      159 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7777 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/edge_adaptor.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    10541 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/network_reader.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7783 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/node_adaptor.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/sonata_schemas/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4394 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_schemas/config_schema.json
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.453473 bmtk-1.0.8/bmtk/simulator/filternet/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      234 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1782 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/cell.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)       57 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/cell_models.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      691 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/config.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.453473 bmtk-1.0.8/bmtk/simulator/filternet/default_setters/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       28 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/default_setters/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9248 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/filternet/default_setters/cell_loaders.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2046 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/filternetwork.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      185 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/filters.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7136 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/filternet/filtersimulator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      756 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/io_tools.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.453473 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      195 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/__init__.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/
+-rwxrwxr-x   0 kael      (1000) kael      (1000)    15615 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv
+-rwxrwxr-x   0 kael      (1000) kael      (1000)    12437 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv
+-rwxrwxr-x   0 kael      (1000) kael      (1000)     4186 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv
+-rwxrwxr-x   0 kael      (1000) kael      (1000)     9904 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv
+-rwxrwxr-x   0 kael      (1000) kael      (1000)     1003 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv
+-rwxrwxr-x   0 kael      (1000) kael      (1000)     2783 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6361 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmetrics.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6596 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmodel.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9019 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cursor.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3567 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/fitfuns.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4642 2023-02-15 16:42:21.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/gaborfilter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    16117 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/kernel.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9140 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2111 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2567 2022-05-24 19:01:38.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/linearfilter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3995 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lnunit.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6022 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/make_cell_list.py
+-rwxrwxr-x   0 kael      (1000) kael      (1000)    14892 2023-03-15 21:19:10.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/movie.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2528 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/poissongeneration.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      263 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/singleunitcell.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4618 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/spatialfilter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3730 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/temporalfilter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2268 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/transferfunction.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7390 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/util_fns.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3188 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/utilities.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/filternet/modules/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       81 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      161 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/base.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4678 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/create_spikes.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6390 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/record_rates.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4158 2023-02-15 16:42:21.000000 bmtk-1.0.8/bmtk/simulator/filternet/pyfunction_cache.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9152 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/sonata_adaptors.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)       64 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/transfer_functions.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      150 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/utils.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/pointnet/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1733 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/pointnet/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2208 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/config.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       59 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      471 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/synapse_models.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      441 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/synaptic_weights.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2409 2022-07-14 00:17:59.000000 bmtk-1.0.8/bmtk/simulator/pointnet/gids.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    26368 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/simulator/pointnet/glif_utils.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2820 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/io_tools.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/simulator/pointnet/modules/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      165 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4376 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/ecephys_module.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2210 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/iclamp.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7014 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/multimeter_reporter.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6456 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/record_spikes.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1751 2022-05-24 19:01:38.000000 bmtk-1.0.8/bmtk/simulator/pointnet/nest_utils.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    10782 2023-01-04 15:58:48.000000 bmtk-1.0.8/bmtk/simulator/pointnet/pointnetwork.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    11371 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/pointsimulator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     7611 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/pointnet/property_map.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1616 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/pointnet/pyfunction_cache.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    14299 2023-01-04 15:58:48.000000 bmtk-1.0.8/bmtk/simulator/pointnet/sonata_adaptors.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6528 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/pointnet/utils.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/simulator/popnet/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1622 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/popnet/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1818 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/config.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3583 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popedge.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    17362 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popnetwork.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     5797 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popnode.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    13400 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popsimulator.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      338 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/popnet/sonata_adaptors.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    10509 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/utils.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/simulator/utils/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1521 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/utils/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4728 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/utils/simulation_inputs.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    11838 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/utils/simulation_reports.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/utils/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1576 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/__init__.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/utils/compile_mechanisms/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       66 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/compile_mechanisms/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      884 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/compile_mechanisms/__main__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1030 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/compile_mechanisms/compile_mechanisms.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/utils/create_environment/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       50 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/create_environment/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6984 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/create_environment/__main__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4009 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/create_environment/create_environment.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    33910 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/create_environment/env_builder.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      417 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/hdf5_helper.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/io/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1596 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/io/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    16015 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/io/cell_vars.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      951 2022-07-13 17:53:48.000000 bmtk-1.0.8/bmtk/utils/io/firing_rates.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      917 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/io/ioutils.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    15109 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/io/spike_trains.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)      260 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/lazy_property.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/reports/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       80 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/__init__.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/reports/compartment/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       49 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    10717 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_reader.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1062 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_report.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    21509 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_writer.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3841 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/core.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    13144 2022-10-28 02:04:43.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/plotting.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6450 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/current_writer.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/reports/spike_trains/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1735 2022-06-14 03:21:34.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3054 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/core.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    16732 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/plotting.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    35586 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_buffer.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    26892 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_readers.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    14343 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    14030 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains_api.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     6763 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spikes_file_writers.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)       46 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/stats.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/scripts/
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/scripts/bionet/
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     5738 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3563 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3383 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3348 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3566 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3558 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2695 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      993 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/default_config.json
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.469473 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.433472 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      704 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1211 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1069 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1005 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)      859 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)      761 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1161 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1031 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)      705 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1394 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)      631 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1413 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1267 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4061 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1170 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)      942 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod
+-rw-rw-r--   0 kael      (1000) kael      (1000)      896 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/
+-rw-rw-r--   0 kael      (1000) kael      (1000)    65973 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    53043 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    83820 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc
+-rw-rw-r--   0 kael      (1000) kael      (1000)    95135 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc
+-rw-rw-r--   0 kael      (1000) kael      (1000)   165301 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/point_neuron_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       68 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_exc_1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)       68 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_inh_1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      462 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/run_bionet.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)       80 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)       80 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)       84 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)       83 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)       55 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/instantaneousExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)       56 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/instantaneousInh.json
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      437 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/BioAllen_old.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1035 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc
+-rw-rw-r--   0 kael      (1000) kael      (1000)      626 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/Biophys1.hoc
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/filternet/
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.477473 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      547 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/run_filternet.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.477473 bmtk-1.0.8/bmtk/utils/scripts/pointnet/
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.477473 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/472363762_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/472912177_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      118 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/473862421_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/473863035_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      118 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/473863510_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_exc_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      117 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_inh_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        4 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/filter_point.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      332 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/run_pointnet.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/ExcToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/ExcToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/InhToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/InhToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousInh.json
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/popnet/
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/popnet/population_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)      143 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/population_models/exc_model.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      143 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/population_models/inh_model.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      415 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/run_popnet.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/
+-rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/ExcToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/ExcToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/InhToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/InhToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        3 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToExc.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)        3 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToInh.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      545 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/sonata.circuit_config.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)      450 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/sonata.simulation_config.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)    37691 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/sim_setup.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.485474 bmtk-1.0.8/bmtk/utils/sonata/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1608 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3971 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/column_property.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.485474 bmtk-1.0.8/bmtk/utils/sonata/config/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     1606 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/config/__init__.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4215 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/config/config_schema.json
+-rw-rw-r--   0 kael      (1000) kael      (1000)    19237 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/config/sonata_config.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3453 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/edge.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     5537 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/file.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    13856 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/file_root.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    19742 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/group.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4417 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/node.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)    25155 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/population.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     9090 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/types_table.py
+-rw-rw-r--   0 kael      (1000) kael      (1000)     4257 2022-07-18 16:28:21.000000 bmtk-1.0.8/bmtk/utils/sonata/utils.py
+drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.433472 bmtk-1.0.8/bmtk.egg-info/
+-rw-rw-r--   0 kael      (1000) kael      (1000)     3215 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/PKG-INFO
+-rw-rw-r--   0 kael      (1000) kael      (1000)    16761 2023-07-02 17:52:21.000000 bmtk-1.0.8/bmtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 kael      (1000) kael      (1000)        1 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 kael      (1000) kael      (1000)      181 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/requires.txt
+-rw-rw-r--   0 kael      (1000) kael      (1000)        5 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/top_level.txt
+-rw-rw-r--   0 kael      (1000) kael      (1000)      315 2023-07-02 17:52:21.485474 bmtk-1.0.8/setup.cfg
+-rw-rw-r--   0 kael      (1000) kael      (1000)     2212 2023-01-04 16:03:28.000000 bmtk-1.0.8/setup.py
```

### Comparing `bmtk-1.0.7/LICENSE.txt` & `bmtk-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/PKG-INFO` & `bmtk-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Brain Modeling Toolkit
 Home-page: https://github.com/AllenInstitute/bmtk
 Author: Kael Dai
 Author-email: kaeld@alleninstitute.org
 License: UNKNOWN
 Keywords: neuroscience,scientific,modeling,simulation
 Platform: any
```

### Comparing `bmtk-1.0.7/README.md` & `bmtk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/__init__.py` & `bmtk-1.0.8/bmtk/builder/auxi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,8 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
-__version__ = '1.0.7'
+#
```

### Comparing `bmtk-1.0.7/bmtk/analyzer/__init__.py` & `bmtk-1.0.8/bmtk/analyzer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 
 def spikes_table(config_file, spikes_file=None):
     config = _get_config(config_file)
     spikes_file = config['output']['spikes_file']
     spikes_h5 = h5py.File(spikes_file, 'r')
     gids = np.array(spikes_h5['/spikes/gids'], dtype=np.uint)
-    times = np.array(spikes_h5['/spikes/timestamps'], dtype=np.float)
+    times = np.array(spikes_h5['/spikes/timestamps'], dtype=float)
     return pd.DataFrame(data={'gid': gids, 'spike time (ms)': times})
     #return pd.read_csv(spikes_ascii, names=['time (ms)', 'cell gid'], sep=' ')
 
 
 def nodes_table(nodes_file, population):
     # TODO: Integrate into sonata api
     nodes_h5 = h5py.File(nodes_file, 'r')
```

### Comparing `bmtk-1.0.7/bmtk/analyzer/cell_vars.py` & `bmtk-1.0.8/bmtk/analyzer/cell_vars.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/analyzer/compartment.py` & `bmtk-1.0.8/bmtk/analyzer/compartment.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/analyzer/ecp.py` & `bmtk-1.0.8/bmtk/analyzer/ecp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/analyzer/firing_rates.py` & `bmtk-1.0.8/bmtk/analyzer/firing_rates.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/analyzer/spike_trains.py` & `bmtk-1.0.8/bmtk/analyzer/spike_trains.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         nodes = _find_nodes(population=pop, config=sonata_config, nodes_file=nodes_file,
                             node_types_file=node_types_file)
         grouped_df = None
         for grp in nodes.groups:
             if group_by in grp.all_columns:
                 grp_df = grp.to_dataframe()
                 grp_df = grp_df[['node_id', group_by]]
-                grouped_df = grp_df if grouped_df is None else grouped_df.append(grp_df, ignore_index=True)
+                grouped_df = grp_df if grouped_df is None else pd.concat([grouped_df, grp_df], ignore_index=True)
 
         if grouped_df is None:
             raise ValueError('Could not find any nodes with group_by attribute "{}"'.format(group_by))
 
         # Convert from string to list so we can always use the isin() method for filtering
         if isinstance(group_excludes, string_types):
             group_excludes = [group_excludes]
```

### Comparing `bmtk-1.0.7/bmtk/analyzer/spikes_analyzer.py` & `bmtk-1.0.8/bmtk/analyzer/spikes_analyzer.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/analyzer/spikes_loader.py` & `bmtk-1.0.8/bmtk/analyzer/spikes_loader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/__init__.py` & `bmtk-1.0.8/bmtk/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/auxi/__init__.py` & `bmtk-1.0.8/bmtk/simulator/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
+#
```

### Comparing `bmtk-1.0.7/bmtk/builder/auxi/edge_connectors.py` & `bmtk-1.0.8/bmtk/builder/auxi/edge_connectors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/bionet/__init__.py` & `bmtk-1.0.8/bmtk/builder/bionet/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from .swc_reader import SWCReader
 from .swc_reader import get_swc
 
 
 def rand_syn_locations(src, trg, sections=('soma', 'apical', 'basal'), distance_range=(0.0, 1.0e20),
-                       morphology_dir='./components/morphologies'):
-    trg_swc = get_swc(trg, morphology_dir=morphology_dir, use_cache=True)
+                       morphology_dir='./components/morphologies', return_coords=False, dL=None):
+    trg_swc = get_swc(trg, morphology_dir=morphology_dir, use_cache=True, dL=dL)
 
     sec_ids, seg_xs = trg_swc.choose_sections(sections, distance_range, n_sections=1)
     sec_id, seg_x = sec_ids[0], seg_xs[0]
     swc_id, swc_dist = trg_swc.get_swc_id(sec_id, seg_x)
-    # coords = trg_swc.get_coords(sec_id, seg_x)
 
-    return [sec_id, seg_x, swc_id, swc_dist]  # coords[0], coords[y], coords[z]
+    if return_coords:
+        coords = trg_swc.get_coords(sec_id, seg_x)
+        return [sec_id, seg_x, swc_id, swc_dist, coords[0], coords[1], coords[2]]
+    else:
+        return [sec_id, seg_x, swc_id, swc_dist]
+
```

### Comparing `bmtk-1.0.7/bmtk/builder/bionet/swc_reader.py` & `bmtk-1.0.8/bmtk/builder/bionet/swc_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,20 +55,23 @@
         self._swc_map = None
         self._axon_fixed = False
         self._axon_deleted = False
 
 
     def _copy(self):
         new_swc = SWCReader(swc_path=self.swc_path, rng_seed=self.rng_seed)
+
         if self._axon_fixed:
             new_swc.fix_axon()
 
         if self._axon_deleted:
             new_swc.delete_axon()
 
+
+
         return new_swc
 
     @property
     def sections(self):
         if self._sections is None:
             self._sections = []
             for sec in self.hobj.all:
@@ -286,14 +289,16 @@
 
         self._sections = None
         self._n_sections = None
         self._axon_deleted = True
 
     def set_segment_dl(self, dl):
         """Define number of segments in a cell"""
+        if self._seg_coords is not None:
+            raise RuntimeError('Unable to segment the morphology after coordinates have already been calculated')
         self._nseg = 0
         for sec in self.hobj.all:
             sec.nseg = 1 + 2 * int(sec.L/(2*dl))
             self._nseg += sec.nseg  # get the total number of segments in the cell
 
     def choose_sections(self, section_names, distance_range, n_sections=1):
         """Similar to find_sections, but will only N=n_section number of sections_ids/x values randomly selected (may
@@ -303,15 +308,15 @@
         :param distance_range: [float, float]: distance range of sections from the soma, in um.
         :param n_sections: int: maximum number of sections to select
         :return: [int], [float]: A list of all section_ids and a list of all segment_x values (as defined by NEURON)
             that meet the given critera.
         """
         secs, probs = self.find_sections(section_names, distance_range)
         secs_ix = self._prng.choice(secs, n_sections, p=probs)
-        return secs_ix, self.seg_props.x[secs_ix]
+        return self.seg_props.sec_id[secs_ix], self.seg_props.x[secs_ix]
 
     def find_sections(self, section_names, distance_range):
         """Retrieves a list of sections ids and section x's given a section name/type (eg axon, soma, apic, dend) and
         the distance from the soma.
 
         :param section_names: 'soma', 'dend', 'apic', 'axon'
         :param distance_range: [float, float]: distance range of sections from the soma, in um.
@@ -327,17 +332,18 @@
 
         # Find the fractional overlap between the segment and the distance range:
         # this is done by finding the overlap between [d0,d1] and [dmin,dmax]
         # np.minimum(seg_d1,dmax) find the smaller of the two end locations
         # np.maximum(seg_d0,dmin) find the larger of the two start locations
         # np.maximum(0,overlap) is used to return zero when segments do not overlap
         # and then dividing by the segment length
+
         frac_overlap = np.maximum(0, (np.minimum(seg_d1, dmax) - np.maximum(seg_d0, dmin))) / seg_length
         ix_drange = np.where(frac_overlap > 0)  # find indexes with non-zero overlap
-        ix_labels = np.array([], dtype=np.int)
+        ix_labels = np.array([], dtype=int)
 
         for tar_sec_label in section_names:  # find indexes within sec_labels
             sec_type = self.sec_type_swc[tar_sec_label]  # get swc code for the section label
             ix_label = np.where(seg_type == sec_type)
             ix_labels = np.append(ix_labels, ix_label)  # target segment indexes
 
         tar_seg_ix = np.intersect1d(ix_drange, ix_labels)  # find intersection between indexes for range and labels
@@ -383,22 +389,27 @@
         new_seg_coords = SegmentCoords(p0=new_p0, p1=new_p1, p05=new_p05)
 
         if inplace:
             self._seg_coords = new_seg_coords
             return self
         else:
             new_swc_reader = self._copy()
+            new_swc_reader._seg_props = self.seg_props
+            new_swc_reader._swc_map = self._swc_map
+            new_swc_reader._nseg = self.nseg
             new_swc_reader._seg_coords = new_seg_coords
             new_swc_reader._soma_pos = new_soma_pos
 
             return new_swc_reader
 
     def get_coords(self, sec_id, sec_x):
         segs_indices = np.argwhere(self.seg_props.sec_id == sec_id).flatten()
-        return self.seg_coords.p05[:, segs_indices][:, 0]
+        dev = abs(sec_x - self.seg_props.x[segs_indices])     # Find segment closest to x position
+        idx = np.argmin(dev)
+        return self.seg_coords.p05[:, segs_indices][:, idx]
 
     def get_swc_id(self, sec_id, sec_x):
         # use sec type and nameindex to find all rows in the swc that correspond to sec_id
         sec = self.sections[sec_id]
         sec_nameindex = self._get_sec_nameindex(sec)
         sec_type = self._get_sec_type(sec)
         filtered_swc = self.swc_map[(self.swc_map['type'] == sec_type) & (self.swc_map['nameindex'] == sec_nameindex)]
@@ -428,15 +439,15 @@
         nameindex_str = re.search(r'\[(\d+)\]', sec_type_name).group(1)
         return int(nameindex_str)
 
 
 swc_cache = {}
 
 
-def get_swc(cell, morphology_dir=None, use_cache=False):
+def get_swc(cell, morphology_dir=None, use_cache=False, dL=None):
     cell_pop = cell.get('population', 'default')
     cell_node_id = cell['node_id']
     if use_cache and cell_pop in swc_cache and cell_node_id in swc_cache[cell_pop]:
         return swc_cache[cell_pop][cell_node_id]
 
     swc_path = cell['morphology']
     if morphology_dir:
@@ -445,14 +456,16 @@
     if not os.path.exists(swc_path) and not swc_path.endswith('.swc'):
         swc_path += '.swc'
 
     if not os.path.exists(swc_path):
         raise ValueError('File {} does not exists.'.format(swc_path))
 
     swc = SWCReader(swc_path)
+    if dL:
+        swc.set_segment_dl(dL)
 
     if cell.get('model_processing', 'NULL') == 'aibs_perisomatic':
         swc.fix_axon()
 
     if any([cn in cell for cn in ['x', 'y', 'z']]):
         soma_coords = [cell.get('x', 0.0), cell.get('y', 0.0), cell.get('z', 0.0)]
     else:
```

### Comparing `bmtk-1.0.7/bmtk/builder/builder_utils.py` & `bmtk-1.0.8/bmtk/builder/builder_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 import hashlib
 import logging
-
+import uuid
 
 try:
     from mpi4py import MPI
 
     comm = MPI.COMM_WORLD
     mpi_rank = comm.Get_rank()
     mpi_size = comm.Get_size()
     barrier = comm.barrier
 
 except ImportError:
+    comm = None
     mpi_rank = 0
     mpi_size = 1
     barrier = lambda: None
 
 
 MPI_fail_params_nonuniform = True  # throw exception unless params across MPI ranks are the same.
 logger = logging.getLogger(__name__)
@@ -106,7 +107,38 @@
         if len(set(ranked_vals)) > 1:
             err_msg = '{} property "{}" varies across ranks, please make sure parameter value is uniform across all' \
                       'ranks or set bmtk.builder.MPI_fail_params_nonuniform to False'.format(graph_type, pkey)
             if not MPI_fail_params_nonuniform:
                 logger.warning(err_msg)
             else:
                 raise TypeError(err_msg)
+
+
+__build_time_uuid = None
+
+
+def build_time_uuid():
+    """Produces a unique identifier that will be unique for each time a network building script is executed.
+    """
+    global __build_time_uuid
+    if __build_time_uuid is not None:
+        return __build_time_uuid
+
+    elif comm is not None and mpi_size > 1:
+        barrier()
+        
+        try:
+            if mpi_rank == 0:
+                bcast_data = str(uuid.uuid4().hex)
+            else:
+                bcast_data = None
+
+            bcast_data = comm.bcast(bcast_data, root=0)
+            __build_time_uuid = bcast_data
+        except Exception as e:
+            __build_time_uuid = 'tmp'
+    
+    else:
+        __build_time_uuid = str(uuid.uuid4().hex)
+
+    # __build_time_uuid = str(uuid.uuid4().hex)
+    return __build_time_uuid
```

### Comparing `bmtk-1.0.7/bmtk/builder/connection_map.py` & `bmtk-1.0.8/bmtk/builder/connection_map.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 from . import connector
 from . import iterator
+import numpy as np
+import pandas as pd
 
 
 class ConnectionMap(object):
     """Class for keeping track of connection rules. Used for saving unique edge properties in a network
 
     For every connection from source --> target this keeps track of rules (functions, literals, lists) for
       1. the number of synapses between source and target
@@ -165,15 +167,15 @@
     def properties_keys(self):
         ordered_keys = sorted(self.property_names)
         return str(ordered_keys)
 
     def max_connections(self):
         return len(self._source_nodes) * len(self._target_nodes)
 
-    def add_properties(self, names, rule, rule_params=None, dtypes=None):
+    def add_properties(self, names, rule=None, rule_params=None, values=None, dtypes=None):
         """Add a synaptic property for an individual edge.
 
         Typically this requires a custom rule that will be used for every source/target pair of nodes and returns
         a value for the property. Such rule is a user defined function, and will be called by NetworkBuilder.build()::
 
             def syn_weight_by_loc(source, target):
                 ...
@@ -201,20 +203,42 @@
             cm.add_properties(['syn_weight', 'syn_loc', 'delay'],
                               rule=syn_weight_by_loc,
                               rule_params={'min_weigth':1.0e-7, 'max_weight': 5.0e-6},
                               dtypes=[np.float, str, np.float])
 
         :param names: list, or single string, of the property
         :param rule: function, list or value of property
+        :param values: A list of values to use for property
         :param rule_params: when rule is a function, rule_params will be passed into function when called.
         :param dtypes: expected property type
         """
+        if not (bool(values is not None) != bool(rule is not None)):
+            raise ValueError('Please specify either the "rule" or "values" parameters')
+        
+        if values is not None:
+            rule = values
+
+        if isinstance(rule, list) or isinstance(rule, np.ndarray):
+            rule = ListIterator(rule)
+            rule_params = {}
+
         self._params.append(self.ParamsRules(names, rule, rule_params, dtypes))
         self._param_keys += names
 
     def connection_itr(self):
         """Returns a generator that will iterate through the source/target pairs (as specified by the iterator function,
         and create a connection rule based on the connector.
         """
         conr = connector.create(self.connector, **(self.connector_params or {}))
         itr = iterator.create(self.iterator, conr, **({}))
         return itr(self.source_nodes, self.target_nodes, conr)
+
+
+class ListIterator(object):
+    def __init__(self, my_list):
+        self.my_list = my_list
+        self._idx = 0
+
+    def __call__(self, *args, **kwds):
+        val = self.my_list[self._idx]
+        self._idx += 1
+        return val
```

### Comparing `bmtk-1.0.7/bmtk/builder/connector.py` & `bmtk-1.0.8/bmtk/builder/connector.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/edge.py` & `bmtk-1.0.8/bmtk/builder/edge.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/edges_sorter/memory_sorter.py` & `bmtk-1.0.8/bmtk/builder/edges_sorter/memory_sorter.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             out_grp[in_name].attrs.update(in_h5_obj.attrs)
 
         elif isinstance(in_h5_obj, h5py.Group):
             copy_attributes(in_h5_obj, out_grp[in_name])
 
 
 def quicksort_edges(input_edges_path, output_edges_path, edges_population, sort_by, sort_model_properties=True,
-                    **kwargs):
+                    compression='gzip', **kwargs):
     assert(os.path.exists(input_edges_path))
 
     output_h5 = h5py.File(output_edges_path, 'w')
 
     with h5py.File(input_edges_path, 'r') as input_h5:
         in_pop_grp = input_h5[edges_population]
 
@@ -72,25 +72,25 @@
         sort_order = np.argsort(sort_vals)
         # TODO: Check if already sorted
 
         for col_name in ['source_node_id', 'target_node_id', 'edge_type_id', 'edge_group_id']:
             col_type = in_pop_grp[col_name].dtype
             col_vals = in_pop_grp[col_name][()]
             sorted_col_vals = col_vals[sort_order]
-            out_pop_grp.create_dataset(col_name, data=sorted_col_vals, dtype=col_type)
+            out_pop_grp.create_dataset(col_name, data=sorted_col_vals, dtype=col_type, compression=compression)
 
         sorted_group_indx = in_pop_grp['edge_group_index'][()][sort_order]
         group_index_dtype = in_pop_grp['edge_group_index'].dtype
         group_ids = np.unique(in_pop_grp['edge_group_id'][()])
         for group_id in group_ids:
             out_model_grp = out_pop_grp.create_group(str(group_id))
             model_cols = [n for n, h5_obj in in_pop_grp[str(group_id)].items() if isinstance(h5_obj, h5py.Dataset)]
             group_id_mask = np.argwhere(out_pop_grp['edge_group_id'][()] == group_id).flatten()
             new_index_order = sorted_group_indx[group_id_mask]
             for col_name in model_cols:
                 prop_data = in_pop_grp[str(group_id)][col_name][()][new_index_order]
-                out_model_grp.create_dataset(col_name, data=prop_data)
+                out_model_grp.create_dataset(col_name, data=prop_data, compression=compression)
 
             sorted_group_indx[group_id_mask] = np.arange(0, len(group_id_mask), dtype=group_index_dtype)
 
-        out_pop_grp.create_dataset('edge_group_index', data=sorted_group_indx)
+        out_pop_grp.create_dataset('edge_group_index', data=sorted_group_indx, compression=compression)
         copy_attributes(input_h5['/'], output_h5['/'])
```

### Comparing `bmtk-1.0.7/bmtk/builder/edges_sorter/merge_sorter.py` & `bmtk-1.0.8/bmtk/builder/edges_sorter/merge_sorter.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,33 +124,33 @@
         elif isinstance(in_h5_obj, h5py.Dataset):
             out_grp[in_name].attrs.update(in_h5_obj.attrs)
 
         elif isinstance(in_h5_obj, h5py.Group):
             _copy_attributes(in_h5_obj, out_grp[in_name])
 
 
-def _create_output_h5(input_file, output_file, edges_root, n_edges):
+def _create_output_h5(input_file, output_file, edges_root, n_edges, compression):
     mode = 'r+' if os.path.exists(output_file) else 'w'
     out_h5 = h5py.File(output_file, mode=mode)
     root_grp = out_h5.create_group(edges_root) if edges_root not in out_h5 else out_h5[edges_root]
 
     if 'source_node_id' not in root_grp:
-        root_grp.create_dataset('source_node_id', (n_edges, ), dtype=np.uint32)
+        root_grp.create_dataset('source_node_id', (n_edges, ), dtype=np.uint32, compression=compression)
 
     if 'target_node_id' not in root_grp:
-        root_grp.create_dataset('target_node_id', (n_edges, ), dtype=np.uint32)
+        root_grp.create_dataset('target_node_id', (n_edges, ), dtype=np.uint32, compression=compression)
 
     if 'edge_type_id' not in root_grp:
-        root_grp.create_dataset('edge_type_id', (n_edges, ), dtype=np.uint32)
+        root_grp.create_dataset('edge_type_id', (n_edges, ), dtype=np.uint32, compression=compression)
 
     if 'edge_group_id' not in root_grp:
-        root_grp.create_dataset('edge_group_id', (n_edges, ), dtype=np.uint32)
+        root_grp.create_dataset('edge_group_id', (n_edges, ), dtype=np.uint32, compression=compression)
 
     if 'edge_group_index' not in root_grp:
-        root_grp.create_dataset('edge_group_index', (n_edges, ), dtype=np.uint32)
+        root_grp.create_dataset('edge_group_index', (n_edges, ), dtype=np.uint32, compression=compression)
 
     # with h5py.File(input_file, 'r') as in_h5:
     #     for h5obj in in_h5[edges_root].values():
     #         if isinstance(h5obj, h5py.Group) and h5obj.name not in root_grp:
     #             root_grp.copy(h5obj, h5obj.name)
 
     _copy_attributes(h5py.File(input_file, 'r'), out_h5)
@@ -501,15 +501,15 @@
     chunk_indices = [c for c in chunk_indices if c != -1]
 
     progress.update(chunk_files=chunk_files, chunk_indices=chunk_indices, write_index=write_end_idx,
                     completed=len(chunk_files) == 0)
 
 
 def external_merge_sort(input_edges_path, output_edges_path, edges_population, sort_by, sort_model_properties=True,
-                        n_chunks=12, max_itrs=13, cache_dir='.sort_cache', **kwargs):
+                        n_chunks=12, max_itrs=13, cache_dir='.sort_cache', compression='gzip', **kwargs):
     """Does an external merge sort on an input edges hdf5 file, saves value in new file. Usefull for large network
     files where we are not able to load into memory.
 
     Will split the original hdf5 into <n_chunks> chunks on the disk in cache_dir, Will sort each individual chunk
     of data in memory, then perform a merge on all the chunks. For speed considers may try to do the chunking and
     merging in multiple iterations.
 
@@ -535,15 +535,15 @@
         os.makedirs(cache_dir)
 
     n_chunks = np.min((n_chunks, n_edges))
     progress = ProgressFile(cache_dir=cache_dir, n_edges=n_edges, n_chunks=int(n_chunks), root_name=edges_population,
                             sort_key=sort_by)
 
     output_root_grp = _create_output_h5(input_file=input_edges_path, output_file=output_edges_path,
-                                        edges_root=edges_population, n_edges=n_edges)
+                                        edges_root=edges_population, n_edges=n_edges, compression=compression)
 
     # Split the edges files into N chunks.
     if not progress.initialized or not os.path.exists(cache_dir):
         _initialize_chunks(edges_file_path=input_edges_path, progress=progress)
     else:
         logger.debug('Edges files has already been initialized. Continuing from last saved point')
```

### Comparing `bmtk-1.0.7/bmtk/builder/functor_cache.py` & `bmtk-1.0.8/bmtk/builder/functor_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/id_generator.py` & `bmtk-1.0.8/bmtk/builder/id_generator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/index_builders.py` & `bmtk-1.0.8/bmtk/builder/index_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 def remove_index(edges_file, edges_population):
     with h5py.File(edges_file, mode='r+') as edges_h5:
         edges_pop_grp = edges_h5[edges_population]
         del edges_pop_grp['indices']
 
 
-def create_index_in_memory(edges_file, edges_population, index_type, force_rebuild=True, **kwargs):
+def create_index_in_memory(edges_file, edges_population, index_type, force_rebuild=True, compression='gzip', **kwargs):
     col_to_index, index_grp_name = _get_names(index_type)
 
     with h5py.File(edges_file, mode='r+') as edges_h5:
         edges_pop_grp = edges_h5[edges_population]
 
         if index_grp_name in edges_pop_grp:
             # Remove existing index if it exists
@@ -69,15 +69,15 @@
         r2e_table_df = pd.DataFrame({
             'lu_ids': ids_array[id_idxs],
             'range_beg': ranges_beg,
             'range_end': ranges_end
         }).sort_values('lu_ids')
 
         index_grp.create_dataset('range_to_edge_id', data=r2e_table_df[['range_beg', 'range_end']].values,
-                                 dtype='uint64') # np.uint64)
+                                 dtype='uint64', compression=compression) # np.uint64)
 
         # create a map to the range_to_edge_id dataset from id --> blocks ranges. The id value is implicitly equal to
         # the index
         # TODO: See if del r2e_table_df will significantly improve memory footprint?
         logger.debug('create_index_in_memory> Creating node_id_to_range table')
         ordered_ids = np.array(r2e_table_df['lu_ids'])
         ordered_ids_diffs = np.diff(ordered_ids).nonzero()[0]
@@ -90,15 +90,15 @@
             'range_end': ordered_ids_end
         }).set_index('lu_ids')
 
         # There may be missing values in the id_cols table so fil them in
         i2r_table_df = i2r_table_df.reindex(pd.RangeIndex(i2r_table_df.index.max()+1), fill_value=0)
 
         index_grp.create_dataset('node_id_to_range', data=i2r_table_df[['range_beg', 'range_end']].values,
-                                 dtype=np.uint64)
+                                 dtype=np.uint64, compression=compression)
 
 
 def create_index_on_disk(edges_file, edges_population, index_type, force_rebuild=False, cache_file=None,
                          max_edge_reads=200000000, **kwargs):
     col_to_index, index_grp_name = _get_names(index_type)
     cache_file = cache_file if cache_file is not None else edges_file
```

### Comparing `bmtk-1.0.7/bmtk/builder/iterator.py` & `bmtk-1.0.8/bmtk/builder/iterator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/__init__.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/dm_network.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,19 @@
     def _add_nodes(self, nodes):
         self._nodes.extend(nodes)
         self._nnodes = len(self._nodes)
 
     def edges_table(self):
         return self.__edges_tables
 
-    def _save_nodes(self, nodes_file_name):
+    def _save_nodes(self, nodes_file_name, compression='gzip'):
         if not self._nodes_built:
             self._build_nodes()
+        if compression == 'none':
+            compression = None  # legit option for h5py for no compression
 
         # save the node_types file
         group_indx = 0
         groups_lookup = {}
         group_indicies = {}
         group_props = {}
         for ns in self._node_sets:
@@ -99,28 +101,28 @@
 
         if mpi_rank == 0:
             with h5py.File(nodes_file_name, 'w') as hf:
                 # Add magic and version attribute
                 add_hdf5_attrs(hf)
 
                 pop_grp = hf.create_group('/nodes/{}'.format(self.name))
-                pop_grp.create_dataset('node_id', data=node_gid_table, dtype='uint64')
-                pop_grp.create_dataset('node_type_id', data=node_type_id_table, dtype='uint64')
-                pop_grp.create_dataset('node_group_id', data=node_group_table, dtype='uint32')
-                pop_grp.create_dataset('node_group_index', data=node_group_index_tables, dtype='uint64')
+                pop_grp.create_dataset('node_id', data=node_gid_table, dtype='uint64', compression=compression)
+                pop_grp.create_dataset('node_type_id', data=node_type_id_table, dtype='uint64', compression=compression)
+                pop_grp.create_dataset('node_group_id', data=node_group_table, dtype='uint32', compression=compression)
+                pop_grp.create_dataset('node_group_index', data=node_group_index_tables, dtype='uint64', compression=compression)
 
                 for grp_id, props in group_props.items():
                     model_grp = pop_grp.create_group('{}'.format(grp_id))
 
                     for key, dataset in props.items():
                         try:
-                            model_grp.create_dataset(key, data=dataset)
+                            model_grp.create_dataset(key, data=dataset, compression=compression)
                         except TypeError:
                             str_list = [str(d) for d in dataset]
-                            hf.create_dataset(key, data=str_list)
+                            hf.create_dataset(key, data=str_list, compression=compression)
         barrier()
 
     def nodes_iter(self, node_ids=None):
         if node_ids is not None:
             return [n for n in self._nodes if n.node_id in node_ids]
         else:
             return self._nodes
@@ -213,20 +215,23 @@
         # than the number of actual edges stored (for efficency), may be a better user-representation.
         self._nedges += edges_table.n_syns  # edges_table.n_edges
         self.__edges_tables.append(edges_table)
 
     def _get_edge_group_id(self, params_hash):
         return int(params_hash)
 
-    def _save_gap_junctions(self, gj_file_name):
+    def _save_gap_junctions(self, gj_file_name, compression='gzip'):
         source_ids = []
         target_ids = []
         src_gap_ids = []
         trg_gap_ids = []
 
+        if compression == 'none':
+            compression = None  # legit option for h5py for no compression
+
         for et in self.__edges_tables:
             try:
                 is_gap = et['edge_types']['is_gap_junction']
             except:
                 continue
             if is_gap:
                 if et['source_network'] != et['target_network']:
@@ -242,23 +247,26 @@
                     trg_gap_ids.append(self._gj_id_gen.next())
             else:
                 continue
 
         if len(source_ids) > 0:
             with h5py.File(gj_file_name, 'w') as f:
                 add_hdf5_attrs(f)
-                f.create_dataset('source_ids', data=np.array(source_ids))
-                f.create_dataset('target_ids', data=np.array(target_ids))
-                f.create_dataset('src_gap_ids', data=np.array(src_gap_ids))
-                f.create_dataset('trg_gap_ids', data=np.array(trg_gap_ids))
+                f.create_dataset('source_ids', data=np.array(source_ids), compression=compression)
+                f.create_dataset('target_ids', data=np.array(target_ids), compression=compression)
+                f.create_dataset('src_gap_ids', data=np.array(src_gap_ids), compression=compression)
+                f.create_dataset('trg_gap_ids', data=np.array(trg_gap_ids), compression=compression)
 
     def _save_edges(self, edges_file_name, src_network, trg_network, pop_name=None, sort_by='target_node_id',
-                    index_by=('target_node_id', 'source_node_id')):
+                    index_by=('target_node_id', 'source_node_id'), compression='gzip'):
         barrier()
 
+        if compression == 'none':
+            compression = None  # legit option for h5py for no compression
+
         if mpi_rank == 0:
             logger.debug('Saving {} --> {} edges to {}.'.format(src_network, trg_network, edges_file_name))
 
         filtered_edge_types = [
             # Some edges may not match the source/target population
             et for et in self.__edges_tables
             if et.source_network == src_network and et.target_network == trg_network
@@ -297,28 +305,28 @@
             logger.debug('Saving {} edges to disk'.format(n_total_conns))
             pop_name = '{}_to_{}'.format(src_network, trg_network) if pop_name is None else pop_name
             with h5py.File(edges_file_name, 'w') as hf:
                 # Initialize the hdf5 groups and datasets
                 add_hdf5_attrs(hf)
                 pop_grp = hf.create_group('/edges/{}'.format(pop_name))
 
-                pop_grp.create_dataset('source_node_id', (n_total_conns,), dtype='uint64')
+                pop_grp.create_dataset('source_node_id', (n_total_conns,), dtype='uint64', compression=compression)
                 pop_grp['source_node_id'].attrs['node_population'] = src_network
-                pop_grp.create_dataset('target_node_id', (n_total_conns,), dtype='uint64')
+                pop_grp.create_dataset('target_node_id', (n_total_conns,), dtype='uint64', compression=compression)
                 pop_grp['target_node_id'].attrs['node_population'] = trg_network
-                pop_grp.create_dataset('edge_group_id', (n_total_conns,), dtype='uint16')
-                pop_grp.create_dataset('edge_group_index', (n_total_conns,), dtype='uint32')
-                pop_grp.create_dataset('edge_type_id', (n_total_conns,), dtype='uint32')
+                pop_grp.create_dataset('edge_group_id', (n_total_conns,), dtype='uint16', compression=compression)
+                pop_grp.create_dataset('edge_group_index', (n_total_conns,), dtype='uint32', compression=compression)
+                pop_grp.create_dataset('edge_type_id', (n_total_conns,), dtype='uint32', compression=compression)
 
                 for group_id in merged_edges.group_ids:
                     # different model-groups will have different datasets/properties depending on what edge information
                     # is being saved for each edges
                     model_grp = pop_grp.create_group(str(group_id))
                     for prop_mdata in merged_edges.get_group_metadata(group_id):
-                        model_grp.create_dataset(prop_mdata['name'], shape=prop_mdata['dim'], dtype=prop_mdata['type'])
+                        model_grp.create_dataset(prop_mdata['name'], shape=prop_mdata['dim'], dtype=prop_mdata['type'], compression=compression)
 
                 # Uses the collated edges (eg combined edges across all edge-types) to actually write the data to hdf5,
                 # potentially in multiple chunks. For small networks doing it this way isn't very effiecent, however
                 # this has the benefits:
                 #  * For very large networks it won't always be possible to store all the data in memory.
                 #  * When using MPI/multi-node the chunks can represent data from different ranks.
                 for chunk_id, idx_beg, idx_end in merged_edges.itr_chunks():
@@ -335,14 +343,15 @@
             if sort_on_disk:
                 logger.debug('Sorting {} by {} to {}'.format(edges_file_name, sort_by, edges_file_name_final))
                 sort_edges(
                     input_edges_path=edges_file_name,
                     output_edges_path=edges_file_name_final,
                     edges_population='/edges/{}'.format(pop_name),
                     sort_by=sort_by,
+                    compression=compression,
                     # sort_on_disk=True,
                 )
                 try:
                     logger.debug('Deleting intermediate edges file {}.'.format(edges_file_name))
                     os.remove(edges_file_name)
                 except OSError as e:
                     logger.warning('Unable to remove intermediate edges file {}.'.format(edges_file_name))
@@ -350,15 +359,16 @@
             if index_by:
                 index_by = index_by if isinstance(index_by, (list, tuple)) else [index_by]
                 for index_type in index_by:
                     logger.debug('Creating index {}'.format(index_type))
                     create_index_in_memory(
                         edges_file=edges_file_name_final,
                         edges_population='/edges/{}'.format(pop_name),
-                        index_type=index_type
+                        index_type=index_type,
+                        compression=compression
                     )
 
         barrier()
         del merged_edges
 
         if mpi_rank == 0:
             logger.debug('Saving completed.')
```

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/dm_network_orig.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network_orig.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/edge_props_table.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/edge_props_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 import h5py
 import hashlib
 import logging
 import pandas as pd
 
-from ..builder_utils import mpi_rank, mpi_size, barrier
+from ..builder_utils import mpi_rank, mpi_size, barrier, build_time_uuid
 
 
 logger = logging.getLogger(__name__)
 
 
 class EdgeTypesTableIFace(object):
     @property
@@ -204,15 +204,16 @@
 
     def __init__(self, connection_map, network_name):
         super(EdgeTypesTableMPI, self).__init__(connection_map, network_name)
         self.tmp_table_name = EdgeTypesTableMPI.get_tmp_table_path(mpi_rank)
 
     @staticmethod
     def get_tmp_table_path(rank=0, name=None):
-        return '.edge_types_table.{}.h5'.format(rank)
+        builder_uuid = build_time_uuid()
+        return '.edge_types_table.{}.{}.h5'.format(rank, builder_uuid)
 
     def _open_tmp_table(self):
         if EdgeTypesTableMPI._tmp_table_handle is None:
             EdgeTypesTableMPI._tmp_table_handle = h5py.File(self.tmp_table_name, 'w')
 
         return EdgeTypesTableMPI._tmp_table_handle
```

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/edges_collator.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/edges_collator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import logging
 import h5py
 
-from ..builder_utils import mpi_rank, mpi_size, barrier
+from ..builder_utils import mpi_rank, mpi_size, barrier, build_time_uuid
 from .edge_props_table import EdgeTypesTableMPI
 
 
 logger = logging.getLogger(__name__)
 
 
 class EdgesCollatorSingular(object):
@@ -204,14 +204,19 @@
         self._model_groups_md = {}  # keep track of all the edge-types metdata/properties across all ranks
         self._group_ids = set()  # keep track of all group_ids
         self._group_offsets = {}
         self._proc_fhandles = {}  # reference to open readable hdf5 handles.
 
         self.can_sort = False
 
+    @staticmethod
+    def get_tmp_table_path(rank=0, name=None):
+        builder_uuid = build_time_uuid()
+        return '.edge_types_table.processed.{}.{}.h5'.format(rank, builder_uuid)
+
     def process(self):
         barrier()
 
         # Iterate through all the temp hdf5 edge-type files on the disk and gather information about all the
         # different edge-types and their properties.
         # NOTE: Assumes that each .edge_type_table*h5 file contains unique edge_type_ids
         for rank in range(mpi_size):
@@ -300,15 +305,16 @@
         else:
             # It is possible a .edge_types_table.<rank>.h5 file doesn't exist because there are no edges on that rank.
             # As such hack together a fake hdf5 format with /unprocessed/network_name/ path but no data.
             unprocessed_h5 = {
                 'unprocessed': {self._network_name: {}}
             }
 
-        with h5py.File('.edge_types_table.processed.{}.h5'.format(mpi_rank), 'w') as local_h5:
+        # with h5py.File('.edge_types_table.processed.{}.h5'.format(mpi_rank), 'w') as local_h5:
+        with h5py.File(EdgesCollatorMPI.get_tmp_table_path(mpi_rank), 'w') as local_h5:
             # WARNING: Trying to process the data back into the .edge_types_table*h5 being read from will randomly cause
             #          resource unavailble errors.
             local_grp_sizes = {}  # count the size of each property model group for all edge-types on this rank
             for edge_id, edge_grp in unprocessed_h5['unprocessed'][self._network_name].items():
                 group_id = self._model_groups_md[int(edge_id)]['edge_group_id']
                 if group_id not in local_grp_sizes:
                     local_grp_sizes[group_id] = 0
@@ -392,15 +398,15 @@
 
         for rank_id in range(mpi_size):
             idx_end = idx_beg + self._edges_by_rank[rank_id]
             yield rank_id, idx_beg, idx_end
             idx_beg = idx_end
 
     def _get_processed_h5(self, rank):
-        h5_path = '.edge_types_table.processed.{}.h5'.format(rank)
+        h5_path = EdgesCollatorMPI.get_tmp_table_path(rank=rank) #  '.edge_types_table.processed.{}.h5'.format(rank)
         if h5_path in self._proc_fhandles:
             return self._proc_fhandles[h5_path]
         else:
             h5_handle = h5py.File(h5_path, 'r')
             self._proc_fhandles[h5_path] = h5_handle
             return h5_handle
 
@@ -441,21 +447,21 @@
 
     def get_group_property(self, prop_name, group_id, chunk_id):
         rank_h5 = self._get_processed_h5(rank=chunk_id)
         return rank_h5['processed'][str(group_id)][prop_name][()]
 
     def __del__(self):
         # clean up .h5 file that is saved to disk
-        tmp_h5_path = '.edge_types_table.processed.{}.h5'.format(mpi_rank)
+        tmp_h5_path = EdgesCollatorMPI.get_tmp_table_path(mpi_rank) # '.edge_types_table.processed.{}.h5'.format(mpi_rank)
         try:
             if os.path.exists(tmp_h5_path):
                 os.remove(tmp_h5_path)
         except (FileNotFoundError, IOError, Exception) as e:
             logger.warning('Unable to delete temp edges file {}.'.format(tmp_h5_path))
 
-
+            
 class EdgesCollator(object):
     def __new__(cls, *args, **kwargs):
         if mpi_size > 1:
             return EdgesCollatorMPI(*args, **kwargs)
         else:
             return EdgesCollatorSingular(*args, **kwargs)
```

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/network.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,27 +542,27 @@
             fname = '{}_{}'.format(self.name, ftype)
             return os.path.join(path_dir, fname)
         elif os.path.isabs(filename):
             return filename
         else:
             return os.path.join(path_dir, filename)
 
-    def save(self, output_dir='.', force_overwrite=True):
+    def save(self, output_dir='.', force_overwrite=True, compression='gzip'):
         """Used to save the network files in the appropriate (eg SONATA) format into the output_dir directory. The file
         names will be automatically generated based on the network names.
 
         To have more control over the output and file names use the **save_nodes()** and **save_edges()** methods.
 
         :param output_dir: string, directory where network files will be generated. Default, current working directory.
         :param force_overwrite: Overwrites existing network files.
         """
-        self.save_nodes(output_dir=output_dir, force_overwrite=force_overwrite)
-        self.save_edges(output_dir=output_dir, force_overwrite=force_overwrite)
+        self.save_nodes(output_dir=output_dir, force_overwrite=force_overwrite, compression=compression)
+        self.save_edges(output_dir=output_dir, force_overwrite=force_overwrite, compression=compression)
 
-    def save_nodes(self, nodes_file_name=None, node_types_file_name=None, output_dir='.', force_overwrite=True):
+    def save_nodes(self, nodes_file_name=None, node_types_file_name=None, output_dir='.', force_overwrite=True, compression='gzip'):
         """Save the instantiated nodes in SONATA format files.
 
         :param nodes_file_name: file-name of hdf5 nodes file. By default will use <network.name>_nodes.h5.
         :param node_types_file_name: file-name of the csv node-types file. By default will use
             <network.name>_node_types.csv
         :param output_dir: Directory where network files will be generated. Default, current working directory.
         :param force_overwrite: Overwrites existing network files.
@@ -579,18 +579,18 @@
         if not force_overwrite and os.path.exists(node_types_file):
             raise Exception('File {} exists. Please use different name or use force_overwrite'.format(node_types_file))
         ntf_dir = os.path.dirname(node_types_file)
         if not os.path.exists(ntf_dir) and mpi_rank == 0:
             os.makedirs(ntf_dir)
         barrier()
 
-        self._save_nodes(nodes_file)
+        self._save_nodes(nodes_file, compression=compression)
         self._save_node_types(node_types_file)
 
-    def _save_nodes(self, nodes_file_name):
+    def _save_nodes(self, nodes_file_name, compression='gzip'):
         raise NotImplementedError
 
     def _save_node_types(self, node_types_file_name):
         if mpi_rank == 0:
             logger.debug('Saving {} node-types to {}.'.format(self.name, node_types_file_name))
 
             node_types_cols = ['node_type_id'] + [col for col in self._node_types_columns if col != 'node_type_id']
@@ -601,15 +601,15 @@
                     csvw.writerow([node_type.get(cname, 'NULL') for cname in node_types_cols])
         barrier()
 
     def import_nodes(self, nodes_file_name, node_types_file_name):
         raise NotImplementedError
 
     def save_edges(self, edges_file_name=None, edge_types_file_name=None, output_dir='.', src_network=None,
-                   trg_network=None, name=None, force_build=True, force_overwrite=False):
+                   trg_network=None, name=None, force_build=True, force_overwrite=False, compression='gzip'):
         """Save the instantiated edges in SONATA format files.
 
         :param edges_file_name: file-name of hdf5 edges file. By default will use <src_network>_<trg_network>_edges.h5.
         :param edge_types_file_name: file-name of csv edge-types file. By default will use
             <src_network>_<trg_network>_edges.h5.
         :param output_dir: Directory where network files will be generated. Default, current working directory.
         :param src_network: Name of the source-node populations.
@@ -644,22 +644,22 @@
         if (edges_file_name or edge_types_file_name) is not None:
             network_params = [(network_params[0][0], network_params[0][1], edges_file_name, edge_types_file_name)]
 
         if not os.path.exists(output_dir) and mpi_rank == 0:
             os.mkdir(output_dir)
         barrier()
 
-        self._save_gap_junctions(os.path.join(output_dir, self._network_name + '_gap_juncs.h5'))
+        self._save_gap_junctions(os.path.join(output_dir, self._network_name + '_gap_juncs.h5'), compression=compression)
 
         for p in network_params:
             if p[3] is not None:
                 self._save_edge_types(os.path.join(output_dir, p[3]), p[0], p[1])
 
             if p[2] is not None:
-                self._save_edges(os.path.join(output_dir, p[2]), p[0], p[1], name)
+                self._save_edges(os.path.join(output_dir, p[2]), p[0], p[1], name, compression=compression)
 
     def _save_edge_types(self, edge_types_file_name, src_network, trg_network):
         if mpi_rank == 0:
             # Get edge-type properties for connections with matching source/target networks
             matching_et = [c.edge_type_properties for c in self._connection_maps
                            if c.source_network_name == src_network and c.target_network_name == trg_network]
```

### Comparing `bmtk-1.0.7/bmtk/builder/network_adaptors/nxnetwork.py` & `bmtk-1.0.8/bmtk/builder/network_adaptors/nxnetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/network_builder.py` & `bmtk-1.0.8/bmtk/builder/network_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,19 +100,19 @@
     @property
     def nedges(self):
         """Returns the total number of edges for this network."""
         return self.adaptor.nedges
 
     def add_nodes(self, N=1, **properties):
         """Used to add nodes (eg cells) to a network. User should specify the number of Nodes (N) and can use any
-        properties/attributes they require to define the nodes. By default all individual cells will be assigned a
+        properties/attributes they require to define the nodes. By default, all individual cells will be assigned a
         unique 'node_id' to identify each node in the network and a 'node_type_id' to identify each group of nodes.
 
-        If a property is a singluar value then said property will be shared by all the nodes in the group. If a value
-        is a list of length N then each property will be uniquly assigned the each node. In the below example a group
+        If a property is a singular value then said property will be shared by all the nodes in the group. If a value
+        is a list of length N then each property will be uniquely assigned to each node. In the below example a group
         of 100 nodes is created, all share the same 'model_type' parameter but the pos_x values will be different for
         each node::
 
             net.add_nodes(N=100, pos_x=np.random.rand(100), model_type='intfire1', ...)
 
         You can use a tuple to store property values (in which the SONATA hdf5 will save it as a dataset with multiple
         columns). For example to have one property 'positions' which keeps track of the x/y/z coordinates of each cell::
@@ -279,64 +279,72 @@
         """Builds nodes and edges.
 
         :param force: set true to force complete rebuilding of nodes and edges, if nodes() or save_nodes() has been
             called before then forcing a rebuild may change gids of each node.
         """
         self.adaptor.build(force=force)
 
-    def save(self, output_dir='.', force_overwrite=True):
+    def save(self, output_dir='.', force_overwrite=True, compression='gzip'):
         """Used to save the network files in the appropriate (eg SONATA) format into the output_dir directory. The file
         names will be automatically generated based on the network names.
 
         To have more control over the output and file names use the **save_nodes()** and **save_edges()** methods.
 
         :param output_dir: string, directory where network files will be generated. Default, current working directory.
         :param force_overwrite: Overwrites existing network files.
+        :param compression: Compression algorithm used to save hdf5 files. 'gzip' (default), 'lzf', 'none', or None.
+            you can also specify an integer (1-9) to specify the level of gzip compression.
         """
-        self.adaptor.save(output_dir=output_dir, force_overwrite=force_overwrite)
+        self.adaptor.save(output_dir=output_dir, force_overwrite=force_overwrite, compression=compression)
 
-    def save_nodes(self, nodes_file_name=None, node_types_file_name=None, output_dir='.', force_overwrite=True):
+    def save_nodes(self, nodes_file_name=None, node_types_file_name=None, output_dir='.', force_overwrite=True, compression='gzip'):
         """Save the instantiated nodes in SONATA format files.
 
         :param nodes_file_name: file-name of hdf5 nodes file. By default will use <network.name>_nodes.h5.
         :param node_types_file_name: file-name of the csv node-types file. By default will use
             <network.name>_node_types.csv
         :param output_dir: Directory where network files will be generated. Default, current working directory.
         :param force_overwrite: Overwrites existing network files.
+        :param compression: Compression algorithm used to save hdf5 files. 'gzip' (default), 'lzf', 'none', or None.
+            you can also specify an integer (1-9) to specify the level of gzip compression.
         """
         self.adaptor.save_nodes(
             nodes_file_name=nodes_file_name,
             node_types_file_name=node_types_file_name,
             output_dir=output_dir,
-            force_overwrite=force_overwrite
+            force_overwrite=force_overwrite,
+            compression=compression,
         )
 
     def save_edges(self, edges_file_name=None, edge_types_file_name=None, output_dir='.', src_network=None,
-                   trg_network=None, name=None, force_build=True, force_overwrite=False):
+                   trg_network=None, name=None, force_build=True, force_overwrite=False, compression='gzip'):
         """Save the instantiated edges in SONATA format files.
 
         :param edges_file_name: file-name of hdf5 edges file. By default will use <src_network>_<trg_network>_edges.h5.
         :param edge_types_file_name: file-name of csv edge-types file. By default will use
             <src_network>_<trg_network>_edges.h5.
         :param output_dir: Directory where network files will be generated. Default, current working directory.
         :param src_network: Name of the source-node populations.
         :param trg_network: Name of the target-node populations.
         :param name: Name of edge populations, eg /edges/<name> in edges.h5 file.
         :param force_build: Force to (re)build the connection matrix if it hasn't already been built.
         :param force_overwrite: Overwrites existing network files.
+        :param compression: Compression algorithm used to save hdf5 files. 'gzip' (default), 'lzf', 'none', or None.
+            you can also specify an integer (1-9) to specify the level of gzip compression.
         """
         self.adaptor.save_edges(
             edges_file_name=edges_file_name,
             edge_types_file_name=edge_types_file_name,
             output_dir=output_dir,
             src_network=src_network,
             trg_network=trg_network,
             name=name,
             force_build=force_build,
-            force_overwrite=force_overwrite
+            force_overwrite=force_overwrite,
+            compression=compression,
         )
 
     def import_nodes(self, nodes_file_name, node_types_file_name):
         """Import nodes from an existing sonata file
 
         :param nodes_file_name:
         :param node_types_file_name:
```

### Comparing `bmtk-1.0.7/bmtk/builder/node.py` & `bmtk-1.0.8/bmtk/builder/node.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/node_pool.py` & `bmtk-1.0.8/bmtk/builder/node_pool.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/builder/node_set.py` & `bmtk-1.0.8/bmtk/builder/node_set.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/__init__.py` & `bmtk-1.0.8/bmtk/simulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/__init__.py` & `bmtk-1.0.8/bmtk/simulator/bionet/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/biocell.py` & `bmtk-1.0.8/bmtk/simulator/bionet/biocell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/bionetwork.py` & `bmtk-1.0.8/bmtk/simulator/bionet/bionetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/biosimulator.py` & `bmtk-1.0.8/bmtk/simulator/bionet/morphology.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017. Allen Institute. All rights reserved
+# Copyright 2022. Allen Institute. All rights reserved
 #
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
 # following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
 # disclaimer.
 #
@@ -16,553 +16,526 @@
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-import time
-from six import string_types
+import re
+from collections import namedtuple
+import warnings
+import numpy as np
+import pandas as pd
 from neuron import h
-from bmtk.simulator.core.simulator import Simulator
-from bmtk.simulator.bionet.io_tools import io
-from bmtk.simulator.bionet.iclamp import IClamp, FileIClamp
-from bmtk.simulator.bionet.seclamp import SEClamp
-from bmtk.simulator.bionet import modules as mods
-from bmtk.simulator.core.node_sets import NodeSet
-import bmtk.simulator.utils.simulation_reports as reports
-import bmtk.simulator.utils.simulation_inputs as inputs
-from bmtk.utils.reports.spike_trains import SpikeTrains
-import h5py
-
-
-pc = h.ParallelContext()    # object to access MPI methods
-
-
-class BioSimulator(Simulator):
-    """Includes methods to run and control the simulation"""
-
-    def __init__(self, network, dt, tstop, v_init, celsius, nsteps_block, start_from_state=False):
-        self.net = network
-
-        self._start_from_state = start_from_state
-        self.dt = dt
-        self.tstop = tstop
-        self.tstart = 0.0
-
-        self._v_init = v_init
-        self._celsius = celsius
-        self._h = h
-
-        self.tstep = int(round(h.t / h.dt))
-        self.tstep_start_block = self.tstep
-        self.nsteps = int(round(h.tstop/h.dt))
-
-        # make sure the block size isn't small than the total number of steps
-        # TODO: should we send a warning that block-step size is being reset?
-        self._nsteps_block = nsteps_block if self.nsteps > nsteps_block else self.nsteps
 
-        self.__tstep_end_block = 0
-        self.__tstep_start_block = 0
-
-        h.runStopAt = h.tstop
-        h.steps_per_ms = 1/h.dt
-        pc.setup_transfer()#Sets up gap junctions.
-        self._set_init_conditions()  # call to save state
-        h.cvode.cache_efficient(1)
-               
-        h.pysim = self  # use this objref to be able to call postFadvance from proc advance in advance.hoc
-        self._iclamps = []
-        self._f_iclamps = []
-        self._seclamps = []
-
-        self._output_dir = 'output'
-        self._log_file = 'output/log.txt'
-
-        self._spikes = {}  # for keeping track of different spike times, key of cell gids
-
-        self._cell_variables = []  # location of saved cell variables
-        self._cell_vars_dir = 'output/cellvars'
-
-        self._sim_mods = []  # list of modules.SimulatorMod's
-
-    @property
-    def dt(self):
-        return h.dt
-
-    @dt.setter
-    def dt(self, ms):
-        h.dt = ms
-
-    @property
-    def tstop(self):
-        return h.tstop
-
-    @tstop.setter
-    def tstop(self, ms):
-        h.tstop = ms
-
-    @property
-    def v_init(self):
-        return self._v_init
-
-    @v_init.setter
-    def v_init(self, voltage):
-        self._v_init = voltage
-
-    @property
-    def celsius(self):
-        return self._celsius
-
-    @celsius.setter
-    def celsius(self, c):
-        self._celsius = c
-
-    @property
-    def n_steps(self):
-        return int(round(self.tstop/self.dt))
-
-    @property
-    def cell_variables(self):
-        return self._cell_variables
-
-    @property
-    def cell_var_output(self):
-        return self._cell_vars_dir
-
-    @property
-    def spikes_table(self):
-        return self._spikes
-
-    @property
-    def nsteps_block(self):
-        return self._nsteps_block
-
-    @property
-    def h(self):
-        return self._h
-
-    @property
-    def biophysical_gids(self):
-        return self.net.cell_type_maps('biophysical').keys()
-
-    @property
-    def local_gids(self):
-        # return self.net.get
-        return self.net.local_gids
-
-    def simulation_time(self, units='ms'):
-        units_lc = units.lower()
-        time_ms = self.tstop - self.tstart
-        if units_lc == 'ms':
-            return time_ms
-        elif units_lc == 's':
-            return time_ms/1000.0
-
-        else:
-            raise AttributeError('Uknown unit type {}'.format(units))
+from bmtk.simulator.bionet.io_tools import io
 
-    def __elapsed_time(self, time_s):
-        if time_s < 120:
-            return '{:.4} seconds'.format(time_s)
-        elif time_s < 7200:
-            mins, secs = divmod(time_s, 60)
-            return '{} minutes, {:.4} seconds'.format(mins, secs)
-        else:
-            mins, secs = divmod(time_s, 60)
-            hours, mins = divmod(mins, 60)
-            return '{} hours, {} minutes and {:.4} seconds'.format(hours, mins, secs)
-
-    def _set_init_conditions(self):
-        """Set up the initial conditions: either read from the h.SaveState or from config["condidtions"]"""
-        pc.set_maxstep(10)
-        h.stdinit()
-        self.tstep = int(round(h.t/h.dt))
-        self.tstep_start_block = self.tstep
-
-        if self._start_from_state:
-            # io.read_state()
-            io.log_info('Read the initial state saved at t_sim: {} ms'.format(h.t))
-        else:
-            h.v_init = self.v_init
 
-        h.celsius = self.celsius
-                
-    def set_spikes_recording(self):
-        for gid, _ in self.net.get_local_cells().items():
-            tvec = self.h.Vector()
-            gidvec = self.h.Vector()
-            pc.spike_record(gid, tvec, gidvec)
-            self._spikes[gid] = tvec
-
-    def attach_current_clamp(self, amplitude, delay, duration, gids=None, section_name='soma', section_index=0,
-                             section_dist=0.5):
-        # TODO: Create appropiate module
-        if gids is None or gids=='all':
-            gids = self.biophysical_gids
-
-        if isinstance(gids, int):
-            gids = [gids]
-        elif isinstance(gids, string_types):
-            gids = [int(gids)]
-        elif isinstance(gids, NodeSet):
-            gids = gids.gids()
-
-        gids = list(set(self.local_gids) & set(gids))
-        n_gids = len(gids)
-        
-        if len(gids) != len(amplitude):
-            amplitude = amplitude * n_gids  # len(gids)
-
-        if len(gids) != len(delay):
-            delay = delay * n_gids
-            duration = duration * n_gids
-
-        for idx, gid in enumerate(gids):
-            cell = self.net.get_cell_gid(gid)
-            Ic = IClamp(amplitude[idx], delay[idx], duration[idx], section_name, section_index, section_dist)
-            
-            Ic.attach_current(cell)
-            self._iclamps.append(Ic)
+pc = h.ParallelContext()  # object to access MPI methods
 
-    def attach_file_current_clamp(self, input_file):
-        file = h5py.File(input_file,'r')
 
-        if "gids" not in list(file.keys()) or file["gids"].value == 'all':
-            gids = self.biophysical_gids
+class _LazySegmentProps(object):
+    """A Struct for storing coordinate invariant properties of each segment of a cell."""
+    def __init__(self, hobj):
+        self._hobj = hobj
+        self.sec_id = None
+        self.type = None
+        self.area = None
+        self.x = None
+        self.x0 = None
+        self.x1 = None
+        self.dist = None
+        self.length = None
+        self.dist0 = None
+        self.dist1 = None
+
+    def get(self):
+        if self.sec_id is None:
+            seg_type = []
+            seg_area = []
+            seg_x = []
+            seg_x0 = []
+            seg_x1 = []
+            seg_dist = []
+            seg_length = []
+            seg_sec_id = []
+
+            h.distance(sec=self._hobj.soma[0])  # measure distance relative to the soma
+
+            for sec_id, sec in enumerate(self._hobj.all):
+                fullsecname = sec.name()
+                sec_type = fullsecname.split(".")[1][:4]  # get sec name type without the cell name
+                sec_type_swc = Morphology.sec_type_swc[sec_type]  # convert to swc code
+                x_range = 1.0 / (sec.nseg * 2)  # used to calculate [x0, x1]
+
+                for seg in sec:
+                    seg_area.append(h.area(seg.x))
+                    seg_x.append(seg.x)
+                    seg_x0.append(seg.x - x_range)
+                    seg_x1.append(seg.x + x_range)
+                    seg_length.append(sec.L / sec.nseg)
+                    seg_type.append(sec_type_swc)  # record section type in a list
+                    # seg_dist.append(h.distance(seg.x))  # distance to the center of the segment
+                    seg_dist.append(h.distance(seg))
+                    seg_sec_id.append(sec_id)
+
+            length_arr = np.array(seg_length)
+            dist_arr = np.array(seg_dist)
+            dist0_arr = dist_arr - length_arr / 2.0
+            dist1_arr = dist_arr + length_arr / 2.0
+
+            self.type = np.array(seg_type)
+            self.area = np.array(seg_area)
+            self.x = np.array(seg_x)
+            self.x0 = np.array(seg_x0)
+            self.x1 = np.array(seg_x1)
+            self.dist = dist_arr
+            self.length = length_arr
+            self.dist0 = dist0_arr
+            self.dist1 = dist1_arr
+            self.sec_id = np.array(seg_sec_id)
+
+        return self
+
+
+class _LazySegmentCoords(object):
+    """A Struct for storing properties of each segment of a cell that vary by soma position and rotation."""
+    def __init__(self, hobj):
+        self._hobj = hobj
+        self.p0 = None
+        self.p1 = None
+        self.p05 = None
+        self.soma_pos = None
+        self.d = None
+
+    def get(self):
+        if self.p0 is None:
+            # Iterates through each segment (one section may contain one or more segments). We use NEURON's
+            # segment.x to get the mid-point and lenght of each segment we we can use to find and store the beginning
+            # (p0) and end (p1) of each segment. We also shift so the middle of the soma is at the origin.
+            nseg = np.sum([s.nseg for s in self._hobj.all])
+
+            n3dsoma = 0
+            soma_pos = np.zeros(3)
+            for sec in self._hobj.soma:
+                n3d = int(h.n3d(sec=sec))  # get number of n3d points in each section
+                n3dsoma += n3d
+                for i in range(n3d):
+                    soma_pos[0] += h.x3d(i, sec=sec)
+                    soma_pos[1] += h.y3d(i, sec=sec)
+                    soma_pos[2] += h.z3d(i, sec=sec)
+
+            soma_pos /= n3dsoma
+
+            ix = 0  # segment index
+            self.p0 = np.zeros((3, nseg))  # hold the coordinates of segment starting points
+            self.p1 = np.zeros((3, nseg))  # hold the coordinates of segment end points
+            self.p05 = np.zeros((3, nseg))
+            for sec in self._hobj.all:
+                n3d = int(h.n3d(sec=sec))  # get number of n3d points in each section
+                p3d = np.zeros((3, n3d))  # to hold locations of 3D morphology for the current section
+                l3d = np.zeros(n3d)  # to hold locations of 3D morphology for the current section
+                # diam3d = np.zeros(n3d)  # to diameters, at the moment we don't need to keep track of diameter
+
+                for i in range(n3d):
+                    p3d[0, i] = h.x3d(i, sec=sec) - soma_pos[0]  # shift coordinates such to place soma at the origin.
+                    p3d[1, i] = h.y3d(i, sec=sec) - soma_pos[1]
+                    p3d[2, i] = h.z3d(i, sec=sec) - soma_pos[2]
+                    # diam3d[i] = h.diam3d(i, sec=sec)
+                    l3d[i] = h.arc3d(i, sec=sec)
+
+                l3d /= sec.L  # normalize
+                nseg = sec.nseg
+
+                l0 = np.zeros(nseg)  # keep range of segment starting point
+                l1 = np.zeros(nseg)  # keep range of segment ending point
+                l05 = np.zeros(nseg)
+
+                for iseg, seg in enumerate(sec):
+                    l0[iseg] = seg.x - 0.5 * 1 / nseg  # x (normalized distance along the section) for the beginning of the segment
+                    l1[iseg] = seg.x + 0.5 * 1 / nseg  # x for the end of the segment
+                    l05[iseg] = seg.x
+
+                self.p0[0, ix:ix + nseg] = np.interp(l0, l3d, p3d[0, :])
+                self.p0[1, ix:ix + nseg] = np.interp(l0, l3d, p3d[1, :])
+                self.p0[2, ix:ix + nseg] = np.interp(l0, l3d, p3d[2, :])
+
+                self.p1[0, ix:ix + nseg] = np.interp(l1, l3d, p3d[0, :])
+                self.p1[1, ix:ix + nseg] = np.interp(l1, l3d, p3d[1, :])
+                self.p1[2, ix:ix + nseg] = np.interp(l1, l3d, p3d[2, :])
+
+                self.p05[0, ix:ix + nseg] = np.interp(l05, l3d, p3d[0, :])
+                self.p05[1, ix:ix + nseg] = np.interp(l05, l3d, p3d[1, :])
+                self.p05[2, ix:ix + nseg] = np.interp(l05, l3d, p3d[2, :])
+
+                # x0[ix:ix + nseg] = l0
+                # x1[ix:ix + nseg] = l1
+
+                ix += nseg
+
+            # TODO: keep track of diameter only when minimum_distance='auto' in EcpMod
+            self.d = np.array([seg.diam for sec in self._hobj.all for seg in sec])
+
+            # Also calculate the middle of the shifted soma, NOTE: in theory this should be (0, 0, 0), but due to
+            # percision the actual soma center might be a little off.
+            n3dsoma = 0
+            r3dsoma = np.zeros(3)
+            for sec in self._hobj.soma:
+                n3d = int(h.n3d(sec=sec))  # get number of n3d points in each section
+                n3dsoma += n3d
+                for i in range(n3d):
+                    r3dsoma[0] += h.x3d(i, sec=sec) - soma_pos[0]
+                    r3dsoma[1] += h.y3d(i, sec=sec) - soma_pos[1]
+                    r3dsoma[2] += h.z3d(i, sec=sec) - soma_pos[2]
+
+            r3dsoma /= n3dsoma
+            self.soma_pos = r3dsoma
+
+        return self
+
+
+# For a lot of different cells created from the same morphology and model_processing function, the core segment
+# properties will be the same (even if coordinates, synapses, hobjs, etc. are different). In such cases we want
+# to calculate and store seg_props only once for all equivelent cells. We can do this by caching the seg_props
+# helper function pointer, then all equivelent morphologies (as defined by __hash__ function) use the same
+# SegmentProps object
+morphology_cache = {}
+
+
+def rotation_matrix(axis, theta):
+    """Return the rotation matrix associated with counterclockwise rotation about the given axis by theta radians.
+    """
+    axis = np.asarray(axis)
+    theta = np.asarray(theta)
+    axis = axis/np.sqrt(np.dot(axis, axis))
+    a = np.cos(theta/2.0)
+    b, c, d = -axis*np.sin(theta/2.0)
+    aa, bb, cc, dd = a*a, b*b, c*c, d*d
+    bc, ad, ac, ab, bd, cd = b*c, a*d, a*c, a*b, b*d, c*d
+
+    return np.array([
+        [aa+bb-cc-dd, 2*(bc+ad), 2*(bd-ac)],
+        [2*(bc-ad), aa+cc-bb-dd, 2*(cd+ab)],
+        [2*(bd+ac), 2*(cd-ab), aa+dd-bb-cc]
+    ])
+
+
+class Morphology(object):
+    sec_type_swc = {
+        'soma': 1, 'somatic': 1,
+        'axon': 2, 'axonal': 2,
+        'dend': 3, 'basal': 3,
+        'apic': 4, 'apical': 4
+    }
+
+    def __init__(self, hobj, rng_seed=None, swc_path=None):
+        self.hobj = hobj  # h.Biophys1(swc_path)
+        self.rng_seed = rng_seed
+        self.swc_path = swc_path
+
+        self._prng = np.random.RandomState(self.rng_seed)
+        self._sections = None
+        self._segments = None
+        self._seg_props = _LazySegmentProps(self.hobj)  # None
+        self._seg_coords = _LazySegmentCoords(self.hobj)  # None
+        self._nseg = None
+        self._swc_map = None
+
+        # Used by find_sections() and other methods when building edges/synapses. Should make it faster to look-up
+        # cooresponding segments for a large number of syns that target the same area of a cell
+        self._trg_segs_cache = {}
+
+    def _copy(self):
+        new_morph = Morphology(hobj=self.hobj, swc_path=self.swc_path)
+        return new_morph
+
+    def _soma_position_orig(self):
+        n3dsoma = 0
+        r3dsoma = np.zeros(3)
+        for sec in self.hobj.soma:
+            n3d = int(h.n3d(sec=sec))  # get number of n3d points in each section
+            # r3d = np.zeros((3, n3d))  # to hold locations of 3D morphology for the current section
+            n3dsoma += n3d
+
+            for i in range(n3d):
+                r3dsoma[0] += h.x3d(i, sec=sec)
+                r3dsoma[1] += h.y3d(i, sec=sec)
+                r3dsoma[2] += h.z3d(i, sec=sec)
+
+        r3dsoma /= n3dsoma
+        return r3dsoma
+
+    @property
+    def segments(self):
+        if self._segments is None:
+            self._segments = []
+            for sec in self.hobj.all:
+                for seg in sec:
+                    self._segments.append(seg)
+
+        return self._segments
+
+    @property
+    def sections(self):
+        if self._sections is None:
+            self._sections = []
+            for sec in self.hobj.all:
+                self._sections.append(sec)
+
+        return self._sections
+
+    @property
+    def n_sections(self):
+        return len(self.sections)
+
+    @property
+    def seg_props(self):
+        return self._seg_props.get()
+
+    @property
+    def seg_coords(self):
+        """Get the coordinates of all segments of the cells. Each segment is defined by three values, the beginning
+        of the segment (seg_coords.p0), the middle of the segment(seg_coords.p05), and the end (seg_coords.p1)."""
+        return self._seg_coords.get()
+
+    @property
+    def nseg(self):
+        if self._nseg is None:
+            nseg = 0
+            for sec in self.hobj.all:
+                nseg += sec.nseg  # get the total # of segments in the cell
+            self._nseg = nseg
+
+        return self._nseg
+
+    @property
+    def soma_position(self):
+        return self.seg_coords.soma_pos
+
+    @property
+    def swc_map(self):
+        if self._swc_map is None:
+            swc_df = pd.read_csv(self.swc_path, sep=' ', names=['id', 'type', 'x', 'y', 'z', 'r', 'pid'], comment='#')
+            swc_df = swc_df[['id', 'type']]
+
+            name_indices = []
+            for ln in range(len(swc_df)):
+                # in read_swc.hoc all non-bifurcating section of rows are assigned a global section-id. But for each
+                # type (soma, dend, etc), there is also a nameindex id which is unique within the type, used to assign
+                # sections to their name. So lines with sec_id=10 may have nameindex=3 (Biophys1[0].dend[3])
+                sec_id = int(self.hobj.nl.point2sec[ln])
+                # swc_id = int(self.hobj.nl.pt2id(ln))
+                # swc_type = int(self.hobj.nl.type[ln])
+                name_index = int(self.hobj.nl.sections.object(sec_id).nameindex)
+                name_indices.append(name_index)
+
+            swc_df['nameindex'] = name_indices
+            self._swc_map = swc_df
+
+        return self._swc_map
+
+    def get_section(self, section_idx):
+        return self.sections[section_idx]
+
+    def set_segment_dl(self, dl):
+        """Define number of segments in a cell"""
+        self._nseg = 0
+        for sec in self.hobj.all:
+            sec.nseg = 1 + 2 * int(sec.L/(2*dl))
+            self._nseg += sec.nseg  # get the total number of segments in the cell
+
+    def choose_sections(self, section_names, distance_range, n_sections=1, cache=True):
+        """Similar to find_sections, but will only N=n_section number of sections_ids/x values randomly selected (may
+        return less if there aren't as many sections
+
+        :param section_names: 'soma', 'dend', 'apic', 'axon'
+        :param distance_range: [float, float]: distance range of sections from the soma, in um.
+        :param n_sections: int: maximum number of sections to select
+        :param cache: caches the segments + probs so that next time the same section_names/distance_range values are
+            called it will return the same values without recalculating. default True.
+        :return: [int], [float]: A list of all section_ids and a list of all segment_x values (as defined by NEURON)
+            that meet the given critera.
+        """
+        secs, probs = self.find_sections(section_names, distance_range, cache=cache)
+        secs_ix = self._prng.choice(secs, n_sections, p=probs)
+        return secs_ix, self.seg_props.x[secs_ix]
+
+    def find_sections(self, section_names, distance_range, cache=True):
+        """Retrieves a list of sections ids and section x's given a section name/type (eg axon, soma, apic, dend) and
+        the distance from the soma.
+
+        :param section_names: A list of sections to target, 'soma', 'dend', 'apic', 'axon'
+        :param distance_range: [float, float]: distance range of sections from the soma, in um.
+        :param cache: caches the segments + probs so that next time the same section_names/distance_range values are
+            called it will return the same values without recalculating. default True.
+        :return: [float], [float]: A list of all section_ids and a list of all segment_x values (as defined by NEURON)
+            that meet the given critera.
+        """
+        cache_key = (tuple(section_names), tuple(distance_range))
+        if cache and cache_key in self._trg_segs_cache:
+            return self._trg_segs_cache[cache_key]
+
+        dmin, dmax = distance_range[0], distance_range[1]
+
+        seg_d0 = self.seg_props.dist0
+        seg_d1 = self.seg_props.dist1
+        seg_length = self.seg_props.length
+        seg_type = self.seg_props.type
+
+        # Find the fractional overlap between the segment and the distance range:
+        # this is done by finding the overlap between [d0,d1] and [dmin,dmax]
+        # np.minimum(seg_d1,dmax) find the smaller of the two end locations
+        # np.maximum(seg_d0,dmin) find the larger of the two start locations
+        # np.maximum(0,overlap) is used to return zero when segments do not overlap
+        # and then dividing by the segment length
+        frac_overlap = np.maximum(0, (np.minimum(seg_d1, dmax) - np.maximum(seg_d0, dmin))) / seg_length
+        ix_drange = np.where(frac_overlap > 0)  # find indexes with non-zero overlap
+        ix_labels = np.array([], dtype=int)
+
+        for tar_sec_label in section_names:  # find indexes within sec_labels
+            sec_type = self.sec_type_swc[tar_sec_label]  # get swc code for the section label
+            ix_label = np.where(seg_type == sec_type)
+            ix_labels = np.append(ix_labels, ix_label)  # target segment indexes
+
+        tar_seg_ix = np.intersect1d(ix_drange, ix_labels)  # find intersection between indexes for range and labels
+        tar_seg_length = seg_length[tar_seg_ix] * frac_overlap[tar_seg_ix]  # weighted length of targeted segments
+        tar_seg_prob = tar_seg_length / np.sum(tar_seg_length)  # probability of targeting segments
+
+        if cache:
+            self._trg_segs_cache[cache_key] = (tar_seg_ix, tar_seg_prob)
+
+        return tar_seg_ix, tar_seg_prob
+
+    def move_and_rotate(self, soma_coords=None, rotation_angles=None, inplace=False):
+        old_seg_coords = self.seg_coords
+        new_p0 = old_seg_coords.p0.copy()
+        new_p1 = old_seg_coords.p1.copy()
+        new_p05 = old_seg_coords.p05.copy()
+        new_soma_pos = self.soma_position.copy()
+
+        if rotation_angles is not None:
+            assert(len(rotation_angles) == 3)
+            # try to calc the euler rotation matrix around an arbitary point was causing problems, instead move coords
+            # so the the soma center (p05[0]) is at the origin
+            soma_pos_mat = new_soma_pos.reshape((3, 1))
+            new_p0 = new_p0 - soma_pos_mat
+            new_p1 = new_p1 - soma_pos_mat
+            new_p05 = new_p05 - soma_pos_mat
+
+            rotx_mat = rotation_matrix([1, 0, 0], rotation_angles[0])
+            roty_mat = rotation_matrix([0, 1, 0], rotation_angles[1])
+            rotz_mat = rotation_matrix([0, 0, 1], rotation_angles[2])
+            rotxyz_mat = np.dot(rotx_mat, roty_mat.dot(rotz_mat))
+
+            new_p0 = np.dot(rotxyz_mat, new_p0) + soma_pos_mat
+            new_p1 = np.dot(rotxyz_mat, new_p1) + soma_pos_mat
+            new_p05 = np.dot(rotxyz_mat, new_p05) + soma_pos_mat
+
+        if soma_coords is not None:
+            assert(len(soma_coords) == 3)
+            soma_coords = soma_coords if isinstance(soma_coords, np.ndarray) else np.array(soma_coords)
+            displacement = soma_coords - self.soma_position
+            displacement = displacement.reshape((3, 1))  # Req to allow adding vector to matrix
+            new_p0 += displacement
+            new_p1 += displacement
+            new_p05 += displacement
+            new_soma_pos = soma_coords
+
+        # new_seg_coords = SegmentCoords(p0=new_p0, p1=new_p1, p05=new_p05, soma_pos=new_soma_pos)
+        new_seg_coords = _LazySegmentCoords(self.hobj)
+        new_seg_coords.p0 = new_p0
+        new_seg_coords.p05 = new_p05
+        new_seg_coords.p1 = new_p1
+        new_seg_coords.soma_pos = new_soma_pos
+        new_seg_coords.d = old_seg_coords.d  # diameter won't change in new position
+
+        if inplace:
+            self._seg_coords = new_seg_coords
+            return self
         else:
-            gids = file["gids"].value
-
-        if isinstance(gids, int):
-            gids = [gids]
-        elif isinstance(gids, string_types):
-            gids = [int(gids)]
-        elif isinstance(gids, NodeSet):
-            gids = gids.gids()
-
-        gids = list(set(self.local_gids) & set(gids))
-
-        amplitudes = file["amplitudes"].value
-
-        if "dts" not in list(file.keys()):
-            dts = [1 for i in range(len(amplitudes))]#Automatically sets dt to 1 ms if it is not present in the config.
+            new_morph = self._copy()
+            new_morph._seg_props = self.seg_props
+            new_morph._seg_coords = new_seg_coords
+            new_morph._soma_pos = new_soma_pos
+            return new_morph
+
+    def get_coords(self, sec_id, sec_x):
+        segs_indices = np.argwhere(self.seg_props.sec_id == sec_id).flatten()
+        return self.seg_coords.p05[:, segs_indices][:, 0]
+
+    def get_swc_id(self, sec_id, sec_x):
+        # use sec type and nameindex to find all rows in the swc that correspond to sec_id
+        sec = self.sections[sec_id]
+        sec_nameindex = self._get_sec_nameindex(sec)
+        sec_type = self._get_sec_type(sec)
+        filtered_swc = self.swc_map[(self.swc_map['type'] == sec_type) & (self.swc_map['nameindex'] == sec_nameindex)]
+        swc_ids = filtered_swc['id'].values
+
+        # use sec_x, a value between [0, 1], to estimate which swc_id/line to choose.
+        # NOTE: At the moment it assumes each line in the swc is the same distance apart, making estimating the sec_x
+        #  location easy by the number it appears in the squence
+        if len(swc_ids) == 0:
+            return -1, 0.0
+        elif len(swc_ids) == 1:
+            return swc_ids[0], sec_x
         else:
-            dts = file["dts"].value
-
-        file.close()
-        
-        for idx,gid in enumerate(gids):
-            cell = self.net.get_cell_gid(gid)
-
-            if len(amplitudes) != 1:
-                Ic = FileIClamp(amplitudes[idx], dts[idx])
-            else:
-                Ic = FileIClamp(amplitudes[0], dts[0])#This makes it so that if there are multiple gids and only one array of amplitudes, that one array is used for all gids.
-
-            Ic.attach_current(cell)
-            self._f_iclamps.append(Ic)
-
-    def attach_se_voltage_clamp(self, amplitudes, durations, gids, rs):
-        if gids is None or gids=='all':
-            gids = self.biophysical_gids
-
-        if isinstance(gids, int):
-            gids = [gids]
-        elif isinstance(gids, string_types):
-            gids = [int(gids)]
-        elif isinstance(gids, NodeSet):
-            gids = gids.gids()
-
-        all_gids = list(gids).copy()
-        gids = list(set(self.local_gids) & set(gids))
-        
-        if len(all_gids)!=len(amplitudes):
-            if len(amplitudes) != 1:
-                raise AttributeError("SEClamp must either have amplitudes for each gid or only one set of amplitudes. " 
-            + "gids: "+ str(all_gids) + ',amps: ' + str(amplitudes) + 'durs,' + str(durations))
-            elif len(durations) != 1:
-                raise AttributeError("SEClamp must either have durations for each gid or only one set of durations. "
-            + "gids: "+ str(all_gids) + ',amps: ' + str(amplitudes) + 'durs,' + str(durations))
-            else:
-                amplitudes = list(amplitudes) * len(gids)
-                durations = list(durations) * len(gids)
-
-        for idx,gid in enumerate(all_gids):
-            if gid in gids:
-                cell = self.net.get_cell_gid(gid)
-
-                try:
-                    length = len(amplitudes[idx])
-                    if length!=3:
-                        raise AttributeError("SEClamp amplitudes must be a non-list or a list of length 3.")
-                except:
-                    amplitudes[idx] = [amplitudes[idx] for i in range(3)]
-
-                try:
-                    length = len(durations[idx])
-                    if length!=3:
-                        raise AttributeError("SEClamp durations must be a non-list or a list of length 3.")
-                except:
-                    durations[idx] = [durations[idx] for i in range(3)]
-
-                SEvc = SEClamp(amplitudes[idx], durations[idx], rs=rs[idx])
-                
-                SEvc.attach_current(cell)
-                self._seclamps.append(SEvc)
-
-    def add_mod(self, module):
-        self._sim_mods.append(module)
-
-    def run(self):
-        """Run the simulation:
-        if beginning from a blank state, then will use h.run(),
-        if continuing from the saved state, then will use h.continuerun() 
-        """
-        for mod in self._sim_mods:
-            if isinstance(mod, mods.ClampReport):
-                if mod.variable == "se":
-                    mod.initialize(self, self._seclamps)
-                elif mod.variable == "ic":
-                    mod.initialize(self, self._iclamps)
-                elif mod.variable == "f_ic":
-                    mod.initialize(self, self._f_iclamps)
-            else:
-                mod.initialize(self)
-
-        self.start_time = h.startsw()
-        s_time = time.time()
-        pc.timeout(0)
-         
-        pc.barrier()  # wait for all hosts to get to this point
-        io.log_info('Running simulation for {:.3f} ms with the time step {:.3f} ms'.format(self.tstop, self.dt))
-        io.log_info('Starting timestep: {} at t_sim: {:.3f} ms'.format(self.tstep, h.t))
-        io.log_info('Block save every {} steps'.format(self.nsteps_block))
-
-        if self._start_from_state:
-            h.continuerun(h.tstop)
+            swc_place = np.max((0.0, sec_x*len(swc_ids) - 1.0))
+            swc_indx = int(np.ceil(swc_place))
+            swc_id = swc_ids[swc_indx]
+            swc_dist = swc_indx - swc_place
+            return swc_id, swc_dist
+
+    def _get_sec_type(self, sec):
+        sec_name = sec.hname()
+        sec_type_str = sec_name.split('.')[-1].split('[')[0]
+        type_str = self.sec_type_swc[sec_type_str]
+        return int(type_str)
+
+    def _get_sec_nameindex(self, sec):
+        sec_name = sec.hname()
+        sec_type_name = sec_name.split('.')[-1]
+        nameindex_str = re.search(r'\[(\d+)\]', sec_type_name).group(1)
+        return int(nameindex_str)
+
+    def __eq__(self, other):
+        if self.swc_path is None or other.swc_path is None:
+            return False
         else:
-            h.run(h.tstop)        # <- runs simuation: works in parallel
-                    
-        pc.barrier()
-
-        for mod in self._sim_mods:
-            mod.finalize(self)
-        pc.barrier()
-
-        end_time = time.time()
-
-        sim_time = self.__elapsed_time(end_time - s_time)
-        io.log_info('Simulation completed in {} '.format(sim_time))
-
-    def report_load_balance(self):
-        comptime = pc.step_time()
-        avgcomp = pc.allreduce(comptime, 1)/pc.nhost()
-        maxcomp = pc.allreduce(comptime, 2)
-        io.log_info('Maximum compute time is {} seconds.'.format(maxcomp))
-        io.log_info('Approximate exchange time is {} seconds.'.format(comptime - maxcomp))
-        if maxcomp != 0.0:
-            io.log_info('Load balance is {}.'.format(avgcomp/maxcomp))
-
-    def post_fadvance(self): 
-        """
-        Runs after every execution of fadvance (see advance.hoc)
-        Called after every time step to perform computation and save data to memory block or to disk.
-        The initial condition tstep=0 is not being saved 
-        """
-        for mod in self._sim_mods:
-            mod.step(self, self.tstep)
+            return hash(self) == hash(other)
 
-        self.tstep += 1
+    def __hash__(self):
+        """Used for comparing two Morphology objects and for storing as dict keys in seg_props_cache.
 
-        if (self.tstep % self.nsteps_block == 0) or self.tstep == self.nsteps:
-            io.log_info('    step:{} t_sim:{:.2f} ms'.format(self.tstep, h.t))
-            self.__tstep_end_block = self.tstep
-            time_step_interval = (self.__tstep_start_block, self.__tstep_end_block)
-
-            for mod in self._sim_mods:
-                mod.block(self, time_step_interval)
-
-            self.__tstep_start_block = self.tstep   # starting point for the next block
+        We assume two Morphologies are the same if they have the same morphology file path + same # of segments. This
+        is not a good way of determining if two Morphologies are equal and in actuality we would need to compare
+        seg_props on an segment-by-segment basis. However that would be comp. expensive for large networks and instead
+        do a quick spot test."""
+        comp_vals = (self.swc_path if self.swc_path else np.random.randint, self.nseg)
+        return hash(comp_vals)
 
     @classmethod
-    def from_config(cls, config, network, set_recordings=True):
-        simulation_inputs = inputs.from_config(config)
-
-        # Special case for setting synapses to spontaneously (for a given set of pre-synaptic cell-types). Using this
-        # input will change the way the network builds cells/connections and thus needs to be set first.
-        for sim_input in simulation_inputs:
-            if sim_input.input_type == 'syn_activity':
-                network.set_spont_syn_activity(
-                    precell_filter=sim_input.params['precell_filter'],
-                    timestamps=sim_input.params['timestamps']
-                )
-
-        # The network must be built before initializing the simulator because
-        # gap junctions must be set up before the simulation is initialized.
-        network.io.log_info('Building cells.')
-        network.build_nodes()
-
-        network.io.log_info('Building recurrent connections')
-        network.build_recurrent_edges()
-
-        sim = cls(network=network,
-                  dt=config.dt,
-                  tstop=config.tstop,
-                  v_init=config.v_init,
-                  celsius=config.celsius,
-                  nsteps_block=config.block_step)
-
-        # TODO: Need to create a gid selector
-        for sim_input in inputs.from_config(config):
-            if sim_input.input_type == 'spikes':
-                io.log_info('Building virtual cell stimulations for {}'.format(sim_input.name))
-                path = sim_input.params['input_file']
-                spikes = SpikeTrains.load(path=path, file_type=sim_input.module, **sim_input.params)
-                # node_set_opts = sim_input.params.get('node_set', 'all')
-                node_set = network.get_node_set(sim_input.node_set)
-                network.add_spike_trains(spikes, node_set)
-
-            elif sim_input.module == "FileIClamp":
-                sim.attach_file_current_clamp(sim_input.params["input_file"])
-
-            elif sim_input.module == 'IClamp':
-                # TODO: Parse from csv file
-                node_set = network.get_node_set(sim_input.node_set)
-                try:
-                    len(sim_input.params['amp'])
-                except:
-                    sim_input.params['amp']=[float(sim_input.params['amp'])]
-                if len(sim_input.params['amp'])>1:
-                    sim_input.params['amp']=[float(i) for i in sim_input.params['amp']]
-
-                try: 
-                    len(sim_input.params['delay'])
-                except:
-                    sim_input.params['delay']=[float(sim_input.params['delay'])]
-                if len(sim_input.params['delay'])>1:
-                    sim_input.params['delay']=[float(i) for i in sim_input.params['delay']]
-                
-                try: 
-                    len(sim_input.params['duration'])
-                except:
-                    sim_input.params['duration']=[float(sim_input.params['duration'])]
-                if len(sim_input.params['duration'])>1:
-                    sim_input.params['duration']=[float(i) for i in sim_input.params['duration']]
-                    
-                amplitude = sim_input.params['amp']
-                delay = sim_input.params['delay']
-                duration = sim_input.params['duration']
-
-                # specificed for location to place iclamp hobj.<section_name>[<section_index>](<section_dist>). The
-                # default is hobj.soma[0](0.5), the center of the soma
-                section_name = sim_input.params.get('section_name', 'soma')
-                section_index = sim_input.params.get('section_index', 0)
-                section_dist = sim_input.params.get('section_dist', 0.5)
-
-                # section_name = section_name if isinstance(section_name, (list, tuple)) else [section_name]
-                # section_index = section_index if isinstance(section_index, (list, tuple)) else [section_index]
-                # section_dist = section_dist if isinstance(section_dist, (list, tuple)) else [section_dist]
-
-                try:
-                    sim_input.params['gids']
-                except:
-                    sim_input.params['gids'] = None
-                if sim_input.params['gids'] is not None:
-                    gids = sim_input.params['gids']
-                else:
-                    gids = list(node_set.gids())
-
-                sim.attach_current_clamp(amplitude, delay, duration, gids, section_name, section_index, section_dist)
-
-            elif sim_input.module == "SEClamp":
-                node_set = network.get_node_set(sim_input.node_set)
-                try:
-                    len(sim_input.params['amps'])
-                except:
-                    sim_input.params['amps']=[float(sim_input.params['amps'])]
-                
-                try: 
-                    len(sim_input.params['durations'])
-                except:
-                    sim_input.params['durations']=[float(sim_input.params['durations'])]
-                    
-                amplitudes = sim_input.params['amps']
-                durations = sim_input.params['durations']
-                rs = None
-
-                if "rs" in sim_input.params.keys():
-                    try: 
-                        len(sim_input.params['rs'])
-                    except:
-                        sim_input.params['rs']=[float(sim_input.params['rs'])]
-                    if len(sim_input.params['rs'])>1:
-                        sim_input.params['rs']=[float(i) for i in sim_input.params['rs']]
-                    rs = sim_input.params["rs"]
-                                   
-                try:
-                    sim_input.params['gids']
-                except:
-                    sim_input.params['gids'] = None
-                if sim_input.params['gids'] is not None:
-                    gids = sim_input.params['gids']
-                else:
-                    gids = list(node_set.gids())
-
-                sim.attach_se_voltage_clamp(amplitudes, durations, gids, rs)
-
-            elif sim_input.module == 'xstim':
-                sim.add_mod(mods.XStimMod(**sim_input.params))
-
-            elif sim_input.module == 'syn_activity':
-                pass
-
-            elif sim_input.module == 'replay':
-                io.log_info('Building replay connections "{}"'.format(sim_input.name))
-                spikes = SpikeTrains.load(path=sim_input.params['spikes_file'])
-                network.build_replay_inputs(
-                    spike_trains=spikes,
-                    edges_path=sim_input.params['edges']['edges_file'],
-                    edge_types_path=sim_input.params['edges']['edge_types_file'],
-                    source_node_set=sim_input.params.get('source_node_set', 'all'),
-                    target_node_set=sim_input.params.get('target_node_set', 'all')
-                )
-
-            else:
-                io.log_exception('Can not parse input format {}'.format(sim_input.name))
+    def load(cls, hobj=None, morphology_file=None, rng_seed=None, cache_seg_props=True):
+        """Factory method, perfered way to create a Morphology object
 
-        # Parse the "reports" section of the config and load an associated output module for each report
-        sim_reports = reports.from_config(config)
-        for report in sim_reports:
-            if isinstance(report, reports.SpikesReport):
-                mod = mods.SpikesMod(**report.params)
-
-            elif report.module == 'netcon_report':
-                mod = mods.NetconReport(**report.params)
-
-            elif isinstance(report, reports.MembraneReport):
-                if report.params['sections'] == 'soma':
-                    mod = mods.SomaReport(**report.params)
-
-                else:
-                    mod = mods.MembraneReport(**report.params)
-            elif isinstance(report, reports.ClampReport):
-                mod = mods.ClampReport(**report.params)
-
-            elif isinstance(report, reports.ECPReport):
-                mod = mods.EcpMod(**report.params)
-                # Set up the ability for ecp on all relevant cells
-                # TODO: According to spec we need to allow a different subset other than only biophysical cells
-                for gid, cell in network.cell_type_maps('biophysical').items():
-                    cell.setup_ecp()
-
-            elif report.module == 'save_synapses':
-                mod = mods.SaveSynapses(**report.params)
+        :param hobj:
+        :param morphology_file:
+        :param rng_seed:
+        :param cache_seg_props:
+        :return:
+        """
+        if hobj is None and morphology_file is None:
+            io.log_exception('Unable to create Morphology, no valid HOC object or morphology file specified')
 
+        elif morphology_file is not None and hobj is None:
+            # If the HOC object hasn't already been created try creating it from the morphology
+            hobj = h.Biophys1(morphology_file)
+
+        morph = cls(hobj=hobj, swc_path=morphology_file, rng_seed=rng_seed)
+
+        if cache_seg_props and morphology_file is not None:
+            if morph in morphology_cache:
+                morph._seg_props = morphology_cache[morph][0]
+                morph._seg_coords = morphology_cache[morph][1]
             else:
-                # TODO: Allow users to register customized modules using pymodules
-                io.log_warning('Unrecognized module {}, skipping.'.format(report.module))
-                continue
-
-            sim.add_mod(mod)
-
-        return sim
+                morphology_cache[morph] = (morph._seg_props, morph._seg_coords)
 
+        return morph
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/cell.py` & `bmtk-1.0.8/bmtk/simulator/bionet/cell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/config.py` & `bmtk-1.0.8/bmtk/simulator/bionet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/default_setters/__init__.py` & `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/default_setters/cell_models.py` & `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/cell_models.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/default_setters/synapse_models.py` & `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synapse_models.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/default_setters/synaptic_weights.py` & `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synaptic_weights.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/default_templates/Biophys1.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/default_templates/Biophys1.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/gids.py` & `bmtk-1.0.8/bmtk/simulator/bionet/gids.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/iclamp.py` & `bmtk-1.0.8/bmtk/simulator/bionet/iclamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,8 +59,7 @@
         self._stim.delay = 0
         self._stim.dur = 1e9
 
         self._vect_stim = h.Vector(self._iclamp_amps)
         self._vect_stim.play(self._stim._ref_amp, self._iclamp_dt)  #Plays the amps to the IClamp amp variable with a given dt.
 
         return self._stim
-
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/import3d_gui.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_gui.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/import3d_sec.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_sec.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_morphml.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_morphml.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_nlcda.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_nlcda3.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda3.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_nts.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nts.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/import3d/read_swc.hoc` & `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_swc.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/io_tools.py` & `bmtk-1.0.8/bmtk/simulator/bionet/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/__init__.py` & `bmtk-1.0.8/bmtk/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,10 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
-from .ecp import EcpMod
-from .record_cellvars import MembraneReport, SomaReport
-from .record_spikes import SpikesMod
-from .xstim import XStimMod
-from .save_synapses import SaveSynapses
-from .record_netcons import NetconReport
-from .record_clamp import ClampReport
+import logging
+from .lazy_property import lazy_property
+
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/ecp.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/ecp.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 pc = h.ParallelContext()
 MPI_RANK = int(pc.id())
 N_HOSTS = int(pc.nhost())
 
 
 class EcpMod(SimulatorMod):
     def __init__(self, tmp_dir, file_name, electrode_positions, contributions_dir=None, cells=None, variable_name='v',
-                 electrode_channels=None, cell_bounds=None):
+                 electrode_channels=None, cell_bounds=None, minimum_distance=None):
         self._ecp_output = file_name if os.path.isabs(file_name) else os.path.join(tmp_dir, file_name)
         self._positions_file = electrode_positions
         self._tmp_outputdir = tmp_dir
 
 
         if contributions_dir is not None:
             self._save_individ_cells = True
@@ -51,14 +51,20 @@
             self._save_individ_cells = False
             self._contributions_dir = None
 
         if cell_bounds is None:
             self._cells = cells
         else:
             self._cells = list(np.arange(cell_bounds[0],cell_bounds[1]+1))
+        if minimum_distance and minimum_distance != 'auto':
+            try:
+                minimum_distance = max(float(minimum_distance), 0)
+            except Exception as e:
+                minimum_distance = 0
+        self.minimum_distance = minimum_distance
         self._rel = None
         self._fih1 = None
         self._rel_nsites = 0
         self._block_size = 0
         self._saved_gids = {}
         self._nsteps = 0
 
@@ -72,15 +78,15 @@
         self._tmp_ecp_file = self._get_tmp_fname(MPI_RANK)
         self._tmp_ecp_handle = None
         # self._tmp_ecp_dataset = None
 
         self._local_gids = []
 
     def _get_tmp_fname(self, rank):
-        return os.path.join(self._tmp_outputdir, 'tmp_{}_ecp.h5'.format(MPI_RANK))
+        return os.path.join(self._tmp_outputdir, 'tmp_{}_{}'.format(MPI_RANK, os.path.basename(self._ecp_output)))
 
     def _create_ecp_file(self, sim):
         dt = sim.dt
         tstop = sim.tstop
         self._nsteps = int(round(tstop/dt))
 
         # create file to temporary store ecp data on each rank
@@ -117,15 +123,15 @@
         file_name = os.path.join(self._contributions_dir, '{}.h5'.format(int(gid)))
         file_h5 = h5py.File(file_name, 'a')
         self._cell_var_files[gid] = file_h5
         file_h5.create_dataset('/ecp/data', (self._nsteps, self._rel_nsites), maxshape=(None, self._rel_nsites), chunks=True)
         # self._cell_var_files[gid] = file_h5['ecp']
 
     def _calculate_ecp(self, sim):
-        self._rel = RecXElectrode(self._positions_file)
+        self._rel = RecXElectrode(self._positions_file, self.minimum_distance)
         for gid in self._local_gids:
             cell = sim.net.get_cell_gid(gid)
             #cell = sim.net.get_local_cell(gid)
             # cell = sim.net.cells[gid]
             self._rel.calc_transfer_resistance(gid, cell.seg_coords)
 
         self._rel_nsites = self._rel.nsites
@@ -235,40 +241,45 @@
 
 
 class RecXElectrode(object):
     """Extracellular electrode
 
     """
 
-    def __init__(self, positions):
+    def __init__(self, positions, minimum_distance):
         """Create an array"""
         # self.conf = conf
         electrode_file = positions  # self.conf["recXelectrode"]["positions"]
 
         # convert coordinates to ndarray, The first index is xyz and the second is the channel number
         el_df = pd.read_csv(electrode_file, sep=' ')
         self.pos = el_df[['x_pos', 'y_pos', 'z_pos']].T.values
         #self.pos = el_df.as_matrix(columns=['x_pos', 'y_pos', 'z_pos']).T
         self.nsites = self.pos.shape[1]
         # self.conf['run']['nsites'] = self.nsites  # add to the config
         self.transfer_resistances = {}  # V_e = transfer_resistance*Im
+        self.minimum_distance = minimum_distance
 
     def drift(self):
         # will include function to model electrode drift
         pass
 
     def get_transfer_resistance(self, gid):
         return self.transfer_resistances[gid]
 
     def calc_transfer_resistance(self, gid, seg_coords):
         """Precompute mapping from segment to electrode locations"""
         sigma = 0.3  # mS/mm
 
         r05 = (seg_coords.p0 + seg_coords.p1) / 2
         dl = seg_coords.p1 - seg_coords.p0
+        if self.minimum_distance == 'auto':
+            rm = seg_coords.d / 2  # set minimum distance to the radius of each segment
+        else:
+            rm = self.minimum_distance  # set a common minimum distance
 
         nseg = r05.shape[1]
 
         tr = np.zeros((self.nsites, nseg))
 
         for j in range(self.nsites):  # calculate mapping for each site on the electrode
             rel = np.expand_dims(self.pos[:, j], axis=1)  # coordinates of a j-th site on the electrode
@@ -280,13 +291,17 @@
             # compute dot product column-wise, the resulting array has as many columns as original
             rlldl = np.einsum('ij,ij->j', rel_05, dl)
             dlmag = np.linalg.norm(dl, axis=0)  # length of each segment
             rll = abs(rlldl / dlmag)  # component of r parallel to the segment axis it must be always positive
             rT2 = r2 - rll ** 2  # square of perpendicular component
             up = rll + dlmag / 2
             low = rll - dlmag / 2
+            if self.minimum_distance:
+                # if electrode projection on segment axis is within distance rm to the segment
+                # check perpendicular distance to the segment axis and set lower limit to rm
+                np.fmax(rT2, rm * rm, out=rT2, where=low < rm)
             num = up + np.sqrt(up ** 2 + rT2)
             den = low + np.sqrt(low ** 2 + rT2)
             tr[j, :] = np.log(num / den) / dlmag  # units of (um) use with im_ (total seg current)
 
         tr *= 1 / (4 * math.pi * sigma)
         self.transfer_resistances[gid] = tr
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/record_cellvars.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_netcons.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,231 +1,237 @@
-# Copyright 2017. Allen Institute. All rights reserved
-#
-# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
-# following conditions are met:
-#
-# 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
-# disclaimer.
-#
-# 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following
-# disclaimer in the documentation and/or other materials provided with the distribution.
-#
-# 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote
-# products derived from this software without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
-# INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
-# WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
 import os
+import csv
 import h5py
 import numpy as np
 from neuron import h
 
-from bmtk.simulator.bionet.modules.sim_module import SimulatorMod
-from bmtk.simulator.bionet.io_tools import io
+from .sim_module import SimulatorMod
+from bmtk.simulator.bionet.biocell import BioCell
+# from bmtk.simulator.bionet.io_tools import io
+# from bmtk.simulator.bionet.pointprocesscell import PointProcessCell
 from bmtk.utils.reports import CompartmentReport
 
 try:
     # Check to see if h5py is built to run in parallel
     if h5py.get_config().mpi:
-        MembraneRecorder = CompartmentReport
+        MembraneRecorder = CompartmentReport  # cell_vars.CellVarRecorderParallel
     else:
-        MembraneRecorder = CompartmentReport
-
+        MembraneRecorder = CompartmentReport  # cell_vars.CellVarRecorder
 except Exception as e:
-    MembraneRecorder = CompartmentReport
-
-MembraneRecorder._io = io
+    MembraneRecorder = CompartmentReport  # cell_vars.CellVarRecorder
 
 pc = h.ParallelContext()
 MPI_RANK = int(pc.id())
 N_HOSTS = int(pc.nhost())
 
 
-def first_element(lst):
-    return lst[0]
-
-
-transforms_table = {
-    'first_element': first_element,
-}
-
-
-swc_type_maps = {
-    'undefined': 0,
-    'soma': 1, 'somatic': 1,
-    'axon': 2, 'axonal': 2,
-    'dend': 3, 'basal': 3, 'basal dendrite': 3, '(basal) dendrite': 3,
-    'apic': 4, 'apical': 4, 'apical denrite': 4,
-    'custom': 5, 'other': 5
-}
-
-
-class MembraneReport(SimulatorMod):
-    def __init__(self, tmp_dir, file_name, variable_name, cells=None, gids=None, sections='all', buffer_data=True, transform={}, **kwargs):
-        """Module used for saving NEURON cell properities at each given step of the simulation.
+class NetconReport(SimulatorMod):
+    def __init__(self, tmp_dir, file_name, variable_name, cells, sections='all', syn_type='Exp2Syn', buffer_data=True,
+                 transform={}, **kwargs):
+        """Module used for saving NEURON cell properties at each given step of the simulation.
 
         :param tmp_dir:
         :param file_name: name of h5 file to save variable.
         :param variables: list of cell variables to record
         :param gids: list of gids to to record
         :param sections:
         :param buffer_data: Set to true then data will be saved to memory until written to disk during each block, reqs.
         more memory but faster. Set to false and data will be written to disk on each step (default: True)
         """
         self._all_variables = list(variable_name)
         self._variables = list(variable_name)
-        self._report_name = self._variables[0]
-        self._transforms = {}
-        # self._special_variables = []
-        for var_name, fnc_name in transform.items():
-            if fnc_name is None or len(fnc_name) == 0:
-                del self._transforms[var_name]
-                continue
-
-            fnc = transforms_table[fnc_name]
-            self._transforms[var_name] = fnc
-            self._variables.remove(var_name)
 
         self._tmp_dir = tmp_dir
 
-        # TODO: Full path should be determined by config/simulation_reports module
         self._file_name = file_name if os.path.isabs(file_name) else os.path.join(tmp_dir, file_name)
         self._all_gids = cells
         self._local_gids = []
+        self._sections = sections
+
         self._var_recorder = None
-        self._gid_list = gids  # list of all gids that will have their variables saved
+        # self._var_recorder = MembraneRecorder(self._file_name, self._tmp_dir, self._all_variables,
+        #                                       buffer_data=buffer_data, mpi_rank=MPI_RANK, mpi_size=N_HOSTS)
+
+        self._virt_lookup = {}
+        self._gid_lookup = {}
+        self._sec_lookup = {}
+
+        self._gid_list = []  # list of all gids that will have their variables saved
         self._data_block = {}  # table of variable data indexed by [gid][variable]
         self._block_step = 0  # time step within a given block
+        self._curr_step = 0
+        self._object_lookup = {}
+        self._syn_type = syn_type
         self._gid_map = None
 
-        self._sections = sections if isinstance(sections, (list, tuple)) else [sections]
-        self._sections = [s.lower() for s in self._sections]
-        if len(self._sections) == 0 or 'all' in self._sections:
-            self._section_types = {v for v in swc_type_maps.values()}
-        else:
-            self._section_types = {v for k, v in swc_type_maps.items() if k in self._sections}
+        # In the use-case that users passes in "dt", "start_time", or "stop_time" parameters manually. Otherwise
+        # set to None and get values from corresponding simulation values in initialize() method
+        self._dt = kwargs.get('dt', None)
+        self._start_time = kwargs.get('start_time', None)
+        self._end_time = kwargs.get('end_time', None)
+
+        self._dt_step = None
+        self._start_step = None
+        self._end_step = None
 
     def _get_gids(self, sim):
-        # get list of gids to save. Will only work for biophysical cells saved on the current MPI rank
-        if self._gid_list is not None:
-            selected_gids = set(self._gid_list)
-        else:
-            selected_gids = set(sim.net.get_node_set(self._all_gids).gids())
-        self._local_gids = list(set(sim.biophysical_gids) & selected_gids)
+        selected_gids = set(sim.net.get_node_set(self._all_gids).gids())
+        self._local_gids = list(set(sim.local_gids) & selected_gids)
 
     def _save_sim_data(self, sim):
-        pass
+        self._var_recorder.tstart = 0.0
+        self._var_recorder.tstop = sim.tstop
+        self._var_recorder.dt = sim.dt
+
+    def _get_syn_location(self, nc, cell):
+        if isinstance(cell, BioCell):
+            sec_x = nc.postloc()
+            sec = h.cas()
+            sec_id = self._sec_lookup[cell.gid][sec]  # cell.get_section_id(sec)
+            h.pop_section()
+            return sec_id, sec_x
+        else:
+            return -1, -1
+
+    def _is_multiple(self, dividend, divisor, rtol=1.0e-4):
+        if np.isclose(dividend, divisor, rtol=rtol):
+            return True
+        else:
+            val = np.float64(dividend/divisor)
+            return val.is_integer()
+
+    def _set_valid_steps(self, sim):
+        # For dt, start_time and stop_time; if not explicitly set by the users then default back to the "run" values
+        # in the config. If user is setting their own values, make sure they are valid/within the simulation range,
+        # and make sure they are all multiples of dt.
+        if self._dt is None:
+            self._dt = sim.dt
+        elif self._dt < sim.dt:
+            raise ValueError('report dt cannot be less than simulation dt ({} < {}).'.format(
+                self._dt, sim.dt
+            ))
+        elif not self._is_multiple(self._dt, sim.dt):
+            # Users can only sample at a rate that in a whole-number multiple of the simulation dt
+            raise ValueError('report dt must be a integer multiple of simulation dt ({} != {}*m).'.format(
+                self._dt, sim.dt
+            ))
+
+        if self._start_time is None:
+            self._start_time = sim.tstart
+        elif self._start_time < sim.tstart:
+            raise ValueError('start_time cannot be less than simulation tstart.')
+        elif not self._is_multiple(self._start_time, self._dt):
+            # Make sure the start-time occurs at a self._dt multiple
+            raise ValueError('report start_time ({}) must be a integer multiple of dt ({}).'.format(
+                self._start_time, self._dt
+            ))
+
+        if self._end_time is None:
+            self._end_time = sim.tstop
+        elif self._end_time > sim.tstop:
+            raise ValueError('end_time value cannot be greater than simulation tstop ({} > {}).'.format(
+                self._end_time, sim.tstop
+            ))
+        elif not self._is_multiple(self._end_time, self._dt):
+            # Make sure the start-time occurs at a dt multiple
+            raise ValueError('report end_time ({}) must be a integer multiple of dt ({}).'.format(
+                self._end_time, self._dt
+            ))
+
+        self._dt_step = int(self._dt/sim.dt)
+        self._start_step = int(self._start_time/sim.dt)
+        self._end_step = (self._end_time/sim.dt)
+
+    def _record_on_step(self, tstep):
+        return self._start_step <= tstep < self._end_step and tstep % self._dt_step == 0
 
     def initialize(self, sim):
-        self._var_recorder = MembraneRecorder(self._file_name, mode='w', variable=self._report_name,
-                                              buffer_size=sim.nsteps_block, tstart=0.0, tstop=sim.tstop, dt=sim.dt)
         self._gid_map = sim.net.gid_pool
-
         self._get_gids(sim)
-        #self._save_sim_data(sim)
 
-        # Build segment/section list
+        self._set_valid_steps(sim)
+        self._var_recorder = MembraneRecorder(
+            self._file_name,
+            mode='w',
+            variable=self._variables[0],
+            buffer_size=sim.nsteps_block,
+            tstart=self._start_time,
+            tstop=self._end_time,
+            dt=self._dt,
+            # n_steps=sim.n_steps
+        )
+
+        for node_pop in sim.net.node_populations:
+            pop_name = node_pop.name
+            for node in node_pop[0::1]:
+                if node.model_type != 'virtual':
+                    self._gid_lookup[node.gid] = (pop_name, node.node_id)
+
+        for gid, cell in sim.net.get_local_cells().items():
+            trg_pop, trg_id = self._gid_lookup[gid]
+            if isinstance(cell, BioCell):
+                self._sec_lookup[gid] = {sec_name: sec_id for sec_id, sec_name in enumerate(cell.get_sections_id())}
+
         for gid in self._local_gids:
             pop_id = self._gid_map.get_pool_id(gid)
             sec_list = []
             seg_list = []
-            swc_ids_beg = []
-            swc_ids_end = []
-            seg_types = []
+            src_list = []
+            syn_objects = []
 
             cell = sim.net.get_cell_gid(gid)
-            morph = cell.morphology
-            segs = morph.seg_props
-            for sec_id, x0, x, x1, stype in zip(segs.sec_id, segs.x0, segs.x, segs.x1, segs.type):
-                if stype in self._section_types:
-                    swc_id_beg, _ = morph.get_swc_id(sec_id, x0)
-                    swc_id_end, _ = morph.get_swc_id(sec_id, x1)
+            for nc in cell.netcons:
+                synapse = nc.syn()
+                if self._syn_type is None or synapse.hname().startswith(self._syn_type):
+                    sec_id, seg_x = self._get_syn_location(nc, cell)
+                    src_gid = int(nc.srcgid())
                     sec_list.append(sec_id)
-                    seg_list.append(x)
+                    seg_list.append(seg_x)
+                    src_list.append(src_gid)
+                    syn_objects.append(nc.syn())
+                elif self._syn_type == 'netcon':
+                    syn_objects.append(nc)
+
+            if syn_objects:
+                # self._var_recorder.add_cell(gid, sec_list, seg_list, src_ids=src_list, trg_ids=[gid]*len(src_list))
+                self._var_recorder.add_cell(
+                    node_id=pop_id.node_id,
+                    population=pop_id.population,
+                    element_ids=sec_list,
+                    element_pos=seg_list,
+                    src_ids=src_list,
+                    trg_ids=[gid]*len(src_list)
+                )
 
-                    # TODO: Have option to turn on/off saving SWC data
-                    swc_ids_beg.append(swc_id_beg)
-                    swc_ids_end.append(swc_id_end)
-                    seg_types.append(stype)
-
-            self._var_recorder.add_cell(
-                node_id=pop_id.node_id, population=pop_id.population,
-                element_ids=sec_list, element_pos=seg_list,
-                swc_ids_beg=swc_ids_beg, swc_ids_end=swc_ids_end,
-                seg_types=seg_types
-            )
+                self._object_lookup[gid] = syn_objects
 
+        # self._var_recorder.initialize(sim.n_steps, sim.nsteps_block)
         self._var_recorder.initialize()
 
     def step(self, sim, tstep):
         # save all necessary cells/variables at the current time-step into memory
-        for gid in self._local_gids:
+        if not self._record_on_step(tstep):
+            return
+
+        for gid, netcon_objs in self._object_lookup.items():
             pop_id = self._gid_map.get_pool_id(gid)
-            cell = sim.net.get_cell_gid(gid)
-            segs = cell.morphology.segments
-            stypes = cell.morphology.seg_props.type
             for var_name in self._variables:
-                seg_vals = [getattr(seg, var_name) for seg, stype in zip(segs, stypes) if stype in self._section_types]
-                self._var_recorder.record_cell(pop_id.node_id, population=pop_id.population, vals=seg_vals, tstep=tstep)
-
-            for var_name, fnc in self._transforms.items():
-                seg_vals = [fnc(getattr(seg, var_name)) for seg, stype in zip(segs, stypes) if stype in self._section_types]
-                self._var_recorder.record_cell(pop_id.node_id, population=pop_id.population, val=seg_vals, tstep=tstep)
+                syn_values = [getattr(syn, var_name) for syn in netcon_objs]
+                if syn_values:
+                    self._var_recorder.record_cell(
+                        pop_id.node_id,
+                        population=pop_id.population,
+                        vals=syn_values,
+                        tstep=self._curr_step
+                    )
 
-        self._block_step += 1
+        # self._block_step += 1
+        self._curr_step += 1
 
     def block(self, sim, block_interval):
         # write variables in memory to file
         self._var_recorder.flush()
 
     def finalize(self, sim):
         # TODO: Build in mpi signaling into var_recorder
         pc.barrier()
         self._var_recorder.close()
-
-        #pc.barrier()
-        #self._var_recorder.merge()
-
-
-class SomaReport(MembraneReport):
-    """Special case for when only needing to save the soma variable"""
-    def __init__(self, tmp_dir, file_name, variable_name, cells, sections='soma', buffer_data=True, transform={}, **kwargs):
-        super(SomaReport, self).__init__(tmp_dir=tmp_dir, file_name=file_name, variable_name=variable_name, cells=cells,
-                                         sections=sections, buffer_data=buffer_data, transform=transform, **kwargs)
-
-    def initialize(self, sim):
-        self._var_recorder = MembraneRecorder(self._file_name, mode='w', variable=self._report_name,
-                                              buffer_size=sim.nsteps_block, tstart=0.0, tstop=sim.tstop, dt=sim.dt)
-        self._gid_map = sim.net.gid_pool
-        self._get_gids(sim)
-
-        for gid in self._local_gids:
-            pop_id = self._gid_map.get_pool_id(gid)
-            self._var_recorder.add_cell(pop_id.node_id, population=pop_id.population, element_ids=[0],
-                                        element_pos=[0.5])
-
-        # self._var_recorder.initialize(sim.n_steps, sim.nsteps_block)
-        self._var_recorder.initialize()
-
-    def step(self, sim, tstep, rel_time=0.0):
-        # save all necessary cells/variables at the current time-step into memory
-        for gid in self._local_gids:
-            pop_id = self._gid_map.get_pool_id(gid)
-            cell = sim.net.get_cell_gid(gid)
-            for var_name in self._variables:
-                var_val = getattr(cell.hobj.soma[0](0.5), var_name)
-                self._var_recorder.record_cell(pop_id.node_id, population=pop_id.population, vals=[var_val],
-                                               tstep=tstep)
-
-            for var_name, fnc in self._transforms.items():
-                var_val = getattr(cell.hobj.soma[0](0.5), var_name)
-                new_val = fnc(var_val)
-                self._var_recorder.record_cell(pop_id.node_id, population=pop_id.population, vals=[new_val],
-                                               tstep=tstep)
-
-        self._block_step += 1
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/record_clamp.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_clamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/record_spikes.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_spikes.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class SpikesMod(SimulatorMod):
     """Module use for saving spikes
 
     """
 
     def __init__(self, tmp_dir, spikes_file_csv=None, spikes_file=None, spikes_file_nwb=None, cache_to_disk=True,
-                 spikes_sort_order=None, mode='a'):
+                 spikes_sort_order=None, mode='a', compression='gzip'):
         # TODO: Have option to turn off caching spikes to csv.
         def _file_path(file_name):
             if file_name is None:
                 return None
 
             if os.path.isabs(file_name):
                 return file_name
@@ -68,14 +68,15 @@
         self._save_nwb = spikes_file_nwb is not None
 
         self._tmpdir = tmp_dir
         self._sort_order = sort_order_lu.get(spikes_sort_order, sort_order.none)
 
         cache_name = os.path.basename(self._h5_fname or self._csv_fname or self._nwb_fname)
         self._spike_writer = SpikeTrains(cache_dir=tmp_dir, cache_name=cache_name, cache_to_disk=cache_to_disk)
+        self._spike_writer.compression = compression
 
         self._gid_map = None
 
     def initialize(self, sim):
         # TODO: since it's possible that other modules may need to access spikes, set_spikes_recordings() should
         # probably be called in the simulator itself.
         sim.set_spikes_recording()
@@ -97,15 +98,16 @@
         pc.barrier()
 
         if self._save_csv:
             self._spike_writer.to_csv(self._csv_fname, sort_order=self._sort_order)
             pc.barrier()
 
         if self._save_h5:
-            self._spike_writer.to_sonata(self._h5_fname, sort_order=self._sort_order, mode=self._mode)
+            self._spike_writer.to_sonata(self._h5_fname, sort_order=self._sort_order, mode=self._mode,
+                                         compression=self._spike_writer.compression)
             pc.barrier()
 
         if self._save_nwb:
             self._spike_writer.to_nwb(self._nwb_fname, sort_order=self._sort_order)
             pc.barrier()
 
         self._spike_writer.close()
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/save_synapses.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/save_synapses.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,18 +129,18 @@
             pop_root.create_dataset('target_node_id', (n_edges_total, ), dtype=np.uint64)
             pop_root['target_node_id'].attrs['node_population'] = trg_pop
 
             pop_root.create_dataset('edge_group_id', (n_edges_total, ), dtype=np.uint16)
             pop_root.create_dataset('edge_group_index', (n_edges_total,), dtype=np.uint16)
             pop_root.create_dataset('edge_type_id', (n_edges_total, ), dtype=np.uint32)
 
-            pop_root.create_dataset('0/syn_weight', (n_edges_bio, ), dtype=np.float)
+            pop_root.create_dataset('0/syn_weight', (n_edges_bio, ), dtype=float)
             pop_root.create_dataset('0/sec_id', (n_edges_bio, ), dtype=np.uint64)
-            pop_root.create_dataset('0/sec_x', (n_edges_bio, ), dtype=np.float)
-            pop_root.create_dataset('1/syn_weight', (n_edges_point, ), dtype=np.float)
+            pop_root.create_dataset('0/sec_x', (n_edges_bio, ), dtype=float)
+            pop_root.create_dataset('1/syn_weight', (n_edges_point, ), dtype=float)
 
             total_offset = 0
             bio_offset = 0
             point_offset = 0
             for grp in in_grps:
                 n_ds = len(grp['source_node_id'])
                 pop_root['source_node_id'][total_offset:(total_offset + n_ds)] = grp['source_node_id'][()]
@@ -230,21 +230,21 @@
                                           chunks=(self._block_size, ), maxshape=(None, ))
             self._pop_root['source_node_id'].attrs['node_population'] = src_pop
             self._pop_root.create_dataset('target_node_id', (self._block_size, ), dtype=np.uint64,
                                           chunks=(self._block_size, ), maxshape=(None, ))
             self._pop_root['target_node_id'].attrs['node_population'] = trg_pop
             self._pop_root.create_dataset('edge_type_id', (self._block_size, ), dtype=np.uint32,
                                           chunks=(self._block_size, ), maxshape=(None, ))
-            self._pop_root.create_dataset('0/syn_weight', (self._block_size, ), dtype=np.float,
+            self._pop_root.create_dataset('0/syn_weight', (self._block_size, ), dtype=float,
                                           chunks=(self._block_size, ), maxshape=(None, ))
             self._pop_root.create_dataset('0/sec_id', (self._block_size, ), dtype=np.uint64,
                                           chunks=(self._block_size, ), maxshape=(None, ))
             self._pop_root.create_dataset('0/sec_x', (self._block_size, ), chunks=(self._block_size, ),
-                                          maxshape=(None, ), dtype=np.float)
-            self._pop_root.create_dataset('1/syn_weight', (self._block_size, ), dtype=np.float,
+                                          maxshape=(None, ), dtype=float)
+            self._pop_root.create_dataset('1/syn_weight', (self._block_size, ), dtype=float,
                                           chunks=(self._block_size, ), maxshape=(None, ))
 
         def _add_conn(self, edge_type_id, src_id, trg_id, grp_id):
             self._pop_root['edge_type_id'][self._nsyns] = edge_type_id
             self._pop_root['source_node_id'][self._nsyns] = src_id
             self._pop_root['target_node_id'][self._nsyns] = trg_id
             self._pop_root['edge_group_id'][self._nsyns] = grp_id
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/sim_module.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/sim_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         pass
 
     def block(self, sim, block_interval):
         """This method is called once after every block of time, as specified by the configuration.
 
         Unlike the step method which is called during every time-step, the block method will typically be called only a
         few times over the entire simulation. The block method is preferable for accessing and saving to the disk,
-        summing up existing data, or simular functionality
+        summing up existing data, or similar functionality
 
         :param sim: Simulation object
         :param block_interval: The time interval (tstep_start, tstep_end) for which the block is being called on.
         """
         pass
 
     def finalize(self, sim):
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/xstim.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 from bmtk.simulator.bionet.modules.xstim_waveforms import stimx_waveform_factory
 from bmtk.simulator.bionet.utils import rotation_matrix
 from bmtk.simulator.bionet.io_tools import io
 
 
 class XStimMod(SimulatorMod):
     def __init__(self, positions_file, waveform, mesh_files_dir=None, cells=None, set_nrn_mechanisms=True,
-                 node_set=None):
+                 resistance=300.0, node_set=None):
         self._positions_file = positions_file
         self._mesh_files_dir = mesh_files_dir if mesh_files_dir is not None \
             else os.path.dirname(os.path.realpath(self._positions_file))
 
         self._waveform = waveform  # TODO: Check if waveform is a file or dict and load it appropiately
 
         self._set_nrn_mechanisms = set_nrn_mechanisms
         self._electrode = None
         self._cells = cells
         self._local_gids = []
         self._fih = None
+        self._resistance = resistance
 
     # def __set_extracellular_mechanism(self):
     #     for gid in self._local_gids:
 
     def initialize(self, sim):
         if self._cells is None:
             # if specific gids not listed just get all biophysically detailed cells on this rank
@@ -38,15 +39,15 @@
             self._local_gids = list(set(sim.local_gids) & set(self._all_gids))
 
         self._electrode = StimXElectrode(self._positions_file, self._waveform, self._mesh_files_dir, sim.dt)
         for gid in self._local_gids:
             # cell = sim.net.get_local_cell(gid)
             cell = sim.net.get_cell_gid(gid)
             cell.setup_xstim(self._set_nrn_mechanisms)
-            self._electrode.set_transfer_resistance(gid, cell.seg_coords)
+            self._electrode.set_transfer_resistance(gid, cell.seg_coords, rho=self._resistance)
 
         def set_pointers():
             for gid in self._local_gids:
                 cell = sim.net.get_cell_gid(gid)
                 # cell = sim.net.get_local_cell(gid)
                 cell.set_ptr2e_extracellular()
 
@@ -133,16 +134,15 @@
             rot_y = rotation_matrix([0, 1, 0], phi_y)
             rot_z = rotation_matrix([0, 0, 1], phi_z)
             rot_xy = rot_x.dot(rot_y)
             rot_xyz = rot_xy.dot(rot_z)
             new_mesh = np.dot(rot_xyz, self.el_mesh[el])
             self.el_mesh[el] = new_mesh
 
-    def set_transfer_resistance(self, gid, seg_coords):
-        rho = 300.0  # ohm cm
+    def set_transfer_resistance(self, gid, seg_coords, rho=300.0):
         r05 = seg_coords.p05
         nseg = r05.shape[1]
         cell_map = np.zeros((self.elnsites, nseg))
         for el in six.moves.range(self.elnsites):
             mesh_size = self.el_mesh_size[el]
             for k in range(mesh_size):
                 rel = np.expand_dims(self.el_mesh[el][:, k], axis=1)
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/modules/xstim_waveforms.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim_waveforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         if file_ext == 'csv':
             return WaveformCustom(waveform)
 
         elif file_ext == 'json':
             with open(waveform, 'r') as f:
                 waveform = json.load(f)
         else:
-            io.log_warning('Unknwon filetype for waveform')
+            io.log_warning('Unknown filetype for waveform')
 
     shape_key = waveform["shape"].lower()
 
     if shape_key not in shape_classes:
         io.log_warning("Waveform shape not known")  # throw error?
 
     Constructor = shape_classes[shape_key]
```

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/nml_reader.py` & `bmtk-1.0.8/bmtk/simulator/bionet/nml_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/nrn.py` & `bmtk-1.0.8/bmtk/simulator/bionet/nrn.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/pointprocesscell.py` & `bmtk-1.0.8/bmtk/simulator/bionet/pointprocesscell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/pyfunction_cache.py` & `bmtk-1.0.8/bmtk/simulator/bionet/pyfunction_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/schemas/config_schema.json` & `bmtk-1.0.8/bmtk/simulator/bionet/schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/schemas/csv_edge_types.json` & `bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_edge_types.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/seclamp.py` & `bmtk-1.0.8/bmtk/simulator/bionet/seclamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/sonata_adaptors.py` & `bmtk-1.0.8/bmtk/simulator/bionet/sonata_adaptors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/utils.py` & `bmtk-1.0.8/bmtk/simulator/bionet/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/bionet/virtualcell.py` & `bmtk-1.0.8/bmtk/simulator/bionet/virtualcell.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 from neuron import h
 import numpy as np
+import pandas as pd
 
 from bmtk.simulator.bionet.io_tools import io
+from bmtk.utils.reports.spike_trains.spike_trains import SpikeTrains
 
 
 class VirtualCell(object):
     """Representation of a Virtual/External node"""
 
     def __init__(self, node, population, spike_train_dataset):
         # VirtualCell is currently not a subclass of bionet.Cell class b/c the parent has a bunch of properties that
@@ -46,15 +48,22 @@
 
     @property
     def hobj(self):
         return self._hobj
 
     def set_stim(self, stim_prop, spike_train):
         """Gets the spike trains for each individual cell."""
-        spikes = spike_train.get_times(node_id=self.node_id)
+        if isinstance(spike_train, SpikeTrains) or hasattr(spike_train, 'get_times'):
+            spikes = spike_train.get_times(node_id=self.node_id)
+        elif isinstance(spike_train, (list, np.ndarray, pd.Series)):
+            spikes = spike_train
+        elif spike_train is None:
+            spikes = []
+        else:
+            spikes = None
 
         if spikes is None:
             spikes = []
 
         if np.any(np.array(spikes) < 0.0):
             # NRN will fail if VecStim contains negative spike-time, throw an exception and log info for user
             io.log_exception('spike train {} contains negative number, unable to run virtual cell in NEURON'.format(
```

### Comparing `bmtk-1.0.7/bmtk/simulator/core/graph.py` & `bmtk-1.0.8/bmtk/simulator/core/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,14 @@
         """
         nodes = sonata_file.nodes
 
         selected_populations = nodes.population_names if populations is None else populations
         for pop_name in selected_populations:
             if pop_name not in nodes:
                 # when user wants to simulation only a few populations in the file
-                print('HERE')
                 continue
 
             if pop_name in self.node_populations:
                 # Make sure their aren't any collisions
                 self.io.log_exception('There are multiple node populations with name {}.'.format(pop_name))
 
             node_pop = nodes[pop_name]
@@ -236,15 +235,15 @@
             if 'virtual' in model_types:
                 self._virtual_populations_map[pop_name] = node_pop
                 self._virtual_cells_nid[pop_name] = {}
                 model_types -= set(['virtual'])
                 if model_types:
                     # We'll allow a population to have virtual and non-virtual nodes but it is not ideal
                     self.io.log_warning('Node population {} contains both virtual and non-virtual nodes which can '.format(pop_name) +
-                                        'cause memory and build-time inefficency. Consider separating virtual nodes ' +
+                                        'cause memory and build-time inefficiency. Consider separating virtual nodes ' +
                                         'into their own population')
 
             if model_types:
                 self._internal_populations_map[pop_name] = node_pop
 
             self._node_sets[pop_name] = NodeSet({'population': pop_name}, self)
```

### Comparing `bmtk-1.0.7/bmtk/simulator/core/io_tools.py` & `bmtk-1.0.8/bmtk/simulator/core/io_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,9 +121,14 @@
         if self.mpi_rank == 0:
             self.logger.error(message)
 
         self.barrier()
         if raise_exception:
             raise Exception(message)
 
+    def log_debug(self, message, all_ranks=False):
+        if all_ranks is False and self.mpi_rank != 0:
+            return
+
+        self.logger.debug(message)
 
 io = IOUtils()
```

### Comparing `bmtk-1.0.7/bmtk/simulator/core/network_reader.py` & `bmtk-1.0.8/bmtk/simulator/core/network_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/node_population.py` & `bmtk-1.0.8/bmtk/simulator/core/node_population.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/node_sets.py` & `bmtk-1.0.8/bmtk/simulator/core/node_sets.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,14 +37,22 @@
             for gid in self._preselected_gids:
                 yield gid
         else:
             for pop in self._populations:
                 for node in pop.filter(self._filter):
                     yield self._network.gid_pool.get_gid(name=pop.name, node_id=node.node_id)
 
+    @property
+    def node_ids(self):
+        node_ids = []
+        for pop in self._populations:
+            for node in pop.filter(self._filter):
+                node_ids.append(node.node_id)
+        return node_ids
+
     def nodes(self):
         return None
 
 
 class NodeSetAll(NodeSet):
     def __init__(self, network):
         super(NodeSetAll, self).__init__({}, network)
```

### Comparing `bmtk-1.0.7/bmtk/simulator/core/pyfunction_cache.py` & `bmtk-1.0.8/bmtk/simulator/core/pyfunction_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/simulation_config.py` & `bmtk-1.0.8/bmtk/simulator/core/simulation_config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/simulation_config_validator.py` & `bmtk-1.0.8/bmtk/simulator/core/simulation_config_validator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/simulator_network.py` & `bmtk-1.0.8/bmtk/simulator/core/simulator_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from six import string_types
 import numpy as np
 import os
 import h5py
+import pandas as pd
 
 from bmtk.simulator.core.io_tools import io
 from .simulation_config import SimulationConfig
 from bmtk.simulator.core.node_sets import NodeSet, NodeSetAll
 from bmtk.simulator.core import sonata_reader
 
 
@@ -115,15 +116,15 @@
             if 'population' not in node_pop_df:
                 node_pop_df['population'] = node_pop.name
 
             node_pop_df = node_pop_df.set_index(['population', node_pop_df.index.astype(dtype=np.uint64)])
             if all_nodes_df is None:
                 all_nodes_df = node_pop_df
             else:
-                all_nodes_df = all_nodes_df.append(node_pop_df)
+                all_nodes_df = pd.concat([all_nodes_df, node_pop_df])
 
         return all_nodes_df
 
     def get_node_groups(self, populations=None):
         if populations is None:
             selected_pops = self.node_populations
 
@@ -138,15 +139,15 @@
             node_pop_df = node_pop.nodes_df(index_by_id=False)
             if 'population' not in node_pop_df:
                 node_pop_df['population'] = node_pop.name
 
             if all_nodes_df is None:
                 all_nodes_df = node_pop_df
             else:
-                all_nodes_df = all_nodes_df.append(node_pop_df, sort=False)
+                all_nodes_df = pd.concat([all_nodes_df, node_pop_df], sort=False)
 
         return all_nodes_df
 
     def get_node_sets(self, populations=None, groupby=None, **filterby):
         selected_nodes_df = self.node_properties(populations)
         for k, v in filterby:
             if isinstance(v, (np.ndarray, list, tuple)):
```

### Comparing `bmtk-1.0.7/bmtk/simulator/core/sonata_reader/edge_adaptor.py` & `bmtk-1.0.8/bmtk/simulator/core/sonata_reader/edge_adaptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,31 +93,37 @@
     def get_edge(self, sonata_node):
         return SonataBaseEdge(sonata_node, self)
 
     @staticmethod
     def preprocess_edge_types(network, edge_population):
         edge_types_table = edge_population.types_table
         edge_type_ids = np.unique(edge_population.type_ids)
+        cached_dynamics = {}
 
         for et_id in edge_type_ids:
             edge_type = edge_types_table[et_id]
             if 'dynamics_params' in edge_types_table.columns and edge_type['dynamics_params'] != None:
                 dynamics_params = edge_type['dynamics_params']
                 params_dir = network.get_component('synaptic_models_dir')
 
                 params_path = os.path.join(params_dir, dynamics_params)
 
                 # see if we can load the dynamics_params as a dictionary. Otherwise just save the file path and let the
                 # cell_model loader function handle the extension.
-                try:
-                    params_val = json.load(open(params_path, 'r'))
-                    edge_type['dynamics_params'] = params_val
-                except Exception:
-                    # TODO: Check dynamics_params before
-                    network.io.log_exception('Could not find edge dynamics_params file {}.'.format(params_path))
+                # Cache the loaded dynamics_params to minimize file access.
+                if params_path in cached_dynamics:
+                    edge_type['dynamics_params'] = cached_dynamics[params_path]
+                else:
+                    try:
+                        params_val = json.load(open(params_path, 'r'))
+                        edge_type['dynamics_params'] = params_val
+                        cached_dynamics[params_path] = params_val
+                    except Exception:
+                        # TODO: Check dynamics_params before
+                        network.io.log_exception('Could not find edge dynamics_params file {}.'.format(params_path))
 
             # Split target_sections
             if 'target_sections' in edge_type:
                 trg_sec = edge_type['target_sections']
                 if trg_sec is not None:
                     try:
                         edge_type['target_sections'] = ast.literal_eval(trg_sec)
```

### Comparing `bmtk-1.0.7/bmtk/simulator/core/sonata_reader/network_reader.py` & `bmtk-1.0.8/bmtk/simulator/core/sonata_reader/network_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/sonata_reader/node_adaptor.py` & `bmtk-1.0.8/bmtk/simulator/core/sonata_reader/node_adaptor.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/core/sonata_schemas/config_schema.json` & `bmtk-1.0.8/bmtk/simulator/core/sonata_schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/cell.py` & `bmtk-1.0.8/bmtk/simulator/filternet/cell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/config.py` & `bmtk-1.0.8/bmtk/simulator/filternet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/default_setters/cell_loaders.py` & `bmtk-1.0.8/bmtk/simulator/filternet/default_setters/cell_loaders.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/filternetwork.py` & `bmtk-1.0.8/bmtk/simulator/filternet/filternetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/filtersimulator.py` & `bmtk-1.0.8/bmtk/simulator/filternet/filtersimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,18 @@
                 if 'data_file' in params:
                     m_data = np.load(params['data_file'])
                 elif 'data' in params:
                     m_data = params['data']
                 else:
                     raise Exception('Could not find movie "data_file" in config to use as input.')
 
-                contrast_min, contrast_max = m_data.min(), m_data.max()
+                # contrast_min, contrast_max = m_data.min(), m_data.max()
                 normalize_data = params.get('normalize', False)
-                if contrast_min < -1.0 or contrast_max > 1.0:
-                    if normalize_data:
-                        self.io.log_info('Normalizing movie data to (-1.0, 1.0).')
-                        m_data = m_data*2.0/(contrast_max - contrast_min) - 1.0
-                    else:
-                        self.io.log_info('Movie data range is not normalized to (-1.0, 1.0).')
+                if normalize_data:
+                    m_data = Movie.normalize_matrix(m_data, domain=normalize_data)
 
                 init_params = FilterSimulator.find_params(['row_range', 'col_range', 'labels', 'units', 'frame_rate',
                                                            't_range'], **params)
                 self._movies.append(Movie(m_data, **init_params))
 
         elif movie_type == 'full_field':
             raise NotImplementedError
@@ -159,17 +155,18 @@
                 raise Exception('Unable to load input type {}'.format(sim_input.input_type))
 
         network.io.log_info('Building cells.')
         network.build_nodes()
 
         rates_csv = config.output.get('rates_csv', None)
         rates_h5 = config.output.get('rates_h5', None)
+        compression = config.output.get('compression', 'gzip')
         if rates_csv or rates_h5:
-            sim.add_mod(mods.RecordRates(rates_csv, rates_h5, config.output_dir))
+            sim.add_mod(mods.RecordRates(rates_csv, rates_h5, config.output_dir, compression=compression))
 
         spikes_csv = config.output.get('spikes_csv', None) or config.output.get('spikes_file_csv', None)
         spikes_h5 = config.output.get('spikes_h5', None) or config.output.get('spikes_file', None)
         spikes_nwb = config.output.get('spikes_nwb', None) or config.output.get('spikes_file_nwb', None)
         if spikes_csv or spikes_h5 or spikes_nwb:
-            sim.add_mod(mods.SpikesGenerator(spikes_csv, spikes_h5, spikes_nwb, config.output_dir))
+            sim.add_mod(mods.SpikesGenerator(spikes_csv, spikes_h5, spikes_nwb, config.output_dir, compression=compression))
 
         return sim
```

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/io_tools.py` & `bmtk-1.0.8/bmtk/simulator/filternet/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cellmetrics.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmetrics.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cellmodel.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmodel.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/cursor.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cursor.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/fitfuns.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/fitfuns.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/kernel.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/kernel.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/linearfilter.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/linearfilter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/lnunit.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lnunit.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/make_cell_list.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/make_cell_list.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/movie.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/movie.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 from .utilities import convert_tmin_tmax_framerate_to_trange
+from bmtk.simulator.filternet.io_tools import io
 
 
 class Movie(object):
     def __init__(self, data, row_range=None, col_range=None, labels=('time', 'y', 'x'),
                  units=('second', 'pixel', 'pixel'), frame_rate=None, t_range=None):
         self.data = data
         self.labels = labels
@@ -125,14 +126,65 @@
         
         return Movie(new_data, row_range=self.row_range.copy(), col_range=self.col_range.copy(), labels=self.labels,
                      units=self.units, frame_rate=self.frame_rate)
 
     def __getitem__(self, *args):
         return self.data.__getitem__(*args)
 
+    @staticmethod
+    def normalize_matrix(m_data, domain=None):
+        """Attempts to take a numpy matrix "movie" and normalize the contrast values to range [-1.0, 1.0].
+
+        :param m_data: A numpy matrix TxRxC containing an original "movie" data
+        :param domain: If A tuple of values [min_contrast, max_contrast], will use those values to normalize. Otherwise
+            will attempt to determine original contrast range from the m_data.
+        :return: m_data that has been normalized
+        """
+        if isinstance(domain, (list, tuple, np.ndarray)):
+            # Allow users to specify the contrast range of the original movie [c_min, c_max] that will be
+            # converted to range [-1.0, +1.0]
+            if len(domain) != 2:
+                raise ValueError(
+                    'Unable to normalize movie; please specify to minimum and maximum contrast for original movie with '
+                    'list [min_contrast, max_contrast]'
+                )
+            c_min, c_max = domain[0], domain[1]
+            if c_min >= c_max:
+                raise ValueError(
+                    'Unable to normalize movie; original movie range must be defined with min_contrast < max_contrast'
+                )
+            elif m_data.min() < c_min or m_data.max() > c_max:
+                raise ValueError(
+                    'Unable to normalize movie; trying to convert movie from contrast values ' +
+                    '[{}, {}] --> [-1.0, 1.0], '.format(c_min, c_max) +
+                    'but movie contains values outside of original domain.'
+                )
+        else:
+            # Use the existing movie to try to best guess the domain the original movie is already in; in most
+            # cases it will be [0.0, 1.0] or [0, 256]
+            m_min, m_max = m_data.min(), m_data.max()
+            if m_min >= 0.0 and m_max <= 1.0:
+                c_min, c_max = 0.0, 1.0
+            elif m_min >= -1.0 and m_max <= 1.0:
+                # All values fall between [-1.0, 1.0], likely movie is likely already normalized.
+                io.log_debug('Input movie is already normalized between contrast values [-1.0, 1.0].')
+                return m_data
+            elif m_min >= 0 and m_max < 256:
+                c_min, c_max = 0.0, 255.0
+            else:
+                c_min, c_max = m_min, m_max
+
+        if c_min == c_max:
+            raise ValueError(
+                'Unable to normalize movie; please specify a range for the contrast min and max of the input movie.'
+            )
+
+        io.log_debug('Normalizing input movie from contrast range [{}, {}] --> [-1.0, 1.0].')
+        return (m_data - c_min)*2.0/(c_max - c_min) - 1.0
+
 
 # TODO: Instead of using subclasses, convert the following movie type to a Factory class/function that returns a Movie
 #   object
 class FullFieldMovie(Movie):
     def __init__(self, f, rows, cols, frame_rate=24.0):
         if np.isscalar(rows):
             rows = np.arange(0, rows)
```

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/poissongeneration.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/poissongeneration.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/spatialfilter.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/spatialfilter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/temporalfilter.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/temporalfilter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/transferfunction.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/transferfunction.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/util_fns.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/util_fns.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/lgnmodel/utilities.py` & `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/utilities.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/modules/create_spikes.py` & `bmtk-1.0.8/bmtk/simulator/filternet/modules/create_spikes.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from bmtk.utils.reports.spike_trains import SpikeTrains, pop_na, sort_order, sort_order_lu
 from bmtk.simulator.filternet.lgnmodel import poissongeneration as pg
 from bmtk.utils.io.ioutils import bmtk_world_comm
 
 
 class SpikesGenerator(SimModule):
     def __init__(self, spikes_file_csv=None, spikes_file=None, spikes_file_nwb=None, tmp_dir='output',
-                 sort_order='node_id'):
+                 sort_order='node_id', compression='gzip'):
         def _get_file_path(file_name):
             if file_name is None or os.path.isabs(file_name):
                 return file_name
 
             else:
                 rel_tmp = os.path.realpath(tmp_dir)
                 rel_fname = os.path.realpath(file_name)
@@ -25,14 +25,15 @@
                     return file_name
 
         self._csv_fname = _get_file_path(spikes_file_csv)
         self._save_csv = spikes_file_csv is not None
 
         self._h5_fname = _get_file_path(spikes_file)
         self._save_h5 = spikes_file is not None
+        self._compression = compression
 
         self._nwb_fname = _get_file_path(spikes_file_nwb)
         self._save_nwb = spikes_file_nwb is not None
 
         self._tmpdir = tmp_dir
 
         # self._spike_writer = SpikeTrainWriter(tmp_dir=tmp_dir)
@@ -53,15 +54,15 @@
     def finalize(self, sim):
         self._spike_writer.flush()
 
         if self._save_csv:
             self._spike_writer.to_csv(self._csv_fname, sort_order=self._sort_order)
 
         if self._save_h5:
-            self._spike_writer.to_sonata(self._h5_fname, sort_order=self._sort_order)
+            self._spike_writer.to_sonata(self._h5_fname, sort_order=self._sort_order, compression=self._compression)
 
         if self._save_nwb:
             self._spike_writer.to_nwb(self._nwb_fname, sort_order=self._sort_order)
 
         self._spike_writer.close()
```

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/modules/record_rates.py` & `bmtk-1.0.8/bmtk/simulator/filternet/modules/record_rates.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 import glob
 
 from .base import SimModule
 from bmtk.utils.io.ioutils import bmtk_world_comm
 
 
 class RecordRates(SimModule):
-    def __init__(self, csv_file=None, h5_file=None, tmp_dir='output', sort_order='node_id'):
+    def __init__(self, csv_file=None, h5_file=None, tmp_dir='output', sort_order='node_id',
+                 compression='gzip'):
         self._tmp_dir = tmp_dir
         self._csv_file = csv_file if csv_file is None or os.path.isabs(csv_file) else os.path.join(tmp_dir, csv_file)
         self._save_to_csv = csv_file is not None
         self._tmp_rates_path = None
 
         h5_file = h5_file if h5_file is None or os.path.isabs(h5_file) else os.path.join(tmp_dir, h5_file)
         self._save_to_h5 = h5_file is not None
         self._h5_file = h5_file
+        # make sure h5py is not confused with string 'none' or 'None'.
+        if isinstance(compression, str):
+            if compression.lower() == 'none':
+                compression = None
+        self._compression = compression
 
         self._sort_order = sort_order
         self._n_nodes = 0
         self._n_timesteps = 0
 
         self._timestamps = None
         self._node_ids = {}
@@ -36,15 +42,15 @@
 
     def save(self, sim, cell, times, rates):
         if self._timestamps is None:
             self._n_timesteps = len(times)
             self._timestamps = times
 
         if cell.population not in self._firing_rates:
-            self._firing_rates[cell.population] = np.zeros((self._n_nodes, self._n_timesteps), dtype=np.float)
+            self._firing_rates[cell.population] = np.zeros((self._n_nodes, self._n_timesteps), dtype=float)
             self._node_ids[cell.population] = np.zeros(self._n_nodes, dtype=np.uint)
 
         self._firing_rates[cell.population][self._node_counter, :] = rates
         self._node_ids[cell.population][self._node_counter] = cell.node_id
         self._node_counter += 1
 
     def finalize(self, sim):
@@ -65,17 +71,17 @@
 
             if self._save_to_h5:
                 try:
                     rates_h5 = h5py.File(self._h5_file, 'w')
                     rates_grp = rates_h5.create_group('/firing_rates')
                     for pop, pop_table in self._firing_rates.items():
                         pop_grp = rates_grp.create_group(pop)
-                        pop_grp.create_dataset('node_id', data=self._node_ids[pop])
-                        pop_grp.create_dataset('times', data=self._timestamps)
-                        pop_grp.create_dataset('firing_rates_Hz', data=self._firing_rates[pop].T)
+                        pop_grp.create_dataset('node_id', data=self._node_ids[pop], compression=self._compression)
+                        pop_grp.create_dataset('times', data=self._timestamps, compression=self._compression)
+                        pop_grp.create_dataset('firing_rates_Hz', data=self._firing_rates[pop].T, compression=self._compression)
 
                 except Exception as e:
                     print(e)
                     print('Unable to save rates to hdf5')
 
             if self._save_to_csv:
                 csv_fhandle = open(self._csv_file, 'w')
@@ -90,17 +96,17 @@
         bmtk_world_comm.barrier()
         self._clean()
 
     def _write_rates_on_rank(self):
         with h5py.File(self._tmp_rates_path, 'w') as h5:
             for pop in self._firing_rates.keys():
                 pop_grp = h5.create_group(pop)
-                pop_grp.create_dataset('time', data=self._timestamps)
-                pop_grp.create_dataset('node_id', data=self._node_ids[pop])
-                pop_grp.create_dataset('firing_rates_Hz', data=self._firing_rates[pop])
+                pop_grp.create_dataset('time', data=self._timestamps, compression=self._compression)
+                pop_grp.create_dataset('node_id', data=self._node_ids[pop], compression=self._compression)
+                pop_grp.create_dataset('firing_rates_Hz', data=self._firing_rates[pop], compression=self._compression)
 
     def _combine_rates(self):
         n_cells = {}
         if bmtk_world_comm.MPI_rank == 0:
             rates_paths = glob.glob(os.path.join(self._tmp_dir, '.rates.*.h5'))
             h5_handles = []
             timestamps = None
@@ -116,15 +122,15 @@
                     if timestamps is None:
                         timestamps = pop_grp['time'][()]
                     else:
                         assert (np.allclose(timestamps, pop_grp['time'][()]))
 
             n_timestamps = len(timestamps)
 
-            self._firing_rates = {pop: np.zeros((n_cells[pop], n_timestamps), dtype=np.float) for pop in n_cells.keys()}
+            self._firing_rates = {pop: np.zeros((n_cells[pop], n_timestamps), dtype=float) for pop in n_cells.keys()}
             self._node_ids = {pop: np.zeros(n_cells[pop], dtype=np.uint32) for pop in n_cells.keys()}
             beg_indices = {pop: 0 for pop in n_cells.keys()}
 
             for h5 in h5_handles:
                 for pop, pop_grp in h5.items():
                     beg_index = beg_indices[pop]
                     end_index = beg_index + pop_grp['node_id'].shape[0]
```

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/pyfunction_cache.py` & `bmtk-1.0.8/bmtk/simulator/filternet/pyfunction_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class _PyFunctions(object):
     """Structure for holding custom user-defined python functions.
 
     Will store a set of functions created by the user. Should not access this directly but rather user the
     decorators or setter functions, and use the py_modules class variable to access individual functions. Is divided
     up into
-    synaptic_weight: functions for calcuating synaptic weight.
+    synaptic_weight: functions for calculating synaptic weight.
     cell_model: should return NEURON cell hobj.
     synapse model: should return a NEURON synapse object.
     """
     def __init__(self):
         self.__cell_processors = {}
 
     def clear(self):
```

### Comparing `bmtk-1.0.7/bmtk/simulator/filternet/sonata_adaptors.py` & `bmtk-1.0.8/bmtk/simulator/filternet/sonata_adaptors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/__init__.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/config.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/gids.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/gids.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/glif_utils.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/glif_utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/io_tools.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/modules/multimeter_reporter.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/modules/multimeter_reporter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/modules/record_spikes.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/modules/record_spikes.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 class SpikesMod(object):
     """Module use for saving spikes
 
     """
 
     def __init__(self, tmp_dir, spikes_file_csv=None, spikes_file=None, spikes_file_nwb=None, spikes_sort_order=None,
-                 cache_to_disk=True):
+                 cache_to_disk=True, compression='gzip'):
         def _get_path(file_name):
             # Unless file-name is an absolute path then it should be placed in the $OUTPUT_DIR
             if file_name is None:
                 return None
 
             if os.path.isabs(file_name):
                 return file_name
@@ -121,14 +121,15 @@
         self._tmp_file_base = 'tmp_spike_times'
         self._spike_labels = os.path.join(self._tmp_dir, self._tmp_file_base)
 
         self._spike_writer = SpikeTrains(cache_dir=tmp_dir, cache_to_disk=cache_to_disk)
         self._spike_writer.delimiter = '\t'
         self._spike_writer.gid_col = 0
         self._spike_writer.time_col = 1
+        self._spike_writer.compression = compression
         self._sort_order = sort_order.none if not spikes_sort_order else sort_order_lu[spikes_sort_order]
 
         self._spike_detector = None
 
     def initialize(self, sim):
         self._spike_detector = create_spike_detector(self._spike_labels)
         nest.Connect(sim.net.gid_map.gids, self._spike_detector)
@@ -143,15 +144,16 @@
 
         if self._csv_fname is not None:
             self._spike_writer.to_csv(self._csv_fname, sort_order=self._sort_order)
             # io.barrier()
 
         if self._h5_fname is not None:
             # TODO: reimplement with pandas
-            self._spike_writer.to_sonata(self._h5_fname, sort_order=self._sort_order)
+            self._spike_writer.to_sonata(self._h5_fname, sort_order=self._sort_order,
+                                         compression=self._spike_writer.compression)
             # io.barrier()
 
         if self._nwb_fname is not None:
             self._spike_writer.to_nwb(self._nwb_fname, sort_order=self._sort_order)
             # io.barrier()
 
         self._spike_writer.close()
```

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/nest_utils.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/nest_utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/pointnetwork.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/pointnetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/pointsimulator.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/pointsimulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import bmtk.simulator.utils.simulation_inputs as inputs
 from bmtk.utils.reports.spike_trains import SpikeTrains
 from . import modules as mods
 from bmtk.simulator.core.node_sets import NodeSet
 
 
 class PointSimulator(Simulator):
-    def __init__(self, graph, dt=0.001, overwrite=True, print_time=False):
+    def __init__(self, graph, dt=0.001, overwrite=True, print_time=False, n_thread=1):
         self._tstop = 0.0  # simulation time
         self._dt = dt  # time step
         self._output_dir = './output/'  # directory where log and temporary output will be stored
         self._overwrite = overwrite
         self._block_run = False
         self._block_size = -1
 
@@ -67,15 +67,15 @@
         # TODO: Make this a parameter in the config file
         # TODO: Allow different inputs to have different options
         self._sg_params = {'precise_times': True}
 
         # Reset the NEST kernel for a new simualtion
         # TODO: move this into it's own function and make sure it is called before network is built
         nest.ResetKernel()
-        nest.SetKernelStatus({"resolution": self._dt, "overwrite_files": self._overwrite, "print_time": print_time})
+        nest.SetKernelStatus({"resolution": self._dt, "overwrite_files": self._overwrite, "print_time": print_time, "local_num_threads": n_thread})
 
     @property
     def tstart(self):
         return 0.0
 
     @property
     def dt(self):
@@ -141,28 +141,15 @@
 
         for pop_name, pop in self._graph._nestid2nodeid_map.items():
             # print pop.keys()
 
             nest.Connect(pop.keys(), self._spike_detector)
         # exit()
     '''
-
-    def add_step_currents(self, amp_times, amp_values, node_set, input_name):
-        scg = nest.Create("step_current_generator",
-                          params={'amplitude_times': amp_times, 'amplitude_values': amp_values})
-
-        if not isinstance(node_set, NodeSet):
-            node_set = self.net.get_node_set(node_set)
-
-        # Convert node set into list of gids and then look-up the nest-ids
-        for pop_name in node_set.population_names():
-            # nest_ids = self.net.gid_map.get_nestids(pop_name, list(node_set.gids()))
-            nest_ids = node_set.gids()
-            nest.Connect(scg, list(nest_ids), syn_spec={'delay': self.dt})
-
+            
     def run(self, tstop=None):
         if tstop is None:
             tstop = self._tstop
 
         for mod in self._mods:
             mod.initialize(self)
 
@@ -185,33 +172,46 @@
         io.barrier()
         io.log_info('Done.')
 
     def add_mod(self, mod):
         self._mods.append(mod)
 
     @classmethod
-    def from_config(cls, configure, graph):
+    def from_config(cls, configure, graph, n_thread=None):
         # load the json file or object
         if isinstance(configure, string_types):
             config = Config.from_json(configure, validate=True)
         elif isinstance(configure, dict):
             config = configure
         else:
             raise Exception('Could not convert {} (type "{}") to json.'.format(configure, type(configure)))
 
         if 'run' not in config:
-            raise Exception('Json file is missing "run" entry. Unable to build Bionetwork.')
+            raise Exception('Json file is missing "run" entry. Unable to build PointNetwork.')
         run_dict = config['run']
+        
+        # override the n_thread setting from the config file
+        if 'n_thread' in run_dict:
+            if n_thread is not None and n_thread != run_dict['n_thread']:
+                # give a warinig that the user is overriding the argument.
+                io.log_warning(
+                    f'Overriding n_thread setting in an argument ({n_thread}) with the value in config file ({run_dict["n_thread"]}).'
+                )
+            n_thread = run_dict['n_thread']
+        else:
+            if n_thread is None:
+                n_thread = 1  # default to 1 thread if not set in config or argument
+
 
         # Get network parameters
         # step time (dt) is set in the kernel and should be passed
         overwrite = run_dict['overwrite_output_dir'] if 'overwrite_output_dir' in run_dict else True
         print_time = run_dict['print_time'] if 'print_time' in run_dict else False
         dt = run_dict['dt']  # TODO: make sure dt exists
-        network = cls(graph, dt=dt, overwrite=overwrite)
+        network = cls(graph, dt=dt, overwrite=overwrite, n_thread=n_thread)
 
         if 'output_dir' in config['output']:
             network.output_dir = config['output']['output_dir']
 
         if 'block_run' in run_dict and run_dict['block_run']:
             if 'block_size' not in run_dict:
                 raise Exception('"block_run" is set to True but "block_size" not found.')
@@ -240,37 +240,28 @@
         graph.build_nodes()
 
         graph.io.log_info('Building recurrent connections')
         graph.build_recurrent_edges()
 
         for sim_input in inputs.from_config(config):
             node_set = graph.get_node_set(sim_input.node_set)
-            if sim_input.input_type == 'spikes':
+            if sim_input.input_type == 'spikes' and sim_input.module in ['nwb', 'csv', 'sonata']:
                 io.log_info('Build virtual cell stimulations for {}'.format(sim_input.name))
                 path = sim_input.params['input_file']
                 spikes = SpikeTrains.load(path=path, file_type=sim_input.module, **sim_input.params)
                 #spikes = spike_trains.SpikesInput.load(name=sim_input.name, module=sim_input.module,
                 #                                       input_type=sim_input.input_type, params=sim_input.params)
                 graph.add_spike_trains(spikes, node_set, network.get_spike_generator_params())
-
-            elif sim_input.input_type == 'current_clamp':
-                # TODO: Need to make this more robust
-                amp_times = sim_input.params.get('amplitude_times', [])
-                amp_values = sim_input.params.get('amplitude_values', [])
-
-                if 'delay' in sim_input.params:
-                    amp_times.append(sim_input.params['delay'])
-                    amp_values.append(sim_input.params['amp'])
-
-                    if 'duration' in sim_input.params:
-                        amp_times.append(sim_input.params['delay'] + sim_input.params['duration'])
-                        amp_values.append(0.0)
-
-                network.add_step_currents(amp_times, amp_values, node_set, sim_input.name)
-
+            
+            elif sim_input.module == 'IClamp':
+                network.add_mod(mods.IClampMod(input_type=sim_input.input_type, **sim_input.params))
+
+            elif sim_input.module == 'ecephys_probe':
+                network.add_mod(mods.PointECEphysUnitsModule(name=sim_input.name, **sim_input.params))
+            
             else:
                 graph.io.log_warning('Unknown input type {}'.format(sim_input.input_type))
 
         sim_reports = reports.from_config(config)
         for report in sim_reports:
             if report.module == 'spikes_report':
                 mod = mods.SpikesMod(**report.params)
```

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/property_map.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/property_map.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/pyfunction_cache.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/pyfunction_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/sonata_adaptors.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/sonata_adaptors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/pointnet/utils.py` & `bmtk-1.0.8/bmtk/simulator/pointnet/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/__init__.py` & `bmtk-1.0.8/bmtk/simulator/popnet/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/config.py` & `bmtk-1.0.8/bmtk/simulator/popnet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/popedge.py` & `bmtk-1.0.8/bmtk/simulator/popnet/popedge.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/popnetwork.py` & `bmtk-1.0.8/bmtk/simulator/popnet/popnetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/popnode.py` & `bmtk-1.0.8/bmtk/simulator/popnet/popnode.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/popsimulator.py` & `bmtk-1.0.8/bmtk/simulator/popnet/popsimulator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/popnet/utils.py` & `bmtk-1.0.8/bmtk/simulator/popnet/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/utils/__init__.py` & `bmtk-1.0.8/bmtk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
+__version__ = '1.0.8'
```

### Comparing `bmtk-1.0.7/bmtk/simulator/utils/simulation_inputs.py` & `bmtk-1.0.8/bmtk/simulator/utils/simulation_inputs.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/simulator/utils/simulation_reports.py` & `bmtk-1.0.8/bmtk/simulator/utils/simulation_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
     def avail_modules():
         return 'spikes_report'
 
     @classmethod
     def from_output_dict(cls, output_dict):
         params = {
             'spikes_file': output_dict.get('spikes_file', None),
+            'compression': output_dict.get('compression', 'gzip'),
             'spikes_file_csv': output_dict.get('spikes_file_csv', None),
             'spikes_file_nwb': output_dict.get('spikes_file_nwb', None),
             'spikes_sort_order': output_dict.get('spikes_sort_order', None),
             'tmp_dir': output_dict.get('output_dir', cls.default_dir),
             'cache_to_disk': output_dict.get('cache_to_disk', True)
         }
```

### Comparing `bmtk-1.0.7/bmtk/utils/__init__.py` & `bmtk-1.0.8/bmtk/utils/sonata/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import logging
-
-
+#
+from .edge import Edge, EdgeSet
+from .file import File
+from .node import Node, NodeSet
```

### Comparing `bmtk-1.0.7/bmtk/utils/compile_mechanisms/__main__.py` & `bmtk-1.0.8/bmtk/utils/compile_mechanisms/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/compile_mechanisms/compile_mechanisms.py` & `bmtk-1.0.8/bmtk/utils/compile_mechanisms/compile_mechanisms.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/create_environment/__main__.py` & `bmtk-1.0.8/bmtk/utils/create_environment/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/create_environment/create_environment.py` & `bmtk-1.0.8/bmtk/utils/create_environment/create_environment.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/create_environment/env_builder.py` & `bmtk-1.0.8/bmtk/utils/create_environment/env_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,16 @@
 
         self._simulation_config['output'] = output_section
 
     def _add_current_clamp(self, current_param):
         if current_param is None:
             return
         logger.info('Adding current clamp')
-
+        if 'node_set' not in current_param.keys():
+            current_param['node_set'] = 'all'
         iclamp_config = {
             "input_type": "current_clamp",
             "module": "IClamp",
             "node_set": current_param['node_set'],
             "gids": current_param.get('gids', 'all'),
             "amp": current_param['amp'],
             "delay": current_param['delay'],
```

### Comparing `bmtk-1.0.7/bmtk/utils/io/__init__.py` & `bmtk-1.0.8/bmtk/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/io/cell_vars.py` & `bmtk-1.0.8/bmtk/utils/io/cell_vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         #root_name = '/report/{}'.format(self._population) if self._population is not None else '/'
         var_grp = self._h5_handle.create_group('/mapping')
         # TODO: gids --> node_ids
         var_grp.create_dataset('gids', shape=(self._n_gids_all,), dtype=np.uint)
         # TODO: element_id --> element_ids
         var_grp.create_dataset('element_id', shape=(self._n_segments_all,), dtype=np.uint)
-        var_grp.create_dataset('element_pos', shape=(self._n_segments_all,), dtype=np.float)
+        var_grp.create_dataset('element_pos', shape=(self._n_segments_all,), dtype=float)
         var_grp.create_dataset('index_pointer', shape=(self._n_gids_all+1,), dtype=np.uint64)
         var_grp.create_dataset('time', data=[self.tstart, self.tstop, self.dt])
         # TODO: Let user determine value
         var_grp['time'].attrs['units'] = 'ms'
         for k, v in self._map_attrs.items():
             var_grp.create_dataset(k, shape=(self._n_segments_all,), dtype=type(v[0]))
 
@@ -172,25 +172,25 @@
 
         for var_name, data_tables in self._data_blocks.items():
             # If users are trying to save multiple variables in the same file put data table in its own /{var} group
             # (not sonata compliant). Otherwise the data table is located at the root
             data_grp = self._h5_handle if self._n_vars == 1 else self._h5_handle.create_group('/{}'.format(var_name))
             if self._buffer_data:
                 # Set up in-memory block to buffer recorded variables before writing to the dataset
-                data_tables.buffer_block = np.zeros((buffer_size, self._n_segments_local), dtype=np.float)
+                data_tables.buffer_block = np.zeros((buffer_size, self._n_segments_local), dtype=float)
                 data_tables.data_block = data_grp.create_dataset('data', shape=(n_steps, self._n_segments_all),
-                                                                 dtype=np.float, chunks=True)
+                                                                 dtype=float, chunks=True)
                 # TODO: Remove Variable name
                 data_tables.data_block.attrs['variable_name'] = var_name
                 if self._units is not None:
                     data_tables.data_block.attrs['units'] = self._units
             else:
                 # Since we are not buffering data, we just write directly to the on-disk dataset
                 data_tables.buffer_block = data_grp.create_dataset('data', shape=(n_steps, self._n_segments_all),
-                                                                   dtype=np.float, chunks=True)
+                                                                   dtype=float, chunks=True)
                 data_tables.buffer_block.attrs['variable_name'] = var_name
                 if self._units is not None:
                     data_tables.buffer_block.attrs['units'] = self._units
 
 
         self._is_initialized = True
 
@@ -266,15 +266,15 @@
 
                 time_ds = h5_tmp['mapping/time']
 
             mapping_grp = h5final.create_group('mapping')
             if time_ds:
                 mapping_grp.create_dataset('time', data=time_ds)
             element_id_ds = mapping_grp.create_dataset('element_id', shape=(total_seg_count,), dtype=np.uint)
-            el_pos_ds = mapping_grp.create_dataset('element_pos', shape=(total_seg_count,), dtype=np.float)
+            el_pos_ds = mapping_grp.create_dataset('element_pos', shape=(total_seg_count,), dtype=float)
             gids_ds = mapping_grp.create_dataset('gids', shape=(total_gid_count,), dtype=np.uint)
             index_pointer_ds = mapping_grp.create_dataset('index_pointer', shape=(total_gid_count+1,), dtype=np.uint)
             for k, v in self._map_attrs.items():
                 mapping_grp.create_dataset(k, shape=(total_seg_count,), dtype=type(v[0]))
 
             # combine the /mapping datasets
             for i, h5_tmp in enumerate(tmp_h5_handles):
@@ -294,15 +294,15 @@
                 index_pointer_ds[beg:(end+1)] = update_index
 
 
             # combine the /var/data datasets
             for var_name in self._variables:
                 data_name = '/data' if self._n_vars == 1 else '/{}/data'.format(var_name)
                 # data_name = '/{}/data'.format(var_name)
-                var_data = h5final.create_dataset(data_name, shape=(self._total_steps, total_seg_count), dtype=np.float)
+                var_data = h5final.create_dataset(data_name, shape=(self._total_steps, total_seg_count), dtype=float)
                 var_data.attrs['variable_name'] = var_name
                 for i, h5_tmp in enumerate(tmp_h5_handles):
                     beg, end = seg_ranges[i]
                     var_data[:, beg:end] = h5_tmp[data_name]
 
             for tmp_file in self._tmp_files:
                 os.remove(tmp_file)
```

### Comparing `bmtk-1.0.7/bmtk/utils/io/firing_rates.py` & `bmtk-1.0.8/bmtk/utils/io/firing_rates.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/io/ioutils.py` & `bmtk-1.0.8/bmtk/utils/io/ioutils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/io/spike_trains.py` & `bmtk-1.0.8/bmtk/utils/io/spike_trains.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
                         interval = -np.log(1.0 - np.random.uniform()) / self._firing_rate
                         c_time += interval
                         gid_list.append(gid)
                         times_list.append(c_time)
 
             with h5py.File(file_name, 'w') as h5:
                 h5.create_dataset('/spikes/gids', data=gid_list, dtype=np.uint)
-                h5.create_dataset('/spikes/timestamps', data=times_list, dtype=np.float)
+                h5.create_dataset('/spikes/timestamps', data=times_list, dtype=float)
                 h5['/spikes'].attrs['sorting'] = 'by_gid'
 
         else:
             raise NotImplementedError
 
 
 class SpikesInput(object):
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/compartment/compartment_reader.py` & `bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,19 +53,19 @@
         return 'node_ids'
 
     def get_population(self, population, default=None):
         raise NotImplementedError()
 
     def units(self, population=None):
         return get_attribute_h5(self.data_ds, 'units', None)
-        #return self.data_ds.attrs.get('units', None)
+        # return self.data_ds.attrs.get('units', None)
 
     def variable(self, population=None):
         return get_attribute_h5(self.data_ds, 'variable', None)
-        #return self.data_ds.attrs.get('variable', None)
+        # return self.data_ds.attrs.get('variable', None)
 
     def tstart(self, population=None):
         return self._t_start
 
     def tstop(self, population=None):
         return self._t_stop
 
@@ -93,16 +93,16 @@
         else:
             return self._mapping['element_pos'][self._get_index(node_id)]#[indx_beg:indx_end]
 
     def element_ids(self, node_id=None, population=None):
         if node_id is None:
             return self._mapping['element_ids'][()]
         else:
-            #indx_beg, indx_end = self._get_index(node_id)
-            #return self._mapping['element_ids'][self._get_index(node_id)]#[indx_beg:indx_end]
+            # indx_beg, indx_end = self._get_index(node_id)
+            # return self._mapping['element_ids'][self._get_index(node_id)]#[indx_beg:indx_end]
             return self._mapping['element_ids'][self._get_index(node_id)]
 
     def n_elements(self, node_id=None, population=None):
         return len(self.element_pos(node_id))
 
     def data(self, node_id=None, population=None, time_window=None, sections='all', **opts):
         # filtered_data = self._data_grp
@@ -126,15 +126,15 @@
         if time_window is None:
             time_slice = slice(0, self._n_steps)
         else:
             if len(time_window) != 2:
                 raise Exception('Invalid time_window, expecting tuple [being, end].')
 
             window_beg = max(int((time_window[0] - self.tstart()) / self.dt()), 0)
-            window_end = min(int((time_window[1] - self.tstart()) / self.dt()), self._n_steps / self.dt())
+            window_end = min(int((time_window[1] - self.tstart()) / self.dt()), self._n_steps)
             time_slice = slice(window_beg, window_end)
 
         filtered_data = np.array(self._data_grp[time_slice, gid_slice])
         return filtered_data if multi_compartments else filtered_data[:]
 
     def custom_columns(self, population=None):
         return {k: v[()] for k,v in self._custom_cols.items()}
@@ -162,16 +162,16 @@
     def node_ids_ds(self):
         return 'gids'
 
     def element_ids(self, node_id=None, population=None):
         if node_id is None:
             return self._mapping['element_id'][()]
         else:
-            #indx_beg, indx_end = self._get_index(node_id)
-            #return self._mapping['element_id'][self._get_index(node_id)]#[indx_beg:indx_end]
+            # indx_beg, indx_end = self._get_index(node_id)
+            # return self._mapping['element_id'][self._get_index(node_id)]#[indx_beg:indx_end]
             return self._mapping['element_id'][self._get_index(node_id)]  # [indx_beg:indx_end]
 
 
 class CompartmentReaderVer01(CompartmentReaderABC):
     def __init__(self, filename, mode='r', **params):
         self._h5_handle = h5py.File(filename, mode)
         self._h5_root = self._h5_handle[params['h5_root']] if 'h5_root' in params else self._h5_handle['/']
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/compartment/compartment_report.py` & `bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_report.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/reports/compartment/compartment_writer.py` & `bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         """
         def __init__(self, var_name):
             self.var_name = var_name
             # If buffering data, buffer_block will be an in-memory array and will write to data_block during when
             # filled. If not buffering buffer_block is an hdf5 dataset and data_block is ignored
             self.data_block = None
             self.buffer_block = None
+            self.block_window = (0.0, 10e20)
 
     def __init__(self, parent, population, variable=None, units=None, tstart=0.0, tstop=1.0, dt=0.01, n_steps=None,
                  buffer_size=0, **kwargs):
         self._h5_base = None
         self._parent = parent
 
         self._population = population
@@ -61,15 +62,15 @@
         self._mapping_element_ids = []  # sections
         self._mapping_element_pos = []  # segments
         self._mapping_index = [0]  # index_pointer
 
         self._buffer_size = buffer_size
         self._buffer_data = buffer_size > 0
         self._data_block = self.DataTable(self._variable)
-        self._last_save_indx = 0  # for buffering, used to keep track of last timestep data was saved to disk
+        # self._last_save_indx = 0  # for buffering, used to keep track of last timestep data was saved to disk
 
         self._buffer_block_size = 0
         self._total_steps = 0
 
         # Keep track of gids across the different ranks
         self._n_gids_all = 0
         self._n_gids_local = 0
@@ -184,90 +185,113 @@
         var_grp['element_ids'][self._seg_offset_beg:self._seg_offset_end] = self._mapping_element_ids
         var_grp['element_pos'][self._seg_offset_beg:self._seg_offset_end] = self._mapping_element_pos
         var_grp['index_pointer'][self._gids_beg:(self._gids_end+1)] = self._mapping_index
         for k, v in self._element_data.items():
             var_grp[k][self._seg_offset_beg:self._seg_offset_end] = v
 
         self._total_steps = n_steps
+        self._buffer_size = np.min((self._total_steps, self._buffer_size))
         self._buffer_block_size = self._buffer_size
 
         if not self._buffer_data:
             # If data is not being buffered and instead written to the main block, we have to add a rank offset
             # to the gid offset
             for gid, gid_offset in self._gid_map.items():
                 self._gid_map[gid] = (gid_offset[0] + self._seg_offset_beg, gid_offset[1] + self._seg_offset_beg)
 
-        
         if self._buffer_data:
             # Set up in-memory block to buffer recorded variables before writing to the dataset
             self._data_block.buffer_block = np.zeros((self._buffer_size, self._n_segments_local), dtype=float)
 
             self._data_block.data_block = base_grp.create_dataset('data', shape=(self.n_steps(), self._n_segments_all),
                                                                   dtype=float, chunks=True)
             if self._variable is not None:
                 self._data_block.data_block.attrs['variable'] = self._variable
 
             if self._units is not None:
                 self._data_block.data_block.attrs['units'] = self._units
 
+            self._data_block.block_window = (0, self._buffer_block_size)
+
         else:
             # Since we are not buffering data, we just write directly to the on-disk dataset
-            self._data_block.buffer_block = base_grp.create_dataset('data', shape=(self.n_steps(), self._n_segments_all),
-                                                               dtype=float, chunks=True)
+            self._data_block.buffer_block = base_grp.create_dataset(
+                'data',
+                shape=(self.n_steps(), self._n_segments_all),
+                dtype=float,
+                chunks=True
+            )
             if self._variable is not None:
                 self._data_block.buffer_block.attrs['variable'] = self._variable
 
             if self._units is not None:
                 self._data_block.buffer_block.attrs['units'] = self._units
 
         self._is_initialized = True
 
+    def _reset_buffer_window(self, tstep):
+        blk_beg = int(tstep/self._buffer_size)*self._buffer_size
+        blk_end = blk_beg + self._buffer_size
+        self._data_block.block_window = (blk_beg, blk_end)
+
     def record_cell(self, node_id, vals, tstep, population=None):
         """Record cell parameters.
 
         :param gid: gid of cell.
         :param var_name: name of variable being recorded.
         :param seg_vals: list of all segment values
         :param tstep: time step
         """
         self.initialize()
         gid_beg, gid_end = self._gid_map[node_id]
         buffer_block = self._data_block.buffer_block
-        update_index = (tstep - self._last_save_indx)
-        buffer_block[update_index, gid_beg:gid_end] = vals
+
+        if not self._buffer_data:
+            buffer_block[tstep, gid_beg:gid_end] = vals
+
+        elif self._data_block.block_window[0] <= tstep < self._data_block.block_window[1]:
+            update_index = tstep - self._data_block.block_window[0]
+            buffer_block[update_index, gid_beg:gid_end] = vals
+
+        else:
+            self.flush()
+            self._reset_buffer_window(tstep)
+            update_index = tstep - self._data_block.block_window[0]
+            buffer_block[update_index, gid_beg:gid_end] = vals
 
     def record_cell_block(self, node_id, vals, beg_step, end_step, population=None):
         """Save cell parameters one block at a time
 
         :param gid: gid of cell.
         :param var_name: name of variable being recorded.
         :param seg_vals: A vector/matrix of values being recorded
         """
         self.initialize()
         gid_beg, gid_end = self._gid_map[node_id]
         buffer_block = self._data_block.buffer_block
         if isinstance(vals, list) or vals.ndim == 1:
             buffer_block[:, gid_beg] = vals
-            #buffer_block[beg_step:end_step, gid_beg:gid_end] = vals
+            # buffer_block[beg_step:end_step, gid_beg:gid_end] = vals
         else:
             buffer_block[:, gid_beg:gid_end] = vals
 
     def flush(self):
         """Move data from memory to dataset"""
         if self._buffer_data:
-            blk_beg = self._last_save_indx
-            blk_end = blk_beg + self._buffer_block_size
+            # blk_beg = self._last_save_indx
+            # blk_end = blk_beg + self._buffer_block_size
+            blk_beg = self._data_block.block_window[0]
+            blk_end = self._data_block.block_window[1]
             if blk_end > self._total_steps:
                 # Need to handle the case that simulation doesn't end on a block step
                 blk_end = blk_beg + self._total_steps - blk_beg
 
             block_size = blk_end - blk_beg
-            self._last_save_indx += block_size
-
             self._data_block.data_block[blk_beg:blk_end, :] = self._data_block.buffer_block[:block_size, :]
+            self._reset_buffer_window(blk_end+1)
 
     def close(self):
         # Let the parent take care of this
         pass
 
     def merge(self):
         # Let the parent take care of this
@@ -295,15 +319,15 @@
 
         self._mpi_rank = kwargs.get('mpi_rank', rank)
         self._mpi_size = kwargs.get('mpi_size', nhosts)
 
         self._final_fpath = file_path  # name of file being writen too.
         self._cache_dir = cache_dir or os.path.dirname(os.path.abspath(file_path))  # used for mulitple ranks
         self._base_name = os.path.basename(file_path)  # make sure file names don't clash if there are multiple reports
-        self._interm_fpath = self._get_iterm_fpath() # In certain cases (parallelized simulation) split the final file by rank.
+        self._interm_fpath = self._get_iterm_fpath()  # In certain cases (parallelized simulation) split the final file by rank.
 
     def _get_iterm_fpath(self):
         if self._mpi_size > 1:
             return self.temp_files[self._mpi_rank]
         else:
             return self._final_fpath
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/compartment/core.py` & `bmtk-1.0.8/bmtk/utils/reports/compartment/core.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/reports/compartment/plotting.py` & `bmtk-1.0.8/bmtk/utils/reports/compartment/plotting.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/reports/current_writer.py` & `bmtk-1.0.8/bmtk/utils/reports/current_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,26 +113,26 @@
         base_grp = self.h5_base
 
         self._total_steps = n_steps
         self._buffer_block_size = self._buffer_size
 
         if self._buffer_data:
             # Set up in-memory block to buffer recorded variables before writing to the dataset.
-            self._data_block.buffer_block = np.zeros((self._buffer_size, self._num_currents), dtype=np.float)
+            self._data_block.buffer_block = np.zeros((self._buffer_size, self._num_currents), dtype=float)
 
             self._data_block.data_block = base_grp.create_dataset('data', shape=(self.n_steps(), self._num_currents),
-                                                                  dtype=np.float, chunks=True)
+                                                                  dtype=float, chunks=True)
 
             if self._units is not None:
                 self._data_block.data_block.attrs['units'] = self._units
 
         else:
             # Since we are not buffering data, we just write directly to the on-disk dataset.
             self._data_block.buffer_block = base_grp.create_dataset('data', shape=(self.n_steps(), self._n_segments_all),
-                                                               dtype=np.float, chunks=True)
+                                                               dtype=float, chunks=True)
 
             if self._units is not None:
                 self._data_block.buffer_block.attrs['units'] = self._units
 
         self._is_initialized = True
 
     def record_clamps(self, vals, tstep):
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/__init__.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/core.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/core.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/plotting.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/plotting.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_train_buffer.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -848,15 +848,15 @@
 
             df = pd.read_csv(file_name, sep=' ', names=[col_timestamps, col_population, col_node_ids])
             if populations is not None:
                 df = df[df[col_population].isin(populations)]
 
             if not with_population_col:
                 df.drop(col_population, axis=1)
-            ret_df = df if ret_df is None else ret_df.append(df)
+            ret_df = df if ret_df is None else pd.concat([ret_df, df])
 
         if ret_df is not None:
             # pandas doesn't always do a good job of reading in the correct dtype for each column
             ret_df = ret_df.astype({col_timestamps: float, col_node_ids: np.int64})
 
             if sort_order == SortOrder.by_time:
                 ret_df = ret_df.sort_values(col_timestamps)
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_train_readers.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,16 @@
             self._units_maps[pop_name] = pop_units
 
     def _build_node_index(self):
         self._indexed = False
         for pop_name, pop_grp in self._population_map.items():
             sort_order = self._population_sorting_map[pop_name]
             nodes_indices = {}
-            node_ids_ds = pop_grp[self._DATASET_node_ids]
+            # loop on h5 is slow, so convert it to np before the loop.
+            node_ids_ds = np.array(pop_grp[self._DATASET_node_ids])
             if sort_order == SortOrder.by_id:
                 indx_beg = 0
                 last_id = node_ids_ds[0]
                 for indx, cur_id in enumerate(node_ids_ds):
                     if cur_id != last_id:
                         # nodes_indices[last_id] = np.arange(indx_beg, indx)
                         nodes_indices[last_id] = slice(indx_beg, indx)
@@ -600,15 +601,15 @@
             return spiketimes
         except KeyError:
             return []
 
     def to_dataframe(self, node_ids=None, populations=None, time_window=None, sort_order=SortOrder.none, **kwargs):
         if self._spikes_df is None:
             self._spikes_df = pd.DataFrame({
-                col_timestamps: pd.Series(dtype=np.float),
+                col_timestamps: pd.Series(dtype=float),
                 col_population: pd.Series(dtype=np.string_),
                 col_node_ids: pd.Series(dtype=np.uint64)
             })
             for node_id, node_grp in self._trial_grp.items():
                 timestamps = node_grp['data'][()]
                 node_df = pd.DataFrame({
                     col_timestamps: timestamps,
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_trains.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains.py`

 * *Files 13% similar despite different names*

```diff
@@ -139,28 +139,28 @@
     def add(self, node_ids, firing_rate, population=None, times=(0.0, 1.0), abs_ref=0, tau_ref=0):
         """
         :param firing_rate: Scalar stationary firing rate or array of values for inhomogeneous (Hz)
         :param times: Start and end time for spike train (s)
         :param abs_ref: Absolute refractory period (s)
         :param tau_ref: Relative refractory period time constant for exponential recovery (s)
         """
+        if tau_ref < 0:
+            raise ValueError('Refractory period time constant (sec) cannot be negative.')
+        if abs_ref < 0:
+            raise ValueError('Absolute refractory period (sec) cannot be negative.')
         if isinstance(node_ids, string_types):
             # if user passes in path to nodes.h5 file count number of nodes
             node_ids = get_node_ids(node_ids, population)
         if np.isscalar(node_ids):
             # In case user passes in single node_id
             node_ids = [node_ids]
         if np.isscalar(firing_rate):
             self._build_fixed_fr(node_ids, population, firing_rate, times, abs_ref, tau_ref)
         elif isinstance(firing_rate, (list, np.ndarray)):
             self._build_inhomogeneous_fr(node_ids, population, firing_rate, times, abs_ref, tau_ref)
-        if tau_ref < 0:
-            raise ValueError('Refractory period time constant (sec) cannot be negative.')
-        if abs_ref < 0:
-            raise ValueError('Absolute refractory period (sec) cannot be negative.')
 
     def time_range(self, population=None):
         df = self.to_dataframe(populations=population, with_population_col=False)
         timestamps = df['timestamps']
         return np.min(timestamps), np.max(timestamps)
 
     def _build_fixed_fr(self, node_ids, population, fr, times, abs_ref, tau_ref):
@@ -171,49 +171,58 @@
             tstart = times[0]
             tstop = times[-1]
             if tstart >= tstop:
                 raise ValueError('Invalid start and stop times.')
         if fr < 0:
             raise ValueError('Firing rates must not be negative.')
 
+        # If there are refractory properties, correct starting firing rate and check firing limit
+        if abs_ref!=0 or tau_ref!=0:
+            max_fr_lim, p = fr_corr(abs_ref, tau_ref)
+            if fr > max_fr_lim:
+                raise ValueError(f'Cannot achieve firing rate above {max_fr_lim} with these absolute'
+                                 f' and relative refractory properties. Also consider using'
+                                 f' the GammaSpikeGenerator instead.')
+            fr = p(fr)
+
         #rs2 = np.random.RandomState(0)
         count = 0
         for node_id in node_ids:
             c_time = tstart
             while True:
                 interval = -np.log(1.0 - np.random.uniform()) / fr
                 preceding_time = c_time
                 c_time += interval
                 if c_time > tstop:
                     break
                 if tau_ref != 0:
-                    w = 1 - np.exp(-(c_time-preceding_time-abs_ref)/tau_ref)
+                    w = 1 - np.exp(-(interval-abs_ref)/tau_ref)
                 else:
                     w = 1  # To avoid divide by zero warning
                 if abs_ref != 0:
                     w = w*(interval>abs_ref)
                 #if (w == 1) or (rs2.uniform() < w):
                 if (w == 1) or (np.random.uniform() < w):
                     self.add_spike(node_id=node_id, population=population, timestamp=c_time*self.output_conversion)
                     count = count+1
-        if (abs_ref != 0) or (tau_ref != 0):
-            fr_actual = count/(tstop-tstart)/len(node_ids)
-            str = (f'When using refractory periods, the actual firing rate ({fr_actual} spk/s) may be less than '
-                   f'the desired firing rate ({fr} spk/s), particularly for high rates, and saturates at 1/abs_ref. '
-                   'See also GammaSpikeGenerator for more exact firing rates with refractory periods.')
-            warnings.warn(str)
 
     def _build_inhomogeneous_fr(self, node_ids, population, fr, times, abs_ref, tau_ref):
         if np.min(fr) < 0:
             raise ValueError('Firing rates must not be negative')
         if len(fr) != len(times):
             raise ValueError('If using a time series for firing rate, times must be an array of equal length')
 
         max_fr = np.max(fr)
 
+        max_fr_lim, p = fr_corr(abs_ref, tau_ref)
+        if max_fr > max_fr_lim:
+            raise ValueError(f'Cannot achieve firing rate above {max_fr_lim} with these absolute and relative refractory properties')
+
+        fr = p(fr)
+
         times = times
         tstart = times[0]
         tstop = times[-1]
 
         for node_id in node_ids:
             c_time = tstart
             time_indx = 0
@@ -221,15 +230,15 @@
                 # Using the pruning method, see Dayan and Abbott Ch 2
                 interval = -np.log(1.0 - np.random.uniform()) / max_fr
                 preceding_time = c_time
                 c_time += interval
                 if c_time > tstop:
                     break
                 if tau_ref != 0:
-                    w = 1 - np.exp(-(c_time-preceding_time-abs_ref)/tau_ref)
+                    w = 1 - np.exp(-(interval-abs_ref)/tau_ref)
                 else:
                     w = 1  # To avoid divide by zero warning
                 if abs_ref != 0:
                     w = w * (interval > abs_ref)
                 # A spike occurs at t_i, find index j st times[j-1] < t_i < times[j], and interpolate the firing rates
                 # using fr[j-1] and fr[j]
                 while times[time_indx] <= c_time:
@@ -237,18 +246,14 @@
 
                 fr_i = _interpolate_fr(c_time, times[time_indx-1], times[time_indx],
                                        fr[time_indx-1], fr[time_indx])
 
                 if not fr_i/max_fr*w < np.random.uniform():
                     self.add_spike(node_id=node_id, population=population, timestamp=c_time*self.output_conversion)
 
-        if (abs_ref != 0) or (tau_ref != 0):
-            str = ('When using refractory periods, the actual firing rates may be less than '
-                   'the desired firing rates, particularly for high rates, and saturates at 1/abs_ref.')
-            warnings.warn(str)
 
 class GammaSpikeGenerator(SpikeGenerator):
     """ A Class for generating spike-trains based on a gamma-distributed renewal process.
     """
     def __init__(self, population=None, seed=None, output_units='ms', **kwargs):
         super(GammaSpikeGenerator, self).__init__(population, seed, output_units, **kwargs)
 
@@ -300,7 +305,28 @@
                 if c_time > tstop:
                     break
                 self.add_spike(node_id=node_id, population=population, timestamp=c_time*self.output_conversion)
 
 def _interpolate_fr(t, t0, t1, fr0, fr1):
     # Used to interpolate the firing rate at time t from a discrete list of firing rates
     return fr0 + (fr1 - fr0)*(t - t0)/(t1 - t0)
+
+def fr_corr(abs_ref, tau_ref):
+    # Firing rate correction for lost spikes
+    if tau_ref != 0:
+        def f(fr_before, abs_ref=abs_ref, tau_ref=tau_ref):
+            return (np.exp(-fr_before * abs_ref) - \
+                    fr_before * np.exp(abs_ref / tau_ref) * tau_ref /
+                    (fr_before * tau_ref + 1) * \
+                    (np.exp(-(fr_before + 1 / tau_ref) * abs_ref))) * fr_before
+    else:
+        def f(fr_before, abs_ref=abs_ref):
+            return np.exp(-fr_before * abs_ref) * fr_before
+
+    fr_befores = np.logspace(0, 3, 40)
+    fr_afters = f(fr_befores)
+    max_fr_lim = np.max(fr_afters)
+    max_ind = np.argmax(fr_afters)
+
+    z = np.polyfit(fr_afters[:max_ind], fr_befores[:max_ind], 10)
+    p = np.poly1d(z)
+    return max_fr_lim, p
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/spike_trains_api.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,26 @@
         :param time_window:
         :param sort_order:
         :param kwargs:
         :return:
         """
         raise NotImplementedError()
 
-    def to_sonata(self, path, mode='w', sort_order=SortOrder.none, **kwargs):
+    def to_sonata(self, path, mode='w', sort_order=SortOrder.none, compression='gzip', **kwargs):
         """Write current spike-trains to a sonata hdf5 file
 
         :param path:
         :param mode:
         :param sort_order:
+        :param compression: Compression algorithm for h5py's dataset_create. 'gzip' is default
+                            Only applied to h5 spike data.
         :param kwargs:
         :return:
         """
-        write_sonata(path=path, spiketrain_reader=self, mode=mode, sort_order=sort_order, **kwargs)
+        write_sonata(path=path, spiketrain_reader=self, mode=mode, sort_order=sort_order, compression=compression, **kwargs)
 
     def to_csv(self, path, mode='w', sort_order=SortOrder.none, **kwargs):
         """Write spikes to csv file
 
         :param path:
         :param mode:
         :param sort_order:
```

### Comparing `bmtk-1.0.7/bmtk/utils/reports/spike_trains/spikes_file_writers.py` & `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spikes_file_writers.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,20 @@
 
 from .core import SortOrder, csv_headers, col_population, find_conversion
 from .core import MPI_rank, comm_barrier
 from bmtk.utils.sonata.utils import add_hdf5_magic, add_hdf5_version
 
 
 def write_sonata(path, spiketrain_reader, mode='w', sort_order=SortOrder.none, units='ms',
-                 population_renames=None, **kwargs):
+                 population_renames=None, compression='gzip', **kwargs):
+    
+    # make sure to take care of 'none' or 'None' compression
+    if isinstance(compression, str):
+        if compression.lower() == 'none':
+            compression = None
     path_dir = os.path.dirname(path)
     if MPI_rank == 0 and path_dir and not os.path.exists(path_dir):
         os.makedirs(path_dir)
 
     spiketrain_reader.flush()
     comm_barrier()
 
@@ -56,22 +61,22 @@
         pop_df = spiketrain_reader.to_dataframe(populations=pop_name, with_population_col=False, sort_order=sort_order,
                                                 on_rank='root')
         if MPI_rank == 0:
             spikes_pop_grp = spikes_root.create_group(pop_name)
             if sort_order != SortOrder.unknown:
                 spikes_pop_grp.attrs['sorting'] = sort_order.value
 
-            spikes_pop_grp.create_dataset('timestamps', data=pop_df['timestamps'])
+            spikes_pop_grp.create_dataset('timestamps', data=pop_df['timestamps'], compression=compression)
             spikes_pop_grp['timestamps'].attrs['units'] = spiketrain_reader.units()
-            spikes_pop_grp.create_dataset('node_ids', data=pop_df['node_ids'])
+            spikes_pop_grp.create_dataset('node_ids', data=pop_df['node_ids'], compression=compression)
     comm_barrier()
 
 
 def write_sonata_itr(path, spiketrain_reader, mode='w', sort_order=SortOrder.none, units='ms', population_renames=None,
-                     **kwargs):
+                     compression='gzip', **kwargs):
     path_dir = os.path.dirname(path)
     if MPI_rank == 0 and path_dir and not os.path.exists(path_dir):
         os.makedirs(path_dir)
 
     spiketrain_reader.flush()
     comm_barrier()
 
@@ -89,17 +94,17 @@
             continue
 
         if MPI_rank == 0:
             spikes_grp = spikes_root.create_group('{}'.format(population_renames.get(pop_name, pop_name)))
             if sort_order != SortOrder.unknown:
                 spikes_grp.attrs['sorting'] = sort_order.value
 
-            timestamps_ds = spikes_grp.create_dataset('timestamps', shape=(n_spikes,), dtype=np.float64)
+            timestamps_ds = spikes_grp.create_dataset('timestamps', shape=(n_spikes,), dtype=np.float64, compression=compression)
             timestamps_ds.attrs['units'] = units
-            node_ids_ds = spikes_grp.create_dataset('node_ids', shape=(n_spikes,), dtype=np.uint64)
+            node_ids_ds = spikes_grp.create_dataset('node_ids', shape=(n_spikes,), dtype=np.uint64, compression=compression)
 
         for i, spk in enumerate(spiketrain_reader.spikes(populations=pop_name, sort_order=sort_order)):
             if MPI_rank == 0:
                 timestamps_ds[i] = spk[0]*conv_factor
                 node_ids_ds[i] = spk[2]
 
     comm_barrier()
```

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/default_config.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/default_config.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/bionet/templates/Biophys1.hoc` & `bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/Biophys1.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/filternet/run_filternet.py` & `bmtk-1.0.8/bmtk/utils/scripts/filternet/run_filternet.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json` & `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/scripts/sonata.circuit_config.json` & `bmtk-1.0.8/bmtk/utils/scripts/sonata.circuit_config.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sim_setup.py` & `bmtk-1.0.8/bmtk/utils/sim_setup.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/__init__.py` & `bmtk-1.0.8/bmtk/utils/sonata/config/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,10 +16,8 @@
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-from .edge import Edge, EdgeSet
-from .file import File
-from .node import Node, NodeSet
+from .sonata_config import SonataConfig, from_dict, from_json, from_yaml, copy_config
```

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/column_property.py` & `bmtk-1.0.8/bmtk/utils/sonata/column_property.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/config/__init__.py` & `bmtk-1.0.8/bmtk/simulator/bionet/modules/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,17 @@
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-from .sonata_config import SonataConfig, from_dict, from_json, from_yaml, copy_config
+from .ecp import EcpMod
+from .record_cellvars import MembraneReport, SomaReport
+from .record_spikes import SpikesMod
+from .xstim import XStimMod
+from .save_synapses import SaveSynapses
+from .record_netcons import NetconReport
+from .record_clamp import ClampReport
+from .iclamp import IClampMod
+from .comsol import ComsolMod
+from .ecephys_module import BioECEphysUnitsModule
```

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/config/config_schema.json` & `bmtk-1.0.8/bmtk/utils/sonata/config/config_schema.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/config/sonata_config.py` & `bmtk-1.0.8/bmtk/utils/sonata/config/sonata_config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/edge.py` & `bmtk-1.0.8/bmtk/utils/sonata/edge.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/file.py` & `bmtk-1.0.8/bmtk/utils/sonata/file.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/file_root.py` & `bmtk-1.0.8/bmtk/utils/sonata/file_root.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/group.py` & `bmtk-1.0.8/bmtk/utils/sonata/group.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/node.py` & `bmtk-1.0.8/bmtk/utils/sonata/node.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/population.py` & `bmtk-1.0.8/bmtk/utils/sonata/population.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/types_table.py` & `bmtk-1.0.8/bmtk/utils/sonata/types_table.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk/utils/sonata/utils.py` & `bmtk-1.0.8/bmtk/utils/sonata/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.7/bmtk.egg-info/PKG-INFO` & `bmtk-1.0.8/bmtk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Brain Modeling Toolkit
 Home-page: https://github.com/AllenInstitute/bmtk
 Author: Kael Dai
 Author-email: kaeld@alleninstitute.org
 License: UNKNOWN
 Keywords: neuroscience,scientific,modeling,simulation
 Platform: any
```

### Comparing `bmtk-1.0.7/bmtk.egg-info/SOURCES.txt` & `bmtk-1.0.8/bmtk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,18 @@
 bmtk/simulator/bionet/import3d/import3d_sec.hoc
 bmtk/simulator/bionet/import3d/read_morphml.hoc
 bmtk/simulator/bionet/import3d/read_nlcda.hoc
 bmtk/simulator/bionet/import3d/read_nlcda3.hoc
 bmtk/simulator/bionet/import3d/read_nts.hoc
 bmtk/simulator/bionet/import3d/read_swc.hoc
 bmtk/simulator/bionet/modules/__init__.py
+bmtk/simulator/bionet/modules/comsol.py
+bmtk/simulator/bionet/modules/ecephys_module.py
 bmtk/simulator/bionet/modules/ecp.py
+bmtk/simulator/bionet/modules/iclamp.py
 bmtk/simulator/bionet/modules/record_cellvars.py
 bmtk/simulator/bionet/modules/record_clamp.py
 bmtk/simulator/bionet/modules/record_netcons.py
 bmtk/simulator/bionet/modules/record_spikes.py
 bmtk/simulator/bionet/modules/save_synapses.py
 bmtk/simulator/bionet/modules/sim_module.py
 bmtk/simulator/bionet/modules/xstim.py
@@ -108,14 +111,20 @@
 bmtk/simulator/core/node_population.py
 bmtk/simulator/core/node_sets.py
 bmtk/simulator/core/pyfunction_cache.py
 bmtk/simulator/core/simulation_config.py
 bmtk/simulator/core/simulation_config_validator.py
 bmtk/simulator/core/simulator.py
 bmtk/simulator/core/simulator_network.py
+bmtk/simulator/core/modules/__init__.py
+bmtk/simulator/core/modules/ecephys_module.py
+bmtk/simulator/core/modules/iclamp.py
+bmtk/simulator/core/modules/ndx-aibs-ecephys.extension.yaml
+bmtk/simulator/core/modules/ndx-aibs-ecephys.namespace.yaml
+bmtk/simulator/core/modules/simulator_module.py
 bmtk/simulator/core/sonata_reader/__init__.py
 bmtk/simulator/core/sonata_reader/edge_adaptor.py
 bmtk/simulator/core/sonata_reader/network_reader.py
 bmtk/simulator/core/sonata_reader/node_adaptor.py
 bmtk/simulator/core/sonata_schemas/config_schema.json
 bmtk/simulator/filternet/__init__.py
 bmtk/simulator/filternet/cell.py
@@ -132,14 +141,15 @@
 bmtk/simulator/filternet/default_setters/__init__.py
 bmtk/simulator/filternet/default_setters/cell_loaders.py
 bmtk/simulator/filternet/lgnmodel/__init__.py
 bmtk/simulator/filternet/lgnmodel/cellmetrics.py
 bmtk/simulator/filternet/lgnmodel/cellmodel.py
 bmtk/simulator/filternet/lgnmodel/cursor.py
 bmtk/simulator/filternet/lgnmodel/fitfuns.py
+bmtk/simulator/filternet/lgnmodel/gaborfilter.py
 bmtk/simulator/filternet/lgnmodel/kernel.py
 bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py
 bmtk/simulator/filternet/lgnmodel/lgnmodel1.py
 bmtk/simulator/filternet/lgnmodel/linearfilter.py
 bmtk/simulator/filternet/lgnmodel/lnunit.py
 bmtk/simulator/filternet/lgnmodel/make_cell_list.py
 bmtk/simulator/filternet/lgnmodel/movie.py
@@ -172,14 +182,16 @@
 bmtk/simulator/pointnet/pyfunction_cache.py
 bmtk/simulator/pointnet/sonata_adaptors.py
 bmtk/simulator/pointnet/utils.py
 bmtk/simulator/pointnet/default_setters/__init__.py
 bmtk/simulator/pointnet/default_setters/synapse_models.py
 bmtk/simulator/pointnet/default_setters/synaptic_weights.py
 bmtk/simulator/pointnet/modules/__init__.py
+bmtk/simulator/pointnet/modules/ecephys_module.py
+bmtk/simulator/pointnet/modules/iclamp.py
 bmtk/simulator/pointnet/modules/multimeter_reporter.py
 bmtk/simulator/pointnet/modules/record_spikes.py
 bmtk/simulator/popnet/__init__.py
 bmtk/simulator/popnet/config.py
 bmtk/simulator/popnet/popedge.py
 bmtk/simulator/popnet/popnetwork.py
 bmtk/simulator/popnet/popnode.py
@@ -187,14 +199,15 @@
 bmtk/simulator/popnet/sonata_adaptors.py
 bmtk/simulator/popnet/utils.py
 bmtk/simulator/utils/__init__.py
 bmtk/simulator/utils/simulation_inputs.py
 bmtk/simulator/utils/simulation_reports.py
 bmtk/utils/__init__.py
 bmtk/utils/hdf5_helper.py
+bmtk/utils/lazy_property.py
 bmtk/utils/sim_setup.py
 bmtk/utils/compile_mechanisms/__init__.py
 bmtk/utils/compile_mechanisms/__main__.py
 bmtk/utils/compile_mechanisms/compile_mechanisms.py
 bmtk/utils/create_environment/__init__.py
 bmtk/utils/create_environment/__main__.py
 bmtk/utils/create_environment/create_environment.py
```

### Comparing `bmtk-1.0.7/setup.py` & `bmtk-1.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         'numpy',
         'six',
         'h5py',
         'matplotlib',
         'enum; python_version <= "2.7"',
         'scipy',
         'scikit-image',  # Only required for filternet, consider making optional
-        'sympy'  # For FilterNet
+        'sympy',  # For FilterNet
+        'pynrrd'   # For nrrd reader
     ],
     extras_require={
         'bionet': ['NEURON'],
         'mintnet': ['tensorflow'],
         'pointnet': ['NEST'],
         'popnet': ['DiPDE']
     },
```

