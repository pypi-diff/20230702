# Comparing `tmp/lacdkeras-1.0.0.2.tar.gz` & `tmp/lacdkeras-1.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacdkeras-1.0.0.2.tar", last modified: Fri Feb 11 13:30:20 2022, max compression
+gzip compressed data, was "lacdkeras-1.0.0.3.tar", last modified: Sun Jul  2 14:03:56 2023, max compression
```

## Comparing `lacdkeras-1.0.0.2.tar` & `lacdkeras-1.0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-02-11 13:30:20.621731 lacdkeras-1.0.0.2/
--rw-rw-rw-   0        0        0     1091 2022-02-11 13:23:15.000000 lacdkeras-1.0.0.2/LICENSE
--rw-rw-rw-   0        0        0      232 2022-02-11 13:30:20.621731 lacdkeras-1.0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-02-11 13:30:20.617730 lacdkeras-1.0.0.2/lacdkeras/
--rw-rw-rw-   0        0        0       29 2019-07-04 18:32:50.000000 lacdkeras-1.0.0.2/lacdkeras/__init__.py
--rw-rw-rw-   0        0        0    15392 2022-02-11 12:35:34.000000 lacdkeras-1.0.0.2/lacdkeras/keras.py
-drwxrwxrwx   0        0        0        0 2022-02-11 13:30:20.620730 lacdkeras-1.0.0.2/lacdkeras.egg-info/
--rw-rw-rw-   0        0        0      232 2022-02-11 13:30:20.000000 lacdkeras-1.0.0.2/lacdkeras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2022-02-11 13:30:20.000000 lacdkeras-1.0.0.2/lacdkeras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-11 13:30:20.000000 lacdkeras-1.0.0.2/lacdkeras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-02-11 13:30:20.000000 lacdkeras-1.0.0.2/lacdkeras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-11 13:20:09.000000 lacdkeras-1.0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-02-11 13:30:20.621731 lacdkeras-1.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      284 2022-02-11 13:29:48.000000 lacdkeras-1.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:03:56.931841 lacdkeras-1.0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-02 12:35:18.000000 lacdkeras-1.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      200 2023-07-02 14:03:56.931841 lacdkeras-1.0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-02 14:03:56.908730 lacdkeras-1.0.0.3/lacdkeras/
+-rw-rw-rw-   0        0        0       29 2023-07-02 12:35:18.000000 lacdkeras-1.0.0.3/lacdkeras/__init__.py
+-rw-rw-rw-   0        0        0    12977 2023-07-02 13:49:40.000000 lacdkeras-1.0.0.3/lacdkeras/keras.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:03:56.930862 lacdkeras-1.0.0.3/lacdkeras.egg-info/
+-rw-rw-rw-   0        0        0      200 2023-07-02 14:03:56.000000 lacdkeras-1.0.0.3/lacdkeras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-07-02 14:03:56.000000 lacdkeras-1.0.0.3/lacdkeras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 14:03:56.000000 lacdkeras-1.0.0.3/lacdkeras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 14:03:56.000000 lacdkeras-1.0.0.3/lacdkeras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-07-02 12:35:18.000000 lacdkeras-1.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 14:03:56.942012 lacdkeras-1.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      284 2023-07-02 13:50:25.000000 lacdkeras-1.0.0.3/setup.py
```

### Comparing `lacdkeras-1.0.0.2/LICENSE` & `lacdkeras-1.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lacdkeras-1.0.0.2/lacdkeras/keras.py` & `lacdkeras-1.0.0.3/lacdkeras/keras.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,34 +3,23 @@
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import Dense
 from tensorflow.keras.utils import to_categorical
 from tensorflow.keras.layers import Dense, Dropout, Activation, Flatten
 from tensorflow.keras.optimizers import SGD
 from sklearn.model_selection import train_test_split
 
-#這邊的資料是用來畫圖的,可以忽略!
+title = []
+
 class lacdkeras_model():
 
     def __init__(self):
         self.activation = 'relu'
         self.epoch = 20
         self.batch_size = 128
-        print('--函式說明--')
-        print('函式1: set_activation(變數名稱)\t\t\t=>用於設定活化函數為何\n')
-        print('函式2: set_epoch(代數)\t\t\t\t=>用於設定要訓練幾代\n')
-        print('函式3: set_train_data(變項資料,分類為何)\t=>用於設定要訓練的資料為何\n')
-        print('函式4: set_test_data(變項資料,分類為何)\t\t=>用於設定批量大小為何\n')
-        print('函式5: set_neuron_level(神經元個數的陣列)\t=>用於設定隱藏層數量及層數為何\n')
-        print('函式6: predict_data()\t\t\t\t=>用於預測新的數據,單筆資料可以放入List(),多筆資料可以使用雙層List\n')
-        print('------單筆資料可以放入List(),多筆資料可以使用雙層List')
-        print('------多筆資料可以使用雙層List\n')
-        print('函式7: get_acc()\t\t\t\t=>用於得到此模型的正確率,回傳(訓練正確率,測試正確率)\n')
-        print('函式8: run_model\t\t\t\t=>開始跑神經網絡\n')
-        print('函式9: show_history()\t\t\t\t=>用於顯示訓練過程\n')
-        print('-----------')
+        self.help()
 
     def set_activation(self,activation_name):
         activation_names = np.array(['relu','sigmoid','tanh'])
         if activation_name in activation_names:
             self.activation = activation_name
             print('Activation設定為:'+activation_name)
         else:
@@ -117,60 +106,58 @@
             for level_Index in range(1,len(self.neuron_count),1):
                 self.model.add(Dense(units = self.neuron_count[level_Index],activation= self.activation))
 
             self.model.add(Dense(units = self.Output_size,activation='softmax'))
         else:
             print('Linear Regression model')
             self.model.add(Dense(units = self.Output_size,activation= 'softmax',input_dim=self.Input_size))
-        self.model.compile(loss='categorical_crossentropy', optimizer=SGD(lr=0.01, momentum=0.9, nesterov=True), metrics=['accuracy'])
+        self.model.compile(loss='categorical_crossentropy', optimizer=SGD(learning_rate=0.01, momentum=0.9, nesterov=True), metrics=['accuracy'])
         self.model.summary()#顯示目前建立的模型結構
 
-
+        #train_history 為紀錄更新的軌跡圖
         self.train_history = self.model.fit(self.x_train, self.y_train,      #輸入 與 輸出
                   epochs = self.epoch,       #子代數
                   batch_size = self.batch_size,#批量大小 一次參考多少的數據 4=> 00 01 10 11一同參考
                   verbose = 1 ,           #是否顯示訓練過程 1=>是  2=>否
                   validation_data=(self.x_test, self.y_test)) #拿來預測的資料  (此使用與輸入相同的資料!)
-        #train_history 為紀錄更新的軌跡圖
 
         #最後輸出測試資料跟訓練資料的正確率!
         score = self.model.evaluate(self.x_train, self.y_train)
         self.train_acc = score[1]
         print ('\nTrain Acc:', score[1])
         score = self.model.evaluate(self.x_test, self.y_test)
         self.test_acc = score[1]
         print ('\nTest Acc:', score[1])
-        #開始使用修正完的參數做預測，並將"預測"的結果放置在classes裡面
-        classes = (self.model.predict(self.x_test,batch_size=self.batch_size) > 0.5).astype("int32")
     
     def predict_data(self,predict_data):
         if not isinstance(predict_data[0], list):
             test = predict_data
             predict_data = []
             predict_data.append(test)
-
-
-        if len(predict_data[0]) != self.Input_size:
+        
+        for data in predict_data:
+          if len(data) != self.Input_size:
             print('預測的變項數量不一喔!')
             print('需要的變項個數為:'+str(self.Input_size))
-            print('但是輸入的變項個數為:'+str(len(predict_data[0])))
+            print('但是輸入的變項個數為:'+str(len(data)))
             return 
 
         predict_data = np.array(predict_data)
-        classes = (self.model.predict(self.x_test,batch_size=self.batch_size) > 0.5).astype("int32")
-        
+        classes = self.model.predict(predict_data,batch_size=self.batch_size)
+
+        global title
         print('預測類別',end = '')
-        for Input_index in range(0,self.Input_size,1):
-            print('\t變項'+str(Input_index+1),end = '')
+        for var in title:
+            print('\t{:10}'.format(var),end = '')
         print()
 
         for dataindex in range(0,len(predict_data),1):
-            print(str(classes[dataindex])+'\t\t',end = '')
+            print(str(classes[dataindex].argmax(axis=0))+'\t\t',end = '')
             for Input_index in predict_data[dataindex]:
-                print(str(Input_index)+'\t',end = '')
+                print('{:10}\t'.format(str(Input_index)),end = '')
             print()
         print('========')
         print('預測完畢!')
     #用於獲得正確率
     def get_acc(self):
         return self.train_acc,self.test_acc
 
@@ -188,15 +175,15 @@
         plt.plot(self.train_history.history['loss'])
         plt.plot(self.train_history.history['val_loss'])
         plt.ylabel('loss')
         plt.xlabel('Epoch')
         plt.legend(['train_loss', 'test_loss'], loc='upper left')
         plt.show()
 
-    def question(self):
+    def help(self):
         print('--函式說明--')
         print('函式1: set_activation(變數名稱)\t\t\t=>用於設定活化函數為何\n')
         print('函式2: set_epoch(代數)\t\t\t\t=>用於設定要訓練幾代\n')
         print('函式3: set_train_data(變項資料,分類為何)\t=>用於設定要訓練的資料為何\n')
         print('函式4: set_test_data(變項資料,分類為何)\t\t=>用於設定批量大小為何\n')
         print('函式5: set_neuron_level(神經元個數的陣列)\t=>用於設定隱藏層數量及層數為何\n')
         print('函式6: predict_data()\t\t\t\t=>用於預測新的數據,單筆資料可以放入List(),多筆資料可以使用雙層List\n')
@@ -206,42 +193,27 @@
         print('函式8: run_model\t\t\t\t=>開始跑神經網絡\n')
         print('函式9: show_history()\t\t\t\t=>用於顯示訓練過程\n')
         print('-----------')
 
 class lacdkeras_data():
 
     def __init__(self):
-        print('--函式說明--')
-        print('函式1: set_csvdata(檔案名稱)\t\t\t=>用於將資料做前處理，整理成類別跟輸入資料\n')
-        print('----請注意資料格式為----')
-        print('-類別\t變項1\t變項2\t變項3')
-        print('0\t1\t2\t3')
-        print('0\t1\t6\t2')
-        print('1\t5\t4\t4')
-        print('1\t2\t4\t5')
-        print('====================')
-        print('函式2: split_train_test_data()\t\t\t=>用於將資料分割成訓練資料及測試資料\n')
-        print('函式3: show()\t\t\t\t\t=>用於顯示目前所有資料的狀況為何?\n')
-        print('-----------')
-        print('--變數說明--')
-        print('Data_Input   =>所有資料的輸入變項')
-        print('Data_Level   =>所有資料的類別\n')
-        print('x_train      =>訓練資料的輸入變項')
-        print('y_train      =>訓練資料的類別\n')
-        print('x_test       =>測試資料的輸入變項')
-        print('y_test       =>測試資料的類別')
+        self.help()
 
     def set_csvdata(self,csv_name):
         self.csv_name = csv_name
         fp = open(self.csv_name,'r',encoding="utf-8")
         All_Lines = fp.readlines()
         Data_Input = []
         Data_Level = []
 
         #第一行為資料集,不放
+        global title
+        title = All_Lines[0].split(',')
+        del title[0]
         for Line_index in range(1,len(All_Lines),1):
             Line_sentence = All_Lines[Line_index].replace('\t',',')
 
             while(',,' in Line_sentence):
                 Line_sentence = Line_sentence.replace(',,',',')
 
             Data_Split = Line_sentence.replace('\n','').split(',')
@@ -292,36 +264,36 @@
         print('類別:拿來預測後最後的結果為何(EX:是否會下雨)')
         print('(1):要拿來預測的變項之一(EX:溫度)')
         print('(2):要拿來預測的變項之一(EX:濕度)')
         print('(3):要拿來預測的變項之一(EX:雲量)')
         print('PS.僅會顯示前10項資訊')
         print('\n\n============================================')
         print('類別\t',end = '')
-        for index in range(0,len(self.Data_Input[0]),1):
-            print('('+str(index+1)+')\t',end = '')
+        for var in title:
+            print('{:>10}\t'.format(var),end = '')
         print()
 
-        if(len(self.Data_Level)>10):
-            for Level_Index in range(0,10,1):
-                print(self.Data_Level[Level_Index]+'\t',end = '')
-                for Input_Index in range(0,len(self.Data_Input[Level_Index]),1):
-                    print(str(self.Data_Input[Level_Index][Input_Index])+'\t',end = '')
-                print()
-        else:
-            for Level_Index in range(0,len(self.Data_Level),1):
-                print(self.Data_Level[Level_Index]+'\t',end = '')
-                for Input_Index in range(0,len(self.Data_Input[Level_Index]),1):
-                    print(self.Data_Input[Level_Index][Input_Index]+'\t',end = '')
-                print()
+        for Level_Index in range(0,min(len(self.Data_Level),10),1):
+          print('{:10}\t'.format(self.Data_Level[Level_Index]),end = '')
+          for Input_Index in range(0,len(self.Data_Input[Level_Index]),1):
+              print('{:10}\t'.format(self.Data_Input[Level_Index][Input_Index]),end = '')
+          print()
 
-    def question(self):
+    def help(self):
         print('--函式說明--')
         print('函式1: set_csvdata(檔案名稱)\t\t\t=>用於將資料做前處理，整理成類別跟輸入資料\n')
+        print('----請注意資料格式為----')
+        print('-類別\t變項1\t變項2\t變項3')
+        print('0\t1\t2\t3')
+        print('0\t1\t6\t2')
+        print('1\t5\t4\t4')
+        print('1\t2\t4\t5')
+        print('====================')
         print('函式2: split_train_test_data()\t\t\t=>用於將資料分割成訓練資料及測試資料\n')
-        print('函式3: show()\t\t\t=>用於顯示目前所有資料的狀況為何?\n')
+        print('函式3: show()\t\t\t\t\t=>用於顯示目前所有資料的狀況為何?\n')
         print('-----------')
         print('--變數說明--')
         print('Data_Input   =>所有資料的輸入變項')
         print('Data_Level   =>所有資料的類別\n')
         print('x_train      =>訓練資料的輸入變項')
         print('y_train      =>訓練資料的類別\n')
         print('x_test       =>測試資料的輸入變項')
```

