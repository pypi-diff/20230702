# Comparing `tmp/open-metric-learning-0.4.2.tar.gz` & `tmp/open-metric-learning-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-0.4.2.tar", last modified: Wed Jun  7 18:27:10 2023, max compression
+gzip compressed data, was "dist/open-metric-learning-0.4.3.tar", last modified: Sun Jul  2 15:09:24 2023, max compression
```

## Comparing `open-metric-learning-0.4.2.tar` & `open-metric-learning-0.4.3.tar`

### file list

```diff
@@ -1,203 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    26089 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24665 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.673302 open-metric-learning-0.4.2/oml/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.673302 open-metric-learning-0.4.2/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.673302 open-metric-learning-0.4.2/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.677302 open-metric-learning-0.4.2/oml/configs/extractor/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/vit_clip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.677302 open-metric-learning-0.4.2/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.681301 open-metric-learning-0.4.2/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.681301 open-metric-learning-0.4.2/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.681301 open-metric-learning-0.4.2/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.685301 open-metric-learning-0.4.2/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.685301 open-metric-learning-0.4.2/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.689301 open-metric-learning-0.4.2/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.689301 open-metric-learning-0.4.2/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.693302 open-metric-learning-0.4.2/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/ddp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.693302 open-metric-learning-0.4.2/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.693302 open-metric-learning-0.4.2/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/pairwise_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.701301 open-metric-learning-0.4.2/oml/lightning/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/train.py
--rw-r--r--   0 runner    (1001) docker     (122)     7566 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.701301 open-metric-learning-0.4.2/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.701301 open-metric-learning-0.4.2/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    15994 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.705301 open-metric-learning-0.4.2/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.705301 open-metric-learning-0.4.2/oml/models/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.705301 open-metric-learning-0.4.2/oml/models/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/meta/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/meta/siamese.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/pooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.709301 open-metric-learning-0.4.2/oml/models/vit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/vision_transformer_clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     8065 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3818 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    26089 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/tests/test_build_readme.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/tests/test_outdated_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    30629 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    29205 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/vit_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/vit_unicom.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.968665 open-metric-learning-0.4.3/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.968665 open-metric-learning-0.4.3/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/unicom_transforms.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/ddp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7566 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15994 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/meta/siamese.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/resnet/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/resnet/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/vit_clip/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_clip/external/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_dino/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_dino/external/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/external/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/external/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_unicom/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_unicom/external/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11680 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/external/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3818 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    30629 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/tests/test_outdated_docs.py
```

### Comparing `open-metric-learning-0.4.2/LICENSE` & `open-metric-learning-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/PKG-INFO` & `open-metric-learning-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 0.4.2
+Version: 0.4.3
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -292,15 +292,15 @@
 ```python
 import torch
 from tqdm import tqdm
 
 from oml.datasets.base import DatasetWithLabels
 from oml.losses.triplet import TripletLossWithMiner
 from oml.miners.inbatch_all_tri import AllTripletsMiner
-from oml.models.vit.vit import ViTExtractor
+from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
 
 dataset_root = "mock_dataset/"
 df_train, _ = download_mock_dataset(dataset_root)
 
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).train()
@@ -324,14 +324,114 @@
 ```
 [comment]:vanilla-train-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kntDAIdIZ9L40jcndguLAb-XqmCFOgS5?usp=sharing)
 <details>
+<summary>Validation</summary>
+<p>
+
+[comment]:vanilla-validation-start
+```python
+import torch
+from tqdm import tqdm
+
+from oml.datasets.base import DatasetQueryGallery
+from oml.metrics.embeddings import EmbeddingMetrics
+from oml.models import ViTExtractor
+from oml.utils.download_mock_dataset import download_mock_dataset
+
+dataset_root = "mock_dataset/"
+_, df_val = download_mock_dataset(dataset_root)
+
+extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).eval()
+
+val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
+
+val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
+calculator = EmbeddingMetrics(extra_keys=("paths",))
+calculator.setup(num_samples=len(val_dataset))
+
+with torch.no_grad():
+    for batch in tqdm(val_loader):
+        batch["embeddings"] = extractor(batch["input_tensors"])
+        calculator.update_data(batch)
+
+metrics = calculator.compute_metrics()
+
+# Logging
+print(calculator.metrics)  # metrics
+print(calculator.metrics_unreduced)  # metrics without averaging over queries
+
+# Visualisation
+calculator.get_plot_for_queries(query_ids=[0, 2], n_instances=5)  # draw predictions on predefined queries
+calculator.get_plot_for_worst_queries(metric_name="OVERALL/map/5", n_queries=2, n_instances=5)  # draw mistakes
+calculator.visualize()  # draw mistakes for all the available metrics
+
+```
+[comment]:vanilla-validation-end
+</p>
+</details>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1O2o3k8I8jN5hRin3dKnAS3WsgG04tmIT?usp=sharing)
+<details>
+<summary>Training + Validation [Lightning and Neptune logging]</summary>
+<p>
+
+[comment]:lightning-start
+```python
+import pytorch_lightning as pl
+import torch
+
+from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels
+from oml.lightning.modules.extractor import ExtractorModule
+from oml.lightning.callbacks.metric import MetricValCallback
+from oml.losses.triplet import TripletLossWithMiner
+from oml.metrics.embeddings import EmbeddingMetrics
+from oml.miners.inbatch_all_tri import AllTripletsMiner
+from oml.models import ViTExtractor
+from oml.samplers.balance import BalanceSampler
+from oml.utils.download_mock_dataset import download_mock_dataset
+from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger
+
+dataset_root = "mock_dataset/"
+df_train, df_val = download_mock_dataset(dataset_root)
+
+# model
+extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
+
+# train
+optimizer = torch.optim.SGD(extractor.parameters(), lr=1e-6)
+train_dataset = DatasetWithLabels(df_train, dataset_root=dataset_root)
+criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner())
+batch_sampler = BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=3)
+train_loader = torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler)
+
+# val
+val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
+val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
+metric_callback = MetricValCallback(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]), log_images=True)
+
+# logging
+logger = TensorBoardLogger(".")  # For TensorBoard
+# logger = NeptuneLogger(api_key="", project="", log_model_checkpoints=False)  # For Neptune
+
+# run
+pl_model = ExtractorModule(extractor, criterion, optimizer)
+trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
+trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
+
+```
+[comment]:lightning-end
+</p>
+</details>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link)
+<details>
 <summary>Using a trained model for retrieval</summary>
 <p>
 
 [comment]:usage-retrieval-start
 ```python
 import torch
 
@@ -404,28 +504,36 @@
 |  `ViTExtractor.from_pretrained("vits16_sop")`   | 0.866 | Stanford Online Products |   [link](https://drive.google.com/file/d/1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A/view?usp=sharing)      |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_sop)   |
 | `ViTExtractor.from_pretrained("vits16_cars")`   | 0.907 |         CARS 196         |   [link](https://drive.google.com/drive/folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cars)  |
 |  `ViTExtractor.from_pretrained("vits16_cub")`   | 0.837 |       CUB 200 2011       |   [link](https://drive.google.com/drive/folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cub)   |
 
 We also provide an integration with the models pretrained by other researchers.
 All metrics below were obtained on the images with the sizes of **224 x 224**:
 
-|                            model                            | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
-|:-----------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
-|    `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")`    |          0.547           |       0.514        |    0.448     |  0.618   |
-|    `ViTCLIPExtractor.from_pretrained("sber_vitb16_224")`    |          0.565           |       0.565        |    0.524     |  0.648   |
-|    `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")`    |          0.512           |       0.555        |    0.606     |  0.707   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`   |          0.612           |       0.491        |    0.560     |  0.693   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`   |          0.648           |       0.606        |    0.665     |  0.767   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`   |          0.670           |       0.675        |    0.745     |  0.844   |
-|        `ViTExtractor.from_pretrained("vits16_dino")`        |          0.648           |       0.509        |    0.627     |  0.265   |
-|        `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
-|        `ViTExtractor.from_pretrained("vitb16_dino")`        |          0.658           |       0.514        |    0.541     |  0.288   |
-|        `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
-|    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`    |          0.493           |       0.267        |    0.264     |  0.149   |
-| `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")` |          0.515           |       0.284        |    0.455     |  0.247   |
+|                            model                             | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
+|:------------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
+|    `ViTUnicomExtractor.from_pretrained("vitb16_unicom")`     |          0.700           |       0.734        |    0.847     |  0.916   |
+|    `ViTUnicomExtractor.from_pretrained("vitb32_unicom")`     |          0.690           |       0.722        |    0.796     |  0.893   |
+|    `ViTUnicomExtractor.from_pretrained("vitl14_unicom")`     |          0.726           |       0.790        |    0.868     |  0.922   |
+| `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`  |          0.745           |       0.810        |    0.875     |  0.924   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")`     |          0.547           |       0.514        |    0.448     |  0.618   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitb16_224")`     |          0.565           |       0.565        |    0.524     |  0.648   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")`     |          0.512           |       0.555        |    0.606     |  0.707   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`    |          0.612           |       0.491        |    0.560     |  0.693   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`    |          0.648           |       0.606        |    0.665     |  0.767   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`    |          0.670           |       0.675        |    0.745     |  0.844   |
+|        `ViTExtractor.from_pretrained("vits16_dino")`         |          0.648           |       0.509        |    0.627     |  0.265   |
+|         `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
+|        `ViTExtractor.from_pretrained("vitb16_dino")`         |          0.658           |       0.514        |    0.541     |  0.288   |
+|         `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
+|    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`     |          0.493           |       0.267        |    0.264     |  0.149   |
+| `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")`  |          0.515           |       0.284        |    0.455     |  0.247   |
+
+**The metrics may be different from the ones reported by papers,
+because the version of train/val split and usage of bounding boxes may differ.
+Particularly, we used bounding boxes during the evaluation.*
 
 ### How to use models from Zoo?
 
 [comment]:zoo-start
 ```python
 from oml.const import CKPT_SAVE_ROOT as CKPT_DIR, MOCK_DATASET_PATH as DATA_DIR
 from oml.models import ViTExtractor
```

### Comparing `open-metric-learning-0.4.2/README.md` & `open-metric-learning-0.4.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 ```python
 import torch
 from tqdm import tqdm
 
 from oml.datasets.base import DatasetWithLabels
 from oml.losses.triplet import TripletLossWithMiner
 from oml.miners.inbatch_all_tri import AllTripletsMiner
-from oml.models.vit.vit import ViTExtractor
+from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
 
 dataset_root = "mock_dataset/"
 df_train, _ = download_mock_dataset(dataset_root)
 
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).train()
@@ -295,14 +295,114 @@
 ```
 [comment]:vanilla-train-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kntDAIdIZ9L40jcndguLAb-XqmCFOgS5?usp=sharing)
 <details>
+<summary>Validation</summary>
+<p>
+
+[comment]:vanilla-validation-start
+```python
+import torch
+from tqdm import tqdm
+
+from oml.datasets.base import DatasetQueryGallery
+from oml.metrics.embeddings import EmbeddingMetrics
+from oml.models import ViTExtractor
+from oml.utils.download_mock_dataset import download_mock_dataset
+
+dataset_root = "mock_dataset/"
+_, df_val = download_mock_dataset(dataset_root)
+
+extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).eval()
+
+val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
+
+val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
+calculator = EmbeddingMetrics(extra_keys=("paths",))
+calculator.setup(num_samples=len(val_dataset))
+
+with torch.no_grad():
+    for batch in tqdm(val_loader):
+        batch["embeddings"] = extractor(batch["input_tensors"])
+        calculator.update_data(batch)
+
+metrics = calculator.compute_metrics()
+
+# Logging
+print(calculator.metrics)  # metrics
+print(calculator.metrics_unreduced)  # metrics without averaging over queries
+
+# Visualisation
+calculator.get_plot_for_queries(query_ids=[0, 2], n_instances=5)  # draw predictions on predefined queries
+calculator.get_plot_for_worst_queries(metric_name="OVERALL/map/5", n_queries=2, n_instances=5)  # draw mistakes
+calculator.visualize()  # draw mistakes for all the available metrics
+
+```
+[comment]:vanilla-validation-end
+</p>
+</details>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1O2o3k8I8jN5hRin3dKnAS3WsgG04tmIT?usp=sharing)
+<details>
+<summary>Training + Validation [Lightning and Neptune logging]</summary>
+<p>
+
+[comment]:lightning-start
+```python
+import pytorch_lightning as pl
+import torch
+
+from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels
+from oml.lightning.modules.extractor import ExtractorModule
+from oml.lightning.callbacks.metric import MetricValCallback
+from oml.losses.triplet import TripletLossWithMiner
+from oml.metrics.embeddings import EmbeddingMetrics
+from oml.miners.inbatch_all_tri import AllTripletsMiner
+from oml.models import ViTExtractor
+from oml.samplers.balance import BalanceSampler
+from oml.utils.download_mock_dataset import download_mock_dataset
+from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger
+
+dataset_root = "mock_dataset/"
+df_train, df_val = download_mock_dataset(dataset_root)
+
+# model
+extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
+
+# train
+optimizer = torch.optim.SGD(extractor.parameters(), lr=1e-6)
+train_dataset = DatasetWithLabels(df_train, dataset_root=dataset_root)
+criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner())
+batch_sampler = BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=3)
+train_loader = torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler)
+
+# val
+val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
+val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
+metric_callback = MetricValCallback(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]), log_images=True)
+
+# logging
+logger = TensorBoardLogger(".")  # For TensorBoard
+# logger = NeptuneLogger(api_key="", project="", log_model_checkpoints=False)  # For Neptune
+
+# run
+pl_model = ExtractorModule(extractor, criterion, optimizer)
+trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
+trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
+
+```
+[comment]:lightning-end
+</p>
+</details>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link)
+<details>
 <summary>Using a trained model for retrieval</summary>
 <p>
 
 [comment]:usage-retrieval-start
 ```python
 import torch
 
@@ -375,28 +475,36 @@
 |  `ViTExtractor.from_pretrained("vits16_sop")`   | 0.866 | Stanford Online Products |   [link](https://drive.google.com/file/d/1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A/view?usp=sharing)      |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_sop)   |
 | `ViTExtractor.from_pretrained("vits16_cars")`   | 0.907 |         CARS 196         |   [link](https://drive.google.com/drive/folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cars)  |
 |  `ViTExtractor.from_pretrained("vits16_cub")`   | 0.837 |       CUB 200 2011       |   [link](https://drive.google.com/drive/folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cub)   |
 
 We also provide an integration with the models pretrained by other researchers.
 All metrics below were obtained on the images with the sizes of **224 x 224**:
 
-|                            model                            | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
-|:-----------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
-|    `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")`    |          0.547           |       0.514        |    0.448     |  0.618   |
-|    `ViTCLIPExtractor.from_pretrained("sber_vitb16_224")`    |          0.565           |       0.565        |    0.524     |  0.648   |
-|    `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")`    |          0.512           |       0.555        |    0.606     |  0.707   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`   |          0.612           |       0.491        |    0.560     |  0.693   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`   |          0.648           |       0.606        |    0.665     |  0.767   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`   |          0.670           |       0.675        |    0.745     |  0.844   |
-|        `ViTExtractor.from_pretrained("vits16_dino")`        |          0.648           |       0.509        |    0.627     |  0.265   |
-|        `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
-|        `ViTExtractor.from_pretrained("vitb16_dino")`        |          0.658           |       0.514        |    0.541     |  0.288   |
-|        `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
-|    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`    |          0.493           |       0.267        |    0.264     |  0.149   |
-| `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")` |          0.515           |       0.284        |    0.455     |  0.247   |
+|                            model                             | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
+|:------------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
+|    `ViTUnicomExtractor.from_pretrained("vitb16_unicom")`     |          0.700           |       0.734        |    0.847     |  0.916   |
+|    `ViTUnicomExtractor.from_pretrained("vitb32_unicom")`     |          0.690           |       0.722        |    0.796     |  0.893   |
+|    `ViTUnicomExtractor.from_pretrained("vitl14_unicom")`     |          0.726           |       0.790        |    0.868     |  0.922   |
+| `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`  |          0.745           |       0.810        |    0.875     |  0.924   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")`     |          0.547           |       0.514        |    0.448     |  0.618   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitb16_224")`     |          0.565           |       0.565        |    0.524     |  0.648   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")`     |          0.512           |       0.555        |    0.606     |  0.707   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`    |          0.612           |       0.491        |    0.560     |  0.693   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`    |          0.648           |       0.606        |    0.665     |  0.767   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`    |          0.670           |       0.675        |    0.745     |  0.844   |
+|        `ViTExtractor.from_pretrained("vits16_dino")`         |          0.648           |       0.509        |    0.627     |  0.265   |
+|         `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
+|        `ViTExtractor.from_pretrained("vitb16_dino")`         |          0.658           |       0.514        |    0.541     |  0.288   |
+|         `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
+|    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`     |          0.493           |       0.267        |    0.264     |  0.149   |
+| `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")`  |          0.515           |       0.284        |    0.455     |  0.247   |
+
+**The metrics may be different from the ones reported by papers,
+because the version of train/val split and usage of bounding boxes may differ.
+Particularly, we used bounding boxes during the evaluation.*
 
 ### How to use models from Zoo?
 
 [comment]:zoo-start
 ```python
 from oml.const import CKPT_SAVE_ROOT as CKPT_DIR, MOCK_DATASET_PATH as DATA_DIR
 from oml.models import ViTExtractor
```

### Comparing `open-metric-learning-0.4.2/oml/const.py` & `open-metric-learning-0.4.3/oml/const.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/datasets/base.py` & `open-metric-learning-0.4.3/oml/datasets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     provide the splitting information (for example, ``DeepFashion InShop`` dataset), but some of them
     don't (for example, ``CARS196`` or ``CUB200``).
     The validation idea for the latter is to calculate the embeddings for the whole validation set,
     then for every item find ``top-k`` nearest neighbors and calculate the desired retrieval metric.
     In other words, for the desired query item, the gallery is the rest of the validation dataset.
 
     Thus, if you want to perform this kind of validation process (`1 vs rest`) you should simply return
-    ``is_query == True`` and ``is_gallery == True`` for every item in the dataset sa the same time.
+    ``is_query == True`` and ``is_gallery == True`` for every item in the dataset as the same time.
 
     """
 
     def __init__(
         self,
         df: pd.DataFrame,
         extra_data: Optional[Dict[str, Any]] = None,
```

### Comparing `open-metric-learning-0.4.2/oml/datasets/list_dataset.py` & `open-metric-learning-0.4.3/oml/datasets/list_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/datasets/pairs.py` & `open-metric-learning-0.4.3/oml/datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/datasets/triplet.py` & `open-metric-learning-0.4.3/oml/datasets/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/ddp/patching.py` & `open-metric-learning-0.4.3/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/ddp/utils.py` & `open-metric-learning-0.4.3/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/functional/label_smoothing.py` & `open-metric-learning-0.4.3/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/functional/losses.py` & `open-metric-learning-0.4.3/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/functional/metrics.py` & `open-metric-learning-0.4.3/oml/functional/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/inference/abstract.py` & `open-metric-learning-0.4.3/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/inference/flat.py` & `open-metric-learning-0.4.3/oml/inference/flat.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/inference/pairs.py` & `open-metric-learning-0.4.3/oml/inference/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/criterions.py` & `open-metric-learning-0.4.3/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/datasets.py` & `open-metric-learning-0.4.3/oml/interfaces/datasets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/metrics.py` & `open-metric-learning-0.4.3/oml/interfaces/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/miners.py` & `open-metric-learning-0.4.3/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/models.py` & `open-metric-learning-0.4.3/oml/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/retrieval.py` & `open-metric-learning-0.4.3/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/interfaces/samplers.py` & `open-metric-learning-0.4.3/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/callbacks/metric.py` & `open-metric-learning-0.4.3/oml/lightning/callbacks/metric.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/modules/ddp.py` & `open-metric-learning-0.4.3/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/modules/extractor.py` & `open-metric-learning-0.4.3/oml/lightning/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/modules/pairwise_postprocessing.py` & `open-metric-learning-0.4.3/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/pipelines/parser.py` & `open-metric-learning-0.4.3/oml/lightning/pipelines/parser.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/pipelines/predict.py` & `open-metric-learning-0.4.3/oml/lightning/pipelines/predict.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/pipelines/train.py` & `open-metric-learning-0.4.3/oml/lightning/pipelines/train.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/pipelines/train_postprocessor.py` & `open-metric-learning-0.4.3/oml/lightning/pipelines/train_postprocessor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/lightning/pipelines/validate.py` & `open-metric-learning-0.4.3/oml/lightning/pipelines/validate.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/losses/arcface.py` & `open-metric-learning-0.4.3/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/losses/surrogate_precision.py` & `open-metric-learning-0.4.3/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/losses/triplet.py` & `open-metric-learning-0.4.3/oml/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/metrics/accumulation.py` & `open-metric-learning-0.4.3/oml/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/metrics/embeddings.py` & `open-metric-learning-0.4.3/oml/metrics/embeddings.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/metrics/triplets.py` & `open-metric-learning-0.4.3/oml/metrics/triplets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/cross_batch.py` & `open-metric-learning-0.4.3/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/inbatch_all_tri.py` & `open-metric-learning-0.4.3/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/inbatch_hard_cluster.py` & `open-metric-learning-0.4.3/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/inbatch_hard_tri.py` & `open-metric-learning-0.4.3/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/inbatch_nhard_tri.py` & `open-metric-learning-0.4.3/oml/miners/inbatch_nhard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/miner_with_bank.py` & `open-metric-learning-0.4.3/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/miners/pairs.py` & `open-metric-learning-0.4.3/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/models/meta/projection.py` & `open-metric-learning-0.4.3/oml/models/meta/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 from torchvision.ops import MLP
 
 from oml.const import STORAGE_CKPTS
 from oml.interfaces.models import IExtractor, IFreezable
 from oml.models.utils import remove_prefix_from_state_dict
-from oml.models.vit.vit import ViTExtractor
+from oml.models.vit_dino.extractor import ViTExtractor
 from oml.utils.io import download_checkpoint
 
 
 class ExtractorWithMLP(IExtractor, IFreezable):
     """
     Class-wrapper for extractors which an additional MLP.
```

### Comparing `open-metric-learning-0.4.2/oml/models/meta/siamese.py` & `open-metric-learning-0.4.3/oml/models/meta/siamese.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/models/pooling.py` & `open-metric-learning-0.4.3/oml/models/resnet/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/models/resnet.py` & `open-metric-learning-0.4.3/oml/models/resnet/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from PIL.Image import Image as TPILImage
 from pytorch_grad_cam import GradCAM
 from pytorch_grad_cam.utils.image import show_cam_on_image
 from torch import nn
 from torchvision.models import resnet18, resnet34, resnet50, resnet101, resnet152
 
 from oml.interfaces.models import IExtractor
-from oml.models.pooling import GEM
+from oml.models.resnet.pooling import GEM
 from oml.models.utils import remove_prefix_from_state_dict
 from oml.transforms.images.albumentations import get_normalisation_albu
 from oml.utils.io import download_checkpoint
 from oml.utils.misc_torch import get_device, normalise
 
 
 def resnet50_projector() -> nn.Module:
```

### Comparing `open-metric-learning-0.4.2/oml/models/utils.py` & `open-metric-learning-0.4.3/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/models/vit/clip.py` & `open-metric-learning-0.4.3/oml/models/vit_clip/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Any, Dict, Iterable, Optional
 
 import torch
 
 from oml.interfaces.models import IExtractor
 from oml.models.utils import TStateDict, filter_state_dict, patch_device_and_float
-from oml.models.vit.vision_transformer_clip import VisionTransformer
+from oml.models.vit_clip.external.model import VisionTransformer
 from oml.utils.io import download_checkpoint
 
 _OPENAI_URL = "https://openaipublic.azureedge.net/clip/models"
 _SBER_URL = "https://huggingface.co/sberbank-ai"
 
 
 def vitb16_224() -> VisionTransformer:
```

### Comparing `open-metric-learning-0.4.2/oml/models/vit/hubconf.py` & `open-metric-learning-0.4.3/oml/models/vit_dino/external/hubconf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import torch
 from torchvision.models.resnet import resnet50
 
-import oml.models.vit.vision_transformer as vits
+import oml.models.vit_dino.external.vision_transformer as vits
 
 dependencies = ["torch", "torchvision"]
 
 
 def dino_vits16(pretrained=True, **kwargs):
     """
     ViT-Small/16x16 pre-trained with DINO.
```

### Comparing `open-metric-learning-0.4.2/oml/models/vit/vision_transformer.py` & `open-metric-learning-0.4.3/oml/models/vit_dino/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/models/vit/vision_transformer_clip.py` & `open-metric-learning-0.4.3/oml/models/vit_clip/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/models/vit/vit.py` & `open-metric-learning-0.4.3/oml/models/vit_dino/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from PIL.Image import Image as TPILImage
 from pytorch_grad_cam.utils.image import show_cam_on_image
 from torch import nn
 
 from oml.const import MEAN, STD, STORAGE_CKPTS, TNormParam
 from oml.interfaces.models import IExtractor
 from oml.models.utils import remove_prefix_from_state_dict
-from oml.models.vit.hubconf import (  # type: ignore
+from oml.models.vit_dino.external.hubconf import (  # type: ignore
     dino_vitb8,
     dino_vitb16,
     dino_vits8,
     dino_vits16,
 )
 from oml.transforms.images.albumentations import get_normalisation_albu
 from oml.utils.io import download_checkpoint_one_of
```

### Comparing `open-metric-learning-0.4.2/oml/registry/__init__.py` & `open-metric-learning-0.4.3/oml/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/losses.py` & `open-metric-learning-0.4.3/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/miners.py` & `open-metric-learning-0.4.3/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/models.py` & `open-metric-learning-0.4.3/oml/registry/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from oml.interfaces.models import IExtractor, IPairwiseModel
 from oml.models.meta.projection import ExtractorWithMLP
 from oml.models.meta.siamese import (
     ConcatSiamese,
     LinearTrivialDistanceSiamese,
     TrivialDistanceSiamese,
 )
-from oml.models.resnet import ResnetExtractor
-from oml.models.vit.clip import ViTCLIPExtractor
-from oml.models.vit.vit import ViTExtractor
+from oml.models.resnet.extractor import ResnetExtractor
+from oml.models.vit_clip.extractor import ViTCLIPExtractor
+from oml.models.vit_dino.extractor import ViTExtractor
+from oml.models.vit_unicom.extractor import ViTUnicomExtractor
 from oml.utils.misc import TCfg, dictconfig_to_dict
 
 EXTRACTORS_REGISTRY = {
     "resnet": ResnetExtractor,
     "vit": ViTExtractor,
     "vit_clip": ViTCLIPExtractor,
+    "vit_unicom": ViTUnicomExtractor,
     "extractor_with_mlp": ExtractorWithMLP,
 }
 
 PAIRWISE_MODELS_REGISTRY = {
     "linear_siamese": LinearTrivialDistanceSiamese,
     "concat_siamese": ConcatSiamese,
     "trivial_distance_siamese": TrivialDistanceSiamese,
```

### Comparing `open-metric-learning-0.4.2/oml/registry/optimizers.py` & `open-metric-learning-0.4.3/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/postprocessors.py` & `open-metric-learning-0.4.3/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/samplers.py` & `open-metric-learning-0.4.3/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/schedulers.py` & `open-metric-learning-0.4.3/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/registry/transforms.py` & `open-metric-learning-0.4.3/oml/registry/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, Tuple
 
+import oml.models.vit_unicom.external.vision_transformer as unicom  # type: ignore
 from oml.transforms.images.albumentations import (
     get_augs_albu,
     get_normalisation_albu,
     get_normalisation_resize_albu,
     get_normalisation_resize_albu_clip,
 )
 from oml.transforms.images.torchvision import (
@@ -26,14 +27,15 @@
 
 TRANSFORMS_TORCH = {
     "augs_torch": get_augs_torch,
     "norm_torch": get_normalisation_torch,
     "norm_resize_torch": get_normalisation_resize_torch,
     "augs_hypvit_torch": get_augs_hypvit,
     "norm_resize_hypvit_torch": get_normalisation_resize_hypvit,
+    "unicom_transforms": unicom.transform,  # type: ignore
 }
 
 TRANSFORMS_REGISTRY = {**TRANSFORMS_ALBU, **TRANSFORMS_TORCH}
 
 
 def get_transforms(name: str, **kwargs: Dict[str, Any]) -> TTransforms:
     augs = TRANSFORMS_REGISTRY[name](**kwargs)  # type: ignore
@@ -64,14 +66,18 @@
     "openai_vitl14_224": get_normalisation_resize_albu_clip(im_size=224),
     "openai_vitl14_336": get_normalisation_resize_albu_clip(im_size=224),
     "vits16_inshop": get_normalisation_resize_hypvit(im_size=224, crop_size=224),
     "vits16_sop": get_normalisation_resize_hypvit(im_size=224, crop_size=224),
     "vits16_cars": get_normalisation_resize_albu(im_size=224),
     "vits16_cub": get_normalisation_resize_albu(im_size=224),
     "vits16_224_mlp_384_inshop": get_normalisation_resize_hypvit(im_size=256, crop_size=224),
+    "vitb32_unicom": unicom.transform(224),  # type: ignore
+    "vitb16_unicom": unicom.transform(224),  # type: ignore
+    "vitl14_unicom": unicom.transform(224),  # type: ignore
+    "vitl14_336px_unicom": unicom.transform(336),  # type: ignore
 }
 
 
 def get_transforms_for_pretrained(weights: str) -> Tuple[TTransforms, TImReader]:
     transforms = TRANSFORMS_FOR_PRETRAINED[weights]
     im_reader = get_im_reader_for_transforms(transforms)
     return transforms, im_reader
```

### Comparing `open-metric-learning-0.4.2/oml/retrieval/postprocessors/pairwise.py` & `open-metric-learning-0.4.3/oml/retrieval/postprocessors/pairwise.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/samplers/balance.py` & `open-metric-learning-0.4.3/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/samplers/category_balance.py` & `open-metric-learning-0.4.3/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/samplers/distinct_category_balance.py` & `open-metric-learning-0.4.3/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/transforms/images/albumentations.py` & `open-metric-learning-0.4.3/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/transforms/images/torchvision.py` & `open-metric-learning-0.4.3/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/dataframe_format.py` & `open-metric-learning-0.4.3/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/download_mock_dataset.py` & `open-metric-learning-0.4.3/oml/utils/download_mock_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/images/images.py` & `open-metric-learning-0.4.3/oml/utils/images/images.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/images/images_resize.py` & `open-metric-learning-0.4.3/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/io.py` & `open-metric-learning-0.4.3/oml/utils/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,19 +104,25 @@
     """
     CKPT_SAVE_ROOT.mkdir(exist_ok=True, parents=True)
 
     fname = fname if fname else Path(url_or_fid).name
     save_path = str(CKPT_SAVE_ROOT / fname)
 
     if Path(save_path).exists():
-        if calc_file_hash(save_path).startswith(hash_md5):
+        actual_hash = calc_file_hash(save_path)
+        if actual_hash.startswith(hash_md5):
             print("Checkpoint is already here.")
             return save_path
         else:
-            print("Checkpoint is already here, but hashed don't match. " "We will remove the old checkpoint.")
+            print(
+                f"Checkpoint is already here, but hashes don't match. "
+                f"{actual_hash} != {hash_md5}."
+                f"We will remove the old checkpoint: "
+                f"{save_path}."
+            )
             Path(save_path).unlink()
 
     print("Downloading checkpoint...")
 
     if validators.url(url_or_fid):
         download_file_from_url(url=url_or_fid, fname=save_path)
     else:  # we assume we work with file id (Google Drive)
```

### Comparing `open-metric-learning-0.4.2/oml/utils/misc.py` & `open-metric-learning-0.4.3/oml/utils/misc.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/misc_torch.py` & `open-metric-learning-0.4.3/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/oml/utils/remote_storage.py` & `open-metric-learning-0.4.3/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/open_metric_learning.egg-info/PKG-INFO` & `open-metric-learning-0.4.3/open_metric_learning.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 0.4.2
+Version: 0.4.3
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -292,15 +292,15 @@
 ```python
 import torch
 from tqdm import tqdm
 
 from oml.datasets.base import DatasetWithLabels
 from oml.losses.triplet import TripletLossWithMiner
 from oml.miners.inbatch_all_tri import AllTripletsMiner
-from oml.models.vit.vit import ViTExtractor
+from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
 
 dataset_root = "mock_dataset/"
 df_train, _ = download_mock_dataset(dataset_root)
 
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).train()
@@ -324,14 +324,114 @@
 ```
 [comment]:vanilla-train-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kntDAIdIZ9L40jcndguLAb-XqmCFOgS5?usp=sharing)
 <details>
+<summary>Validation</summary>
+<p>
+
+[comment]:vanilla-validation-start
+```python
+import torch
+from tqdm import tqdm
+
+from oml.datasets.base import DatasetQueryGallery
+from oml.metrics.embeddings import EmbeddingMetrics
+from oml.models import ViTExtractor
+from oml.utils.download_mock_dataset import download_mock_dataset
+
+dataset_root = "mock_dataset/"
+_, df_val = download_mock_dataset(dataset_root)
+
+extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).eval()
+
+val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
+
+val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
+calculator = EmbeddingMetrics(extra_keys=("paths",))
+calculator.setup(num_samples=len(val_dataset))
+
+with torch.no_grad():
+    for batch in tqdm(val_loader):
+        batch["embeddings"] = extractor(batch["input_tensors"])
+        calculator.update_data(batch)
+
+metrics = calculator.compute_metrics()
+
+# Logging
+print(calculator.metrics)  # metrics
+print(calculator.metrics_unreduced)  # metrics without averaging over queries
+
+# Visualisation
+calculator.get_plot_for_queries(query_ids=[0, 2], n_instances=5)  # draw predictions on predefined queries
+calculator.get_plot_for_worst_queries(metric_name="OVERALL/map/5", n_queries=2, n_instances=5)  # draw mistakes
+calculator.visualize()  # draw mistakes for all the available metrics
+
+```
+[comment]:vanilla-validation-end
+</p>
+</details>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1O2o3k8I8jN5hRin3dKnAS3WsgG04tmIT?usp=sharing)
+<details>
+<summary>Training + Validation [Lightning and Neptune logging]</summary>
+<p>
+
+[comment]:lightning-start
+```python
+import pytorch_lightning as pl
+import torch
+
+from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels
+from oml.lightning.modules.extractor import ExtractorModule
+from oml.lightning.callbacks.metric import MetricValCallback
+from oml.losses.triplet import TripletLossWithMiner
+from oml.metrics.embeddings import EmbeddingMetrics
+from oml.miners.inbatch_all_tri import AllTripletsMiner
+from oml.models import ViTExtractor
+from oml.samplers.balance import BalanceSampler
+from oml.utils.download_mock_dataset import download_mock_dataset
+from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger
+
+dataset_root = "mock_dataset/"
+df_train, df_val = download_mock_dataset(dataset_root)
+
+# model
+extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
+
+# train
+optimizer = torch.optim.SGD(extractor.parameters(), lr=1e-6)
+train_dataset = DatasetWithLabels(df_train, dataset_root=dataset_root)
+criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner())
+batch_sampler = BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=3)
+train_loader = torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler)
+
+# val
+val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
+val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
+metric_callback = MetricValCallback(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]), log_images=True)
+
+# logging
+logger = TensorBoardLogger(".")  # For TensorBoard
+# logger = NeptuneLogger(api_key="", project="", log_model_checkpoints=False)  # For Neptune
+
+# run
+pl_model = ExtractorModule(extractor, criterion, optimizer)
+trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
+trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
+
+```
+[comment]:lightning-end
+</p>
+</details>
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link)
+<details>
 <summary>Using a trained model for retrieval</summary>
 <p>
 
 [comment]:usage-retrieval-start
 ```python
 import torch
 
@@ -404,28 +504,36 @@
 |  `ViTExtractor.from_pretrained("vits16_sop")`   | 0.866 | Stanford Online Products |   [link](https://drive.google.com/file/d/1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A/view?usp=sharing)      |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_sop)   |
 | `ViTExtractor.from_pretrained("vits16_cars")`   | 0.907 |         CARS 196         |   [link](https://drive.google.com/drive/folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cars)  |
 |  `ViTExtractor.from_pretrained("vits16_cub")`   | 0.837 |       CUB 200 2011       |   [link](https://drive.google.com/drive/folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cub)   |
 
 We also provide an integration with the models pretrained by other researchers.
 All metrics below were obtained on the images with the sizes of **224 x 224**:
 
-|                            model                            | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
-|:-----------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
-|    `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")`    |          0.547           |       0.514        |    0.448     |  0.618   |
-|    `ViTCLIPExtractor.from_pretrained("sber_vitb16_224")`    |          0.565           |       0.565        |    0.524     |  0.648   |
-|    `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")`    |          0.512           |       0.555        |    0.606     |  0.707   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`   |          0.612           |       0.491        |    0.560     |  0.693   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`   |          0.648           |       0.606        |    0.665     |  0.767   |
-|   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`   |          0.670           |       0.675        |    0.745     |  0.844   |
-|        `ViTExtractor.from_pretrained("vits16_dino")`        |          0.648           |       0.509        |    0.627     |  0.265   |
-|        `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
-|        `ViTExtractor.from_pretrained("vitb16_dino")`        |          0.658           |       0.514        |    0.541     |  0.288   |
-|        `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
-|    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`    |          0.493           |       0.267        |    0.264     |  0.149   |
-| `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")` |          0.515           |       0.284        |    0.455     |  0.247   |
+|                            model                             | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
+|:------------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
+|    `ViTUnicomExtractor.from_pretrained("vitb16_unicom")`     |          0.700           |       0.734        |    0.847     |  0.916   |
+|    `ViTUnicomExtractor.from_pretrained("vitb32_unicom")`     |          0.690           |       0.722        |    0.796     |  0.893   |
+|    `ViTUnicomExtractor.from_pretrained("vitl14_unicom")`     |          0.726           |       0.790        |    0.868     |  0.922   |
+| `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`  |          0.745           |       0.810        |    0.875     |  0.924   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")`     |          0.547           |       0.514        |    0.448     |  0.618   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitb16_224")`     |          0.565           |       0.565        |    0.524     |  0.648   |
+|    `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")`     |          0.512           |       0.555        |    0.606     |  0.707   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`    |          0.612           |       0.491        |    0.560     |  0.693   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`    |          0.648           |       0.606        |    0.665     |  0.767   |
+|   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`    |          0.670           |       0.675        |    0.745     |  0.844   |
+|        `ViTExtractor.from_pretrained("vits16_dino")`         |          0.648           |       0.509        |    0.627     |  0.265   |
+|         `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
+|        `ViTExtractor.from_pretrained("vitb16_dino")`         |          0.658           |       0.514        |    0.541     |  0.288   |
+|         `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
+|    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`     |          0.493           |       0.267        |    0.264     |  0.149   |
+| `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")`  |          0.515           |       0.284        |    0.455     |  0.247   |
+
+**The metrics may be different from the ones reported by papers,
+because the version of train/val split and usage of bounding boxes may differ.
+Particularly, we used bounding boxes during the evaluation.*
 
 ### How to use models from Zoo?
 
 [comment]:zoo-start
 ```python
 from oml.const import CKPT_SAVE_ROOT as CKPT_DIR, MOCK_DATASET_PATH as DATA_DIR
 from oml.models import ViTExtractor
```

### Comparing `open-metric-learning-0.4.2/open_metric_learning.egg-info/SOURCES.txt` & `open-metric-learning-0.4.3/open_metric_learning.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 oml/configs/criterion/triplet.yaml
 oml/configs/criterion/triplet_plain.yaml
 oml/configs/criterion/triplet_with_miner.yaml
 oml/configs/extractor/extractor_with_mlp.yaml
 oml/configs/extractor/resnet.yaml
 oml/configs/extractor/vit.yaml
 oml/configs/extractor/vit_clip.yaml
+oml/configs/extractor/vit_unicom.yaml
 oml/configs/miner/all_triplets.yaml
 oml/configs/miner/hard_cluster.yaml
 oml/configs/miner/hard_triplets.yaml
 oml/configs/miner/miner_with_bank.yaml
 oml/configs/miner/n_hard_triplets.yaml
 oml/configs/miner/triplets_with_memory.yaml
 oml/configs/optimizer/adadelta.yaml
@@ -54,14 +55,15 @@
 oml/configs/transforms/augs_torch.yaml
 oml/configs/transforms/norm_albu.yaml
 oml/configs/transforms/norm_resize_albu.yaml
 oml/configs/transforms/norm_resize_albu_clip.yaml
 oml/configs/transforms/norm_resize_hypvit_torch.yaml
 oml/configs/transforms/norm_resize_torch.yaml
 oml/configs/transforms/norm_torch.yaml
+oml/configs/transforms/unicom_transforms.yaml
 oml/datasets/__init__.py
 oml/datasets/base.py
 oml/datasets/list_dataset.py
 oml/datasets/pairs.py
 oml/datasets/triplet.py
 oml/ddp/__init__.py
 oml/ddp/patching.py
@@ -108,26 +110,35 @@
 oml/miners/inbatch_all_tri.py
 oml/miners/inbatch_hard_cluster.py
 oml/miners/inbatch_hard_tri.py
 oml/miners/inbatch_nhard_tri.py
 oml/miners/miner_with_bank.py
 oml/miners/pairs.py
 oml/models/__init__.py
-oml/models/pooling.py
-oml/models/resnet.py
 oml/models/utils.py
 oml/models/meta/__init__.py
 oml/models/meta/projection.py
 oml/models/meta/siamese.py
-oml/models/vit/__init__.py
-oml/models/vit/clip.py
-oml/models/vit/hubconf.py
-oml/models/vit/vision_transformer.py
-oml/models/vit/vision_transformer_clip.py
-oml/models/vit/vit.py
+oml/models/resnet/__init__.py
+oml/models/resnet/extractor.py
+oml/models/resnet/pooling.py
+oml/models/vit_clip/__init__.py
+oml/models/vit_clip/extractor.py
+oml/models/vit_clip/external/__init__.py
+oml/models/vit_clip/external/model.py
+oml/models/vit_dino/__init__.py
+oml/models/vit_dino/extractor.py
+oml/models/vit_dino/external/__init__.py
+oml/models/vit_dino/external/hubconf.py
+oml/models/vit_dino/external/vision_transformer.py
+oml/models/vit_unicom/__init__.py
+oml/models/vit_unicom/extractor.py
+oml/models/vit_unicom/external/__init__.py
+oml/models/vit_unicom/external/model.py
+oml/models/vit_unicom/external/vision_transformer.py
 oml/registry/__init__.py
 oml/registry/losses.py
 oml/registry/miners.py
 oml/registry/models.py
 oml/registry/optimizers.py
 oml/registry/postprocessors.py
 oml/registry/samplers.py
```

### Comparing `open-metric-learning-0.4.2/setup.py` & `open-metric-learning-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/tests/test_build_readme.py` & `open-metric-learning-0.4.3/tests/test_build_readme.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/tests/test_imports.py` & `open-metric-learning-0.4.3/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.2/tests/test_outdated_docs.py` & `open-metric-learning-0.4.3/tests/test_outdated_docs.py`

 * *Files identical despite different names*

