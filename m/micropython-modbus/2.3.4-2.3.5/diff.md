# Comparing `tmp/micropython-modbus-2.3.4.tar.gz` & `tmp/micropython-modbus-2.3.5.tar.gz`

## Comparing `micropython-modbus-2.3.4.tar` & `micropython-modbus-2.3.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-03-20 16:45:50.000000 micropython-modbus-2.3.4/micropython_modbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33536 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-20 16:45:39.000000 micropython-modbus-2.3.4/umodbus/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-20 16:45:49.000000 micropython-modbus-2.3.4/umodbus/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-02 05:09:14.000000 micropython-modbus-2.3.5/micropython_modbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33536 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-02 05:09:03.000000 micropython-modbus-2.3.5/umodbus/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-02 05:09:13.000000 micropython-modbus-2.3.5/umodbus/version.py
```

### Comparing `micropython-modbus-2.3.4/micropython_modbus.egg-info/PKG-INFO` & `micropython-modbus-2.3.5/micropython_modbus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-modbus
-Version: 2.3.4
+Version: 2.3.5
 Summary: MicroPython ModBus TCP and RTU library supporting client and host mode
 Home-page: https://github.com/brainelectronics/micropython-modbus
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-modbus/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-modbus
```

### Comparing `micropython-modbus-2.3.4/umodbus/common.py` & `micropython-modbus-2.3.5/umodbus/common.py`

 * *Files identical despite different names*

### Comparing `micropython-modbus-2.3.4/umodbus/const.py` & `micropython-modbus-2.3.5/umodbus/const.py`

 * *Files identical despite different names*

### Comparing `micropython-modbus-2.3.4/umodbus/functions.py` & `micropython-modbus-2.3.5/umodbus/functions.py`

 * *Files identical despite different names*

### Comparing `micropython-modbus-2.3.4/umodbus/modbus.py` & `micropython-modbus-2.3.5/umodbus/modbus.py`

 * *Files identical despite different names*

### Comparing `micropython-modbus-2.3.4/umodbus/serial.py` & `micropython-modbus-2.3.5/umodbus/serial.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 
 # system packages
 from machine import UART
 from machine import Pin
 import struct
 import time
-import machine
 
 # custom packages
 from . import const as Const
 from . import functions
 from .common import Request, CommonModbusFunctions
 from .common import ModbusException
 from .modbus import Modbus
@@ -92,14 +91,16 @@
         :param      parity:      The parity, default None
         :type       parity:      Optional[int]
         :param      pins:        The pins as list [TX, RX]
         :type       pins:        List[Union[int, Pin], Union[int, Pin]]
         :param      ctrl_pin:    The control pin
         :type       ctrl_pin:    int
         """
+        # UART flush function is introduced in Micropython v1.20.0
+        self._has_uart_flush = callable(getattr(UART, "flush", None))
         self._uart = UART(uart_id,
                           baudrate=baudrate,
                           bits=data_bits,
                           parity=parity,
                           stop=stop_bits,
                           # timeout_chars=2,  # WiPy only
                           # pins=pins         # WiPy only
@@ -108,20 +109,24 @@
                           )
 
         if ctrl_pin is not None:
             self._ctrlPin = Pin(ctrl_pin, mode=Pin.OUT)
         else:
             self._ctrlPin = None
 
+        # timing of 1 character in microseconds (us)
         self._t1char = (1000000 * (data_bits + stop_bits + 2)) // baudrate
+
+        # inter-frame delay in microseconds (us)
+        # - <= 19200 bps: 3.5x timing of 1 character
+        # - > 19200 bps: 1750 us
         if baudrate <= 19200:
-            # 4010us (approx. 4ms) @ 9600 baud
-            self._t35chars = (3500000 * (data_bits + stop_bits + 2)) // baudrate
+            self._inter_frame_delay = (self._t1char * 3500) // 1000
         else:
-            self._t35chars = 1750   # 1750us (approx. 1.75ms)
+            self._inter_frame_delay = 1750
 
     def _calculate_crc16(self, data: bytearray) -> bytes:
         """
         Calculates the CRC16.
 
         :param      data:        The data
         :type       data:        bytearray
@@ -139,50 +144,54 @@
     def _exit_read(self, response: bytearray) -> bool:
         """
         Return on modbus read error
 
         :param      response:    The response
         :type       response:    bytearray
 
-        :returns:   State of basic read response evaluation
+        :returns:   State of basic read response evaluation,
+                    True if entire response has been read
         :rtype:     bool
         """
-        if response[1] >= Const.ERROR_BIAS:
-            if len(response) < Const.ERROR_RESP_LEN:
+        response_len = len(response)
+        if response_len >= 2 and response[1] >= Const.ERROR_BIAS:
+            if response_len < Const.ERROR_RESP_LEN:
                 return False
-        elif (Const.READ_COILS <= response[1] <= Const.READ_INPUT_REGISTER):
+        elif response_len >= 3 and (Const.READ_COILS <= response[1] <= Const.READ_INPUT_REGISTER):
             expected_len = Const.RESPONSE_HDR_LENGTH + 1 + response[2] + Const.CRC_LENGTH
-            if len(response) < expected_len:
+            if response_len < expected_len:
                 return False
-        elif len(response) < Const.FIXED_RESP_LEN:
+        elif response_len < Const.FIXED_RESP_LEN:
             return False
 
         return True
 
     def _uart_read(self) -> bytearray:
         """
-        Read up to 40 bytes from UART
+        Read incoming slave response from UART
 
         :returns:   Read content
         :rtype:     bytearray
         """
         response = bytearray()
 
-        for x in range(1, 40):
+        # TODO: use some kind of hint or user-configurable delay
+        #       to determine this loop counter
+        for x in range(1, 120):
             if self._uart.any():
                 # WiPy only
                 # response.extend(self._uart.readall())
                 response.extend(self._uart.read())
 
                 # variable length function codes may require multiple reads
                 if self._exit_read(response):
                     break
 
             # wait for the maximum time between two frames
-            time.sleep_us(self._t35chars)
+            time.sleep_us(self._inter_frame_delay)
 
         return response
 
     def _uart_read_frame(self, timeout: Optional[int] = None) -> bytearray:
         """
         Read a Modbus frame
 
@@ -190,37 +199,36 @@
         :type       timeout:  Optional[int]
 
         :returns:   Received message
         :rtype:     bytearray
         """
         received_bytes = bytearray()
 
-        # set timeout to at least twice the time between two frames in case the
-        # timeout was set to zero or None
+        # set default timeout to at twice the inter-frame delay
         if timeout == 0 or timeout is None:
-            timeout = 2 * self._t35chars  # in milliseconds
+            timeout = 2 * self._inter_frame_delay  # in microseconds
 
         start_us = time.ticks_us()
 
         # stay inside this while loop at least for the timeout time
         while (time.ticks_diff(time.ticks_us(), start_us) <= timeout):
             # check amount of available characters
             if self._uart.any():
                 # remember this time in microseconds
                 last_byte_ts = time.ticks_us()
 
                 # do not stop reading and appending the result to the buffer
                 # until the time between two frames elapsed
-                while time.ticks_diff(time.ticks_us(), last_byte_ts) <= self._t35chars:
+                while time.ticks_diff(time.ticks_us(), last_byte_ts) <= self._inter_frame_delay:
                     # WiPy only
                     # r = self._uart.readall()
                     r = self._uart.read()
 
                     # if something has been read after the first iteration of
-                    # this inner while loop (during self._t35chars time)
+                    # this inner while loop (within self._inter_frame_delay)
                     if r is not None:
                         # append the new read stuff to the buffer
                         received_bytes.extend(r)
 
                         # update the timestamp of the last byte being read
                         last_byte_ts = time.ticks_us()
 
@@ -231,40 +239,57 @@
         # return the result in case the overall timeout has been reached
         return received_bytes
 
     def _send(self, modbus_pdu: bytes, slave_addr: int) -> None:
         """
         Send Modbus frame via UART
 
-        If a flow control pin has been setup, it will be controller accordingly
+        If a flow control pin has been setup, it will be controlled accordingly
 
         :param      modbus_pdu:  The modbus Protocol Data Unit
         :type       modbus_pdu:  bytes
         :param      slave_addr:  The slave address
         :type       slave_addr:  int
         """
-        serial_pdu = bytearray()
-        serial_pdu.append(slave_addr)
-        serial_pdu.extend(modbus_pdu)
-
-        crc = self._calculate_crc16(serial_pdu)
-        serial_pdu.extend(crc)
+        # modbus_adu: Modbus Application Data Unit
+        # consists of the Modbus PDU, with slave address prepended and checksum appended
+        modbus_adu = bytearray()
+        modbus_adu.append(slave_addr)
+        modbus_adu.extend(modbus_pdu)
+        modbus_adu.extend(self._calculate_crc16(modbus_adu))
 
         if self._ctrlPin:
-            self._ctrlPin(1)
-            time.sleep_us(1000)     # wait until the control pin really changed
-            send_start_time = time.ticks_us()
-
-        self._uart.write(serial_pdu)
+            self._ctrlPin.on()
+            # wait until the control pin really changed
+            # 85-95us (ESP32 @ 160/240MHz)
+            time.sleep_us(200)
+
+        # the timing of this part is critical:
+        # - if we disable output too early,
+        #   the command will not be received in full
+        # - if we disable output too late,
+        #   the incoming response will lose some data at the beginning
+        # easiest to just wait for the bytes to be sent out on the wire
+
+        send_start_time = time.ticks_us()
+        # 360-400us @ 9600-115200 baud (measured) (ESP32 @ 160/240MHz)
+        self._uart.write(modbus_adu)
+        send_finish_time = time.ticks_us()
+        if self._has_uart_flush:
+            self._uart.flush()
+        else:
+            sleep_time_us = (
+                self._t1char * len(modbus_adu) -    # total frame time in us
+                time.ticks_diff(send_finish_time, send_start_time) +
+                100     # only required at baudrates above 57600, but hey 100us
+            )
+            time.sleep_us(sleep_time_us)
 
         if self._ctrlPin:
-            total_frame_time_us = self._t1char * len(serial_pdu)
-            while time.ticks_us() <= send_start_time + total_frame_time_us:
-                machine.idle()
-            self._ctrlPin(0)
+            self._ctrlPin.off()
 
     def _send_receive(self,
                       modbus_pdu: bytes,
                       slave_addr: int,
                       count: bool) -> bytes:
         """
         Send a modbus message and receive the reponse.
@@ -275,15 +300,15 @@
         :type       slave_addr:  int
         :param      count:       The count
         :type       count:       bool
 
         :returns:   Validated response content
         :rtype:     bytes
         """
-        # flush the Rx FIFO
+        # flush the Rx FIFO buffer
         self._uart.read()
 
         self._send(modbus_pdu=modbus_pdu, slave_addr=slave_addr)
 
         return self._validate_resp_hdr(response=self._uart_read(),
                                        slave_addr=slave_addr,
                                        function_code=modbus_pdu[0],
```

### Comparing `micropython-modbus-2.3.4/umodbus/tcp.py` & `micropython-modbus-2.3.5/umodbus/tcp.py`

 * *Files identical despite different names*

### Comparing `micropython-modbus-2.3.4/umodbus/typing.py` & `micropython-modbus-2.3.5/umodbus/typing.py`

 * *Files identical despite different names*

