# Comparing `tmp/kayle-0.5.8-py3-none-any.whl.zip` & `tmp/kayle-0.5.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14837 bytes, number of entries: 13
+Zip file size: 14950 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      225 b- defN 22-Dec-18 23:12 kayle/__init__.py
 -rw-rw-rw-  2.0 fat    45570 b- defN 23-Jan-12 18:33 kayle/match.py
 -rw-rw-rw-  2.0 fat      169 b- defN 22-Dec-18 23:12 kayle/ddragon/__init__.py
--rw-rw-rw-  2.0 fat     5165 b- defN 22-Dec-18 23:12 kayle/ddragon/champions.py
--rw-rw-rw-  2.0 fat    10659 b- defN 23-Jan-01 22:31 kayle/ddragon/factory.py
--rw-rw-rw-  2.0 fat     1156 b- defN 22-Dec-18 23:12 kayle/ddragon/items.py
--rw-rw-rw-  2.0 fat      906 b- defN 22-Dec-27 16:27 kayle/ddragon/maps.py
--rw-rw-rw-  2.0 fat     1793 b- defN 22-Dec-18 23:12 kayle/ddragon/runes.py
--rw-rw-rw-  2.0 fat     2057 b- defN 22-Dec-18 23:12 kayle/ddragon/summonerSpells.py
--rw-rw-rw-  2.0 fat      440 b- defN 23-Jan-12 18:34 kayle-0.5.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-12 18:34 kayle-0.5.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jan-12 18:34 kayle-0.5.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1003 b- defN 23-Jan-12 18:34 kayle-0.5.8.dist-info/RECORD
-13 files, 69255 bytes uncompressed, 13183 bytes compressed:  81.0%
+-rw-rw-rw-  2.0 fat     5165 b- defN 23-Jan-05 01:32 kayle/ddragon/champions.py
+-rw-rw-rw-  2.0 fat    11226 b- defN 23-Jan-08 15:51 kayle/ddragon/factory.py
+-rw-rw-rw-  2.0 fat     1156 b- defN 23-Jan-05 01:32 kayle/ddragon/items.py
+-rw-rw-rw-  2.0 fat      906 b- defN 23-Jan-05 01:32 kayle/ddragon/maps.py
+-rw-rw-rw-  2.0 fat     1793 b- defN 23-Jan-05 01:32 kayle/ddragon/runes.py
+-rw-rw-rw-  2.0 fat     2057 b- defN 23-Jan-05 01:32 kayle/ddragon/summonerSpells.py
+-rw-rw-rw-  2.0 fat      440 b- defN 23-Jan-16 13:55 kayle-0.5.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-16 13:55 kayle-0.5.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jan-16 13:55 kayle-0.5.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1003 b- defN 23-Jan-16 13:55 kayle-0.5.9.dist-info/RECORD
+13 files, 69822 bytes uncompressed, 13296 bytes compressed:  81.0%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: kayle/ddragon/runes.py
 Comment: 
 
 Filename: kayle/ddragon/summonerSpells.py
 Comment: 
 
-Filename: kayle-0.5.8.dist-info/METADATA
+Filename: kayle-0.5.9.dist-info/METADATA
 Comment: 
 
-Filename: kayle-0.5.8.dist-info/WHEEL
+Filename: kayle-0.5.9.dist-info/WHEEL
 Comment: 
 
-Filename: kayle-0.5.8.dist-info/top_level.txt
+Filename: kayle-0.5.9.dist-info/top_level.txt
 Comment: 
 
-Filename: kayle-0.5.8.dist-info/RECORD
+Filename: kayle-0.5.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kayle/ddragon/factory.py

```diff
@@ -60,14 +60,26 @@
         return self._summoners[version + language]
 
     def summonerFromId(self, summonerSpellId, version, language='en_US'):
         if summonerSpellId == '0' or summonerSpellId == 0:
             return DefaultMunch({"name":""})
         return self.summoners(version, language)[str(summonerSpellId)]
 
+    def summonerFromIdName(self, summonerName, version, language='en_US'):
+        if summonerName == "S12_SummonerTeleportUpgrade":
+            summonerName = "SummonerTeleport"
+        if "Smite" in summonerName:
+            summonerName = "SummonerSmite"
+        if "FlashPerksHextechFlashtraption" in summonerName:
+            summonerName = "SummonerFlash"
+        summs = self.summoners(version, language)
+        for summonerSpellId in summs:
+            if summs[summonerSpellId].id == summonerName:
+                return summs[summonerSpellId]
+
     def champion(self, champion, version, language='en_US', returnFormat='ddragonFactory'):
         if champion + version + language not in self._champions:
             url = "https://ddragon.leagueoflegends.com/cdn/{}/data/{}/champion/{}.json".format(
                 version, language,
                 champion
             )
             # print(url)
```

## Comparing `kayle-0.5.8.dist-info/RECORD` & `kayle-0.5.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 kayle/__init__.py,sha256=OSUfktu8xzx3NiFOKvI-H35A1uj67yCIGnYSi9ZEUls,225
 kayle/match.py,sha256=qSnwPQ1AUjrJv0fwzOIx7r4WHughTIYHY8U01Nvd-P4,45570
 kayle/ddragon/__init__.py,sha256=vaXRXQrkha3cDuR2mtTffnFFwTdYRRiCzk_bLJ6mIXU,169
 kayle/ddragon/champions.py,sha256=0QoxroAGQJeeIVS3JMWvdDadUmMh5fUTD1Cj-eyANvU,5165
-kayle/ddragon/factory.py,sha256=x5g1OwJi5c2gehr1a-bprQx_c_CIJmZxGYPyHIXW54s,10659
+kayle/ddragon/factory.py,sha256=lplLa0lAQTvjm80GucEKdE-taYACh_3A6z9WI0E3UZk,11226
 kayle/ddragon/items.py,sha256=e-_OxtA8DUdHnpuirN6Al9-QX8fpwrqYosXyLFmCWmU,1156
 kayle/ddragon/maps.py,sha256=0XT778iKXwNxeEmsJPvh07Qqu92bQJzBMVYDTP-Nj3M,906
 kayle/ddragon/runes.py,sha256=M8rSYD8F5m9mkMCYA9_6ZTpTv1nsVBnFROmD0tHttrI,1793
 kayle/ddragon/summonerSpells.py,sha256=TTCj7tb_ucCbk3e7KCZNS7I_K1NhSgFKM-qcHN8PGdI,2057
-kayle-0.5.8.dist-info/METADATA,sha256=2wmNzXm5Vqu6WdUlTb7R8fNSye9fZcB54YXYnvH8WBo,440
-kayle-0.5.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kayle-0.5.8.dist-info/top_level.txt,sha256=G-HDrTPbb1WxzqVBwlliO6rSG5mSQzvQVsjti6B9gKY,20
-kayle-0.5.8.dist-info/RECORD,,
+kayle-0.5.9.dist-info/METADATA,sha256=OC1R8a0SoVy-K9lPS9cMkiexHSXfcmUAAIhhmK5izRM,440
+kayle-0.5.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+kayle-0.5.9.dist-info/top_level.txt,sha256=G-HDrTPbb1WxzqVBwlliO6rSG5mSQzvQVsjti6B9gKY,20
+kayle-0.5.9.dist-info/RECORD,,
```

