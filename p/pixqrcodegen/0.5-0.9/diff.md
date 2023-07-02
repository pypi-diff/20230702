# Comparing `tmp/pixqrcodegen-0.5.tar.gz` & `tmp/pixqrcodegen-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixqrcodegen-0.5.tar", last modified: Sun Sep 18 18:40:26 2022, max compression
+gzip compressed data, was "pixqrcodegen-0.9.tar", last modified: Sun Jul  2 01:37:41 2023, max compression
```

## Comparing `pixqrcodegen-0.5.tar` & `pixqrcodegen-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2022-09-18 18:40:26.931711 pixqrcodegen-0.5/
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)     1070 2022-09-15 18:59:18.000000 pixqrcodegen-0.5/LICENSE.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)     2506 2022-09-18 18:40:26.931711 pixqrcodegen-0.5/PKG-INFO
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)     1909 2022-09-18 18:39:58.000000 pixqrcodegen-0.5/README.md
-drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2022-09-18 18:40:26.931711 pixqrcodegen-0.5/pixqrcodegen/
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)       28 2022-09-15 20:30:52.000000 pixqrcodegen-0.5/pixqrcodegen/__init__.py
--rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2936 2022-09-18 18:39:44.000000 pixqrcodegen-0.5/pixqrcodegen/pixqrcodegen.py
-drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2022-09-18 18:40:26.931711 pixqrcodegen-0.5/pixqrcodegen.egg-info/
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)     2506 2022-09-18 18:40:26.000000 pixqrcodegen-0.5/pixqrcodegen.egg-info/PKG-INFO
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)      273 2022-09-18 18:40:26.000000 pixqrcodegen-0.5/pixqrcodegen.egg-info/SOURCES.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)        1 2022-09-18 18:40:26.000000 pixqrcodegen-0.5/pixqrcodegen.egg-info/dependency_links.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)       21 2022-09-18 18:40:26.000000 pixqrcodegen-0.5/pixqrcodegen.egg-info/requires.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)       13 2022-09-18 18:40:26.000000 pixqrcodegen-0.5/pixqrcodegen.egg-info/top_level.txt
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)      107 2022-09-18 18:40:26.931711 pixqrcodegen-0.5/setup.cfg
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)      902 2022-09-18 18:40:12.000000 pixqrcodegen-0.5/setup.py
+drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-07-02 01:37:41.083161 pixqrcodegen-0.9/
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     1070 2022-09-15 18:59:18.000000 pixqrcodegen-0.9/LICENSE.txt
+-rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)     2654 2023-07-02 01:37:41.083161 pixqrcodegen-0.9/PKG-INFO
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2057 2023-06-01 15:06:22.000000 pixqrcodegen-0.9/README.md
+drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-07-02 01:37:41.079162 pixqrcodegen-0.9/pixqrcodegen/
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)       28 2022-09-15 20:30:52.000000 pixqrcodegen-0.9/pixqrcodegen/__init__.py
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2726 2023-07-02 01:36:25.000000 pixqrcodegen-0.9/pixqrcodegen/pixqrcodegen.py
+drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-07-02 01:37:41.083161 pixqrcodegen-0.9/pixqrcodegen.egg-info/
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2654 2023-07-02 01:37:41.000000 pixqrcodegen-0.9/pixqrcodegen.egg-info/PKG-INFO
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)      273 2023-07-02 01:37:41.000000 pixqrcodegen-0.9/pixqrcodegen.egg-info/SOURCES.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)        1 2023-07-02 01:37:41.000000 pixqrcodegen-0.9/pixqrcodegen.egg-info/dependency_links.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)       21 2023-07-02 01:37:41.000000 pixqrcodegen-0.9/pixqrcodegen.egg-info/requires.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)       13 2023-07-02 01:37:41.000000 pixqrcodegen-0.9/pixqrcodegen.egg-info/top_level.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)      107 2023-07-02 01:37:41.083161 pixqrcodegen-0.9/setup.cfg
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)      902 2023-07-02 01:37:34.000000 pixqrcodegen-0.9/setup.py
```

### Comparing `pixqrcodegen-0.5/LICENSE.txt` & `pixqrcodegen-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pixqrcodegen-0.5/PKG-INFO` & `pixqrcodegen-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixqrcodegen
-Version: 0.5
+Version: 0.9
 Summary: Gera a Payload do PIX e o QR Code
 Home-page: https://github.com/Alexsussa/pixqrcodegen
 Author: Alex Pinheiro
 License: MIT
 Keywords: qrcode,payload,qrcode-generator,pix,pix-payload-generator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,21 @@
 """Observação"""
 
 QR Code é gerado após a criação da Payload do Pix e salvo no diretório de desenvolvimento.
 
 ```
 # Importante
 
-Nenhum dos dados podem ter caracteres especiais como acentos ou "ç" e os valores monetários devem ser dividos por ponto (.) e não vírgula (,).
+Nenhum dos dados podem ter caracteres especiais como acentos ou "ç" ~~e os valores monetários devem ser dividos por ponto (.) e não vírgula (,).~~
 
-Exemplo:
+~~Exemplo:~~
+
+~~Valor incorreto: 50,00~~
+
+~~Valor correto: 50.00~~
 
-Valor incorreto: 50,00 
+Os valores monetários podem ser digitados tanto com ponto (.) quanto com vírgula (,).
+
+Exemplo:
 
-Valor correto: 50.00
+Valores corretos: 50.00 ou 50,00
```

### Comparing `pixqrcodegen-0.5/README.md` & `pixqrcodegen-0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -41,15 +41,21 @@
 """Observação"""
 
 QR Code é gerado após a criação da Payload do Pix e salvo no diretório de desenvolvimento.
 
 ```
 # Importante
 
-Nenhum dos dados podem ter caracteres especiais como acentos ou "ç" e os valores monetários devem ser dividos por ponto (.) e não vírgula (,).
+Nenhum dos dados podem ter caracteres especiais como acentos ou "ç" ~~e os valores monetários devem ser dividos por ponto (.) e não vírgula (,).~~
 
-Exemplo:
+~~Exemplo:~~
+
+~~Valor incorreto: 50,00~~
+
+~~Valor correto: 50.00~~
 
-Valor incorreto: 50,00 
+Os valores monetários podem ser digitados tanto com ponto (.) quanto com vírgula (,).
+
+Exemplo:
 
-Valor correto: 50.00
+Valores corretos: 50.00 ou 50,00
```

### Comparing `pixqrcodegen-0.5/pixqrcodegen/pixqrcodegen.py` & `pixqrcodegen-0.9/pixqrcodegen/pixqrcodegen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+
 import crcmod
 import qrcode
 import os
 
 
 class Payload():
     def __init__(self, nome, chavepix, valor, cidade, txtId, diretorio=''):
         
         self.nome = nome
         self.chavepix = chavepix
-        self.valor = valor
+        self.valor = valor.replace(',', '.')
         self.cidade = cidade
         self.txtId = txtId
         self.diretorioQrCode = diretorio
 
         self.nome_tam = len(self.nome)
         self.chavepix_tam = len(self.chavepix)
         self.valor_tam = len(self.valor)
         self.cidade_tam = len(self.cidade)
         self.txtId_tam = len(self.txtId)
 
-        self.merchantAccount_tam = f'0014BR.GOV.BCB.PIX01{self.chavepix_tam}{self.chavepix}'
-        if self.valor_tam <= 9:
-            self.transactionAmount_tam = f'0{self.valor_tam}{self.valor}'
-        else:
-            self.transactionAmount_tam = f'{self.valor_tam}{self.valor}'
-
-        if self.txtId_tam <= 9:
-            self.addDataField_tam = f'050{self.txtId_tam}{self.txtId}'
-        else:
-            self.addDataField_tam = f'05{self.txtId_tam}{self.txtId}'
+        self.merchantAccount_tam = f'0014BR.GOV.BCB.PIX01{self.chavepix_tam:02}{self.chavepix}'
+        self.transactionAmount_tam = f'{self.valor_tam:02}{float(self.valor):.2f}'
+
+        self.addDataField_tam = f'05{self.txtId_tam:02}{self.txtId}'
 
-        if self.nome_tam <= 9:
-            self.nome_tam = f'0{self.nome_tam}'
+        self.nome_tam = f'{self.nome_tam:02}'
 
-        if self.cidade_tam <= 9:
-            self.cidade_tam = f'0{self.cidade_tam}'
+        self.cidade_tam = f'{self.cidade_tam:02}'
 
         self.payloadFormat = '000201'
-        self.merchantAccount = f'26{len(self.merchantAccount_tam)}{self.merchantAccount_tam}'
+        self.merchantAccount = f'26{len(self.merchantAccount_tam):02}{self.merchantAccount_tam}'
         self.merchantCategCode = '52040000'
         self.transactionCurrency = '5303986'
         self.transactionAmount = f'54{self.transactionAmount_tam}'
         self.countryCode = '5802BR'
-        self.merchantName = f'59{self.nome_tam}{self.nome}'
-        self.merchantCity = f'60{self.cidade_tam}{self.cidade}'
-        self.addDataField = f'62{len(self.addDataField_tam)}{self.addDataField_tam}'
+        self.merchantName = f'59{self.nome_tam:02}{self.nome}'
+        self.merchantCity = f'60{self.cidade_tam:02}{self.cidade}'
+        self.addDataField = f'62{len(self.addDataField_tam):02}{self.addDataField_tam}'
         self.crc16 = '6304'
 
   
     def gerarPayload(self):
         self.payload = f'{self.payloadFormat}{self.merchantAccount}{self.merchantCategCode}{self.transactionCurrency}{self.transactionAmount}{self.countryCode}{self.merchantName}{self.merchantCity}{self.addDataField}{self.crc16}'
 
         self.gerarCrc16(self.payload)
 
     
     def gerarCrc16(self, payload):
         crc16 = crcmod.mkCrcFun(poly=0x11021, initCrc=0xFFFF, rev=False, xorOut=0x0000)
 
         self.crc16Code = hex(crc16(str(payload).encode('utf-8')))
 
-        self.crc16Code_formatado = str(self.crc16Code).replace('0x', '').upper()
+        self.crc16Code_formatado = str(self.crc16Code).replace('0x', '').upper().zfill(4)
 
         self.payload_completa = f'{payload}{self.crc16Code_formatado}'
 
         self.gerarQrCode(self.payload_completa, self.diretorioQrCode)
 
     
     def gerarQrCode(self, payload, diretorio):
```

### Comparing `pixqrcodegen-0.5/pixqrcodegen.egg-info/PKG-INFO` & `pixqrcodegen-0.9/pixqrcodegen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixqrcodegen
-Version: 0.5
+Version: 0.9
 Summary: Gera a Payload do PIX e o QR Code
 Home-page: https://github.com/Alexsussa/pixqrcodegen
 Author: Alex Pinheiro
 License: MIT
 Keywords: qrcode,payload,qrcode-generator,pix,pix-payload-generator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,21 @@
 """Observação"""
 
 QR Code é gerado após a criação da Payload do Pix e salvo no diretório de desenvolvimento.
 
 ```
 # Importante
 
-Nenhum dos dados podem ter caracteres especiais como acentos ou "ç" e os valores monetários devem ser dividos por ponto (.) e não vírgula (,).
+Nenhum dos dados podem ter caracteres especiais como acentos ou "ç" ~~e os valores monetários devem ser dividos por ponto (.) e não vírgula (,).~~
 
-Exemplo:
+~~Exemplo:~~
+
+~~Valor incorreto: 50,00~~
+
+~~Valor correto: 50.00~~
 
-Valor incorreto: 50,00 
+Os valores monetários podem ser digitados tanto com ponto (.) quanto com vírgula (,).
+
+Exemplo:
 
-Valor correto: 50.00
+Valores corretos: 50.00 ou 50,00
```

### Comparing `pixqrcodegen-0.5/setup.py` & `pixqrcodegen-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as rm:
     full_desc = rm.read()
 
 setup(
     name="pixqrcodegen",
-    version="0.5",
+    version="0.9",
     author="Alex Pinheiro",
     url="https://github.com/Alexsussa/pixqrcodegen",
     packages=['pixqrcodegen'],
     description="Gera a Payload do PIX e o QR Code",
     long_description=full_desc,
     long_description_content_type='text/markdown',
     python_requires=">= 3.6",
```

