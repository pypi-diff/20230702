# Comparing `tmp/tonic-1.2.8.dev8.tar.gz` & `tmp/tonic-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.2.8.dev8.tar", last modified: Wed Jun 21 10:38:20 2023, max compression
+gzip compressed data, was "tonic-1.3.2.tar", last modified: Sun Jul  2 06:38:17 2023, max compression
```

## Comparing `tonic-1.2.8.dev8.tar` & `tonic-1.3.2.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.980976 tonic-1.2.8.dev8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.980976 tonic-1.2.8.dev8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    39739 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38250 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 06:37:55.000000 tonic-1.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.852789 tonic-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.856789 tonic-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-02 06:37:55.000000 tonic-1.3.2/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 06:37:55.000000 tonic-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 06:37:55.000000 tonic-1.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-02 06:38:17.000000 tonic-1.3.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    39958 2023-07-02 06:38:17.000000 tonic-1.3.2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 06:37:55.000000 tonic-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 06:37:55.000000 tonic-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-02 06:38:17.884791 tonic-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-02 06:37:55.000000 tonic-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.868790 tonic-1.3.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-02 06:37:55.000000 tonic-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-02 06:38:17.884791 tonic-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-02 06:37:55.000000 tonic-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.868790 tonic-1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-02 06:37:55.000000 tonic-1.3.2/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-02 06:37:55.000000 tonic-1.3.2/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 06:37:55.000000 tonic-1.3.2/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.872790 tonic-1.3.2/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-02 06:37:55.000000 tonic-1.3.2/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.876790 tonic-1.3.2/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.876790 tonic-1.3.2/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37426 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.876790 tonic-1.3.2/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.2.8.dev8/.github/workflows/ci-pipeline.yml` & `tonic-1.3.2/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/AUTHORS` & `tonic-1.3.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/ChangeLog` & `tonic-1.3.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 CHANGES
 =======
 
+v1.3.2
+------
+
+* update docs notebook with new ToTimesurface transform
+
+v1.3.1
+------
+
+* update docs gallery script for ToTimesurface
+
+1.3.0
+-----
+
+* change Timesurface transform parameters and speed it up considerably
 * Compose takes into account empty event arrays now
 * update NMNIST prototype dataset and tests to make compatible with Python 3.11
 * test Python 3.11
 * simplify STMNIST prototype dataset, broke keep\_compressed option though
 * Add delta\_t as a parameter to time surface test
 * Remove print statements to evaluate correctness
 * Time surface returns time surfaces at interval
```

### Comparing `tonic-1.2.8.dev8/LICENSE.txt` & `tonic-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/PKG-INFO` & `tonic-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.8.dev8
+Version: 1.3.2
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.8.dev8/README.md` & `tonic-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/Makefile` & `tonic-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/event-cameras/eventstream.png` & `tonic-1.3.2/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/event-cameras/framestream.png` & `tonic-1.3.2/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.3.2/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.3.2/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/snn/neuron-models.png` & `tonic-1.3.2/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/snn/surrogates.png` & `tonic-1.3.2/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/tonic-logo-black.png` & `tonic-1.3.2/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/tonic-logo-white.png` & `tonic-1.3.2/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/_static/tonic_favicon.png` & `tonic-1.3.2/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/about/info.rst` & `tonic-1.3.2/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/about/prototype.rst` & `tonic-1.3.2/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/about/release_notes.rst` & `tonic-1.3.2/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/conf.py` & `tonic-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/datasets.rst` & `tonic-1.3.2/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.3.2/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/representations/plot_toframe.py` & `tonic-1.3.2/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/representations/plot_toimage.py` & `tonic-1.3.2/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.3.2/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.3.2/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_decimation.py` & `tonic-1.3.2/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_denoise.py` & `tonic-1.3.2/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_downsample.py` & `tonic-1.3.2/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.3.2/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.3.2/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.3.2/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.3.2/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.3.2/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.3.2/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.3.2/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.3.2/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.3.2/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.3.2/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.3.2/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/getting_involved/communication_channels.rst` & `tonic-1.3.2/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/getting_involved/contribute.rst` & `tonic-1.3.2/docs/getting_involved/contribute.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 * Where is the dataset hosted?
 * What format is it in?
 
 To download a dataset, Tonic makes use of a copy of pytorch vision's tools that can be found 
 `here <https://github.com/neuromorphs/tonic/blob/develop/tonic/datasets/download_utils.py>`_.
 Cloud providers such as Dropbox, Google Drive, OneDrive etc. are usually not straightforward 
 to automatically download from, so if the dataset owner provides multiple mirrors,
-prefer a simple REST-like webpage such as https://www.neuromorphic-vision.com/public/downloads/.
+prefer a simple REST-like webpage.
 
 The trickier question is the one of file decoding. There exist a variety of file formats that 
 events and related data are saved in, including .txt, .aedat, .dat, .es, .mat, .hdf5, .rosbag 
 and more. Ordered by degree of easiness to decode a file format, here is one subjective ranking:
 
 #. **hdf5**. This bundles everything in a single file which prevents it from getting messy on 
    your file system and the h5py python package is reliable and a breeze to use. Easy!
```

### Comparing `tonic-1.2.8.dev8/docs/getting_started/install.rst` & `tonic-1.3.2/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/getting_started/nmnist.ipynb` & `tonic-1.3.2/docs/getting_started/nmnist.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874198717948719%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 2: {'attachments': OrderedDict()}, 4: "*

 * *            "{'attachments': OrderedDict()}, 6: {'attachments': OrderedDict()}, 8: {'attachments': "*

 * *            "OrderedDict()}, 10: {'attachments': OrderedDict()}, 12: {'attachments': "*

 * *            "OrderedDict()}, 13: {'source': {insert: [(1, '    sensor_size=sensor_size, dt=10000, "*

 * *            "tau=30000,\\n')], delete: [1]}}, 14: {'attachments': OrderedDict()}, 16: "*

 * *            "{'attachments': OrderedDict()}, 18 […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "72ab4fec-4fe8-49cc-867f-6a77bcfaa062",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Loading the event-based version of MNIST\n",
@@ -33,14 +34,15 @@
             "source": [
                 "import tonic\n",
                 "\n",
                 "dataset = tonic.datasets.NMNIST(save_to=\"../tutorials/data\", train=False)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "6e9f45be-20da-44f8-962b-2b842fc862df",
             "metadata": {},
             "source": [
                 "Now you can index the samples manually for inspection! Depending on the dataset, you can expect different return values. N-MNIST returns events and the target class for each sample. Other datasets provide images, IMU data, GPS data and more. You will find the details in the dataset reference. Events are a structured numpy array with different channels. For recordings from event cameras, those channels are typically x, y, time and polarity."
             ]
         },
@@ -52,14 +54,15 @@
             "outputs": [],
             "source": [
                 "events, target = dataset[1000]\n",
                 "events"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "dba2d3f0-f82b-4f16-a06f-97669b73bec4",
             "metadata": {},
             "source": [
                 "Event timestamps in Tonic will always have microsecond resolution. We can accumulate/bin many events into a frame to visualise them. That's what we're going to do next.\n",
                 "\n",
                 "Applying a transform manually\n",
@@ -78,14 +81,15 @@
                 "sensor_size = tonic.datasets.NMNIST.sensor_size\n",
                 "frame_transform = transforms.ToFrame(sensor_size=sensor_size, n_time_bins=3)\n",
                 "\n",
                 "frames = frame_transform(events)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "dcfd768d-0a7f-48c8-b1d1-6f80d0b516a4",
             "metadata": {},
             "source": [
                 "The frames have dimensions (Time, Number of polarities, Height and Width). Let's plot one frame for each of the three saccades in a sample of N-MNIST. We'll take the difference between two camera polarities to see the direction of movement."
             ]
         },
@@ -108,14 +112,15 @@
                 "    plt.tight_layout()\n",
                 "\n",
                 "\n",
                 "plot_frames(frames)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "9733a1da-96a5-4ab1-ad0e-d0d46f7a305c",
             "metadata": {},
             "source": [
                 "You can see nicely the three saccades for this sample. The bright and dark version of the digit is because an event camera outputs two polarities, one for ON events that signify an increase in illuminance, and one for OFF events that signify a decrease.\n",
                 "\n",
                 "In the previous plot we can see some isolated noise events, let's try to get rid of them. We'll use a transform that deletes such isolated events, and then apply it to our events. Notice the order we're applying. Then we are going to plot the denoised frames:"
@@ -133,14 +138,15 @@
                 "events_denoised = denoise_transform(events)\n",
                 "frames_denoised = frame_transform(events_denoised)\n",
                 "\n",
                 "plot_frames(frames_denoised)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "10406fbc-ddb2-4104-9a0d-ab375f3e653c",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "That looks a bit cleaner!\n",
@@ -163,14 +169,15 @@
                 "for axis, slice in zip(axes, volume):\n",
                 "    axis.imshow(slice[0])\n",
                 "    axis.axis(\"off\")\n",
                 "plt.tight_layout()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "5c9d5bb7-8658-409a-bcc7-24c7e0587479",
             "metadata": {},
             "source": [
                 "Or time surfaces:"
             ]
         },
@@ -178,28 +185,29 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "2bb332e9-fc69-428c-bf20-2b71fed89edd",
             "metadata": {},
             "outputs": [],
             "source": [
                 "surfaces = transforms.ToTimesurface(\n",
-                "    sensor_size=sensor_size, surface_dimensions=None, tau=10000, decay=\"exp\"\n",
+                "    sensor_size=sensor_size, dt=10000, tau=30000,\n",
                 ")(events_denoised)\n",
                 "\n",
                 "n_events = events_denoised.shape[0]\n",
                 "n_events_per_slice = n_events // 3\n",
                 "fig, axes = plt.subplots(1, 3)\n",
                 "for i, axis in enumerate(axes):\n",
                 "    surf = surfaces[(i + 1) * n_events_per_slice - 1]\n",
                 "    axis.imshow(surf[0] - surf[1])\n",
                 "    axis.axis(\"off\")\n",
                 "plt.tight_layout()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a167e44a-39d8-4e42-b5e5-39a9e9179463",
             "metadata": {},
             "source": [
                 "Putting it all together\n",
                 "-----------------------\n",
                 "Previously we applied the transformations manually. We can simplify this code, by chaining the transforms and passing them to our dataset."
@@ -216,14 +224,15 @@
                 "\n",
                 "dataset = tonic.datasets.NMNIST(\n",
                 "    save_to=\"../tutorials/data\", train=False, transform=transform\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "b2f027cc-55ba-46b6-848d-deedf4e5a3e4",
             "metadata": {},
             "source": [
                 "Now the transforms will be applied whenever a new sample is loaded. To simplify the loading, we make use of a PyTorch DataLoader in a final step:"
             ]
         },
@@ -241,14 +250,15 @@
                 "dataloader = torch.utils.data.DataLoader(dataset, shuffle=True)\n",
                 "frames, target = next(iter(dataloader))\n",
                 "\n",
                 "plot_frames(frames.squeeze())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "aac04620-cf13-4c03-b653-7d3520d52380",
             "metadata": {},
             "source": [
                 "And that's there is to it!"
             ]
         },
```

### Comparing `tonic-1.2.8.dev8/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.3.2/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/how-tos/visualizing-data.ipynb` & `tonic-1.3.2/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.3.2/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/index.md` & `tonic-1.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/make.bat` & `tonic-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/reading_material/design_choices.rst` & `tonic-1.3.2/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/reading_material/intro-event-cameras.rst` & `tonic-1.3.2/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/reading_material/intro-snns.rst` & `tonic-1.3.2/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/reading_material/training-snns.rst` & `tonic-1.3.2/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/transformations.rst` & `tonic-1.3.2/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/tutorials/batching.ipynb` & `tonic-1.3.2/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/tutorials/davis_data.ipynb` & `tonic-1.3.2/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.3.2/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/tutorials/large_datasets.ipynb` & `tonic-1.3.2/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/docs/tutorials/slicing.ipynb` & `tonic-1.3.2/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/setup.cfg` & `tonic-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/dataset_utils.py` & `tonic-1.3.2/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/prototype_dataset_utils.py` & `tonic-1.3.2/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_audio_transforms.py` & `tonic-1.3.2/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_caching.py` & `tonic-1.3.2/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_chained_transforms.py` & `tonic-1.3.2/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_data/sample.aedat4` & `tonic-1.3.2/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_data/sample_ncars.dat` & `tonic-1.3.2/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_data/sample_nmnist.bin` & `tonic-1.3.2/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_data/sample_stmnist.mat` & `tonic-1.3.2/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_datasets.py` & `tonic-1.3.2/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_dsec.py` & `tonic-1.3.2/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_io.py` & `tonic-1.3.2/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_prototype_datasets.py` & `tonic-1.3.2/test/test_prototype_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_representations.py` & `tonic-1.3.2/test/test_representations.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,37 +197,36 @@
     orig_events, _ = create_random_input(n_events=10000, sensor_size=sensor_size)
     transform = transforms.ToImage(sensor_size=sensor_size)
     image = transform(orig_events)
     assert image.shape == sensor_size[::-1]
 
 
 @pytest.mark.parametrize(
-    "surface_dimensions, tau, delta_t", [((15, 15), 100, 0), ((3, 3), 10, 1e4), (None, 1e4, 1e5)]
+    "sensor_size, dt, tau,",
+    [
+        ((40, 15, 2), 10000, 10000),
+        ((10, 20, 2), 20000, 1000),
+        ((30, 30, 2), 30000, 3000),
+    ],
 )
-def test_representation_time_surface(surface_dimensions, tau, delta_t):
-    orig_events, sensor_size = create_random_input(n_events=1000)
-
-    transform = transforms.ToTimesurface(
-        sensor_size=sensor_size, surface_dimensions=surface_dimensions, tau=tau, delta_t=delta_t
+def test_representation_time_surface(sensor_size, dt, tau):
+    orig_events, sensor_size = create_random_input(
+        sensor_size=sensor_size, n_events=10000
     )
 
+    transform = transforms.ToTimesurface(sensor_size=sensor_size, dt=dt, tau=tau)
+
     surfaces = transform(orig_events)
 
-    if delta_t == 0:
-        assert surfaces.shape[0] == len(orig_events)
-    else:
-        duration = orig_events["t"][-1] - orig_events["t"][0]
-        assert surfaces.shape[0] == duration // delta_t 
-        
+    duration = orig_events["t"][-1] - orig_events["t"][0]
+    assert surfaces.shape[0] == duration // dt
+
     assert surfaces.shape[1] == 2
-    if surface_dimensions:
-        assert surfaces.shape[2:] == surface_dimensions
-    else:
-        assert surfaces.shape[2] == sensor_size[1]
-        assert surfaces.shape[3] == sensor_size[0]
+    assert surfaces.shape[2] == sensor_size[1]
+    assert surfaces.shape[3] == sensor_size[0]
     assert surfaces is not orig_events
 
 
 @pytest.mark.parametrize(
     "surface_size, cell_size, tau, decay",
     [(7, 9, 100, "lin"), (3, 4, 1000, "exp")],
 )
```

### Comparing `tonic-1.2.8.dev8/test/test_sliced_dataset.py` & `tonic-1.3.2/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_slicers.py` & `tonic-1.3.2/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_tonic_utils.py` & `tonic-1.3.2/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/test_transforms.py` & `tonic-1.3.2/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/test/utils.py` & `tonic-1.3.2/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/audio_transforms.py` & `tonic-1.3.2/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/cached_dataset.py` & `tonic-1.3.2/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/collation.py` & `tonic-1.3.2/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/dataset.py` & `tonic-1.3.2/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/__init__.py` & `tonic-1.3.2/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/asl_dvs.py` & `tonic-1.3.2/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/cifar10dvs.py` & `tonic-1.3.2/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/davisdataset.py` & `tonic-1.3.2/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/dsec.py` & `tonic-1.3.2/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/dvs_lips.py` & `tonic-1.3.2/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/dvsgesture.py` & `tonic-1.3.2/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/hsd.py` & `tonic-1.3.2/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/mvsec.py` & `tonic-1.3.2/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/ncaltech101.py` & `tonic-1.3.2/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/nmnist.py` & `tonic-1.3.2/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/pokerdvs.py` & `tonic-1.3.2/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/s_mnist.py` & `tonic-1.3.2/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/tum_vie.py` & `tonic-1.3.2/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/datasets/visual_place_recognition.py` & `tonic-1.3.2/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/download_utils.py` & `tonic-1.3.2/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/__init__.py` & `tonic-1.3.2/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/crop.py` & `tonic-1.3.2/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/decimate.py` & `tonic-1.3.2/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/denoise.py` & `tonic-1.3.2/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/drop_event.py` & `tonic-1.3.2/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/drop_pixel.py` & `tonic-1.3.2/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/refractory_period.py` & `tonic-1.3.2/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/spatial_jitter.py` & `tonic-1.3.2/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/time_jitter.py` & `tonic-1.3.2/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/time_skew.py` & `tonic-1.3.2/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/to_averaged_timesurface.py` & `tonic-1.3.2/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/to_bina_rep.py` & `tonic-1.3.2/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/to_frame.py` & `tonic-1.3.2/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/to_voxel_grid.py` & `tonic-1.3.2/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/functional/uniform_noise.py` & `tonic-1.3.2/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/io.py` & `tonic-1.3.2/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/README.md` & `tonic-1.3.2/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/datasets/ncars.py` & `tonic-1.3.2/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/datasets/nmnist.py` & `tonic-1.3.2/tonic/prototype/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/datasets/prophesee.py` & `tonic-1.3.2/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/datasets/stmnist.py` & `tonic-1.3.2/tonic/prototype/datasets/stmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.3.2/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.3.2/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/prototype/slicers.py` & `tonic-1.3.2/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/sliced_dataset.py` & `tonic-1.3.2/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/slicers.py` & `tonic-1.3.2/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic/transforms.py` & `tonic-1.3.2/tonic/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -900,42 +900,32 @@
         )
 
         return frames.squeeze(0)
 
 
 @dataclass(frozen=True)
 class ToTimesurface:
-    """Create global or local time surfaces for each event. Modeled after the paper Lagorce et al.
-    2016, Hots: a hierarchy of event-based time-surfaces for pattern recognition
-    https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7508476.
+    """Create global time surfaces at a specific time interval dt.
 
     Parameters:
-        sensor_size: a 3-tuple of x,y,p for sensor_size
-        surface_dimensions (int, int): width does not have to be equal to height, however both numbers have to be odd.
-            if surface_dimensions is None: the time surface is defined globally, on the whole sensor grid.
-        tau (float): time constant to decay events around occuring event with.
-        delta_t (float): the interval at which the time-surfaces are accumulated, if set 0 number of time-surfaces will
-            equal to the number of events. (defaults to 0.0)
-        decay (str): can be either 'lin' or 'exp', corresponding to linear or exponential decay.
+        sensor_size: A 3-tuple of x,y,p for sensor_size
+        dt (float): The interval at which the time-surfaces are accumulated.
+        tau (float): Time constant to decay events with.
     """
 
     sensor_size: Tuple[int, int, int]
-    surface_dimensions: Union[None, Tuple[int, int]] = None
-    tau: float = 5e3
-    delta_t: float = 0.0
-    decay: str = "lin"
+    dt: float
+    tau: float
 
     def __call__(self, events):
         return functional.to_timesurface_numpy(
             events=events,
             sensor_size=self.sensor_size,
-            surface_dimensions=self.surface_dimensions,
+            dt=self.dt,
             tau=self.tau,
-            delta_t=self.delta_t,
-            decay=self.decay,
         )
 
 
 @dataclass(frozen=True)
 class ToVoxelGrid:
     """Build a voxel grid with bilinear interpolation in the time domain from a set of events.
     Implements the event volume from Zhu et al. 2019, Unsupervised event-based learning of optical
```

### Comparing `tonic-1.2.8.dev8/tonic/utils.py` & `tonic-1.3.2/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic-logo-padded.png` & `tonic-1.3.2/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev8/tonic.egg-info/PKG-INFO` & `tonic-1.3.2/tonic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.8.dev8
+Version: 1.3.2
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.8.dev8/tonic.egg-info/SOURCES.txt` & `tonic-1.3.2/tonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

