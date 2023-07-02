# Comparing `tmp/modbus2mqtt-0.65.tar.gz` & `tmp/modbus2mqtt-0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbus2mqtt-0.65.tar", last modified: Fri Nov 25 02:33:43 2022, max compression
+gzip compressed data, was "modbus2mqtt-0.67.tar", last modified: Sun Jul  2 14:38:59 2023, max compression
```

## Comparing `modbus2mqtt-0.65.tar` & `modbus2mqtt-0.67.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-11-25 02:33:43.586851 modbus2mqtt-0.65/
--rw-r--r--   0 max       (1000) max       (1000)     1199 2022-01-05 14:39:31.000000 modbus2mqtt-0.65/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)       16 2022-02-06 05:39:30.000000 modbus2mqtt-0.65/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)      228 2022-11-25 02:33:43.586851 modbus2mqtt-0.65/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     9747 2022-11-25 02:32:39.000000 modbus2mqtt-0.65/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-11-25 02:33:43.582851 modbus2mqtt-0.65/modbus2mqtt/
--rw-r--r--   0 max       (1000) max       (1000)       22 2022-02-06 05:39:30.000000 modbus2mqtt-0.65/modbus2mqtt/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)       59 2022-02-06 05:39:30.000000 modbus2mqtt-0.65/modbus2mqtt/__main__.py
--rw-r--r--   0 max       (1000) max       (1000)     2425 2022-02-06 05:39:30.000000 modbus2mqtt-0.65/modbus2mqtt/addToHomeAssistant.py
--rw-r--r--   0 max       (1000) max       (1000)    37697 2022-11-25 02:20:48.000000 modbus2mqtt-0.65/modbus2mqtt/modbus2mqtt.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-11-25 02:33:43.586851 modbus2mqtt-0.65/modbus2mqtt.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)      228 2022-11-25 02:33:43.000000 modbus2mqtt-0.65/modbus2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      359 2022-11-25 02:33:43.000000 modbus2mqtt-0.65/modbus2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2022-11-25 02:33:43.000000 modbus2mqtt-0.65/modbus2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       61 2022-11-25 02:33:43.000000 modbus2mqtt-0.65/modbus2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       19 2022-11-25 02:33:43.000000 modbus2mqtt-0.65/modbus2mqtt.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)       12 2022-11-25 02:33:43.000000 modbus2mqtt-0.65/modbus2mqtt.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)       38 2022-11-25 02:33:43.586851 modbus2mqtt-0.65/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      854 2022-02-06 05:39:30.000000 modbus2mqtt-0.65/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-07-02 14:38:59.167681 modbus2mqtt-0.67/
+-rw-r--r--   0 max       (1000) max       (1000)     1199 2022-01-05 14:39:31.000000 modbus2mqtt-0.67/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)       16 2022-02-06 05:39:30.000000 modbus2mqtt-0.67/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)      228 2023-07-02 14:38:59.167681 modbus2mqtt-0.67/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     9830 2022-11-29 00:25:25.000000 modbus2mqtt-0.67/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-07-02 14:38:59.167681 modbus2mqtt-0.67/modbus2mqtt/
+-rw-r--r--   0 max       (1000) max       (1000)       22 2022-02-06 05:39:30.000000 modbus2mqtt-0.67/modbus2mqtt/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)       59 2022-02-06 05:39:30.000000 modbus2mqtt-0.67/modbus2mqtt/__main__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2425 2022-02-06 05:39:30.000000 modbus2mqtt-0.67/modbus2mqtt/addToHomeAssistant.py
+-rw-r--r--   0 max       (1000) max       (1000)    37823 2023-07-02 14:37:47.000000 modbus2mqtt-0.67/modbus2mqtt/modbus2mqtt.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-07-02 14:38:59.167681 modbus2mqtt-0.67/modbus2mqtt.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)      228 2023-07-02 14:38:59.000000 modbus2mqtt-0.67/modbus2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      359 2023-07-02 14:38:59.000000 modbus2mqtt-0.67/modbus2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-07-02 14:38:59.000000 modbus2mqtt-0.67/modbus2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       61 2023-07-02 14:38:59.000000 modbus2mqtt-0.67/modbus2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       19 2023-07-02 14:38:59.000000 modbus2mqtt-0.67/modbus2mqtt.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       12 2023-07-02 14:38:59.000000 modbus2mqtt-0.67/modbus2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)       38 2023-07-02 14:38:59.167681 modbus2mqtt-0.67/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      854 2022-02-06 05:39:30.000000 modbus2mqtt-0.67/setup.py
```

### Comparing `modbus2mqtt-0.65/LICENSE` & `modbus2mqtt-0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `modbus2mqtt-0.65/README.md` & `modbus2mqtt-0.67/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 values via MQTT.
 
 It is intended as a building block in heterogeneous smart home environments where 
 an MQTT message broker is used as the centralized message bus.
 
 Changelog
 ---------
+- version 0.66, 29. of November 2022: print Modbus exceptions generated by devices
 - version 0.65, 25. of November 2022: fixed incompatibility with newer version of pymodbus, readjusted the Dockerfile
 - version 0.64, 16. of October 2022: Adjustment of the Dockerfile (enforcing pymodbus 2.5.3, otherwise it tries to use 3.0 and this failes); typo fixed; main-/poller-loop log entry
 - version 0.63, 04. of October 2022: added reading and writing of int32 values, fix regarding negative floats
 - version 0.62, 6. of February 2022: major refactoring, project is now python module available via pip
 - version 0.5, 21. of September 2019: print error messages in case of badly configured pollers
 - version 0.4, 25. of May 2019: When writing to a device, updated states are now published immediately, if writing was successful.
```

### Comparing `modbus2mqtt-0.65/modbus2mqtt/addToHomeAssistant.py` & `modbus2mqtt-0.67/modbus2mqtt/addToHomeAssistant.py`

 * *Files identical despite different names*

### Comparing `modbus2mqtt-0.65/modbus2mqtt/modbus2mqtt.py` & `modbus2mqtt-0.67/modbus2mqtt/modbus2mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     from pymodbus.client.sync import ModbusSerialClient as SerialModbusClient
     from pymodbus.client.sync import ModbusTcpClient as TCPModbusClient
 except:
     from pymodbus.client import ModbusSerialClient as SerialModbusClient
     from pymodbus.client import ModbusTcpClient as TCPModbusClient 
 from pymodbus.transaction import ModbusRtuFramer
 
-__version__ = "0.65"
+__version__ = "0.67"
 mqtt_port = None
 mqc = None
 parser = None
 args = None
 verbosity = None
 addToHass = None
 loopBreak = None
@@ -168,48 +168,48 @@
 
     def poll(self):
             result = None
             if master.is_socket_open()==True:
                 failed = False
                 try:
                     if self.functioncode == 3:
-                        result = master.read_holding_registers(self.reference, self.size, unit=self.slaveid)
+                        result = master.read_holding_registers(self.reference, self.size, self.slaveid)
                         if result.function_code < 0x80:
                             data = result.registers
                         else:
                             failed = True
                     if self.functioncode == 1:
-                        result = master.read_coils(self.reference, self.size, unit=self.slaveid)
+                        result = master.read_coils(self.reference, self.size, self.slaveid)
                         if result.function_code < 0x80:
                             data = result.bits
                         else:
                             failed = True
 
                     if self.functioncode == 2:
-                        result = master.read_discrete_inputs(self.reference, self.size, unit=self.slaveid)
+                        result = master.read_discrete_inputs(self.reference, self.size, self.slaveid)
                         if result.function_code < 0x80:
                             data = result.bits
                         else:
                             failed = True
                     if self.functioncode == 4:
-                        result = master.read_input_registers(self.reference, self.size, unit=self.slaveid)
+                        result = master.read_input_registers(self.reference, self.size, self.slaveid)
                         if result.function_code < 0x80:
                             data = result.registers
                         else:
                             failed = True
                     if not failed:
                         if verbosity>=4:
                             print("Read MODBUS, FC:"+str(self.functioncode)+", DataType:"+str(self.dataType)+", ref:"+str(self.reference)+", Qty:"+str(self.size)+", SI:"+str(self.slaveid))
                             print("Read MODBUS, DATA:"+str(data))
                         for ref in self.readableReferences:
-                            val = data[ref.relativeReference:(ref.length+ref.relativeReference)]
+                            val = data[ref.relativeReference:(ref.regAmount+ref.relativeReference)]
                             ref.checkPublish(val)
                     else:
                         if verbosity>=1:
-                            print("Slave device "+str(self.slaveid)+" responded with error code: "+str(result.function_code))
+                            print("Slave device "+str(self.slaveid)+" responded with error code:"+str(result).split(',', 3)[2].rstrip(')'))
                 except:
                     failed = True
                     if verbosity>=1:
                         print("Error talking to slave device:"+str(self.slaveid)+" (connection timeout)")
                 self.failCount(failed)
             else:
                 if master.connect():
@@ -263,260 +263,293 @@
                        self.device.writableReferences.append(myRef)
                        referenceList.append(myRef)
             else:
                 print("Reference \""+str(myRef.reference)+"\" with topic "+myRef.topic+" in poller \""+self.topic+"\" is neither read nor writable, therefore ignoring it.")
         else:
             print("Reference topic ("+str(myRef.topic)+") is already occupied for poller \""+self.topic+"\", therefore ignoring it.")
 
-class dataTypes:
-    def __init__(self,conf):
-        if conf is None or conf == "uint16" or conf == "":
-            self.regAmount=1          
-            self.parse=self.parseuint16
-            self.combine=self.combineuint16
-        elif conf.startswith("string"):
-            try:
-                length = int(conf[6:9])
-            except:
-                length = 2
-            if length > 100:
-                print("Data type string: length too long")
-                length = 100
-            if  math.fmod(length,2) != 0:
-                length=length-1
-                print("Data type string: length must be divisible by 2")
-            self.parse=self.parseString
-            self.combine=self.combineString
-            self.stringLength=length
-            self.regAmount=int(length/2)
-        elif conf == "int32LE":
-            self.parse=self.parseint32LE
-            self.combine=self.combineint32LE
-            self.regAmount=2
-        elif conf == "int32BE":
-            self.regAmount=2
-            self.parse=self.parseint32BE
-            self.combine=self.combineint32BE
-        elif conf == "int16":
-            self.regAmount=1         
-            self.parse=self.parseint16
-            self.combine=self.combineint16
-        elif conf == "uint32LE":
-            self.regAmount=2          
-            self.parse=self.parseuint32LE
-            self.combine=self.combineuint32LE
-        elif conf == "uint32BE":
-            self.regAmount=2          
-            self.parse=self.parseuint32BE
-            self.combine=self.combineuint32BE
-        elif conf == "bool":
-            self.regAmount=1         
-            self.parse=self.parsebool
-            self.combine=self.combinebool
-        elif conf == "float32LE":
-            self.regAmount=2          
-            self.parse=self.parsefloat32LE
-            self.combine=self.combinefloat32LE
-        elif conf == "float32BE":
-           self.regAmount=2          
-           self.parse=self.parsefloat32BE
-           self.combine=self.combinefloat32BE
-   
-    def parsebool(self,payload):
-        if payload == 'True' or payload == 'true' or payload == '1' or payload == 'TRUE':
-            value = True
-        elif payload == 'False' or payload == 'false' or payload == '0' or payload == 'FALSE':
-            value = False
+def dataTypes(self,conf):
+    if conf is None or conf == "uint16" or conf == "":
+        self.regAmount=1
+        self.parse=parseuint16
+        self.combine=combineuint16
+    elif conf.startswith("list-uint16-"):
+        try:
+            length = int(conf[12:15])
+        except:
+            length = 1
+        if length > 50:
+            print("Data type list-uint16: length too long")
+            length = 50
+        self.parse=parseListUint16
+        self.combine=combineListUint16
+        self.regAmount=length
+    elif conf.startswith("string"):
+        try:
+            length = int(conf[6:9])
+        except:
+            length = 2
+        if length > 100:
+            print("Data type string: length too long")
+            length = 100
+        if  math.fmod(length,2) != 0:
+            length=length-1
+            print("Data type string: length must be divisible by 2")
+        self.parse=parseString
+        self.combine=combineString
+        self.stringLength=length
+        self.regAmount=int(length/2)
+    elif conf == "int32LE":
+        self.parse=parseint32LE
+        self.combine=combineint32LE
+        self.regAmount=2
+    elif conf == "int32BE":
+        self.regAmount=2
+        self.parse=parseint32BE
+        self.combine=combineint32BE
+    elif conf == "int16":
+        self.regAmount=1
+        self.parse=parseint16
+        self.combine=combineint16
+    elif conf == "uint32LE":
+        self.regAmount=2
+        self.parse=parseuint32LE
+        self.combine=combineuint32LE
+    elif conf == "uint32BE":
+        self.regAmount=2
+        self.parse=parseuint32BE
+        self.combine=combineuint32BE
+    elif conf == "bool":
+        self.regAmount=1
+        self.parse=parsebool
+        self.combine=combinebool
+    elif conf == "float32LE":
+        self.regAmount=2
+        self.parse=parsefloat32LE
+        self.combine=combinefloat32LE
+    elif conf == "float32BE":
+       self.regAmount=2
+       self.parse=parsefloat32BE
+       self.combine=combinefloat32BE
+
+def parsebool(self,payload):
+    if payload == 'True' or payload == 'true' or payload == '1' or payload == 'TRUE':
+        value = True
+    elif payload == 'False' or payload == 'false' or payload == '0' or payload == 'FALSE':
+        value = False
+    else:
+        value = None
+    return value
+
+def combinebool(self,val):
+    try:
+        len(val)
+        return bool(val[0])
+    except:
+        return bool(val)
+
+def parseListUint16(self,msg):
+    out=[]
+    try:
+        msg=msg.rstrip()
+        msg=msg.lstrip()
+        msg=msg.split(" ")
+        if len(msg) != self.regAmount:
+            return None
+        for x in range(0, len(msg)):
+            out.append(int(msg[x]))
+    except:
+        return None
+    return out
+
+def combineListUint16(self,val):
+    out=""
+    for x in val:
+        out+=str(x)+" "
+    return out
+
+def parseString(self,msg):
+    out=[]
+    if len(msg)<=self.stringLength:
+        for x in range(1,len(msg)+1):
+            if math.fmod(x,2)>0:
+                out.append(ord(msg[x-1])<<8)
+            else:
+                pass
+                out[int(x/2-1)]+=ord(msg[x-1])
+    else:
+        out = None
+    return out
+def combineString(self,val):
+    out=""
+    for x in val:
+        out+=chr(x>>8)
+        out+=chr(x&0x00FF)
+    return out
+
+def parseint16(self,msg):
+    try:
+        value=int(msg)
+        if value > 32767 or value < -32768:
+            out = None
         else:
-            value = None
-        return value
-
-    def combinebool(self,val):
-        try:
-            len(val)
-            return bool(val[0])
-        except:
-            return bool(val)
-
-    def parseString(self,msg):
-        out=[]
-        if len(msg)<=self.stringLength:
-            for x in range(1,len(msg)+1):
-                if math.fmod(x,2)>0:
-                    out.append(ord(msg[x-1])<<8)
-                else:
-                    pass
-                    out[int(x/2-1)]+=ord(msg[x-1])
+            out = value&0xFFFF
+    except:
+        out=None
+    return out
+def combineint16(self,val):
+    try:
+        len(val)
+        myval=val[0]
+    except:
+        myval=val
+
+    if (myval & 0x8000) > 0:
+        out = -((~myval & 0x7FFF)+1)
+    else:
+        out = myval
+    return out
+
+def parseuint32LE(self,msg):
+    try:
+        value=int(msg)
+        if value > 4294967295 or value < 0:
+            out = None
         else:
+            out=[int(value>>16),int(value&0x0000FFFF)]
+    except:
+        out=None
+    return out
+def combineuint32LE(self,val):
+    out = val[0]*65536 + val[1]
+    return out
+
+def parseuint32BE(self,msg):
+    try:
+        value=int(msg)
+        if value > 4294967295 or value < 0:
             out = None
-        return out
-    def combineString(self,val):
-        out=""
-        for x in val:
-            out+=chr(x>>8)
-            out+=chr(x&0x00FF)
-        return out
-
-    def parseint16(self,msg):
-        try:
-            value=int(msg)
-            if value > 32767 or value < -32768:
-                out = None
-            else:
-                out = value&0xFFFF
-        except:
-            out=None
-        return out
-    def combineint16(self,val):
-        try:
-            len(val)
-            myval=val[0]
-        except:
-            myval=val
-
-        if (myval & 0x8000) > 0:
-            out = -((~myval & 0x7FFF)+1)
         else:
-            out = myval
-        return out
-
-    def parseuint32LE(self,msg):
-        try:
-            value=int(msg)
-            if value > 4294967295 or value < 0:
-                out = None
-            else:
-                out=[int(value>>16),int(value&0x0000FFFF)]
-        except:
-            out=None
-        return out
-    def combineuint32LE(self,val):
-        out = val[0]*65536 + val[1]
-        return out
-
-    def parseuint32BE(self,msg):
-        try:
-            value=int(msg)
-            if value > 4294967295 or value < 0:
-                out = None
-            else:
-                out=[int(value&0x0000FFFF),int(value>>16)]
-        except:
-            out=None
-        return out
-    def combineuint32BE(self,val):
-        out = val[0] + val[1]*65536
-        return out
-
-    def parseint32LE(self,msg):
-        try:
-            value=int(msg)
-            value = int.from_bytes(value.to_bytes(4, 'little', signed=False), 'little', signed=True)
-        except:
-            out=None
-        return out
-    def combineint32LE(self,val):
-        out = val[0]*65536 + val[1]
-        out = int.from_bytes(out.to_bytes(4, 'little', signed=False), 'little', signed=True)
-        return out
-
-    def parseint32BE(self,msg):
-        try:
-            value=int(msg)
-            value = int.from_bytes(value.to_bytes(4, 'big', signed=False), 'big', signed=True)
-        except:
-            out=None
-        return out
-    def combineint32BE(self,val):
-        out = val[0] + val[1]*65536
-        out = int.from_bytes(out.to_bytes(4, 'big', signed=False), 'big', signed=True)
-        return out
-    
-    def parseuint16(self,msg):
-        try:
-            value=int(msg)
-            if value > 65535 or value < 0:
-                value = None
-        except:
-            value=None
-        return value
-    def combineuint16(self,val):
-        try:
-            len(val)
-            return val[0]
-        except:
-            return val
-
-    def parsefloat32LE(self,msg):
-        try:
-            out=None
-            #value=int(msg)
-            #if value > 4294967295 or value < 0:
-            #    out = None
-            #else:
-            #    out=[int(value&0x0000FFFF),int(value>>16)]
-        except:
-            out=None
-        return out
-    def combinefloat32LE(self,val):
-        out = str(struct.unpack('=f', struct.pack('=I',int(val[0])<<16|int(val[1])))[0])
-        return out
-
-    def parsefloat32BE(self,msg):
-        try:
-            out=None
-            #value=int(msg)
-            #if value > 4294967295 or value < 0:
-            #    out = None
-            #else:
-            #    out=[int(value&0x0000FFFF),int(value>>16)]
-        except:
-            out=None
-        return out
-    def combinefloat32BE(self,val):
-        out = str(struct.unpack('=f', struct.pack('=I',int(val[1])<<16|int(val[0])))[0])
-        return out
+            out=[int(value&0x0000FFFF),int(value>>16)]
+    except:
+        out=None
+    return out
+def combineuint32BE(self,val):
+    out = val[0] + val[1]*65536
+    return out
+
+def parseint32LE(self,msg):
+    #try:
+    #    value=int(msg)
+    #    value = int.from_bytes(value.to_bytes(4, 'little', signed=False), 'little', signed=True)
+    #except:
+    #    out=None
+    #return out
+    return None
+def combineint32LE(self,val):
+    out = val[0]*65536 + val[1]
+    out = int.from_bytes(out.to_bytes(4, 'little', signed=False), 'little', signed=True)
+    return out
+
+def parseint32BE(self,msg):
+    #try:
+    #    value=int(msg)
+    #    value = int.from_bytes(value.to_bytes(4, 'big', signed=False), 'big', signed=True)
+    #except:
+    #    out=None
+    #return out
+    return None
+def combineint32BE(self,val):
+    out = val[0] + val[1]*65536
+    out = int.from_bytes(out.to_bytes(4, 'big', signed=False), 'big', signed=True)
+    return out
+
+def parseuint16(self,msg):
+    try:
+        value=int(msg)
+        if value > 65535 or value < 0:
+            value = None
+    except:
+        value=None
+    return value
+def combineuint16(self,val):
+    try:
+        len(val)
+        return val[0]
+    except:
+        return val
+
+def parsefloat32LE(self,msg):
+    try:
+        out=None
+        #value=int(msg)
+        #if value > 4294967295 or value < 0:
+        #    out = None
+        #else:
+        #    out=[int(value&0x0000FFFF),int(value>>16)]
+    except:
+        out=None
+    return out
+def combinefloat32LE(self,val):
+    out = str(struct.unpack('=f', struct.pack('=I',int(val[0])<<16|int(val[1])))[0])
+    return out
+
+def parsefloat32BE(self,msg):
+    try:
+        out=None
+        #value=int(msg)
+        #if value > 4294967295 or value < 0:
+        #    out = None
+        #else:
+        #    out=[int(value&0x0000FFFF),int(value>>16)]
+    except:
+        out=None
+    return out
+def combinefloat32BE(self,val):
+    out = str(struct.unpack('=f', struct.pack('=I',int(val[1])<<16|int(val[0])))[0])
+    return out
 
 class Reference:
     def __init__(self,topic,reference,dtype,rw,poller,scaling):
         self.topic=topic
         self.reference=int(reference)
         self.lastval=None
         self.scale=None
+        self.regAmount=None
+        self.stringLength=None
+
         if scaling:
             try:
                 self.scale=float(scaling)
             except ValueError as e:
               if verbosity>=1:
                 print("Scaling Error:", e)
         self.rw=rw
         self.relativeReference=None
         self.writefunctioncode=None
         self.device=None
         self.poller=poller
-        self.dtype=None
         if self.poller.functioncode == 1:
-            self.dtype=dataTypes("bool")
+            dataTypes(self,"bool")
             
         elif self.poller.functioncode == 2:
-            self.dtype=dataTypes("bool")
+            dataTypes(self,"bool")
         else:
-            self.dtype=dataTypes(dtype)
-        self.length=self.dtype.regAmount
+            dataTypes(self,dtype)
 
     def checkSanity(self,reference,size):
-        if self.reference in range(reference,size+reference) and self.reference+self.length-1 in range(reference,size+reference):
+        if self.reference in range(reference,size+reference) and self.reference+self.regAmount-1 in range(reference,size+reference):
             self.relativeReference=self.reference-reference
             return True
 
     def checkPublish(self,val):
         # Only publish messages after the initial connection has been made. If it became disconnected then the offline buffer will store messages,
         # but only after the intial connection was made.
         if mqc.initial_connection_made == True:
-            val = self.dtype.combine(val)
+            val = self.combine(self,val)
             if self.lastval != val or args.always_publish:
                 self.lastval = val
                 if self.scale:
                     val = val * self.scale
                 try:
                     publish_result = mqc.publish(globaltopic+self.device.name+"/state/"+self.topic,val,retain=True)
                     if verbosity>=4:
@@ -555,48 +588,55 @@
     for iterRef in myDevice.writableReferences:
         if iterRef.topic == reference:
             myRef=iterRef
     if myRef == None: # no such reference
         return    
     payload = str(msg.payload.decode("utf-8"))
     if myRef.writefunctioncode == 5:
-        value = myRef.dtype.parse(str(payload))
+        value = myRef.parse(myRef,str(payload))
         if value != None:
-                result = master.write_coil(int(myRef.reference),value,unit=int(myRef.device.slaveid))
+                result = master.write_coil(int(myRef.reference),value,int(myRef.device.slaveid))
                 try:
                     if result.function_code < 0x80:
                         myRef.checkPublish(value) # writing was successful => we can assume, that the corresponding state can be set and published
                         if verbosity>=3:
                             print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" successful.")
                     else:
                         if verbosity>=1:
-                            print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" FAILED! (Devices responded with errorcode. Maybe bad configuration?)")
+                            print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" FAILED! (Devices responded with errorcode"+str(result).split(',', 3)[2].rstrip(')')+". Maybe bad configuration?)")
             
                 except:
                     if verbosity>=1:
                         print("Error writing to slave device "+str(myDevice.slaveid)+" (maybe CRC error or timeout)")
         else:
             if verbosity >= 1:
                 print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" not possible. Given value is not \"True\" or \"False\".")
 
 
     if myRef.writefunctioncode == 6:
-        value = myRef.dtype.parse(str(payload))
+        value = myRef.parse(myRef,str(payload))
         if value is not None:
-            if myRef.scale: # reverse scale if required
-                value = type(value)(value / myRef.scale)
-            result = master.write_registers(int(myRef.reference),value,unit=myRef.device.slaveid)
+            #if myRef.scale: # reverse scale if required
+            #    value = type(value)(value / myRef.scale)
+            try:
+                valLen=len(value)
+            except:
+                valLen=1
+            if valLen>1:
+                result = master.write_registers(int(myRef.reference),value,myRef.device.slaveid)
+            else:
+                result = master.write_register(int(myRef.reference),value,myRef.device.slaveid)
             try:
                 if result.function_code < 0x80:
                     myRef.checkPublish(value) # writing was successful => we can assume, that the corresponding state can be set and published
                     if verbosity>=3:
                         print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" successful.")
                 else:
                     if verbosity>=1:
-                        print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" FAILED! (Devices responded with errorcode. Maybe bad configuration?)")
+                        print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" FAILED! (Devices responded with errorcode"+str(result).split(',', 3)[2].rstrip(')')+". Maybe bad configuration?)")
             except:
                 if verbosity >= 1:
                     print("Error writing to slave device "+str(myDevice.slaveid)+" (maybe CRC error or timeout)")
         else:
             if verbosity >= 1:
                 print("Writing to device "+str(myDevice.name)+", Slave-ID="+str(myDevice.slaveid)+" at Reference="+str(myRef.reference)+" using function code "+str(myRef.writefunctioncode)+" not possible. Value does not fulfill criteria.")
```

### Comparing `modbus2mqtt-0.65/setup.py` & `modbus2mqtt-0.67/setup.py`

 * *Files identical despite different names*

