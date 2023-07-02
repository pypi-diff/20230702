# Comparing `tmp/JsMacrosAC-1.8.4.8263756.tar.gz` & `tmp/JsMacrosAC-1.8.5.8296535.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/JsMacrosAC-1.8.4.8263756.tar", last modified: Sun Jul  2 02:09:17 2023, max compression
+gzip compressed data, was "dist/JsMacrosAC-1.8.5.8296535.tar", last modified: Sun Jul  2 11:15:36 2023, max compression
```

## Comparing `JsMacrosAC-1.8.4.8263756.tar` & `JsMacrosAC-1.8.5.8296535.tar`

### file list

```diff
@@ -1,591 +1,591 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AboutOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractHorseEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractMapSettingContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractPiglinEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractRenderCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractSettingContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractSettingField.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractWidgetBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AdvancementHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AdvancementManagerHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AdvancementProgressHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Alignable.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AllayEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AndFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AnimalEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AnnotatedCheckBox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AnvilInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AreaEffectCloudEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ArmorStandEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ArrowEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AutoCompleteSuggester.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AutoCompleteSuggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/AxolotlEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseEventRegistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseLanguage.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseScriptContext.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseScriptContext_ScriptAssertionError.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseScriptContext_SleepRunnable.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseWrappedException.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseWrappedException_GuestLocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseWrappedException_HostLocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseWrappedException_SourceLocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BasicFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BatEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BeaconInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BeeEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlazeEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockDataHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockPosHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockStateFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockStateHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BoatEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BooleanCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BooleanField.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BossBarConsumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BossBarHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Box.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Box_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/BrewingStandInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Button.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ButtonWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ButtonWidgetHelper_ButtonBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ButtonWidgetHelper_TexturedButtonBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CancelScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CancelScreen_RTCSort.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CartographyInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CatEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CategoryTreeContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CharCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ChatHistoryManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ChatHudLineHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-02 02:08:45.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBox.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBoxContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBoxWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBoxWidgetHelper_CheckBoxBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ChunkHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_AnnotationBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_BodyBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_ConstructorBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_FieldBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_MethodBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassWrapperFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClickableWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClientConfigV2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClientPlayerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CodeCompileEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ColorMapSetting.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ColorMapSetting_ColorEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandContextHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandNodeAccessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandNodeHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ConfigFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ConfirmOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ContainerInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CoreConfigV2.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CraftingInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CreativeInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CreativeItemStackHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CreeperEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CustomClickEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CustomImage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CyclingButtonWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/CyclingButtonWidgetHelper_CyclicButtonBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DefaultCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DirectionHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DocletEnumType.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DocletReplaceParams.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DocletReplaceReturn.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DocletReplaceTypeParams.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DocletTypescriptExtends.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DolphinEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DonkeyEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DoubleField.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw2DElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-02 02:08:46.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw2DElement_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DrownedEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/DyeColorHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EditorScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EnchantInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EnchantmentHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EndCrystalEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EnderDragonEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EndermanEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventAirChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventArmorChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventAttackBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventAttackEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventBlockUpdate.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventBossbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventChooser.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventChooser_EventObj.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventChunkLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventChunkUnload.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventClickSlot.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDamage.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDeath.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDimensionChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDisconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDropSlot.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventEXPChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventEntityDamaged.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventEntityHealed.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventEntityLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventEntityUnload.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventFallFlying.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventHeal.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventHealthChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventHeldItemChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventHungerChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventInteractBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventInteractEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventItemDamage.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventItemPickup.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinedRecvPacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinedSendPacket.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinedTick.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventKey.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventLaunchGame.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventListener.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventLockWatchdog.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventMacrosScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventOpenContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventOpenScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventPlayerJoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventPlayerLeave.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventProfileLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 02:08:47.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventQuitGame.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventRecvMessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventRecvPacket.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventRegistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventResourcePackLoaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventRiding.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventSendMessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventSendPacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventService.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventSignEdit.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventSound.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventStatusEffectUpdate.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventTick.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventWrappedScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ExtensionClassLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ExtensionLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Extension_ExtMatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FChat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FFS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FGlobalVars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FHud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FJavaUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FJsMacros.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FJsMacros_EventAndContext.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FJsMacros_ScriptEventListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FKeyBind.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FKeyBind_KeyTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FPlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FPositionCommon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FReflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FReflection_CombinedVariableClassLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FWorld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FakeServerCommandSource.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FallingBlockEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileChooser.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileChooser_fileObj.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileChooser_sortFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileField.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileHandler_FileLineIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileMapSetting.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileMapSetting_FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FishEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FishingBobberEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FloatField.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FluidStateHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FoodComponentHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FormattingHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FoxEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FrogEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FurnaceInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/FurnaceMinecartEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GhastEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GoatEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GrindStoneInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GroupFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GroupFilter_AllMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GroupFilter_AnyMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GroupFilter_CountMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GroupFilter_NoneMatchFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/GuardianEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/HTTPRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/HTTPRequest_Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_Add.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_HistoryStep.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_Remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_Replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_ShiftLine.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_TabLines.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/History_TabLinesKeepCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/HorseEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/HorseInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IAdvancedFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IBeaconScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IBossBarHud.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ICancelable.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ICategoryTreeParent.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IChatHud.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IChunkSection.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ICompare.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IContainerParent.py
--rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IDraw2D.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IEventListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IFWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IFontManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IHorseScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IItemCooldownEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IItemCooldownManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ILoomScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IMerchantEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IMerchantScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IMinecraftClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IMixinEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IOverlayParent.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IPackedIntegerArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IPalettedContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IPalettedContainerData.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IPlayerListHud.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IRecipeBookResults.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IRecipeBookWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IResourcePackManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IScreenInternal.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ISignEditScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IllagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Image_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IntField.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/IronGolemEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Item.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemFrameEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemStackHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Item_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/JsMacros.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/JsMacrosThreadPool.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/JsMacrosThreadPool_PoolThread.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/KeyListener.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/KeyMacrosScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Library.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LibraryBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LibraryRegistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line3D_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ListContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LivingEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LlamaEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LockButtonWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LockButtonWidgetHelper_LockButtonBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LongField.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/LoomInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MacroContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MacroListTopbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MacroScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Mappings_ClassData.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Mappings_MappedClass.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Mappings_MethodData.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MerchantEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MethodWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAbstractFurnaceScreenHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAbstractHorseEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAbstractPiglinEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAdvancementManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAdvancementProgress.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAdvancementRewards.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAllayEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinAnvilScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinBeaconScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinBoatEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinBossBarHud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinChatHud.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinChatScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinChunkSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientAdvancementManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientPlayNetworkHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientPlayerInteractionManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientWorld.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinCreativeInventoryScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinCreeperEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinCyclingButton.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinDisconnectedScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinFishingBobberEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinFontManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinFontStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinFoxEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinHandledScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinHorseEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinHorseScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinHungerManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinItemCooldownEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinItemCooldownManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinLivingEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinLoomScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinMerchantEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinMerchantScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinMinecraftClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinOcelotEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPackedIntegerArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPacketHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPalettedContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPalettedContainerData.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPhaseType.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPlayerEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinPlayerListHud.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinRecipeBookResults.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinRecipeBookWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinResourcePackManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinShulkerEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinSignEditScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinSimpleOption.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinSoundSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinSpellcastingIllagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinSplashOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinStatHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinStyleSerializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinTextFieldWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinTranslationStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinTridentEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinTrueTypeFont.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MobEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ModContainerHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ModLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MooshroomEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MovementDummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MovementQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/MultiElementContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper_NBTListHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NameUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Neighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NoStyleCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NotFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/NumberCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OcelotEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Option.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionType.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsField.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_AccessibilityOptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_ChatOptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_ControlOptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_MusicOptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_SkinOptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_VideoOptionsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OrFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/OverlayContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33397 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PacketByteBufferHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PaintingEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PandaEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ParrotEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PerExecLanguageLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PerExecLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PerLanguageLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PhantomEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PigEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PiglinEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PillagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Plane3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerAbilitiesHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerListEntryHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PolarBearEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Pos2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Pos3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PrimitiveSettingGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PrioryFiFoTaskQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_clike.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_groovy.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_javascript.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_kotlin.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_lua.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_ruby.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Prism_typescript.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ProfileSetting.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ProfileSetting_ProfileEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ProxyBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ProxyBuilder_ProxyReference.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/PufferfishEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RabbitEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RecipeHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RecipeInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Rect_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RegistryHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RenderElement.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RenderElement3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RenderElementBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/RunningContextContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScoreboardObjectiveHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScoreboardsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptCodeCompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptTrigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptTrigger_TriggerType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Scrollbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SelectCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SelectorDropdownOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServerInfoHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceListTopbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceManager_ServiceStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceTrigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SettingsOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SettingsOverlay_SettingField.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SheepEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ShulkerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SliderWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SliderWidgetHelper_SliderBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SlimeEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SmithingInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SnowGolemEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_MacroSortMethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_ServiceSortMethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortByEnabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortByFileName.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortByTriggerName.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortServiceByEnabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortServiceByFileName.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortServiceByName.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Sorting_SortServiceByRunning.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SpellcastingIllagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SpiderEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StateHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StatsHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StatusEffectHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StoneCutterInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StriderEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringCompareFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringCompareFilter_FilterMethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringField.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringHashTrie.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringMapSetting.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringMapSetting_StringEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringifyFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/StyleHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SuggestionsBuilderHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Surface_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/SynchronizedWeakHashSet.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TPSData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TameableEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TeamHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextFieldWidgetHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextFieldWidgetHelper_TextFieldBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 02:08:55.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextStyleCompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-02 02:08:53.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Text_Builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TickBasedEvents.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TickSync.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TntEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TntMinecartEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TradeOfferHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TranslationUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TridentEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/TropicalFishEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/UniversalBlockStateHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Vec2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Vec3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/VexEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/VillagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/VillagerInventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/VindicatorEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WardenEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/Websocket_Disconnected.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WitchEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WitherEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WitherSkullEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WolfEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WorldScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WorldScannerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WrappedClassInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 02:08:54.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WrappedClassInstance_MethodSigParts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 02:08:55.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/WrappedScript.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 02:08:55.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/XorFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-02 02:08:55.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ZombieEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-02 02:08:55.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/ZombieVillagerEntityHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-02 02:08:48.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-02 02:08:49.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-02 02:08:50.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-02 02:08:51.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-02 02:08:52.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:09:17.000000 JsMacrosAC-1.8.4.8263756/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 02:08:44.000000 JsMacrosAC-1.8.4.8263756/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AboutOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractHorseEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractMapSettingContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractPiglinEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractRenderCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractSettingContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractSettingField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractWidgetBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AdvancementHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AdvancementManagerHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AdvancementProgressHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Alignable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AllayEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AndFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AnimalEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AnnotatedCheckBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AnvilInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AreaEffectCloudEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ArmorStandEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ArrowEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AutoCompleteSuggester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AutoCompleteSuggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/AxolotlEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseEventRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseScriptContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseScriptContext_ScriptAssertionError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseScriptContext_SleepRunnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseWrappedException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseWrappedException_GuestLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseWrappedException_HostLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseWrappedException_SourceLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BasicFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BeaconInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BeeEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlazeEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockDataHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockPosHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockStateFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockStateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BoatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BooleanCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BooleanField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BossBarConsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BossBarHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Box_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/BrewingStandInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ButtonWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ButtonWidgetHelper_ButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ButtonWidgetHelper_TexturedButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CancelScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CancelScreen_RTCSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CartographyInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CategoryTreeContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CharCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ChatHistoryManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ChatHudLineHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBoxContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBoxWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBoxWidgetHelper_CheckBoxBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ChunkHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_AnnotationBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_BodyBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_ConstructorBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_FieldBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_MethodBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassWrapperFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClickableWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClientConfigV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClientPlayerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CodeCompileEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ColorMapSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ColorMapSetting_ColorEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandContextHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandNodeAccessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandNodeHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ConfigFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ConfirmOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ContainerInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CoreConfigV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CraftingInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CreativeInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CreativeItemStackHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CreeperEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CustomClickEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CustomImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CyclingButtonWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/CyclingButtonWidgetHelper_CyclicButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DefaultCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DirectionHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DocletEnumType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DocletReplaceParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DocletReplaceReturn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DocletReplaceTypeParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DocletTypescriptExtends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DolphinEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DonkeyEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DoubleField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw2DElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw2DElement_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-02 11:15:08.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DrownedEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/DyeColorHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EditorScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EnchantInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EnchantmentHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EndCrystalEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EnderDragonEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EndermanEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventAirChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventArmorChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventAttackBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventAttackEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventBlockUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventBossbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventChooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventChooser_EventObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventChunkLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventChunkUnload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventClickSlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDeath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDimensionChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDisconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDropSlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventEXPChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventEntityDamaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventEntityHealed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventEntityLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventEntityUnload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventFallFlying.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventHeal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventHealthChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventHeldItemChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventHungerChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventInteractBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventInteractEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventItemDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventItemPickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinedRecvPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinedSendPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinedTick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventLaunchGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventLockWatchdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventMacrosScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventOpenContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventOpenScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventPlayerJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventPlayerLeave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventProfileLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventQuitGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventRecvMessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventRecvPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventResourcePackLoaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventRiding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventSendMessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventSendPacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventSignEdit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventSound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventStatusEffectUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventTick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventWrappedScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ExtensionClassLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ExtensionLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Extension_ExtMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FChat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FGlobalVars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FJavaUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FJsMacros.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FJsMacros_EventAndContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FJsMacros_ScriptEventListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FKeyBind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FKeyBind_KeyTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FPositionCommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FReflection_CombinedVariableClassLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FWorld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FakeServerCommandSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FallingBlockEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileChooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileChooser_fileObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileChooser_sortFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileHandler_FileLineIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileMapSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileMapSetting_FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FishEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FishingBobberEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FloatField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FluidStateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FoodComponentHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FormattingHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FoxEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FrogEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FurnaceInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/FurnaceMinecartEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GhastEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GoatEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GrindStoneInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GroupFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GroupFilter_AllMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GroupFilter_AnyMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GroupFilter_CountMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GroupFilter_NoneMatchFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/GuardianEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/HTTPRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/HTTPRequest_Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_Add.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_HistoryStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_Remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_Replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_ShiftLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_TabLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/History_TabLinesKeepCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/HorseEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/HorseInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IAdvancedFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IBeaconScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IBossBarHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ICancelable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ICategoryTreeParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IChatHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IChunkSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ICompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IContainerParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IDraw2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IEventListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IFWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IFontManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IHorseScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IItemCooldownEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IItemCooldownManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ILoomScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IMerchantEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IMerchantScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IMinecraftClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IMixinEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IOverlayParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IPackedIntegerArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IPalettedContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IPalettedContainerData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IPlayerListHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IRecipeBookResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IRecipeBookWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IResourcePackManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IScreenInternal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ISignEditScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IllagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Image_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IntField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/IronGolemEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemFrameEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemStackHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Item_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/JsMacros.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/JsMacrosThreadPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/JsMacrosThreadPool_PoolThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/KeyListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/KeyMacrosScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LibraryBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LibraryRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line3D_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ListContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LivingEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LlamaEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LockButtonWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LockButtonWidgetHelper_LockButtonBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LongField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/LoomInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MacroContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MacroListTopbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MacroScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Mappings_ClassData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Mappings_MappedClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Mappings_MethodData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MerchantEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MethodWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAbstractFurnaceScreenHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAbstractHorseEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAbstractPiglinEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAdvancementManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAdvancementProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAdvancementRewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAllayEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinAnvilScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinBeaconScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinBoatEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinBossBarHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinChatHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinChatScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinChunkSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinClientAdvancementManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinClientConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinClientPlayNetworkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinClientPlayerInteractionManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinClientWorld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinCreativeInventoryScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinCreeperEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinCyclingButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinDisconnectedScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinFishingBobberEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinFontManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinFontStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinFoxEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinHandledScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinHorseEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinHorseScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinHungerManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinItemCooldownEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinItemCooldownManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-02 11:15:12.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinLivingEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinLoomScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinMerchantEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinMerchantScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinMinecraftClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinOcelotEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPackedIntegerArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPacketHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPalettedContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPalettedContainerData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPhaseType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPlayerEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinPlayerListHud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinRecipeBookResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinRecipeBookWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinResourcePackManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinShulkerEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinSignEditScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinSimpleOption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinSoundSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinSpellcastingIllagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinSplashOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinStatHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinStyleSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinTextFieldWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinTranslationStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinTridentEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinTrueTypeFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MobEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ModContainerHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ModLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MooshroomEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MovementDummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MovementQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/MultiElementContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper_NBTListHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NameUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NoStyleCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NotFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/NumberCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OcelotEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_AccessibilityOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_ChatOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_ControlOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_MusicOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_SkinOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_VideoOptionsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OrFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/OverlayContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34273 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PacketByteBufferHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PaintingEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PandaEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ParrotEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PerExecLanguageLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PerExecLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PerLanguageLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PhantomEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PigEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PiglinEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PillagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Plane3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerAbilitiesHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerListEntryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PolarBearEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Pos2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Pos3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PrimitiveSettingGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PrioryFiFoTaskQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_clike.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_groovy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_kotlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_lua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-02 11:15:14.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_ruby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Prism_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProfileSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProfileSetting_ProfileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProxyBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProxyBuilder_ProxyReference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/PufferfishEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RabbitEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RecipeHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RecipeInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Rect_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RegistryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RenderElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RenderElement3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RenderElementBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/RunningContextContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScoreboardObjectiveHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScoreboardsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScriptCodeCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScriptScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScriptTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScriptTrigger_TriggerType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Scrollbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SelectCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SelectorDropdownOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServerInfoHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceListTopbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceManager_ServiceStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SettingsOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SettingsOverlay_SettingField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SheepEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ShulkerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SliderWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SliderWidgetHelper_SliderBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SlimeEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SmithingInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SnowGolemEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_MacroSortMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_ServiceSortMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortByEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortByFileName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortByTriggerName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortServiceByEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortServiceByFileName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortServiceByName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Sorting_SortServiceByRunning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SpellcastingIllagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SpiderEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StatsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StatusEffectHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StoneCutterInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StriderEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringCompareFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringCompareFilter_FilterMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringHashTrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringMapSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringMapSetting_StringEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringifyFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/StyleHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SuggestionsBuilderHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Surface_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/SynchronizedWeakHashSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TPSData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TameableEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TeamHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextFieldWidgetHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextFieldWidgetHelper_TextFieldBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextStyleCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Text_Builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TickBasedEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TickSync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TntEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TntMinecartEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TradeOfferHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TranslationUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TridentEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/TropicalFishEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/UniversalBlockStateHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Vec2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Vec3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/VexEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/VillagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/VillagerInventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/VindicatorEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WardenEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/Websocket_Disconnected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WitchEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WitherEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WitherSkullEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WolfEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WorldScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WorldScannerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WrappedClassInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WrappedClassInstance_MethodSigParts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/WrappedScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/XorFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ZombieEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-02 11:15:16.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/ZombieVillagerEntityHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-02 11:15:09.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-02 11:15:10.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-02 11:15:11.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-02 11:15:13.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-02 11:15:15.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 11:15:36.000000 JsMacrosAC-1.8.5.8296535/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 11:15:07.000000 JsMacrosAC-1.8.5.8296535/setup.py
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AboutOverlay.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProfileSetting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .OverlayContainer import OverlayContainer
-from .IOverlayParent import IOverlayParent
+from .AbstractMapSettingContainer import AbstractMapSettingContainer
+from .SettingsOverlay import SettingsOverlay
+from .ScriptTrigger import ScriptTrigger
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-class AboutOverlay(OverlayContainer):
+
+class ProfileSetting(AbstractMapSettingContainer):
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def addField(self, key: str, value: List[ScriptTrigger]) -> None:
 		pass
 
 	@overload
-	def setMessage(self, message: Text) -> None:
+	def removeField(self, key: str) -> None:
 		pass
 
 	@overload
-	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
+	def changeKey(self, key: str, newKey: str) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractHorseEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractHorseEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractMapSettingContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractMapSettingContainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,26 @@
 from typing import Generic
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 from .SettingsOverlay import SettingsOverlay
 
 T = TypeVar("T")
 U = TypeVar("U")
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-OrderedText = TypeVar["net.minecraft.text.OrderedText"]
-Supplier = TypeVar["java.util.function.Supplier_T_"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_OrderedText = TypeVar("net_minecraft_text_OrderedText")
+OrderedText = net_minecraft_text_OrderedText
+
+java_util_function_Supplier_T_ = TypeVar("java_util_function_Supplier_T_")
+Supplier = java_util_function_Supplier_T_
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class AbstractMapSettingContainer(Generic[T, U], AbstractSettingContainer):
 	setting: SettingsOverlay_SettingField
 	settingName: OrderedText
 	map: Mapping[str, U]
 	topScroll: int
 	totalHeight: int
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractMapSettingContainer_MapSettingEntry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
 from .MultiElementContainer import MultiElementContainer
 from .AbstractMapSettingContainer import AbstractMapSettingContainer
 
 T = TypeVar("T")
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class AbstractMapSettingContainer_MapSettingEntry(Generic[T], MultiElementContainer):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractMapSettingContainer, key: str, value: T) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractRenderCodeCompiler.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractRenderCodeCompiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
-Runnable = TypeVar["java.lang.Runnable"]
-Text = TypeVar["net.minecraft.text.Text"]
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
 
 class AbstractRenderCodeCompiler:
 
 	@overload
 	def __init__(self, language: str, screen: EditorScreen) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractSettingContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractSettingContainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List
 from typing import TypeVar
 from .MultiElementContainer import MultiElementContainer
 from .Scrollbar import Scrollbar
 from .SettingsOverlay import SettingsOverlay
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class AbstractSettingContainer(MultiElementContainer):
 	group: List[str]
 	scroll: Scrollbar
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractSettingField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractSettingField.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import TypeVar
 from typing import Generic
 from .MultiElementContainer import MultiElementContainer
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
 T = TypeVar("T")
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class AbstractSettingField(Generic[T], MultiElementContainer):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AbstractWidgetBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AbstractWidgetBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
 from .Alignable import Alignable
 from .TextHelper import TextHelper
 
 B = TypeVar("B")
+B = B
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 class AbstractWidgetBuilder(Alignable, Generic[B, T, U]):
 	"""
 	Since: 1.8.4 
 	"""
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AdvancementHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AdvancementHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .BaseHelper import BaseHelper
 from .AdvancementProgressHelper import AdvancementProgressHelper
 
-Advancement = TypeVar["net.minecraft.advancement.Advancement"]
+net_minecraft_advancement_Advancement = TypeVar("net_minecraft_advancement_Advancement")
+Advancement = net_minecraft_advancement_Advancement
+
 
 class AdvancementHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AdvancementManagerHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AdvancementManagerHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .BaseHelper import BaseHelper
 from .AdvancementHelper import AdvancementHelper
 from .AdvancementProgressHelper import AdvancementProgressHelper
 
-AdvancementManager = TypeVar["net.minecraft.advancement.AdvancementManager"]
+net_minecraft_advancement_AdvancementManager = TypeVar("net_minecraft_advancement_AdvancementManager")
+AdvancementManager = net_minecraft_advancement_AdvancementManager
+
 
 class AdvancementManagerHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AdvancementProgressHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AdvancementProgressHelper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .BaseHelper import BaseHelper
 
-AdvancementProgress = TypeVar["net.minecraft.advancement.AdvancementProgress"]
-Date = TypeVar["java.util.Date"]
+net_minecraft_advancement_AdvancementProgress = TypeVar("net_minecraft_advancement_AdvancementProgress")
+AdvancementProgress = net_minecraft_advancement_AdvancementProgress
+
+java_util_Date = TypeVar("java_util_Date")
+Date = java_util_Date
+
 
 class AdvancementProgressHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Alignable.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Alignable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import overload
 from typing import TypeVar
 
 B = TypeVar("B")
+B = B
+
 
 class Alignable:
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AllayEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AllayEntityHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 
-AllayEntity = TypeVar["net.minecraft.entity.passive.AllayEntity"]
+net_minecraft_entity_passive_AllayEntity = TypeVar("net_minecraft_entity_passive_AllayEntity")
+AllayEntity = net_minecraft_entity_passive_AllayEntity
+
 
 class AllayEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AnimalEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AnimalEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AnnotatedCheckBox.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ConfirmOverlay.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 from typing import overload
 from typing import TypeVar
-from .Button import Button
+from .OverlayContainer import OverlayContainer
+from .IOverlayParent import IOverlayParent
 
-Consumer = TypeVar["java.util.function.Consumer_xyz.wagyourtail.wagyourgui.elements.Button_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Consumer_xyz_wagyourtail_wagyourgui_overlays_ConfirmOverlay_ = TypeVar("java_util_function_Consumer_xyz_wagyourtail_wagyourgui_overlays_ConfirmOverlay_")
+Consumer = java_util_function_Consumer_xyz_wagyourtail_wagyourgui_overlays_ConfirmOverlay_
 
-class AnnotatedCheckBox(Button):
-	value: bool
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
+
+class ConfirmOverlay(OverlayContainer):
+	hcenter: bool
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: Text, initialValue: bool, onPress: Consumer) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, message: Text, parent: IOverlayParent, accept: Consumer) -> None:
 		pass
 
 	@overload
-	def onPress(self) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, hcenter: bool, textRenderer: TextRenderer, message: Text, parent: IOverlayParent, accept: Consumer) -> None:
 		pass
 
 	@overload
 	def setMessage(self, message: Text) -> None:
 		pass
 
 	@overload
+	def init(self) -> None:
+		pass
+
+	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AnvilInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AnvilInventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .Inventory import Inventory
 from .ItemStackHelper import ItemStackHelper
 
-AnvilScreen = TypeVar["net.minecraft.client.gui.screen.ingame.AnvilScreen"]
+net_minecraft_client_gui_screen_ingame_AnvilScreen = TypeVar("net_minecraft_client_gui_screen_ingame_AnvilScreen")
+AnvilScreen = net_minecraft_client_gui_screen_ingame_AnvilScreen
+
 
 class AnvilInventory(Inventory):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AreaEffectCloudEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SlimeEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,40 @@
 from typing import overload
 from typing import TypeVar
-from .EntityHelper import EntityHelper
+from .MobEntityHelper import MobEntityHelper
 
-AreaEffectCloudEntity = TypeVar["net.minecraft.entity.AreaEffectCloudEntity"]
+net_minecraft_entity_mob_SlimeEntity = TypeVar("net_minecraft_entity_mob_SlimeEntity")
+SlimeEntity = net_minecraft_entity_mob_SlimeEntity
 
-class AreaEffectCloudEntityHelper(EntityHelper):
+
+class SlimeEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, e: AreaEffectCloudEntity) -> None:
-		pass
-
-	@overload
-	def getRadius(self) -> float:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the radius of this cloud. 
-		"""
+	def __init__(self, base: SlimeEntity) -> None:
 		pass
 
 	@overload
-	def getColor(self) -> int:
+	def getSize(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the color of this cloud. 
+			the size of this slime. 
 		"""
 		pass
 
 	@overload
-	def getParticleType(self) -> str:
-		"""
+	def isSmall(self) -> bool:
+		"""Small slimes, with a size less than 1, don't attack the player.\n
 		Since: 1.8.4 
 
 		Returns:
-			the id of this cloud's particles. 
-		"""
-		pass
-
-	@overload
-	def isWaiting(self) -> bool:
-		"""
-		Since: 1.8.4 
+			'true' if this slime is small, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ArmorStandEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ArmorStandEntityHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .LivingEntityHelper import LivingEntityHelper
 
-ArmorStandEntity = TypeVar["net.minecraft.entity.decoration.ArmorStandEntity"]
+net_minecraft_entity_decoration_ArmorStandEntity = TypeVar("net_minecraft_entity_decoration_ArmorStandEntity")
+ArmorStandEntity = net_minecraft_entity_decoration_ArmorStandEntity
+
 
 class ArmorStandEntityHelper(LivingEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ArrowEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ArrowEntityHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 
-PersistentProjectileEntity = TypeVar["net.minecraft.entity.projectile.PersistentProjectileEntity"]
+net_minecraft_entity_projectile_PersistentProjectileEntity = TypeVar("net_minecraft_entity_projectile_PersistentProjectileEntity")
+PersistentProjectileEntity = net_minecraft_entity_projectile_PersistentProjectileEntity
+
 
 class ArrowEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/AxolotlEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AxolotlEntityHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-AxolotlEntity = TypeVar["net.minecraft.entity.passive.AxolotlEntity"]
+net_minecraft_entity_passive_AxolotlEntity = TypeVar("net_minecraft_entity_passive_AxolotlEntity")
+AxolotlEntity = net_minecraft_entity_passive_AxolotlEntity
+
 
 class AxolotlEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseEventRegistry.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseEventRegistry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseLanguage.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseLanguage.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 from .Core import Core
 from .ScriptTrigger import ScriptTrigger
 from .BaseEvent import BaseEvent
 from .EventContainer import EventContainer
 from .BaseLibrary import BaseLibrary
 
 T = TypeVar("T")
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Throwable_"]
+java_util_function_Consumer_java_lang_Throwable_ = TypeVar("java_util_function_Consumer_java_lang_Throwable_")
+Consumer = java_util_function_Consumer_java_lang_Throwable_
+
 U = TypeVar("U")
-Runnable = TypeVar["java.lang.Runnable"]
-File = TypeVar["java.io.File"]
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class BaseLanguage(Generic[U, T]):
 	"""Language class for languages to be implemented on top of.\n
 	Since: 1.1.3 
 	"""
 	extension: Extension
 	preThread: Runnable
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseListener.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseListener.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseProfile.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TeamHelper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,155 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from typing import Set
-from .Core import Core
-from .BaseEventRegistry import BaseEventRegistry
-from .BaseEvent import BaseEvent
-
-Throwable = TypeVar["java.lang.Throwable"]
-Logger = TypeVar["org.slf4j.Logger"]
-Thread = TypeVar["java.lang.Thread"]
+from .BaseHelper import BaseHelper
+from .TextHelper import TextHelper
+from .FormattingHelper import FormattingHelper
+from .ScoreboardsHelper import ScoreboardsHelper
 
-class BaseProfile:
+net_minecraft_scoreboard_Team = TypeVar("net_minecraft_scoreboard_Team")
+Team = net_minecraft_scoreboard_Team
+
+
+class TeamHelper(BaseHelper):
 	"""
-	Since: 1.2.7 
+	Since: 1.3.0 
 	"""
-	LOGGER: Logger
-	joinedThreadStack: Set[Thread]
-	profileName: str
 
 	@overload
-	def __init__(self, runner: Core, logger: Logger) -> None:
+	def __init__(self, t: Team) -> None:
 		pass
 
 	@overload
-	def logError(self, ex: Throwable) -> None:
+	def getName(self) -> str:
+		"""
+		Since: 1.3.0 
+		"""
 		pass
 
 	@overload
-	def getRegistry(self) -> BaseEventRegistry:
+	def getDisplayName(self) -> TextHelper:
 		"""
-		Since: 1.1.2 [citation needed] 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def checkJoinedThreadStack(self) -> bool:
+	def getPlayerList(self) -> List[str]:
 		"""
-		Since: 1.6.0 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def loadOrCreateProfile(self, profileName: str) -> None:
+	def getColorFormat(self) -> FormattingHelper:
 		"""
-		Since: 1.1.2 [citation needed] 
+		Since: 1.8.4 
 
-		Args:
-			profileName: 
+		Returns:
+			the formatting of this team's color. 
 		"""
 		pass
 
 	@overload
-	def saveProfile(self) -> None:
+	def getColor(self) -> int:
 		"""
-		Since: 1.0.8 [citation needed] 
+		Since: 1.3.0 
 		"""
 		pass
 
 	@overload
-	def triggerEvent(self, event: BaseEvent) -> None:
+	def getColorIndex(self) -> int:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			event: 
+		Returns:
+			the color index of this team. 
 		"""
 		pass
 
 	@overload
-	def triggerEventJoin(self, event: BaseEvent) -> None:
+	def getColorValue(self) -> int:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			event: 
+		Returns:
+			the color value for this team or '-1' if it has no color. 
 		"""
 		pass
 
 	@overload
-	def triggerEventNoAnything(self, event: BaseEvent) -> None:
+	def getColorName(self) -> str:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			event: 
+		Returns:
+			the name of this team's color. 
 		"""
 		pass
 
 	@overload
-	def triggerEventJoinNoAnything(self, event: BaseEvent) -> None:
+	def getScoreboard(self) -> ScoreboardsHelper:
 		"""
-		Since: 1.2.7 
+		Since: 1.8.4 
 
-		Args:
-			event: 
+		Returns:
+			the scoreboard including this team. 
 		"""
 		pass
 
 	@overload
-	def init(self, defaultProfile: str) -> None:
+	def getPrefix(self) -> TextHelper:
+		"""
+		Since: 1.3.0 
+		"""
 		pass
 
 	@overload
-	def getCurrentProfileName(self) -> str:
+	def getSuffix(self) -> TextHelper:
+		"""
+		Since: 1.3.0 
+		"""
+		pass
+
+	@overload
+	def getCollisionRule(self) -> str:
+		"""
+		Since: 1.3.0 
+		"""
+		pass
+
+	@overload
+	def isFriendlyFire(self) -> bool:
+		"""
+		Since: 1.3.0 
+		"""
+		pass
+
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
+		"""
 		pass
 
 	@overload
-	def renameCurrentProfile(self, profile: str) -> None:
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MacroContainer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,64 @@
 from typing import overload
 from typing import TypeVar
-from .IOverlayParent import IOverlayParent
-from .OverlayContainer import OverlayContainer
+from .MultiElementContainer import MultiElementContainer
+from .ScriptTrigger import ScriptTrigger
+from .MacroScreen import MacroScreen
 
-T = TypeVar("T")
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Element = TypeVar["net.minecraft.client.gui.Element"]
-StringVisitable = TypeVar["net.minecraft.text.StringVisitable"]
-OrderedText = TypeVar["net.minecraft.text.OrderedText"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class BaseScreen(IOverlayParent, Screen):
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
 
-	@overload
-	def trimmed(self, textRenderer: TextRenderer, str: StringVisitable, width: int) -> OrderedText:
-		pass
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
 
-	@overload
-	def setParent(self, parent: Screen) -> None:
-		pass
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def reload(self) -> None:
-		pass
 
-	@overload
-	def removed(self) -> None:
-		pass
-
-	@overload
-	def openOverlay(self, overlay: OverlayContainer) -> None:
-		pass
-
-	@overload
-	def getFirstOverlayParent(self) -> IOverlayParent:
-		pass
+class MacroContainer(MultiElementContainer):
 
 	@overload
-	def getChildOverlay(self) -> OverlayContainer:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, macro: ScriptTrigger, parent: MacroScreen) -> None:
 		pass
 
 	@overload
-	def openOverlay(self, overlay: OverlayContainer, disableButtons: bool) -> None:
+	def getRawMacro(self) -> ScriptTrigger:
 		pass
 
 	@overload
-	def closeOverlay(self, overlay: OverlayContainer) -> None:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def remove(self, btn: Element) -> None:
+	def setEventType(self, type: str) -> None:
 		pass
 
 	@overload
-	def addDrawableChild(self, drawableElement: T) -> T:
+	def setFile(self, f: File) -> None:
 		pass
 
 	@overload
-	def setFocused(self, focused: Element) -> None:
+	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
-	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
+	def onKey(self, translationKey: str) -> bool:
 		pass
 
 	@overload
-	def mouseScrolled(self, mouseX: float, mouseY: float, amount: float) -> bool:
+	def buildKeyName(self, translationKeys: str) -> Text:
 		pass
 
 	@overload
-	def mouseClicked(self, mouseX: float, mouseY: float, button: int) -> bool:
+	def setKey(self, translationKeys: str) -> None:
 		pass
 
 	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
-	@overload
-	def shouldCloseOnEsc(self) -> bool:
-		pass
-
-	@overload
-	def updateSettings(self) -> None:
-		pass
-
-	@overload
-	def close(self) -> None:
-		pass
-
-	@overload
-	def openParent(self) -> None:
-		pass
-
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseScriptContext.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseScriptContext.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 from typing import Set
 from typing import Generic
 from .BaseEvent import BaseEvent
 from .EventContainer import EventContainer
 from .BaseScriptContext_SleepRunnable import BaseScriptContext_SleepRunnable
 
 T = TypeVar("T")
-WeakReference = TypeVar["java.lang.ref.WeakReference_java.lang.Object_"]
-File = TypeVar["java.io.File"]
-Thread = TypeVar["java.lang.Thread"]
+java_lang_ref_WeakReference_java_lang_Object_ = TypeVar("java_lang_ref_WeakReference_java_lang_Object_")
+WeakReference = java_lang_ref_WeakReference_java_lang_Object_
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
+java_lang_Thread = TypeVar("java_lang_Thread")
+Thread = java_lang_Thread
+
 
 class BaseScriptContext(Generic[T]):
 	"""
 	Since: 1.4.0 
 	"""
 	startTime: float
 	syncObject: WeakReference
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BaseWrappedException.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseWrappedException.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
 from .BaseWrappedException_SourceLocation import BaseWrappedException_SourceLocation
 
 T = TypeVar("T")
-StackTraceElement = TypeVar["java.lang.StackTraceElement"]
+java_lang_StackTraceElement = TypeVar("java_lang_StackTraceElement")
+StackTraceElement = java_lang_StackTraceElement
+
 
 class BaseWrappedException(Generic[T]):
 	stackFrame: T
 	location: BaseWrappedException_SourceLocation
 	message: str
 	next: "BaseWrappedException"
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BasicFilter.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BasicFilter.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BeaconInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BeaconInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BeeEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StriderEntityHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-BeeEntity = TypeVar["net.minecraft.entity.passive.BeeEntity"]
+net_minecraft_entity_passive_StriderEntity = TypeVar("net_minecraft_entity_passive_StriderEntity")
+StriderEntity = net_minecraft_entity_passive_StriderEntity
 
-class BeeEntityHelper(AnimalEntityHelper):
+
+class StriderEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: BeeEntity) -> None:
-		pass
-
-	@overload
-	def hasNectar(self) -> bool:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			'true' if the bee has nectar, 'false' otherwise. 
-		"""
+	def __init__(self, base: StriderEntity) -> None:
 		pass
 
 	@overload
-	def isAngry(self) -> bool:
+	def isSaddled(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the bee is angry at a player, 'false' otherwise. 
+			'true' if this strider is saddled, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def hasStung(self) -> bool:
+	def isShivering(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the bee has already stung a player, 'false' otherwise. 
+			'true' if this strider is shivering in the cold, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockDataHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockDataHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,26 @@
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 from .NBTElementHelper import NBTElementHelper
 from .BlockStateHelper import BlockStateHelper
 from .BlockHelper import BlockHelper
 from .BlockPosHelper import BlockPosHelper
 
-BlockState = TypeVar["net.minecraft.block.BlockState"]
-Block = TypeVar["net.minecraft.block.Block"]
-BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
-BlockEntity = TypeVar["net.minecraft.block.entity.BlockEntity"]
+net_minecraft_block_BlockState = TypeVar("net_minecraft_block_BlockState")
+BlockState = net_minecraft_block_BlockState
+
+net_minecraft_block_Block = TypeVar("net_minecraft_block_Block")
+Block = net_minecraft_block_Block
+
+net_minecraft_util_math_BlockPos = TypeVar("net_minecraft_util_math_BlockPos")
+BlockPos = net_minecraft_util_math_BlockPos
+
+net_minecraft_block_entity_BlockEntity = TypeVar("net_minecraft_block_entity_BlockEntity")
+BlockEntity = net_minecraft_block_entity_BlockEntity
+
 
 class BlockDataHelper(BaseHelper):
 	"""
 	"""
 
 	@overload
 	def __init__(self, b: BlockState, e: BlockEntity, bp: BlockPos) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .BlockStateHelper import BlockStateHelper
 from .ItemStackHelper import ItemStackHelper
 from .TextHelper import TextHelper
 
-Block = TypeVar["net.minecraft.block.Block"]
+net_minecraft_block_Block = TypeVar("net_minecraft_block_Block")
+Block = net_minecraft_block_Block
+
 
 class BlockHelper(BaseHelper):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockPosHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockPosHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .EntityHelper import EntityHelper
 from .Pos3D import Pos3D
 
-BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
+net_minecraft_util_math_BlockPos = TypeVar("net_minecraft_util_math_BlockPos")
+BlockPos = net_minecraft_util_math_BlockPos
+
 
 class BlockPosHelper(BaseHelper):
 	"""
 	Since: 1.2.6 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BlockStateHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BlockStateHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import TypeVar
 from .StateHelper import StateHelper
 from .BlockHelper import BlockHelper
 from .FluidStateHelper import FluidStateHelper
 from .BlockPosHelper import BlockPosHelper
 from .UniversalBlockStateHelper import UniversalBlockStateHelper
 
-BlockState = TypeVar["net.minecraft.block.BlockState"]
+net_minecraft_block_BlockState = TypeVar("net_minecraft_block_BlockState")
+BlockState = net_minecraft_block_BlockState
+
 
 class BlockStateHelper(StateHelper):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BoatEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BoatEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 from .BlockHelper import BlockHelper
 
-BoatEntity = TypeVar["net.minecraft.entity.vehicle.BoatEntity"]
+net_minecraft_entity_vehicle_BoatEntity = TypeVar("net_minecraft_entity_vehicle_BoatEntity")
+BoatEntity = net_minecraft_entity_vehicle_BoatEntity
+
 
 class BoatEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BooleanField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileMapSetting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .AbstractSettingField import AbstractSettingField
-from .AbstractSettingContainer import AbstractSettingContainer
-from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
+from .AbstractMapSettingContainer import AbstractMapSettingContainer
+from .SettingsOverlay import SettingsOverlay
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-class BooleanField(AbstractSettingField):
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
-		pass
-
-	@overload
-	def init(self) -> None:
-		pass
+class FileMapSetting(AbstractMapSettingContainer):
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
 		pass
 
 	@overload
-	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
+	def addField(self, key: str, value: str) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BossBarHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BossBarHelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .FormattingHelper import FormattingHelper
 from .TextHelper import TextHelper
 
-BossBar = TypeVar["net.minecraft.entity.boss.BossBar"]
+net_minecraft_entity_boss_BossBar = TypeVar("net_minecraft_entity_boss_BossBar")
+BossBar = net_minecraft_entity_boss_BossBar
+
 
 class BossBarHelper(BaseHelper):
 	"""
 	Since: 1.2.1 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Box.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Box.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement3D import RenderElement3D
 from .Vec3D import Vec3D
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-BufferBuilder = TypeVar["net.minecraft.client.render.BufferBuilder"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_render_BufferBuilder = TypeVar("net_minecraft_client_render_BufferBuilder")
+BufferBuilder = net_minecraft_client_render_BufferBuilder
+
 
 class Box(RenderElement3D):
 	"""
 	"""
 	pos: Vec3D
 	color: int
 	fillColor: int
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Box_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Box_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/BrewingStandInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BrewingStandInventory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .Inventory import Inventory
 from .ItemStackHelper import ItemStackHelper
 
-BrewingStandScreen = TypeVar["net.minecraft.client.gui.screen.ingame.BrewingStandScreen"]
+net_minecraft_client_gui_screen_ingame_BrewingStandScreen = TypeVar("net_minecraft_client_gui_screen_ingame_BrewingStandScreen")
+BrewingStandScreen = net_minecraft_client_gui_screen_ingame_BrewingStandScreen
+
 
 class BrewingStandInventory(Inventory):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Button.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Button.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from typing import overload
 from typing import TypeVar
 
-Consumer = TypeVar["java.util.function.Consumer_xyz.wagyourtail.wagyourgui.elements.Button_"]
-PressableWidget = TypeVar["net.minecraft.client.gui.widget.PressableWidget"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_Button_ = TypeVar("java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_Button_")
+Consumer = java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_Button_
+
+net_minecraft_client_gui_widget_PressableWidget = TypeVar("net_minecraft_client_gui_widget_PressableWidget")
+PressableWidget = net_minecraft_client_gui_widget_PressableWidget
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class Button(PressableWidget):
 	horizCenter: bool
 	onPress: Consumer
 	hovering: bool
 	forceHover: bool
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ButtonWidgetHelper_ButtonBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ButtonWidgetHelper_ButtonBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ButtonWidgetHelper_TexturedButtonBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ButtonWidgetHelper_TexturedButtonBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CancelScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CancelScreen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import TypeVar
 from .BaseScreen import BaseScreen
 from .BaseScriptContext import BaseScriptContext
 from .RunningContextContainer import RunningContextContainer
 
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_screen_Screen = TypeVar("net_minecraft_client_gui_screen_Screen")
+Screen = net_minecraft_client_gui_screen_Screen
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class CancelScreen(BaseScreen):
 
 	@overload
 	def __init__(self, parent: Screen) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CartographyInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CartographyInventory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .Inventory import Inventory
 from .ItemStackHelper import ItemStackHelper
 
-CartographyTableScreen = TypeVar["net.minecraft.client.gui.screen.ingame.CartographyTableScreen"]
+net_minecraft_client_gui_screen_ingame_CartographyTableScreen = TypeVar("net_minecraft_client_gui_screen_ingame_CartographyTableScreen")
+CartographyTableScreen = net_minecraft_client_gui_screen_ingame_CartographyTableScreen
+
 
 class CartographyInventory(Inventory):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CatEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FrogEntityHelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from typing import overload
 from typing import TypeVar
-from .TameableEntityHelper import TameableEntityHelper
-from .DyeColorHelper import DyeColorHelper
+from .AnimalEntityHelper import AnimalEntityHelper
+from .EntityHelper import EntityHelper
 
-CatEntity = TypeVar["net.minecraft.entity.passive.CatEntity"]
+net_minecraft_entity_passive_FrogEntity = TypeVar("net_minecraft_entity_passive_FrogEntity")
+FrogEntity = net_minecraft_entity_passive_FrogEntity
 
-class CatEntityHelper(TameableEntityHelper):
+
+class FrogEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: CatEntity) -> None:
+	def __init__(self, base: FrogEntity) -> None:
 		pass
 
 	@overload
-	def isSleeping(self) -> bool:
+	def getVariant(self) -> str:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this cat is sleeping, 'false' otherwise. 
+			the variant of this frog. 
 		"""
 		pass
 
 	@overload
-	def getCollarColor(self) -> DyeColorHelper:
+	def getTarget(self) -> EntityHelper:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the color of this cat's collar. 
+			the target of this frog, or 'null' if it has none. 
 		"""
 		pass
 
 	@overload
-	def getVariant(self) -> str:
+	def isCroaking(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the variant of this cat. 
+			'true' if this frog is croaking, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CategoryTreeContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CategoryTreeContainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 from typing import TypeVar
 from typing import Mapping
 from .ICategoryTreeParent import ICategoryTreeParent
 from .MultiElementContainer import MultiElementContainer
 from .Scrollbar import Scrollbar
 from .Button import Button
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class CategoryTreeContainer(ICategoryTreeParent, MultiElementContainer):
 	category: str
 	scroll: Scrollbar
 	children: Mapping[str, "CategoryTreeContainer"]
 	expandBtn: Button
 	showBtn: Button
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ChatHistoryManager.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ChatHistoryManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .ChatHudLineHelper import ChatHudLineHelper
 from .TextHelper import TextHelper
 from .MethodWrapper import MethodWrapper
 
-ChatHud = TypeVar["net.minecraft.client.gui.hud.ChatHud"]
+net_minecraft_client_gui_hud_ChatHud = TypeVar("net_minecraft_client_gui_hud_ChatHud")
+ChatHud = net_minecraft_client_gui_hud_ChatHud
+
 
 class ChatHistoryManager:
 	"""
 	Since: 1.6.0 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ChatHudLineHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDeath.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from typing import overload
-from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
+from typing import List
+from .BaseEvent import BaseEvent
+from .BlockPosHelper import BlockPosHelper
+from .ItemStackHelper import ItemStackHelper
 
-ChatHudLine = TypeVar["net.minecraft.client.gui.hud.ChatHudLine"]
-ChatHud = TypeVar["net.minecraft.client.gui.hud.ChatHud"]
 
-class ChatHudLineHelper(BaseHelper):
+class EventDeath(BaseEvent):
+	"""
+	Since: 1.2.7 
+	"""
+	deathPos: BlockPosHelper
+	inventory: List[ItemStackHelper]
 
 	@overload
-	def __init__(self, base: ChatHudLine, hud: ChatHud) -> None:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def getText(self) -> TextHelper:
-		pass
-
-	@overload
-	def getCreationTick(self) -> int:
-		pass
-
-	@overload
-	def deleteById(self) -> "ChatHudLineHelper":
+	def respawn(self) -> None:
+		"""Respawns the player. Should be used with some delay, one tick should be enough.\n
+		Since: 1.8.4 
+		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBox.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import overload
 from typing import TypeVar
 
-Consumer = TypeVar["java.util.function.Consumer_xyz.wagyourtail.wagyourgui.elements.CheckBox_"]
-CheckboxWidget = TypeVar["net.minecraft.client.gui.widget.CheckboxWidget"]
-Text = TypeVar["net.minecraft.text.Text"]
+java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_CheckBox_ = TypeVar("java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_CheckBox_")
+Consumer = java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_CheckBox_
+
+net_minecraft_client_gui_widget_CheckboxWidget = TypeVar("net_minecraft_client_gui_widget_CheckboxWidget")
+CheckboxWidget = net_minecraft_client_gui_widget_CheckboxWidget
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
 
 class CheckBox(CheckboxWidget):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBoxContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceContainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,51 @@
 from typing import overload
 from typing import TypeVar
 from .MultiElementContainer import MultiElementContainer
-from .IContainerParent import IContainerParent
+from .ServiceScreen import ServiceScreen
+from .ServiceTrigger import ServiceTrigger
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Boolean_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class CheckBoxContainer(MultiElementContainer):
-	message: Text
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
+
+class ServiceContainer(MultiElementContainer):
+	service: str
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, defaultState: bool, message: Text, parent: IContainerParent, setState: Consumer) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: ServiceScreen, service: str) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
+	def getEnabled(self) -> bool:
+		pass
+
+	@overload
+	def getRunning(self) -> bool:
+		pass
+
+	@overload
+	def getTrigger(self) -> ServiceTrigger:
+		pass
+
+	@overload
+	def setFile(self, file: File) -> None:
+		pass
+
+	@overload
 	def setPos(self, x: int, y: int, width: int, height: int) -> None:
 		pass
 
 	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBoxWidgetHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBoxWidgetHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CheckBoxWidgetHelper_CheckBoxBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CheckBoxWidgetHelper_CheckBoxBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ChunkHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ChunkHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 from typing import List
 from typing import TypeVar
 from typing import Any
 from .BaseHelper import BaseHelper
 from .BlockPosHelper import BlockPosHelper
 from .MethodWrapper import MethodWrapper
 
-Heightmap = TypeVar["net.minecraft.world.Heightmap"]
-Map_Entry = TypeVar["java.util.Map.Entry_net.minecraft.world.Heightmap.Type,net.minecraft.world.Heightmap_"]
-Chunk = TypeVar["net.minecraft.world.chunk.Chunk"]
+net_minecraft_world_Heightmap = TypeVar("net_minecraft_world_Heightmap")
+Heightmap = net_minecraft_world_Heightmap
+
+java_util_Map_Entry_net_minecraft_world_Heightmap_Type,net_minecraft_world_Heightmap_ = TypeVar("java_util_Map_Entry_net_minecraft_world_Heightmap_Type,net_minecraft_world_Heightmap_")
+Map_Entry = java_util_Map_Entry_net_minecraft_world_Heightmap_Type,net_minecraft_world_Heightmap_
+
+net_minecraft_world_chunk_Chunk = TypeVar("net_minecraft_world_chunk_Chunk")
+Chunk = net_minecraft_world_chunk_Chunk
+
 
 class ChunkHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_AnnotationBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_AnnotationBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_AnnotationBuilder_AnnotationArrayBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_BodyBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_BodyBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_ConstructorBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_ConstructorBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_FieldBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_FieldBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_FieldBuilder_FieldInitializerBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClassBuilder_MethodBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClassBuilder_MethodBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClickableWidgetHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClickableWidgetHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 from typing import Generic
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 
 B = TypeVar("B")
+B = B
+
 T = TypeVar("T")
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
 
 class ClickableWidgetHelper(RenderElement, Alignable, Generic[B, T], BaseHelper):
 	"""
 	Since: 1.0.5 
 	"""
 	zIndex: int
 	tooltips: List[Text]
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClientConfigV2.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClientConfigV2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .Sorting_MacroSortMethod import Sorting_MacroSortMethod
 from .Sorting_ServiceSortMethod import Sorting_ServiceSortMethod
 
-JsonObject = TypeVar["com.google.gson.JsonObject"]
-Comparator = TypeVar["java.util.Comparator_java.lang.String_"]
+com_google_gson_JsonObject = TypeVar("com_google_gson_JsonObject")
+JsonObject = com_google_gson_JsonObject
+
+java_util_Comparator_java_lang_String_ = TypeVar("java_util_Comparator_java_lang_String_")
+Comparator = java_util_Comparator_java_lang_String_
+
 
 class ClientConfigV2:
 	sortMethod: Sorting_MacroSortMethod
 	sortServicesMethod: Sorting_ServiceSortMethod
 	showSlotIndexes: bool
 	disableKeyWhenScreenOpen: bool
 	editorTheme: Mapping[str, List[float]]
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ClientPlayerEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ClientPlayerEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CodeCompileEvent.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CodeCompileEvent.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from .EditorScreen import EditorScreen
 from .TextHelper import TextHelper
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 from .MethodWrapper import MethodWrapper
 from .TextBuilder import TextBuilder
 from .StringHashTrie import StringHashTrie
 
-Prism4j_Node = TypeVar["io.noties.prism4j.Prism4j.Node"]
+io_noties_prism4j_Prism4j_Node = TypeVar("io_noties_prism4j_Prism4j_Node")
+Prism4j_Node = io_noties_prism4j_Prism4j_Node
+
 
 class CodeCompileEvent(BaseEvent):
 	""""hidden" event for script based code style compiling / linting tasks.
 remember to 'consumer.autoWrap()' everything.\n
 	Since: 1.3.1 
 	"""
 	cursor: SelectCursor
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ColorMapSetting.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringMapSetting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .AbstractMapSettingContainer import AbstractMapSettingContainer
 from .SettingsOverlay import SettingsOverlay
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-class ColorMapSetting(AbstractMapSettingContainer):
+
+class StringMapSetting(AbstractMapSettingContainer):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
 		pass
 
 	@overload
-	def addField(self, key: str, value: List[float]) -> None:
+	def addField(self, key: str, value: str) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ColorMapSetting_ColorEntry.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ColorMapSetting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from .AbstractMapSettingContainer_MapSettingEntry import AbstractMapSettingContainer_MapSettingEntry
-from .ColorMapSetting import ColorMapSetting
+from .AbstractMapSettingContainer import AbstractMapSettingContainer
+from .SettingsOverlay import SettingsOverlay
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-class ColorMapSetting_ColorEntry(AbstractMapSettingContainer_MapSettingEntry):
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: ColorMapSetting, key: str, value: List[float]) -> None:
-		pass
-
-	@overload
-	def convertColorToString(self, color: List[float]) -> str:
-		pass
-
-	@overload
-	def convertStringToColor(self, color: str) -> List[float]:
-		pass
+class ColorMapSetting(AbstractMapSettingContainer):
 
 	@overload
-	def convertColorToInt(self, color: List[float]) -> int:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def addField(self, key: str, value: List[float]) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandContextHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandContextHelper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .BaseHelper import BaseHelper
 
-CommandContext = TypeVar["com.mojang.brigadier.context.CommandContext__"]
-StringRange = TypeVar["com.mojang.brigadier.context.StringRange"]
+com_mojang_brigadier_context_CommandContext__ = TypeVar("com_mojang_brigadier_context_CommandContext__")
+CommandContext = com_mojang_brigadier_context_CommandContext__
+
+com_mojang_brigadier_context_StringRange = TypeVar("com_mojang_brigadier_context_StringRange")
+StringRange = com_mojang_brigadier_context_StringRange
+
 
 class CommandContextHelper(BaseEvent, BaseHelper):
 	"""
 	Since: 1.4.2 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CommandManager.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CommandManager.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ConfigManager.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ConfigManager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from typing import overload
 from typing import TypeVar
 from typing import Mapping
 
 T = TypeVar("T")
-JsonObject = TypeVar["com.google.gson.JsonObject"]
-Logger = TypeVar["org.slf4j.Logger"]
-File = TypeVar["java.io.File"]
+com_google_gson_JsonObject = TypeVar("com_google_gson_JsonObject")
+JsonObject = com_google_gson_JsonObject
+
+org_slf4j_Logger = TypeVar("org_slf4j_Logger")
+Logger = org_slf4j_Logger
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class ConfigManager:
 	optionClasses: Mapping[str, Class]
 	options: Mapping[Class, object]
 	configFolder: File
 	macroFolder: File
 	configFile: File
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ConfirmOverlay.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AnnotatedCheckBox.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from typing import overload
 from typing import TypeVar
-from .OverlayContainer import OverlayContainer
-from .IOverlayParent import IOverlayParent
+from .Button import Button
 
-Consumer = TypeVar["java.util.function.Consumer_xyz.wagyourtail.wagyourgui.overlays.ConfirmOverlay_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_Button_ = TypeVar("java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_Button_")
+Consumer = java_util_function_Consumer_xyz_wagyourtail_wagyourgui_elements_Button_
 
-class ConfirmOverlay(OverlayContainer):
-	hcenter: bool
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, message: Text, parent: IOverlayParent, accept: Consumer) -> None:
-		pass
+
+class AnnotatedCheckBox(Button):
+	value: bool
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, hcenter: bool, textRenderer: TextRenderer, message: Text, parent: IOverlayParent, accept: Consumer) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: Text, initialValue: bool, onPress: Consumer) -> None:
 		pass
 
 	@overload
-	def setMessage(self, message: Text) -> None:
+	def onPress(self) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def setMessage(self, message: Text) -> None:
 		pass
 
 	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Core.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Core.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,37 @@
 from .JsMacrosThreadPool import JsMacrosThreadPool
 from .EventContainer import EventContainer
 from .BaseScriptContext import BaseScriptContext
 from .ScriptTrigger import ScriptTrigger
 from .BaseEvent import BaseEvent
 from .BaseWrappedException import BaseWrappedException
 
-Function = TypeVar["java.util.function.Function_xyz.wagyourtail.jsmacros.core.Core_V,R_,R_"]
+java_util_function_Function_xyz_wagyourtail_jsmacros_core_Core_V,R_,R_ = TypeVar("java_util_function_Function_xyz_wagyourtail_jsmacros_core_Core_V,R_,R_")
+Function = java_util_function_Function_xyz_wagyourtail_jsmacros_core_Core_V,R_,R_
+
 T = TypeVar("T")
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Throwable_"]
+java_util_function_Consumer_java_lang_Throwable_ = TypeVar("java_util_function_Consumer_java_lang_Throwable_")
+Consumer = java_util_function_Consumer_java_lang_Throwable_
+
 U = TypeVar("U")
-BiFunction = TypeVar["java.util.function.BiFunction_xyz.wagyourtail.jsmacros.core.Core_V,R_,org.slf4j.Logger,V_"]
-Runnable = TypeVar["java.lang.Runnable"]
-Throwable = TypeVar["java.lang.Throwable"]
-Logger = TypeVar["org.slf4j.Logger"]
-File = TypeVar["java.io.File"]
+java_util_function_BiFunction_xyz_wagyourtail_jsmacros_core_Core_V,R_,org_slf4j_Logger,V_ = TypeVar("java_util_function_BiFunction_xyz_wagyourtail_jsmacros_core_Core_V,R_,org_slf4j_Logger,V_")
+BiFunction = java_util_function_BiFunction_xyz_wagyourtail_jsmacros_core_Core_V,R_,org_slf4j_Logger,V_
+
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
+
+java_lang_Throwable = TypeVar("java_lang_Throwable")
+Throwable = java_lang_Throwable
+
+org_slf4j_Logger = TypeVar("org_slf4j_Logger")
+Logger = org_slf4j_Logger
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class Core(Generic[T, U]):
 	libraryRegistry: LibraryRegistry
 	eventRegistry: BaseEventRegistry
 	extensions: ExtensionLoader
 	profile: T
 	config: ConfigManager
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CoreConfigV2.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CoreConfigV2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .ScriptTrigger import ScriptTrigger
 from .ServiceTrigger import ServiceTrigger
 
-JsonObject = TypeVar["com.google.gson.JsonObject"]
+com_google_gson_JsonObject = TypeVar("com_google_gson_JsonObject")
+JsonObject = com_google_gson_JsonObject
+
 
 class CoreConfigV2:
 	maxLockTime: float
 	defaultProfile: str
 	profiles: Mapping[str, List[ScriptTrigger]]
 	services: Mapping[str, ServiceTrigger]
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CraftingInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CraftingInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CreativeInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CreativeInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CreativeItemStackHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CreativeItemStackHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .ItemStackHelper import ItemStackHelper
 from .TextHelper import TextHelper
 from .EnchantmentHelper import EnchantmentHelper
 
-ItemStack = TypeVar["net.minecraft.item.ItemStack"]
+net_minecraft_item_ItemStack = TypeVar("net_minecraft_item_ItemStack")
+ItemStack = net_minecraft_item_ItemStack
+
 
 class CreativeItemStackHelper(ItemStackHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CreeperEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CreeperEntityHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 
-CreeperEntity = TypeVar["net.minecraft.entity.mob.CreeperEntity"]
+net_minecraft_entity_mob_CreeperEntity = TypeVar("net_minecraft_entity_mob_CreeperEntity")
+CreeperEntity = net_minecraft_entity_mob_CreeperEntity
+
 
 class CreeperEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CustomImage.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CustomImage.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CyclingButtonWidgetHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CyclingButtonWidgetHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
 from .ClickableWidgetHelper import ClickableWidgetHelper
 
 T = TypeVar("T")
-CyclingButtonWidget = TypeVar["net.minecraft.client.gui.widget.CyclingButtonWidget_T_"]
+net_minecraft_client_gui_widget_CyclingButtonWidget_T_ = TypeVar("net_minecraft_client_gui_widget_CyclingButtonWidget_T_")
+CyclingButtonWidget = net_minecraft_client_gui_widget_CyclingButtonWidget_T_
+
 
 class CyclingButtonWidgetHelper(Generic[T], ClickableWidgetHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/CyclingButtonWidgetHelper_CyclicButtonBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CyclingButtonWidgetHelper_CyclicButtonBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/DefaultCodeCompiler.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScriptCodeCompiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,30 @@
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
-Runnable = TypeVar["java.lang.Runnable"]
-Text = TypeVar["net.minecraft.text.Text"]
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
 
-class DefaultCodeCompiler(AbstractRenderCodeCompiler):
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
+
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

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/DirectionHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/DirectionHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .Pos3D import Pos3D
 
-Direction = TypeVar["net.minecraft.util.math.Direction"]
+net_minecraft_util_math_Direction = TypeVar("net_minecraft_util_math_Direction")
+Direction = net_minecraft_util_math_Direction
+
 
 class DirectionHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/DolphinEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/AreaEffectCloudEntityHelper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 from typing import overload
 from typing import TypeVar
-from .MobEntityHelper import MobEntityHelper
-from .BlockPosHelper import BlockPosHelper
+from .EntityHelper import EntityHelper
 
-DolphinEntity = TypeVar["net.minecraft.entity.passive.DolphinEntity"]
+net_minecraft_entity_AreaEffectCloudEntity = TypeVar("net_minecraft_entity_AreaEffectCloudEntity")
+AreaEffectCloudEntity = net_minecraft_entity_AreaEffectCloudEntity
 
-class DolphinEntityHelper(MobEntityHelper):
+
+class AreaEffectCloudEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: DolphinEntity) -> None:
+	def __init__(self, e: AreaEffectCloudEntity) -> None:
 		pass
 
 	@overload
-	def hasFish(self) -> bool:
+	def getRadius(self) -> float:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the dolphin has a fish in its mouth, 'false' otherwise. 
+			the radius of this cloud. 
 		"""
 		pass
 
 	@overload
-	def getTreasurePos(self) -> BlockPosHelper:
-		"""The position will be 0 0 0 by default.\n
+	def getColor(self) -> int:
+		"""
 		Since: 1.8.4 
 
 		Returns:
-			the position of the treasure the dolphin is looking for. 
+			the color of this cloud. 
 		"""
 		pass
 
 	@overload
-	def getMoistness(self) -> int:
+	def getParticleType(self) -> str:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the moisture level of the dolphin. 
+			the id of this cloud's particles. 
+		"""
+		pass
+
+	@overload
+	def isWaiting(self) -> bool:
+		"""
+		Since: 1.8.4 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/DoubleField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceListTopbar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from typing import overload
 from typing import TypeVar
-from .AbstractSettingField import AbstractSettingField
-from .AbstractSettingContainer import AbstractSettingContainer
-from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
+from .MultiElementContainer import MultiElementContainer
+from .ServiceScreen import ServiceScreen
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class DoubleField(AbstractSettingField):
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
-		pass
+
+class ServiceListTopbar(MultiElementContainer):
 
 	@overload
-	def init(self) -> None:
+	def __init__(self, parent: ServiceScreen, x: int, y: int, width: int, height: int, textRenderer: TextRenderer) -> None:
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
+	def init(self) -> None:
 		pass
 
 	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw2D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 from .Image import Image
 from .Draw2DElement import Draw2DElement
 from .RenderElement import RenderElement
 from .TextHelper import TextHelper
 from .ItemStackHelper import ItemStackHelper
 
 T = TypeVar("T")
-IntSupplier = TypeVar["java.util.function.IntSupplier"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+java_util_function_IntSupplier = TypeVar("java_util_function_IntSupplier")
+IntSupplier = java_util_function_IntSupplier
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class Draw2D(IDraw2D):
 	"""
 	Since: 1.0.5 
 	"""
 	widthSupplier: IntSupplier
 	heightSupplier: IntSupplier
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw2DElement.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw2DElement.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .Draw2D import Draw2D
 from .IDraw2D import IDraw2D
 
-IntSupplier = TypeVar["java.util.function.IntSupplier"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+java_util_function_IntSupplier = TypeVar("java_util_function_IntSupplier")
+IntSupplier = java_util_function_IntSupplier
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class Draw2DElement(RenderElement, Alignable):
 	"""
 	Since: 1.8.4 
 	"""
 	draw2D: Draw2D
 	parent: IDraw2D
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw2DElement_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw2DElement_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Draw3D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Draw3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from .RenderElement3D import RenderElement3D
 from .Pos3D import Pos3D
 from .Box_Builder import Box_Builder
 from .BlockPosHelper import BlockPosHelper
 from .Line3D_Builder import Line3D_Builder
 from .Surface_Builder import Surface_Builder
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class Draw3D:
 	"""Draw2D is cool\n
 	Since: 1.0.6 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/DrownedEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/DrownedEntityHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .ZombieEntityHelper import ZombieEntityHelper
 
-DrownedEntity = TypeVar["net.minecraft.entity.mob.DrownedEntity"]
+net_minecraft_entity_mob_DrownedEntity = TypeVar("net_minecraft_entity_mob_DrownedEntity")
+DrownedEntity = net_minecraft_entity_mob_DrownedEntity
+
 
 class DrownedEntityHelper(ZombieEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/DyeColorHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SheepEntityHelper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,62 @@
 from typing import overload
 from typing import TypeVar
-from .BaseHelper import BaseHelper
+from .AnimalEntityHelper import AnimalEntityHelper
+from .DyeColorHelper import DyeColorHelper
 
-DyeColor = TypeVar["net.minecraft.util.DyeColor"]
+net_minecraft_entity_passive_SheepEntity = TypeVar("net_minecraft_entity_passive_SheepEntity")
+SheepEntity = net_minecraft_entity_passive_SheepEntity
 
-class DyeColorHelper(BaseHelper):
+
+class SheepEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: DyeColor) -> None:
-		pass
-
-	@overload
-	def getName(self) -> str:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the name of the color. 
-		"""
+	def __init__(self, base: SheepEntity) -> None:
 		pass
 
 	@overload
-	def getId(self) -> int:
+	def isSheared(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the color's identifier. 
+			'true' if this sheep is sheared, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getColorValue(self) -> int:
+	def isShearable(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the color's rgb value. 
+			'true' if this sheep can be sheared, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getFireworkColor(self) -> int:
+	def getColor(self) -> DyeColorHelper:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the color's variation when used in fireworks. 
+			the color of this sheep. 
 		"""
 		pass
 
 	@overload
-	def getSignColor(self) -> int:
-		"""
+	def isJeb(self) -> bool:
+		"""Sheep named 'jeb_' will cycle through all colors when rendered. If sheared, they will
+drop their original colored wool.\n
 		Since: 1.8.4 
 
 		Returns:
-			the color's variation when used on signs. 
+			'true' if the sheep has a rainbow overlay, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EditorScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EditorScreen.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 from typing import List
 from typing import TypeVar
 from .BaseScreen import BaseScreen
 from .History import History
 from .SelectCursor import SelectCursor
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Style = TypeVar["net.minecraft.text.Style"]
-File = TypeVar["java.io.File"]
+net_minecraft_client_gui_screen_Screen = TypeVar("net_minecraft_client_gui_screen_Screen")
+Screen = net_minecraft_client_gui_screen_Screen
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Style = TypeVar("net_minecraft_text_Style")
+Style = net_minecraft_text_Style
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class EditorScreen(BaseScreen):
 	langs: List[str]
 	defaultStyle: Style
 	history: History
 	cursor: SelectCursor
 	blockFirst: bool
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EnchantInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EnchantInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EnchantmentHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EnchantmentHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 from .ItemHelper import ItemHelper
 from .ItemStackHelper import ItemStackHelper
 
-Enchantment = TypeVar["net.minecraft.enchantment.Enchantment"]
+net_minecraft_enchantment_Enchantment = TypeVar("net_minecraft_enchantment_Enchantment")
+Enchantment = net_minecraft_enchantment_Enchantment
+
 
 class EnchantmentHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EndCrystalEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EndCrystalEntityHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 from .BlockPosHelper import BlockPosHelper
 
-EndCrystalEntity = TypeVar["net.minecraft.entity.decoration.EndCrystalEntity"]
+net_minecraft_entity_decoration_EndCrystalEntity = TypeVar("net_minecraft_entity_decoration_EndCrystalEntity")
+EndCrystalEntity = net_minecraft_entity_decoration_EndCrystalEntity
+
 
 class EndCrystalEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EnderDragonEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EnderDragonEntityHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Any
 from .MobEntityHelper import MobEntityHelper
 from .EntityHelper import EntityHelper
 
-EnderDragonEntity = TypeVar["net.minecraft.entity.boss.dragon.EnderDragonEntity"]
+net_minecraft_entity_boss_dragon_EnderDragonEntity = TypeVar("net_minecraft_entity_boss_dragon_EnderDragonEntity")
+EnderDragonEntity = net_minecraft_entity_boss_dragon_EnderDragonEntity
+
 
 class EnderDragonEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EndermanEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TameableEntityHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 from typing import overload
 from typing import TypeVar
-from .MobEntityHelper import MobEntityHelper
-from .BlockStateHelper import BlockStateHelper
+from typing import Generic
+from .AnimalEntityHelper import AnimalEntityHelper
+from .LivingEntityHelper import LivingEntityHelper
 
-EndermanEntity = TypeVar["net.minecraft.entity.mob.EndermanEntity"]
+T = TypeVar("T")
 
-class EndermanEntityHelper(MobEntityHelper):
+class TameableEntityHelper(Generic[T], AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: EndermanEntity) -> None:
+	def __init__(self, base: T) -> None:
 		pass
 
 	@overload
-	def isScreaming(self) -> bool:
+	def isTamed(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this enderman is screaming, 'false' otherwise. 
+			'true' if the entity is tamed, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isProvoked(self) -> bool:
+	def isSitting(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this enderman was provoked by a player, 'false' otherwise. 
+			'true' if the entity is sitting, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isHoldingBlock(self) -> bool:
+	def getOwner(self) -> str:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this enderman is holding a block, 'false' otherwise. 
+			the owner's uuid, or 'null' if the entity is not tamed. 
 		"""
 		pass
 
 	@overload
-	def getHeldBlock(self) -> BlockStateHelper:
+	def isOwner(self, owner: LivingEntityHelper) -> bool:
 		"""
 		Since: 1.8.4 
 
+		Args:
+			owner: the possible owner 
+
 		Returns:
-			the held block of this enderman, or 'null' if it is not holding a block. 
+			'true' if the entity is tamed by the given owner, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EntityHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from .ClientPlayerEntityHelper import ClientPlayerEntityHelper
 from .PlayerEntityHelper import PlayerEntityHelper
 from .VillagerEntityHelper import VillagerEntityHelper
 from .MerchantEntityHelper import MerchantEntityHelper
 from .LivingEntityHelper import LivingEntityHelper
 from .ItemEntityHelper import ItemEntityHelper
 
-Entity = TypeVar["net.minecraft.entity.Entity"]
+net_minecraft_entity_Entity = TypeVar("net_minecraft_entity_Entity")
+Entity = net_minecraft_entity_Entity
+
 T = TypeVar("T")
 
 class EntityHelper(Generic[T], BaseHelper):
 	"""
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventChooser.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventChooser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from typing import overload
 from typing import TypeVar
 from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.String_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Consumer_java_lang_String_ = TypeVar("java_util_function_Consumer_java_lang_String_")
+Consumer = java_util_function_Consumer_java_lang_String_
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class EventChooser(OverlayContainer):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, selected: str, parent: IOverlayParent, setEvent: Consumer) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventClickSlot.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventClickSlot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .ICancelable import ICancelable
 from .Inventory import Inventory
 
-HandledScreen = TypeVar["net.minecraft.client.gui.screen.ingame.HandledScreen__"]
+net_minecraft_client_gui_screen_ingame_HandledScreen__ = TypeVar("net_minecraft_client_gui_screen_ingame_HandledScreen__")
+HandledScreen = net_minecraft_client_gui_screen_ingame_HandledScreen__
+
 
 class EventClickSlot(BaseEvent, ICancelable):
 	"""event triggered when the user "clicks" a slot in an inventory\n
 	Since: 1.6.4 
 	"""
 	mode: int
 	button: int
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventContainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
 
 T = TypeVar("T")
-Runnable = TypeVar["java.lang.Runnable"]
-Thread = TypeVar["java.lang.Thread"]
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
+
+java_lang_Thread = TypeVar("java_lang_Thread")
+Thread = java_lang_Thread
+
 
 class EventContainer(Generic[T]):
 	"""
 	Since: 1.4.0 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventCustom.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventCustom.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDeath.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SynchronizedWeakHashSet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 from typing import overload
-from typing import List
-from .BaseEvent import BaseEvent
-from .BlockPosHelper import BlockPosHelper
-from .ItemStackHelper import ItemStackHelper
+from typing import TypeVar
+from typing import Generic
 
+java_io_Serializable = TypeVar("java_io_Serializable")
+Serializable = java_io_Serializable
 
-class EventDeath(BaseEvent):
-	"""
-	Since: 1.2.7 
-	"""
-	deathPos: BlockPosHelper
-	inventory: List[ItemStackHelper]
+E = TypeVar("E")
+E = E
+
+java_util_AbstractSet_E_ = TypeVar("java_util_AbstractSet_E_")
+AbstractSet = java_util_AbstractSet_E_
+
+
+class SynchronizedWeakHashSet(Serializable, Generic[E], AbstractSet):
 
 	@overload
 	def __init__(self) -> None:
 		pass
 
 	@overload
-	def respawn(self) -> None:
-		"""Respawns the player. Should be used with some delay, one tick should be enough.\n
-		Since: 1.8.4 
-		"""
+	def size(self) -> int:
+		pass
+
+	@overload
+	def contains(self, o: object) -> bool:
+		pass
+
+	@overload
+	def add(self, o: E) -> bool:
+		pass
+
+	@overload
+	def remove(self, o: object) -> bool:
+		pass
+
+	@overload
+	def clear(self) -> None:
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def iterator(self) -> iter:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventDropSlot.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventDropSlot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .ICancelable import ICancelable
 from .Inventory import Inventory
 
-HandledScreen = TypeVar["net.minecraft.client.gui.screen.ingame.HandledScreen__"]
+net_minecraft_client_gui_screen_ingame_HandledScreen__ = TypeVar("net_minecraft_client_gui_screen_ingame_HandledScreen__")
+HandledScreen = net_minecraft_client_gui_screen_ingame_HandledScreen__
+
 
 class EventDropSlot(BaseEvent, ICancelable):
 	"""event triggered when an item is dropped\n
 	Since: 1.6.4 
 	"""
 	slot: int
 	all: bool
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinedRecvPacket.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinedRecvPacket.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .ICancelable import ICancelable
 from .PacketByteBufferHelper import PacketByteBufferHelper
 
-Packet = TypeVar["net.minecraft.network.packet.Packet__"]
+net_minecraft_network_packet_Packet__ = TypeVar("net_minecraft_network_packet_Packet__")
+Packet = net_minecraft_network_packet_Packet__
+
 
 class EventJoinedRecvPacket(BaseEvent, ICancelable):
 	"""
 	Since: 1.8.4 
 	"""
 	cancel: bool
 	packet: Packet
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventJoinedSendPacket.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventJoinedSendPacket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .ICancelable import ICancelable
 from .PacketByteBufferHelper import PacketByteBufferHelper
 
-Packet = TypeVar["net.minecraft.network.packet.Packet__"]
+net_minecraft_network_packet_Packet__ = TypeVar("net_minecraft_network_packet_Packet__")
+Packet = net_minecraft_network_packet_Packet__
+
 
 class EventJoinedSendPacket(BaseEvent, ICancelable):
 	"""
 	Since: 1.8.4 
 	"""
 	cancel: bool
 	packet: Packet
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventKey.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventKey.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventOpenContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventOpenContainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .ICancelable import ICancelable
 from .Inventory import Inventory
 from .IScreen import IScreen
 
-HandledScreen = TypeVar["net.minecraft.client.gui.screen.ingame.HandledScreen__"]
+net_minecraft_client_gui_screen_ingame_HandledScreen__ = TypeVar("net_minecraft_client_gui_screen_ingame_HandledScreen__")
+HandledScreen = net_minecraft_client_gui_screen_ingame_HandledScreen__
+
 
 class EventOpenContainer(BaseEvent, ICancelable):
 	"""
 	Since: 1.6.5 
 	"""
 	inventory: Inventory
 	screen: IScreen
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventRecvPacket.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventRecvPacket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .BaseEvent import BaseEvent
 from .PacketByteBufferHelper import PacketByteBufferHelper
 
-Packet = TypeVar["net.minecraft.network.packet.Packet__"]
+net_minecraft_network_packet_Packet__ = TypeVar("net_minecraft_network_packet_Packet__")
+Packet = net_minecraft_network_packet_Packet__
+
 
 class EventRecvPacket(BaseEvent):
 	"""
 	Since: 1.8.4 
 	"""
 	packet: Packet
 	type: str
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventRegistry.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventRegistry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventResourcePackLoaded.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventResourcePackLoaded.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventService.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventService.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/EventWrappedScript.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EventWrappedScript.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Extension.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 from typing import Mapping
 from typing import Set
 from .Extension_ExtMatch import Extension_ExtMatch
 from .Core import Core
 from .BaseLanguage import BaseLanguage
 from .BaseWrappedException import BaseWrappedException
 
-Throwable = TypeVar["java.lang.Throwable"]
-File = TypeVar["java.io.File"]
+java_lang_Throwable = TypeVar("java_lang_Throwable")
+Throwable = java_lang_Throwable
+
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class Extension:
 
 	@overload
 	def init(self) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ExtensionLoader.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ExtensionLoader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Set
 from .Core import Core
 from .Extension import Extension
 
-File = TypeVar["java.io.File"]
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class ExtensionLoader:
 
 	@overload
 	def __init__(self, core: Core) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FChat.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FChat.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from .TextHelper import TextHelper
 from .TextBuilder import TextBuilder
 from .CommandBuilder import CommandBuilder
 from .CommandNodeHelper import CommandNodeHelper
 from .CommandManager import CommandManager
 from .ChatHistoryManager import ChatHistoryManager
 
-Logger = TypeVar["org.slf4j.Logger"]
+org_slf4j_Logger = TypeVar("org_slf4j_Logger")
+Logger = org_slf4j_Logger
+
 
 class FChat(BaseLibrary):
 	"""Functions for interacting with chat. 
 An instance of this class is passed to scripts as the 'Chat' variable.
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FClient.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 from .MethodWrapper import MethodWrapper
 from .OptionsHelper import OptionsHelper
 from .ServerInfoHelper import ServerInfoHelper
 from .ModContainerHelper import ModContainerHelper
 from .BlockHelper import BlockHelper
 from .ItemHelper import ItemHelper
 
-Packet = TypeVar["net.minecraft.network.packet.Packet_net.minecraft.network.listener.ClientPlayPacketListener_"]
-MinecraftClient = TypeVar["net.minecraft.client.MinecraftClient"]
+net_minecraft_network_packet_Packet_net_minecraft_network_listener_ClientPlayPacketListener_ = TypeVar("net_minecraft_network_packet_Packet_net_minecraft_network_listener_ClientPlayPacketListener_")
+Packet = net_minecraft_network_packet_Packet_net_minecraft_network_listener_ClientPlayPacketListener_
+
+net_minecraft_client_MinecraftClient = TypeVar("net_minecraft_client_MinecraftClient")
+MinecraftClient = net_minecraft_client_MinecraftClient
+
 
 class FClient(PerExecLibrary):
 	"""Functions that interact with minecraft that don't fit into their own module. 
 An instance of this class is passed to scripts as the 'Client' variable.\n
 	Since: 1.2.9 
 	"""
 	tickSynchronizer: TickSync
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FFS.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List
 from typing import TypeVar
 from .PerExecLibrary import PerExecLibrary
 from .BaseScriptContext import BaseScriptContext
 from .FileHandler import FileHandler
 from .MethodWrapper import MethodWrapper
 
-File = TypeVar["java.io.File"]
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class FFS(PerExecLibrary):
 	"""Better File-System functions. 
 An instance of this class is passed to scripts as the 'FS' variable.\n
 	Since: 1.1.8 
 	"""
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FGlobalVars.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FGlobalVars.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FHud.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FHud.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FJavaUtils.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FJavaUtils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseLibrary import BaseLibrary
 from .BaseHelper import BaseHelper
 
 T = TypeVar("T")
-HashMap = TypeVar["java.util.HashMap_,_"]
-ArrayList = TypeVar["java.util.ArrayList_T_"]
-SplittableRandom = TypeVar["java.util.SplittableRandom"]
-HashSet = TypeVar["java.util.HashSet__"]
+java_util_HashMap_,_ = TypeVar("java_util_HashMap_,_")
+HashMap = java_util_HashMap_,_
+
+java_util_ArrayList_T_ = TypeVar("java_util_ArrayList_T_")
+ArrayList = java_util_ArrayList_T_
+
+java_util_SplittableRandom = TypeVar("java_util_SplittableRandom")
+SplittableRandom = java_util_SplittableRandom
+
+java_util_HashSet__ = TypeVar("java_util_HashSet__")
+HashSet = java_util_HashSet__
+
 
 class FJavaUtils(BaseLibrary):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FJsMacros.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FJsMacros.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FKeyBind.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FKeyBind.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Mapping
 from typing import Set
 from .BaseLibrary import BaseLibrary
 
-InputUtil_Key = TypeVar["net.minecraft.client.util.InputUtil.Key"]
+net_minecraft_client_util_InputUtil_Key = TypeVar("net_minecraft_client_util_InputUtil_Key")
+InputUtil_Key = net_minecraft_client_util_InputUtil_Key
+
 
 class FKeyBind(BaseLibrary):
 	"""Functions for getting and modifying key pressed states. 
 An instance of this class is passed to scripts as the 'KeyBind' variable.
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FPlayer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FPlayer.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FPositionCommon.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FPositionCommon.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FReflection.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FReflection.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 from .BaseScriptContext import BaseScriptContext
 from .ProxyBuilder import ProxyBuilder
 from .ClassBuilder import ClassBuilder
 from .LibraryBuilder import LibraryBuilder
 from .Mappings import Mappings
 from .WrappedClassInstance import WrappedClassInstance
 
-Field = TypeVar["java.lang.reflect.Field"]
+java_lang_reflect_Field = TypeVar("java_lang_reflect_Field")
+Field = java_lang_reflect_Field
+
 T = TypeVar("T")
-Reflect = TypeVar["org.joor.Reflect"]
-Method = TypeVar["java.lang.reflect.Method"]
+org_joor_Reflect = TypeVar("org_joor_Reflect")
+Reflect = org_joor_Reflect
+
+java_lang_reflect_Method = TypeVar("java_lang_reflect_Method")
+Method = java_lang_reflect_Method
+
 
 class FReflection(PerExecLibrary):
 	"""Functions for getting and using raw java classes, methods and functions. 
 An instance of this class is passed to scripts as the 'Reflection' variable.\n
 	Since: 1.2.3 
 	"""
 	classLoader: FReflection_CombinedVariableClassLoader
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FReflection_CombinedVariableClassLoader.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FReflection_CombinedVariableClassLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import overload
 from typing import TypeVar
 
-File = TypeVar["java.io.File"]
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class FReflection_CombinedVariableClassLoader(ClassLoader):
 	"""I know this is probably bad practice, but lets be real, this whole library is bad practice, So I can make it
 worse, right? at least this should work better than 'try/catch' 'ing using ClassLoader#loadClass(java.lang.String) to search through every URLClassLoader that FReflection#loadJarFile(java.lang.String) would make, or how I was previously doing it by pre-loading and caching
 all the classes to a Map  
 This class is a modification to Christian d'Heureuse's JoinClassLoader , under the Apache-2.0 license to change it from a Class array to a Set , to allow for modifications to the ClassLoader contained in the classLoader.\n
 	Since: 1.2.8
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FRequest.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FRequest.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FTime.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FTime.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FUtils.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FUtils.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FWorld.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FWorld.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FakeServerCommandSource.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FakeServerCommandSource.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Set
 
-CompletableFuture = TypeVar["java.util.concurrent.CompletableFuture_com.mojang.brigadier.suggestion.Suggestions_"]
-CommandContext = TypeVar["com.mojang.brigadier.context.CommandContext__"]
-ClientCommandSource = TypeVar["net.minecraft.client.network.ClientCommandSource"]
-CommandSource_RelativePosition = TypeVar["net.minecraft.command.CommandSource.RelativePosition"]
-DynamicRegistryManager = TypeVar["net.minecraft.registry.DynamicRegistryManager"]
-Stream = TypeVar["java.util.stream.Stream_net.minecraft.util.Identifier_"]
-Supplier = TypeVar["java.util.function.Supplier_net.minecraft.text.Text_"]
-ClientPlayerEntity = TypeVar["net.minecraft.client.network.ClientPlayerEntity"]
-RegistryKey = TypeVar["net.minecraft.registry.RegistryKey_net.minecraft.world.World_"]
-ServerCommandSource = TypeVar["net.minecraft.server.command.ServerCommandSource"]
+java_util_concurrent_CompletableFuture_com_mojang_brigadier_suggestion_Suggestions_ = TypeVar("java_util_concurrent_CompletableFuture_com_mojang_brigadier_suggestion_Suggestions_")
+CompletableFuture = java_util_concurrent_CompletableFuture_com_mojang_brigadier_suggestion_Suggestions_
+
+com_mojang_brigadier_context_CommandContext__ = TypeVar("com_mojang_brigadier_context_CommandContext__")
+CommandContext = com_mojang_brigadier_context_CommandContext__
+
+net_minecraft_client_network_ClientCommandSource = TypeVar("net_minecraft_client_network_ClientCommandSource")
+ClientCommandSource = net_minecraft_client_network_ClientCommandSource
+
+net_minecraft_command_CommandSource_RelativePosition = TypeVar("net_minecraft_command_CommandSource_RelativePosition")
+CommandSource_RelativePosition = net_minecraft_command_CommandSource_RelativePosition
+
+net_minecraft_registry_DynamicRegistryManager = TypeVar("net_minecraft_registry_DynamicRegistryManager")
+DynamicRegistryManager = net_minecraft_registry_DynamicRegistryManager
+
+java_util_stream_Stream_net_minecraft_util_Identifier_ = TypeVar("java_util_stream_Stream_net_minecraft_util_Identifier_")
+Stream = java_util_stream_Stream_net_minecraft_util_Identifier_
+
+java_util_function_Supplier_net_minecraft_text_Text_ = TypeVar("java_util_function_Supplier_net_minecraft_text_Text_")
+Supplier = java_util_function_Supplier_net_minecraft_text_Text_
+
+net_minecraft_client_network_ClientPlayerEntity = TypeVar("net_minecraft_client_network_ClientPlayerEntity")
+ClientPlayerEntity = net_minecraft_client_network_ClientPlayerEntity
+
+net_minecraft_registry_RegistryKey_net_minecraft_world_World_ = TypeVar("net_minecraft_registry_RegistryKey_net_minecraft_world_World_")
+RegistryKey = net_minecraft_registry_RegistryKey_net_minecraft_world_World_
+
+net_minecraft_server_command_ServerCommandSource = TypeVar("net_minecraft_server_command_ServerCommandSource")
+ServerCommandSource = net_minecraft_server_command_ServerCommandSource
+
 
 class FakeServerCommandSource(ServerCommandSource):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FallingBlockEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FallingBlockEntityHelper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 from .BlockPosHelper import BlockPosHelper
 from .BlockStateHelper import BlockStateHelper
 
-FallingBlockEntity = TypeVar["net.minecraft.entity.FallingBlockEntity"]
+net_minecraft_entity_FallingBlockEntity = TypeVar("net_minecraft_entity_FallingBlockEntity")
+FallingBlockEntity = net_minecraft_entity_FallingBlockEntity
+
 
 class FallingBlockEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileChooser.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SettingsOverlay.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,47 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
+from .ICategoryTreeParent import ICategoryTreeParent
 from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
-from .FileChooser_fileObj import FileChooser_fileObj
 
-Consumer = TypeVar["java.util.function.Consumer_java.io.File_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-File = TypeVar["java.io.File"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class FileChooser(OverlayContainer):
-	root: File
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, directory: File, selected: File, parent: IOverlayParent, setFile: Consumer, editFile: Consumer) -> None:
-		pass
 
-	@overload
-	def setDir(self, dir: File) -> None:
-		pass
+class SettingsOverlay(ICategoryTreeParent, OverlayContainer):
 
 	@overload
-	def selectFile(self, f: File) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
-	def addFile(self, f: File) -> None:
-		pass
-
-	@overload
-	def addFile(self, f: File, btnText: str) -> None:
-		pass
-
-	@overload
-	def updateFilePos(self) -> None:
+	def clearCategory(self) -> None:
 		pass
 
 	@overload
-	def confirmDelete(self, f: FileChooser_fileObj) -> None:
+	def selectCategory(self, category: List[str]) -> None:
 		pass
 
 	@overload
-	def delete(self, f: FileChooser_fileObj) -> None:
+	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	@overload
-	def onScrollbar(self, page: float) -> None:
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
-	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
+	def onClose(self) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/DoubleField.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-File = TypeVar["java.io.File"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class FileField(AbstractSettingField):
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
-		pass
 
-	@overload
-	def getTopLevel(self, setting: SettingsOverlay_SettingField) -> File:
-		pass
+class DoubleField(AbstractSettingField):
 
 	@overload
-	def relativize(self, setting: SettingsOverlay_SettingField, file: File) -> str:
+	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileHandler.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerListEntryHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,130 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from .FileHandler_FileLineIterator import FileHandler_FileLineIterator
+from .BaseHelper import BaseHelper
+from .TextHelper import TextHelper
+from .TeamHelper import TeamHelper
 
-BufferedInputStream = TypeVar["java.io.BufferedInputStream"]
-File = TypeVar["java.io.File"]
+net_minecraft_client_network_PlayerListEntry = TypeVar("net_minecraft_client_network_PlayerListEntry")
+PlayerListEntry = net_minecraft_client_network_PlayerListEntry
 
-class FileHandler:
+
+class PlayerListEntryHelper(BaseHelper):
 	"""
-	Since: 1.1.8 
+	Since: 1.0.2 
 	"""
 
 	@overload
-	def __init__(self, path: str) -> None:
-		pass
-
-	@overload
-	def __init__(self, path: str, charset: str) -> None:
-		pass
-
-	@overload
-	def __init__(self, path: File, charset: str) -> None:
+	def __init__(self, p: PlayerListEntry) -> None:
 		pass
 
 	@overload
-	def __init__(self, path: str, charset: Charset) -> None:
+	def getUUID(self) -> str:
+		"""
+		Since: 1.1.9 
+		"""
 		pass
 
 	@overload
-	def __init__(self, path: File) -> None:
+	def getName(self) -> str:
+		"""
+		Since: 1.0.2 
+		"""
 		pass
 
 	@overload
-	def __init__(self, path: File, charset: Charset) -> None:
+	def getPing(self) -> int:
+		"""
+		Since: 1.6.5 
+		"""
 		pass
 
 	@overload
-	def write(self, s: str) -> "FileHandler":
-		"""writes a string to the file. this is a destructive operation that replaces the file contents.\n
-		Since: 1.1.8 
+	def getGamemode(self) -> str:
+		"""
+		Since: 1.6.5 
 
-		Args:
-			s: 
+		Returns:
+			null if unknown 
 		"""
 		pass
 
 	@overload
-	def write(self, b: List[float]) -> "FileHandler":
-		"""writes a byte array to the file. this is a destructive operation that replaces the file contents.\n
-		Since: 1.1.8 
-
-		Args:
-			b: 
+	def getDisplayText(self) -> TextHelper:
+		"""
+		Since: 1.1.9 
 		"""
 		pass
 
 	@overload
-	def read(self) -> str:
+	def getPublicKey(self) -> List[float]:
 		"""
-		Since: 1.1.8 
+		Since: 1.8.2 
 		"""
 		pass
 
 	@overload
-	def readBytes(self) -> List[float]:
+	def hasCape(self) -> bool:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the player has a cape enabled, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def readLines(self) -> FileHandler_FileLineIterator:
-		"""get an iterator for the lines in the file.
-please call FileHandler_FileLineIterator#close() when you are done with the iterator to not leak resources.\n
+	def hasSlimModel(self) -> bool:
+		"""A slim skin is an Alex skin, while the default one is Steve.\n
 		Since: 1.8.4 
+
+		Returns:
+			'true' if the player has a slim skin, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def streamBytes(self) -> BufferedInputStream:
-		"""get an input stream for the file.
-please call BufferedInputStream#close() when you are done with the stream to not leak resources.\n
+	def getSkinTexture(self) -> str:
+		"""
 		Since: 1.8.4 
+
+		Returns:
+			the identifier of the player's skin texture or 'null' if it's unknown. 
 		"""
 		pass
 
 	@overload
-	def append(self, s: str) -> "FileHandler":
+	def getCapeTexture(self) -> str:
 		"""
-		Since: 1.1.8 
+		Since: 1.8.4 
 
-		Args:
-			s: 
+		Returns:
+			the identifier of the player's cape texture or 'null' if it's unknown. 
 		"""
 		pass
 
 	@overload
-	def append(self, b: List[float]) -> "FileHandler":
+	def getElytraTexture(self) -> str:
 		"""
-		Since: 1.2.6 
+		Since: 1.8.4 
 
-		Args:
-			b: 
+		Returns:
+			the identifier of the player's elytra texture or 'null' if it's unknown. 
 		"""
 		pass
 
 	@overload
-	def getFile(self) -> File:
+	def getTeam(self) -> TeamHelper:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the team of the player or 'null' if the player is not in a team. 
+		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileMapSetting.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringMapSetting_StringEntry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .AbstractMapSettingContainer import AbstractMapSettingContainer
-from .SettingsOverlay import SettingsOverlay
+from .AbstractMapSettingContainer_MapSettingEntry import AbstractMapSettingContainer_MapSettingEntry
+from .StringMapSetting import StringMapSetting
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-class FileMapSetting(AbstractMapSettingContainer):
+
+class StringMapSetting_StringEntry(AbstractMapSettingContainer_MapSettingEntry):
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
+	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: StringMapSetting, key: str, value: str) -> None:
 		pass
 
 	@overload
-	def addField(self, key: str, value: str) -> None:
+	def init(self) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FileMapSetting_FileEntry.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileMapSetting_FileEntry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractMapSettingContainer_MapSettingEntry import AbstractMapSettingContainer_MapSettingEntry
 from .FileMapSetting import FileMapSetting
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class FileMapSetting_FileEntry(AbstractMapSettingContainer_MapSettingEntry):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: FileMapSetting, key: str, value: str) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FishingBobberEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FishingBobberEntityHelper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 
-FishingBobberEntity = TypeVar["net.minecraft.entity.projectile.FishingBobberEntity"]
+net_minecraft_entity_projectile_FishingBobberEntity = TypeVar("net_minecraft_entity_projectile_FishingBobberEntity")
+FishingBobberEntity = net_minecraft_entity_projectile_FishingBobberEntity
+
 
 class FishingBobberEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FloatField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FloatField.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class FloatField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FluidStateHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FluidStateHelper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import TypeVar
 from .StateHelper import StateHelper
 from .BlockPosHelper import BlockPosHelper
 from .Pos3D import Pos3D
 from .BlockStateHelper import BlockStateHelper
 
-FluidState = TypeVar["net.minecraft.fluid.FluidState"]
+net_minecraft_fluid_FluidState = TypeVar("net_minecraft_fluid_FluidState")
+FluidState = net_minecraft_fluid_FluidState
+
 
 class FluidStateHelper(StateHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FoodComponentHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FoodComponentHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Mapping
 from .BaseHelper import BaseHelper
 from .StatusEffectHelper import StatusEffectHelper
 
-FoodComponent = TypeVar["net.minecraft.item.FoodComponent"]
+net_minecraft_item_FoodComponent = TypeVar("net_minecraft_item_FoodComponent")
+FoodComponent = net_minecraft_item_FoodComponent
+
 
 class FoodComponentHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FormattingHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FormattingHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 
-Formatting = TypeVar["net.minecraft.util.Formatting"]
+net_minecraft_util_Formatting = TypeVar("net_minecraft_util_Formatting")
+Formatting = net_minecraft_util_Formatting
+
 
 class FormattingHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FoxEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FoxEntityHelper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 from .ItemStackHelper import ItemStackHelper
 from .EntityHelper import EntityHelper
 
-FoxEntity = TypeVar["net.minecraft.entity.passive.FoxEntity"]
+net_minecraft_entity_passive_FoxEntity = TypeVar("net_minecraft_entity_passive_FoxEntity")
+FoxEntity = net_minecraft_entity_passive_FoxEntity
+
 
 class FoxEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FrogEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemFrameEntityHelper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from typing import overload
 from typing import TypeVar
-from .AnimalEntityHelper import AnimalEntityHelper
 from .EntityHelper import EntityHelper
+from .ItemStackHelper import ItemStackHelper
 
-FrogEntity = TypeVar["net.minecraft.entity.passive.FrogEntity"]
+net_minecraft_entity_decoration_ItemFrameEntity = TypeVar("net_minecraft_entity_decoration_ItemFrameEntity")
+ItemFrameEntity = net_minecraft_entity_decoration_ItemFrameEntity
 
-class FrogEntityHelper(AnimalEntityHelper):
+
+class ItemFrameEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: FrogEntity) -> None:
+	def __init__(self, base: ItemFrameEntity) -> None:
 		pass
 
 	@overload
-	def getVariant(self) -> str:
+	def isGlowingFrame(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the variant of this frog. 
+			'true' if the item frame is glowing, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getTarget(self) -> EntityHelper:
+	def getRotation(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the target of this frog, or 'null' if it has none. 
+			the rotation of the item inside this frame. 
 		"""
 		pass
 
 	@overload
-	def isCroaking(self) -> bool:
+	def getItem(self) -> ItemStackHelper:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this frog is croaking, 'false' otherwise. 
+			the item inside this item frame. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/FurnaceInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FurnaceInventory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from typing import Mapping
 from .RecipeInventory import RecipeInventory
 from .ItemStackHelper import ItemStackHelper
 
-AbstractFurnaceScreen = TypeVar["net.minecraft.client.gui.screen.ingame.AbstractFurnaceScreen__"]
+net_minecraft_client_gui_screen_ingame_AbstractFurnaceScreen__ = TypeVar("net_minecraft_client_gui_screen_ingame_AbstractFurnaceScreen__")
+AbstractFurnaceScreen = net_minecraft_client_gui_screen_ingame_AbstractFurnaceScreen__
+
 
 class FurnaceInventory(RecipeInventory):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/GoatEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/GoatEntityHelper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-GoatEntity = TypeVar["net.minecraft.entity.passive.GoatEntity"]
+net_minecraft_entity_passive_GoatEntity = TypeVar("net_minecraft_entity_passive_GoatEntity")
+GoatEntity = net_minecraft_entity_passive_GoatEntity
+
 
 class GoatEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/GrindStoneInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/GrindStoneInventory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .Inventory import Inventory
 from .ItemStackHelper import ItemStackHelper
 
-GrindstoneScreen = TypeVar["net.minecraft.client.gui.screen.ingame.GrindstoneScreen"]
+net_minecraft_client_gui_screen_ingame_GrindstoneScreen = TypeVar("net_minecraft_client_gui_screen_ingame_GrindstoneScreen")
+GrindstoneScreen = net_minecraft_client_gui_screen_ingame_GrindstoneScreen
+
 
 class GrindStoneInventory(Inventory):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/GroupFilter.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/GroupFilter.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/GuardianEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WolfEntityHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 from typing import overload
 from typing import TypeVar
-from .MobEntityHelper import MobEntityHelper
-from .EntityHelper import EntityHelper
+from .TameableEntityHelper import TameableEntityHelper
+from .DyeColorHelper import DyeColorHelper
 
-GuardianEntity = TypeVar["net.minecraft.entity.mob.GuardianEntity"]
+net_minecraft_entity_passive_WolfEntity = TypeVar("net_minecraft_entity_passive_WolfEntity")
+WolfEntity = net_minecraft_entity_passive_WolfEntity
 
-class GuardianEntityHelper(MobEntityHelper):
+
+class WolfEntityHelper(TameableEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: GuardianEntity) -> None:
+	def __init__(self, base: WolfEntity) -> None:
 		pass
 
 	@overload
-	def isElder(self) -> bool:
+	def isBegging(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this guardian is an elder guardian, 'false' otherwise. 
+			'true' if this wolf is tamed and the player has either a bone or meat in one of
+their hands, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def hasTarget(self) -> bool:
+	def getCollarColor(self) -> DyeColorHelper:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this guardian is targeting a mob, 'false' otherwise. 
+			the color of this wolf's collar. 
 		"""
 		pass
 
 	@overload
-	def getTarget(self) -> EntityHelper:
+	def isAngry(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the target of this guardian's beam, or 'null' if it has no target. 
+			'true' if this wolf is angry, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def hasSpikesRetracted(self) -> bool:
+	def isWet(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this guardian has its spikes extended, 'false' otherwise. 
+			'true' if this wolf is wet, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/HTTPRequest.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/HTTPRequest_Response.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/HTTPRequest_Response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 
-InputStream = TypeVar["java.io.InputStream"]
+java_io_InputStream = TypeVar("java_io_InputStream")
+InputStream = java_io_InputStream
+
 
 class HTTPRequest_Response:
 	"""
 	Since: 1.1.8 
 	"""
 	headers: Mapping[str, List[str]]
 	responseCode: int
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/History.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/History.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .SelectCursor import SelectCursor
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.String_"]
+java_util_function_Consumer_java_lang_String_ = TypeVar("java_util_function_Consumer_java_lang_String_")
+Consumer = java_util_function_Consumer_java_lang_String_
+
 
 class History:
 	"""
 	"""
 	onChange: Consumer
 	current: str
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/HorseInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/HorseInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IContainerParent.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IContainerParent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
 
 T = TypeVar("T")
-Element = TypeVar["net.minecraft.client.gui.Element"]
+net_minecraft_client_gui_Element = TypeVar("net_minecraft_client_gui_Element")
+Element = net_minecraft_client_gui_Element
+
 
 class IContainerParent:
 
 	@overload
 	def addDrawableChild(self, drawableElement: T) -> T:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IDraw2D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IDraw2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 from .Rect_Builder import Rect_Builder
 from .Line_Builder import Line_Builder
 from .Text_Builder import Text_Builder
 from .Draw2DElement_Builder import Draw2DElement_Builder
 from .MethodWrapper import MethodWrapper
 
 T = TypeVar("T")
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class IDraw2D:
 	"""
 	Since: 1.2.7 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IFWrapper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IFWrapper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IRecipeBookWidget.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IRecipeBookWidget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import overload
 from typing import TypeVar
 
-ClientRecipeBook = TypeVar["net.minecraft.client.recipebook.ClientRecipeBook"]
-RecipeBookResults = TypeVar["net.minecraft.client.gui.screen.recipebook.RecipeBookResults"]
+net_minecraft_client_recipebook_ClientRecipeBook = TypeVar("net_minecraft_client_recipebook_ClientRecipeBook")
+ClientRecipeBook = net_minecraft_client_recipebook_ClientRecipeBook
+
+net_minecraft_client_gui_screen_recipebook_RecipeBookResults = TypeVar("net_minecraft_client_gui_screen_recipebook_RecipeBookResults")
+RecipeBookResults = net_minecraft_client_gui_screen_recipebook_RecipeBookResults
+
 
 class IRecipeBookWidget:
 
 	@overload
 	def jsmacros_getResults(self) -> RecipeBookResults:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IScreen.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IScreenInternal.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IScreenInternal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import overload
 from typing import TypeVar
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class IScreenInternal:
 
 	@overload
 	def jsmacros_render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Image.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .IDraw2D import IDraw2D
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class Image(RenderElement, Alignable):
 	"""
 	Since: 1.2.3 
 	"""
 	parent: IDraw2D
 	rotation: float
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Image_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Image_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/IntField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringField.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class IntField(AbstractSettingField):
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
+
+class StringField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Inventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from typing import TypeVar
 from typing import Mapping
 from typing import Generic
 from .ItemStackHelper import ItemStackHelper
 from .Pos2D import Pos2D
 
 T = TypeVar("T")
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
+net_minecraft_client_gui_screen_Screen = TypeVar("net_minecraft_client_gui_screen_Screen")
+Screen = net_minecraft_client_gui_screen_Screen
+
 
 class Inventory(Generic[T]):
 	"""
 	Since: 1.0.8 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Item.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .IDraw2D import IDraw2D
 from .ItemStackHelper import ItemStackHelper
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-ItemStack = TypeVar["net.minecraft.item.ItemStack"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_item_ItemStack = TypeVar("net_minecraft_item_ItemStack")
+ItemStack = net_minecraft_item_ItemStack
+
 
 class Item(RenderElement, Alignable):
 	"""
 	Since: 1.0.5 
 	"""
 	parent: IDraw2D
 	item: ItemStack
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemFrameEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/EndermanEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 from typing import overload
 from typing import TypeVar
-from .EntityHelper import EntityHelper
-from .ItemStackHelper import ItemStackHelper
+from .MobEntityHelper import MobEntityHelper
+from .BlockStateHelper import BlockStateHelper
 
-ItemFrameEntity = TypeVar["net.minecraft.entity.decoration.ItemFrameEntity"]
+net_minecraft_entity_mob_EndermanEntity = TypeVar("net_minecraft_entity_mob_EndermanEntity")
+EndermanEntity = net_minecraft_entity_mob_EndermanEntity
 
-class ItemFrameEntityHelper(EntityHelper):
+
+class EndermanEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: ItemFrameEntity) -> None:
+	def __init__(self, base: EndermanEntity) -> None:
+		pass
+
+	@overload
+	def isScreaming(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this enderman is screaming, 'false' otherwise. 
+		"""
 		pass
 
 	@overload
-	def isGlowingFrame(self) -> bool:
+	def isProvoked(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the item frame is glowing, 'false' otherwise. 
+			'true' if this enderman was provoked by a player, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getRotation(self) -> int:
+	def isHoldingBlock(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the rotation of the item inside this frame. 
+			'true' if this enderman is holding a block, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getItem(self) -> ItemStackHelper:
+	def getHeldBlock(self) -> BlockStateHelper:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the item inside this item frame. 
+			the held block of this enderman, or 'null' if it is not holding a block. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 from .ItemStackHelper import ItemStackHelper
 from .BlockHelper import BlockHelper
 from .BlockStateHelper import BlockStateHelper
 from .FoodComponentHelper import FoodComponentHelper
 
-Item = TypeVar["net.minecraft.item.Item"]
+net_minecraft_item_Item = TypeVar("net_minecraft_item_Item")
+Item = net_minecraft_item_Item
+
 
 class ItemHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ItemStackHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ItemStackHelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from .TextHelper import TextHelper
 from .NBTElementHelper import NBTElementHelper
 from .BlockHelper import BlockHelper
 from .BlockStateHelper import BlockStateHelper
 from .CreativeItemStackHelper import CreativeItemStackHelper
 from .ItemHelper import ItemHelper
 
-ItemStack = TypeVar["net.minecraft.item.ItemStack"]
+net_minecraft_item_ItemStack = TypeVar("net_minecraft_item_ItemStack")
+ItemStack = net_minecraft_item_ItemStack
+
 
 class ItemStackHelper(BaseHelper):
 	"""
 	"""
 
 	@overload
 	def __init__(self, id: str, count: int) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Item_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Item_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/JsMacros.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MacroListTopbar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,35 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .BaseScreen import BaseScreen
-from .Core import Core
-from .ModLoader import ModLoader
-
-KeyBinding = TypeVar["net.minecraft.client.option.KeyBinding"]
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
-MinecraftClient = TypeVar["net.minecraft.client.MinecraftClient"]
-InputUtil_Key = TypeVar["net.minecraft.client.util.InputUtil.Key"]
-Text = TypeVar["net.minecraft.text.Text"]
-Logger = TypeVar["org.slf4j.Logger"]
-
-class JsMacros:
-	MOD_ID: str
-	LOGGER: Logger
-	keyBinding: KeyBinding
-	prevScreen: BaseScreen
-	core: Core
+from .MultiElementContainer import MultiElementContainer
+from .ScriptTrigger_TriggerType import ScriptTrigger_TriggerType
+from .MacroScreen import MacroScreen
 
-	@overload
-	def __init__(self) -> None:
-		pass
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-	@overload
-	def onInitialize(self) -> None:
-		pass
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def onInitializeClient(self) -> None:
-		pass
-
-	@overload
-	def getKeyText(self, translationKey: str) -> Text:
-		pass
 
-	@overload
-	def getScreenName(self, s: Screen) -> str:
-		pass
-
-	@overload
-	def getLocalizedName(self, keyCode: InputUtil_Key) -> str:
-		pass
-
-	@overload
-	def getMinecraft(self) -> MinecraftClient:
-		pass
+class MacroListTopbar(MultiElementContainer):
+	deftype: ScriptTrigger_TriggerType
 
 	@overload
-	def range(self, end: int) -> List[int]:
+	def __init__(self, parent: MacroScreen, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, deftype: ScriptTrigger_TriggerType) -> None:
 		pass
 
 	@overload
-	def range(self, start: int, end: int) -> List[int]:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def range(self, start: int, end: int, iter: int) -> List[int]:
+	def updateType(self, type: ScriptTrigger_TriggerType) -> None:
 		pass
 
 	@overload
-	def getModLoader(self) -> ModLoader:
+	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LibraryBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LibraryBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LibraryRegistry.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LibraryRegistry.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .IDraw2D import IDraw2D
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class Line(RenderElement, Alignable):
 	"""
 	Since: 1.8.4 
 	"""
 	parent: IDraw2D
 	x1: int
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line3D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line3D.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement3D import RenderElement3D
 from .Vec3D import Vec3D
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-BufferBuilder = TypeVar["net.minecraft.client.render.BufferBuilder"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_render_BufferBuilder = TypeVar("net_minecraft_client_render_BufferBuilder")
+BufferBuilder = net_minecraft_client_render_BufferBuilder
+
 
 class Line3D(RenderElement3D):
 	"""
 	"""
 	pos: Vec3D
 	color: int
 	cull: bool
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line3D_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line3D_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Line_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Line_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ListContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ListContainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .MultiElementContainer import MultiElementContainer
 from .IOverlayParent import IOverlayParent
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Integer_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Consumer_java_lang_Integer_ = TypeVar("java_util_function_Consumer_java_lang_Integer_")
+Consumer = java_util_function_Consumer_java_lang_Integer_
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class ListContainer(MultiElementContainer):
 	onSelect: Consumer
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, list: List[Text], parent: IOverlayParent, onSelect: Consumer) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LivingEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LivingEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LlamaEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LlamaEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LockButtonWidgetHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/GuardianEntityHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 from typing import overload
 from typing import TypeVar
-from .ClickableWidgetHelper import ClickableWidgetHelper
+from .MobEntityHelper import MobEntityHelper
+from .EntityHelper import EntityHelper
 
-LockButtonWidget = TypeVar["net.minecraft.client.gui.widget.LockButtonWidget"]
+net_minecraft_entity_mob_GuardianEntity = TypeVar("net_minecraft_entity_mob_GuardianEntity")
+GuardianEntity = net_minecraft_entity_mob_GuardianEntity
 
-class LockButtonWidgetHelper(ClickableWidgetHelper):
+
+class GuardianEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, btn: LockButtonWidget) -> None:
+	def __init__(self, base: GuardianEntity) -> None:
 		pass
 
 	@overload
-	def __init__(self, btn: LockButtonWidget, zIndex: int) -> None:
+	def isElder(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this guardian is an elder guardian, 'false' otherwise. 
+		"""
 		pass
 
 	@overload
-	def isLocked(self) -> bool:
+	def hasTarget(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the button is locked, 'false' otherwise. 
+			'true' if this guardian is targeting a mob, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def setLocked(self, locked: bool) -> "LockButtonWidgetHelper":
+	def getTarget(self) -> EntityHelper:
 		"""
 		Since: 1.8.4 
 
-		Args:
-			locked: whether to lock the button or not 
-
 		Returns:
-			self for chaining. 
+			the target of this guardian's beam, or 'null' if it has no target. 
 		"""
 		pass
 
 	@overload
-	def toString(self) -> str:
+	def hasSpikesRetracted(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if this guardian has its spikes extended, 'false' otherwise. 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LockButtonWidgetHelper_LockButtonBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LockButtonWidgetHelper_LockButtonBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LongField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BooleanField.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class LongField(AbstractSettingField):
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
+
+class BooleanField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/LoomInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LoomInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MacroContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MacroScreen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,74 @@
 from typing import overload
 from typing import TypeVar
-from .MultiElementContainer import MultiElementContainer
+from .BaseScreen import BaseScreen
 from .ScriptTrigger import ScriptTrigger
-from .MacroScreen import MacroScreen
+from .MultiElementContainer import MultiElementContainer
+from .MacroContainer import MacroContainer
+
+net_minecraft_client_gui_screen_Screen = TypeVar("net_minecraft_client_gui_screen_Screen")
+Screen = net_minecraft_client_gui_screen_Screen
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
-File = TypeVar["java.io.File"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
 
-class MacroContainer(MultiElementContainer):
+
+class MacroScreen(BaseScreen):
+
+	@overload
+	def __init__(self, parent: Screen) -> None:
+		pass
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, macro: ScriptTrigger, parent: MacroScreen) -> None:
+	def mouseScrolled(self, mouseX: float, mouseY: float, amount: float) -> bool:
 		pass
 
 	@overload
-	def getRawMacro(self) -> ScriptTrigger:
+	def addMacro(self, macro: ScriptTrigger) -> None:
 		pass
 
 	@overload
-	def init(self) -> None:
+	def setFile(self, macro: MultiElementContainer) -> None:
 		pass
 
 	@overload
-	def setEventType(self, type: str) -> None:
+	def setEvent(self, macro: MacroContainer) -> None:
 		pass
 
 	@overload
-	def setFile(self, f: File) -> None:
+	def runFile(self) -> None:
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
+	def confirmRemoveMacro(self, macro: MultiElementContainer) -> None:
 		pass
 
 	@overload
-	def onKey(self, translationKey: str) -> bool:
+	def removeMacro(self, macro: MultiElementContainer) -> None:
 		pass
 
 	@overload
-	def buildKeyName(self, translationKeys: str) -> Text:
+	def setMacroPos(self) -> None:
 		pass
 
 	@overload
-	def setKey(self, translationKeys: str) -> None:
+	def editFile(self, file: File) -> None:
 		pass
 
 	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
+	@overload
+	def updateSettings(self) -> None:
+		pass
+
+	@overload
+	def close(self) -> None:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MacroScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SmithingInventory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,55 @@
 from typing import overload
 from typing import TypeVar
-from .BaseScreen import BaseScreen
-from .ScriptTrigger import ScriptTrigger
-from .MultiElementContainer import MultiElementContainer
-from .MacroContainer import MacroContainer
-
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-File = TypeVar["java.io.File"]
+from .Inventory import Inventory
+from .ItemStackHelper import ItemStackHelper
 
-class MacroScreen(BaseScreen):
+net_minecraft_client_gui_screen_ingame_SmithingScreen = TypeVar("net_minecraft_client_gui_screen_ingame_SmithingScreen")
+SmithingScreen = net_minecraft_client_gui_screen_ingame_SmithingScreen
 
-	@overload
-	def __init__(self, parent: Screen) -> None:
-		pass
 
-	@overload
-	def mouseScrolled(self, mouseX: float, mouseY: float, amount: float) -> bool:
-		pass
+class SmithingInventory(Inventory):
+	"""
+	Since: 1.8.4 
+	"""
 
 	@overload
-	def addMacro(self, macro: ScriptTrigger) -> None:
+	def __init__(self, inventory: SmithingScreen) -> None:
 		pass
 
 	@overload
-	def setFile(self, macro: MultiElementContainer) -> None:
-		pass
+	def getLeftInput(self) -> ItemStackHelper:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def setEvent(self, macro: MacroContainer) -> None:
+		Returns:
+			the left input item. 
+		"""
 		pass
 
 	@overload
-	def runFile(self) -> None:
-		pass
+	def getRightInput(self) -> ItemStackHelper:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def confirmRemoveMacro(self, macro: MultiElementContainer) -> None:
+		Returns:
+			the right input item. 
+		"""
 		pass
 
 	@overload
-	def removeMacro(self, macro: MultiElementContainer) -> None:
-		pass
+	def getOutput(self) -> ItemStackHelper:
+		"""
+		Since: 1.8.4 
 
-	@overload
-	def setMacroPos(self) -> None:
-		pass
-
-	@overload
-	def editFile(self, file: File) -> None:
-		pass
-
-	@overload
-	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
-		pass
-
-	@overload
-	def updateSettings(self) -> None:
+		Returns:
+			the expected output item. 
+		"""
 		pass
 
 	@overload
-	def close(self) -> None:
+	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Mappings.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Mappings.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MerchantEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MerchantEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientPlayerInteractionManager.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinClientPlayerInteractionManager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 from typing import overload
 from typing import TypeVar
 
-Entity = TypeVar["net.minecraft.entity.Entity"]
-CallbackInfoReturnable = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfoReturnable_net.minecraft.util.ActionResult_"]
-CallbackInfo = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfo"]
-BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
-ClientPlayerEntity = TypeVar["net.minecraft.client.network.ClientPlayerEntity"]
-BlockHitResult = TypeVar["net.minecraft.util.hit.BlockHitResult"]
-Hand = TypeVar["net.minecraft.util.Hand"]
-Direction = TypeVar["net.minecraft.util.math.Direction"]
-PlayerEntity = TypeVar["net.minecraft.entity.player.PlayerEntity"]
+net_minecraft_entity_Entity = TypeVar("net_minecraft_entity_Entity")
+Entity = net_minecraft_entity_Entity
+
+org_spongepowered_asm_mixin_injection_callback_CallbackInfoReturnable_net_minecraft_util_ActionResult_ = TypeVar("org_spongepowered_asm_mixin_injection_callback_CallbackInfoReturnable_net_minecraft_util_ActionResult_")
+CallbackInfoReturnable = org_spongepowered_asm_mixin_injection_callback_CallbackInfoReturnable_net_minecraft_util_ActionResult_
+
+org_spongepowered_asm_mixin_injection_callback_CallbackInfo = TypeVar("org_spongepowered_asm_mixin_injection_callback_CallbackInfo")
+CallbackInfo = org_spongepowered_asm_mixin_injection_callback_CallbackInfo
+
+net_minecraft_util_math_BlockPos = TypeVar("net_minecraft_util_math_BlockPos")
+BlockPos = net_minecraft_util_math_BlockPos
+
+net_minecraft_client_network_ClientPlayerEntity = TypeVar("net_minecraft_client_network_ClientPlayerEntity")
+ClientPlayerEntity = net_minecraft_client_network_ClientPlayerEntity
+
+net_minecraft_util_hit_BlockHitResult = TypeVar("net_minecraft_util_hit_BlockHitResult")
+BlockHitResult = net_minecraft_util_hit_BlockHitResult
+
+net_minecraft_util_Hand = TypeVar("net_minecraft_util_Hand")
+Hand = net_minecraft_util_Hand
+
+net_minecraft_util_math_Direction = TypeVar("net_minecraft_util_math_Direction")
+Direction = net_minecraft_util_math_Direction
+
+net_minecraft_entity_player_PlayerEntity = TypeVar("net_minecraft_entity_player_PlayerEntity")
+PlayerEntity = net_minecraft_entity_player_PlayerEntity
+
 
 class MixinClientPlayerInteractionManager:
 
 	@overload
 	def __init__(self) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinClientWorld.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinLivingEntity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from typing import overload
 from typing import TypeVar
 
-Entity = TypeVar["net.minecraft.entity.Entity"]
-Entity_RemovalReason = TypeVar["net.minecraft.entity.Entity.RemovalReason"]
-CallbackInfo = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfo"]
+net_minecraft_entity_EntityType__ = TypeVar("net_minecraft_entity_EntityType__")
+EntityType = net_minecraft_entity_EntityType__
 
-class MixinClientWorld:
+net_minecraft_entity_Entity = TypeVar("net_minecraft_entity_Entity")
+Entity = net_minecraft_entity_Entity
+
+org_spongepowered_asm_mixin_injection_callback_CallbackInfo = TypeVar("org_spongepowered_asm_mixin_injection_callback_CallbackInfo")
+CallbackInfo = org_spongepowered_asm_mixin_injection_callback_CallbackInfo
+
+net_minecraft_world_World = TypeVar("net_minecraft_world_World")
+World = net_minecraft_world_World
+
+
+class MixinLivingEntity(Entity):
 
 	@overload
-	def __init__(self) -> None:
+	def __init__(self, arg: EntityType, arg2: World) -> None:
 		pass
 
 	@overload
-	def onAddEntity(self, id: int, entity: Entity, ci: CallbackInfo) -> None:
+	def getMaxHealth(self) -> float:
 		pass
 
 	@overload
-	def onRemoveEntity(self, entityId: int, removalReason: Entity_RemovalReason, ci: CallbackInfo, entity: Entity) -> None:
+	def onSetHealth(self, health: float, ci: CallbackInfo) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinLivingEntity.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceScreen.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from typing import overload
 from typing import TypeVar
+from .MacroScreen import MacroScreen
+from .MultiElementContainer import MultiElementContainer
 
-EntityType = TypeVar["net.minecraft.entity.EntityType__"]
-Entity = TypeVar["net.minecraft.entity.Entity"]
-CallbackInfo = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfo"]
-World = TypeVar["net.minecraft.world.World"]
+net_minecraft_client_gui_screen_Screen = TypeVar("net_minecraft_client_gui_screen_Screen")
+Screen = net_minecraft_client_gui_screen_Screen
 
-class MixinLivingEntity(Entity):
+
+class ServiceScreen(MacroScreen):
+
+	@overload
+	def __init__(self, parent: Screen) -> None:
+		pass
+
+	@overload
+	def addService(self, service: str) -> None:
+		pass
 
 	@overload
-	def __init__(self, arg: EntityType, arg2: World) -> None:
+	def removeMacro(self, macro: MultiElementContainer) -> None:
 		pass
 
 	@overload
-	def getMaxHealth(self) -> float:
+	def setFile(self, macro: MultiElementContainer) -> None:
 		pass
 
 	@overload
-	def onSetHealth(self, health: float, ci: CallbackInfo) -> None:
+	def close(self) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinMinecraftClient.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MovementQueue.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 from typing import overload
 from typing import TypeVar
+from .Draw3D import Draw3D
+from .PlayerInput import PlayerInput
 
-ClientPlayerInteractionManager = TypeVar["net.minecraft.client.network.ClientPlayerInteractionManager"]
-CallbackInfo = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfo"]
-Screen = TypeVar["net.minecraft.client.gui.screen.Screen"]
-ClientWorld = TypeVar["net.minecraft.client.world.ClientWorld"]
-
-class MixinMinecraftClient:
-	currentScreen: Screen
-	interactionManager: ClientPlayerInteractionManager
+net_minecraft_client_network_ClientPlayerEntity = TypeVar("net_minecraft_client_network_ClientPlayerEntity")
+ClientPlayerEntity = net_minecraft_client_network_ClientPlayerEntity
 
-	@overload
-	def __init__(self) -> None:
-		pass
+
+class MovementQueue:
+	predPoints: Draw3D
 
 	@overload
-	def setScreen(self, screen: Screen) -> None:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def onJoinWorld(self, world: ClientWorld, info: CallbackInfo) -> None:
+	def tick(self, newPlayer: ClientPlayerEntity) -> PlayerInput:
 		pass
 
 	@overload
-	def onOpenScreen(self, screen: Screen, info: CallbackInfo) -> None:
+	def append(self, input: PlayerInput, newPlayer: ClientPlayerEntity) -> None:
 		pass
 
 	@overload
-	def afterOpenScreen(self, screen: Screen, info: CallbackInfo) -> None:
+	def setDrawPredictions(self, val: bool) -> None:
 		pass
 
 	@overload
-	def onDisconnect(self, s: Screen, info: CallbackInfo) -> None:
+	def clear(self) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinRecipeBookWidget.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinRecipeBookResults.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .IRecipeBookWidget import IRecipeBookWidget
+from .IRecipeBookResults import IRecipeBookResults
 
-ClientRecipeBook = TypeVar["net.minecraft.client.recipebook.ClientRecipeBook"]
-RecipeBookResults = TypeVar["net.minecraft.client.gui.screen.recipebook.RecipeBookResults"]
+net_minecraft_client_gui_screen_recipebook_RecipeResultCollection = TypeVar("net_minecraft_client_gui_screen_recipebook_RecipeResultCollection")
+RecipeResultCollection = net_minecraft_client_gui_screen_recipebook_RecipeResultCollection
 
-class MixinRecipeBookWidget(IRecipeBookWidget):
 
-	@overload
-	def __init__(self) -> None:
-		pass
-
-	@overload
-	def jsmacros_getResults(self) -> RecipeBookResults:
-		pass
+class MixinRecipeBookResults(IRecipeBookResults):
 
 	@overload
-	def jsmacros_isSearching(self) -> bool:
-		pass
-
-	@overload
-	def jsmacros_refreshResultList(self) -> None:
+	def __init__(self) -> None:
 		pass
 
 	@overload
-	def jsmacros_getRecipeBook(self) -> ClientRecipeBook:
+	def jsmacros_getResultCollections(self) -> List[RecipeResultCollection]:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MixinScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MixinScreen.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,30 @@
 from .CheckBoxWidgetHelper_CheckBoxBuilder import CheckBoxWidgetHelper_CheckBoxBuilder
 from .CyclingButtonWidgetHelper_CyclicButtonBuilder import CyclingButtonWidgetHelper_CyclicButtonBuilder
 from .LockButtonWidgetHelper_LockButtonBuilder import LockButtonWidgetHelper_LockButtonBuilder
 from .SliderWidgetHelper_SliderBuilder import SliderWidgetHelper_SliderBuilder
 from .TextFieldWidgetHelper_TextFieldBuilder import TextFieldWidgetHelper_TextFieldBuilder
 from .ButtonWidgetHelper_TexturedButtonBuilder import ButtonWidgetHelper_TexturedButtonBuilder
 
-AbstractParentElement = TypeVar["net.minecraft.client.gui.AbstractParentElement"]
+net_minecraft_client_gui_AbstractParentElement = TypeVar("net_minecraft_client_gui_AbstractParentElement")
+AbstractParentElement = net_minecraft_client_gui_AbstractParentElement
+
 T = TypeVar("T")
-CallbackInfoReturnable = TypeVar["org.spongepowered.asm.mixin.injection.callback.CallbackInfoReturnable_java.lang.Boolean_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Style = TypeVar["net.minecraft.text.Style"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+org_spongepowered_asm_mixin_injection_callback_CallbackInfoReturnable_java_lang_Boolean_ = TypeVar("org_spongepowered_asm_mixin_injection_callback_CallbackInfoReturnable_java_lang_Boolean_")
+CallbackInfoReturnable = org_spongepowered_asm_mixin_injection_callback_CallbackInfoReturnable_java_lang_Boolean_
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Style = TypeVar("net_minecraft_text_Style")
+Style = net_minecraft_text_Style
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class MixinScreen(IScreen, IScreenInternal, AbstractParentElement):
 	width: int
 	height: int
 	textRenderer: TextRenderer
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MobEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MobEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ModContainerHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ModContainerHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ModLoader.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ModLoader.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MooshroomEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MooshroomEntityHelper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-MooshroomEntity = TypeVar["net.minecraft.entity.passive.MooshroomEntity"]
+net_minecraft_entity_passive_MooshroomEntity = TypeVar("net_minecraft_entity_passive_MooshroomEntity")
+MooshroomEntity = net_minecraft_entity_passive_MooshroomEntity
+
 
 class MooshroomEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MovementDummy.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MovementDummy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,39 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .PlayerInput import PlayerInput
 
-LivingEntity = TypeVar["net.minecraft.entity.LivingEntity"]
-Iterable = TypeVar["java.lang.Iterable_net.minecraft.item.ItemStack_"]
-EquipmentSlot = TypeVar["net.minecraft.entity.EquipmentSlot"]
-Box = TypeVar["net.minecraft.util.math.Box"]
-ClientPlayerEntity = TypeVar["net.minecraft.client.network.ClientPlayerEntity"]
-World = TypeVar["net.minecraft.world.World"]
-ItemStack = TypeVar["net.minecraft.item.ItemStack"]
-Arm = TypeVar["net.minecraft.util.Arm"]
-Vec3d = TypeVar["net.minecraft.util.math.Vec3d"]
+net_minecraft_entity_LivingEntity = TypeVar("net_minecraft_entity_LivingEntity")
+LivingEntity = net_minecraft_entity_LivingEntity
+
+java_lang_Iterable_net_minecraft_item_ItemStack_ = TypeVar("java_lang_Iterable_net_minecraft_item_ItemStack_")
+Iterable = java_lang_Iterable_net_minecraft_item_ItemStack_
+
+net_minecraft_entity_EquipmentSlot = TypeVar("net_minecraft_entity_EquipmentSlot")
+EquipmentSlot = net_minecraft_entity_EquipmentSlot
+
+net_minecraft_util_math_Box = TypeVar("net_minecraft_util_math_Box")
+Box = net_minecraft_util_math_Box
+
+net_minecraft_client_network_ClientPlayerEntity = TypeVar("net_minecraft_client_network_ClientPlayerEntity")
+ClientPlayerEntity = net_minecraft_client_network_ClientPlayerEntity
+
+net_minecraft_world_World = TypeVar("net_minecraft_world_World")
+World = net_minecraft_world_World
+
+net_minecraft_item_ItemStack = TypeVar("net_minecraft_item_ItemStack")
+ItemStack = net_minecraft_item_ItemStack
+
+net_minecraft_util_Arm = TypeVar("net_minecraft_util_Arm")
+Arm = net_minecraft_util_Arm
+
+net_minecraft_util_math_Vec3d = TypeVar("net_minecraft_util_math_Vec3d")
+Vec3d = net_minecraft_util_math_Vec3d
+
 
 class MovementDummy(LivingEntity):
 
 	@overload
 	def __init__(self, player: "MovementDummy") -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/MultiElementContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/MultiElementContainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 from typing import TypeVar
 from typing import Generic
 from .IContainerParent import IContainerParent
 from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
 
 T = TypeVar("T")
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Element = TypeVar["net.minecraft.client.gui.Element"]
-ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_gui_Element = TypeVar("net_minecraft_client_gui_Element")
+Element = net_minecraft_client_gui_Element
+
+net_minecraft_client_gui_widget_ClickableWidget = TypeVar("net_minecraft_client_gui_widget_ClickableWidget")
+ClickableWidget = net_minecraft_client_gui_widget_ClickableWidget
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class MultiElementContainer(IContainerParent, Generic[T]):
 	parent: T
 	x: int
 	y: int
 	width: int
 	height: int
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from typing import Generic
 from .BaseHelper import BaseHelper
 from .NBTElementHelper_NBTNumberHelper import NBTElementHelper_NBTNumberHelper
 from .NBTElementHelper_NBTListHelper import NBTElementHelper_NBTListHelper
 from .NBTElementHelper_NBTCompoundHelper import NBTElementHelper_NBTCompoundHelper
 
 T = TypeVar("T")
-NbtElement = TypeVar["net.minecraft.nbt.NbtElement"]
+net_minecraft_nbt_NbtElement = TypeVar("net_minecraft_nbt_NbtElement")
+NbtElement = net_minecraft_nbt_NbtElement
+
 
 class NBTElementHelper(Generic[T], BaseHelper):
 	"""
 	Since: 1.5.1 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper_NBTCompoundHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper_NBTListHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper_NBTListHelper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .NBTElementHelper import NBTElementHelper
 
-UUID = TypeVar["java.util.UUID"]
+java_util_UUID = TypeVar("java_util_UUID")
+UUID = java_util_UUID
+
 
 class NBTElementHelper_NBTListHelper(NBTElementHelper):
 	"""
 	Since: 1.5.1 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/NBTElementHelper_NBTNumberHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/NameUtil.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/NameUtil.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/NoStyleCodeCompiler.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/DefaultCodeCompiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
-Runnable = TypeVar["java.lang.Runnable"]
-Text = TypeVar["net.minecraft.text.Text"]
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
 
-class NoStyleCodeCompiler(AbstractRenderCodeCompiler):
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+
+class DefaultCodeCompiler(AbstractRenderCodeCompiler):
 
 	@overload
 	def __init__(self, language: str, screen: EditorScreen) -> None:
 		pass
 
 	@overload
 	def recompileRenderedText(self, text: str) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OcelotEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PigEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-OcelotEntity = TypeVar["net.minecraft.entity.passive.OcelotEntity"]
+net_minecraft_entity_passive_PigEntity = TypeVar("net_minecraft_entity_passive_PigEntity")
+PigEntity = net_minecraft_entity_passive_PigEntity
 
-class OcelotEntityHelper(AnimalEntityHelper):
+
+class PigEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: OcelotEntity) -> None:
+	def __init__(self, base: PigEntity) -> None:
 		pass
 
 	@overload
-	def isTrusting(self) -> bool:
-		"""Ocelots trust players after being fed with cod or salmon.\n
+	def isSaddled(self) -> bool:
+		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this ocelot is trusting player and not running away form them, 'false' otherwise. 
+			'true' if this pig is saddled, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsField.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class OptionsField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from .OptionsHelper_SkinOptionsHelper import OptionsHelper_SkinOptionsHelper
 from .OptionsHelper_VideoOptionsHelper import OptionsHelper_VideoOptionsHelper
 from .OptionsHelper_MusicOptionsHelper import OptionsHelper_MusicOptionsHelper
 from .OptionsHelper_ControlOptionsHelper import OptionsHelper_ControlOptionsHelper
 from .OptionsHelper_ChatOptionsHelper import OptionsHelper_ChatOptionsHelper
 from .OptionsHelper_AccessibilityOptionsHelper import OptionsHelper_AccessibilityOptionsHelper
 
-GameOptions = TypeVar["net.minecraft.client.option.GameOptions"]
+net_minecraft_client_option_GameOptions = TypeVar("net_minecraft_client_option_GameOptions")
+GameOptions = net_minecraft_client_option_GameOptions
+
 
 class OptionsHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 	skin: OptionsHelper_SkinOptionsHelper
 	video: OptionsHelper_VideoOptionsHelper
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_AccessibilityOptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_AccessibilityOptionsHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_ChatOptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_ChatOptionsHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_ControlOptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_ControlOptionsHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .OptionsHelper import OptionsHelper
 
-KeyBinding = TypeVar["net.minecraft.client.option.KeyBinding"]
+net_minecraft_client_option_KeyBinding = TypeVar("net_minecraft_client_option_KeyBinding")
+KeyBinding = net_minecraft_client_option_KeyBinding
+
 
 class OptionsHelper_ControlOptionsHelper:
 	parent: OptionsHelper
 
 	@overload
 	def __init__(self, OptionsHelper: OptionsHelper) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_MusicOptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_MusicOptionsHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_SkinOptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_SkinOptionsHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OptionsHelper_VideoOptionsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OptionsHelper_VideoOptionsHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/OverlayContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/OverlayContainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from typing import overload
 from typing import TypeVar
 from typing import Mapping
 from .IOverlayParent import IOverlayParent
 from .MultiElementContainer import MultiElementContainer
 from .Scrollbar import Scrollbar
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Element = TypeVar["net.minecraft.client.gui.Element"]
-ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_gui_Element = TypeVar("net_minecraft_client_gui_Element")
+Element = net_minecraft_client_gui_Element
+
+net_minecraft_client_gui_widget_ClickableWidget = TypeVar("net_minecraft_client_gui_widget_ClickableWidget")
+ClickableWidget = net_minecraft_client_gui_widget_ClickableWidget
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class OverlayContainer(IOverlayParent, MultiElementContainer):
 	savedBtnStates: Mapping[ClickableWidget, bool]
 	scroll: Scrollbar
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PacketByteBufferHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PacketByteBufferHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,58 @@
 from .TextBuilder import TextBuilder
 from .TextHelper import TextHelper
 from .NBTElementHelper_NBTCompoundHelper import NBTElementHelper_NBTCompoundHelper
 from .NBTElementHelper import NBTElementHelper
 from .ItemStackHelper import ItemStackHelper
 from .Pos3D import Pos3D
 
-Packet = TypeVar["net.minecraft.network.packet.Packet__"]
-IndexedIterable = TypeVar["net.minecraft.util.collection.IndexedIterable_T_"]
-Optional = TypeVar["java.util.Optional_T_"]
-BitSet = TypeVar["java.util.BitSet"]
+net_minecraft_network_packet_Packet__ = TypeVar("net_minecraft_network_packet_Packet__")
+Packet = net_minecraft_network_packet_Packet__
+
+net_minecraft_util_collection_IndexedIterable_T_ = TypeVar("net_minecraft_util_collection_IndexedIterable_T_")
+IndexedIterable = net_minecraft_util_collection_IndexedIterable_T_
+
+java_util_Optional_T_ = TypeVar("java_util_Optional_T_")
+Optional = java_util_Optional_T_
+
+java_util_BitSet = TypeVar("java_util_BitSet")
+BitSet = java_util_BitSet
+
 K = TypeVar("K")
+K = K
+
 L = TypeVar("L")
-Date = TypeVar["java.util.Date"]
-Function = TypeVar["java.util.function.Function_net.minecraft.network.PacketByteBuf, extends net.minecraft.network.packet.Packet___"]
+L = L
+
+java_util_Date = TypeVar("java_util_Date")
+Date = java_util_Date
+
+java_util_function_Function_net_minecraft_network_PacketByteBuf, extends net_minecraft_network_packet_Packet___ = TypeVar("java_util_function_Function_net_minecraft_network_PacketByteBuf, extends net_minecraft_network_packet_Packet___")
+Function = java_util_function_Function_net_minecraft_network_PacketByteBuf, extends net_minecraft_network_packet_Packet___
+
 R = TypeVar("R")
 T = TypeVar("T")
-GameProfile = TypeVar["com.mojang.authlib.GameProfile"]
+com_mojang_authlib_GameProfile = TypeVar("com_mojang_authlib_GameProfile")
+GameProfile = com_mojang_authlib_GameProfile
+
 V = TypeVar("V")
-PacketByteBuf = TypeVar["net.minecraft.network.PacketByteBuf"]
-UUID = TypeVar["java.util.UUID"]
-BlockHitResult = TypeVar["net.minecraft.util.hit.BlockHitResult"]
-RegistryKey = TypeVar["net.minecraft.registry.RegistryKey_T_"]
+V = V
+
+net_minecraft_network_PacketByteBuf = TypeVar("net_minecraft_network_PacketByteBuf")
+PacketByteBuf = net_minecraft_network_PacketByteBuf
+
+java_util_UUID = TypeVar("java_util_UUID")
+UUID = java_util_UUID
+
+net_minecraft_util_hit_BlockHitResult = TypeVar("net_minecraft_util_hit_BlockHitResult")
+BlockHitResult = net_minecraft_util_hit_BlockHitResult
+
+net_minecraft_registry_RegistryKey_T_ = TypeVar("net_minecraft_registry_RegistryKey_T_")
+RegistryKey = net_minecraft_registry_RegistryKey_T_
+
 
 class PacketByteBufferHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 	BUFFER_TO_PACKET: Mapping[Class, Function]
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PaintingEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PaintingEntityHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 
-PaintingEntity = TypeVar["net.minecraft.entity.decoration.painting.PaintingEntity"]
+net_minecraft_entity_decoration_painting_PaintingEntity = TypeVar("net_minecraft_entity_decoration_painting_PaintingEntity")
+PaintingEntity = net_minecraft_entity_decoration_painting_PaintingEntity
+
 
 class PaintingEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PandaEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PandaEntityHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-PandaEntity = TypeVar["net.minecraft.entity.passive.PandaEntity"]
+net_minecraft_entity_passive_PandaEntity = TypeVar("net_minecraft_entity_passive_PandaEntity")
+PandaEntity = net_minecraft_entity_passive_PandaEntity
+
 
 class PandaEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ParrotEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ParrotEntityHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .TameableEntityHelper import TameableEntityHelper
 
-ParrotEntity = TypeVar["net.minecraft.entity.passive.ParrotEntity"]
+net_minecraft_entity_passive_ParrotEntity = TypeVar("net_minecraft_entity_passive_ParrotEntity")
+ParrotEntity = net_minecraft_entity_passive_ParrotEntity
+
 
 class ParrotEntityHelper(TameableEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PiglinEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PiglinEntityHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractPiglinEntityHelper import AbstractPiglinEntityHelper
 
-PiglinEntity = TypeVar["net.minecraft.entity.mob.PiglinEntity"]
+net_minecraft_entity_mob_PiglinEntity = TypeVar("net_minecraft_entity_mob_PiglinEntity")
+PiglinEntity = net_minecraft_entity_mob_PiglinEntity
+
 
 class PiglinEntityHelper(AbstractPiglinEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Plane3D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Plane3D.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerAbilitiesHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerAbilitiesHelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 
-PlayerAbilities = TypeVar["net.minecraft.entity.player.PlayerAbilities"]
+net_minecraft_entity_player_PlayerAbilities = TypeVar("net_minecraft_entity_player_PlayerAbilities")
+PlayerAbilities = net_minecraft_entity_player_PlayerAbilities
+
 
 class PlayerAbilitiesHelper(BaseHelper):
 	"""
 	Since: 1.0.3 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerInput.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerInput.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 
-Input = TypeVar["net.minecraft.client.input.Input"]
+net_minecraft_client_input_Input = TypeVar("net_minecraft_client_input_Input")
+Input = net_minecraft_client_input_Input
+
 
 class PlayerInput:
 	"""An object, that combines all possible player inputs\n
 	Since: 1.4.0 
 	"""
 	movementForward: float
 	movementSideways: float
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PlayerInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PlayerListEntryHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StyleHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,131 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
-from .TeamHelper import TeamHelper
+from .FormattingHelper import FormattingHelper
 
-PlayerListEntry = TypeVar["net.minecraft.client.network.PlayerListEntry"]
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
 
-class PlayerListEntryHelper(BaseHelper):
+net_minecraft_text_Style = TypeVar("net_minecraft_text_Style")
+Style = net_minecraft_text_Style
+
+
+class StyleHelper(BaseHelper):
 	"""
-	Since: 1.0.2 
+	Since: 1.6.5 
 	"""
 
 	@overload
-	def __init__(self, p: PlayerListEntry) -> None:
+	def __init__(self, base: Style) -> None:
 		pass
 
 	@overload
-	def getUUID(self) -> str:
-		"""
-		Since: 1.1.9 
-		"""
+	def hasColor(self) -> bool:
 		pass
 
 	@overload
-	def getName(self) -> str:
+	def getColor(self) -> int:
 		"""
-		Since: 1.0.2 
-		"""
-		pass
 
-	@overload
-	def getPing(self) -> int:
-		"""
-		Since: 1.6.5 
+		Returns:
+			the color index of this style or '-1' if no color is set. 
 		"""
 		pass
 
 	@overload
-	def getGamemode(self) -> str:
+	def getFormatting(self) -> FormattingHelper:
 		"""
-		Since: 1.6.5 
+		Since: 1.8.4 
 
 		Returns:
-			null if unknown 
+			the formatting of this style, or 'null' if no formatting was found. 
 		"""
 		pass
 
 	@overload
-	def getDisplayText(self) -> TextHelper:
+	def getColorIndex(self) -> int:
 		"""
-		Since: 1.1.9 
+		Since: 1.8.4 
+
+		Returns:
+			the color index of this style or '-1' if no color is set. 
 		"""
 		pass
 
 	@overload
-	def getPublicKey(self) -> List[float]:
+	def getColorValue(self) -> int:
 		"""
-		Since: 1.8.2 
+		Since: 1.8.4 
+
+		Returns:
+			the color value of this style or '-1' if it doesn't have one. 
 		"""
 		pass
 
 	@overload
-	def hasCape(self) -> bool:
+	def getColorName(self) -> str:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the player has a cape enabled, 'false' otherwise. 
+			the color name of this style or 'null' if it has no color. 
 		"""
 		pass
 
 	@overload
-	def hasSlimModel(self) -> bool:
-		"""A slim skin is an Alex skin, while the default one is Steve.\n
-		Since: 1.8.4 
+	def hasCustomColor(self) -> bool:
+		pass
 
-		Returns:
-			'true' if the player has a slim skin, 'false' otherwise. 
-		"""
+	@overload
+	def getCustomColor(self) -> int:
 		pass
 
 	@overload
-	def getSkinTexture(self) -> str:
-		"""
-		Since: 1.8.4 
+	def bold(self) -> bool:
+		pass
 
-		Returns:
-			the identifier of the player's skin texture or 'null' if it's unknown. 
-		"""
+	@overload
+	def italic(self) -> bool:
 		pass
 
 	@overload
-	def getCapeTexture(self) -> str:
-		"""
-		Since: 1.8.4 
+	def underlined(self) -> bool:
+		pass
 
-		Returns:
-			the identifier of the player's cape texture or 'null' if it's unknown. 
-		"""
+	@overload
+	def strikethrough(self) -> bool:
 		pass
 
 	@overload
-	def getElytraTexture(self) -> str:
-		"""
-		Since: 1.8.4 
+	def obfuscated(self) -> bool:
+		pass
 
-		Returns:
-			the identifier of the player's elytra texture or 'null' if it's unknown. 
-		"""
+	@overload
+	def getClickAction(self) -> str:
 		pass
 
 	@overload
-	def getTeam(self) -> TeamHelper:
-		"""
-		Since: 1.8.4 
+	def getClickValue(self) -> str:
+		pass
 
-		Returns:
-			the team of the player or 'null' if the player is not in a team. 
-		"""
+	@overload
+	def getCustomClickValue(self) -> Runnable:
+		pass
+
+	@overload
+	def getHoverAction(self) -> str:
+		pass
+
+	@overload
+	def getHoverValue(self) -> object:
+		pass
+
+	@overload
+	def getInsertion(self) -> str:
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Pos2D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Pos2D.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Pos3D.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Pos3D.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import TypeVar
 from .Pos2D import Pos2D
 from .Vec3D import Vec3D
 from .BlockPosHelper import BlockPosHelper
 
-BlockPos = TypeVar["net.minecraft.util.math.BlockPos"]
-Vec3d = TypeVar["net.minecraft.util.math.Vec3d"]
+net_minecraft_util_math_BlockPos = TypeVar("net_minecraft_util_math_BlockPos")
+BlockPos = net_minecraft_util_math_BlockPos
+
+net_minecraft_util_math_Vec3d = TypeVar("net_minecraft_util_math_Vec3d")
+Vec3d = net_minecraft_util_math_Vec3d
+
 
 class Pos3D(Pos2D):
 	"""
 	Since: 1.2.6 [citation needed] 
 	"""
 	ZERO: "Pos3D"
 	z: float
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PrimitiveSettingGroup.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PrimitiveSettingGroup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay import SettingsOverlay
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class PrimitiveSettingGroup(AbstractSettingContainer):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PrioryFiFoTaskQueue.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Vec3D.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,185 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from typing import Any
-from typing import Generic
+from .Vec2D import Vec2D
+from .Pos3D import Pos3D
 
-Function = TypeVar["java.util.function.Function_E,java.lang.Integer_"]
-T = TypeVar("T")
-E = TypeVar("E")
-Queue = TypeVar["java.util.Queue_E_"]
+org_joml_Vector3f = TypeVar("org_joml_Vector3f")
+Vector3f = org_joml_Vector3f
 
-class PrioryFiFoTaskQueue(Queue, Generic[E]):
+
+class Vec3D(Vec2D):
+	"""
+	Since: 1.2.6 [citation needed] 
+	"""
+	z1: float
+	z2: float
 
 	@overload
-	def __init__(self, priorityFunction: Function) -> None:
+	def __init__(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> None:
 		pass
 
 	@overload
-	def size(self) -> int:
+	def __init__(self, start: Pos3D, end: Pos3D) -> None:
 		pass
 
 	@overload
-	def isEmpty(self) -> bool:
+	def getZ1(self) -> float:
 		pass
 
 	@overload
-	def contains(self, o: object) -> bool:
+	def getZ2(self) -> float:
 		pass
 
 	@overload
-	def iterator(self) -> iter:
+	def getDeltaZ(self) -> float:
 		pass
 
 	@overload
-	def toArray(self) -> List[object]:
+	def getStart(self) -> Pos3D:
 		pass
 
 	@overload
-	def toArray(self, ts: List[T]) -> List[T]:
+	def getEnd(self) -> Pos3D:
 		pass
 
 	@overload
-	def add(self, e: E) -> bool:
+	def getMagnitude(self) -> float:
 		pass
 
 	@overload
-	def remove(self, o: object) -> bool:
+	def getMagnitudeSq(self) -> float:
 		pass
 
 	@overload
-	def containsAll(self, collection: List[Any]) -> bool:
+	def add(self, vec: "Vec3D") -> "Vec3D":
 		pass
 
 	@overload
-	def addAll(self, collection: List[Any]) -> bool:
+	def addStart(self, pos: Pos3D) -> "Vec3D":
+		"""
+		Since: 1.6.4 
+
+		Args:
+			pos: 
+		"""
 		pass
 
 	@overload
-	def removeAll(self, collection: List[Any]) -> bool:
+	def addEnd(self, pos: Pos3D) -> "Vec3D":
+		"""
+		Since: 1.6.4 
+
+		Args:
+			pos: 
+		"""
 		pass
 
 	@overload
-	def retainAll(self, collection: List[Any]) -> bool:
+	def addStart(self, x: float, y: float, z: float) -> "Vec3D":
+		"""
+		Since: 1.6.4 
+
+		Args:
+			x: 
+			y: 
+			z: 
+		"""
 		pass
 
 	@overload
-	def clear(self) -> None:
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
-	def offer(self, e: E) -> bool:
+	def multiply(self, vec: "Vec3D") -> "Vec3D":
+		pass
+
+	@overload
+	def multiply(self, x1: float, y1: float, z1: float, x2: float, y2: float, z2: float) -> "Vec3D":
+		"""
+		Since: 1.6.3 
+
+		Args:
+			z1: 
+			y1: 
+			z2: 
+			x1: 
+			y2: 
+			x2: 
+		"""
+		pass
+
+	@overload
+	def scale(self, scale: float) -> "Vec3D":
+		"""
+		Since: 1.6.3 
+
+		Args:
+			scale: 
+		"""
 		pass
 
 	@overload
-	def remove(self) -> E:
+	def normalize(self) -> "Vec3D":
+		"""
+		Since: 1.6.5 
+		"""
 		pass
 
 	@overload
-	def poll(self) -> E:
+	def getPitch(self) -> float:
 		pass
 
 	@overload
-	def pollWaiting(self) -> E:
+	def getYaw(self) -> float:
 		pass
 
 	@overload
-	def pollWaiting(self, timeout: float) -> E:
+	def dotProduct(self, vec: "Vec3D") -> float:
 		pass
 
 	@overload
-	def peekWaiting(self) -> E:
+	def crossProduct(self, vec: "Vec3D") -> "Vec3D":
 		pass
 
 	@overload
-	def peekWaiting(self, timeout: float) -> E:
+	def reverse(self) -> "Vec3D":
 		pass
 
 	@overload
-	def element(self) -> E:
+	def toString(self) -> str:
 		pass
 
 	@overload
-	def peek(self) -> E:
+	def toMojangFloatVector(self) -> Vector3f:
+		"""
+		Since: 1.6.5 
+		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Profile.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Profile.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseProfile import BaseProfile
 from .Core import Core
 from .BaseEvent import BaseEvent
 
-Throwable = TypeVar["java.lang.Throwable"]
-Logger = TypeVar["org.slf4j.Logger"]
+java_lang_Throwable = TypeVar("java_lang_Throwable")
+Throwable = java_lang_Throwable
+
+org_slf4j_Logger = TypeVar("org_slf4j_Logger")
+Logger = org_slf4j_Logger
+
 
 class Profile(BaseProfile):
 	ignoredErrors: List[Class]
 
 	@overload
 	def __init__(self, runner: Core, logger: Logger) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ProfileSetting.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProfileSetting_ProfileEntry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from .AbstractMapSettingContainer import AbstractMapSettingContainer
-from .SettingsOverlay import SettingsOverlay
+from .AbstractMapSettingContainer_MapSettingEntry import AbstractMapSettingContainer_MapSettingEntry
+from .ProfileSetting import ProfileSetting
 from .ScriptTrigger import ScriptTrigger
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-class ProfileSetting(AbstractMapSettingContainer):
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: SettingsOverlay, group: List[str]) -> None:
-		pass
-
-	@overload
-	def addField(self, key: str, value: List[ScriptTrigger]) -> None:
-		pass
+class ProfileSetting_ProfileEntry(AbstractMapSettingContainer_MapSettingEntry):
 
 	@overload
-	def removeField(self, key: str) -> None:
+	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: ProfileSetting, key: str, value: List[ScriptTrigger]) -> None:
 		pass
 
 	@overload
-	def changeKey(self, key: str, newKey: str) -> None:
+	def init(self) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ProxyBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ProxyBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/PufferfishEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PufferfishEntityHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .FishEntityHelper import FishEntityHelper
 
-PufferfishEntity = TypeVar["net.minecraft.entity.passive.PufferfishEntity"]
+net_minecraft_entity_passive_PufferfishEntity = TypeVar("net_minecraft_entity_passive_PufferfishEntity")
+PufferfishEntity = net_minecraft_entity_passive_PufferfishEntity
+
 
 class PufferfishEntityHelper(FishEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/RabbitEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BeeEntityHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from typing import overload
 from typing import TypeVar
 from .AnimalEntityHelper import AnimalEntityHelper
 
-RabbitEntity = TypeVar["net.minecraft.entity.passive.RabbitEntity"]
+net_minecraft_entity_passive_BeeEntity = TypeVar("net_minecraft_entity_passive_BeeEntity")
+BeeEntity = net_minecraft_entity_passive_BeeEntity
 
-class RabbitEntityHelper(AnimalEntityHelper):
+
+class BeeEntityHelper(AnimalEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: RabbitEntity) -> None:
+	def __init__(self, base: BeeEntity) -> None:
+		pass
+
+	@overload
+	def hasNectar(self) -> bool:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			'true' if the bee has nectar, 'false' otherwise. 
+		"""
 		pass
 
 	@overload
-	def getVariant(self) -> str:
+	def isAngry(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the variant of this rabbit. 
+			'true' if the bee is angry at a player, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isKillerBunny(self) -> bool:
+	def hasStung(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this rabbit is a killer bunny, 'false' otherwise. 
+			'true' if the bee has already stung a player, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/RecipeHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/RecipeHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .ItemStackHelper import ItemStackHelper
 
-Recipe = TypeVar["net.minecraft.recipe.Recipe__"]
+net_minecraft_recipe_Recipe__ = TypeVar("net_minecraft_recipe_Recipe__")
+Recipe = net_minecraft_recipe_Recipe__
+
 
 class RecipeHelper(BaseHelper):
 	"""
 	Since: 1.3.1 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/RecipeInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/RecipeInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Rect.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Rect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .IDraw2D import IDraw2D
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
 
 class Rect(RenderElement, Alignable):
 	"""
 	Since: 1.0.5 
 	"""
 	parent: IDraw2D
 	rotation: float
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Rect_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Rect_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/RegistryHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/RegistryHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 from .BlockHelper import BlockHelper
 from .BlockStateHelper import BlockStateHelper
 from .StatusEffectHelper import StatusEffectHelper
 from .EnchantmentHelper import EnchantmentHelper
 from .EntityHelper import EntityHelper
 from .FluidStateHelper import FluidStateHelper
 
-EntityType = TypeVar["net.minecraft.entity.EntityType__"]
-Identifier = TypeVar["net.minecraft.util.Identifier"]
+net_minecraft_entity_EntityType__ = TypeVar("net_minecraft_entity_EntityType__")
+EntityType = net_minecraft_entity_EntityType__
+
+net_minecraft_util_Identifier = TypeVar("net_minecraft_util_Identifier")
+Identifier = net_minecraft_util_Identifier
+
 
 class RegistryHelper:
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/RunningContextContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/RunningContextContainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import TypeVar
 from .MultiElementContainer import MultiElementContainer
 from .BaseScriptContext import BaseScriptContext
 from .CancelScreen import CancelScreen
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class RunningContextContainer(MultiElementContainer):
 	t: BaseScriptContext
 	service: bool
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: CancelScreen, t: BaseScriptContext) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScoreboardObjectiveHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScoreboardObjectiveHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 
-ScoreboardObjective = TypeVar["net.minecraft.scoreboard.ScoreboardObjective"]
+net_minecraft_scoreboard_ScoreboardObjective = TypeVar("net_minecraft_scoreboard_ScoreboardObjective")
+ScoreboardObjective = net_minecraft_scoreboard_ScoreboardObjective
+
 
 class ScoreboardObjectiveHelper(BaseHelper):
 	"""
 	Since: 1.2.9 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScoreboardsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScoreboardsHelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .ScoreboardObjectiveHelper import ScoreboardObjectiveHelper
 from .PlayerEntityHelper import PlayerEntityHelper
 from .FormattingHelper import FormattingHelper
 from .TeamHelper import TeamHelper
 
-Scoreboard = TypeVar["net.minecraft.scoreboard.Scoreboard"]
+net_minecraft_scoreboard_Scoreboard = TypeVar("net_minecraft_scoreboard_Scoreboard")
+Scoreboard = net_minecraft_scoreboard_Scoreboard
+
 
 class ScoreboardsHelper(BaseHelper):
 	"""
 	Since: 1.2.9 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptCodeCompiler.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/NoStyleCodeCompiler.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .AbstractRenderCodeCompiler import AbstractRenderCodeCompiler
 from .EditorScreen import EditorScreen
 from .AutoCompleteSuggestion import AutoCompleteSuggestion
 
-Runnable = TypeVar["java.lang.Runnable"]
-Text = TypeVar["net.minecraft.text.Text"]
-File = TypeVar["java.io.File"]
-
-class ScriptCodeCompiler(AbstractRenderCodeCompiler):
-	"""
-	"""
+java_lang_Runnable = TypeVar("java_lang_Runnable")
+Runnable = java_lang_Runnable
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+
+class NoStyleCodeCompiler(AbstractRenderCodeCompiler):
 
 	@overload
-	def __init__(self, language: str, screen: EditorScreen, scriptFile: File) -> None:
+	def __init__(self, language: str, screen: EditorScreen) -> None:
 		pass
 
 	@overload
 	def recompileRenderedText(self, text: str) -> None:
 		pass
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptScreen.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextInput.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from typing import overload
 from typing import TypeVar
-from .BaseScreen import BaseScreen
-from .IScreen import IScreen
-from .MethodWrapper import MethodWrapper
+from .Button import Button
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
+java_util_function_Consumer_java_lang_String_ = TypeVar("java_util_function_Consumer_java_lang_String_")
+Consumer = java_util_function_Consumer_java_lang_String_
 
-class ScriptScreen(BaseScreen):
-	"""just go look at IScreen since all the methods are done through a mixin...\n
-	Since: 1.0.5 
-	"""
-	drawTitle: bool
-	shouldCloseOnEsc: bool
-	shouldPause: bool
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
+
+class TextInput(Button):
+	onChange: Consumer
+	mask: str
+	content: str
+	selStartIndex: int
+	selEndIndex: int
+
+	@overload
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: str, onClick: Consumer, onChange: Consumer) -> None:
+		pass
+
+	@overload
+	def setMessage(self, message: str) -> None:
+		pass
 
 	@overload
-	def __init__(self, title: str, dirt: bool) -> None:
+	def updateSelStart(self, startIndex: int) -> None:
 		pass
 
 	@overload
-	def setParent(self, parent: IScreen) -> None:
-		"""
-		Since: 1.4.0 
+	def updateSelEnd(self, endIndex: int) -> None:
+		pass
 
-		Args:
-			parent: parent screen to go to when this one exits. 
-		"""
+	@overload
+	def mouseClicked(self, mouseX: float, mouseY: float, button: int) -> bool:
 		pass
 
 	@overload
-	def setOnRender(self, onRender: MethodWrapper) -> None:
-		"""add custom stuff to the render function on the main thread.\n
-		Since: 1.4.0 
+	def mouseDragged(self, mouseX: float, mouseY: float, button: int, deltaX: float, deltaY: float) -> bool:
+		pass
 
-		Args:
-			onRender: pos3d elements are mousex, mousey, tickDelta 
-		"""
+	@overload
+	def swapStartEnd(self) -> None:
 		pass
 
 	@overload
-	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
-	def close(self) -> None:
+	def charTyped(self, chr: str, keyCode: int) -> bool:
 		pass
 
 	@overload
-	def shouldPause(self) -> bool:
+	def clicked(self, mouseX: float, mouseY: float) -> bool:
 		pass
 
 	@overload
-	def shouldCloseOnEsc(self) -> bool:
+	def setSelected(self, sel: bool) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ScriptTrigger.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ScriptTrigger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .ScriptTrigger_TriggerType import ScriptTrigger_TriggerType
 
-File = TypeVar["java.io.File"]
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
 
 class ScriptTrigger:
 	triggerType: ScriptTrigger_TriggerType
 	event: str
 	scriptFile: str
 	enabled: bool
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Scrollbar.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Scrollbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import overload
 from typing import TypeVar
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.Double_"]
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-ClickableWidget = TypeVar["net.minecraft.client.gui.widget.ClickableWidget"]
+java_util_function_Consumer_java_lang_Double_ = TypeVar("java_util_function_Consumer_java_lang_Double_")
+Consumer = java_util_function_Consumer_java_lang_Double_
+
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_gui_widget_ClickableWidget = TypeVar("net_minecraft_client_gui_widget_ClickableWidget")
+ClickableWidget = net_minecraft_client_gui_widget_ClickableWidget
+
 
 class Scrollbar(ClickableWidget):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, height: int, color: int, borderColor: int, highlightColor: int, scrollPages: float, onChange: Consumer) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServerInfoHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServerInfoHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 from .NBTElementHelper import NBTElementHelper
 
-ServerInfo = TypeVar["net.minecraft.client.network.ServerInfo"]
+net_minecraft_client_network_ServerInfo = TypeVar("net_minecraft_client_network_ServerInfo")
+ServerInfo = net_minecraft_client_network_ServerInfo
+
 
 class ServerInfoHelper(BaseHelper):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceContainer.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SelectorDropdownOverlay.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .MultiElementContainer import MultiElementContainer
-from .ServiceScreen import ServiceScreen
-from .ServiceTrigger import ServiceTrigger
+from .OverlayContainer import OverlayContainer
+from .IOverlayParent import IOverlayParent
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-File = TypeVar["java.io.File"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Consumer_java_lang_Integer_ = TypeVar("java_util_function_Consumer_java_lang_Integer_")
+Consumer = java_util_function_Consumer_java_lang_Integer_
 
-class ServiceContainer(MultiElementContainer):
-	service: str
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: ServiceScreen, service: str) -> None:
-		pass
+
+class SelectorDropdownOverlay(OverlayContainer):
 
 	@overload
-	def init(self) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, choices: List[Text], textRenderer: TextRenderer, parent: IOverlayParent, onChoice: Consumer) -> None:
 		pass
 
 	@overload
-	def getEnabled(self) -> bool:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def getRunning(self) -> bool:
+	def onScroll(self, page: float) -> None:
 		pass
 
 	@overload
-	def getTrigger(self) -> ServiceTrigger:
+	def onClick(self, mouseX: float, mouseY: float, button: int) -> None:
 		pass
 
 	@overload
-	def setFile(self, file: File) -> None:
+	def setSelected(self, sel: int) -> None:
 		pass
 
 	@overload
-	def setPos(self, x: int, y: int, width: int, height: int) -> None:
+	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
 	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ServiceManager.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ServiceManager.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SettingsOverlay.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextOverlay.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,33 @@
 from typing import overload
-from typing import List
 from typing import TypeVar
-from .ICategoryTreeParent import ICategoryTreeParent
 from .OverlayContainer import OverlayContainer
 from .IOverlayParent import IOverlayParent
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class SettingsOverlay(ICategoryTreeParent, OverlayContainer):
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
 
-	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent) -> None:
-		pass
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
 
-	@overload
-	def init(self) -> None:
-		pass
 
-	@overload
-	def clearCategory(self) -> None:
-		pass
+class TextOverlay(OverlayContainer):
+	centered: bool
 
 	@overload
-	def selectCategory(self, category: List[str]) -> None:
+	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, parent: IOverlayParent, text: Text) -> None:
 		pass
 
 	@overload
-	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
-		pass
-
-	@overload
-	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def onClose(self) -> None:
+	def render(self, drawContext: DrawContext, mouseX: int, mouseY: int, delta: float) -> None:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SettingsOverlay_SettingField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringifyFilter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Generic
-from .Option import Option
+from .BasicFilter import BasicFilter
 
-Field = TypeVar["java.lang.reflect.Field"]
 T = TypeVar("T")
-Method = TypeVar["java.lang.reflect.Method"]
 
-class SettingsOverlay_SettingField(Generic[T]):
-	type: Class
-	option: Option
+class StringifyFilter(Generic[T], BasicFilter):
+	"""
+	Since: 1.6.5 
+	"""
 
 	@overload
-	def __init__(self, option: Option, containingClass: object, f: Field, getter: Method, setter: Method, type: Class) -> None:
+	def __init__(self, operation: str) -> None:
 		pass
 
 	@overload
-	def set(self, o: T) -> None:
+	def addOption(self, toAdd: str) -> "StringifyFilter":
 		pass
 
 	@overload
-	def get(self) -> T:
+	def addOption(self, toAdd: List[str]) -> "StringifyFilter":
 		pass
 
 	@overload
-	def hasOptions(self) -> bool:
+	def removeOption(self, toRemove: str) -> "StringifyFilter":
 		pass
 
 	@overload
-	def getOptions(self) -> List[T]:
+	def removeOption(self, toRemove: List[str]) -> "StringifyFilter":
 		pass
 
 	@overload
-	def isSimple(self) -> bool:
+	def apply(self, obj: object) -> bool:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SheepEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/CatEntityHelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 from typing import overload
 from typing import TypeVar
-from .AnimalEntityHelper import AnimalEntityHelper
+from .TameableEntityHelper import TameableEntityHelper
 from .DyeColorHelper import DyeColorHelper
 
-SheepEntity = TypeVar["net.minecraft.entity.passive.SheepEntity"]
+net_minecraft_entity_passive_CatEntity = TypeVar("net_minecraft_entity_passive_CatEntity")
+CatEntity = net_minecraft_entity_passive_CatEntity
 
-class SheepEntityHelper(AnimalEntityHelper):
+
+class CatEntityHelper(TameableEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: SheepEntity) -> None:
+	def __init__(self, base: CatEntity) -> None:
 		pass
 
 	@overload
-	def isSheared(self) -> bool:
+	def isSleeping(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this sheep is sheared, 'false' otherwise. 
+			'true' if this cat is sleeping, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isShearable(self) -> bool:
+	def getCollarColor(self) -> DyeColorHelper:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this sheep can be sheared, 'false' otherwise. 
+			the color of this cat's collar. 
 		"""
 		pass
 
 	@overload
-	def getColor(self) -> DyeColorHelper:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the color of this sheep. 
+	def getVariant(self) -> str:
 		"""
-		pass
-
-	@overload
-	def isJeb(self) -> bool:
-		"""Sheep named 'jeb_' will cycle through all colors when rendered. If sheared, they will
-drop their original colored wool.\n
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the sheep has a rainbow overlay, 'false' otherwise. 
+			the variant of this cat. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ShulkerEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ShulkerEntityHelper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 from .DirectionHelper import DirectionHelper
 from .DyeColorHelper import DyeColorHelper
 
-ShulkerEntity = TypeVar["net.minecraft.entity.mob.ShulkerEntity"]
+net_minecraft_entity_mob_ShulkerEntity = TypeVar("net_minecraft_entity_mob_ShulkerEntity")
+ShulkerEntity = net_minecraft_entity_mob_ShulkerEntity
+
 
 class ShulkerEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SliderWidgetHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SliderWidgetHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SliderWidgetHelper_SliderBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SliderWidgetHelper_SliderBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SlimeEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SnowGolemEntityHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 
-SlimeEntity = TypeVar["net.minecraft.entity.mob.SlimeEntity"]
+net_minecraft_entity_passive_SnowGolemEntity = TypeVar("net_minecraft_entity_passive_SnowGolemEntity")
+SnowGolemEntity = net_minecraft_entity_passive_SnowGolemEntity
 
-class SlimeEntityHelper(MobEntityHelper):
+
+class SnowGolemEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: SlimeEntity) -> None:
+	def __init__(self, base: SnowGolemEntity) -> None:
 		pass
 
 	@overload
-	def getSize(self) -> int:
+	def hasPumpkin(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the size of this slime. 
+			'true' if the snow golem has a pumpkin on its head, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isSmall(self) -> bool:
-		"""Small slimes, with a size less than 1, don't attack the player.\n
+	def isShearable(self) -> bool:
+		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this slime is small, 'false' otherwise. 
+			'true' if this snow golem can be sheared, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SmithingInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LockButtonWidgetHelper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from typing import overload
 from typing import TypeVar
-from .Inventory import Inventory
-from .ItemStackHelper import ItemStackHelper
+from .ClickableWidgetHelper import ClickableWidgetHelper
 
-SmithingScreen = TypeVar["net.minecraft.client.gui.screen.ingame.SmithingScreen"]
+net_minecraft_client_gui_widget_LockButtonWidget = TypeVar("net_minecraft_client_gui_widget_LockButtonWidget")
+LockButtonWidget = net_minecraft_client_gui_widget_LockButtonWidget
 
-class SmithingInventory(Inventory):
+
+class LockButtonWidgetHelper(ClickableWidgetHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, inventory: SmithingScreen) -> None:
+	def __init__(self, btn: LockButtonWidget) -> None:
 		pass
 
 	@overload
-	def getLeftInput(self) -> ItemStackHelper:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the left input item. 
-		"""
+	def __init__(self, btn: LockButtonWidget, zIndex: int) -> None:
 		pass
 
 	@overload
-	def getRightInput(self) -> ItemStackHelper:
+	def isLocked(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the right input item. 
+			'true' if the button is locked, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getOutput(self) -> ItemStackHelper:
+	def setLocked(self, locked: bool) -> "LockButtonWidgetHelper":
 		"""
 		Since: 1.8.4 
 
+		Args:
+			locked: whether to lock the button or not 
+
 		Returns:
-			the expected output item. 
+			self for chaining. 
 		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SnowGolemEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/IronGolemEntityHelper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 
-SnowGolemEntity = TypeVar["net.minecraft.entity.passive.SnowGolemEntity"]
+net_minecraft_entity_passive_IronGolemEntity = TypeVar("net_minecraft_entity_passive_IronGolemEntity")
+IronGolemEntity = net_minecraft_entity_passive_IronGolemEntity
 
-class SnowGolemEntityHelper(MobEntityHelper):
+
+class IronGolemEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: SnowGolemEntity) -> None:
-		pass
-
-	@overload
-	def hasPumpkin(self) -> bool:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			'true' if the snow golem has a pumpkin on its head, 'false' otherwise. 
-		"""
+	def __init__(self, base: IronGolemEntity) -> None:
 		pass
 
 	@overload
-	def isShearable(self) -> bool:
+	def isPlayerCreated(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this snow golem can be sheared, 'false' otherwise. 
+			'true' if this iron golem was created by a player, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SpellcastingIllagerEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SpellcastingIllagerEntityHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StateHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StateHelper.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StatsHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StatsHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .BaseHelper import BaseHelper
 
-StatHandler = TypeVar["net.minecraft.stat.StatHandler"]
-Text = TypeVar["net.minecraft.text.Text"]
+net_minecraft_stat_StatHandler = TypeVar("net_minecraft_stat_StatHandler")
+StatHandler = net_minecraft_stat_StatHandler
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
 
 class StatsHelper(BaseHelper):
 
 	@overload
 	def __init__(self, base: StatHandler) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StatusEffectHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StatusEffectHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 
-StatusEffect = TypeVar["net.minecraft.entity.effect.StatusEffect"]
-StatusEffectInstance = TypeVar["net.minecraft.entity.effect.StatusEffectInstance"]
+net_minecraft_entity_effect_StatusEffect = TypeVar("net_minecraft_entity_effect_StatusEffect")
+StatusEffect = net_minecraft_entity_effect_StatusEffect
+
+net_minecraft_entity_effect_StatusEffectInstance = TypeVar("net_minecraft_entity_effect_StatusEffectInstance")
+StatusEffectInstance = net_minecraft_entity_effect_StatusEffectInstance
+
 
 class StatusEffectHelper(BaseHelper):
 	"""
 	Since: 1.2.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StoneCutterInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StoneCutterInventory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .Inventory import Inventory
 from .ItemStackHelper import ItemStackHelper
 
-StonecutterScreen = TypeVar["net.minecraft.client.gui.screen.ingame.StonecutterScreen"]
+net_minecraft_client_gui_screen_ingame_StonecutterScreen = TypeVar("net_minecraft_client_gui_screen_ingame_StonecutterScreen")
+StonecutterScreen = net_minecraft_client_gui_screen_ingame_StonecutterScreen
+
 
 class StoneCutterInventory(Inventory):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StriderEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BatEntityHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 from typing import overload
 from typing import TypeVar
-from .AnimalEntityHelper import AnimalEntityHelper
+from .MobEntityHelper import MobEntityHelper
 
-StriderEntity = TypeVar["net.minecraft.entity.passive.StriderEntity"]
+net_minecraft_entity_passive_BatEntity = TypeVar("net_minecraft_entity_passive_BatEntity")
+BatEntity = net_minecraft_entity_passive_BatEntity
 
-class StriderEntityHelper(AnimalEntityHelper):
+
+class BatEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: StriderEntity) -> None:
-		pass
-
-	@overload
-	def isSaddled(self) -> bool:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			'true' if this strider is saddled, 'false' otherwise. 
-		"""
+	def __init__(self, base: BatEntity) -> None:
 		pass
 
 	@overload
-	def isShivering(self) -> bool:
+	def isResting(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this strider is shivering in the cold, 'false' otherwise. 
+			'true' if the bat is hanging upside down, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringCompareFilter_FilterMethod.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringCompareFilter_FilterMethod.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringField.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/LongField.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractSettingField import AbstractSettingField
 from .AbstractSettingContainer import AbstractSettingContainer
 from .SettingsOverlay_SettingField import SettingsOverlay_SettingField
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
 
-class StringField(AbstractSettingField):
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
+
+class LongField(AbstractSettingField):
 
 	@overload
 	def __init__(self, x: int, y: int, width: int, textRenderer: TextRenderer, parent: AbstractSettingContainer, field: SettingsOverlay_SettingField) -> None:
 		pass
 
 	@overload
 	def init(self) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringHashTrie.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/StringHashTrie.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StringifyFilter.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WrappedClassInstance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Generic
-from .BasicFilter import BasicFilter
 
 T = TypeVar("T")
 
-class StringifyFilter(Generic[T], BasicFilter):
+class WrappedClassInstance(Generic[T]):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
-	def __init__(self, operation: str) -> None:
+	def __init__(self, instance: T) -> None:
 		pass
 
 	@overload
-	def addOption(self, toAdd: str) -> "StringifyFilter":
+	def __init__(self, instanceNullable: T, tClass: Class) -> None:
 		pass
 
 	@overload
-	def addOption(self, toAdd: List[str]) -> "StringifyFilter":
+	def getFieldValue(self, fieldName: str) -> object:
 		pass
 
 	@overload
-	def removeOption(self, toRemove: str) -> "StringifyFilter":
+	def getFieldValueAsClass(self, asClass: str, fieldName: str) -> object:
 		pass
 
 	@overload
-	def removeOption(self, toRemove: List[str]) -> "StringifyFilter":
+	def setFieldValue(self, fieldName: str, fieldValue: object) -> None:
 		pass
 
 	@overload
-	def apply(self, obj: object) -> bool:
+	def setFieldValueAsClass(self, asClass: str, fieldName: str, fieldValue: object) -> None:
+		pass
+
+	@overload
+	def invokeMethod(self, methodNameOrSig: str, params: List[object]) -> object:
+		pass
+
+	@overload
+	def invokeMethodAsClass(self, asClass: str, methodNameOrSig: str, params: List[object]) -> object:
+		pass
+
+	@overload
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

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/StyleHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Vec2D.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,141 @@
 from typing import overload
-from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .FormattingHelper import FormattingHelper
+from .Pos2D import Pos2D
+from .Vec3D import Vec3D
 
-Runnable = TypeVar["java.lang.Runnable"]
-Style = TypeVar["net.minecraft.text.Style"]
 
-class StyleHelper(BaseHelper):
+class Vec2D:
 	"""
-	Since: 1.6.5 
+	Since: 1.2.6 [citation needed] 
 	"""
+	x1: float
+	y1: float
+	x2: float
+	y2: float
 
 	@overload
-	def __init__(self, base: Style) -> None:
+	def __init__(self, x1: float, y1: float, x2: float, y2: float) -> None:
 		pass
 
 	@overload
-	def hasColor(self) -> bool:
+	def __init__(self, start: Pos2D, end: Pos2D) -> None:
 		pass
 
 	@overload
-	def getColor(self) -> int:
-		"""
-
-		Returns:
-			the color index of this style or '-1' if no color is set. 
-		"""
+	def getX1(self) -> float:
 		pass
 
 	@overload
-	def getFormatting(self) -> FormattingHelper:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the formatting of this style, or 'null' if no formatting was found. 
-		"""
+	def getY1(self) -> float:
 		pass
 
 	@overload
-	def getColorIndex(self) -> int:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the color index of this style or '-1' if no color is set. 
-		"""
+	def getX2(self) -> float:
 		pass
 
 	@overload
-	def getColorValue(self) -> int:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the color value of this style or '-1' if it doesn't have one. 
-		"""
+	def getY2(self) -> float:
 		pass
 
 	@overload
-	def getColorName(self) -> str:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the color name of this style or 'null' if it has no color. 
-		"""
+	def getDeltaX(self) -> float:
 		pass
 
 	@overload
-	def hasCustomColor(self) -> bool:
+	def getDeltaY(self) -> float:
 		pass
 
 	@overload
-	def getCustomColor(self) -> int:
+	def getStart(self) -> Pos2D:
 		pass
 
 	@overload
-	def bold(self) -> bool:
+	def getEnd(self) -> Pos2D:
 		pass
 
 	@overload
-	def italic(self) -> bool:
+	def getMagnitude(self) -> float:
 		pass
 
 	@overload
-	def underlined(self) -> bool:
+	def getMagnitudeSq(self) -> float:
+		"""
+		Since: 1.6.5 
+
+		Returns:
+			magnitude squared 
+		"""
 		pass
 
 	@overload
-	def strikethrough(self) -> bool:
+	def add(self, vec: "Vec2D") -> "Vec2D":
 		pass
 
 	@overload
-	def obfuscated(self) -> bool:
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
 		pass
 
 	@overload
-	def getClickAction(self) -> str:
+	def multiply(self, vec: "Vec2D") -> "Vec2D":
 		pass
 
 	@overload
-	def getClickValue(self) -> str:
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
 		pass
 
 	@overload
-	def getCustomClickValue(self) -> Runnable:
+	def scale(self, scale: float) -> "Vec2D":
+		"""
+		Since: 1.6.3 
+
+		Args:
+			scale: 
+		"""
 		pass
 
 	@overload
-	def getHoverAction(self) -> str:
+	def dotProduct(self, vec: "Vec2D") -> float:
 		pass
 
 	@overload
-	def getHoverValue(self) -> object:
+	def reverse(self) -> "Vec2D":
 		pass
 
 	@overload
-	def getInsertion(self) -> str:
+	def normalize(self) -> "Vec2D":
+		"""
+		Since: 1.6.5 
+
+		Returns:
+			a new Vec2D with the same direction but a magnitude of 1 
+		"""
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
+	@overload
+	def to3D(self) -> Vec3D:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SuggestionsBuilderHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/SuggestionsBuilderHelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .TextHelper import TextHelper
 from .BlockPosHelper import BlockPosHelper
 
-SuggestionsBuilder = TypeVar["com.mojang.brigadier.suggestion.SuggestionsBuilder"]
+com_mojang_brigadier_suggestion_SuggestionsBuilder = TypeVar("com_mojang_brigadier_suggestion_SuggestionsBuilder")
+SuggestionsBuilder = com_mojang_brigadier_suggestion_SuggestionsBuilder
+
 
 class SuggestionsBuilderHelper(BaseHelper):
 	"""
 	Since: 1.6.5 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Surface.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Surface.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 from .RenderElement3D import RenderElement3D
 from .Draw2D import Draw2D
 from .EntityHelper import EntityHelper
 from .Pos3D import Pos3D
 from .Pos2D import Pos2D
 from .BlockPosHelper import BlockPosHelper
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-BufferBuilder = TypeVar["net.minecraft.client.render.BufferBuilder"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_client_render_BufferBuilder = TypeVar("net_minecraft_client_render_BufferBuilder")
+BufferBuilder = net_minecraft_client_render_BufferBuilder
+
 
 class Surface(RenderElement, RenderElement3D, Draw2D):
 	"""
 	Since: 1.6.5 
 	"""
 	rotateToPlayer: bool
 	rotateCenter: bool
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Surface_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Surface_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/SynchronizedWeakHashSet.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/KeyMacrosScreen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,29 @@
 from typing import overload
 from typing import TypeVar
-from typing import Generic
+from .MacroScreen import MacroScreen
 
-Serializable = TypeVar["java.io.Serializable"]
-E = TypeVar("E")
-AbstractSet = TypeVar["java.util.AbstractSet_E_"]
+net_minecraft_client_gui_screen_Screen = TypeVar("net_minecraft_client_gui_screen_Screen")
+Screen = net_minecraft_client_gui_screen_Screen
 
-class SynchronizedWeakHashSet(Serializable, Generic[E], AbstractSet):
 
-	@overload
-	def __init__(self) -> None:
-		pass
-
-	@overload
-	def size(self) -> int:
-		pass
-
-	@overload
-	def contains(self, o: object) -> bool:
-		pass
+class KeyMacrosScreen(MacroScreen):
 
 	@overload
-	def add(self, o: E) -> bool:
+	def __init__(self, parent: Screen) -> None:
 		pass
 
 	@overload
-	def remove(self, o: object) -> bool:
+	def init(self) -> None:
 		pass
 
 	@overload
-	def clear(self) -> None:
+	def keyReleased(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
 		pass
 
 	@overload
-	def iterator(self) -> iter:
+	def mouseReleased(self, mouseX: float, mouseY: float, button: int) -> bool:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TameableEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WardenEntityHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,80 @@
 from typing import overload
 from typing import TypeVar
-from typing import Generic
-from .AnimalEntityHelper import AnimalEntityHelper
-from .LivingEntityHelper import LivingEntityHelper
+from .MobEntityHelper import MobEntityHelper
 
-T = TypeVar("T")
+net_minecraft_entity_mob_WardenEntity = TypeVar("net_minecraft_entity_mob_WardenEntity")
+WardenEntity = net_minecraft_entity_mob_WardenEntity
 
-class TameableEntityHelper(Generic[T], AnimalEntityHelper):
+
+class WardenEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: T) -> None:
+	def __init__(self, base: WardenEntity) -> None:
+		pass
+
+	@overload
+	def getAnger(self) -> int:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			this warden's anger towards its active target. 
+		"""
 		pass
 
 	@overload
-	def isTamed(self) -> bool:
+	def isDigging(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the entity is tamed, 'false' otherwise. 
+			'true' if this warden is digging into the ground, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isSitting(self) -> bool:
+	def isEmerging(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if the entity is sitting, 'false' otherwise. 
+			'true' if this warden is emerging from the ground, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getOwner(self) -> str:
+	def isRoaring(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the owner's uuid, or 'null' if the entity is not tamed. 
+			'true' if this warden is roaring, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def isOwner(self, owner: LivingEntityHelper) -> bool:
+	def isSniffing(self) -> bool:
 		"""
 		Since: 1.8.4 
 
-		Args:
-			owner: the possible owner 
+		Returns:
+			'true' if this warden is sniffing, 'false' otherwise. 
+		"""
+		pass
+
+	@overload
+	def isChargingSonicBoom(self) -> bool:
+		"""
+		Since: 1.8.4 
 
 		Returns:
-			'true' if the entity is tamed by the given owner, 'false' otherwise. 
+			'true' if this warden is charging its sonic boom attack, 'false' otherwise. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TeamHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/FileHandler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,151 +1,120 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
-from .BaseHelper import BaseHelper
-from .TextHelper import TextHelper
-from .FormattingHelper import FormattingHelper
-from .ScoreboardsHelper import ScoreboardsHelper
+from .FileHandler_FileLineIterator import FileHandler_FileLineIterator
 
-Team = TypeVar["net.minecraft.scoreboard.Team"]
+java_io_BufferedInputStream = TypeVar("java_io_BufferedInputStream")
+BufferedInputStream = java_io_BufferedInputStream
 
-class TeamHelper(BaseHelper):
+java_io_File = TypeVar("java_io_File")
+File = java_io_File
+
+
+class FileHandler:
 	"""
-	Since: 1.3.0 
+	Since: 1.1.8 
 	"""
 
 	@overload
-	def __init__(self, t: Team) -> None:
+	def __init__(self, path: str) -> None:
 		pass
 
 	@overload
-	def getName(self) -> str:
-		"""
-		Since: 1.3.0 
-		"""
+	def __init__(self, path: str, charset: str) -> None:
 		pass
 
 	@overload
-	def getDisplayName(self) -> TextHelper:
-		"""
-		Since: 1.3.0 
-		"""
+	def __init__(self, path: File, charset: str) -> None:
 		pass
 
 	@overload
-	def getPlayerList(self) -> List[str]:
-		"""
-		Since: 1.3.0 
-		"""
+	def __init__(self, path: str, charset: Charset) -> None:
 		pass
 
 	@overload
-	def getColorFormat(self) -> FormattingHelper:
-		"""
-		Since: 1.8.4 
-
-		Returns:
-			the formatting of this team's color. 
-		"""
+	def __init__(self, path: File) -> None:
 		pass
 
 	@overload
-	def getColor(self) -> int:
-		"""
-		Since: 1.3.0 
-		"""
+	def __init__(self, path: File, charset: Charset) -> None:
 		pass
 
 	@overload
-	def getColorIndex(self) -> int:
-		"""
-		Since: 1.8.4 
+	def write(self, s: str) -> "FileHandler":
+		"""writes a string to the file. this is a destructive operation that replaces the file contents.\n
+		Since: 1.1.8 
 
-		Returns:
-			the color index of this team. 
+		Args:
+			s: 
 		"""
 		pass
 
 	@overload
-	def getColorValue(self) -> int:
-		"""
-		Since: 1.8.4 
+	def write(self, b: List[float]) -> "FileHandler":
+		"""writes a byte array to the file. this is a destructive operation that replaces the file contents.\n
+		Since: 1.1.8 
 
-		Returns:
-			the color value for this team or '-1' if it has no color. 
+		Args:
+			b: 
 		"""
 		pass
 
 	@overload
-	def getColorName(self) -> str:
+	def read(self) -> str:
 		"""
-		Since: 1.8.4 
-
-		Returns:
-			the name of this team's color. 
+		Since: 1.1.8 
 		"""
 		pass
 
 	@overload
-	def getScoreboard(self) -> ScoreboardsHelper:
+	def readBytes(self) -> List[float]:
 		"""
-		Since: 1.8.4 
-
-		Returns:
-			the scoreboard including this team. 
+		Since: 1.2.6 
 		"""
 		pass
 
 	@overload
-	def getPrefix(self) -> TextHelper:
-		"""
-		Since: 1.3.0 
+	def readLines(self) -> FileHandler_FileLineIterator:
+		"""get an iterator for the lines in the file.
+please call FileHandler_FileLineIterator#close() when you are done with the iterator to not leak resources.\n
+		Since: 1.8.4 
 		"""
 		pass
 
 	@overload
-	def getSuffix(self) -> TextHelper:
-		"""
-		Since: 1.3.0 
+	def streamBytes(self) -> BufferedInputStream:
+		"""get an input stream for the file.
+please call BufferedInputStream#close() when you are done with the stream to not leak resources.\n
+		Since: 1.8.4 
 		"""
 		pass
 
 	@overload
-	def getCollisionRule(self) -> str:
-		"""
-		Since: 1.3.0 
+	def append(self, s: str) -> "FileHandler":
 		"""
-		pass
+		Since: 1.1.8 
 
-	@overload
-	def isFriendlyFire(self) -> bool:
-		"""
-		Since: 1.3.0 
+		Args:
+			s: 
 		"""
 		pass
 
 	@overload
-	def showFriendlyInvisibles(self) -> bool:
+	def append(self, b: List[float]) -> "FileHandler":
 		"""
-		Since: 1.3.0 
-		"""
-		pass
+		Since: 1.2.6 
 
-	@overload
-	def nametagVisibility(self) -> str:
-		"""
-		Since: 1.3.0 
+		Args:
+			b: 
 		"""
 		pass
 
 	@overload
-	def deathMessageVisibility(self) -> str:
-		"""
-		Since: 1.3.0 
-		"""
+	def getFile(self) -> File:
 		pass
 
 	@overload
 	def toString(self) -> str:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Text.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import TypeVar
 from .RenderElement import RenderElement
 from .Alignable import Alignable
 from .IDraw2D import IDraw2D
 from .TextHelper import TextHelper
 
-DrawContext = TypeVar["net.minecraft.client.gui.DrawContext"]
-Text = TypeVar["net.minecraft.text.Text"]
+net_minecraft_client_gui_DrawContext = TypeVar("net_minecraft_client_gui_DrawContext")
+DrawContext = net_minecraft_client_gui_DrawContext
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
 
 class Text(RenderElement, Alignable):
 	"""
 	Since: 1.0.5 
 	"""
 	parent: IDraw2D
 	text: Text
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextFieldWidgetHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextFieldWidgetHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .ClickableWidgetHelper import ClickableWidgetHelper
 from .MethodWrapper import MethodWrapper
 
-TextFieldWidget = TypeVar["net.minecraft.client.gui.widget.TextFieldWidget"]
+net_minecraft_client_gui_widget_TextFieldWidget = TypeVar("net_minecraft_client_gui_widget_TextFieldWidget")
+TextFieldWidget = net_minecraft_client_gui_widget_TextFieldWidget
+
 
 class TextFieldWidgetHelper(ClickableWidgetHelper):
 	"""
 	Since: 1.0.5 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextFieldWidgetHelper_TextFieldBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextFieldWidgetHelper_TextFieldBuilder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import overload
 from typing import TypeVar
 from .AbstractWidgetBuilder import AbstractWidgetBuilder
 from .IScreen import IScreen
 from .MethodWrapper import MethodWrapper
 from .TextFieldWidgetHelper import TextFieldWidgetHelper
 
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+net_minecraft_client_font_TextRenderer = TypeVar("net_minecraft_client_font_TextRenderer")
+TextRenderer = net_minecraft_client_font_TextRenderer
+
 
 class TextFieldWidgetHelper_TextFieldBuilder(AbstractWidgetBuilder):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TextHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import overload
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .MethodWrapper import MethodWrapper
 
-Pattern = TypeVar["java.util.regex.Pattern"]
-Text = TypeVar["net.minecraft.text.Text"]
+java_util_regex_Pattern = TypeVar("java_util_regex_Pattern")
+Pattern = java_util_regex_Pattern
+
+net_minecraft_text_Text = TypeVar("net_minecraft_text_Text")
+Text = net_minecraft_text_Text
+
 
 class TextHelper(BaseHelper):
 	"""
 	Since: 1.0.8 
 	"""
 	STRIP_FORMATTING_PATTERN: Pattern
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TextInput.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/PrioryFiFoTaskQueue.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,114 @@
 from typing import overload
+from typing import List
 from typing import TypeVar
-from .Button import Button
+from typing import Any
+from typing import Generic
 
-Consumer = TypeVar["java.util.function.Consumer_java.lang.String_"]
-TextRenderer = TypeVar["net.minecraft.client.font.TextRenderer"]
+java_util_function_Function_E,java_lang_Integer_ = TypeVar("java_util_function_Function_E,java_lang_Integer_")
+Function = java_util_function_Function_E,java_lang_Integer_
 
-class TextInput(Button):
-	onChange: Consumer
-	mask: str
-	content: str
-	selStartIndex: int
-	selEndIndex: int
+T = TypeVar("T")
+E = TypeVar("E")
+E = E
+
+java_util_Queue_E_ = TypeVar("java_util_Queue_E_")
+Queue = java_util_Queue_E_
+
+
+class PrioryFiFoTaskQueue(Queue, Generic[E]):
+
+	@overload
+	def __init__(self, priorityFunction: Function) -> None:
+		pass
+
+	@overload
+	def size(self) -> int:
+		pass
+
+	@overload
+	def isEmpty(self) -> bool:
+		pass
+
+	@overload
+	def contains(self, o: object) -> bool:
+		pass
+
+	@overload
+	def iterator(self) -> iter:
+		pass
+
+	@overload
+	def toArray(self) -> List[object]:
+		pass
+
+	@overload
+	def toArray(self, ts: List[T]) -> List[T]:
+		pass
+
+	@overload
+	def add(self, e: E) -> bool:
+		pass
+
+	@overload
+	def remove(self, o: object) -> bool:
+		pass
+
+	@overload
+	def containsAll(self, collection: List[Any]) -> bool:
+		pass
+
+	@overload
+	def addAll(self, collection: List[Any]) -> bool:
+		pass
+
+	@overload
+	def removeAll(self, collection: List[Any]) -> bool:
+		pass
 
 	@overload
-	def __init__(self, x: int, y: int, width: int, height: int, textRenderer: TextRenderer, color: int, borderColor: int, highlightColor: int, textColor: int, message: str, onClick: Consumer, onChange: Consumer) -> None:
+	def retainAll(self, collection: List[Any]) -> bool:
 		pass
 
 	@overload
-	def setMessage(self, message: str) -> None:
+	def clear(self) -> None:
 		pass
 
 	@overload
-	def updateSelStart(self, startIndex: int) -> None:
+	def offer(self, e: E) -> bool:
 		pass
 
 	@overload
-	def updateSelEnd(self, endIndex: int) -> None:
+	def remove(self) -> E:
 		pass
 
 	@overload
-	def mouseClicked(self, mouseX: float, mouseY: float, button: int) -> bool:
+	def poll(self) -> E:
 		pass
 
 	@overload
-	def mouseDragged(self, mouseX: float, mouseY: float, button: int, deltaX: float, deltaY: float) -> bool:
+	def pollWaiting(self) -> E:
 		pass
 
 	@overload
-	def swapStartEnd(self) -> None:
+	def pollWaiting(self, timeout: float) -> E:
 		pass
 
 	@overload
-	def keyPressed(self, keyCode: int, scanCode: int, modifiers: int) -> bool:
+	def peekWaiting(self) -> E:
 		pass
 
 	@overload
-	def charTyped(self, chr: str, keyCode: int) -> bool:
+	def peekWaiting(self, timeout: float) -> E:
 		pass
 
 	@overload
-	def clicked(self, mouseX: float, mouseY: float) -> bool:
+	def element(self) -> E:
 		pass
 
 	@overload
-	def setSelected(self, sel: bool) -> None:
+	def peek(self) -> E:
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Text_Builder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Text_Builder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TntMinecartEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TntMinecartEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 
-TntMinecartEntity = TypeVar["net.minecraft.entity.vehicle.TntMinecartEntity"]
+net_minecraft_entity_vehicle_TntMinecartEntity = TypeVar("net_minecraft_entity_vehicle_TntMinecartEntity")
+TntMinecartEntity = net_minecraft_entity_vehicle_TntMinecartEntity
+
 
 class TntMinecartEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TradeOfferHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TradeOfferHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List
 from typing import TypeVar
 from .BaseHelper import BaseHelper
 from .VillagerInventory import VillagerInventory
 from .ItemStackHelper import ItemStackHelper
 from .NBTElementHelper import NBTElementHelper
 
-TradeOffer = TypeVar["net.minecraft.village.TradeOffer"]
+net_minecraft_village_TradeOffer = TypeVar("net_minecraft_village_TradeOffer")
+TradeOffer = net_minecraft_village_TradeOffer
+
 
 class TradeOfferHelper(BaseHelper):
 
 	@overload
 	def __init__(self, base: TradeOffer, index: int, inv: VillagerInventory) -> None:
 		pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TridentEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TridentEntityHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .EntityHelper import EntityHelper
 
-TridentEntity = TypeVar["net.minecraft.entity.projectile.TridentEntity"]
+net_minecraft_entity_projectile_TridentEntity = TypeVar("net_minecraft_entity_projectile_TridentEntity")
+TridentEntity = net_minecraft_entity_projectile_TridentEntity
+
 
 class TridentEntityHelper(EntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/TropicalFishEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/TropicalFishEntityHelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .FishEntityHelper import FishEntityHelper
 
-TropicalFishEntity = TypeVar["net.minecraft.entity.passive.TropicalFishEntity"]
+net_minecraft_entity_passive_TropicalFishEntity = TypeVar("net_minecraft_entity_passive_TropicalFishEntity")
+TropicalFishEntity = net_minecraft_entity_passive_TropicalFishEntity
+
 
 class TropicalFishEntityHelper(FishEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/UniversalBlockStateHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/UniversalBlockStateHelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from .BlockStateHelper import BlockStateHelper
 from .DirectionHelper import DirectionHelper
 
-BlockState = TypeVar["net.minecraft.block.BlockState"]
+net_minecraft_block_BlockState = TypeVar("net_minecraft_block_BlockState")
+BlockState = net_minecraft_block_BlockState
+
 
 class UniversalBlockStateHelper(BlockStateHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/VillagerEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/VillagerEntityHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .MerchantEntityHelper import MerchantEntityHelper
 
-VillagerEntity = TypeVar["net.minecraft.entity.passive.VillagerEntity"]
+net_minecraft_entity_passive_VillagerEntity = TypeVar("net_minecraft_entity_passive_VillagerEntity")
+VillagerEntity = net_minecraft_entity_passive_VillagerEntity
+
 
 class VillagerEntityHelper(MerchantEntityHelper):
 	"""
 	Since: 1.6.3 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/VillagerInventory.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/VillagerInventory.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WardenEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/BaseProfile.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,119 @@
 from typing import overload
 from typing import TypeVar
-from .MobEntityHelper import MobEntityHelper
+from typing import Set
+from .Core import Core
+from .BaseEventRegistry import BaseEventRegistry
+from .BaseEvent import BaseEvent
 
-WardenEntity = TypeVar["net.minecraft.entity.mob.WardenEntity"]
+java_lang_Throwable = TypeVar("java_lang_Throwable")
+Throwable = java_lang_Throwable
 
-class WardenEntityHelper(MobEntityHelper):
+org_slf4j_Logger = TypeVar("org_slf4j_Logger")
+Logger = org_slf4j_Logger
+
+java_lang_Thread = TypeVar("java_lang_Thread")
+Thread = java_lang_Thread
+
+
+class BaseProfile:
 	"""
-	Since: 1.8.4 
+	Since: 1.2.7 
 	"""
+	LOGGER: Logger
+	joinedThreadStack: Set[Thread]
+	profileName: str
+
+	@overload
+	def __init__(self, runner: Core, logger: Logger) -> None:
+		pass
 
 	@overload
-	def __init__(self, base: WardenEntity) -> None:
+	def logError(self, ex: Throwable) -> None:
 		pass
 
 	@overload
-	def getAnger(self) -> int:
+	def getRegistry(self) -> BaseEventRegistry:
 		"""
-		Since: 1.8.4 
+		Since: 1.1.2 [citation needed] 
+		"""
+		pass
 
-		Returns:
-			this warden's anger towards its active target. 
+	@overload
+	def checkJoinedThreadStack(self) -> bool:
+		"""
+		Since: 1.6.0 
 		"""
 		pass
 
 	@overload
-	def isDigging(self) -> bool:
+	def loadOrCreateProfile(self, profileName: str) -> None:
+		"""
+		Since: 1.1.2 [citation needed] 
+
+		Args:
+			profileName: 
 		"""
-		Since: 1.8.4 
+		pass
 
-		Returns:
-			'true' if this warden is digging into the ground, 'false' otherwise. 
+	@overload
+	def saveProfile(self) -> None:
+		"""
+		Since: 1.0.8 [citation needed] 
 		"""
 		pass
 
 	@overload
-	def isEmerging(self) -> bool:
+	def triggerEvent(self, event: BaseEvent) -> None:
 		"""
-		Since: 1.8.4 
+		Since: 1.2.7 
 
-		Returns:
-			'true' if this warden is emerging from the ground, 'false' otherwise. 
+		Args:
+			event: 
 		"""
 		pass
 
 	@overload
-	def isRoaring(self) -> bool:
+	def triggerEventJoin(self, event: BaseEvent) -> None:
 		"""
-		Since: 1.8.4 
+		Since: 1.2.7 
 
-		Returns:
-			'true' if this warden is roaring, 'false' otherwise. 
+		Args:
+			event: 
 		"""
 		pass
 
 	@overload
-	def isSniffing(self) -> bool:
+	def triggerEventNoAnything(self, event: BaseEvent) -> None:
 		"""
-		Since: 1.8.4 
+		Since: 1.2.7 
 
-		Returns:
-			'true' if this warden is sniffing, 'false' otherwise. 
+		Args:
+			event: 
 		"""
 		pass
 
 	@overload
-	def isChargingSonicBoom(self) -> bool:
+	def triggerEventJoinNoAnything(self, event: BaseEvent) -> None:
 		"""
-		Since: 1.8.4 
+		Since: 1.2.7 
 
-		Returns:
-			'true' if this warden is charging its sonic boom attack, 'false' otherwise. 
+		Args:
+			event: 
 		"""
 		pass
 
+	@overload
+	def init(self, defaultProfile: str) -> None:
+		pass
+
+	@overload
+	def getCurrentProfileName(self) -> str:
+		pass
+
+	@overload
+	def renameCurrentProfile(self, profile: str) -> None:
+		pass
+
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/Websocket.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/Websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .MethodWrapper import MethodWrapper
 
-WebSocket = TypeVar["com.neovisionaries.ws.client.WebSocket"]
+com_neovisionaries_ws_client_WebSocket = TypeVar("com_neovisionaries_ws_client_WebSocket")
+WebSocket = com_neovisionaries_ws_client_WebSocket
+
 
 class Websocket:
 	"""
 	"""
 	onConnect: MethodWrapper
 	onTextMessage: MethodWrapper
 	onDisconnect: MethodWrapper
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WitchEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WitchEntityHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 from .ItemStackHelper import ItemStackHelper
 
-WitchEntity = TypeVar["net.minecraft.entity.mob.WitchEntity"]
+net_minecraft_entity_mob_WitchEntity = TypeVar("net_minecraft_entity_mob_WitchEntity")
+WitchEntity = net_minecraft_entity_mob_WitchEntity
+
 
 class WitchEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WitherEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WitherEntityHelper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import overload
 from typing import TypeVar
 from .MobEntityHelper import MobEntityHelper
 
-WitherEntity = TypeVar["net.minecraft.entity.boss.WitherEntity"]
+net_minecraft_entity_boss_WitherEntity = TypeVar("net_minecraft_entity_boss_WitherEntity")
+WitherEntity = net_minecraft_entity_boss_WitherEntity
+
 
 class WitherEntityHelper(MobEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WolfEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/ZombieVillagerEntityHelper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 from typing import overload
 from typing import TypeVar
-from .TameableEntityHelper import TameableEntityHelper
-from .DyeColorHelper import DyeColorHelper
+from .ZombieEntityHelper import ZombieEntityHelper
 
-WolfEntity = TypeVar["net.minecraft.entity.passive.WolfEntity"]
+net_minecraft_entity_mob_ZombieVillagerEntity = TypeVar("net_minecraft_entity_mob_ZombieVillagerEntity")
+ZombieVillagerEntity = net_minecraft_entity_mob_ZombieVillagerEntity
 
-class WolfEntityHelper(TameableEntityHelper):
+
+class ZombieVillagerEntityHelper(ZombieEntityHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: WolfEntity) -> None:
+	def __init__(self, base: ZombieVillagerEntity) -> None:
 		pass
 
 	@overload
-	def isBegging(self) -> bool:
+	def isConvertingToVillager(self) -> bool:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this wolf is tamed and the player has either a bone or meat in one of
-their hands, 'false' otherwise. 
+			'true' if this zombie villager is currently being converted back to a villager, 'false' otherwise. 
 		"""
 		pass
 
 	@overload
-	def getCollarColor(self) -> DyeColorHelper:
+	def getVillagerBiomeType(self) -> str:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the color of this wolf's collar. 
+			the type of biome the villager belonged to it was converted to a zombie. 
 		"""
 		pass
 
 	@overload
-	def isAngry(self) -> bool:
+	def getProfession(self) -> str:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this wolf is angry, 'false' otherwise. 
+			the profession of the villager before it was converted to a zombie. 
 		"""
 		pass
 
 	@overload
-	def isWet(self) -> bool:
+	def getLevel(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this wolf is wet, 'false' otherwise. 
+			the level of the villager before it was converted to a zombie. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WorldScanner.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WorldScanner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from typing import overload
 from typing import List
 from typing import TypeVar
 from typing import Mapping
 from .Pos3D import Pos3D
 
-Function = TypeVar["java.util.function.Function_xyz.wagyourtail.jsmacros.client.api.helpers.world.BlockStateHelper,java.lang.Boolean_"]
-ChunkPos = TypeVar["net.minecraft.util.math.ChunkPos"]
-World = TypeVar["net.minecraft.world.World"]
+java_util_function_Function_xyz_wagyourtail_jsmacros_client_api_helpers_world_BlockStateHelper,java_lang_Boolean_ = TypeVar("java_util_function_Function_xyz_wagyourtail_jsmacros_client_api_helpers_world_BlockStateHelper,java_lang_Boolean_")
+Function = java_util_function_Function_xyz_wagyourtail_jsmacros_client_api_helpers_world_BlockStateHelper,java_lang_Boolean_
+
+net_minecraft_util_math_ChunkPos = TypeVar("net_minecraft_util_math_ChunkPos")
+ChunkPos = net_minecraft_util_math_ChunkPos
+
+net_minecraft_world_World = TypeVar("net_minecraft_world_World")
+World = net_minecraft_world_World
+
 
 class WorldScanner:
 	"""A class to scan the world for certain blocks. The results of the filters are cached,
 so it's a good idea to reuse an instance of this if possible.
 The scanner can either return a list of all block positions or
 a list of blocks and their respective count for every block / state matching the filters criteria.\n
 	Since: 1.6.5
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WorldScannerBuilder.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WorldScannerBuilder.py`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/WrappedScript.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/WrappedScript.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import overload
 from typing import TypeVar
 from typing import Generic
 from .MethodWrapper import MethodWrapper
 
-Function = TypeVar["java.util.function.Function_xyz.wagyourtail.jsmacros.core.event.BaseEvent,xyz.wagyourtail.jsmacros.core.language.EventContainer_xyz.wagyourtail.jsmacros.core.language.BaseScriptContext____"]
+java_util_function_Function_xyz_wagyourtail_jsmacros_core_event_BaseEvent,xyz_wagyourtail_jsmacros_core_language_EventContainer_xyz_wagyourtail_jsmacros_core_language_BaseScriptContext____ = TypeVar("java_util_function_Function_xyz_wagyourtail_jsmacros_core_event_BaseEvent,xyz_wagyourtail_jsmacros_core_language_EventContainer_xyz_wagyourtail_jsmacros_core_language_BaseScriptContext____")
+Function = java_util_function_Function_xyz_wagyourtail_jsmacros_core_event_BaseEvent,xyz_wagyourtail_jsmacros_core_language_EventContainer_xyz_wagyourtail_jsmacros_core_language_BaseScriptContext____
+
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
+V = V
+
 
 class WrappedScript(Generic[T, U, V], MethodWrapper):
 	f: Function
 	_async: bool
 
 	@overload
 	def __init__(self, f: Function, _async: bool) -> None:
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/ZombieVillagerEntityHelper.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/DyeColorHelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 from typing import overload
 from typing import TypeVar
-from .ZombieEntityHelper import ZombieEntityHelper
+from .BaseHelper import BaseHelper
 
-ZombieVillagerEntity = TypeVar["net.minecraft.entity.mob.ZombieVillagerEntity"]
+net_minecraft_util_DyeColor = TypeVar("net_minecraft_util_DyeColor")
+DyeColor = net_minecraft_util_DyeColor
 
-class ZombieVillagerEntityHelper(ZombieEntityHelper):
+
+class DyeColorHelper(BaseHelper):
 	"""
 	Since: 1.8.4 
 	"""
 
 	@overload
-	def __init__(self, base: ZombieVillagerEntity) -> None:
+	def __init__(self, base: DyeColor) -> None:
+		pass
+
+	@overload
+	def getName(self) -> str:
+		"""
+		Since: 1.8.4 
+
+		Returns:
+			the name of the color. 
+		"""
 		pass
 
 	@overload
-	def isConvertingToVillager(self) -> bool:
+	def getId(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			'true' if this zombie villager is currently being converted back to a villager, 'false' otherwise. 
+			the color's identifier. 
 		"""
 		pass
 
 	@overload
-	def getVillagerBiomeType(self) -> str:
+	def getColorValue(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the type of biome the villager belonged to it was converted to a zombie. 
+			the color's rgb value. 
 		"""
 		pass
 
 	@overload
-	def getProfession(self) -> str:
+	def getFireworkColor(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the profession of the villager before it was converted to a zombie. 
+			the color's variation when used in fireworks. 
 		"""
 		pass
 
 	@overload
-	def getLevel(self) -> int:
+	def getSignColor(self) -> int:
 		"""
 		Since: 1.8.4 
 
 		Returns:
-			the level of the villager before it was converted to a zombie. 
+			the color's variation when used on signs. 
 		"""
 		pass
 
 	pass
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/events.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,9 +56,9 @@
 from .EventService import EventService
 from .EventEntityLoad import EventEntityLoad
 from .EventChunkUnload import EventChunkUnload
 from .EventArmorChange import EventArmorChange
 from .EventPlayerJoin import EventPlayerJoin
 from .EventHeldItemChange import EventHeldItemChange
 
-File = TypeVar["java.io.File"]
+File = TypeVar("java.io.File")
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/helpers.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,9 +139,9 @@
 from .OptionsHelper_AccessibilityOptionsHelper import OptionsHelper_AccessibilityOptionsHelper
 from .RabbitEntityHelper import RabbitEntityHelper
 from .BlockHelper import BlockHelper
 from .AbstractHorseEntityHelper import AbstractHorseEntityHelper
 from .SheepEntityHelper import SheepEntityHelper
 from .VindicatorEntityHelper import VindicatorEntityHelper
 
-File = TypeVar["java.io.File"]
+File = TypeVar("java.io.File")
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/libraries.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/libraries.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .FUtils import FUtils
 from .FClient import FClient
 from .FWorld import FWorld
 from .FGlobalVars import FGlobalVars
 from .IFWrapper import IFWrapper
 from .FPositionCommon import FPositionCommon
 
-File = TypeVar["java.io.File"]
+File = TypeVar("java.io.File")
 
 
 
 Chat = FChat()
 Player = FPlayer()
 Request = FRequest()
 KeyBind = FKeyBind()
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/mixins.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,9 +62,9 @@
 from .MixinMerchantScreen import MixinMerchantScreen
 from .MixinHorseEntity import MixinHorseEntity
 from .MixinCyclingButton import MixinCyclingButton
 from .MixinStatHandler import MixinStatHandler
 from .MixinAdvancementProgress import MixinAdvancementProgress
 from .MixinPalettedContainerData import MixinPalettedContainerData
 
-File = TypeVar["java.io.File"]
+File = TypeVar("java.io.File")
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC/rest.py` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,9 +297,9 @@
 from .ClassBuilder_AnnotationBuilder import ClassBuilder_AnnotationBuilder
 from .BossBarConsumer import BossBarConsumer
 from .ScriptCodeCompiler import ScriptCodeCompiler
 from .CommandBuilder import CommandBuilder
 from .Draw2DElement_Builder import Draw2DElement_Builder
 from .RunningContextContainer import RunningContextContainer
 
-File = TypeVar["java.io.File"]
+File = TypeVar("java.io.File")
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/PKG-INFO` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsMacrosAC
-Version: 1.8.4.8263756
+Version: 1.8.5.8296535
 Summary: A package to let your IDE know what JsMacros can do
 Home-page: UNKNOWN
 Author: Hasenzahn1
 Author-email: <motzer10@gmx.de>
 License: UNKNOWN
 Description: # JsMacrosAC
```

### Comparing `JsMacrosAC-1.8.4.8263756/JsMacrosAC.egg-info/SOURCES.txt` & `JsMacrosAC-1.8.5.8296535/JsMacrosAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/PKG-INFO` & `JsMacrosAC-1.8.5.8296535/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsMacrosAC
-Version: 1.8.4.8263756
+Version: 1.8.5.8296535
 Summary: A package to let your IDE know what JsMacros can do
 Home-page: UNKNOWN
 Author: Hasenzahn1
 Author-email: <motzer10@gmx.de>
 License: UNKNOWN
 Description: # JsMacrosAC
```

### Comparing `JsMacrosAC-1.8.4.8263756/README.md` & `JsMacrosAC-1.8.5.8296535/README.md`

 * *Files identical despite different names*

### Comparing `JsMacrosAC-1.8.4.8263756/setup.py` & `JsMacrosAC-1.8.5.8296535/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
-VERSION = '1.8.4'
+VERSION = '1.8.5'
 if "-" in VERSION: VERSION = VERSION.split("-")[0]
 VERSION += "." + str(time.time()).split(".")[0][3:]
 DESCRIPTION = 'A package to let your IDE know what JsMacros can do'
 
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
```

