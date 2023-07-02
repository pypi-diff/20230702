# Comparing `tmp/vios-1.0.3-py3-none-any.whl.zip` & `tmp/vios-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 33360 bytes, number of entries: 23
+Zip file size: 33387 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat      781 b- defN 23-Jun-26 13:01 vios/__init__.py
 -rw-rw-rw-  2.0 fat     4936 b- defN 23-Jun-26 13:00 vios/collection/__init__.py
 -rw-rw-rw-  2.0 fat     3515 b- defN 23-Jun-26 11:28 vios/collection/support.py
 -rw-rw-rw-  2.0 fat    11254 b- defN 23-Jun-19 15:11 vios/collection/tasks.py
 -rw-rw-rw-  2.0 fat    10198 b- defN 23-Jun-28 07:10 vios/collection/uapi.py
 -rw-rw-rw-  2.0 fat     4756 b- defN 23-Jun-19 15:11 vios/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat     2962 b- defN 23-Jun-19 15:11 vios/driver/__init__.py
 -rw-rw-rw-  2.0 fat      209 b- defN 23-Jun-26 11:28 vios/driver/common/__init__.py
 -rw-rw-rw-  2.0 fat     4192 b- defN 23-Jun-28 07:10 vios/driver/common/basedriver.py
 -rw-rw-rw-  2.0 fat     4666 b- defN 23-Jun-19 15:11 vios/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5546 b- defN 23-Jun-19 15:11 vios/driver/common/visadriver.py
 -rw-rw-rw-  2.0 fat      784 b- defN 23-Jun-30 06:18 vios/envelope/__init__.py
--rw-rw-rw-  2.0 fat    13293 b- defN 23-Jun-30 05:21 vios/envelope/assembler.py
+-rw-rw-rw-  2.0 fat    13418 b- defN 23-Jul-01 14:52 vios/envelope/assembler.py
 -rw-rw-rw-  2.0 fat    10541 b- defN 23-Jun-26 11:28 vios/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-Jun-19 15:11 vios/envelope/device.py
 -rw-rw-rw-  2.0 fat     1719 b- defN 23-Jun-26 11:28 vios/envelope/processor.py
 -rw-rw-rw-  2.0 fat     2980 b- defN 23-Jun-26 12:50 vios/envelope/rule.py
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-26 11:28 vios/tools/__init__.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1000 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1857 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/RECORD
-23 files, 87944 bytes uncompressed, 30380 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-02 09:20 vios-1.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1000 b- defN 23-Jul-02 09:20 vios-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-02 09:20 vios-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-02 09:20 vios-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1857 b- defN 23-Jul-02 09:20 vios-1.0.4.dist-info/RECORD
+23 files, 88069 bytes uncompressed, 30407 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: vios/envelope/rule.py
 Comment: 
 
 Filename: vios/tools/__init__.py
 Comment: 
 
-Filename: vios-1.0.3.dist-info/LICENSE
+Filename: vios-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: vios-1.0.3.dist-info/METADATA
+Filename: vios-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: vios-1.0.3.dist-info/WHEEL
+Filename: vios-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: vios-1.0.3.dist-info/top_level.txt
+Filename: vios-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-1.0.3.dist-info/RECORD
+Filename: vios-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vios/envelope/assembler.py

```diff
@@ -27,14 +27,17 @@
 
     def reset(self, snapshot):
         if isinstance(snapshot, dict):
             self._QuarkLocalConfig__driver = DictDriver(deepcopy(snapshot))
         else:
             self._QuarkLocalConfig__driver = snapshot
 
+    def snapshot(self):
+        return self._QuarkLocalConfig__driver 
+
 
 cfg = CompilerContext({})  # cfg (QuarkLocalConfig): 线路编绎所需配置
 
 
 def initialize(snapshot, **kwds):
     """初始化编译上下文环境，即每个线路对应的当前的cfg表
 
@@ -144,14 +147,15 @@
                 'arch': 'baqis'}}
 
     """
     kwds['signal'] = _form_signal(kwds.get('signal'))
     kwds['lib'] = stdlib
 
     ctx = kwds.get('ctx', cfg)
+    ctx.snapshot().cache = kwds.get('cache', {})
 
     # print('Compiling', circuit)
     code = _compile(circuit, cfg=ctx, **kwds)
     cmds, datamap = assembly_code(code)
     # print('Compiled', cmds)
     instruction = {}
     for cmd in cmds:
```

## Comparing `vios-1.0.3.dist-info/LICENSE` & `vios-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-1.0.3.dist-info/METADATA` & `vios-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 1.0.3
+Version: 1.0.4
 Summary: runtime requirements for systemq
 Author-email: YL <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-1.0.3.dist-info/RECORD` & `vios-1.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 vios/driver/VirtualDevice.py,sha256=sf87LAcRvJIVZW-OyP8Hw-CWu7isonbr2-TjFGZHYSk,4756
 vios/driver/__init__.py,sha256=rvTlhtDHO_l1rHNsgb3PA9LnEirl4TIm0bvlgRseRnY,2962
 vios/driver/common/__init__.py,sha256=rwnAg6V2hY1vinIHlvGwKTXn34SRQHX8bnIleycTM6k,209
 vios/driver/common/basedriver.py,sha256=jQ3svU_t1v0Zt8lRX8ij8MhwilmIwziozwuTFeRxRnE,4192
 vios/driver/common/quantity.py,sha256=70feNhld2lF04KHQ3zWDliS_cmD1q97Yi0oFqlwYijs,4666
 vios/driver/common/visadriver.py,sha256=WY6TqGmow_K5ePAYIYkG12IxjHfAczuxYTvPk4VmVG4,5546
 vios/envelope/__init__.py,sha256=97kXED9oaUd56J2OoVCTQpctkQZDcAZWxpEQakTxCRM,784
-vios/envelope/assembler.py,sha256=9UcTDB-hL3EA8B0QUA7luD22gCipzJrn-VRRu7VA9ZM,13293
+vios/envelope/assembler.py,sha256=8uXlKJZLZCsaeWlMVXIXCUH1K2FPiZBTrs8XqGf_Sd8,13418
 vios/envelope/calculator.py,sha256=eE7730YFzArrukuDh0dI0JabG2PiEz3eo3N4Czqgk88,10541
 vios/envelope/device.py,sha256=rQeLe_Y9MTwLZfJsSK9MhvZxdOnrtJNcOZriS6Rm1Io,1047
 vios/envelope/processor.py,sha256=4py3AwLurBTrhXXJCvdfHrMeKGzOFl-gICQTNjpoyQM,1719
 vios/envelope/rule.py,sha256=ANiUVCtozVP6B6m8En55VLqOHWdeMkuA7KqiAiFyAnQ,2980
 vios/tools/__init__.py,sha256=vq-1N9Zjm_ZYcD9_lwX9fKlcMT9Rx7Kd3BDRqmKhMT0,522
-vios-1.0.3.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
-vios-1.0.3.dist-info/METADATA,sha256=QGh6SLu3E1TVTsVMXl7euSmxhUZrikrLMqTIJavIm20,1000
-vios-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vios-1.0.3.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
-vios-1.0.3.dist-info/RECORD,,
+vios-1.0.4.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
+vios-1.0.4.dist-info/METADATA,sha256=aejBy3jdCCVzzdNMmwcWWwuJYdROuUp13NdnYEASlWE,1000
+vios-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vios-1.0.4.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
+vios-1.0.4.dist-info/RECORD,,
```

