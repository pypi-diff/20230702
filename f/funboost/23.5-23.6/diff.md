# Comparing `tmp/funboost-23.5-py3-none-any.whl.zip` & `tmp/funboost-23.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1684056 bytes, number of entries: 220
--rw-rw-rw-  2.0 fat     2402 b- defN 23-Jun-23 09:05 funboost/__init__.py
+Zip file size: 1686336 bytes, number of entries: 222
+-rw-rw-rw-  2.0 fat     2401 b- defN 23-Jun-30 14:15 funboost/__init__.py
 -rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-03 06:12 funboost/__init__old.py
 -rw-rw-rw-  2.0 fat     6489 b- defN 23-Jun-21 13:54 funboost/constant.py
--rw-rw-rw-  2.0 fat     7399 b- defN 23-Jun-23 09:05 funboost/funboost_config_deafult.py
+-rw-rw-rw-  2.0 fat     7430 b- defN 23-Jun-30 14:15 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-27 12:40 funboost/set_frame_config.py
--rw-rw-rw-  2.0 fat     4186 b- defN 23-Jun-17 05:37 funboost/assist/celery_helper.py
+-rw-rw-rw-  2.0 fat     4569 b- defN 23-Jun-30 14:15 funboost/assist/celery_helper.py
 -rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 13:41 funboost/assist/dramatiq_helper.py
 -rw-rw-rw-  2.0 fat     1760 b- defN 23-May-26 03:56 funboost/assist/huey_helper.py
 -rw-rw-rw-  2.0 fat     1509 b- defN 23-Jun-09 14:04 funboost/assist/rq_helper.py
 -rw-rw-rw-  2.0 fat     4831 b- defN 23-Jun-08 14:14 funboost/assist/rq_windows_worker.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 23-Apr-27 12:40 funboost/beggar_version_implementation/beggar_redis_consumer.py
 -rw-rw-rw-  2.0 fat      759 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/__init__.py
 -rw-rw-rw-  2.0 fat     3256 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/async_helper.py
@@ -23,16 +23,16 @@
 -rw-rw-rw-  2.0 fat     9317 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/custom_threadpool_executor000.py
 -rw-rw-rw-  2.0 fat      373 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/single_thread_executor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/__init__.py
 -rw-rw-rw-  2.0 fat     9548 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor0223.py
 -rw-rw-rw-  2.0 fat     9568 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor_back.py
 -rw-rw-rw-  2.0 fat     5728 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor_janus.py
 -rw-rw-rw-  2.0 fat      126 b- defN 23-Apr-27 12:40 funboost/consumers/__init__.py
--rw-rw-rw-  2.0 fat    85044 b- defN 23-Jun-24 02:53 funboost/consumers/base_consumer.py
--rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-05 13:53 funboost/consumers/celery_consumer.py
+-rw-rw-rw-  2.0 fat    86846 b- defN 23-Jun-30 14:29 funboost/consumers/base_consumer.py
+-rw-rw-rw-  2.0 fat     8815 b- defN 23-Jun-30 14:15 funboost/consumers/celery_consumer.py
 -rw-rw-rw-  2.0 fat     4574 b- defN 23-Apr-27 12:40 funboost/consumers/celery_consumer000.py
 -rw-rw-rw-  2.0 fat     6033 b- defN 23-Jun-20 13:31 funboost/consumers/confirm_mixin.py
 -rw-rw-rw-  2.0 fat     2144 b- defN 23-May-26 03:56 funboost/consumers/dramatiq_consumer.py
 -rw-rw-rw-  2.0 fat     2025 b- defN 23-May-13 11:56 funboost/consumers/http_consumer.py
 -rw-rw-rw-  2.0 fat     4463 b- defN 23-Apr-27 12:40 funboost/consumers/http_consumer000.py
 -rw-rw-rw-  2.0 fat     1080 b- defN 23-May-13 08:23 funboost/consumers/httpsqs_consumer.py
 -rw-rw-rw-  2.0 fat     1856 b- defN 23-May-26 03:56 funboost/consumers/huey_consumer.py
@@ -44,22 +44,22 @@
 -rw-rw-rw-  2.0 fat     2228 b- defN 23-May-13 08:23 funboost/consumers/mqtt_consumer.py
 -rw-rw-rw-  2.0 fat     2183 b- defN 23-May-13 08:23 funboost/consumers/nameko_consumer.py
 -rw-rw-rw-  2.0 fat     1076 b- defN 23-May-13 08:23 funboost/consumers/nats_consumer.py
 -rw-rw-rw-  2.0 fat     1461 b- defN 23-May-13 08:23 funboost/consumers/nsq_consumer.py
 -rw-rw-rw-  2.0 fat     1238 b- defN 23-May-13 08:16 funboost/consumers/peewee_conusmer.py
 -rw-rw-rw-  2.0 fat     1005 b- defN 23-May-13 08:16 funboost/consumers/persist_queue_consumer.py
 -rw-rw-rw-  2.0 fat     2414 b- defN 23-May-13 08:16 funboost/consumers/pulsar_consumer.py
--rw-rw-rw-  2.0 fat     2048 b- defN 23-Jun-20 13:31 funboost/consumers/rabbitmq_amqpstorm_consumer.py
+-rw-rw-rw-  2.0 fat     2049 b- defN 23-Jun-30 14:15 funboost/consumers/rabbitmq_amqpstorm_consumer.py
 -rw-rw-rw-  2.0 fat     5433 b- defN 23-May-13 08:17 funboost/consumers/rabbitmq_pika_consumer.py
 -rw-rw-rw-  2.0 fat     4674 b- defN 23-May-13 08:23 funboost/consumers/rabbitmq_pika_consumerv0.py
 -rw-rw-rw-  2.0 fat     1260 b- defN 23-May-13 08:23 funboost/consumers/rabbitmq_rabbitpy_consumer.py
 -rw-rw-rw-  2.0 fat     3031 b- defN 23-May-13 08:23 funboost/consumers/redis_brpoplpush_consumer.py
 -rw-rw-rw-  2.0 fat     2829 b- defN 23-May-13 08:23 funboost/consumers/redis_consumer.py
--rw-rw-rw-  2.0 fat     7545 b- defN 23-May-13 08:23 funboost/consumers/redis_consumer_ack_able.py
--rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-21 13:54 funboost/consumers/redis_consumer_priority.py
+-rw-rw-rw-  2.0 fat     7545 b- defN 23-Jun-30 14:15 funboost/consumers/redis_consumer_ack_able.py
+-rw-rw-rw-  2.0 fat     5827 b- defN 23-Jun-30 14:15 funboost/consumers/redis_consumer_priority.py
 -rw-rw-rw-  2.0 fat      922 b- defN 23-May-13 08:23 funboost/consumers/redis_consumer_simple.py
 -rw-rw-rw-  2.0 fat     7135 b- defN 23-Apr-27 12:40 funboost/consumers/redis_filter.py
 -rw-rw-rw-  2.0 fat     1206 b- defN 23-May-13 08:23 funboost/consumers/redis_pubsub_consumer.py
 -rw-rw-rw-  2.0 fat     6497 b- defN 23-Jun-03 04:51 funboost/consumers/redis_stream_consumer.py
 -rw-rw-rw-  2.0 fat     1653 b- defN 23-May-13 08:23 funboost/consumers/rocketmq_consumer.py
 -rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-08 14:00 funboost/consumers/rq_consumer.py
 -rw-rw-rw-  2.0 fat     1309 b- defN 23-May-13 08:23 funboost/consumers/sqlachemy_consumer.py
@@ -79,14 +79,15 @@
 -rw-rw-rw-  2.0 fat     8886 b- defN 23-Jun-23 09:05 funboost/core/function_result_status_saver.py
 -rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-08 14:00 funboost/core/get_booster.py
 -rw-rw-rw-  2.0 fat      340 b- defN 23-Jun-08 14:00 funboost/core/global_boosters.py
 -rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-23 09:05 funboost/core/helper_funs.py
 -rw-rw-rw-  2.0 fat     8159 b- defN 23-Jun-24 06:54 funboost/core/kill_remote_task.py
 -rw-rw-rw-  2.0 fat     7782 b- defN 23-Apr-27 12:40 funboost/core/msg_result_getter.py
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-08 14:00 funboost/core/muliti_process_enhance.py
+-rw-rw-rw-  2.0 fat     5725 b- defN 23-Jun-30 14:15 funboost/core/show_funboost_flag.py
 -rw-rw-rw-  2.0 fat      178 b- defN 23-Apr-27 12:40 funboost/factories/__init__.py
 -rw-rw-rw-  2.0 fat     8976 b- defN 23-Jun-21 13:54 funboost/factories/broker_kind__publsiher_consumer_type_map.py
 -rw-rw-rw-  2.0 fat      946 b- defN 23-Jun-03 04:51 funboost/factories/consumer_factory.py
 -rw-rw-rw-  2.0 fat     2281 b- defN 23-Jun-03 04:51 funboost/factories/publisher_factotry.py
 -rw-rw-rw-  2.0 fat     4841 b- defN 23-Apr-27 12:40 funboost/function_result_web/app.py
 -rw-rw-rw-  2.0 fat     7345 b- defN 23-Apr-27 12:40 funboost/function_result_web/functions.py
 -rw-rw-rw-  2.0 fat     7674 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/assets/css/custom.css
@@ -99,16 +100,16 @@
 -rw-rw-rw-  2.0 fat      546 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/password.png
 -rw-rw-rw-  2.0 fat     2912 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/tick.png
 -rw-rw-rw-  2.0 fat      622 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/user.png
 -rw-rw-rw-  2.0 fat    96383 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/js/jquery-1.11.0.min.js
 -rw-rw-rw-  2.0 fat    19501 b- defN 22-Jul-15 16:25 funboost/function_result_web/templates/index.html
 -rw-rw-rw-  2.0 fat     2007 b- defN 22-Jul-15 16:25 funboost/function_result_web/templates/login.html
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Apr-27 12:40 funboost/publishers/__init__.py
--rw-rw-rw-  2.0 fat    15860 b- defN 23-Jun-23 09:09 funboost/publishers/base_publisher.py
--rw-rw-rw-  2.0 fat     3081 b- defN 23-Jun-23 09:09 funboost/publishers/celery_publisher.py
+-rw-rw-rw-  2.0 fat    15863 b- defN 23-Jun-30 14:15 funboost/publishers/base_publisher.py
+-rw-rw-rw-  2.0 fat     2334 b- defN 23-Jun-30 14:15 funboost/publishers/celery_publisher.py
 -rw-rw-rw-  2.0 fat     3897 b- defN 23-Apr-28 13:25 funboost/publishers/celery_publisher000.py
 -rw-rw-rw-  2.0 fat     3541 b- defN 23-Apr-27 12:40 funboost/publishers/confluent_kafka_publisher.py
 -rw-rw-rw-  2.0 fat     1410 b- defN 23-May-21 15:14 funboost/publishers/dramatiq_publisher.py
 -rw-rw-rw-  2.0 fat      753 b- defN 23-May-13 08:23 funboost/publishers/http_publisher.py
 -rw-rw-rw-  2.0 fat     2783 b- defN 23-Apr-27 12:40 funboost/publishers/httpsqs_publisher.py
 -rw-rw-rw-  2.0 fat     1101 b- defN 23-May-26 03:56 funboost/publishers/huey_publisher.py
 -rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-27 12:40 funboost/publishers/kafka_publisher.py
@@ -121,19 +122,20 @@
 -rw-rw-rw-  2.0 fat     1302 b- defN 23-Apr-27 12:40 funboost/publishers/nsq_publisher.py
 -rw-rw-rw-  2.0 fat     1095 b- defN 23-Apr-27 12:40 funboost/publishers/peewee_publisher.py
 -rw-rw-rw-  2.0 fat     2540 b- defN 23-Apr-27 12:40 funboost/publishers/persist_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-27 12:40 funboost/publishers/pulsar_publisher.py
 -rw-rw-rw-  2.0 fat     3137 b- defN 23-Jun-20 13:31 funboost/publishers/rabbitmq_amqpstorm_publisher.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-27 12:40 funboost/publishers/rabbitmq_pika_publisher.py
 -rw-rw-rw-  2.0 fat     1953 b- defN 23-Apr-27 12:40 funboost/publishers/rabbitmq_rabbitpy_publisher.py
--rw-rw-rw-  2.0 fat     3982 b- defN 23-May-13 08:23 funboost/publishers/redis_publisher.py
+-rw-rw-rw-  2.0 fat     3358 b- defN 23-Jun-30 14:15 funboost/publishers/redis_publisher.py
 -rw-rw-rw-  2.0 fat      278 b- defN 23-Apr-27 12:40 funboost/publishers/redis_publisher_lpush.py
--rw-rw-rw-  2.0 fat     2104 b- defN 23-Jun-20 13:31 funboost/publishers/redis_publisher_priority.py
--rw-rw-rw-  2.0 fat      872 b- defN 23-Apr-28 13:25 funboost/publishers/redis_publisher_simple.py
--rw-rw-rw-  2.0 fat      721 b- defN 23-Apr-27 12:40 funboost/publishers/redis_pubsub_publisher.py
+-rw-rw-rw-  2.0 fat     1972 b- defN 23-Jun-30 14:15 funboost/publishers/redis_publisher_priority.py
+-rw-rw-rw-  2.0 fat      740 b- defN 23-Jun-30 14:15 funboost/publishers/redis_publisher_simple.py
+-rw-rw-rw-  2.0 fat      723 b- defN 23-Jun-30 14:15 funboost/publishers/redis_pubsub_publisher.py
+-rw-rw-rw-  2.0 fat      732 b- defN 23-Jun-30 14:15 funboost/publishers/redis_queue_flush.py
 -rw-rw-rw-  2.0 fat     2037 b- defN 22-Jul-15 16:25 funboost/publishers/redis_stream_publisher.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-27 12:40 funboost/publishers/rocketmq_publisher.py
 -rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-10 08:06 funboost/publishers/rq_publisher.py
 -rw-rw-rw-  2.0 fat     1215 b- defN 23-Apr-27 12:40 funboost/publishers/sqla_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-May-13 08:23 funboost/publishers/tcp_publisher.py
 -rw-rw-rw-  2.0 fat     1380 b- defN 23-Apr-27 12:40 funboost/publishers/txt_file_publisher.py
 -rw-rw-rw-  2.0 fat     1194 b- defN 23-May-13 08:23 funboost/publishers/udp_publisher.py
@@ -155,15 +157,15 @@
 -rw-rw-rw-  2.0 fat     3412 b- defN 23-Jun-23 06:28 funboost/utils/kill_thread.py
 -rw-rw-rw-  2.0 fat     2984 b- defN 23-Apr-27 12:40 funboost/utils/mongo_util.py
 -rw-rw-rw-  2.0 fat     7367 b- defN 23-Apr-27 12:40 funboost/utils/monkey_color_log.py
 -rw-rw-rw-  2.0 fat     2882 b- defN 23-Apr-27 12:40 funboost/utils/monkey_patches.py
 -rw-rw-rw-  2.0 fat     3199 b- defN 22-Jul-15 16:25 funboost/utils/mqtt_util.py
 -rw-rw-rw-  2.0 fat     4901 b- defN 22-Jul-15 16:25 funboost/utils/paramiko_util.py
 -rw-rw-rw-  2.0 fat     2963 b- defN 23-Apr-27 12:40 funboost/utils/rabbitmq_factory.py
--rw-rw-rw-  2.0 fat     4628 b- defN 23-May-20 04:45 funboost/utils/redis_manager.py
+-rw-rw-rw-  2.0 fat     4649 b- defN 23-Jun-30 14:15 funboost/utils/redis_manager.py
 -rw-rw-rw-  2.0 fat     5532 b- defN 23-Apr-27 12:40 funboost/utils/resource_monitoring.py
 -rw-rw-rw-  2.0 fat     1418 b- defN 23-Apr-27 12:40 funboost/utils/restart_python.py
 -rw-rw-rw-  2.0 fat     2985 b- defN 23-Jun-17 05:42 funboost/utils/show_funboost_flag.py
 -rw-rw-rw-  2.0 fat     1204 b- defN 22-Jul-15 16:25 funboost/utils/simple_data_class.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 22-Jul-15 16:25 funboost/utils/time_util.py
 -rw-rw-rw-  2.0 fat      408 b- defN 22-Jul-15 16:25 funboost/utils/un_strict_json_dumps.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/__init__.py
@@ -210,13 +212,13 @@
 -rw-rw-rw-  2.0 fat      909 b- defN 22-Jul-15 16:25 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 22-Jul-15 16:25 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/variables.py
 -rw-rw-rw-  2.0 fat     2332 b- defN 23-Jun-08 14:07 funboost/utils/times/__init__.py
 -rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-08 14:07 funboost/utils/times/version.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    26615 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    22651 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/RECORD
-220 files, 2712982 bytes uncompressed, 1646906 bytes compressed:  39.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-02 08:26 funboost-23.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26928 b- defN 23-Jul-02 08:26 funboost-23.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-02 08:26 funboost-23.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-02 08:26 funboost-23.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    22839 b- defN 23-Jul-02 08:26 funboost-23.6.dist-info/RECORD
+222 files, 2723333 bytes uncompressed, 1648884 bytes compressed:  39.5%
```

## zipnote {}

```diff
@@ -246,14 +246,17 @@
 
 Filename: funboost/core/msg_result_getter.py
 Comment: 
 
 Filename: funboost/core/muliti_process_enhance.py
 Comment: 
 
+Filename: funboost/core/show_funboost_flag.py
+Comment: 
+
 Filename: funboost/factories/__init__.py
 Comment: 
 
 Filename: funboost/factories/broker_kind__publsiher_consumer_type_map.py
 Comment: 
 
 Filename: funboost/factories/consumer_factory.py
@@ -387,14 +390,17 @@
 
 Filename: funboost/publishers/redis_publisher_simple.py
 Comment: 
 
 Filename: funboost/publishers/redis_pubsub_publisher.py
 Comment: 
 
+Filename: funboost/publishers/redis_queue_flush.py
+Comment: 
+
 Filename: funboost/publishers/redis_stream_publisher.py
 Comment: 
 
 Filename: funboost/publishers/rocketmq_publisher.py
 Comment: 
 
 Filename: funboost/publishers/rq_publisher.py
@@ -639,23 +645,23 @@
 
 Filename: funboost/utils/times/__init__.py
 Comment: 
 
 Filename: funboost/utils/times/version.py
 Comment: 
 
-Filename: funboost-23.5.dist-info/LICENSE
+Filename: funboost-23.6.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-23.5.dist-info/METADATA
+Filename: funboost-23.6.dist-info/METADATA
 Comment: 
 
-Filename: funboost-23.5.dist-info/WHEEL
+Filename: funboost-23.6.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-23.5.dist-info/top_level.txt
+Filename: funboost-23.6.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-23.5.dist-info/RECORD
+Filename: funboost-23.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/__init__.py

```diff
@@ -1,12 +1,12 @@
 # noinspection PyUnresolvedReferences
 from funboost.utils.dependency_packages_in_pythonpath import add_to_pythonpath # 这是把 dependency_packages_in_pythonpath 添加到 PYTHONPATH了。
 
 from funboost.utils import monkey_patches
-from funboost.utils import show_funboost_flag
+from funboost.core import show_funboost_flag
 
 # noinspection PyUnresolvedReferences
 import nb_log
 from funboost.set_frame_config import patch_frame_config, show_frame_config
 from funboost.funboost_config_deafult import BoostDecoratorDefaultParams
 
 from funboost.core.fabric_deploy_helper import fabric_deploy, kill_all_remote_tasks
```

## funboost/funboost_config_deafult.py

```diff
@@ -23,15 +23,15 @@
 框架使用文档是 https://funboost.readthedocs.io/zh_CN/latest/
 
 '''
 
 # $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$  以下是中间件连接配置    $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
 
 
-MONGO_CONNECT_URL = f'mongodb://127.0.0.1:27017'  # 如果有密码连接 'mongodb://myUserAdmin:8mwTdy1klnSYepNo@192.168.199.202:27016/MONGO_CONNECT_URL = 'mongodb://root:123456@192.168.64.151:27017?authSource=admin''
+MONGO_CONNECT_URL = f'mongodb://127.0.0.1:27017'  # 如果有密码连接 'mongodb://myUserAdmin:8mwTdy1klnSYepNo@192.168.199.202:27016/'   authSource 指定鉴权db，MONGO_CONNECT_URL = 'mongodb://root:123456@192.168.64.151:27017?authSource=admin'
 
 RABBITMQ_USER = 'rabbitmq_user'
 RABBITMQ_PASS = 'rabbitmq_pass'
 RABBITMQ_HOST = '127.0.0.1'
 RABBITMQ_PORT = 5672
 RABBITMQ_VIRTUAL_HOST = ''  # my_host # 这个是rabbitmq的虚拟子host用户自己创建的，如果你想直接用rabbitmq的根host而不是使用虚拟子host，这里写 空字符串 即可。
 RABBITMQ_URL= f'amqp://{RABBITMQ_USER}:{RABBITMQ_PASS}@{RABBITMQ_HOST}:{RABBITMQ_PORT}/{RABBITMQ_VIRTUAL_HOST}'
```

## funboost/assist/celery_helper.py

```diff
@@ -11,42 +11,46 @@
 from nb_log import get_logger
 
 celery_app = celery.Celery(main='funboost_celery', broker=funboost_config_deafult.CELERY_BROKER_URL,
                            backend=funboost_config_deafult.CELERY_RESULT_BACKEND,
                            task_routes={}, timezone=funboost_config_deafult.TIMEZONE, enable_utc=False, )
 
 celery_app.conf.task_acks_late = True
-celery_app.conf.worker_redirect_stdouts = False
+celery_app.conf.update({
+    'worker_redirect_stdouts': False,
+    'worker_concurrency': 200
+}
+)
 
 logger = get_logger('funboost.CeleryHelper')
 
 
 class CeleryHelper:
     celery_app = celery_app
     to_be_start_work_celery_queue_name_set = set()  # start_consuming_message时候，添加需要worker运行的queue name。
 
     concurrent_mode = None
 
     @staticmethod
     def update_celery_app_conf(celery_app_conf: dict):
         """
         更新celery app的配置，celery app配置大全见 https://docs.celeryq.dev/en/stable/userguide/configuration.html
-        :param celery_app_conf:
+        :param celery_app_conf: celery app 配置，字典
         :return:
         """
         celery_app.conf.update(celery_app_conf)
 
     @staticmethod
     def show_celery_app_conf():
         logger.debug('展示celery app的配置')
         conf_dict_json_able = {}
         for k, v in celery_app.conf.items():
             conf_dict_json_able[k] = str(v)
             # print(k, ' : ', v)
-        print('celery app 的配置是：',json.dumps(conf_dict_json_able,ensure_ascii=False,indent=4))
+        print('celery app 的配置是：', json.dumps(conf_dict_json_able, ensure_ascii=False, indent=4))
 
     @staticmethod
     def celery_start_beat(beat_schedule: dict):
         celery_app.conf.beat_schedule = beat_schedule  # 配置celery定时任务
 
         def _f():
             beat = partial(celery_app.Beat, loglevel='INFO', )
@@ -64,29 +68,36 @@
 
             logger.info(f'启动flower命令:   {cmd}')
             os.system(cmd)
 
         threading.Thread(target=_f).start()
 
     @classmethod
-    def realy_start_celery_worker(cls, worker_name=None):
+    def realy_start_celery_worker(cls, worker_name=None, loglevel='INFO'):
         if len(cls.to_be_start_work_celery_queue_name_set) == 0:
             raise Exception('celery worker 没有需要运行的queue')
         queue_names_str = ','.join(list(cls.to_be_start_work_celery_queue_name_set))
         # '--concurrency=200',
         # '--autoscale=5,500' threads 并发模式不支持自动扩大缩小并发数量,
         worker_name = worker_name or f'pid_{os.getpid()}'
         pool_name = 'threads'
         if cls.concurrent_mode == ConcurrentModeEnum.GEVENT:
             pool_name = 'gevent'
         if cls.concurrent_mode == ConcurrentModeEnum.EVENTLET:
             pool_name = 'eventlet'
-        argv = ['worker', f'--pool={pool_name}', '--concurrency=200',
-                '-n', f'worker_funboost_{worker_name}@%h', f'--loglevel=INFO',
-                f'--queues={queue_names_str}',
+        '''
+        并发数量在app配置中已经制定了。自己用 update_celery_app_conf 方法更新就好了。
+        celery_app.conf.update({
+             'worker_redirect_stdouts': False,
+             'worker_concurrency': 200
+         }
+        '''
+        argv = ['worker', f'--pool={pool_name}',
+                '-n', f'worker_funboost_{worker_name}@%h', f'--loglevel={loglevel}',
+                f'--queues={queue_names_str}',         # 并发数量是
                 ]
         logger.info(f'celery 启动work参数 {argv}')
         celery_app.worker_main(argv)
 
     @staticmethod
     def use_nb_log_instead_celery_log(log_level: int = logging.INFO, log_filename='celery.log', formatter_template=7):
         """
```

## funboost/consumers/base_consumer.py

```diff
@@ -369,14 +369,17 @@
         self._unit_time_for_count = 10  # 每隔多少秒计数，显示单位时间内执行多少次，暂时固定为10秒。
         self._execute_task_times_every_unit_time = 0  # 每单位时间执行了多少次任务。
         self._lock_for_count_execute_task_times_every_unit_time = Lock()
         self._current_time_for_execute_task_times_every_unit_time = time.time()
         self._consuming_function_cost_time_total_every_unit_time = 0
         self._last_execute_task_time = time.time()  # 最近一次执行任务的时间。
 
+        self._last_show_remaining_execution_time = 0
+        self._show_remaining_execution_time_interval = 300
+
         self._msg_num_in_broker = 0
         self._last_timestamp_when_has_task_in_queue = 0
         self._last_timestamp_print_msg_num = 0
 
         self._is_do_not_run_by_specify_time_effect = is_do_not_run_by_specify_time_effect
         self._do_not_run_by_specify_time = do_not_run_by_specify_time  # 可以设置在指定的时间段不运行。
         self._schedule_tasks_on_main_thread = schedule_tasks_on_main_thread
@@ -447,21 +450,21 @@
         elif self._concurrent_mode == 3:
             check_evenlet_monkey_patch()
         else:
             check_not_monkey()
 
     ''' 日志跳转代码行不正确，不用这种方式'''
 
-    # def _log_error(self, msg, exc_info=None):
-    #     self.logger.error(msg=f'{msg} \n', exc_info=exc_info)
-    #     self.error_file_logger.error(msg=f'{msg} \n', exc_info=exc_info)
-    #
-    # def _log_critical(self, msg, exc_info=None):
-    #     self.logger.critical(msg=f'{msg} \n', exc_info=exc_info)
-    #     self.error_file_logger.critical(msg=f'{msg} \n', exc_info=exc_info)
+    def _log_error(self, msg, exc_info=None):
+        self.logger.error(msg=f'{msg} \n', exc_info=exc_info, extra={'sys_getframe_n': 3})
+        self.error_file_logger.error(msg=f'{msg} \n', exc_info=exc_info, extra={'sys_getframe_n': 3})
+
+    def _log_critical(self, msg, exc_info=None):
+        self.logger.critical(msg=f'{msg} \n', exc_info=exc_info, extra={'sys_getframe_n': 3})
+        self.error_file_logger.critical(msg=f'{msg} \n', exc_info=exc_info, extra={'sys_getframe_n': 3})
 
     @property
     @decorators.synchronized
     def concurrent_pool(self):
         return self._concurrent_mode_dispatcher.build_pool()
 
     def custom_init(self):
@@ -488,16 +491,17 @@
                         try:
                             result = func(*args, **kwargs)
                             if exit_if_function_run_sucsess:
                                 return result
                         except BaseException as e:
                             log_msg = func.__name__ + '   运行出错\n ' + traceback.format_exc(
                                 limit=10) if is_display_detail_exception else str(e)
-                            self.logger.error(msg=f'{log_msg} \n', exc_info=True)
-                            self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=True)
+                            # self.logger.error(msg=f'{log_msg} \n', exc_info=True)
+                            # self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=True)
+                            self._log_error(msg=log_msg, exc_info=True)
                         finally:
                             time.sleep(time_sleep)
 
                 if block:
                     return ___keep_circulating()
                 else:
                     threading.Thread(target=___keep_circulating, ).start()
@@ -520,17 +524,18 @@
         self._result_persistence_helper = ResultPersistenceHelper(self._function_result_status_persistance_conf, self._queue_name)
 
         self._distributed_consumer_statistics = DistributedConsumerStatistics(self)
         if self._is_send_consumer_hearbeat_to_redis:
             self._distributed_consumer_statistics.run()
             self.logger.warning(f'启动了分布式环境 使用 redis 的键 hearbeat:{self._queue_name} 统计活跃消费者 ，当前消费者唯一标识为 {self.consumer_identification}')
 
-        self.keep_circulating(10, block=False)(self.check_heartbeat_and_message_count)()  # 间隔时间最好比self._unit_time_for_count小整数倍，不然日志不准。
+        self.keep_circulating(60, block=False)(self.check_heartbeat_and_message_count)()  # 间隔时间最好比self._unit_time_for_count小整数倍，不然日志不准。
         if self._is_support_remote_kill_task:
-            kill_remote_task.RemoteTaskKiller(self.queue_name, None).start_cycle_kill_task()
+            self.keep_circulating(10, block=False)(kill_remote_task.RemoteTaskKiller(self.queue_name, None).start_cycle_kill_task)()
+            self._is_show_message_get_from_broker = True  # 方便用户看到从消息队列取出来的消息的task_id,然后使用task_id杀死运行中的消息。
         if self._do_task_filtering:
             self._redis_filter.delete_expire_filter_task_cycle()  # 这个默认是RedisFilter类，是个pass不运行。所以用别的消息中间件模式，不需要安装和配置redis。
         if self._schedule_tasks_on_main_thread:
             self.keep_circulating(1)(self._shedual_task)()
         else:
             self._concurrent_mode_dispatcher.schedulal_task_with_no_block()
         setattr(funboost_config_deafult, 'has_start_a_consumer_flag', 1)
@@ -735,16 +740,17 @@
             if self._get_priority_conf(kw, 'do_task_filtering'):
                 self._redis_filter.add_a_value(function_only_params)  # 函数执行成功后，添加函数的参数排序后的键值对字符串到set中。
             if current_function_result_status.success is False and current_retry_times == max_retry_times:
                 log_msg = f'函数 {self.consuming_function.__name__} 达到最大重试次数 {self._get_priority_conf(kw, "max_retry_times")} 后,仍然失败， 入参是  {function_only_params} '
                 if self._is_push_to_dlx_queue_when_retry_max_times:
                     log_msg += f'  。发送到死信队列 {self._dlx_queue_name} 中'
                     self.publisher_of_dlx_queue.publish(kw['body'])
-                self.logger.critical(msg=f'{log_msg} \n', )
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n', )
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
 
             if self._get_priority_conf(kw, 'is_using_rpc_mode'):
                 # print(function_result_status.get_status_dict(without_datetime_obj=
                 if (current_function_result_status.success is False and current_retry_times == max_retry_times) or current_function_result_status.success is True:
                     with RedisMixin().redis_db_filter_and_rpc_result.pipeline() as p:
                         # RedisMixin().redis_db_frame.lpush(kw['body']['extra']['task_id'], json.dumps(function_result_status.get_status_dict(without_datetime_obj=True)))
                         # RedisMixin().redis_db_frame.expire(kw['body']['extra']['task_id'], 600)
@@ -756,31 +762,34 @@
             with self._lock_for_count_execute_task_times_every_unit_time:
                 self._execute_task_times_every_unit_time += 1
                 self._consuming_function_cost_time_total_every_unit_time += time.time() - t_start_run_fun
                 self._last_execute_task_time = time.time()
                 if time.time() - self._current_time_for_execute_task_times_every_unit_time > self._unit_time_for_count:
                     avarage_function_spend_time = round(self._consuming_function_cost_time_total_every_unit_time / self._execute_task_times_every_unit_time, 4)
                     msg = f'{self._unit_time_for_count} 秒内执行了 {self._execute_task_times_every_unit_time} 次函数 [ {self.consuming_function.__name__} ] ,' \
-                          f'函数平均运行耗时 {avarage_function_spend_time} 秒'
-                    if self._msg_num_in_broker != -1:  # 有的中间件无法统计或没实现统计队列剩余数量的，统一返回的是-1，不显示这句话。
+                          f'函数平均运行耗时 {avarage_function_spend_time} 秒。 '
+                    self.logger.debug(msg)
+                    if self._msg_num_in_broker != -1 and time.time() - self._last_show_remaining_execution_time > self._show_remaining_execution_time_interval:  # 有的中间件无法统计或没实现统计队列剩余数量的，统一返回的是-1，不显示这句话。
                         # msg += f''' ，预计还需要 {time_util.seconds_to_hour_minute_second(self._msg_num_in_broker * avarage_function_spend_time / active_consumer_num)} 时间 才能执行完成 {self._msg_num_in_broker}个剩余的任务'''
                         need_time = time_util.seconds_to_hour_minute_second(self._msg_num_in_broker / (self._execute_task_times_every_unit_time / self._unit_time_for_count) /
                                                                             self._distributed_consumer_statistics.active_consumer_num)
-                        msg += f''' ，预计还需要 {need_time}''' + \
-                               f''' 时间 才能执行完成 {self._msg_num_in_broker}个剩余的任务'''
-                    self.logger.info(msg)
+                        msg += f''' 预计还需要 {need_time} 时间 才能执行完成 队列 {self.queue_name} 中的 {self._msg_num_in_broker} 个剩余任务'''
+                        self.logger.info(msg)
+                        self._last_show_remaining_execution_time = time.time()
                     self._current_time_for_execute_task_times_every_unit_time = time.time()
                     self._consuming_function_cost_time_total_every_unit_time = 0
                     self._execute_task_times_every_unit_time = 0
+
             if self._user_custom_record_process_info_func:
                 self._user_custom_record_process_info_func(current_function_result_status)
         except BaseException as e:
             log_msg = f' error 严重错误 {type(e)} {e} '
-            self.logger.critical(msg=f'{log_msg} \n', exc_info=True)
-            self.error_file_logger.critical(msg=f'{log_msg} \n', exc_info=True)
+            # self.logger.critical(msg=f'{log_msg} \n', exc_info=True)
+            # self.error_file_logger.critical(msg=f'{log_msg} \n', exc_info=True)
+            self._log_critical(msg=log_msg, exc_info=True)
 
     # noinspection PyProtectedMember
     def _run_consuming_function_with_confirm_and_retry(self, kw: dict, current_retry_times,
                                                        function_result_status: FunctionResultStatus, ):
         function_only_params = delete_keys_and_return_new_dict(kw['body']) if self._do_not_delete_extra_from_msg is False else kw['body']
         task_id = kw['body']['extra']['task_id']
         t_start = time.time()
@@ -791,59 +800,65 @@
             function_run = function_run0 if not function_timeout else self._concurrent_mode_dispatcher.timeout_deco(
                 function_timeout)(function_run0)
             if self._is_support_remote_kill_task:
                 if kill_remote_task.RemoteTaskKiller(self.queue_name, task_id).judge_need_revoke_run():  # 如果远程指令杀死任务，如果还没开始运行函数，就取消运行
                     function_result_status._has_kill_task = True
                     self.logger.warning(f'取消运行 {task_id} {function_only_params}')
                     return function_result_status
-                function_run = kill_remote_task.kill_fun_deco(task_id)(function_run)  # 用杀死装饰器包装起来在另一个线程运行函数
+                function_run = kill_remote_task.kill_fun_deco(task_id)(function_run)  # 用杀死装饰器包装起来在另一个线程运行函数,以便等待远程杀死。
             function_result_status.result = function_run(**function_only_params)
             if asyncio.iscoroutine(function_result_status.result):
                 log_msg = f'''异步的协程消费函数必须使用 async 并发模式并发,请设置消费函数 {self.consuming_function.__name__} 的concurrent_mode 为 ConcurrentModeEnum.ASYNC 或 4'''
-                self.logger.critical(msg=f'{log_msg} \n')
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n')
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
                 # noinspection PyProtectedMember,PyUnresolvedReferences
 
                 os._exit(4)
             function_result_status.success = True
             if self._log_level <= logging.DEBUG:
                 result_str_to_be_print = str(function_result_status.result)[:100] if len(str(function_result_status.result)) < 100 else str(function_result_status.result)[:100] + '  。。。。。  '
                 self.logger.debug(f' 函数 {self.consuming_function.__name__}  '
                                   f'第{current_retry_times + 1}次 运行, 正确了，函数运行时间是 {round(time.time() - t_start, 4)} 秒,入参是 {function_only_params}  '
                                   f' 结果是  {result_str_to_be_print} ，  {self._get_concurrent_info()}  ')
         except BaseException as e:
             if isinstance(e, (ExceptionForRequeue,)):  # mongo经常维护备份时候插入不了或挂了，或者自己主动抛出一个ExceptionForRequeue类型的错误会重新入队，不受指定重试次数逇约束。
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e} 。消息重新放入当前队列 {self._queue_name}'
-                self.logger.critical(msg=f'{log_msg} \n')
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n')
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
                 time.sleep(0.1)  # 防止快速无限出错入队出队，导致cpu和中间件忙
                 # 重回队列如果不修改task_id,insert插入函数消费状态结果到mongo会主键重复。要么保存函数消费状态使用replace，要么需要修改taskikd
                 # kw_new = copy.deepcopy(kw)
                 # new_task_id =f'{self._queue_name}_result:{uuid.uuid4()}'
                 # kw_new['body']['extra']['task_id'] = new_task_id
                 # self._requeue(kw_new)
                 self._requeue(kw)
                 function_result_status._has_requeue = True
             if isinstance(e, ExceptionForPushToDlxqueue):
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e}，消息放入死信队列 {self._dlx_queue_name}'
-                self.logger.critical(msg=f'{log_msg} \n')
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n')
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
                 self.publisher_of_dlx_queue.publish(kw['body'])  # 发布到死信队列，不重回当前队列
                 function_result_status._has_to_dlx_queue = True
             if isinstance(e, kill_remote_task.TaskHasKilledError):
                 log_msg = f'task_id 为 {task_id} , 函数 [{self.consuming_function.__name__}] 运行入参 {function_only_params}   ，已被远程指令杀死 {type(e)}  {e}'
-                self.logger.critical(msg=f'{log_msg} ')
-                self.error_file_logger.critical(msg=f'{log_msg} ')
+                # self.logger.critical(msg=f'{log_msg} ')
+                # self.error_file_logger.critical(msg=f'{log_msg} ')
+                self._log_critical(msg=log_msg)
                 function_result_status._has_kill_task = True
             if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue, kill_remote_task.TaskHasKilledError)):
                 return function_result_status
             log_msg = f'''函数 {self.consuming_function.__name__}  第{current_retry_times + 1}次运行发生错误，
-                              函数运行时间是 {round(time.time() - t_start, 4)} 秒,\n  入参是  {function_only_params}    \n 原因是 {type(e)} {e} '''
-            self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
-            self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
+                          函数运行时间是 {round(time.time() - t_start, 4)} 秒,  入参是  {function_only_params}    
+                          {type(e)} {e} '''
+            # self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
+            # self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
+            self._log_error(msg=log_msg, exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             # traceback.print_exc()
             function_result_status.exception = f'{e.__class__.__name__}    {str(e)}'
             function_result_status.result = FunctionResultStatus.FUNC_RUN_ERROR
         return function_result_status
 
     # noinspection PyProtectedMember
     async def _async_run(self, kw: dict, ):
@@ -872,16 +887,17 @@
                 # self._redis_filter.add_a_value(function_only_params)  # 函数执行成功后，添加函数的参数排序后的键值对字符串到set中。
                 await simple_run_in_executor(self._redis_filter.add_a_value, function_only_params)
             if current_function_result_status.success is False and current_retry_times == max_retry_times:
                 log_msg = f'函数 {self.consuming_function.__name__} 达到最大重试次数 {self._get_priority_conf(kw, "max_retry_times")} 后,仍然失败， 入参是  {function_only_params} '
                 if self._is_push_to_dlx_queue_when_retry_max_times:
                     log_msg += f'  。发送到死信队列 {self._dlx_queue_name} 中'
                     await simple_run_in_executor(self.publisher_of_dlx_queue.publish, kw['body'])
-                self.logger.critical(msg=f'{log_msg} \n', )
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n', )
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
 
                 # self._confirm_consume(kw)  # 错得超过指定的次数了，就确认消费了。
             if self._get_priority_conf(kw, 'is_using_rpc_mode'):
                 def push_result():
                     with RedisMixin().redis_db_filter_and_rpc_result.pipeline() as p:
                         p.lpush(kw['body']['extra']['task_id'],
                                 json.dumps(current_function_result_status.get_status_dict(without_datetime_obj=True)))
@@ -894,48 +910,51 @@
             # 异步执行不存在线程并发，不需要加锁。
             self._execute_task_times_every_unit_time += 1
             self._consuming_function_cost_time_total_every_unit_time += time.time() - t_start_run_fun
             self._last_execute_task_time = time.time()
             if time.time() - self._current_time_for_execute_task_times_every_unit_time > self._unit_time_for_count:
                 avarage_function_spend_time = round(self._consuming_function_cost_time_total_every_unit_time / self._execute_task_times_every_unit_time, 4)
                 msg = f'{self._unit_time_for_count} 秒内执行了 {self._execute_task_times_every_unit_time} 次函数 [ {self.consuming_function.__name__} ] ,' \
-                      f'函数平均运行耗时 {avarage_function_spend_time} 秒'
-                if self._msg_num_in_broker != -1:
-                    if self._msg_num_in_broker != -1:  # 有的中间件无法统计或没实现统计队列剩余数量的，统一返回的是-1，不显示这句话。
-                        # msg += f''' ，预计还需要 {time_util.seconds_to_hour_minute_second(self._msg_num_in_broker * avarage_function_spend_time / active_consumer_num)} 时间 才能执行完成 {self._msg_num_in_broker}个剩余的任务'''
-                        need_time = time_util.seconds_to_hour_minute_second(self._msg_num_in_broker / (self._execute_task_times_every_unit_time / self._unit_time_for_count) /
-                                                                            self._distributed_consumer_statistics.active_consumer_num)
-                        msg += f''' ，预计还需要 {need_time}''' + \
-                               f''' 时间 才能执行完成 {self._msg_num_in_broker}个剩余的任务'''
-                self.logger.info(msg)
+                      f'函数平均运行耗时 {avarage_function_spend_time} 秒。 '
+                self.logger.debug(msg)
+                if self._msg_num_in_broker != -1 and time.time() - self._last_show_remaining_execution_time > self._show_remaining_execution_time_interval:  # 有的中间件无法统计或没实现统计队列剩余数量的，统一返回的是-1，不显示这句话。
+                    # msg += f''' ，预计还需要 {time_util.seconds_to_hour_minute_second(self._msg_num_in_broker * avarage_function_spend_time / active_consumer_num)} 时间 才能执行完成 {self._msg_num_in_broker}个剩余的任务'''
+                    need_time = time_util.seconds_to_hour_minute_second(self._msg_num_in_broker / (self._execute_task_times_every_unit_time / self._unit_time_for_count) /
+                                                                        self._distributed_consumer_statistics.active_consumer_num)
+                    msg += f''' 预计还需要 {need_time} 时间 才能执行完成 队列 {self.queue_name} 中的 {self._msg_num_in_broker} 个剩余任务'''
+                    self.logger.info(msg)
+                    self._last_show_remaining_execution_time = time.time()
                 self._current_time_for_execute_task_times_every_unit_time = time.time()
                 self._consuming_function_cost_time_total_every_unit_time = 0
                 self._execute_task_times_every_unit_time = 0
+
             if self._user_custom_record_process_info_func:
                 await self._user_custom_record_process_info_func(current_function_result_status)
         except BaseException as e:
             log_msg = f' error 严重错误 {type(e)} {e} '
-            self.logger.critical(msg=f'{log_msg} \n', exc_info=True)
-            self.error_file_logger.critical(msg=f'{log_msg} \n', exc_info=True)
+            # self.logger.critical(msg=f'{log_msg} \n', exc_info=True)
+            # self.error_file_logger.critical(msg=f'{log_msg} \n', exc_info=True)
+            self._log_critical(msg=log_msg, exc_info=True)
 
     # noinspection PyProtectedMember
     async def _async_run_consuming_function_with_confirm_and_retry(self, kw: dict, current_retry_times,
                                                                    function_result_status: FunctionResultStatus, ):
         """虽然和上面有点大面积重复相似，这个是为了asyncio模式的，asyncio模式真的和普通同步模式的代码思维和形式区别太大，
         框架实现兼容async的消费函数很麻烦复杂，连并发池都要单独写"""
         function_only_params = delete_keys_and_return_new_dict(kw['body']) if self._do_not_delete_extra_from_msg is False else kw['body']
         function_result_status.run_times = current_retry_times + 1
         # noinspection PyBroadException
         t_start = time.time()
         try:
             corotinue_obj = self.consuming_function(**function_only_params)
             if not asyncio.iscoroutine(corotinue_obj):
                 log_msg = f'''当前设置的并发模式为 async 并发模式，但消费函数不是异步协程函数，请不要把消费函数 {self.consuming_function.__name__} 的 concurrent_mode 设置为 4'''
-                self.logger.critical(msg=f'{log_msg} \n')
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n')
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
                 # noinspection PyProtectedMember,PyUnresolvedReferences
                 os._exit(444)
             if self._function_timeout == 0:
                 rs = await corotinue_obj
                 # rs = await asyncio.wait_for(corotinue_obj, timeout=4)
             else:
                 rs = await asyncio.wait_for(corotinue_obj, timeout=self._function_timeout)
@@ -945,33 +964,37 @@
                 result_str_to_be_print = str(rs)[:100] if len(str(rs)) < 100 else str(rs)[:100] + '  。。。。。  '
                 self.logger.debug(f' 函数 {self.consuming_function.__name__}  '
                                   f'第{current_retry_times + 1}次 运行, 正确了，函数运行时间是 {round(time.time() - t_start, 4)} 秒,'
                                   f'入参是 【 {function_only_params} 】 ,结果是 {result_str_to_be_print}  。 {corotinue_obj} ')
         except BaseException as e:
             if isinstance(e, (ExceptionForRequeue,)):  # mongo经常维护备份时候插入不了或挂了，或者自己主动抛出一个ExceptionForRequeue类型的错误会重新入队，不受指定重试次数逇约束。
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e} 。 消息重新放入当前队列 {self._queue_name}'
-                self.logger.critical(msg=f'{log_msg} \n')
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n')
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
                 # time.sleep(1)  # 防止快速无限出错入队出队，导致cpu和中间件忙
                 await asyncio.sleep(0.1)
                 # return self._requeue(kw)
                 await simple_run_in_executor(self._requeue, kw)
                 function_result_status._has_requeue = True
             if isinstance(e, ExceptionForPushToDlxqueue):
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e}，消息放入死信队列 {self._dlx_queue_name}'
-                self.logger.critical(msg=f'{log_msg} \n')
-                self.error_file_logger.critical(msg=f'{log_msg} \n')
+                # self.logger.critical(msg=f'{log_msg} \n')
+                # self.error_file_logger.critical(msg=f'{log_msg} \n')
+                self._log_critical(msg=log_msg)
                 await simple_run_in_executor(self.publisher_of_dlx_queue.publish, kw['body'])  # 发布到死信队列，不重回当前队列
                 function_result_status._has_to_dlx_queue = True
             if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue)):
                 return function_result_status
             log_msg = f'''函数 {self.consuming_function.__name__}  第{current_retry_times + 1}次运行发生错误，
-                              函数运行时间是 {round(time.time() - t_start, 4)} 秒,\n  入参是  {function_only_params}    \n 原因是 {type(e)} {e} '''
-            self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
-            self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
+                          函数运行时间是 {round(time.time() - t_start, 4)} 秒,  入参是  {function_only_params}     
+                          原因是 {type(e)} {e} '''
+            # self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
+            # self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
+            self._log_error(msg=log_msg, exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             function_result_status.exception = f'{e.__class__.__name__}    {str(e)}'
             function_result_status.result = FunctionResultStatus.FUNC_RUN_ERROR
         return function_result_status
 
     @abc.abstractmethod
     def _confirm_consume(self, kw):
         """确认消费"""
@@ -1000,16 +1023,17 @@
         ev.function = job.func
         :return:
         """
         # print(event.scheduled_run_time)
         misfire_grace_time = self._get_priority_conf(event.function_kwargs["kw"], 'misfire_grace_time')
         log_msg = f''' 现在时间是 {time_util.DatetimeConverter().datetime_str} ,比此任务规定的本应该的运行时间 {event.scheduled_run_time} 相比 超过了指定的 {misfire_grace_time} 秒,放弃执行此任务 
                              {event.function_kwargs["kw"]["body"]} '''
-        self.logger.critical(msg=f'{log_msg} \n')
-        self.error_file_logger.critical(msg=f'{log_msg} \n')
+        # self.logger.critical(msg=f'{log_msg} \n')
+        # self.error_file_logger.critical(msg=f'{log_msg} \n')
+        self._log_critical(msg=log_msg)
         self._confirm_consume(event.function_kwargs["kw"])
 
         '''
         if self._get_priority_conf(event.function_kwargs["kw"], 'execute_delay_task_even_if_when_task_is_expired') is False:
             self.logger.critical(f'现在时间是 {time_util.DatetimeConverter().datetime_str} ,此任务设置的延时运行已过期 \n'
                                  f'{event.function_kwargs["kw"]["body"]} ， 此任务放弃执行')
             self._confirm_consume(event.function_kwargs["kw"])
```

## funboost/consumers/celery_consumer.py

```diff
@@ -152,21 +152,37 @@
         resultrepr_maxsize = 1024
 
         #: Task request stack, the current request will be the topmost.
         request_stack = None
     '''
 
     def custom_init(self):
-        # 这就是核心，@boost时候回注册任务路由到celery_app
+        # 这就是核心，@boost时候会 @ celery app.task装饰器
         @celery_app.task(name=self.queue_name, rate_limit=f'{self._qps}/s', soft_time_limit=self._function_timeout,
                          max_retries=self._max_retry_times,
-                         **self.broker_exclusive_config['celery_task_config'])
-        def f(*args, **kwargs):
+                         **self.broker_exclusive_config['celery_task_config'],
+                         bind=True)
+        def f(this, *args, **kwargs):
             self.logger.debug(f' 这条消息是 celery 从 {self.queue_name} 队列中取出 ,是由 celery 框架调度 {self.consuming_function.__name__} 函数处理: args:  {args} ,  kwargs: {kwargs}')
-            return self.consuming_function(*args, **kwargs)
+            # return self.consuming_function(*args, **kwargs) # 如果没有声明 autoretry_for ，那么消费函数出错了就不会自动重试了。
+            try:
+                return self.consuming_function(*args, **kwargs)
+            except BaseException as exc:  # 改成自动重试。
+                # print(this.request.__dict__,dir(this))
+
+                if this.request.retries != self._max_retry_times:
+                    log_msg = f'fun: {self.consuming_function}  args: {args} , kwargs: {kwargs} 消息第{this.request.retries}次运行出错,  {exc} \n'
+                    self._log_error(log_msg, exc_info=self._is_print_detail_exception)
+                else:
+                    log_msg = f'fun: {self.consuming_function}  args: {args} , kwargs: {kwargs} 消息达到最大重试次数{this.request.retries}次仍然出错,  {exc} \n'
+                    self._log_critical(log_msg, exc_info=self._is_print_detail_exception)
+                # 发生异常，尝试重试任务,countdown 是多少秒后重试
+                raise this.retry(exc=exc, countdown=5)
+
+        celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})  # 自动配置celery每个函数使用不同的队列名。
         self.celery_task = f
         CeleryHelper.concurrent_mode = self._concurrent_mode
 
     def start_consuming_message(self):
         # 不单独每个函数都启动一次celery的worker消费，是把要消费的 queue name放到列表中，CeleryHelper.realy_start_celery_worker 一次性启动多个函数消费。
         CeleryHelper.to_be_start_work_celery_queue_name_set.add(self.queue_name)
         super().start_consuming_message()
```

## funboost/consumers/rabbitmq_amqpstorm_consumer.py

```diff
@@ -25,15 +25,15 @@
             body = json.loads(body)
             kw = {'amqpstorm_message': amqpstorm_message, 'body': body}
             self._submit_task(kw)
 
         rp = RabbitmqPublisherUsingAmqpStorm(self.queue_name,broker_exclusive_config=self.broker_exclusive_config)
         rp.init_broker()
         rp.channel_wrapper_by_ampqstormbaic.qos(self._concurrent_num)
-        rp.channel_wrapper_by_ampqstormbaic.consume(callback=callback, queue=self.queue_name, no_ack=False)
+        rp.channel_wrapper_by_ampqstormbaic.consume(callback=callback, queue=self.queue_name, no_ack=False,)
         rp.channel.start_consuming(auto_decode=True)
 
     def _confirm_consume(self, kw):
         # noinspection PyBroadException
         try:
             kw['amqpstorm_message'].ack()  # 确认消费
         except BaseException as e:
```

## funboost/consumers/redis_consumer_ack_able.py

```diff
@@ -152,11 +152,11 @@
                 self._print_message_get_from_broker('redis', task_str_list)
                 # self.logger.debug(f'从redis的 [{self._queue_name}] 队列中 取出的消息是：  {task_str_list}  ')
                 for task_str in task_str_list:
                     task_dict = json.loads(task_str)
                     kw = {'body': task_dict, 'task_str': task_str}
                     self._submit_task(kw)
             else:
-                time.sleep(0.5)
+                time.sleep(0.2)
 
     def _requeue(self, kw):
         self.redis_db_frame.rpush(self._queue_name, json.dumps(kw['body']))
```

## funboost/consumers/redis_consumer_priority.py

```diff
@@ -6,14 +6,17 @@
 这个是加强版的可确认消费的redis消费实现，所以比redis_conusmer实现复杂很多。
 这个可以确保随意反复多次停止重启脚本，任务不丢失，没人采用lua，随意反复重启代码极小概率丢失一个任务。
 
 这个是支持任务优先级的redis队列实现。
 """
 import json
 import time
+
+import redis3
+
 from funboost.consumers.redis_consumer_ack_able import RedisConsumerAckAble
 
 
 class RedisPriorityConsumer(RedisConsumerAckAble):
     """
        使用多个redis list来实现redis支持队列优先级。brpop可以支持监听多个redis键。
        根据消息的 priroty 来决定发送到哪个队列。我这个想法和celery依赖的kombu实现的redis具有队列优先级是一样的。
@@ -45,24 +48,50 @@
             f.publish({'x': randx}, priority_control_config=PriorityConsumingControlConfig(other_extra_params={'priroty': randx}))
         print(f.get_message_count())
         f.consume()
     """
 
     BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'x-max-priority': None}  # x-max-priority 是 rabbitmq的优先级队列配置，必须为整数，强烈建议要小于5。为None就代表队列不支持优先级。
 
-    def _shedual_task(self):
+    def _shedual_task0000(self):
 
         while True:
             # task_str_list = script(keys=[queues_str, self._unack_zset_name], args=[time.time()])
             task_tuple = self.redis_db_frame_version3.blpop(keys=self.publisher_of_same_queue.queue_list, timeout=60)  # 监听了多个键名，所以间接实现了优先级，和kombu的redis 支持优先级的设计思路不谋而合。
             if task_tuple:
                 msg = task_tuple[1]
                 self.redis_db_frame_version3.zadd(self._unack_zset_name, {msg: time.time()})
                 self.logger.debug(task_tuple)
                 self._print_message_get_from_broker('redis', msg)
                 # self.logger.debug(f'从redis的 [{self._queue_name}] 队列中 取出的消息是：  {task_str_list}  ')
                 task_dict = json.loads(msg)
                 kw = {'body': task_dict, 'task_str': msg}
                 self._submit_task(kw)
 
+    def _shedual_task(self):
+        """https://redis.readthedocs.io/en/latest/advanced_features.html#default-pipelines """
+        while True:
+            # task_str_list = script(keys=[queues_str, self._unack_zset_name], args=[time.time()])
+            while True:
+                try:
+                    with self.redis_db_frame_version3.pipeline() as p:
+                        p.watch(self._unack_zset_name, *self.publisher_of_same_queue.queue_list, )
+                        task_tuple = p.blpop(keys=self.publisher_of_same_queue.queue_list, timeout=60)  # 监听了多个键名，所以间接实现了优先级，和kombu的redis 支持优先级的设计思路不谋而合。
+                        # print(task_tuple)
+                        if task_tuple:
+                            msg = task_tuple[1]
+                            p.zadd(self._unack_zset_name, {msg: time.time()})
+                            # self.logger.debug(task_tuple)
+                            p.unwatch()
+                            p.execute()
+                            break
+                except redis3.WatchError:
+                    continue
+            if task_tuple:
+                self._print_message_get_from_broker('redis', msg)
+                # self.logger.debug(f'从redis的 [{self._queue_name}] 队列中 取出的消息是：  {task_str_list}  ')
+                task_dict = json.loads(msg)
+                kw = {'body': task_dict, 'task_str': msg}
+                self._submit_task(kw)
+
     def _requeue(self, kw):
         self.publisher_of_same_queue.publish(kw['body'])
```

## funboost/publishers/base_publisher.py

```diff
@@ -195,15 +195,15 @@
     @staticmethod
     def _get_from_other_extra_params(k: str, msg):
         msg_dict = json.loads(msg) if isinstance(msg, str) else msg
         return msg_dict['extra'].get('other_extra_params', {}).get(k, None)
 
     def _convert_msg(self, msg: typing.Union[str, dict], task_id=None,
                      priority_control_config: PriorityConsumingControlConfig = None) -> (typing.Dict, typing.Dict, typing.Dict):
-        if isinstance(msg, (str,bytes)):
+        if isinstance(msg, (str, bytes)):
             msg = json.loads(msg)
         msg_function_kw = copy.deepcopy(msg)
         raw_extra = {}
         if 'extra' in msg:
             msg_function_kw.pop('extra')
             raw_extra = msg['extra']
         if self.publish_params_checker:
@@ -211,26 +211,26 @@
         task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
         extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
                         'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
         if priority_control_config:
             extra_params.update(priority_control_config.to_dict())
         extra_params.update(raw_extra)
         msg['extra'] = extra_params
-        return msg, msg_function_kw, extra_params,task_id
+        return msg, msg_function_kw, extra_params, task_id
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None):
         """
 
         :param msg:函数的入参字典或者字典转json。,例如消费函数是 def add(x,y)，你就发布 {"x":1,"y":2}
         :param task_id:可以指定task_id,也可以不指定就随机生产uuid
         :param priority_control_config:优先级配置，消息可以携带优先级配置，覆盖boost的配置。
         :return:
         """
-        msg, msg_function_kw, extra_params,task_id = self._convert_msg(msg, task_id, priority_control_config)
+        msg, msg_function_kw, extra_params, task_id = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         decorators.handle_exception(retry_times=10, is_throw_error=True, time_sleep=0.1)(
             self.concrete_realization_of_publish)(json.dumps(msg, ensure_ascii=False))
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
```

## funboost/publishers/celery_publisher.py

```diff
@@ -1,47 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 12:12
 import os
 import sys
-import uuid
-import copy
 import time
-import threading
-import json
 import celery
 import celery.result
 import typing
 
 from funboost.assist.celery_helper import celery_app
 from funboost.publishers.base_publisher import AbstractPublisher, PriorityConsumingControlConfig
 
 
 class CeleryPublisher(AbstractPublisher, ):
     """
     使用celery作为中间件
     """
-    celery_conf_lock = threading.Lock()
-
-    # noinspection PyAttributeOutsideInit
-    def custom_init(self):
-        # self.broker_exclusive_config['task_routes'] = {self.queue_name: {"queue": self.queue_name}}
-        # celery_app.config_from_object(self.broker_exclusive_config)
-        pass
-
-        # celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})
-        #
-        # @celery_app.task(name=self.queue_name)
-        # def f(*args, **kwargs):
-        #     pass
-        #
-        # self._celery_app = celery_app
-        # self._celery_fun = f
-
-        celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None) -> celery.result.AsyncResult:
         msg, msg_function_kw, extra_params,task_id = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         celery_result = celery_app.send_task(name=self.queue_name, kwargs=msg_function_kw, task_id=extra_params['task_id'])  # type: celery.result.AsyncResult
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
```

## funboost/publishers/redis_publisher.py

```diff
@@ -5,18 +5,19 @@
 import time
 # noinspection PyUnresolvedReferences
 from queue import Queue, Empty
 from threading import Lock
 
 from funboost import funboost_config_deafult
 from funboost.publishers.base_publisher import AbstractPublisher
+from funboost.publishers.redis_queue_flush import FlushRedisQueueMixin
 from funboost.utils import RedisMixin, decorators
 
 
-class RedisPublisher(AbstractPublisher, RedisMixin):
+class RedisPublisher(FlushRedisQueueMixin, AbstractPublisher, RedisMixin, ):
     """
     使用redis作为中间件,这个是大幅优化了发布速度的方式。简单的发布是 redis_publisher_0000.py 中的代码方式。
 
     这个是复杂版，批量推送，简单版在 funboost/publishers/redis_publisher_simple.py
     """
     _push_method = 'rpush'
 
@@ -38,36 +39,25 @@
         with self._lock_for_bulk_push:
             self.__bulk_push_and_init()
 
     def concrete_realization_of_publish(self, msg):
         # print(getattr(frame_config,'has_start_a_consumer_flag',0))
         # 这里的 has_start_a_consumer_flag 是一个标志，借用此模块设置的一个标识变量而已，框架运行时候自动设定的，不要把这个变量写到模块里面。
         # if getattr(funboost_config_deafult, 'has_start_a_consumer_flag', 0) == 0:  # 加快速度推送，否则每秒只能推送4000次。如果是独立脚本推送，使用批量推送，如果是消费者中发布任务，为了保持原子性，用原来的单个推送。
-        if self.broker_exclusive_config.get('redis_bulk_push',0) == 1:   # RedisConsumer传了,  RedisAckAble  没传
+        if self.broker_exclusive_config.get('redis_bulk_push', 0) == 1:  # RedisConsumer传了,  RedisAckAble  没传
             # self._temp_msg_queue.put(msg)
             with self._lock_for_bulk_push:
                 self._temp_msg_list.append(msg)
                 if len(self._temp_msg_list) >= 1000:
                     # print(len(self._temp_msg_list))
                     self.__bulk_push_and_init()
         else:
             getattr(self.redis_db_frame, self._push_method)(self._queue_name, msg)
             # print(msg)
 
-        # self.redis_db_frame.rpush(self._queue_name, msg)
-    def clear(self):
-        self.redis_db_frame.delete(self._queue_name)
-        # self.redis_db_frame.delete(f'{self._queue_name}__unack')
-        unack_queue_name_list = self.redis_db_frame.scan(match=f'{self._queue_name}__unack_id_*', count=10000)[1] + \
-                                self.redis_db_frame.scan(match=f'unack_{self._queue_name}_*', count=10000)[1]  # noqa
-        self.logger.warning(f'清除 {self._queue_name} 队列中的消息成功')
-        if unack_queue_name_list:
-            self.redis_db_frame.delete(*unack_queue_name_list)
-            self.logger.warning(f'清除 {unack_queue_name_list} 队列中的消息成功')
-
     def get_message_count(self):
         # print(self.redis_db7,self._queue_name)
         return self.redis_db_frame.llen(self._queue_name)
 
     def close(self):
         # self.redis_db7.connection_pool.disconnect()
         pass
```

## funboost/publishers/redis_publisher_priority.py

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 12:12
 
 from funboost.publishers.base_publisher import AbstractPublisher
+from funboost.publishers.redis_queue_flush import FlushRedisQueueMixin
 from funboost.utils.redis_manager import RedisMixin
 
 
-class RedisPriorityPublisher(AbstractPublisher, RedisMixin):
+class RedisPriorityPublisher(FlushRedisQueueMixin,AbstractPublisher, RedisMixin,):
     """
     redis队列，支持任务优先级。
     """
 
     def custom_init(self):
         queue_list = [self._queue_name]
         x_max_priority = self.broker_exclusive_config['x-max-priority']
@@ -35,18 +36,14 @@
         return queue_name
 
     def concrete_realization_of_publish(self, msg):
         queue_name = self.build_queue_name_by_msg(msg)
         self.logger.debug([queue_name, msg])
         self.redis_db_frame.rpush(queue_name, msg)
 
-    def clear(self):
-        self.redis_db_frame.delete(*self.queue_list)
-        self.redis_db_frame.delete(f'{self._queue_name}__unack')
-        self.logger.warning(f'清除 {self._queue_name} 队列中的消息成功')
 
     def get_message_count(self):
         count = 0
         for queue_name in self.queue_list:
             count += self.redis_db_frame.llen(queue_name)
         return count
```

## funboost/publishers/redis_publisher_simple.py

```diff
@@ -1,27 +1,23 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2023/8/8 0008 12:12
 from funboost.publishers.base_publisher import AbstractPublisher
+from funboost.publishers.redis_queue_flush import FlushRedisQueueMixin
 from funboost.utils import RedisMixin
 
 
-class RedisPublisher(AbstractPublisher, RedisMixin):
+class RedisPublisher(FlushRedisQueueMixin, AbstractPublisher, RedisMixin, ):
     """
     使用redis作为中间件
     """
 
     def concrete_realization_of_publish(self, msg):
         self.redis_db_frame.rpush(self._queue_name, msg)
 
-    def clear(self):
-        self.redis_db_frame.delete(self._queue_name)
-        self.redis_db_frame.delete(f'{self._queue_name}__unack')
-        self.logger.warning(f'清除 {self._queue_name} 队列中的消息成功')
-
     def get_message_count(self):
         # nb_print(self.redis_db7,self._queue_name)
         return self.redis_db_frame.llen(self._queue_name)
 
     def close(self):
         # self.redis_db7.connection_pool.disconnect()
         pass
```

## funboost/publishers/redis_pubsub_publisher.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 12:12
 from funboost.publishers.base_publisher import AbstractPublisher
 from funboost.utils import RedisMixin
 
 
-class RedisPubSubPublisher(AbstractPublisher, RedisMixin):
+class RedisPubSubPublisher(AbstractPublisher, RedisMixin, ):
     """
     使用redis作为中间件
     """
 
     def concrete_realization_of_publish(self, msg):
         self.redis_db_frame.publish(self._queue_name, msg)
```

## funboost/utils/redis_manager.py

```diff
@@ -10,15 +10,15 @@
 class RedisManager(object):
     _pool_dict = {}
 
     def __init__(self, host='127.0.0.1', port=6379, db=0, password='123456'):
         if (host, port, db, password) not in self.__class__._pool_dict:
             # print ('创建一个连接池')
             self.__class__._pool_dict[(host, port, db, password)] = redis.ConnectionPool(host=host, port=port, db=db,
-                                                                                         password=password)
+                                                                                         password=password,max_connections=100)
         self._r = redis.Redis(connection_pool=self._pool_dict[(host, port, db, password)])
         self._ping()
 
     def get_redis(self):
         """
         :rtype :redis.Redis
         """
@@ -37,15 +37,15 @@
     可以被作为万能mixin能被继承，也可以单独实例化使用。
     """
 
     @property
     @decorators.cached_method_result
     def redis_db0(self):
         return RedisManager(host=funboost_config_deafult.REDIS_HOST, port=funboost_config_deafult.REDIS_PORT,
-                            password=funboost_config_deafult.REDIS_PASSWORD, db=0).get_redis()
+                            password=funboost_config_deafult.REDIS_PASSWORD, db=0,).get_redis()
 
     @property
     @decorators.cached_method_result
     def redis_db8(self):
         return RedisManager(host=funboost_config_deafult.REDIS_HOST, port=funboost_config_deafult.REDIS_PORT,
                             password=funboost_config_deafult.REDIS_PASSWORD, db=8).get_redis()
```

## Comparing `funboost-23.5.dist-info/LICENSE` & `funboost-23.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-23.5.dist-info/METADATA` & `funboost-23.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 23.5
+Version: 23.6
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -46,15 +46,15 @@
 Requires-Dist: peewee (==3.15.1)
 Requires-Dist: apscheduler (==3.10.1)
 Requires-Dist: pikav0
 Requires-Dist: pikav1
 Requires-Dist: redis2
 Requires-Dist: redis3
 Requires-Dist: redis
-Requires-Dist: nb-log (>=8.5)
+Requires-Dist: nb-log (>=9.0)
 Requires-Dist: rocketmq
 Requires-Dist: zmq
 Requires-Dist: pyzmq
 Requires-Dist: paho-mqtt
 Requires-Dist: setuptools-rust
 Requires-Dist: fabric2 (==2.6.0)
 Requires-Dist: nats-python
@@ -155,17 +155,19 @@
 
 
 <span style="font-size:15px">旧框架地址：<span><a href="https://github.com/ydf0509/distributed_framework" style="font-size: 15px">function_scheduling_distributed_framework框架地址链接</a>
 
 
 ## 1.1 安装方式
 
+```
 pip install funboost --upgrade
 
-
+或pip install funboost[extra_brokers]  一次性安装所有小众三方中间件
+```
 
 ## 1.2 框架功能介绍
 
 分布式函数调度框架，支持5种并发模式，20+种消息中间件，20种任务控制功能。<br>
 用途概念就是常规经典的 生产者 + 消息队列中间件 + 消费者 编程思想。
 
 有了这个框架，用户再也无需亲自手写操作进程、线程、协程的并发的代码了。
@@ -327,14 +329,20 @@
      远程服务器部署消费函数：
         代码里面 task_fun.fabric_deploy('192.168.6.133', 22, 'xiaomin', '123456', process_num=2) 只需要这样就可以自动将函数部署在远程机器运行，
         无需任何额外操作，不需要借助阿里云codepipeline发版工具 和 任何运维发版管理工具，就能轻松将函数运行在多台远程机器。task_fun指的是被@boost装饰的函数
 
      暂停消费：
         支持从python解释器外部/远程机器 ，控制暂停消息消费和继续消费。
 
+     优先级队列：
+         支持队列优先级消息。
+
+     远程杀死任务：
+         支持在发布端杀死正在运行的消息，发送杀死命令时候对还未取出的消息则放弃运行消息。
+
 </pre>
 
 
 关于稳定性和性能，一句话概括就是直面百万c端用户（包括app和小程序）， 已经连续超过三个季度稳定高效运行无事故，从没有出现过假死、崩溃、内存泄漏等问题。 windows和linux行为100%一致，不会像celery一样，相同代码前提下，很多功能在win上不能运行或出错。
 
 
 ## 1.3 框架使用例子
```

## Comparing `funboost-23.5.dist-info/RECORD` & `funboost-23.6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-funboost/__init__.py,sha256=eBTjiQBcy0DoDZiOdcRJpgb5RHwv8d1ekgVwDkhoHoc,2402
+funboost/__init__.py,sha256=YKM0VVSXRcZJnQbuqkIjS3PnLJxxIjw1-1JjI13Nn3A,2401
 funboost/__init__old.py,sha256=cSzw-ZQqtAAp5_-7eONXQT5fwz_JbZlRjDQPASDLUHk,20378
 funboost/constant.py,sha256=tSdHQ8nrZH63jOKKZFtOfTo2melCsiMrk-O1lFcsIKA,6489
-funboost/funboost_config_deafult.py,sha256=xpmiZBCVylJe4pC4fG2J-LZZ0c0QJsYXOM1YxQMcMtw,7399
+funboost/funboost_config_deafult.py,sha256=mh9o91CgMC26glIWkw7489GxmJ7bibi4_oBMnv3SCNU,7430
 funboost/set_frame_config.py,sha256=hz_38C-IXEulYpHQdr1fhsMcdEDCHIsF2la8MkHiIjA,9149
-funboost/assist/celery_helper.py,sha256=YvKP21xUzgazZHeFGq4FTgtd0A1g3BGNWzKLQ3gNygc,4186
+funboost/assist/celery_helper.py,sha256=ZJ8jNSC-D8fE6pjxMVGAAA4j9i0gA1kVH14_BbTkXaQ,4569
 funboost/assist/dramatiq_helper.py,sha256=lRNouO8MyCB_Qj2ppYG4FbMpf-2Aok8QhtGZLH1zWkg,2089
 funboost/assist/huey_helper.py,sha256=VEzMdQDVJJ-ujcOXKw7chrTgvieLz4si3hrjt8gIK38,1760
 funboost/assist/rq_helper.py,sha256=-tUZ00FzkczwBAkbbISPHF-8J0K7HLSZsue39WiF-cM,1509
 funboost/assist/rq_windows_worker.py,sha256=jQlGmU0FWPVoKVP8cyuwTuAca9VfSd75F5Qw_hR04y0,4831
 funboost/beggar_version_implementation/beggar_redis_consumer.py,sha256=aiucCkj7-GWbLMIWHhevdQrAsxzyc55AL69fue8esYs,3930
 funboost/concurrent_pool/__init__.py,sha256=dGgxgzMSwcXWMexwAnojsML7EMjHAAsmAofNgrxtl2w,759
 funboost/concurrent_pool/async_helper.py,sha256=iyb0Jcjyx-vkUGC_saSUWqN657kcR5K7B-L_SB6cDCE,3256
@@ -22,16 +22,16 @@
 funboost/concurrent_pool/custom_threadpool_executor000.py,sha256=jJLXy3h-bELap6nZA6yLtdozzTWcvCtZ7IY6MTqLEAM,9317
 funboost/concurrent_pool/single_thread_executor.py,sha256=NDWOegh8Nxpb-Bp-lUlj-DONWvepSmA9qepL1yNgdQI,373
 funboost/concurrent_pool/backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
-funboost/consumers/base_consumer.py,sha256=2wZW7m4i63xf9zfXvsGIp26khTAjMod9-K9828LvbC8,85044
-funboost/consumers/celery_consumer.py,sha256=6CqorZH5pbxIjVwn5gNzcxSbos5YWT8eYqxYyYjgUcY,7574
+funboost/consumers/base_consumer.py,sha256=8goq0tx2db0ErfMeuKuNe62K5SOI-4Io58_7-xs2-X8,86846
+funboost/consumers/celery_consumer.py,sha256=l0UQbO_KmvhCLtMtUgoHxHtEqyBCIABykyVKj04lZPM,8815
 funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
 funboost/consumers/confirm_mixin.py,sha256=oVBQ1RayIBFOzGNTJ69HdBR_kLd46xd0VfCOKfqDpLA,6033
 funboost/consumers/dramatiq_consumer.py,sha256=kiHM1wpSZykYDomtSGZ2PlMInCDn_8GOGEHqHUD9m0o,2144
 funboost/consumers/http_consumer.py,sha256=3HF8tsH90fUPX3iOmVid_nqW_7hZCFaL7feOkuAM36U,2025
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
 funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
 funboost/consumers/huey_consumer.py,sha256=_Z2lpfAzvs1HqkSouncN7eH1VfyQJPYNZNgv1FbZj-U,1856
@@ -43,22 +43,22 @@
 funboost/consumers/mqtt_consumer.py,sha256=StlfPUeQ6o0HiZBpt7TlC_r2DjzPHBZBF2xLSxQW13A,2228
 funboost/consumers/nameko_consumer.py,sha256=IVwUxBixUx2m3F_q8Xn-UsnJWXayMpnOIZjICCd6mcU,2183
 funboost/consumers/nats_consumer.py,sha256=lIYLKvMHNReHnNqGtBA4wot4Ncaobtk60zVHFgm-9Zc,1076
 funboost/consumers/nsq_consumer.py,sha256=PaMRsP8oeRg0H_tq4FL7YhNUdOWAqJkjrwZWoYPNkqU,1461
 funboost/consumers/peewee_conusmer.py,sha256=fbspeWbv6F3EsIIBAjkM_FNh2vMyrDsydju23WAVHvE,1238
 funboost/consumers/persist_queue_consumer.py,sha256=8HzRcMFE6OKiF_CL3atC42Ien_yf5daG3LU38YBKWi0,1005
 funboost/consumers/pulsar_consumer.py,sha256=2DuklBV5dSY-_gW2EpRWz8QSy-VjZclj0gJUvLTyJHA,2414
-funboost/consumers/rabbitmq_amqpstorm_consumer.py,sha256=Qg1Uv4Tk6Tbu9szys6P4U_5BpsOgZuO_kdiR6lb1MlQ,2048
+funboost/consumers/rabbitmq_amqpstorm_consumer.py,sha256=JJnSvewyWJDjAZmBi23r9PYUkt01knHfpRFjpmasjVw,2049
 funboost/consumers/rabbitmq_pika_consumer.py,sha256=9L7CA2wYT-RNpaVfLKrFk6UJtONEIlfuDZYCjxHDOtc,5433
 funboost/consumers/rabbitmq_pika_consumerv0.py,sha256=Yr-GJlgtkYB4qx8hKZZRx8PyCGwKAlSvRFKEf-SBXnM,4674
 funboost/consumers/rabbitmq_rabbitpy_consumer.py,sha256=q-DXy2MHgsFfBssVIlqgziFw2jPkxAT4TyeDnlE0zwI,1260
 funboost/consumers/redis_brpoplpush_consumer.py,sha256=rVdlmODLEQ8_k-gXFnaMFK8LaiKu3EiZMG2q5jmG8qk,3031
 funboost/consumers/redis_consumer.py,sha256=f9nASEQUR3VHk5JH5Plf3RqKXmxogfrshu63RaFnfDM,2829
-funboost/consumers/redis_consumer_ack_able.py,sha256=DlZd76FTPo-AUiTreQd7cSiT5QAM5K9rFItAwLt2n5Y,7545
-funboost/consumers/redis_consumer_priority.py,sha256=avxU89EZuGk-wQeWEpASBU7ustxAHp3KzQcq34wb2Fg,4282
+funboost/consumers/redis_consumer_ack_able.py,sha256=7bdG2282POZ_nbtMK2aAgYi43jNNXbw56uG0eUIII7M,7545
+funboost/consumers/redis_consumer_priority.py,sha256=2BnNvsbNPZCRHdRxrnh1C3mJlqTgb1ql7xRn4-cHULU,5827
 funboost/consumers/redis_consumer_simple.py,sha256=9D3uvLw_9WOmLmwys1K39DK3gj1ex_q6NXadXwyGwrs,922
 funboost/consumers/redis_filter.py,sha256=TVyT2i9JhmhsJFyQZDx98phTiwBccNTl9fcErEDGXTM,7135
 funboost/consumers/redis_pubsub_consumer.py,sha256=eSy5QBMPaouiQbeGQ3ZaLVpU1BF8g3B_4CAJHFqhmmI,1206
 funboost/consumers/redis_stream_consumer.py,sha256=hPUMBoixd7F0Y9U4A8xC6QyOdM4EJAbXsgocHkRCarQ,6497
 funboost/consumers/rocketmq_consumer.py,sha256=sqJwxNFOz7c-4Dbk5Rgj_iJqDVwRVCGsw_tMTArGc2o,1653
 funboost/consumers/rq_consumer.py,sha256=JX84k6Jiv4pBiQMmnhdJ7s7Qz4ub5TWS4T7qTF-WdlM,876
 funboost/consumers/sqlachemy_consumer.py,sha256=-pY9pvAVUCw_T-1bRKRT37vNGjvv6BK9h-I5kfelpVk,1309
@@ -78,14 +78,15 @@
 funboost/core/function_result_status_saver.py,sha256=tNYRvUfb2T59mda9fLWDftbPbLvyKQg7Sph6BTBy_J4,8886
 funboost/core/get_booster.py,sha256=YlImXa5yjvuON_9JOa2yAlPw0tHj7RET5jBjmbj1gcM,1169
 funboost/core/global_boosters.py,sha256=CDrnKhxEEb-GxTL7JhrDTD1tyhLj7ciAtO1Cy2iyi1Q,340
 funboost/core/helper_funs.py,sha256=SKSMKytJTOFQJsuMKWJ-_mQg6e_Bgpq1ANDzjjBAcio,1192
 funboost/core/kill_remote_task.py,sha256=Rj4nrz13CKka8he1T8-k6CYN_yjvcaYZaZ7yurKcKzo,8159
 funboost/core/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
 funboost/core/muliti_process_enhance.py,sha256=zNodv3Ww5yCmwO6xCh7k8HntFHjIYYJ9EPaGinvPV9Q,3814
+funboost/core/show_funboost_flag.py,sha256=EouUN_ioNXWaguA9qKQJKw1xYJqa1aLNxtd9SvL6g8A,5725
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
 funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=Ig1Kze8keS04_vXMNenZSDxibBSjxVrcMkDHviPsxnQ,8976
 funboost/factories/consumer_factory.py,sha256=KFvYkx1a7egtSiTLuVsoRMKLUAotx-QJX1jAI8Xzo3s,946
 funboost/factories/publisher_factotry.py,sha256=Vz66GrCxMt7GV5iqyIXSzZcC_eHF8fj-2kYduzbTTpg,2281
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
 funboost/function_result_web/functions.py,sha256=OIPMxc4jv51qnhBxFGfTZnpMx5p4lQflPoTviDTbJUc,7345
 funboost/function_result_web/static/assets/css/custom.css,sha256=3brvjy2aBOTIXcTUK4NV6dX5wFRqx6K2aLu_jQn63jM,7674
@@ -98,16 +99,16 @@
 funboost/function_result_web/static/images/password.png,sha256=0jRivuQAhWKtkS73p8f_KiLy3D39_flqVTrpFKJPNqk,546
 funboost/function_result_web/static/images/tick.png,sha256=S9dZYN4HQzw7JsWPw3ut1dQp4OTJ_Uh2Qp2KUDF1Jv8,2912
 funboost/function_result_web/static/images/user.png,sha256=HxLjNc83WZzZEscZRdmVhGKlPXNdp_EKmmYxafuyb3g,622
 funboost/function_result_web/static/js/jquery-1.11.0.min.js,sha256=ryQZ3RXgnqkTz-lNEw-YcEhnMuV3ZODwLqOEbyBBRu4,96383
 funboost/function_result_web/templates/index.html,sha256=dWe-JFQhsDpoNjSsBF4P6SJWp_KvHX8EP_yECS5r7_o,19501
 funboost/function_result_web/templates/login.html,sha256=q37dj7O0LeyiV38Zd5P1Qn_qmhjdFomuYTRY1Yk48Bo,2007
 funboost/publishers/__init__.py,sha256=xqBHlvsJQVPfbdvP84G0LHmVB7-pFBS7vDnX1Uo9pVY,131
-funboost/publishers/base_publisher.py,sha256=CU0xjCpt1tsQRcy6Orhuxd8bwsmIJ80wmMZw0JDHevY,15860
-funboost/publishers/celery_publisher.py,sha256=XCR-xvkHEQhbJSluuhrlMPv-V4RTlpA9Ot10mfe4a3E,3081
+funboost/publishers/base_publisher.py,sha256=uuchEFgHMUlY2fBtGwZFLAzeKiWa7_34UTocGADTt2c,15863
+funboost/publishers/celery_publisher.py,sha256=ELT-JR8RtmmCpsxYqVTuuFeKMFZMuK9ROKXWHkGVEjE,2334
 funboost/publishers/celery_publisher000.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
 funboost/publishers/confluent_kafka_publisher.py,sha256=cpbyWvZ0T_kM62LWeBKRUuEuMkJAKOof97UUMSz6-Dk,3541
 funboost/publishers/dramatiq_publisher.py,sha256=RoZzfvkS5H-XXcmHGBomuvkQRQBlVyiaCdWpgy0LL9o,1410
 funboost/publishers/http_publisher.py,sha256=pS3z_AVqH6h4PAgqB7usihvzLJP5ZzfPKQRMQfHrJHQ,753
 funboost/publishers/httpsqs_publisher.py,sha256=7cf5ijwrbp4smq6ofndrKisruAqG0Wzfo_d_7bnLUk4,2783
 funboost/publishers/huey_publisher.py,sha256=z1CF18YZkQY6lqeoc6tiJkaYsRjRicbhYYeoHSvdD-w,1101
 funboost/publishers/kafka_publisher.py,sha256=cmlJ0mvwq0Ajlth4VQqwnoe6v_bZ4eIz49GgkiJr-ZU,2160
@@ -120,19 +121,20 @@
 funboost/publishers/nsq_publisher.py,sha256=Go4UjLd_Vt4JuVtfkmCuuXrmxUXv1y6NaBQJX6s1XUo,1302
 funboost/publishers/peewee_publisher.py,sha256=RsYAqBKf_ZLxkGJeZPWExzG4cpUac7weCeNhcSQ9hZc,1095
 funboost/publishers/persist_queue_publisher.py,sha256=x6qRiR3Ln-jX9KPC5GvBzUzAlmZ0HDjU1KTnILXVJrw,2540
 funboost/publishers/pulsar_publisher.py,sha256=3BqDtywExvTIw1KZWG4kT1uz029uw2YkntLggZ-Ao6A,1238
 funboost/publishers/rabbitmq_amqpstorm_publisher.py,sha256=C32sQZpjv1iJtFDD6g_q0wI7Arw9i0RDsRVVOBRKzi4,3137
 funboost/publishers/rabbitmq_pika_publisher.py,sha256=jZZw3DUiZ4VqJ6FqZGdv7qo3F_ltzHuKsy_5-j4jkCs,2343
 funboost/publishers/rabbitmq_rabbitpy_publisher.py,sha256=GGXPKxE6-mAjqMIKqwvR9d7L-zuJQcQoU9uRsQLNGas,1953
-funboost/publishers/redis_publisher.py,sha256=mUHxfdHYrUn_Dw59NifN-mFsnj53hOhZDoEFlWs-W5M,3982
+funboost/publishers/redis_publisher.py,sha256=FUxvvYvf73J2Im33MRJd-5dmjnccjAFHaTMd4rLvdNM,3358
 funboost/publishers/redis_publisher_lpush.py,sha256=xEWuCTtbDcKFLTxGrECrbIVapFfUwqX2-GHenMClu-Q,278
-funboost/publishers/redis_publisher_priority.py,sha256=zGhSAvpFVBXfAmfGQdWL9cixdpLhLQ6yR3XvBLnbdF4,2104
-funboost/publishers/redis_publisher_simple.py,sha256=hLVWiDjy9ObGTmv7Vtrz21d18Fxkb52IfO5ZzaXjzMQ,872
-funboost/publishers/redis_pubsub_publisher.py,sha256=_6s7sbcGOSXxN2ZkBSDk9ILskmbj9cZTQyYHLQTYOuI,721
+funboost/publishers/redis_publisher_priority.py,sha256=YJCIMdiY0Sdttc7Xv85V-2P1R7ZoX5hqWz7waoibioQ,1972
+funboost/publishers/redis_publisher_simple.py,sha256=fzEurzFQxrTO6PlCONz4m1jQljwuN66spbj4tIJ3Y6c,740
+funboost/publishers/redis_pubsub_publisher.py,sha256=BxVn31I-Rt6gHFSTqntpsajmsl0ZftgMJMtiZd1LMyA,723
+funboost/publishers/redis_queue_flush.py,sha256=d-AgJiCuX25mOwP2gMorGbXCaLuFpqWO4jAJXJDBfk0,732
 funboost/publishers/redis_stream_publisher.py,sha256=DLxFcTlze0IdYFoaRmTcY8GCOaRwbj4aBNbylkt9gRA,2037
 funboost/publishers/rocketmq_publisher.py,sha256=vY82WgutDPsS9px6rukU1d3AexmsT_tqSS2dmX-Pw-c,2343
 funboost/publishers/rq_publisher.py,sha256=ANHrYnPTEj7KF_D_ov2L7PAT9swl82kjDazFqN1ULBY,893
 funboost/publishers/sqla_queue_publisher.py,sha256=yUbge08K311-jWlFyOUw6g7-Z-flbxEeWCeCTGnJcic,1215
 funboost/publishers/tcp_publisher.py,sha256=qMecOpgVqwTy-VYyevv4mCR6H5bQhCirRbJmcJIaFCE,1335
 funboost/publishers/txt_file_publisher.py,sha256=twTrqRAYnaNmFkXn0nr1xGBjeHCPJStt83voLX3vPao,1380
 funboost/publishers/udp_publisher.py,sha256=TOiKrhmCMjx4teqIgdUwRic0lxyK2cupinafsz--wzY,1194
@@ -154,15 +156,15 @@
 funboost/utils/kill_thread.py,sha256=PPw1WQ1zZmINVgzGByMCj2aevFcHKB7KyrN9iyeJdGE,3412
 funboost/utils/mongo_util.py,sha256=9oAWgYMBdP1rqY2KySW_VEuEBq8Xdsf5lgml4484OzM,2984
 funboost/utils/monkey_color_log.py,sha256=QChhQMTB6phZ2eBaPq-9tFZF1n7pWeJgmJPIB_ugkvs,7367
 funboost/utils/monkey_patches.py,sha256=Q0_jKxOfFrSgrIDSuSZFrgNh6w_LRGaKAITghrIpEwI,2882
 funboost/utils/mqtt_util.py,sha256=BfCmyYwI-B8VL9499_IuYlJDCbv6ZhwyWThMf8dANOU,3199
 funboost/utils/paramiko_util.py,sha256=pu67zkgptqNSV9m2Lznezb3zF1AFYvkWJp_6DVKFSPU,4901
 funboost/utils/rabbitmq_factory.py,sha256=NPzTwG-INZG9aJgkzp-QVk3TgV0rjiuTVT5lmRT77zg,2963
-funboost/utils/redis_manager.py,sha256=2Hg9UT-X6nS5TkZ-YrTRxRK-WPHZaLOsuvTxYuD1cCc,4628
+funboost/utils/redis_manager.py,sha256=0mkPxBFE4pBv22Zi9O0YN-txvlRHdpjpl0maW5M0QvM,4649
 funboost/utils/resource_monitoring.py,sha256=vf1htYa3a4wlMfQqksvIINMw8laiXwG5N8NXU2Zm3qQ,5532
 funboost/utils/restart_python.py,sha256=bFbV0_24ajL8hBwVRLxWe9v9kTwiX1fGLhXRroNnmgQ,1418
 funboost/utils/show_funboost_flag.py,sha256=YPXtykSkRBJZ4ulOIAXiTAfpOmo9IsjePz9G9AEE6cg,2985
 funboost/utils/simple_data_class.py,sha256=HgFyyrw2mDuMX6l-re8W6q-6HXwhg2MalpIbP9JKW70,1204
 funboost/utils/time_util.py,sha256=Y-P6KowTNgGwXHzfQd4KnHdfLl8vAOqhg626MCKDvtA,5407
 funboost/utils/un_strict_json_dumps.py,sha256=uh2mXNRCq5dJcqMhb9CkfvehfEGYZAgI6RY1oLcYX_M,408
 funboost/utils/dependency_packages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -209,12 +211,12 @@
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
 funboost/utils/times/__init__.py,sha256=z-KQTxXapfu2ScJxISGe7QGffASuyJYL6JGsLXxD6O0,2332
 funboost/utils/times/version.py,sha256=JiZLGTB-HYyBOV4xS0rnx2K2OqVMTebUj30sZRbrleE,16
-funboost-23.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-23.5.dist-info/METADATA,sha256=vP7DG7GGXW7ktzISGDk4Vsgo-GkvlLpCatSrtc9z9uE,26615
-funboost-23.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-funboost-23.5.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-23.5.dist-info/RECORD,,
+funboost-23.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-23.6.dist-info/METADATA,sha256=TZ38IJIfUBK6FglySO_5TCIwxPA5wm8EsMkWNh5B1cE,26928
+funboost-23.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+funboost-23.6.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-23.6.dist-info/RECORD,,
```

