# Comparing `tmp/ezcord-0.3.1.tar.gz` & `tmp/ezcord-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.3.1.tar", last modified: Thu Jun 22 22:40:26 2023, max compression
+gzip compressed data, was "ezcord-0.3.2.tar", last modified: Sun Jul  2 10:05:59 2023, max compression
```

## Comparing `ezcord-0.3.1.tar` & `ezcord-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.718749 ezcord-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 22:40:14.000000 ezcord-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 22:40:14.000000 ezcord-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-22 22:40:26.718749 ezcord-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-22 22:40:14.000000 ezcord-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 22:40:14.000000 ezcord-0.3.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.710749 ezcord-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 22:40:14.000000 ezcord-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 22:40:14.000000 ezcord-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 22:40:14.000000 ezcord-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:40:26.718749 ezcord-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.710749 ezcord-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.714749 ezcord-0.3.1/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.714749 ezcord-0.3.1/src/ezcord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/cogs/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.718749 ezcord-0.3.1/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.718749 ezcord-0.3.1/src/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.714749 ezcord-0.3.1/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.271898 ezcord-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 10:05:47.000000 ezcord-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 10:05:47.000000 ezcord-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-02 10:05:59.267897 ezcord-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-02 10:05:47.000000 ezcord-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 10:05:47.000000 ezcord-0.3.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 10:05:47.000000 ezcord-0.3.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/cogs/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-02 10:05:47.000000 ezcord-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 10:05:47.000000 ezcord-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:05:59.271898 ezcord-0.3.2/setup.cfg
```

### Comparing `ezcord-0.3.1/LICENSE` & `ezcord-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/PKG-INFO` & `ezcord-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.3.1
+Version: 0.3.2
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.3.1/README.md` & `ezcord-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/pyproject.toml` & `ezcord-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/bot.py` & `ezcord-0.3.2/ezcord/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -431,14 +431,15 @@
         *,
         style: HelpStyle = HelpStyle.embed_description,
         embed: discord.Embed | None = None,
         show_categories: bool = True,
         timeout: int = 500,
         ephemeral: bool = True,
         author_only: bool = True,
+        guild_only: bool = True,
     ):
         """Add a help command that uses a select menu to group commands by cogs.
 
         If you use :class:`Cog`, you can pass in emojis to use for the select menu.
 
         Parameters
         ----------
@@ -452,24 +453,27 @@
         timeout:
             The timeout for the select menu. Defaults to ``500``.
         ephemeral:
             Whether the help command should be ephemeral. Defaults to ``True``.
         author_only:
             Whether the help command should only be visible to the author. Defaults to ``True``.
             This only works if ``ephemeral`` is ``False``.
+        guild_only:
+            Whether the help command should only be visible in guilds. Defaults to ``True``.
         """
-        self.load_extension(f".cogs.help", package="ezcord")
         self.help = {
             "style": style,
             "embed": embed,
             "show_categories": show_categories,
             "timeout": timeout,
             "ephemeral": ephemeral,
             "author_only": author_only,
+            "guild_only": guild_only,
         }
+        self.load_extension(f".cogs.help", package="ezcord")
 
 
 class PrefixBot(Bot, commands.Bot):
     """A subclass of :class:`discord.ext.commands.Bot` that implements the :class:`Bot` class.
 
     This class can be used if you want to use EzCord with prefix commands.
     """
```

### Comparing `ezcord-0.3.1/src/ezcord/cogs/help.py` & `ezcord-0.3.2/ezcord/cogs/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 def get_group(cog: Cog) -> str | None:
     if hasattr(cog, "group") and cog.group:
         return cog.group
     return None
 
 
 class Help(Cog, hidden=True):
+    def __init__(self, bot: Bot):
+        super().__init__(bot)
+        self.help.guild_only = bot.help["guild_only"]
+
     @slash_command(name=t("cmd_name"), description=t("cmd_description"))
     async def help(self, ctx: discord.ApplicationContext):
         embed = self.bot.help["embed"]
         if embed is None:
             embed = discord.Embed(title=t("embed_title"), color=discord.Color.blue())
         else:
             embed = replace_embed_values(embed, ctx.interaction)
```

### Comparing `ezcord-0.3.1/src/ezcord/components.py` & `ezcord-0.3.2/ezcord/components.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/emb.py` & `ezcord-0.3.2/ezcord/emb.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from __future__ import annotations
 
 import copy
 
 import discord
 
 from .internal import copy_kwargs, load_embed, replace_dict, save_embeds
+from .logs import log
 
 
 def set_embed_templates(
     *,
     error_embed: discord.Embed | str | None = None,
     success_embed: discord.Embed | str | None = None,
     warn_embed: discord.Embed | str | None = None,
@@ -89,14 +90,15 @@
     )
 
 
 async def _send_embed(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     embed: discord.Embed | str,
     ephemeral: bool = True,
+    edit: bool = False,
     **kwargs,
 ):
     """Respond to an interaction or send an embed to a target.
 
     If the interaction has already been responded to,
     the message will be sent as a followup.
 
@@ -111,14 +113,21 @@
     """
     content = None
     if isinstance(embed, str):
         content = embed
         embed = None
 
     if isinstance(target, discord.ApplicationContext) or isinstance(target, discord.Interaction):
+        if edit:
+            try:
+                await target.edit(content=content, embed=embed, **kwargs)
+                return
+            except AttributeError:
+                log.error("'edit=True' can only be used with Pycord master branch.")
+
         if not target.response.is_done():
             await target.response.send_message(
                 content=content, embed=embed, ephemeral=ephemeral, **kwargs
             )
         else:
             await target.followup.send(content=content, embed=embed, ephemeral=ephemeral, **kwargs)
     else:
@@ -149,159 +158,160 @@
 
 
 async def _process_message(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     embed: discord.Embed | str,
     txt: str | None,
     title: str | None,
+    edit: bool,
     ephemeral: bool,
     **kwargs,
 ):
-    """Adds embed attributes to the embed before sending it.
-
-    Parameters
-    ----------
-    target:
-        The target to send the message to.
-    txt:
-        The text to send.
-    title:
-        The title of the embed. Defaults to ``None``.
-    ephemeral:
-        Whether the message should be ephemeral.
-    """
     if isinstance(embed, discord.Embed):
         embed = copy.deepcopy(embed)
         if txt is not None:
             embed.description = txt
         if title is not None:
             embed.title = title
     elif isinstance(embed, str) and embed == "":
         embed = txt
 
     embed = _insert_info(target, embed)
 
-    await _send_embed(target, embed, ephemeral, **kwargs)
+    await _send_embed(target, embed, ephemeral, edit, **kwargs)
 
 
 @copy_kwargs(discord.InteractionResponse.send_message)
 async def error(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str | None = None,
     *,
     title: str | None = None,
+    edit: bool = False,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send an error message. By default, this is a red embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
         The text for the embed description. If this is ``None``,
         you need to provide a non-empty ``Embed`` when using :func:`set_embed_templates`.
     title:
         The title of the embed. Defaults to ``None``.
+    edit:
+        Whether to edit the last message instead of sending a new one. Defaults to ``False``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("error_embed")
-    await _process_message(target, embed, txt, title, ephemeral, **kwargs)
+    await _process_message(target, embed, txt, title, edit, ephemeral, **kwargs)
 
 
 @copy_kwargs(discord.abc.Messageable.send)
 async def success(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str | None = None,
     *,
     title: str | None = None,
+    edit: bool = False,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send a success message. By default, this is a green embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
         The text for the embed description. If this is ``None``,
         you need to provide a non-empty ``Embed`` when using :func:`set_embed_templates`.
     title:
         The title of the embed. Defaults to ``None``.
+    edit:
+        Whether to edit the last message instead of sending a new one. Defaults to ``False``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("success_embed")
-    await _process_message(target, embed, txt, title, ephemeral, **kwargs)
+    await _process_message(target, embed, txt, title, edit, ephemeral, **kwargs)
 
 
 @copy_kwargs(discord.abc.Messageable.send)
 async def warn(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str | None = None,
     *,
     title: str | None = None,
+    edit: bool = False,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send a warning message. By default, this is a golden embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
         The text for the embed description. If this is ``None``,
         you need to provide a non-empty ``Embed`` when using :func:`set_embed_templates`.
     title:
         The title of the embed. Defaults to ``None``.
+    edit:
+        Whether to edit the last message instead of sending a new one. Defaults to ``False``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("warn_embed")
-    await _process_message(target, embed, txt, title, ephemeral, **kwargs)
+    await _process_message(target, embed, txt, title, edit, ephemeral, **kwargs)
 
 
 @copy_kwargs(discord.abc.Messageable.send)
 async def info(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str | None = None,
     *,
     title: str | None = None,
+    edit: bool = False,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send an info message. By default, this is a blue embed.
 
     Parameters
     ----------
     target:
         The target to send the message to.
     txt:
         The text for the embed description. If this is ``None``,
         you need to provide a non-empty ``Embed`` when using :func:`set_embed_templates`.
     title:
         The title of the embed. Defaults to ``None``.
+    edit:
+        Whether to edit the last message instead of sending a new one. Defaults to ``False``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed("info_embed")
-    await _process_message(target, embed, txt, title, ephemeral, **kwargs)
+    await _process_message(target, embed, txt, title, edit, ephemeral, **kwargs)
 
 
 @copy_kwargs(discord.abc.Messageable.send)
 async def send(
     template: str,
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     txt: str | None = None,
     *,
     title: str | None = None,
+    edit: bool = False,
     ephemeral: bool = True,
     **kwargs,
 ):
     """Send a custom embed template. This needs to be set up with :func:`set_embed_templates`.
 
     Parameters
     ----------
@@ -310,12 +320,14 @@
     target:
         The target to send the message to.
     txt:
         The text for the embed description. If this is ``None``,
         you need to provide a non-empty ``Embed`` when using :func:`set_embed_templates`.
     title:
         The title of the embed. Defaults to ``None``.
+    edit:
+        Whether to edit the last message instead of sending a new one. Defaults to ``False``.
     ephemeral:
         Whether the message should be ephemeral. Defaults to ``True``.
     """
     embed = load_embed(template)
-    await _process_message(target, embed, txt, title, ephemeral, **kwargs)
+    await _process_message(target, embed, txt, title, edit, ephemeral, **kwargs)
```

### Comparing `ezcord-0.3.1/src/ezcord/enums.py` & `ezcord-0.3.2/ezcord/enums.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/internal/colors.py` & `ezcord-0.3.2/ezcord/internal/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,23 @@
 
 
 def remove_escapes(string: str) -> str:
     """Removes ansi escape codes from a string."""
     return re.sub(r"\x1b\[[0-9;]*m", "", string)
 
 
-def replace_dc_format(string: str, color: str | None = None, file: bool = False) -> str:
-    """Replaces Discord markdown with ansi colors."""
+def replace_dc_format(string: str, color: str | None = None, remove_stars: bool = False) -> str:
+    """Replaces Discord markdown with ansi colors.
+    If logs are written to a file or the log message if fully colored, ``remove`` should be ``True``.
+    """
     if color is None:
         color = DEFAULT_COLOR
     color = get_escape_code(color)
 
-    if file:
+    if remove_stars:
         string = string.replace("***", "").replace("**", "")
         string = remove_escapes(string)
     else:
         string = replace_second(string, "***", color)  # text that contains multiple other colors
         string = replace_second(string, "**", color)
 
     string = re.sub("```.*?```", "", string, flags=re.DOTALL)  # remove codeblocks
```

### Comparing `ezcord-0.3.1/src/ezcord/internal/embed_templates.py` & `ezcord-0.3.2/ezcord/internal/embed_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import os
 import traceback
+from copy import deepcopy
 from functools import cache
 from pathlib import Path
 
 import discord
 from discord import Color, Embed
 
 _TEMPLATES: dict[str, Embed] = {
@@ -129,10 +130,10 @@
         elif isinstance(value, dict):
             content[key] = replace_dict(value, interaction)
 
     return content
 
 
 def replace_embed_values(embed: discord.Embed, interaction: discord.Interaction):
-    embed_dict = embed.to_dict()
+    embed_dict = deepcopy(embed).to_dict()
     embed_dict = replace_dict(embed_dict, interaction)
     return discord.Embed.from_dict(embed_dict)
```

### Comparing `ezcord-0.3.1/src/ezcord/internal/language/de.json` & `ezcord-0.3.2/ezcord/internal/language/de.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/internal/language/en.json` & `ezcord-0.3.2/ezcord/internal/language/en.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/internal/language/languages.py` & `ezcord-0.3.2/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/internal/ready_style.py` & `ezcord-0.3.2/ezcord/internal/ready_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,17 @@
     title: str,
     modifications: tuple,
     style: ReadyEvent = ReadyEvent.default,
     default_info: bool = True,
     new_info: dict | None = None,
     colors: list[str] | None = None,
 ):
+    if not bot.user:
+        return log.error("The ready function must be called within the on_ready event.")
+
     colors = list(map(get_escape_code, colors or DEFAULT_COLORS))
 
     if default_info:
         infos, colors = modify_info(bot, modifications, colors)
     else:
         infos = get_default_info(bot)
```

### Comparing `ezcord-0.3.1/src/ezcord/internal/translation.py` & `ezcord-0.3.2/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/logs.py` & `ezcord-0.3.2/ezcord/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,18 @@
                     log_format = log_format.replace(
                         substring, get_escape_code(substring.strip("{}"))
                     )
 
                 color_formats[level] = log_format.format(color=final_colors[level], end=Fore.RESET)
     else:
         for level in final_colors:
-            color_formats[level] = final_colors[level] + log_format + Fore.RESET
+            if file:
+                color_formats[level] = log_format
+            else:
+                color_formats[level] = final_colors[level] + log_format + Fore.RESET
 
     return color_formats
 
 
 def _format_colors(colors: dict[int, str] | str | None = None) -> dict[int, str]:
     """Overwrite the default colors for the given log levels in the given format."""
 
@@ -170,15 +173,16 @@
         # color new lines
         if isinstance(log_format, str) and log_format.endswith("//"):
             log_format = log_format.replace("//", "")
             split = new_record.msg.split("\n", 1)
             if len(split) > 1:
                 new_record.msg = split[0] + "\n***" + split[1] + "***"
 
-        new_record.msg = replace_dc_format(new_record.msg, current_level_color, self.file)
+        remove_stars = self.file or "{end}" not in self.LOG_FORMAT
+        new_record.msg = replace_dc_format(new_record.msg, current_level_color, remove_stars)
 
         formatter = logging.Formatter(log_format, self.TIME_FORMAT)
         return formatter.format(new_record)
 
 
 class _DiscordHandler(logging.Handler):
     """A logging handler that sends logs to a Discord webhook."""
@@ -237,15 +241,15 @@
     return True
 
 
 def set_log(
     name: str = DEFAULT_LOG,
     log_level: int = logging.INFO,
     *,
-    file: bool = False,
+    file: bool | str = False,
     log_format: str | LogFormat = LogFormat.default,
     time_format: str | TimeFormat = TimeFormat.default,
     discord_log_level: int = logging.WARNING,
     webhook_url: str | None = None,
     dc_codeblocks: bool = True,
     level_spacing: int = 8,
     space_mode: Literal["auto", "always", "never"] = "auto",
@@ -259,14 +263,15 @@
     ----------
     name:
         The name of the logger.
     log_level:
         The log level for default log messages ``logging.INFO``.
     file:
         Whether to log to a file. Defaults to ``False``.
+        You can also pass a path to a log file.
     log_format:
         The log format. Defaults to :attr:`.LogFormat.default`.
     time_format:
         The time format. Defaults to :attr:`.TimeFormat.default`.
     discord_log_level:
         The log level for discord log messages. Defaults to ``logging.WARNING``.
 
@@ -306,28 +311,34 @@
     """
     logger = logging.getLogger(name)
     if logger.handlers:
         return logger
     logger.setLevel(log_level)
 
     handler: logging.FileHandler | logging.StreamHandler
-    if file:
+    if isinstance(file, bool) and file:
         if not os.path.exists("logs"):
             os.mkdir("logs")
         filename = name.split(".")[-1]
         handler = logging.FileHandler(f"logs/{filename}.log", mode="w", encoding="utf-8")
+    elif isinstance(file, str):
+        handler = logging.FileHandler(file, mode="w", encoding="utf-8")
+        file = True
     else:
         handler = logging.StreamHandler(sys.stdout)
 
     space_after_level = True
     if "%(levelname)s " not in log_format and "%(levelname)s{end} " not in log_format:
         space_after_level = False
-        if space_mode == "never" or space_mode == "auto":
+        if space_mode == "auto":
             level_spacing = 0
 
+    if space_mode == "never":
+        level_spacing = 0
+
     color_formatter = _ColorFormatter(
         file, log_format, time_format, dc_codeblocks, level_spacing, space_after_level, colors
     )
 
     handler.setFormatter(color_formatter)
     handler.setLevel(log_level)
     logger.addHandler(handler)
```

### Comparing `ezcord-0.3.1/src/ezcord/sql.py` & `ezcord-0.3.2/ezcord/sql.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/times.py` & `ezcord-0.3.2/ezcord/times.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord/utils.py` & `ezcord-0.3.2/ezcord/utils.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.1/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.3.2/ezcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.3.1
+Version: 0.3.2
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

