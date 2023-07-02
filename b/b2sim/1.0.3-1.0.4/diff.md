# Comparing `tmp/b2sim-1.0.3.tar.gz` & `tmp/b2sim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.3.tar", last modified: Sat Jul  1 20:38:37 2023, max compression
+gzip compressed data, was "b2sim-1.0.4.tar", last modified: Sun Jul  2 01:42:07 2023, max compression
```

## Comparing `b2sim-1.0.3.tar` & `b2sim-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.130669 b2sim-1.0.3/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.3/LICENSE
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.3/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-01 20:38:37.129668 b2sim-1.0.3/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10205 2023-06-30 02:57:26.000000 b2sim-1.0.3/README.md
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.097654 b2sim-1.0.3/b2sim/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.3/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     9099 2023-07-01 19:00:38.000000 b2sim-1.0.3/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8686 2023-06-28 19:52:48.000000 b2sim-1.0.3/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    97691 2023-07-01 20:11:44.000000 b2sim-1.0.3/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.3/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.106662 b2sim-1.0.3/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.3/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.3/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.104661 b2sim-1.0.3/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-01 20:38:37.131670 b2sim-1.0.3/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-01 20:38:26.000000 b2sim-1.0.3/setup.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.748640 b2sim-1.0.4/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.4/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.4/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 01:42:07.748640 b2sim-1.0.4/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10205 2023-06-30 02:57:26.000000 b2sim-1.0.4/README.md
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.718612 b2sim-1.0.4/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.4/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     9343 2023-07-02 00:15:34.000000 b2sim-1.0.4/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8686 2023-06-28 19:52:48.000000 b2sim-1.0.4/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    99065 2023-07-02 01:21:17.000000 b2sim-1.0.4/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.4/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.746638 b2sim-1.0.4/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.4/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.4/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 01:42:07.743635 b2sim-1.0.4/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-02 01:42:07.000000 b2sim-1.0.4/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-02 01:42:07.748640 b2sim-1.0.4/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-02 01:40:52.000000 b2sim-1.0.4/setup.py
```

### Comparing `b2sim-1.0.3/LICENSE` & `b2sim-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.3/README.md` & `b2sim-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.3/b2sim/actions.py` & `b2sim-1.0.4/b2sim/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,20 @@
         'Minimum Buy Time': min_buy_time,
         'Maximum Buy Time': max_buy_time,
         'Maximum Amount': max_amount,
         'Buffer': buffer,
         'Message': 'Trigger repeated supply drop buys until time %s'%(max_buy_time)
     }
 
+def sellAllSupplyDrops(min_buy_time = 0):
+    return {
+        'Type': 'Sell All Supply Drops',
+        'Minimum Buy Time': min_buy_time #Okay, this might be confusing, but this is actually the minimum *sell* time for this action.
+    }
+
 # WARNING: This function is for declaring supply drops in the initial game state. 
 # Do NOT use it to add supply drops during simulation
 def initSupplyDrops(purchase_times, elite_sniper = None):
     dictionary = {}
     for i in range(len(purchase_times)):
         dictionary[i] = purchase_times[i]
     dictionary['Elite Sniper Index'] = elite_sniper
```

### Comparing `b2sim-1.0.3/b2sim/info.py` & `b2sim-1.0.4/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.3/b2sim/main.py` & `b2sim-1.0.4/b2sim/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
             
         self.logs.append("MESSAGE FROM GameState.__init__(): ")
         self.logs.append("Initialized Game State!")
         self.logs.append("The current game round is %s"%(self.current_round))
         self.logs.append("The current game time is %s seconds"%(self.current_time))
         self.logs.append("The game round start times are given by %s \n"%(self.rounds.round_starts))
         
-    def viewCashEcoHistory(self, dim = (15,18), display_farms = True):
+    def viewCashEcoHistory(self, dim = (15,18), display_farms = True, font_size = 12):
         self.logs.append("MESSAGE FROM GameState.viewCashEcoHistory():")
         self.logs.append("Graphing history of cash and eco!")
 
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         #Graph the cash and eco values over time
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -298,16 +298,16 @@
         
         ax[0].set_ylabel("Cash")
         ax[1].set_ylabel("Eco")
         
         ax[0].set_xlabel("Time (seconds)")
         ax[1].set_xlabel("Time (seconds)")
         
-        ax[0].legend(bbox_to_anchor = (1.02, 1))
-        ax[1].legend(bbox_to_anchor = (1.02, 1))
+        ax[0].legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
+        ax[1].legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
         
         fig.tight_layout()
 
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         #Create a table that displays the revenue made by each farm
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
@@ -1029,29 +1029,30 @@
         # self.logs.append("Max Send Amount: %s"%(self.max_send_amount))
 
         while self.attack_queue_unlock_time <= target_time and self.send_name != 'Zero' and (self.max_send_amount is None or self.number_of_sends < self.max_send_amount) and (self.max_eco_amount is None or self.eco < self.max_eco_amount):
             self.current_time = max(self.attack_queue_unlock_time, self.current_time)
             # self.logs.append("Advanced current time to %s"%(self.current_time))
 
             # First, check if we can remove any items from the attack queue
-            for attack_end in self.attack_queue:
-                if self.current_time >= attack_end:
-                    self.attack_queue.remove(attack_end)
+            while len(self.attack_queue) > 0 and self.current_time >= self.attack_queue[0]:
+                self.attack_queue.pop(0)
             
             # Next, try to add an attack to the attack_queue.
             # Can we send an attack?
             if self.cash >= self.eco_cost and len(self.attack_queue) < 6:
                 # Yes, the queue is empty and we have enough cash
                 if len(self.attack_queue) == 0:
                     self.attack_queue.append(self.current_time + self.eco_time)
                 else:
                     self.attack_queue.append(self.attack_queue[-1] + self.eco_time)
                 self.cash -= self.eco_cost
                 self.eco += self.eco_gain
                 self.logs.append("Sent a set of %s at time %s"%(self.send_name, self.current_time))
+                self.logs.append("Currently, the send queue looks like this: ")
+                self.logs.append(str(self.attack_queue))
 
                 # Will the attack we send fill up the queue completely?
                 if len(self.attack_queue) == 5:
                     # Yes, The next send will cause the attack queue to fill up. Wait until the queue empties (if necessary)
                     self.attack_queue_unlock_time = max(self.current_time + self.eco_delay, self.attack_queue[0])
                 else:
                     # No, there's still space afterwards. Check again after the eco delay is up.
@@ -1142,14 +1143,21 @@
                 # FARM RELATED MATTERS
                 elif dict_obj['Type'] == 'Buy Farm':
                     h_new_cash, h_new_loan = impact(h_cash, h_loan, -1*farm_globals['Farm Cost'])
                 elif dict_obj['Type'] == 'Upgrade Farm':
                     ind = dict_obj['Index']
                     path = dict_obj['Path']
                     farm = self.farms[ind]
+                    #Do not upgrade a farm that has already been sold!
+                    if farm.sell_time is not None:
+                        self.logs.append("WARNING! Tried to upgrade a farm that was already sold! Aborting buy queue!")
+                        self.warnings.append(len(self.logs)-1)
+                        self.valid_action_flag = False
+                        break
+
                     #The following code prevents from the player from having multiple T5's in play
                     if farm.upgrades[path]+1 == 5 and self.T5_exists[path] == True:
                         self.logs.append("WARNING! Tried to purchase a T5 farm when one of the same kind already existed! Aborting buy queue!")
                         self.warnings.append(len(self.logs)-1)
                         self.valid_action_flag = False
                         break
                     h_cash, h_loan = impact(h_cash, h_loan, -1*farm_upgrades_costs[path][farm.upgrades[path]])
@@ -1170,14 +1178,20 @@
                         break
 
                 elif dict_obj['Type'] == 'Withdraw Bank':
                     #WARNING: The farm in question must actually be a bank for us to perform a withdrawal!
                     #If it isn't, break the loop prematurely
                     ind = dict_obj['Index']
                     farm = self.farms[ind]
+                    if farm.sell_time is not None:
+                        self.logs.append("WARNING! Tried to withdraw from a bank that was already sold! Aborting buy queue!")
+                        self.warnings.append(len(self.logs)-1)
+                        self.valid_action_flag = False
+                        break
+
                     if farm.upgrades[1] < 3:
                         self.logs.append("WARNING! Tried to Withdraw from a farm that is not a bank! Aborting buy queue!")
                         self.warnings.append(len(self.logs)-1)
                         self.valid_action_flag = False
                         break
                     
                     h_new_cash, h_new_loan = impact(h_cash, h_loan, farm.account_value)
@@ -1185,14 +1199,21 @@
                     farm.h_revenue += h_new_cash - h_cash
                     h_cash, h_loan = h_new_cash, h_new_loan
 
                 elif dict_obj['Type'] == 'Activate IMF':
                     #WARNING: The farm in question must actually be an IMF Loan for us to use this ability!
                     #If it isn't, set a flag to False and break the loop.
                     #DEVELOPER'S NOTE: A farm that has a min_use_time is not necessarily an IMF loan, it could also be an Monkeyopolis
+                    #Do not upgrade a farm that has already been sold!
+                    if farm.sell_time is not None:
+                        self.logs.append("WARNING! Tried to take out a loan from a bank that was already sold! Aborting buy queue!")
+                        self.warnings.append(len(self.logs)-1)
+                        self.valid_action_flag = False
+                        break
+
                     if farm.upgrades[1] != 4:
                         self.logs.append("WARNING! Tried to take out a loan from a farm that is not an IMF! Aborting buy queue!")
                         self.warnings.append(len(self.logs)-1)
                         self.valid_action_flag = False
                         break
                         
                     ind = dict_obj['Index']
@@ -1604,15 +1625,15 @@
 
 
 
 # %% [markdown]
 # The goal of a simulator like this is to compare different strategies and see which one is better. To this end, we define a function capable of simulating multiple game states at once and comparing them.
 
 # %%
-def compareStrategies(initial_state, eco_queues, buy_queues, target_time = None, target_round = 30, display_farms = True):
+def compareStrategies(initial_state, eco_queues, buy_queues, target_time = None, target_round = 30, display_farms = True, font_size = 12):
     
     # Log file in case we need to check outputs
     logs = []
     
     # Given an common initial state and N different tuples of (eco_queue, buy_queue), 
     # Build N different instances of GameState, advance them to the target_time (or target round if specified)
     # Finally, graph their cash and eco histories
@@ -1717,16 +1738,16 @@
     ax[1].set_title("Eco vs Time")
 
     ax[0].set_ylabel("Cash")
     ax[1].set_ylabel("Eco")
 
     ax[1].set_xlabel("Time (seconds)")
 
-    ax[0].legend(loc='upper left')
-    ax[1].legend(loc='upper left')
+    ax[0].legend(loc='upper left', fontsize = font_size)
+    ax[1].legend(loc='upper left', fontsize = font_size)
     
     d = {'Game State': [i for i in range(N)], 'Farm Income': [farm_incomes[i] for i in range(N)]}
     df = pd.DataFrame(data=d)
     
     fig.tight_layout()
     display(df)
     logs.append("Successfully generated graph! \n")
```

### Comparing `b2sim-1.0.3/b2sim/rounds.py` & `b2sim-1.0.4/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.3/b2sim/templates/eco_send_info.csv` & `b2sim-1.0.4/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

