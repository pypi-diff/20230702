# Comparing `tmp/pydatawork-0.17.2.0.tar.gz` & `tmp/pydatawork-0.17.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.2.0.tar", last modified: Sat Jul  1 18:03:58 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.2.1.tar", last modified: Sun Jul  2 07:21:16 2023, max compression
```

## Comparing `pydatawork-0.17.2.0.tar` & `pydatawork-0.17.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15838 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12159 2023-07-01 18:02:42.000000 pydatawork-0.17.2.0/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15838 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    32580 2023-07-01 17:10:17.000000 pydatawork-0.17.2.0/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-01 18:03:58.000000 pydatawork-0.17.2.0/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-01 18:03:28.000000 pydatawork-0.17.2.0/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15838 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12159 2023-07-01 18:02:42.000000 pydatawork-0.17.2.1/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15838 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    32701 2023-07-02 06:25:14.000000 pydatawork-0.17.2.1/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-02 07:20:38.000000 pydatawork-0.17.2.1/setup.py
```

### Comparing `pydatawork-0.17.2.0/PKG-INFO` & `pydatawork-0.17.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.2.0
+Version: 0.17.2.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.2.0/README.md` & `pydatawork-0.17.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.2.0/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.2.1/pydatawork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.2.0
+Version: 0.17.2.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.2.0/pydatawork.py` & `pydatawork-0.17.2.1/pydatawork.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import shutil
 import re
 import datetime
 import random
 import time
 
 
+# others
+
 # def break_words(stuff):
 #     """This function will break up words for us."""
 #     words = stuff.split(' ')
 #     return words
 
 # def sort_words(words):
 #     """Sorts the words.""" # 文档字符串，是注释的一种
@@ -44,293 +46,142 @@
 # def print_first_and_last_sorted(sentence):
 #     """Sorts the words then prints the first and last one."""
 #     words = sort_sentence(sentence)
 #     print_first_word(words)
 #     print_last_word(words)
 
 
+# 维护
+
+# 折叠：ctrl + k , ctrl + 1
+# 展开：ctrl + k , ctrl + j
+
+
 # get help
 def hello_jkzhou():
     """If you need help or have a better idea, send me an e-mail."""
     print("如果需要帮助，可以给我发邮件: zhouqiling.bjfu@foxmail.com")
     print("也可以描述你的需求，给pydatawork提一个功能建议：\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
 
 
 
-# get a card
-def current_folder_name(path):
-    """
-    path:一个路径，可以是文件夹路径，也可以是文件路径
-    结果：返回current_folder_name
-    """
-    # 判断路径是文件夹路径还是文件路径
-    if os.path.isdir(path):
-        # 如果是文件夹路径
-        current_folder_name = os.path.basename(path)
-    else:
-        # 如果是文件路径
-        current_folder_name = os.path.basename(os.path.dirname(path))
-    return current_folder_name
 
 
 
-def file_name(path):
-    """
-    path:一个路径，可以是文件夹路径，也可以是文件路径
-    结果：返回file_name,当path为文件夹路径值，返回的值为空值
-    """
-    # 判断路径是文件夹路径还是文件路径
-    if os.path.isdir(path):
-        # 如果是文件夹路径
-        file_name = None
-    else:
-        # 如果是文件路径
-        file_name = os.path.basename(path)
-    return file_name
+# Basic Functions
 
 
-# get a program
-def get_weibo(path,id,weibo_name):
+def copy_files_by_keyword(raw_data_path,working_path):
     """
-    path: 内容存放路径
-    id: 微博id
-    weibo_name: 内容存放路径下文件夹的名字
-
-    示例：获取梅西的微博id，获取其微博内容
-
-    import pydatawork as dw 
-
-    path="/home/Desktop/pydatawork"
-    id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
-    weibo_name="mx"
-
-    dw.get_weibo(path,id,weibo_name)
-
+    raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
+    working_path：工作路径，提取出来的文件将存放到该路径。
+    keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
+    目标：根据文件名中的关键词复制文件。
     """
-    path = path
-    id = id # 在微博上获取
-
-    proxy_addr = "122.241.72.191:808"
-    weibo_name = weibo_name # 可以自定义名字
-
-
-    def use_proxy(url, proxy_addr):
-        req = urllib.request.Request(url)
-        req.add_header("User-Agent",
-                    "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2623.221 Safari/537.36 SE 2.X MetaSr 1.0")
-        proxy = urllib.request.ProxyHandler({'http': proxy_addr})
-        opener = urllib.request.build_opener(proxy, urllib.request.HTTPHandler)
-        urllib.request.install_opener(opener)
-        data = urllib.request.urlopen(req).read().decode('utf-8', 'ignore')
-        return data
-
-
-    def get_containerid(url):
-        data = use_proxy(url, proxy_addr)
-        content = json.loads(data).get('data')
-        for data in content.get('tabsInfo').get('tabs'):
-            if (data.get('tab_type') == 'weibo'):
-                containerid = data.get('containerid')
-        return containerid
-
-
-    def get_userInfo(id):
-        url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id
-        data = use_proxy(url, proxy_addr)
-        content = json.loads(data).get('data')
-        profile_image_url = content.get('userInfo').get('profile_image_url')
-        description = content.get('userInfo').get('description')
-        profile_url = content.get('userInfo').get('profile_url')
-        verified = content.get('userInfo').get('verified')
-        guanzhu = content.get('userInfo').get('follow_count')
-        name = content.get('userInfo').get('screen_name')
-        fensi = content.get('userInfo').get('followers_count')
-        gender = content.get('userInfo').get('gender')
-        urank = content.get('userInfo').get('urank')
-        print("微博昵称：" + name + "\n" + "微博主页地址：" + profile_url + "\n" + "微博头像地址：" + profile_image_url + "\n" + "是否认证：" + str(verified) + "\n" + "微博说明：" + description + "\n" + "关注人数：" + str(guanzhu) + "\n" + "粉丝数：" + str(fensi) + "\n" + "性别：" + gender + "\n" + "微博等级：" + str(urank) + "\n")
 
+    # 原始数据文件夹
+    raw_data_path = raw_data_path
+    # 给定工作路径，或基础路径，用于制作结果文件夹路径
+    working_path = working_path
 
-    def get_weibo(id, file):
-        global pic_num
-        pic_num = 0
-        i = 1
-        while True:
-            url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id
-            weibo_url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id + '&containerid=' + get_containerid(url) + '&page=' + str(i)
-            try:
-                data = use_proxy(weibo_url, proxy_addr)
-                content = json.loads(data).get('data')
-                cards = content.get('cards')
-                if (len(cards) > 0):
-                    for j in range(len(cards)):
-                        print("-----正在爬取第" + str(i) + "页，第" + str(j) + "条微博------")
-                        card_type = cards[j].get('card_type')
-                        if (card_type == 9):
-                            mblog = cards[j].get('mblog')
-                            attitudes_count = mblog.get('attitudes_count')
-                            comments_count = mblog.get('comments_count')
-                            created_at = mblog.get('created_at')
-                            reposts_count = mblog.get('reposts_count')
-                            scheme = cards[j].get('scheme')
-                            text = mblog.get('text')
-                            if mblog.get('pics') != None:
-                                # print(mblog.get('original_pic'))
-                                # print(mblog.get('pics'))
-                                pic_archive = mblog.get('pics')
-                                for _ in range(len(pic_archive)):
-                                    pic_num += 1
-                                    print(pic_archive[_]['large']['url'])
-                                    imgurl = pic_archive[_]['large']['url']
-                                    img = requests.get(imgurl)
-                                    # f = open(path + weibo_name + '\\' + str(pic_num) + str(imgurl[-4:]),'ab')  # 存储图片，多媒体文件需要参数b（二进制文件）# 原始代码
-                                    f = open(os.path.join(path, weibo_name, str(pic_num) + str(imgurl[-4:])), 'ab') # 存储图片，多媒体文件需要参数b（二进制文件）
-                                    f.write(img.content)  # 多媒体存储content
-                                    f.close()
+    # 根据keyword制作目标路径——复制文件存放的位置
+    keyword = str(input("请输入要复制的文件包含的关键词:\n"))
 
-                            with open(file, 'a', encoding='utf-8') as fh:
-                                fh.write("----第" + str(i) + "页，第" + str(j) + "条微博----" + "\n")
-                                fh.write("微博地址：" + str(scheme) + "\n" + "发布时间：" + str(
-                                    created_at) + "\n" + "微博内容：" + text + "\n" + "点赞数：" + str(
-                                    attitudes_count) + "\n" + "评论数：" + str(comments_count) + "\n" + "转发数：" + str(
-                                    reposts_count) + "\n")
-                    i += 1
-                else:
-                    break
-            except Exception as e:
-                print(e)
-                i += 1  # 添加这一行
-                pass
+    # 判断结果文件夹是否已存在，不依赖上一步，如果此处发现目标文件夹不存在，可以现场新建一个
+    result_path = working_path + "/" + str(keyword)
+    if os.path.exists(result_path) == False:
+        os.mkdir(result_path)
 
-    # # 在指定路径下，先建立一个名为weibo的文件夹
-    # if os.path.isdir(os.path.join(path,"weibo")):
-    #     pass
-    # else:
-    #     os.mkdir(os.path.join(path,"weibo"))
+    # 提取raw_path中的文件列表，获取列表里面的文件，再根据文件名制作文件当前的完整路径——这一串操作都是为了制作路径
+    every_file_list_path = os.listdir(raw_data_path)
+    for i in every_file_list_path:
+        file_path = os.path.join(raw_data_path, i)  # 使用os.path.join()函数拼接路径
+        if os.path.isfile(file_path):  # 判断是否为文件
+            if str(keyword) in i:
+                print(f"找到名称中包括 {keyword} 的文件")
+                shutil.copy(file_path, result_path)
+                print(f"copying: {i} to {result_path}")
+            else:
+                continue 
 
-    if os.path.isdir(os.path.join(path,weibo_name)):
-        pass
-    else:
-        os.mkdir(os.path.join(path,weibo_name))
-    file = os.path.join(path, weibo_name, weibo_name + ".txt")
+    print(f"名称中包括 {keyword} 的文件已提取（复制）完毕") 
 
-    get_userInfo(id)
-    get_weibo(id, file)
-    print("微博数据获取完毕")
-    # 该程序最初来源：http://www.omegaxyz.com/2018/02/13/python_weibo/
 
 
 
-def rename_folder_numeric_serialize(path):
+def move_files_by_keyword(raw_data_path,working_path):
     """
-    path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+    raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
+    working_path：工作路径，提取出来的文件将存放到该路径。
+    keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
+    目标：根据文件名中的关键词移动文件。
     """
 
-    # 定义一个函数，将输入的字符串按照数字和非数字的部分进行分割，并将数字部分转换为整数
-    def split_key(s): # 【一个字符串一个字符串处理】
-        parts = [] # 初始化一个空列表，用于存储分割后的字符串
-        current_part = "" # 初始化一个空字符串，用于存储当前正在处理的部分
-        for c in s: # 遍历字符串中的每个字符
-            if c.isalnum(): # 如果当前字符是字母或数字
-                current_part += c # 将其添加到 current_part 变量中
-            else: # 如果当前字符是非字母和数字的符号
-                if current_part: # 如果 current_part 不为空
-                    if current_part.isdigit(): # 如果 current_part 是数字
-                        current_part = int(current_part) # 将其转换为整数
-                    parts.append(current_part) # 将 current_part 添加到 parts 列表中
-                    current_part = "" # 将 current_part 重置为空字符串
-        if current_part: # 如果 current_part 不为空
-            if current_part.isdigit(): # 如果 current_part 是数字
-                current_part = int(current_part) # 将其转换为整数
-            parts.append(current_part) # 将 current_part 添加到 parts 列表中
-            # print(parts)
-            # exit()
-        return parts # 返回分割后的字符串列表
+    # 原始数据文件夹
+    raw_data_path = raw_data_path
+    # 给定工作路径，或基础路径，用于制作结果文件夹路径
+    working_path = working_path
 
-        
-    # 定义文件夹路径
-    images_path = path
+    # 根据keyword制作目标路径——复制文件存放的位置
+    keyword = str(input("请输入要移动的文件包含的关键词:\n"))
 
-    # 获取images_path下的所有子文件夹
-    subfolders = [f.path for f in os.scandir(images_path) if f.is_dir()]
+    # 判断结果文件夹是否已存在，不依赖上一步，如果此处发现目标文件夹不存在，可以现场新建一个
+    result_path = working_path + "/" + str(keyword)
+    if os.path.exists(result_path) == False:
+        os.mkdir(result_path)
 
-    # 对子文件夹按名字进行递增排序 @ 知识卡片 键函数。把subfolders中的每个元素，传给split_key按规则进行处理，并返回一个键，按返回的键进行排序。
-    subfolders.sort(key=split_key)
+    # 提取raw_path中的文件列表，获取列表里面的文件，再根据文件名制作文件当前的完整路径——这一串操作都是为了制作路径
+    every_file_list_path = os.listdir(raw_data_path)
+    for i in every_file_list_path:
+        file_path = os.path.join(raw_data_path, i)  # 使用os.path.join()函数拼接路径
+        if os.path.isfile(file_path):  # 判断是否为文件
+            if str(keyword) in i:
+                print(f"找到名称中包括 {keyword} 的文件")
+                file_path = raw_data_path + "/" + i
+                shutil.move(file_path, result_path)
+                print(f"moving: {i} to {result_path}")
+            else:
+                continue 
 
-    # 对排序后的子文件夹从1开始序列化，序列化的值加在原文件名末尾，以_进行拼接
-    for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化 @ 知识卡片
-        new_name = f"{folder}_{i}" # 将序列化的值加在原文件名末尾，以_进行拼接
-        os.rename(folder, new_name) # 重命名文件夹 @ 知识卡片
-        print(os.path.basename(new_name)) # 打印重命名后的文件夹名字，不包括路径
+    print(f"名称中包括 {keyword} 的文件已提取（移动）完毕") 
 
 
 
-def obsidian_move_md_or_canvas_linked_images(images_path,folder_path,target_folder):
+
+def current_folder_name(path):
     """
-    提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
-    需要指定三个路径：
-    images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
-    folder_path:待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去
-    target_folder:提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片
-    执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+    path:一个路径，可以是文件夹路径，也可以是文件路径
+    结果：返回current_folder_name
     """
+    # 判断路径是文件夹路径还是文件路径
+    if os.path.isdir(path):
+        # 如果是文件夹路径
+        current_folder_name = os.path.basename(path)
+    else:
+        # 如果是文件路径
+        current_folder_name = os.path.basename(os.path.dirname(path))
+    return current_folder_name
 
-    # 001-图片文件夹:原始库的附件文件夹路径
-    images_path = images_path
-    # 002-文件夹路径：准备移动归档的文件夹，里面包含.md和.canvas格式的文件
-    folder_path = folder_path
-    # 003-图片移动的目标文件夹：通常，在002中建立一个文件夹，用于存放图片即可
-    target_folder = target_folder
 
-    for root, dirs, files in os.walk(folder_path):
-        for file in files:
-            if file.endswith(".md"):
-            # 将md文件打印出来
-                print(file)
-            # 处理markdown文档
-                with open(os.path.join(root, file), "r", encoding="utf-8") as f:
-                    content = f.read()
-                    # 查找文档中的图片
-                    images = re.findall(r"\!\[\[(.*?)\]\]", content) # @@知识卡片 正则匹配
-                    # exit()
-                    for image_name in images:
-                        # 在images文件夹中查找对应图片
-                        for image_root, _, image_files in os.walk(images_path):
-                            if image_name in image_files:
-                                # 移动图片到指定文件夹
-                                shutil.move(os.path.join(image_root, image_name), os.path.join(target_folder, image_name))
-                                # 打印移动过程
-                                print(f"moving:{os.path.join(image_root, image_name)}--->{os.path.join(target_folder, image_name)}")
-            # exit()
 
-            # 处理canvas文档
-            elif file.endswith(".canvas"):
-                # 将canvas文件打印出来
-                print(file)
-                with open(os.path.join(root, file), "r", encoding="utf-8") as f:
-                    content = f.read() # @知识卡片 不必非用json的读取方式
-                    # 查找文档中的图片
-                    # images = re.findall(r'"file":"(.*?\.png)"', content) # @知识卡片 匹配形如"file":"Pasted image 20230531214326.png"的字符串，得到的是绝对路径
-                    images = re.findall(r'"file":"(.*?)"', content) # @知识卡片 匹配形如"file":"Pasted image 20230531214326.png"的字符串，得到的是绝对路径。不用指定png、jpeg等格式。
-                    # print(images)
-                    for file_path in images:
-                        # print(file_path)
-                        image_name = os.path.basename(file_path) #  @知识卡片 从绝对路径中提取文件名。Pasted image 20230531214326.png
-                        # 在images文件夹中查找对应图片
-                        for image_root, _, image_files in os.walk(images_path):
-                            if image_name in image_files:
-                                # 移动图片到指定文件夹
-                                shutil.move(os.path.join(image_root, image_name), os.path.join(target_folder, image_name))
-                                # 打印移动过程
-                                print(f"moving:{os.path.join(image_root, image_name)}--->{os.path.join(target_folder, image_name)}")
 
-    # 统计附件整理情况
-    images_list = os.listdir(target_folder)
-    num_images = len(images_list)
+def file_name(path):
+    """
+    path:一个路径，可以是文件夹路径，也可以是文件路径
+    结果：返回file_name,当path为文件夹路径值，返回的值为空值
+    """
+    # 判断路径是文件夹路径还是文件路径
+    if os.path.isdir(path):
+        # 如果是文件夹路径
+        file_name = None
+    else:
+        # 如果是文件路径
+        file_name = os.path.basename(path)
+    return file_name
 
-    print(f"\n已整理{num_images}个附件！")
 
 
 
 def move_all_files(folder_path, target_folder, file_type_list):
     """
     folder_path:待整理文件夹，可包含多层级子文件夹
     target_folder:目标文件夹
@@ -469,14 +320,194 @@
                     print(f"Copying {file} to {target_folder}")
                     shutil.copy(file_path, target_folder)
             else:
                 continue
 
 
 
+def rename_folder_numeric_serialize(path):
+    """
+    path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+    """
+
+    # 定义一个函数，将输入的字符串按照数字和非数字的部分进行分割，并将数字部分转换为整数
+    def split_key(s): # 【一个字符串一个字符串处理】
+        parts = [] # 初始化一个空列表，用于存储分割后的字符串
+        current_part = "" # 初始化一个空字符串，用于存储当前正在处理的部分
+        for c in s: # 遍历字符串中的每个字符
+            if c.isalnum(): # 如果当前字符是字母或数字
+                current_part += c # 将其添加到 current_part 变量中
+            else: # 如果当前字符是非字母和数字的符号
+                if current_part: # 如果 current_part 不为空
+                    if current_part.isdigit(): # 如果 current_part 是数字
+                        current_part = int(current_part) # 将其转换为整数
+                    parts.append(current_part) # 将 current_part 添加到 parts 列表中
+                    current_part = "" # 将 current_part 重置为空字符串
+        if current_part: # 如果 current_part 不为空
+            if current_part.isdigit(): # 如果 current_part 是数字
+                current_part = int(current_part) # 将其转换为整数
+            parts.append(current_part) # 将 current_part 添加到 parts 列表中
+            # print(parts)
+            # exit()
+        return parts # 返回分割后的字符串列表
+        
+    # 定义文件夹路径
+    images_path = path
+
+    # 获取images_path下的所有子文件夹
+    subfolders = [f.path for f in os.scandir(images_path) if f.is_dir()]
+
+    # 对子文件夹按名字进行递增排序 @ 知识卡片 键函数。把subfolders中的每个元素，传给split_key按规则进行处理，并返回一个键，按返回的键进行排序。
+    subfolders.sort(key=split_key)
+
+    # 对排序后的子文件夹从1开始序列化，序列化的值加在原文件名末尾，以_进行拼接
+    for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化 @ 知识卡片
+        new_name = f"{folder}_{i}" # 将序列化的值加在原文件名末尾，以_进行拼接
+        os.rename(folder, new_name) # 重命名文件夹 @ 知识卡片
+        print(os.path.basename(new_name)) # 打印重命名后的文件夹名字，不包括路径
+
+
+
+
+
+
+
+
+# Data Processing
+
+
+def game_number_guessing(number=100):
+    """
+    游戏规则：指定一个整数，确定数字的范围；根据提示猜数字，直到猜中。
+    number:大于1的整数，用于指定数字的范围，默认100，说明要猜的数字在100以内。
+    用法1：若不设定参数，可以写成 game_number_guessing() ，这时默认值为100。
+    用法2：自定义参数，可以写成 game_number_guessing(number=200)，这时，数字范围设定为在200以内。
+    """
+
+    # 自定义数字的范围，不局限于100以内
+    # x = int(input("输入一个数字，限定一个范围："))
+    x = int(number)
+
+    # 每次程序运行执行该行代码的时候，都会产生一个 指定范围内 的随机整数，并赋值给 answer 变量
+    answer = random.randint(1, x)
+
+    # 游戏设置
+    print("\nloading...")
+    time.sleep(0.5)
+    print("猜数字游戏加载中")
+    time.sleep(1)
+    print("ok...")
+    time.sleep(0.5)
+    print("加载完毕")
+    time.sleep(0.5)
+    print("start...")
+    time.sleep(0.5)
+    print("游戏已开局")
+    time.sleep(0.5)
+    user = input("设定你的游戏角色名字(若暂不设定，可按回车跳过)：")
+    if user:
+        print("角色名设定完毕...")
+        time.sleep(0.5)
+        print("gogogo...")
+        time.sleep(0.5)
+    else:
+        print("skiping...")
+        time.sleep(0.5)
+
+    num = 1
+    while True:
+
+        aa = int(input("\n输入答案："))
+        time.sleep(0.25)
+
+        if aa == answer:
+            print("猜对了！")
+            break
+        elif aa < answer:
+            print("大一点")
+        else:
+            print("小一点")
+        num = num + 1
+    
+    # 输出结果
+    if user:
+        print(f"\nhi，{user}，你一共猜了{num}次。")
+    else:
+        print(f"\nhi，无名氏，你一共猜了{num}次。")
+
+
+
+def obsidian_move_md_or_canvas_linked_images(images_path,folder_path,target_folder):
+    """
+    提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+    需要指定三个路径：
+    images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
+    folder_path:待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去
+    target_folder:提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片
+    执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+    """
+
+    # 001-图片文件夹:原始库的附件文件夹路径
+    images_path = images_path
+    # 002-文件夹路径：准备移动归档的文件夹，里面包含.md和.canvas格式的文件
+    folder_path = folder_path
+    # 003-图片移动的目标文件夹：通常，在002中建立一个文件夹，用于存放图片即可
+    target_folder = target_folder
+
+    for root, dirs, files in os.walk(folder_path):
+        for file in files:
+            if file.endswith(".md"):
+            # 将md文件打印出来
+                print(file)
+            # 处理markdown文档
+                with open(os.path.join(root, file), "r", encoding="utf-8") as f:
+                    content = f.read()
+                    # 查找文档中的图片
+                    images = re.findall(r"\!\[\[(.*?)\]\]", content) # @@知识卡片 正则匹配
+                    # exit()
+                    for image_name in images:
+                        # 在images文件夹中查找对应图片
+                        for image_root, _, image_files in os.walk(images_path):
+                            if image_name in image_files:
+                                # 移动图片到指定文件夹
+                                shutil.move(os.path.join(image_root, image_name), os.path.join(target_folder, image_name))
+                                # 打印移动过程
+                                print(f"moving:{os.path.join(image_root, image_name)}--->{os.path.join(target_folder, image_name)}")
+            # exit()
+
+            # 处理canvas文档
+            elif file.endswith(".canvas"):
+                # 将canvas文件打印出来
+                print(file)
+                with open(os.path.join(root, file), "r", encoding="utf-8") as f:
+                    content = f.read() # @知识卡片 不必非用json的读取方式
+                    # 查找文档中的图片
+                    # images = re.findall(r'"file":"(.*?\.png)"', content) # @知识卡片 匹配形如"file":"Pasted image 20230531214326.png"的字符串，得到的是绝对路径
+                    images = re.findall(r'"file":"(.*?)"', content) # @知识卡片 匹配形如"file":"Pasted image 20230531214326.png"的字符串，得到的是绝对路径。不用指定png、jpeg等格式。
+                    # print(images)
+                    for file_path in images:
+                        # print(file_path)
+                        image_name = os.path.basename(file_path) #  @知识卡片 从绝对路径中提取文件名。Pasted image 20230531214326.png
+                        # 在images文件夹中查找对应图片
+                        for image_root, _, image_files in os.walk(images_path):
+                            if image_name in image_files:
+                                # 移动图片到指定文件夹
+                                shutil.move(os.path.join(image_root, image_name), os.path.join(target_folder, image_name))
+                                # 打印移动过程
+                                print(f"moving:{os.path.join(image_root, image_name)}--->{os.path.join(target_folder, image_name)}")
+
+    # 统计附件整理情况
+    images_list = os.listdir(target_folder)
+    num_images = len(images_list)
+
+    print(f"\n已整理{num_images}个附件！")
+
+
+
+
 def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
     """
     函数设计：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
     original_bookmarks_path:一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
     result_path:一个路径，用于存放最终结果。
     """
 
@@ -510,15 +541,14 @@
 
         print(f"原始json中书签的个数: {num_original}")
         print(f"去重后的新书签数量: {num_new}")
         print(f"重复书签数量: {num_duplicates}")
 
         return new
 
-
     # json文件合并 @知识卡片 两个数据格式相同的字典合并
     def merge_json_files(original_bookmarks_path, result_path):
         data = {"bookmarks": [], "categories": []}
         for file_name in os.listdir(original_bookmarks_path):
             if file_name.endswith('.json'):
                 file_path = os.path.join(original_bookmarks_path, file_name)
                 with open(file_path, 'r') as f:
@@ -529,32 +559,162 @@
         # 合并结果存为：temp-surfing-bookmark.json
         with open(os.path.join(result_path, "temp-surfing-bookmark.json"), 'w') as f:
             json.dump(data, f, ensure_ascii=False, indent=2)
 
         print(
             f"Merged {len(os.listdir(original_bookmarks_path))} files into {result_path}")
 
-
     # 调用
     merge_json_files(original_bookmarks_path, result_path)
 
 
     # 合并后再去重一次:单个去重，得到 surfing-bookmark.json
     final_bookmarks = get_no_duplicates_bookmarks(os.path.join(
         result_path, "temp-surfing-bookmark.json"))  # final_bookmarks是一个完整的标签内容
 
     with open(os.path.join(result_path, "surfing-bookmark.json"), 'w') as f:
         json.dump(final_bookmarks, f, indent=2,
                 ensure_ascii=False)  # 这里写final_bookmarks
 
-
     print("书签合并与去重完毕！")
 
 
 
+
+def get_weibo(path,id,weibo_name):
+    """
+    path: 内容存放路径
+    id: 微博id
+    weibo_name: 内容存放路径下文件夹的名字
+
+    示例：获取梅西的微博id，获取其微博内容
+
+    import pydatawork as dw 
+
+    path="/home/Desktop/pydatawork"
+    id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
+    weibo_name="mx"
+
+    dw.get_weibo(path,id,weibo_name)
+
+    """
+    path = path
+    id = id # 在微博上获取
+
+    proxy_addr = "122.241.72.191:808"
+    weibo_name = weibo_name # 可以自定义名字
+
+    def use_proxy(url, proxy_addr):
+        req = urllib.request.Request(url)
+        req.add_header("User-Agent",
+                    "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2623.221 Safari/537.36 SE 2.X MetaSr 1.0")
+        proxy = urllib.request.ProxyHandler({'http': proxy_addr})
+        opener = urllib.request.build_opener(proxy, urllib.request.HTTPHandler)
+        urllib.request.install_opener(opener)
+        data = urllib.request.urlopen(req).read().decode('utf-8', 'ignore')
+        return data
+
+    def get_containerid(url):
+        data = use_proxy(url, proxy_addr)
+        content = json.loads(data).get('data')
+        for data in content.get('tabsInfo').get('tabs'):
+            if (data.get('tab_type') == 'weibo'):
+                containerid = data.get('containerid')
+        return containerid
+
+    def get_userInfo(id):
+        url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id
+        data = use_proxy(url, proxy_addr)
+        content = json.loads(data).get('data')
+        profile_image_url = content.get('userInfo').get('profile_image_url')
+        description = content.get('userInfo').get('description')
+        profile_url = content.get('userInfo').get('profile_url')
+        verified = content.get('userInfo').get('verified')
+        guanzhu = content.get('userInfo').get('follow_count')
+        name = content.get('userInfo').get('screen_name')
+        fensi = content.get('userInfo').get('followers_count')
+        gender = content.get('userInfo').get('gender')
+        urank = content.get('userInfo').get('urank')
+        print("微博昵称：" + name + "\n" + "微博主页地址：" + profile_url + "\n" + "微博头像地址：" + profile_image_url + "\n" + "是否认证：" + str(verified) + "\n" + "微博说明：" + description + "\n" + "关注人数：" + str(guanzhu) + "\n" + "粉丝数：" + str(fensi) + "\n" + "性别：" + gender + "\n" + "微博等级：" + str(urank) + "\n")
+
+    def get_weibo(id, file):
+        global pic_num
+        pic_num = 0
+        i = 1
+        while True:
+            url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id
+            weibo_url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id + '&containerid=' + get_containerid(url) + '&page=' + str(i)
+            try:
+                data = use_proxy(weibo_url, proxy_addr)
+                content = json.loads(data).get('data')
+                cards = content.get('cards')
+                if (len(cards) > 0):
+                    for j in range(len(cards)):
+                        print("-----正在爬取第" + str(i) + "页，第" + str(j) + "条微博------")
+                        card_type = cards[j].get('card_type')
+                        if (card_type == 9):
+                            mblog = cards[j].get('mblog')
+                            attitudes_count = mblog.get('attitudes_count')
+                            comments_count = mblog.get('comments_count')
+                            created_at = mblog.get('created_at')
+                            reposts_count = mblog.get('reposts_count')
+                            scheme = cards[j].get('scheme')
+                            text = mblog.get('text')
+                            if mblog.get('pics') != None:
+                                # print(mblog.get('original_pic'))
+                                # print(mblog.get('pics'))
+                                pic_archive = mblog.get('pics')
+                                for _ in range(len(pic_archive)):
+                                    pic_num += 1
+                                    print(pic_archive[_]['large']['url'])
+                                    imgurl = pic_archive[_]['large']['url']
+                                    img = requests.get(imgurl)
+                                    # f = open(path + weibo_name + '\\' + str(pic_num) + str(imgurl[-4:]),'ab')  # 存储图片，多媒体文件需要参数b（二进制文件）# 原始代码
+                                    f = open(os.path.join(path, weibo_name, str(pic_num) + str(imgurl[-4:])), 'ab') # 存储图片，多媒体文件需要参数b（二进制文件）
+                                    f.write(img.content)  # 多媒体存储content
+                                    f.close()
+
+                            with open(file, 'a', encoding='utf-8') as fh:
+                                fh.write("----第" + str(i) + "页，第" + str(j) + "条微博----" + "\n")
+                                fh.write("微博地址：" + str(scheme) + "\n" + "发布时间：" + str(
+                                    created_at) + "\n" + "微博内容：" + text + "\n" + "点赞数：" + str(
+                                    attitudes_count) + "\n" + "评论数：" + str(comments_count) + "\n" + "转发数：" + str(
+                                    reposts_count) + "\n")
+                    i += 1
+                else:
+                    break
+            except Exception as e:
+                print(e)
+                i += 1  # 添加这一行
+                pass
+
+    # # 在指定路径下，先建立一个名为weibo的文件夹
+    # if os.path.isdir(os.path.join(path,"weibo")):
+    #     pass
+    # else:
+    #     os.mkdir(os.path.join(path,"weibo"))
+
+    if os.path.isdir(os.path.join(path,weibo_name)):
+        pass
+    else:
+        os.mkdir(os.path.join(path,weibo_name))
+    file = os.path.join(path, weibo_name, weibo_name + ".txt")
+
+    get_userInfo(id)
+    get_weibo(id, file)
+    print("微博数据获取完毕")
+    # 该程序最初来源：http://www.omegaxyz.com/2018/02/13/python_weibo/
+
+
+
+
+
+
+# Data Analysis
+
 def get_BMI(height,weight):
     """
     height：身高（m）（注意，单位为米）
     weight：体重（kg）（注意，单位为千克）
     调用示例：dw.get_BMI(height=1.75,weight=73)
     BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
     """
@@ -586,146 +746,9 @@
         print("当前BMI健康状态评价：体重超重")
 
     # print(f"建议体重保持在{suggested_weight_lower}至{suggested_weight_higher}之间")
     print("正常体重范围：建议体重保持在 %0.2f kg 至 %0.2f kg 之间\n(注意：男女有别，请结合自身实际情况判断自己的体重状态)" % (suggested_weight_lower,suggested_weight_higher))
 
 
 
-def game_number_guessing(number=100):
-    """
-    游戏规则：指定一个整数，确定数字的范围；根据提示猜数字，直到猜中。
-    number:大于1的整数，用于指定数字的范围，默认100，说明要猜的数字在100以内。
-    用法1：若不设定参数，可以写成 game_number_guessing() ，这时默认值为100。
-    用法2：自定义参数，可以写成 game_number_guessing(number=200)，这时，数字范围设定为在200以内。
-    """
-
-    # 自定义数字的范围，不局限于100以内
-    # x = int(input("输入一个数字，限定一个范围："))
-    x = int(number)
-
-    # 每次程序运行执行该行代码的时候，都会产生一个 指定范围内 的随机整数，并赋值给 answer 变量
-    answer = random.randint(1, x)
-
-    # 游戏设置
-    print("\nloading...")
-    time.sleep(0.5)
-    print("猜数字游戏加载中")
-    time.sleep(1)
-    print("ok...")
-    time.sleep(0.5)
-    print("加载完毕")
-    time.sleep(0.5)
-    print("start...")
-    time.sleep(0.5)
-    print("游戏已开局")
-    time.sleep(0.5)
-    user = input("设定你的游戏角色名字(若暂不设定，可按回车跳过)：")
-    if user:
-        print("角色名设定完毕...")
-        time.sleep(0.5)
-        print("gogogo...")
-        time.sleep(0.5)
-    else:
-        print("skiping...")
-        time.sleep(0.5)
-
-    num = 1
-    while True:
-
-        aa = int(input("\n输入答案："))
-        time.sleep(0.25)
-
-        if aa == answer:
-            print("猜对了！")
-            break
-        elif aa < answer:
-            print("大一点")
-        else:
-            print("小一点")
-        num = num + 1
-    
-    # 输出结果
-    if user:
-        print(f"\nhi，{user}，你一共猜了{num}次。")
-    else:
-        print(f"\nhi，无名氏，你一共猜了{num}次。")
-
-
-
-
-def copy_files_by_keyword(raw_data_path,working_path):
-    """
-    raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
-    working_path：工作路径，提取出来的文件将存放到该路径。
-    keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-    目标：根据文件名中的关键词复制文件。
-    """
-
-    # 原始数据文件夹
-    raw_data_path = raw_data_path
-    # 给定工作路径，或基础路径，用于制作结果文件夹路径
-    working_path = working_path
-
-    # 根据keyword制作目标路径——复制文件存放的位置
-    keyword = str(input("请输入要复制的文件包含的关键词:\n"))
-
-    # 判断结果文件夹是否已存在，不依赖上一步，如果此处发现目标文件夹不存在，可以现场新建一个
-    result_path = working_path + "/" + str(keyword)
-    if os.path.exists(result_path) == False:
-        os.mkdir(result_path)
-
-    # 提取raw_path中的文件列表，获取列表里面的文件，再根据文件名制作文件当前的完整路径——这一串操作都是为了制作路径
-    every_file_list_path = os.listdir(raw_data_path)
-    for i in every_file_list_path:
-        file_path = os.path.join(raw_data_path, i)  # 使用os.path.join()函数拼接路径
-        if os.path.isfile(file_path):  # 判断是否为文件
-            if str(keyword) in i:
-                print(f"找到名称中包括 {keyword} 的文件")
-                shutil.copy(file_path, result_path)
-                print(f"copying: {i} to {result_path}")
-            else:
-                continue 
-
-    print(f"名称中包括 {keyword} 的文件已提取（复制）完毕") 
-
-
-
-
-def move_files_by_keyword(raw_data_path,working_path):
-    """
-    raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
-    working_path：工作路径，提取出来的文件将存放到该路径。
-    keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-    目标：根据文件名中的关键词移动文件。
-    """
-
-    # 原始数据文件夹
-    raw_data_path = raw_data_path
-    # 给定工作路径，或基础路径，用于制作结果文件夹路径
-    working_path = working_path
-
-    # 根据keyword制作目标路径——复制文件存放的位置
-    keyword = str(input("请输入要移动的文件包含的关键词:\n"))
-
-    # 判断结果文件夹是否已存在，不依赖上一步，如果此处发现目标文件夹不存在，可以现场新建一个
-    result_path = working_path + "/" + str(keyword)
-    if os.path.exists(result_path) == False:
-        os.mkdir(result_path)
-
-    # 提取raw_path中的文件列表，获取列表里面的文件，再根据文件名制作文件当前的完整路径——这一串操作都是为了制作路径
-    every_file_list_path = os.listdir(raw_data_path)
-    for i in every_file_list_path:
-        file_path = os.path.join(raw_data_path, i)  # 使用os.path.join()函数拼接路径
-        if os.path.isfile(file_path):  # 判断是否为文件
-            if str(keyword) in i:
-                print(f"找到名称中包括 {keyword} 的文件")
-                file_path = raw_data_path + "/" + i
-                shutil.move(file_path, result_path)
-                print(f"moving: {i} to {result_path}")
-            else:
-                continue 
-
-    print(f"名称中包括 {keyword} 的文件已提取（移动）完毕") 
-
-
```

### Comparing `pydatawork-0.17.2.0/setup.py` & `pydatawork-0.17.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.2.0',
+    version='0.17.2.1',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

