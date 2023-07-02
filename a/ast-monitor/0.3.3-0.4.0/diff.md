# Comparing `tmp/ast_monitor-0.3.3.tar.gz` & `tmp/ast_monitor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast_monitor-0.3.3.tar", max compression
+gzip compressed data, was "ast_monitor-0.4.0.tar", max compression
```

## Comparing `ast_monitor-0.3.3.tar` & `ast_monitor-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     5245 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0      782 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/CITATION.cff
--rw-r--r--   0        0        0     1086 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/LICENSE
--rw-r--r--   0        0        0    11544 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/README.md
--rw-r--r--   0        0        0      698 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/ast_monitor/__init__.py
--rw-r--r--   0        0        0     3749 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/ast_monitor/basic_data.py
--rw-r--r--   0        0        0     5276 2023-06-21 19:21:55.981004 ast_monitor-0.3.3/ast_monitor/digital_twin.py
--rw-r--r--   0        0        0     2395 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/gps_sensor.py
--rw-r--r--   0        0        0     1967 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/hr_sensor.py
--rw-r--r--   0        0        0     2193 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/arrow_down.svg
--rw-r--r--   0        0        0     1980 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/arrow_left.svg
--rw-r--r--   0        0        0     1991 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/arrow_right.svg
--rw-r--r--   0        0        0     2192 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/arrow_up.svg
--rw-r--r--   0        0        0     6101 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/ascent.svg
--rw-r--r--   0        0        0     6514 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/bicycle.svg
--rw-r--r--   0        0        0     7083 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/clock.svg
--rw-r--r--   0        0        0     5676 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/distance.svg
--rw-r--r--   0        0        0     2750 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/heart.svg
--rw-r--r--   0        0        0       62 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/licence.txt
--rw-r--r--   0        0        0     2310 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/play.svg
--rw-r--r--   0        0        0     2596 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/shutdown.svg
--rw-r--r--   0        0        0     4639 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/speed.svg
--rw-r--r--   0        0        0     1858 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/icons/stop.svg
--rw-r--r--   0        0        0     5582 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/interval_training.py
--rw-r--r--   0        0        0    68335 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/mainwindow.py
--rw-r--r--   0        0        0       79 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/map/map.css
--rw-r--r--   0        0        0      441 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/map/map.html
--rw-r--r--   0        0        0      246 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/map/map.js
--rw-r--r--   0        0        0    14551 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/model.py
--rw-r--r--   0        0        0     3378 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/simulation.py
--rw-r--r--   0        0        0     1190 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/training_session.py
--rw-r--r--   0        0        0     1576 2023-06-21 19:21:55.982004 ast_monitor-0.3.3/ast_monitor/write_log.py
--rw-r--r--   0        0        0     1040 2023-06-21 19:21:55.997005 ast_monitor-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    12672 2023-06-21 19:22:03.707448 ast_monitor-0.3.3/setup.py
--rw-r--r--   0        0        0    12575 2023-06-21 19:22:03.708131 ast_monitor-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     5245 2023-07-02 20:00:41.010990 ast_monitor-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      782 2023-07-02 20:00:41.010990 ast_monitor-0.4.0/CITATION.cff
+-rw-r--r--   0        0        0     1086 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11644 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/README.md
+-rw-r--r--   0        0        0      699 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/ast_monitor/__init__.py
+-rw-r--r--   0        0        0     3749 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/ast_monitor/basic_data.py
+-rw-r--r--   0        0        0     5276 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/ast_monitor/digital_twin.py
+-rw-r--r--   0        0        0     2395 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/ast_monitor/gps_sensor.py
+-rw-r--r--   0        0        0     1967 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/ast_monitor/hr_sensor.py
+-rw-r--r--   0        0        0     2193 2023-07-02 20:00:41.011990 ast_monitor-0.4.0/ast_monitor/icons/arrow_down.svg
+-rw-r--r--   0        0        0     1980 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/arrow_left.svg
+-rw-r--r--   0        0        0     1991 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/arrow_right.svg
+-rw-r--r--   0        0        0     2192 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/arrow_up.svg
+-rw-r--r--   0        0        0     6101 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/ascent.svg
+-rw-r--r--   0        0        0     6514 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/bicycle.svg
+-rw-r--r--   0        0        0     7083 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/clock.svg
+-rw-r--r--   0        0        0     5676 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/distance.svg
+-rw-r--r--   0        0        0     2750 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/heart.svg
+-rw-r--r--   0        0        0       62 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/licence.txt
+-rw-r--r--   0        0        0     2310 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/play.svg
+-rw-r--r--   0        0        0     2596 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/shutdown.svg
+-rw-r--r--   0        0        0     4639 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/speed.svg
+-rw-r--r--   0        0        0     1858 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/icons/stop.svg
+-rw-r--r--   0        0        0     5582 2023-07-02 20:00:41.012990 ast_monitor-0.4.0/ast_monitor/interval_training.py
+-rw-r--r--   0        0        0    70675 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/mainwindow.py
+-rw-r--r--   0        0        0       79 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/map/map.css
+-rw-r--r--   0        0        0      620 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/map/map.html
+-rw-r--r--   0        0        0      246 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/map/map.js
+-rw-r--r--   0        0        0    14859 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/model.py
+-rw-r--r--   0        0        0     3378 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/simulation.py
+-rw-r--r--   0        0        0     1190 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/training_session.py
+-rw-r--r--   0        0        0     1576 2023-07-02 20:00:41.013990 ast_monitor-0.4.0/ast_monitor/write_log.py
+-rw-r--r--   0        0        0     1046 2023-07-02 20:00:41.034990 ast_monitor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12780 2023-07-02 20:00:48.014559 ast_monitor-0.4.0/setup.py
+-rw-r--r--   0        0        0    12686 2023-07-02 20:00:48.015291 ast_monitor-0.4.0/PKG-INFO
```

### Comparing `ast_monitor-0.3.3/CHANGELOG.md` & `ast_monitor-0.4.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/CITATION.cff` & `ast_monitor-0.4.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/LICENSE` & `ast_monitor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/README.md` & `ast_monitor-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Code">💻</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a> <a href="#platform-firefly-cpp" title="Packaging/porting to new platform">📦</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/luckyLukac"><img src="https://avatars.githubusercontent.com/u/73126820?v=4?s=100" width="100px;" alt="luckyLukac"/><br /><sub><b>luckyLukac</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AluckyLukac" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Code">💻</a> <a href="#design-luckyLukac" title="Design">🎨</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="#content-alenrajsp" title="Content">🖋</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="#content-alenrajsp" title="Content">🖋</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=alenrajsp" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/KukovecRok"><img src="https://avatars.githubusercontent.com/u/33880044?v=4?s=100" width="100px;" alt="Tatookie"/><br /><sub><b>Tatookie</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=KukovecRok" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AKukovecRok" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -100,11 +100,11 @@
 Fister Jr, I., Fister, I., Iglesias, A., Galvez, A., Deb, S., & Fister, D.
 (2021). On deploying the Artificial Sport Trainer into practice. arXiv preprint
 [arXiv:2109.13334](https://arxiv.org/abs/2109.13334). Fister Jr, I., Salcedo-
 Sanz, S., Iglesias, A., Fister, D., GÃ¡lvez, A., & Fister, I. (2021). New
 Perspectives in the Development of the Artificial Sport Trainer. Applied
 Sciences, 11(23), 11452. DOI: [10.3390/app112311452](https://doi.org/10.3390/
 app112311452) ## Contributors
-                        [Iztok_Fister_Jr.]                                     [luckyLukac]             [Oromion] [alenrajsp]    [Tatookie]
-                         Iztok_Fister_Jr.                                       luckyLukac               Oromion   alenrajsp      Tatookie
-               ð ð ð» ð§ ð§âð�        ð ð ð» �  ð¦   ð     ð ð
+                        [Iztok_Fister_Jr.]                                     [luckyLukac]             [Oromion]    [alenrajsp]       [Tatookie]
+                         Iztok_Fister_Jr.                                       luckyLukac               Oromion      alenrajsp         Tatookie
+               ð ð ð» ð§ ð§âð�        ð ð ð» �  ð¦    ð ð�    ð ð
```

### Comparing `ast_monitor-0.3.3/ast_monitor/__init__.py` & `ast_monitor-0.4.0/ast_monitor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from ast_monitor.mainwindow import Ui_MainWindow
 from ast_monitor.model import AST
 from ast_monitor.simulation import Simulation
 from ast_monitor.training_session import TrainingSession
 from ast_monitor.write_log import WriteLog
 
 
+
 __all__ = [
     BasicData,
     DigitalTwin,
     GpsSensor,
     HrSensor,
     IntervalTraining,
     Ui_MainWindow,
     AST,
     Simulation,
     TrainingSession,
     WriteLog
 ]
 
 __project__ = 'ast_monitor'
-__version__ = '0.3.3'
+__version__ = '0.4.0'
```

### Comparing `ast_monitor-0.3.3/ast_monitor/basic_data.py` & `ast_monitor-0.4.0/ast_monitor/basic_data.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/digital_twin.py` & `ast_monitor-0.4.0/ast_monitor/digital_twin.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/gps_sensor.py` & `ast_monitor-0.4.0/ast_monitor/gps_sensor.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/hr_sensor.py` & `ast_monitor-0.4.0/ast_monitor/hr_sensor.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/arrow_down.svg` & `ast_monitor-0.4.0/ast_monitor/icons/arrow_down.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/arrow_left.svg` & `ast_monitor-0.4.0/ast_monitor/icons/arrow_left.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/arrow_right.svg` & `ast_monitor-0.4.0/ast_monitor/icons/arrow_right.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/arrow_up.svg` & `ast_monitor-0.4.0/ast_monitor/icons/arrow_up.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/ascent.svg` & `ast_monitor-0.4.0/ast_monitor/icons/ascent.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/bicycle.svg` & `ast_monitor-0.4.0/ast_monitor/icons/bicycle.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/clock.svg` & `ast_monitor-0.4.0/ast_monitor/icons/clock.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/distance.svg` & `ast_monitor-0.4.0/ast_monitor/icons/distance.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/heart.svg` & `ast_monitor-0.4.0/ast_monitor/icons/heart.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/play.svg` & `ast_monitor-0.4.0/ast_monitor/icons/play.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/shutdown.svg` & `ast_monitor-0.4.0/ast_monitor/icons/shutdown.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/speed.svg` & `ast_monitor-0.4.0/ast_monitor/icons/speed.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/icons/stop.svg` & `ast_monitor-0.4.0/ast_monitor/icons/stop.svg`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/interval_training.py` & `ast_monitor-0.4.0/ast_monitor/interval_training.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/mainwindow.py` & `ast_monitor-0.4.0/ast_monitor/mainwindow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,404 +1,402 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file 'uis/GUI2.ui'
+# Form implementation generated from reading ui file 'uis\GUI2.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt6 UI code generator 6.4.2
 #
-# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.setEnabled(True)
         MainWindow.resize(800, 480)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(MainWindow.sizePolicy().hasHeightForWidth())
         MainWindow.setSizePolicy(sizePolicy)
         MainWindow.setMinimumSize(QtCore.QSize(800, 480))
         MainWindow.setMaximumSize(QtCore.QSize(800, 480))
         MainWindow.setStyleSheet("")
-        self.centralwidget = QtWidgets.QWidget(MainWindow)
+        self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setStyleSheet("font: \"Bahnschrift Light\";\n"
 "background-color: rgb(255, 255, 255);")
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout_24.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_24.setSpacing(0)
         self.verticalLayout_24.setObjectName("verticalLayout_24")
         self.verticalLayout_23 = QtWidgets.QVBoxLayout()
         self.verticalLayout_23.setSpacing(0)
         self.verticalLayout_23.setObjectName("verticalLayout_23")
-        self.widget = QtWidgets.QWidget(self.centralwidget)
+        self.widget = QtWidgets.QWidget(parent=self.centralwidget)
         self.widget.setStyleSheet("background-color: rgba(240, 240, 240, 1);border-bottom: 1px solid black;")
         self.widget.setObjectName("widget")
         self.horizontalLayout_9 = QtWidgets.QHBoxLayout(self.widget)
         self.horizontalLayout_9.setContentsMargins(0, 0, 0, 0)
         self.horizontalLayout_9.setSpacing(0)
         self.horizontalLayout_9.setObjectName("horizontalLayout_9")
         self.horizontalLayout_10 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_10.setContentsMargins(15, 10, -1, 10)
         self.horizontalLayout_10.setObjectName("horizontalLayout_10")
-        self.widget_title = QtWidgets.QStackedWidget(self.widget)
+        self.widget_title = QtWidgets.QStackedWidget(parent=self.widget)
         self.widget_title.setStyleSheet("border: none;")
         self.widget_title.setObjectName("widget_title")
         self.page_3 = QtWidgets.QWidget()
         self.page_3.setObjectName("page_3")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.page_3)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.lbl_page = QtWidgets.QLabel(self.page_3)
+        self.lbl_page = QtWidgets.QLabel(parent=self.page_3)
         self.lbl_page.setStyleSheet("font: 23px \"Bahnschrift SemiBold\"; border: none;")
         self.lbl_page.setObjectName("lbl_page")
         self.verticalLayout_2.addWidget(self.lbl_page)
         self.widget_title.addWidget(self.page_3)
         self.page_4 = QtWidgets.QWidget()
         self.page_4.setObjectName("page_4")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.page_4)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
-        self.lbl_page_2 = QtWidgets.QLabel(self.page_4)
+        self.lbl_page_2 = QtWidgets.QLabel(parent=self.page_4)
         self.lbl_page_2.setStyleSheet("font: 23px \"Bahnschrift SemiBold\"; border: none;")
         self.lbl_page_2.setObjectName("lbl_page_2")
         self.verticalLayout_3.addWidget(self.lbl_page_2)
         self.widget_title.addWidget(self.page_4)
         self.page_5 = QtWidgets.QWidget()
         self.page_5.setObjectName("page_5")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.page_5)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
-        self.lbl_page_3 = QtWidgets.QLabel(self.page_5)
+        self.lbl_page_3 = QtWidgets.QLabel(parent=self.page_5)
         self.lbl_page_3.setStyleSheet("font: 23px \"Bahnschrift SemiBold\"; border: none;")
         self.lbl_page_3.setObjectName("lbl_page_3")
         self.verticalLayout_4.addWidget(self.lbl_page_3)
         self.widget_title.addWidget(self.page_5)
         self.page_8 = QtWidgets.QWidget()
         self.page_8.setObjectName("page_8")
         self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.page_8)
         self.verticalLayout_10.setObjectName("verticalLayout_10")
-        self.lbl_page_4 = QtWidgets.QLabel(self.page_8)
+        self.lbl_page_4 = QtWidgets.QLabel(parent=self.page_8)
         self.lbl_page_4.setStyleSheet("font: 23px \"Bahnschrift SemiBold\"; border: none;")
         self.lbl_page_4.setObjectName("lbl_page_4")
         self.verticalLayout_10.addWidget(self.lbl_page_4)
         self.widget_title.addWidget(self.page_8)
         self.horizontalLayout_10.addWidget(self.widget_title)
         self.horizontalLayout_9.addLayout(self.horizontalLayout_10)
         self.verticalLayout_23.addWidget(self.widget)
-        self.widget_14 = QtWidgets.QWidget(self.centralwidget)
+        self.widget_14 = QtWidgets.QWidget(parent=self.centralwidget)
         self.widget_14.setMaximumSize(QtCore.QSize(1000, 500))
         self.widget_14.setObjectName("widget_14")
         self.verticalLayout_21 = QtWidgets.QVBoxLayout(self.widget_14)
         self.verticalLayout_21.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_21.setObjectName("verticalLayout_21")
         self.horizontalLayout_11 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_11.setContentsMargins(5, -1, 5, -1)
         self.horizontalLayout_11.setSpacing(0)
         self.horizontalLayout_11.setObjectName("horizontalLayout_11")
-        self.btn_move_left = QtWidgets.QPushButton(self.widget_14)
+        self.btn_move_left = QtWidgets.QPushButton(parent=self.widget_14)
         self.btn_move_left.setAutoFillBackground(False)
         self.btn_move_left.setStyleSheet("background-color: rgba(255, 255, 255, 0);")
         self.btn_move_left.setText("")
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap("../ast_monitor/icons/arrow_left.svg"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon.addPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/arrow_left.svg"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.btn_move_left.setIcon(icon)
         self.btn_move_left.setIconSize(QtCore.QSize(30, 50))
         self.btn_move_left.setCheckable(False)
         self.btn_move_left.setAutoRepeat(False)
         self.btn_move_left.setAutoExclusive(False)
         self.btn_move_left.setAutoDefault(False)
         self.btn_move_left.setDefault(False)
         self.btn_move_left.setFlat(False)
         self.btn_move_left.setObjectName("btn_move_left")
         self.horizontalLayout_11.addWidget(self.btn_move_left)
-        self.stackedWidget = QtWidgets.QStackedWidget(self.widget_14)
+        self.stackedWidget = QtWidgets.QStackedWidget(parent=self.widget_14)
         self.stackedWidget.setObjectName("stackedWidget")
         self.page_main = QtWidgets.QWidget()
         self.page_main.setObjectName("page_main")
         self.verticalLayout_12 = QtWidgets.QVBoxLayout(self.page_main)
         self.verticalLayout_12.setContentsMargins(60, 15, 60, 15)
         self.verticalLayout_12.setObjectName("verticalLayout_12")
         self.gridLayout_3 = QtWidgets.QGridLayout()
-        self.gridLayout_3.setSizeConstraint(QtWidgets.QLayout.SetDefaultConstraint)
+        self.gridLayout_3.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetDefaultConstraint)
         self.gridLayout_3.setContentsMargins(0, -1, -1, -1)
         self.gridLayout_3.setSpacing(0)
         self.gridLayout_3.setObjectName("gridLayout_3")
-        self.widget_11 = QtWidgets.QWidget(self.page_main)
+        self.widget_11 = QtWidgets.QWidget(parent=self.page_main)
         self.widget_11.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_11.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_11.setObjectName("widget_11")
         self.verticalLayout_17 = QtWidgets.QVBoxLayout(self.widget_11)
         self.verticalLayout_17.setObjectName("verticalLayout_17")
         self.horizontalLayout_16 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_16.setObjectName("horizontalLayout_16")
-        self.img_distance = QtWidgets.QLabel(self.widget_11)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.img_distance = QtWidgets.QLabel(parent=self.widget_11)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(50)
         sizePolicy.setVerticalStretch(40)
         sizePolicy.setHeightForWidth(self.img_distance.sizePolicy().hasHeightForWidth())
         self.img_distance.setSizePolicy(sizePolicy)
         self.img_distance.setMinimumSize(QtCore.QSize(45, 35))
         self.img_distance.setMaximumSize(QtCore.QSize(45, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_distance.setFont(font)
-        self.img_distance.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_distance.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_distance.setStyleSheet("border: none")
-        self.img_distance.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_distance.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_distance.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_distance.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_distance.setText("")
-        self.img_distance.setPixmap(QtGui.QPixmap("../ast_monitor/icons/distance.svg"))
+        self.img_distance.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/distance.svg"))
         self.img_distance.setScaledContents(True)
-        self.img_distance.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_distance.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_distance.setObjectName("img_distance")
         self.horizontalLayout_16.addWidget(self.img_distance)
         self.verticalLayout_17.addLayout(self.horizontalLayout_16)
-        self.lbl_distance = QtWidgets.QLabel(self.widget_11)
+        self.lbl_distance = QtWidgets.QLabel(parent=self.widget_11)
         self.lbl_distance.setMaximumSize(QtCore.QSize(800, 480))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_distance.setFont(font)
         self.lbl_distance.setStyleSheet("border: 0px;")
-        self.lbl_distance.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_distance.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_distance.setObjectName("lbl_distance")
         self.verticalLayout_17.addWidget(self.lbl_distance)
         self.gridLayout_3.addWidget(self.widget_11, 0, 0, 1, 1)
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.gridLayout_3.addItem(spacerItem, 2, 0, 1, 1)
         self.horizontalLayout_12 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_12.setObjectName("horizontalLayout_12")
-        self.widget_8 = QtWidgets.QWidget(self.page_main)
+        self.widget_8 = QtWidgets.QWidget(parent=self.page_main)
         self.widget_8.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_8.setMaximumSize(QtCore.QSize(177, 16777215))
         self.widget_8.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_8.setObjectName("widget_8")
         self.verticalLayout_14 = QtWidgets.QVBoxLayout(self.widget_8)
         self.verticalLayout_14.setObjectName("verticalLayout_14")
         self.horizontalLayout_13 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_13.setObjectName("horizontalLayout_13")
-        self.img_speed = QtWidgets.QLabel(self.widget_8)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.img_speed = QtWidgets.QLabel(parent=self.widget_8)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(40)
         sizePolicy.setHeightForWidth(self.img_speed.sizePolicy().hasHeightForWidth())
         self.img_speed.setSizePolicy(sizePolicy)
         self.img_speed.setMinimumSize(QtCore.QSize(45, 35))
         self.img_speed.setMaximumSize(QtCore.QSize(45, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_speed.setFont(font)
-        self.img_speed.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_speed.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_speed.setStyleSheet("border: none")
-        self.img_speed.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_speed.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_speed.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_speed.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_speed.setText("")
-        self.img_speed.setPixmap(QtGui.QPixmap("../ast_monitor/icons/speed.svg"))
+        self.img_speed.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/speed.svg"))
         self.img_speed.setScaledContents(True)
-        self.img_speed.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_speed.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_speed.setObjectName("img_speed")
         self.horizontalLayout_13.addWidget(self.img_speed)
         self.verticalLayout_14.addLayout(self.horizontalLayout_13)
-        self.lbl_speed = QtWidgets.QLabel(self.widget_8)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        self.lbl_speed = QtWidgets.QLabel(parent=self.widget_8)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.lbl_speed.sizePolicy().hasHeightForWidth())
         self.lbl_speed.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_speed.setFont(font)
         self.lbl_speed.setStyleSheet("border:none")
-        self.lbl_speed.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_speed.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_speed.setObjectName("lbl_speed")
         self.verticalLayout_14.addWidget(self.lbl_speed)
         self.horizontalLayout_12.addWidget(self.widget_8)
         self.gridLayout_3.addLayout(self.horizontalLayout_12, 2, 1, 1, 1)
-        spacerItem1 = QtWidgets.QSpacerItem(500, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
+        spacerItem1 = QtWidgets.QSpacerItem(500, 20, QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout_3.addItem(spacerItem1, 0, 1, 1, 1)
-        self.widget_12 = QtWidgets.QWidget(self.page_main)
+        self.widget_12 = QtWidgets.QWidget(parent=self.page_main)
         self.widget_12.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_12.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_12.setObjectName("widget_12")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.widget_12)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.horizontalLayout_17 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_17.setObjectName("horizontalLayout_17")
-        self.img_heart = QtWidgets.QLabel(self.widget_12)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.img_heart = QtWidgets.QLabel(parent=self.widget_12)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(35)
         sizePolicy.setHeightForWidth(self.img_heart.sizePolicy().hasHeightForWidth())
         self.img_heart.setSizePolicy(sizePolicy)
         self.img_heart.setMinimumSize(QtCore.QSize(40, 35))
         self.img_heart.setMaximumSize(QtCore.QSize(40, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_heart.setFont(font)
-        self.img_heart.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_heart.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_heart.setStyleSheet("border: none;")
-        self.img_heart.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_heart.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_heart.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_heart.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_heart.setText("")
-        self.img_heart.setPixmap(QtGui.QPixmap("../ast_monitor/icons/heart.svg"))
+        self.img_heart.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/heart.svg"))
         self.img_heart.setScaledContents(True)
-        self.img_heart.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_heart.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_heart.setObjectName("img_heart")
         self.horizontalLayout_17.addWidget(self.img_heart)
         self.verticalLayout_18.addLayout(self.horizontalLayout_17)
-        self.lbl_heart_rate = QtWidgets.QLabel(self.widget_12)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.lbl_heart_rate = QtWidgets.QLabel(parent=self.widget_12)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(48)
         sizePolicy.setVerticalStretch(33)
         sizePolicy.setHeightForWidth(self.lbl_heart_rate.sizePolicy().hasHeightForWidth())
         self.lbl_heart_rate.setSizePolicy(sizePolicy)
         self.lbl_heart_rate.setMinimumSize(QtCore.QSize(48, 33))
         self.lbl_heart_rate.setMaximumSize(QtCore.QSize(500, 33))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_heart_rate.setFont(font)
         self.lbl_heart_rate.setStyleSheet("border:none")
-        self.lbl_heart_rate.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_heart_rate.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_heart_rate.setObjectName("lbl_heart_rate")
-        self.verticalLayout_18.addWidget(self.lbl_heart_rate, 0, QtCore.Qt.AlignHCenter)
+        self.verticalLayout_18.addWidget(self.lbl_heart_rate, 0, QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.gridLayout_3.addWidget(self.widget_12, 4, 0, 1, 1)
-        self.widget_9 = QtWidgets.QWidget(self.page_main)
+        self.widget_9 = QtWidgets.QWidget(parent=self.page_main)
         self.widget_9.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_9.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_9.setObjectName("widget_9")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.widget_9)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.horizontalLayout_14 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_14.setObjectName("horizontalLayout_14")
-        self.img_ascent = QtWidgets.QLabel(self.widget_9)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.img_ascent = QtWidgets.QLabel(parent=self.widget_9)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(40)
         sizePolicy.setHeightForWidth(self.img_ascent.sizePolicy().hasHeightForWidth())
         self.img_ascent.setSizePolicy(sizePolicy)
         self.img_ascent.setMinimumSize(QtCore.QSize(65, 35))
         self.img_ascent.setMaximumSize(QtCore.QSize(65, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_ascent.setFont(font)
-        self.img_ascent.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_ascent.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_ascent.setStyleSheet("border: none")
-        self.img_ascent.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_ascent.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_ascent.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_ascent.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_ascent.setText("")
-        self.img_ascent.setPixmap(QtGui.QPixmap("../ast_monitor/icons/ascent.svg"))
+        self.img_ascent.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/ascent.svg"))
         self.img_ascent.setScaledContents(True)
-        self.img_ascent.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_ascent.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_ascent.setObjectName("img_ascent")
         self.horizontalLayout_14.addWidget(self.img_ascent)
         self.verticalLayout_6.addLayout(self.horizontalLayout_14)
-        self.lbl_ascent = QtWidgets.QLabel(self.widget_9)
+        self.lbl_ascent = QtWidgets.QLabel(parent=self.widget_9)
         self.lbl_ascent.setMaximumSize(QtCore.QSize(16777215, 50))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_ascent.setFont(font)
         self.lbl_ascent.setStyleSheet("border: none;")
-        self.lbl_ascent.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_ascent.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_ascent.setObjectName("lbl_ascent")
         self.verticalLayout_6.addWidget(self.lbl_ascent)
         self.gridLayout_3.addWidget(self.widget_9, 4, 2, 1, 1)
-        self.widget_10 = QtWidgets.QWidget(self.page_main)
+        self.widget_10 = QtWidgets.QWidget(parent=self.page_main)
         self.widget_10.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_10.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_10.setObjectName("widget_10")
         self.verticalLayout_16 = QtWidgets.QVBoxLayout(self.widget_10)
         self.verticalLayout_16.setObjectName("verticalLayout_16")
         self.horizontalLayout_15 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_15.setObjectName("horizontalLayout_15")
-        self.img_clock = QtWidgets.QLabel(self.widget_10)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.img_clock = QtWidgets.QLabel(parent=self.widget_10)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(40)
         sizePolicy.setHeightForWidth(self.img_clock.sizePolicy().hasHeightForWidth())
         self.img_clock.setSizePolicy(sizePolicy)
         self.img_clock.setMinimumSize(QtCore.QSize(30, 35))
         self.img_clock.setMaximumSize(QtCore.QSize(30, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_clock.setFont(font)
-        self.img_clock.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_clock.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_clock.setStyleSheet("border: none")
-        self.img_clock.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_clock.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_clock.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_clock.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_clock.setText("")
-        self.img_clock.setPixmap(QtGui.QPixmap("../ast_monitor/icons/clock.svg"))
+        self.img_clock.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/clock.svg"))
         self.img_clock.setScaledContents(True)
-        self.img_clock.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_clock.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_clock.setObjectName("img_clock")
         self.horizontalLayout_15.addWidget(self.img_clock)
         self.verticalLayout_16.addLayout(self.horizontalLayout_15)
-        self.widget_2 = QtWidgets.QWidget(self.widget_10)
+        self.widget_2 = QtWidgets.QWidget(parent=self.widget_10)
         self.widget_2.setStyleSheet("border:none")
         self.widget_2.setObjectName("widget_2")
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout(self.widget_2)
         self.horizontalLayout_2.setContentsMargins(0, 0, 0, 0)
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        self.lbl_watch = QtWidgets.QLabel(self.widget_2)
+        self.lbl_watch = QtWidgets.QLabel(parent=self.widget_2)
         self.lbl_watch.setMinimumSize(QtCore.QSize(120, 30))
         self.lbl_watch.setMaximumSize(QtCore.QSize(150, 16777215))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_watch.setFont(font)
         self.lbl_watch.setStyleSheet("")
-        self.lbl_watch.setTextFormat(QtCore.Qt.AutoText)
-        self.lbl_watch.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_watch.setTextFormat(QtCore.Qt.TextFormat.AutoText)
+        self.lbl_watch.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_watch.setObjectName("lbl_watch")
         self.horizontalLayout_2.addWidget(self.lbl_watch)
         self.verticalLayout_16.addWidget(self.widget_2)
         self.gridLayout_3.addWidget(self.widget_10, 0, 2, 1, 1)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.gridLayout_3.addItem(spacerItem2, 1, 0, 1, 1)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.gridLayout_3.addItem(spacerItem3, 3, 0, 1, 1)
         self.verticalLayout_12.addLayout(self.gridLayout_3)
         self.stackedWidget.addWidget(self.page_main)
         self.page_map = QtWidgets.QWidget()
         self.page_map.setStyleSheet("")
         self.page_map.setObjectName("page_map")
         self.verticalLayout_19 = QtWidgets.QVBoxLayout(self.page_map)
         self.verticalLayout_19.setContentsMargins(9, 1, 9, 1)
         self.verticalLayout_19.setObjectName("verticalLayout_19")
-        self.widget_13 = QtWidgets.QWidget(self.page_map)
+        self.widget_13 = QtWidgets.QWidget(parent=self.page_map)
         self.widget_13.setStyleSheet("border: 1px solid black;")
         self.widget_13.setObjectName("widget_13")
         self.verticalLayout_20 = QtWidgets.QVBoxLayout(self.widget_13)
         self.verticalLayout_20.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_20.setObjectName("verticalLayout_20")
         self.vb_map = QtWidgets.QVBoxLayout()
         self.vb_map.setContentsMargins(1, 1, 1, 1)
@@ -411,224 +409,224 @@
         self.page_interval.setObjectName("page_interval")
         self.horizontalLayout_22 = QtWidgets.QHBoxLayout(self.page_interval)
         self.horizontalLayout_22.setContentsMargins(60, 15, 60, 15)
         self.horizontalLayout_22.setObjectName("horizontalLayout_22")
         self.gridLayout = QtWidgets.QGridLayout()
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.widget_18 = QtWidgets.QWidget(self.page_interval)
+        self.widget_18 = QtWidgets.QWidget(parent=self.page_interval)
         self.widget_18.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_18.setMaximumSize(QtCore.QSize(177, 100))
         self.widget_18.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_18.setObjectName("widget_18")
         self.verticalLayout_27 = QtWidgets.QVBoxLayout(self.widget_18)
         self.verticalLayout_27.setObjectName("verticalLayout_27")
         self.horizontalLayout_20 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_20.setContentsMargins(-1, 0, -1, -1)
         self.horizontalLayout_20.setObjectName("horizontalLayout_20")
-        self.widget_4 = QtWidgets.QWidget(self.widget_18)
+        self.widget_4 = QtWidgets.QWidget(parent=self.widget_18)
         self.widget_4.setMaximumSize(QtCore.QSize(40, 35))
         self.widget_4.setStyleSheet("border:none;")
         self.widget_4.setObjectName("widget_4")
-        self.img_heart_3 = QtWidgets.QLabel(self.widget_4)
+        self.img_heart_3 = QtWidgets.QLabel(parent=self.widget_4)
         self.img_heart_3.setGeometry(QtCore.QRect(0, 0, 40, 35))
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(35)
         sizePolicy.setHeightForWidth(self.img_heart_3.sizePolicy().hasHeightForWidth())
         self.img_heart_3.setSizePolicy(sizePolicy)
         self.img_heart_3.setMinimumSize(QtCore.QSize(40, 35))
         self.img_heart_3.setMaximumSize(QtCore.QSize(40, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_heart_3.setFont(font)
-        self.img_heart_3.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_heart_3.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_heart_3.setStyleSheet("border: none;")
-        self.img_heart_3.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_heart_3.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_heart_3.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_heart_3.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_heart_3.setText("")
-        self.img_heart_3.setTextFormat(QtCore.Qt.PlainText)
-        self.img_heart_3.setPixmap(QtGui.QPixmap("../ast_monitor/icons/heart.svg"))
+        self.img_heart_3.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.img_heart_3.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/heart.svg"))
         self.img_heart_3.setScaledContents(True)
-        self.img_heart_3.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_heart_3.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_heart_3.setObjectName("img_heart_3")
-        self.label_2 = QtWidgets.QLabel(self.widget_4)
+        self.label_2 = QtWidgets.QLabel(parent=self.widget_4)
         self.label_2.setGeometry(QtCore.QRect(0, 0, 41, 31))
         self.label_2.setStyleSheet("font: 14px \"Bahnschrift\"; border: none; background-color: rgba(0,0,0,0); color: white;")
-        self.label_2.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_2.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_2.setObjectName("label_2")
         self.horizontalLayout_20.addWidget(self.widget_4)
         self.verticalLayout_27.addLayout(self.horizontalLayout_20)
         self.horizontalLayout_8 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_8.setContentsMargins(-1, -1, -1, 5)
         self.horizontalLayout_8.setObjectName("horizontalLayout_8")
-        self.lbl_interval_average_heart_rate = QtWidgets.QLabel(self.widget_18)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.lbl_interval_average_heart_rate = QtWidgets.QLabel(parent=self.widget_18)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(48)
         sizePolicy.setVerticalStretch(33)
         sizePolicy.setHeightForWidth(self.lbl_interval_average_heart_rate.sizePolicy().hasHeightForWidth())
         self.lbl_interval_average_heart_rate.setSizePolicy(sizePolicy)
         self.lbl_interval_average_heart_rate.setMinimumSize(QtCore.QSize(120, 10))
         self.lbl_interval_average_heart_rate.setMaximumSize(QtCore.QSize(120, 30))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_average_heart_rate.setFont(font)
         self.lbl_interval_average_heart_rate.setStyleSheet("border:none")
-        self.lbl_interval_average_heart_rate.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_average_heart_rate.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_average_heart_rate.setObjectName("lbl_interval_average_heart_rate")
         self.horizontalLayout_8.addWidget(self.lbl_interval_average_heart_rate)
         self.verticalLayout_27.addLayout(self.horizontalLayout_8)
         self.gridLayout.addWidget(self.widget_18, 2, 0, 1, 1)
-        self.widget_19 = QtWidgets.QWidget(self.page_interval)
+        self.widget_19 = QtWidgets.QWidget(parent=self.page_interval)
         self.widget_19.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_19.setMaximumSize(QtCore.QSize(177, 100))
         self.widget_19.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_19.setObjectName("widget_19")
         self.verticalLayout_28 = QtWidgets.QVBoxLayout(self.widget_19)
         self.verticalLayout_28.setObjectName("verticalLayout_28")
         self.horizontalLayout_21 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_21.setContentsMargins(-1, 0, -1, -1)
         self.horizontalLayout_21.setObjectName("horizontalLayout_21")
-        self.widget_6 = QtWidgets.QWidget(self.widget_19)
+        self.widget_6 = QtWidgets.QWidget(parent=self.widget_19)
         self.widget_6.setMaximumSize(QtCore.QSize(40, 35))
         self.widget_6.setStyleSheet("border:none;")
         self.widget_6.setObjectName("widget_6")
-        self.img_heart_4 = QtWidgets.QLabel(self.widget_6)
+        self.img_heart_4 = QtWidgets.QLabel(parent=self.widget_6)
         self.img_heart_4.setGeometry(QtCore.QRect(0, 0, 40, 35))
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(35)
         sizePolicy.setHeightForWidth(self.img_heart_4.sizePolicy().hasHeightForWidth())
         self.img_heart_4.setSizePolicy(sizePolicy)
         self.img_heart_4.setMinimumSize(QtCore.QSize(40, 35))
         self.img_heart_4.setMaximumSize(QtCore.QSize(40, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_heart_4.setFont(font)
-        self.img_heart_4.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_heart_4.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_heart_4.setStyleSheet("border: none;")
-        self.img_heart_4.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_heart_4.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_heart_4.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_heart_4.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_heart_4.setText("")
-        self.img_heart_4.setTextFormat(QtCore.Qt.PlainText)
-        self.img_heart_4.setPixmap(QtGui.QPixmap("../ast_monitor/icons/heart.svg"))
+        self.img_heart_4.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.img_heart_4.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/heart.svg"))
         self.img_heart_4.setScaledContents(True)
-        self.img_heart_4.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_heart_4.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_heart_4.setObjectName("img_heart_4")
-        self.label_3 = QtWidgets.QLabel(self.widget_6)
+        self.label_3 = QtWidgets.QLabel(parent=self.widget_6)
         self.label_3.setGeometry(QtCore.QRect(0, 0, 41, 31))
         self.label_3.setStyleSheet("font: 14px \"Bahnschrift\"; border: none; background-color: rgba(0,0,0,0); color: white;")
-        self.label_3.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_3.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_3.setObjectName("label_3")
         self.horizontalLayout_21.addWidget(self.widget_6)
         self.verticalLayout_28.addLayout(self.horizontalLayout_21)
         self.horizontalLayout_23 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_23.setContentsMargins(-1, -1, -1, 5)
         self.horizontalLayout_23.setObjectName("horizontalLayout_23")
-        self.lbl_interval_proposed_heart_rate = QtWidgets.QLabel(self.widget_19)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.lbl_interval_proposed_heart_rate = QtWidgets.QLabel(parent=self.widget_19)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(48)
         sizePolicy.setVerticalStretch(33)
         sizePolicy.setHeightForWidth(self.lbl_interval_proposed_heart_rate.sizePolicy().hasHeightForWidth())
         self.lbl_interval_proposed_heart_rate.setSizePolicy(sizePolicy)
         self.lbl_interval_proposed_heart_rate.setMinimumSize(QtCore.QSize(120, 10))
         self.lbl_interval_proposed_heart_rate.setMaximumSize(QtCore.QSize(120, 30))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_proposed_heart_rate.setFont(font)
         self.lbl_interval_proposed_heart_rate.setStyleSheet("border:none")
-        self.lbl_interval_proposed_heart_rate.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_proposed_heart_rate.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_proposed_heart_rate.setObjectName("lbl_interval_proposed_heart_rate")
         self.horizontalLayout_23.addWidget(self.lbl_interval_proposed_heart_rate)
         self.verticalLayout_28.addLayout(self.horizontalLayout_23)
         self.gridLayout.addWidget(self.widget_19, 2, 2, 1, 1)
         self.horizontalLayout_27 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_27.setObjectName("horizontalLayout_27")
-        self.widget_20 = QtWidgets.QWidget(self.page_interval)
+        self.widget_20 = QtWidgets.QWidget(parent=self.page_interval)
         self.widget_20.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_20.setMaximumSize(QtCore.QSize(177, 100))
         self.widget_20.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_20.setObjectName("widget_20")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.widget_20)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.verticalLayout_13 = QtWidgets.QVBoxLayout()
         self.verticalLayout_13.setContentsMargins(-1, -1, -1, 5)
         self.verticalLayout_13.setObjectName("verticalLayout_13")
-        self.swgt_interval_performance = QtWidgets.QStackedWidget(self.widget_20)
+        self.swgt_interval_performance = QtWidgets.QStackedWidget(parent=self.widget_20)
         self.swgt_interval_performance.setStyleSheet("border: none;")
         self.swgt_interval_performance.setObjectName("swgt_interval_performance")
         self.page_11 = QtWidgets.QWidget()
         self.page_11.setObjectName("page_11")
         self.horizontalLayout_26 = QtWidgets.QHBoxLayout(self.page_11)
         self.horizontalLayout_26.setObjectName("horizontalLayout_26")
-        self.lbl_interval_performance = QtWidgets.QLabel(self.page_11)
+        self.lbl_interval_performance = QtWidgets.QLabel(parent=self.page_11)
         self.lbl_interval_performance.setMinimumSize(QtCore.QSize(0, 63))
         self.lbl_interval_performance.setMaximumSize(QtCore.QSize(200, 120))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift SemiLight")
         font.setPointSize(17)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_performance.setFont(font)
         self.lbl_interval_performance.setStyleSheet("border:none;")
-        self.lbl_interval_performance.setTextFormat(QtCore.Qt.AutoText)
-        self.lbl_interval_performance.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_performance.setTextFormat(QtCore.Qt.TextFormat.AutoText)
+        self.lbl_interval_performance.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_performance.setObjectName("lbl_interval_performance")
         self.horizontalLayout_26.addWidget(self.lbl_interval_performance)
         self.swgt_interval_performance.addWidget(self.page_11)
         self.page_6 = QtWidgets.QWidget()
         self.page_6.setObjectName("page_6")
         self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.page_6)
         self.verticalLayout_9.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_9.setSpacing(0)
         self.verticalLayout_9.setObjectName("verticalLayout_9")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout()
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.horizontalLayout_25 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_25.setSpacing(0)
         self.horizontalLayout_25.setObjectName("horizontalLayout_25")
-        self.lbl_interval_arrow_up = QtWidgets.QLabel(self.page_6)
+        self.lbl_interval_arrow_up = QtWidgets.QLabel(parent=self.page_6)
         self.lbl_interval_arrow_up.setMinimumSize(QtCore.QSize(0, 0))
         self.lbl_interval_arrow_up.setMaximumSize(QtCore.QSize(80, 80))
         self.lbl_interval_arrow_up.setSizeIncrement(QtCore.QSize(0, 0))
         self.lbl_interval_arrow_up.setText("")
-        self.lbl_interval_arrow_up.setPixmap(QtGui.QPixmap("../ast_monitor/icons/arrow_up.svg"))
+        self.lbl_interval_arrow_up.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/arrow_up.svg"))
         self.lbl_interval_arrow_up.setScaledContents(False)
-        self.lbl_interval_arrow_up.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_arrow_up.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_arrow_up.setObjectName("lbl_interval_arrow_up")
         self.horizontalLayout_25.addWidget(self.lbl_interval_arrow_up)
         self.verticalLayout_7.addLayout(self.horizontalLayout_25)
         self.horizontalLayout_28 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_28.setObjectName("horizontalLayout_28")
-        self.lbl_interval_performance_up = QtWidgets.QLabel(self.page_6)
+        self.lbl_interval_performance_up = QtWidgets.QLabel(parent=self.page_6)
         self.lbl_interval_performance_up.setMinimumSize(QtCore.QSize(0, 20))
         self.lbl_interval_performance_up.setMaximumSize(QtCore.QSize(150, 120))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_performance_up.setFont(font)
         self.lbl_interval_performance_up.setStyleSheet("border:none;")
-        self.lbl_interval_performance_up.setTextFormat(QtCore.Qt.AutoText)
-        self.lbl_interval_performance_up.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_performance_up.setTextFormat(QtCore.Qt.TextFormat.AutoText)
+        self.lbl_interval_performance_up.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_performance_up.setObjectName("lbl_interval_performance_up")
         self.horizontalLayout_28.addWidget(self.lbl_interval_performance_up)
         self.verticalLayout_7.addLayout(self.horizontalLayout_28)
         self.verticalLayout_9.addLayout(self.verticalLayout_7)
         self.swgt_interval_performance.addWidget(self.page_6)
         self.page_7 = QtWidgets.QWidget()
         self.page_7.setObjectName("page_7")
@@ -636,464 +634,464 @@
         self.horizontalLayout_24.setContentsMargins(0, 0, 0, 0)
         self.horizontalLayout_24.setObjectName("horizontalLayout_24")
         self.verticalLayout_29 = QtWidgets.QVBoxLayout()
         self.verticalLayout_29.setObjectName("verticalLayout_29")
         self.horizontalLayout_29 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_29.setSpacing(0)
         self.horizontalLayout_29.setObjectName("horizontalLayout_29")
-        self.label_5 = QtWidgets.QLabel(self.page_7)
+        self.label_5 = QtWidgets.QLabel(parent=self.page_7)
         self.label_5.setMinimumSize(QtCore.QSize(0, 0))
         self.label_5.setMaximumSize(QtCore.QSize(80, 80))
         self.label_5.setSizeIncrement(QtCore.QSize(0, 0))
         self.label_5.setText("")
-        self.label_5.setPixmap(QtGui.QPixmap("../ast_monitor/icons/arrow_down.svg"))
+        self.label_5.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/arrow_down.svg"))
         self.label_5.setScaledContents(False)
-        self.label_5.setAlignment(QtCore.Qt.AlignCenter)
+        self.label_5.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_5.setObjectName("label_5")
         self.horizontalLayout_29.addWidget(self.label_5)
         self.verticalLayout_29.addLayout(self.horizontalLayout_29)
         self.horizontalLayout_30 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_30.setObjectName("horizontalLayout_30")
-        self.lbl_interval_performance_down = QtWidgets.QLabel(self.page_7)
+        self.lbl_interval_performance_down = QtWidgets.QLabel(parent=self.page_7)
         self.lbl_interval_performance_down.setMinimumSize(QtCore.QSize(0, 20))
         self.lbl_interval_performance_down.setMaximumSize(QtCore.QSize(150, 120))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_performance_down.setFont(font)
         self.lbl_interval_performance_down.setStyleSheet("border:none;")
-        self.lbl_interval_performance_down.setTextFormat(QtCore.Qt.AutoText)
-        self.lbl_interval_performance_down.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_performance_down.setTextFormat(QtCore.Qt.TextFormat.AutoText)
+        self.lbl_interval_performance_down.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_performance_down.setObjectName("lbl_interval_performance_down")
         self.horizontalLayout_30.addWidget(self.lbl_interval_performance_down)
         self.verticalLayout_29.addLayout(self.horizontalLayout_30)
         self.horizontalLayout_24.addLayout(self.verticalLayout_29)
         self.swgt_interval_performance.addWidget(self.page_7)
         self.verticalLayout_13.addWidget(self.swgt_interval_performance)
         self.verticalLayout_5.addLayout(self.verticalLayout_13)
         self.horizontalLayout_27.addWidget(self.widget_20)
         self.gridLayout.addLayout(self.horizontalLayout_27, 1, 1, 1, 1)
-        self.widget_17 = QtWidgets.QWidget(self.page_interval)
+        self.widget_17 = QtWidgets.QWidget(parent=self.page_interval)
         self.widget_17.setMinimumSize(QtCore.QSize(170, 100))
         self.widget_17.setMaximumSize(QtCore.QSize(170, 100))
         self.widget_17.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_17.setObjectName("widget_17")
         self.verticalLayout_26 = QtWidgets.QVBoxLayout(self.widget_17)
         self.verticalLayout_26.setObjectName("verticalLayout_26")
         self.horizontalLayout_19 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_19.setContentsMargins(-1, 0, -1, -1)
         self.horizontalLayout_19.setObjectName("horizontalLayout_19")
-        self.widget_3 = QtWidgets.QWidget(self.widget_17)
+        self.widget_3 = QtWidgets.QWidget(parent=self.widget_17)
         self.widget_3.setMaximumSize(QtCore.QSize(40, 35))
         self.widget_3.setStyleSheet("border:none;")
         self.widget_3.setObjectName("widget_3")
-        self.img_heart_2 = QtWidgets.QLabel(self.widget_3)
+        self.img_heart_2 = QtWidgets.QLabel(parent=self.widget_3)
         self.img_heart_2.setGeometry(QtCore.QRect(0, 0, 40, 35))
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(35)
         sizePolicy.setHeightForWidth(self.img_heart_2.sizePolicy().hasHeightForWidth())
         self.img_heart_2.setSizePolicy(sizePolicy)
         self.img_heart_2.setMinimumSize(QtCore.QSize(40, 35))
         self.img_heart_2.setMaximumSize(QtCore.QSize(40, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_heart_2.setFont(font)
-        self.img_heart_2.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_heart_2.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_heart_2.setStyleSheet("border: none;")
-        self.img_heart_2.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_heart_2.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_heart_2.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_heart_2.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_heart_2.setText("")
-        self.img_heart_2.setTextFormat(QtCore.Qt.PlainText)
-        self.img_heart_2.setPixmap(QtGui.QPixmap("../ast_monitor/icons/heart.svg"))
+        self.img_heart_2.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.img_heart_2.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/heart.svg"))
         self.img_heart_2.setScaledContents(True)
-        self.img_heart_2.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_heart_2.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_heart_2.setObjectName("img_heart_2")
-        self.label = QtWidgets.QLabel(self.widget_3)
+        self.label = QtWidgets.QLabel(parent=self.widget_3)
         self.label.setGeometry(QtCore.QRect(0, 0, 41, 31))
         self.label.setStyleSheet("font: 14px \"Bahnschrift\"; border: none; background-color: rgba(0,0,0,0); color: white;")
-        self.label.setAlignment(QtCore.Qt.AlignCenter)
+        self.label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label.setObjectName("label")
         self.horizontalLayout_19.addWidget(self.widget_3)
         self.verticalLayout_26.addLayout(self.horizontalLayout_19)
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_6.setContentsMargins(-1, -1, -1, 5)
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
-        self.lbl_interval_heart_rate = QtWidgets.QLabel(self.widget_17)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.lbl_interval_heart_rate = QtWidgets.QLabel(parent=self.widget_17)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(48)
         sizePolicy.setVerticalStretch(33)
         sizePolicy.setHeightForWidth(self.lbl_interval_heart_rate.sizePolicy().hasHeightForWidth())
         self.lbl_interval_heart_rate.setSizePolicy(sizePolicy)
         self.lbl_interval_heart_rate.setMinimumSize(QtCore.QSize(120, 10))
         self.lbl_interval_heart_rate.setMaximumSize(QtCore.QSize(120, 30))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_heart_rate.setFont(font)
         self.lbl_interval_heart_rate.setStyleSheet("border:none")
-        self.lbl_interval_heart_rate.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_heart_rate.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_heart_rate.setObjectName("lbl_interval_heart_rate")
         self.horizontalLayout_6.addWidget(self.lbl_interval_heart_rate)
         self.verticalLayout_26.addLayout(self.horizontalLayout_6)
         self.gridLayout.addWidget(self.widget_17, 0, 2, 1, 1)
-        self.widget_16 = QtWidgets.QWidget(self.page_interval)
+        self.widget_16 = QtWidgets.QWidget(parent=self.page_interval)
         self.widget_16.setMinimumSize(QtCore.QSize(177, 100))
         self.widget_16.setMaximumSize(QtCore.QSize(177, 100))
         self.widget_16.setStyleSheet("background-color: rgb(248, 248, 248);\n"
 "border: 2px solid black;\n"
 "border-radius: 5px;")
         self.widget_16.setObjectName("widget_16")
         self.verticalLayout_25 = QtWidgets.QVBoxLayout(self.widget_16)
         self.verticalLayout_25.setObjectName("verticalLayout_25")
         self.horizontalLayout_18 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_18.setContentsMargins(-1, 5, -1, -1)
         self.horizontalLayout_18.setObjectName("horizontalLayout_18")
-        self.img_clock_2 = QtWidgets.QLabel(self.widget_16)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.img_clock_2 = QtWidgets.QLabel(parent=self.widget_16)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(40)
         sizePolicy.setVerticalStretch(40)
         sizePolicy.setHeightForWidth(self.img_clock_2.sizePolicy().hasHeightForWidth())
         self.img_clock_2.setSizePolicy(sizePolicy)
         self.img_clock_2.setMinimumSize(QtCore.QSize(30, 35))
         self.img_clock_2.setMaximumSize(QtCore.QSize(30, 35))
         font = QtGui.QFont()
         font.setBold(False)
         font.setItalic(False)
         self.img_clock_2.setFont(font)
-        self.img_clock_2.setLayoutDirection(QtCore.Qt.LeftToRight)
+        self.img_clock_2.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
         self.img_clock_2.setStyleSheet("border: none;")
-        self.img_clock_2.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.img_clock_2.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.img_clock_2.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.img_clock_2.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.img_clock_2.setText("")
-        self.img_clock_2.setPixmap(QtGui.QPixmap("../ast_monitor/icons/clock.svg"))
+        self.img_clock_2.setPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/clock.svg"))
         self.img_clock_2.setScaledContents(True)
-        self.img_clock_2.setAlignment(QtCore.Qt.AlignCenter)
+        self.img_clock_2.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.img_clock_2.setObjectName("img_clock_2")
         self.horizontalLayout_18.addWidget(self.img_clock_2)
         self.verticalLayout_25.addLayout(self.horizontalLayout_18)
         self.horizontalLayout_5 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_5.setContentsMargins(-1, -1, -1, 5)
         self.horizontalLayout_5.setSpacing(0)
         self.horizontalLayout_5.setObjectName("horizontalLayout_5")
-        self.lbl_interval_watch = QtWidgets.QLabel(self.widget_16)
+        self.lbl_interval_watch = QtWidgets.QLabel(parent=self.widget_16)
         self.lbl_interval_watch.setMinimumSize(QtCore.QSize(120, 10))
         self.lbl_interval_watch.setMaximumSize(QtCore.QSize(150, 30))
         font = QtGui.QFont()
         font.setFamily("Bahnschrift Light")
         font.setPointSize(25)
         font.setBold(False)
         font.setItalic(False)
         self.lbl_interval_watch.setFont(font)
         self.lbl_interval_watch.setStyleSheet("border:none;")
-        self.lbl_interval_watch.setTextFormat(QtCore.Qt.AutoText)
-        self.lbl_interval_watch.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_interval_watch.setTextFormat(QtCore.Qt.TextFormat.AutoText)
+        self.lbl_interval_watch.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_interval_watch.setObjectName("lbl_interval_watch")
         self.horizontalLayout_5.addWidget(self.lbl_interval_watch)
         self.verticalLayout_25.addLayout(self.horizontalLayout_5)
         self.gridLayout.addWidget(self.widget_16, 0, 0, 1, 1)
         self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
         self.gridLayout.addLayout(self.horizontalLayout_3, 1, 2, 1, 1)
-        spacerItem4 = QtWidgets.QSpacerItem(500, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem4 = QtWidgets.QSpacerItem(500, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout.addItem(spacerItem4, 0, 1, 1, 1)
-        spacerItem5 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.gridLayout.addItem(spacerItem5, 1, 0, 1, 1)
         self.horizontalLayout_22.addLayout(self.gridLayout)
         self.stackedWidget.addWidget(self.page_interval)
         self.page_training = QtWidgets.QWidget()
         self.page_training.setObjectName("page_training")
         self.verticalLayout_30 = QtWidgets.QVBoxLayout(self.page_training)
         self.verticalLayout_30.setContentsMargins(-1, 0, -1, 0)
         self.verticalLayout_30.setObjectName("verticalLayout_30")
-        self.widget_training_data = QtWidgets.QStackedWidget(self.page_training)
+        self.widget_training_data = QtWidgets.QStackedWidget(parent=self.page_training)
         self.widget_training_data.setObjectName("widget_training_data")
         self.page_12 = QtWidgets.QWidget()
         self.page_12.setObjectName("page_12")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.page_12)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
-        self.lbl_no_training = QtWidgets.QLabel(self.page_12)
+        self.lbl_no_training = QtWidgets.QLabel(parent=self.page_12)
         self.lbl_no_training.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_no_training.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_no_training.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_no_training.setObjectName("lbl_no_training")
         self.verticalLayout_11.addWidget(self.lbl_no_training)
         self.widget_training_data.addWidget(self.page_12)
         self.page_13 = QtWidgets.QWidget()
         self.page_13.setObjectName("page_13")
         self.verticalLayout_32 = QtWidgets.QVBoxLayout(self.page_13)
         self.verticalLayout_32.setObjectName("verticalLayout_32")
         self.verticalLayout_31 = QtWidgets.QVBoxLayout()
         self.verticalLayout_31.setContentsMargins(160, -1, 160, -1)
         self.verticalLayout_31.setSpacing(20)
         self.verticalLayout_31.setObjectName("verticalLayout_31")
-        self.lbl_training_file = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_file = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_file.setStyleSheet("font: 25px \"Bahnschrift Semibold\";")
-        self.lbl_training_file.setAlignment(QtCore.Qt.AlignCenter)
+        self.lbl_training_file.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.lbl_training_file.setObjectName("lbl_training_file")
         self.verticalLayout_31.addWidget(self.lbl_training_file)
         self.gridLayout_2 = QtWidgets.QGridLayout()
         self.gridLayout_2.setContentsMargins(5, 5, 5, 5)
         self.gridLayout_2.setHorizontalSpacing(80)
         self.gridLayout_2.setVerticalSpacing(13)
         self.gridLayout_2.setObjectName("gridLayout_2")
-        self.lbl_training_type = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_type = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_type.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_type.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_type.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_type.setObjectName("lbl_training_type")
         self.gridLayout_2.addWidget(self.lbl_training_type, 0, 1, 1, 1)
-        self.lbl_training_speed_hr = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_speed_hr = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_speed_hr.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_speed_hr.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_speed_hr.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_speed_hr.setObjectName("lbl_training_speed_hr")
         self.gridLayout_2.addWidget(self.lbl_training_speed_hr, 2, 1, 1, 1)
-        self.lbl_training_speed_hr_title = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_speed_hr_title = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_speed_hr_title.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_speed_hr_title.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_speed_hr_title.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_speed_hr_title.setObjectName("lbl_training_speed_hr_title")
         self.gridLayout_2.addWidget(self.lbl_training_speed_hr_title, 2, 0, 1, 1)
-        self.lbl_training_rest_duration_title = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_rest_duration_title = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_rest_duration_title.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_rest_duration_title.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_rest_duration_title.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_rest_duration_title.setObjectName("lbl_training_rest_duration_title")
         self.gridLayout_2.addWidget(self.lbl_training_rest_duration_title, 3, 0, 1, 1)
-        self.lbl_training_rest_duration = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_rest_duration = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_rest_duration.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_rest_duration.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_rest_duration.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_rest_duration.setObjectName("lbl_training_rest_duration")
         self.gridLayout_2.addWidget(self.lbl_training_rest_duration, 3, 1, 1, 1)
-        self.lbl_training_type_title = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_type_title = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_type_title.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_type_title.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_type_title.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_type_title.setObjectName("lbl_training_type_title")
         self.gridLayout_2.addWidget(self.lbl_training_type_title, 0, 0, 1, 1)
-        self.lbl_training_speed_duration_title = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_speed_duration_title = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_speed_duration_title.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_speed_duration_title.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_speed_duration_title.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_speed_duration_title.setObjectName("lbl_training_speed_duration_title")
         self.gridLayout_2.addWidget(self.lbl_training_speed_duration_title, 1, 0, 1, 1)
-        self.lbl_training_speed_duration = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_speed_duration = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_speed_duration.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_speed_duration.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_speed_duration.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_speed_duration.setObjectName("lbl_training_speed_duration")
         self.gridLayout_2.addWidget(self.lbl_training_speed_duration, 1, 1, 1, 1)
-        self.lbl_training_rest_hr_title = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_rest_hr_title = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_rest_hr_title.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_rest_hr_title.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_rest_hr_title.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_rest_hr_title.setObjectName("lbl_training_rest_hr_title")
         self.gridLayout_2.addWidget(self.lbl_training_rest_hr_title, 4, 0, 1, 1)
-        self.lbl_training_repetitions_title = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_repetitions_title = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_repetitions_title.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
         self.lbl_training_repetitions_title.setObjectName("lbl_training_repetitions_title")
         self.gridLayout_2.addWidget(self.lbl_training_repetitions_title, 5, 0, 1, 1)
-        self.lbl_training_rest_hr = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_rest_hr = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_rest_hr.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_rest_hr.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_rest_hr.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_rest_hr.setObjectName("lbl_training_rest_hr")
         self.gridLayout_2.addWidget(self.lbl_training_rest_hr, 4, 1, 1, 1)
-        self.lbl_training_repetitions = QtWidgets.QLabel(self.page_13)
+        self.lbl_training_repetitions = QtWidgets.QLabel(parent=self.page_13)
         self.lbl_training_repetitions.setStyleSheet("font: 22px \"Bahnschrift Semilight\";")
-        self.lbl_training_repetitions.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.lbl_training_repetitions.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.lbl_training_repetitions.setObjectName("lbl_training_repetitions")
         self.gridLayout_2.addWidget(self.lbl_training_repetitions, 5, 1, 1, 1)
         self.verticalLayout_31.addLayout(self.gridLayout_2)
         self.verticalLayout_32.addLayout(self.verticalLayout_31)
         self.widget_training_data.addWidget(self.page_13)
         self.verticalLayout_30.addWidget(self.widget_training_data)
         self.lyt_training = QtWidgets.QVBoxLayout()
         self.lyt_training.setSpacing(0)
         self.lyt_training.setObjectName("lyt_training")
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        spacerItem6 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem6 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_4.addItem(spacerItem6)
-        self.btn_load_training = QtWidgets.QPushButton(self.page_training)
+        self.btn_load_training = QtWidgets.QPushButton(parent=self.page_training)
         self.btn_load_training.setMinimumSize(QtCore.QSize(70, 40))
         self.btn_load_training.setMaximumSize(QtCore.QSize(70, 40))
         self.btn_load_training.setStyleSheet("font: 20px \"Bahnschrift Semilight\";\n"
 "background-color: rgb(255, 255, 255);\n"
 "border: 1px solid black;\n"
 "border-radius: 5px;")
         self.btn_load_training.setIconSize(QtCore.QSize(16, 16))
         self.btn_load_training.setObjectName("btn_load_training")
         self.horizontalLayout_4.addWidget(self.btn_load_training)
-        self.stackedWidget_2 = QtWidgets.QStackedWidget(self.page_training)
+        self.stackedWidget_2 = QtWidgets.QStackedWidget(parent=self.page_training)
         self.stackedWidget_2.setMaximumSize(QtCore.QSize(80, 16777215))
         self.stackedWidget_2.setObjectName("stackedWidget_2")
         self.page_9 = QtWidgets.QWidget()
         self.page_9.setObjectName("page_9")
         self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.page_9)
         self.verticalLayout_8.setObjectName("verticalLayout_8")
-        self.btn_start_training = QtWidgets.QPushButton(self.page_9)
+        self.btn_start_training = QtWidgets.QPushButton(parent=self.page_9)
         self.btn_start_training.setMinimumSize(QtCore.QSize(70, 40))
         self.btn_start_training.setMaximumSize(QtCore.QSize(70, 40))
         self.btn_start_training.setStyleSheet("font: 20px \"Bahnschrift Semilight\";\n"
 "background-color: rgb(255, 255, 255);\n"
 "border: 1px solid black;\n"
 "border-radius: 5px;")
         self.btn_start_training.setObjectName("btn_start_training")
         self.verticalLayout_8.addWidget(self.btn_start_training)
         self.stackedWidget_2.addWidget(self.page_9)
         self.page_10 = QtWidgets.QWidget()
         self.page_10.setObjectName("page_10")
         self.stackedWidget_2.addWidget(self.page_10)
         self.horizontalLayout_4.addWidget(self.stackedWidget_2)
-        spacerItem7 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem7 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_4.addItem(spacerItem7)
         self.lyt_training.addLayout(self.horizontalLayout_4)
         self.verticalLayout_30.addLayout(self.lyt_training)
         self.verticalLayout_30.setStretch(0, 1)
         self.stackedWidget.addWidget(self.page_training)
         self.horizontalLayout_11.addWidget(self.stackedWidget)
-        self.btn_move_right = QtWidgets.QPushButton(self.widget_14)
+        self.btn_move_right = QtWidgets.QPushButton(parent=self.widget_14)
         self.btn_move_right.setStyleSheet("background-color: rgba(255, 255, 255, 0);")
         self.btn_move_right.setText("")
         icon1 = QtGui.QIcon()
-        icon1.addPixmap(QtGui.QPixmap("../ast_monitor/icons/arrow_right.svg"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon1.addPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/arrow_right.svg"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.btn_move_right.setIcon(icon1)
         self.btn_move_right.setIconSize(QtCore.QSize(30, 50))
         self.btn_move_right.setFlat(False)
         self.btn_move_right.setObjectName("btn_move_right")
         self.horizontalLayout_11.addWidget(self.btn_move_right)
         self.verticalLayout_21.addLayout(self.horizontalLayout_11)
         self.verticalLayout_23.addWidget(self.widget_14)
-        self.widget_15 = QtWidgets.QWidget(self.centralwidget)
+        self.widget_15 = QtWidgets.QWidget(parent=self.centralwidget)
         self.widget_15.setStyleSheet("background-color: rgba(240, 240, 240, 1);border-top: 1px solid black;")
         self.widget_15.setObjectName("widget_15")
         self.verticalLayout_22 = QtWidgets.QVBoxLayout(self.widget_15)
         self.verticalLayout_22.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_22.setSpacing(0)
         self.verticalLayout_22.setObjectName("verticalLayout_22")
         self.horizontalLayout_7 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_7.setContentsMargins(15, 1, 15, 1)
         self.horizontalLayout_7.setObjectName("horizontalLayout_7")
-        self.btn_shutdown = QtWidgets.QPushButton(self.widget_15)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
+        self.btn_shutdown = QtWidgets.QPushButton(parent=self.widget_15)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.btn_shutdown.sizePolicy().hasHeightForWidth())
         self.btn_shutdown.setSizePolicy(sizePolicy)
         self.btn_shutdown.setMaximumSize(QtCore.QSize(50, 50))
         self.btn_shutdown.setAutoFillBackground(False)
         self.btn_shutdown.setStyleSheet("background-color: rgba(255, 255, 255, 0);\n"
 "border: none;")
         self.btn_shutdown.setText("")
         icon2 = QtGui.QIcon()
-        icon2.addPixmap(QtGui.QPixmap("../ast_monitor/icons/shutdown.svg"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon2.addPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/shutdown.svg"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.btn_shutdown.setIcon(icon2)
         self.btn_shutdown.setIconSize(QtCore.QSize(50, 50))
         self.btn_shutdown.setAutoRepeat(False)
         self.btn_shutdown.setFlat(False)
         self.btn_shutdown.setObjectName("btn_shutdown")
         self.horizontalLayout_7.addWidget(self.btn_shutdown)
-        spacerItem8 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem8 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_7.addItem(spacerItem8)
-        self.widget_start_stop = QtWidgets.QStackedWidget(self.widget_15)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        self.widget_start_stop = QtWidgets.QStackedWidget(parent=self.widget_15)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.widget_start_stop.sizePolicy().hasHeightForWidth())
         self.widget_start_stop.setSizePolicy(sizePolicy)
         self.widget_start_stop.setMinimumSize(QtCore.QSize(120, 0))
         self.widget_start_stop.setMaximumSize(QtCore.QSize(120, 70))
         self.widget_start_stop.setStyleSheet("border-top: 0px solid black;")
         self.widget_start_stop.setObjectName("widget_start_stop")
         self.page = QtWidgets.QWidget()
         self.page.setObjectName("page")
         self.verticalLayout_15 = QtWidgets.QVBoxLayout(self.page)
         self.verticalLayout_15.setObjectName("verticalLayout_15")
-        self.btn_start_tracking = QtWidgets.QPushButton(self.page)
+        self.btn_start_tracking = QtWidgets.QPushButton(parent=self.page)
         self.btn_start_tracking.setMinimumSize(QtCore.QSize(50, 50))
         self.btn_start_tracking.setMaximumSize(QtCore.QSize(50, 50))
         self.btn_start_tracking.setStyleSheet("background-color: rgb(255, 255, 255);\n"
 "border: 1px solid black;\n"
 "border-radius: 5px;")
         self.btn_start_tracking.setText("")
         icon3 = QtGui.QIcon()
-        icon3.addPixmap(QtGui.QPixmap("../ast_monitor/icons/play.svg"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon3.addPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/play.svg"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.btn_start_tracking.setIcon(icon3)
         self.btn_start_tracking.setIconSize(QtCore.QSize(30, 30))
         self.btn_start_tracking.setFlat(False)
         self.btn_start_tracking.setObjectName("btn_start_tracking")
         self.verticalLayout_15.addWidget(self.btn_start_tracking)
         self.widget_start_stop.addWidget(self.page)
         self.page_2 = QtWidgets.QWidget()
         self.page_2.setObjectName("page_2")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.page_2)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.btn_stop_tracking = QtWidgets.QPushButton(self.page_2)
+        self.btn_stop_tracking = QtWidgets.QPushButton(parent=self.page_2)
         self.btn_stop_tracking.setMinimumSize(QtCore.QSize(50, 50))
         self.btn_stop_tracking.setMaximumSize(QtCore.QSize(50, 50))
         self.btn_stop_tracking.setStyleSheet("background-color: rgb(255, 255, 255);\n"
 "border: 1px solid black;\n"
 "border-radius: 5px;")
         self.btn_stop_tracking.setText("")
         icon4 = QtGui.QIcon()
-        icon4.addPixmap(QtGui.QPixmap("../ast_monitor/icons/stop.svg"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon4.addPixmap(QtGui.QPixmap("uis\\../../ast_monitor/icons/stop.svg"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.btn_stop_tracking.setIcon(icon4)
         self.btn_stop_tracking.setIconSize(QtCore.QSize(25, 25))
         self.btn_stop_tracking.setObjectName("btn_stop_tracking")
         self.verticalLayout.addWidget(self.btn_stop_tracking)
         self.widget_start_stop.addWidget(self.page_2)
         self.horizontalLayout_7.addWidget(self.widget_start_stop)
-        spacerItem9 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem9 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_7.addItem(spacerItem9)
         self.verticalLayout_22.addLayout(self.horizontalLayout_7)
         self.verticalLayout_23.addWidget(self.widget_15)
         self.verticalLayout_24.addLayout(self.verticalLayout_23)
         MainWindow.setCentralWidget(self.centralwidget)
-        self.menubar = QtWidgets.QMenuBar(MainWindow)
+        self.menubar = QtWidgets.QMenuBar(parent=MainWindow)
         self.menubar.setEnabled(True)
         self.menubar.setGeometry(QtCore.QRect(0, 0, 800, 0))
         self.menubar.setMaximumSize(QtCore.QSize(16777215, 0))
         self.menubar.setObjectName("menubar")
-        self.menuMenu = QtWidgets.QMenu(self.menubar)
+        self.menuMenu = QtWidgets.QMenu(parent=self.menubar)
         self.menuMenu.setObjectName("menuMenu")
-        self.menuAbout = QtWidgets.QMenu(self.menubar)
+        self.menuAbout = QtWidgets.QMenu(parent=self.menubar)
         self.menuAbout.setObjectName("menuAbout")
         MainWindow.setMenuBar(self.menubar)
-        self.actionOpen = QtWidgets.QAction(MainWindow)
+        self.actionOpen = QtGui.QAction(parent=MainWindow)
         self.actionOpen.setObjectName("actionOpen")
-        self.actionSave = QtWidgets.QAction(MainWindow)
+        self.actionSave = QtGui.QAction(parent=MainWindow)
         self.actionSave.setObjectName("actionSave")
-        self.action_exit = QtWidgets.QAction(MainWindow)
+        self.action_exit = QtGui.QAction(parent=MainWindow)
         self.action_exit.setObjectName("action_exit")
-        self.action_license = QtWidgets.QAction(MainWindow)
+        self.action_license = QtGui.QAction(parent=MainWindow)
         self.action_license.setObjectName("action_license")
-        self.action_about_program = QtWidgets.QAction(MainWindow)
+        self.action_about_program = QtGui.QAction(parent=MainWindow)
         self.action_about_program.setObjectName("action_about_program")
-        self.action_disclaimer = QtWidgets.QAction(MainWindow)
+        self.action_disclaimer = QtGui.QAction(parent=MainWindow)
         self.action_disclaimer.setObjectName("action_disclaimer")
         self.menuMenu.addAction(self.action_exit)
         self.menuAbout.addAction(self.action_about_program)
         self.menuAbout.addAction(self.action_license)
         self.menuAbout.addAction(self.action_disclaimer)
         self.menubar.addAction(self.menuMenu.menuAction())
         self.menubar.addAction(self.menuAbout.menuAction())
 
         self.retranslateUi(MainWindow)
         self.widget_title.setCurrentIndex(0)
-        self.stackedWidget.setCurrentIndex(0)
+        self.stackedWidget.setCurrentIndex(2)
         self.swgt_interval_performance.setCurrentIndex(0)
         self.widget_training_data.setCurrentIndex(0)
         self.stackedWidget_2.setCurrentIndex(0)
         self.widget_start_stop.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "TrainingFeedback"))
         self.lbl_page.setText(_translate("MainWindow", "Basic data"))
-        self.lbl_page_2.setText(_translate("MainWindow", "Map"))
+        self.lbl_page_2.setText(_translate("MainWindow", "Mapss"))
         self.lbl_page_3.setText(_translate("MainWindow", "Intervals"))
         self.lbl_page_4.setText(_translate("MainWindow", "Training"))
         self.lbl_distance.setText(_translate("MainWindow", "-"))
         self.lbl_speed.setText(_translate("MainWindow", "-"))
         self.lbl_heart_rate.setText(_translate("MainWindow", "-"))
         self.lbl_ascent.setText(_translate("MainWindow", "-"))
         self.lbl_watch.setText(_translate("MainWindow", "-"))
```

### Comparing `ast_monitor-0.3.3/ast_monitor/model.py` & `ast_monitor-0.4.0/ast_monitor/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import glob
 import json
 import os
-import PyQt5
-from PyQt5.QtCore import pyqtSlot, Qt, QTimer
-from PyQt5.QtWidgets import QMainWindow
+import PyQt6
+from PyQt6.QtCore import pyqtSlot, Qt, QTimer, QUrl
+from PyQt6.QtWebEngineCore import QWebEngineSettings
+from PyQt6.QtWidgets import QMainWindow
 try:
-    from PyQt5.QtWebChannel import QWebChannel
-    from PyQt5.QtWebEngineWidgets import QWebEngineView
+    from PyQt6.QtWebChannel import QWebChannel
+    from PyQt6.QtWebEngineWidgets import QWebEngineView
 except Exception:
     pass
 from pyqt_feedback_flow.feedback import (
     AnimationDirection,
     AnimationType,
     TextFeedback
 )
@@ -44,30 +45,33 @@
         self.basic_data = BasicData(hr_data_path, gps_data_path)
         self.initialize_GUI()
 
     def initialize_GUI(self) -> None:
         """
         Initialization method for the GUI of the app.
         """
-        QMainWindow.__init__(self, flags=Qt.FramelessWindowHint)
+        QMainWindow.__init__(self, flags=Qt.WindowType.FramelessWindowHint)
         Ui_MainWindow.__init__(self)
         self.setupUi(self)
 
         # Map setting (not working on Raspberry Pi
         # OS due to missing dependencies).
         try:
             self.view = QWebEngineView()
+            self.view.settings().setAttribute(QWebEngineSettings.WebAttribute.LocalContentCanAccessRemoteUrls, True)
+            self.view.settings().setAttribute(QWebEngineSettings.WebAttribute.LocalContentCanAccessFileUrls, True)
             self.channel = QWebChannel()
             self.channel.registerObject("MainWindow", self)
             self.view.page().setWebChannel(self.channel)
-            file = os.path.join(
+            file = str(os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
                 '../ast_monitor/map/map.html',
-            )
-            self.view.setUrl(PyQt5.QtCore.QUrl.fromLocalFile(file))
+            ))
+
+            self.view.setUrl(PyQt6.QtCore.QUrl.fromLocalFile(file))
             self.vb_map.addWidget(self.view)
         except NameError:
             print('No QtWebEngine module found.')
 
         # Shutdown of the computer.
         self.btn_shutdown.clicked.connect(self.shutdown)
```

### Comparing `ast_monitor-0.3.3/ast_monitor/simulation.py` & `ast_monitor-0.4.0/ast_monitor/simulation.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/training_session.py` & `ast_monitor-0.4.0/ast_monitor/training_session.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/ast_monitor/write_log.py` & `ast_monitor-0.4.0/ast_monitor/write_log.py`

 * *Files identical despite different names*

### Comparing `ast_monitor-0.3.3/pyproject.toml` & `ast_monitor-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ast_monitor"
-version = "0.3.3"
+version = "0.4.0"
 description = "AST-Monitor is a wearable Raspberry Pi computer for cyclists"
 license = "MIT"
 authors = ["Iztok Fister Jr. <iztok@iztok-jr-fister.eu>", "Luka Lukač <luka.lukac@student.um.si>"]
 keywords = ['artificial sport trainer', 'computational intelligence', 'data mining', 'datasets', 'digital twin', 'optimization', 'sport activities', 'tcx']
 homepage = "https://github.com/firefly-cpp/AST-Monitor"
 repository = "https://github.com/firefly-cpp/AST-Monitor"
 readme = "README.md"
@@ -13,22 +13,23 @@
     { path="LICENSE", format="sdist" },
     { path="CHANGELOG.md", format="sdist" },
     { path="CITATION.cff", format="sdist" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-PyQt5 = "*"
 matplotlib = "*"
 geopy = "*"
-pyqt-feedback-flow = "^0.1.6"
 tcxreader = "^0.4.2"
 sport-activities-features = "^0.3.12"
-PyQtWebEngine = "^5.15.5"
 openant = "^1.2.0"
+PyQt6 = "6.4.2"
+PyQt6-WebEngine = "^6.5.0"
+pyqt-feedback-flow = "^0.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ast_monitor-0.3.3/setup.py` & `ast_monitor-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['ast_monitor']
 
 package_data = \
 {'': ['*'], 'ast_monitor': ['icons/*', 'map/*']}
 
 install_requires = \
-['PyQt5',
- 'PyQtWebEngine>=5.15.5,<6.0.0',
+['PyQt6-WebEngine>=6.5.0,<7.0.0',
+ 'PyQt6==6.4.2',
  'geopy',
  'matplotlib',
  'openant>=1.2.0,<2.0.0',
- 'pyqt-feedback-flow>=0.1.6,<0.2.0',
+ 'pyqt-feedback-flow>=0.3.0,<0.4.0',
  'sport-activities-features>=0.3.12,<0.4.0',
  'tcxreader>=0.4.2,<0.5.0']
 
 setup_kwargs = {
     'name': 'ast-monitor',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'AST-Monitor is a wearable Raspberry Pi computer for cyclists',
-    'long_description': '# AST-Monitor --- A wearable Raspberry Pi computer for cyclists\n[![PyPI Version](https://img.shields.io/pypi/v/ast-monitor.svg)](https://pypi.python.org/pypi/ast-monitor)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ast-monitor.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/ast-monitor.svg)\n[![Downloads](https://pepy.tech/badge/ast-monitor)](https://pepy.tech/project/ast-monitor)\n![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/ast-monitor?style=flat-square)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/ast-monitor.svg)](https://github.com/firefly-cpp/AST-Monitor/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/ast-monitor.svg)\n![GitHub contributors](https://img.shields.io/github/contributors/firefly-cpp/ast-monitor.svg)\n[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)\n\n[![DOI](https://img.shields.io/badge/DOI-10.1109/ISCMI53840.2021.9654817-blue)](https://doi.org/10.1109/ISCMI53840.2021.9654817)\n[![DOI](https://img.shields.io/badge/DOI-10.3390/app122412741-blue)](https://doi.org/10.3390/app122412741)\n[![Fedora package](https://img.shields.io/fedora/v/python3-ast-monitor?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-ast-monitor)\n[![AUR package](https://img.shields.io/aur/version/python-ast-monitor?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-ast-monitor)\n\n* **Documentation:** [https://ast-monitor.readthedocs.io/en/latest](https://ast-monitor.readthedocs.io/en/latest)\n* **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**\n  \n## Short description\nThis repository is devoted to AST-Monitor, i.e., a low-cost and efficient embedded device for monitoring the realization of sport training sessions that are dedicated to monitoring cycling training sessions.\nAST-Monitor is a part of the Artificial Sport Trainer (AST) system. The first bits of AST-Monitor were presented in the following [paper](https://arxiv.org/abs/2109.13334).\n\n\n## Graphical User Interface of the application\n### Basic data\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/179205064-160bdd44-fd67-4d8d-85dd-badea999885c.png" alt="AST-GUI">\n</p>\nThe initial page of the application depicts basic parameters of an athlete\'s activity: current speed and current heart rate. If a training session is conducted, total distance, total time of the session and total ascent are displayed as well.\n\n---\n### Interactive map\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/179205118-19cbb6e2-f410-4371-a762-c4c77344ab24.png" alt="AST-Map">\n</p>\nThe second page of the application is devoted to an interactive map, which depicts athlete\'s current position.\n\nNote: the position is currently hardcoded and does not respond according to GPS data.\n\n---\n### Interval training data\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/179205160-edce581c-1ea8-4287-a795-7d05fb7c8ddc.png" alt="AST-Intervals">\n</p>\nThe third page of the application depicts interval training data. During an interval training, total duration of the current phase is displayed along with current heart rate, average heart rate, Digital Twin proposed heart rate and the difference between the current and the proposed heart rate.\n\n---\n### Interval training plan\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/189926103-e0895132-9bbc-41bf-8868-51e3e6c23f8a.png" alt="AST-Trainings">\n</p>\nThe fourth and final page of the application is intended for loading and starting interval trainings located in the folder "AST-Monitor/development/trainings". In order to be parsed correctly, trainings must be written in domain-specific language <a href="https://github.com/firefly-cpp/ast-tdl">AST-TDL</a> and converted to JavaScript Object Notation (JSON). After successful loading of an interval training, the training plan is displayed on this page.\n\n\n## Hardware outline\nThe complete hardware part is shown in the figure from which it can be seen that the AST-computer is split into the following pieces:\n\n* a platform with fixing straps that attach to a bicycle,\n* the Raspberry Pi 4 Model B micro-controller with Raspbian OS installed,\n* a five-inch LCD touch screen display,\n* a USB ANT+ stick,\n* Adafruit\'s Ultimate GPS HAT module.\n\n<p align="center">\n  <img width="600" src="https://raw.githubusercontent.com/firefly-cpp/AST-Monitor/main/.github/img/complete_small.JPG" alt="AST-Monitor">\n</p>\n\nA Serial Peripheral Interface (SPI) protocol was dedicated to communication between the Raspberry Pi and the GPS peripheral. A specialized USB ANT+ stick was used to capture the HR signal. The screen display was connected using a modified (physically shortened) HDMI cable, while the touch feedback was implemented using physical wires. The computer was powered during the testing phase using the Trust\'s (5 VDC) power bank. The AST-Monitor prototype is still a little bulky, but a more discrete solution is being searched for, including the sweat drainer of the AST. Internal components of AST-Monitor are depicted in the following scheme.\n\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/189920171-ac946a93-ad78-4e4b-bf09-5de5bf69bef9.png" alt="AST-Monitor">\n</p>\n\n## Software outline\n### Dependencies\nList of dependencies:\n\n| Package      | Version    | Platform |\n| ------------ |:----------:|:--------:|\n| PyQt5        | ^5.15.6    | All      |\n| matplotlib   | ^3.5.1     | All      |\n| geopy        | ^2.2.0     | All      |\n| openant      | ^1.2.0     | All      |\n| pyqt-feedback-flow       | ^0.1.0     | All      |\n| tcxreader       | ^0.4.1     | All      |\n| sport-activities-features       | ^0.3.6     | All      |\n\nAdditional note: adafruit-circuitpython-gps package must be installed in order to work with the GPS sensor:\n\n```sh\n$ pip install adafruit-circuitpython-gps\n```\n\n## Installation\nInstall AST-Monitor with pip:\n\n```sh\n$ pip install ast-monitor\n```\nIn case you want to install directly from the source code, use:\n\n```sh\n$ git clone https://github.com/firefly-cpp/AST-Monitor.git\n$ cd AST-Monitor\n$ poetry build\n$ python setup.py install\n```\n\nTo install AST-Monitor on Fedora Linux, please use:\n\n```sh\n$ dnf install python3-ast-monitor\n```\n\nTo install AST-Monitor on Alpine Linux, please use:\n\n```sh\n$ apk add py3-ast-monitor\n```\n\nTo install AST-Monitor on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):\n\n```sh\n$ yay -Syyu python-ast-monitor\n```\n\n## Deployment\nOur project was deployed on a Raspberry Pi device using Raspberry Pi OS.\n\nThe hardware configuration of AST-Monitor using Raspberry Pi OS is described in <a href="https://github.com/firefly-cpp/AST-Monitor/blob/main/HARDWARE_CONFIGURATION.md">HARDWARE_CONFIGURATION.md</a>.\n\n## Examples\n\n### Basic run\n```python\nfrom PyQt5 import QtWidgets\nimport sys\n\ntry:\n    from ast_monitor.model import AST\nexcept ModuleNotFoundError:\n    sys.path.append(\'../\')\n    from ast_monitor.model import AST\n\n\n# Paths to the files with heart rates and GPS data.\nhr_data = \'../sensor_data/hr.txt\'\ngps_data = \'../sensor_data/gps.txt\'\n\nif __name__ == \'__main__\':\n    app = QtWidgets.QApplication(sys.argv)\n    window = AST(hr_data, gps_data)\n    window.show()\n    sys.exit(app.exec_())\n```\n\n## License\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n\n## Cite us\nLukač, L., Fister Jr., I., Fister, I. "[Digital Twin in Sport: From an Idea to Realization](https://www.mdpi.com/2076-3417/12/24/12741)." Applied Sciences 12.24 (2022): 12741.\n\n## References\nFister Jr, I., Fister, I., Iglesias, A., Galvez, A., Deb, S., & Fister, D. (2021). On deploying the Artificial Sport Trainer into practice. arXiv preprint [arXiv:2109.13334](https://arxiv.org/abs/2109.13334).\n\nFister Jr, I., Salcedo-Sanz, S., Iglesias, A., Fister, D., Gálvez, A., & Fister, I. (2021). New Perspectives in the Development of the Artificial Sport Trainer. Applied Sciences, 11(23), 11452. DOI: [10.3390/app112311452](https://doi.org/10.3390/app112311452)\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Code">💻</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑\u200d🏫</a> <a href="#platform-firefly-cpp" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/luckyLukac"><img src="https://avatars.githubusercontent.com/u/73126820?v=4?s=100" width="100px;" alt="luckyLukac"/><br /><sub><b>luckyLukac</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AluckyLukac" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Code">💻</a> <a href="#design-luckyLukac" title="Design">🎨</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="#content-alenrajsp" title="Content">🖋</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/KukovecRok"><img src="https://avatars.githubusercontent.com/u/33880044?v=4?s=100" width="100px;" alt="Tatookie"/><br /><sub><b>Tatookie</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=KukovecRok" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AKukovecRok" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n',
+    'long_description': '# AST-Monitor --- A wearable Raspberry Pi computer for cyclists\n[![PyPI Version](https://img.shields.io/pypi/v/ast-monitor.svg)](https://pypi.python.org/pypi/ast-monitor)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ast-monitor.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/ast-monitor.svg)\n[![Downloads](https://pepy.tech/badge/ast-monitor)](https://pepy.tech/project/ast-monitor)\n![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/ast-monitor?style=flat-square)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/ast-monitor.svg)](https://github.com/firefly-cpp/AST-Monitor/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/ast-monitor.svg)\n![GitHub contributors](https://img.shields.io/github/contributors/firefly-cpp/ast-monitor.svg)\n[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)\n\n[![DOI](https://img.shields.io/badge/DOI-10.1109/ISCMI53840.2021.9654817-blue)](https://doi.org/10.1109/ISCMI53840.2021.9654817)\n[![DOI](https://img.shields.io/badge/DOI-10.3390/app122412741-blue)](https://doi.org/10.3390/app122412741)\n[![Fedora package](https://img.shields.io/fedora/v/python3-ast-monitor?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-ast-monitor)\n[![AUR package](https://img.shields.io/aur/version/python-ast-monitor?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-ast-monitor)\n\n* **Documentation:** [https://ast-monitor.readthedocs.io/en/latest](https://ast-monitor.readthedocs.io/en/latest)\n* **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**\n  \n## Short description\nThis repository is devoted to AST-Monitor, i.e., a low-cost and efficient embedded device for monitoring the realization of sport training sessions that are dedicated to monitoring cycling training sessions.\nAST-Monitor is a part of the Artificial Sport Trainer (AST) system. The first bits of AST-Monitor were presented in the following [paper](https://arxiv.org/abs/2109.13334).\n\n\n## Graphical User Interface of the application\n### Basic data\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/179205064-160bdd44-fd67-4d8d-85dd-badea999885c.png" alt="AST-GUI">\n</p>\nThe initial page of the application depicts basic parameters of an athlete\'s activity: current speed and current heart rate. If a training session is conducted, total distance, total time of the session and total ascent are displayed as well.\n\n---\n### Interactive map\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/179205118-19cbb6e2-f410-4371-a762-c4c77344ab24.png" alt="AST-Map">\n</p>\nThe second page of the application is devoted to an interactive map, which depicts athlete\'s current position.\n\nNote: the position is currently hardcoded and does not respond according to GPS data.\n\n---\n### Interval training data\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/179205160-edce581c-1ea8-4287-a795-7d05fb7c8ddc.png" alt="AST-Intervals">\n</p>\nThe third page of the application depicts interval training data. During an interval training, total duration of the current phase is displayed along with current heart rate, average heart rate, Digital Twin proposed heart rate and the difference between the current and the proposed heart rate.\n\n---\n### Interval training plan\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/189926103-e0895132-9bbc-41bf-8868-51e3e6c23f8a.png" alt="AST-Trainings">\n</p>\nThe fourth and final page of the application is intended for loading and starting interval trainings located in the folder "AST-Monitor/development/trainings". In order to be parsed correctly, trainings must be written in domain-specific language <a href="https://github.com/firefly-cpp/ast-tdl">AST-TDL</a> and converted to JavaScript Object Notation (JSON). After successful loading of an interval training, the training plan is displayed on this page.\n\n\n## Hardware outline\nThe complete hardware part is shown in the figure from which it can be seen that the AST-computer is split into the following pieces:\n\n* a platform with fixing straps that attach to a bicycle,\n* the Raspberry Pi 4 Model B micro-controller with Raspbian OS installed,\n* a five-inch LCD touch screen display,\n* a USB ANT+ stick,\n* Adafruit\'s Ultimate GPS HAT module.\n\n<p align="center">\n  <img width="600" src="https://raw.githubusercontent.com/firefly-cpp/AST-Monitor/main/.github/img/complete_small.JPG" alt="AST-Monitor">\n</p>\n\nA Serial Peripheral Interface (SPI) protocol was dedicated to communication between the Raspberry Pi and the GPS peripheral. A specialized USB ANT+ stick was used to capture the HR signal. The screen display was connected using a modified (physically shortened) HDMI cable, while the touch feedback was implemented using physical wires. The computer was powered during the testing phase using the Trust\'s (5 VDC) power bank. The AST-Monitor prototype is still a little bulky, but a more discrete solution is being searched for, including the sweat drainer of the AST. Internal components of AST-Monitor are depicted in the following scheme.\n\n<p align="center">\n  <img width="600" src="https://user-images.githubusercontent.com/73126820/189920171-ac946a93-ad78-4e4b-bf09-5de5bf69bef9.png" alt="AST-Monitor">\n</p>\n\n## Software outline\n### Dependencies\nList of dependencies:\n\n| Package      | Version    | Platform |\n| ------------ |:----------:|:--------:|\n| PyQt5        | ^5.15.6    | All      |\n| matplotlib   | ^3.5.1     | All      |\n| geopy        | ^2.2.0     | All      |\n| openant      | ^1.2.0     | All      |\n| pyqt-feedback-flow       | ^0.1.0     | All      |\n| tcxreader       | ^0.4.1     | All      |\n| sport-activities-features       | ^0.3.6     | All      |\n\nAdditional note: adafruit-circuitpython-gps package must be installed in order to work with the GPS sensor:\n\n```sh\n$ pip install adafruit-circuitpython-gps\n```\n\n## Installation\nInstall AST-Monitor with pip:\n\n```sh\n$ pip install ast-monitor\n```\nIn case you want to install directly from the source code, use:\n\n```sh\n$ git clone https://github.com/firefly-cpp/AST-Monitor.git\n$ cd AST-Monitor\n$ poetry build\n$ python setup.py install\n```\n\nTo install AST-Monitor on Fedora Linux, please use:\n\n```sh\n$ dnf install python3-ast-monitor\n```\n\nTo install AST-Monitor on Alpine Linux, please use:\n\n```sh\n$ apk add py3-ast-monitor\n```\n\nTo install AST-Monitor on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):\n\n```sh\n$ yay -Syyu python-ast-monitor\n```\n\n## Deployment\nOur project was deployed on a Raspberry Pi device using Raspberry Pi OS.\n\nThe hardware configuration of AST-Monitor using Raspberry Pi OS is described in <a href="https://github.com/firefly-cpp/AST-Monitor/blob/main/HARDWARE_CONFIGURATION.md">HARDWARE_CONFIGURATION.md</a>.\n\n## Examples\n\n### Basic run\n```python\nfrom PyQt5 import QtWidgets\nimport sys\n\ntry:\n    from ast_monitor.model import AST\nexcept ModuleNotFoundError:\n    sys.path.append(\'../\')\n    from ast_monitor.model import AST\n\n\n# Paths to the files with heart rates and GPS data.\nhr_data = \'../sensor_data/hr.txt\'\ngps_data = \'../sensor_data/gps.txt\'\n\nif __name__ == \'__main__\':\n    app = QtWidgets.QApplication(sys.argv)\n    window = AST(hr_data, gps_data)\n    window.show()\n    sys.exit(app.exec_())\n```\n\n## License\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n\n## Cite us\nLukač, L., Fister Jr., I., Fister, I. "[Digital Twin in Sport: From an Idea to Realization](https://www.mdpi.com/2076-3417/12/24/12741)." Applied Sciences 12.24 (2022): 12741.\n\n## References\nFister Jr, I., Fister, I., Iglesias, A., Galvez, A., Deb, S., & Fister, D. (2021). On deploying the Artificial Sport Trainer into practice. arXiv preprint [arXiv:2109.13334](https://arxiv.org/abs/2109.13334).\n\nFister Jr, I., Salcedo-Sanz, S., Iglesias, A., Fister, D., Gálvez, A., & Fister, I. (2021). New Perspectives in the Development of the Artificial Sport Trainer. Applied Sciences, 11(23), 11452. DOI: [10.3390/app112311452](https://doi.org/10.3390/app112311452)\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Code">💻</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑\u200d🏫</a> <a href="#platform-firefly-cpp" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/luckyLukac"><img src="https://avatars.githubusercontent.com/u/73126820?v=4?s=100" width="100px;" alt="luckyLukac"/><br /><sub><b>luckyLukac</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AluckyLukac" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Code">💻</a> <a href="#design-luckyLukac" title="Design">🎨</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="#content-alenrajsp" title="Content">🖋</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=alenrajsp" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/KukovecRok"><img src="https://avatars.githubusercontent.com/u/33880044?v=4?s=100" width="100px;" alt="Tatookie"/><br /><sub><b>Tatookie</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=KukovecRok" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AKukovecRok" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n',
     'author': 'Iztok Fister Jr.',
     'author_email': 'iztok@iztok-jr-fister.eu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/firefly-cpp/AST-Monitor',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ast_monitor-0.3.3/PKG-INFO` & `ast_monitor-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ast-monitor
-Version: 0.3.3
+Version: 0.4.0
 Summary: AST-Monitor is a wearable Raspberry Pi computer for cyclists
 Home-page: https://github.com/firefly-cpp/AST-Monitor
 License: MIT
 Keywords: artificial sport trainer,computational intelligence,data mining,datasets,digital twin,optimization,sport activities,tcx
 Author: Iztok Fister Jr.
 Author-email: iztok@iztok-jr-fister.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyQt5
-Requires-Dist: PyQtWebEngine (>=5.15.5,<6.0.0)
+Requires-Dist: PyQt6 (==6.4.2)
+Requires-Dist: PyQt6-WebEngine (>=6.5.0,<7.0.0)
 Requires-Dist: geopy
 Requires-Dist: matplotlib
 Requires-Dist: openant (>=1.2.0,<2.0.0)
-Requires-Dist: pyqt-feedback-flow (>=0.1.6,<0.2.0)
+Requires-Dist: pyqt-feedback-flow (>=0.3.0,<0.4.0)
 Requires-Dist: sport-activities-features (>=0.3.12,<0.4.0)
 Requires-Dist: tcxreader (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/firefly-cpp/AST-Monitor
 Description-Content-Type: text/markdown
 
 # AST-Monitor --- A wearable Raspberry Pi computer for cyclists
 [![PyPI Version](https://img.shields.io/pypi/v/ast-monitor.svg)](https://pypi.python.org/pypi/ast-monitor)
@@ -201,15 +201,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=firefly-cpp" title="Code">💻</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a> <a href="#platform-firefly-cpp" title="Packaging/porting to new platform">📦</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/luckyLukac"><img src="https://avatars.githubusercontent.com/u/73126820?v=4?s=100" width="100px;" alt="luckyLukac"/><br /><sub><b>luckyLukac</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AluckyLukac" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=luckyLukac" title="Code">💻</a> <a href="#design-luckyLukac" title="Design">🎨</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="#content-alenrajsp" title="Content">🖋</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="#content-alenrajsp" title="Content">🖋</a> <a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=alenrajsp" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/KukovecRok"><img src="https://avatars.githubusercontent.com/u/33880044?v=4?s=100" width="100px;" alt="Tatookie"/><br /><sub><b>Tatookie</b></sub></a><br /><a href="https://github.com/firefly-cpp/AST-Monitor/commits?author=KukovecRok" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/AST-Monitor/issues?q=author%3AKukovecRok" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

