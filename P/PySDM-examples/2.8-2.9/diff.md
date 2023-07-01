# Comparing `tmp/PySDM-examples-2.8.tar.gz` & `tmp/PySDM-examples-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySDM-examples-2.8.tar", last modified: Wed May 18 16:48:44 2022, max compression
+gzip compressed data, was "PySDM-examples-2.9.tar", last modified: Wed Jun  1 21:23:07 2022, max compression
```

## Comparing `PySDM-examples-2.8.tar` & `PySDM-examples-2.9.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.290430 PySDM-examples-2.8/
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.250429 PySDM-examples-2.8/.github/
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.254429 PySDM-examples-2.8/.github/workflows/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      292 2022-03-03 20:47:40.000000 PySDM-examples-2.8/.github/workflows/cancel.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1196 2022-02-17 22:39:03.000000 PySDM-examples-2.8/.github/workflows/main.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      745 2022-01-03 01:39:16.000000 PySDM-examples-2.8/.github/workflows/pdoc.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      670 2022-04-24 06:51:26.000000 PySDM-examples-2.8/.github/workflows/precommithooks.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1393 2022-01-14 18:52:14.000000 PySDM-examples-2.8/.github/workflows/pylint.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      717 2021-09-18 19:40:16.000000 PySDM-examples-2.8/.github/workflows/stale.yml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1837 2022-05-18 16:48:27.000000 PySDM-examples-2.8/.gitignore
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      418 2022-04-24 06:51:26.000000 PySDM-examples-2.8/.pre-commit-config.yaml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    35149 2021-09-14 23:05:15.000000 PySDM-examples-2.8/LICENSE
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20683 2022-05-18 16:48:44.290430 PySDM-examples-2.8/PKG-INFO
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.258429 PySDM-examples-2.8/PySDM_examples/
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.258429 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2702 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/aerosol.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    11585 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_ARG2000_paper.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    11547 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_CloudMicrophysics_ARG.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   345238 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/fig_4_kinetic_limitations.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   439901 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/figs1-5.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5379 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/run_ARG_parcel.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.262429 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      244 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    41463 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_1.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4183 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    15556 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_3.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    59386 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_4.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    61291 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_5.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     9929 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/simulation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      228 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/table.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3792 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/table_1.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1857 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/table_2.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.262429 PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      150 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      284 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/example.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   186384 2021-11-11 22:45:17.000000 PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/fig_5.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2333 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3886 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.266430 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       90 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      828 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/example.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2317 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/example_benchmark.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2819 2022-01-03 01:39:16.000000 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/gui.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1052 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      837 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/spin_up.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.266430 PySDM-examples-2.8/PySDM_examples/Bartman_2020_MasterThesis/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Bartman_2020_MasterThesis/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2338 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bartman_2020_MasterThesis/fig_4_adaptive_sdm.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4092 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bartman_2020_MasterThesis/fig_5_BDF_VS_ADAPTIVE.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.270429 PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     8098 2022-02-17 22:39:03.000000 PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/demo.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   515402 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/demo_fig2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   159304 2022-02-17 22:39:03.000000 PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/demo_fig3.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      507 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/label.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.270429 PySDM-examples-2.8/PySDM_examples/Berry_1967/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      154 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Berry_1967/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2551 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Berry_1967/example.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3103 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Berry_1967/example_fig_6.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7074 2022-02-17 22:39:03.000000 PySDM-examples-2.8/PySDM_examples/Berry_1967/figs_5_8_10.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1494 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Berry_1967/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1024 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Berry_1967/spectrum_plotter.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.270429 PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       83 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    23317 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/make_fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1575 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1295 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.270429 PySDM-examples-2.8/PySDM_examples/Jaruga_and_Pawlowska_2018/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Jaruga_and_Pawlowska_2018/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   109981 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   180432 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_3.ipynb
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.274430 PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    67752 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/fig_1.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2756 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4352 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.274430 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6358 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/aerosol.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   217700 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/fig_1.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   182228 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5338 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/fig_3.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6081 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/plot_helper.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2914 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4957 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.274430 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       60 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4639 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/common.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4460 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/cumulus.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    22906 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    41426 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/fig_3.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      949 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/strato_cumulus.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.278430 PySDM-examples-2.8/PySDM_examples/Pyrcel/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2022-02-23 23:47:06.000000 PySDM-examples-2.8/PySDM_examples/Pyrcel/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   143144 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Pyrcel/example_basic_run.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2095 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Pyrcel/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3603 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Pyrcel/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.278430 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      253 2021-09-14 23:05:15.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/error_measure.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2536 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/example.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1807 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/example_timing.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6557 2021-11-11 22:45:17.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1175 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5409 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/spectrum_plotter.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.278430 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      120 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   233495 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/fig_1.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1906 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/mpdata_1d.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1639 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/plot.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4667 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     8387 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.278430 PySDM-examples-2.8/PySDM_examples/Singer_Ward/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    78182 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Singer_Ward/MWE_joss_paper.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Singer_Ward/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5328 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Singer_Ward/aerosol.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   114930 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/Singer_Ward/kohler.ipynb
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.282430 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      166 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1583 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/fields.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1309 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4283 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui_controller.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    13262 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui_settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    13088 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui_viewer.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4218 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/make_default_product_collection.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4137 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/mpdata_2d.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7034 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/plots.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6571 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/simulation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1439 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/sounding.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2579 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/storage.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.286430 PySDM-examples-2.8/PySDM_examples/UIUC_2021/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      214 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)  1097783 2022-01-14 18:52:14.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/copula_hello.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      783 2022-01-03 01:39:16.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/frozen_fraction.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2034 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/make_particulator.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4383 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/plots.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1166 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/run_simulation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   110251 2022-01-14 18:52:14.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/theory.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7007 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/UIUC_2021/zigzag.ipynb
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.286430 PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2021-09-30 22:11:26.000000 PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   203297 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2153 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3603 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/simulation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      252 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/__init__.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.290430 PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      177 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   179778 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/make_fig_1.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)   144368 2022-05-18 16:48:27.000000 PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/make_fig_2.ipynb
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1490 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/settings.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3635 2022-05-03 21:33:29.000000 PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/simulation.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.290430 PySDM-examples-2.8/PySDM_examples/utils/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      142 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/utils/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      698 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/utils/basic_simulation.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      741 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/utils/dummy_controller.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      470 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/utils/progbar_controller.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.290430 PySDM-examples-2.8/PySDM_examples/utils/widgets/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      520 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/utils/widgets/__init__.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      407 2021-11-11 22:45:17.000000 PySDM-examples-2.8/PySDM_examples/utils/widgets/freezer.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      267 2022-04-24 06:51:26.000000 PySDM-examples-2.8/PySDM_examples/utils/widgets/progbar_updater.py
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.258429 PySDM-examples-2.8/PySDM_examples.egg-info/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20683 2022-05-18 16:48:43.000000 PySDM-examples-2.8/PySDM_examples.egg-info/PKG-INFO
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6519 2022-05-18 16:48:44.000000 PySDM-examples-2.8/PySDM_examples.egg-info/SOURCES.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)        1 2022-05-18 16:48:43.000000 PySDM-examples-2.8/PySDM_examples.egg-info/dependency_links.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      106 2022-05-18 16:48:44.000000 PySDM-examples-2.8/PySDM_examples.egg-info/requires.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       15 2022-05-18 16:48:44.000000 PySDM-examples-2.8/PySDM_examples.egg-info/top_level.txt
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20257 2022-05-18 16:48:27.000000 PySDM-examples-2.8/README.md
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       30 2022-04-24 06:51:26.000000 PySDM-examples-2.8/pyproject.toml
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)       38 2022-05-18 16:48:44.290430 PySDM-examples-2.8/setup.cfg
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1122 2022-05-18 16:48:35.000000 PySDM-examples-2.8/setup.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      518 2022-05-18 16:48:27.000000 PySDM-examples-2.8/test-time-requirements.txt
-drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-05-18 16:48:44.290430 PySDM-examples-2.8/tests/
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2073 2022-04-24 06:51:26.000000 PySDM-examples-2.8/tests/test_Arabas_et_al_2015_export.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      878 2022-04-24 06:51:26.000000 PySDM-examples-2.8/tests/test_run_examples.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1189 2022-04-24 06:51:26.000000 PySDM-examples-2.8/tests/test_run_notebooks.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2397 2022-04-24 06:51:26.000000 PySDM-examples-2.8/tests/test_todos_annotated.py
--rw-r--r--   0 slayoo    (1000) slayoo    (1000)      668 2022-04-24 06:51:26.000000 PySDM-examples-2.8/tests/tests_uiuc_2021.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.801179 PySDM-examples-2.9/
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.757179 PySDM-examples-2.9/.github/
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.761179 PySDM-examples-2.9/.github/workflows/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      292 2022-03-03 20:47:40.000000 PySDM-examples-2.9/.github/workflows/cancel.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1196 2022-02-17 22:39:03.000000 PySDM-examples-2.9/.github/workflows/main.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      745 2022-01-03 01:39:16.000000 PySDM-examples-2.9/.github/workflows/pdoc.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      670 2022-04-24 06:51:26.000000 PySDM-examples-2.9/.github/workflows/precommithooks.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1393 2022-01-14 18:52:14.000000 PySDM-examples-2.9/.github/workflows/pylint.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      717 2021-09-18 19:40:16.000000 PySDM-examples-2.9/.github/workflows/stale.yml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1837 2022-05-18 16:48:27.000000 PySDM-examples-2.9/.gitignore
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      418 2022-04-24 06:51:26.000000 PySDM-examples-2.9/.pre-commit-config.yaml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    35149 2021-09-14 23:05:15.000000 PySDM-examples-2.9/LICENSE
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20686 2022-06-01 21:23:07.801179 PySDM-examples-2.9/PKG-INFO
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.761179 PySDM-examples-2.9/PySDM_examples/
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.765179 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2702 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/aerosol.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    11585 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_ARG2000_paper.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    11547 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_CloudMicrophysics_ARG.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   345238 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/fig_4_kinetic_limitations.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   439901 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/figs1-5.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5379 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/run_ARG_parcel.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.765179 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      244 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    41463 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_1.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4183 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    15556 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_3.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    59386 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_4.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    61291 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_5.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     9929 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/simulation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      228 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/table.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3792 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/table_1.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1857 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/table_2.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.769178 PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      150 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      284 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/example.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   186384 2021-11-11 22:45:17.000000 PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/fig_5.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2333 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3886 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.769178 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       90 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      828 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/example.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2317 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/example_benchmark.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2819 2022-01-03 01:39:16.000000 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/gui.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1052 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      837 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/spin_up.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.769178 PySDM-examples-2.9/PySDM_examples/Bartman_2020_MasterThesis/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Bartman_2020_MasterThesis/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2338 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bartman_2020_MasterThesis/fig_4_adaptive_sdm.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4092 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bartman_2020_MasterThesis/fig_5_BDF_VS_ADAPTIVE.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.773179 PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     8098 2022-02-17 22:39:03.000000 PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/demo.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   515402 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/demo_fig2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   159304 2022-02-17 22:39:03.000000 PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/demo_fig3.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      507 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/label.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.773179 PySDM-examples-2.9/PySDM_examples/Berry_1967/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      154 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Berry_1967/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2551 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Berry_1967/example.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3103 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Berry_1967/example_fig_6.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7074 2022-02-17 22:39:03.000000 PySDM-examples-2.9/PySDM_examples/Berry_1967/figs_5_8_10.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1494 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Berry_1967/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1024 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Berry_1967/spectrum_plotter.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.777179 PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       83 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    23317 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/make_fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1575 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1295 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.777179 PySDM-examples-2.9/PySDM_examples/Jaruga_and_Pawlowska_2018/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Jaruga_and_Pawlowska_2018/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   109981 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   180432 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_3.ipynb
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.777179 PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    67752 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/fig_1.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2756 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4352 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.781179 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6358 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/aerosol.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   217700 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/fig_1.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   182228 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5338 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/fig_3.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6081 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/plot_helper.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2914 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4957 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.781179 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       60 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4639 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/common.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4460 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/cumulus.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    22906 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    41426 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/fig_3.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      949 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/strato_cumulus.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.781179 PySDM-examples-2.9/PySDM_examples/Pyrcel/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2022-02-23 23:47:06.000000 PySDM-examples-2.9/PySDM_examples/Pyrcel/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   143144 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Pyrcel/example_basic_run.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2095 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Pyrcel/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3603 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Pyrcel/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.785179 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      253 2021-09-14 23:05:15.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/error_measure.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2536 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/example.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1807 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/example_timing.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6557 2021-11-11 22:45:17.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1175 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5409 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/spectrum_plotter.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.785179 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      120 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   228509 2022-06-01 21:22:40.000000 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/fig_1.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1906 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/mpdata_1d.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1639 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/plot.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4712 2022-06-01 21:22:40.000000 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     8448 2022-06-01 21:22:40.000000 PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.785179 PySDM-examples-2.9/PySDM_examples/Singer_Ward/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    78182 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Singer_Ward/MWE_joss_paper.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       31 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Singer_Ward/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     5328 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Singer_Ward/aerosol.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   114930 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/Singer_Ward/kohler.ipynb
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.789179 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      166 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1583 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/fields.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1309 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4283 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui_controller.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    13262 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui_settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    13088 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui_viewer.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4218 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/make_default_product_collection.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4137 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/mpdata_2d.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7034 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/plots.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6571 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/simulation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1439 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/sounding.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2579 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/storage.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.793179 PySDM-examples-2.9/PySDM_examples/UIUC_2021/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      214 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)  1097783 2022-01-14 18:52:14.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/copula_hello.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      783 2022-01-03 01:39:16.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/frozen_fraction.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2034 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/make_particulator.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     4383 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/plots.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1166 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/run_simulation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   110251 2022-01-14 18:52:14.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/theory.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     7007 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/UIUC_2021/zigzag.ipynb
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.793179 PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       97 2021-09-30 22:11:26.000000 PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   203297 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2153 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3603 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/simulation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      252 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/__init__.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.797179 PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      177 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   179778 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/make_fig_1.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)   144368 2022-05-18 16:48:27.000000 PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/make_fig_2.ipynb
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1490 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/settings.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     3635 2022-05-03 21:33:29.000000 PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/simulation.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.797179 PySDM-examples-2.9/PySDM_examples/utils/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      142 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/utils/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      698 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/utils/basic_simulation.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      741 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/utils/dummy_controller.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      470 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/utils/progbar_controller.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.797179 PySDM-examples-2.9/PySDM_examples/utils/widgets/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      520 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/utils/widgets/__init__.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      407 2021-11-11 22:45:17.000000 PySDM-examples-2.9/PySDM_examples/utils/widgets/freezer.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      267 2022-04-24 06:51:26.000000 PySDM-examples-2.9/PySDM_examples/utils/widgets/progbar_updater.py
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.761179 PySDM-examples-2.9/PySDM_examples.egg-info/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20686 2022-06-01 21:23:07.000000 PySDM-examples-2.9/PySDM_examples.egg-info/PKG-INFO
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     6519 2022-06-01 21:23:07.000000 PySDM-examples-2.9/PySDM_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)        1 2022-06-01 21:23:07.000000 PySDM-examples-2.9/PySDM_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      106 2022-06-01 21:23:07.000000 PySDM-examples-2.9/PySDM_examples.egg-info/requires.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       15 2022-06-01 21:23:07.000000 PySDM-examples-2.9/PySDM_examples.egg-info/top_level.txt
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)    20260 2022-06-01 21:22:40.000000 PySDM-examples-2.9/README.md
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       30 2022-04-24 06:51:26.000000 PySDM-examples-2.9/pyproject.toml
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)       38 2022-06-01 21:23:07.801179 PySDM-examples-2.9/setup.cfg
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1122 2022-06-01 21:22:50.000000 PySDM-examples-2.9/setup.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      511 2022-06-01 21:22:40.000000 PySDM-examples-2.9/test-time-requirements.txt
+drwxr-xr-x   0 slayoo    (1000) slayoo    (1000)        0 2022-06-01 21:23:07.797179 PySDM-examples-2.9/tests/
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2073 2022-04-24 06:51:26.000000 PySDM-examples-2.9/tests/test_Arabas_et_al_2015_export.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      878 2022-04-24 06:51:26.000000 PySDM-examples-2.9/tests/test_run_examples.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     1189 2022-04-24 06:51:26.000000 PySDM-examples-2.9/tests/test_run_notebooks.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)     2397 2022-04-24 06:51:26.000000 PySDM-examples-2.9/tests/test_todos_annotated.py
+-rw-r--r--   0 slayoo    (1000) slayoo    (1000)      668 2022-04-24 06:51:26.000000 PySDM-examples-2.9/tests/tests_uiuc_2021.py
```

### Comparing `PySDM-examples-2.8/.github/workflows/main.yml` & `PySDM-examples-2.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/.github/workflows/pdoc.yml` & `PySDM-examples-2.9/.github/workflows/pdoc.yml`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/.github/workflows/precommithooks.yml` & `PySDM-examples-2.9/.github/workflows/precommithooks.yml`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/.github/workflows/pylint.yml` & `PySDM-examples-2.9/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/.github/workflows/stale.yml` & `PySDM-examples-2.9/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/.gitignore` & `PySDM-examples-2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/LICENSE` & `PySDM-examples-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PKG-INFO` & `PySDM-examples-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySDM-examples
-Version: 2.8
+Version: 2.9
 Summary: PySDM usage examples reproducing results from literature and depicting how to use PySDM from Python Jupyter notebooks
 Home-page: https://github.com/atmos-cloud-sim-uj/PySDM-examples
 Author: https://github.com/orgs/atmos-cloud-sim-uj/people
 Author-email: sylwester.arabas@uj.edu.pl
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 
 [![Github Actions Build Status](https://github.com/atmos-cloud-sim-uj/PySDM-examples/workflows/PySDM-examples/badge.svg?branch=main)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/actions)    
 [![GitHub issues](https://img.shields.io/github/issues-pr/atmos-cloud-sim-uj/PySDM-examples.svg?logo=github&logoColor=white)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/pulls?q=)
 [![GitHub issues](https://img.shields.io/github/issues-pr-closed/atmos-cloud-sim-uj/PySDM-examples.svg?logo=github&logoColor=white)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/pulls?q=is:closed)    
 [![PyPI version](https://badge.fury.io/py/PySDM-examples.svg)](https://pypi.org/project/PySDM-examples)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://atmos-cloud-sim-uj.github.io/PySDM-examples/)
 
-s repository stores example files for `PySDM` depicting usage of `PySDM` from Python via Jupyter.
+This repository stores example files for `PySDM` depicting usage of `PySDM` from Python via Jupyter.
 For information on the `PySDM` package itself and examples of usage from Julia and Matlab, 
 see [PySDM README.md](https://github.com/atmos-cloud-sim-uj/PySDM/blob/master/README.md) file.
 
 Please use the [PySDM issue-tracking](https://github.com/atmos-cloud-sim-uj/PySDM/issues) and [discussion](https://github.com/atmos-cloud-sim-uj/PySDM/discussions) infrastructure for `PySDM-examples` as well.
 
 ### 0D box-model coalescence-only examples:
 - [Shima et al. 2009](http://doi.org/10.1002/qj.441) (Box model, coalescence only, test case employing Golovin analytical solution):
```

### Comparing `PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/aerosol.py` & `PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/aerosol.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_ARG2000_paper.py` & `PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_ARG2000_paper.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_CloudMicrophysics_ARG.py` & `PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/data_from_CloudMicrophysics_ARG.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/fig_4_kinetic_limitations.ipynb` & `PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/fig_4_kinetic_limitations.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/figs1-5.ipynb` & `PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/figs1-5.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Abdul_Razzak_Ghan_2000/run_ARG_parcel.py` & `PySDM-examples-2.9/PySDM_examples/Abdul_Razzak_Ghan_2000/run_ARG_parcel.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_1.ipynb` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_1.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_3.ipynb` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_3.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_4.ipynb` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_4.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/fig_5.ipynb` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/fig_5.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/table_1.py` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/table_1.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Alpert_and_Knopf_2016/table_2.py` & `PySDM-examples-2.9/PySDM_examples/Alpert_and_Knopf_2016/table_2.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/fig_5.ipynb` & `PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/fig_5.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/settings.py` & `PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_and_Shima_2017/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Arabas_and_Shima_2017/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/example.py` & `PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/example.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/example_benchmark.py` & `PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/example_benchmark.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/gui.ipynb` & `PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/gui.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/settings.py` & `PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Arabas_et_al_2015/spin_up.py` & `PySDM-examples-2.9/PySDM_examples/Arabas_et_al_2015/spin_up.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bartman_2020_MasterThesis/fig_4_adaptive_sdm.py` & `PySDM-examples-2.9/PySDM_examples/Bartman_2020_MasterThesis/fig_4_adaptive_sdm.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bartman_2020_MasterThesis/fig_5_BDF_VS_ADAPTIVE.py` & `PySDM-examples-2.9/PySDM_examples/Bartman_2020_MasterThesis/fig_5_BDF_VS_ADAPTIVE.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/demo.ipynb` & `PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/demo.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/demo_fig2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/demo_fig2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bartman_et_al_2021/demo_fig3.ipynb` & `PySDM-examples-2.9/PySDM_examples/Bartman_et_al_2021/demo_fig3.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Berry_1967/example.py` & `PySDM-examples-2.9/PySDM_examples/Berry_1967/example.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Berry_1967/example_fig_6.py` & `PySDM-examples-2.9/PySDM_examples/Berry_1967/example_fig_6.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Berry_1967/figs_5_8_10.ipynb` & `PySDM-examples-2.9/PySDM_examples/Berry_1967/figs_5_8_10.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Berry_1967/settings.py` & `PySDM-examples-2.9/PySDM_examples/Berry_1967/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Berry_1967/spectrum_plotter.py` & `PySDM-examples-2.9/PySDM_examples/Berry_1967/spectrum_plotter.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/make_fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/make_fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/settings.py` & `PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Bieli_et_al_2022/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Bieli_et_al_2022/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_3.ipynb` & `PySDM-examples-2.9/PySDM_examples/Jaruga_and_Pawlowska_2018/fig_3.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/fig_1.ipynb` & `PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/fig_1.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/settings.py` & `PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Kreidenweis_et_al_2003/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Kreidenweis_et_al_2003/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/aerosol.py` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/aerosol.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/fig_1.ipynb` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/fig_1.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/fig_3.ipynb` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/fig_3.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/plot_helper.py` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/plot_helper.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/settings.py` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Lowe_et_al_2019/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Lowe_et_al_2019/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/common.py` & `PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/common.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/cumulus.py` & `PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/cumulus.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/fig_3.ipynb` & `PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/fig_3.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Morrison_and_Grabowski_2007/strato_cumulus.py` & `PySDM-examples-2.9/PySDM_examples/Morrison_and_Grabowski_2007/strato_cumulus.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Pyrcel/example_basic_run.ipynb` & `PySDM-examples-2.9/PySDM_examples/Pyrcel/example_basic_run.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Pyrcel/settings.py` & `PySDM-examples-2.9/PySDM_examples/Pyrcel/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Pyrcel/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Pyrcel/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/example.py` & `PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/example.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/example_timing.py` & `PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/example_timing.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/settings.py` & `PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shima_et_al_2009/spectrum_plotter.py` & `PySDM-examples-2.9/PySDM_examples/Shima_et_al_2009/spectrum_plotter.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/mpdata_1d.py` & `PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/mpdata_1d.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/plot.py` & `PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/plot.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/settings.py` & `PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         assert rhod_solution.success
         self.rhod = interp1d(z_points, rhod_solution.y[0])
 
         self.mpdata_settings = {"n_iters": 3, "iga": True, "fct": True, "tot": True}
         self.condensation_rtol_x = condensation.DEFAULTS.rtol_x
         self.condensation_rtol_thd = condensation.DEFAULTS.rtol_thd
         self.condensation_adaptive = True
+        self.condensation_update_thd = False
         self.coalescence_adaptive = True
 
         self.number_of_bins = 100
         self.r_bins_edges_dry = np.logspace(
             np.log10(0.001 * si.um),
             np.log10(1 * si.um),
             self.number_of_bins + 1,
```

### Comparing `PySDM-examples-2.8/PySDM_examples/Shipway_and_Hill_2012/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Shipway_and_Hill_2012/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         builder.set_environment(env)
         builder.add_dynamic(AmbientThermodynamics())
         builder.add_dynamic(
             Condensation(
                 adaptive=settings.condensation_adaptive,
                 rtol_thd=settings.condensation_rtol_thd,
                 rtol_x=settings.condensation_rtol_x,
+                update_thd=settings.condensation_update_thd,
             )
         )
         builder.add_dynamic(EulerianAdvection(self.mpdata))
         if settings.precip:
             if settings.breakup:
                 builder.add_dynamic(
                     Collision(
```

### Comparing `PySDM-examples-2.8/PySDM_examples/Singer_Ward/MWE_joss_paper.ipynb` & `PySDM-examples-2.9/PySDM_examples/Singer_Ward/MWE_joss_paper.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Singer_Ward/aerosol.py` & `PySDM-examples-2.9/PySDM_examples/Singer_Ward/aerosol.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Singer_Ward/kohler.ipynb` & `PySDM-examples-2.9/PySDM_examples/Singer_Ward/kohler.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/fields.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/fields.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui_controller.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui_controller.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui_settings.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui_settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/gui_viewer.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/gui_viewer.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/make_default_product_collection.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/make_default_product_collection.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/mpdata_2d.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/mpdata_2d.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/plots.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/plots.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/sounding.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/sounding.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Szumowski_et_al_1998/storage.py` & `PySDM-examples-2.9/PySDM_examples/Szumowski_et_al_1998/storage.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/copula_hello.ipynb` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/copula_hello.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/frozen_fraction.py` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/frozen_fraction.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/make_particulator.py` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/make_particulator.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/plots.py` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/plots.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/run_simulation.py` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/run_simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/theory.ipynb` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/theory.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/UIUC_2021/zigzag.ipynb` & `PySDM-examples-2.9/PySDM_examples/UIUC_2021/zigzag.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/settings.py` & `PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/Yang_et_al_2018/simulation.py` & `PySDM-examples-2.9/PySDM_examples/Yang_et_al_2018/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/make_fig_1.ipynb` & `PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/make_fig_1.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/make_fig_2.ipynb` & `PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/make_fig_2.ipynb`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/settings.py` & `PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/settings.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/deJong_Mackay_2022/simulation.py` & `PySDM-examples-2.9/PySDM_examples/deJong_Mackay_2022/simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/utils/basic_simulation.py` & `PySDM-examples-2.9/PySDM_examples/utils/basic_simulation.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/utils/dummy_controller.py` & `PySDM-examples-2.9/PySDM_examples/utils/dummy_controller.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples/utils/widgets/__init__.py` & `PySDM-examples-2.9/PySDM_examples/utils/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/PySDM_examples.egg-info/PKG-INFO` & `PySDM-examples-2.9/PySDM_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySDM-examples
-Version: 2.8
+Version: 2.9
 Summary: PySDM usage examples reproducing results from literature and depicting how to use PySDM from Python Jupyter notebooks
 Home-page: https://github.com/atmos-cloud-sim-uj/PySDM-examples
 Author: https://github.com/orgs/atmos-cloud-sim-uj/people
 Author-email: sylwester.arabas@uj.edu.pl
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 
 [![Github Actions Build Status](https://github.com/atmos-cloud-sim-uj/PySDM-examples/workflows/PySDM-examples/badge.svg?branch=main)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/actions)    
 [![GitHub issues](https://img.shields.io/github/issues-pr/atmos-cloud-sim-uj/PySDM-examples.svg?logo=github&logoColor=white)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/pulls?q=)
 [![GitHub issues](https://img.shields.io/github/issues-pr-closed/atmos-cloud-sim-uj/PySDM-examples.svg?logo=github&logoColor=white)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/pulls?q=is:closed)    
 [![PyPI version](https://badge.fury.io/py/PySDM-examples.svg)](https://pypi.org/project/PySDM-examples)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://atmos-cloud-sim-uj.github.io/PySDM-examples/)
 
-s repository stores example files for `PySDM` depicting usage of `PySDM` from Python via Jupyter.
+This repository stores example files for `PySDM` depicting usage of `PySDM` from Python via Jupyter.
 For information on the `PySDM` package itself and examples of usage from Julia and Matlab, 
 see [PySDM README.md](https://github.com/atmos-cloud-sim-uj/PySDM/blob/master/README.md) file.
 
 Please use the [PySDM issue-tracking](https://github.com/atmos-cloud-sim-uj/PySDM/issues) and [discussion](https://github.com/atmos-cloud-sim-uj/PySDM/discussions) infrastructure for `PySDM-examples` as well.
 
 ### 0D box-model coalescence-only examples:
 - [Shima et al. 2009](http://doi.org/10.1002/qj.441) (Box model, coalescence only, test case employing Golovin analytical solution):
```

### Comparing `PySDM-examples-2.8/PySDM_examples.egg-info/SOURCES.txt` & `PySDM-examples-2.9/PySDM_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/README.md` & `PySDM-examples-2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![Github Actions Build Status](https://github.com/atmos-cloud-sim-uj/PySDM-examples/workflows/PySDM-examples/badge.svg?branch=main)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/actions)    
 [![GitHub issues](https://img.shields.io/github/issues-pr/atmos-cloud-sim-uj/PySDM-examples.svg?logo=github&logoColor=white)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/pulls?q=)
 [![GitHub issues](https://img.shields.io/github/issues-pr-closed/atmos-cloud-sim-uj/PySDM-examples.svg?logo=github&logoColor=white)](https://github.com/atmos-cloud-sim-uj/PySDM-examples/pulls?q=is:closed)    
 [![PyPI version](https://badge.fury.io/py/PySDM-examples.svg)](https://pypi.org/project/PySDM-examples)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://atmos-cloud-sim-uj.github.io/PySDM-examples/)
 
-s repository stores example files for `PySDM` depicting usage of `PySDM` from Python via Jupyter.
+This repository stores example files for `PySDM` depicting usage of `PySDM` from Python via Jupyter.
 For information on the `PySDM` package itself and examples of usage from Julia and Matlab, 
 see [PySDM README.md](https://github.com/atmos-cloud-sim-uj/PySDM/blob/master/README.md) file.
 
 Please use the [PySDM issue-tracking](https://github.com/atmos-cloud-sim-uj/PySDM/issues) and [discussion](https://github.com/atmos-cloud-sim-uj/PySDM/discussions) infrastructure for `PySDM-examples` as well.
 
 ### 0D box-model coalescence-only examples:
 - [Shima et al. 2009](http://doi.org/10.1002/qj.441) (Box model, coalescence only, test case employing Golovin analytical solution):
```

### Comparing `PySDM-examples-2.8/setup.py` & `PySDM-examples-2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return long_description
 
 
 setup(
     name="PySDM-examples",
     description="PySDM usage examples reproducing results from literature "
     "and depicting how to use PySDM from Python Jupyter notebooks",
-    version='2.8',
+    version='2.9',
     setup_requires=["setuptools_scm"],
     install_requires=[
         "PySDM",
         "PyMPDATA",
         "atmos-cloud-sim-uj-utils",
         "pystrict",
         "matplotlib",
```

### Comparing `PySDM-examples-2.8/tests/test_Arabas_et_al_2015_export.py` & `PySDM-examples-2.9/tests/test_Arabas_et_al_2015_export.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/tests/test_run_examples.py` & `PySDM-examples-2.9/tests/test_run_examples.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/tests/test_run_notebooks.py` & `PySDM-examples-2.9/tests/test_run_notebooks.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/tests/test_todos_annotated.py` & `PySDM-examples-2.9/tests/test_todos_annotated.py`

 * *Files identical despite different names*

### Comparing `PySDM-examples-2.8/tests/tests_uiuc_2021.py` & `PySDM-examples-2.9/tests/tests_uiuc_2021.py`

 * *Files identical despite different names*

