# Comparing `tmp/docrobot-1.0.8.tar.gz` & `tmp/docrobot-1.1.0.tar.gz`

## Comparing `docrobot-1.0.8.tar` & `docrobot-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.8/convert.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.8/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/form.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/form.ui
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.8/LICENSE
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.0.8/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 docrobot-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.1.0/convert.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.1.0/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 docrobot-1.1.0/src/docrobot/form.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 docrobot-1.1.0/src/docrobot/form.ui
+-rw-r--r--   0        0        0    24356 2020-02-02 00:00:00.000000 docrobot-1.1.0/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.1.0/LICENSE
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.1.0/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 docrobot-1.1.0/PKG-INFO
```

### Comparing `docrobot-1.0.8/.github/workflows/python-publish.yml` & `docrobot-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.8/src/docrobot/form.py` & `docrobot-1.1.0/src/docrobot/form.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'form.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.1
+## Created by: Qt User Interface Compiler version 6.5.1
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
     QCursor, QFont, QFontDatabase, QGradient,
     QIcon, QImage, QKeySequence, QLinearGradient,
     QPainter, QPalette, QPixmap, QRadialGradient,
     QTransform)
-from PySide6.QtWidgets import (QApplication, QLabel, QLineEdit, QMainWindow,
-    QMenu, QMenuBar, QSizePolicy, QStatusBar,
-    QTextEdit, QWidget)
+from PySide6.QtWidgets import (QApplication, QHBoxLayout, QLabel, QLineEdit,
+    QMainWindow, QMenu, QMenuBar, QSizePolicy,
+    QStatusBar, QTextEdit, QWidget)
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
-        MainWindow.resize(800, 600)
+        MainWindow.resize(800, 632)
         self.actionSelect_Dir = QAction(MainWindow)
         self.actionSelect_Dir.setObjectName(u"actionSelect_Dir")
         self.actioncheck = QAction(MainWindow)
         self.actioncheck.setObjectName(u"actioncheck")
         self.actionreplace = QAction(MainWindow)
         self.actionreplace.setObjectName(u"actionreplace")
         self.actioncheckall = QAction(MainWindow)
         self.actioncheckall.setObjectName(u"actioncheckall")
+        self.actionsearchall = QAction(MainWindow)
+        self.actionsearchall.setObjectName(u"actionsearchall")
         self.centralwidget = QWidget(MainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
         self.textEdit = QTextEdit(self.centralwidget)
         self.textEdit.setObjectName(u"textEdit")
-        self.textEdit.setGeometry(QRect(10, 40, 781, 521))
-        self.label = QLabel(self.centralwidget)
+        self.textEdit.setGeometry(QRect(10, 40, 781, 551))
+        self.layoutWidget = QWidget(self.centralwidget)
+        self.layoutWidget.setObjectName(u"layoutWidget")
+        self.layoutWidget.setGeometry(QRect(10, 10, 781, 22))
+        self.horizontalLayout = QHBoxLayout(self.layoutWidget)
+        self.horizontalLayout.setObjectName(u"horizontalLayout")
+        self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
+        self.label = QLabel(self.layoutWidget)
         self.label.setObjectName(u"label")
-        self.label.setGeometry(QRect(10, 10, 91, 16))
-        self.lineEdit = QLineEdit(self.centralwidget)
+
+        self.horizontalLayout.addWidget(self.label)
+
+        self.lineEdit = QLineEdit(self.layoutWidget)
         self.lineEdit.setObjectName(u"lineEdit")
-        self.lineEdit.setGeometry(QRect(100, 10, 691, 20))
+
+        self.horizontalLayout.addWidget(self.lineEdit)
+
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QMenuBar(MainWindow)
         self.menubar.setObjectName(u"menubar")
-        self.menubar.setGeometry(QRect(0, 0, 800, 26))
+        self.menubar.setGeometry(QRect(0, 0, 800, 22))
         self.menu = QMenu(self.menubar)
         self.menu.setObjectName(u"menu")
         self.menu_2 = QMenu(self.menubar)
         self.menu_2.setObjectName(u"menu_2")
         self.menu_3 = QMenu(self.menubar)
         self.menu_3.setObjectName(u"menu_3")
         self.menu_4 = QMenu(self.menubar)
@@ -66,26 +78,28 @@
         self.menubar.addAction(self.menu_2.menuAction())
         self.menubar.addAction(self.menu_3.menuAction())
         self.menu.addAction(self.actionSelect_Dir)
         self.menu_2.addAction(self.actionreplace)
         self.menu_3.addAction(self.actioncheck)
         self.menu_4.addSeparator()
         self.menu_4.addAction(self.actioncheckall)
+        self.menu_4.addAction(self.actionsearchall)
 
         self.retranslateUi(MainWindow)
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
         self.actionSelect_Dir.setText(QCoreApplication.translate("MainWindow", u"Select Dir", None))
-        self.actioncheck.setText(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5", None))
+        self.actioncheck.setText(QCoreApplication.translate("MainWindow", u"\u66ff\u6362", None))
         self.actionreplace.setText(QCoreApplication.translate("MainWindow", u"\u6279\u91cf\u66ff\u6362", None))
         self.actioncheckall.setText(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5\u6240\u6709\u9879", None))
+        self.actionsearchall.setText(QCoreApplication.translate("MainWindow", u"\u5168\u6587\u641c\u7d22", None))
         self.label.setText(QCoreApplication.translate("MainWindow", u"\u5f53\u524d\u5904\u7406\u76ee\u5f55\uff1a", None))
         self.menu.setTitle(QCoreApplication.translate("MainWindow", u"\u8bbe\u7f6e", None))
-        self.menu_2.setTitle(QCoreApplication.translate("MainWindow", u"\u9879\u76ee", None))
-        self.menu_3.setTitle(QCoreApplication.translate("MainWindow", u"\u4e13\u5229", None))
+        self.menu_2.setTitle(QCoreApplication.translate("MainWindow", u"\u9879\u76ee\u6587\u6863", None))
+        self.menu_3.setTitle(QCoreApplication.translate("MainWindow", u"\u7acb\u9879\u603b\u8868", None))
         self.menu_4.setTitle(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5", None))
     # retranslateUi
```

### Comparing `docrobot-1.0.8/src/docrobot/form.ui` & `docrobot-1.1.0/src/docrobot/form.ui`

 * *Files 11% similar despite different names*

#### Comparing `docrobot-1.0.8/src/docrobot/form.ui` & `docrobot-1.1.0/src/docrobot/form.ui`

```diff
@@ -3,112 +3,117 @@
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>800</width>
-        <height>600</height>
+        <height>632</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>MainWindow</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <widget class="QTextEdit" name="textEdit">
         <property name="geometry">
           <rect>
             <x>10</x>
             <y>40</y>
             <width>781</width>
-            <height>521</height>
+            <height>551</height>
           </rect>
         </property>
       </widget>
-      <widget class="QLabel" name="label">
+      <widget class="QWidget" name="layoutWidget">
         <property name="geometry">
           <rect>
             <x>10</x>
             <y>10</y>
-            <width>91</width>
-            <height>16</height>
-          </rect>
-        </property>
-        <property name="text">
-          <string>当前处理目录：</string>
-        </property>
-      </widget>
-      <widget class="QLineEdit" name="lineEdit">
-        <property name="geometry">
-          <rect>
-            <x>100</x>
-            <y>10</y>
-            <width>691</width>
-            <height>20</height>
+            <width>781</width>
+            <height>22</height>
           </rect>
         </property>
+        <layout class="QHBoxLayout" name="horizontalLayout">
+          <item>
+            <widget class="QLabel" name="label">
+              <property name="text">
+                <string>当前处理目录：</string>
+              </property>
+            </widget>
+          </item>
+          <item>
+            <widget class="QLineEdit" name="lineEdit"/>
+          </item>
+        </layout>
       </widget>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>800</width>
-          <height>26</height>
+          <height>22</height>
         </rect>
       </property>
       <widget class="QMenu" name="menu">
         <property name="title">
           <string>设置</string>
         </property>
         <addaction name="actionSelect_Dir"/>
       </widget>
       <widget class="QMenu" name="menu_2">
         <property name="title">
-          <string>项目</string>
+          <string>项目文档</string>
         </property>
         <addaction name="actionreplace"/>
       </widget>
       <widget class="QMenu" name="menu_3">
         <property name="title">
-          <string>专利</string>
+          <string>立项总表</string>
         </property>
         <addaction name="actioncheck"/>
       </widget>
       <widget class="QMenu" name="menu_4">
         <property name="title">
           <string>检查</string>
         </property>
         <addaction name="separator"/>
         <addaction name="actioncheckall"/>
+        <addaction name="actionsearchall"/>
       </widget>
       <addaction name="menu"/>
       <addaction name="menu_4"/>
       <addaction name="menu_2"/>
       <addaction name="menu_3"/>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
     <action name="actionSelect_Dir">
       <property name="text">
         <string>Select Dir</string>
       </property>
     </action>
     <action name="actioncheck">
       <property name="text">
-        <string>检查</string>
+        <string>替换</string>
       </property>
     </action>
     <action name="actionreplace">
       <property name="text">
         <string>批量替换</string>
       </property>
     </action>
     <action name="actioncheckall">
       <property name="text">
         <string>检查所有项</string>
       </property>
     </action>
+    <action name="actionsearchall">
+      <property name="text">
+        <string>全文搜索</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `docrobot-1.0.8/src/docrobot/guimain.pyw` & `docrobot-1.1.0/src/docrobot/guimain.pyw`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 import sys
 from configparser import ConfigParser
 
 from PySide6 import QtCore
 from PySide6.QtCore import QEventLoop, QTimer
-from PySide6.QtWidgets import QApplication, QMainWindow, QFileDialog
+from PySide6.QtWidgets import QApplication, QMainWindow, QFileDialog, QInputDialog, QLineEdit
 from docx import Document
 from docx.opc.exceptions import PackageNotFoundError
 from openpyxl.reader.excel import load_workbook
 from win32com.client import DispatchEx
 
 from docrobot.form import Ui_MainWindow
 
@@ -24,14 +24,27 @@
     p_cost = ''
     p_people = ''  # 人数
     p_owner = ''  # 项目负责人
     p_rnd = ''  # 研发人员
     p_money = ''  # 总预算
 
 
+class CheckR(object):
+    """文档检查结果"""
+
+    def __init__(self, match=0, unmatch=0):
+        self.match = match
+        self.unmatch = unmatch
+
+    def __add__(self, other):
+        match = self.match + other.match
+        unmatch = self.unmatch + other.unmatch
+        return CheckR(match, unmatch)
+
+
 class EmittingStr(QtCore.QObject):
     textWritten = QtCore.Signal(str)
 
     def write(self, text):
         self.textWritten.emit(str(text))
         loop = QEventLoop()
         QTimer.singleShot(100, loop.quit)
@@ -55,14 +68,15 @@
         sys.stderr = EmittingStr()
         sys.stderr.textWritten.connect(self.outputWritten)
 
         self.actionSelect_Dir.triggered.connect(self.setDocUrl)
         self.actioncheck.triggered.connect(lambda: self.checkpatent(True))
         self.actionreplace.triggered.connect(lambda: self.replaceprj(True))
         self.actioncheckall.triggered.connect(self.checkall)
+        self.actionsearchall.triggered.connect(self.searchall)
 
         self.config = ConfigParser()
         try:
             self.config.read('config.ini', encoding='UTF-8')
             self.workdir = self.config['config']['lasting']
         except KeyError:
             self.config.add_section('config')
@@ -102,42 +116,40 @@
     def replaceprj(self, modify=False):
         if modify:
             self.textEdit.setText('')
             self.update_data()
 
         for project in self.arr_prj:
             # self.textEdit.append(project.p_order + ' 项目开始处理...')
-            match = 0  # 已匹配条目数
+            checkr = CheckR()  # 已匹配条目数
             doc_name = ''
             try:
                 doc_name = self.workdir + '/RD' + project.p_order + project.p_name + '.docx'
                 document = Document(doc_name)
                 # debug_doc(document)
-                match = match + self.replace_comname(document, project)
-                match = match + self.first_table(document, project)
-                match = match + self.start_time(document, project)
-                match = match + self.second_table(document, project)
-                match = match + self.third_table(document, project)
+                checkr = checkr + self.replace_comname(document, project)
+                checkr = checkr + self.first_table(document, project)
+                checkr = checkr + self.start_time(document, project)
+                checkr = checkr + self.second_table(document, project)
+                checkr = checkr + self.third_table(document, project)
 
-                match = match + self.checkpat2(document, project)
+                checkr = checkr + self.checkpat2(document, project)
 
                 if modify:
                     document.save(doc_name)
             except PackageNotFoundError:
                 self.textEdit.append('Error打开文件错误：' + doc_name)
             except PermissionError:
                 self.textEdit.append('Error 保存文件错误，可能是文件已被打开：' + doc_name)
-            # 基础17项替换和检查 + N项专利
-            needmatch = 17 + len(project.pat_list.splitlines())
-            if needmatch - match > 0:
-                self.textEdit.append(project.p_order + ' 项目检查完成。 <font color="red"><b>'
-                                     + str(needmatch - match) + ' </b></font> 项条目不匹配。')
-            else:
-                self.textEdit.append(project.p_order + ' 项目检查完成。 <font color="green"><b>'
-                                     + str(match) + ' </b></font> 项条目完全匹配。')
+
+            prompt = project.p_order + ' 项目检查完成。 <font color="green"><b>' + str(
+                checkr.match) + ' </b></font> 项匹配。'
+            if checkr.unmatch > 0:
+                prompt = prompt + ' <font color="red"><b>' + str(checkr.unmatch) + ' </b></font> 项不匹配。'
+            self.textEdit.append(prompt)
 
     def checkpatent(self, modify=False):
         if modify:
             self.textEdit.setText('')
             self.update_data()
 
         match = 0  # 已匹配条目数
@@ -203,40 +215,45 @@
                 xl_book.Close(True)
                 xl_book = None
                 xl_app.Quit()
                 xl_app = None
         except PermissionError:
             self.textEdit.append('写文件失败，关闭其他占用该文件的程序.' + self.file_prj)
         wb.close()
-        self.textEdit.append('项目立项表IP更新完成。 <font color="green"><b>' + str(match) + ' </b></font> 项条目匹配。')
+
+        prompt = '项目立项表IP更新完成。 <font color="green"><b>' + str(match) + ' </b></font> 项条目匹配。'
         if unmatch != 0:
-            self.textEdit.append(' <font color="red"><b>' + str(unmatch) + ' </b></font> 项条目不匹配。')
+            prompt = prompt + ' <font color="red"><b>' + str(unmatch) + ' </b></font> 项条目不匹配。'
+        self.textEdit.append(prompt)
 
     def checkpat2(self, doc, prj):
-        match = 0
+        match = unmatch = 0
         lst = prj.pat_list.splitlines()
         for pat_name in lst:
             if pat_name in self.pat_dict2:
                 pat_num = self.pat_dict2[pat_name]
                 found = False
                 regex = pat_name.replace('[', r'\[').replace(']', r'\]'.replace('(', r'\(').replace(')', r'\)'))
                 for i, para in enumerate(doc.tables[2].rows[4].cells[0].paragraphs):
                     if re.search(regex + '，.*号：', para.text):
                         found |= True
                         result = re.search(regex + '，.*号：' + pat_num, para.text)
                         if result is None:
+                            unmatch = unmatch + 1
                             self.textEdit.append('专利名和编号不匹配：' + pat_name + ' , ' + pat_num)
                             self.textEdit.append('文档内容：' + para.text)
                         else:
                             match = match + 1
                 if not found:
+                    unmatch = unmatch + 1
                     self.textEdit.append('全文找不到：' + pat_name)
-            else:
+            elif pat_name != "无":
+                unmatch = unmatch + 1
                 self.textEdit.append('Error没有找到专利：' + pat_name)
-        return match
+        return CheckR(match, unmatch)
 
     def update_data(self):
         self.pat_dict.clear()
         self.pat_dict2.clear()
         with open(self.file_pat, "rb") as f:
             in_mem_file = io.BytesIO(f.read())
         wb = load_workbook(in_mem_file, read_only=True, data_only=True)
@@ -295,39 +312,40 @@
     def checkall(self):
         self.textEdit.setText('')
         self.update_data()
 
         self.checkpatent(False)
         self.replaceprj(False)
 
-    def check_and_change(self, doc, replace):
-        """
-        遍历word中的所有 paragraphs，在每一段中发现含有key 的内容，就替换为 value 。
-        （key 和 value 都是replace_dict中的键值对。）
-        """
-        for para in doc.paragraphs:
-            for i in range(len(para.runs)):
-                for key, value in replace.items():
-                    if key in para.runs[i].text:
-                        self.textEdit.append(key + "-->" + value)
-                        para.runs[i].text = para.runs[i].text.replace(key, value)
-        return doc
-
-    def replace_tables(self, doc, replace):
-        for table in doc.tables:
-            for row in table.rows:
-                for cell in row.cells:
-                    for para in cell.paragraphs:
-                        for i in range(len(para.runs)):
-                            # self.textEdit.append(">>>" + para.runs[i].text)
-                            for key, value in replace.items():
-                                if key in para.runs[i].text:
-                                    self.textEdit.append(key + "-->" + value)
-                                    para.runs[i].text = para.runs[i].text.replace(key, value)
-        return doc
+    def searchall(self):
+        self.textEdit.setText('')
+        self.update_data()
+        text, ok = QInputDialog.getText(self, "全项目查找",
+                                        "查找内容:", QLineEdit.Normal)
+        if ok and text:
+            for project in self.arr_prj:
+                # self.textEdit.append(project.p_order + ' 项目开始处理...')
+                checkr = CheckR()  # 已匹配条目数
+                doc_name = ''
+                try:
+                    doc_name = self.workdir + '/RD' + project.p_order + project.p_name + '.docx'
+                    document = Document(doc_name)
+                    checkr = checkr + self.findindoc(document, text)
+                    # if modify:
+                    #     document.save(doc_name)
+                except PackageNotFoundError:
+                    self.textEdit.append('Error打开文件错误：' + doc_name)
+                except PermissionError:
+                    self.textEdit.append('Error保存文件错误，可能是文件已被打开：' + doc_name)
+
+                prompt = project.p_order + ' 项目检查完成。 <font color="green"><b>' + str(
+                    checkr.match) + ' </b></font> 项匹配。'
+                if checkr.unmatch > 0:
+                    prompt = prompt + ' <font color="red"><b>' + str(checkr.unmatch) + ' </b></font> 项不匹配。'
+                self.textEdit.append(prompt)
 
     @staticmethod
     def clear_runs(runs):
         for i, run in enumerate(runs):
             if i > 0:
                 run.clear()
         return runs
@@ -346,134 +364,173 @@
             for j, row in enumerate(table.rows):
                 for k, cell in enumerate(row.cells):
                     for l, para in enumerate(cell.paragraphs):
                         self.textEdit.append(f'Table.{i} Row.{j} Cell{k} Para.{l} : ', para.text, sep='')
                         # for j, run in enumerate(para.runs):
                         #     self.textEdit.append(f'Para.{i} Run{j}: ', run.text, sep='')
 
-    def replace_comname(self, doc, prj):
+    def findindoc(self, doc, keyword):
         match = 0
+        for i, sect in enumerate(doc.sections):
+            for j, para in enumerate(sect.header.paragraphs):
+                if keyword in para.text:
+                    match = match + 1
+                    newstr = para.text.replace(keyword, f'<font color="red"><b>{keyword}</b></font>')
+                    self.textEdit.append(f'节.{i} 段.{j} : {newstr}')
+                # for k, run in enumerate(para.runs):
+                #     self.textEdit.append(f'Sec.{i} Para.{j} Run{k}: ', run.text, sep='')
+        for i, para in enumerate(doc.paragraphs):
+            if keyword in para.text:
+                match = match + 1
+                newstr = para.text.replace(keyword, f'<font color="red"><b>{keyword}</b></font>')
+                self.textEdit.append(f'段.{i} : {newstr}')
+                # for j, run in enumerate(para.runs):
+                #     self.textEdit.append(f'段.{i} Run{j}: ', run.text, sep='')
+        for i, table in enumerate(doc.tables):
+            for j, row in enumerate(table.rows):
+                for k, cell in enumerate(row.cells):
+                    for l, para in enumerate(cell.paragraphs):
+                        if keyword in para.text:
+                            match = match + 1
+                            newstr = para.text.replace(keyword, f'<font color="red"><b>{keyword}</b></font>')
+                            self.textEdit.append(f'表.{i} 行.{j} 列{k} 段.{l} : {newstr}')
+        return CheckR(match, 0)
+
+    def replace_comname(self, doc, prj):
+        match = unmatch = 0
         para = doc.sections[0].header.paragraphs[0]
         oldname = para.text.strip()
 
         if prj.p_comname in para.text:
-            match = match +1
+            match = match + 1
         else:
+            unmatch = unmatch + 1
             self.textEdit.append(oldname + ' ===> ' + prj.p_comname)
             # TODO 这个地方还有个问题， 先用临时凑合一下
             # found = False
             # for i, run in enumerate(para.runs):
             #     if found:
             #         run.clear()
             #     if run.text != '':
             #         run.text = '\t\t' + prj.p_comname
             #         found = True
             for i, run in enumerate(para.runs):
                 if run.text == oldname:
                     run.text = prj.p_comname
                     self.textEdit.append(oldname + ' ===> ' + prj.p_comname)
                     match = match + 1
-        match = match + self.check_replace(doc.paragraphs, oldname, prj.p_comname)
+        checkr = CheckR(match, unmatch) + self.check_replace(doc.paragraphs, oldname, prj.p_comname)
         for table in doc.tables:
             for row in table.rows:
                 for cell in row.cells:
-                    match = match + self.check_replace(cell.paragraphs, oldname, prj.p_comname)
+                    checkr = checkr + self.check_replace(cell.paragraphs, oldname, prj.p_comname)
 
         # 检查其他可能的未替换的内容，例如去掉深圳，有限公司等
         # TODO
 
-        return match
-
+        return checkr
 
     def first_table(self, doc, prj):
-        match = 0
+        match = unmatch = 0
         if doc.tables[0].rows[0].cells[0].paragraphs[0].text == '项目名称：':
             doc.tables[0].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[0].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
+        else:
+            unmatch = unmatch + 1
         if doc.tables[0].rows[1].cells[0].paragraphs[0].text == '项目编号：':
             doc.tables[0].rows[1].cells[1].paragraphs[0].runs[0].text = prj.p_start[0:4] + 'RD' + prj.p_order
             self.clear_runs(doc.tables[0].rows[1].cells[1].paragraphs[0].runs)
             match = match + 1
+        else:
+            unmatch = unmatch + 1
         if doc.tables[0].rows[2].cells[0].paragraphs[0].text == '项目负责人：':
             doc.tables[0].rows[2].cells[1].paragraphs[0].runs[0].text = prj.p_owner
             self.clear_runs(doc.tables[0].rows[2].cells[1].paragraphs[0].runs)
             match = match + 1
+        else:
+            unmatch = unmatch + 1
         if doc.tables[0].rows[3].cells[0].paragraphs[0].text == '项目周期：':
             doc.tables[0].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_start + '至' + prj.p_end
             self.clear_runs(doc.tables[0].rows[3].cells[1].paragraphs[0].runs)
             match = match + 1
-        return match
+        else:
+            unmatch = unmatch + 1
+        return CheckR(match, unmatch)
 
     def start_time(self, doc, prj):
-        match = self.check_replace(doc.paragraphs, '申请立项时间：\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
-                                   '申请立项时间：' + prj.p_start)
-        return match
+        return self.check_replace(doc.paragraphs, '申请立项时间：\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
+                                  '申请立项时间：' + prj.p_start)
 
     def second_table(self, doc, prj):
-        match = 0
+        match = unmatch = 0
         if doc.tables[1].rows[0].cells[0].paragraphs[0].text == '项目立项名称':
             doc.tables[1].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
+        else:
+            unmatch = unmatch + 1
 
-        match = match + self.check_replace(doc.tables[1].rows[1].cells[1].paragraphs,
-                                           '项目团队由(.*)人组成，项目实施周期为(.*)个月。',
-                                           '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
-        match = match + self.check_replace(doc.tables[1].rows[6].cells[1].paragraphs,
-                                           '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
-                                           prj.p_start + '至' + prj.p_end)
-        match = match + self.check_replace(doc.tables[1].rows[7].cells[1].paragraphs,
-                                           '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
+        checkr = CheckR(match, unmatch) + self.check_replace(doc.tables[1].rows[1].cells[1].paragraphs,
+                                                             '项目团队由(.*)人组成，项目实施周期为(.*)个月。',
+                                                             '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
+        checkr = checkr + self.check_replace(doc.tables[1].rows[6].cells[1].paragraphs,
+                                             '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
+                                             prj.p_start + '至' + prj.p_end)
+        checkr = checkr + self.check_replace(doc.tables[1].rows[7].cells[1].paragraphs,
+                                             '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
 
-        match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs,
-                                           '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
+        checkr = checkr + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs,
+                                             '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
         if prj.p_owner != 'None':
-            match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
-                                               '项目负责人：' + prj.p_owner)
+            checkr = checkr + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
+                                                 '项目负责人：' + prj.p_owner)
         if prj.p_rnd != 'None':
-            match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*',
-                                               '研发成员：' + prj.p_rnd)
-        match = match + self.check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
-                                           prj.p_start)
+            checkr = checkr + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*',
+                                                 '研发成员：' + prj.p_rnd)
+        checkr = checkr + self.check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
+                                             prj.p_start)
 
-        return match
+        return checkr
 
     def check_replace(self, paras, regex, dst):
-        match = 0
+        match = unmatch = 0
         for i, para in enumerate(paras):
             result = re.search(regex, para.text)
             if result is not None:
                 if result.group() != dst:
+                    unmatch = unmatch + 1
                     self.textEdit.append(str(result.group()) + ' ===> ' + dst)
                     para.runs[0].text = re.sub(regex, dst,
                                                para.text)
                     self.clear_runs(para.runs)
                 else:
                     match = match + 1
                 break  # 只替换一次就够用
-        return match
+        return CheckR(match, unmatch)
 
     def third_table(self, doc, prj):
-        match = 0
+        match = unmatch = 0
         if doc.tables[2].rows[0].cells[0].paragraphs[0].text == '项目名称':
             doc.tables[2].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[2].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
-        match = match + self.check_replace(doc.tables[2].rows[1].cells[1].paragraphs,
-                                           '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
-        match = match + self.check_replace(doc.tables[2].rows[2].cells[1].paragraphs,
-                                           '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
-                                           prj.p_start + '至' + prj.p_end)
+        else:
+            unmatch = unmatch + 1
+        checkr = CheckR(match, unmatch) + self.check_replace(doc.tables[2].rows[1].cells[1].paragraphs,
+                                                             '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
+        checkr = checkr + self.check_replace(doc.tables[2].rows[2].cells[1].paragraphs,
+                                             '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
+                                             prj.p_start + '至' + prj.p_end)
 
         if prj.p_owner != 'None':
             doc.tables[2].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_owner
             self.clear_runs(doc.tables[2].rows[3].cells[1].paragraphs[0].runs)
-            match = match + 1
-        return match
+            checkr = checkr + CheckR(1, 0)
+        return checkr
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
     sys.exit(app.exec())
```

### Comparing `docrobot-1.0.8/LICENSE` & `docrobot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.8/pyproject.toml` & `docrobot-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.8"
+version = "1.1.0"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.8/PKG-INFO` & `docrobot-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.8
+Version: 1.1.0
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

