# Comparing `tmp/xgo-pythonlib-0.2.0.tar.gz` & `tmp/xgo-pythonlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.2.0.tar", last modified: Wed Jun 21 08:00:23 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.2.1.tar", last modified: Sun Jul  2 10:40:47 2023, max compression
```

## Comparing `xgo-pythonlib-0.2.0.tar` & `xgo-pythonlib-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:00:23.455258 xgo-pythonlib-0.2.0/
--rw-rw-rw-   0        0        0     2334 2023-06-21 08:00:23.454259 xgo-pythonlib-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1707 2023-06-21 07:59:24.000000 xgo-pythonlib-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 08:00:23.455258 xgo-pythonlib-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-06-21 07:57:44.000000 xgo-pythonlib-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:00:23.444261 xgo-pythonlib-0.2.0/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2334 2023-06-21 08:00:23.000000 xgo-pythonlib-0.2.0/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-21 08:00:23.000000 xgo-pythonlib-0.2.0/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:00:23.000000 xgo-pythonlib-0.2.0/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-21 08:00:23.000000 xgo-pythonlib-0.2.0/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 08:00:23.445261 xgo-pythonlib-0.2.0/xgoedu/
--rw-rw-rw-   0        0        0    37629 2023-06-21 07:57:29.000000 xgo-pythonlib-0.2.0/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:00:23.447262 xgo-pythonlib-0.2.0/xgolib/
--rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.0/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:00:23.453260 xgo-pythonlib-0.2.0/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.0/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.0/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.0/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.061341 xgo-pythonlib-0.2.1/
+-rw-rw-rw-   0        0        0     2337 2023-07-02 10:40:47.059836 xgo-pythonlib-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1710 2023-07-02 10:39:24.000000 xgo-pythonlib-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 10:40:47.061341 xgo-pythonlib-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-07-02 10:40:40.000000 xgo-pythonlib-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.051523 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2337 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-02 10:40:46.000000 xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.052829 xgo-pythonlib-0.2.1/xgoedu/
+-rw-rw-rw-   0        0        0    46584 2023-07-02 10:39:06.000000 xgo-pythonlib-0.2.1/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.053836 xgo-pythonlib-0.2.1/xgolib/
+-rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.1/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:40:47.058835 xgo-pythonlib-0.2.1/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.1/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.1/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.1/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.2.0/PKG-INFO` & `xgo-pythonlib-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.0
+Version: 0.2.1
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,25 +20,20 @@
 
 XGO2 has built-in motion libraries for controlling the movement and various features of the machine dog, including battery level, firmware version, and servo angle. The motion library enables users to control translation and pose movement, as well as single servo and single-leg movement. The education library facilitates camera, screen, key, microphone, and speaker operations, as well as commonly used AI functions such as gesture recognition, face detection, emotional recognition, and age and gender recognition.  The detailed instructions for use of the library are as follows.
 
 PythonLib included xgolib.py and xgoedu.py
 
 [Luwu Dynamics · WIKI](https://www.yuque.com/luwudynamics)
 
-[PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
-
-
 
 ## Install instructions 
 
-1 Burn the official 0609 img image 
-
-2 Copy all files from the "model" directory to `\home\pi\model`
+1 Burn the latest official image 
 
-3 Run this command:
+2 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
 sudo pip install --upgrade xgo-pythonlib
 ```
 
 ## Examples
@@ -61,14 +56,20 @@
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
 
 ## Change Log
 
+### [0.2.1] - 2023-07-02
+
+#### Added
+
+- Five Methods: SpeechRecognition SpeechSynthesis QRRecognition CircleRecognition ColorRecognitio added.
+
 ### [0.2.0] - 2023-06-21
 
 #### Fixed
 
 - xgoVideo and xgoVideoRecord method can be used.
 
 ### [0.1.9] - 2023-06-20
```

### Comparing `xgo-pythonlib-0.2.0/README.md` & `xgo-pythonlib-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,20 @@
 
 XGO2 has built-in motion libraries for controlling the movement and various features of the machine dog, including battery level, firmware version, and servo angle. The motion library enables users to control translation and pose movement, as well as single servo and single-leg movement. The education library facilitates camera, screen, key, microphone, and speaker operations, as well as commonly used AI functions such as gesture recognition, face detection, emotional recognition, and age and gender recognition.  The detailed instructions for use of the library are as follows.
 
 PythonLib included xgolib.py and xgoedu.py
 
 [Luwu Dynamics · WIKI](https://www.yuque.com/luwudynamics)
 
-[PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
-
-
 
 ## Install instructions 
 
-1 Burn the official 0609 img image 
-
-2 Copy all files from the "model" directory to `\home\pi\model`
+1 Burn the latest official image 
 
-3 Run this command:
+2 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
 sudo pip install --upgrade xgo-pythonlib
 ```
 
 ## Examples
@@ -43,14 +38,20 @@
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
 
 ## Change Log
 
+### [0.2.1] - 2023-07-02
+
+#### Added
+
+- Five Methods: SpeechRecognition SpeechSynthesis QRRecognition CircleRecognition ColorRecognitio added.
+
 ### [0.2.0] - 2023-06-21
 
 #### Fixed
 
 - xgoVideo and xgoVideoRecord method can be used.
 
 ### [0.1.9] - 2023-06-20
```

### Comparing `xgo-pythonlib-0.2.0/setup.py` & `xgo-pythonlib-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.2.0/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.2.1/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.0
+Version: 0.2.1
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,25 +20,20 @@
 
 XGO2 has built-in motion libraries for controlling the movement and various features of the machine dog, including battery level, firmware version, and servo angle. The motion library enables users to control translation and pose movement, as well as single servo and single-leg movement. The education library facilitates camera, screen, key, microphone, and speaker operations, as well as commonly used AI functions such as gesture recognition, face detection, emotional recognition, and age and gender recognition.  The detailed instructions for use of the library are as follows.
 
 PythonLib included xgolib.py and xgoedu.py
 
 [Luwu Dynamics · WIKI](https://www.yuque.com/luwudynamics)
 
-[PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
-
-
 
 ## Install instructions 
 
-1 Burn the official 0609 img image 
-
-2 Copy all files from the "model" directory to `\home\pi\model`
+1 Burn the latest official image 
 
-3 Run this command:
+2 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
 sudo pip install --upgrade xgo-pythonlib
 ```
 
 ## Examples
@@ -61,14 +56,20 @@
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
 
 ## Change Log
 
+### [0.2.1] - 2023-07-02
+
+#### Added
+
+- Five Methods: SpeechRecognition SpeechSynthesis QRRecognition CircleRecognition ColorRecognitio added.
+
 ### [0.2.0] - 2023-06-21
 
 #### Fixed
 
 - xgoVideo and xgoVideoRecord method can be used.
 
 ### [0.1.9] - 2023-06-20
```

### Comparing `xgo-pythonlib-0.2.0/xgoedu/__init__.py` & `xgo-pythonlib-0.2.1/xgoedu/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 '''
 xgo图形化python库  edu库
 '''
 import cv2
 import numpy as np
 import math
-import os,sys,time
+import os,sys,time,json,base64
 import spidev as SPI
 import xgoscreen.LCD_2inch as LCD_2inch
 import RPi.GPIO as GPIO
 from PIL import Image,ImageDraw,ImageFont
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.6'
-__last_modified__ = '2023/6/21'
+__versinon__ = '1.2.7'
+__last_modified__ = '2023/7/2'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -127,14 +127,50 @@
 
     def open_camera(self):
         if self.cap==None:
             self.cap =cv2.VideoCapture(0)
             self.cap.set(3,320)
             self.cap.set(4,240)
 
+    def fetch_token(self):
+        from urllib.request import urlopen
+        from urllib.request import Request
+        from urllib.error import URLError
+        from urllib.parse import urlencode
+        API_KEY = 'Q4ZgU8bfnhA8HQFnNucBO2ut'
+        SECRET_KEY = 'MqFrVgdwoM8ZuGIp0NIFF7qfYti4mjP6'
+        TOKEN_URL = 'http://aip.baidubce.com/oauth/2.0/token'
+        params = {'grant_type': 'client_credentials',
+                'client_id': API_KEY,
+                'client_secret': SECRET_KEY}
+        post_data = urlencode(params)
+        post_data = post_data.encode( 'utf-8')
+        req = Request(TOKEN_URL, post_data)
+        try:
+            f = urlopen(req)
+            result_str = f.read()
+        except URLError as err:
+            print('token http response http code : ' + str(err.code))
+            result_str = err.read()
+        result_str =  result_str.decode()
+
+        #print(result_str)
+        result = json.loads(result_str)
+        #print(result)
+        SCOPE=False
+        if ('access_token' in result.keys() and 'scope' in result.keys()):
+            #print(SCOPE)
+            if SCOPE and (not SCOPE in result['scope'].split(' ')):  # SCOPE = False 忽略检查
+                raise DemoError('scope is not correct')
+            #print('SUCCESS WITH TOKEN: %s  EXPIRES IN SECONDS: %s' % (result['access_token'], result['expires_in']))
+            return result['access_token']
+        else:
+            raise DemoError('MAYBE API_KEY or SECRET_KEY not correct: access_token or scope not found in token response')
+
+
 
     #绘画直线
     '''
     x1,y1为初始点坐标,x2,y2为终止点坐标
     '''
     def lcd_line(self,x1,y1,x2,y2,color="WHITE",width=2):
         self.draw.line([(x1,y1),(x2,y2)],fill=color ,width=width)
@@ -252,15 +288,15 @@
     '''
     filename 文件名 字符串
     seconds 录制时间S 字符串
     '''
     def xgoAudioRecord(self,filename="record",seconds=5):
         path="/home/pi/xgoMusic/"
         command1 = "sudo arecord -d"
-        command2 = "-f S32_LE -r 16000 -c 1 -t wav"
+        command2 = "-f S32_LE -r 8000 -c 1 -t wav"
         cmd=command1+" "+str(seconds)+" "+command2+" "+path+filename+".wav"
         print(cmd)
         os.system(cmd)
 
     def xgoCamera(self,switch):
         global camera_still
         if switch:
@@ -610,15 +646,214 @@
         
     def circle(self,frame,xy,rad,colors,tk):
         frame=cv2.circle(frame,xy,rad,color(colors),tk)
         return frame
     
     def text(self,frame,text,xy,font_size,colors,size):
         frame=cv2.putText(frame,text,xy,cv2.FONT_HERSHEY_SIMPLEX,font_size,color(colors),size)
-        return frame       
+        return frame   
+
+    def SpeechRecognition(self,seconds=3):
+        self.xgoAudioRecord(filename="recog",seconds=seconds)
+        from urllib.request import urlopen
+        from urllib.request import Request
+        from urllib.error import URLError
+        from urllib.parse import urlencode
+        timer = time.perf_counter
+        AUDIO_FILE = 'recog.wav' 
+        FORMAT = AUDIO_FILE[-3:]  
+        CUID = '123456PYTHON'
+        RATE = 16000
+        DEV_PID = 1537  
+        ASR_URL = 'http://vop.baidu.com/server_api'
+        SCOPE = 'audio_voice_assistant_get' 
+
+        token = self.fetch_token()
+
+        speech_data = []
+        path="/home/pi/xgoMusic/"
+        with open(path+AUDIO_FILE, 'rb') as speech_file:
+            speech_data = speech_file.read()
+
+        length = len(speech_data)
+        if length == 0:
+            raise DemoError('file %s length read 0 bytes' % AUDIO_FILE)
+        speech = base64.b64encode(speech_data)
+        speech = str(speech, 'utf-8')
+        params = {'dev_pid': DEV_PID,
+                'format': FORMAT,
+                'rate': RATE,
+                'token': token,
+                'cuid': CUID,
+                'channel': 1,
+                'speech': speech,
+                'len': length
+                }
+        post_data = json.dumps(params, sort_keys=False)
+        req = Request(ASR_URL, post_data.encode('utf-8'))
+        req.add_header('Content-Type', 'application/json')
+        try:
+            begin = timer()
+            f = urlopen(req)
+            result_str = f.read()
+            print ("Request time cost %f" % (timer() - begin))
+        except URLError as err:
+            print('asr http response http code : ' + str(err.code))
+            result_str = err.read()
+        try:
+            result_str = str(result_str, 'utf-8')
+            re=json.loads(result_str)
+            text=re['result'][0]
+        except:
+            text='error!'
+        return text
+
+    def SpeechSynthesis(self,texts):
+        from urllib.request import urlopen
+        from urllib.request import Request
+        from urllib.error import URLError
+        from urllib.parse import urlencode
+        from urllib.parse import quote_plus
+
+        TEXT = texts
+        PER = 0
+        SPD = 5
+        PIT = 5
+        VOL = 5
+        AUE = 6
+        FORMATS = {3: "mp3", 4: "pcm", 5: "pcm", 6: "wav"}
+        FORMAT = FORMATS[AUE]
+        CUID = "123456PYTHON"
+        TTS_URL = 'http://tsn.baidu.com/text2audio'
+
+        SCOPE = 'audio_tts_post' 
+
+        token = self.fetch_token()
+        tex = quote_plus(TEXT) 
+        print(tex)
+        params = {'tok': token, 'tex': tex, 'per': PER, 'spd': SPD, 'pit': PIT, 'vol': VOL, 'aue': AUE, 'cuid': CUID,
+                'lan': 'zh', 'ctp': 1}  
+
+        data = urlencode(params)
+        print('test on Web Browser' + TTS_URL + '?' + data)
+
+        req = Request(TTS_URL, data.encode('utf-8'))
+        has_error = False
+        try:
+            f = urlopen(req)
+            result_str = f.read()
+
+            headers = dict((name.lower(), value) for name, value in f.headers.items())
+
+            has_error = ('content-type' not in headers.keys() or headers['content-type'].find('audio/') < 0)
+        except  URLError as err:
+            print('asr http response http code : ' + str(err.code))
+            result_str = err.read()
+            has_error = True
+
+        path="/home/pi/xgoMusic/"
+        save_file = "error.txt" if has_error else 'result.' + FORMAT
+        with open(path+save_file, 'wb') as of:
+            of.write(result_str)
+
+        if has_error:
+            if (IS_PY3):
+                result_str = str(result_str, 'utf-8')
+            print("tts api  error:" + result_str)
+
+        print("result saved as :" + save_file)
+
+        self.xgoSpeaker("result.wav")
+    
+    def QRRecognition(self,target="camera"):
+        import pyzbar.pyzbar as pyzbar
+        if target=="camera":
+            self.xgoTakePhoto(filename="photo")
+            path="/home/pi/xgoPictures/photo.jpg"
+            img=cv2.imread(path)
+        else:
+            img=cv2.imread("/home/pi/xgoPictures/"+target)
+        barcodes = pyzbar.decode(img) 
+        result=[]
+        for barcode in barcodes:
+            barcodeData = barcode.data.decode("utf-8")
+            barcodeType = barcode.type
+            result.append(barcodeData)
+        try:
+            re=result[0]
+        except:
+            result=[]
+        self.xgoCamera(False)
+        return result
+
+    def ColorRecognitio(self,target="camera",mode='R'):
+        color_x = 0
+        color_y = 0
+        color_radius = 0
+
+        if mode=='R':  #red
+            color_lower = np.array([0, 43, 46])
+            color_upper = np.array([10, 255, 255])
+        elif mode=='G': #green
+            color_lower = np.array([35, 43, 46])
+            color_upper = np.array([77, 255, 255])
+        elif mode=='B':   #blue
+            color_lower = np.array([100, 43, 46])
+            color_upper = np.array([124, 255, 255])
+        elif mode=='Y':   #yellow
+            color_lower = np.array([26, 43, 46])
+            color_upper = np.array([34, 255, 255])
+        if target=="camera":
+            self.xgoTakePhoto(filename="photo")
+            path="/home/pi/xgoPictures/photo.jpg"
+            img=cv2.imread(path)
+        else:
+            img=cv2.imread("/home/pi/xgoPictures/"+target)
+        frame_ = cv2.GaussianBlur(img,(5,5),0)                    
+        hsv = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
+        mask = cv2.inRange(hsv,color_lower,color_upper)  
+        mask = cv2.erode(mask,None,iterations=2)
+        mask = cv2.dilate(mask,None,iterations=2)
+        mask = cv2.GaussianBlur(mask,(3,3),0)     
+        cnts = cv2.findContours(mask.copy(),cv2.RETR_EXTERNAL,cv2.CHAIN_APPROX_SIMPLE)[-2] 
+
+        if len(cnts) > 0:
+            cnt = max (cnts, key = cv2.contourArea)
+            (color_x,color_y),color_radius = cv2.minEnclosingCircle(cnt)
+
+        self.xgoCamera(False)
+
+        return ((color_x,color_y),color_radius)
+
+    def CircleRecognition(self,target="camera"):
+        if target=="camera":
+            self.xgoTakePhoto(filename="photo")
+            path="/home/pi/xgoPictures/photo.jpg"
+            img = cv2.imread(path, cv2.IMREAD_GRAYSCALE)     # 0 转为灰度图像
+            #img2 = cv2.imread(path, cv2.IMREAD_COLOR)     # 1 为彩色图像
+        else:
+            img=cv2.imread("/home/pi/xgoPictures/"+target,cv2.IMREAD_GRAYSCALE)
+        numpy_img = cv2.adaptiveThreshold(img, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 11, 15)   # 自动阈值二值化
+        #                                                      圆心距 canny阈值    投票数      最小半径       最大半径
+        circles = cv2.HoughCircles(img, cv2.HOUGH_GRADIENT, 1, 18,   param1=100, param2=80,  minRadius=40, maxRadius=150)
+        arr1 = np.zeros([0, 2], dtype=int)                      # 创建一个0行, 2列的空数组
+        re=[]
+        if circles is not None:
+            circles = np.uint16(np.around(circles))   
+            for i in circles[0, :]:
+                re.append(((i[0], i[1]), i[2]))
+        self.xgoCamera(False)
+        return re
+
+
+
+
+
+class DemoError(Exception):
+    pass
 
 class hands():
     def __init__(self,model_complexity,max_num_hands,min_detection_confidence,min_tracking_confidence):
         import mediapipe as mp
         self.model_complexity = model_complexity
         self.max_num_hands = max_num_hands
         self.min_detection_confidence = min_detection_confidence
```

### Comparing `xgo-pythonlib-0.2.0/xgolib/__init__.py` & `xgo-pythonlib-0.2.1/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.0/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.2.1/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.0/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.2.1/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

