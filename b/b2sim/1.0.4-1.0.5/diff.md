# Comparing `tmp/b2sim-1.0.4.tar.gz` & `tmp/b2sim-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.4.tar", last modified: Sun Jul  2 01:42:07 2023, max compression
+gzip compressed data, was "b2sim-1.0.5.tar", last modified: Sun Jul  2 13:13:59 2023, max compression
```

## Comparing `b2sim-1.0.4.tar` & `b2sim-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.748640 b2sim-1.0.4/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.4/LICENSE
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.4/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 01:42:07.748640 b2sim-1.0.4/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10205 2023-06-30 02:57:26.000000 b2sim-1.0.4/README.md
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.718612 b2sim-1.0.4/b2sim/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.4/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     9343 2023-07-02 00:15:34.000000 b2sim-1.0.4/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8686 2023-06-28 19:52:48.000000 b2sim-1.0.4/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    99065 2023-07-02 01:21:17.000000 b2sim-1.0.4/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.4/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.746638 b2sim-1.0.4/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.4/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.4/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.743635 b2sim-1.0.4/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-02 01:42:07.748640 b2sim-1.0.4/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-02 01:40:52.000000 b2sim-1.0.4/setup.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 13:13:59.652355 b2sim-1.0.5/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.5/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.5/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 13:13:59.651354 b2sim-1.0.5/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10205 2023-06-30 02:57:26.000000 b2sim-1.0.5/README.md
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 13:13:59.636340 b2sim-1.0.5/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.5/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     9346 2023-07-02 11:36:54.000000 b2sim-1.0.5/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8686 2023-06-28 19:52:48.000000 b2sim-1.0.5/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)   100949 2023-07-02 12:26:45.000000 b2sim-1.0.5/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.5/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 13:13:59.645348 b2sim-1.0.5/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.5/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.5/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 13:13:59.642346 b2sim-1.0.5/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 13:13:59.000000 b2sim-1.0.5/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-02 13:13:59.000000 b2sim-1.0.5/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-02 13:13:59.000000 b2sim-1.0.5/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-02 13:13:59.000000 b2sim-1.0.5/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-02 13:13:59.000000 b2sim-1.0.5/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-02 13:13:59.652355 b2sim-1.0.5/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-02 11:37:48.000000 b2sim-1.0.5/setup.py
```

### Comparing `b2sim-1.0.4/LICENSE` & `b2sim-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.4/README.md` & `b2sim-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.4/b2sim/actions.py` & `b2sim-1.0.5/b2sim/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         'Message': 'Trigger Jericho Steal'
     }
 
 ###########
 # ECO QUEUE
 ###########
 
-def ecoSend(time = 0, send_name = 'Zero', property = 'Normal', max_send_amount = None, max_eco_amount = None):
+def ecoSend(time = None, send_name = 'Zero', property = 'Normal', max_send_amount = None, max_eco_amount = None):
     
     fortified = False
     camo = False
     regrow = False
 
     if property == 'Fortified':
         fortified = True
```

### Comparing `b2sim-1.0.4/b2sim/info.py` & `b2sim-1.0.5/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.4/b2sim/main.py` & `b2sim-1.0.5/b2sim/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # %%
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from b2sim.info import *
+from b2sim.actions import *
 import copy
 
 # %%
 
 
 # %%
 def impact(cash, loan, amount):
@@ -386,45 +387,48 @@
 
                 #Are we under the eco threshold to use the eco send?
                 if self.eco_queue[0]['Max Eco Amount'] is not None and self.eco >= self.eco_queue[0]['Max Eco Amount']:
                     #No, do not use the eco send.
                     self.eco_queue.pop(0)
                 else:
                     #Yes, we are under the threshold. Now check if the given time for the send is a valid time..
-
-                    #Is the eco send too late?
-                    if self.eco_queue[0]['Time'] >= self.rounds.getTimeFromRound(eco_send_info[self.eco_queue[0]['Send Name']]['End Round']+1):
-                        #Yes, the send is too late. Remove it from the queue.
-                        self.logs.append("Warning! Time %s is too late to call %s. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
-                        self.eco_queue.pop(0)
-                        
+                    if self.eco_queue[0]['Time'] is None:
+                        #Bypass the time check if no time is given.
+                        break_flag = True
                     else:
-                        #No, the send is not too late
-                        
-                        #Is the eco send too early?
-                        candidate_time = self.rounds.getTimeFromRound(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round'])
-                        if self.eco_queue[0]['Time'] < candidate_time:
-                            #Yes, the send is too early
-                            self.logs.append("Warning! Time %s is too early to call %s. Adjusting the queue time to %s"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name'], candidate_time))
-                            self.eco_queue[0] = (candidate_time, self.eco_queue[0]['Send Name'])
-                            #Is the adjusted time still valid?
-                            if len(self.eco_queue) < 2 or self.eco_queue[0]['Time'] < self.eco_queue[1]['Time']:
-                                #Yes, it's still valid
+                        #Is the eco send too late?
+                        if self.eco_queue[0]['Time'] >= self.rounds.getTimeFromRound(eco_send_info[self.eco_queue[0]['Send Name']]['End Round']+1):
+                            #Yes, the send is too late. Remove it from the queue.
+                            self.logs.append("Warning! Time %s is too late to call %s. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
+                            self.eco_queue.pop(0)
+                            
+                        else:
+                            #No, the send is not too late
+                            
+                            #Is the eco send too early?
+                            candidate_time = self.rounds.getTimeFromRound(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round'])
+                            if self.eco_queue[0]['Time'] < candidate_time:
+                                #Yes, the send is too early
+                                self.logs.append("Warning! Time %s is too early to call %s. Adjusting the queue time to %s"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name'], candidate_time))
+                                self.eco_queue[0] = (candidate_time, self.eco_queue[0]['Send Name'])
+                                #Is the adjusted time still valid?
+                                if len(self.eco_queue) < 2 or self.eco_queue[0]['Time'] < self.eco_queue[1]['Time']:
+                                    #Yes, it's still valid
+                                    self.checkProperties()
+                                    break_flag = True
+                                else:
+                                    #No, it's not valid
+                                    self.logs.append("Warning! Time %s is too late to call %s because the next item in the eco queue is slated to come earlier. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
+                                    self.eco_queue.pop(0)
+                            else:
+                                #No, the send is not too early
                                 self.checkProperties()
                                 break_flag = True
-                            else:
-                                #No, it's not valid
-                                self.logs.append("Warning! Time %s is too late to call %s because the next item in the eco queue is slated to come earlier. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
-                                self.eco_queue.pop(0)
-                        else:
-                            #No, the send is not too early
-                            self.checkProperties()
-                            break_flag = True
             
-            if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] <= self.current_time:
+            if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] <= self.current_time:
                 self.changeEcoSend(self.eco_queue[0])
                 self.eco_queue.pop(0)
             else:
                 future_flag = True
         
     def changeEcoSend(self,send_info):
         # NOTE: This function does NOT contain safeguards to prevent the player from changing to unavailable eco sends.
@@ -444,14 +448,33 @@
         # Check if the given send name corresponds to a valid send. If not, default to the zero send.
         eco_send_keys = list(eco_send_info.keys())
         if eco_send_keys.count(send_info['Send Name']) == 0:
             self.logs.append("Warning! The name %s does not correspond with an eco send! Switching to the zero send."%(send_info['Send Name']))
             send_info['Send Name'] = 'Zero'
             self.warnings.append(len(self.logs) - 1)
 
+        self.current_round = self.rounds.getRoundFromTime(self.current_time)
+
+        # FAIL SAFE: Switch to the zero send instead if the send is not yet available and reinsert the eco send we wanted to change to into the queue
+        if self.current_round < eco_send_info[send_info['Send Name']]['Start Round']:
+            self.logs.append("Warning! The eco send %s is not available yet! Switching to the zero send for now, we will attempt to use this send later."%(send_info['Send Name']))
+            self.warnings.append(len(self.logs) - 1)
+            send_info['Time'] = self.rounds.getTimeFromRound(eco_send_info[send_info['Send Name']]['Start Round'])
+            self.eco_queue.insert(0,send_info)
+        
+        # FAIL SAFE: Switch to the zero send if the send is no longer available.
+        # WARNING: If this fail-safe triggers, something is probably wrong with the code.
+        if self.current_round > eco_send_info[send_info['Send Name']]['End Round']:
+            self.logs.append("Warning! The eco send %s is no longer available! Switching to the zero send."%(send_info['Send Name']))
+            self.logs.append("Warning! The above message occurred during the changeEcoSend method, which means something's probably wrong with the code!")
+            self.warnings.append(len(self.logs) - 1)
+            self.warnings.append(len(self.logs) - 2)
+            send_info['Send Name'] = 'Zero'
+
+
         # First, check if the send has any fortied, camo, or regrow characteristics
         eco_cost_multiplier = 1
         if send_info['Fortified'] == True:
             eco_cost_multiplier *= game_globals['Fortified Multiplier']
         if send_info['Camoflauge'] == True:
             eco_cost_multiplier *= game_globals['Camoflauge Multiplier']
         if send_info['Regrow'] == True:
@@ -522,15 +545,15 @@
         #PART 0: FAIL-SAFES
         ###################
 
         # If the eco queue has the player try to use eco sends when they unavailable, automatically modify the queue so this doesn't happen
         self.ecoQueueCorrection()
         
         # FAIL-SAFE: Terminate advanceGameState early if an eco change is scheduled before the target_time.
-        if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] < target_time:
+        if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] < target_time:
             #Yes, an eco change will occur
             target_time = self.eco_queue[0]['Time']
 
         # FAIL-SAFE: Check whether the current eco send is valid. If it is not, change the eco send to zero.
         if eco_send_info[self.send_name]['End Round'] < self.current_round:
             self.logs.append("Warning! The eco send %s is no longer available! Switching to the zero send."%(self.send_name))
             self.warnings.append(len(self.logs) - 1)
@@ -738,15 +761,15 @@
         self.current_time = target_time
 
         while self.rounds.round_starts[self.current_round] <= self.current_time:
             self.current_round += 1
         self.current_round -= 1
         
         #Update the eco send, if necessary
-        if len(self.eco_queue) > 0 and target_time >= self.eco_queue[0]['Time']:
+        if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] and target_time >= self.eco_queue[0]['Time']:
             self.changeEcoSend(self.eco_queue[0])
             self.eco_queue.pop(0)
         
         #self.logs.append("Advanced game state to round " + str(self.current_round))
         #self.logs.append("The current time is " + str(self.current_time))
         #self.logs.append("The next round starts at time " + str(self.rounds.round_starts[self.current_round+1]))
         #self.logs.append("Our new cash and eco is given by (%s,%s) \n"%(np.round(self.cash,2),np.round(self.eco,2)))
```

### Comparing `b2sim-1.0.4/b2sim/rounds.py` & `b2sim-1.0.5/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.4/b2sim/templates/eco_send_info.csv` & `b2sim-1.0.5/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

