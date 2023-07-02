# Comparing `tmp/mindmate-0.1.6.tar.gz` & `tmp/mindmate-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindmate-0.1.6.tar", last modified: Fri Jun  9 20:40:50 2023, max compression
+gzip compressed data, was "mindmate-0.1.7.tar", last modified: Sun Jul  2 03:09:42 2023, max compression
```

## Comparing `mindmate-0.1.6.tar` & `mindmate-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.865685 mindmate-0.1.6/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2083 2023-06-09 20:40:50.862176 mindmate-0.1.6/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      759 2023-06-06 20:02:53.000000 mindmate-0.1.6/README.md
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.074108 mindmate-0.1.6/mindmate/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.6/mindmate/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      637 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/cli.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.473520 mindmate-0.1.6/mindmate/commands/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.6/mindmate/commands/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2538 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/chat.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      768 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/configure.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4038 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/directory.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1680 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/image.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/commands/version.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1216 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/error.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/meta.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.667514 mindmate-0.1.6/mindmate/services/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/services/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/services/directory.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1500 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/services/generic.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/services/models.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4957 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/services/openai.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.832785 mindmate-0.1.6/mindmate/utils/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.6/mindmate/utils/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      773 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/conf.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      657 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/env.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      328 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/helper.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2461 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/utils.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.250293 mindmate-0.1.6/mindmate.egg-info/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2083 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      725 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/entry_points.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/requires.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/top_level.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-09 20:40:50.866686 mindmate-0.1.6/setup.cfg
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2259 2023-06-08 18:06:48.000000 mindmate-0.1.6/setup.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-07-02 03:09:42.495594 mindmate-0.1.7/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2367 2023-07-02 03:09:42.492594 mindmate-0.1.7/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      869 2023-07-02 03:05:08.000000 mindmate-0.1.7/README.md
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-07-02 03:09:41.626375 mindmate-0.1.7/mindmate/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.7/mindmate/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      702 2023-07-02 03:05:08.000000 mindmate-0.1.7/mindmate/cli.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-07-02 03:09:42.113480 mindmate-0.1.7/mindmate/commands/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.7/mindmate/commands/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2539 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/commands/chat.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      768 2023-06-09 20:37:05.000000 mindmate-0.1.7/mindmate/commands/configure.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4038 2023-06-09 20:37:05.000000 mindmate-0.1.7/mindmate/commands/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1680 2023-06-09 20:37:05.000000 mindmate-0.1.7/mindmate/commands/image.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.1.7/mindmate/commands/version.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1572 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/commands/voice.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1216 2023-06-09 20:37:05.000000 mindmate-0.1.7/mindmate/error.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/meta.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-07-02 03:09:42.306889 mindmate-0.1.7/mindmate/services/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.1.7/mindmate/services/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.1.7/mindmate/services/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1739 2023-07-02 02:27:38.000000 mindmate-0.1.7/mindmate/services/generic.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.1.7/mindmate/services/models.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     6119 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/services/openai.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1199 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/services/voice.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-07-02 03:09:42.466242 mindmate-0.1.7/mindmate/utils/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.7/mindmate/utils/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      808 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/utils/conf.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      657 2023-06-09 20:37:05.000000 mindmate-0.1.7/mindmate/utils/env.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      405 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/utils/helper.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2456 2023-07-02 03:05:09.000000 mindmate-0.1.7/mindmate/utils/utils.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-07-02 03:09:41.840463 mindmate-0.1.7/mindmate.egg-info/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2367 2023-07-02 03:09:40.000000 mindmate-0.1.7/mindmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      779 2023-07-02 03:09:40.000000 mindmate-0.1.7/mindmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-07-02 03:09:40.000000 mindmate-0.1.7/mindmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-07-02 03:09:40.000000 mindmate-0.1.7/mindmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       51 2023-07-02 03:09:40.000000 mindmate-0.1.7/mindmate.egg-info/requires.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-07-02 03:09:40.000000 mindmate-0.1.7/mindmate.egg-info/top_level.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-07-02 03:09:42.496619 mindmate-0.1.7/setup.cfg
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2414 2023-07-02 03:05:09.000000 mindmate-0.1.7/setup.py
```

### Comparing `mindmate-0.1.6/PKG-INFO` & `mindmate-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.1.6
+Version: 0.1.7
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
@@ -15,46 +15,51 @@
         ```
         > It's not recommended to install in virtual environment _(except for  testing)_ try it with default `pip`
         
         ## operating system level
         ```
         sudo apt update
         sudo apt install -y python3-pip
-        export PATH="$PATH:/home/<USER>/.local/bin"
+        export PATH="$PATH:/home/$USER/.local/bin"
         pip install mindmate
         ```
         # usage
         ```
         $ mindmate [ARGUMENT] [OPTIONS] [OPTIONS] [OPTIONS] --help
         ```
         
         ## examples
         ```
         $ mindmate configure
-        $ mindmate ai prompting list
+        $ mindmate directory prompting list
         
         $ mindmate chat --platform openai \
           --model text-davinci-003 \
           --stream true \
           --max-tokens 500 \
           --prompt "Act as a professional developer, provide best file structure for fastAPI framework"
+        
+        $ mindmate image create -p "mindmate written on the background in a garden and friends playing around"
         ```
         
         # compatibility
         
         __Not tested__ yet, but should be compatible with any Python >= 3.8
         
 Keywords: cli,ai,nlp,ml,developers,productivity,openai,directory,manifest
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: System Shells
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Internet
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `mindmate-0.1.6/README.md` & `mindmate-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,32 @@
 ```
 > It's not recommended to install in virtual environment _(except for  testing)_ try it with default `pip`
 
 ## operating system level
 ```
 sudo apt update
 sudo apt install -y python3-pip
-export PATH="$PATH:/home/<USER>/.local/bin"
+export PATH="$PATH:/home/$USER/.local/bin"
 pip install mindmate
 ```
 # usage
 ```
 $ mindmate [ARGUMENT] [OPTIONS] [OPTIONS] [OPTIONS] --help
 ```
 
 ## examples
 ```
 $ mindmate configure
-$ mindmate ai prompting list
+$ mindmate directory prompting list
 
 $ mindmate chat --platform openai \
   --model text-davinci-003 \
   --stream true \
   --max-tokens 500 \
   --prompt "Act as a professional developer, provide best file structure for fastAPI framework"
+
+$ mindmate image create -p "mindmate written on the background in a garden and friends playing around"
 ```
 
 # compatibility
 
 __Not tested__ yet, but should be compatible with any Python >= 3.8
```

### Comparing `mindmate-0.1.6/mindmate/cli.py` & `mindmate-0.1.7/mindmate/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import click
 from mindmate.utils import helper
 from mindmate.commands.configure import configure
 from mindmate.commands.chat import chat
 from mindmate.commands.directory import directory
 from mindmate.commands.image import image
+from mindmate.commands.voice import voice
 from mindmate.commands.version import version
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
     """hi to mindmate cli, try option --help for more information"""
     pass
 
 cli.add_command(configure)
 cli.add_command(chat)
 cli.add_command(directory)
 cli.add_command(image)
+cli.add_command(voice)
 cli.add_command(version)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `mindmate-0.1.6/mindmate/commands/chat.py` & `mindmate-0.1.7/mindmate/commands/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return None
 
 @click.command()
 @click.option('-P', '--platform', required=True, default='openai', show_default=False, type=click.Choice(constants.PLATFORM_OPTIONS), help='use platform as an underlying technology')
 @click.option('-m', '--model', required=True, default='text-davinci-003', show_default=True, type=str, callback=model_option_callback, help='select targeted model to utilize')
 @click.option('-p', '--prompt', required=True, show_default=False, type=str, help='Your prompt to AI')
 @click.option('-s', '--stream', required=False, default=True, show_default=True, type=bool, help='stream AI response on your terminal')
-@click.option('--max-tokens', required=False, default=100, show_default=True, type=int, help='stream AI response on your terminal')
+@click.option('--max-tokens', required=False, default=3000, show_default=True, type=int, help='stream AI response on your terminal')
 def chat(platform, model, prompt, stream, max_tokens):
     """offers text-based response to your prompt"""
     click.echo(help.generic_message())
     # click.echo(click.get_current_context().params)
     KEYS = utility.get_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)['keys']
     if platform == 'openai':
         openai_client = OpenAIManager(id=KEYS['openai_id'], token=KEYS['openai_token'])
```

### Comparing `mindmate-0.1.6/mindmate/commands/configure.py` & `mindmate-0.1.7/mindmate/commands/configure.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/commands/directory.py` & `mindmate-0.1.7/mindmate/commands/directory.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/commands/image.py` & `mindmate-0.1.7/mindmate/commands/image.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/error.py` & `mindmate-0.1.7/mindmate/error.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/services/directory.py` & `mindmate-0.1.7/mindmate/services/directory.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/services/generic.py` & `mindmate-0.1.7/mindmate/services/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,21 @@
         return self.last_prompt +' -- '+ str(self.expires_at)
 
 class Image:
     url: str or None
     def __init__(self, url) -> None:
         self.url = url
     def download_image_to_current_path(self) -> None:
+        """
+        Downloads an image from the specified URL and saves it to the current working directory.
+
+        Args:
+            self: The instance of the class containing this method.
+
+        Returns:
+            None
+        """
         image = requests.get(self.url)
         current_path = utility.get_the_current_path()
         image_path = os.path.join(current_path, utility.generate_random_string())
         with open(image_path+'.png', 'wb') as f:
             f.write(image.content)
```

### Comparing `mindmate-0.1.6/mindmate/services/models.py` & `mindmate-0.1.7/mindmate/services/models.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/utils/conf.py` & `mindmate-0.1.7/mindmate/utils/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import base64
+import os
 
 class mongo:
     DATA_API_APP_ID = 'data-mzlwr'
     BASE_URL = f'https://data.mongodb-api.com/app/{DATA_API_APP_ID}/endpoint/data/v1'
     API_KEY = base64.b64decode('UHg0emhsV2pPam4wbk1BYWg4SHZ6dWREY2N5NmlWZVRtRHNEeThpTE52N3pTNFZwb0lhMld3UXRQUmZuYkhnUwo=').decode('utf-8').rstrip()
     headers = {
         'Content-Type': 'application/json',
         'Access-Control-Request-Headers': '*',
         'api-key': API_KEY,
     }
     def initialize_client() -> object:
         return mongo
 
 class constants:
-    FILE_PATH = '~/.mindmate'
+    FILE_PATH = os.path.expanduser("~") + '/.mindmate'
     FILE_NAME = 'environment.yaml'
     SYS_ROLE = 'system'
     AI_ROLE = 'AI bot'
     HINT_ROLE = 'HINT'
     PLATFORM_OPTIONS = ['openai']
     MODEL_OPTIONS = {
         'openai': ['text-davinci-003', 'text-davinci-002'],
```

### Comparing `mindmate-0.1.6/mindmate/utils/env.py` & `mindmate-0.1.7/mindmate/utils/env.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.6/mindmate/utils/utils.py` & `mindmate-0.1.7/mindmate/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,8 +53,8 @@
         return final
     def generate_random_string() -> str:
         length = random.randint(5, 10)
         letters = string.ascii_letters
         random_string = ''.join(random.choice(letters) for _ in range(length))
         return random_string
     def get_the_current_path() -> str:
-        return os.getenv('PWD')
+        return os.getcwd()
```

### Comparing `mindmate-0.1.6/mindmate.egg-info/PKG-INFO` & `mindmate-0.1.7/mindmate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.1.6
+Version: 0.1.7
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
@@ -15,46 +15,51 @@
         ```
         > It's not recommended to install in virtual environment _(except for  testing)_ try it with default `pip`
         
         ## operating system level
         ```
         sudo apt update
         sudo apt install -y python3-pip
-        export PATH="$PATH:/home/<USER>/.local/bin"
+        export PATH="$PATH:/home/$USER/.local/bin"
         pip install mindmate
         ```
         # usage
         ```
         $ mindmate [ARGUMENT] [OPTIONS] [OPTIONS] [OPTIONS] --help
         ```
         
         ## examples
         ```
         $ mindmate configure
-        $ mindmate ai prompting list
+        $ mindmate directory prompting list
         
         $ mindmate chat --platform openai \
           --model text-davinci-003 \
           --stream true \
           --max-tokens 500 \
           --prompt "Act as a professional developer, provide best file structure for fastAPI framework"
+        
+        $ mindmate image create -p "mindmate written on the background in a garden and friends playing around"
         ```
         
         # compatibility
         
         __Not tested__ yet, but should be compatible with any Python >= 3.8
         
 Keywords: cli,ai,nlp,ml,developers,productivity,openai,directory,manifest
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: System Shells
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Internet
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `mindmate-0.1.6/mindmate.egg-info/SOURCES.txt` & `mindmate-0.1.7/mindmate.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 mindmate.egg-info/top_level.txt
 mindmate/commands/__init__.py
 mindmate/commands/chat.py
 mindmate/commands/configure.py
 mindmate/commands/directory.py
 mindmate/commands/image.py
 mindmate/commands/version.py
+mindmate/commands/voice.py
 mindmate/services/__init__.py
 mindmate/services/directory.py
 mindmate/services/generic.py
 mindmate/services/models.py
 mindmate/services/openai.py
+mindmate/services/voice.py
 mindmate/utils/__init__.py
 mindmate/utils/conf.py
 mindmate/utils/env.py
 mindmate/utils/helper.py
 mindmate/utils/utils.py
```

### Comparing `mindmate-0.1.6/setup.py` & `mindmate-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,26 @@
     entry_points={
         'console_scripts': [
             'mindmate = mindmate.cli:cli',  # Update with your CLI entry point
         ],
     },
     # reference: https://pypi.org/classifiers/
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Other Environment',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'Topic :: Software Development',
         'Topic :: System :: System Shells',
+        'Topic :: Communications :: Chat',
+        'Topic :: Internet',
+        'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Utilities',
     ],
     # platforms=[],
     license='LGPL-2.1 license',
 )
```

