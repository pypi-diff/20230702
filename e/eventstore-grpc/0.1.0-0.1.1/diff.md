# Comparing `tmp/eventstore_grpc-0.1.0.tar.gz` & `tmp/eventstore_grpc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventstore_grpc-0.1.0.tar", max compression
+gzip compressed data, was "eventstore_grpc-0.1.1.tar", max compression
```

## Comparing `eventstore_grpc-0.1.0.tar` & `eventstore_grpc-0.1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     1085 2023-06-26 16:37:55.287113 eventstore_grpc-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1333 2023-06-26 16:37:55.287113 eventstore_grpc-0.1.0/README.md
--rw-r--r--   0        0        0     2249 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/event_store.py
--rw-r--r--   0        0        0      489 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/gossip.py
--rw-r--r--   0        0        0     2317 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/operations.py
--rw-r--r--   0        0        0     8831 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/persistent.py
--rw-r--r--   0        0        0     6110 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/projections.py
--rw-r--r--   0        0        0     2763 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/streams.py
--rw-r--r--   0        0        0     2801 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/subscriptions.py
--rw-r--r--   0        0        0     3614 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/client/users.py
--rw-r--r--   0        0        0     1021 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/constants.py
--rw-r--r--   0        0        0       92 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/core/__init__.py
--rw-r--r--   0        0        0     3382 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/core/auth.py
--rw-r--r--   0        0        0      439 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/core/client_base.py
--rw-r--r--   0        0        0      157 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/core/settings.py
--rw-r--r--   0        0        0     2514 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/core/transport.py
--rw-r--r--   0        0        0     3263 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/discovery.py
--rw-r--r--   0        0        0     3604 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/event_data.py
--rw-r--r--   0        0        0       45 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/gossip/__init__.py
--rw-r--r--   0        0        0      243 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/gossip/read.py
--rw-r--r--   0        0        0      511 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/__init__.py
--rw-r--r--   0        0        0      289 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/merge_indexes.py
--rw-r--r--   0        0        0      275 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/resign_node.py
--rw-r--r--   0        0        0      364 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/restart_persistent_subscritions.py
--rw-r--r--   0        0        0      415 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/set_node_priority.py
--rw-r--r--   0        0        0      278 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/shutdown.py
--rw-r--r--   0        0        0      590 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/start_scavenge.py
--rw-r--r--   0        0        0      498 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/operations/stop_scavenge.py
--rw-r--r--   0        0        0      412 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/__init__.py
--rw-r--r--   0        0        0     2877 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/base_options.py
--rw-r--r--   0        0        0      406 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/channel_credential.py
--rw-r--r--   0        0        0      124 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/client.py
--rw-r--r--   0        0        0      370 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/connection_type.py
--rw-r--r--   0        0        0      396 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/discovery.py
--rw-r--r--   0        0        0      271 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/dns_cluster.py
--rw-r--r--   0        0        0      308 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/gossip_cluster.py
--rw-r--r--   0        0        0      177 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/options/single_node.py
--rw-r--r--   0        0        0      502 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/__init__.py
--rw-r--r--   0        0        0     6334 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/create.py
--rw-r--r--   0        0        0      837 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/delete.py
--rw-r--r--   0        0        0      813 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/get_info.py
--rw-r--r--   0        0        0     1013 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/list.py
--rw-r--r--   0        0        0     1723 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/read.py
--rw-r--r--   0        0        0     1011 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/replay_parked.py
--rw-r--r--   0        0        0     7101 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/update.py
--rw-r--r--   0        0        0     1016 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/__init__.py
--rw-r--r--   0        0        0      775 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/create_continuous.py
--rw-r--r--   0        0        0      620 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/create_one_time.py
--rw-r--r--   0        0        0      676 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/create_transient.py
--rw-r--r--   0        0        0      786 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/delete.py
--rw-r--r--   0        0        0      575 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/disable.py
--rw-r--r--   0        0        0      478 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/enable.py
--rw-r--r--   0        0        0     1446 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/list.py
--rw-r--r--   0        0        0      561 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/reset.py
--rw-r--r--   0        0        0      333 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/restart.py
--rw-r--r--   0        0        0      574 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/result.py
--rw-r--r--   0        0        0      484 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/state.py
--rw-r--r--   0        0        0      553 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/statistics.py
--rw-r--r--   0        0        0      781 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/projections/update.py
--rw-r--r--   0        0        0    46009 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/ClientMessageDtos_pb2.py
--rw-r--r--   0        0        0      158 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/ClientMessageDtos_pb2_grpc.py
--rw-r--r--   0        0        0    13532 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/cluster_pb2.py
--rw-r--r--   0        0        0    23711 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/cluster_pb2.pyi
--rw-r--r--   0        0        0    17185 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     2107 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/code_pb2.py
--rw-r--r--   0        0        0    12954 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/code_pb2.pyi
--rw-r--r--   0        0        0      158 2023-06-26 16:37:55.291113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/code_pb2_grpc.py
--rw-r--r--   0        0        0     3768 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/gossip_pb2.py
--rw-r--r--   0        0        0     5276 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/gossip_pb2.pyi
--rw-r--r--   0        0        0     2491 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/gossip_pb2_grpc.py
--rw-r--r--   0        0        0     3049 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/monitoring_pb2.py
--rw-r--r--   0        0        0     2120 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/monitoring_pb2.pyi
--rw-r--r--   0        0        0     2516 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     6045 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/operations_pb2.py
--rw-r--r--   0        0        0     4735 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/operations_pb2.pyi
--rw-r--r--   0        0        0    12133 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/operations_pb2_grpc.py
--rw-r--r--   0        0        0    41523 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/persistent_pb2.py
--rw-r--r--   0        0        0    70817 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/persistent_pb2.pyi
--rw-r--r--   0        0        0    14040 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/persistent_pb2_grpc.py
--rw-r--r--   0        0        0    21840 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/projections_pb2.py
--rw-r--r--   0        0        0    24427 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/projections_pb2.pyi
--rw-r--r--   0        0        0    16690 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/projections_pb2_grpc.py
--rw-r--r--   0        0        0     2644 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/serverfeatures_pb2.py
--rw-r--r--   0        0        0     2182 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/serverfeatures_pb2.pyi
--rw-r--r--   0        0        0     2734 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/serverfeatures_pb2_grpc.py
--rw-r--r--   0        0        0     8516 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/shared_pb2.py
--rw-r--r--   0        0        0     9515 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1789 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/status_pb2.py
--rw-r--r--   0        0        0     2137 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/status_pb2.pyi
--rw-r--r--   0        0        0      158 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/status_pb2_grpc.py
--rw-r--r--   0        0        0    38534 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/streams_pb2.py
--rw-r--r--   0        0        0    69287 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/streams_pb2.pyi
--rw-r--r--   0        0        0     8692 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/streams_pb2_grpc.py
--rw-r--r--   0        0        0    17358 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/users_pb2.py
--rw-r--r--   0        0        0    15301 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/users_pb2.pyi
--rw-r--r--   0        0        0    13153 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/proto/users_pb2_grpc.py
--rw-r--r--   0        0        0      421 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/streams/__init__.py
--rw-r--r--   0        0        0     5609 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/streams/append.py
--rw-r--r--   0        0        0     1115 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/streams/delete.py
--rw-r--r--   0        0        0     5886 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/streams/read.py
--rw-r--r--   0        0        0     5210 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/streams/subscribe.py
--rw-r--r--   0        0        0      949 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/streams/tombstone.py
--rw-r--r--   0        0        0      226 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/__init__.py
--rw-r--r--   0        0        0     2966 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/requests_stream.py
--rw-r--r--   0        0        0     3244 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/subscription.py
--rw-r--r--   0        0        0     5941 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/subscriptions_manager.py
--rw-r--r--   0        0        0      422 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/__init__.py
--rw-r--r--   0        0        0      639 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/change_password.py
--rw-r--r--   0        0        0      657 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/create.py
--rw-r--r--   0        0        0      432 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/delete.py
--rw-r--r--   0        0        0      495 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/details.py
--rw-r--r--   0        0        0      439 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/disable.py
--rw-r--r--   0        0        0      432 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/enable.py
--rw-r--r--   0        0        0      545 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/reset_password.py
--rw-r--r--   0        0        0      850 2023-06-26 16:37:55.295113 eventstore_grpc-0.1.0/src/eventstore_grpc/users/update.py
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 eventstore_grpc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1333 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/README.md
+-rw-r--r--   0        0        0     2248 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/__init__.py
+-rw-r--r--   0        0        0     3282 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/event_store.py
+-rw-r--r--   0        0        0      489 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/gossip.py
+-rw-r--r--   0        0        0     2317 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/operations.py
+-rw-r--r--   0        0        0     8831 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/persistent.py
+-rw-r--r--   0        0        0     6110 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/projections.py
+-rw-r--r--   0        0        0     2763 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/streams.py
+-rw-r--r--   0        0        0     2801 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/subscriptions.py
+-rw-r--r--   0        0        0     3614 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/client/users.py
+-rw-r--r--   0        0        0     1021 2023-07-02 13:32:23.406705 eventstore_grpc-0.1.1/src/eventstore_grpc/constants.py
+-rw-r--r--   0        0        0       92 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/core/__init__.py
+-rw-r--r--   0        0        0     3382 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/core/auth.py
+-rw-r--r--   0        0        0      439 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/core/client_base.py
+-rw-r--r--   0        0        0      157 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/core/settings.py
+-rw-r--r--   0        0        0     2514 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/core/transport.py
+-rw-r--r--   0        0        0     3263 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/discovery.py
+-rw-r--r--   0        0        0     4019 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/event_data.py
+-rw-r--r--   0        0        0       45 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/gossip/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/gossip/read.py
+-rw-r--r--   0        0        0      511 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/merge_indexes.py
+-rw-r--r--   0        0        0      275 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/resign_node.py
+-rw-r--r--   0        0        0      364 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/restart_persistent_subscritions.py
+-rw-r--r--   0        0        0      415 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/set_node_priority.py
+-rw-r--r--   0        0        0      278 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/shutdown.py
+-rw-r--r--   0        0        0      590 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/start_scavenge.py
+-rw-r--r--   0        0        0      498 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/operations/stop_scavenge.py
+-rw-r--r--   0        0        0      412 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/__init__.py
+-rw-r--r--   0        0        0     2877 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/base_options.py
+-rw-r--r--   0        0        0      406 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/channel_credential.py
+-rw-r--r--   0        0        0      124 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/client.py
+-rw-r--r--   0        0        0      370 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/connection_type.py
+-rw-r--r--   0        0        0      396 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/discovery.py
+-rw-r--r--   0        0        0      271 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/dns_cluster.py
+-rw-r--r--   0        0        0      308 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/gossip_cluster.py
+-rw-r--r--   0        0        0      177 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/options/single_node.py
+-rw-r--r--   0        0        0      502 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/__init__.py
+-rw-r--r--   0        0        0     6334 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/create.py
+-rw-r--r--   0        0        0      837 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/delete.py
+-rw-r--r--   0        0        0      813 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/get_info.py
+-rw-r--r--   0        0        0     1013 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/list.py
+-rw-r--r--   0        0        0     1723 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/read.py
+-rw-r--r--   0        0        0     1011 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/replay_parked.py
+-rw-r--r--   0        0        0     7101 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/update.py
+-rw-r--r--   0        0        0     1016 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/__init__.py
+-rw-r--r--   0        0        0      775 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/create_continuous.py
+-rw-r--r--   0        0        0      620 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/create_one_time.py
+-rw-r--r--   0        0        0      676 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/create_transient.py
+-rw-r--r--   0        0        0      786 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/delete.py
+-rw-r--r--   0        0        0      575 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/disable.py
+-rw-r--r--   0        0        0      478 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/enable.py
+-rw-r--r--   0        0        0     1446 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/list.py
+-rw-r--r--   0        0        0      561 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/reset.py
+-rw-r--r--   0        0        0      333 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/restart.py
+-rw-r--r--   0        0        0      574 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/result.py
+-rw-r--r--   0        0        0      484 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/state.py
+-rw-r--r--   0        0        0      553 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/statistics.py
+-rw-r--r--   0        0        0      781 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/projections/update.py
+-rw-r--r--   0        0        0    46009 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/ClientMessageDtos_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/ClientMessageDtos_pb2_grpc.py
+-rw-r--r--   0        0        0    13532 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/cluster_pb2.py
+-rw-r--r--   0        0        0    23711 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/cluster_pb2.pyi
+-rw-r--r--   0        0        0    17185 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     2107 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/code_pb2.py
+-rw-r--r--   0        0        0    12954 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/code_pb2_grpc.py
+-rw-r--r--   0        0        0     3768 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/gossip_pb2.py
+-rw-r--r--   0        0        0     5276 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2491 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0     3049 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/monitoring_pb2.py
+-rw-r--r--   0        0        0     2120 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/monitoring_pb2.pyi
+-rw-r--r--   0        0        0     2516 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     6045 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/operations_pb2.py
+-rw-r--r--   0        0        0     4735 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/operations_pb2.pyi
+-rw-r--r--   0        0        0    12133 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/operations_pb2_grpc.py
+-rw-r--r--   0        0        0    41523 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/persistent_pb2.py
+-rw-r--r--   0        0        0    70817 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/persistent_pb2.pyi
+-rw-r--r--   0        0        0    14040 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0    21840 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/projections_pb2.py
+-rw-r--r--   0        0        0    24427 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/projections_pb2.pyi
+-rw-r--r--   0        0        0    16690 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/projections_pb2_grpc.py
+-rw-r--r--   0        0        0     2644 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/serverfeatures_pb2.py
+-rw-r--r--   0        0        0     2182 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/serverfeatures_pb2.pyi
+-rw-r--r--   0        0        0     2734 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/serverfeatures_pb2_grpc.py
+-rw-r--r--   0        0        0     8516 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/shared_pb2.py
+-rw-r--r--   0        0        0     9515 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1789 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/status_pb2.py
+-rw-r--r--   0        0        0     2137 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/status_pb2_grpc.py
+-rw-r--r--   0        0        0    38534 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/streams_pb2.py
+-rw-r--r--   0        0        0    69287 2023-07-02 13:32:23.410704 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/streams_pb2.pyi
+-rw-r--r--   0        0        0     8692 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/streams_pb2_grpc.py
+-rw-r--r--   0        0        0    17358 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/users_pb2.py
+-rw-r--r--   0        0        0    15301 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/users_pb2.pyi
+-rw-r--r--   0        0        0    13153 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/proto/users_pb2_grpc.py
+-rw-r--r--   0        0        0      421 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/streams/__init__.py
+-rw-r--r--   0        0        0     5609 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/streams/append.py
+-rw-r--r--   0        0        0     1115 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/streams/delete.py
+-rw-r--r--   0        0        0     5886 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/streams/read.py
+-rw-r--r--   0        0        0     5210 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/streams/subscribe.py
+-rw-r--r--   0        0        0      949 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/streams/tombstone.py
+-rw-r--r--   0        0        0      226 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/__init__.py
+-rw-r--r--   0        0        0     2966 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/requests_stream.py
+-rw-r--r--   0        0        0     3244 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/subscription.py
+-rw-r--r--   0        0        0     5941 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/subscriptions_manager.py
+-rw-r--r--   0        0        0      422 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/__init__.py
+-rw-r--r--   0        0        0      639 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/change_password.py
+-rw-r--r--   0        0        0      657 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/create.py
+-rw-r--r--   0        0        0      432 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/delete.py
+-rw-r--r--   0        0        0      495 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/details.py
+-rw-r--r--   0        0        0      439 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/disable.py
+-rw-r--r--   0        0        0      432 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/enable.py
+-rw-r--r--   0        0        0      545 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/reset_password.py
+-rw-r--r--   0        0        0      850 2023-07-02 13:32:23.414705 eventstore_grpc-0.1.1/src/eventstore_grpc/users/update.py
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 eventstore_grpc-0.1.1/PKG-INFO
```

### Comparing `eventstore_grpc-0.1.0/LICENSE.md` & `eventstore_grpc-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/README.md` & `eventstore_grpc-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 </div>
 <br>
 
 # EventStoreDB GRPC Client.
 
 Use this client to interact with [EventStoreDB](https://developers.eventstore.com/) via GRPC.
 
-[Documenation](https://stefanondisponibile.github.io/eventstore_grpc/).
+[Documentation](https://stefanondisponibile.github.io/eventstore_grpc).
 
 ## Quickstart
 
 ### Installation
 
 ```bash
 pip install eventstore_grpc
```

### Comparing `eventstore_grpc-0.1.0/pyproject.toml` & `eventstore_grpc-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "eventstore_grpc"
-version = "0.1.0"
+version = "0.1.1"
 description = "EventStoreDB gRPC client."
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 maintainers = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stefanondisponibile/eventstore_grpc"
 repository = "https://github.com/stefanondisponibile/eventstore_grpc"
-documentation = "https://stefanondisponibile.github.io/eventstore_grpc/"
+documentation = "https://stefanondisponibile.github.io/eventstore_grpc"
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
     "Topic :: Internet",
```

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/event_store.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/event_store.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/operations.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/operations.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/persistent.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/persistent.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/projections.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/projections.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/streams.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/streams.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/subscriptions.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/subscriptions.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/client/users.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/client/users.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/constants.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/constants.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/core/auth.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/core/auth.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/core/transport.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/core/transport.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/discovery.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/discovery.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/event_data.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/event_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     * `event_id`: this takes the format of `Uuid` and is used to uniquely identify the
         event your are trying to append. If two events with the same `Uuid` are appended
         to the same stream in quick succession, EventStoreDB will only append one copy
         of the event to the stream.
     * `type`: an event type should be supplied for each event. This is a unique string
         used to identify the type of event you are saving.
-
         It is common to see the explicit event code type name used as the type as
         it makes serializing and de-serializing of the event easy. However we recommend
         against this as it couples the storage to the type and will make it more
         difficult if you need to version the event at a later date.
     * `data`: representation of your event data. It is recommended that you store your
         events as JSON objects as this will allow you to make use of all of
         EventStoreDB's functionality such as projections. Ultimately though, you can
@@ -55,14 +54,28 @@
 
     def __repr__(self):
         return f"{self.__class__.__name__}(**{self.__dict__!r})"  # pragma: nocover
 
     def __str__(self):
         return f"{self.type} => {self.data}"  # pragma: nocover
 
+    @staticmethod
+    def _validate_event_id(event_id: Any) -> uuid.UUID:
+        if not isinstance(event_id, uuid.UUID):
+            return uuid.UUID(str(event_id))  # raises ValueError
+        return event_id
+
+    @property
+    def event_id(self) -> uuid.UUID:
+        return self._event_id
+
+    @event_id.setter
+    def event_id(self, value: Any) -> None:
+        self._event_id = self._validate_event_id(value)
+
     @property
     def data_content_type(self):
         return "application/json" if self.is_json else "application/octet-stream"
 
     @property
     def serialized_metadata(self):
         return json.dumps(self.metadata).encode()
```

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/operations/start_scavenge.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/operations/start_scavenge.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/options/base_options.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/options/base_options.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/create.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/create.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/delete.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/delete.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/get_info.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/get_info.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/list.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/list.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/read.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/read.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/replay_parked.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/replay_parked.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/persistent/update.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/persistent/update.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/__init__.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/create_continuous.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/create_continuous.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/create_one_time.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/create_one_time.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/create_transient.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/create_transient.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/delete.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/delete.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/disable.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/disable.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/list.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/list.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/reset.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/reset.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/result.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/result.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/statistics.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/statistics.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/projections/update.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/projections/update.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/ClientMessageDtos_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/ClientMessageDtos_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/cluster_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/cluster_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/cluster_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/code_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/code_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/code_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/gossip_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/gossip_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/gossip_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/monitoring_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/monitoring_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/monitoring_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/operations_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/operations_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/operations_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/persistent_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/persistent_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/persistent_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/projections_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/projections_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/projections_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/projections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/projections_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/projections_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/serverfeatures_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/serverfeatures_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/serverfeatures_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/serverfeatures_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/serverfeatures_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/serverfeatures_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/shared_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/shared_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/status_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/status_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/status_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/streams_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/streams_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/streams_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/users_pb2.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/users_pb2.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/users_pb2.pyi` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/proto/users_pb2_grpc.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/proto/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/streams/append.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/streams/append.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/streams/delete.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/streams/delete.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/streams/read.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/streams/read.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/streams/subscribe.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/streams/subscribe.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/streams/tombstone.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/streams/tombstone.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/requests_stream.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/requests_stream.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/subscription.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/subscriptions/subscriptions_manager.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/subscriptions/subscriptions_manager.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/users/change_password.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/users/change_password.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/users/create.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/users/create.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/users/reset_password.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/users/reset_password.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/src/eventstore_grpc/users/update.py` & `eventstore_grpc-0.1.1/src/eventstore_grpc/users/update.py`

 * *Files identical despite different names*

### Comparing `eventstore_grpc-0.1.0/PKG-INFO` & `eventstore_grpc-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventstore-grpc
-Version: 0.1.0
+Version: 0.1.1
 Summary: EventStoreDB gRPC client.
 Home-page: https://github.com/stefanondisponibile/eventstore_grpc
 License: MIT
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Maintainer: Stefano Frassetto
 Maintainer-email: frassetto.stefano@gmail.com
@@ -22,30 +22,30 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Internet
 Requires-Dist: grpcio (>=1.54.2,<2.0.0)
 Requires-Dist: grpcio-status (>=1.0.0,<2.0.0)
 Requires-Dist: protobuf (>=4.21.6,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
-Project-URL: Documentation, https://stefanondisponibile.github.io/eventstore_grpc/
+Project-URL: Documentation, https://stefanondisponibile.github.io/eventstore_grpc
 Project-URL: Repository, https://github.com/stefanondisponibile/eventstore_grpc
 Description-Content-Type: text/markdown
 
 <div align="left">
     <img src="https://github.com/stefanondisponibile/eventstore_grpc/actions/workflows/test.yaml/badge.svg?event=push" style="text-align: right" />
     <a target="_blank" href="https://codecov.io/gh/stefanondisponibile/eventstore_grpc"><img src="https://codecov.io/gh/stefanondisponibile/eventstore_grpc/branch/develop/graph/badge.svg?token=O86CZ83P50" style="text-align: right" /></a>
     <a target="_blank" href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" style="text-align: right" /></a>
 </div>
 <br>
 
 # EventStoreDB GRPC Client.
 
 Use this client to interact with [EventStoreDB](https://developers.eventstore.com/) via GRPC.
 
-[Documenation](https://stefanondisponibile.github.io/eventstore_grpc/).
+[Documentation](https://stefanondisponibile.github.io/eventstore_grpc).
 
 ## Quickstart
 
 ### Installation
 
 ```bash
 pip install eventstore_grpc
```

