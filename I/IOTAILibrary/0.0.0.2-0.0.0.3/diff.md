# Comparing `tmp/IOTAILibrary-0.0.0.2-py3-none-any.whl.zip` & `tmp/IOTAILibrary-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6597 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     9262 b- defN 23-May-29 17:21 IOTData/Processor.py
+Zip file size: 6669 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     9262 b- defN 23-Jul-02 17:48 IOTData/Processor.py
 -rw-rw-rw-  2.0 fat     1391 b- defN 22-Nov-29 15:30 IOTData/Structure.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-10 16:28 IOTData/__init__.py
--rw-rw-rw-  2.0 fat     7630 b- defN 23-May-29 17:21 IOTModel/Generator.py
+-rw-rw-rw-  2.0 fat     7980 b- defN 23-Jul-02 17:39 IOTModel/Generator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-10 16:28 IOTModel/__init__.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      704 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/RECORD
-9 files, 19566 bytes uncompressed, 5379 bytes compressed:  72.5%
+-rw-rw-rw-  2.0 fat      470 b- defN 23-Jul-02 17:49 IOTAILibrary-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-02 17:49 IOTAILibrary-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-02 17:49 IOTAILibrary-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      704 b- defN 23-Jul-02 17:49 IOTAILibrary-0.0.0.3.dist-info/RECORD
+9 files, 19916 bytes uncompressed, 5451 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: IOTModel/Generator.py
 Comment: 
 
 Filename: IOTModel/__init__.py
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.2.dist-info/METADATA
+Filename: IOTAILibrary-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.2.dist-info/WHEEL
+Filename: IOTAILibrary-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.2.dist-info/top_level.txt
+Filename: IOTAILibrary-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.2.dist-info/RECORD
+Filename: IOTAILibrary-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## IOTModel/Generator.py

```diff
@@ -67,20 +67,31 @@
         print ('\nTest Acc:', score[1])
         print('End training model')
         self._show_model_train_history()
 
     def _predict_data(self, input_data):
         if self._model != "":
             convert_test_x, convert_test_y = self._get_data_format(input_data)
-            test_predict_result = self._model.predict_classes(convert_test_x)
+            test_predict_result = self._model.predict(convert_test_x)
             for index in range(0,len(test_predict_result),1):
-                input_data[index].set_predict_label(test_predict_result[index])
+                input_data[index].set_predict_label(self._probabilityToClass(test_predict_result[index]))
         else:
             print('predict model fail')
 
+    def _probabilityToClass(self, proabilitysList):
+
+        max_index = 0
+        probability = 0
+        for index in range(0, len(proabilitysList),1):
+            if proabilitysList[index] > probability:
+                max_index = index
+                probability = proabilitysList[index]
+
+        return max_index
+
 
     def evaluate(self, evaluate_data):
         print('start evaluating model')
         self._predict_data(evaluate_data)
         print('end evaluating model')
 
     def infer(self):
```

