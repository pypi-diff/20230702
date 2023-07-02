# Comparing `tmp/vocab-coverage-0.5.tar.gz` & `tmp/vocab-coverage-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocab-coverage-0.5.tar", last modified: Thu Jun 22 22:38:47 2023, max compression
+gzip compressed data, was "vocab-coverage-0.6.tar", last modified: Sun Jul  2 04:56:24 2023, max compression
```

## Comparing `vocab-coverage-0.5.tar` & `vocab-coverage-0.6.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-22 22:38:47.066887 vocab-coverage-0.5/
--rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.5/LICENSE
--rw-r--r--   0 tao        (502) staff       (20)    24281 2023-06-22 22:38:47.066715 vocab-coverage-0.5/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)    23456 2023-06-22 06:23:03.000000 vocab-coverage-0.5/README.md
--rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-22 22:38:47.066928 vocab-coverage-0.5/setup.cfg
--rw-r--r--   0 tao        (502) staff       (20)     1482 2023-06-22 22:35:32.000000 vocab-coverage-0.5/setup.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-22 22:38:47.065398 vocab-coverage-0.5/vocab_coverage/
--rw-r--r--   0 tao        (502) staff       (20)      170 2023-06-19 22:57:11.000000 vocab-coverage-0.5/vocab_coverage/__init__.py
--rw-r--r--   0 tao        (502) staff       (20)    11667 2023-06-22 18:50:50.000000 vocab-coverage-0.5/vocab_coverage/charsets.py
--rw-r--r--   0 tao        (502) staff       (20)     7331 2023-06-21 19:52:17.000000 vocab-coverage-0.5/vocab_coverage/draw.py
--rw-r--r--   0 tao        (502) staff       (20)     8296 2023-06-22 18:56:13.000000 vocab-coverage-0.5/vocab_coverage/embedding.py
--rw-r--r--   0 tao        (502) staff       (20)     2714 2023-06-19 23:08:26.000000 vocab-coverage-0.5/vocab_coverage/main.py
--rw-r--r--   0 tao        (502) staff       (20)     5285 2023-06-20 04:53:16.000000 vocab-coverage-0.5/vocab_coverage/model.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-22 22:38:47.066470 vocab-coverage-0.5/vocab_coverage.egg-info/
--rw-r--r--   0 tao        (502) staff       (20)    24281 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)      408 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 tao        (502) staff       (20)       55 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/entry_points.txt
--rw-r--r--   0 tao        (502) staff       (20)      125 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/requires.txt
--rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-07-02 04:56:24.030416 vocab-coverage-0.6/
+-rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.6/LICENSE
+-rw-r--r--   0 tao        (502) staff       (20)       30 2023-07-01 17:33:36.000000 vocab-coverage-0.6/MANIFEST.in
+-rw-r--r--   0 tao        (502) staff       (20)    35485 2023-07-02 04:56:24.030252 vocab-coverage-0.6/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)    34660 2023-07-02 04:32:24.000000 vocab-coverage-0.6/README.md
+-rw-r--r--   0 tao        (502) staff       (20)       38 2023-07-02 04:56:24.030466 vocab-coverage-0.6/setup.cfg
+-rw-r--r--   0 tao        (502) staff       (20)     1556 2023-07-02 04:54:38.000000 vocab-coverage-0.6/setup.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-07-02 04:56:24.029027 vocab-coverage-0.6/vocab_coverage/
+-rw-r--r--   0 tao        (502) staff       (20)      179 2023-07-01 16:39:12.000000 vocab-coverage-0.6/vocab_coverage/__init__.py
+-rw-r--r--   0 tao        (502) staff       (20)   319549 2023-06-16 08:24:01.000000 vocab-coverage-0.6/vocab_coverage/charsets.json
+-rw-r--r--   0 tao        (502) staff       (20)    11679 2023-06-26 16:57:52.000000 vocab-coverage-0.6/vocab_coverage/charsets.py
+-rw-r--r--   0 tao        (502) staff       (20)     5327 2023-07-01 16:39:15.000000 vocab-coverage-0.6/vocab_coverage/coverage.py
+-rw-r--r--   0 tao        (502) staff       (20)     7782 2023-06-26 18:05:18.000000 vocab-coverage-0.6/vocab_coverage/draw.py
+-rw-r--r--   0 tao        (502) staff       (20)    19432 2023-07-01 16:07:09.000000 vocab-coverage-0.6/vocab_coverage/embedding.py
+-rw-r--r--   0 tao        (502) staff       (20)    16153 2023-07-02 04:31:08.000000 vocab-coverage-0.6/vocab_coverage/generate.py
+-rw-r--r--   0 tao        (502) staff       (20)     3606 2023-07-01 17:52:08.000000 vocab-coverage-0.6/vocab_coverage/main.py
+-rw-r--r--   0 tao        (502) staff       (20)     3833 2023-07-01 17:17:46.000000 vocab-coverage-0.6/vocab_coverage/models.json
+-rw-r--r--   0 tao        (502) staff       (20)     2733 2023-07-02 04:32:04.000000 vocab-coverage-0.6/vocab_coverage/models_readme.json
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-07-02 04:56:24.029981 vocab-coverage-0.6/vocab_coverage.egg-info/
+-rw-r--r--   0 tao        (502) staff       (20)    35485 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)      540 2023-07-02 04:56:24.000000 vocab-coverage-0.6/vocab_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 tao        (502) staff       (20)        1 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 tao        (502) staff       (20)       55 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 tao        (502) staff       (20)      146 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/requires.txt
+-rw-r--r--   0 tao        (502) staff       (20)       15 2023-07-02 04:56:23.000000 vocab-coverage-0.6/vocab_coverage.egg-info/top_level.txt
```

### Comparing `vocab-coverage-0.5/LICENSE` & `vocab-coverage-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.5/setup.py` & `vocab-coverage-0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vocab-coverage',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=[
         'Pillow',
         'protobuf==3.20.0',
         'sentencepiece',
         'tiktoken',
         'torch',
         'transformers',
         'beautifulsoup4',
         'bs4',
         'pandas',
         'requests',
         'scikit-learn',
         'accelerate',
+        'openai',
+        'python-dotenv',
     ],
     description='语言模型中文识字率分析\nA Python package designed to perform coverage analysis on Chinese vocabulary for language models.',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
+    include_package_data=True,
     author='Tao Wang',
     author_email='twang2218@gmail.com',
     url='https://github.com/twang2218/vocab-coverage',
     license='Apache License 2.0',
     classifiers=[
         'Development Status :: 3 - Alpha',
         "Intended Audience :: Developers",
```

### Comparing `vocab-coverage-0.5/vocab_coverage/charsets.py` & `vocab-coverage-0.6/vocab_coverage/charsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
     adjusted_color = tuple(
         int(round(old_value * (1 - amount) + white * amount))
         for old_value in color
     )
     return adjusted_color
 
 class CharsetClassifier:
-    def __init__(self, charsets:dict, is_detail=False):
+    def __init__(self, charsets:dict, is_detailed=False):
         self.charsets = charsets
-        self.is_detail = is_detail
+        self.is_detailed = is_detailed
         self.palette = None
 
     @staticmethod
     def is_japanese_kana(word:str):
         word = word.strip()
         for character in word:
             unicode_value = ord(character)
@@ -199,15 +199,15 @@
         elif self.is_numeric(word):
             return '数字'
         elif self.is_japanese_kana(word):
             return '日文'
         elif self.is_korean(word):
             return '韩文'
         else:
-            if self.is_detail:
+            if self.is_detailed:
                 cats = [
                     '《通用规范汉字表》一级汉字',
                     '《通用规范汉字表》二级汉字',
                     '《通用规范汉字表》三级汉字',
                     '《常用國字標準字體表》甲表(增)',
                     '《常用國字標準字體表》乙表(增)',
                     '《Unicode中日韩统一表意文字》(增)',
@@ -239,15 +239,15 @@
             self.palette = palette.copy()
             for k, v in self.palette.items():
                 if isinstance(v, str):
                     self.palette[k] = ImageColor.getrgb(v)
             self.palette.update(prefix_palette)
             return self.palette
 
-        if self.is_detail:
+        if self.is_detailed:
             self.palette = {
                 '《通用规范汉字表》一级汉字': '#B04759',
                 '《通用规范汉字表》二级汉字': '#E76161',
                 '《通用规范汉字表》三级汉字': '#F99B7D',
                 '《常用國字標準字體表》甲表(增)': '#146C94',
                 '《常用國字標準字體表》乙表(增)': '#19A7CE',
                 '其他汉字': '#E893CF',
@@ -266,15 +266,15 @@
                 '英文': '#2E7D32',
                 '数字': '#01579B',
                 '其他': '#212121',
             }
         return self.palette
 
     def get_types(self):
-        if self.is_detail:
+        if self.is_detailed:
             return [
                 '《通用规范汉字表》一级汉字',
                 '《通用规范汉字表》二级汉字',
                 '《通用规范汉字表》三级汉字',
                 '《常用國字標準字體表》甲表(增)',
                 '《常用國字標準字體表》乙表(增)',
                 '其他汉字',
```

### Comparing `vocab-coverage-0.5/vocab_coverage/draw.py` & `vocab-coverage-0.6/vocab_coverage/draw.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,75 +118,85 @@
     image.save(filename)
 
 
 from vocab_coverage.charsets import CharsetClassifier
 import math
 
 # model: {model_name, model, tokenizer, vocab, embeddings, embeddings_2d}
-def draw_vocab_embeddings(model, charsets, width=8000, height=8000, is_detail=False, debug=False):
+# def draw_vocab_embeddings(model, charsets, width=8000, height=8000, is_detail=False, debug=False):
+def draw_vocab_embeddings(model_name:str, embeddings_2d:List[List[float]], vocab:List[str], charsets:List[str],
+                        embedding_type:str, width=8000, height=8000, is_detailed=False, debug=False):
+    vocab_size = len(vocab)
+
     # calculate image size, margin, etc.
     margin = int(width / 20)
     image_width = width + margin * (2+2) # outer + inner margin
     image_height = height + margin * (2+2+3) # outer + inner margin + banner
 
     # normalize embeddings
     scaler = MinMaxScaler()
-    embeddings_2d_norm = scaler.fit_transform(model['embeddings_2d'])
+    embeddings_2d_norm = scaler.fit_transform(embeddings_2d)
 
     # draw embeddings
     image = Image.new('RGB', (image_width, image_height), (255, 255, 255))
     draw = ImageDraw.Draw(image)
     draw.rectangle((margin, margin, width + (3*margin), height + (3*margin)), fill='#F0F0F0')
 
     # CharsetClassifier
-    classifier = CharsetClassifier(charsets=charsets, is_detail=is_detail)
+    classifier = CharsetClassifier(charsets=charsets, is_detailed=is_detailed)
     word_type_count = {k: 0 for k in classifier.get_types()}
     palette = classifier.get_palette(with_prefix_palette=True)
 
     if debug:
-        print(f"palette: {palette}")
-        print(f"draw embedding point: {len(model['vocab'])}")
+        # print(f"palette: {palette}")
+        print(f"[{model_name}]: draw embedding point: {vocab_size}")
 
     # draw embedding point
     # clip font size to [12, margin]
-    font_size = int(margin * 2000 / len(model['vocab']))
+    font_size = int(margin * 2000 / vocab_size)
     font_size = int(min(max(font_size, 12), margin))
     zh_font = get_chinese_font(font_size)
     if debug:
         print(f"font size: {font_size}, font: {zh_font.getname()}")
     for i, (x, y) in enumerate(embeddings_2d_norm):
-        word = model['vocab'][i]
+        word = vocab[i]
         word_type = classifier.get_word_type(word)
         word_type_count[word_type] += 1
 
         if word.startswith('##'):
             word_type = '##' + word_type
 
         c = palette[word_type]
 
         # draw text
         x = x * width + margin * 2
         y = y * height + margin * 2
         try:
             draw.text((x, y), word, fill=c, stroke_width=1, stroke_fill='#F0F0F0', font=zh_font)
         except Exception as e:
-            print(f"Warning: draw text error: {e}")
+            print(f"[{model_name}]: warning: draw text error: {e}")
 
     if debug:
-        print(f"token type counts: {word_type_count}")
+        print(f"[{model_name}]: token type counts: {word_type_count}")
     # draw model name
     font_size = int(margin / 2)
     draw.text((margin, image_height - (3*margin)),
-        f'[ {model["model_name"]} ]',
+        f'[ {model_name} ]',
         fill='#000000',
         font=get_english_font(font_size))
 
+    # draw embedding type
+    draw.text((margin, image_height - int(2.3*margin)),
+        f"[ {embedding_type} embeddings ]",
+        fill='#000000',
+        font=get_english_font(int(font_size/1.5)))
+
     # draw vocab size
-    draw.text((margin+font_size, image_height - int(2.3*margin)),
-        f'vocab size: {len(model["vocab"])}',
+    draw.text((margin, image_height - int(1.8*margin)),
+        "[ vocab size: {:,} ]".format(vocab_size),
         fill='#000000',
         font=get_english_font(int(font_size/1.5)))
 
     # draw legend
     font_size = int(margin / 3)
     box_width = int(margin / 2)
     column = 4
```

### Comparing `vocab-coverage-0.5/vocab_coverage/main.py` & `vocab-coverage-0.6/vocab_coverage/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,72 @@
 import os
 import sys
 import argparse
 import json
+from dotenv import load_dotenv
 
 if __name__ == "__main__":
     sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from vocab_coverage import model_check, embedding_analysis
+from vocab_coverage import coverage_analysis, embedding_analysis
 
 def main():
     parser = argparse.ArgumentParser()
 
     subcommands = parser.add_subparsers(dest='command')
 
-    cmdModel = subcommands.add_parser('model', help='模型汉字识字率分析')
-    cmdModel.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
-    cmdModel.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件（默认为 charset.json）")
-    cmdModel.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
-    cmdModel.add_argument("--debug", action='store_true', help="是否打印调试信息")
+    cmdCoverage = subcommands.add_parser('coverage', help='模型汉字识字率分析')
+    cmdCoverage.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
+    cmdCoverage.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为内置字符集文件）")
+    cmdCoverage.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
+    cmdCoverage.add_argument("--debug", action='store_true', help="是否打印调试信息")
 
     cmdEmbedding = subcommands.add_parser('embedding', help='词向量可视化分析')
     cmdEmbedding.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
-    cmdEmbedding.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件（默认为 charset.json）")
+    cmdEmbedding.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为内置字符集文件）")
     cmdEmbedding.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
-    cmdEmbedding.add_argument("--is_detail", action='store_true', help="是否对汉字进行详细分类（默认为 False）")
+    cmdEmbedding.add_argument("--is_detailed", action='store_true', help="是否对汉字进行详细分类（默认为 False）")
     cmdEmbedding.add_argument("--debug", action='store_true', help="是否打印调试信息（默认为 False）")
+    cmdEmbedding.add_argument("--skip_input_embeddings", action='store_true', help="不计算输入层的词向量")
+    cmdEmbedding.add_argument("--output_embeddings", action='store_true', help="计算输出层的词向量")
 
     cmdCharset = subcommands.add_parser('charset', help='生成用以统计识字率的字表文件')
-    cmdCharset.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件（默认为 charset.json）")
+    cmdCharset.add_argument("--charset_file", type=str, default="", help="用以统计识字率的字表文件（默认为内置字符集文件）")
 
     args = parser.parse_args()
 
-    if args.command == 'charset':
+    if len(args.charset_file) == 0:
+        # 使用内置字符集文件
+        charset_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'charsets.json')
+
+    if args.command == 'charsets':
         from vocab_coverage import generate_charsets
+        if len(args.charset_file) == 0:
+            print(f'请指定 --charset_file 参数')
+            exit(1)
         generate_charsets(args.charset_file)
         return
-    elif args.command == 'model':
-        charsets = json.load(open(args.charset_file, 'r'))
-        model_check(args.model_name, charsets, args.output_dir, args.debug)
+    elif args.command == 'coverage':
+        charsets = json.load(open(charset_file, 'r'))
+        coverage_analysis(args.model_name, charsets, args.output_dir, args.debug)
         return
     elif args.command == 'embedding':
-        charsets = json.load(open(args.charset_file, 'r'))
-        embedding_analysis(args.model_name, charsets, args.output_dir, args.is_detail, args.debug)
+        charsets = json.load(open(charset_file, 'r'))
+        etypes = []
+        if not args.skip_input_embeddings:
+            etypes.append('input')
+        if args.output_embeddings:
+            etypes.append('output')
+        embedding_analysis(
+            model_name=args.model_name,
+            charsets=charsets,
+            output_dir=args.output_dir,
+            embedding_type=etypes,
+            is_detailed=args.is_detailed,
+            debug=args.debug)
     else:
         parser.print_help()
         return
 
 if __name__ == "__main__":
+    load_dotenv()
     main()
```

### Comparing `vocab-coverage-0.5/vocab_coverage/model.py` & `vocab-coverage-0.6/vocab_coverage/coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 
 from transformers import AutoTokenizer
 
 from vocab_coverage.draw import draw_vocab_graph
 
-def model_check(model_name:str, charsets, output_dir:str, debug=False):
+def coverage_analysis(model_name:str, charsets, output_dir:str=None, debug=False):
     print("检查模型 {} 的字表".format(model_name))
     try:
         tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
     except Exception as e:
         if "LLaMATokenizer" in e.args[0]:
             from transformers import LlamaTokenizer
             tokenizer = LlamaTokenizer.from_pretrained(model_name, trust_remote_code=True)
@@ -106,15 +106,16 @@
                     print("[{}] 汉字({})被拆分了，编码为{}".format(tn, c, tokens_ids))
 
     # 统计显示
     for name, stats in charset_stats.items():
         print("字表{}：{}/{} ({:.2%})".format(name, stats['known'], stats['total'], float(stats['known'])/stats['total']))
 
     # 生成文件名
-    filename = model_name.replace('/', '_') + '.png'
-    filename = 'coverage_' + filename
+    filename = model_name.replace('/', '_') + '.coverage.png'
+    if output_dir is None:
+        output_dir = os.getcwd()
     output_dir = os.path.join(output_dir, 'coverage')
     os.makedirs(output_dir, exist_ok=True)
     filename = os.path.join(output_dir, filename)
 
     # 生成字表图
     draw_vocab_graph(model_name, charset_stats, tokenizer.vocab_size, filename, width=150)
```

