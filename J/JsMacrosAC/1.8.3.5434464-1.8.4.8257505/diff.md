# Comparing `tmp/JsMacrosAC-1.8.3.5434464.tar.gz` & `tmp/JsMacrosAC-1.8.4.8257505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/JsMacrosAC-1.8.3.5434464.tar", last modified: Mon Oct 10 20:41:04 2022, max compression
+gzip compressed data, was "dist/JsMacrosAC-1.8.4.8257505.tar", last modified: Sun Jul  2 00:25:05 2023, max compression
```

## Comparing `JsMacrosAC-1.8.3.5434464.tar` & `JsMacrosAC-1.8.4.8257505.tar`

### file list

```diff
@@ -1,411 +1,591 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-10 20:40:02.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AboutOverlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-10-10 20:40:02.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractMapSettingContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-10-10 20:40:02.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractRenderCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractSettingContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractSettingField.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AndFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AnnotatedCheckBox.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AutoCompleteSuggestion.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/AutoCompleteSuggestor.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseEventRegistry.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseLanguage.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseLibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseListener.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseProfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseScriptContext.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseScriptContext_ScriptAssertionError.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-10 20:40:03.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseScriptContext_SleepRunnable.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseWrappedException.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseWrappedException_GuestLocation.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseWrappedException_HostLocation.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseWrappedException_SourceLocation.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BasicFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BeaconInventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockDataHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockPosHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockStateFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3594 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockStateHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BooleanCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BooleanField.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BossBarConsumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/BossBarHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Button.py
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ButtonWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-10-10 20:40:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CancelScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CancelScreen_RTCSort.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CategoryTreeContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CharCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ChatHistoryManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ChatHudLineHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CheckBoxContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_AnnotationBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_BodyBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_ConstructorBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_FieldBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_MethodBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassWrapperFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-10-10 20:40:05.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClientConfigV2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4071 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClientPlayerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CodeCompileEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ColorMapSetting.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ColorMapSetting_ColorEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandContextHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandNodeAccessor.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandNodeHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ConfigFolder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ConfirmOverlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Core.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CoreConfigV2.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/CustomClickEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/DefaultCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-10 20:40:06.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/DocletReplaceParams.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/DocletReplaceReturn.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/DoubleField.py
--rw-r--r--   0 runner    (1001) docker     (121)     7851 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw2D.py
--rw-r--r--   0 runner    (1001) docker     (121)     6909 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D_Box.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D_Line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D_Surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EditorScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EnchantInventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5328 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Event.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventAirChange.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventArmorChange.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventAttackBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventAttackEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-10 20:40:07.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventBlockUpdate.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventBossbar.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventChooser.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventChooser_EventObj.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventChunkLoad.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventChunkUnload.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventClickSlot.py
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventCustom.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventDamage.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventDeath.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventDimensionChange.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventDisconnect.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventDropSlot.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventEXPChange.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-10-10 20:40:08.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventEntityDamaged.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventEntityHealed.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventEntityLoad.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventEntityUnload.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventFallFlying.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventHeal.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventHeldItemChange.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventHungerChange.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventInteractBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventInteractEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventItemDamage.py
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventItemPickup.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventJoinServer.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventJoinedKey.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventJoinedTick.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventKey.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventListener.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-10 20:40:09.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventLockWatchdog.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventMacrosScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventOpenContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventOpenScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventPlayerJoin.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventPlayerLeave.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventProfileLoad.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventRecvMessage.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventRegistry.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventResourcePackLoaded.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventRiding.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventSendMessage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventService.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventSignEdit.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventSound.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventTick.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventTitle.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventWrappedScript.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Extension.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ExtensionClassLoader.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ExtensionLoader.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Extension_ExtMatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FChat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3736 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FClient.py
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FFS.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FGlobalVars.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FHud.py
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FJsMacros.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FJsMacros_EventAndContext.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FJsMacros_ScriptEventListener.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FKeyBind.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FKeyBind_KeyTracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     7507 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FPlayer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FPositionCommon.py
--rw-r--r--   0 runner    (1001) docker     (121)     5738 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FReflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FReflection_CombinedVariableClassLoader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FTime.py
--rw-r--r--   0 runner    (1001) docker     (121)     8731 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FWorld.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileChooser.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-10-10 20:40:11.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileChooser_fileObj.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileChooser_sortFile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileField.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileMapSetting.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileMapSetting_FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-10 20:40:12.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/FloatField.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/GroupFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/GroupFilter_AllMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/GroupFilter_AnyMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/GroupFilter_CountMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/GroupFilter_NoneMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/HTTPRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/HTTPRequest_Response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_Add.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_HistoryStep.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_Remove.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_Replace.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_ShiftLine.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_TabLines.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/History_TabLinesKeepCursor.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IAdvancedFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IBeaconScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IBossBarHud.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ICategoryTreeParent.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IChatHud.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IChunkSection.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IClientPlayerEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ICompare.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IContainerParent.py
--rw-r--r--   0 runner    (1001) docker     (121)    15623 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IDraw2D.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IEventListener.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IFWrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-10 20:40:14.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IFontManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IHorseScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IInventory.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IItemCooldownEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IItemCooldownManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ILoomScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IMerchantEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IMerchantScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IMinecraftClient.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IMixinEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IOverlayParent.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IPackedIntegerArray.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IPalettedContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IPalettedContainerData.py
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IPlayerListHud.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IRecipeBookResults.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IRecipeBookWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IResourcePackManager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ISignEditScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/IntField.py
--rw-r--r--   0 runner    (1001) docker     (121)     4809 2022-10-10 20:40:15.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ItemEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ItemStackHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/JsMacros.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/KeyListener.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/KeyMacrosScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Library.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/LibraryBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/LibraryRegistry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ListContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/LivingEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/LongField.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/LoomInventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MacroContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MacroListTopbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MacroScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Mappings.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Mappings_ClassData.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Mappings_MappedClass.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Mappings_MethodData.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MerchantEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MethodWrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinBeaconScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinBossBarHud.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinChatHud.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-10 20:40:17.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinChunkSelection.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientPlayNetworkHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientPlayerEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientPlayerInteractionManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientWorld.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinCreativeInventoryScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinDisconnectedScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinFontManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinFontStorage.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinHandledScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinHorseScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinHungerManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-10 20:40:18.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinItemCooldownEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinItemCooldownManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinLivingEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinLoomScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinMerchantEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinMerchantScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinMinecraftClient.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPackedIntegerArray.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPalettedContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPalettedContainerData.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPlayerEntity.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPlayerListHud.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinRecipeBookResults.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinRecipeBookWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinResourcePackManager.py
--rw-r--r--   0 runner    (1001) docker     (121)     9606 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinSignEditScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinSimpleOption.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinSoundSystem.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinSplashOverlay.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinStatHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinStyleSerializer.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinTranslationStorage.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinTrueTypeFont.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MovementDummy.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MovementQueue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-10 20:40:20.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/MultiElementContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper_NBTListHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Neighbor.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NoStyleCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NotFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/NumberCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Option.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/OptionType.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/OptionsField.py
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/OptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/OrFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/OverlayContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Pair.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PerExecLanguageLibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-10 20:40:21.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PerExecLibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PerLanguageLibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerAbilitiesHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerInput.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerListEntryHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Plane3D.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Pos2D.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Pos3D.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Vec2D.py
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Vec3D.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PrimitiveSettingGroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/PrioryFiFoTaskQueue.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_clike.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-10 20:40:22.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_groovy.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_javascript.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_kotlin.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_lua.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_python.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_regex.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_ruby.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism_typescript.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Profile.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProfileSetting.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProfileSetting_ProfileEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProxyBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProxyBuilder_ProxyReference.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RecipeHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-10 20:40:23.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Rect.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_RenderElement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Text.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/RunningContextContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScoreboardObjectiveHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScoreboardsHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptTrigger.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptTrigger_TriggerType.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Scrollbar.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/SelectCursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/SelectorDropdownOverlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServerInfoHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceListTopbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceManager.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceManager_ServiceStatus.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceScreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceTrigger.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/SettingsOverlay.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/SettingsOverlay_SettingField.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Sorting.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Sorting_MacroSortMethod.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Sorting_SortByEnabled.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Sorting_SortByFileName.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Sorting_SortByTriggerName.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StatsHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StatusEffectHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-10 20:40:25.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringCompareFilter_FilterMethod.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringField.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringHashTrie.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringMapSetting.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringMapSetting_StringEntry.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringifyFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/StyleHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/SuggestionsBuilderHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/SynchronizedWeakHashSet.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TPSData.py
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TeamHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextFieldWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextInput.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextOverlay.py
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextPrompt.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-10 20:40:26.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextStyleCompiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TickBasedEvents.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TickSync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TradeOfferHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/TranslationUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Util.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/VillagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/VillagerInventory.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Websocket.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/Websocket_Disconnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/WorldScanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/WorldScannerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-10 20:40:27.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/WrappedClassInstance.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-10 20:40:28.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/WrappedClassInstance_MethodSigParts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-10-10 20:40:28.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/WrappedScript.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-10 20:40:28.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/XorFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-10 20:40:02.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-10-10 20:40:10.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-10-10 20:40:13.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-10 20:40:16.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/libraries.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-10-10 20:40:19.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    12273 2022-10-10 20:40:24.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12616 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-10-10 20:40:01.000000 JsMacrosAC-1.8.3.5434464/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-10 20:41:04.000000 JsMacrosAC-1.8.3.5434464/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-10-10 20:40:01.000000 JsMacrosAC-1.8.3.5434464/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AboutOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractHorseEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractMapSettingContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractPiglinEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractRenderCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractSettingContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractSettingField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractWidgetBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AdvancementHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AdvancementManagerHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AdvancementProgressHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Alignable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AllayEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AndFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AnimalEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AnnotatedCheckBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AnvilInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AreaEffectCloudEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ArmorStandEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ArrowEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AutoCompleteSuggester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AutoCompleteSuggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/AxolotlEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseEventRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseScriptContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseScriptContext_ScriptAssertionError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseScriptContext_SleepRunnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseWrappedException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseWrappedException_GuestLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseWrappedException_HostLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseWrappedException_SourceLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BasicFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BeaconInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BeeEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlazeEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockDataHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockPosHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockStateFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockStateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BoatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BooleanCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BooleanField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BossBarConsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BossBarHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Box_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/BrewingStandInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ButtonWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ButtonWidgetHelper_ButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ButtonWidgetHelper_TexturedButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CancelScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CancelScreen_RTCSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CartographyInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CategoryTreeContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CharCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ChatHistoryManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ChatHudLineHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CheckBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CheckBoxContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CheckBoxWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CheckBoxWidgetHelper_CheckBoxBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ChunkHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_AnnotationBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_BodyBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-02 00:24:24.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_ConstructorBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_FieldBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_MethodBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassWrapperFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClickableWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClientConfigV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClientPlayerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CodeCompileEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ColorMapSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ColorMapSetting_ColorEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandContextHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandNodeAccessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandNodeHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ConfigFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ConfirmOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ContainerInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CoreConfigV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CraftingInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CreativeInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CreativeItemStackHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CreeperEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CustomClickEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CustomImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CyclingButtonWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/CyclingButtonWidgetHelper_CyclicButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DefaultCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DirectionHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DocletEnumType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DocletReplaceParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DocletReplaceReturn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DocletReplaceTypeParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DocletTypescriptExtends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DolphinEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DonkeyEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DoubleField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw2DElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw2DElement_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DrownedEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/DyeColorHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EditorScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-02 00:24:25.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EnchantInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EnchantmentHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EndCrystalEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EnderDragonEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EndermanEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventAirChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventArmorChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventAttackBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventAttackEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventBlockUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventBossbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 00:24:30.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventChooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventChooser_EventObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventChunkLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventChunkUnload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventClickSlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventDeath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventDimensionChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventDisconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventDropSlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventEXPChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventEntityDamaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventEntityHealed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventEntityLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventEntityUnload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventFallFlying.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventHeal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventHealthChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventHeldItemChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventHungerChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 00:24:31.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventInteractBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventInteractEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventItemDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventItemPickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventJoinServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventJoinedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventJoinedRecvPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventJoinedSendPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventJoinedTick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventLaunchGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventLockWatchdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventMacrosScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventOpenContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventOpenScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventPlayerJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventPlayerLeave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventProfileLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventQuitGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventRecvMessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventRecvPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventResourcePackLoaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventRiding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventSendMessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventSendPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventSignEdit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventSound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventStatusEffectUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventTick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventWrappedScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ExtensionClassLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ExtensionLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Extension_ExtMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FChat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FGlobalVars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FJavaUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FJsMacros.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FJsMacros_EventAndContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FJsMacros_ScriptEventListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FKeyBind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FKeyBind_KeyTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FPositionCommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FReflection_CombinedVariableClassLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FWorld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FakeServerCommandSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FallingBlockEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileChooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileChooser_fileObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileChooser_sortFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileHandler_FileLineIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileMapSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileMapSetting_FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FishEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FishingBobberEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FloatField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FluidStateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FoodComponentHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FormattingHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FoxEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FrogEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FurnaceInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/FurnaceMinecartEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GhastEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GoatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GrindStoneInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GroupFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GroupFilter_AllMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GroupFilter_AnyMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GroupFilter_CountMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GroupFilter_NoneMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/GuardianEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/HTTPRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/HTTPRequest_Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_Add.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_HistoryStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_Remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_Replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_ShiftLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_TabLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/History_TabLinesKeepCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/HorseEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/HorseInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IAdvancedFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IBeaconScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IBossBarHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ICancelable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ICategoryTreeParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IChatHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IChunkSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ICompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IContainerParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21949 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IDraw2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IEventListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IFWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IFontManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IHorseScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IItemCooldownEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IItemCooldownManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ILoomScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IMerchantEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IMerchantScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IMinecraftClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IMixinEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IOverlayParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IPackedIntegerArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IPalettedContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IPalettedContainerData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IPlayerListHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IRecipeBookResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IRecipeBookWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IResourcePackManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IScreenInternal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ISignEditScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IllagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Image_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IntField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/IronGolemEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ItemEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ItemFrameEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ItemHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ItemStackHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Item_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/JsMacros.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-02 00:24:34.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/JsMacrosThreadPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/JsMacrosThreadPool_PoolThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/KeyListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/KeyMacrosScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LibraryBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LibraryRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Line3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Line3D_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Line_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ListContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LivingEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LlamaEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LockButtonWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LockButtonWidgetHelper_LockButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LongField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/LoomInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MacroContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MacroListTopbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MacroScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Mappings_ClassData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Mappings_MappedClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Mappings_MethodData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MerchantEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MethodWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAbstractFurnaceScreenHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAbstractHorseEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAbstractPiglinEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAdvancementManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAdvancementProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAdvancementRewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAllayEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinAnvilScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinBeaconScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinBoatEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinBossBarHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinChatHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinChatScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinChunkSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientAdvancementManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientPlayNetworkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientPlayerInteractionManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientWorld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinCreativeInventoryScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinCreeperEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinCyclingButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinDisconnectedScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinFishingBobberEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinFontManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinFontStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinFoxEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinHandledScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinHorseEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinHorseScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinHungerManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinItemCooldownEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinItemCooldownManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinLivingEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinLoomScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinMerchantEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinMerchantScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinMinecraftClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinOcelotEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPackedIntegerArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPacketHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPalettedContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPalettedContainerData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPhaseType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPlayerEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPlayerListHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinRecipeBookResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinRecipeBookWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinResourcePackManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinShulkerEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinSignEditScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinSimpleOption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinSoundSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinSpellcastingIllagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinSplashOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinStatHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinStyleSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinTextFieldWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinTranslationStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinTridentEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinTrueTypeFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MobEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ModContainerHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ModLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MooshroomEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MovementDummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MovementQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/MultiElementContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper_NBTListHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NameUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NoStyleCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NotFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/NumberCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OcelotEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper_AccessibilityOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper_ChatOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper_ControlOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper_MusicOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper_SkinOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsHelper_VideoOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OrFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/OverlayContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33397 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PacketByteBufferHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PaintingEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PandaEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ParrotEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PerExecLanguageLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PerExecLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PerLanguageLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PhantomEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PigEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PiglinEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PillagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Plane3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerAbilitiesHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerListEntryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PolarBearEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Pos2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Pos3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PrimitiveSettingGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PrioryFiFoTaskQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_clike.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_groovy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_kotlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_lua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_ruby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 00:24:37.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProfileSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProfileSetting_ProfileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProxyBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProxyBuilder_ProxyReference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/PufferfishEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RabbitEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RecipeHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RecipeInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Rect_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RegistryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RenderElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RenderElement3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RenderElementBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/RunningContextContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScoreboardObjectiveHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScoreboardsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptTrigger_TriggerType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Scrollbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SelectCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SelectorDropdownOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServerInfoHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceListTopbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceManager_ServiceStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SettingsOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SettingsOverlay_SettingField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SheepEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ShulkerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SliderWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SliderWidgetHelper_SliderBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SlimeEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SmithingInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SnowGolemEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_MacroSortMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_ServiceSortMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortByEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortByFileName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortByTriggerName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortServiceByEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortServiceByFileName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortServiceByName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Sorting_SortServiceByRunning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SpellcastingIllagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SpiderEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StatsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StatusEffectHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StoneCutterInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StriderEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringCompareFilter_FilterMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringHashTrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringMapSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringMapSetting_StringEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringifyFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/StyleHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SuggestionsBuilderHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Surface_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/SynchronizedWeakHashSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TPSData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TameableEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TeamHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextFieldWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextFieldWidgetHelper_TextFieldBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextStyleCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Text_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TickBasedEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TickSync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TntEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TntMinecartEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TradeOfferHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TranslationUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TridentEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/TropicalFishEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/UniversalBlockStateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Vec2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Vec3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/VexEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/VillagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/VillagerInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/VindicatorEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WardenEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/Websocket_Disconnected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-02 00:24:39.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WitchEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WitherEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WitherSkullEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WolfEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WorldScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WorldScannerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WrappedClassInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WrappedClassInstance_MethodSigParts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/WrappedScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/XorFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ZombieEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-02 00:24:40.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/ZombieVillagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-02 00:24:32.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-02 00:24:33.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-02 00:24:35.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-02 00:24:36.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-02 00:24:38.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:25:05.000000 JsMacrosAC-1.8.4.8257505/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 00:24:23.000000 JsMacrosAC-1.8.4.8257505/setup.py
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AboutOverlay.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AboutOverlay.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 		pass
 
 	@overload
 	def setMessage(self, message: Text) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractMapSettingContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractMapSettingContainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,13 +55,13 @@
 		pass
 
 	@overload
 	def addSetting(self, setting: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 		pass
 
 	@overload
 	def setValue(self, newValue: T) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractRenderCodeCompiler.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractRenderCodeCompiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
 Runnable = TypeVar["java.lang.Runnable"]
+Text = TypeVar["net.minecraft.text.Text"]
 
 class AbstractRenderCodeCompiler:
 
 	@overload
 	def __init__(self, language: str, screen: EditorScreen) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractSettingContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractSettingContainer.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AbstractSettingField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AbstractSettingField.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/AnnotatedCheckBox.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AnnotatedCheckBox.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 Text = TypeVar["net.minecraft.text.Text"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
 class AnnotatedCheckBox(Button):
 	value: bool
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, hilightColor: int, textColor: int, message: Text, initialValue: bool, onPress: Consumer) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: Text, initialValue: bool, onPress: Consumer) -> None:
 		pass
 
 	@overload
 	def onPress(self) -> None:
 		pass
 
 	@overload
 	def setMessage(self, message: Text) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseEventRegistry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseEventRegistry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseLanguage.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseLanguage.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseListener.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseListener.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,13 +23,17 @@
 		pass
 
 	@overload
 	def equals(self, o: object) -> bool:
 		pass
 
 	@overload
+	def off(self) -> None:
+		pass
+
+	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseProfile.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseProfile.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseScreen.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 		pass
 
 	@overload
 	def mouseClicked(self, mouseX: float, mouseY: float, button: int) -> bool:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def shouldCloseOnEsc(self) -> bool:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseScriptContext.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseScriptContext.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BaseWrappedException.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BaseWrappedException.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BasicFilter.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BasicFilter.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BeaconInventory.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BeaconInventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,10 +51,14 @@
 	@overload
 	def applyEffects(self) -> bool:
 		"""
 		Since: 1.5.1 
 		"""
 		pass
 
+	@overload
+	def toString(self) -> str:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockDataHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockDataHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,24 @@
 	def getBlockHelper(self) -> BlockHelper:
 		"""
 		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
+	def getBlock(self) -> BlockHelper:
+		"""
+		Since: 1.6.5 
+
+		Returns:
+			the block 
+		"""
+		pass
+
+	@overload
 	def getBlockState(self) -> Mapping[str, str]:
 		"""
 		Since: 1.1.7 
 
 		Returns:
 			block state data as a Map . 
 		"""
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .BlockStateHelper import BlockStateHelper
 from .ItemStackHelper import ItemStackHelper
+from .TextHelper import TextHelper
 
 Block = TypeVar["net.minecraft.block.Block"]
 
 class BlockHelper(BaseHelper):
 	"""
 	Since: 1.6.5 
 	"""
@@ -127,13 +128,23 @@
 
 		Returns:
 			the identifier of the block. 
 		"""
 		pass
 
 	@overload
+	def getName(self) -> TextHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the name of the block. 
+		"""
+		pass
+
+	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockPosHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/DirectionHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,143 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
+from .Pos3D import Pos3D
 
-BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
+Direction = TypeVar["net.minecraft.util.math.Direction"]
 
-class BlockPosHelper(BaseHelper):
+class DirectionHelper(BaseHelper):
 	"""
-	Since: 1.2.6 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, b: BlockPos) -> None:
+	def __init__(self, base: Direction) -> None:
 		pass
 
 	@overload
-	def __init__(self, x: int, y: int, z: int) -> None:
-		pass
-
-	@overload
-	def getX(self) -> int:
-		"""
-		Since: 1.2.6 
-
-		Returns:
-			the 'x' value of the block. 
-		"""
-		pass
-
-	@overload
-	def getY(self) -> int:
-		"""
-		Since: 1.2.6 
-
-		Returns:
-			the 'y' value of the block. 
-		"""
-		pass
-
-	@overload
-	def getZ(self) -> int:
-		"""
-		Since: 1.2.6 
-
-		Returns:
-			the 'z' value of the block. 
-		"""
-		pass
-
-	@overload
-	def up(self) -> "BlockPosHelper":
-		"""
-		Since: 1.6.5 
-
-		Returns:
-			the block above. 
-		"""
-		pass
-
-	@overload
-	def up(self, distance: int) -> "BlockPosHelper":
-		"""
-		Since: 1.6.5 
-
-		Args:
-			distance: 
-
-		Returns:
-			the block n-th block above. 
-		"""
-		pass
-
-	@overload
-	def down(self) -> "BlockPosHelper":
+	def getName(self) -> str:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the block below. 
+			the name of this direction. 
 		"""
 		pass
 
 	@overload
-	def down(self, distance: int) -> "BlockPosHelper":
+	def getAxis(self) -> str:
 		"""
-		Since: 1.6.5 
-
-		Args:
-			distance: 
+		Since: 1.8.4 
 
 		Returns:
-			the block n-th block below. 
+			the name of the axis this direction is aligned to. 
 		"""
 		pass
 
 	@overload
-	def north(self) -> "BlockPosHelper":
+	def isVertical(self) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the block to the north. 
+			'true' if this direction is vertical, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def north(self, distance: int) -> "BlockPosHelper":
+	def isHorizontal(self) -> bool:
 		"""
-		Since: 1.6.5 
-
-		Args:
-			distance: 
+		Since: 1.8.4 
 
 		Returns:
-			the n-th block to the north. 
+			'true' if this direction is horizontal, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def south(self) -> "BlockPosHelper":
+	def isTowardsPositive(self) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the block to the south. 
+			'true' if this direction is pointing in a positive direction, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def south(self, distance: int) -> "BlockPosHelper":
+	def getYaw(self) -> float:
 		"""
-		Since: 1.6.5 
-
-		Args:
-			distance: 
+		Since: 1.8.4 
 
 		Returns:
-			the n-th block to the south. 
+			the yaw of this direction. 
 		"""
 		pass
 
 	@overload
-	def east(self) -> "BlockPosHelper":
+	def getPitch(self) -> float:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the block to the east. 
+			the pitch of this direction. 
 		"""
 		pass
 
 	@overload
-	def east(self, distance: int) -> "BlockPosHelper":
+	def getOpposite(self) -> "DirectionHelper":
 		"""
-		Since: 1.6.5 
-
-		Args:
-			distance: 
+		Since: 1.8.4 
 
 		Returns:
-			the n-th block to the east. 
+			the opposite direction. 
 		"""
 		pass
 
 	@overload
-	def west(self) -> "BlockPosHelper":
+	def getLeft(self) -> "DirectionHelper":
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the block to the west. 
+			the direction to the left. 
 		"""
 		pass
 
 	@overload
-	def west(self, distance: int) -> "BlockPosHelper":
+	def getRight(self) -> "DirectionHelper":
 		"""
-		Since: 1.6.5 
-
-		Args:
-			distance: 
+		Since: 1.8.4 
 
 		Returns:
-			the n-th block to the west. 
+			the direction to the right. 
 		"""
 		pass
 
 	@overload
-	def offset(self, direction: str) -> "BlockPosHelper":
+	def getVector(self) -> Pos3D:
 		"""
-		Since: 1.6.5 
-
-		Args:
-			direction: 0-5 in order: [DOWN, UP, NORTH, SOUTH, WEST, EAST]; 
+		Since: 1.8.4 
 
 		Returns:
-			the block offset by the given direction. 
+			the direction as a directional vector. 
 		"""
 		pass
 
 	@overload
-	def offset(self, direction: str, distance: int) -> "BlockPosHelper":
+	def pointsTo(self, yaw: float) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Args:
-			distance: 
-			direction: 0-5 in order: [DOWN, UP, NORTH, SOUTH, WEST, EAST]; 
+			yaw: the yaw to check 
 
 		Returns:
-			the n-th block offset by the given direction. 
+			'true' if the yaw is facing this direction more than any other one, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BlockStateHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BlockStateHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 from typing import overload
 from typing import TypeVar
-from typing import Mapping
-from .BaseHelper import BaseHelper
+from .StateHelper import StateHelper
 from .BlockHelper import BlockHelper
+from .FluidStateHelper import FluidStateHelper
 from .BlockPosHelper import BlockPosHelper
+from .UniversalBlockStateHelper import UniversalBlockStateHelper
 
 BlockState = TypeVar["net.minecraft.block.BlockState"]
 
-class BlockStateHelper(BaseHelper):
+class BlockStateHelper(StateHelper):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
 	def __init__(self, base: BlockState) -> None:
 		pass
 
 	@overload
-	def toMap(self) -> Mapping[str, str]:
+	def getBlock(self) -> BlockHelper:
 		"""
 		Since: 1.6.5 
 
 		Returns:
-			a map of the state properties with its identifier and value. 
+			the block the state belongs to. 
 		"""
 		pass
 
 	@overload
-	def getBlock(self) -> BlockHelper:
+	def getId(self) -> str:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the block the state belongs to. 
+			the block's id. 
+		"""
+		pass
+
+	@overload
+	def getFluidState(self) -> FluidStateHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the fluid state of this block state. 
 		"""
 		pass
 
 	@overload
 	def getHardness(self) -> float:
 		"""
 		Since: 1.6.5 
@@ -143,24 +154,14 @@
 
 		Returns:
 			the piston behaviour of the state. 
 		"""
 		pass
 
 	@overload
-	def blocksLight(self) -> bool:
-		"""
-		Since: 1.6.5 
-
-		Returns:
-			'true' if the state blocks light. 
-		"""
-		pass
-
-	@overload
 	def blocksMovement(self) -> bool:
 		"""
 		Since: 1.6.5 
 
 		Returns:
 			'true' if the state blocks the movement of entities. 
 		"""
@@ -175,66 +176,78 @@
 			'true' if the state is burnable. 
 		"""
 		pass
 
 	@overload
 	def isLiquid(self) -> bool:
 		"""
-		Since: 1.6.5* @since 1.6.5 
+		Since: 1.6.5 
 
 		Returns:
 			'true' if the state is a liquid. 
 		"""
 		pass
 
 	@overload
 	def isSolid(self) -> bool:
 		"""
-		Since: 1.6.5* @since 1.6.5 
+		Since: 1.6.5 
 
 		Returns:
 			'true' if the state is solid. 
 		"""
 		pass
 
 	@overload
 	def isReplaceable(self) -> bool:
-		"""This will return true for blocks like air and grass, that can be replaced
-without breaking them first.\n
+		"""This will return true for blocks like air and grass, that can be replaced without breaking
+them first.\n
 		Since: 1.6.5 
 
 		Returns:
 			'true' if the state can be replaced. 
 		"""
 		pass
 
 	@overload
 	def allowsSpawning(self, pos: BlockPosHelper, entity: str) -> bool:
 		"""
 		Since: 1.6.5 
 
 		Args:
-			pos: 
-			entity: 
+			pos: the position of the block to check 
+			entity: the entity type to check 
 
 		Returns:
-			'true' if the entity can spawn on this block state at the given position in the current world. 
+			'true' if the entity can spawn on this block state at the given position in the
+current world. 
 		"""
 		pass
 
 	@overload
 	def shouldSuffocate(self, pos: BlockPosHelper) -> bool:
 		"""
 		Since: 1.6.5 
 
 		Args:
-			pos: 
+			pos: the position of the block to check 
+
+		Returns:
+			'true' if an entity can suffocate in this block state at the given position in
+the current world. 
+		"""
+		pass
+
+	@overload
+	def getUniversal(self) -> UniversalBlockStateHelper:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			'true' if an entity can suffocate in this block state at the given position in the current world. 
+			an UniversalBlockStateHelper to access all properties of this block state. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BooleanField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileField.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+File = TypeVar["java.io.File"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class BooleanField(AbstractSettingField):
+class FileField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
+	def getTopLevel(self, setting: SettingsOverlay_SettingField) -> File:
+		pass
+
+	@overload
+	def relativize(self, setting: SettingsOverlay_SettingField, file: File) -> str:
+		pass
+
+	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BossBarConsumer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BossBarConsumer.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/BossBarHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ModContainerHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,87 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
+from typing import Generic
 from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
 
-BossBar = TypeVar["net.minecraft.entity.boss.BossBar"]
+T = TypeVar("T")
 
-class BossBarHelper(BaseHelper):
+class ModContainerHelper(Generic[T], BaseHelper):
 	"""
-	Since: 1.2.1 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, b: BossBar) -> None:
+	def getId(self) -> str:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the mod's id. 
+		"""
+		pass
+
+	@overload
+	def getName(self) -> str:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the mod's name. 
+		"""
 		pass
 
 	@overload
-	def getUUID(self) -> str:
+	def getDescription(self) -> str:
 		"""
-		Since: 1.2.1 
+		Since: 1.8.4 
 
 		Returns:
-			boss bar uuid. 
+			the mod's description. 
 		"""
 		pass
 
 	@overload
-	def getPercent(self) -> float:
+	def getVersion(self) -> str:
 		"""
-		Since: 1.2.1 
+		Since: 1.8.4 
 
 		Returns:
-			percent of boss bar remaining. 
+			the mod's version. 
 		"""
 		pass
 
 	@overload
-	def getColor(self) -> str:
+	def getEnv(self) -> str:
 		"""
-		Since: 1.2.1 
+		Since: 1.8.4 
 
 		Returns:
-			boss bar color. 
+			the environment this mod is intended for. 
 		"""
 		pass
 
 	@overload
-	def getStyle(self) -> str:
+	def getAuthors(self) -> List[str]:
 		"""
-		Since: 1.2.1 
+		Since: 1.8.4 
 
 		Returns:
-			boss bar notch style. 
+			a list of all authors. 
 		"""
 		pass
 
 	@overload
-	def getName(self) -> TextHelper:
+	def getDependencies(self) -> List[str]:
 		"""
-		Since: 1.2.1 
+		Since: 1.8.4 
 
 		Returns:
-			name of boss bar 
+			a list of all dependencies. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Button.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Button.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from typing import overload
 from typing import TypeVar
 
-NarrationMessageBuilder = TypeVar["net.minecraft.client.gui.screen.narration.NarrationMessageBuilder"]
 Consumer = TypeVar["java.util.function.Consumer_xyz.wagyourtail.wagyourgui.elements.Button_"]
 PressableWidget = TypeVar["net.minecraft.client.gui.widget.PressableWidget"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 Text = TypeVar["net.minecraft.text.Text"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
 class Button(PressableWidget):
 	horizCenter: bool
 	onPress: Consumer
 	hovering: bool
 	forceHover: bool
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, hilightColor: int, textColor: int, message: Text, onPress: Consumer) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: Text, onPress: Consumer) -> None:
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> "Button":
 		pass
 
 	@overload
@@ -31,33 +30,29 @@
 		pass
 
 	@overload
 	def setColor(self, color: int) -> None:
 		pass
 
 	@overload
-	def setHilightColor(self, color: int) -> None:
+	def setHighlightColor(self, color: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def onClick(self, mouseX: float, mouseY: float) -> None:
 		pass
 
 	@overload
 	def onRelease(self, mouseX: float, mouseY: float) -> None:
 		pass
 
 	@overload
 	def onPress(self) -> None:
 		pass
 
-	@overload
-	def appendNarrations(self, builder: NarrationMessageBuilder) -> None:
-		pass
-
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ButtonWidgetHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextFieldWidgetHelper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,150 +1,204 @@
 from typing import overload
 from typing import TypeVar
-from typing import Generic
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
+from .ClickableWidgetHelper import ClickableWidgetHelper
+from .MethodWrapper import MethodWrapper
 
-T = TypeVar("T")
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+TextFieldWidget = TypeVar["net.minecraft.client.gui.widget.TextFieldWidget"]
 
-class ButtonWidgetHelper(RenderCommon_RenderElement, Generic[T], BaseHelper):
+class TextFieldWidgetHelper(ClickableWidgetHelper):
 	"""
 	Since: 1.0.5 
 	"""
-	zIndex: int
 
 	@overload
-	def __init__(self, btn: T) -> None:
+	def __init__(self, t: TextFieldWidget) -> None:
 		pass
 
 	@overload
-	def __init__(self, btn: T, zIndex: int) -> None:
+	def __init__(self, t: TextFieldWidget, zIndex: int) -> None:
 		pass
 
 	@overload
-	def getX(self) -> int:
+	def getText(self) -> str:
 		"""
 		Since: 1.0.5 
 
 		Returns:
-			the 'x' coordinate of the button. 
+			the currently entered String . 
 		"""
 		pass
 
 	@overload
-	def getY(self) -> int:
+	def setText(self, text: str) -> "TextFieldWidgetHelper":
 		"""
 		Since: 1.0.5 
 
-		Returns:
-			the 'y' coordinate of the button. 
+		Args:
+			text: 
 		"""
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int) -> "ButtonWidgetHelper":
-		"""Set the button position.\n
-		Since: 1.0.5 
+	def setText(self, text: str, await_: bool) -> "TextFieldWidgetHelper":
+		"""set the currently entered String .\n
+		Since: 1.3.1 
 
 		Args:
-			x: 
-			y: 
+			await: 
+			text: 
 		"""
 		pass
 
 	@overload
-	def getWidth(self) -> int:
+	def setEditableColor(self, color: int) -> "TextFieldWidgetHelper":
 		"""
 		Since: 1.0.5 
+
+		Args:
+			color: 
 		"""
 		pass
 
 	@overload
-	def setLabel(self, label: str) -> "ButtonWidgetHelper":
-		"""change the text.\n
-		Since: 1.0.5, renamed from 'setText' in 1.3.1 
+	def setEditable(self, edit: bool) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.0.5 
 
 		Args:
-			label: 
+			edit: 
 		"""
 		pass
 
 	@overload
-	def setLabel(self, helper: TextHelper) -> "ButtonWidgetHelper":
-		"""change the text.\n
-		Since: 1.3.1 
+	def isEditable(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the text field is editable, 'false' otherwise. 
+		"""
+		pass
+
+	@overload
+	def setUneditableColor(self, color: int) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.0.5 
 
 		Args:
-			helper: 
+			color: 
 		"""
 		pass
 
 	@overload
-	def getLabel(self) -> TextHelper:
+	def getSelectedText(self) -> str:
 		"""
-		Since: 1.2.3, renamed fro 'getText' in 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			current button text. 
+			the selected text. 
 		"""
 		pass
 
 	@overload
-	def getActive(self) -> bool:
+	def setSuggestion(self, suggestion: str) -> "TextFieldWidgetHelper":
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
+
+		Args:
+			suggestion: the suggestion to set 
 
 		Returns:
-			button clickable state. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setActive(self, t: bool) -> "ButtonWidgetHelper":
-		"""set the button clickable state.\n
-		Since: 1.0.5 
+	def getMaxLength(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the maximum length of this text field. 
+		"""
+		pass
+
+	@overload
+	def setMaxLength(self, length: int) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			t: 
+			length: the new maximum length 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setWidth(self, width: int) -> "ButtonWidgetHelper":
-		"""set the button width.\n
-		Since: 1.0.5 
+	def setSelection(self, start: int, end: int) -> "TextFieldWidgetHelper":
+		pass
+
+	@overload
+	def setTextPredicate(self, predicate: MethodWrapper) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			width: 
+			predicate: the text filter 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def click(self) -> "ButtonWidgetHelper":
-		"""clicks button\n
-		Since: 1.3.1 
+	def resetTextPredicate(self) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def click(self, await_: bool) -> "ButtonWidgetHelper":
-		"""clicks button\n
-		Since: 1.3.1 
+	def setCursorPosition(self, position: int) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			await: should wait for button to finish clicking. 
+			position: the cursor position 
+
+		Returns:
+			self for chaining. 
+		"""
+		pass
+
+	@overload
+	def setCursorToStart(self) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def setCursorToEnd(self) -> "TextFieldWidgetHelper":
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			self for chaining. 
+		"""
 		pass
 
 	@overload
-	def getZIndex(self) -> int:
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CancelScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CancelScreen.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 		pass
 
 	@overload
 	def mouseScrolled(self, mouseX: float, mouseY: float, amount: float) -> bool:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def removed(self) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CategoryTreeContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CategoryTreeContainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 		pass
 
 	@overload
 	def onScrollbar(self, page: float) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ChatHistoryManager.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ChatHistoryManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,34 @@
 
 		Args:
 			index: 
 		"""
 		pass
 
 	@overload
+	def getRecvCount(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the amount of messages in the chat history. 
+		"""
+		pass
+
+	@overload
+	def getRecvLines(self) -> List[ChatHudLineHelper]:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			all received messages in the chat history. 
+		"""
+		pass
+
+	@overload
 	def insertRecvText(self, index: int, line: TextHelper) -> None:
 		"""
 		Since: 1.6.0 
 
 		Args:
 			line: 
 			index:
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ChatHudLineHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ChatHudLineHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,13 +17,17 @@
 		pass
 
 	@overload
 	def getCreationTick(self) -> int:
 		pass
 
 	@overload
-	def deleteById(self) -> None:
+	def deleteById(self) -> "ChatHudLineHelper":
+		pass
+
+	@overload
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CheckBoxContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CheckBoxContainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_AnnotationBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_AnnotationBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_BodyBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_BodyBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_ConstructorBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_ConstructorBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_FieldBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_FieldBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClassBuilder_MethodBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClassBuilder_MethodBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClientConfigV2.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClientConfigV2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .Sorting_MacroSortMethod import Sorting_MacroSortMethod
+from .Sorting_ServiceSortMethod import Sorting_ServiceSortMethod
 
 JsonObject = TypeVar["com.google.gson.JsonObject"]
-Comparator = TypeVar["java.util.Comparator_xyz.wagyourtail.jsmacros.core.config.ScriptTrigger_"]
+Comparator = TypeVar["java.util.Comparator_java.lang.String_"]
 
 class ClientConfigV2:
 	sortMethod: Sorting_MacroSortMethod
+	sortServicesMethod: Sorting_ServiceSortMethod
+	showSlotIndexes: bool
 	disableKeyWhenScreenOpen: bool
 	editorTheme: Mapping[str, List[float]]
 	editorLinterOverrides: Mapping[str, str]
 	editorHistorySize: int
 	editorSuggestions: bool
 	editorFont: str
 	externalEditor: bool
 	externalEditorCommand: str
+	showRunningServices: bool
+	serviceAutoReload: bool
 
 	@overload
 	def __init__(self) -> None:
 		pass
 
 	@overload
 	def languages(self) -> List[str]:
@@ -31,17 +36,25 @@
 		pass
 
 	@overload
 	def getThemeData(self) -> Mapping[str, List[float]]:
 		pass
 
 	@overload
+	def setServiceAutoReload(self, value: bool) -> None:
+		pass
+
+	@overload
 	def getSortComparator(self) -> Comparator:
 		pass
 
 	@overload
+	def getServiceSortComparator(self) -> Comparator:
+		pass
+
+	@overload
 	def fromV1(self, v1: JsonObject) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ClientPlayerEntityHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ClickableWidgetHelper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,253 +1,259 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from typing import Mapping
 from typing import Generic
-from .PlayerEntityHelper import PlayerEntityHelper
-from .EntityHelper import EntityHelper
+from .RenderElement import RenderElement
+from .Alignable import Alignable
+from .BaseHelper import BaseHelper
+from .TextHelper import TextHelper
 
+B = TypeVar("B")
 T = TypeVar("T")
+MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+Text = TypeVar["net.minecraft.text.Text"]
 
-class ClientPlayerEntityHelper(Generic[T], PlayerEntityHelper):
+class ClickableWidgetHelper(RenderElement, Alignable, Generic[B, T], BaseHelper):
 	"""
-	Since: 1.0.3 
+	Since: 1.0.5 
 	"""
+	zIndex: int
+	tooltips: List[Text]
 
 	@overload
-	def __init__(self, e: T) -> None:
+	def __init__(self, btn: T) -> None:
 		pass
 
 	@overload
-	def lookAt(self, yaw: float, pitch: float) -> "ClientPlayerEntityHelper":
+	def __init__(self, btn: T, zIndex: int) -> None:
+		pass
+
+	@overload
+	def getX(self) -> int:
 		"""
-		Since: 1.0.3 
+		Since: 1.0.5 
 
-		Args:
-			pitch: (was yaw prior to 1.2.6) 
-			yaw: (was pitch prior to 1.2.6) 
+		Returns:
+			the 'x' coordinate of the button. 
 		"""
 		pass
 
 	@overload
-	def lookAt(self, x: float, y: float, z: float) -> "ClientPlayerEntityHelper":
-		"""look at the specified coordinates.\n
-		Since: 1.2.8 
+	def getY(self) -> int:
+		"""
+		Since: 1.0.5 
 
-		Args:
-			x: 
-			y: 
-			z: 
+		Returns:
+			the 'y' coordinate of the button. 
 		"""
 		pass
 
 	@overload
-	def attack(self, entity: EntityHelper) -> "ClientPlayerEntityHelper":
-		"""
-		Since: 1.5.0 
+	def setPos(self, x: int, y: int) -> B:
+		"""Set the button position.\n
+		Since: 1.0.5 
 
 		Args:
-			entity: 
+			x: 
+			y: 
 		"""
 		pass
 
 	@overload
-	def attack(self, entity: EntityHelper, await_: bool) -> "ClientPlayerEntityHelper":
+	def getWidth(self) -> int:
 		"""
-		Since: 1.6.0 
-
-		Args:
-			await: 
-			entity: 
+		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def attack(self, x: int, y: int, z: int, direction: int) -> "ClientPlayerEntityHelper":
+	def getHeight(self) -> int:
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
 
-		Args:
-			x: 
-			y: 
-			z: 
-			direction: 0-5 in order: [DOWN, UP, NORTH, SOUTH, WEST, EAST]; 
+		Returns:
+			the height of the button. 
 		"""
 		pass
 
 	@overload
-	def attack(self, x: int, y: int, z: int, direction: int, await_: bool) -> "ClientPlayerEntityHelper":
-		"""
-		Since: 1.6.0 
+	def setLabel(self, label: str) -> B:
+		"""change the text.\n
+		Since: 1.0.5, renamed from 'setText' in 1.3.1 
 
 		Args:
-			x: 
-			await: 
-			y: 
-			z: 
-			direction: 0-5 in order: [DOWN, UP, NORTH, SOUTH, WEST, EAST]; 
+			label: 
 		"""
 		pass
 
 	@overload
-	def interactEntity(self, entity: EntityHelper, offHand: bool) -> "ClientPlayerEntityHelper":
-		"""
-		Since: 1.5.0, renamed from 'interact' in 1.6.0 
+	def setLabel(self, helper: TextHelper) -> B:
+		"""change the text.\n
+		Since: 1.3.1 
 
 		Args:
-			entity: 
-			offHand: 
+			helper: 
 		"""
 		pass
 
 	@overload
-	def interactEntity(self, entity: EntityHelper, offHand: bool, await_: bool) -> "ClientPlayerEntityHelper":
+	def getLabel(self) -> TextHelper:
 		"""
-		Since: 1.6.0 
+		Since: 1.2.3, renamed fro 'getText' in 1.3.1 
 
-		Args:
-			await: 
-			entity: 
-			offHand: 
+		Returns:
+			current button text. 
 		"""
 		pass
 
 	@overload
-	def interactItem(self, offHand: bool) -> "ClientPlayerEntityHelper":
+	def getActive(self) -> bool:
 		"""
-		Since: 1.5.0, renamed from 'interact' in 1.6.0 
+		Since: 1.0.5 
 
-		Args:
-			offHand: 
+		Returns:
+			button clickable state. 
 		"""
 		pass
 
 	@overload
-	def interactItem(self, offHand: bool, await_: bool) -> "ClientPlayerEntityHelper":
-		"""
-		Since: 1.6.0 
+	def setActive(self, t: bool) -> B:
+		"""set the button clickable state.\n
+		Since: 1.0.5 
 
 		Args:
-			await: 
-			offHand: 
+			t: 
 		"""
 		pass
 
 	@overload
-	def interactBlock(self, x: int, y: int, z: int, direction: int, offHand: bool) -> "ClientPlayerEntityHelper":
-		"""
-		Since: 1.5.0, renamed from 'interact' in 1.6.0 
+	def setWidth(self, width: int) -> B:
+		"""set the button width.\n
+		Since: 1.0.5 
 
 		Args:
-			x: 
-			y: 
-			z: 
-			direction: 0-5 in order: [DOWN, UP, NORTH, SOUTH, WEST, EAST]; 
-			offHand: 
+			width: 
 		"""
 		pass
 
 	@overload
-	def interactBlock(self, x: int, y: int, z: int, direction: int, offHand: bool, await_: bool) -> "ClientPlayerEntityHelper":
+	def click(self) -> B:
+		"""clicks button\n
+		Since: 1.3.1 
+		"""
 		pass
 
 	@overload
-	def interact(self) -> "ClientPlayerEntityHelper":
-		"""
-		Since: 1.5.0 
+	def click(self, await_: bool) -> B:
+		"""clicks button\n
+		Since: 1.3.1 
+
+		Args:
+			await: should wait for button to finish clicking. 
 		"""
 		pass
 
 	@overload
-	def interact(self, await_: bool) -> "ClientPlayerEntityHelper":
+	def setTooltip(self, tooltips: List[object]) -> B:
 		"""
-		Since: 1.6.0 
+		Since: 1.8.4 
 
 		Args:
-			await: 
+			tooltips: the tooltips to set 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def attack(self) -> "ClientPlayerEntityHelper":
+	def addTooltip(self, tooltip: object) -> B:
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
+
+		Args:
+			tooltip: the tooltips to add 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def attack(self, await_: bool) -> "ClientPlayerEntityHelper":
+	def removeTooltip(self, index: int) -> bool:
 		"""
-		Since: 1.6.0 
+		Since: 1.8.4 
 
 		Args:
-			await: 
+			index: the index of the tooltip to remove 
+
+		Returns:
+			'true' if the tooltip was removed successfully, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def setLongAttack(self, stop: bool) -> "ClientPlayerEntityHelper":
+	def removeTooltip(self, tooltip: TextHelper) -> bool:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
 		Args:
-			stop: 
+			tooltip: the tooltip to remove 
+
+		Returns:
+			'true' if the tooltip was removed successfully, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def setLongInteract(self, stop: bool) -> "ClientPlayerEntityHelper":
+	def getTooltips(self) -> List[TextHelper]:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
-		Args:
-			stop: 
+		Returns:
+			a copy of the tooltips. 
 		"""
 		pass
 
 	@overload
-	def getItemCooldownsRemainingTicks(self) -> Mapping[str, int]:
-		"""
-		Since: 1.6.5 
-		"""
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
-	def getItemCooldownRemainingTicks(self, item: str) -> int:
-		"""
-		Since: 1.6.5 
+	def getZIndex(self) -> int:
+		pass
 
-		Args:
-			item: 
-		"""
+	@overload
+	def toString(self) -> str:
 		pass
 
 	@overload
-	def getTicksSinceCooldownsStart(self) -> Mapping[str, int]:
-		"""
-		Since: 1.6.5 
-		"""
+	def getScaledWidth(self) -> int:
 		pass
 
 	@overload
-	def getTicksSinceCooldownStart(self, item: str) -> int:
-		"""
-		Since: 1.6.5 
+	def getParentWidth(self) -> int:
+		pass
 
-		Args:
-			item: 
-		"""
+	@overload
+	def getScaledHeight(self) -> int:
 		pass
 
 	@overload
-	def getFoodLevel(self) -> int:
-		"""
-		Since: 1.1.2 
-		"""
+	def getParentHeight(self) -> int:
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def getScaledLeft(self) -> int:
+		pass
+
+	@overload
+	def getScaledTop(self) -> int:
+		pass
+
+	@overload
+	def moveTo(self, x: int, y: int) -> B:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CodeCompileEvent.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CodeCompileEvent.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 	@overload
 	def genPrismNodes(self) -> List[Prism4j_Node]:
 		"""
 
 		Returns:
 			Prism4j's
-    node list you don't have to use it but if you're not compiling your own...
-    peek at the code of TextStyleCompiler for the default impl for walking the node tree. 
+node list you don't have to use it but if you're not compiling your own...
+peek at the code of TextStyleCompiler for the default impl for walking the node tree. 
 		"""
 		pass
 
 	@overload
 	def createMap(self) -> Mapping[Any, Any]:
 		"""Easy access to the Map object for use with CodeCompileEvent#rightClickActions
 
@@ -79,30 +79,29 @@
 		pass
 
 	@overload
 	def createPrefixTree(self) -> StringHashTrie:
 		"""prefix tree data structure written for you, it's a bit intensive to add things to, especially how I wrote it, but
 lookup times are much better at least on larger data sets,
 so create a single copy of this for your static autocompletes and don't be re-creating this every time, store it
-in 'globalvars' , probably per language
-
+in 'globalvars' , probably per language 
 or just don't use it, I'm not forcing you to.
 
 		Returns:
 			a new StringHashTrie 
 		"""
 		pass
 
 	@overload
 	def getThemeData(self) -> Mapping[str, List[float]]:
 		"""
 
 		Returns:
 			'key -> hex integer' values for theme data points, this can be used with the prism data for
-    coloring, just have to use TextBuilder#withColor(int,int,int) on 1.15 and older versions the integer values with be the default color's index so you can directly pass it
-    to TextBuilder#withColor(int) 
+coloring, just have to use TextBuilder#withColor(int,int,int) on 1.15 and older versions the integer values with be the default color's index so you can directly pass it
+to TextBuilder#withColor(int) 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ColorMapSetting.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ColorMapSetting.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ColorMapSetting_ColorEntry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ColorMapSetting_ColorEntry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandContextHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandContextHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CommandManager.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CommandManager.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ConfigManager.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ConfirmOverlay.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ConfirmOverlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Core.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Core.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Set
 from typing import Generic
 from .LibraryRegistry import LibraryRegistry
 from .BaseEventRegistry import BaseEventRegistry
 from .ExtensionLoader import ExtensionLoader
 from .ConfigManager import ConfigManager
 from .ServiceManager import ServiceManager
+from .JsMacrosThreadPool import JsMacrosThreadPool
 from .EventContainer import EventContainer
 from .BaseScriptContext import BaseScriptContext
 from .ScriptTrigger import ScriptTrigger
 from .BaseEvent import BaseEvent
 from .BaseWrappedException import BaseWrappedException
 
 Function = TypeVar["java.util.function.Function_xyz.wagyourtail.jsmacros.core.Core_V,R_,R_"]
@@ -26,14 +27,15 @@
 class Core(Generic[T, U]):
 	libraryRegistry: LibraryRegistry
 	eventRegistry: BaseEventRegistry
 	extensions: ExtensionLoader
 	profile: T
 	config: ConfigManager
 	services: ServiceManager
+	threadPool: JsMacrosThreadPool
 
 	@overload
 	def getInstance(self) -> "Core":
 		"""static reference to instance created by Core#<V,R>createInstance(java.util.function.Function<xyz.wagyourtail.jsmacros.core.Core<V,R>,R>,java.util.function.BiFunction<xyz.wagyourtail.jsmacros.core.Core<V,R>,org.slf4j.Logger,V>,java.io.File,java.io.File,org.slf4j.Logger)
 		"""
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/CoreConfigV2.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CoreConfigV2.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/DefaultCodeCompiler.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptCodeCompiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 from typing import TypeVar
 from typing import Mapping
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
 Runnable = TypeVar["java.lang.Runnable"]
+Text = TypeVar["net.minecraft.text.Text"]
+File = TypeVar["java.io.File"]
 
-class DefaultCodeCompiler(AbstractRenderCodeCompiler):
+class ScriptCodeCompiler(AbstractRenderCodeCompiler):
+	"""
+	"""
 
 	@overload
-	def __init__(self, language: str, screen: EditorScreen) -> None:
+	def __init__(self, language: str, screen: EditorScreen, scriptFile: File) -> None:
 		pass
 
 	@overload
 	def recompileRenderedText(self, text: str) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/DoubleField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/DoubleField.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw2D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw2D.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .IDraw2D import IDraw2D
 from .MethodWrapper import MethodWrapper
-from .RenderCommon_Text import RenderCommon_Text
-from .RenderCommon_Rect import RenderCommon_Rect
-from .RenderCommon_Item import RenderCommon_Item
-from .RenderCommon_Image import RenderCommon_Image
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
+from .Text import Text
+from .Rect import Rect
+from .Line import Line
+from .Item import Item
+from .Image import Image
+from .Draw2DElement import Draw2DElement
+from .RenderElement import RenderElement
 from .TextHelper import TextHelper
 from .ItemStackHelper import ItemStackHelper
 
-DrawableHelper = TypeVar["net.minecraft.client.gui.DrawableHelper"]
+T = TypeVar("T")
+IntSupplier = TypeVar["java.util.function.IntSupplier"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 
-class Draw2D(IDraw2D, DrawableHelper):
+class Draw2D(IDraw2D):
 	"""
 	Since: 1.0.5 
 	"""
+	widthSupplier: IntSupplier
+	heightSupplier: IntSupplier
+	zIndex: int
+	visible: bool
 	onInit: MethodWrapper
 	catchInit: MethodWrapper
 
 	@overload
 	def __init__(self) -> None:
 		pass
 
@@ -36,255 +43,330 @@
 	def getHeight(self) -> int:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def getTexts(self) -> List[RenderCommon_Text]:
+	def getTexts(self) -> List[Text]:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def getRects(self) -> List[RenderCommon_Rect]:
+	def getRects(self) -> List[Rect]:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def getItems(self) -> List[RenderCommon_Item]:
+	def getLines(self) -> List[Line]:
+		pass
+
+	@overload
+	def getItems(self) -> List[Item]:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def getImages(self) -> List[RenderCommon_Image]:
+	def getImages(self) -> List[Image]:
 		"""
 		Since: 1.2.3 
 		"""
 		pass
 
 	@overload
-	def getElements(self) -> List[RenderCommon_RenderElement]:
+	def getDraw2Ds(self) -> List[Draw2DElement]:
+		pass
+
+	@overload
+	def getElements(self) -> List[RenderElement]:
+		pass
+
+	@overload
+	def removeElement(self, e: RenderElement) -> "Draw2D":
+		pass
+
+	@overload
+	def reAddElement(self, e: T) -> T:
+		pass
+
+	@overload
+	def setVisible(self, visible: bool) -> "Draw2D":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			visible: whether to render this element. 
+
+		Returns:
+			self for chaining. 
+		"""
+		pass
+
+	@overload
+	def isVisible(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this draw2d is visible, 'false' otherwise. 
+		"""
+		pass
+
+	@overload
+	def addDraw2D(self, draw2D: "Draw2D", x: int, y: int, width: int, height: int) -> Draw2DElement:
 		pass
 
 	@overload
-	def removeElement(self, e: RenderCommon_RenderElement) -> "Draw2D":
+	def addDraw2D(self, draw2D: "Draw2D", x: int, y: int, width: int, height: int, zIndex: int) -> Draw2DElement:
 		pass
 
 	@overload
-	def reAddElement(self, e: RenderCommon_RenderElement) -> RenderCommon_RenderElement:
+	def removeDraw2D(self, draw2D: Draw2DElement) -> "Draw2D":
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, shadow: bool) -> Text:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool) -> Text:
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> Text:
 		"""
 		Since: 1.2.6 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> Text:
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool) -> Text:
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool) -> Text:
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> Text:
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> Text:
 		pass
 
 	@overload
-	def removeText(self, t: RenderCommon_Text) -> "Draw2D":
+	def removeText(self, t: Text) -> "Draw2D":
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> Image:
 		"""
 		Since: 1.2.3 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> Image:
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.2.6 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.4.0 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, alpha: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, alpha: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
-	def removeImage(self, i: RenderCommon_Image) -> "Draw2D":
+	def removeImage(self, i: Image) -> "Draw2D":
 		"""
 		Since: 1.2.3 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int) -> Rect:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int) -> Rect:
 		"""
 		Since: 1.1.8 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float) -> Rect:
 		"""
 		Since: 1.2.6 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float, zIndex: int) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float, zIndex: int) -> Rect:
 		pass
 
 	@overload
-	def removeRect(self, r: RenderCommon_Rect) -> "Draw2D":
+	def removeRect(self, r: Rect) -> "Draw2D":
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str) -> RenderCommon_Item:
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int) -> Line:
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, zIndex: int) -> Line:
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, width: float) -> Line:
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, zIndex: int, width: float) -> Line:
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, width: float, rotation: float) -> Line:
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, zIndex: int, width: float, rotation: float) -> Line:
+		pass
+
+	@overload
+	def removeLine(self, l: Line) -> "Draw2D":
+		pass
+
+	@overload
+	def addItem(self, x: int, y: int, id: str) -> Item:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, id: str) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, id: str) -> Item:
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, id: str, overlay: bool) -> Item:
 		"""
 		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool) -> Item:
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, id: str, overlay: bool, scale: float, rotation: float) -> Item:
 		"""
 		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool, scale: float, rotation: float) -> Item:
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, Item: ItemStackHelper) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, Item: ItemStackHelper) -> Item:
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper) -> Item:
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, Item: ItemStackHelper, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, Item: ItemStackHelper, overlay: bool) -> Item:
 		"""
 		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool) -> Item:
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> Item:
 		"""
 		Since: 1.2.6 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> Item:
 		pass
 
 	@overload
-	def removeItem(self, i: RenderCommon_Item) -> "Draw2D":
+	def removeItem(self, i: Item) -> "Draw2D":
 		"""
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def render(self, matrixStack: MatrixStack) -> None:
+	def render(self, drawContext: MatrixStack) -> None:
+		pass
+
+	@overload
+	def getElementsByZIndex(self) -> iter:
 		pass
 
 	@overload
 	def setOnInit(self, onInit: MethodWrapper) -> "Draw2D":
 		"""init function, called when window is resized or screen/draw2d is registered.
 clears all previous elements when called.\n
 		Since: 1.2.7 
@@ -320,10 +402,18 @@
 		Since: 1.6.5 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
+	@overload
+	def setZIndex(self, zIndex: int) -> None:
+		pass
+
+	@overload
+	def getZIndex(self) -> int:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw3D.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,101 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from .Draw3D_Box import Draw3D_Box
-from .Draw3D_Line import Draw3D_Line
-from .Draw3D_Surface import Draw3D_Surface
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
+from .Box import Box
+from .Line3D import Line3D
+from .Surface import Surface
+from .RenderElement3D import RenderElement3D
+from .Pos3D import Pos3D
+from .Box_Builder import Box_Builder
+from .BlockPosHelper import BlockPosHelper
+from .Line3D_Builder import Line3D_Builder
+from .Surface_Builder import Surface_Builder
 
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 
 class Draw3D:
 	"""Draw2D is cool\n
 	Since: 1.0.6 
 	"""
 
 	@overload
 	def __init__(self) -> None:
 		pass
 
 	@overload
-	def getBoxes(self) -> List[Draw3D_Box]:
+	def getBoxes(self) -> List[Box]:
 		"""
 		Since: 1.0.6 
 		"""
 		pass
 
 	@overload
-	def getLines(self) -> List[Draw3D_Line]:
+	def getLines(self) -> List[Line3D]:
 		"""
 		Since: 1.0.6 
 		"""
 		pass
 
 	@overload
-	def getDraw2Ds(self) -> List[Draw3D_Surface]:
+	def getDraw2Ds(self) -> List[Surface]:
 		"""
 		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
-	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, fillColor: int, fill: bool) -> Draw3D_Box:
+	def clear(self) -> None:
+		"""
+		Since: 1.8.4 
+		"""
+		pass
+
+	@overload
+	def reAddElement(self, element: RenderElement3D) -> None:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			element: 
+		"""
+		pass
+
+	@overload
+	def addBox(self, box: Box) -> None:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			box: 
+		"""
+		pass
+
+	@overload
+	def addLine(self, line: Line3D) -> None:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			line: 
+		"""
+		pass
+
+	@overload
+	def addSurface(self, surface: Surface) -> None:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			surface: 
+		"""
+		pass
+
+	@overload
+	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, fillColor: int, fill: bool) -> Box:
 		"""
 		Since: 1.0.6 
 
 		Args:
 			fillColor: 
 			color: 
 			z1: 
@@ -51,20 +103,20 @@
 			z2: 
 			x1: 
 			y2: 
 			x2: 
 			fill: 
 
 		Returns:
-			The Draw3D_Box you added. 
+			The Box you added. 
 		"""
 		pass
 
 	@overload
-	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, fillColor: int, fill: bool, cull: bool) -> Draw3D_Box:
+	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, fillColor: int, fill: bool, cull: bool) -> Box:
 		"""
 		Since: 1.3.1 
 
 		Args:
 			fillColor: 
 			color: 
 			z1: 
@@ -75,15 +127,15 @@
 			x2: 
 			fill: 
 			cull: 
 		"""
 		pass
 
 	@overload
-	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, fillColor: int, fillAlpha: int, fill: bool) -> Draw3D_Box:
+	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, fillColor: int, fillAlpha: int, fill: bool) -> Box:
 		"""
 		Since: 1.1.8 
 
 		Args:
 			fillColor: 
 			color: 
 			z1: 
@@ -93,53 +145,53 @@
 			x1: 
 			y2: 
 			fillAlpha: 
 			x2: 
 			fill: 
 
 		Returns:
-			the Draw3D_Box you added. 
+			the Box you added. 
 		"""
 		pass
 
 	@overload
-	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, fillColor: int, fillAlpha: int, fill: bool, cull: bool) -> Draw3D_Box:
+	def addBox(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, fillColor: int, fillAlpha: int, fill: bool, cull: bool) -> Box:
 		pass
 
 	@overload
-	def removeBox(self, b: Draw3D_Box) -> "Draw3D":
+	def removeBox(self, b: Box) -> "Draw3D":
 		"""
 		Since: 1.0.6 
 
 		Args:
 			b: 
 		"""
 		pass
 
 	@overload
-	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int) -> Draw3D_Line:
+	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int) -> Line3D:
 		"""
 		Since: 1.0.6 
 
 		Args:
 			color: 
 			z1: 
 			y1: 
 			z2: 
 			x1: 
 			y2: 
 			x2: 
 
 		Returns:
-			the Draw3D_Line you added. 
+			the Line3D you added. 
 		"""
 		pass
 
 	@overload
-	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, cull: bool) -> Draw3D_Line:
+	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, cull: bool) -> Line3D:
 		"""
 		Since: 1.3.1 
 
 		Args:
 			color: 
 			z1: 
 			y1: 
@@ -148,35 +200,35 @@
 			y2: 
 			x2: 
 			cull: 
 		"""
 		pass
 
 	@overload
-	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int) -> Draw3D_Line:
+	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int) -> Line3D:
 		"""
 		Since: 1.1.8 
 
 		Args:
 			color: 
 			z1: 
 			alpha: 
 			y1: 
 			z2: 
 			x1: 
 			y2: 
 			x2: 
 
 		Returns:
-			the Draw3D_Line you added. 
+			the Line3D you added. 
 		"""
 		pass
 
 	@overload
-	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, cull: bool) -> Draw3D_Line:
+	def addLine(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, cull: bool) -> Line3D:
 		"""
 		Since: 1.3.1 
 
 		Args:
 			color: 
 			z1: 
 			alpha: 
@@ -186,117 +238,117 @@
 			y2: 
 			x2: 
 			cull: 
 		"""
 		pass
 
 	@overload
-	def removeLine(self, l: Draw3D_Line) -> "Draw3D":
+	def removeLine(self, l: Line3D) -> "Draw3D":
 		"""
 		Since: 1.0.6 
 
 		Args:
 			l: 
 		"""
 		pass
 
 	@overload
-	def addPoint(self, point: PositionCommon_Pos3D, radius: float, color: int) -> Draw3D_Box:
-		"""Draws a cube( Draw3D_Box ) with a specific radius( 'side length = 2*radius' )\n
+	def addPoint(self, point: Pos3D, radius: float, color: int) -> Box:
+		"""Draws a cube( Box ) with a specific radius( 'side length = 2*radius' )\n
 		Since: 1.4.0 
 
 		Args:
 			color: point color 
 			radius: 1/2 of the side length of the cube 
 			point: the center point 
 
 		Returns:
-			the Draw3D_Box generated, and visualized 
+			the Box generated, and visualized 
 		"""
 		pass
 
 	@overload
-	def addPoint(self, x: float, y: float, z: float, radius: float, color: int) -> Draw3D_Box:
-		"""Draws a cube( Draw3D_Box ) with a specific radius( 'side length = 2*radius' )\n
+	def addPoint(self, x: float, y: float, z: float, radius: float, color: int) -> Box:
+		"""Draws a cube( Box ) with a specific radius( 'side length = 2*radius' )\n
 		Since: 1.4.0 
 
 		Args:
 			color: point color 
 			x: x value of the center point 
 			y: y value of the center point 
 			z: z value of the center point 
 			radius: 1/2 of the side length of the cube 
 
 		Returns:
-			the Draw3D_Box generated, and visualized 
+			the Box generated, and visualized 
 		"""
 		pass
 
 	@overload
-	def addPoint(self, x: float, y: float, z: float, radius: float, color: int, alpha: int, cull: bool) -> Draw3D_Box:
-		"""Draws a cube( Draw3D_Box ) with a specific radius( 'side length = 2*radius' )\n
+	def addPoint(self, x: float, y: float, z: float, radius: float, color: int, alpha: int, cull: bool) -> Box:
+		"""Draws a cube( Box ) with a specific radius( 'side length = 2*radius' )\n
 		Since: 1.4.0 
 
 		Args:
 			color: point color 
 			alpha: alpha of the point 
 			x: x value of the center point 
 			y: y value of the center point 
 			z: z value of the center point 
 			radius: 1/2 of the side length of the cube 
 			cull: whether to cull the point or not 
 
 		Returns:
-			the Draw3D_Box generated, and visualized 
+			the Box generated, and visualized 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			x: top left 
 			y: 
 			z: 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float, width: float, height: float) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float, width: float, height: float) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			x: 
 			width: 
 			y: 
 			z: 
 			height: 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			zRot: 
 			yRot: 
 			x: 
 			xRot: 
 			y: 
 			z: 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			zRot: 
 			yRot: 
 			x: 
@@ -305,15 +357,15 @@
 			y: 
 			z: 
 			height: 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float, minSubdivisions: int) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float, minSubdivisions: int) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			zRot: 
 			yRot: 
 			x: 
@@ -323,15 +375,15 @@
 			z: 
 			minSubdivisions: 
 			height: 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float, minSubdivisions: int, renderBack: bool) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float, minSubdivisions: int, renderBack: bool) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			zRot: 
 			yRot: 
 			x: 
@@ -342,15 +394,15 @@
 			minSubdivisions: 
 			renderBack: 
 			height: 
 		"""
 		pass
 
 	@overload
-	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float, minSubdivisions: int, renderBack: bool, cull: bool) -> Draw3D_Surface:
+	def addDraw2D(self, x: float, y: float, z: float, xRot: float, yRot: float, zRot: float, width: float, height: float, minSubdivisions: int, renderBack: bool, cull: bool) -> Surface:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			zRot: 
 			yRot: 
 			x: top left 
@@ -361,21 +413,79 @@
 			minSubdivisions: 
 			renderBack: 
 			height: 
 		"""
 		pass
 
 	@overload
-	def removeDraw2D(self, surface: Draw3D_Surface) -> None:
+	def removeDraw2D(self, surface: Surface) -> None:
 		"""
 		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
+	def boxBuilder(self) -> Box_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a new Box_Builder instance. 
+		"""
+		pass
+
+	@overload
+	def boxBuilder(self, pos: BlockPosHelper) -> Box_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			pos: the block position of the box 
+
+		Returns:
+			a new Box_Builder instance. 
+		"""
+		pass
+
+	@overload
+	def boxBuilder(self, x: int, y: int, z: int) -> Box_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			x: the x coordinate of the box 
+			y: the y coordinate of the box 
+			z: the z coordinate of the box 
+
+		Returns:
+			a new Box_Builder instance. 
+		"""
+		pass
+
+	@overload
+	def lineBuilder(self) -> Line3D_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a new Line3D_Builder instance. 
+		"""
+		pass
+
+	@overload
+	def surfaceBuilder(self) -> Surface_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a new Surface_Builder instance. 
+		"""
+		pass
+
+	@overload
 	def register(self) -> "Draw3D":
 		"""register so it actually shows up\n
 		Since: 1.6.5 
 
 		Returns:
 			self for chaining 
 		"""
@@ -388,13 +498,13 @@
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def render(self, matrixStack: MatrixStack) -> None:
+	def render(self, matrixStack: MatrixStack, tickDelta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D_Box.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Box.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import TypeVar
-from .PositionCommon_Vec3D import PositionCommon_Vec3D
+from .RenderElement3D import RenderElement3D
+from .Vec3D import Vec3D
 
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+BufferBuilder = TypeVar["net.minecraft.client.render.BufferBuilder"]
 
-class Draw3D_Box:
-	pos: PositionCommon_Vec3D
+class Box(RenderElement3D):
+	"""
+	"""
+	pos: Vec3D
 	color: int
 	fillColor: int
 	fill: bool
 	cull: bool
 
 	@overload
 	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, fillColor: int, fill: bool, cull: bool) -> None:
@@ -103,13 +107,13 @@
 
 		Args:
 			fill: 
 		"""
 		pass
 
 	@overload
-	def render(self, matrixStack: MatrixStack) -> None:
+	def render(self, matrixStack: MatrixStack, builder: BufferBuilder, tickDelta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D_Line.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Vec3D.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,183 @@
 from typing import overload
 from typing import TypeVar
-from .PositionCommon_Vec3D import PositionCommon_Vec3D
+from .Vec2D import Vec2D
+from .Pos3D import Pos3D
 
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+Vector3f = TypeVar["org.joml.Vector3f"]
 
-class Draw3D_Line:
-	pos: PositionCommon_Vec3D
-	color: int
-	cull: bool
+class Vec3D(Vec2D):
+	"""
+	Since: 1.2.6 [citation needed] 
+	"""
+	z1: float
+	z2: float
 
 	@overload
-	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, cull: bool) -> None:
+	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> None:
 		pass
 
 	@overload
-	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, cull: bool) -> None:
+	def __init__(self, start: Pos3D, end: Pos3D) -> None:
 		pass
 
 	@overload
-	def setPos(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> None:
+	def getZ1(self) -> float:
+		pass
+
+	@overload
+	def getZ2(self) -> float:
+		pass
+
+	@overload
+	def getDeltaZ(self) -> float:
+		pass
+
+	@overload
+	def getStart(self) -> Pos3D:
+		pass
+
+	@overload
+	def getEnd(self) -> Pos3D:
+		pass
+
+	@overload
+	def getMagnitude(self) -> float:
+		pass
+
+	@overload
+	def getMagnitudeSq(self) -> float:
+		pass
+
+	@overload
+	def add(self, vec: "Vec3D") -> "Vec3D":
+		pass
+
+	@overload
+	def addStart(self, pos: Pos3D) -> "Vec3D":
 		"""
-		Since: 1.0.6 
+		Since: 1.6.4 
+
+		Args:
+			pos: 
+		"""
+		pass
+
+	@overload
+	def addEnd(self, pos: Pos3D) -> "Vec3D":
+		"""
+		Since: 1.6.4 
+
+		Args:
+			pos: 
+		"""
+		pass
+
+	@overload
+	def addStart(self, x: float, y: float, z: float) -> "Vec3D":
+		"""
+		Since: 1.6.4 
+
+		Args:
+			x: 
+			y: 
+			z: 
+		"""
+		pass
+
+	@overload
+	def addEnd(self, x: float, y: float, z: float) -> "Vec3D":
+		"""
+		Since: 1.6.4 
+
+		Args:
+			x: 
+			y: 
+			z: 
+		"""
+		pass
+
+	@overload
+	def add(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> "Vec3D":
+		"""
+		Since: 1.6.3 
 
 		Args:
 			z1: 
 			y1: 
 			z2: 
 			x1: 
 			y2: 
 			x2: 
 		"""
 		pass
 
 	@overload
-	def setColor(self, color: int) -> None:
+	def multiply(self, vec: "Vec3D") -> "Vec3D":
+		pass
+
+	@overload
+	def multiply(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> "Vec3D":
 		"""
-		Since: 1.0.6 
+		Since: 1.6.3 
 
 		Args:
-			color: 
+			z1: 
+			y1: 
+			z2: 
+			x1: 
+			y2: 
+			x2: 
 		"""
 		pass
 
 	@overload
-	def setColor(self, color: int, alpha: int) -> None:
+	def scale(self, scale: float) -> "Vec3D":
 		"""
-		Since: 1.1.8 
+		Since: 1.6.3 
 
 		Args:
-			color: 
-			alpha: 
+			scale: 
 		"""
 		pass
 
 	@overload
-	def setAlpha(self, alpha: int) -> None:
+	def normalize(self) -> "Vec3D":
 		"""
-		Since: 1.1.8 
-
-		Args:
-			alpha: 
+		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
-	def render(self, matrixStack: MatrixStack) -> None:
+	def getPitch(self) -> float:
+		pass
+
+	@overload
+	def getYaw(self) -> float:
+		pass
+
+	@overload
+	def dotProduct(self, vec: "Vec3D") -> float:
+		pass
+
+	@overload
+	def crossProduct(self, vec: "Vec3D") -> "Vec3D":
+		pass
+
+	@overload
+	def reverse(self) -> "Vec3D":
+		pass
+
+	@overload
+	def toString(self) -> str:
+		pass
+
+	@overload
+	def toMojangFloatVector(self) -> Vector3f:
+		"""
+		Since: 1.6.5 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Draw3D_Surface.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileChooser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,61 @@
 from typing import overload
 from typing import TypeVar
-from .Draw2D import Draw2D
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
-from .PositionCommon_Pos2D import PositionCommon_Pos2D
+from .OverlayContainer import OverlayContainer
+from .IOverlayParent import IOverlayParent
+from .FileChooser_fileObj import FileChooser_fileObj
 
+Consumer = TypeVar["java.util.function.Consumer_java.io.File_"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+File = TypeVar["java.io.File"]
+TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class Draw3D_Surface(Draw2D):
-	"""
-	Since: 1.6.5 
-	"""
-	pos: PositionCommon_Pos3D
-	rotations: PositionCommon_Pos3D
-	zIndexScale: float
-	renderBack: bool
-	cull: bool
+class FileChooser(OverlayContainer):
+	root: File
 
 	@overload
-	def __init__(self, pos: PositionCommon_Pos3D, rotations: PositionCommon_Pos3D, sizes: PositionCommon_Pos2D, minSubdivisions: int, renderBack: bool, cull: bool) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, directory: File, selected: File, parent: IOverlayParent, setFile: Consumer, editFile: Consumer) -> None:
 		pass
 
 	@overload
-	def setPos(self, x: float, y: float, z: float) -> None:
+	def setDir(self, dir: File) -> None:
 		pass
 
 	@overload
-	def setRotations(self, x: float, y: float, z: float) -> None:
+	def selectFile(self, f: File) -> None:
 		pass
 
 	@overload
-	def setSizes(self, x: float, y: float) -> None:
-		pass
-
-	@overload
-	def getSizes(self) -> PositionCommon_Pos2D:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def setMinSubdivisions(self, minSubdivisions: int) -> None:
+	def addFile(self, f: File) -> None:
 		pass
 
 	@overload
-	def getMinSubdivisions(self) -> int:
+	def addFile(self, f: File, btnText: str) -> None:
 		pass
 
 	@overload
-	def getHeight(self) -> int:
+	def updateFilePos(self) -> None:
 		pass
 
 	@overload
-	def getWidth(self) -> int:
+	def confirmDelete(self, f: FileChooser_fileObj) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def delete(self, f: FileChooser_fileObj) -> None:
 		pass
 
 	@overload
-	def render3D(self, matrixStack: MatrixStack) -> None:
+	def onScrollbar(self, page: float) -> None:
 		pass
 
 	@overload
-	def render(self, matrixStack: MatrixStack) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EditorScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EditorScreen.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .History import History
 from .SelectCursor import SelectCursor
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 
 Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 Style = TypeVar["net.minecraft.text.Style"]
+File = TypeVar["java.io.File"]
 
 class EditorScreen(BaseScreen):
 	langs: List[str]
 	defaultStyle: Style
 	history: History
 	cursor: SelectCursor
 	blockFirst: bool
@@ -78,15 +79,15 @@
 		pass
 
 	@overload
 	def mouseScrolled(self, mouseX: float, mouseY: float, amount: float) -> bool:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def openParent(self) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EnchantInventory.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/WardenEntityHelper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 from typing import overload
-from typing import List
-from .Inventory import Inventory
-from .TextHelper import TextHelper
+from typing import TypeVar
+from .MobEntityHelper import MobEntityHelper
 
+WardenEntity = TypeVar["net.minecraft.entity.mob.WardenEntity"]
 
-class EnchantInventory(Inventory):
+class WardenEntityHelper(MobEntityHelper):
 	"""
-	Since: 1.3.1 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def getRequiredLevels(self) -> List[int]:
+	def __init__(self, base: WardenEntity) -> None:
+		pass
+
+	@overload
+	def getAnger(self) -> int:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			xp level required to do enchantments 
+			this warden's anger towards its active target. 
 		"""
 		pass
 
 	@overload
-	def getEnchantments(self) -> List[TextHelper]:
+	def isDigging(self) -> bool:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			list of enchantments text. 
+			'true' if this warden is digging into the ground, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getEnchantmentIds(self) -> List[str]:
+	def isEmerging(self) -> bool:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			id for enchantments 
+			'true' if this warden is emerging from the ground, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getEnchantmentLevels(self) -> List[int]:
+	def isRoaring(self) -> bool:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			level of enchantments 
+			'true' if this warden is roaring, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def doEnchant(self, index: int) -> bool:
-		"""clicks the button to enchant.\n
-		Since: 1.3.1 
+	def isSniffing(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this warden is sniffing, 'false' otherwise. 
+		"""
+		pass
 
-		Args:
-			index: 
+	@overload
+	def isChargingSonicBoom(self) -> bool:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			success 
+			'true' if this warden is charging its sonic boom attack, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EntityHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EntityHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Generic
 from .BaseHelper import BaseHelper
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
-from .PositionCommon_Pos2D import PositionCommon_Pos2D
+from .Pos3D import Pos3D
+from .BlockPosHelper import BlockPosHelper
+from .Pos2D import Pos2D
 from .TextHelper import TextHelper
 from .NBTElementHelper import NBTElementHelper
+from .DirectionHelper import DirectionHelper
+from .ChunkHelper import ChunkHelper
 from .ClientPlayerEntityHelper import ClientPlayerEntityHelper
 from .PlayerEntityHelper import PlayerEntityHelper
 from .VillagerEntityHelper import VillagerEntityHelper
 from .MerchantEntityHelper import MerchantEntityHelper
 from .LivingEntityHelper import LivingEntityHelper
 from .ItemEntityHelper import ItemEntityHelper
 
@@ -18,34 +21,44 @@
 T = TypeVar("T")
 
 class EntityHelper(Generic[T], BaseHelper):
 	"""
 	"""
 
 	@overload
-	def getPos(self) -> PositionCommon_Pos3D:
+	def getPos(self) -> Pos3D:
 		"""
 
 		Returns:
 			entity position. 
 		"""
 		pass
 
 	@overload
-	def getBlockPos(self) -> PositionCommon_Pos3D:
+	def getBlockPos(self) -> BlockPosHelper:
 		"""
 		Since: 1.6.5 
 
 		Returns:
 			entity block position. 
 		"""
 		pass
 
 	@overload
-	def getChunkPos(self) -> PositionCommon_Pos2D:
+	def getEyePos(self) -> Pos3D:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the entity's eye position. 
+		"""
+		pass
+
+	@overload
+	def getChunkPos(self) -> Pos2D:
 		"""
 		Since: 1.6.5 
 
 		Returns:
 			entity chunk coordinates. Since Pos2D only has x and y fields, z coord is y. 
 		"""
 		pass
@@ -156,14 +169,34 @@
 
 		Returns:
 			if the entity is on fire. 
 		"""
 		pass
 
 	@overload
+	def isSneaking(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the entity is sneaking, 'false' otherwise. 
+		"""
+		pass
+
+	@overload
+	def isSprinting(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the entity is sprinting, 'false' otherwise. 
+		"""
+		pass
+
+	@overload
 	def getVehicle(self) -> "EntityHelper":
 		"""
 		Since: 1.1.8 [citation needed] 
 
 		Returns:
 			the vehicle of the entity. 
 		"""
@@ -183,44 +216,44 @@
 	def getNBT(self) -> NBTElementHelper:
 		"""
 		Since: 1.2.8, was a String until 1.5.0 
 		"""
 		pass
 
 	@overload
-	def setCustomName(self, name: TextHelper) -> None:
+	def setCustomName(self, name: TextHelper) -> "EntityHelper":
 		"""
 		Since: 1.6.4 
 
 		Args:
 			name: 
 		"""
 		pass
 
 	@overload
-	def setCustomNameVisible(self, b: bool) -> None:
+	def setCustomNameVisible(self, b: bool) -> "EntityHelper":
 		"""sets the name to always display\n
 		Since: 1.8.0 
 
 		Args:
 			b: 
 		"""
 		pass
 
 	@overload
-	def setGlowingColor(self, color: int) -> None:
+	def setGlowingColor(self, color: int) -> "EntityHelper":
 		"""
 
 		Args:
 			color: 
 		"""
 		pass
 
 	@overload
-	def resetGlowingColor(self) -> None:
+	def resetGlowingColor(self) -> "EntityHelper":
 		"""
 		"""
 		pass
 
 	@overload
 	def getGlowingColor(self) -> int:
 		"""warning: affected by setGlowingColor\n
@@ -262,14 +295,124 @@
 
 		Returns:
 			UUID of the entity, random* if not a player, otherwise the player's uuid. 
 		"""
 		pass
 
 	@overload
+	def getMaxAir(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the maximum amount of air this entity can have. 
+		"""
+		pass
+
+	@overload
+	def getAir(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the amount of air this entity has. 
+		"""
+		pass
+
+	@overload
+	def getSpeed(self) -> float:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			this entity's current speed in blocks per second. 
+		"""
+		pass
+
+	@overload
+	def getFacingDirection(self) -> DirectionHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the direction the entity is facing, rounded to the nearest 45 degrees. 
+		"""
+		pass
+
+	@overload
+	def distanceTo(self, entity: "EntityHelper") -> float:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the distance between this entity and the specified one. 
+		"""
+		pass
+
+	@overload
+	def distanceTo(self, pos: BlockPosHelper) -> float:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the distance between this entity and the specified position. 
+		"""
+		pass
+
+	@overload
+	def distanceTo(self, pos: Pos3D) -> float:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the distance between this entity and the specified position. 
+		"""
+		pass
+
+	@overload
+	def distanceTo(self, x: float, y: float, z: float) -> float:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the distance between this entity and the specified position. 
+		"""
+		pass
+
+	@overload
+	def getVelocity(self) -> Pos3D:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the velocity vector. 
+		"""
+		pass
+
+	@overload
+	def getChunk(self) -> ChunkHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the chunk helper for the chunk this entity is in. 
+		"""
+		pass
+
+	@overload
+	def getBiome(self) -> str:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the name of the biome this entity is in. 
+		"""
+		pass
+
+	@overload
 	def toString(self) -> str:
 		pass
 
 	@overload
 	def create(self, e: Entity) -> "EntityHelper":
 		"""mostly for internal use.
 
@@ -328,19 +471,39 @@
 
 		Returns:
 			cast of this entity helper (mainly for typescript) 
 		"""
 		pass
 
 	@overload
+	def asAnimal(self) -> LivingEntityHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			this helper as an animal entity helper (mainly for typescript). 
+		"""
+		pass
+
+	@overload
 	def asItem(self) -> ItemEntityHelper:
 		"""
 		Since: 1.6.3 
 
 		Returns:
 			cast of this entity helper (mainly for typescript) 
 		"""
 		pass
 
+	@overload
+	def asServerEntity(self) -> "EntityHelper":
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the entity as a server entity if an integrated server is running and 'null' otherwise. 
+		"""
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventBlockUpdate.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventBlockUpdate.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventChooser.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventChooser.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 		pass
 
 	@overload
 	def onScrollbar(self, page: float) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventClickSlot.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventClickSlot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
+from .ICancelable import ICancelable
 from .Inventory import Inventory
 
 HandledScreen = TypeVar["net.minecraft.client.gui.screen.ingame.HandledScreen__"]
 
-class EventClickSlot(BaseEvent):
+class EventClickSlot(BaseEvent, ICancelable):
 	"""event triggered when the user "clicks" a slot in an inventory\n
 	Since: 1.6.4 
 	"""
 	mode: int
 	button: int
 	slot: int
 	cancel: bool
@@ -24,13 +25,21 @@
 
 		Returns:
 			inventory associated with the event 
 		"""
 		pass
 
 	@overload
+	def cancel(self) -> None:
+		pass
+
+	@overload
+	def isCanceled(self) -> bool:
+		pass
+
+	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventContainer.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventCustom.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventCustom.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventDropSlot.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventDropSlot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
+from .ICancelable import ICancelable
 from .Inventory import Inventory
 
 HandledScreen = TypeVar["net.minecraft.client.gui.screen.ingame.HandledScreen__"]
 
-class EventDropSlot(BaseEvent):
+class EventDropSlot(BaseEvent, ICancelable):
 	"""event triggered when an item is dropped\n
 	Since: 1.6.4 
 	"""
 	slot: int
 	all: bool
 	cancel: bool
 
@@ -23,13 +24,21 @@
 
 		Returns:
 			inventory associated with the event 
 		"""
 		pass
 
 	@overload
+	def cancel(self) -> None:
+		pass
+
+	@overload
+	def isCanceled(self) -> bool:
+		pass
+
+	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventKey.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventKey.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventRecvMessage.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventRecvMessage.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventRegistry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventRegistry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventResourcePackLoaded.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventResourcePackLoaded.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventService.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventService.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 		Args:
 			name: 
 		"""
 		pass
 
 	@overload
 	def remove(self, key: str) -> None:
-		"""removes a key from the global varaible space.\n
+		"""removes a key from the global variable space.\n
 		Since: 1.6.5 
 
 		Args:
 			key: 
 		"""
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/EventWrappedScript.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/EventWrappedScript.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Extension.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Extension.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ExtensionLoader.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ExtensionLoader.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FChat.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FChat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
 from .BaseLibrary import BaseLibrary
 from .TextHelper import TextHelper
 from .TextBuilder import TextBuilder
 from .CommandBuilder import CommandBuilder
 from .CommandNodeHelper import CommandNodeHelper
 from .CommandManager import CommandManager
 from .ChatHistoryManager import ChatHistoryManager
 
 Logger = TypeVar["org.slf4j.Logger"]
 
 class FChat(BaseLibrary):
-	"""Functions for interacting with chat.
-
+	"""Functions for interacting with chat. 
 An instance of this class is passed to scripts as the 'Chat' variable.
 	"""
 
 	@overload
 	def __init__(self) -> None:
 		pass
 
@@ -37,14 +37,39 @@
 		Args:
 			await: should wait for message to actually be sent to chat to continue. 
 			message: 
 		"""
 		pass
 
 	@overload
+	def logf(self, message: str, args: List[object]) -> None:
+		"""Logs the formatted message to the player's chat. The message is formatted using the default
+java String#format(java.lang.String,java.lang.Object...) syntax.\n
+		Since: 1.8.4 
+
+		Args:
+			args: the arguments used to format the message 
+			message: the message to format and log 
+		"""
+		pass
+
+	@overload
+	def logf(self, message: str, await_: bool, args: List[object]) -> None:
+		"""Logs the formatted message to the player's chat. The message is formatted using the default
+java String#format(java.lang.String,java.lang.Object...) syntax.\n
+		Since: 1.8.4 
+
+		Args:
+			args: the arguments used to format the message 
+			await: whether to wait for message to be sent to chat before continuing 
+			message: the message to format and log 
+		"""
+		pass
+
+	@overload
 	def say(self, message: str) -> None:
 		"""Say to server as player.\n
 		Since: 1.0.0 
 
 		Args:
 			message: 
 		"""
@@ -58,14 +83,37 @@
 		Args:
 			await: 
 			message: 
 		"""
 		pass
 
 	@overload
+	def sayf(self, message: str, args: List[object]) -> None:
+		"""Sends the formatted message to the server. The message is formatted using the default java String#format(java.lang.String,java.lang.Object...) syntax.\n
+		Since: 1.8.4 
+
+		Args:
+			args: the arguments used to format the message 
+			message: the message to format and send to the server 
+		"""
+		pass
+
+	@overload
+	def sayf(self, message: str, await_: bool, args: List[object]) -> None:
+		"""Sends the formatted message to the server. The message is formatted using the default java String#format(java.lang.String,java.lang.Object...) syntax.\n
+		Since: 1.8.4 
+
+		Args:
+			args: the arguments used to format the message 
+			await: whether to wait for message to be sent to chat before continuing 
+			message: the message to format and send to the server 
+		"""
+		pass
+
+	@overload
 	def open(self, message: str) -> None:
 		"""open the chat input box with specific text already typed.\n
 		Since: 1.6.4 
 
 		Args:
 			message: the message to start the chat screen with 
 		"""
@@ -224,14 +272,27 @@
 	def getHistory(self) -> ChatHistoryManager:
 		"""
 		Since: 1.7.0 
 		"""
 		pass
 
 	@overload
+	def getTextWidth(self, text: str) -> int:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			text: the text to get the width of 
+
+		Returns:
+			the width of the given text in pixels. 
+		"""
+		pass
+
+	@overload
 	def sectionSymbolToAmpersand(self, string: str) -> str:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			string:
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FClient.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Draw2DElement_Builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,190 +1,256 @@
 from typing import overload
-from typing import TypeVar
-from .PerExecLibrary import PerExecLibrary
-from .TickSync import TickSync
-from .BaseScriptContext import BaseScriptContext
-from .MethodWrapper import MethodWrapper
-from .OptionsHelper import OptionsHelper
-from .ServerInfoHelper import ServerInfoHelper
+from .Alignable import Alignable
+from .RenderElementBuilder import RenderElementBuilder
+from .IDraw2D import IDraw2D
+from .Draw2D import Draw2D
 
-MinecraftClient = TypeVar["net.minecraft.client.MinecraftClient"]
 
-class FClient(PerExecLibrary):
-	"""Functions that interact with minecraft that don't fit into their own module.
-
-An instance of this class is passed to scripts as the 'Client' variable.\n
-	Since: 1.2.9 
+class Draw2DElement_Builder(Alignable, RenderElementBuilder):
+	"""
+	Since: 1.8.4 
 	"""
-	tickSynchronizer: TickSync
 
 	@overload
-	def __init__(self, context: BaseScriptContext) -> None:
+	def __init__(self, parent: IDraw2D, draw2D: Draw2D) -> None:
 		pass
 
 	@overload
-	def getMinecraft(self) -> MinecraftClient:
+	def x(self, x: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.0.0 (was in the 'jsmacros' library until 1.2.9) 
+		Since: 1.8.4 
+
+		Args:
+			x: the x position of the draw2D 
 
 		Returns:
-			the raw minecraft client class, it may be useful to use Minecraft Mappings Viewer for this. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def runOnMainThread(self, runnable: MethodWrapper) -> None:
-		"""Run your task on the main minecraft thread\n
-		Since: 1.4.0 
+	def getX(self) -> int:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			runnable: task to run 
+		Returns:
+			the x position of the draw2D. 
 		"""
 		pass
 
 	@overload
-	def runOnMainThread(self, runnable: MethodWrapper, watchdogMaxTime: float) -> None:
+	def y(self, y: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Args:
-			runnable: 
-			watchdogMaxTime: max time for the watchdog to wait before killing the script 
+			y: the y position of the draw2D 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getGameOptions(self) -> OptionsHelper:
+	def getY(self) -> int:
 		"""
-		Since: 1.1.7 (was in the 'jsmacros' library until 1.2.9) 
+		Since: 1.8.4 
 
 		Returns:
-			an OptionsHelper for the game options. 
+			the y position of the draw2D. 
 		"""
 		pass
 
 	@overload
-	def mcVersion(self) -> str:
+	def pos(self, x: int, y: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.1.2 (was in the 'jsmacros' library until 1.2.9) 
+		Since: 1.8.4 
+
+		Args:
+			x: the x position of the draw2D 
+			y: the y position of the draw2D 
 
 		Returns:
-			the current minecraft version as a String . 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getFPS(self) -> str:
+	def width(self, width: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.2.0 (was in the 'jsmacros' library until 1.2.9) 
+		Since: 1.8.4 
+
+		Args:
+			width: the width of the draw2D 
 
 		Returns:
-			the fps debug string from minecraft. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def loadWorld(self, folderName: str) -> None:
-		"""Join singleplayer world\n
-		Since: 1.6.6 
+	def getWidth(self) -> int:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			folderName: 
+		Returns:
+			the width of the draw2D. 
 		"""
 		pass
 
 	@overload
-	def connect(self, ip: str) -> None:
+	def height(self, height: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.2.3 (was in the 'jsmacros' library until 1.2.9) 
+		Since: 1.8.4 
 
 		Args:
-			ip: 
+			height: the height of the draw2D 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def connect(self, ip: str, port: int) -> None:
-		"""Connect to a server\n
-		Since: 1.2.3 (was in the 'jsmacros' library until 1.2.9) 
+	def getHeight(self) -> int:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			port: 
-			ip: 
+		Returns:
+			the height of the draw2D. 
 		"""
 		pass
 
 	@overload
-	def disconnect(self) -> None:
+	def size(self, width: int, height: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.2.3 (was in the 'jsmacros' library until 1.2.9) 
+		Since: 1.8.4 
+
+		Args:
+			width: the width of the draw2D 
+			height: the height of the draw2D 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def disconnect(self, callback: MethodWrapper) -> None:
-		"""Disconnect from a server with callback.\n
-		Since: 1.2.3 (was in the 'jsmacros' library until 1.2.9) 'callback' defaults to 'null' 
+	def scale(self, scale: float) -> "Draw2DElement_Builder":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			callback: calls your method as a Consumer Boolean 
+			scale: the scale of the draw2D 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def shutdown(self) -> None:
-		"""Closes the client (stops the game).
-Waits until the game has stopped, meaning no further code is executed (for obvious reasons).
-Warning: this does not wait on joined threads, so your script may stop at an undefined point.\n
-		Since: 1.6.0 
+	def getScale(self) -> float:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the scale of the draw2D. 
+		"""
+		pass
+
+	@overload
+	def rotation(self, rotation: float) -> "Draw2DElement_Builder":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			rotation: the rotation (clockwise) of the draw2D in degrees 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def waitTick(self) -> None:
+	def getRotation(self) -> float:
 		"""
-		Since: 1.2.4 
+		Since: 1.8.4 
+
+		Returns:
+			the rotation (clockwise) of the draw2D in degrees. 
 		"""
 		pass
 
 	@overload
-	def waitTick(self, i: int) -> None:
-		"""waits the specified number of client ticks.
-don't use this on an event that the main thread waits on (joins)... that'll cause circular waiting.\n
-		Since: 1.2.6 
+	def rotateCenter(self, rotateCenter: bool) -> "Draw2DElement_Builder":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			i: 
+			rotateCenter: whether this draw2D should be rotated around its center 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def ping(self, ip: str) -> ServerInfoHelper:
+	def isRotatingCenter(self) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
-		Args:
-			ip: 
+		Returns:
+			'true' if this draw2D should be rotated around its center, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def pingAsync(self, ip: str, callback: MethodWrapper) -> None:
+	def zIndex(self, zIndex: int) -> "Draw2DElement_Builder":
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
-		Args:
-			ip: 
-			callback: 
+		Returns:
+			the z-index of the draw2D. 
 		"""
 		pass
 
 	@overload
-	def cancelAllPings(self) -> None:
+	def getZIndex(self) -> int:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
+
+		Returns:
+			the z-index of the draw2D. 
 		"""
 		pass
 
+	@overload
+	def getScaledWidth(self) -> int:
+		pass
+
+	@overload
+	def getParentWidth(self) -> int:
+		pass
+
+	@overload
+	def getScaledHeight(self) -> int:
+		pass
+
+	@overload
+	def getParentHeight(self) -> int:
+		pass
+
+	@overload
+	def getScaledLeft(self) -> int:
+		pass
+
+	@overload
+	def getScaledTop(self) -> int:
+		pass
+
+	@overload
+	def moveTo(self, x: int, y: int) -> "Draw2DElement_Builder":
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FFS.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/RecipeHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,155 +1,129 @@
 from typing import overload
 from typing import List
-from .PerExecLibrary import PerExecLibrary
-from .BaseScriptContext import BaseScriptContext
-from .FileHandler import FileHandler
+from typing import TypeVar
+from .BaseHelper import BaseHelper
+from .ItemStackHelper import ItemStackHelper
 
+Recipe = TypeVar["net.minecraft.recipe.Recipe__"]
 
-class FFS(PerExecLibrary):
-	"""Better File-System functions.
-
-An instance of this class is passed to scripts as the 'FS' variable.\n
-	Since: 1.1.8 
+class RecipeHelper(BaseHelper):
+	"""
+	Since: 1.3.1 
 	"""
 
 	@overload
-	def __init__(self, context: BaseScriptContext) -> None:
+	def __init__(self, base: Recipe, syncId: int) -> None:
 		pass
 
 	@overload
-	def list(self, path: str) -> List[str]:
-		"""List files in path.\n
-		Since: 1.1.8 
-
-		Args:
-			path: relative to the script's folder. 
-
-		Returns:
-			An array of file names as String . 
+	def getId(self) -> str:
+		"""
+		Since: 1.3.1 
 		"""
 		pass
 
 	@overload
-	def exists(self, path: str) -> bool:
-		"""Check if a file exists.\n
-		Since: 1.1.8 
-
-		Args:
-			path: relative to the script's folder. 
+	def getIngredients(self) -> List[List[ItemStackHelper]]:
+		"""get ingredients list\n
+		Since: 1.8.3 
 		"""
 		pass
 
 	@overload
-	def isDir(self, path: str) -> bool:
-		"""Check if a file is a directory.\n
-		Since: 1.1.8 
-
-		Args:
-			path: relative to the script's folder. 
+	def getOutput(self) -> ItemStackHelper:
+		"""
+		Since: 1.3.1 
 		"""
 		pass
 
 	@overload
-	def getName(self, path: str) -> str:
-		"""Get the last part (name) of a file.\n
-		Since: 1.1.8 
+	def craft(self, craftAll: bool) -> "RecipeHelper":
+		"""
+		Since: 1.3.1 
 
 		Args:
-			path: relative to the script's folder. 
-
-		Returns:
-			a String of the file name. 
+			craftAll: 
 		"""
 		pass
 
 	@overload
-	def makeDir(self, path: str) -> bool:
-		"""Make a directory.\n
-		Since: 1.1.8 
-
-		Args:
-			path: relative to the script's folder. 
+	def getGroup(self) -> str:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			a Boolean for success. 
+			the type of this recipe. 
 		"""
 		pass
 
 	@overload
-	def move(self, from_: str, to: str) -> None:
-		"""Move a file.\n
-		Since: 1.1.8 
+	def hasRecipeRemainders(self) -> bool:
+		"""This will not account for the actual items used in the recipe, but only the default recipe
+itself. Items with durability or with a lot of tags will probably not work correctly.\n
+		Since: 1.8.4 
 
-		Args:
-			from: relative to the script's folder. 
-			to: relative to the script's folder. 
+		Returns:
+			will return 'true' if any of the default ingredients have a recipe remainder. 
 		"""
 		pass
 
 	@overload
-	def copy(self, from_: str, to: str) -> None:
-		"""Copy a file.\n
-		Since: 1.1.8 
+	def getRecipeRemainders(self) -> List[List[ItemStackHelper]]:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			from: relative to the script's folder. 
-			to: relative to the script's folder. 
+		Returns:
+			a list of all possible recipe remainders. 
 		"""
 		pass
 
 	@overload
-	def unlink(self, path: str) -> bool:
-		"""Delete a file.\n
-		Since: 1.2.9 
-
-		Args:
-			path: relative to the script's folder. 
+	def getType(self) -> str:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			a Boolean for success. 
+			the type of this recipe. 
 		"""
 		pass
 
 	@overload
-	def combine(self, patha: str, pathb: str) -> str:
-		"""Combine 2 paths.\n
-		Since: 1.1.8 
-
-		Args:
-			patha: path is relative to the script's folder. 
-			pathb: 
+	def canCraft(self) -> bool:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			a String of the combined path. 
+			'true' if the recipe can be crafted with the current inventory, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getDir(self, path: str) -> str:
-		"""Gets the directory part of a file path, or the parent directory of a folder.\n
-		Since: 1.1.8 
+	def canCraft(self, amount: int) -> bool:
+		"""
+		Since: 1.8.4 
 
 		Args:
-			path: relative to the script's folder. 
+			amount: the amount of items to craft 
 
 		Returns:
-			a String of the combined path. 
+			'true' if the given amount of items can be crafted with the current inventory, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def open(self, path: str) -> FileHandler:
-		"""Open a FileHandler for the file at the specified path.\n
-		Since: 1.1.8 
-
-		Args:
-			path: relative to the script's folder. 
+	def getCraftableAmount(self) -> int:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			a FileHandler for the file path. 
+			how often the recipe can be crafted with the current player inventory. 
 		"""
 		pass
 
+	@overload
+	def toString(self) -> str:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FGlobalVars.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FGlobalVars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import overload
 from typing import Mapping
 from .BaseLibrary import BaseLibrary
 
 
 class FGlobalVars(BaseLibrary):
-	""""Global" variables for passing to other contexts.
-
+	""""Global" variables for passing to other contexts. 
 An instance of this class is passed to scripts as the 'GlobalVars' variable.\n
 	Since: 1.0.4 
 	"""
 	globalRaw: Mapping[str, object]
 
 	@overload
 	def __init__(self) -> None:
@@ -178,15 +177,15 @@
 		Args:
 			name: 
 		"""
 		pass
 
 	@overload
 	def remove(self, key: str) -> None:
-		"""removes a key from the global varaible space.\n
+		"""removes a key from the global variable space.\n
 		Since: 1.2.0 
 
 		Args:
 			key: 
 		"""
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FHud.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FHud.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import overload
 from typing import List
+from typing import Mapping
 from typing import Set
 from .BaseLibrary import BaseLibrary
 from .IDraw2D import IDraw2D
 from .Draw3D import Draw3D
 from .ScriptScreen import ScriptScreen
 from .IScreen import IScreen
+from .CustomImage import CustomImage
 from .Draw2D import Draw2D
 
 
 class FHud(BaseLibrary):
-	"""Functions for displaying stuff in 2 to 3 dimensions
-
+	"""Functions for displaying stuff in 2 to 3 dimensions 
 An instance of this class is passed to scripts as the 'Hud' variable.\n
 	Since: 1.0.5 
 	"""
 	overlays: Set[IDraw2D]
 	renders: Set[Draw3D]
 
 	@overload
@@ -53,14 +54,63 @@
 
 		Returns:
 			the currently open Screen as an IScreen 
 		"""
 		pass
 
 	@overload
+	def createTexture(self, width: int, height: int, name: str) -> CustomImage:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			width: the width of the canvas 
+			height: the height of the canvas 
+
+		Returns:
+			a CustomImage that can be used as a texture for screen backgrounds, rendering
+images, etc. 
+		"""
+		pass
+
+	@overload
+	def createTexture(self, path: str, name: str) -> CustomImage:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			path: absolute path to an image file 
+
+		Returns:
+			a CustomImage that can be used as a texture for screen backgrounds, rendering
+images, etc. 
+		"""
+		pass
+
+	@overload
+	def getRegisteredTextures(self) -> Mapping[str, CustomImage]:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			an immutable Map of all registered custom textures. 
+		"""
+		pass
+
+	@overload
+	def getScaleFactor(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the current gui scale factor of minecraft. 
+		"""
+		pass
+
+	@overload
 	def getOpenScreenName(self) -> str:
 		"""
 		Since: 1.0.5, renamed from 'getOpenScreen' in 1.2.7 
 
 		Returns:
 			The name of the currently open screen. 
 		"""
@@ -82,28 +132,26 @@
 		Since: 1.0.5 
 		"""
 		pass
 
 	@overload
 	def registerDraw2D(self, overlay: IDraw2D) -> None:
 		"""
-		Since: 1.0.5
-
+		Since: 1.0.5 
 Registers an IDraw2D to be rendered. 
 
 		Args:
 			overlay: 
 		"""
 		pass
 
 	@overload
 	def unregisterDraw2D(self, overlay: IDraw2D) -> None:
 		"""
-		Since: 1.0.5
-
+		Since: 1.0.5 
 Unregisters an IDraw2D to stop it being rendered. 
 
 		Args:
 			overlay: 
 		"""
 		pass
 
@@ -116,16 +164,15 @@
 			A list of current IDraw2D . 
 		"""
 		pass
 
 	@overload
 	def clearDraw2Ds(self) -> None:
 		"""
-		Since: 1.0.5
-
+		Since: 1.0.5 
 clears the Draw2D render list. 
 		"""
 		pass
 
 	@overload
 	def createDraw3D(self) -> Draw3D:
 		"""
@@ -135,28 +182,26 @@
 			a new Draw3D . 
 		"""
 		pass
 
 	@overload
 	def registerDraw3D(self, draw: Draw3D) -> None:
 		"""
-		Since: 1.0.6
-
+		Since: 1.0.6 
 Registers an Draw3D to be rendered. 
 
 		Args:
 			draw: 
 		"""
 		pass
 
 	@overload
 	def unregisterDraw3D(self, draw: Draw3D) -> None:
 		"""
-		Since: 1.0.6
-
+		Since: 1.0.6 
 Unregisters an Draw3D to stop it being rendered. 
 
 		Args:
 			draw: 
 		"""
 		pass
 
@@ -169,16 +214,15 @@
 			A list of current Draw3D . 
 		"""
 		pass
 
 	@overload
 	def clearDraw3Ds(self) -> None:
 		"""
-		Since: 1.0.6
-
+		Since: 1.0.6 
 clears the Draw2D render list. 
 		"""
 		pass
 
 	@overload
 	def getMouseX(self) -> float:
 		"""
@@ -195,10 +239,30 @@
 		Since: 1.1.3 
 
 		Returns:
 			the current Y coordinate of the mouse 
 		"""
 		pass
 
+	@overload
+	def getWindowWidth(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the current window width. 
+		"""
+		pass
+
+	@overload
+	def getWindowHeight(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the current window height. 
+		"""
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FJsMacros.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FPlayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,365 +1,374 @@
 from typing import overload
 from typing import List
-from .PerExecLibrary import PerExecLibrary
-from .BaseScriptContext import BaseScriptContext
-from .BaseProfile import BaseProfile
-from .ConfigManager import ConfigManager
-from .ServiceManager import ServiceManager
-from .EventContainer import EventContainer
-from .BaseEvent import BaseEvent
+from .BaseLibrary import BaseLibrary
+from .Inventory import Inventory
+from .ClientPlayerEntityHelper import ClientPlayerEntityHelper
+from .BlockDataHelper import BlockDataHelper
+from .EntityHelper import EntityHelper
 from .MethodWrapper import MethodWrapper
-from .IEventListener import IEventListener
-from .FJsMacros_EventAndContext import FJsMacros_EventAndContext
-from .EventCustom import EventCustom
+from .StatsHelper import StatsHelper
+from .PlayerInput import PlayerInput
+from .Pos3D import Pos3D
 
 
-class FJsMacros(PerExecLibrary):
-	"""Functions that interact directly with JsMacros or Events.
-
-An instance of this class is passed to scripts as the 'JsMacros' variable.
+class FPlayer(BaseLibrary):
+	"""Functions for getting and modifying the player's state. 
+An instance of this class is passed to scripts as the 'Player' variable.
 	"""
 
 	@overload
-	def __init__(self, context: BaseScriptContext) -> None:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def getProfile(self) -> BaseProfile:
+	def openInventory(self) -> Inventory:
 		"""
 
 		Returns:
-			the JsMacros profile class. 
+			the Inventory handler 
 		"""
 		pass
 
 	@overload
-	def getConfig(self) -> ConfigManager:
+	def getPlayer(self) -> ClientPlayerEntityHelper:
 		"""
+		Since: 1.0.3 
 
 		Returns:
-			the JsMacros config management class. 
+			the player entity wrapper. 
 		"""
 		pass
 
 	@overload
-	def getServiceManager(self) -> ServiceManager:
-		"""services are background scripts designed to run full time and are mainly noticed by their side effects.\n
-		Since: 1.6.3 
+	def getGameMode(self) -> str:
+		"""
+		Since: 1.0.9 
 
 		Returns:
-			for managing services. 
+			the player's current gamemode. 
 		"""
 		pass
 
 	@overload
-	def getOpenContexts(self) -> List[BaseScriptContext]:
+	def setGameMode(self, gameMode: str) -> None:
 		"""
-		Since: 1.4.0 
+		Since: 1.8.4 
 
-		Returns:
-			list of non-garbage-collected ScriptContext's 
+		Args:
+			gameMode: possible values are survival, creative, adventure, spectator (case insensitive) 
 		"""
 		pass
 
 	@overload
-	def runScript(self, file: str) -> EventContainer:
+	def rayTraceBlock(self, distance: float, fluid: bool) -> BlockDataHelper:
 		"""
-		Since: 1.1.5 
+		Since: 1.0.5 
 
 		Args:
-			file: 
+			distance: 
+			fluid: 
+
+		Returns:
+			the block/liquid the player is currently looking at. 
 		"""
 		pass
 
 	@overload
-	def runScript(self, file: str, fakeEvent: BaseEvent) -> EventContainer:
+	def rayTraceEntity(self) -> EntityHelper:
 		"""
-		Since: 1.6.3 
+		Since: 1.0.5 
 
-		Args:
-			file: 
-			fakeEvent: you probably actually want to pass an instance created by FJsMacros#createCustomEvent(java.lang.String) 
+		Returns:
+			the entity the camera is currently looking at. 
 		"""
 		pass
 
 	@overload
-	def runScript(self, file: str, fakeEvent: BaseEvent, callback: MethodWrapper) -> EventContainer:
-		"""runs a script with a eventCustom to be able to pass args\n
-		Since: 1.6.3 (1.1.5 - 1.6.3 didn't have fakeEvent) 
+	def rayTraceEntity(self, distance: int) -> EntityHelper:
+		"""
+		Since: 1.8.3 
 
 		Args:
-			file: 
-			fakeEvent: 
-			callback: 
+			distance: 
 
 		Returns:
-			container the script is running on. 
+			entity the player entity is currently looking at (if any). 
 		"""
 		pass
 
 	@overload
-	def runScript(self, language: str, script: str) -> EventContainer:
-		"""
-		Since: 1.2.4 
+	def writeSign(self, l1: str, l2: str, l3: str, l4: str) -> bool:
+		"""Write to a sign screen if a sign screen is currently open.\n
+		Since: 1.2.2 
 
 		Args:
-			language: 
-			script: 
+			l1: 
+			l2: 
+			l3: 
+			l4: 
+
+		Returns:
+			of success. 
 		"""
 		pass
 
 	@overload
-	def runScript(self, language: str, script: str, callback: MethodWrapper) -> EventContainer:
-		"""Runs a string as a script.\n
-		Since: 1.2.4 
+	def takeScreenshot(self, folder: str, callback: MethodWrapper) -> None:
+		"""
+		Since: 1.2.6 
 
 		Args:
-			callback: calls your method as a Consumer String 
-			language: 
-			script: 
-
-		Returns:
-			the EventContainer the script is running on. 
+			folder: 
+			callback: calls your method as a Consumer TextHelper 
 		"""
 		pass
 
 	@overload
-	def runScript(self, language: str, script: str, file: str, callback: MethodWrapper) -> EventContainer:
-		"""
-		Since: 1.6.0 
+	def takeScreenshot(self, folder: str, file: str, callback: MethodWrapper) -> None:
+		"""Take a screenshot and save to a file. 
+'file' is the optional one, typescript doesn't like it not being the last one that's optional\n
+		Since: 1.2.6 
 
 		Args:
+			folder: 
 			file: 
-			callback: 
-			language: 
-			script: 
+			callback: calls your method as a Consumer TextHelper 
 		"""
 		pass
 
 	@overload
-	def runScript(self, language: str, script: str, file: str, event: BaseEvent, callback: MethodWrapper) -> EventContainer:
+	def takePanorama(self, folder: str, width: int, height: int, callback: MethodWrapper) -> None:
 		"""
-		Since: 1.7.0 
+		Since: 1.8.4 
 
 		Args:
-			file: 
-			callback: 
-			language: 
-			event: 
-			script: 
+			folder: the folder to save the screenshot to, relative to the macro folder 
+			width: the width of the panorama 
+			callback: calls your method as a Consumer TextHelper 
+			height: the height of the panorama 
 		"""
 		pass
 
 	@overload
-	def wrapScriptRun(self, file: str) -> MethodWrapper:
+	def getStatistics(self) -> StatsHelper:
+		pass
+
+	@overload
+	def getReach(self) -> float:
 		"""
-		Since: 1.7.0 
+		Since: 1.8.4 
 
-		Args:
-			R: 
-			file: 
-			T: 
-			U: 
+		Returns:
+			the current reach distance of the player. 
 		"""
 		pass
 
 	@overload
-	def wrapScriptRun(self, language: str, script: str) -> MethodWrapper:
+	def createPlayerInput(self) -> PlayerInput:
+		"""Creates a new PlayerInput object.\n
+		Since: 1.4.0 
 		"""
-		Since: 1.7.0 
+		pass
 
-		Args:
-			R: 
-			T: 
-			U: 
-			language: 
-			script: 
+	@overload
+	def createPlayerInput(self, movementForward: float, movementSideways: float, yaw: float) -> PlayerInput:
+		"""Creates a new PlayerInput object.\n
+		Since: 1.4.0 
 		"""
 		pass
 
 	@overload
-	def wrapScriptRun(self, language: str, script: str, file: str) -> MethodWrapper:
+	def createPlayerInput(self, movementForward: float, yaw: float, jumping: bool, sprinting: bool) -> PlayerInput:
+		"""Creates a new PlayerInput object.\n
+		Since: 1.4.0 
 		"""
-		Since: 1.7.0 
+		pass
+
+	@overload
+	def createPlayerInput(self, movementForward: float, movementSideways: float, yaw: float, pitch: float, jumping: bool, sneaking: bool, sprinting: bool) -> PlayerInput:
+		"""Creates a new PlayerInput object.\n
+		Since: 1.4.0 
 
 		Args:
-			R: 
-			file: 
-			T: 
-			U: 
-			language: 
-			script: 
+			movementForward: 1 = forward input (W); 0 = no input; -1 = backward input (S) 
+			sprinting: sprint input 
+			jumping: jump input 
+			sneaking: sneak input 
+			pitch: pitch of the player 
+			yaw: yaw of the player 
+			movementSideways: 1 = left input (A); 0 = no input; -1 = right input (D) 
 		"""
 		pass
 
 	@overload
-	def wrapScriptRunAsync(self, file: str) -> MethodWrapper:
-		"""
-		Since: 1.7.0 
+	def createPlayerInputsFromCsv(self, csv: str) -> List[PlayerInput]:
+		"""Parses each row of CSV string into a 'PlayerInput' .
+The capitalization of the header matters. About the columns:  
+-  'movementForward' and 'movementSideways' as a number  
+- 'yaw' and 'pitch' as an absolute number  
+- 'jumping' , 'sneaking' and 'sprinting' have to be boolean   
+The separation must be a "," it's a csv...(but spaces don't matter) Quoted values don't work\n
+		Since: 1.4.0 
 
 		Args:
-			R: 
-			file: 
-			T: 
-			U: 
+			csv: CSV string to be parsed 
 		"""
 		pass
 
 	@overload
-	def wrapScriptRunAsync(self, language: str, script: str) -> MethodWrapper:
-		"""
-		Since: 1.7.0 
+	def createPlayerInputsFromJson(self, json: str) -> PlayerInput:
+		"""Parses a JSON string into a 'PlayerInput' Object.
+For details see 'PlayerInput.fromCsv()' , on what has to be present. Capitalization of the keys matters.\n
+		Since: 1.4.0 
 
 		Args:
-			R: 
-			T: 
-			U: 
-			language: 
-			script: 
+			json: JSON string to be parsed 
+
+		Returns:
+			The JSON parsed into a 'PlayerInput' 
 		"""
 		pass
 
 	@overload
-	def wrapScriptRunAsync(self, language: str, script: str, file: str) -> MethodWrapper:
+	def getCurrentPlayerInput(self) -> PlayerInput:
+		"""Creates a new 'PlayerInput' object with the current inputs of the player.\n
+		Since: 1.4.0 
 		"""
-		Since: 1.7.0 
+		pass
+
+	@overload
+	def addInput(self, input: PlayerInput) -> None:
+		"""Adds a new 'PlayerInput' to 'MovementQueue' to be executed\n
+		Since: 1.4.0 
 
 		Args:
-			R: 
-			file: 
-			T: 
-			U: 
-			language: 
-			script: 
+			input: the PlayerInput to be executed 
 		"""
 		pass
 
 	@overload
-	def open(self, path: str) -> None:
-		"""Opens a file with the default system program.\n
-		Since: 1.1.8 
+	def addInputs(self, inputs: List[PlayerInput]) -> None:
+		"""Adds multiple new 'PlayerInput' to 'MovementQueue' to be executed\n
+		Since: 1.4.0 
 
 		Args:
-			path: relative to the script's folder. 
+			inputs: the PlayerInputs to be executed 
 		"""
 		pass
 
 	@overload
-	def openUrl(self, url: str) -> None:
+	def clearInputs(self) -> None:
+		"""Clears all inputs in the 'MovementQueue'\n
+		Since: 1.4.0 
 		"""
-		Since: 1.6.0 
+		pass
 
-		Args:
-			url: 
-		"""
+	@overload
+	def setDrawPredictions(self, val: bool) -> None:
 		pass
 
 	@overload
-	def on(self, event: str, callback: MethodWrapper) -> IEventListener:
-		"""Creates a listener for an event, this function can be more efficient that running a script file when used properly.\n
-		Since: 1.2.7 
+	def predictInput(self, input: PlayerInput) -> Pos3D:
+		"""Predicts where one tick with a 'PlayerInput' as input would lead to.\n
+		Since: 1.4.0 
 
 		Args:
-			callback: calls your method as a BiConsumer BaseEvent , EventContainer 
-			event: 
+			input: the PlayerInput for the prediction 
+
+		Returns:
+			the position after the input 
 		"""
 		pass
 
 	@overload
-	def once(self, event: str, callback: MethodWrapper) -> IEventListener:
-		"""Creates a single-run listener for an event, this function can be more efficient that running a script file when used properly.\n
-		Since: 1.2.7 
+	def predictInput(self, input: PlayerInput, draw: bool) -> Pos3D:
+		"""Predicts where one tick with a 'PlayerInput' as input would lead to.\n
+		Since: 1.4.0 
 
 		Args:
-			callback: calls your method as a BiConsumer BaseEvent , EventContainer 
-			event: 
+			input: the PlayerInput for the prediction 
+			draw: whether to visualize the result or not 
 
 		Returns:
-			the listener. 
+			the position after the input 
 		"""
 		pass
 
 	@overload
-	def off(self, listener: IEventListener) -> bool:
-		"""
-		Since: 1.2.3 
+	def predictInputs(self, inputs: List[PlayerInput]) -> List[Pos3D]:
+		"""Predicts where each 'PlayerInput' executed in a row would lead
+without drawing it.\n
+		Since: 1.4.0 
 
 		Args:
-			listener: 
+			inputs: the PlayerInputs for each tick for the prediction 
+
+		Returns:
+			the position after each input 
 		"""
 		pass
 
 	@overload
-	def off(self, event: str, listener: IEventListener) -> bool:
-		"""Removes a IEventListener from an event.\n
-		Since: 1.2.3 
-
-		Args:
-			listener: 
-			event: 
+	def isBreakingBlock(self) -> bool:
+		"""
+		Since: 1.8.0 
 		"""
 		pass
 
 	@overload
-	def waitForEvent(self, event: str) -> FJsMacros_EventAndContext:
-		"""
-		Since: 1.5.0 
+	def predictInputs(self, inputs: List[PlayerInput], draw: bool) -> List[Pos3D]:
+		"""Predicts where each 'PlayerInput' executed in a row would lead\n
+		Since: 1.4.0 
 
 		Args:
-			event: event to wait for 
+			inputs: the PlayerInputs for each tick for the prediction 
+			draw: whether to visualize the result or not 
 
 		Returns:
-			a event and a new context if the event you're waiting for was joined, to leave it early. 
+			the position after each input 
 		"""
 		pass
 
 	@overload
-	def waitForEvent(self, event: str, filter: MethodWrapper) -> FJsMacros_EventAndContext:
-		"""
+	def moveForward(self, yaw: float) -> None:
+		"""Adds a forward movement with a relative yaw value to the MovementQueue.\n
+		Since: 1.4.0 
 
 		Args:
-			event: 
+			yaw: the relative yaw for the player 
 		"""
 		pass
 
 	@overload
-	def waitForEvent(self, event: str, filter: MethodWrapper, runBeforeWaiting: MethodWrapper) -> FJsMacros_EventAndContext:
-		"""waits for an event. if this thread is bound to an event already, this will release current lock.\n
-		Since: 1.5.0 
+	def moveBackward(self, yaw: float) -> None:
+		"""Adds a backward movement with a relative yaw value to the MovementQueue.\n
+		Since: 1.4.0 
 
 		Args:
-			filter: filter the event until it has the proper values or whatever. 
-			runBeforeWaiting: runs as a Runnable , run before waiting, this is a thread-safety thing to prevent "interrupts" from going in between this and things like deferCurrentTask 
-			event: event to wait for 
-
-		Returns:
-			a event and a new context if the event you're waiting for was joined, to leave it early. 
+			yaw: the relative yaw for the player 
 		"""
 		pass
 
 	@overload
-	def listeners(self, event: str) -> List[IEventListener]:
-		"""
-		Since: 1.2.3 
+	def moveStrafeLeft(self, yaw: float) -> None:
+		"""Adds sideways movement with a relative yaw value to the MovementQueue.\n
+		Since: 1.4.2 
 
 		Args:
-			event: 
-
-		Returns:
-			a list of script-added listeners. 
+			yaw: the relative yaw for the player 
 		"""
 		pass
 
 	@overload
-	def createCustomEvent(self, eventName: str) -> EventCustom:
-		"""create a custom event object that can trigger a event. It's recommended to use EventCustom#registerEvent() to set up the event to be visible in the GUI.\n
-		Since: 1.2.8 
+	def moveStrafeRight(self, yaw: float) -> None:
+		"""Adds sideways movement with a relative yaw value to the MovementQueue.\n
+		Since: 1.4.2 
 
 		Args:
-			eventName: name of the event. please don't use an existing one... your scripts might not like that. 
+			yaw: the relative yaw for the player 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FKeyBind.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FoodComponentHelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,84 @@
 from typing import overload
 from typing import TypeVar
 from typing import Mapping
-from typing import Set
-from .BaseLibrary import BaseLibrary
+from .BaseHelper import BaseHelper
+from .StatusEffectHelper import StatusEffectHelper
 
-InputUtil_Key = TypeVar["net.minecraft.client.util.InputUtil.Key"]
+FoodComponent = TypeVar["net.minecraft.item.FoodComponent"]
 
-class FKeyBind(BaseLibrary):
-	"""Functions for getting and modifying key pressed states.
-
-An instance of this class is passed to scripts as the 'KeyBind' variable.
+class FoodComponentHelper(BaseHelper):
+	"""
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self) -> None:
+	def __init__(self, base: FoodComponent) -> None:
 		pass
 
 	@overload
-	def getKeyCode(self, keyName: str) -> InputUtil_Key:
-		"""Dont use this one... get the raw minecraft keycode class.
-
-		Args:
-			keyName: 
+	def getHunger(self) -> int:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			the raw minecraft keycode class 
+			the amount of hunger this food restores. 
 		"""
 		pass
 
 	@overload
-	def getKeyBindings(self) -> Mapping[str, str]:
+	def getSaturation(self) -> float:
 		"""
-		Since: 1.2.2 
+		Since: 1.8.4 
 
 		Returns:
-			A Map of all the minecraft keybinds. 
+			the amount of saturation this food restores. 
 		"""
 		pass
 
 	@overload
-	def setKeyBind(self, bind: str, key: str) -> None:
-		"""Sets a minecraft keybind to the specified key.\n
-		Since: 1.2.2 
+	def isMeat(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			bind: 
-			key: 
+		Returns:
+			'true' if this food can be eaten by wolves, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def key(self, keyName: str, keyState: bool) -> None:
-		"""Set a key-state for a key.
+	def isAlwaysEdible(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			keyState: 
-			keyName: 
+		Returns:
+			'true' if this food can be eaten even when the player is not hungry, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def keyBind(self, keyBind: str, keyState: bool) -> None:
-		"""Set a key-state using the name of the keybind rather than the name of the key.
-
-This is probably the one you should use.\n
-		Since: 1.2.2 
+	def isFastFood(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			keyBind: 
-			keyState: 
+		Returns:
+			'true' if the food can be eaten faster than usual, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getPressedKeys(self) -> Set[str]:
+	def getStatusEffects(self) -> Mapping[StatusEffectHelper, Float]:
 		"""
-		Since: 1.2.6 (turned into set instead of list in 1.6.5) 
+		Since: 1.8.4 
 
 		Returns:
-			a set of currently pressed keys. 
+			a map of status effects and their respective probabilities. 
 		"""
 		pass
 
+	@overload
+	def toString(self) -> str:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FKeyBind_KeyTracker.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FKeyBind_KeyTracker.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FPlayer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Inventory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,342 +1,443 @@
 from typing import overload
 from typing import List
-from .BaseLibrary import BaseLibrary
-from .Inventory import Inventory
-from .ClientPlayerEntityHelper import ClientPlayerEntityHelper
-from .BlockDataHelper import BlockDataHelper
-from .EntityHelper import EntityHelper
-from .MethodWrapper import MethodWrapper
-from .StatsHelper import StatsHelper
-from .PlayerInput import PlayerInput
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
+from typing import TypeVar
+from typing import Mapping
+from typing import Generic
+from .ItemStackHelper import ItemStackHelper
+from .Pos2D import Pos2D
 
+T = TypeVar("T")
+Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
 
-class FPlayer(BaseLibrary):
-	"""Functions for getting and modifying the player's state.
-
-An instance of this class is passed to scripts as the 'Player' variable.
+class Inventory(Generic[T]):
+	"""
+	Since: 1.0.8 
 	"""
 
 	@overload
-	def __init__(self) -> None:
+	def create(self) -> "Inventory":
+		pass
+
+	@overload
+	def create(self, s: Screen) -> "Inventory":
 		pass
 
 	@overload
-	def openInventory(self) -> Inventory:
+	def click(self, slot: int) -> "Inventory":
 		"""
+		Since: 1.5.0 
 
-		Returns:
-			the Inventory handler 
+		Args:
+			slot: 
+		"""
+		pass
+
+	@overload
+	def click(self, slot: int, mousebutton: int) -> "Inventory":
+		"""Clicks a slot with a mouse button.~~if the slot is a container, it will click the first slot in the container\n
+		Since: 1.0.8 
+
+		Args:
+			mousebutton: 
+			slot: 
 		"""
 		pass
 
 	@overload
-	def getPlayer(self) -> ClientPlayerEntityHelper:
+	def dragClick(self, slots: List[int], mousebutton: int) -> "Inventory":
+		"""Does a drag-click with a mouse button. (the slots don't have to be in order or even adjacent, but when vanilla minecraft calls the underlying function they're always sorted...)
+
+		Args:
+			slots: 
+			mousebutton: 
 		"""
-		Since: 1.0.3 
+		pass
+
+	@overload
+	def dropSlot(self, slot: int) -> "Inventory":
+		"""
+		Since: 1.5.0 
+
+		Args:
+			slot: 
+		"""
+		pass
+
+	@overload
+	def dropSlot(self, slot: int, stack: bool) -> "Inventory":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			stack: decide whether to drop the whole stack or just a single item 
+			slot: the slot to drop 
 
 		Returns:
-			the player entity wrapper. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getGameMode(self) -> str:
+	def contains(self, item: ItemStackHelper) -> bool:
 		"""
-		Since: 1.0.9 
+		Since: 1.8.4 
+
+		Args:
+			item: the item to check for 
 
 		Returns:
-			the player's current gamemode. 
+			'true' if the item is contined anywhere in the inventory, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def rayTraceBlock(self, distance: float, fluid: bool) -> BlockDataHelper:
+	def contains(self, item: str) -> bool:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Args:
-			distance: 
-			fluid: 
+			item: the item to check for 
 
 		Returns:
-			the block/liquid the player is currently looking at. 
+			'true' if the item is contined anywhere in the inventory, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def rayTraceEntity(self) -> EntityHelper:
+	def findFreeInventorySlot(self) -> int:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Returns:
-			the entity the camera is currently looking at. 
+			the first empty slot in the main inventory or '-1' if there are no empty
+slots. 
 		"""
 		pass
 
 	@overload
-	def rayTraceEntity(self, distance: int) -> EntityHelper:
+	def findFreeHotbarSlot(self) -> int:
 		"""
-		Since: 1.8.3 
+		Since: 1.8.4 
+
+		Returns:
+			the first empty hotbar slot or '-1' if there are no empty slots. 
+		"""
+		pass
+
+	@overload
+	def findFreeSlot(self, mapIdentifiers: List[str]) -> int:
+		"""
+		Since: 1.8.4 
 
 		Args:
-			distance: 
+			mapIdentifiers: the identifier of the inventory sections to check 
+
+		Returns:
+			the first empty slot in the given inventory sections, or '-1' if there are no
+empty slots. 
+		"""
+		pass
+
+	@overload
+	def getItemCount(self) -> Mapping[str, int]:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a map of all item ids and their total count inside the inventory. 
+		"""
+		pass
+
+	@overload
+	def getItems(self) -> List[ItemStackHelper]:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			entity the player entity is currently looking at (if any). 
+			a list of all items in the inventory. 
 		"""
 		pass
 
 	@overload
-	def writeSign(self, l1: str, l2: str, l3: str, l4: str) -> bool:
-		"""Write to a sign screen if a sign screen is currently open.\n
-		Since: 1.2.2 
+	def getItems(self, mapIdentifiers: List[str]) -> List[ItemStackHelper]:
+		"""
+		Since: 1.8.4 
 
 		Args:
-			l1: 
-			l2: 
-			l3: 
-			l4: 
+			mapIdentifiers: the inventory sections 
 
 		Returns:
-			of success. 
+			a list of all items in the given inventory sections. 
 		"""
 		pass
 
 	@overload
-	def takeScreenshot(self, folder: str, callback: MethodWrapper) -> None:
+	def findItem(self, item: ItemStackHelper) -> List[int]:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
 		Args:
-			folder: 
-			callback: calls your method as a Consumer TextHelper 
+			item: the item to search for 
+
+		Returns:
+			all slots containing the given item. 
 		"""
 		pass
 
 	@overload
-	def getStatistics(self) -> StatsHelper:
+	def findItem(self, item: str) -> List[int]:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			item: the item to search for 
+
+		Returns:
+			all slots containing the given item. 
+		"""
 		pass
 
 	@overload
-	def takeScreenshot(self, folder: str, file: str, callback: MethodWrapper) -> None:
-		"""Take a screenshot and save to a file. 
-'file' is the optional one, typescript doesn't like it not being the last one that's optional\n
-		Since: 1.2.6 
+	def getSlots(self, mapIdentifiers: List[str]) -> List[int]:
+		"""
+		Since: 1.8.4 
 
 		Args:
-			folder: 
-			file: 
-			callback: calls your method as a Consumer TextHelper 
+			mapIdentifiers: the inventory sections 
+
+		Returns:
+			all slots indexes in the given inventory sections. 
+		"""
+		pass
+
+	@overload
+	def getSelectedHotbarSlotIndex(self) -> int:
+		"""
+		Since: 1.2.5 
+
+		Returns:
+			the index of the selected hotbar slot. 
 		"""
 		pass
 
 	@overload
-	def createPlayerInput(self) -> PlayerInput:
-		"""Creates a new PlayerInput object.\n
-		Since: 1.4.0 
+	def setSelectedHotbarSlotIndex(self, index: int) -> None:
+		"""
+		Since: 1.2.5 
+
+		Args:
+			index: 
 		"""
 		pass
 
 	@overload
-	def createPlayerInput(self, movementForward: float, movementSideways: float, yaw: float) -> PlayerInput:
-		"""Creates a new PlayerInput object.\n
-		Since: 1.4.0 
+	def closeAndDrop(self) -> "Inventory":
+		"""closes the inventory, (if the inventory/container is visible it will close the gui). also drops any "held on mouse" items.
 		"""
 		pass
 
 	@overload
-	def createPlayerInput(self, movementForward: float, yaw: float, jumping: bool, sprinting: bool) -> PlayerInput:
-		"""Creates a new PlayerInput object.\n
-		Since: 1.4.0 
+	def close(self) -> None:
+		"""Closes the inventory, and open gui if applicable.
 		"""
 		pass
 
 	@overload
-	def createPlayerInput(self, movementForward: float, movementSideways: float, yaw: float, pitch: float, jumping: bool, sneaking: bool, sprinting: bool) -> PlayerInput:
-		"""Creates a new PlayerInput object.\n
-		Since: 1.4.0 
+	def quick(self, slot: int) -> "Inventory":
+		"""simulates a shift-click on a slot.
+It should be safe to chain these without FClient#waitTick() at least for a bunch of the same item.
 
 		Args:
-			movementForward: 1 = forward input (W); 0 = no input; -1 = backward input (S) 
-			sprinting: sprint input 
-			jumping: jump input 
-			sneaking: sneak input 
-			pitch: pitch of the player 
-			yaw: yaw of the player 
-			movementSideways: 1 = left input (A); 0 = no input; -1 = right input (D) 
+			slot: 
 		"""
 		pass
 
 	@overload
-	def createPlayerInputsFromCsv(self, csv: str) -> List[PlayerInput]:
-		"""Parses each row of CSV string into a 'PlayerInput' .
-The capitalization of the header matters. About the columns:  
--  'movementForward' and 'movementSideways' as a number  
-- 'yaw' and 'pitch' as an absolute number  
-- 'jumping' , 'sneaking' and 'sprinting' have to be boolean   
-The separation must be a "," it's a csv...(but spaces don't matter) Quoted values don't work\n
-		Since: 1.4.0 
+	def quickAll(self, slot: int) -> int:
+		"""
+		Since: 1.7.0 
 
 		Args:
-			csv: CSV string to be parsed 
+			slot: 
 		"""
 		pass
 
 	@overload
-	def createPlayerInputsFromJson(self, json: str) -> PlayerInput:
-		"""Parses a JSON string into a 'PlayerInput' Object
-For details see 'PlayerInput.fromCsv()' , on what has to be present. Capitalization of the keys matters.\n
-		Since: 1.4.0 
+	def quickAll(self, slot: int, button: int) -> int:
+		"""quicks all that match the slot\n
+		Since: 1.7.0 
 
 		Args:
-			json: JSON string to be parsed 
+			button: 
+			slot: a slot from the section you want to move items from 
 
 		Returns:
-			The JSON parsed into a 'PlayerInput' 
+			number of items that matched 
 		"""
 		pass
 
 	@overload
-	def getCurrentPlayerInput(self) -> PlayerInput:
-		"""Creates a new 'PlayerInput' object with the current inputs of the player.\n
-		Since: 1.4.0 
+	def getHeld(self) -> ItemStackHelper:
+		"""
+
+		Returns:
+			the held (by the mouse) item. 
 		"""
 		pass
 
 	@overload
-	def addInput(self, input: PlayerInput) -> None:
-		"""Adds a new 'PlayerInput' to 'MovementQueue' to be executed\n
-		Since: 1.4.0 
+	def getSlot(self, slot: int) -> ItemStackHelper:
+		"""
 
 		Args:
-			input: the PlayerInput to be executed 
+			slot: 
+
+		Returns:
+			the item in the slot. 
 		"""
 		pass
 
 	@overload
-	def addInputs(self, inputs: List[PlayerInput]) -> None:
-		"""Adds multiple new 'PlayerInput' to 'MovementQueue' to be executed\n
-		Since: 1.4.0 
+	def getTotalSlots(self) -> int:
+		"""
 
-		Args:
-			inputs: the PlayerInputs to be executed 
+		Returns:
+			the size of the container/inventory. 
 		"""
 		pass
 
 	@overload
-	def clearInputs(self) -> None:
-		"""Clears all inputs in the 'MovementQueue'\n
-		Since: 1.4.0 
+	def split(self, slot1: int, slot2: int) -> "Inventory":
+		"""Splits the held stack into two slots. can be alternatively done with Inventory#dragClick(int[],int) if this one has issues on some servers.
+
+		Args:
+			slot2: 
+			slot1: 
 		"""
 		pass
 
 	@overload
-	def setDrawPredictions(self, val: bool) -> None:
+	def grabAll(self, slot: int) -> "Inventory":
+		"""Does that double click thingy to turn a incomplete stack pickup into a complete stack pickup if you have more in your inventory.
+
+		Args:
+			slot: 
+		"""
 		pass
 
 	@overload
-	def predictInput(self, input: PlayerInput) -> PositionCommon_Pos3D:
-		"""Predicts where one tick with a 'PlayerInput' as input would lead to.\n
-		Since: 1.4.0 
+	def swap(self, slot1: int, slot2: int) -> "Inventory":
+		"""swaps the items in two slots.
 
 		Args:
-			input: the PlayerInput for the prediction 
-
-		Returns:
-			the position after the input 
+			slot2: 
+			slot1: 
 		"""
 		pass
 
 	@overload
-	def predictInput(self, input: PlayerInput, draw: bool) -> PositionCommon_Pos3D:
-		"""Predicts where one tick with a 'PlayerInput' as input would lead to.\n
-		Since: 1.4.0 
+	def swapHotbar(self, slot: int, hotbarSlot: int) -> "Inventory":
+		"""equivalent to hitting the numbers or f for swapping slots to hotbar\n
+		Since: 1.6.5 [citation needed] 
 
 		Args:
-			input: the PlayerInput for the prediction 
-			draw: whether to visualize the result or not 
+			hotbarSlot: 0-8 or 40 for offhand 
+			slot: 
+		"""
+		pass
 
-		Returns:
-			the position after the input 
+	@overload
+	def openGui(self) -> None:
+		"""
+		Since: 1.2.8 
 		"""
 		pass
 
 	@overload
-	def predictInputs(self, inputs: List[PlayerInput]) -> List[PositionCommon_Pos3D]:
-		"""Predicts where each 'PlayerInput' executed in a row would lead
-without drawing it.\n
-		Since: 1.4.0 
+	def getSlotUnderMouse(self) -> int:
+		"""
+		Since: 1.1.3 
 
-		Args:
-			inputs: the PlayerInputs for each tick for the prediction 
+		Returns:
+			the id of the slot under the mouse. 
+		"""
+		pass
+
+	@overload
+	def getType(self) -> str:
+		"""
+		Since: 1.1.3 
 
 		Returns:
-			the position after each input 
+			the part of the mapping the slot is in. 
 		"""
 		pass
 
 	@overload
-	def isBreakingBlock(self) -> bool:
+	def getMap(self) -> Mapping[str, List[int]]:
 		"""
-		Since: 1.8.0 
+		Since: 1.1.3 
+
+		Returns:
+			the inventory mappings different depending on the type of open container/inventory. 
 		"""
 		pass
 
 	@overload
-	def predictInputs(self, inputs: List[PlayerInput], draw: bool) -> List[PositionCommon_Pos3D]:
-		"""Predicts where each 'PlayerInput' executed in a row would lead\n
-		Since: 1.4.0 
+	def getLocation(self, slotNum: int) -> str:
+		"""
+		Since: 1.1.3 
 
 		Args:
-			inputs: the PlayerInputs for each tick for the prediction 
-			draw: whether to visualize the result or not 
+			slotNum: 
 
 		Returns:
-			the position after each input 
+			returns the part of the mapping the slot is in. 
 		"""
 		pass
 
 	@overload
-	def moveForward(self, yaw: float) -> None:
-		"""Adds a forward movement with a relative yaw value to the MovementQueue.\n
-		Since: 1.4.0 
+	def getSlotPos(self, slot: int) -> Pos2D:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			yaw: the relative yaw for the player 
+		Returns:
+			the x/y position of the specified slot index 
 		"""
 		pass
 
 	@overload
-	def moveBackward(self, yaw: float) -> None:
-		"""Adds a backward movement with a relative yaw value to the MovementQueue.\n
-		Since: 1.4.0 
+	def isContainer(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			yaw: the relative yaw for the player 
+		Returns:
+			'true' if the inventory is a container, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def moveStrafeLeft(self, yaw: float) -> None:
-		"""Adds sideways movement with a relative yaw value to the MovementQueue.\n
-		Since: 1.4.2 
-
-		Args:
-			yaw: the relative yaw for the player 
+	def getContainerTitle(self) -> str:
+		"""
+		Since: 1.2.3 
 		"""
 		pass
 
 	@overload
-	def moveStrafeRight(self, yaw: float) -> None:
-		"""Adds sideways movement with a relative yaw value to the MovementQueue.\n
-		Since: 1.4.2 
+	def getRawContainer(self) -> T:
+		pass
 
-		Args:
-			yaw: the relative yaw for the player 
+	@overload
+	def toString(self) -> str:
+		pass
+
+	@overload
+	def getCurrentSyncId(self) -> int:
+		"""
+		Since: 1.6.0 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FReflection.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FReflection.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from .ClassBuilder import ClassBuilder
 from .LibraryBuilder import LibraryBuilder
 from .Mappings import Mappings
 from .WrappedClassInstance import WrappedClassInstance
 
 Field = TypeVar["java.lang.reflect.Field"]
 T = TypeVar("T")
+Reflect = TypeVar["org.joor.Reflect"]
 Method = TypeVar["java.lang.reflect.Method"]
 
 class FReflection(PerExecLibrary):
-	"""Functions for getting and using raw java classes, methods and functions.
-
+	"""Functions for getting and using raw java classes, methods and functions. 
 An instance of this class is passed to scripts as the 'Reflection' variable.\n
 	Since: 1.2.3 
 	"""
 	classLoader: FReflection_CombinedVariableClassLoader
 
 	@overload
 	def __init__(self, context: BaseScriptContext) -> None:
@@ -168,15 +168,15 @@
 		"""
 		pass
 
 	@overload
 	def newInstance(self, c: Class, objects: List[object]) -> T:
 		"""Attempts to create a new instance of a class. You probably don't have to use this one and can just call '
 new' on a Class unless you're in LUA, but then you also have the (kinda poorly
-doccumented, can someone find a better docs link for me) LuaJava Library .\n
+documented, can someone find a better docs link for me) LuaJava Library .\n
 		Since: 1.2.7 
 
 		Args:
 			c: 
 			objects: 
 		"""
 		pass
@@ -217,14 +217,83 @@
 		pass
 
 	@overload
 	def createLibraryBuilder(self, name: str, perExec: bool, acceptedLangs: List[str]) -> LibraryBuilder:
 		pass
 
 	@overload
+	def createLibrary(self, className: str, javaCode: str) -> None:
+		"""A library class always has a Library annotation containing the name of the library,
+which may differ from the actual class name. A library class must also extend BaseLibrary in some way, either directly or through PerExecLibrary , PerExecLanguageLibrary or PerLanguageLibrary .\n
+		Since: 1.8.4 
+
+		Args:
+			javaCode: the source code of the library 
+			className: the fully qualified name of the class, including the package 
+		"""
+		pass
+
+	@overload
+	def compileJavaClass(self, className: str, code: str) -> Class:
+		"""A Java Development Kit (JDK) must be installed (and potentially used to start Minecraft) in
+order to compile whole classes. 
+Compiled classes can't be accessed from any guest language, but must be either stored through FGlobalVars#putObject(java.lang.String,java.lang.Object) or retrieved from this library. Unlike normal
+hot swapping, already created instances of the class will not be updated. Thus, it's
+important to know which version of the class you're using when instantiating it.\n
+		Since: 1.8.4 
+
+		Args:
+			code: the java code to compile 
+			className: the fully qualified name of the class, including the package 
+
+		Returns:
+			the compiled class. 
+		"""
+		pass
+
+	@overload
+	def getCompiledJavaClass(self, className: str) -> Class:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			className: the fully qualified name of the class, including the package 
+
+		Returns:
+			the latest compiled class or 'null' if it doesn't exist. 
+		"""
+		pass
+
+	@overload
+	def getAllCompiledJavaClassVersions(self, className: str) -> List[Class]:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			className: the fully qualified name of the class, including the package 
+
+		Returns:
+			all compiled versions of the class, in order of compilation. 
+		"""
+		pass
+
+	@overload
+	def getReflect(self, obj: object) -> Reflect:
+		"""See jOOR Github for more information.\n
+		Since: 1.8.4 
+
+		Args:
+			obj: the object to wrap 
+
+		Returns:
+			a wrapper for the passed object to do help with java reflection. 
+		"""
+		pass
+
+	@overload
 	def loadJarFile(self, file: str) -> bool:
 		"""Loads a jar file to be accessible with this library.\n
 		Since: 1.2.6 
 
 		Args:
 			file: relative to the script's folder.
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FReflection_CombinedVariableClassLoader.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FReflection_CombinedVariableClassLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from typing import TypeVar
 
 File = TypeVar["java.io.File"]
 
 class FReflection_CombinedVariableClassLoader(ClassLoader):
 	"""I know this is probably bad practice, but lets be real, this whole library is bad practice, So I can make it
 worse, right? at least this should work better than 'try/catch' 'ing using ClassLoader#loadClass(java.lang.String) to search through every URLClassLoader that FReflection#loadJarFile(java.lang.String) would make, or how I was previously doing it by pre-loading and caching
-all the classes to a Map This class is a modification to Christian d'Heureuse's JoinClassLoader , under the Apache-2.0 license to change it from a Class array to a Set , to allow for modifications to the ClassLoader contained in the classLoader.\n
+all the classes to a Map  
+This class is a modification to Christian d'Heureuse's JoinClassLoader , under the Apache-2.0 license to change it from a Class array to a Set , to allow for modifications to the ClassLoader contained in the classLoader.\n
 	Since: 1.2.8 
 	"""
 
 	@overload
 	def __init__(self, parent: ClassLoader) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FRequest.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from .BaseLibrary import BaseLibrary
 from .HTTPRequest import HTTPRequest
 from .HTTPRequest_Response import HTTPRequest_Response
 from .Websocket import Websocket
 
 
 class FRequest(BaseLibrary):
-	"""Functions for getting and using raw java classes, methods and functions.
-
+	"""Functions for getting and using raw java classes, methods and functions. 
 An instance of this class is passed to scripts as the 'Request' variable.\n
 	Since: 1.1.8 
 	"""
 
 	@overload
 	def __init__(self) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FTime.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FTime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import overload
 from .PerExecLibrary import PerExecLibrary
 from .BaseScriptContext import BaseScriptContext
 
 
 class FTime(PerExecLibrary):
-	"""Functions for getting and using raw java classes, methods and functions.
-
+	"""Functions for getting and using raw java classes, methods and functions. 
 An instance of this class is passed to scripts as the 'Time' variable.
 	"""
 
 	@overload
 	def __init__(self, context: BaseScriptContext) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileChooser.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MultiElementContainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
+from typing import Generic
+from .IContainerParent import IContainerParent
 from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
-from .FileChooser_fileObj import FileChooser_fileObj
 
-Consumer = TypeVar["java.util.function.Consumer_java.io.File_"]
+T = TypeVar("T")
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-File = TypeVar["java.io.File"]
+Element = TypeVar["net.minecraft.client.gui.Element"]
+ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class FileChooser(OverlayContainer):
-	root: File
+class MultiElementContainer(IContainerParent, Generic[T]):
+	parent: T
+	x: int
+	y: int
+	width: int
+	height: int
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, directory: File, selected: File, parent: IOverlayParent, setFile: Consumer, editFile: Consumer) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: T) -> None:
 		pass
 
 	@overload
-	def setDir(self, dir: File) -> None:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def selectFile(self, f: File) -> None:
+	def getVisible(self) -> bool:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def setVisible(self, visible: bool) -> None:
+		pass
+
+	@overload
+	def addDrawableChild(self, drawableElement: T) -> T:
 		pass
 
 	@overload
-	def addFile(self, f: File) -> None:
+	def getButtons(self) -> List[ClickableWidget]:
 		pass
 
 	@overload
-	def addFile(self, f: File, btnText: str) -> None:
+	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def updateFilePos(self) -> None:
+	def openOverlay(self, overlay: OverlayContainer) -> None:
 		pass
 
 	@overload
-	def confirmDelete(self, f: FileChooser_fileObj) -> None:
+	def openOverlay(self, overlay: OverlayContainer, disableButtons: bool) -> None:
 		pass
 
 	@overload
-	def delete(self, f: FileChooser_fileObj) -> None:
+	def remove(self, button: Element) -> None:
 		pass
 
 	@overload
-	def onScrollbar(self, page: float) -> None:
+	def getFirstOverlayParent(self) -> IOverlayParent:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringField.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-File = TypeVar["java.io.File"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class FileField(AbstractSettingField):
+class StringField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
-	def getTopLevel(self, setting: SettingsOverlay_SettingField) -> File:
-		pass
-
-	@overload
-	def relativize(self, setting: SettingsOverlay_SettingField, file: File) -> str:
-		pass
-
-	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileHandler.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TropicalFishEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,68 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
+from .FishEntityHelper import FishEntityHelper
 
-File = TypeVar["java.io.File"]
+TropicalFishEntity = TypeVar["net.minecraft.entity.passive.TropicalFishEntity"]
 
-class FileHandler:
+class TropicalFishEntityHelper(FishEntityHelper):
 	"""
-	Since: 1.1.8 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, path: str) -> None:
+	def __init__(self, base: TropicalFishEntity) -> None:
 		pass
 
 	@overload
-	def __init__(self, path: File) -> None:
-		pass
-
-	@overload
-	def write(self, s: str) -> "FileHandler":
-		"""writes a string to the file. this is a destructive operation that replaces the file contents.\n
-		Since: 1.1.8 
-
-		Args:
-			s: 
+	def getVariant(self) -> str:
 		"""
-		pass
-
-	@overload
-	def write(self, b: List[float]) -> "FileHandler":
-		"""writes a byte array to the file. this is a destructive operation that replaces the file contents.\n
-		Since: 1.1.8 
+		Since: 1.8.4 
 
-		Args:
-			b: 
+		Returns:
+			the variant of this tropical fish. 
 		"""
 		pass
 
 	@overload
-	def read(self) -> str:
-		"""
-		Since: 1.1.8 
+	def getSize(self) -> str:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def readBytes(self) -> List[float]:
-		"""
-		Since: 1.2.6 
+		Returns:
+			the size of this tropical fish's variant. 
 		"""
 		pass
 
 	@overload
-	def append(self, s: str) -> "FileHandler":
+	def getBaseColor(self) -> int:
 		"""
-		Since: 1.1.8 
+		Since: 1.8.4 
 
-		Args:
-			s: 
+		Returns:
+			the base color of this tropical fish's pattern. 
 		"""
 		pass
 
 	@overload
-	def append(self, b: List[float]) -> "FileHandler":
+	def getPatternColor(self) -> int:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
-		Args:
-			b: 
+		Returns:
+			the pattern color of this tropical fish's pattern. 
 		"""
 		pass
 
 	@overload
-	def getFile(self) -> File:
-		pass
+	def getVarietyId(self) -> int:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def toString(self) -> str:
+		Returns:
+			the id of this tropical fish's variant. 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileMapSetting.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileMapSetting.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FileMapSetting_FileEntry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FileMapSetting_FileEntry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/FloatField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FloatField.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/GroupFilter.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/GroupFilter.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/HTTPRequest.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/HTTPRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import overload
+from typing import List
 from typing import Mapping
 from .HTTPRequest_Response import HTTPRequest_Response
 
 
 class HTTPRequest:
 	"""
 	Since: 1.1.8 
@@ -38,10 +39,62 @@
 		Since: 1.1.8 
 
 		Args:
 			data: 
 		"""
 		pass
 
+	@overload
+	def post(self, data: List[float]) -> HTTPRequest_Response:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			data: 
+		"""
+		pass
+
+	@overload
+	def put(self, data: str) -> HTTPRequest_Response:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			data: 
+		"""
+		pass
+
+	@overload
+	def put(self, data: List[float]) -> HTTPRequest_Response:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			data: 
+		"""
+		pass
+
+	@overload
+	def send(self, method: str, data: str) -> HTTPRequest_Response:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			method: 
+			data: 
+		"""
+		pass
+
+	@overload
+	def send(self, method: str, data: List[float]) -> HTTPRequest_Response:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			method: 
+			data: 
+		"""
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/HTTPRequest_Response.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/HTTPRequest_Response.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/History.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/History.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/IChatHud.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/IChatHud.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/IContainerParent.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/IContainerParent.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/IDraw2D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/IDraw2D.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from .RenderCommon_Text import RenderCommon_Text
-from .RenderCommon_Rect import RenderCommon_Rect
-from .RenderCommon_Item import RenderCommon_Item
-from .RenderCommon_Image import RenderCommon_Image
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
+from .Text import Text
+from .Rect import Rect
+from .Line import Line
+from .Item import Item
+from .Image import Image
+from .Draw2DElement import Draw2DElement
+from .RenderElement import RenderElement
 from .TextHelper import TextHelper
 from .ItemStackHelper import ItemStackHelper
+from .Draw2D import Draw2D
+from .Item_Builder import Item_Builder
+from .Image_Builder import Image_Builder
+from .Rect_Builder import Rect_Builder
+from .Line_Builder import Line_Builder
+from .Text_Builder import Text_Builder
+from .Draw2DElement_Builder import Draw2DElement_Builder
 from .MethodWrapper import MethodWrapper
 
 T = TypeVar("T")
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 
 class IDraw2D:
 	"""
@@ -35,85 +44,105 @@
 
 		Returns:
 			screen height 
 		"""
 		pass
 
 	@overload
-	def getTexts(self) -> List[RenderCommon_Text]:
+	def getTexts(self) -> List[Text]:
 		"""
 		Since: 1.2.7 
 
 		Returns:
 			text elements 
 		"""
 		pass
 
 	@overload
-	def getRects(self) -> List[RenderCommon_Rect]:
+	def getRects(self) -> List[Rect]:
 		"""
 		Since: 1.2.7 
 
 		Returns:
 			rect elements 
 		"""
 		pass
 
 	@overload
-	def getItems(self) -> List[RenderCommon_Item]:
+	def getLines(self) -> List[Line]:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			all registered line elements. 
+		"""
+		pass
+
+	@overload
+	def getItems(self) -> List[Item]:
 		"""
 		Since: 1.2.7 
 
 		Returns:
 			item elements 
 		"""
 		pass
 
 	@overload
-	def getImages(self) -> List[RenderCommon_Image]:
+	def getImages(self) -> List[Image]:
 		"""
 		Since: 1.2.7 
 
 		Returns:
 			image elements 
 		"""
 		pass
 
 	@overload
-	def getElements(self) -> List[RenderCommon_RenderElement]:
+	def getDraw2Ds(self) -> List[Draw2DElement]:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			all registered draw2d elements. 
+		"""
+		pass
+
+	@overload
+	def getElements(self) -> List[RenderElement]:
 		"""
 		Since: 1.2.9 
 
 		Returns:
 			a read only copy of the list of all elements added by scripts. 
 		"""
 		pass
 
 	@overload
-	def removeElement(self, e: RenderCommon_RenderElement) -> T:
+	def removeElement(self, e: RenderElement) -> T:
 		"""removes any element regardless of type.\n
 		Since: 1.2.9 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def reAddElement(self, e: RenderCommon_RenderElement) -> RenderCommon_RenderElement:
-		"""re-add an element you removed with IDraw2D#removeElement(xyz.wagyourtail.jsmacros.client.api.sharedclasses.RenderCommon.RenderElement)\n
+	def reAddElement(self, e: T) -> T:
+		"""re-add an element you removed with IDraw2D#removeElement(xyz.wagyourtail.jsmacros.client.api.classes.render.components.RenderElement)\n
 		Since: 1.2.9 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, shadow: bool) -> Text:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			x: screen x 
@@ -122,15 +151,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool) -> Text:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			x: screen x 
@@ -140,15 +169,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> Text:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			rotation: text rotation (as degrees) 
@@ -159,15 +188,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> Text:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			rotation: text rotation (as degrees) 
@@ -179,15 +208,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool) -> Text:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			x: screen x 
@@ -196,15 +225,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool) -> Text:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			x: screen x 
@@ -214,15 +243,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, shadow: bool, scale: float, rotation: float) -> Text:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			rotation: text rotation (as degrees) 
@@ -233,15 +262,15 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> RenderCommon_Text:
+	def addText(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> Text:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			color: text color 
 			shadow: include shadow layer 
 			rotation: text rotation (as degrees) 
@@ -253,28 +282,28 @@
 
 		Returns:
 			added text 
 		"""
 		pass
 
 	@overload
-	def removeText(self, t: RenderCommon_Text) -> T:
+	def removeText(self, t: Text) -> T:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			t: 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> Image:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			imageY: the top-most coordinate of the texture region 
 			textureWidth: the width of the entire texture 
 			imageX: the left-most coordinate of the texture region 
@@ -289,15 +318,15 @@
 
 		Returns:
 			added image 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> Image:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			imageY: the top-most coordinate of the texture region 
 			textureWidth: the width of the entire texture 
 			imageX: the left-most coordinate of the texture region 
@@ -313,23 +342,23 @@
 
 		Returns:
 			added image 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			imageY: the top-most coordinate of the texture region 
 			textureWidth: the width of the entire texture 
 			imageX: the left-most coordinate of the texture region 
-			rotation: the rotation of the texture (as degrees) 
+			rotation: the rotation (clockwise) of the texture (as degrees) 
 			x: screen x, top left corner 
 			width: width on screen 
 			y: screen y, top left corner 
 			regionHeight: the height the texture region 
 			id: image id, in the form 'minecraft:textures' path'd as found in texture packs, ie 'assets/minecraft/textures/gui/recipe_book.png' becomes 'minecraft:textures/gui/recipe_book.png' 
 			regionWidth: the width the texture region 
 			textureHeight: the height of the entire texture 
@@ -337,23 +366,23 @@
 
 		Returns:
 			added image 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			imageY: the top-most coordinate of the texture region 
 			textureWidth: the width of the entire texture 
 			imageX: the left-most coordinate of the texture region 
-			rotation: the rotation of the texture (as degrees) 
+			rotation: the rotation (clockwise) of the texture (as degrees) 
 			regionWidth: the width the texture region 
 			textureHeight: the height of the entire texture 
 			x: screen x, top left corner 
 			width: width on screen 
 			y: screen y, top left corner 
 			regionHeight: the height the texture region 
 			id: image id, in the form 'minecraft:textures' path'd as found in texture packs, ie 'assets/minecraft/textures/gui/recipe_book.png' becomes 'minecraft:textures/gui/recipe_book.png' 
@@ -362,15 +391,15 @@
 
 		Returns:
 			added image 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			color: 
 			imageY: 
 			textureWidth: 
@@ -385,15 +414,15 @@
 			id: 
 			height: 
 			zIndex: 
 		"""
 		pass
 
 	@overload
-	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, alpha: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> RenderCommon_Image:
+	def addImage(self, x: int, y: int, width: int, height: int, zIndex: int, alpha: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> Image:
 		"""
 		Since: 1.6.5 
 
 		Args:
 			color: 
 			imageY: 
 			textureWidth: 
@@ -409,28 +438,28 @@
 			id: 
 			height: 
 			zIndex: 
 		"""
 		pass
 
 	@overload
-	def removeImage(self, i: RenderCommon_Image) -> T:
+	def removeImage(self, i: Image) -> T:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			i: 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int) -> Rect:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: as hex, with alpha channel 
 			y1: 
 			x1: 
@@ -439,15 +468,15 @@
 
 		Returns:
 			added rect 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int) -> Rect:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: as hex 
 			alpha: alpha channel 0-255 
 			y1: 
@@ -457,15 +486,15 @@
 
 		Returns:
 			added rect 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float) -> Rect:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			color: as hex 
 			alpha: alpha channel 0-255 
 			rotation: as degrees 
@@ -476,15 +505,15 @@
 
 		Returns:
 			added rect 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float, zIndex: int) -> RenderCommon_Rect:
+	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float, zIndex: int) -> Rect:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			color: as hex 
 			alpha: alpha channel 0-255 
 			rotation: as degrees 
@@ -496,43 +525,167 @@
 
 		Returns:
 			added rect 
 		"""
 		pass
 
 	@overload
-	def removeRect(self, r: RenderCommon_Rect) -> T:
+	def removeRect(self, r: Rect) -> T:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			r: 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str) -> RenderCommon_Item:
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int) -> Line:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			color: the color of the line, can include alpha value 
+			y1: the y position of the start 
+			x1: the x position of the start 
+			y2: the y position of the end 
+			x2: the x position of the end 
+
+		Returns:
+			the added line. 
+		"""
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, zIndex: int) -> Line:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			color: the color of the line, can include alpha value 
+			y1: the y position of the start 
+			x1: the x position of the start 
+			y2: the y position of the end 
+			x2: the x position of the end 
+			zIndex: the z-index of the line 
+
+		Returns:
+			the added line. 
+		"""
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, width: float) -> Line:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			color: the color of the line, can include alpha value 
+			y1: the y position of the start 
+			width: the width of the line 
+			x1: the x position of the start 
+			y2: the y position of the end 
+			x2: the x position of the end 
+
+		Returns:
+			the added line. 
+		"""
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, zIndex: int, width: float) -> Line:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			color: the color of the line, can include alpha value 
+			y1: the y position of the start 
+			width: the width of the line 
+			x1: the x position of the start 
+			y2: the y position of the end 
+			x2: the x position of the end 
+			zIndex: the z-index of the line 
+
+		Returns:
+			the added line. 
+		"""
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, width: float, rotation: float) -> Line:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			color: the color of the line, can include alpha value 
+			rotation: the rotation (clockwise) of the line (as degrees) 
+			y1: the y position of the start 
+			width: the width of the line 
+			x1: the x position of the start 
+			y2: the y position of the end 
+			x2: the x position of the end 
+
+		Returns:
+			the added line. 
+		"""
+		pass
+
+	@overload
+	def addLine(self, x1: int, y1: int, x2: int, y2: int, color: int, zIndex: int, width: float, rotation: float) -> Line:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			color: the color of the line, can include alpha value 
+			rotation: the rotation (clockwise) of the line (as degrees) 
+			y1: the y position of the start 
+			width: the width of the line 
+			x1: the x position of the start 
+			y2: the y position of the end 
+			x2: the x position of the end 
+			zIndex: the z-index of the line 
+
+		Returns:
+			the added line. 
+		"""
+		pass
+
+	@overload
+	def removeLine(self, l: Line) -> T:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			l: the line to remove 
+
+		Returns:
+			self chaining. 
+		"""
+		pass
+
+	@overload
+	def addItem(self, x: int, y: int, id: str) -> Item:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			x: left most corner 
 			y: top most corner 
 			id: item id 
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, id: str) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, id: str) -> Item:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			x: left most corner 
 			y: top most corner 
 			id: item id 
@@ -540,15 +693,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, id: str, overlay: bool) -> Item:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			overlay: should include overlay health and count 
 			x: left most corner 
 			y: top most corner 
@@ -556,15 +709,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool) -> Item:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			overlay: should include overlay health and count 
 			x: left most corner 
 			y: top most corner 
@@ -573,15 +726,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, id: str, overlay: bool, scale: float, rotation: float) -> Item:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			overlay: should include overlay health and count 
 			rotation: rotation of item 
 			x: left most corner 
@@ -591,15 +744,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, id: str, overlay: bool, scale: float, rotation: float) -> Item:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			overlay: should include overlay health and count 
 			rotation: rotation of item 
 			x: left most corner 
@@ -610,30 +763,30 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, item: ItemStackHelper) -> Item:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			item: from inventory as helper 
 			x: left most corner 
 			y: top most corner 
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper) -> Item:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			item: from inventory as helper 
 			x: left most corner 
 			y: top most corner 
@@ -641,15 +794,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool) -> Item:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			item: from inventory as helper 
 			overlay: should include overlay health and count 
 			x: left most corner 
@@ -657,15 +810,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool) -> Item:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			item: from inventory as helper 
 			overlay: should include overlay health and count 
 			x: left most corner 
@@ -674,15 +827,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> Item:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			item: from inventory as helper 
 			overlay: should include overlay health and count 
 			rotation: rotation of item 
@@ -692,15 +845,15 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def addItem(self, x: int, y: int, zIndex: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> Item:
 		"""
 		Since: 1.4.0 
 
 		Args:
 			item: from inventory as helper 
 			overlay: should include overlay health and count 
 			rotation: rotation of item 
@@ -711,27 +864,222 @@
 
 		Returns:
 			added item 
 		"""
 		pass
 
 	@overload
-	def removeItem(self, i: RenderCommon_Item) -> T:
+	def removeItem(self, i: Item) -> T:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			i: 
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
+	def addDraw2D(self, draw2D: Draw2D, x: int, y: int, width: int, height: int) -> Draw2DElement:
+		"""Tries to add the given draw2d as a child. Fails if cyclic dependencies are detected.\n
+		Since: 1.8.4 
+
+		Args:
+			x: the x position on this draw2d 
+			width: the width of the given draw2d 
+			y: the y position on this draw2d 
+			draw2D: the draw2d to add 
+			height: the height of the given draw2d 
+
+		Returns:
+			a wrapper for the draw2d. 
+		"""
+		pass
+
+	@overload
+	def addDraw2D(self, draw2D: Draw2D, x: int, y: int, width: int, height: int, zIndex: int) -> Draw2DElement:
+		"""Tries to add the given draw2d as a child. Fails if cyclic dependencies are detected.\n
+		Since: 1.8.4 
+
+		Args:
+			x: the x position on this draw2d 
+			width: the width of the given draw2d 
+			y: the y position on this draw2d 
+			draw2D: the draw2d to add 
+			height: the height of the given draw2d 
+			zIndex: the z-index for the draw2d 
+
+		Returns:
+			a wrapper for the draw2d. 
+		"""
+		pass
+
+	@overload
+	def removeDraw2D(self, draw2D: Draw2DElement) -> T:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			draw2D: the draw2d to remove 
+
+		Returns:
+			self chaining. 
+		"""
+		pass
+
+	@overload
+	def itemBuilder(self) -> Item_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a builder for an Item . 
+		"""
+		pass
+
+	@overload
+	def itemBuilder(self, item: ItemStackHelper) -> Item_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			item: the item to use 
+
+		Returns:
+			a builder for an Item . 
+		"""
+		pass
+
+	@overload
+	def imageBuilder(self) -> Image_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a builder for an Image . 
+		"""
+		pass
+
+	@overload
+	def imageBuilder(self, id: str) -> Image_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			id: the id of the image 
+
+		Returns:
+			a builder for an Image . 
+		"""
+		pass
+
+	@overload
+	def rectBuilder(self) -> Rect_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a builder for a Rect . 
+		"""
+		pass
+
+	@overload
+	def rectBuilder(self, x: int, y: int, width: int, height: int) -> Rect_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			x: the x position of the rectangle 
+			width: the width of the rectangle 
+			y: the y position of the rectangle 
+			height: the height of the rectangle 
+
+		Returns:
+			a builder for a Rect . 
+		"""
+		pass
+
+	@overload
+	def lineBuilder(self) -> Line_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a builder for a Line . 
+		"""
+		pass
+
+	@overload
+	def lineBuilder(self, x1: int, y1: int, x2: int, y2: int) -> Line_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			y1: the y position of the first point 
+			x1: the x position of the first point 
+			y2: the y position of the second point 
+			x2: the x position of the second point 
+
+		Returns:
+			a builder for a Line . 
+		"""
+		pass
+
+	@overload
+	def textBuilder(self) -> Text_Builder:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			a builder for a Text . 
+		"""
+		pass
+
+	@overload
+	def textBuilder(self, text: str) -> Text_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			text: the text to display 
+
+		Returns:
+			a builder for a Text . 
+		"""
+		pass
+
+	@overload
+	def textBuilder(self, text: TextHelper) -> Text_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			text: the text to display 
+
+		Returns:
+			a builder for a Text . 
+		"""
+		pass
+
+	@overload
+	def draw2DBuilder(self, draw2D: Draw2D) -> Draw2DElement_Builder:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			draw2D: the draw2d to add 
+
+		Returns:
+			a builder for a Draw2D . 
+		"""
+		pass
+
+	@overload
 	def setOnInit(self, onInit: MethodWrapper) -> T:
 		"""
 		Since: 1.2.7 
 
 		Args:
 			onInit: calls your method as a Consumer IDraw2D#T 
 
@@ -750,18 +1098,35 @@
 
 		Returns:
 			self for chaining 
 		"""
 		pass
 
 	@overload
-	def render(self, matrixStack: MatrixStack) -> None:
+	def render(self, drawContext: MatrixStack) -> None:
 		"""internal
 
 		Args:
-			matrixStack: 
+			drawContext: 
+		"""
+		pass
+
+	@overload
+	def setZIndex(self, zIndex: int) -> None:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			zIndex: 
+		"""
+		pass
+
+	@overload
+	def getZIndex(self) -> int:
+		"""
+		Since: 1.8.4 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/IFWrapper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/IFWrapper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/IScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Text_Builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,293 +1,350 @@
 from typing import overload
-from typing import List
-from typing import TypeVar
+from .Alignable import Alignable
+from .RenderElementBuilder import RenderElementBuilder
 from .IDraw2D import IDraw2D
-from .ButtonWidgetHelper import ButtonWidgetHelper
-from .TextFieldWidgetHelper import TextFieldWidgetHelper
-from .MethodWrapper import MethodWrapper
-from .RenderCommon_Rect import RenderCommon_Rect
-from .RenderCommon_Item import RenderCommon_Item
-from .ItemStackHelper import ItemStackHelper
+from .TextHelper import TextHelper
+from .TextBuilder import TextBuilder
+from .Text import Text
 
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 
-class IScreen(IDraw2D):
+class Text_Builder(Alignable, RenderElementBuilder):
 	"""
-	Since: 1.2.7 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def getScreenClassName(self) -> str:
-		"""
-		Since: 1.2.7 
-		"""
+	def __init__(self, draw2D: IDraw2D) -> None:
 		pass
 
 	@overload
-	def getTitleText(self) -> str:
+	def text(self, text: TextHelper) -> "Text_Builder":
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
+
+		Args:
+			text: the content of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getButtonWidgets(self) -> List[ButtonWidgetHelper]:
-		"""in '1.3.1' updated to work with all button widgets not just ones added by scripts.\n
-		Since: 1.0.5 
+	def text(self, text: TextBuilder) -> "Text_Builder":
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getTextFields(self) -> List[TextFieldWidgetHelper]:
-		"""in '1.3.1' updated to work with all text fields not just ones added by scripts.\n
-		Since: 1.0.5 
+		Args:
+			text: the content of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addButton(self, x: int, y: int, width: int, height: int, text: str, callback: MethodWrapper) -> ButtonWidgetHelper:
+	def text(self, text: str) -> "Text_Builder":
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Args:
-			x: 
-			width: 
-			y: 
-			callback: calls your method as a Consumer ButtonWidgetHelper 
-			text: 
-			height: 
+			text: the content of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addButton(self, x: int, y: int, width: int, height: int, zIndex: int, text: str, callback: MethodWrapper) -> ButtonWidgetHelper:
+	def getText(self) -> TextHelper:
 		"""
-		Since: 1.4.0 
+		Since: 1.8.4 
 
-		Args:
-			x: 
-			width: 
-			y: 
-			callback: calls your method as a Consumer ButtonWidgetHelper 
-			text: 
-			height: 
-			zIndex: 
+		Returns:
+			the content of the text element. 
 		"""
 		pass
 
 	@overload
-	def removeButton(self, btn: ButtonWidgetHelper) -> "IScreen":
+	def x(self, x: int) -> "Text_Builder":
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Args:
-			btn: 
+			x: the x position of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addTextInput(self, x: int, y: int, width: int, height: int, message: str, onChange: MethodWrapper) -> TextFieldWidgetHelper:
+	def getX(self) -> int:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			onChange: calls your method as a Consumer String 
-			x: 
-			width: 
-			y: 
-			message: 
-			height: 
+		Returns:
+			the x position of the text element. 
 		"""
 		pass
 
 	@overload
-	def addTextInput(self, x: int, y: int, width: int, height: int, zIndex: int, message: str, onChange: MethodWrapper) -> TextFieldWidgetHelper:
+	def y(self, y: int) -> "Text_Builder":
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Args:
-			onChange: calls your method as a Consumer String 
-			x: 
-			width: 
-			y: 
-			message: 
-			height: 
-			zIndex: 
+			y: the y position of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def removeTextInput(self, inp: TextFieldWidgetHelper) -> "IScreen":
+	def getY(self) -> int:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			inp: 
+		Returns:
+			the y position of the text element. 
 		"""
 		pass
 
 	@overload
-	def setOnMouseDown(self, onMouseDown: MethodWrapper) -> "IScreen":
+	def pos(self, x: int, y: int) -> "Text_Builder":
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Args:
-			onMouseDown: calls your method as a BiConsumer PositionCommon_Pos2D , Integer 
+			x: the x position of the text element 
+			y: the y position of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setOnMouseDrag(self, onMouseDrag: MethodWrapper) -> "IScreen":
+	def getWidth(self) -> int:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			onMouseDrag: calls your method as a BiConsumer PositionCommon_Vec2D , Integer 
+		Returns:
+			the width of the string. 
 		"""
 		pass
 
 	@overload
-	def setOnMouseUp(self, onMouseUp: MethodWrapper) -> "IScreen":
+	def getHeight(self) -> int:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			onMouseUp: calls your method as a BiConsumer PositionCommon_Pos2D , Integer 
+		Returns:
+			the height of the string. 
 		"""
 		pass
 
 	@overload
-	def setOnScroll(self, onScroll: MethodWrapper) -> "IScreen":
+	def color(self, color: int) -> "Text_Builder":
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Args:
-			onScroll: calls your method as a BiConsumer PositionCommon_Pos2D , Double 
+			color: the color of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setOnKeyPressed(self, onKeyPressed: MethodWrapper) -> "IScreen":
+	def color(self, r: int, g: int, b: int) -> "Text_Builder":
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Args:
-			onKeyPressed: calls your method as a BiConsumer Integer , Integer 
+			r: the red component of the color 
+			b: the blue component of the color 
+			g: the green component of the color 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setOnClose(self, onClose: MethodWrapper) -> "IScreen":
+	def color(self, r: int, g: int, b: int, a: int) -> "Text_Builder":
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Args:
-			onClose: calls your method as a Consumer IScreen 
+			a: the alpha component of the color 
+			r: the red component of the color 
+			b: the blue component of the color 
+			g: the green component of the color 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def close(self) -> None:
+	def getColor(self) -> int:
 		"""
-		Since: 1.1.9 
+		Since: 1.8.4 
+
+		Returns:
+			the color of the text element. 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int) -> RenderCommon_Rect:
+	def scale(self, scale: float) -> "Text_Builder":
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Args:
+			scale: the scale of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int) -> RenderCommon_Rect:
+	def getScale(self) -> float:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			the scale of the text element. 
 		"""
 		pass
 
 	@overload
-	def addRect(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float) -> RenderCommon_Rect:
+	def rotation(self, rotation: float) -> "Text_Builder":
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Args:
+			rotation: the rotation (clockwise) of the text element in degrees 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def removeRect(self, r: RenderCommon_Rect) -> "IScreen":
+	def getRotation(self) -> float:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			the rotation (clockwise) of the text element in degrees. 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str) -> RenderCommon_Item:
+	def rotateCenter(self, rotateCenter: bool) -> "Text_Builder":
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Args:
+			rotateCenter: whether this text should be rotated around its center 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str, overlay: bool) -> RenderCommon_Item:
+	def isRotatingCenter(self) -> bool:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this text should be rotated around its center, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, id: str, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def shadow(self, shadow: bool) -> "Text_Builder":
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Args:
+			shadow: whether the text should have a shadow or not 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper) -> RenderCommon_Item:
+	def hasShadow(self) -> bool:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the text element has a shadow, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool) -> RenderCommon_Item:
+	def zIndex(self, zIndex: int) -> "Text_Builder":
 		"""
-		Since: 1.2.0 
+
+		Args:
+			zIndex: the z-index of the text element 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def addItem(self, x: int, y: int, item: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> RenderCommon_Item:
+	def getZIndex(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			the z-index of the text element. 
 		"""
 		pass
 
 	@overload
-	def removeItem(self, i: RenderCommon_Item) -> "IScreen":
-		"""
-		Since: 1.2.0 
-		"""
+	def createElement(self) -> Text:
 		pass
 
 	@overload
-	def reloadScreen(self) -> "IScreen":
-		"""calls the screen's init function re-loading it.\n
-		Since: 1.2.7 
-		"""
+	def getScaledWidth(self) -> int:
 		pass
 
 	@overload
-	def onRenderInternal(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
-		"""DON'T TOUCH\n
-		Since: 1.4.1 
-		"""
+	def getParentWidth(self) -> int:
+		pass
+
+	@overload
+	def getScaledHeight(self) -> int:
+		pass
+
+	@overload
+	def getParentHeight(self) -> int:
+		pass
+
+	@overload
+	def getScaledLeft(self) -> int:
+		pass
+
+	@overload
+	def getScaledTop(self) -> int:
 		pass
 
 	@overload
-	def getOnClose(self) -> MethodWrapper:
+	def moveTo(self, x: int, y: int) -> "Text_Builder":
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/IntField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/IntField.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Inventory.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Item_Builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,286 +1,295 @@
 from typing import overload
-from typing import List
-from typing import TypeVar
-from typing import Mapping
-from typing import Generic
+from .Alignable import Alignable
+from .RenderElementBuilder import RenderElementBuilder
+from .IDraw2D import IDraw2D
 from .ItemStackHelper import ItemStackHelper
-from .RecipeHelper import RecipeHelper
 
-T = TypeVar("T")
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
 
-class Inventory(Generic[T]):
+class Item_Builder(Alignable, RenderElementBuilder):
 	"""
-	Since: 1.0.8 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def create(self) -> "Inventory":
+	def __init__(self, draw2D: IDraw2D) -> None:
 		pass
 
 	@overload
-	def create(self, s: Screen) -> "Inventory":
-		pass
-
-	@overload
-	def click(self, slot: int) -> "Inventory":
+	def x(self, x: int) -> "Item_Builder":
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
 
 		Args:
-			slot: 
-		"""
-		pass
-
-	@overload
-	def click(self, slot: int, mousebutton: int) -> "Inventory":
-		"""Clicks a slot with a mouse button.~~if the slot is a container, it will click the first slot in the container\n
-		Since: 1.0.8 
+			x: the x position of the item 
 
-		Args:
-			mousebutton: 
-			slot: 
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def dragClick(self, slots: List[int], mousebutton: int) -> "Inventory":
-		"""Does a drag-click with a mouse button. (the slots don't have to be in order or even adjacent, but when vanilla minecraft calls the underlying function they're always sorted...)
+	def getX(self) -> int:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			slots: 
-			mousebutton: 
+		Returns:
+			the x position of the item. 
 		"""
 		pass
 
 	@overload
-	def dropSlot(self, slot: int) -> "Inventory":
+	def y(self, y: int) -> "Item_Builder":
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
 
 		Args:
-			slot: 
+			y: the y position of the item 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getSelectedHotbarSlotIndex(self) -> int:
+	def getY(self) -> int:
 		"""
-		Since: 1.2.5 
+		Since: 1.8.4 
 
 		Returns:
-			the index of the selected hotbar slot. 
+			the y position of the item. 
 		"""
 		pass
 
 	@overload
-	def setSelectedHotbarSlotIndex(self, index: int) -> None:
+	def pos(self, x: int, y: int) -> "Item_Builder":
 		"""
-		Since: 1.2.5 
+		Since: 1.8.4 
 
 		Args:
-			index: 
-		"""
-		pass
+			x: the x position of the item 
+			y: the y position of the item 
 
-	@overload
-	def closeAndDrop(self) -> "Inventory":
-		"""closes the inventory, (if the inventory/container is visible it will close the gui). also drops any "held on mouse" items.
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def close(self) -> None:
-		"""Closes the inventory, and open gui if applicable.
+	def item(self, item: ItemStackHelper) -> "Item_Builder":
 		"""
-		pass
-
-	@overload
-	def quick(self, slot: int) -> "Inventory":
-		"""simulates a shift-click on a slot.
-It should be safe to chain these without FClient#waitTick() at least for a bunch of the same item.
+		Since: 1.8.4 
 
 		Args:
-			slot: 
+			item: the item to draw 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def quickAll(self, slot: int) -> int:
+	def item(self, id: str) -> "Item_Builder":
 		"""
-		Since: 1.7.0 
+		Since: 1.8.4 
 
 		Args:
-			slot: 
+			id: the id of the item to draw 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def quickAll(self, slot: int, button: int) -> int:
-		"""quicks all that match the slot\n
-		Since: 1.7.0 
+	def item(self, id: str, count: int) -> "Item_Builder":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			button: 
-			slot: a slot from the section you want to move items from 
+			count: the stack size 
+			id: the id of the item to draw 
 
 		Returns:
-			number of items that matched 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getHeld(self) -> ItemStackHelper:
+	def getItem(self) -> ItemStackHelper:
 		"""
+		Since: 1.8.4 
 
 		Returns:
-			the held (by the mouse) item. 
+			the item to be drawn. 
 		"""
 		pass
 
 	@overload
-	def getSlot(self, slot: int) -> ItemStackHelper:
-		"""
+	def overlayText(self, overlayText: str) -> "Item_Builder":
+		"""This also sets the overlay to be shown.\n
+		Since: 1.8.4 
 
 		Args:
-			slot: 
+			overlayText: the overlay text 
 
 		Returns:
-			the item in the slot. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getTotalSlots(self) -> int:
+	def getOverlayText(self) -> str:
 		"""
+		Since: 1.8.4 
 
 		Returns:
-			the size of the container/inventory. 
+			the overlay text. 
 		"""
 		pass
 
 	@overload
-	def split(self, slot1: int, slot2: int) -> "Inventory":
-		"""Splits the held stack into two slots. can be alternatively done with Inventory#dragClick(int[],int) if this one has issues on some servers.
+	def overlayVisible(self, visible: bool) -> "Item_Builder":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			slot2: 
-			slot1: 
+			visible: whether the overlay should be visible or not 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def grabAll(self, slot: int) -> "Inventory":
-		"""Does that double click thingy to turn a incomplete stack pickup into a complete stack pickup if you have more in your inventory.
+	def isOverlayVisible(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			slot: 
+		Returns:
+			'true' if the overlay should be visible, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def swap(self, slot1: int, slot2: int) -> "Inventory":
-		"""swaps the items in two slots.
+	def scale(self, scale: float) -> "Item_Builder":
+		"""
+		Since: 1.8.4 
 
 		Args:
-			slot2: 
-			slot1: 
+			scale: the scale of the item 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def swapHotbar(self, slot: int, hotbarSlot: int) -> "Inventory":
-		"""equivelent to hitting the numbers or f for swapping slots to hotbar\n
-		Since: 1.6.5 [citation needed] 
+	def getScale(self) -> float:
+		"""
+		Since: 1.8.4 
 
-		Args:
-			hotbarSlot: 0-8 or 40 for offhand 
-			slot: 
+		Returns:
+			the scale of the item. 
 		"""
 		pass
 
 	@overload
-	def openGui(self) -> None:
+	def rotation(self, rotation: float) -> "Item_Builder":
 		"""
-		Since: 1.2.8 
+		Since: 1.8.4 
+
+		Args:
+			rotation: the rotation (clockwise) of the item in degrees 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getSlotUnderMouse(self) -> int:
+	def getRotation(self) -> float:
 		"""
-		Since: 1.1.3 
+		Since: 1.8.4 
 
 		Returns:
-			the id of the slot under the mouse. 
+			the rotation (clockwise) of the item in degrees. 
 		"""
 		pass
 
 	@overload
-	def getType(self) -> str:
+	def rotateCenter(self, rotateCenter: bool) -> "Item_Builder":
 		"""
-		Since: 1.1.3 
+		Since: 1.8.4 
+
+		Args:
+			rotateCenter: whether the item should be rotated around its center 
 
 		Returns:
-			the part of the mapping the slot is in. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getMap(self) -> Mapping[str, List[int]]:
+	def isRotatingCenter(self) -> bool:
 		"""
-		Since: 1.1.3 
+		Since: 1.8.4 
 
 		Returns:
-			the inventory mappings different depending on the type of open container/inventory. 
+			'true' if this item should be rotated around its center, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getLocation(self, slotNum: int) -> str:
+	def zIndex(self, zIndex: int) -> "Item_Builder":
 		"""
-		Since: 1.1.3 
+		Since: 1.8.4 
 
 		Args:
-			slotNum: 
+			zIndex: the z-index of the item 
 
 		Returns:
-			returns the part of the mapping the slot is in. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def getCraftableRecipes(self) -> List[RecipeHelper]:
+	def getZIndex(self) -> int:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			all craftable recipes 
+			the z-index of the item. 
 		"""
 		pass
 
 	@overload
-	def getContainerTitle(self) -> str:
-		"""
-		Since: 1.2.3 
-		"""
+	def getScaledWidth(self) -> int:
 		pass
 
 	@overload
-	def getRawContainer(self) -> T:
+	def getParentWidth(self) -> int:
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def getScaledHeight(self) -> int:
 		pass
 
 	@overload
-	def getCurrentSyncId(self) -> int:
-		"""
-		Since: 1.6.0 
-		"""
+	def getParentHeight(self) -> int:
+		pass
+
+	@overload
+	def getScaledLeft(self) -> int:
+		pass
+
+	@overload
+	def getScaledTop(self) -> int:
+		pass
+
+	@overload
+	def moveTo(self, x: int, y: int) -> "Item_Builder":
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ItemStackHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FKeyBind.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,262 +1,125 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
-from .NBTElementHelper import NBTElementHelper
-
-ItemStack = TypeVar["net.minecraft.item.ItemStack"]
-
-class ItemStackHelper(BaseHelper):
-	"""
+from typing import Mapping
+from typing import Set
+from .BaseLibrary import BaseLibrary
+
+InputUtil_Key = TypeVar["net.minecraft.client.util.InputUtil.Key"]
+
+class FKeyBind(BaseLibrary):
+	"""Functions for getting and modifying key pressed states. 
+An instance of this class is passed to scripts as the 'KeyBind' variable.
 	"""
 
 	@overload
-	def __init__(self, i: ItemStack) -> None:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def setDamage(self, damage: int) -> "ItemStackHelper":
-		"""Sets the item damage value.
-
-You may want to use ItemStackHelper#copy() first.\n
-		Since: 1.2.0 
+	def getKeyCode(self, keyName: str) -> InputUtil_Key:
+		"""Dont use this one... get the raw minecraft keycode class.
 
 		Args:
-			damage: 
-		"""
-		pass
-
-	@overload
-	def isDamageable(self) -> bool:
-		"""
-		Since: 1.2.0 
-		"""
-		pass
-
-	@overload
-	def isEnchantable(self) -> bool:
-		"""
-		Since: 1.2.0 
-		"""
-		pass
-
-	@overload
-	def getDamage(self) -> int:
-		"""
-		"""
-		pass
-
-	@overload
-	def getMaxDamage(self) -> int:
-		"""
-		"""
-		pass
-
-	@overload
-	def getDefaultName(self) -> TextHelper:
-		"""
-		Since: 1.2.0 
+			keyName: 
 
 		Returns:
-			was string before 1.6.5 
+			the raw minecraft keycode class 
 		"""
 		pass
 
 	@overload
-	def getName(self) -> TextHelper:
+	def getKeyBindings(self) -> Mapping[str, str]:
 		"""
+		Since: 1.2.2 
 
 		Returns:
-			was string before 1.6.5 
-		"""
-		pass
-
-	@overload
-	def getCount(self) -> int:
-		"""
-		"""
-		pass
-
-	@overload
-	def getMaxCount(self) -> int:
-		"""
-		"""
-		pass
-
-	@overload
-	def getNBT(self) -> NBTElementHelper:
-		"""
-		Since: 1.1.6, was a String until 1.5.1 
-		"""
-		pass
-
-	@overload
-	def getCreativeTab(self) -> str:
-		"""
-		Since: 1.1.3 
-		"""
-		pass
-
-	@overload
-	def getItemID(self) -> str:
-		"""
-		"""
-		pass
-
-	@overload
-	def getItemId(self) -> str:
+			A Map of all the minecraft keybinds. 
 		"""
-		Since: 1.6.4 
-		"""
-		pass
-
-	@overload
-	def getTags(self) -> List[str]:
-		"""
-		Since: 1.8.2 
-		"""
-		pass
-
-	@overload
-	def isFood(self) -> bool:
-		"""
-		Since: 1.8.2 
-		"""
-		pass
-
-	@overload
-	def isTool(self) -> bool:
-		"""
-		Since: 1.8.2 
-		"""
-		pass
-
-	@overload
-	def isWearable(self) -> bool:
-		"""
-		Since: 1.8.2 
-		"""
-		pass
-
-	@overload
-	def getMiningLevel(self) -> int:
-		"""
-		Since: 1.8.2 
-		"""
-		pass
-
-	@overload
-	def isEmpty(self) -> bool:
-		"""
-		"""
-		pass
-
-	@overload
-	def toString(self) -> str:
 		pass
 
 	@overload
-	def equals(self, ish: "ItemStackHelper") -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def setKeyBind(self, bind: str, key: str) -> None:
+		"""Sets a minecraft keybind to the specified key.\n
+		Since: 1.2.2 
 
 		Args:
-			ish: 
+			bind: 
+			key: 
 		"""
 		pass
 
 	@overload
-	def equals(self, is_: ItemStack) -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def key(self, keyName: str, keyState: bool) -> None:
+		"""Set a key-state for a key.
 
 		Args:
-			is: 
+			keyState: 
+			keyName: 
 		"""
 		pass
 
 	@overload
-	def isItemEqual(self, ish: "ItemStackHelper") -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def pressKey(self, keyName: str) -> None:
+		"""Calls FKeyBind#key(java.lang.String,boolean) with keyState set to true.\n
+		Since: 1.8.4 
 
 		Args:
-			ish: 
+			keyName: the name of the key to press 
 		"""
 		pass
 
 	@overload
-	def isItemEqual(self, is_: ItemStack) -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def releaseKey(self, keyName: str) -> None:
+		"""Calls FKeyBind#key(java.lang.String,boolean) with keyState set to false.\n
+		Since: 1.8.4 
 
 		Args:
-			is: 
+			keyName: the name of the key to release 
 		"""
 		pass
 
 	@overload
-	def isItemEqualIgnoreDamage(self, ish: "ItemStackHelper") -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def keyBind(self, keyBind: str, keyState: bool) -> None:
+		"""Set a key-state using the name of the keybind rather than the name of the key. 
+This is probably the one you should use.\n
+		Since: 1.2.2 
 
 		Args:
-			ish: 
+			keyBind: 
+			keyState: 
 		"""
 		pass
 
 	@overload
-	def isItemEqualIgnoreDamage(self, is_: ItemStack) -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def pressKeyBind(self, keyBind: str) -> None:
+		"""Calls FKeyBind#keyBind(java.lang.String,boolean) with keyState set to true.\n
+		Since: 1.8.4 
 
 		Args:
-			is: 
+			keyBind: the name of the keybinding to press 
 		"""
 		pass
 
 	@overload
-	def isNBTEqual(self, ish: "ItemStackHelper") -> bool:
-		"""
-		Since: 1.1.3 [citation needed] 
+	def releaseKeyBind(self, keyBind: str) -> None:
+		"""Calls FKeyBind#keyBind(java.lang.String,boolean) with keyState set to false.\n
+		Since: 1.8.4 
 
 		Args:
-			ish: 
+			keyBind: the name of the keybinding to release 
 		"""
 		pass
 
 	@overload
-	def isNBTEqual(self, is_: ItemStack) -> bool:
+	def getPressedKeys(self) -> Set[str]:
 		"""
-		Since: 1.1.3 [citation needed] 
+		Since: 1.2.6 (turned into set instead of list in 1.6.5) 
 
-		Args:
-			is: 
-		"""
-		pass
-
-	@overload
-	def isOnCooldown(self) -> bool:
-		"""
-		Since: 1.6.5 
-		"""
-		pass
-
-	@overload
-	def getCooldownProgress(self) -> float:
-		"""
-		Since: 1.6.5 
-		"""
-		pass
-
-	@overload
-	def copy(self) -> "ItemStackHelper":
-		"""
-		Since: 1.2.0 
+		Returns:
+			a set of currently pressed keys. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/JsMacros.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/JsMacros.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseScreen import BaseScreen
 from .Core import Core
+from .ModLoader import ModLoader
 
 KeyBinding = TypeVar["net.minecraft.client.option.KeyBinding"]
 Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
 MinecraftClient = TypeVar["net.minecraft.client.MinecraftClient"]
 InputUtil_Key = TypeVar["net.minecraft.client.util.InputUtil.Key"]
 Text = TypeVar["net.minecraft.text.Text"]
 Logger = TypeVar["org.slf4j.Logger"]
@@ -54,10 +55,14 @@
 	def range(self, start: int, end: int) -> List[int]:
 		pass
 
 	@overload
 	def range(self, start: int, end: int, iter: int) -> List[int]:
 		pass
 
+	@overload
+	def getModLoader(self) -> ModLoader:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/LibraryBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/LibraryBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 	@overload
 	def __init__(self, name: str, perExec: bool, allowedLangs: List[str]) -> None:
 		pass
 
 	@overload
 	def addConstructor(self) -> ClassBuilder_ConstructorBuilder:
 		"""constructor, if perExec run every context, if per language run once for each lang;
-params are context and language class
-if not per exec, param will be skipped
+params are context and language class.
+if not per exec, param will be skipped.
 ie:
 BaseLibrary: no params
 PerExecLibrary: context
 PerExecLanguageLibrary: context, language
-PerLanguageLibrary: language
-
+PerLanguageLibrary: language 
 Don't do other constructors...
 		"""
 		pass
 
 	@overload
 	def finishBuildAndFreeze(self) -> Class:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/LibraryRegistry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/LibraryRegistry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ListContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ListContainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 		pass
 
 	@overload
 	def onScrollbar(self, page: float) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/LivingEntityHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerEntityHelper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,156 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
 from typing import Generic
-from .EntityHelper import EntityHelper
-from .StatusEffectHelper import StatusEffectHelper
+from .LivingEntityHelper import LivingEntityHelper
+from .PlayerAbilitiesHelper import PlayerAbilitiesHelper
 from .ItemStackHelper import ItemStackHelper
+from .FishingBobberEntityHelper import FishingBobberEntityHelper
 
 T = TypeVar("T")
 
-class LivingEntityHelper(Generic[T], EntityHelper):
+class PlayerEntityHelper(Generic[T], LivingEntityHelper):
+	"""
+	"""
 
 	@overload
 	def __init__(self, e: T) -> None:
 		pass
 
 	@overload
-	def getStatusEffects(self) -> List[StatusEffectHelper]:
+	def getPlayerName(self) -> str:
+		"""get player's actual name. (not display name)\n
+		Since: 1.8.4 
 		"""
-		Since: 1.2.7 
+		pass
 
-		Returns:
-			entity status effects. 
+	@overload
+	def getAbilities(self) -> PlayerAbilitiesHelper:
+		"""
+		Since: 1.0.3 
 		"""
 		pass
 
 	@overload
 	def getMainHand(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.7 
-
-		Returns:
-			the item in the entity's main hand. 
+		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
 	def getOffHand(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.7 
-
-		Returns:
-			the item in the entity's off hand. 
+		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
 	def getHeadArmor(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.7 
-
-		Returns:
-			the item in the entity's head armor slot. 
+		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
 	def getChestArmor(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.7 
-
-		Returns:
-			the item in the entity's chest armor slot. 
+		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
 	def getLegArmor(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.7 
-
-		Returns:
-			the item in the entity's leg armor slot. 
+		Since: 1.2.0 
 		"""
 		pass
 
 	@overload
 	def getFootArmor(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.7 
+		Since: 1.2.0 
+		"""
+		pass
 
-		Returns:
-			the item in the entity's foot armor slot. 
+	@overload
+	def getXP(self) -> int:
+		"""
+		Since: 1.2.5 [citation needed] 
 		"""
 		pass
 
 	@overload
-	def getHealth(self) -> float:
+	def getXPLevel(self) -> int:
+		"""
+		Since: 1.6.5 
 		"""
-		Since: 1.3.1 
+		pass
 
-		Returns:
-			entity's health 
+	@overload
+	def getXPProgress(self) -> float:
+		"""
+		Since: 1.6.5 
 		"""
 		pass
 
 	@overload
-	def getMaxHealth(self) -> float:
+	def getXPToLevelUp(self) -> int:
 		"""
 		Since: 1.6.5 
+		"""
+		pass
+
+	@overload
+	def isSleeping(self) -> bool:
+		"""
+		Since: 1.2.5 [citation needed] 
+		"""
+		pass
+
+	@overload
+	def isSleepingLongEnough(self) -> bool:
+		"""
+		Since: 1.2.5 [citation needed] 
 
 		Returns:
-			entity's max health 
+			if the player has slept the minimum ammount of time to pass the night. 
 		"""
 		pass
 
 	@overload
-	def isSleeping(self) -> bool:
+	def getFishingBobber(self) -> FishingBobberEntityHelper:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Returns:
-			if the entity is in a bed. 
+			the fishing bobber of the player, or 'null' if the player is not fishing. 
+		"""
+		pass
+
+	@overload
+	def getAttackCooldownProgress(self) -> float:
+		"""
+		Since: 1.8.4 
+		"""
+		pass
+
+	@overload
+	def getAttackCooldownProgressPerTick(self) -> float:
+		"""
+		Since: 1.8.4 
 		"""
 		pass
 
 	@overload
-	def isFallFlying(self) -> bool:
+	def getScore(self) -> int:
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
 
 		Returns:
-			if the entity has elytra deployed 
+			the player's score. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/LongField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/LongField.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/LoomInventory.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/LoomInventory.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,10 +53,14 @@
 			index: 
 
 		Returns:
 			success 
 		"""
 		pass
 
+	@overload
+	def toString(self) -> str:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MacroContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MacroContainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,13 +44,13 @@
 		pass
 
 	@overload
 	def setKey(self, translationKeys: str) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MacroListTopbar.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MacroListTopbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 		pass
 
 	@overload
 	def updateType(self, type: ScriptTrigger_TriggerType) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MacroScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MacroScreen.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 		pass
 
 	@overload
 	def editFile(self, file: File) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def updateSettings(self) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Mappings.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Mappings.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MerchantEntityHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MerchantEntityHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,10 @@
 
 	@overload
 	def hasCustomer(self) -> bool:
 		"""
 		"""
 		pass
 
-	@overload
-	def toString(self) -> str:
-		pass
-
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MethodWrapper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MethodWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TypeVar
 from typing import Generic
 
 C = TypeVar("C")
 Predicate = TypeVar["java.util.function.Predicate_T_"]
 Comparator = TypeVar["java.util.Comparator_T_"]
 Thread = TypeVar["java.lang.Thread"]
-Function = TypeVar["java.util.function.Function_T,R_"]
+Function = TypeVar["java.util.function.Function_ super R, extends V_"]
 R = TypeVar("R")
 T = TypeVar("T")
 Consumer = TypeVar["java.util.function.Consumer_T_"]
 U = TypeVar("U")
 BiFunction = TypeVar["java.util.function.BiFunction_T,U,R_"]
 Runnable = TypeVar["java.lang.Runnable"]
 Supplier = TypeVar["java.util.function.Supplier_R_"]
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinBeaconScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinBeaconScreen.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinChatHud.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinChatHud.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientPlayNetworkHandler.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientPlayNetworkHandler.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientPlayerEntity.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MovementQueue.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from typing import overload
 from typing import TypeVar
-from .IClientPlayerEntity import IClientPlayerEntity
+from .Draw3D import Draw3D
+from .PlayerInput import PlayerInput
 
-GameProfile = TypeVar["com.mojang.authlib.GameProfile"]
-AbstractClientPlayerEntity = TypeVar["net.minecraft.client.network.AbstractClientPlayerEntity"]
-ClientWorld = TypeVar["net.minecraft.client.world.ClientWorld"]
+ClientPlayerEntity = TypeVar["net.minecraft.client.network.ClientPlayerEntity"]
 
-class MixinClientPlayerEntity(IClientPlayerEntity, AbstractClientPlayerEntity):
+class MovementQueue:
+	predPoints: Draw3D
 
 	@overload
-	def __init__(self, world: ClientWorld, profile: GameProfile, publicKey: PlayerPublicKey) -> None:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def jsmacros_sendChatMessageBypass(self, message: str) -> None:
+	def tick(self, newPlayer: ClientPlayerEntity) -> PlayerInput:
+		pass
+
+	@overload
+	def append(self, input: PlayerInput, newPlayer: ClientPlayerEntity) -> None:
+		pass
+
+	@overload
+	def setDrawPredictions(self, val: bool) -> None:
+		pass
+
+	@overload
+	def clear(self) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientPlayerInteractionManager.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientPlayerInteractionManager.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinClientWorld.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinClientWorld.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinEntity.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinEntity.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinMinecraftClient.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinMinecraftClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import overload
 from typing import TypeVar
 
+ClientPlayerInteractionManager = TypeVar["net.minecraft.client.network.ClientPlayerInteractionManager"]
 CallbackInfo = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfo"]
 Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
 ClientWorld = TypeVar["net.minecraft.client.world.ClientWorld"]
 
 class MixinMinecraftClient:
 	currentScreen: Screen
 	interactionManager: ClientPlayerInteractionManager
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPalettedContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinPalettedContainerData.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
-from .IPalettedContainer import IPalettedContainer
 from .IPalettedContainerData import IPalettedContainerData
 
+Palette = TypeVar["net.minecraft.world.chunk.Palette_T_"]
 T = TypeVar("T")
-PalettedContainer_PaletteProvider = TypeVar["net.minecraft.world.chunk.PalettedContainer.PaletteProvider"]
+PaletteStorage = TypeVar["net.minecraft.util.collection.PaletteStorage"]
 
-class MixinPalettedContainer(IPalettedContainer, Generic[T]):
+class MixinPalettedContainerData(IPalettedContainerData, Generic[T]):
 
 	@overload
 	def __init__(self) -> None:
 		pass
 
 	@overload
-	def jsmacros_getData(self) -> IPalettedContainerData:
+	def jsmacros_getStorage(self) -> PaletteStorage:
 		pass
 
 	@overload
-	def jsmacros_getPaletteProvider(self) -> PalettedContainer_PaletteProvider:
+	def jsmacros_getPalette(self) -> Palette:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinPalettedContainerData.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ShulkerEntityHelper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import overload
 from typing import TypeVar
-from typing import Generic
-from .IPalettedContainerData import IPalettedContainerData
+from .MobEntityHelper import MobEntityHelper
+from .DirectionHelper import DirectionHelper
+from .DyeColorHelper import DyeColorHelper
+
+ShulkerEntity = TypeVar["net.minecraft.entity.mob.ShulkerEntity"]
+
+class ShulkerEntityHelper(MobEntityHelper):
+	"""
+	Since: 1.8.4 
+	"""
 
-Palette = TypeVar["net.minecraft.world.chunk.Palette_T_"]
-T = TypeVar("T")
-PaletteStorage = TypeVar["net.minecraft.util.collection.PaletteStorage"]
-
-class MixinPalettedContainerData(IPalettedContainerData, Generic[T]):
+	@overload
+	def __init__(self, base: ShulkerEntity) -> None:
+		pass
 
 	@overload
-	def __init__(self) -> None:
+	def isClosed(self) -> bool:
 		pass
 
 	@overload
-	def jsmacros_getStorage(self) -> PaletteStorage:
+	def getAttachedSide(self) -> DirectionHelper:
 		pass
 
 	@overload
-	def jsmacros_getPalette(self) -> Palette:
+	def getColor(self) -> DyeColorHelper:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MixinResourcePackManager.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MixinResourcePackManager.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MovementDummy.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/MovementDummy.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/MultiElementContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/OverlayContainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from typing import Generic
-from .IContainerParent import IContainerParent
-from .OverlayContainer import OverlayContainer
+from typing import Mapping
 from .IOverlayParent import IOverlayParent
+from .MultiElementContainer import MultiElementContainer
+from .Scrollbar import Scrollbar
 
-T = TypeVar("T")
-DrawableHelper = TypeVar["net.minecraft.client.gui.DrawableHelper"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 Element = TypeVar["net.minecraft.client.gui.Element"]
 ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class MultiElementContainer(IContainerParent, Generic[T], DrawableHelper):
-	parent: T
-	x: int
-	y: int
-	width: int
-	height: int
+class OverlayContainer(IOverlayParent, MultiElementContainer):
+	savedBtnStates: Mapping[ClickableWidget, bool]
+	scroll: Scrollbar
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: T) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def remove(self, btn: Element) -> None:
 		pass
 
 	@overload
-	def getVisible(self) -> bool:
+	def openOverlay(self, overlay: "OverlayContainer") -> None:
 		pass
 
 	@overload
-	def setVisible(self, visible: bool) -> None:
+	def getFirstOverlayParent(self) -> IOverlayParent:
 		pass
 
 	@overload
-	def addDrawableChild(self, drawableElement: T) -> T:
+	def openOverlay(self, overlay: "OverlayContainer", disableButtons: bool) -> None:
 		pass
 
 	@overload
-	def getButtons(self) -> List[ClickableWidget]:
+	def getChildOverlay(self) -> "OverlayContainer":
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
+	def closeOverlay(self, overlay: "OverlayContainer") -> None:
 		pass
 
 	@overload
-	def openOverlay(self, overlay: OverlayContainer) -> None:
+	def setFocused(self, focused: Element) -> None:
 		pass
 
 	@overload
-	def openOverlay(self, overlay: OverlayContainer, disableButtons: bool) -> None:
+	def onClick(self, mouseX: float, mouseY: float, button: int) -> None:
 		pass
 
 	@overload
-	def remove(self, button: Element) -> None:
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
+		"""
+
+		Returns:
+			true if should be handled by overlay 
+		"""
 		pass
 
 	@overload
-	def getFirstOverlayParent(self) -> IOverlayParent:
+	def close(self) -> None:
+		pass
+
+	@overload
+	def onClose(self) -> None:
+		pass
+
+	@overload
+	def renderBackground(self, drawContext: MatrixStack) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper_NBTListHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper_NBTListHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/NoStyleCodeCompiler.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/NoStyleCodeCompiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TypeVar
 from typing import Mapping
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
 Runnable = TypeVar["java.lang.Runnable"]
+Text = TypeVar["net.minecraft.text.Text"]
 
 class NoStyleCodeCompiler(AbstractRenderCodeCompiler):
 
 	@overload
 	def __init__(self, language: str, screen: EditorScreen) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/OptionsField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/OptionsField.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/OptionsHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ChunkHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,304 +1,255 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from typing import Mapping
+from typing import Any
 from .BaseHelper import BaseHelper
+from .BlockPosHelper import BlockPosHelper
+from .MethodWrapper import MethodWrapper
 
-GameOptions = TypeVar["net.minecraft.client.option.GameOptions"]
+Heightmap = TypeVar["net.minecraft.world.Heightmap"]
+Map_Entry = TypeVar["java.util.Map.Entry_net.minecraft.world.Heightmap.Type,net.minecraft.world.Heightmap_"]
+Chunk = TypeVar["net.minecraft.world.chunk.Chunk"]
 
-class OptionsHelper(BaseHelper):
+class ChunkHelper(BaseHelper):
 	"""
-	Since: 1.1.7 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, options: GameOptions) -> None:
+	def __init__(self, base: Chunk) -> None:
 		pass
 
 	@overload
-	def getCloudMode(self) -> int:
+	def getStartingBlock(self) -> BlockPosHelper:
 		"""
-		Since: 1.1.7 
+		Since: 1.8.4 
 
 		Returns:
-			0: off, 2: fancy 
+			the first block (0 0 0 coordinate) of this chunk. 
 		"""
 		pass
 
 	@overload
-	def setCloudMode(self, mode: int) -> "OptionsHelper":
-		"""
-		Since: 1.1.7 
+	def getOffsetBlock(self, xOffset: int, y: int, zOffset: int) -> BlockPosHelper:
+		"""The coordinates are relative to the starting chunk position, see ChunkHelper#getStartingBlock() .\n
+		Since: 1.8.4 
 
 		Args:
-			mode: 0: off, 2: fancy 
-		"""
-		pass
+			xOffset: the xOffset offset 
+			y: the actual y coordinate 
+			zOffset: the zOffset offset 
 
-	@overload
-	def getGraphicsMode(self) -> int:
-		"""
-		Since: 1.1.7 
+		Returns:
+			the block offset from the starting block of this chunk by xOffset y zOffset. 
 		"""
 		pass
 
 	@overload
-	def setGraphicsMode(self, mode: int) -> "OptionsHelper":
+	def getMaxBuildHeight(self) -> int:
 		"""
-		Since: 1.1.7 
+		Since: 1.8.4 
 
-		Args:
-			mode: 0: fast, 2: fabulous 
+		Returns:
+			the maximum height of this chunk. 
 		"""
 		pass
 
 	@overload
-	def getResourcePacks(self) -> List[str]:
+	def getMinBuildHeight(self) -> int:
 		"""
-		Since: 1.1.7 
+		Since: 1.8.4 
 
 		Returns:
-			list of names of resource packs. 
+			the minimum height of this chunk. 
 		"""
 		pass
 
 	@overload
-	def getEnabledResourcePacks(self) -> List[str]:
+	def getHeight(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
 
 		Returns:
-			list of names of enabled resource packs. 
-		"""
-		pass
-
-	@overload
-	def setEnabledResourcePacks(self, enabled: List[str]) -> "OptionsHelper":
-		"""Set the enabled resource packs to the provided list.\n
-		Since: 1.2.0 
-
-		Args:
-			enabled: 
+			the height of this chunk. 
 		"""
 		pass
 
 	@overload
-	def removeServerResourcePack(self, state: bool) -> None:
+	def getTopYAt(self, xOffset: int, zOffset: int, heightmap: Heightmap) -> int:
 		"""
-		Since: 1.8.3 
+		Since: 1.8.4 
 
 		Args:
-			state: false to put it back 
-		"""
-		pass
+			heightmap: the heightmap to use 
+			xOffset: the xOffset coordinate 
+			zOffset: the zOffset coordinate 
 
-	@overload
-	def isRightHanded(self) -> bool:
-		"""
-		Since: 1.1.7 
+		Returns:
+			the maximum 'y' position of all blocks inside this chunk. 
 		"""
 		pass
 
 	@overload
-	def setRightHanded(self, val: bool) -> None:
+	def getChunkX(self) -> int:
 		"""
-		Since: 1.1.7 
+		Since: 1.8.4 
 
-		Args:
-			val: 
+		Returns:
+			the 'x' coordinate (not the world coordinate) of this chunk. 
 		"""
 		pass
 
 	@overload
-	def getFov(self) -> float:
+	def getChunkZ(self) -> int:
 		"""
-		Since: 1.1.7 
+		Since: 1.8.4 
+
+		Returns:
+			the 'z' coordinate (not the world coordinate) of this chunk. 
 		"""
 		pass
 
 	@overload
-	def setFov(self, fov: int) -> "OptionsHelper":
+	def getBiome(self, xOffset: int, y: int, zOffset: int) -> str:
 		"""
-		Since: 1.1.7 
+		Since: 1.8.4 
 
 		Args:
-			fov: (int since 1.7.0) 
-		"""
-		pass
+			xOffset: the x offset 
+			y: the y coordinate 
+			zOffset: the z offset 
 
-	@overload
-	def getRenderDistance(self) -> int:
-		"""
-		Since: 1.1.7 
+		Returns:
+			the biome at the given position. 
 		"""
 		pass
 
 	@overload
-	def setRenderDistance(self, d: int) -> None:
-		"""
-		Since: 1.1.7 
+	def getInhabitedTime(self) -> float:
+		"""With an increasing inhabited time, the local difficulty increases and stronger mobs will
+spawn. Because the time is cumulative, the more players are in the chunk, the faster the time
+will increase.\n
+		Since: 1.8.4 
 
-		Args:
-			d: 
+		Returns:
+			the cumulative time players have spent inside this chunk. 
 		"""
 		pass
 
 	@overload
-	def getWidth(self) -> int:
-		"""
-		Since: 1.2.6 
+	def getEntities(self) -> List[Any]:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getHeight(self) -> int:
-		"""
-		Since: 1.2.6 
+		Returns:
+			all entities inside this chunk. 
 		"""
 		pass
 
 	@overload
-	def setWidth(self, w: int) -> None:
+	def getTileEntities(self) -> List[BlockPosHelper]:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
-		Args:
-			w: 
+		Returns:
+			all tile entity positions inside this chunk. 
 		"""
 		pass
 
 	@overload
-	def setHeight(self, h: int) -> None:
+	def forEach(self, includeAir: bool, callback: MethodWrapper) -> "ChunkHelper":
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
 		Args:
-			h: 
+			includeAir: whether to include air blocks or not 
+			callback: the callback function 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setSize(self, w: int, h: int) -> None:
+	def containsAny(self, blocks: List[str]) -> bool:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
 		Args:
-			w: 
-			h: 
-		"""
-		pass
-
-	@overload
-	def getGamma(self) -> float:
-		"""
-		Since: 1.3.0
-normal values for gamam are between '0' and '1' 
-		"""
-		pass
+			blocks: the blocks to search for 
 
-	@overload
-	def setGamma(self, gamma: float) -> None:
-		"""
-		Since: 1.3.0
-normal values for gamma are between '0' and '1' 
+		Returns:
+			'true' if this chunk contains at least one of the specified blocks, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def setVolume(self, vol: float) -> None:
+	def containsAll(self, blocks: List[str]) -> bool:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Args:
-			vol: 
-		"""
-		pass
+			blocks: the blocks to search for 
 
-	@overload
-	def setVolume(self, category: str, volume: float) -> None:
-		"""set volume by category.\n
-		Since: 1.3.1 
-
-		Args:
-			volume: 
-			category: 
+		Returns:
+			'true' if the chunk contains all the specified blocks, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getVolumes(self) -> Mapping[str, Float]:
+	def getHeightmaps(self) -> List[Map_Entry]:
 		"""
-		Since: 1.3.1 
-		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def setGuiScale(self, scale: int) -> None:
-		"""sets gui scale, '0' for auto.\n
-		Since: 1.3.1 
-
-		Args:
-			scale: 
+		Returns:
+			a map of the raw heightmap data. 
 		"""
 		pass
 
 	@overload
-	def getGuiScale(self) -> int:
+	def getSurfaceHeightmap(self) -> Heightmap:
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Returns:
-			gui scale, '0' for auto. 
+			the raw surface heightmap. 
 		"""
 		pass
 
 	@overload
-	def getVolume(self, category: str) -> float:
+	def getOceanFloorHeightmap(self) -> Heightmap:
 		"""
-		Since: 1.3.1 
-
-		Args:
-			category: 
-		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getSmoothCamera(self) -> bool:
-		"""
-		Since: 1.5.0 
+		Returns:
+			the raw ocean floor heightmap. 
 		"""
 		pass
 
 	@overload
-	def setSmoothCamera(self, val: bool) -> None:
+	def getMotionBlockingHeightmap(self) -> Heightmap:
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
 
-		Args:
-			val: 
+		Returns:
+			the raw motion blocking heightmap. 
 		"""
 		pass
 
 	@overload
-	def getCameraMode(self) -> int:
+	def getMotionBlockingNoLeavesHeightmap(self) -> Heightmap:
 		"""
-		Since: 1.5.0 
+		Since: 1.8.4 
 
 		Returns:
-			0 for 1st person, 2 for in front. 
+			the raw motion blocking heightmap without leaves. 
 		"""
 		pass
 
 	@overload
-	def setCameraMode(self, mode: int) -> None:
-		"""
-		Since: 1.5.0 
-
-		Args:
-			mode: 0: first, 2: front 
-		"""
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/OverlayContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/SelectorDropdownOverlay.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,44 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from typing import Mapping
+from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
-from .MultiElementContainer import MultiElementContainer
-from .Scrollbar import Scrollbar
 
+Consumer = TypeVar["java.util.function.Consumer_java.lang.Integer_"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-Element = TypeVar["net.minecraft.client.gui.Element"]
-ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
+Text = TypeVar["net.minecraft.text.Text"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class OverlayContainer(IOverlayParent, MultiElementContainer):
-	savedBtnStates: Mapping[ClickableWidget, bool]
-	scroll: Scrollbar
+class SelectorDropdownOverlay(OverlayContainer):
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, choices: List[Text], textRenderer: TextRenderer, parent: IOverlayParent, onChoice: Consumer) -> None:
 		pass
 
 	@overload
-	def remove(self, btn: Element) -> None:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def openOverlay(self, overlay: "OverlayContainer") -> None:
-		pass
-
-	@overload
-	def getFirstOverlayParent(self) -> IOverlayParent:
-		pass
-
-	@overload
-	def openOverlay(self, overlay: "OverlayContainer", disableButtons: bool) -> None:
-		pass
-
-	@overload
-	def getChildOverlay(self) -> "OverlayContainer":
-		pass
-
-	@overload
-	def closeOverlay(self, overlay: "OverlayContainer") -> None:
-		pass
-
-	@overload
-	def setFocused(self, focused: Element) -> None:
+	def onScroll(self, page: float) -> None:
 		pass
 
 	@overload
 	def onClick(self, mouseX: float, mouseY: float, button: int) -> None:
 		pass
 
 	@overload
-	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
-		"""
-
-		Returns:
-			true if should be handled by overlay 
-		"""
-		pass
-
-	@overload
-	def close(self) -> None:
-		pass
-
-	@overload
-	def onClose(self) -> None:
+	def setSelected(self, sel: int) -> None:
 		pass
 
 	@overload
-	def renderBackground(self, matrices: MatrixStack) -> None:
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerAbilitiesHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextHelper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,118 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
+from .MethodWrapper import MethodWrapper
 
-PlayerAbilities = TypeVar["net.minecraft.entity.player.PlayerAbilities"]
+Pattern = TypeVar["java.util.regex.Pattern"]
+Text = TypeVar["net.minecraft.text.Text"]
 
-class PlayerAbilitiesHelper(BaseHelper):
+class TextHelper(BaseHelper):
 	"""
-	Since: 1.0.3 
+	Since: 1.0.8 
 	"""
+	STRIP_FORMATTING_PATTERN: Pattern
 
 	@overload
-	def __init__(self, a: PlayerAbilities) -> None:
+	def __init__(self, t: Text) -> None:
 		pass
 
 	@overload
-	def getInvulnerable(self) -> bool:
+	def replaceFromJson(self, json: str) -> "TextHelper":
+		"""replace the text in this class with JSON data.\n
+		Since: 1.0.8 
+
+		Args:
+			json: 
 		"""
-		Since: 1.0.3 
+		pass
 
-		Returns:
-			whether the player can be damaged. 
+	@overload
+	def replaceFromString(self, content: str) -> "TextHelper":
+		"""replace the text in this class with String data.\n
+		Since: 1.0.8 
+
+		Args:
+			content: 
 		"""
 		pass
 
 	@overload
-	def getFlying(self) -> bool:
+	def getJson(self) -> str:
 		"""
-		Since: 1.0.3 
+		Since: 1.2.7 
 
 		Returns:
-			if the player is currently flying. 
+			JSON data representation. 
 		"""
 		pass
 
 	@overload
-	def getAllowFlying(self) -> bool:
+	def getString(self) -> str:
 		"""
-		Since: 1.0.3 
+		Since: 1.2.7 
 
 		Returns:
-			if the player is allowed to fly. 
+			the text content. 
 		"""
 		pass
 
 	@overload
-	def getCreativeMode(self) -> bool:
+	def getStringStripFormatting(self) -> str:
 		"""
-		Since: 1.0.3 
+		Since: 1.6.5 
 
 		Returns:
-			if the player is in creative. 
+			the text content. stripped formatting when servers send it the (super) old way due to shitty coders. 
 		"""
 		pass
 
 	@overload
-	def setFlying(self, b: bool) -> "PlayerAbilitiesHelper":
-		"""set the player flying state.\n
-		Since: 1.0.3 
+	def withoutFormatting(self) -> "TextHelper":
+		"""
+		Since: 1.8.4 
 
-		Args:
-			b: 
+		Returns:
+			the text helper without the formatting applied. 
 		"""
 		pass
 
 	@overload
-	def setAllowFlying(self, b: bool) -> "PlayerAbilitiesHelper":
-		"""set the player allow flying state.\n
-		Since: 1.0.3 
+	def visit(self, visitor: MethodWrapper) -> "TextHelper":
+		"""
+		Since: 1.6.5 
 
 		Args:
-			b: 
+			visitor: function with 2 args, no return. 
 		"""
 		pass
 
 	@overload
-	def getFlySpeed(self) -> float:
+	def getWidth(self) -> int:
 		"""
-		Since: 1.0.3 
+		Since: 1.8.4 
 
 		Returns:
-			the player fly speed multiplier. 
+			the width of this text. 
 		"""
 		pass
 
 	@overload
-	def setFlySpeed(self, flySpeed: float) -> "PlayerAbilitiesHelper":
-		"""set the player fly speed multiplier.\n
-		Since: 1.0.3 
+	def toJson(self) -> str:
+		"""
+		Since: 1.0.8 
+		"""
+		pass
 
-		Args:
-			flySpeed: 
+	@overload
+	def toString(self) -> str:
+		"""
+		Since: 1.0.8, this used to do the same as TextHelper#getString() 
+
+		Returns:
+			String representation of text helper. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerEntityHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TeamHelper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,115 +1,150 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from typing import Generic
-from .LivingEntityHelper import LivingEntityHelper
-from .PlayerAbilitiesHelper import PlayerAbilitiesHelper
-from .ItemStackHelper import ItemStackHelper
+from .BaseHelper import BaseHelper
+from .TextHelper import TextHelper
+from .FormattingHelper import FormattingHelper
+from .ScoreboardsHelper import ScoreboardsHelper
 
-T = TypeVar("T")
+Team = TypeVar["net.minecraft.scoreboard.Team"]
 
-class PlayerEntityHelper(Generic[T], LivingEntityHelper):
+class TeamHelper(BaseHelper):
 	"""
+	Since: 1.3.0 
 	"""
 
 	@overload
-	def __init__(self, e: T) -> None:
+	def __init__(self, t: Team) -> None:
 		pass
 
 	@overload
-	def getAbilities(self) -> PlayerAbilitiesHelper:
+	def getName(self) -> str:
 		"""
-		Since: 1.0.3 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def getMainHand(self) -> ItemStackHelper:
+	def getDisplayName(self) -> TextHelper:
 		"""
-		Since: 1.2.0 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def getOffHand(self) -> ItemStackHelper:
+	def getPlayerList(self) -> List[str]:
 		"""
-		Since: 1.2.0 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def getHeadArmor(self) -> ItemStackHelper:
+	def getColorFormat(self) -> FormattingHelper:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			the formatting of this team's color. 
 		"""
 		pass
 
 	@overload
-	def getChestArmor(self) -> ItemStackHelper:
+	def getColor(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def getLegArmor(self) -> ItemStackHelper:
+	def getColorIndex(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			the color index of this team. 
 		"""
 		pass
 
 	@overload
-	def getFootArmor(self) -> ItemStackHelper:
+	def getColorValue(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
+
+		Returns:
+			the color value for this team or '-1' if it has no color. 
 		"""
 		pass
 
 	@overload
-	def getXP(self) -> int:
+	def getColorName(self) -> str:
 		"""
-		Since: 1.2.5 [citation needed] 
+		Since: 1.8.4 
+
+		Returns:
+			the name of this team's color. 
 		"""
 		pass
 
 	@overload
-	def getXPLevel(self) -> int:
+	def getScoreboard(self) -> ScoreboardsHelper:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
+
+		Returns:
+			the scoreboard including this team. 
 		"""
 		pass
 
 	@overload
-	def getXPProgress(self) -> float:
+	def getPrefix(self) -> TextHelper:
 		"""
-		Since: 1.6.5 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def getXPToLevelUp(self) -> int:
+	def getSuffix(self) -> TextHelper:
 		"""
-		Since: 1.6.5 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def isSleeping(self) -> bool:
+	def getCollisionRule(self) -> str:
 		"""
-		Since: 1.2.5 [citation needed] 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def isSleepingLongEnough(self) -> bool:
+	def isFriendlyFire(self) -> bool:
 		"""
-		Since: 1.2.5 [citation needed] 
+		Since: 1.3.0 
+		"""
+		pass
 
-		Returns:
-			if the player has slept the minimum ammount of time to pass the night. 
+	@overload
+	def showFriendlyInvisibles(self) -> bool:
+		"""
+		Since: 1.3.0 
+		"""
+		pass
+
+	@overload
+	def nametagVisibility(self) -> str:
+		"""
+		Since: 1.3.0 
+		"""
+		pass
+
+	@overload
+	def deathMessageVisibility(self) -> str:
+		"""
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerInput.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerInput.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PlayerListEntryHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptScreen.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,59 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
-
-PlayerListEntry = TypeVar["net.minecraft.client.network.PlayerListEntry"]
-
-class PlayerListEntryHelper(BaseHelper):
-	"""
-	Since: 1.0.2 
+from .BaseScreen import BaseScreen
+from .IScreen import IScreen
+from .MethodWrapper import MethodWrapper
+
+MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+
+class ScriptScreen(BaseScreen):
+	"""just go look at IScreen since all the methods are done through a mixin...\n
+	Since: 1.0.5 
 	"""
+	drawTitle: bool
+	shouldCloseOnEsc: bool
+	shouldPause: bool
 
 	@overload
-	def __init__(self, p: PlayerListEntry) -> None:
+	def __init__(self, title: str, dirt: bool) -> None:
 		pass
 
 	@overload
-	def getUUID(self) -> str:
-		"""
-		Since: 1.1.9 
+	def setParent(self, parent: IScreen) -> None:
 		"""
-		pass
+		Since: 1.4.0 
 
-	@overload
-	def getName(self) -> str:
-		"""
-		Since: 1.0.2 
+		Args:
+			parent: parent screen to go to when this one exits. 
 		"""
 		pass
 
 	@overload
-	def getPing(self) -> int:
-		"""
-		Since: 1.6.5 
+	def setOnRender(self, onRender: MethodWrapper) -> None:
+		"""add custom stuff to the render function on the main thread.\n
+		Since: 1.4.0 
+
+		Args:
+			onRender: pos3d elements are mousex, mousey, tickDelta 
 		"""
 		pass
 
 	@overload
-	def getGamemode(self) -> str:
-		"""
-		Since: 1.6.5 
-
-		Returns:
-			null if unknown 
-		"""
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
-	def getDisplayText(self) -> TextHelper:
-		"""
-		Since: 1.1.9 
-		"""
+	def close(self) -> None:
 		pass
 
 	@overload
-	def getPublicKey(self) -> List[float]:
-		"""
-		Since: 1.8.2 
-		"""
+	def shouldPause(self) -> bool:
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def shouldCloseOnEsc(self) -> bool:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Plane3D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Scrollbar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from typing import overload
-from .PositionCommon_Vec3D import PositionCommon_Vec3D
+from typing import TypeVar
 
+Consumer = TypeVar["java.util.function.Consumer_java.lang.Double_"]
+MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
 
-class PositionCommon_Plane3D:
-	"""
-	Since: 1.6.5 
-	"""
-	x1: float
-	y1: float
-	z1: float
-	x2: float
-	y2: float
-	z2: float
-	x3: float
-	y3: float
-	z3: float
+class Scrollbar(ClickableWidget):
 
 	@overload
-	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, x3: float, y3: float, z3: float) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, color: int, borderColor: int, highlightColor: int, scrollPages: float, onChange: Consumer) -> None:
 		pass
 
 	@overload
-	def getNormalVector(self) -> PositionCommon_Vec3D:
+	def setPos(self, x: int, y: int, width: int, height: int) -> "Scrollbar":
 		pass
 
 	@overload
-	def getVec12(self) -> PositionCommon_Vec3D:
+	def setScrollPages(self, scrollPages: float) -> None:
 		pass
 
 	@overload
-	def getVec13(self) -> PositionCommon_Vec3D:
+	def scrollToPercent(self, percent: float) -> None:
 		pass
 
 	@overload
-	def getVec23(self) -> PositionCommon_Vec3D:
+	def onClick(self, mouseX: float, mouseY: float) -> None:
+		pass
+
+	@overload
+	def onChange(self) -> None:
+		pass
+
+	@overload
+	def mouseDragged(self, mouseX: float, mouseY: float, button: int, deltaX: float, deltaY: float) -> bool:
+		pass
+
+	@overload
+	def renderButton(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Pos2D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FPositionCommon.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,109 @@
 from typing import overload
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
-from .PositionCommon_Vec2D import PositionCommon_Vec2D
+from .BaseLibrary import BaseLibrary
+from .Vec3D import Vec3D
+from .EntityHelper import EntityHelper
+from .Vec2D import Vec2D
+from .Pos3D import Pos3D
+from .Pos2D import Pos2D
+from .BlockPosHelper import BlockPosHelper
 
 
-class PositionCommon_Pos2D:
+class FPositionCommon(BaseLibrary):
+	"""position helper classes\n
+	Since: 1.6.3 
 	"""
-	Since: 1.2.6 [citation needed] 
-	"""
-	ZERO: "PositionCommon_Pos2D"
-	x: float
-	y: float
-
-	@overload
-	def __init__(self, x: float, y: float) -> None:
-		pass
 
 	@overload
-	def getX(self) -> float:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def getY(self) -> float:
-		pass
-
-	@overload
-	def add(self, pos: "PositionCommon_Pos2D") -> "PositionCommon_Pos2D":
-		pass
-
-	@overload
-	def add(self, x: float, y: float) -> "PositionCommon_Pos2D":
-		"""
+	def createVec(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> Vec3D:
+		"""create a new vector object\n
 		Since: 1.6.3 
 
 		Args:
-			x: 
-			y: 
+			z1: 
+			y1: 
+			z2: 
+			x1: 
+			y2: 
+			x2: 
 		"""
 		pass
 
 	@overload
-	def multiply(self, pos: "PositionCommon_Pos2D") -> "PositionCommon_Pos2D":
-		pass
-
-	@overload
-	def multiply(self, x: float, y: float) -> "PositionCommon_Pos2D":
+	def createLookingVector(self, entity: EntityHelper) -> Vec3D:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
 		Args:
-			x: 
-			y: 
+			entity: 
 		"""
 		pass
 
 	@overload
-	def scale(self, scale: float) -> "PositionCommon_Pos2D":
+	def createLookingVector(self, yaw: float, pitch: float) -> Vec3D:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
 		Args:
-			scale: 
+			pitch: 
+			yaw: 
 		"""
 		pass
 
 	@overload
-	def toString(self) -> str:
-		pass
-
-	@overload
-	def to3D(self) -> PositionCommon_Pos3D:
-		pass
-
-	@overload
-	def toVector(self) -> PositionCommon_Vec2D:
-		pass
-
-	@overload
-	def toVector(self, start_pos: "PositionCommon_Pos2D") -> PositionCommon_Vec2D:
+	def createVec(self, x1: float, y1: float, x2: float, y2: float) -> Vec2D:
 		"""
-		Since: 1.6.4 
+		Since: 1.6.3 
 
 		Args:
-			start_pos: 
+			y1: 
+			x1: 
+			y2: 
+			x2: 
 		"""
 		pass
 
 	@overload
-	def toVector(self, start_x: float, start_y: float) -> PositionCommon_Vec2D:
+	def createPos(self, x: float, y: float, z: float) -> Pos3D:
 		"""
-		Since: 1.6.4 
+		Since: 1.6.3 
 
 		Args:
-			start_x: 
-			start_y: 
-		"""
-		pass
-
-	@overload
-	def toReverseVector(self) -> PositionCommon_Vec2D:
-		"""
-		Since: 1.6.4 
+			x: 
+			y: 
+			z: 
 		"""
 		pass
 
 	@overload
-	def toReverseVector(self, end_pos: "PositionCommon_Pos2D") -> PositionCommon_Vec2D:
+	def createPos(self, x: float, y: float) -> Pos2D:
 		"""
-		Since: 1.6.4 
+		Since: 1.6.3 
 
 		Args:
-			end_pos: 
+			x: 
+			y: 
 		"""
 		pass
 
 	@overload
-	def toReverseVector(self, end_x: float, end_y: float) -> PositionCommon_Vec2D:
+	def createBlockPos(self, x: int, y: int, z: int) -> BlockPosHelper:
 		"""
-		Since: 1.6.4 
+		Since: 1.8.4 
 
 		Args:
-			end_x: 
-			end_y: 
+			x: the x position of the block 
+			y: the y position of the block 
+			z: the z position of the block 
+
+		Returns:
+			a BlockPosHelper for the given coordinates. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Pos3D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Pos2D.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,160 +1,183 @@
 from typing import overload
-from typing import TypeVar
-from .PositionCommon_Pos2D import PositionCommon_Pos2D
-from .PositionCommon_Vec3D import PositionCommon_Vec3D
-from .BlockPosHelper import BlockPosHelper
+from .Pos3D import Pos3D
+from .Vec2D import Vec2D
 
-BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
-Vec3d = TypeVar["net.minecraft.util.math.Vec3d"]
 
-class PositionCommon_Pos3D(PositionCommon_Pos2D):
+class Pos2D:
 	"""
 	Since: 1.2.6 [citation needed] 
 	"""
-	ZERO: "PositionCommon_Pos3D"
-	z: float
+	ZERO: "Pos2D"
+	x: float
+	y: float
 
 	@overload
-	def __init__(self, vec: Vec3d) -> None:
+	def __init__(self, x: float, y: float) -> None:
 		pass
 
 	@overload
-	def __init__(self, x: float, y: float, z: float) -> None:
+	def getX(self) -> float:
 		pass
 
 	@overload
-	def getZ(self) -> float:
+	def getY(self) -> float:
 		pass
 
 	@overload
-	def add(self, pos: "PositionCommon_Pos3D") -> "PositionCommon_Pos3D":
+	def add(self, pos: "Pos2D") -> "Pos2D":
 		pass
 
 	@overload
-	def add(self, x: float, y: float, z: float) -> "PositionCommon_Pos3D":
+	def add(self, x: float, y: float) -> "Pos2D":
 		"""
 		Since: 1.6.3 
 
 		Args:
 			x: 
 			y: 
-			z: 
 		"""
 		pass
 
 	@overload
-	def multiply(self, pos: "PositionCommon_Pos3D") -> "PositionCommon_Pos3D":
+	def sub(self, pos: "Pos2D") -> "Pos2D":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			pos: the position to subtract 
+
+		Returns:
+			the new position. 
+		"""
+		pass
+
+	@overload
+	def sub(self, x: float, y: float) -> "Pos2D":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			x: the x coordinate to subtract 
+			y: the y coordinate to subtract 
+
+		Returns:
+			the new position. 
+		"""
 		pass
 
 	@overload
-	def multiply(self, x: float, y: float, z: float) -> "PositionCommon_Pos3D":
+	def multiply(self, pos: "Pos2D") -> "Pos2D":
+		pass
+
+	@overload
+	def multiply(self, x: float, y: float) -> "Pos2D":
 		"""
 		Since: 1.6.3 
 
 		Args:
 			x: 
 			y: 
-			z: 
 		"""
 		pass
 
 	@overload
-	def scale(self, scale: float) -> "PositionCommon_Pos3D":
+	def divide(self, pos: "Pos2D") -> "Pos2D":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			pos: the position to divide by 
+
+		Returns:
+			the new position. 
+		"""
+		pass
+
+	@overload
+	def divide(self, x: float, y: float) -> "Pos2D":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			x: the x coordinate to divide by 
+			y: the y coordinate to divide by 
+
+		Returns:
+			the new position. 
+		"""
+		pass
+
+	@overload
+	def scale(self, scale: float) -> "Pos2D":
 		"""
 		Since: 1.6.3 
 
 		Args:
 			scale: 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
 	@overload
-	def toVector(self) -> PositionCommon_Vec3D:
+	def to3D(self) -> Pos3D:
 		pass
 
 	@overload
-	def toVector(self, start_pos: PositionCommon_Pos2D) -> PositionCommon_Vec3D:
-		"""
-		Since: 1.6.4 
-
-		Args:
-			start_pos: 
-		"""
+	def toVector(self) -> Vec2D:
 		pass
 
 	@overload
-	def toVector(self, start_pos: "PositionCommon_Pos3D") -> PositionCommon_Vec3D:
+	def toVector(self, start_pos: "Pos2D") -> Vec2D:
 		"""
 		Since: 1.6.4 
 
 		Args:
 			start_pos: 
 		"""
 		pass
 
 	@overload
-	def toVector(self, start_x: float, start_y: float, start_z: float) -> PositionCommon_Vec3D:
+	def toVector(self, start_x: float, start_y: float) -> Vec2D:
 		"""
 		Since: 1.6.4 
 
 		Args:
 			start_x: 
-			start_z: 
 			start_y: 
 		"""
 		pass
 
 	@overload
-	def toReverseVector(self) -> PositionCommon_Vec3D:
+	def toReverseVector(self) -> Vec2D:
 		"""
 		Since: 1.6.4 
 		"""
 		pass
 
 	@overload
-	def toReverseVector(self, end_pos: PositionCommon_Pos2D) -> PositionCommon_Vec3D:
-		pass
-
-	@overload
-	def toReverseVector(self, end_pos: "PositionCommon_Pos3D") -> PositionCommon_Vec3D:
+	def toReverseVector(self, end_pos: "Pos2D") -> Vec2D:
 		"""
 		Since: 1.6.4 
 
 		Args:
 			end_pos: 
 		"""
 		pass
 
 	@overload
-	def toReverseVector(self, end_x: float, end_y: float, end_z: float) -> PositionCommon_Vec3D:
+	def toReverseVector(self, end_x: float, end_y: float) -> Vec2D:
 		"""
 		Since: 1.6.4 
 
 		Args:
-			end_z: 
 			end_x: 
 			end_y: 
 		"""
 		pass
 
-	@overload
-	def toBlockPos(self) -> BlockPosHelper:
-		"""
-		Since: 1.8.0 
-		"""
-		pass
-
-	@overload
-	def toRawBlockPos(self) -> BlockPos:
-		"""
-		Since: 1.8.0 
-		"""
-		pass
-
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Vec2D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AdvancementProgressHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,152 @@
 from typing import overload
-from .PositionCommon_Pos2D import PositionCommon_Pos2D
-from .PositionCommon_Vec3D import PositionCommon_Vec3D
+from typing import List
+from typing import TypeVar
+from typing import Mapping
+from .BaseHelper import BaseHelper
 
+AdvancementProgress = TypeVar["net.minecraft.advancement.AdvancementProgress"]
+Date = TypeVar["java.util.Date"]
 
-class PositionCommon_Vec2D:
+class AdvancementProgressHelper(BaseHelper):
 	"""
-	Since: 1.2.6 [citation needed] 
+	Since: 1.8.4 
 	"""
-	x1: float
-	y1: float
-	x2: float
-	y2: float
 
 	@overload
-	def __init__(self, x1: float, y1: float, x2: float, y2: float) -> None:
+	def __init__(self, base: AdvancementProgress) -> None:
 		pass
 
 	@overload
-	def __init__(self, start: PositionCommon_Pos2D, end: PositionCommon_Pos2D) -> None:
-		pass
+	def isDone(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getX1(self) -> float:
+		Returns:
+			'true' if the advancement is finished, 'false' otherwise. 
+		"""
 		pass
 
 	@overload
-	def getY1(self) -> float:
-		pass
+	def isAnyObtained(self) -> bool:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getX2(self) -> float:
+		Returns:
+			'true' if any criteria has already been met, 'false' otherwise. 
+		"""
 		pass
 
 	@overload
-	def getY2(self) -> float:
-		pass
+	def getCriteria(self) -> Mapping[str, Date]:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getDeltaX(self) -> float:
+		Returns:
+			a map of all criteria and their completion date. 
+		"""
 		pass
 
 	@overload
-	def getDeltaY(self) -> float:
-		pass
+	def getRequirements(self) -> List[List[str]]:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getStart(self) -> PositionCommon_Pos2D:
+		Returns:
+			all requirements of this advancement. 
+		"""
 		pass
 
 	@overload
-	def getEnd(self) -> PositionCommon_Pos2D:
-		pass
+	def getPercentage(self) -> float:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getMagnitude(self) -> float:
+		Returns:
+			the percentage of finished requirements. 
+		"""
 		pass
 
 	@overload
-	def getMagnitudeSq(self) -> float:
+	def getFraction(self) -> str:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			magnitude squared 
+			the fraction of finished requirements to total requirements. 
 		"""
 		pass
 
 	@overload
-	def add(self, vec: "PositionCommon_Vec2D") -> "PositionCommon_Vec2D":
-		pass
-
-	@overload
-	def add(self, x1: float, y1: float, x2: float, y2: float) -> "PositionCommon_Vec2D":
+	def countObtainedRequirements(self) -> int:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
-		Args:
-			y1: 
-			x1: 
-			y2: 
-			x2: 
+		Returns:
+			the amount of requirements criteria. 
 		"""
 		pass
 
 	@overload
-	def multiply(self, vec: "PositionCommon_Vec2D") -> "PositionCommon_Vec2D":
+	def getUnobtainedCriteria(self) -> List[str]:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the amount of missing criteria. 
+		"""
 		pass
 
 	@overload
-	def multiply(self, x1: float, y1: float, x2: float, y2: float) -> "PositionCommon_Vec2D":
+	def getObtainedCriteria(self) -> List[str]:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
-		Args:
-			y1: 
-			x1: 
-			y2: 
-			x2: 
+		Returns:
+			the ids of the finished requirements. 
 		"""
 		pass
 
 	@overload
-	def scale(self, scale: float) -> "PositionCommon_Vec2D":
+	def getEarliestProgressObtainDate(self) -> Date:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
 
-		Args:
-			scale: 
+		Returns:
+			the earliest completion date of all criteria. 
 		"""
 		pass
 
 	@overload
-	def dotProduct(self, vec: "PositionCommon_Vec2D") -> float:
-		pass
+	def getCriterionProgress(self, criteria: str) -> Date:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def reverse(self) -> "PositionCommon_Vec2D":
+		Args:
+			criteria: the criteria 
+
+		Returns:
+			the completion date of the given criteria or 'null' if the criteria is not met
+yet. 
+		"""
 		pass
 
 	@overload
-	def normalize(self) -> "PositionCommon_Vec2D":
+	def isCriteriaObtained(self, criteria: str) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
+
+		Args:
+			criteria: the criteria 
 
 		Returns:
-			a new Vec2D with the same direction but a magnitude of 1 
+			'true' if the given criteria is met, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
-	@overload
-	def to3D(self) -> PositionCommon_Vec3D:
-		pass
-
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PositionCommon_Vec3D.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Pos3D.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,183 +1,226 @@
 from typing import overload
 from typing import TypeVar
-from .PositionCommon_Vec2D import PositionCommon_Vec2D
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
+from .Pos2D import Pos2D
+from .Vec3D import Vec3D
+from .BlockPosHelper import BlockPosHelper
 
-Vec3f = TypeVar["net.minecraft.util.math.Vec3f"]
+BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
+Vec3d = TypeVar["net.minecraft.util.math.Vec3d"]
 
-class PositionCommon_Vec3D(PositionCommon_Vec2D):
+class Pos3D(Pos2D):
 	"""
 	Since: 1.2.6 [citation needed] 
 	"""
-	z1: float
-	z2: float
+	ZERO: "Pos3D"
+	z: float
 
 	@overload
-	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> None:
+	def __init__(self, vec: Vec3d) -> None:
 		pass
 
 	@overload
-	def __init__(self, start: PositionCommon_Pos3D, end: PositionCommon_Pos3D) -> None:
+	def __init__(self, x: float, y: float, z: float) -> None:
 		pass
 
 	@overload
-	def getZ1(self) -> float:
+	def getZ(self) -> float:
 		pass
 
 	@overload
-	def getZ2(self) -> float:
+	def add(self, pos: "Pos3D") -> "Pos3D":
 		pass
 
 	@overload
-	def getDeltaZ(self) -> float:
-		pass
-
-	@overload
-	def getStart(self) -> PositionCommon_Pos3D:
-		pass
+	def add(self, x: float, y: float, z: float) -> "Pos3D":
+		"""
+		Since: 1.6.3 
 
-	@overload
-	def getEnd(self) -> PositionCommon_Pos3D:
+		Args:
+			x: 
+			y: 
+			z: 
+		"""
 		pass
 
 	@overload
-	def getMagnitude(self) -> float:
-		pass
+	def sub(self, pos: "Pos3D") -> "Pos3D":
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getMagnitudeSq(self) -> float:
-		pass
+		Args:
+			pos: the position to subtract 
 
-	@overload
-	def add(self, vec: "PositionCommon_Vec3D") -> "PositionCommon_Vec3D":
+		Returns:
+			the new position. 
+		"""
 		pass
 
 	@overload
-	def addStart(self, pos: PositionCommon_Pos3D) -> "PositionCommon_Vec3D":
+	def sub(self, x: float, y: float, z: float) -> "Pos3D":
 		"""
-		Since: 1.6.4 
+		Since: 1.8.4 
 
 		Args:
-			pos: 
+			x: the x coordinate to subtract 
+			y: the y coordinate to subtract 
+			z: the z coordinate to subtract 
+
+		Returns:
+			the new position. 
 		"""
 		pass
 
 	@overload
-	def addEnd(self, pos: PositionCommon_Pos3D) -> "PositionCommon_Vec3D":
+	def multiply(self, pos: "Pos3D") -> "Pos3D":
+		pass
+
+	@overload
+	def multiply(self, x: float, y: float, z: float) -> "Pos3D":
 		"""
-		Since: 1.6.4 
+		Since: 1.6.3 
 
 		Args:
-			pos: 
+			x: 
+			y: 
+			z: 
 		"""
 		pass
 
 	@overload
-	def addStart(self, x: float, y: float, z: float) -> "PositionCommon_Vec3D":
+	def divide(self, pos: "Pos3D") -> "Pos3D":
 		"""
-		Since: 1.6.4 
+		Since: 1.8.4 
 
 		Args:
-			x: 
-			y: 
-			z: 
+			pos: the position to divide by 
+
+		Returns:
+			the new position. 
 		"""
 		pass
 
 	@overload
-	def addEnd(self, x: float, y: float, z: float) -> "PositionCommon_Vec3D":
+	def divide(self, x: float, y: float, z: float) -> "Pos3D":
 		"""
-		Since: 1.6.4 
+		Since: 1.8.4 
 
 		Args:
-			x: 
-			y: 
-			z: 
+			x: the x coordinate to divide by 
+			y: the y coordinate to divide by 
+			z: the z coordinate to divide by 
+
+		Returns:
+			the new position. 
 		"""
 		pass
 
 	@overload
-	def add(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> "PositionCommon_Vec3D":
+	def scale(self, scale: float) -> "Pos3D":
 		"""
 		Since: 1.6.3 
 
 		Args:
-			z1: 
-			y1: 
-			z2: 
-			x1: 
-			y2: 
-			x2: 
+			scale: 
 		"""
 		pass
 
 	@overload
-	def multiply(self, vec: "PositionCommon_Vec3D") -> "PositionCommon_Vec3D":
+	def toString(self) -> str:
 		pass
 
 	@overload
-	def multiply(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> "PositionCommon_Vec3D":
+	def toVector(self) -> Vec3D:
+		pass
+
+	@overload
+	def toVector(self, start_pos: Pos2D) -> Vec3D:
 		"""
-		Since: 1.6.3 
+		Since: 1.6.4 
 
 		Args:
-			z1: 
-			y1: 
-			z2: 
-			x1: 
-			y2: 
-			x2: 
+			start_pos: 
 		"""
 		pass
 
 	@overload
-	def scale(self, scale: float) -> "PositionCommon_Vec3D":
+	def toVector(self, start_pos: "Pos3D") -> Vec3D:
 		"""
-		Since: 1.6.3 
+		Since: 1.6.4 
 
 		Args:
-			scale: 
+			start_pos: 
 		"""
 		pass
 
 	@overload
-	def normalize(self) -> "PositionCommon_Vec3D":
+	def toVector(self, start_x: float, start_y: float, start_z: float) -> Vec3D:
 		"""
-		Since: 1.6.5 
+		Since: 1.6.4 
+
+		Args:
+			start_x: 
+			start_z: 
+			start_y: 
 		"""
 		pass
 
 	@overload
-	def getPitch(self) -> float:
+	def toReverseVector(self) -> Vec3D:
+		"""
+		Since: 1.6.4 
+		"""
 		pass
 
 	@overload
-	def getYaw(self) -> float:
+	def toReverseVector(self, end_pos: Pos2D) -> Vec3D:
 		pass
 
 	@overload
-	def dotProduct(self, vec: "PositionCommon_Vec3D") -> float:
+	def toReverseVector(self, end_pos: "Pos3D") -> Vec3D:
+		"""
+		Since: 1.6.4 
+
+		Args:
+			end_pos: 
+		"""
 		pass
 
 	@overload
-	def crossProduct(self, vec: "PositionCommon_Vec3D") -> "PositionCommon_Vec3D":
+	def toReverseVector(self, end_x: float, end_y: float, end_z: float) -> Vec3D:
+		"""
+		Since: 1.6.4 
+
+		Args:
+			end_z: 
+			end_x: 
+			end_y: 
+		"""
 		pass
 
 	@overload
-	def reverse(self) -> "PositionCommon_Vec3D":
+	def toBlockPos(self) -> BlockPosHelper:
+		"""
+		Since: 1.8.0 
+		"""
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def toRawBlockPos(self) -> BlockPos:
+		"""
+		Since: 1.8.0 
+		"""
 		pass
 
 	@overload
-	def toMojangFloatVector(self) -> Vec3f:
+	def toMojangDoubleVector(self) -> Vec3d:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
+
+		Returns:
+			the raw minecraft double vector with the same coordinates as this position. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PrimitiveSettingGroup.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/PrimitiveSettingGroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 		pass
 
 	@overload
 	def onScrollbar(self, page: float) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def addSetting(self, setting: SettingsOverlay_SettingField) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/PrioryFiFoTaskQueue.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/PrioryFiFoTaskQueue.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Prism.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Prism.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 from typing import TypeVar
 from typing import Set
 
 Prism4j_Grammar = TypeVar["io.noties.prism4j.Prism4j.Grammar"]
 Prism4j_Node = TypeVar["io.noties.prism4j.Prism4j.Node"]
 GrammarLocator = TypeVar["io.noties.prism4j.GrammarLocator"]
+Prism4j = TypeVar["io.noties.prism4j.Prism4j"]
 
 class Prism(GrammarLocator):
 
 	@overload
 	def __init__(self) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Profile.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Profile.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProfileSetting.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProfileSetting.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProfileSetting_ProfileEntry.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProfileSetting_ProfileEntry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ProxyBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ProxyBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/RecipeHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/LockButtonWidgetHelper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .ItemStackHelper import ItemStackHelper
+from .ClickableWidgetHelper import ClickableWidgetHelper
 
-Recipe = TypeVar["net.minecraft.recipe.Recipe__"]
+LockButtonWidget = TypeVar["net.minecraft.client.gui.widget.LockButtonWidget"]
 
-class RecipeHelper(BaseHelper):
+class LockButtonWidgetHelper(ClickableWidgetHelper):
 	"""
-	Since: 1.3.1 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: Recipe, syncId: int) -> None:
+	def __init__(self, btn: LockButtonWidget) -> None:
 		pass
 
 	@overload
-	def getId(self) -> str:
-		"""
-		Since: 1.3.1 
-		"""
+	def __init__(self, btn: LockButtonWidget, zIndex: int) -> None:
 		pass
 
 	@overload
-	def getIngredients(self) -> List[List[ItemStackHelper]]:
-		"""get ingredients list\n
-		Since: 1.8.3 
+	def isLocked(self) -> bool:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getOutput(self) -> ItemStackHelper:
-		"""
-		Since: 1.3.1 
+		Returns:
+			'true' if the button is locked, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def craft(self, craftAll: bool) -> None:
+	def setLocked(self, locked: bool) -> "LockButtonWidgetHelper":
 		"""
-		Since: 1.3.1 
+		Since: 1.8.4 
 
 		Args:
-			craftAll: 
+			locked: whether to lock the button or not 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Image.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Slider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,68 @@
 from typing import overload
 from typing import TypeVar
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
 
+Consumer = TypeVar["java.util.function.Consumer_xyz.wagyourtail.wagyourgui.elements.Slider_"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
+Text = TypeVar["net.minecraft.text.Text"]
 
-class RenderCommon_Image(RenderCommon_RenderElement):
+class Slider(ClickableWidget):
 	"""
-	Since: 1.2.3 
+	Since: 1.8.4 
 	"""
-	rotation: float
-	x: int
-	y: int
-	width: int
-	height: int
-	imageX: int
-	imageY: int
-	regionWidth: int
-	regionHeight: int
-	textureWidth: int
-	textureHeight: int
-	color: int
-	zIndex: int
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, zIndex: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, text: Text, value: float, action: Consumer, steps: int) -> None:
 		pass
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, zIndex: int, alpha: int, color: int, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int, rotation: float) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, text: Text, value: float, action: Consumer) -> None:
 		pass
 
 	@overload
-	def setColor(self, color: int) -> "RenderCommon_Image":
-		"""
-		Since: 1.6.5 
-
-		Args:
-			color: 
-		"""
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
-	def setColor(self, color: int, alpha: int) -> "RenderCommon_Image":
-		"""
-		Since: 1.6.5 
-
-		Args:
-			color: 
-			alpha: 
-		"""
+	def roundValue(self, value: float) -> float:
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
-		"""
-		Since: 1.2.3 
+	def getValue(self) -> float:
+		pass
 
-		Args:
-			x: 
-			width: 
-			y: 
-			height: 
-		"""
+	@overload
+	def setValue(self, mouseX: float) -> None:
 		pass
 
 	@overload
-	def setRotation(self, rotation: float) -> "RenderCommon_Image":
-		"""
-		Since: 1.2.6 
+	def getSteps(self) -> int:
+		pass
 
-		Args:
-			rotation: 
-		"""
+	@overload
+	def setSteps(self, steps: int) -> None:
 		pass
 
 	@overload
-	def setImage(self, id: str, imageX: int, imageY: int, regionWidth: int, regionHeight: int, textureWidth: int, textureHeight: int) -> None:
-		"""
-		Since: 1.2.3 
+	def renderButton(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+		pass
 
-		Args:
-			imageY: 
-			textureWidth: 
-			imageX: 
-			regionHeight: 
-			id: 
-			regionWidth: 
-			textureHeight: 
-		"""
+	@overload
+	def onClick(self, mouseX: float, mouseY: float) -> None:
 		pass
 
 	@overload
-	def getImage(self) -> str:
-		"""
-		Since: 1.2.3 
-		"""
+	def onRelease(self, mouseX: float, mouseY: float) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def setMessage(self, message: str) -> None:
 		pass
 
 	@overload
-	def getZIndex(self) -> int:
+	def setMessage(self, message: Text) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Item.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/RecipeInventory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,149 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
+from typing import Generic
+from .Inventory import Inventory
 from .ItemStackHelper import ItemStackHelper
+from .RecipeHelper import RecipeHelper
 
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-ItemStack = TypeVar["net.minecraft.item.ItemStack"]
+T = TypeVar("T")
 
-class RenderCommon_Item(RenderCommon_RenderElement):
+class RecipeInventory(Generic[T], Inventory):
 	"""
-	Since: 1.0.5 
+	Since: 1.8.4 
 	"""
-	item: ItemStack
-	ovText: str
-	overlay: bool
-	scale: float
-	rotation: float
-	x: int
-	y: int
-	zIndex: int
 
 	@overload
-	def __init__(self, x: int, y: int, zIndex: int, id: str, overlay: bool, scale: float, rotation: float) -> None:
+	def getOutput(self) -> ItemStackHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the output item. 
+		"""
 		pass
 
 	@overload
-	def __init__(self, x: int, y: int, zIndex: int, i: ItemStackHelper, overlay: bool, scale: float, rotation: float) -> None:
+	def getInputSize(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the maximum input size for all recipes in this inventory. 
+		"""
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int) -> "RenderCommon_Item":
+	def getInput(self, x: int, z: int) -> ItemStackHelper:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Args:
-			x: 
-			y: 
+			x: the x position of the input slot, starting at 0, left to right. Must be less than RecipeInventory#getCraftingWidth() 
+			z: the z position of the input slot, starting at 0, top to bottom. Must be less than RecipeInventory#getCraftingHeight() 
+
+		Returns:
+			the input item at the given position. 
 		"""
 		pass
 
 	@overload
-	def setScale(self, scale: float) -> "RenderCommon_Item":
+	def getInput(self) -> List[List[ItemStackHelper]]:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
-		Args:
-			scale: 
+		Returns:
+			the input items of the crafting grid, in a 2d array. 
 		"""
 		pass
 
 	@overload
-	def setRotation(self, rotation: float) -> "RenderCommon_Item":
+	def getCraftingWidth(self) -> int:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
-		Args:
-			rotation: 
+		Returns:
+			the width of the crafting grid. 
 		"""
 		pass
 
 	@overload
-	def setOverlay(self, overlay: bool) -> "RenderCommon_Item":
+	def getCraftingHeight(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
 
-		Args:
-			overlay: 
+		Returns:
+			the height of the crafting grid. 
 		"""
 		pass
 
 	@overload
-	def setOverlayText(self, ovText: str) -> "RenderCommon_Item":
+	def getCraftingSlotCount(self) -> int:
 		"""
-		Since: 1.2.0 
+		Since: 1.8.4 
 
-		Args:
-			ovText: 
+		Returns:
+			the amount of slots used for crafting. 
 		"""
 		pass
 
 	@overload
-	def setItem(self, i: ItemStackHelper) -> "RenderCommon_Item":
+	def getCategory(self) -> str:
 		"""
-		Since: 1.0.5 [citation needed] 
+		Since: 1.8.4 
 
-		Args:
-			i: 
+		Returns:
+			the recipe category of recipes that can be crafted in this inventory. 
 		"""
 		pass
 
 	@overload
-	def setItem(self, id: str, count: int) -> "RenderCommon_Item":
+	def getCraftableRecipes(self) -> List[RecipeHelper]:
 		"""
-		Since: 1.0.5 [citation needed] 
-
-		Args:
-			count: 
-			id: 
+		Since: 1.3.1 
 		"""
 		pass
 
 	@overload
-	def getItem(self) -> ItemStackHelper:
+	def getRecipes(self, craftable: bool) -> List[RecipeHelper]:
 		"""
-		Since: 1.0.5 [citation needed] 
+		Since: 1.8.4 
+
+		Args:
+			craftable: whether only to list craftable recipes 
+
+		Returns:
+			a list of recipes that can be crafted in this inventory. 
 		"""
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def isRecipeBookOpened(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the recipe book is visible, 'false' otherwise. 
+		"""
 		pass
 
 	@overload
-	def render3D(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def toggleRecipeBook(self) -> None:
+		"""
+		Since: 1.8.4 
+		"""
 		pass
 
 	@overload
-	def getZIndex(self) -> int:
+	def setRecipeBook(self, open: bool) -> None:
+		"""
+		Since: 1.8.4 
+
+		Args:
+			open: whether to open or close the recipe book 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Rect.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextInput.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,61 @@
 from typing import overload
 from typing import TypeVar
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
+from .Button import Button
 
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+Consumer = TypeVar["java.util.function.Consumer_java.lang.String_"]
+TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class RenderCommon_Rect(RenderCommon_RenderElement):
-	"""
-	Since: 1.0.5 
-	"""
-	rotation: float
-	x1: int
-	y1: int
-	x2: int
-	y2: int
-	color: int
-	zIndex: int
+class TextInput(Button):
+	onChange: Consumer
+	mask: str
+	content: str
+	selStartIndex: int
+	selEndIndex: int
 
 	@overload
-	def __init__(self, x1: int, y1: int, x2: int, y2: int, color: int, rotation: float, zIndex: int) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: str, onClick: Consumer, onChange: Consumer) -> None:
 		pass
 
 	@overload
-	def __init__(self, x1: int, y1: int, x2: int, y2: int, color: int, alpha: int, rotation: float, zIndex: int) -> None:
+	def setMessage(self, message: str) -> None:
 		pass
 
 	@overload
-	def setColor(self, color: int) -> "RenderCommon_Rect":
-		"""
-		Since: 1.0.5 
-
-		Args:
-			color: 
-		"""
+	def updateSelStart(self, startIndex: int) -> None:
 		pass
 
 	@overload
-	def setColor(self, color: int, alpha: int) -> "RenderCommon_Rect":
-		"""
-		Since: 1.1.8 
-
-		Args:
-			color: 
-			alpha: 
-		"""
+	def updateSelEnd(self, endIndex: int) -> None:
 		pass
 
 	@overload
-	def setAlpha(self, alpha: int) -> "RenderCommon_Rect":
-		"""
-		Since: 1.1.8 
-
-		Args:
-			alpha: 
-		"""
+	def mouseClicked(self, mouseX: float, mouseY: float, button: int) -> bool:
 		pass
 
 	@overload
-	def setPos(self, x1: int, y1: int, x2: int, y2: int) -> "RenderCommon_Rect":
-		"""
-		Since: 1.1.8 
+	def mouseDragged(self, mouseX: float, mouseY: float, button: int, deltaX: float, deltaY: float) -> bool:
+		pass
 
-		Args:
-			y1: 
-			x1: 
-			y2: 
-			x2: 
-		"""
+	@overload
+	def swapStartEnd(self) -> None:
 		pass
 
 	@overload
-	def setRotation(self, rotation: float) -> "RenderCommon_Rect":
-		"""
-		Since: 1.2.6 
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
+		pass
 
-		Args:
-			rotation: 
-		"""
+	@overload
+	def charTyped(self, chr: str, keyCode: int) -> bool:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def clicked(self, mouseX: float, mouseY: float) -> bool:
 		pass
 
 	@overload
-	def getZIndex(self) -> int:
+	def setSelected(self, sel: bool) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/RenderCommon_Text.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StoneCutterInventory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,87 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
-from .TextHelper import TextHelper
+from .Inventory import Inventory
+from .ItemStackHelper import ItemStackHelper
 
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-Text = TypeVar["net.minecraft.text.Text"]
+StonecutterScreen = TypeVar["net.minecraft.client.gui.screen.ingame.StonecutterScreen"]
 
-class RenderCommon_Text(RenderCommon_RenderElement):
+class StoneCutterInventory(Inventory):
 	"""
-	Since: 1.0.5 
+	Since: 1.8.4 
 	"""
-	text: Text
-	scale: float
-	rotation: float
-	x: int
-	y: int
-	color: int
-	width: int
-	shadow: bool
-	zIndex: int
 
 	@overload
-	def __init__(self, text: str, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> None:
+	def __init__(self, inventory: StonecutterScreen) -> None:
 		pass
 
 	@overload
-	def __init__(self, text: TextHelper, x: int, y: int, color: int, zIndex: int, shadow: bool, scale: float, rotation: float) -> None:
-		pass
-
-	@overload
-	def setScale(self, scale: float) -> "RenderCommon_Text":
+	def getSelectedRecipeIndex(self) -> int:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			scale: 
+		Returns:
+			the selected recipe index. 
 		"""
 		pass
 
 	@overload
-	def setRotation(self, rotation: float) -> "RenderCommon_Text":
+	def getOutput(self) -> ItemStackHelper:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			rotation: 
+		Returns:
+			the output item for the selected recipe. 
 		"""
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int) -> "RenderCommon_Text":
+	def selectRecipe(self, idx: int) -> "StoneCutterInventory":
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Args:
-			x: 
-			y: 
+			idx: the index to select 
+
+		Returns:
+			self for chaining. 
 		"""
 		pass
 
 	@overload
-	def setText(self, text: str) -> "RenderCommon_Text":
+	def getAvailableRecipeCount(self) -> int:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			text: 
+		Returns:
+			the amount of available recipes. 
 		"""
 		pass
 
 	@overload
-	def setText(self, text: TextHelper) -> "RenderCommon_Text":
+	def getRecipes(self) -> List[ItemStackHelper]:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			text: 
+		Returns:
+			a list of all available recipe results in the form of item stacks. 
 		"""
 		pass
 
 	@overload
-	def getText(self) -> TextHelper:
-		"""
-		Since: 1.2.7 
+	def canCraft(self) -> bool:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getWidth(self) -> int:
-		"""
-		Since: 1.0.5 
+		Returns:
+			'true' if there is a selected recipe, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
-		pass
-
-	@overload
-	def render3D(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
-		pass
-
-	@overload
-	def getZIndex(self) -> int:
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/RunningContextContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/RunningContextContainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 		pass
 
 	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScoreboardObjectiveHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScoreboardObjectiveHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,10 +62,14 @@
 		Since: 1.2.9 
 
 		Returns:
 			name of scoreboard 
 		"""
 		pass
 
+	@overload
+	def toString(self) -> str:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScoreboardsHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerInventory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,91 @@
 from typing import overload
-from typing import List
-from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .ScoreboardObjectiveHelper import ScoreboardObjectiveHelper
-from .PlayerEntityHelper import PlayerEntityHelper
-from .TeamHelper import TeamHelper
+from .RecipeInventory import RecipeInventory
+from .ItemStackHelper import ItemStackHelper
 
-Scoreboard = TypeVar["net.minecraft.scoreboard.Scoreboard"]
 
-class ScoreboardsHelper(BaseHelper):
+class PlayerInventory(RecipeInventory):
 	"""
-	Since: 1.2.9 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, board: Scoreboard) -> None:
-		pass
-
-	@overload
-	def getObjectiveForTeamColorIndex(self, index: int) -> ScoreboardObjectiveHelper:
+	def getInput(self, x: int, y: int) -> ItemStackHelper:
 		"""
-		Since: 1.2.9 
+		Since: 1.8.4 
 
 		Args:
-			index: 
-		"""
-		pass
-
-	@overload
-	def getObjectiveSlot(self, slot: int) -> ScoreboardObjectiveHelper:
-		"""'0' is tab list, '1' or '3 + getPlayerTeamColorIndex()' is sidebar, '2' should be below name.
-therefore max slot number is 18.\n
-		Since: 1.2.9 
+			x: the x position of the input from 0 to 1, going left to right 
+			y: the y position of the input from 0 to 1, going top to bottom 
 
-		Args:
-			slot: 
+		Returns:
+			the input item at the given position of the crafting grid. 
 		"""
 		pass
 
 	@overload
-	def getPlayerTeamColorIndex(self, entity: PlayerEntityHelper) -> int:
+	def isInHotbar(self, slot: int) -> bool:
 		"""
-		Since: 1.2.9 
+		Since: 1.8.4 
 
 		Args:
-			entity: 
+			slot: the slot to check 
+
+		Returns:
+			'true' if the slot is in the hotbar or the offhand slot, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getPlayerTeamColorIndex(self) -> int:
+	def getOffhand(self) -> ItemStackHelper:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			team index for client player 
+			the item in the offhand. 
 		"""
 		pass
 
 	@overload
-	def getTeams(self) -> List[TeamHelper]:
+	def getHelmet(self) -> ItemStackHelper:
 		"""
-		Since: 1.3.0 
+		Since: 1.8.4 
+
+		Returns:
+			the equipped helmet item. 
 		"""
 		pass
 
 	@overload
-	def getPlayerTeam(self, p: PlayerEntityHelper) -> TeamHelper:
+	def getChestplate(self) -> ItemStackHelper:
 		"""
-		Since: 1.3.0 
+		Since: 1.8.4 
 
-		Args:
-			p: 
+		Returns:
+			the equipped chestplate item. 
 		"""
 		pass
 
 	@overload
-	def getPlayerTeam(self) -> TeamHelper:
+	def getLeggings(self) -> ItemStackHelper:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			team for client player 
+			the equipped leggings item. 
 		"""
 		pass
 
 	@overload
-	def getCurrentScoreboard(self) -> ScoreboardObjectiveHelper:
+	def getBoots(self) -> ItemStackHelper:
 		"""
-		Since: 1.2.9 
+		Since: 1.8.4 
 
 		Returns:
-			the ScoreboardObjectiveHelper for the currently displayed sidebar scoreboard. 
+			the equipped boots item. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptCodeCompiler.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/DefaultCodeCompiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 from typing import TypeVar
 from typing import Mapping
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
 Runnable = TypeVar["java.lang.Runnable"]
-File = TypeVar["java.io.File"]
+Text = TypeVar["net.minecraft.text.Text"]
 
-class ScriptCodeCompiler(AbstractRenderCodeCompiler):
-	"""
-	"""
+class DefaultCodeCompiler(AbstractRenderCodeCompiler):
 
 	@overload
-	def __init__(self, language: str, screen: EditorScreen, scriptFile: File) -> None:
+	def __init__(self, language: str, screen: EditorScreen) -> None:
 		pass
 
 	@overload
 	def recompileRenderedText(self, text: str) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceContainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import overload
 from typing import TypeVar
-from .BaseScreen import BaseScreen
-from .IScreen import IScreen
-from .MethodWrapper import MethodWrapper
+from .MultiElementContainer import MultiElementContainer
+from .ServiceScreen import ServiceScreen
+from .ServiceTrigger import ServiceTrigger
 
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
+File = TypeVar["java.io.File"]
+TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class ScriptScreen(BaseScreen):
-	"""just go look at IScreen since all the methods are done through a mixin...\n
-	Since: 1.0.5 
-	"""
+class ServiceContainer(MultiElementContainer):
+	service: str
 
 	@overload
-	def __init__(self, title: str, dirt: bool) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: ServiceScreen, service: str) -> None:
 		pass
 
 	@overload
-	def setParent(self, parent: IScreen) -> None:
-		"""
-		Since: 1.4.0 
+	def init(self) -> None:
+		pass
 
-		Args:
-			parent: parent screen to go to when this one exits. 
-		"""
+	@overload
+	def getEnabled(self) -> bool:
 		pass
 
 	@overload
-	def setOnRender(self, onRender: MethodWrapper) -> None:
-		"""add custom stuff to the render function on the main thread.\n
-		Since: 1.4.0 
+	def getRunning(self) -> bool:
+		pass
 
-		Args:
-			onRender: pos3d elements are mousex, mousey, tickDelta 
-		"""
+	@overload
+	def getTrigger(self) -> ServiceTrigger:
+		pass
+
+	@overload
+	def setFile(self, file: File) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def close(self) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ScriptTrigger.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ScriptTrigger.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Scrollbar.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Vec2D.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,141 @@
 from typing import overload
-from typing import TypeVar
+from .Pos2D import Pos2D
+from .Vec3D import Vec3D
 
-NarrationMessageBuilder = TypeVar["net.minecraft.client.gui.screen.narration.NarrationMessageBuilder"]
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Double_"]
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
 
-class Scrollbar(ClickableWidget):
+class Vec2D:
+	"""
+	Since: 1.2.6 [citation needed] 
+	"""
+	x1: float
+	y1: float
+	x2: float
+	y2: float
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, color: int, borderColor: int, hilightColor: int, scrollPages: float, onChange: Consumer) -> None:
+	def __init__(self, x1: float, y1: float, x2: float, y2: float) -> None:
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> "Scrollbar":
+	def __init__(self, start: Pos2D, end: Pos2D) -> None:
 		pass
 
 	@overload
-	def setScrollPages(self, scrollPages: float) -> None:
+	def getX1(self) -> float:
 		pass
 
 	@overload
-	def scrollToPercent(self, percent: float) -> None:
+	def getY1(self) -> float:
 		pass
 
 	@overload
-	def onClick(self, mouseX: float, mouseY: float) -> None:
+	def getX2(self) -> float:
 		pass
 
 	@overload
-	def onChange(self) -> None:
+	def getY2(self) -> float:
 		pass
 
 	@overload
-	def mouseDragged(self, mouseX: float, mouseY: float, button: int, deltaX: float, deltaY: float) -> bool:
+	def getDeltaX(self) -> float:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def getDeltaY(self) -> float:
 		pass
 
 	@overload
-	def appendNarrations(self, builder: NarrationMessageBuilder) -> None:
+	def getStart(self) -> Pos2D:
+		pass
+
+	@overload
+	def getEnd(self) -> Pos2D:
+		pass
+
+	@overload
+	def getMagnitude(self) -> float:
+		pass
+
+	@overload
+	def getMagnitudeSq(self) -> float:
+		"""
+		Since: 1.6.5 
+
+		Returns:
+			magnitude squared 
+		"""
+		pass
+
+	@overload
+	def add(self, vec: "Vec2D") -> "Vec2D":
+		pass
+
+	@overload
+	def add(self, x1: float, y1: float, x2: float, y2: float) -> "Vec2D":
+		"""
+		Since: 1.6.3 
+
+		Args:
+			y1: 
+			x1: 
+			y2: 
+			x2: 
+		"""
+		pass
+
+	@overload
+	def multiply(self, vec: "Vec2D") -> "Vec2D":
+		pass
+
+	@overload
+	def multiply(self, x1: float, y1: float, x2: float, y2: float) -> "Vec2D":
+		"""
+		Since: 1.6.3 
+
+		Args:
+			y1: 
+			x1: 
+			y2: 
+			x2: 
+		"""
+		pass
+
+	@overload
+	def scale(self, scale: float) -> "Vec2D":
+		"""
+		Since: 1.6.3 
+
+		Args:
+			scale: 
+		"""
+		pass
+
+	@overload
+	def dotProduct(self, vec: "Vec2D") -> float:
+		pass
+
+	@overload
+	def reverse(self) -> "Vec2D":
+		pass
+
+	@overload
+	def normalize(self) -> "Vec2D":
+		"""
+		Since: 1.6.5 
+
+		Returns:
+			a new Vec2D with the same direction but a magnitude of 1 
+		"""
+		pass
+
+	@overload
+	def toString(self) -> str:
+		pass
+
+	@overload
+	def to3D(self) -> Vec3D:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/SelectCursor.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/SelectCursor.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/SelectorDropdownOverlay.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Line3D.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,76 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .OverlayContainer import OverlayContainer
-from .IOverlayParent import IOverlayParent
+from .RenderElement3D import RenderElement3D
+from .Vec3D import Vec3D
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Integer_"]
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+BufferBuilder = TypeVar["net.minecraft.client.render.BufferBuilder"]
 
-class SelectorDropdownOverlay(OverlayContainer):
+class Line3D(RenderElement3D):
+	"""
+	"""
+	pos: Vec3D
+	color: int
+	cull: bool
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, choices: List[Text], textRenderer: TextRenderer, parent: IOverlayParent, onChoice: Consumer) -> None:
+	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, cull: bool) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float, color: int, alpha: int, cull: bool) -> None:
 		pass
 
 	@overload
-	def onScroll(self, page: float) -> None:
+	def setPos(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> None:
+		"""
+		Since: 1.0.6 
+
+		Args:
+			z1: 
+			y1: 
+			z2: 
+			x1: 
+			y2: 
+			x2: 
+		"""
 		pass
 
 	@overload
-	def onClick(self, mouseX: float, mouseY: float, button: int) -> None:
+	def setColor(self, color: int) -> None:
+		"""
+		Since: 1.0.6 
+
+		Args:
+			color: 
+		"""
 		pass
 
 	@overload
-	def setSelected(self, sel: int) -> None:
+	def setColor(self, color: int, alpha: int) -> None:
+		"""
+		Since: 1.1.8 
+
+		Args:
+			color: 
+			alpha: 
+		"""
 		pass
 
 	@overload
-	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
+	def setAlpha(self, alpha: int) -> None:
+		"""
+		Since: 1.1.8 
+
+		Args:
+			alpha: 
+		"""
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, matrixStack: MatrixStack, builder: BufferBuilder, tickDelta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServerInfoHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServerInfoHelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,13 +65,23 @@
 		pass
 
 	@overload
 	def getNbt(self) -> NBTElementHelper:
 		pass
 
 	@overload
+	def isSecureChatEnforced(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the server enforces secure chat, 'false' otherwise. 
+		"""
+		pass
+
+	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceContainer.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BooleanField.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,30 @@
 from typing import overload
 from typing import TypeVar
-from .MultiElementContainer import MultiElementContainer
-from .ServiceScreen import ServiceScreen
-from .ServiceTrigger import ServiceTrigger
+from .AbstractSettingField import AbstractSettingField
+from .AbstractSettingContainer import AbstractSettingContainer
+from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
 MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
-File = TypeVar["java.io.File"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class ServiceContainer(MultiElementContainer):
-	service: str
+class BooleanField(AbstractSettingField):
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: ServiceScreen, service: str) -> None:
+	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def getEnabled(self) -> bool:
+	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def getRunning(self) -> bool:
-		pass
-
-	@overload
-	def getTrigger(self) -> ServiceTrigger:
-		pass
-
-	@overload
-	def setFile(self, file: File) -> None:
-		pass
-
-	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceListTopbar.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceListTopbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/ServiceScreen.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ServiceScreen.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/SettingsOverlay.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/SettingsOverlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 		pass
 
 	@overload
 	def selectCategory(self, category: List[str]) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
 	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/SettingsOverlay_SettingField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/SettingsOverlay_SettingField.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StatusEffectHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/VillagerEntityHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import overload
 from typing import TypeVar
-from .BaseHelper import BaseHelper
+from .MerchantEntityHelper import MerchantEntityHelper
 
-StatusEffectInstance = TypeVar["net.minecraft.entity.effect.StatusEffectInstance"]
+VillagerEntity = TypeVar["net.minecraft.entity.passive.VillagerEntity"]
 
-class StatusEffectHelper(BaseHelper):
+class VillagerEntityHelper(MerchantEntityHelper):
 	"""
-	Since: 1.2.4 
+	Since: 1.6.3 
 	"""
 
 	@overload
-	def __init__(self, s: StatusEffectInstance) -> None:
+	def __init__(self, e: VillagerEntity) -> None:
 		pass
 
 	@overload
-	def getId(self) -> str:
+	def getProfession(self) -> str:
 		"""
-		Since: 1.2.4 
+		Since: 1.6.3 
 		"""
 		pass
 
 	@overload
-	def getStrength(self) -> int:
+	def getStyle(self) -> str:
 		"""
-		Since: 1.2.4 
+		Since: 1.6.3 
 		"""
 		pass
 
 	@overload
-	def getTime(self) -> int:
+	def getLevel(self) -> int:
 		"""
-		Since: 1.2.4 
+		Since: 1.6.3 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringCompareFilter_FilterMethod.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringCompareFilter_FilterMethod.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringField.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringMapSetting_StringEntry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 from typing import overload
 from typing import TypeVar
-from .AbstractSettingField import AbstractSettingField
-from .AbstractSettingContainer import AbstractSettingContainer
-from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
+from .AbstractMapSettingContainer_MapSettingEntry import AbstractMapSettingContainer_MapSettingEntry
+from .StringMapSetting import StringMapSetting
 
-MatrixStack = TypeVar["net.minecraft.client.util.math.MatrixStack"]
 TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
 
-class StringField(AbstractSettingField):
+class StringMapSetting_StringEntry(AbstractMapSettingContainer_MapSettingEntry):
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
+	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: StringMapSetting, key: str, value: str) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
-	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
-		pass
-
-	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
-		pass
-
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringHashTrie.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringHashTrie.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringMapSetting.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringMapSetting.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StringifyFilter.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/StringifyFilter.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/StyleHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/BossBarHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,92 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
+from .FormattingHelper import FormattingHelper
+from .TextHelper import TextHelper
 
-Runnable = TypeVar["java.lang.Runnable"]
-Style = TypeVar["net.minecraft.text.Style"]
+BossBar = TypeVar["net.minecraft.entity.boss.BossBar"]
 
-class StyleHelper(BaseHelper):
+class BossBarHelper(BaseHelper):
 	"""
-	Since: 1.6.5 
+	Since: 1.2.1 
 	"""
 
 	@overload
-	def __init__(self, base: Style) -> None:
+	def __init__(self, b: BossBar) -> None:
 		pass
 
 	@overload
-	def hasColor(self) -> bool:
-		pass
+	def getUUID(self) -> str:
+		"""
+		Since: 1.2.1 
 
-	@overload
-	def getColor(self) -> int:
+		Returns:
+			boss bar uuid. 
+		"""
 		pass
 
 	@overload
-	def hasCustomColor(self) -> bool:
-		pass
+	def getPercent(self) -> float:
+		"""
+		Since: 1.2.1 
 
-	@overload
-	def getCustomColor(self) -> int:
+		Returns:
+			percent of boss bar remaining. 
+		"""
 		pass
 
 	@overload
-	def bold(self) -> bool:
-		pass
+	def getColor(self) -> str:
+		"""
+		Since: 1.2.1 
 
-	@overload
-	def italic(self) -> bool:
+		Returns:
+			boss bar color. 
+		"""
 		pass
 
 	@overload
-	def underlined(self) -> bool:
-		pass
+	def getStyle(self) -> str:
+		"""
+		Since: 1.2.1 
 
-	@overload
-	def strikethrough(self) -> bool:
+		Returns:
+			boss bar notch style. 
+		"""
 		pass
 
 	@overload
-	def obfuscated(self) -> bool:
-		pass
+	def getColorValue(self) -> int:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getClickAction(self) -> str:
-		pass
-
-	@overload
-	def getClickValue(self) -> str:
+		Returns:
+			the color of this boss bar. 
+		"""
 		pass
 
 	@overload
-	def getCustomClickValue(self) -> Runnable:
-		pass
+	def getColorFormat(self) -> FormattingHelper:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def getHoverAction(self) -> str:
+		Returns:
+			the format of the boss bar's color. 
+		"""
 		pass
 
 	@overload
-	def getHoverValue(self) -> object:
-		pass
+	def getName(self) -> TextHelper:
+		"""
+		Since: 1.2.1 
 
-	@overload
-	def getInsertion(self) -> str:
+		Returns:
+			name of boss bar 
+		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/SuggestionsBuilderHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/WrappedClassInstance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
+from typing import Generic
 
-SuggestionsBuilder = TypeVar["com.mojang.brigadier.suggestion.SuggestionsBuilder"]
+T = TypeVar("T")
 
-class SuggestionsBuilderHelper(BaseHelper):
+class WrappedClassInstance(Generic[T]):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
-	def __init__(self, base: SuggestionsBuilder) -> None:
+	def __init__(self, instance: T) -> None:
 		pass
 
 	@overload
-	def getInput(self) -> str:
+	def __init__(self, instanceNullable: T, tClass: Class) -> None:
 		pass
 
 	@overload
-	def getStart(self) -> int:
+	def getFieldValue(self, fieldName: str) -> object:
 		pass
 
 	@overload
-	def getRemaining(self) -> str:
+	def getFieldValueAsClass(self, asClass: str, fieldName: str) -> object:
 		pass
 
 	@overload
-	def getRemainingLowerCase(self) -> str:
+	def setFieldValue(self, fieldName: str, fieldValue: object) -> None:
 		pass
 
 	@overload
-	def suggest(self, suggestion: str) -> "SuggestionsBuilderHelper":
+	def setFieldValueAsClass(self, asClass: str, fieldName: str, fieldValue: object) -> None:
 		pass
 
 	@overload
-	def suggest(self, value: int) -> "SuggestionsBuilderHelper":
+	def invokeMethod(self, methodNameOrSig: str, params: List[object]) -> object:
 		pass
 
 	@overload
-	def suggestWithTooltip(self, suggestion: str, tooltip: TextHelper) -> "SuggestionsBuilderHelper":
+	def invokeMethodAsClass(self, asClass: str, methodNameOrSig: str, params: List[object]) -> object:
 		pass
 
 	@overload
-	def suggestWithTooltip(self, value: int, tooltip: TextHelper) -> "SuggestionsBuilderHelper":
+	def getRawInstance(self) -> T:
+		"""
+		Since: 1.6.5 
+		"""
+		pass
+
+	@overload
+	def getRawClass(self) -> Class:
+		"""
+		Since: 1.6.5 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/SynchronizedWeakHashSet.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/SynchronizedWeakHashSet.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TeamHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/AxolotlEntityHelper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,58 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
+from .AnimalEntityHelper import AnimalEntityHelper
 
-Team = TypeVar["net.minecraft.scoreboard.Team"]
+AxolotlEntity = TypeVar["net.minecraft.entity.passive.AxolotlEntity"]
 
-class TeamHelper(BaseHelper):
+class AxolotlEntityHelper(AnimalEntityHelper):
 	"""
-	Since: 1.3.0 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, t: Team) -> None:
+	def __init__(self, base: AxolotlEntity) -> None:
 		pass
 
 	@overload
-	def getName(self) -> str:
+	def getVariantId(self) -> int:
 		"""
-		Since: 1.3.0 
-		"""
-		pass
-
-	@overload
-	def getDisplayName(self) -> TextHelper:
-		"""
-		Since: 1.3.0 
-		"""
-		pass
-
-	@overload
-	def getPlayerList(self) -> List[str]:
-		"""
-		Since: 1.3.0 
-		"""
-		pass
-
-	@overload
-	def getColor(self) -> int:
-		"""
-		Since: 1.3.0 
-		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getPrefix(self) -> TextHelper:
-		"""
-		Since: 1.3.0 
+		Returns:
+			the id of this axolotl's variant. 
 		"""
 		pass
 
 	@overload
-	def getSuffix(self) -> TextHelper:
-		"""
-		Since: 1.3.0 
+	def getVariantName(self) -> str:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def getCollisionRule(self) -> str:
-		"""
-		Since: 1.3.0 
+		Returns:
+			the name of this axolotl's variant. 
 		"""
 		pass
 
 	@overload
-	def isFriendlyFire(self) -> bool:
-		"""
-		Since: 1.3.0 
+	def isPlayingDead(self) -> bool:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def showFriendlyInvisibles(self) -> bool:
-		"""
-		Since: 1.3.0 
+		Returns:
+			'true' if the axolotl is playing dead, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def nametagVisibility(self) -> str:
-		"""
-		Since: 1.3.0 
+	def isFromBucket(self) -> bool:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def deathMessageVisibility(self) -> str:
+		Returns:
+			'true' if the axolotl came from a bucket, 'false' otherwise. 
 		"""
-		Since: 1.3.0 
-		"""
-		pass
-
-	@overload
-	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextBuilder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import overload
+from typing import List
+from .FormattingHelper import FormattingHelper
 from .TextHelper import TextHelper
 from .ItemStackHelper import ItemStackHelper
 from .EntityHelper import EntityHelper
 from .MethodWrapper import MethodWrapper
 from .StyleHelper import StyleHelper
 
 
@@ -59,14 +61,27 @@
 			bold: 
 			strikethrough: 
 			italic: 
 		"""
 		pass
 
 	@overload
+	def withFormatting(self, formattings: List[FormattingHelper]) -> "TextBuilder":
+		"""
+		Since: 1.8.4 
+
+		Args:
+			formattings: the formattings to apply 
+
+		Returns:
+			self for chaining. 
+		"""
+		pass
+
+	@overload
 	def withShowTextHover(self, text: TextHelper) -> "TextBuilder":
 		"""set current section's hover event to show text\n
 		Since: 1.3.0 
 
 		Args:
 			text: 
 		"""
@@ -114,14 +129,24 @@
 		pass
 
 	@overload
 	def withStyle(self, style: StyleHelper) -> "TextBuilder":
 		pass
 
 	@overload
+	def getWidth(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the width of this text. 
+		"""
+		pass
+
+	@overload
 	def build(self) -> TextHelper:
 		"""Build to a TextHelper\n
 		Since: 1.3.0 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextFieldWidgetHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/FormattingHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,82 @@
 from typing import overload
 from typing import TypeVar
-from .ButtonWidgetHelper import ButtonWidgetHelper
+from .BaseHelper import BaseHelper
 
-TextFieldWidget = TypeVar["net.minecraft.client.gui.widget.TextFieldWidget"]
+Formatting = TypeVar["net.minecraft.util.Formatting"]
 
-class TextFieldWidgetHelper(ButtonWidgetHelper):
-	"""F\n
-	Since: 1.0.5 
+class FormattingHelper(BaseHelper):
+	"""
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, t: TextFieldWidget) -> None:
+	def __init__(self, base: Formatting) -> None:
 		pass
 
 	@overload
-	def __init__(self, t: TextFieldWidget, zIndex: int) -> None:
+	def getColorValue(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the color value of this formatting. 
+		"""
 		pass
 
 	@overload
-	def getText(self) -> str:
+	def getColorIndex(self) -> int:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
 		Returns:
-			the currently entered String . 
+			the index of this formatting or '-1' if this formatting is a modifier. 
 		"""
 		pass
 
 	@overload
-	def setText(self, text: str) -> "TextFieldWidgetHelper":
+	def getName(self) -> str:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			text: 
+		Returns:
+			the name of this formatting. 
 		"""
 		pass
 
 	@overload
-	def setText(self, text: str, await_: bool) -> "TextFieldWidgetHelper":
-		"""set the currently entered String .\n
-		Since: 1.3.1 
+	def getCode(self) -> str:
+		"""The color code can be used with the paragraph to color text.\n
+		Since: 1.8.4 
 
-		Args:
-			await: 
-			text: 
+		Returns:
+			the color code of this formatting. 
 		"""
 		pass
 
 	@overload
-	def setEditableColor(self, color: int) -> "TextFieldWidgetHelper":
+	def isColor(self) -> bool:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			color: 
+		Returns:
+			'true' if this formatting is a color, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def setEditable(self, edit: bool) -> "TextFieldWidgetHelper":
+	def isModifier(self) -> bool:
 		"""
-		Since: 1.0.5 
+		Since: 1.8.4 
 
-		Args:
-			edit: 
+		Returns:
+			'true' if this formatting is a modifier, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def setUneditableColor(self, color: int) -> "TextFieldWidgetHelper":
-		"""
-		Since: 1.0.5 
-
-		Args:
-			color: 
-		"""
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/ParrotEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,78 @@
 from typing import overload
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .MethodWrapper import MethodWrapper
+from .TameableEntityHelper import TameableEntityHelper
 
-Text = TypeVar["net.minecraft.text.Text"]
+ParrotEntity = TypeVar["net.minecraft.entity.passive.ParrotEntity"]
 
-class TextHelper(BaseHelper):
+class ParrotEntityHelper(TameableEntityHelper):
 	"""
-	Since: 1.0.8 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, t: Text) -> None:
+	def __init__(self, base: ParrotEntity) -> None:
 		pass
 
 	@overload
-	def replaceFromJson(self, json: str) -> "TextHelper":
-		"""replace the text in this class with JSON data.\n
-		Since: 1.0.8 
-
-		Args:
-			json: 
+	def getVariant(self) -> str:
 		"""
-		pass
-
-	@overload
-	def replaceFromString(self, content: str) -> "TextHelper":
-		"""replace the text in this class with String data.\n
-		Since: 1.0.8 
+		Since: 1.8.4 
 
-		Args:
-			content: 
+		Returns:
+			the variant of this parrot. 
 		"""
 		pass
 
 	@overload
-	def getJson(self) -> str:
+	def isSitting(self) -> bool:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Returns:
-			JSON data representation. 
+			'true' if this parrot is sitting, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getString(self) -> str:
+	def isFlying(self) -> bool:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
 		Returns:
-			the text content. 
+			'true' if this parrot is flying, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getStringStripFormatting(self) -> str:
+	def isPartying(self) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			the text content. stripped formatting when servers send it the (super) old way due to shitty coders. 
+			'true' if this parrot is dancing to music, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def visit(self, visitor: MethodWrapper) -> None:
+	def isStanding(self) -> bool:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
-		Args:
-			visitor: function with 2 args, no return. 
-		"""
-		pass
-
-	@overload
-	def toJson(self) -> str:
-		"""
-		Since: 1.0.8 
+		Returns:
+			'true' if this parrot is just standing around, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def isSittingOnShoulder(self) -> bool:
 		"""
-		Since: 1.0.8, this used to do the same as TextHelper#getString() 
+		Since: 1.8.4 
 
 		Returns:
-			String representation of text helper. 
+			'true' if this parrot is sitting on any player's shoulder, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextOverlay.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextOverlay.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TextPrompt.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TextPrompt.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def render(self, matrices: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
+	def render(self, drawContext: MatrixStack, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TickBasedEvents.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/TickBasedEvents.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/TradeOfferHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/PlayerListEntryHelper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,127 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
-from .VillagerInventory import VillagerInventory
-from .ItemStackHelper import ItemStackHelper
-from .NBTElementHelper import NBTElementHelper
+from .TextHelper import TextHelper
+from .TeamHelper import TeamHelper
 
-TradeOffer = TypeVar["net.minecraft.village.TradeOffer"]
+PlayerListEntry = TypeVar["net.minecraft.client.network.PlayerListEntry"]
 
-class TradeOfferHelper(BaseHelper):
+class PlayerListEntryHelper(BaseHelper):
+	"""
+	Since: 1.0.2 
+	"""
 
 	@overload
-	def __init__(self, base: TradeOffer, index: int, inv: VillagerInventory) -> None:
+	def __init__(self, p: PlayerListEntry) -> None:
 		pass
 
 	@overload
-	def getInput(self) -> List[ItemStackHelper]:
+	def getUUID(self) -> str:
 		"""
+		Since: 1.1.9 
+		"""
+		pass
 
-		Returns:
-			list of input items required 
+	@overload
+	def getName(self) -> str:
+		"""
+		Since: 1.0.2 
 		"""
 		pass
 
 	@overload
-	def getOutput(self) -> ItemStackHelper:
+	def getPing(self) -> int:
 		"""
+		Since: 1.6.5 
+		"""
+		pass
+
+	@overload
+	def getGamemode(self) -> str:
+		"""
+		Since: 1.6.5 
 
 		Returns:
-			output item that will be recieved 
+			null if unknown 
 		"""
 		pass
 
 	@overload
-	def select(self) -> None:
-		"""select trade offer on screen
+	def getDisplayText(self) -> TextHelper:
+		"""
+		Since: 1.1.9 
 		"""
 		pass
 
 	@overload
-	def isAvailable(self) -> bool:
+	def getPublicKey(self) -> List[float]:
 		"""
+		Since: 1.8.2 
 		"""
 		pass
 
 	@overload
-	def getNBT(self) -> NBTElementHelper:
+	def hasCape(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the player has a cape enabled, 'false' otherwise. 
 		"""
+		pass
+
+	@overload
+	def hasSlimModel(self) -> bool:
+		"""A slim skin is an Alex skin, while the default one is Steve.\n
+		Since: 1.8.4 
 
 		Returns:
-			trade offer as nbt tag 
+			'true' if the player has a slim skin, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getUses(self) -> int:
+	def getSkinTexture(self) -> str:
 		"""
+		Since: 1.8.4 
 
 		Returns:
-			current number of uses 
+			the identifier of the player's skin texture or 'null' if it's unknown. 
 		"""
 		pass
 
 	@overload
-	def getMaxUses(self) -> int:
+	def getCapeTexture(self) -> str:
 		"""
+		Since: 1.8.4 
 
 		Returns:
-			max uses before it locks 
+			the identifier of the player's cape texture or 'null' if it's unknown. 
 		"""
 		pass
 
 	@overload
-	def getExperience(self) -> int:
+	def getElytraTexture(self) -> str:
 		"""
+		Since: 1.8.4 
 
 		Returns:
-			experience gained for trade 
+			the identifier of the player's elytra texture or 'null' if it's unknown. 
 		"""
 		pass
 
 	@overload
-	def getCurrentPriceAdjustment(self) -> int:
+	def getTeam(self) -> TeamHelper:
 		"""
+		Since: 1.8.4 
 
 		Returns:
-			current price adjustment, negative is discount. 
+			the team of the player or 'null' if the player is not in a team. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/VillagerEntityHelper.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/CatEntityHelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 from typing import overload
 from typing import TypeVar
-from .MerchantEntityHelper import MerchantEntityHelper
+from .TameableEntityHelper import TameableEntityHelper
+from .DyeColorHelper import DyeColorHelper
 
-VillagerEntity = TypeVar["net.minecraft.entity.passive.VillagerEntity"]
+CatEntity = TypeVar["net.minecraft.entity.passive.CatEntity"]
 
-class VillagerEntityHelper(MerchantEntityHelper):
+class CatEntityHelper(TameableEntityHelper):
 	"""
-	Since: 1.6.3 
+	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, e: VillagerEntity) -> None:
+	def __init__(self, base: CatEntity) -> None:
 		pass
 
 	@overload
-	def getProfession(self) -> str:
+	def isSleeping(self) -> bool:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this cat is sleeping, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getStyle(self) -> str:
+	def getCollarColor(self) -> DyeColorHelper:
 		"""
-		Since: 1.6.3 
+		Since: 1.8.4 
+
+		Returns:
+			the color of this cat's collar. 
 		"""
 		pass
 
 	@overload
-	def getLevel(self) -> int:
-		"""
-		Since: 1.6.3 
+	def getVariant(self) -> str:
 		"""
-		pass
+		Since: 1.8.4 
 
-	@overload
-	def toString(self) -> str:
+		Returns:
+			the variant of this cat. 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/VillagerInventory.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/VillagerInventory.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class VillagerInventory(Inventory):
 	"""
 	Since: 1.3.1 
 	"""
 
 	@overload
 	def selectTrade(self, index: int) -> "VillagerInventory":
-		"""select the trade by it's index\n
+		"""select the trade by its index\n
 		Since: 1.3.1 
 
 		Args:
 			index: 
 
 		Returns:
 			self for chaining 
@@ -63,10 +63,14 @@
 		Since: 1.3.1 
 
 		Returns:
 			list of trade offers 
 		"""
 		pass
 
+	@overload
+	def toString(self) -> str:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/Websocket.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/Websocket.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/WorldScannerBuilder.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/WorldScannerBuilder.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 All other commands need some arguments to work. For String functions, it's one of these functions: 'equals', 'contains', 'startsWith', 'endsWith' or 'matches'.
 The strings to match are passed as vararg parameters (as many as needed, separated by a comma 'is("chest", "barrel", "ore"' ) and the filter acts
 like a logical or, so only one of the arguments needs to match the criteria. It should be noted, that string functions call the toString method, so
 comparing a block with something like "minecraft:stone" will always return false, because the toString method gives "{minecraft:stone}". For doing this
 use either contains or the equals method with 'getId', as shown later. This will match any block that includes 'stone' or 'diorit' in its name: withStringBlockFilter().contains("stone") //create new block filter, check if it contains stone
 .orStringBlockFilter().contains("diorit") //append new block filter with or and check if it contains diorit  
 For non String functions, the method name must be passed when creating the filter. The names can be any method in BlockStateHelper or BlockHelper .
-For more complex filters, use the MethodWrapper function FWorld#getWorldScanner(xyz.wagyourtail.jsmacros.core.MethodWrapper<xyz.wagyourtail.jsmacros.client.api.helpers.BlockHelper,java.lang.Object,java.lang.Boolean,?>,xyz.wagyourtail.jsmacros.core.MethodWrapper<xyz.wagyourtail.jsmacros.client.api.helpers.BlockStateHelper,java.lang.Object,java.lang.Boolean,?>) .
+For more complex filters, use the MethodWrapper function FWorld#getWorldScanner(xyz.wagyourtail.jsmacros.core.MethodWrapper<xyz.wagyourtail.jsmacros.client.api.helpers.world.BlockHelper,java.lang.Object,java.lang.Boolean,?>,xyz.wagyourtail.jsmacros.core.MethodWrapper<xyz.wagyourtail.jsmacros.client.api.helpers.world.BlockStateHelper,java.lang.Object,java.lang.Boolean,?>) .
 Depending on the return type of the method, the following parameters must be passed to 'is' or 'test'. There are two methods, because 'is' is a keyword in some languages.  For any number:
   - is(operation, number) with operation = '>', '>=', ' ', ' =', '==', '!=' and the number that should be compared to,
     i.e. is(">=", 8) returns true if the returned number is greater or equal to 8.
 For any String:
   - is(method, string) with method = 'EQUALS', 'CONTAINS', 'STARTS_WITH', 'ENDS_WITH', 'MATCHES' and the string is the one to compare the returned value to,
     i.e. is("ENDS_WITH", "ore") checks if the returned string ends with ore (can be used with withBlockFilter("getId")).
 For any Boolean:
-  - is(val) with val either 'true' or 'false' is(false) returns true if the returned boolean value is false\n
+  - is(val) with val either 'true' or 'false' i.e. is(false) returns true if the returned boolean value is false\n
 	Since: 1.6.5 
 	"""
 
 	@overload
 	def __init__(self) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/WrappedScript.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/WrappedScript.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/events.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,44 +8,52 @@
 from .EventWrappedScript import EventWrappedScript
 from .EventAirChange import EventAirChange
 from .CodeCompileEvent import CodeCompileEvent
 from .EventResourcePackLoaded import EventResourcePackLoaded
 from .EventItemDamage import EventItemDamage
 from .EventJoinedTick import EventJoinedTick
 from .EventTitle import EventTitle
+from .EventJoinedRecvPacket import EventJoinedRecvPacket
 from .EventOpenContainer import EventOpenContainer
 from .EventBossbar import EventBossbar
 from .EventAttackBlock import EventAttackBlock
 from .EventDamage import EventDamage
 from .EventPlayerLeave import EventPlayerLeave
 from .EventChunkLoad import EventChunkLoad
 from .EventHungerChange import EventHungerChange
 from .EventDropSlot import EventDropSlot
+from .EventHealthChange import EventHealthChange
 from .EventRiding import EventRiding
-from .EventJoinServer import EventJoinServer
 from .EventEntityUnload import EventEntityUnload
+from .EventJoinServer import EventJoinServer
+from .EventLaunchGame import EventLaunchGame
 from .EventEntityDamaged import EventEntityDamaged
+from .EventStatusEffectUpdate import EventStatusEffectUpdate
 from .EventFallFlying import EventFallFlying
 from .EventDisconnect import EventDisconnect
 from .EventInteractBlock import EventInteractBlock
+from .EventSendPacket import EventSendPacket
 from .EventHeal import EventHeal
+from .EventJoinedSendPacket import EventJoinedSendPacket
 from .EventInteractEntity import EventInteractEntity
 from .EventBlockUpdate import EventBlockUpdate
 from .EventEntityHealed import EventEntityHealed
 from .EventClickSlot import EventClickSlot
 from .EventDimensionChange import EventDimensionChange
 from .EventItemPickup import EventItemPickup
+from .EventQuitGame import EventQuitGame
 from .EventOpenScreen import EventOpenScreen
 from .EventDeath import EventDeath
-from .EventSignEdit import EventSignEdit
 from .EventAttackEntity import EventAttackEntity
+from .EventSignEdit import EventSignEdit
+from .EventRecvPacket import EventRecvPacket
 from .EventSendMessage import EventSendMessage
 from .CommandContextHelper import CommandContextHelper
-from .EventTick import EventTick
 from .EventJoinedKey import EventJoinedKey
+from .EventTick import EventTick
 from .EventSound import EventSound
 from .EventKey import EventKey
 from .EventProfileLoad import EventProfileLoad
 from .EventService import EventService
 from .EventEntityLoad import EventEntityLoad
 from .EventChunkUnload import EventChunkUnload
 from .EventArmorChange import EventArmorChange
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/libraries.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/libraries.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,38 +3,42 @@
 from .EventContainer import EventContainer
 from .BaseEvent import BaseEvent
 from .FChat import FChat
 from .FPlayer import FPlayer
 from .FRequest import FRequest
 from .FKeyBind import FKeyBind
 from .FHud import FHud
+from .FJavaUtils import FJavaUtils
 from .FTime import FTime
-from .FJsMacros import FJsMacros
 from .FFS import FFS
+from .FJsMacros import FJsMacros
 from .FReflection import FReflection
+from .FUtils import FUtils
 from .FClient import FClient
 from .FWorld import FWorld
-from .IFWrapper import IFWrapper
 from .FGlobalVars import FGlobalVars
+from .IFWrapper import IFWrapper
 from .FPositionCommon import FPositionCommon
 
 File = TypeVar["java.io.File"]
 
 
 
 Chat = FChat()
 Player = FPlayer()
 Request = FRequest()
 KeyBind = FKeyBind()
 Hud = FHud()
+JavaUtils = FJavaUtils()
 Time = FTime()
-JsMacros = FJsMacros()
 FS = FFS()
+JsMacros = FJsMacros()
 Reflection = FReflection()
+Utils = FUtils()
 Client = FClient()
 World = FWorld()
-JavaWrapper = IFWrapper()
 GlobalVars = FGlobalVars()
+JavaWrapper = IFWrapper()
 PositionCommon = FPositionCommon()
 context = EventContainer()
 file = File()
 event = BaseEvent()
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/mixins.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,70 @@
 from typing import TypeVar
 
 from .EventContainer import EventContainer
 from .BaseEvent import BaseEvent
-from .MixinSignEditScreen import MixinSignEditScreen
-from .MixinHungerManager import MixinHungerManager
+from .MixinAbstractFurnaceScreenHandler import MixinAbstractFurnaceScreenHandler
 from .MixinRecipeBookWidget import MixinRecipeBookWidget
 from .MixinFontManager import MixinFontManager
 from .MixinChunkSelection import MixinChunkSelection
-from .IMixinEntity import IMixinEntity
 from .MixinLivingEntity import MixinLivingEntity
+from .MixinClientConnection import MixinClientConnection
 from .MixinMinecraftClient import MixinMinecraftClient
-from .MixinPackedIntegerArray import MixinPackedIntegerArray
 from .MixinClientPlayNetworkHandler import MixinClientPlayNetworkHandler
-from .MixinClientPlayerEntity import MixinClientPlayerEntity
-from .MixinMerchantEntity import MixinMerchantEntity
 from .MixinDisconnectedScreen import MixinDisconnectedScreen
+from .MixinMerchantEntity import MixinMerchantEntity
+from .MixinShulkerEntity import MixinShulkerEntity
 from .MixinSplashOverlay import MixinSplashOverlay
 from .MixinTrueTypeFont import MixinTrueTypeFont
 from .MixinClientPlayerInteractionManager import MixinClientPlayerInteractionManager
-from .MixinHorseScreen import MixinHorseScreen
+from .MixinAdvancementRewards import MixinAdvancementRewards
 from .MixinCreativeInventoryScreen import MixinCreativeInventoryScreen
 from .MixinChatHud import MixinChatHud
-from .MixinPalettedContainer import MixinPalettedContainer
-from .MixinLoomScreen import MixinLoomScreen
-from .MixinSimpleOption import MixinSimpleOption
-from .MixinItemCooldownManager import MixinItemCooldownManager
-from .MixinResourcePackManager import MixinResourcePackManager
 from .MixinHandledScreen import MixinHandledScreen
-from .MixinClientWorld import MixinClientWorld
+from .MixinItemCooldownManager import MixinItemCooldownManager
 from .MixinSoundSystem import MixinSoundSystem
 from .MixinTranslationStorage import MixinTranslationStorage
-from .MixinBeaconScreen import MixinBeaconScreen
 from .MixinPlayerListHud import MixinPlayerListHud
-from .MixinItemCooldownEntry import MixinItemCooldownEntry
+from .MixinAbstractHorseEntity import MixinAbstractHorseEntity
+from .MixinFishingBobberEntity import MixinFishingBobberEntity
 from .MixinFontStorage import MixinFontStorage
 from .MixinBossBarHud import MixinBossBarHud
-from .MixinEntity import MixinEntity
 from .MixinPlayerEntity import MixinPlayerEntity
 from .MixinRecipeBookResults import MixinRecipeBookResults
-from .MixinMerchantScreen import MixinMerchantScreen
+from .MixinTridentEntity import MixinTridentEntity
+from .MixinCreeperEntity import MixinCreeperEntity
 from .MixinStyleSerializer import MixinStyleSerializer
-from .MixinStatHandler import MixinStatHandler
+from .MixinOcelotEntity import MixinOcelotEntity
 from .MixinScreen import MixinScreen
+from .MixinAllayEntity import MixinAllayEntity
+from .MixinSignEditScreen import MixinSignEditScreen
+from .MixinBoatEntity import MixinBoatEntity
+from .MixinHungerManager import MixinHungerManager
+from .MixinAdvancementManager import MixinAdvancementManager
+from .IMixinEntity import IMixinEntity
+from .MixinPackedIntegerArray import MixinPackedIntegerArray
+from .MixinClientAdvancementManager import MixinClientAdvancementManager
+from .MixinPhaseType import MixinPhaseType
+from .MixinAbstractPiglinEntity import MixinAbstractPiglinEntity
+from .MixinHorseScreen import MixinHorseScreen
+from .MixinPalettedContainer import MixinPalettedContainer
+from .MixinChatScreen import MixinChatScreen
+from .MixinLoomScreen import MixinLoomScreen
+from .MixinResourcePackManager import MixinResourcePackManager
+from .MixinSimpleOption import MixinSimpleOption
+from .MixinClientWorld import MixinClientWorld
+from .MixinTextFieldWidget import MixinTextFieldWidget
+from .MixinBeaconScreen import MixinBeaconScreen
+from .MixinItemCooldownEntry import MixinItemCooldownEntry
+from .MixinPacketHandler import MixinPacketHandler
+from .MixinEntity import MixinEntity
+from .MixinFoxEntity import MixinFoxEntity
+from .MixinAnvilScreen import MixinAnvilScreen
+from .MixinMerchantScreen import MixinMerchantScreen
+from .MixinHorseEntity import MixinHorseEntity
+from .MixinCyclingButton import MixinCyclingButton
+from .MixinStatHandler import MixinStatHandler
+from .MixinAdvancementProgress import MixinAdvancementProgress
 from .MixinPalettedContainerData import MixinPalettedContainerData
 
 File = TypeVar["java.io.File"]
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC/rest.py` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC/rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,260 +2,304 @@
 
 from .EventContainer import EventContainer
 from .BaseEvent import BaseEvent
 from .GroupFilter_CountMatchFilter import GroupFilter_CountMatchFilter
 from .Util import Util
 from .History import History
 from .OptionsField import OptionsField
+from .Vec3D import Vec3D
 from .TextOverlay import TextOverlay
 from .CharCompareFilter import CharCompareFilter
 from .LongField import LongField
 from .IRecipeBookResults import IRecipeBookResults
 from .CommandManager import CommandManager
+from .RecipeInventory import RecipeInventory
 from .Button import Button
+from .Sorting_SortServiceByFileName import Sorting_SortServiceByFileName
 from .IDraw2D import IDraw2D
 from .TextInput import TextInput
 from .Prism_typescript import Prism_typescript
 from .DoubleField import DoubleField
 from .BaseScriptContext_ScriptAssertionError import BaseScriptContext_ScriptAssertionError
 from .IChunkSection import IChunkSection
+from .Rect import Rect
+from .RenderElement3D import RenderElement3D
 from .IItemCooldownManager import IItemCooldownManager
 from .ClientConfigV2 import ClientConfigV2
 from .Prism_groovy import Prism_groovy
 from .ColorMapSetting import ColorMapSetting
+from .Vec2D import Vec2D
 from .IPalettedContainer import IPalettedContainer
+from .Line3D import Line3D
 from .ColorMapSetting_ColorEntry import ColorMapSetting_ColorEntry
 from .IFontManager import IFontManager
 from .PlayerInput import PlayerInput
-from .IRecipeBookWidget import IRecipeBookWidget
 from .IBeaconScreen import IBeaconScreen
+from .IRecipeBookWidget import IRecipeBookWidget
+from .Line import Line
 from .StringifyFilter import StringifyFilter
 from .IHorseScreen import IHorseScreen
 from .WrappedClassInstance_MethodSigParts import WrappedClassInstance_MethodSigParts
 from .IFilter import IFilter
 from .IPackedIntegerArray import IPackedIntegerArray
-from .RenderCommon_Item import RenderCommon_Item
-from .ChatHistoryManager import ChatHistoryManager
 from .Inventory import Inventory
+from .ChatHistoryManager import ChatHistoryManager
+from .Line3D_Builder import Line3D_Builder
 from .Sorting_SortByTriggerName import Sorting_SortByTriggerName
 from .BaseWrappedException_HostLocation import BaseWrappedException_HostLocation
 from .TranslationUtil import TranslationUtil
 from .IntField import IntField
 from .BaseListener import BaseListener
+from .Surface import Surface
+from .AutoCompleteSuggester import AutoCompleteSuggester
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SelectorDropdownOverlay import SelectorDropdownOverlay
 from .ServiceContainer import ServiceContainer
 from .FileChooser_fileObj import FileChooser_fileObj
 from .BlockStateFilter import BlockStateFilter
 from .IMerchantScreen import IMerchantScreen
-from .KeyMacrosScreen import KeyMacrosScreen
 from .EnchantInventory import EnchantInventory
+from .KeyMacrosScreen import KeyMacrosScreen
+from .Rect_Builder import Rect_Builder
 from .ClassBuilder_ConstructorBuilder import ClassBuilder_ConstructorBuilder
 from .History_TabLinesKeepCursor import History_TabLinesKeepCursor
 from .AbstractMapSettingContainer_MapSettingEntry import AbstractMapSettingContainer_MapSettingEntry
 from .History_HistoryStep import History_HistoryStep
 from .Scrollbar import Scrollbar
-from .FileChooser_sortFile import FileChooser_sortFile
-from .History_Add import History_Add
 from .BooleanCompareFilter import BooleanCompareFilter
+from .History_Add import History_Add
+from .FileChooser_sortFile import FileChooser_sortFile
+from .CraftingInventory import CraftingInventory
 from .EventRegistry import EventRegistry
 from .ScriptTrigger import ScriptTrigger
 from .Websocket import Websocket
+from .Plane3D import Plane3D
+from .Sorting_SortServiceByRunning import Sorting_SortServiceByRunning
+from .StoneCutterInventory import StoneCutterInventory
+from .AbstractWidgetBuilder import AbstractWidgetBuilder
 from .ServiceListTopbar import ServiceListTopbar
+from .DocletTypescriptExtends import DocletTypescriptExtends
+from .CustomImage import CustomImage
 from .Event import Event
 from .KeyListener import KeyListener
+from .BrewingStandInventory import BrewingStandInventory
 from .BasicFilter import BasicFilter
 from .ExtensionLoader import ExtensionLoader
 from .VillagerInventory import VillagerInventory
+from .CartographyInventory import CartographyInventory
 from .BaseWrappedException import BaseWrappedException
 from .PerExecLanguageLibrary import PerExecLanguageLibrary
-from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
+from .Box_Builder import Box_Builder
 from .NumberCompareFilter import NumberCompareFilter
+from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 from .ClassBuilder import ClassBuilder
 from .CustomClickEvent import CustomClickEvent
 from .TextBuilder import TextBuilder
-from .RenderCommon_RenderElement import RenderCommon_RenderElement
 from .IContainerParent import IContainerParent
 from .StringMapSetting_StringEntry import StringMapSetting_StringEntry
-from .PositionCommon_Pos2D import PositionCommon_Pos2D
 from .BaseWrappedException_GuestLocation import BaseWrappedException_GuestLocation
 from .FileChooser import FileChooser
 from .Sorting_SortByEnabled import Sorting_SortByEnabled
+from .Draw2DElement import Draw2DElement
+from .Item_Builder import Item_Builder
+from .FakeServerCommandSource import FakeServerCommandSource
 from .PrimitiveSettingGroup import PrimitiveSettingGroup
 from .LibraryBuilder import LibraryBuilder
 from .Draw3D import Draw3D
 from .Prism_kotlin import Prism_kotlin
+from .DocletEnumType import DocletEnumType
 from .FReflection_CombinedVariableClassLoader import FReflection_CombinedVariableClassLoader
-from .IClientPlayerEntity import IClientPlayerEntity
-from .PositionCommon_Pos3D import PositionCommon_Pos3D
+from .ModLoader import ModLoader
 from .TickSync import TickSync
+from .CheckBox import CheckBox
 from .EventChooser_EventObj import EventChooser_EventObj
+from .Image_Builder import Image_Builder
 from .StringField import StringField
 from .BaseScriptContext_SleepRunnable import BaseScriptContext_SleepRunnable
-from .AutoCompleteSuggestor import AutoCompleteSuggestor
 from .MovementDummy import MovementDummy
 from .IOverlayParent import IOverlayParent
-from .RenderCommon_Text import RenderCommon_Text
+from .Slider import Slider
 from .IMinecraftClient import IMinecraftClient
 from .ScriptScreen import ScriptScreen
 from .WorldScannerBuilder import WorldScannerBuilder
 from .Draw2D import Draw2D
 from .FloatField import FloatField
-from .PositionCommon import PositionCommon
 from .StringMapSetting import StringMapSetting
 from .FJsMacros_EventAndContext import FJsMacros_EventAndContext
-from .Sorting_MacroSortMethod import Sorting_MacroSortMethod
 from .CancelScreen_RTCSort import CancelScreen_RTCSort
-from .AboutOverlay import AboutOverlay
+from .Sorting_MacroSortMethod import Sorting_MacroSortMethod
 from .NoStyleCodeCompiler import NoStyleCodeCompiler
+from .AboutOverlay import AboutOverlay
 from .CheckBoxContainer import CheckBoxContainer
 from .IResourcePackManager import IResourcePackManager
 from .ListContainer import ListContainer
 from .DocletReplaceParams import DocletReplaceParams
 from .PerLanguageLibrary import PerLanguageLibrary
 from .BaseScriptContext import BaseScriptContext
 from .Extension_ExtMatch import Extension_ExtMatch
+from .NameUtil import NameUtil
 from .Pair import Pair
 from .ProxyBuilder import ProxyBuilder
 from .IInventory import IInventory
 from .IScreen import IScreen
 from .TextPrompt import TextPrompt
 from .Prism_json import Prism_json
+from .FileHandler_FileLineIterator import FileHandler_FileLineIterator
 from .ServiceScreen import ServiceScreen
+from .CreativeInventory import CreativeInventory
 from .ClassBuilder_FieldBuilder import ClassBuilder_FieldBuilder
 from .Extension import Extension
+from .Surface_Builder import Surface_Builder
 from .ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder import ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder
+from .Line_Builder import Line_Builder
 from .Mappings import Mappings
 from .BaseLibrary import BaseLibrary
 from .ICategoryTreeParent import ICategoryTreeParent
 from .ServiceTrigger import ServiceTrigger
 from .WrappedScript import WrappedScript
 from .CommandNodeAccessor import CommandNodeAccessor
 from .StringCompareFilter_FilterMethod import StringCompareFilter_FilterMethod
 from .PrioryFiFoTaskQueue import PrioryFiFoTaskQueue
+from .RenderElement import RenderElement
 from .ClassWrapperFilter import ClassWrapperFilter
-from .Draw3D_Box import Draw3D_Box
-from .RenderCommon_Rect import RenderCommon_Rect
+from .ContainerInventory import ContainerInventory
+from .Text_Builder import Text_Builder
+from .Image import Image
+from .Sorting_ServiceSortMethod import Sorting_ServiceSortMethod
+from .RenderElementBuilder import RenderElementBuilder
+from .Item import Item
 from .IMerchantEntity import IMerchantEntity
-from .DefaultCodeCompiler import DefaultCodeCompiler
+from .HorseInventory import HorseInventory
 from .WorldScanner import WorldScanner
+from .DefaultCodeCompiler import DefaultCodeCompiler
+from .Pos2D import Pos2D
 from .BlockFilter import BlockFilter
-from .Draw3D_Surface import Draw3D_Surface
 from .HTTPRequest import HTTPRequest
 from .ISignEditScreen import ISignEditScreen
 from .FileField import FileField
 from .OrFilter import OrFilter
 from .FKeyBind_KeyTracker import FKeyBind_KeyTracker
-from .RenderCommon import RenderCommon
 from .IAdvancedFilter import IAdvancedFilter
 from .LibraryRegistry import LibraryRegistry
 from .ILoomScreen import ILoomScreen
 from .TickBasedEvents import TickBasedEvents
-from .SettingsOverlay import SettingsOverlay
 from .NotFilter import NotFilter
-from .HTTPRequest_Response import HTTPRequest_Response
+from .SettingsOverlay import SettingsOverlay
 from .BaseWrappedException_SourceLocation import BaseWrappedException_SourceLocation
+from .HTTPRequest_Response import HTTPRequest_Response
 from .Prism_python import Prism_python
+from .Pos3D import Pos3D
 from .MacroScreen import MacroScreen
+from .IScreenInternal import IScreenInternal
 from .ExtensionClassLoader import ExtensionClassLoader
-from .ConfigFolder import ConfigFolder
 from .ICompare import ICompare
+from .ConfigFolder import ConfigFolder
 from .IBossBarHud import IBossBarHud
 from .History_TabLines import History_TabLines
 from .Mappings_MethodData import Mappings_MethodData
 from .Profile import Profile
 from .BaseEventRegistry import BaseEventRegistry
-from .MacroListTopbar import MacroListTopbar
 from .GroupFilter_NoneMatchFilter import GroupFilter_NoneMatchFilter
+from .MacroListTopbar import MacroListTopbar
 from .BooleanField import BooleanField
-from .RenderCommon_Image import RenderCommon_Image
 from .Prism_regex import Prism_regex
 from .IPlayerListHud import IPlayerListHud
+from .AnvilInventory import AnvilInventory
 from .Prism_lua import Prism_lua
 from .EventListener import EventListener
 from .ClassBuilder_FieldBuilder_FieldInitializerBuilder import ClassBuilder_FieldBuilder_FieldInitializerBuilder
+from .ICancelable import ICancelable
 from .BaseProfile import BaseProfile
+from .GrindStoneInventory import GrindStoneInventory
 from .TPSData import TPSData
 from .ConfirmOverlay import ConfirmOverlay
 from .SynchronizedWeakHashSet import SynchronizedWeakHashSet
 from .GroupFilter import GroupFilter
 from .Neighbor import Neighbor
-from .Draw3D_Line import Draw3D_Line
+from .SmithingInventory import SmithingInventory
+from .Text import Text
 from .StringHashTrie import StringHashTrie
 from .ConfigManager import ConfigManager
+from .Sorting_SortServiceByName import Sorting_SortServiceByName
 from .EventLockWatchdog import EventLockWatchdog
 from .AndFilter import AndFilter
 from .OverlayContainer import OverlayContainer
+from .Alignable import Alignable
 from .AbstractMapSettingContainer import AbstractMapSettingContainer
-from .PositionCommon_Plane3D import PositionCommon_Plane3D
 from .Mappings_ClassData import Mappings_ClassData
 from .BaseLanguage import BaseLanguage
 from .CategoryTreeContainer import CategoryTreeContainer
 from .MultiElementContainer import MultiElementContainer
 from .BeaconInventory import BeaconInventory
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 from .AnnotatedCheckBox import AnnotatedCheckBox
 from .MacroContainer import MacroContainer
-from .PositionCommon_Vec2D import PositionCommon_Vec2D
+from .Sorting_SortServiceByEnabled import Sorting_SortServiceByEnabled
+from .JsMacrosThreadPool_PoolThread import JsMacrosThreadPool_PoolThread
 from .ProxyBuilder_ProxyReference import ProxyBuilder_ProxyReference
 from .IChatHud import IChatHud
 from .History_Replace import History_Replace
 from .GroupFilter_AllMatchFilter import GroupFilter_AllMatchFilter
 from .XorFilter import XorFilter
 from .ScriptTrigger_TriggerType import ScriptTrigger_TriggerType
 from .StringCompareFilter import StringCompareFilter
 from .EditorScreen import EditorScreen
 from .Sorting_SortByFileName import Sorting_SortByFileName
 from .BaseScreen import BaseScreen
 from .IItemCooldownEntry import IItemCooldownEntry
 from .Prism_ruby import Prism_ruby
 from .JsMacros import JsMacros
 from .EventMacrosScreen import EventMacrosScreen
-from .Core import Core
 from .CoreConfigV2 import CoreConfigV2
+from .Core import Core
 from .SelectCursor import SelectCursor
 from .History_Remove import History_Remove
-from .PositionCommon_Vec3D import PositionCommon_Vec3D
 from .Websocket_Disconnected import Websocket_Disconnected
 from .Prism_javascript import Prism_javascript
+from .Box import Box
+from .DocletReplaceTypeParams import DocletReplaceTypeParams
 from .AbstractSettingField import AbstractSettingField
 from .DocletReplaceReturn import DocletReplaceReturn
 from .Option import Option
 from .MethodWrapper import MethodWrapper
-from .Library import Library
 from .ClassBuilder_MethodBuilder import ClassBuilder_MethodBuilder
+from .Library import Library
 from .ProfileSetting import ProfileSetting
 from .Prism import Prism
 from .FileMapSetting import FileMapSetting
 from .FileMapSetting_FileEntry import FileMapSetting_FileEntry
-from .WrappedClassInstance import WrappedClassInstance
 from .Mappings_MappedClass import Mappings_MappedClass
+from .WrappedClassInstance import WrappedClassInstance
 from .FJsMacros_ScriptEventListener import FJsMacros_ScriptEventListener
 from .LoomInventory import LoomInventory
 from .ServiceManager_ServiceStatus import ServiceManager_ServiceStatus
 from .CancelScreen import CancelScreen
 from .GroupFilter_AnyMatchFilter import GroupFilter_AnyMatchFilter
 from .PerExecLibrary import PerExecLibrary
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .ServiceManager import ServiceManager
+from .JsMacrosThreadPool import JsMacrosThreadPool
 from .MovementQueue import MovementQueue
 from .EventChooser import EventChooser
 from .OptionType import OptionType
 from .EventContainer import EventContainer
 from .BaseEvent import BaseEvent
+from .PlayerInventory import PlayerInventory
 from .TextStyleCompiler import TextStyleCompiler
 from .Sorting import Sorting
 from .FileHandler import FileHandler
 from .ProfileSetting_ProfileEntry import ProfileSetting_ProfileEntry
 from .IEventListener import IEventListener
 from .Prism_clike import Prism_clike
 from .IPalettedContainerData import IPalettedContainerData
+from .FurnaceInventory import FurnaceInventory
 from .ClassBuilder_BodyBuilder import ClassBuilder_BodyBuilder
 from .History_ShiftLine import History_ShiftLine
 from .ClassBuilder_AnnotationBuilder import ClassBuilder_AnnotationBuilder
 from .BossBarConsumer import BossBarConsumer
 from .ScriptCodeCompiler import ScriptCodeCompiler
 from .CommandBuilder import CommandBuilder
+from .Draw2DElement_Builder import Draw2DElement_Builder
 from .RunningContextContainer import RunningContextContainer
 
 File = TypeVar["java.io.File"]
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/PKG-INFO` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 Metadata-Version: 2.1
 Name: JsMacrosAC
-Version: 1.8.3.5434464
+Version: 1.8.4.8257505
 Summary: A package to let your IDE know what JsMacros can do
 Home-page: UNKNOWN
 Author: Hasenzahn1
 Author-email: <motzer10@gmx.de>
 License: UNKNOWN
 Description: # JsMacrosAC
-        The sole purpose of this package is to let your IDE know what functions the various [JsMacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros) classes have.\
-        Please note that this package does **not** add functionality and will crash your scripts if it is not imported correctly.
         
+        The sole purpose of this package is to let your IDE know what functions the
+        various [JsMacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros) classes have.\
+        Please note that this package does **not** add functionality and will crash your scripts if it is not imported
+        correctly.
         
         # How to import
+        
         Each import should be imported with leading `if __name__ == "":` otherwise the script will break.
         **Import all classes:**
+        
         ```python
         if __name__ == "": from JsMacrosAC import *
         ```
+        
         **Import all classes from a specific module:**
+        
         ```python
         if __name__ == "": from JsMacrosAC.<moduleName> import *
         ```
+        
         **Import one class:**
+        
         ```python
         if __name__ == "": from JsMacrosAC import <ClassName>
         ```
+        
         **Import in an event file**
+        
         ```python
         if __name__ == "": 
             from JsMacrosAC import EventAirChange
             event = EventAirChange() #No need of arguments
         ```
         
-        #Modules
+        # Modules
+        
         There are some modules in JsMacrosAC that can be imported as well, so you don't have to import all the files.\
         These Modules are:
         > - libraries (Contains all libraries and constants like Chat or GlobalVars)
         > - helpers (Contains all helper classes)
         > - events (Contains all event classes)
         > - mixins (Contains all mixin classes)
         > - rest (Contains all other classes)
         
         #Libraries
-        The Chat, JavaWrapper, Player, Request, Hud, Time, KeyBind, JsMacros, FS, Reflection, Client, World and GlobalVars libraries can be accessed by either importing all classes or importing the library module mentioned above. 
+        The Chat, JavaWrapper, Player, Request, Hud, Time, KeyBind, JsMacros, FS, Reflection, Client, World and GlobalVars
+        libraries can be accessed by either importing all classes or importing the library module mentioned above.
         
         #Things to note
-        Since Python does not support function overloading, only one function will be displayed in some IDEs. See the function description or class to learn more about the different ways to use this function.
+        Since Python does not support function overloading, only one function will be displayed in some IDEs. See the function
+        description or class to learn more about the different ways to use this function.
+        
 Keywords: python,JsMacros,Autocomplete,Doc
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `JsMacrosAC-1.8.3.5434464/JsMacrosAC.egg-info/SOURCES.txt` & `JsMacrosAC-1.8.4.8257505/JsMacrosAC.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 README.md
 setup.py
 JsMacrosAC/AboutOverlay.py
+JsMacrosAC/AbstractHorseEntityHelper.py
 JsMacrosAC/AbstractMapSettingContainer.py
 JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py
+JsMacrosAC/AbstractPiglinEntityHelper.py
 JsMacrosAC/AbstractRenderCodeCompiler.py
 JsMacrosAC/AbstractSettingContainer.py
 JsMacrosAC/AbstractSettingField.py
+JsMacrosAC/AbstractWidgetBuilder.py
+JsMacrosAC/AdvancementHelper.py
+JsMacrosAC/AdvancementManagerHelper.py
+JsMacrosAC/AdvancementProgressHelper.py
+JsMacrosAC/Alignable.py
+JsMacrosAC/AllayEntityHelper.py
 JsMacrosAC/AndFilter.py
+JsMacrosAC/AnimalEntityHelper.py
 JsMacrosAC/AnnotatedCheckBox.py
+JsMacrosAC/AnvilInventory.py
+JsMacrosAC/AreaEffectCloudEntityHelper.py
+JsMacrosAC/ArmorStandEntityHelper.py
+JsMacrosAC/ArrowEntityHelper.py
+JsMacrosAC/AutoCompleteSuggester.py
 JsMacrosAC/AutoCompleteSuggestion.py
-JsMacrosAC/AutoCompleteSuggestor.py
+JsMacrosAC/AxolotlEntityHelper.py
 JsMacrosAC/BaseEvent.py
 JsMacrosAC/BaseEventRegistry.py
 JsMacrosAC/BaseHelper.py
 JsMacrosAC/BaseLanguage.py
 JsMacrosAC/BaseLibrary.py
 JsMacrosAC/BaseListener.py
 JsMacrosAC/BaseProfile.py
@@ -22,70 +36,105 @@
 JsMacrosAC/BaseScriptContext_ScriptAssertionError.py
 JsMacrosAC/BaseScriptContext_SleepRunnable.py
 JsMacrosAC/BaseWrappedException.py
 JsMacrosAC/BaseWrappedException_GuestLocation.py
 JsMacrosAC/BaseWrappedException_HostLocation.py
 JsMacrosAC/BaseWrappedException_SourceLocation.py
 JsMacrosAC/BasicFilter.py
+JsMacrosAC/BatEntityHelper.py
 JsMacrosAC/BeaconInventory.py
+JsMacrosAC/BeeEntityHelper.py
+JsMacrosAC/BlazeEntityHelper.py
 JsMacrosAC/BlockDataHelper.py
 JsMacrosAC/BlockFilter.py
 JsMacrosAC/BlockHelper.py
 JsMacrosAC/BlockPosHelper.py
 JsMacrosAC/BlockStateFilter.py
 JsMacrosAC/BlockStateHelper.py
+JsMacrosAC/BoatEntityHelper.py
 JsMacrosAC/BooleanCompareFilter.py
 JsMacrosAC/BooleanField.py
 JsMacrosAC/BossBarConsumer.py
 JsMacrosAC/BossBarHelper.py
+JsMacrosAC/Box.py
+JsMacrosAC/Box_Builder.py
+JsMacrosAC/BrewingStandInventory.py
 JsMacrosAC/Button.py
 JsMacrosAC/ButtonWidgetHelper.py
+JsMacrosAC/ButtonWidgetHelper_ButtonBuilder.py
+JsMacrosAC/ButtonWidgetHelper_TexturedButtonBuilder.py
 JsMacrosAC/CancelScreen.py
 JsMacrosAC/CancelScreen_RTCSort.py
+JsMacrosAC/CartographyInventory.py
+JsMacrosAC/CatEntityHelper.py
 JsMacrosAC/CategoryTreeContainer.py
 JsMacrosAC/CharCompareFilter.py
 JsMacrosAC/ChatHistoryManager.py
 JsMacrosAC/ChatHudLineHelper.py
+JsMacrosAC/CheckBox.py
 JsMacrosAC/CheckBoxContainer.py
+JsMacrosAC/CheckBoxWidgetHelper.py
+JsMacrosAC/CheckBoxWidgetHelper_CheckBoxBuilder.py
+JsMacrosAC/ChunkHelper.py
 JsMacrosAC/ClassBuilder.py
 JsMacrosAC/ClassBuilder_AnnotationBuilder.py
 JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py
 JsMacrosAC/ClassBuilder_BodyBuilder.py
 JsMacrosAC/ClassBuilder_ConstructorBuilder.py
 JsMacrosAC/ClassBuilder_FieldBuilder.py
 JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py
 JsMacrosAC/ClassBuilder_MethodBuilder.py
 JsMacrosAC/ClassWrapperFilter.py
+JsMacrosAC/ClickableWidgetHelper.py
 JsMacrosAC/ClientConfigV2.py
 JsMacrosAC/ClientPlayerEntityHelper.py
 JsMacrosAC/CodeCompileEvent.py
 JsMacrosAC/ColorMapSetting.py
 JsMacrosAC/ColorMapSetting_ColorEntry.py
 JsMacrosAC/CommandBuilder.py
 JsMacrosAC/CommandContextHelper.py
 JsMacrosAC/CommandManager.py
 JsMacrosAC/CommandNodeAccessor.py
 JsMacrosAC/CommandNodeHelper.py
 JsMacrosAC/ConfigFolder.py
 JsMacrosAC/ConfigManager.py
 JsMacrosAC/ConfirmOverlay.py
+JsMacrosAC/ContainerInventory.py
 JsMacrosAC/Core.py
 JsMacrosAC/CoreConfigV2.py
+JsMacrosAC/CraftingInventory.py
+JsMacrosAC/CreativeInventory.py
+JsMacrosAC/CreativeItemStackHelper.py
+JsMacrosAC/CreeperEntityHelper.py
 JsMacrosAC/CustomClickEvent.py
+JsMacrosAC/CustomImage.py
+JsMacrosAC/CyclingButtonWidgetHelper.py
+JsMacrosAC/CyclingButtonWidgetHelper_CyclicButtonBuilder.py
 JsMacrosAC/DefaultCodeCompiler.py
+JsMacrosAC/DirectionHelper.py
+JsMacrosAC/DocletEnumType.py
 JsMacrosAC/DocletReplaceParams.py
 JsMacrosAC/DocletReplaceReturn.py
+JsMacrosAC/DocletReplaceTypeParams.py
+JsMacrosAC/DocletTypescriptExtends.py
+JsMacrosAC/DolphinEntityHelper.py
+JsMacrosAC/DonkeyEntityHelper.py
 JsMacrosAC/DoubleField.py
 JsMacrosAC/Draw2D.py
+JsMacrosAC/Draw2DElement.py
+JsMacrosAC/Draw2DElement_Builder.py
 JsMacrosAC/Draw3D.py
-JsMacrosAC/Draw3D_Box.py
-JsMacrosAC/Draw3D_Line.py
-JsMacrosAC/Draw3D_Surface.py
+JsMacrosAC/DrownedEntityHelper.py
+JsMacrosAC/DyeColorHelper.py
 JsMacrosAC/EditorScreen.py
 JsMacrosAC/EnchantInventory.py
+JsMacrosAC/EnchantmentHelper.py
+JsMacrosAC/EndCrystalEntityHelper.py
+JsMacrosAC/EnderDragonEntityHelper.py
+JsMacrosAC/EndermanEntityHelper.py
 JsMacrosAC/EntityHelper.py
 JsMacrosAC/Event.py
 JsMacrosAC/EventAirChange.py
 JsMacrosAC/EventArmorChange.py
 JsMacrosAC/EventAttackBlock.py
 JsMacrosAC/EventAttackEntity.py
 JsMacrosAC/EventBlockUpdate.py
@@ -105,94 +154,122 @@
 JsMacrosAC/EventEXPChange.py
 JsMacrosAC/EventEntityDamaged.py
 JsMacrosAC/EventEntityHealed.py
 JsMacrosAC/EventEntityLoad.py
 JsMacrosAC/EventEntityUnload.py
 JsMacrosAC/EventFallFlying.py
 JsMacrosAC/EventHeal.py
+JsMacrosAC/EventHealthChange.py
 JsMacrosAC/EventHeldItemChange.py
 JsMacrosAC/EventHungerChange.py
 JsMacrosAC/EventInteractBlock.py
 JsMacrosAC/EventInteractEntity.py
 JsMacrosAC/EventItemDamage.py
 JsMacrosAC/EventItemPickup.py
 JsMacrosAC/EventJoinServer.py
 JsMacrosAC/EventJoinedKey.py
+JsMacrosAC/EventJoinedRecvPacket.py
+JsMacrosAC/EventJoinedSendPacket.py
 JsMacrosAC/EventJoinedTick.py
 JsMacrosAC/EventKey.py
+JsMacrosAC/EventLaunchGame.py
 JsMacrosAC/EventListener.py
 JsMacrosAC/EventLockWatchdog.py
 JsMacrosAC/EventMacrosScreen.py
 JsMacrosAC/EventOpenContainer.py
 JsMacrosAC/EventOpenScreen.py
 JsMacrosAC/EventPlayerJoin.py
 JsMacrosAC/EventPlayerLeave.py
 JsMacrosAC/EventProfileLoad.py
+JsMacrosAC/EventQuitGame.py
 JsMacrosAC/EventRecvMessage.py
+JsMacrosAC/EventRecvPacket.py
 JsMacrosAC/EventRegistry.py
 JsMacrosAC/EventResourcePackLoaded.py
 JsMacrosAC/EventRiding.py
 JsMacrosAC/EventSendMessage.py
+JsMacrosAC/EventSendPacket.py
 JsMacrosAC/EventService.py
 JsMacrosAC/EventSignEdit.py
 JsMacrosAC/EventSound.py
+JsMacrosAC/EventStatusEffectUpdate.py
 JsMacrosAC/EventTick.py
 JsMacrosAC/EventTitle.py
 JsMacrosAC/EventWrappedScript.py
 JsMacrosAC/Extension.py
 JsMacrosAC/ExtensionClassLoader.py
 JsMacrosAC/ExtensionLoader.py
 JsMacrosAC/Extension_ExtMatch.py
 JsMacrosAC/FChat.py
 JsMacrosAC/FClient.py
 JsMacrosAC/FFS.py
 JsMacrosAC/FGlobalVars.py
 JsMacrosAC/FHud.py
+JsMacrosAC/FJavaUtils.py
 JsMacrosAC/FJsMacros.py
 JsMacrosAC/FJsMacros_EventAndContext.py
 JsMacrosAC/FJsMacros_ScriptEventListener.py
 JsMacrosAC/FKeyBind.py
 JsMacrosAC/FKeyBind_KeyTracker.py
 JsMacrosAC/FPlayer.py
 JsMacrosAC/FPositionCommon.py
 JsMacrosAC/FReflection.py
 JsMacrosAC/FReflection_CombinedVariableClassLoader.py
 JsMacrosAC/FRequest.py
 JsMacrosAC/FTime.py
+JsMacrosAC/FUtils.py
 JsMacrosAC/FWorld.py
+JsMacrosAC/FakeServerCommandSource.py
+JsMacrosAC/FallingBlockEntityHelper.py
 JsMacrosAC/FileChooser.py
 JsMacrosAC/FileChooser_fileObj.py
 JsMacrosAC/FileChooser_sortFile.py
 JsMacrosAC/FileField.py
 JsMacrosAC/FileHandler.py
+JsMacrosAC/FileHandler_FileLineIterator.py
 JsMacrosAC/FileMapSetting.py
 JsMacrosAC/FileMapSetting_FileEntry.py
+JsMacrosAC/FishEntityHelper.py
+JsMacrosAC/FishingBobberEntityHelper.py
 JsMacrosAC/FloatField.py
+JsMacrosAC/FluidStateHelper.py
+JsMacrosAC/FoodComponentHelper.py
+JsMacrosAC/FormattingHelper.py
+JsMacrosAC/FoxEntityHelper.py
+JsMacrosAC/FrogEntityHelper.py
+JsMacrosAC/FurnaceInventory.py
+JsMacrosAC/FurnaceMinecartEntityHelper.py
+JsMacrosAC/GhastEntityHelper.py
+JsMacrosAC/GoatEntityHelper.py
+JsMacrosAC/GrindStoneInventory.py
 JsMacrosAC/GroupFilter.py
 JsMacrosAC/GroupFilter_AllMatchFilter.py
 JsMacrosAC/GroupFilter_AnyMatchFilter.py
 JsMacrosAC/GroupFilter_CountMatchFilter.py
 JsMacrosAC/GroupFilter_NoneMatchFilter.py
+JsMacrosAC/GuardianEntityHelper.py
 JsMacrosAC/HTTPRequest.py
 JsMacrosAC/HTTPRequest_Response.py
 JsMacrosAC/History.py
 JsMacrosAC/History_Add.py
 JsMacrosAC/History_HistoryStep.py
 JsMacrosAC/History_Remove.py
 JsMacrosAC/History_Replace.py
 JsMacrosAC/History_ShiftLine.py
 JsMacrosAC/History_TabLines.py
 JsMacrosAC/History_TabLinesKeepCursor.py
+JsMacrosAC/HorseEntityHelper.py
+JsMacrosAC/HorseInventory.py
 JsMacrosAC/IAdvancedFilter.py
 JsMacrosAC/IBeaconScreen.py
 JsMacrosAC/IBossBarHud.py
+JsMacrosAC/ICancelable.py
 JsMacrosAC/ICategoryTreeParent.py
 JsMacrosAC/IChatHud.py
 JsMacrosAC/IChunkSection.py
-JsMacrosAC/IClientPlayerEntity.py
 JsMacrosAC/ICompare.py
 JsMacrosAC/IContainerParent.py
 JsMacrosAC/IDraw2D.py
 JsMacrosAC/IEventListener.py
 JsMacrosAC/IFWrapper.py
 JsMacrosAC/IFilter.py
 JsMacrosAC/IFontManager.py
@@ -210,109 +287,169 @@
 JsMacrosAC/IPalettedContainer.py
 JsMacrosAC/IPalettedContainerData.py
 JsMacrosAC/IPlayerListHud.py
 JsMacrosAC/IRecipeBookResults.py
 JsMacrosAC/IRecipeBookWidget.py
 JsMacrosAC/IResourcePackManager.py
 JsMacrosAC/IScreen.py
+JsMacrosAC/IScreenInternal.py
 JsMacrosAC/ISignEditScreen.py
+JsMacrosAC/IllagerEntityHelper.py
+JsMacrosAC/Image.py
+JsMacrosAC/Image_Builder.py
 JsMacrosAC/IntField.py
 JsMacrosAC/Inventory.py
+JsMacrosAC/IronGolemEntityHelper.py
+JsMacrosAC/Item.py
 JsMacrosAC/ItemEntityHelper.py
+JsMacrosAC/ItemFrameEntityHelper.py
+JsMacrosAC/ItemHelper.py
 JsMacrosAC/ItemStackHelper.py
+JsMacrosAC/Item_Builder.py
 JsMacrosAC/JsMacros.py
+JsMacrosAC/JsMacrosThreadPool.py
+JsMacrosAC/JsMacrosThreadPool_PoolThread.py
 JsMacrosAC/KeyListener.py
 JsMacrosAC/KeyMacrosScreen.py
 JsMacrosAC/Library.py
 JsMacrosAC/LibraryBuilder.py
 JsMacrosAC/LibraryRegistry.py
+JsMacrosAC/Line.py
+JsMacrosAC/Line3D.py
+JsMacrosAC/Line3D_Builder.py
+JsMacrosAC/Line_Builder.py
 JsMacrosAC/ListContainer.py
 JsMacrosAC/LivingEntityHelper.py
+JsMacrosAC/LlamaEntityHelper.py
+JsMacrosAC/LockButtonWidgetHelper.py
+JsMacrosAC/LockButtonWidgetHelper_LockButtonBuilder.py
 JsMacrosAC/LongField.py
 JsMacrosAC/LoomInventory.py
 JsMacrosAC/MacroContainer.py
 JsMacrosAC/MacroListTopbar.py
 JsMacrosAC/MacroScreen.py
 JsMacrosAC/Mappings.py
 JsMacrosAC/Mappings_ClassData.py
 JsMacrosAC/Mappings_MappedClass.py
 JsMacrosAC/Mappings_MethodData.py
 JsMacrosAC/MerchantEntityHelper.py
 JsMacrosAC/MethodWrapper.py
+JsMacrosAC/MixinAbstractFurnaceScreenHandler.py
+JsMacrosAC/MixinAbstractHorseEntity.py
+JsMacrosAC/MixinAbstractPiglinEntity.py
+JsMacrosAC/MixinAdvancementManager.py
+JsMacrosAC/MixinAdvancementProgress.py
+JsMacrosAC/MixinAdvancementRewards.py
+JsMacrosAC/MixinAllayEntity.py
+JsMacrosAC/MixinAnvilScreen.py
 JsMacrosAC/MixinBeaconScreen.py
+JsMacrosAC/MixinBoatEntity.py
 JsMacrosAC/MixinBossBarHud.py
 JsMacrosAC/MixinChatHud.py
+JsMacrosAC/MixinChatScreen.py
 JsMacrosAC/MixinChunkSelection.py
+JsMacrosAC/MixinClientAdvancementManager.py
+JsMacrosAC/MixinClientConnection.py
 JsMacrosAC/MixinClientPlayNetworkHandler.py
-JsMacrosAC/MixinClientPlayerEntity.py
 JsMacrosAC/MixinClientPlayerInteractionManager.py
 JsMacrosAC/MixinClientWorld.py
 JsMacrosAC/MixinCreativeInventoryScreen.py
+JsMacrosAC/MixinCreeperEntity.py
+JsMacrosAC/MixinCyclingButton.py
 JsMacrosAC/MixinDisconnectedScreen.py
 JsMacrosAC/MixinEntity.py
+JsMacrosAC/MixinFishingBobberEntity.py
 JsMacrosAC/MixinFontManager.py
 JsMacrosAC/MixinFontStorage.py
+JsMacrosAC/MixinFoxEntity.py
 JsMacrosAC/MixinHandledScreen.py
+JsMacrosAC/MixinHorseEntity.py
 JsMacrosAC/MixinHorseScreen.py
 JsMacrosAC/MixinHungerManager.py
 JsMacrosAC/MixinItemCooldownEntry.py
 JsMacrosAC/MixinItemCooldownManager.py
 JsMacrosAC/MixinLivingEntity.py
 JsMacrosAC/MixinLoomScreen.py
 JsMacrosAC/MixinMerchantEntity.py
 JsMacrosAC/MixinMerchantScreen.py
 JsMacrosAC/MixinMinecraftClient.py
+JsMacrosAC/MixinOcelotEntity.py
 JsMacrosAC/MixinPackedIntegerArray.py
+JsMacrosAC/MixinPacketHandler.py
 JsMacrosAC/MixinPalettedContainer.py
 JsMacrosAC/MixinPalettedContainerData.py
+JsMacrosAC/MixinPhaseType.py
 JsMacrosAC/MixinPlayerEntity.py
 JsMacrosAC/MixinPlayerListHud.py
 JsMacrosAC/MixinRecipeBookResults.py
 JsMacrosAC/MixinRecipeBookWidget.py
 JsMacrosAC/MixinResourcePackManager.py
 JsMacrosAC/MixinScreen.py
+JsMacrosAC/MixinShulkerEntity.py
 JsMacrosAC/MixinSignEditScreen.py
 JsMacrosAC/MixinSimpleOption.py
 JsMacrosAC/MixinSoundSystem.py
+JsMacrosAC/MixinSpellcastingIllagerEntityHelper.py
 JsMacrosAC/MixinSplashOverlay.py
 JsMacrosAC/MixinStatHandler.py
 JsMacrosAC/MixinStyleSerializer.py
+JsMacrosAC/MixinTextFieldWidget.py
 JsMacrosAC/MixinTranslationStorage.py
+JsMacrosAC/MixinTridentEntity.py
 JsMacrosAC/MixinTrueTypeFont.py
+JsMacrosAC/MobEntityHelper.py
+JsMacrosAC/ModContainerHelper.py
+JsMacrosAC/ModLoader.py
+JsMacrosAC/MooshroomEntityHelper.py
 JsMacrosAC/MovementDummy.py
 JsMacrosAC/MovementQueue.py
 JsMacrosAC/MultiElementContainer.py
 JsMacrosAC/NBTElementHelper.py
 JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py
 JsMacrosAC/NBTElementHelper_NBTListHelper.py
 JsMacrosAC/NBTElementHelper_NBTNumberHelper.py
+JsMacrosAC/NameUtil.py
 JsMacrosAC/Neighbor.py
 JsMacrosAC/NoStyleCodeCompiler.py
 JsMacrosAC/NotFilter.py
 JsMacrosAC/NumberCompareFilter.py
+JsMacrosAC/OcelotEntityHelper.py
 JsMacrosAC/Option.py
 JsMacrosAC/OptionType.py
 JsMacrosAC/OptionsField.py
 JsMacrosAC/OptionsHelper.py
+JsMacrosAC/OptionsHelper_AccessibilityOptionsHelper.py
+JsMacrosAC/OptionsHelper_ChatOptionsHelper.py
+JsMacrosAC/OptionsHelper_ControlOptionsHelper.py
+JsMacrosAC/OptionsHelper_MusicOptionsHelper.py
+JsMacrosAC/OptionsHelper_SkinOptionsHelper.py
+JsMacrosAC/OptionsHelper_VideoOptionsHelper.py
 JsMacrosAC/OrFilter.py
 JsMacrosAC/OverlayContainer.py
+JsMacrosAC/PacketByteBufferHelper.py
+JsMacrosAC/PaintingEntityHelper.py
 JsMacrosAC/Pair.py
+JsMacrosAC/PandaEntityHelper.py
+JsMacrosAC/ParrotEntityHelper.py
 JsMacrosAC/PerExecLanguageLibrary.py
 JsMacrosAC/PerExecLibrary.py
 JsMacrosAC/PerLanguageLibrary.py
+JsMacrosAC/PhantomEntityHelper.py
+JsMacrosAC/PigEntityHelper.py
+JsMacrosAC/PiglinEntityHelper.py
+JsMacrosAC/PillagerEntityHelper.py
+JsMacrosAC/Plane3D.py
 JsMacrosAC/PlayerAbilitiesHelper.py
 JsMacrosAC/PlayerEntityHelper.py
 JsMacrosAC/PlayerInput.py
+JsMacrosAC/PlayerInventory.py
 JsMacrosAC/PlayerListEntryHelper.py
-JsMacrosAC/PositionCommon.py
-JsMacrosAC/PositionCommon_Plane3D.py
-JsMacrosAC/PositionCommon_Pos2D.py
-JsMacrosAC/PositionCommon_Pos3D.py
-JsMacrosAC/PositionCommon_Vec2D.py
-JsMacrosAC/PositionCommon_Vec3D.py
+JsMacrosAC/PolarBearEntityHelper.py
+JsMacrosAC/Pos2D.py
+JsMacrosAC/Pos3D.py
 JsMacrosAC/PrimitiveSettingGroup.py
 JsMacrosAC/PrioryFiFoTaskQueue.py
 JsMacrosAC/Prism.py
 JsMacrosAC/Prism_clike.py
 JsMacrosAC/Prism_groovy.py
 JsMacrosAC/Prism_javascript.py
 JsMacrosAC/Prism_json.py
@@ -323,21 +460,24 @@
 JsMacrosAC/Prism_ruby.py
 JsMacrosAC/Prism_typescript.py
 JsMacrosAC/Profile.py
 JsMacrosAC/ProfileSetting.py
 JsMacrosAC/ProfileSetting_ProfileEntry.py
 JsMacrosAC/ProxyBuilder.py
 JsMacrosAC/ProxyBuilder_ProxyReference.py
+JsMacrosAC/PufferfishEntityHelper.py
+JsMacrosAC/RabbitEntityHelper.py
 JsMacrosAC/RecipeHelper.py
-JsMacrosAC/RenderCommon.py
-JsMacrosAC/RenderCommon_Image.py
-JsMacrosAC/RenderCommon_Item.py
-JsMacrosAC/RenderCommon_Rect.py
-JsMacrosAC/RenderCommon_RenderElement.py
-JsMacrosAC/RenderCommon_Text.py
+JsMacrosAC/RecipeInventory.py
+JsMacrosAC/Rect.py
+JsMacrosAC/Rect_Builder.py
+JsMacrosAC/RegistryHelper.py
+JsMacrosAC/RenderElement.py
+JsMacrosAC/RenderElement3D.py
+JsMacrosAC/RenderElementBuilder.py
 JsMacrosAC/RunningContextContainer.py
 JsMacrosAC/ScoreboardObjectiveHelper.py
 JsMacrosAC/ScoreboardsHelper.py
 JsMacrosAC/ScriptCodeCompiler.py
 JsMacrosAC/ScriptScreen.py
 JsMacrosAC/ScriptTrigger.py
 JsMacrosAC/ScriptTrigger_TriggerType.py
@@ -349,55 +489,95 @@
 JsMacrosAC/ServiceListTopbar.py
 JsMacrosAC/ServiceManager.py
 JsMacrosAC/ServiceManager_ServiceStatus.py
 JsMacrosAC/ServiceScreen.py
 JsMacrosAC/ServiceTrigger.py
 JsMacrosAC/SettingsOverlay.py
 JsMacrosAC/SettingsOverlay_SettingField.py
+JsMacrosAC/SheepEntityHelper.py
+JsMacrosAC/ShulkerEntityHelper.py
+JsMacrosAC/Slider.py
+JsMacrosAC/SliderWidgetHelper.py
+JsMacrosAC/SliderWidgetHelper_SliderBuilder.py
+JsMacrosAC/SlimeEntityHelper.py
+JsMacrosAC/SmithingInventory.py
+JsMacrosAC/SnowGolemEntityHelper.py
 JsMacrosAC/Sorting.py
 JsMacrosAC/Sorting_MacroSortMethod.py
+JsMacrosAC/Sorting_ServiceSortMethod.py
 JsMacrosAC/Sorting_SortByEnabled.py
 JsMacrosAC/Sorting_SortByFileName.py
 JsMacrosAC/Sorting_SortByTriggerName.py
+JsMacrosAC/Sorting_SortServiceByEnabled.py
+JsMacrosAC/Sorting_SortServiceByFileName.py
+JsMacrosAC/Sorting_SortServiceByName.py
+JsMacrosAC/Sorting_SortServiceByRunning.py
+JsMacrosAC/SpellcastingIllagerEntityHelper.py
+JsMacrosAC/SpiderEntityHelper.py
+JsMacrosAC/StateHelper.py
 JsMacrosAC/StatsHelper.py
 JsMacrosAC/StatusEffectHelper.py
+JsMacrosAC/StoneCutterInventory.py
+JsMacrosAC/StriderEntityHelper.py
 JsMacrosAC/StringCompareFilter.py
 JsMacrosAC/StringCompareFilter_FilterMethod.py
 JsMacrosAC/StringField.py
 JsMacrosAC/StringHashTrie.py
 JsMacrosAC/StringMapSetting.py
 JsMacrosAC/StringMapSetting_StringEntry.py
 JsMacrosAC/StringifyFilter.py
 JsMacrosAC/StyleHelper.py
 JsMacrosAC/SuggestionsBuilderHelper.py
+JsMacrosAC/Surface.py
+JsMacrosAC/Surface_Builder.py
 JsMacrosAC/SynchronizedWeakHashSet.py
 JsMacrosAC/TPSData.py
+JsMacrosAC/TameableEntityHelper.py
 JsMacrosAC/TeamHelper.py
+JsMacrosAC/Text.py
 JsMacrosAC/TextBuilder.py
 JsMacrosAC/TextFieldWidgetHelper.py
+JsMacrosAC/TextFieldWidgetHelper_TextFieldBuilder.py
 JsMacrosAC/TextHelper.py
 JsMacrosAC/TextInput.py
 JsMacrosAC/TextOverlay.py
 JsMacrosAC/TextPrompt.py
 JsMacrosAC/TextStyleCompiler.py
+JsMacrosAC/Text_Builder.py
 JsMacrosAC/TickBasedEvents.py
 JsMacrosAC/TickSync.py
+JsMacrosAC/TntEntityHelper.py
+JsMacrosAC/TntMinecartEntityHelper.py
 JsMacrosAC/TradeOfferHelper.py
 JsMacrosAC/TranslationUtil.py
+JsMacrosAC/TridentEntityHelper.py
+JsMacrosAC/TropicalFishEntityHelper.py
+JsMacrosAC/UniversalBlockStateHelper.py
 JsMacrosAC/Util.py
+JsMacrosAC/Vec2D.py
+JsMacrosAC/Vec3D.py
+JsMacrosAC/VexEntityHelper.py
 JsMacrosAC/VillagerEntityHelper.py
 JsMacrosAC/VillagerInventory.py
+JsMacrosAC/VindicatorEntityHelper.py
+JsMacrosAC/WardenEntityHelper.py
 JsMacrosAC/Websocket.py
 JsMacrosAC/Websocket_Disconnected.py
+JsMacrosAC/WitchEntityHelper.py
+JsMacrosAC/WitherEntityHelper.py
+JsMacrosAC/WitherSkullEntityHelper.py
+JsMacrosAC/WolfEntityHelper.py
 JsMacrosAC/WorldScanner.py
 JsMacrosAC/WorldScannerBuilder.py
 JsMacrosAC/WrappedClassInstance.py
 JsMacrosAC/WrappedClassInstance_MethodSigParts.py
 JsMacrosAC/WrappedScript.py
 JsMacrosAC/XorFilter.py
+JsMacrosAC/ZombieEntityHelper.py
+JsMacrosAC/ZombieVillagerEntityHelper.py
 JsMacrosAC/__init__.py
 JsMacrosAC/events.py
 JsMacrosAC/helpers.py
 JsMacrosAC/libraries.py
 JsMacrosAC/mixins.py
 JsMacrosAC/rest.py
 JsMacrosAC.egg-info/PKG-INFO
```

### Comparing `JsMacrosAC-1.8.3.5434464/PKG-INFO` & `JsMacrosAC-1.8.4.8257505/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 Metadata-Version: 2.1
 Name: JsMacrosAC
-Version: 1.8.3.5434464
+Version: 1.8.4.8257505
 Summary: A package to let your IDE know what JsMacros can do
 Home-page: UNKNOWN
 Author: Hasenzahn1
 Author-email: <motzer10@gmx.de>
 License: UNKNOWN
 Description: # JsMacrosAC
-        The sole purpose of this package is to let your IDE know what functions the various [JsMacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros) classes have.\
-        Please note that this package does **not** add functionality and will crash your scripts if it is not imported correctly.
         
+        The sole purpose of this package is to let your IDE know what functions the
+        various [JsMacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros) classes have.\
+        Please note that this package does **not** add functionality and will crash your scripts if it is not imported
+        correctly.
         
         # How to import
+        
         Each import should be imported with leading `if __name__ == "":` otherwise the script will break.
         **Import all classes:**
+        
         ```python
         if __name__ == "": from JsMacrosAC import *
         ```
+        
         **Import all classes from a specific module:**
+        
         ```python
         if __name__ == "": from JsMacrosAC.<moduleName> import *
         ```
+        
         **Import one class:**
+        
         ```python
         if __name__ == "": from JsMacrosAC import <ClassName>
         ```
+        
         **Import in an event file**
+        
         ```python
         if __name__ == "": 
             from JsMacrosAC import EventAirChange
             event = EventAirChange() #No need of arguments
         ```
         
-        #Modules
+        # Modules
+        
         There are some modules in JsMacrosAC that can be imported as well, so you don't have to import all the files.\
         These Modules are:
         > - libraries (Contains all libraries and constants like Chat or GlobalVars)
         > - helpers (Contains all helper classes)
         > - events (Contains all event classes)
         > - mixins (Contains all mixin classes)
         > - rest (Contains all other classes)
         
         #Libraries
-        The Chat, JavaWrapper, Player, Request, Hud, Time, KeyBind, JsMacros, FS, Reflection, Client, World and GlobalVars libraries can be accessed by either importing all classes or importing the library module mentioned above. 
+        The Chat, JavaWrapper, Player, Request, Hud, Time, KeyBind, JsMacros, FS, Reflection, Client, World and GlobalVars
+        libraries can be accessed by either importing all classes or importing the library module mentioned above.
         
         #Things to note
-        Since Python does not support function overloading, only one function will be displayed in some IDEs. See the function description or class to learn more about the different ways to use this function.
+        Since Python does not support function overloading, only one function will be displayed in some IDEs. See the function
+        description or class to learn more about the different ways to use this function.
+        
 Keywords: python,JsMacros,Autocomplete,Doc
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `JsMacrosAC-1.8.3.5434464/README.md` & `JsMacrosAC-1.8.4.8257505/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 # JsMacrosAC
-The sole purpose of this package is to let your IDE know what functions the various [JsMacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros) classes have.\
-Please note that this package does **not** add functionality and will crash your scripts if it is not imported correctly.
 
+The sole purpose of this package is to let your IDE know what functions the
+various [JsMacros](https://www.curseforge.com/minecraft/mc-mods/jsmacros) classes have.\
+Please note that this package does **not** add functionality and will crash your scripts if it is not imported
+correctly.
 
 # How to import
+
 Each import should be imported with leading `if __name__ == "":` otherwise the script will break.
 **Import all classes:**
+
 ```python
 if __name__ == "": from JsMacrosAC import *
 ```
+
 **Import all classes from a specific module:**
+
 ```python
 if __name__ == "": from JsMacrosAC.<moduleName> import *
 ```
+
 **Import one class:**
+
 ```python
 if __name__ == "": from JsMacrosAC import <ClassName>
 ```
+
 **Import in an event file**
+
 ```python
 if __name__ == "": 
     from JsMacrosAC import EventAirChange
     event = EventAirChange() #No need of arguments
 ```
 
-#Modules
+# Modules
+
 There are some modules in JsMacrosAC that can be imported as well, so you don't have to import all the files.\
 These Modules are:
 > - libraries (Contains all libraries and constants like Chat or GlobalVars)
 > - helpers (Contains all helper classes)
 > - events (Contains all event classes)
 > - mixins (Contains all mixin classes)
 > - rest (Contains all other classes)
 
 #Libraries
-The Chat, JavaWrapper, Player, Request, Hud, Time, KeyBind, JsMacros, FS, Reflection, Client, World and GlobalVars libraries can be accessed by either importing all classes or importing the library module mentioned above. 
+The Chat, JavaWrapper, Player, Request, Hud, Time, KeyBind, JsMacros, FS, Reflection, Client, World and GlobalVars
+libraries can be accessed by either importing all classes or importing the library module mentioned above.
 
 #Things to note
-Since Python does not support function overloading, only one function will be displayed in some IDEs. See the function description or class to learn more about the different ways to use this function.
+Since Python does not support function overloading, only one function will be displayed in some IDEs. See the function
+description or class to learn more about the different ways to use this function.
```

### Comparing `JsMacrosAC-1.8.3.5434464/setup.py` & `JsMacrosAC-1.8.4.8257505/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
-VERSION = '1.8.3'
+VERSION = '1.8.4'
 if "-" in VERSION: VERSION = VERSION.split("-")[0]
 VERSION += "." + str(time.time()).split(".")[0][3:]
 DESCRIPTION = 'A package to let your IDE know what JsMacros can do'
 
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
```

