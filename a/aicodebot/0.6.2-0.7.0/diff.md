# Comparing `tmp/aicodebot-0.6.2.tar.gz` & `tmp/aicodebot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.6.2.tar", last modified: Thu Jun 29 19:43:30 2023, max compression
+gzip compressed data, was "aicodebot-0.7.0.tar", last modified: Sun Jul  2 04:30:34 2023, max compression
```

## Comparing `aicodebot-0.6.2.tar` & `aicodebot-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 19:43:05.000000 aicodebot-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-29 19:43:30.361267 aicodebot-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-06-29 19:43:05.000000 aicodebot-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-29 19:43:05.000000 aicodebot-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:43:30.361267 aicodebot-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-29 19:43:05.000000 aicodebot-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.282827 aicodebot-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-02 04:30:10.000000 aicodebot-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-02 04:30:34.278828 aicodebot-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-07-02 04:30:10.000000 aicodebot-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.278828 aicodebot-0.7.0/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.278828 aicodebot-0.7.0/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.278828 aicodebot-0.7.0/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-02 04:30:10.000000 aicodebot-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:30:34.282827 aicodebot-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-02 04:30:10.000000 aicodebot-0.7.0/setup.py
```

### Comparing `aicodebot-0.6.2/LICENSE` & `aicodebot-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.2/PKG-INFO` & `aicodebot-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,44 @@
-Metadata-Version: 2.1
-Name: aicodebot
-Version: 0.6.2
-Summary: Your AI-powered coding companion: AI Code Bot 🤖
-Home-page: https://github.com/novara_ai/aicodebot
-Author: Nick Sullivan
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
-There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
+We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features. ⬇
+⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
 
-⚠️ It uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
 
 We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
-## Current features - how you can use it
+## Current features - how you can use it today
 
 ### AI-Assisted Git Commit
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that describes the change. It will also commit the changes for you once everything checks out.
+`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
 ### AI-Assisted Code Review
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
 ### AI-Assisted Debugging
 
-`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
-
-### AI-Assisted Code Creation (Work in Progress)
-
-The aicodebot code feature is an AI-powered tool that automates coding tasks. It understands your task, formulates a plan, learns necessary information, and generates code that fits your codebase style. It also reviews its own work, modifies the local code, and creates unit tests. This feature is designed to streamline your coding process and boost productivity. In the future, we plan to enhance its performance through a continuous learning system based on user feedback and interaction outcomes.
+`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
-This feature is a work in progress, and it's more thoroughly documented [here](docs/code_agent.md) and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
+[![PyPI version](https://badge.fury.io/py/aicodebot.svg?0.6.2)](https://badge.fury.io/py/aicodebot)
 
-## Getting Started
-
-[![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
+## Installation and Usage
 
 To install AICodeBot, run:
 
 `pip install aicodebot`
 
 And then run `aicodebot --help` to get started.
 
@@ -80,20 +57,22 @@
   review     Do a code review, with [un]staged changes, or a specified...
   ```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
-#### GPT-3.5 vs GPT-4
+#### Which Language Model? GPT-3.5 vs GPT-4
 
 When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
+Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
+
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
 * [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 * [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 * [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
@@ -131,12 +110,12 @@
 * [ ] **Supportive Encouragement**: High fives and kudos for a job well done
 * [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Alignment ❤️ + 🤖
 
-Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
+Technology itself is amoral, it just imbues the values of the people who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building AICodeBot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Development / Contributing
 
 We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.6.2/README.md` & `aicodebot-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,61 @@
+Metadata-Version: 2.1
+Name: aicodebot
+Version: 0.7.0
+Summary: Your AI-powered coding companion: AI Code Bot 🤖
+Home-page: https://github.com/novara_ai/aicodebot
+Author: Nick Sullivan
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
-There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
+We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features. ⬇
+⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
 
-⚠️ It uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
 
 We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
-## Current features - how you can use it
+## Current features - how you can use it today
 
 ### AI-Assisted Git Commit
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that describes the change. It will also commit the changes for you once everything checks out.
+`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
 ### AI-Assisted Code Review
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
 ### AI-Assisted Debugging
 
-`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
-
-### AI-Assisted Code Creation (Work in Progress)
-
-The aicodebot code feature is an AI-powered tool that automates coding tasks. It understands your task, formulates a plan, learns necessary information, and generates code that fits your codebase style. It also reviews its own work, modifies the local code, and creates unit tests. This feature is designed to streamline your coding process and boost productivity. In the future, we plan to enhance its performance through a continuous learning system based on user feedback and interaction outcomes.
+`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
-This feature is a work in progress, and it's more thoroughly documented [here](docs/code_agent.md) and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
+[![PyPI version](https://badge.fury.io/py/aicodebot.svg?0.6.2)](https://badge.fury.io/py/aicodebot)
 
-## Getting Started
-
-[![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
+## Installation and Usage
 
 To install AICodeBot, run:
 
 `pip install aicodebot`
 
 And then run `aicodebot --help` to get started.
 
@@ -63,20 +74,22 @@
   review     Do a code review, with [un]staged changes, or a specified...
   ```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
-#### GPT-3.5 vs GPT-4
+#### Which Language Model? GPT-3.5 vs GPT-4
 
 When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
+Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
+
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
 * [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 * [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 * [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
@@ -114,12 +127,12 @@
 * [ ] **Supportive Encouragement**: High fives and kudos for a job well done
 * [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Alignment ❤️ + 🤖
 
-Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
+Technology itself is amoral, it just imbues the values of the people who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building AICodeBot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Development / Contributing
 
 We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.6.2/aicodebot/cli.py` & `aicodebot-0.7.0/aicodebot/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from aicodebot import version as aicodebot_version
+from aicodebot.agents import get_agent
 from aicodebot.helpers import exec_and_get_output, get_token_length, git_diff_context
 from dotenv import load_dotenv
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.prompts import load_prompt
 from openai.api_resources import engine
 from pathlib import Path
@@ -196,15 +197,15 @@
         # Select a random year so that we get a different answer each time
         year = random.randint(1942, datetime.datetime.utcnow().year)
         response = chat_chain.run(f"programming and artificial intelligence in the year {year}")
         console.print(response, style=bot_style)
 
 
 @cli.command
-@click.option("-c", "--commit", help="The commit hash to review.")
+@click.option("-c", "--commit", help="The commit hash to review (otherwise look at [un]staged changes).")
 @click.option("-v", "--verbose", count=True)
 def review(commit, verbose):
     """Do a code review, with [un]staged changes, or a specified commit."""
     setup_environment()
 
     diff_context = git_diff_context(commit)
     if not diff_context:
@@ -228,14 +229,32 @@
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     with console.status("Reviewing code", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
         console.print(response, style=bot_style)
 
 
+@cli.command
+@click.option("--task", "-t", help="The task you want to perform - a description of what you want to do.")
+@click.option("-v", "--verbose", count=True)
+def sidekick(task, verbose):
+    """ALPHA/EXPERIMENTAL: Get help with a task from your AI sidekick."""
+    setup_environment()
+
+    model = get_llm_model()
+    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=3500, verbose=verbose)
+
+    agent = get_agent("sidekick", llm, verbose)
+
+    with console.status("Thinking", spinner=DEFAULT_SPINNER):
+        response = agent({"input": task})
+        console.print("")
+        console.print(response["output"], style=bot_style)
+
+
 # ---------------------------------------------------------------------------- #
 #                               Helper functions                               #
 # ---------------------------------------------------------------------------- #
 
 
 def setup_environment():
     # Load environment variables from the config file
@@ -291,15 +310,15 @@
         sys.exit(0)
 
     raise click.ClickException(
         "🛑 Please set an API key in the OPENAI_API_KEY environment variable or in a .aicodebot file."
     )
 
 
-def get_llm_model(token_size):
+def get_llm_model(token_size=0):
     # https://platform.openai.com/docs/models/gpt-3-5
     # We want to use GPT-4, if it is available for this OPENAI_API_KEY, otherwise GPT-3.5
     # We also want to use the largest model that supports the token size we need
     model_options = {
         "gpt-4": 8192,
         "gpt-4-32k": 32768,
         "gpt-3.5-turbo": 4096,
```

### Comparing `aicodebot-0.6.2/aicodebot/helpers.py` & `aicodebot-0.7.0/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.2/aicodebot/prompts/alignment.yaml` & `aicodebot-0.7.0/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.2/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.7.0/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.2/aicodebot/prompts/review.yaml` & `aicodebot-0.7.0/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.2/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.7.0/aicodebot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.6.2
+Version: 0.7.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -17,51 +17,45 @@
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
-There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
+We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features. ⬇
+⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
 
-⚠️ It uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
 
 We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
-## Current features - how you can use it
+## Current features - how you can use it today
 
 ### AI-Assisted Git Commit
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that describes the change. It will also commit the changes for you once everything checks out.
+`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
 ### AI-Assisted Code Review
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code and makes us better programmers. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
 ### AI-Assisted Debugging
 
-`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
+`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, command output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
-### AI-Assisted Code Creation (Work in Progress)
+[![PyPI version](https://badge.fury.io/py/aicodebot.svg?0.6.2)](https://badge.fury.io/py/aicodebot)
 
-The aicodebot code feature is an AI-powered tool that automates coding tasks. It understands your task, formulates a plan, learns necessary information, and generates code that fits your codebase style. It also reviews its own work, modifies the local code, and creates unit tests. This feature is designed to streamline your coding process and boost productivity. In the future, we plan to enhance its performance through a continuous learning system based on user feedback and interaction outcomes.
-
-This feature is a work in progress, and it's more thoroughly documented [here](docs/code_agent.md) and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
-
-## Getting Started
-
-[![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
+## Installation and Usage
 
 To install AICodeBot, run:
 
 `pip install aicodebot`
 
 And then run `aicodebot --help` to get started.
 
@@ -80,20 +74,22 @@
   review     Do a code review, with [un]staged changes, or a specified...
   ```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
-#### GPT-3.5 vs GPT-4
+#### Which Language Model? GPT-3.5 vs GPT-4
 
 When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
+Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
+
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
 * [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 * [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 * [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
@@ -131,12 +127,12 @@
 * [ ] **Supportive Encouragement**: High fives and kudos for a job well done
 * [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Alignment ❤️ + 🤖
 
-Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
+Technology itself is amoral, it just imbues the values of the people who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building AICodeBot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Development / Contributing
 
 We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.6.2/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.7.0/aicodebot.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 aicodebot/.aicodebot.template
 aicodebot/__init__.py
+aicodebot/agents.py
 aicodebot/cli.py
 aicodebot/helpers.py
 aicodebot.egg-info/PKG-INFO
 aicodebot.egg-info/SOURCES.txt
 aicodebot.egg-info/dependency_links.txt
 aicodebot.egg-info/entry_points.txt
 aicodebot.egg-info/requires.txt
```

### Comparing `aicodebot-0.6.2/pyproject.toml` & `aicodebot-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.2/setup.py` & `aicodebot-0.7.0/setup.py`

 * *Files identical despite different names*

