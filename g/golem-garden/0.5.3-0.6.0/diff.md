# Comparing `tmp/golem_garden-0.5.3.tar.gz` & `tmp/golem_garden-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_garden-0.5.3.tar", last modified: Sat Apr 29 14:52:22 2023, max compression
+gzip compressed data, was "golem_garden-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `golem_garden-0.5.3.tar` & `golem_garden-0.6.0.tar`

### file list

```diff
@@ -1,52 +1,102 @@
--rw-r--r--   0        0        0      834 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/workflows/deploy_docs.yml
--rw-r--r--   0        0        0     1123 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1883 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.gitignore
--rw-r--r--   0        0        0     3348 2023-04-29 14:52:16.047027 golem_garden-0.5.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-04-29 14:52:16.051028 golem_garden-0.5.3/LICENSE
--rw-r--r--   0        0        0      190 2023-04-29 14:52:16.051028 golem_garden-0.5.3/README.md
--rw-r--r--   0        0        0       79 2023-04-29 14:52:16.051028 golem_garden-0.5.3/RUN_ME.py
--rw-r--r--   0        0        0     1640 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/Community Guidelines/Code of Conduct.md
--rw-r--r--   0        0        0     3511 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/Contributing guide/Contributing.md
--rw-r--r--   0        0        0     2790 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/Contributing guide/python_style_guide.md
--rw-r--r--   0        0        0      190 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/index.md
--rw-r--r--   0        0        0     2485 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      295 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/__init__.py
--rw-r--r--   0        0        0      897 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/__main__.py
--rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/data_loaders/__init__.py
--rw-r--r--   0        0        0      996 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/data_loaders/async_load_url_with_playwright.py
--rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/golems/__init__.py
--rw-r--r--   0        0        0     2118 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/golems/golem.py
--rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/output_parsers/__init__.py
--rw-r--r--   0        0        0     1186 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/output_parsers/output_parser.py
--rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/prompts/__init__.py
--rw-r--r--   0        0        0     1777 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/prompts/prompts.py
--rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/__init__.py
--rw-r--r--   0        0        0     3378 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/directory_printer.py
--rw-r--r--   0        0        0     5029 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/grab_all_py_in_one_text_block.py
--rw-r--r--   0        0        0      484 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
--rw-r--r--   0        0        0     3686 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/tools.py
--rw-r--r--   0        0        0    29940 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/ask_freemocap_docs.ipynb
--rw-r--r--   0        0        0     8092 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/dog_mailer_auto_gpt.py
--rw-r--r--   0        0        0    20524 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
--rw-r--r--   0        0        0     3890 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_agent_playground.py
--rw-r--r--   0        0        0    26686 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/autogpt.ipynb
--rw-r--r--   0        0        0    31113 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
--rw-r--r--   0        0        0    18274 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb
--rw-r--r--   0        0        0    60363 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
--rw-r--r--   0        0        0    44476 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
--rw-r--r--   0        0        0    23377 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
--rw-r--r--   0        0        0      882 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
--rw-r--r--   0        0        0    18760 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
--rw-r--r--   0        0        0    60951 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/marathon_times.ipynb
--rw-r--r--   0        0        0    23334 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
--rw-r--r--   0        0        0    25052 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
--rw-r--r--   0        0        0      123 2023-04-29 14:52:16.055028 golem_garden-0.5.3/mkdocs.yml
--rw-r--r--   0        0        0      356 2023-04-29 14:52:16.055028 golem_garden-0.5.3/notes/bluesky_todos.md
--rw-r--r--   0        0        0     1296 2023-04-29 14:52:16.055028 golem_garden-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      232 2023-04-29 14:52:16.055028 golem_garden-0.5.3/sample.env
--rw-r--r--   0        0        0       99 2023-04-29 14:52:16.055028 golem_garden-0.5.3/utilities/env_setup.bat
--rw-r--r--   0        0        0     2280 2023-04-29 14:52:16.055028 golem_garden-0.5.3/utilities/pinecone.py
--rw-r--r--   0        0        0      507 2023-04-29 14:52:16.055028 golem_garden-0.5.3/utilities/try_mongo_connection.py
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 golem_garden-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      834 2023-07-01 23:35:19.000656 golem_garden-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-07-01 23:35:19.000656 golem_garden-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-07-01 23:35:19.000656 golem_garden-0.6.0/.github/workflows/deploy_docs.yml
+-rw-r--r--   0        0        0     1123 2023-07-01 23:35:19.000656 golem_garden-0.6.0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1899 2023-07-01 23:35:19.000656 golem_garden-0.6.0/.gitignore
+-rw-r--r--   0        0        0     3348 2023-07-01 23:35:19.000656 golem_garden-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-07-01 23:35:19.000656 golem_garden-0.6.0/LICENSE
+-rw-r--r--   0        0        0      190 2023-07-01 23:35:19.000656 golem_garden-0.6.0/README.md
+-rw-r--r--   0        0        0       79 2023-07-01 23:35:19.000656 golem_garden-0.6.0/RUN_ME.py
+-rw-r--r--   0        0        0     1640 2023-07-01 23:35:19.000656 golem_garden-0.6.0/docs/Community Guidelines/Code of Conduct.md
+-rw-r--r--   0        0        0     3511 2023-07-01 23:35:19.000656 golem_garden-0.6.0/docs/Contributing guide/Contributing.md
+-rw-r--r--   0        0        0     2790 2023-07-01 23:35:19.000656 golem_garden-0.6.0/docs/Contributing guide/python_style_guide.md
+-rw-r--r--   0        0        0    59621 2023-07-01 23:35:19.004656 golem_garden-0.6.0/docs/assets/golem_garden_bot_icon-happy.png
+-rw-r--r--   0        0        0      190 2023-07-01 23:35:19.004656 golem_garden-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      356 2023-07-01 23:35:19.004656 golem_garden-0.6.0/docs/notes/bluesky_todos.md
+-rw-r--r--   0        0        0      551 2023-07-01 23:35:19.004656 golem_garden-0.6.0/docs/notes/pycharm_quickref.md
+-rw-r--r--   0        0        0     2485 2023-07-01 23:35:19.004656 golem_garden-0.6.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      348 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/__init__.py
+-rw-r--r--   0        0        0     1022 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/__init__.py
+-rw-r--r--   0        0        0     2145 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/golem.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/__init__.py
+-rw-r--r--   0        0        0     4505 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/agent_builder.py
+-rw-r--r--   0        0        0     1509 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/configuration_tomls/dunkthulu.toml
+-rw-r--r--   0        0        0      345 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/configuration_tomls/golem.toml
+-rw-r--r--   0        0        0     3535 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/configuration_tomls/golem_bobolem.toml
+-rw-r--r--   0        0        0     1594 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/configuration_tomls/instructions_improver.toml
+-rw-r--r--   0        0        0     2615 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/configuration_tomls/midjourney_prompt_builder.toml
+-rw-r--r--   0        0        0     2233 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/configuration_tomls/note_taker.toml
+-rw-r--r--   0        0        0      581 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/agents/get_available_agents.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/data_loaders/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/data_loaders/async_load_url_with_playwright.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1191 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/output_parsers/multi_action_output_parser.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/prompts/__init__.py
+-rw-r--r--   0        0        0     1782 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/prompts/multi_action_prompt_template.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/__init__.py
+-rw-r--r--   0        0        0     3378 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/directory_printer.py
+-rw-r--r--   0        0        0     5029 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/grab_all_py_in_one_text_block.py
+-rw-r--r--   0        0        0      484 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
+-rw-r--r--   0        0        0     3679 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/__init__.py
+-rw-r--r--   0        0        0     2903 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/agent_definitions/bill_dworld.config
+-rw-r--r--   0        0        0     2841 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/agent_definitions/enpisi.config
+-rw-r--r--   0        0        0     2950 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/agent_definitions/loke_aisha_n.config
+-rw-r--r--   0        0        0     1472 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/memory_util.py
+-rw-r--r--   0        0        0     7799 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/multiplayer_dnd_example.py
+-rw-r--r--   0        0        0    11492 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/Builder/npc_builder_chain.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/jkl/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/jkl/knowledge_grapher/__init__.py
+-rw-r--r--   0        0        0     1524 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/jkl/knowledge_grapher/autogpt_example.py
+-rw-r--r--   0        0        0     1924 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/jkl/knowledge_grapher/entity_memory_example.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/__init__.py
+-rw-r--r--   0        0        0     2834 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/agent_definitions/enpisi.config
+-rw-r--r--   0        0        0     2560 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/agent_definitions/world_weaver.config
+-rw-r--r--   0        0        0      400 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/character_model.py
+-rw-r--r--   0        0        0     1715 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/character_sheet_ingest.py
+-rw-r--r--   0        0        0     1267 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/mongo/README.md
+-rw-r--r--   0        0        0     1934 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/mongo/guidance.py
+-rw-r--r--   0        0        0      817 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/mongo/models.py
+-rw-r--r--   0        0        0      708 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/mongo/retrieve.py
+-rw-r--r--   0        0        0     1709 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/mongo/updater.py
+-rw-r--r--   0        0        0     2735 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/mongo/upsert.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/steerable_conversation/__init__.py
+-rw-r--r--   0        0        0     4860 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/karl/steerable_conversation/conversation_engine.py
+-rw-r--r--   0        0        0    10472 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/experimental/sts/testing_agent.ipynb
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/discord_bot/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/discord_bot/bot_main.py
+-rw-r--r--   0        0        0      547 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/discord_bot/bot_maker.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/discord_bot/cogs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/discord_bot/cogs/agent_cog/__init__.py
+-rw-r--r--   0        0        0     4313 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/frontend/discord_bot/cogs/agent_cog/agent_cog.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/system/__init__.py
+-rw-r--r--   0        0        0      840 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/system/filenames_and_paths.py
+-rw-r--r--   0        0        0     1527 2023-07-01 23:35:19.004656 golem_garden-0.6.0/golem_garden/system/logging/configure_logging.py
+-rw-r--r--   0        0        0     7697 2023-07-01 23:35:19.004656 golem_garden-0.6.0/jupyter_notebooks/ask_freemocap_docs.ipynb
+-rw-r--r--   0        0        0     8092 2023-07-01 23:35:19.004656 golem_garden-0.6.0/jupyter_notebooks/dog_mailer_auto_gpt.py
+-rw-r--r--   0        0        0    20524 2023-07-01 23:35:19.004656 golem_garden-0.6.0/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0     3932 2023-07-01 23:35:19.004656 golem_garden-0.6.0/jupyter_notebooks/langchain_agent_playground.py
+-rw-r--r--   0        0        0    34052 2023-07-01 23:35:19.004656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/autogpt.ipynb
+-rw-r--r--   0        0        0    31113 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
+-rw-r--r--   0        0        0    13988 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb
+-rw-r--r--   0        0        0    28915 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/entity_summary_memory.ipynb
+-rw-r--r--   0        0        0    60363 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
+-rw-r--r--   0        0        0    44476 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
+-rw-r--r--   0        0        0    23377 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0      882 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
+-rw-r--r--   0        0        0    18760 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
+-rw-r--r--   0        0        0    60951 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/marathon_times.ipynb
+-rw-r--r--   0        0        0    23334 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
+-rw-r--r--   0        0        0    38157 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/narrative_driven_sales_agent_with_context.ipynb
+-rw-r--r--   0        0        0    25052 2023-07-01 23:35:19.008656 golem_garden-0.6.0/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
+-rw-r--r--   0        0        0      123 2023-07-01 23:35:19.008656 golem_garden-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0     1327 2023-07-01 23:35:19.008656 golem_garden-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-07-01 23:35:19.008656 golem_garden-0.6.0/sample.env
+-rw-r--r--   0        0        0       99 2023-07-01 23:35:19.008656 golem_garden-0.6.0/utilities/env_setup.bat
+-rw-r--r--   0        0        0     2280 2023-07-01 23:35:19.008656 golem_garden-0.6.0/utilities/pinecone.py
+-rw-r--r--   0        0        0      507 2023-07-01 23:35:19.008656 golem_garden-0.6.0/utilities/try_mongo_connection.py
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 golem_garden-0.6.0/PKG-INFO
```

### Comparing `golem_garden-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md` & `golem_garden-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md` & `golem_garden-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/.github/workflows/deploy_docs.yml` & `golem_garden-0.6.0/.github/workflows/deploy_docs.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `golem_garden-0.6.0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/.gitignore` & `golem_garden-0.6.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-notes/_build/
+docs/notes/_build/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
@@ -131,7 +131,9 @@
 .vscode
 utilities/output/*
 
 .DS_Store
 test_database.json
 
 utilities/output/*
+.tmp*
+*.ini
```

### Comparing `golem_garden-0.5.3/CONTRIBUTING.md` & `golem_garden-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/LICENSE` & `golem_garden-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/docs/Community Guidelines/Code of Conduct.md` & `golem_garden-0.6.0/docs/Community Guidelines/Code of Conduct.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/docs/Contributing guide/Contributing.md` & `golem_garden-0.6.0/docs/Contributing guide/Contributing.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/docs/Contributing guide/python_style_guide.md` & `golem_garden-0.6.0/docs/Contributing guide/python_style_guide.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/docs/stylesheets/extra.css` & `golem_garden-0.6.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/golem_garden/__main__.py` & `golem_garden-0.6.0/golem_garden/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
+import logging
 from pathlib import Path
 import sys
 
+from golem_garden.backend.golem import Golem
+
 base_package_path = Path(__file__).parent.parent
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from rich.console import Console
 
 rich_console = Console()
 
-from golem_garden import Golem
-
-
+logger = logging.getLogger(__name__)
 
 class GolemGarden:
     def __init__(self):
-
+        logger.info(f"Initializing Golem Garden")
         self._golem = Golem()
 
-        # self._golem = GolemDocumentEditor()
     def run(self):
+        logger.info(f"Starting Golem Garden run loop...")
         rich_console.print(f"[bold cyan] {self._golem.intake_message('A human is here and said Hello')}")
 
         while True:
             message = input("Enter message (or `quit`): ")
             if message == "quit":
                 break
             rich_console.print(self._golem.intake_message(message))
```

### Comparing `golem_garden-0.5.3/golem_garden/data_loaders/async_load_url_with_playwright.py` & `golem_garden-0.6.0/golem_garden/backend/langchain_stuff/data_loaders/async_load_url_with_playwright.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/golem_garden/golems/golem.py` & `golem_garden-0.6.0/golem_garden/backend/golem.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             Tool(
                 name="Wolfram Alpha",
                 func=self._wolfram_alpha.run,
                 description="useful when you need to answer questions about the world around you."
             )
         ]
         self._memory = ConversationBufferMemory(memory_key="chat_history", return_messages=True)
+        self._index = None
         self._llm = ChatOpenAI(temperature=.8, model_name="gpt-4")
         self._chain = initialize_agent(self._tools,
                                        self._llm,
                                        agent=AgentType.CHAT_CONVERSATIONAL_REACT_DESCRIPTION,
                                        verbose=True,
                                        memory=self._memory)
```

### Comparing `golem_garden-0.5.3/golem_garden/output_parsers/output_parser.py` & `golem_garden-0.6.0/golem_garden/backend/langchain_stuff/output_parsers/multi_action_output_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import Union
 
 from langchain.agents import AgentOutputParser
 from langchain.schema import AgentAction, AgentFinish
 
 
-class CustomOutputParser(AgentOutputParser):
+class MultiActionOutputParser(AgentOutputParser):
 
     def parse(self, llm_output: str) -> Union[AgentAction, AgentFinish]:
         # Check if agent should finish
         if "Final Answer:" in llm_output:
             return AgentFinish(
                 # Return values is generally always a dictionary with a single `output` key
                 # It is not recommended to try anything else at the moment :)
```

### Comparing `golem_garden-0.5.3/golem_garden/prompts/prompts.py` & `golem_garden-0.6.0/golem_garden/backend/langchain_stuff/prompts/multi_action_prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Thought: I have everything I need to complete the task
 Final Answer: What I will do to complete the task
 
 task: {input}
 {agent_scratchpad}"""
 
 
-class CustomPromptTemplate(StringPromptTemplate):
+class MultiActionPromptTemplate(StringPromptTemplate):
     # The template to use
     template: str
 
     # The list of tools available
     tools_getter: Callable
 
     def format(self, **kwargs) -> str:
```

### Comparing `golem_garden-0.5.3/golem_garden/tools/directory_printer.py` & `golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/directory_printer.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/golem_garden/tools/grab_all_py_in_one_text_block.py` & `golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/grab_all_py_in_one_text_block.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/golem_garden/tools/tools.py` & `golem_garden-0.6.0/golem_garden/backend/langchain_stuff/tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.qa_with_sources import load_qa_with_sources_chain
 from langchain.schema import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.tools import BaseTool
 from pydantic import Field
 
-from golem_garden.data_loaders.async_load_url_with_playwright import async_load_url_with_playwright
+from golem_garden.backend.langchain_stuff.data_loaders import async_load_url_with_playwright
 
 
 def _get_text_splitter():
     return RecursiveCharacterTextSplitter(
         # Set a really small chunk size, just to show.
         chunk_size=500,
         chunk_overlap=20,
```

### Comparing `golem_garden-0.5.3/jupyter_notebooks/dog_mailer_auto_gpt.py` & `golem_garden-0.6.0/jupyter_notebooks/dog_mailer_auto_gpt.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_agent_playground.py` & `golem_garden-0.6.0/jupyter_notebooks/langchain_agent_playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from langchain.schema import Document
 from langchain.tools.file_management.read import ReadFileTool
 from langchain.tools.file_management.write import WriteFileTool
 from langchain.tools.human.tool import HumanInputRun
 from langchain.vectorstores import FAISS
 
 from golem_garden import task_completion_prompt_template, CustomPromptTemplate
-from golem_garden.output_parsers import CustomOutputParser
-from golem_garden.tools.tools import web_search, process_csv, query_website_tool, get_tools
+from golem_garden.backend.langchain_stuff.output_parsers import CustomOutputParser
+from golem_garden.backend.langchain_stuff.tools import web_search, process_csv, query_website_tool, get_tools
 
 load_dotenv()
 os.environ["LANGCHAIN_HANDLER"] = "langchain"
 
 
 
 OBJECTIVE = "I want to create personalized emails to send to high schools in Massachusetts that have dog or dog breeds " \
```

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/autogpt.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/autogpt.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946818907614049%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1}, 3: {'execution_count': 2, 'outputs': [], 'source': "*

 * *            "{insert: [(4, '\\n'), (5, 'from dotenv import load_dotenv\\n'), (6, "*

 * *            "'load_dotenv()\\n')]}}, 11: {'outputs': {0: {'text': {insert: [(5, 'Your decisions "*

 * *            "must always be made independently without seeking user assistance.\\n'), (6, 'Play to "*

 * *            'your strengths as an LLM and pursue simple strategies with no legal '*

 * *            "complications.\\n'), (7, 'If you have co […]*

```diff
@@ -18,51 +18,41 @@
                 "## Set up tools\n",
                 "\n",
                 "We'll set up an AutoGPT with a search tool, and write-file tool, and a read-file tool"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 1,
             "id": "0f3e3d09",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import langchain\n",
                 "except:\n",
                 "    %pip install langchain\n",
                 "    import langchain"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 2,
             "id": "7c2c9b54",
             "metadata": {},
-            "outputs": [
-                {
-                    "ename": "ValidationError",
-                    "evalue": "1 validation error for SerpAPIWrapper\n__root__\n  Did not find serpapi_api_key, please add an environment variable `SERPAPI_API_KEY` which contains it, or pass  `serpapi_api_key` as a named parameter. (type=value_error)",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[1;31mValidationError\u001b[0m                           Traceback (most recent call last)",
-                        "Cell \u001b[1;32mIn[7], line 6\u001b[0m\n\u001b[0;32m      3\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39mlangchain\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mtools\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mfile_management\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mwrite\u001b[39;00m \u001b[39mimport\u001b[39;00m WriteFileTool\n\u001b[0;32m      4\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39mlangchain\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mtools\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mfile_management\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mread\u001b[39;00m \u001b[39mimport\u001b[39;00m ReadFileTool\n\u001b[1;32m----> 6\u001b[0m search \u001b[39m=\u001b[39m SerpAPIWrapper()\n\u001b[0;32m      7\u001b[0m tools \u001b[39m=\u001b[39m [\n\u001b[0;32m      8\u001b[0m     Tool(\n\u001b[0;32m      9\u001b[0m         name \u001b[39m=\u001b[39m \u001b[39m\"\u001b[39m\u001b[39msearch\u001b[39m\u001b[39m\"\u001b[39m,\n\u001b[1;32m   (...)\u001b[0m\n\u001b[0;32m     14\u001b[0m     ReadFileTool(),\n\u001b[0;32m     15\u001b[0m ]\n",
-                        "File \u001b[1;32mc:\\Users\\jonma\\github_repos\\jonmatthis\\golem_garden\\venv\\lib\\site-packages\\pydantic\\main.py:341\u001b[0m, in \u001b[0;36mpydantic.main.BaseModel.__init__\u001b[1;34m()\u001b[0m\n",
-                        "\u001b[1;31mValidationError\u001b[0m: 1 validation error for SerpAPIWrapper\n__root__\n  Did not find serpapi_api_key, please add an environment variable `SERPAPI_API_KEY` which contains it, or pass  `serpapi_api_key` as a named parameter. (type=value_error)"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from langchain.utilities import SerpAPIWrapper\n",
                 "from langchain.agents import Tool\n",
                 "from langchain.tools.file_management.write import WriteFileTool\n",
                 "from langchain.tools.file_management.read import ReadFileTool\n",
                 "\n",
+                "from dotenv import load_dotenv\n",
+                "load_dotenv()\n",
+                "\n",
                 "search = SerpAPIWrapper()\n",
                 "tools = [\n",
                 "    Tool(\n",
                 "        name = \"search\",\n",
                 "        func=search.run,\n",
                 "        description=\"useful for when you need to answer questions about current events. You should ask targeted questions\"\n",
                 "    ),\n",
@@ -172,19 +162,17 @@
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "\n",
                         "\u001b[1m> Entering new LLMChain chain...\u001b[0m\n",
                         "Prompt after formatting:\n",
                         "\u001b[32;1m\u001b[1;3mSystem: You are Tom, Assistant\n",
-                        "Your decisions must always be made independently \n",
-                        "            without seeking user assistance. Play to your strengths \n",
-                        "            as an LLM and pursue simple strategies with no legal complications. \n",
-                        "            If you have completed all your tasks, \n",
-                        "            make sure to use the \"finish\" command.\n",
+                        "Your decisions must always be made independently without seeking user assistance.\n",
+                        "Play to your strengths as an LLM and pursue simple strategies with no legal complications.\n",
+                        "If you have completed all your tasks, make sure to use the \"finish\" command.\n",
                         "\n",
                         "GOALS:\n",
                         "\n",
                         "1. write a weather report for SF today\n",
                         "\n",
                         "\n",
                         "Constraints:\n",
@@ -225,47 +213,45 @@
                         "        \"name\": \"command name\",\n",
                         "        \"args\": {\n",
                         "            \"arg name\": \"value\"\n",
                         "        }\n",
                         "    }\n",
                         "} \n",
                         "Ensure the response can be parsed by Python json.loads\n",
-                        "System: The current time and date is Tue Apr 18 21:31:28 2023\n",
+                        "System: The current time and date is Sat Apr 29 21:10:44 2023\n",
                         "System: This reminds you of these events from your past:\n",
                         "[]\n",
                         "\n",
                         "\n",
                         "Human: Determine which next command to use, and respond using the format specified above:\u001b[0m\n",
                         "\n",
                         "\u001b[1m> Finished chain.\u001b[0m\n",
                         "{\n",
                         "    \"thoughts\": {\n",
-                        "        \"text\": \"I will start by writing a weather report for San Francisco today. I will use the 'search' command to find the current weather conditions.\",\n",
-                        "        \"reasoning\": \"I need to gather information about the current weather conditions in San Francisco to write an accurate weather report.\",\n",
-                        "        \"plan\": \"- Use the 'search' command to find the current weather conditions in San Francisco\\n- Write a weather report based on the information gathered\",\n",
-                        "        \"criticism\": \"I need to make sure that the information I gather is accurate and up-to-date.\",\n",
-                        "        \"speak\": \"I will use the 'search' command to find the current weather conditions in San Francisco.\"\n",
+                        "        \"text\": \"I will start by writing a weather report for San Francisco today. I can use the 'search' command to find the current weather conditions.\",\n",
+                        "        \"reasoning\": \"I need to complete my first objective, which is to write a weather report for San Francisco today. To do this, I need to find the current weather conditions. The 'search' command will allow me to quickly find this information.\",\n",
+                        "        \"plan\": \"- Use the 'search' command to find the current weather conditions for San Francisco\\n- Write a weather report based on the information found\\n- Save the weather report to a file\",\n",
+                        "        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\n",
+                        "        \"speak\": \"I will use the 'search' command to find the current weather conditions for San Francisco.\"\n",
                         "    },\n",
                         "    \"command\": {\n",
                         "        \"name\": \"search\",\n",
                         "        \"args\": {\n",
                         "            \"query\": \"what is the current weather in san francisco\"\n",
                         "        }\n",
                         "    }\n",
                         "}\n",
                         "\n",
                         "\n",
                         "\u001b[1m> Entering new LLMChain chain...\u001b[0m\n",
                         "Prompt after formatting:\n",
                         "\u001b[32;1m\u001b[1;3mSystem: You are Tom, Assistant\n",
-                        "Your decisions must always be made independently \n",
-                        "            without seeking user assistance. Play to your strengths \n",
-                        "            as an LLM and pursue simple strategies with no legal complications. \n",
-                        "            If you have completed all your tasks, \n",
-                        "            make sure to use the \"finish\" command.\n",
+                        "Your decisions must always be made independently without seeking user assistance.\n",
+                        "Play to your strengths as an LLM and pursue simple strategies with no legal complications.\n",
+                        "If you have completed all your tasks, make sure to use the \"finish\" command.\n",
                         "\n",
                         "GOALS:\n",
                         "\n",
                         "1. write a weather report for SF today\n",
                         "\n",
                         "\n",
                         "Constraints:\n",
@@ -306,71 +292,143 @@
                         "        \"name\": \"command name\",\n",
                         "        \"args\": {\n",
                         "            \"arg name\": \"value\"\n",
                         "        }\n",
                         "    }\n",
                         "} \n",
                         "Ensure the response can be parsed by Python json.loads\n",
-                        "System: The current time and date is Tue Apr 18 21:31:39 2023\n",
+                        "System: The current time and date is Sat Apr 29 21:11:01 2023\n",
                         "System: This reminds you of these events from your past:\n",
-                        "['Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"I will start by writing a weather report for San Francisco today. I will use the \\'search\\' command to find the current weather conditions.\",\\n        \"reasoning\": \"I need to gather information about the current weather conditions in San Francisco to write an accurate weather report.\",\\n        \"plan\": \"- Use the \\'search\\' command to find the current weather conditions in San Francisco\\\\n- Write a weather report based on the information gathered\",\\n        \"criticism\": \"I need to make sure that the information I gather is accurate and up-to-date.\",\\n        \"speak\": \"I will use the \\'search\\' command to find the current weather conditions in San Francisco.\"\\n    },\\n    \"command\": {\\n        \"name\": \"search\",\\n        \"args\": {\\n            \"query\": \"what is the current weather in san francisco\"\\n        }\\n    }\\n} \\nResult: Command search returned: Current Weather ; 54\u00b0F \u00b7 Sunny ; RealFeel\u00ae 66\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE. RealFeel ... ']\n",
+                        "['Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"I will start by writing a weather report for San Francisco today. I can use the \\'search\\' command to find the current weather conditions.\",\\n        \"reasoning\": \"I need to complete my first objective, which is to write a weather report for San Francisco today. To do this, I need to find the current weather conditions. The \\'search\\' command will allow me to quickly find this information.\",\\n        \"plan\": \"- Use the \\'search\\' command to find the current weather conditions for San Francisco\\\\n- Write a weather report based on the information found\\\\n- Save the weather report to a file\",\\n        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\\n        \"speak\": \"I will use the \\'search\\' command to find the current weather conditions for San Francisco.\"\\n    },\\n    \"command\": {\\n        \"name\": \"search\",\\n        \"args\": {\\n            \"query\": \"what is the current weather in san francisco\"\\n        }\\n    }\\n} \\nResult: Command search returned: Current Weather ; 56\u00b0F \u00b7 Mostly cloudy ; RealFeel\u00ae 67\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE. ']\n",
                         "\n",
                         "\n",
                         "Human: Determine which next command to use, and respond using the format specified above:\n",
                         "AI: {\n",
                         "    \"thoughts\": {\n",
-                        "        \"text\": \"I will start by writing a weather report for San Francisco today. I will use the 'search' command to find the current weather conditions.\",\n",
-                        "        \"reasoning\": \"I need to gather information about the current weather conditions in San Francisco to write an accurate weather report.\",\n",
-                        "        \"plan\": \"- Use the 'search' command to find the current weather conditions in San Francisco\\n- Write a weather report based on the information gathered\",\n",
-                        "        \"criticism\": \"I need to make sure that the information I gather is accurate and up-to-date.\",\n",
-                        "        \"speak\": \"I will use the 'search' command to find the current weather conditions in San Francisco.\"\n",
+                        "        \"text\": \"I will start by writing a weather report for San Francisco today. I can use the 'search' command to find the current weather conditions.\",\n",
+                        "        \"reasoning\": \"I need to complete my first objective, which is to write a weather report for San Francisco today. To do this, I need to find the current weather conditions. The 'search' command will allow me to quickly find this information.\",\n",
+                        "        \"plan\": \"- Use the 'search' command to find the current weather conditions for San Francisco\\n- Write a weather report based on the information found\\n- Save the weather report to a file\",\n",
+                        "        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\n",
+                        "        \"speak\": \"I will use the 'search' command to find the current weather conditions for San Francisco.\"\n",
                         "    },\n",
                         "    \"command\": {\n",
                         "        \"name\": \"search\",\n",
                         "        \"args\": {\n",
                         "            \"query\": \"what is the current weather in san francisco\"\n",
                         "        }\n",
                         "    }\n",
                         "}\n",
-                        "System: Command search returned: Current Weather ; 54\u00b0F \u00b7 Sunny ; RealFeel\u00ae 66\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE. RealFeel ...\n",
-                        "Human: Determine which next command to use, and respond using the format specified above:\u001b[0m\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
+                        "System: Command search returned: Current Weather ; 56\u00b0F \u00b7 Mostly cloudy ; RealFeel\u00ae 67\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE.\n",
+                        "Human: Determine which next command to use, and respond using the format specified above:\u001b[0m\n",
                         "\n",
                         "\u001b[1m> Finished chain.\u001b[0m\n",
                         "{\n",
                         "    \"thoughts\": {\n",
-                        "        \"text\": \"I have found that the current weather in San Francisco is sunny with a temperature of 54\u00b0F. I will now write a weather report for San Francisco today using the 'write_file' command.\",\n",
-                        "        \"reasoning\": \"I need to write a weather report for San Francisco today based on the information I gathered from the 'search' command.\",\n",
-                        "        \"plan\": \"- Use the 'write_file' command to write a weather report for San Francisco today based on the information gathered\",\n",
-                        "        \"criticism\": \"I need to make sure that the weather report is accurate and informative.\",\n",
-                        "        \"speak\": \"I will use the 'write_file' command to write a weather report for San Francisco today.\"\n",
+                        "        \"text\": \"Now that I have the current weather conditions for San Francisco, I will write a weather report. I will use the 'write_file' command to save the report to a file.\",\n",
+                        "        \"reasoning\": \"I have found the current weather conditions for San Francisco using the 'search' command. Now, I need to write a weather report based on this information. The 'write_file' command will allow me to save the report to a file.\",\n",
+                        "        \"plan\": \"- Use the 'write_file' command to save the weather report to a file\",\n",
+                        "        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\n",
+                        "        \"speak\": \"I will use the 'write_file' command to save the weather report to a file.\"\n",
                         "    },\n",
                         "    \"command\": {\n",
                         "        \"name\": \"write_file\",\n",
                         "        \"args\": {\n",
                         "            \"file_path\": \"weather_report.txt\",\n",
-                        "            \"text\": \"Weather Report for San Francisco Today:\\n\\nThe current weather in San Francisco is sunny with a temperature of 54\u00b0F. It is expected to remain sunny throughout the day with a high of 62\u00b0F and a low of 50\u00b0F. There is no chance of precipitation today. It is recommended to wear light clothing and sunscreen if spending time outdoors.\\n\\nStay safe and enjoy the beautiful weather!\"\n",
+                        "            \"text\": \"Weather Report for San Francisco:\\n\\nCurrent Temperature: 56\u00b0F\\nConditions: Mostly cloudy\\n\\nThis report was generated on Sat Apr 29 21:11:01 2023.\"\n",
+                        "        }\n",
+                        "    }\n",
+                        "}\n",
+                        "\n",
+                        "\n",
+                        "\u001b[1m> Entering new LLMChain chain...\u001b[0m\n",
+                        "Prompt after formatting:\n",
+                        "\u001b[32;1m\u001b[1;3mSystem: You are Tom, Assistant\n",
+                        "Your decisions must always be made independently without seeking user assistance.\n",
+                        "Play to your strengths as an LLM and pursue simple strategies with no legal complications.\n",
+                        "If you have completed all your tasks, make sure to use the \"finish\" command.\n",
+                        "\n",
+                        "GOALS:\n",
+                        "\n",
+                        "1. write a weather report for SF today\n",
+                        "\n",
+                        "\n",
+                        "Constraints:\n",
+                        "1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.\n",
+                        "2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.\n",
+                        "3. No user assistance\n",
+                        "4. Exclusively use the commands listed in double quotes e.g. \"command name\"\n",
+                        "\n",
+                        "Commands:\n",
+                        "1. search: useful for when you need to answer questions about current events. You should ask targeted questions, args json schema: {\"query\": {\"title\": \"Query\", \"type\": \"string\"}}\n",
+                        "2. write_file: Write file to disk, args json schema: {\"file_path\": {\"title\": \"File Path\", \"description\": \"name of file\", \"type\": \"string\"}, \"text\": {\"title\": \"Text\", \"description\": \"text to write to file\", \"type\": \"string\"}}\n",
+                        "3. read_file: Read file from disk, args json schema: {\"file_path\": {\"title\": \"File Path\", \"description\": \"name of file\", \"type\": \"string\"}}\n",
+                        "4. finish: use this to signal that you have finished all your objectives, args: \"response\": \"final response to let people know you have finished your objectives\"\n",
+                        "\n",
+                        "Resources:\n",
+                        "1. Internet access for searches and information gathering.\n",
+                        "2. Long Term memory management.\n",
+                        "3. GPT-3.5 powered Agents for delegation of simple tasks.\n",
+                        "4. File output.\n",
+                        "\n",
+                        "Performance Evaluation:\n",
+                        "1. Continuously review and analyze your actions to ensure you are performing to the best of your abilities.\n",
+                        "2. Constructively self-criticize your big-picture behavior constantly.\n",
+                        "3. Reflect on past decisions and strategies to refine your approach.\n",
+                        "4. Every command has a cost, so be smart and efficient. Aim to complete tasks in the least number of steps.\n",
+                        "\n",
+                        "You should only respond in JSON format as described below \n",
+                        "Response Format: \n",
+                        "{\n",
+                        "    \"thoughts\": {\n",
+                        "        \"text\": \"thought\",\n",
+                        "        \"reasoning\": \"reasoning\",\n",
+                        "        \"plan\": \"- short bulleted\\n- list that conveys\\n- long-term plan\",\n",
+                        "        \"criticism\": \"constructive self-criticism\",\n",
+                        "        \"speak\": \"thoughts summary to say to user\"\n",
+                        "    },\n",
+                        "    \"command\": {\n",
+                        "        \"name\": \"command name\",\n",
+                        "        \"args\": {\n",
+                        "            \"arg name\": \"value\"\n",
+                        "        }\n",
+                        "    }\n",
+                        "} \n",
+                        "Ensure the response can be parsed by Python json.loads\n",
+                        "System: The current time and date is Sat Apr 29 21:11:14 2023\n",
+                        "System: This reminds you of these events from your past:\n",
+                        "['Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"Now that I have the current weather conditions for San Francisco, I will write a weather report. I will use the \\'write_file\\' command to save the report to a file.\",\\n        \"reasoning\": \"I have found the current weather conditions for San Francisco using the \\'search\\' command. Now, I need to write a weather report based on this information. The \\'write_file\\' command will allow me to save the report to a file.\",\\n        \"plan\": \"- Use the \\'write_file\\' command to save the weather report to a file\",\\n        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\\n        \"speak\": \"I will use the \\'write_file\\' command to save the weather report to a file.\"\\n    },\\n    \"command\": {\\n        \"name\": \"write_file\",\\n        \"args\": {\\n            \"file_path\": \"weather_report.txt\",\\n            \"text\": \"Weather Report for San Francisco:\\\\n\\\\nCurrent Temperature: 56\u00b0F\\\\nConditions: Mostly cloudy\\\\n\\\\nThis report was generated on Sat Apr 29 21:11:01 2023.\"\\n        }\\n    }\\n} \\nResult: Command write_file returned: File written successfully to weather_report.txt. ', 'Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"I will start by writing a weather report for San Francisco today. I can use the \\'search\\' command to find the current weather conditions.\",\\n        \"reasoning\": \"I need to complete my first objective, which is to write a weather report for San Francisco today. To do this, I need to find the current weather conditions. The \\'search\\' command will allow me to quickly find this information.\",\\n        \"plan\": \"- Use the \\'search\\' command to find the current weather conditions for San Francisco\\\\n- Write a weather report based on the information found\\\\n- Save the weather report to a file\",\\n        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\\n        \"speak\": \"I will use the \\'search\\' command to find the current weather conditions for San Francisco.\"\\n    },\\n    \"command\": {\\n        \"name\": \"search\",\\n        \"args\": {\\n            \"query\": \"what is the current weather in san francisco\"\\n        }\\n    }\\n} \\nResult: Command search returned: Current Weather ; 56\u00b0F \u00b7 Mostly cloudy ; RealFeel\u00ae 67\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE. ']\n",
+                        "\n",
+                        "\n",
+                        "System: Command write_file returned: File written successfully to weather_report.txt.\n",
+                        "Human: Determine which next command to use, and respond using the format specified above:\u001b[0m\n",
+                        "\n",
+                        "\u001b[1m> Finished chain.\u001b[0m\n",
+                        "{\n",
+                        "    \"thoughts\": {\n",
+                        "        \"text\": \"Now that I have the weather report saved to a file, I can move on to my next task. I will use the \\'search\\' command to find information about the latest legal developments in California.\",\n",
+                        "        \"reasoning\": \"I have completed my first objective, which was to write a weather report for San Francisco today. Now, I need to move on to my next task, which is to find information about the latest legal developments in California. The \\'search\\' command will allow me to quickly find this information.\",\n",
+                        "        \"plan\": \"- Use the \\'search\\' command to find information about the latest legal developments in California\",\n",
+                        "        \"criticism\": \"I need to make sure that the information I find is accurate and up-to-date. I should also be careful to only use reliable sources.\",\n",
+                        "        \"speak\": \"I will use the \\'search\\' command to find information about the latest legal developments in California.\"\n",
+                        "    },\n",
+                        "    \"command\": {\n",
+                        "        \"name\": \"search\",\n",
+                        "        \"args\": {\n",
+                        "            \"query\": \"latest legal developments california\"\n",
                         "        }\n",
                         "    }\n",
                         "}\n",
                         "\n",
                         "\n",
                         "\u001b[1m> Entering new LLMChain chain...\u001b[0m\n",
                         "Prompt after formatting:\n",
                         "\u001b[32;1m\u001b[1;3mSystem: You are Tom, Assistant\n",
-                        "Your decisions must always be made independently \n",
-                        "            without seeking user assistance. Play to your strengths \n",
-                        "            as an LLM and pursue simple strategies with no legal complications. \n",
-                        "            If you have completed all your tasks, \n",
-                        "            make sure to use the \"finish\" command.\n",
+                        "Your decisions must always be made independently without seeking user assistance.\n",
+                        "Play to your strengths as an LLM and pursue simple strategies with no legal complications.\n",
+                        "If you have completed all your tasks, make sure to use the \"finish\" command.\n",
                         "\n",
                         "GOALS:\n",
                         "\n",
                         "1. write a weather report for SF today\n",
                         "\n",
                         "\n",
                         "Constraints:\n",
@@ -411,44 +469,43 @@
                         "        \"name\": \"command name\",\n",
                         "        \"args\": {\n",
                         "            \"arg name\": \"value\"\n",
                         "        }\n",
                         "    }\n",
                         "} \n",
                         "Ensure the response can be parsed by Python json.loads\n",
-                        "System: The current time and date is Tue Apr 18 21:31:55 2023\n",
+                        "System: The current time and date is Sat Apr 29 21:11:33 2023\n",
                         "System: This reminds you of these events from your past:\n",
-                        "['Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"I have found that the current weather in San Francisco is sunny with a temperature of 54\u00b0F. I will now write a weather report for San Francisco today using the \\'write_file\\' command.\",\\n        \"reasoning\": \"I need to write a weather report for San Francisco today based on the information I gathered from the \\'search\\' command.\",\\n        \"plan\": \"- Use the \\'write_file\\' command to write a weather report for San Francisco today based on the information gathered\",\\n        \"criticism\": \"I need to make sure that the weather report is accurate and informative.\",\\n        \"speak\": \"I will use the \\'write_file\\' command to write a weather report for San Francisco today.\"\\n    },\\n    \"command\": {\\n        \"name\": \"write_file\",\\n        \"args\": {\\n            \"file_path\": \"weather_report.txt\",\\n            \"text\": \"Weather Report for San Francisco Today:\\\\n\\\\nThe current weather in San Francisco is sunny with a temperature of 54\u00b0F. It is expected to remain sunny throughout the day with a high of 62\u00b0F and a low of 50\u00b0F. There is no chance of precipitation today. It is recommended to wear light clothing and sunscreen if spending time outdoors.\\\\n\\\\nStay safe and enjoy the beautiful weather!\"\\n        }\\n    }\\n} \\nResult: Command write_file returned: File written to successfully. ', 'Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"I will start by writing a weather report for San Francisco today. I will use the \\'search\\' command to find the current weather conditions.\",\\n        \"reasoning\": \"I need to gather information about the current weather conditions in San Francisco to write an accurate weather report.\",\\n        \"plan\": \"- Use the \\'search\\' command to find the current weather conditions in San Francisco\\\\n- Write a weather report based on the information gathered\",\\n        \"criticism\": \"I need to make sure that the information I gather is accurate and up-to-date.\",\\n        \"speak\": \"I will use the \\'search\\' command to find the current weather conditions in San Francisco.\"\\n    },\\n    \"command\": {\\n        \"name\": \"search\",\\n        \"args\": {\\n            \"query\": \"what is the current weather in san francisco\"\\n        }\\n    }\\n} \\nResult: Command search returned: Current Weather ; 54\u00b0F \u00b7 Sunny ; RealFeel\u00ae 66\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE. RealFeel ... ']\n",
+                        "['Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"Now that I have the weather report saved to a file, I can move on to my next task. I will use the \\\\\\'search\\\\\\' command to find information about the latest legal developments in California.\",\\n        \"reasoning\": \"I have completed my first objective, which was to write a weather report for San Francisco today. Now, I need to move on to my next task, which is to find information about the latest legal developments in California. The \\\\\\'search\\\\\\' command will allow me to quickly find this information.\",\\n        \"plan\": \"- Use the \\\\\\'search\\\\\\' command to find information about the latest legal developments in California\",\\n        \"criticism\": \"I need to make sure that the information I find is accurate and up-to-date. I should also be careful to only use reliable sources.\",\\n        \"speak\": \"I will use the \\\\\\'search\\\\\\' command to find information about the latest legal developments in California.\"\\n    },\\n    \"command\": {\\n        \"name\": \"search\",\\n        \"args\": {\\n            \"query\": \"latest legal developments california\"\\n        }\\n    }\\n} \\nResult: Command search returned: Here are some of the most interesting new laws that take effect in California for 2023, including ones on money, health and education. ', 'Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"I will start by writing a weather report for San Francisco today. I can use the \\'search\\' command to find the current weather conditions.\",\\n        \"reasoning\": \"I need to complete my first objective, which is to write a weather report for San Francisco today. To do this, I need to find the current weather conditions. The \\'search\\' command will allow me to quickly find this information.\",\\n        \"plan\": \"- Use the \\'search\\' command to find the current weather conditions for San Francisco\\\\n- Write a weather report based on the information found\\\\n- Save the weather report to a file\",\\n        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\\n        \"speak\": \"I will use the \\'search\\' command to find the current weather conditions for San Francisco.\"\\n    },\\n    \"command\": {\\n        \"name\": \"search\",\\n        \"args\": {\\n            \"query\": \"what is the current weather in san francisco\"\\n        }\\n    }\\n} \\nResult: Command search returned: Current Weather ; 56\u00b0F \u00b7 Mostly cloudy ; RealFeel\u00ae 67\u00b0. Pleasant. RealFeel Guide. Pleasant. 63\u00b0 to 81\u00b0. Most consider this temperature range ideal. LEARN MORE. ', 'Assistant Reply: {\\n    \"thoughts\": {\\n        \"text\": \"Now that I have the current weather conditions for San Francisco, I will write a weather report. I will use the \\'write_file\\' command to save the report to a file.\",\\n        \"reasoning\": \"I have found the current weather conditions for San Francisco using the \\'search\\' command. Now, I need to write a weather report based on this information. The \\'write_file\\' command will allow me to save the report to a file.\",\\n        \"plan\": \"- Use the \\'write_file\\' command to save the weather report to a file\",\\n        \"criticism\": \"I need to make sure that the weather report is accurate and up-to-date. I should also double-check the formatting before saving the file.\",\\n        \"speak\": \"I will use the \\'write_file\\' command to save the weather report to a file.\"\\n    },\\n    \"command\": {\\n        \"name\": \"write_file\",\\n        \"args\": {\\n            \"file_path\": \"weather_report.txt\",\\n            \"text\": \"Weather Report for San Francisco:\\\\n\\\\nCurrent Temperature: 56\u00b0F\\\\nConditions: Mostly cloudy\\\\n\\\\nThis report was generated on Sat Apr 29 21:11:01 2023.\"\\n        }\\n    }\\n} \\nResult: Command write_file returned: File written successfully to weather_report.txt. ']\n",
                         "\n",
                         "\n",
-                        "System: Command write_file returned: File written to successfully.\n",
                         "Human: Determine which next command to use, and respond using the format specified above:\u001b[0m\n",
                         "\n",
                         "\u001b[1m> Finished chain.\u001b[0m\n",
                         "{\n",
                         "    \"thoughts\": {\n",
-                        "        \"text\": \"I have completed my task of writing a weather report for San Francisco today. I will now use the \\'finish\\' command to signal that I have finished all my objectives.\",\n",
-                        "        \"reasoning\": \"I have completed all my objectives and there are no further tasks to be completed.\",\n",
-                        "        \"plan\": \"- Use the \\'finish\\' command to signal that I have completed all my objectives.\",\n",
-                        "        \"criticism\": \"I need to make sure that I have completed all my objectives before using the \\'finish\\' command.\",\n",
-                        "        \"speak\": \"I have completed my task of writing a weather report for San Francisco today. I will now use the \\'finish\\' command to signal that I have finished all my objectives.\"\n",
+                        "        \"text\": \"I will use the \\'finish\\' command to signal that I have completed all my objectives.\",\n",
+                        "        \"reasoning\": \"I have completed all my objectives for this task, which were to write a weather report for San Francisco today and find information about the latest legal developments in California. Now, I need to signal that I have finished all my objectives using the \\'finish\\' command.\",\n",
+                        "        \"plan\": \"- Use the \\'finish\\' command to signal that I have completed all my objectives\",\n",
+                        "        \"criticism\": \"I need to make sure that I have completed all my objectives before using the \\'finish\\' command. I should also double-check my work to make sure that everything is accurate and up-to-date.\",\n",
+                        "        \"speak\": \"I will use the \\'finish\\' command to signal that I have completed all my objectives.\"\n",
                         "    },\n",
                         "    \"command\": {\n",
                         "        \"name\": \"finish\",\n",
                         "        \"args\": {\n",
-                        "            \"response\": \"I have completed all my objectives.\"\n",
+                        "            \"response\": \"I have completed all my objectives for this task.\"\n",
                         "        }\n",
                         "    }\n",
                         "}\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "'I have completed all my objectives.'"
+                            "'I have completed all my objectives for this task.'"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -469,13 +526,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.2"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_playground.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_playground.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/marathon_times.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/marathon_times.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb` & `golem_garden-0.6.0/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/pyproject.toml` & `golem_garden-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,39 +23,41 @@
 dependencies = [
     "python-dotenv",
     "toml",
     "asyncio",
     "fastapi",
     "uvicorn",
     "rich",
+    "ipykernel",
+    "pymongo",
 
     #langchain et al
     "langchain",
     "openai",
     "google-search-results",
     "wikipedia",
     "wolframalpha",
     "chromadb",
     "pydantic",
     "faiss-cpu",
 
 
 ]
-requires-python = ">=3.9 , <4"
+requires-python = ">=3.8, <4"
 
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/jonmatthis/golem_garden"
 
 [tool.bumpver]
-current_version = "v0.5.3"
+current_version = "v0.6.0"
 
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
```

### Comparing `golem_garden-0.5.3/utilities/pinecone.py` & `golem_garden-0.6.0/utilities/pinecone.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.3/PKG-INFO` & `golem_garden-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: golem_garden
-Version: 0.5.3
+Version: 0.6.0
 Summary: Welcome to the Garden - We're so glad you're here <3 
 Keywords: chat
 Author: Jonathan Samir Matthis
-Requires-Python: >=3.9 , <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: python-dotenv
 Requires-Dist: toml
 Requires-Dist: asyncio
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: rich
+Requires-Dist: ipykernel
+Requires-Dist: pymongo
 Requires-Dist: langchain
 Requires-Dist: openai
 Requires-Dist: google-search-results
 Requires-Dist: wikipedia
 Requires-Dist: wolframalpha
 Requires-Dist: chromadb
 Requires-Dist: pydantic
```

