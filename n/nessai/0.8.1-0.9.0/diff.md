# Comparing `tmp/nessai-0.8.1.tar.gz` & `tmp/nessai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai-0.8.1.tar", last modified: Fri Apr 14 10:22:16 2023, max compression
+gzip compressed data, was "nessai-0.9.0.tar", last modified: Sun Jul  2 09:21:34 2023, max compression
```

## Comparing `nessai-0.8.1.tar` & `nessai-0.9.0.tar`

### file list

```diff
@@ -1,226 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.907367 nessai-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.847367 nessai-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.855367 nessai-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.859367 nessai-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/compatibility-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 10:22:03.000000 nessai-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-14 10:22:03.000000 nessai-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-14 10:22:03.000000 nessai-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    38342 2023-04-14 10:22:03.000000 nessai-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 10:22:03.000000 nessai-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-14 10:22:03.000000 nessai-0.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-14 10:22:16.907367 nessai-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-14 10:22:03.000000 nessai-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 10:22:03.000000 nessai-0.8.1/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.863367 nessai-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.863367 nessai-0.8.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/insertion_indices.png
--rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/logXlogL.png
--rw-r--r--   0 runner    (1001) docker     (123)    70482 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/posterior_distribution.png
--rw-r--r--   0 runner    (1001) docker     (123)   159636 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/state.png
--rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/trace.png
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/bilby-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/further-details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/gaussian-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/gravitational-wave-inference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/normalising-flows-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/parallelisation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/reparameterisations.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/running-the-sampler.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/sampler-configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.867367 nessai-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/2d_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/augmented_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/bilby_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/bilby_unbounded_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/corner_plot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/eggbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.867367 nessai-0.8.1/examples/gw/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/gw/basic_gw_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/gw/calibration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/gw/full_gw_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/half_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/parallelisation_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/reparameterisations_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/unbounded_prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.871367 nessai-0.8.1/nessai/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/evidence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.875367 nessai-0.8.1/nessai/flowmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.875367 nessai-0.8.1/nessai/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/realnvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.879367 nessai-0.8.1/nessai/gw/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/reparameterisations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/livepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/nestedsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.879367 nessai-0.8.1/nessai/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/augmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    57696 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/flowproposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.883367 nessai-0.8.1/nessai/reparameterisations/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/null.py
--rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.883367 nessai-0.8.1/nessai/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/samplers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    47635 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/samplers/nestedsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.887367 nessai-0.8.1/nessai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/bilbyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/torchutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.871367 nessai-0.8.1/nessai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 10:22:03.000000 nessai-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 10:22:03.000000 nessai-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-14 10:22:16.911367 nessai-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 10:22:03.000000 nessai-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.891367 nessai-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_bilby_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_evidence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.891367 nessai-0.8.1/tests/test_flowmodel/
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flowmodel/test_flowmodel_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flowmodel/test_flowmodel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.891367 nessai-0.8.1/tests/test_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_flow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_included_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_specific_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    21368 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flowsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.895367 nessai-0.8.1/tests/test_gw/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_distance_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_gw_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_gw_reparameterisations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_reparameterisation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_livepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.895367 nessai-0.8.1/tests/test_proposal/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_augmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_base_proposal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.899367 nessai-0.8.1/tests/test_proposal/test_flowproposal/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.899367 nessai-0.8.1/tests/test_reparameterisations/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_angle_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_base_reparameterisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_get_reparameterisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    36520 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_rescale_to_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_scale_and_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_to_cartesian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.899367 nessai-0.8.1/tests/test_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_base_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.903367 nessai-0.8.1/tests/test_samplers/test_nested_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_core_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_general_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_live_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_manage_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_proposal_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_yield_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.907367 nessai-0.8.1/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_bilbyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_distance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_distribution_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_hist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_rescaling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_sampling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_sorting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_stats_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_structures_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_threading_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_torchtutils_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.174573 nessai-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.090571 nessai-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.102571 nessai-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.102571 nessai-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/compatibility-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-02 09:21:24.000000 nessai-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-02 09:21:24.000000 nessai-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 09:21:24.000000 nessai-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    39295 2023-07-02 09:21:24.000000 nessai-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-02 09:21:24.000000 nessai-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-02 09:21:24.000000 nessai-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-02 09:21:34.174573 nessai-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-02 09:21:24.000000 nessai-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-02 09:21:24.000000 nessai-0.9.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-02 09:21:24.000000 nessai-0.9.0/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.106571 nessai-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.110571 nessai-0.9.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/insertion_indices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/logXlogL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70482 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/posterior_distribution.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159636 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/state.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/trace.png
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/bilby-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/further-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/gaussian-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/gravitational-wave-inference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/importance-nested-sampling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/normalising-flows-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/parallelisation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/reparameterisations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/running-the-sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/sampler-configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.114571 nessai-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/2d_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/augmented_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/bilby_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/bilby_unbounded_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/corner_plot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/eggbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.114571 nessai-0.9.0/examples/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/gw/basic_gw_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/gw/calibration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/gw/full_gw_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/half_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.114571 nessai-0.9.0/examples/importance_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/importance_nested_sampler/basic_ins_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/importance_nested_sampler/nsf_unit_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/parallelisation_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/reparameterisations_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/unbounded_prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.118572 nessai-0.9.0/nessai/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/evidence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.122572 nessai-0.9.0/nessai/flowmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.126572 nessai-0.9.0/nessai/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/realnvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.126572 nessai-0.9.0/nessai/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/reparameterisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/livepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/nestedsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.130572 nessai-0.9.0/nessai/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/augmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58980 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/flowproposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27273 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.130572 nessai-0.9.0/nessai/reparameterisations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.134572 nessai-0.9.0/nessai/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67237 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/importancesampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47766 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/nestedsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.138572 nessai-0.9.0/nessai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/bilbyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/torchutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.118572 nessai-0.9.0/nessai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-02 09:21:24.000000 nessai-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-02 09:21:24.000000 nessai-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-02 09:21:34.174573 nessai-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 09:21:24.000000 nessai-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.142572 nessai-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_bilby_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_deprecation_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.142572 nessai-0.9.0/tests/test_evidence/
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_evidence/test_ins_evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_evidence/test_standard_evidence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.142572 nessai-0.9.0/tests/test_flowmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowmodel/test_flowmodel_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowmodel/test_flowmodel_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowmodel/test_flowmodel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.146572 nessai-0.9.0/tests/test_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_base_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.146572 nessai-0.9.0/tests/test_flows/test_distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_distributions/test_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_distributions/test_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_flow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_included_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_specific_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.146572 nessai-0.9.0/tests/test_gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_distance_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_gw_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_gw_reparameterisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_reparameterisation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_livepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.150572 nessai-0.9.0/tests/test_proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_augmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_base_proposal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.154572 nessai-0.9.0/tests/test_proposal/test_flowproposal/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.154572 nessai-0.9.0/tests/test_proposal/test_importance/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.158572 nessai-0.9.0/tests/test_reparameterisations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_angle_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_base_reparameterisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_get_reparameterisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36520 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_rescale_to_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_scale_and_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_to_cartesian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.158572 nessai-0.9.0/tests/test_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_base_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.162572 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.166573 nessai-0.9.0/tests/test_samplers/test_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_core_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_flow_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_general_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_live_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_manage_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_ns_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_proposal_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_yield_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.166573 nessai-0.9.0/tests/test_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_sampling/test_ins_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_sampling/test_standard_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.174573 nessai-0.9.0/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_bilbyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_distance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_distribution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_hist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_information_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_optimise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_rescaling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_sampling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_sorting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_stats_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_structures_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_threading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_torchtutils_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_version.py
```

### Comparing `nessai-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `nessai-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/.github/workflows/compatibility-tests.yml` & `nessai-0.9.0/.github/workflows/compatibility-tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/.github/workflows/integration-tests.yml` & `nessai-0.9.0/.github/workflows/integration-tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,34 @@
   integration-tests:
     name: Integration tests - Python ${{ matrix.python-version }} (${{ matrix.os }})
 
     strategy:
       fail-fast: false
       matrix:
         os: [macOS, Ubuntu, Windows]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10"]
     runs-on: ${{ matrix.os }}-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -r requirements.txt
-        pip install -r dev_requirements.txt
-        pip install -e .
+        pip install .[test]
+        pip install .[dev,nflows]
+        pip install .[gw]
+    - name: Check dependencies
+      if: success() || failure()
+      run: |
+        python -m pip check
     - name: Set MPL backend on Windows
       if: runner.os == 'Windows'
       run: |
         echo "MPLBACKEND=agg" >> $env:GITHUB_ENV
     - name: Print environment variables
       run: |
         env
```

### Comparing `nessai-0.8.1/.github/workflows/lint.yml` & `nessai-0.9.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/.github/workflows/publish-to-pypi.yml` & `nessai-0.9.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/.github/workflows/tests.yml` & `nessai-0.9.0/.github/workflows/tests.yml`

 * *Files 20% similar despite different names*

```diff
@@ -14,30 +14,34 @@
   unittests:
     name: Unit tests - Python ${{ matrix.python-version }} (${{ matrix.os }})
 
     strategy:
       fail-fast: false
       matrix:
         os: [macOS, Ubuntu, Windows]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10"]
     runs-on: ${{ matrix.os }}-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -r requirements.txt
-        pip install -r dev_requirements.txt
-        pip install -e .
+        pip install .[test]
+        pip install .[dev,nflows]
+        pip install .[gw]
+    - name: Check dependencies
+      if: success() || failure()
+      run: |
+        python -m pip check
     - name: Set MPL backend on Windows
       if: runner.os == 'Windows'
       run: |
         echo "MPLBACKEND=agg" >> $env:GITHUB_ENV
     - name: Print environment variables
       run: |
         env
```

### Comparing `nessai-0.8.1/.gitignore` & `nessai-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/.pre-commit-config.yaml` & `nessai-0.9.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     -   id: check-yaml
     -   id: check-added-large-files
 -   repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
         language_version: python3
--   repo: https://gitlab.com/pycqa/flake8
+-   repo: https://github.com/pycqa/flake8
     rev: 3.8.3
     hooks:
     -   id: flake8
 -   repo: https://github.com/codespell-project/codespell
     rev: v2.1.0
     hooks:
     -   id: codespell
```

### Comparing `nessai-0.8.1/CHANGELOG.md` & `nessai-0.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.0]
+
+### Added
+
+- Add importance nested sampler ([#285](https://github.com/mj-will/nessai/pull/285))
+- Add support for using regex for specifying parameters in the reparametersations dictionary ([#312](https://github.com/mj-will/nessai/pull/312))
+
+
+### Changed
+
+- Enable constant volume mode with uniform nball latent prior ([#306](https://github.com/mj-will/nessai/pull/306))
+- Pass kwargs in RealNVP to the coupling class ([#307](https://github.com/mj-will/nessai/pull/307))
+- Use log-scale on state plot ([#308](https://github.com/mj-will/nessai/pull/308))
+- Support `forkserver` and `spawn` multiprocessing start methods ([#313](https://github.com/mj-will/nessai/pull/313))
+
+### Fixed
+
+- Fix resume bug with fallback reparameterisation ([#302](https://github.com/mj-will/nessai/pull/302))
+- Fix bugs caused by numpy 1.25 ([#311](https://github.com/mj-will/nessai/pull/311))
+
 ## [0.8.1]
 
 ### Fixed
 
 - Fix incorrect sign in delta phase reparameterisation ([#292](https://github.com/mj-will/nessai/pull/292))
 - Remove maximum scipy version ([#295](https://github.com/mj-will/nessai/pull/295))
 - Specify three quantiles in default corner kwargs as required by corner 2.2.2 ([#298](https://github.com/mj-will/nessai/pull/298))
@@ -493,15 +513,16 @@
 
 - Fix a bug where `maximum_uninformed` did not have the expected behaviour.
 
 ### Deprecated
 
 - Original `GWFlowProposal` method renamed to `LegacyGWFlowProposal`. Will be removed in the next release.
 
-[Unreleased]: https://github.com/mj-will/nessai/compare/v0.8.1...HEAD
+[Unreleased]: https://github.com/mj-will/nessai/compare/v0.9.0...HEAD
+[0.9.0]: https://github.com/mj-will/nessai/compare/v0.8.1...v0.9.0
 [0.8.1]: https://github.com/mj-will/nessai/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/mj-will/nessai/compare/v0.7.1...v0.8.0
 [0.7.1]: https://github.com/mj-will/nessai/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/mj-will/nessai/compare/v0.6.0...v0.7.0
 [0.6.0]: https://github.com/mj-will/nessai/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/mj-will/nessai/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/mj-will/nessai/compare/v0.4.0...v0.5.0
```

### Comparing `nessai-0.8.1/CONTRIBUTING.md` & `nessai-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/LICENSE.md` & `nessai-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/PKG-INFO` & `nessai-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nessai
-Version: 0.8.1
+Version: 0.9.0
 Summary: Nessai: Nested Sampling with Artificial Intelligence
 Home-page: https://github.com/mj-will/nessai
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 Project-URL: Documentation, https://nessai.readthedocs.io/
 Keywords: nested sampling,normalising flows,machine learning
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -30,15 +29,15 @@
 ![int-tests](https://github.com/mj-will/nessai/actions/workflows/integration-tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/mj-will/nessai/branch/main/graph/badge.svg?token=O7SN167SK6)](https://codecov.io/gh/mj-will/nessai)
 
 # nessai: Nested Sampling with Artificial Intelligence
 
 ``nessai`` (/ˈnɛsi/): Nested Sampling with Artificial Intelligence
 
-``nessai`` is a nested sampling algorithm for Bayesian Inference that incorporates normalisings flows. It is designed for applications where the Bayesian likelihood is computationally expensive.
+``nessai`` is a nested sampling algorithm for Bayesian Inference that incorporates normalising flows. It is designed for applications where the Bayesian likelihood is computationally expensive.
 
 ## Installation
 
 ``nessai`` can be installed using ``pip``:
 
 ```console
 pip install nessai
@@ -78,36 +77,47 @@
 
 Other code snippets that draw on existing code reference the source in their corresponding doc-strings.
 
 The authors also thank Christian Chapman-Bird, Laurence Datrier, Fergus Hayes, Jethro Linley and Simon Tait for their feedback and help finding bugs in ``nessai``.
 
 ## Citing
 
-If you find ``nessai`` useful in your work please cite the DOI for this code and our paper:
+If you find ``nessai`` useful in your work please cite the DOI for this code and our papers:
 
 ```bibtex
 @software{nessai,
   author       = {Michael J. Williams},
   title        = {nessai: Nested Sampling with Artificial Intelligence},
   month        = feb,
   year         = 2021,
   publisher    = {Zenodo},
   version      = {latest},
   doi          = {10.5281/zenodo.4550693},
   url          = {https://doi.org/10.5281/zenodo.4550693}
 }
 
-@article{PhysRevD.103.103006,
-  title = {Nested sampling with normalizing flows for gravitational-wave inference},
-  author = {Williams, Michael J. and Veitch, John and Messenger, Chris},
-  journal = {Phys. Rev. D},
-  volume = {103},
-  issue = {10},
-  pages = {103006},
-  numpages = {19},
-  year = {2021},
-  month = {May},
-  publisher = {American Physical Society},
-  doi = {10.1103/PhysRevD.103.103006},
-  url = {https://link.aps.org/doi/10.1103/PhysRevD.103.103006}
+@article{Williams:2021qyt,
+    author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+    title = "{Nested sampling with normalizing flows for gravitational-wave inference}",
+    eprint = "2102.11056",
+    archivePrefix = "arXiv",
+    primaryClass = "gr-qc",
+    doi = "10.1103/PhysRevD.103.103006",
+    journal = "Phys. Rev. D",
+    volume = "103",
+    number = "10",
+    pages = "103006",
+    year = "2021"
 }
+
+@article{Williams:2023ppp,
+    author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+    title = "{Importance nested sampling with normalising flows}",
+    eprint = "2302.08526",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    reportNumber = "LIGO-P2200283",
+    month = "2",
+    year = "2023"
+}
+
 ```
```

### Comparing `nessai-0.8.1/README.md` & `nessai-0.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ![int-tests](https://github.com/mj-will/nessai/actions/workflows/integration-tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/mj-will/nessai/branch/main/graph/badge.svg?token=O7SN167SK6)](https://codecov.io/gh/mj-will/nessai)
 
 # nessai: Nested Sampling with Artificial Intelligence
 
 ``nessai`` (/ˈnɛsi/): Nested Sampling with Artificial Intelligence
 
-``nessai`` is a nested sampling algorithm for Bayesian Inference that incorporates normalisings flows. It is designed for applications where the Bayesian likelihood is computationally expensive.
+``nessai`` is a nested sampling algorithm for Bayesian Inference that incorporates normalising flows. It is designed for applications where the Bayesian likelihood is computationally expensive.
 
 ## Installation
 
 ``nessai`` can be installed using ``pip``:
 
 ```console
 pip install nessai
@@ -55,36 +55,47 @@
 
 Other code snippets that draw on existing code reference the source in their corresponding doc-strings.
 
 The authors also thank Christian Chapman-Bird, Laurence Datrier, Fergus Hayes, Jethro Linley and Simon Tait for their feedback and help finding bugs in ``nessai``.
 
 ## Citing
 
-If you find ``nessai`` useful in your work please cite the DOI for this code and our paper:
+If you find ``nessai`` useful in your work please cite the DOI for this code and our papers:
 
 ```bibtex
 @software{nessai,
   author       = {Michael J. Williams},
   title        = {nessai: Nested Sampling with Artificial Intelligence},
   month        = feb,
   year         = 2021,
   publisher    = {Zenodo},
   version      = {latest},
   doi          = {10.5281/zenodo.4550693},
   url          = {https://doi.org/10.5281/zenodo.4550693}
 }
 
-@article{PhysRevD.103.103006,
-  title = {Nested sampling with normalizing flows for gravitational-wave inference},
-  author = {Williams, Michael J. and Veitch, John and Messenger, Chris},
-  journal = {Phys. Rev. D},
-  volume = {103},
-  issue = {10},
-  pages = {103006},
-  numpages = {19},
-  year = {2021},
-  month = {May},
-  publisher = {American Physical Society},
-  doi = {10.1103/PhysRevD.103.103006},
-  url = {https://link.aps.org/doi/10.1103/PhysRevD.103.103006}
+@article{Williams:2021qyt,
+    author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+    title = "{Nested sampling with normalizing flows for gravitational-wave inference}",
+    eprint = "2102.11056",
+    archivePrefix = "arXiv",
+    primaryClass = "gr-qc",
+    doi = "10.1103/PhysRevD.103.103006",
+    journal = "Phys. Rev. D",
+    volume = "103",
+    number = "10",
+    pages = "103006",
+    year = "2021"
 }
+
+@article{Williams:2023ppp,
+    author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+    title = "{Importance nested sampling with normalising flows}",
+    eprint = "2302.08526",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    reportNumber = "LIGO-P2200283",
+    month = "2",
+    year = "2023"
+}
+
 ```
```

### Comparing `nessai-0.8.1/docs/Makefile` & `nessai-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/assets/insertion_indices.png` & `nessai-0.9.0/docs/assets/insertion_indices.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/assets/logXlogL.png` & `nessai-0.9.0/docs/assets/logXlogL.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/assets/posterior_distribution.png` & `nessai-0.9.0/docs/assets/posterior_distribution.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/assets/state.png` & `nessai-0.9.0/docs/assets/state.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/assets/trace.png` & `nessai-0.9.0/docs/assets/trace.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/conf.py` & `nessai-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/further-details.rst` & `nessai-0.9.0/docs/further-details.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/gaussian-example.rst` & `nessai-0.9.0/docs/gaussian-example.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/gravitational-wave-inference.rst` & `nessai-0.9.0/docs/gravitational-wave-inference.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/index.rst` & `nessai-0.9.0/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .. toctree::
    :maxdepth: 1
    :caption: Contents:
 
    installation
    running-the-sampler
    sampler-configuration
+   importance-nested-sampling
    reparameterisations
    normalising-flows-configuration
    parallelisation
    gravitational-wave-inference
    further-details
    API reference </autoapi/nessai/index>
 
@@ -52,15 +53,31 @@
       year         = 2021,
       publisher    = {Zenodo},
       version      = {latest},
       doi          = {10.5281/zenodo.4550693},
       url          = {https://doi.org/10.5281/zenodo.4550693}
     }
 
-    @article{williams2021nested,
-      title={Nested Sampling with Normalising Flows for Gravitational-Wave Inference},
-      author={Michael J. Williams and John Veitch and Chris Messenger},
-      year={2021},
-      eprint={2102.11056},
-      archivePrefix={arXiv},
-      primaryClass={gr-qc}
-    }
+    @article{Williams:2021qyt,
+      author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+      title = "{Nested sampling with normalizing flows for gravitational-wave inference}",
+      eprint = "2102.11056",
+      archivePrefix = "arXiv",
+      primaryClass = "gr-qc",
+      doi = "10.1103/PhysRevD.103.103006",
+      journal = "Phys. Rev. D",
+      volume = "103",
+      number = "10",
+      pages = "103006",
+      year = "2021"
+   }
+
+   @article{Williams:2023ppp,
+      author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+      title = "{Importance nested sampling with normalising flows}",
+      eprint = "2302.08526",
+      archivePrefix = "arXiv",
+      primaryClass = "astro-ph.IM",
+      reportNumber = "LIGO-P2200283",
+      month = "2",
+      year = "2023"
+   }
```

### Comparing `nessai-0.8.1/docs/installation.rst` & `nessai-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/normalising-flows-configuration.rst` & `nessai-0.9.0/docs/normalising-flows-configuration.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/parallelisation.rst` & `nessai-0.9.0/docs/parallelisation.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/reparameterisations.rst` & `nessai-0.9.0/docs/reparameterisations.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/running-the-sampler.rst` & `nessai-0.9.0/docs/running-the-sampler.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/docs/sampler-configuration.rst` & `nessai-0.9.0/docs/sampler-configuration.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-=====================
-Sampler configuration
-=====================
+==============================
+Standard sampler configuration
+==============================
+
+.. important::
+    Some of settings discussed here only apply to standard ``nessai`` not ``i-nessai``. For ``i-nessai`` see :ref:`Importance Nested Sampling`
 
 There are various settings in ``nessai`` which can be configured. These can be grouped in to general settings and proposal settings. The former controls general aspects of the sampler such as the model being sampler or how many live points are used. The latter affect the proposal process and how new points are drawn.
 
 All of the settings are controlled when creating an instance of :py:class:`~nessai.flowsampler.FlowSampler`. The most important settings to consider when using ``nessai`` are the :doc:`reparameterisations<reparameterisations>` used for the proposals.
 
 General configuration
 =====================
```

### Comparing `nessai-0.8.1/examples/2d_gaussian.py` & `nessai-0.9.0/examples/2d_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/augmented_example.py` & `nessai-0.9.0/examples/augmented_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/bilby_example.py` & `nessai-0.9.0/examples/bilby_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/bilby_unbounded_priors.py` & `nessai-0.9.0/examples/bilby_unbounded_priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/corner_plot_example.py` & `nessai-0.9.0/examples/corner_plot_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/eggbox.py` & `nessai-0.9.0/examples/eggbox.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/gw/basic_gw_example.py` & `nessai-0.9.0/examples/gw/basic_gw_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/gw/calibration_example.py` & `nessai-0.9.0/examples/gw/calibration_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,14 @@
 calib_phases = [
     "recalib_H1_phase_0",
     "recalib_L1_phase_0",
     "recalib_H1_phase_1",
     "recalib_L1_phase_1",
 ]
 
-calib_parameters = calib_amplitudes + calib_phases
-
 # Entry 8 is the detector (H or L)
 for name in calib_amplitudes:
     priors[name] = bilby.prior.Gaussian(
         mu=0, sigma=0.2, name=name, latex_label=f"{name[8]}1 $A_{name[-1]}$"
     )
 
 for name in calib_phases:
@@ -150,9 +148,9 @@
     conversion_function=bilby.gw.conversion.generate_all_bbh_parameters,
     injection_parameters=injection_parameters,
     outdir=outdir,
     label=label,
     plot=True,
     sampler="nessai",
     flow_class="gwflowproposal",
-    reparameterisations={"null": {"parameters": calib_parameters}},
+    reparameterisations={"z-score": {"parameters": "recalib.*"}},
 )
```

### Comparing `nessai-0.8.1/examples/gw/full_gw_example.py` & `nessai-0.9.0/examples/gw/full_gw_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/half_gaussian.py` & `nessai-0.9.0/examples/half_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/parallelisation_example.py` & `nessai-0.9.0/examples/parallelisation_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/reparameterisations_example.py` & `nessai-0.9.0/examples/reparameterisations_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/rosenbrock.py` & `nessai-0.9.0/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/examples/unbounded_prior.py` & `nessai-0.9.0/examples/unbounded_prior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/__init__.py` & `nessai-0.9.0/nessai/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 """nessai: Nested sampling with Artificial Intelligence
 
 nessai is a nested sampling algorithm for Bayesian Inference that incorporates
 normalising flows. It is designed for applications where the Bayesian
 likelihood is computationally expensive.
 """
 import logging
-
-try:
-    from importlib.metadata import version, PackageNotFoundError
-except ImportError:  # for Python < 3.8
-    from importlib_metadata import version, PackageNotFoundError
-
+from importlib.metadata import PackageNotFoundError, version
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:
     # package is not installed
     __version__ = "unknown"
```

### Comparing `nessai-0.8.1/nessai/config.py` & `nessai-0.9.0/nessai/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,9 +132,18 @@
     """Maximum figure size in either width or height.
 
     Based on the default DPI in matplotlib of 100, so this will give a maximum
     size of 5000 pixels.
     """
 
 
+@dataclass
+class GeneralConfig:
+    """General configuration options"""
+
+    eps: float = 1e-8
+    """Epsilon value used for numerical stability"""
+
+
 livepoints = LivepointsConfig()
 plotting = PlottingConfig()
+general = GeneralConfig()
```

### Comparing `nessai-0.8.1/nessai/flowmodel/base.py` & `nessai-0.9.0/nessai/flowmodel/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/flowmodel/config.py` & `nessai-0.9.0/nessai/flowmodel/config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/flowmodel/utils.py` & `nessai-0.9.0/nessai/flowmodel/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,49 @@
 """
 Utilities for configuring FlowModel.
 """
 from .config import DEFAULT_MODEL_CONFIG, DEFAULT_FLOW_CONFIG
 from ..flows.utils import get_n_neurons
 
 
+def update_model_config(d):
+    """Update the model (flow) configuration dictionary based on the defaults.
+
+    Parameters
+    ----------
+    d : Union[dict, None]
+        Dictionary with the current configuration. If None, then the default is
+        used.
+
+    Returns
+    -------
+    dict
+        Updated configuration dictionary.
+
+    Raises
+    ------
+    TypeError
+        Raised if the input is not a dictionary or None.
+    """
+    default = DEFAULT_MODEL_CONFIG.copy()
+    if d is None:
+        return default
+    elif not isinstance(d, dict):
+        raise TypeError(
+            "Must pass a dictionary to update the default model config"
+        )
+    else:
+        default.update(d)
+        default["n_neurons"] = get_n_neurons(
+            n_neurons=default.get("n_neurons"),
+            n_inputs=default.get("n_inputs"),
+        )
+    return default
+
+
 def update_config(d):
     """
     Update the configuration dictionary to include the defaults.
 
     Notes
     -----
     The default configuration is specified in :py:mod:`nessai.flowmodel.config`
@@ -25,32 +60,26 @@
 
     Returns
     -------
     dict
         Dictionary with updated default configuration
     """
     default = DEFAULT_FLOW_CONFIG.copy()
-    default_model = DEFAULT_MODEL_CONFIG.copy()
 
     if d is None:
-        default["model_config"] = default_model
+        default["model_config"] = update_model_config(None)
+    elif not isinstance(d, dict):
+        raise TypeError(
+            "Must pass a dictionary to update the default " "trainer settings"
+        )
     else:
-        if not isinstance(d, dict):
-            raise TypeError(
-                "Must pass a dictionary to update the default "
-                "trainer settings"
-            )
-        else:
-            default.update(d)
-            default_model.update(d.get("model_config", {}))
-            default_model["n_neurons"] = get_n_neurons(
-                n_neurons=default_model.get("n_neurons"),
-                n_inputs=default_model.get("n_inputs"),
-            )
-            default["model_config"] = default_model
+        default.update(d)
+        default["model_config"] = update_model_config(
+            default.get("model_config", None)
+        )
 
     if default["noise_type"] is not None and default["noise_scale"] is None:
         raise RuntimeError(
             "`noise_scale` must be specified when `noise_type` is given."
         )
     if isinstance(default["noise_scale"], float):
         if default["noise_type"] is None:
```

### Comparing `nessai-0.8.1/nessai/flows/base.py` & `nessai-0.9.0/nessai/flows/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/flows/distributions.py` & `nessai-0.9.0/nessai/flows/distributions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Distributions to use as the 'base distribution' for normalising flows.
 """
 import math
 
+from glasflow.distributions import (
+    ResampledGaussian as BaseResampledGaussian,
+)
 from glasflow.nflows.distributions import Distribution
 from glasflow.nflows.utils import torchutils
 import numpy as np
 import torch
 
 
 class MultivariateNormal(Distribution):
@@ -63,7 +66,27 @@
             raise NotImplementedError
 
     def _mean(self, context):
         if context is None:
             return self._log_z.new_zeros(self._shape)
         else:
             raise NotImplementedError
+
+
+class ResampledGaussian(BaseResampledGaussian):
+    """Wrapper for ResampledGaussian.
+
+    Adds methods needed in nessai.
+    """
+
+    end_iteration = BaseResampledGaussian.estimate_normalisation_constant
+    """Function to be called at the end of an iteration.
+
+    For LARS this updates the estimate of the normalisation constant
+    independently of the other parameters in the flow.
+    """
+
+    def finalise(self, n_samples: int = 10_000, n_batches: int = 10) -> None:
+        """Finalise the estimate of the normalisation constant."""
+        self.estimate_normalisation_constant(
+            n_samples=n_samples, n_batches=n_batches
+        )
```

### Comparing `nessai-0.8.1/nessai/flows/maf.py` & `nessai-0.9.0/nessai/flows/maf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/flows/nets.py` & `nessai-0.9.0/nessai/flows/nets.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/flows/nsf.py` & `nessai-0.9.0/nessai/flows/nsf.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,16 @@
        Enable or disable batch norm within the neural network for each coupling
        transform
     batch_norm_between_layers : bool, optional (False)
        Enable or disable batch norm between coupling transforms
     linear_transform : {'permutation', 'lu', 'svd'}
         Linear transform to use between coupling layers. Not recommended when
         using a custom mask.
+    distribution : :obj: `glasflow.nflows.distributions.Distribution`
+        Distribution for the latent space.
     kwargs : dict
         Additional kwargs parsed to the spline constructor, e.g. `tails` or
         `tail_bound`. See nflows for details
     """
 
     def __init__(
         self,
@@ -67,14 +69,15 @@
         dropout_probability=0.0,
         batch_norm_within_layers=False,
         batch_norm_between_layers=False,
         apply_unconditional_transform=False,
         linear_transform="permutation",
         tails="linear",
         tail_bound=5.0,
+        distribution=None,
         **kwargs,
     ):
 
         if features <= 1:
             raise ValueError(
                 "Coupling based Neural Spline flow requires at least 2 "
                 f"dimensions. Specified dimensions: {features}."
@@ -111,13 +114,14 @@
                 transforms_list.append(
                     create_linear_transform(linear_transform, features)
                 )
             transforms_list.append(spline_constructor(i))
             if batch_norm_between_layers:
                 transforms_list.append(transforms.BatchNorm(features=features))
 
-        distribution = StandardNormal([features])
+        if distribution is None:
+            distribution = StandardNormal([features])
 
         super().__init__(
             transform=transforms.CompositeTransform(transforms_list),
             distribution=distribution,
         )
```

### Comparing `nessai-0.8.1/nessai/flows/realnvp.py` & `nessai-0.9.0/nessai/flows/realnvp.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,19 @@
         Linear transform to use between coupling layers. Not recommended when
         using a custom mask.
     pre_transform : str
         Linear transform to use before the first transform.
     pre_transform_kwargs : dict
         Keyword arguments to pass to the transform class used for the pre-
         transform.
+    actnorm : bool
+        Include activation normalisation as described in arXiv:1807.03039.
+        Batch norm between layers must be disabled if using this option.
+    kwargs :
+        Keyword arguments are passed to the coupling class.
     """
 
     def __init__(
         self,
         features,
         hidden_features,
         num_layers,
@@ -81,23 +86,31 @@
         activation=F.relu,
         dropout_probability=0.0,
         batch_norm_within_layers=False,
         batch_norm_between_layers=False,
         linear_transform=None,
         pre_transform=None,
         pre_transform_kwargs=None,
+        actnorm=False,
         distribution=None,
+        **kwargs,
     ):
 
         if features <= 1:
             raise ValueError(
                 "RealNVP requires at least 2 dimensions. "
                 f"Specified dimensions: {features}."
             )
 
+        if actnorm and batch_norm_between_layers:
+            raise RuntimeError(
+                "Cannot enable actnorm and batchnorm between layers "
+                "simultaneously."
+            )
+
         if use_volume_preserving:
             coupling_constructor = transforms.AdditiveCouplingTransform
         else:
             coupling_constructor = transforms.AffineCouplingTransform
 
         if mask is None:
             mask = torch.ones(features)
@@ -168,20 +181,28 @@
             layers.append(
                 create_pre_transform(
                     pre_transform, features, **pre_transform_kwargs
                 )
             )
 
         for i in range(num_layers):
+
+            if actnorm:
+                layers.append(
+                    transforms.normalization.ActNorm(features=features)
+                )
+
             if linear_transform is not None:
                 layers.append(
                     create_linear_transform(linear_transform, features)
                 )
             transform = coupling_constructor(
-                mask=mask[i], transform_net_create_fn=create_net
+                mask=mask[i],
+                transform_net_create_fn=create_net,
+                **kwargs,
             )
             layers.append(transform)
             if batch_norm_between_layers:
                 layers.append(transforms.BatchNorm(features=features))
 
         if distribution is None:
             distribution = StandardNormal([features])
```

### Comparing `nessai-0.8.1/nessai/flows/transforms.py` & `nessai-0.9.0/nessai/flows/transforms.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/flows/utils.py` & `nessai-0.9.0/nessai/flows/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import inspect
 import logging
 from typing import Optional, Type, Union
 import warnings
 
 from glasflow.nflows import transforms
 from glasflow.nflows.distributions import Distribution
+from glasflow.distributions import MultivariateUniform
 import numpy as np
 import torch
 import torch.nn.functional as F
 
-from .distributions import MultivariateNormal
+from .distributions import MultivariateNormal, ResampledGaussian
+from .nets import MLP
 
 
 logger = logging.getLogger(__name__)
 
 
 def silu(x):
     """
@@ -45,29 +47,58 @@
         Distribution class or name of known distribution
     kwargs : Any
         Keyword arguments used when creating an instance of distribution.
     """
     distributions = {
         "mvn": MultivariateNormal,
         "normal": MultivariateNormal,
+        "lars": ResampledGaussian,
+        "resampled": ResampledGaussian,
+        "uniform": MultivariateUniform,
     }
 
     DistClass = None
 
     if isinstance(distribution, str):
         DistClass = distributions.get(distribution.lower())
         if not DistClass:
             raise ValueError(f"Unknown distribution: {distribution}")
     elif inspect.isclass(distribution):
         logger.debug("Distribution is class. Creating an instance.")
         DistClass = distribution
 
     if DistClass:
         logger.debug("Creating instance of the base distribution")
-        dist = DistClass([n_inputs], **kwargs)
+        if DistClass is ResampledGaussian:
+            n_layers = kwargs.pop("n_layers", 2)
+            n_neurons = get_n_neurons(
+                kwargs.pop("n_neurons", None), n_inputs=n_inputs
+            )
+            layers_list = n_layers * [n_neurons]
+            logger.debug(
+                f"LARS acceptance network will have {n_layers} layers with "
+                f"{n_neurons} neurons each."
+            )
+            net_kwargs = kwargs.pop("net_kwargs", {})
+            acc_fn = MLP(
+                [n_inputs],
+                [1],
+                layers_list,
+                activate_output=torch.sigmoid,
+                **net_kwargs,
+            )
+            logger.debug(f"Other LARs kwargs: {kwargs}")
+            dist = DistClass([n_inputs], acc_fn, **kwargs)
+        elif DistClass is MultivariateUniform:
+            dist = DistClass(
+                low=torch.zeros(n_inputs, dtype=torch.get_default_dtype()),
+                high=torch.ones(n_inputs, dtype=torch.get_default_dtype()),
+            )
+        else:
+            dist = DistClass([n_inputs], **kwargs)
     elif distribution is None:
         dist = None
     else:
         dist = distribution
     return dist
```

### Comparing `nessai-0.8.1/nessai/flowsampler.py` & `nessai-0.9.0/nessai/samplers/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,356 +1,339 @@
 # -*- coding: utf-8 -*-
-"""
-Main code that handles running and checkpoiting the sampler.
-"""
+"""Base nested sampler object"""
+from abc import ABC, abstractmethod
+import datetime
 import logging
 import os
-import signal
-import sys
-from typing import Optional
-
-from .livepoint import live_points_to_dict
-from .samplers.nestedsampler import NestedSampler
-from .posterior import draw_posterior_samples
-from .utils import configure_threads
-from .utils.io import save_to_json, save_dict_to_hdf5
-
+import pickle
+import time
+from typing import Any, Optional, Union
+
+from glasflow import __version__ as glasflow_version
+import numpy as np
+import torch
+
+from .. import __version__ as version
+from ..model import Model
+from ..utils import safe_file_dump
 
 logger = logging.getLogger(__name__)
 
 
-class FlowSampler:
-    """
-    Main class to handle running the nested sampler.
+class BaseNestedSampler(ABC):
+    """Base nested sampler class.
 
     Parameters
     ----------
     model : :obj:`nessai.model.Model`
-        User-defined model.
+        User-defined model
     output : str, optional
-        Output directory
-    resume : bool, optional
-        If True try to resume the sampler is the resume file exists.
+        Path for the output. If not specified the current working directory
+        is used.
+    seed : int, optional
+        Seed used to seed numpy and torch.
+    checkpointing : bool, optional
+        Boolean to toggle checkpointing, must be enabled to resume the sampler.
+        If false the sampler is still saved at the end of sampling.
+    checkpoint_interval : int
+        The interval used for checkpointing. By default this is a time interval
+        in seconds. If :code:`checkpoint_on_iteration=True` this corresponds to
+        the number of iterations between checkpointing.
+    checkpoint_on_iteration : bool
+        If true the checkpointing interval is checked against the number of
+        iterations
+    logging_interval : int, optional
+        The interval in seconds used for periodic logging. If not specified,
+        then periodic logging is disabled.
+    log_on_iteration : bool
+        If true logging will occur based on the iteration. If false logging
+        will be periodic if `logging_interval` is set. In case where neither
+        logging is enabled, `log_on_iteration` will be set to true with an
+        interval of :code:`nlive`.
     resume_file : str, optional
-        File to resume sampler from.
-    weights_files : str, optional
-        Weights files used to resume sampler that replaces the weights file
-        saved internally.
-    pytorch_threads : int
-        Maximum number of threads to use for torch. If ``None`` torch uses all
-        available threads.
-    max_threads : int
-        Deprecated and will be removed in a future release.
-    signal_handling : bool
-        Enable or disable signal handling.
-    exit_code : int, optional
-        Exit code to use when forceably exiting the sampler.
-    close_pool : bool
-        If True, the multiprocessing pool will be closed once the run method
-        has been called. Disables the option in :code:`NestedSampler` if
-        enabled.
-    disable_vectorisation : bool
-        Disable likelihood vectorisation. Overrides the value of
-        :py:attr:`nessai.model.Model.allow_vectorised`.
-    likelihood_chunksize : Optional[int]
-        Chunksize used when evaluating a vectorised likelihood. Overrides the
-        of :py:attr:`nessai.model.Model.likelihood_chunksize`. Set to None to
-        evaluate the likelihood with all available points.
-    allow_multi_valued_likelihood : Optional[bool]
-        Allow for a multi-valued likelihood function that will return different
-        likelihood values for the same point in parameter space. See
-        :py:attr:`nessai.model.Model.allow_multi_valued_likelihood` for more
-        details.
-    result_extension : str
-        Extension used when saving the result format. Defaults to HDF5, but
-        also supports JSON.
-    kwargs :
-        Keyword arguments passed to
-        :obj:`~nessai.samplers.nestedsampler.NestedSampler`.
+        Name of the file the sampler will be saved to and resumed from.
+    plot : bool, optional
+        Boolean to enable or disable plotting.
+    n_pool : int, optional
+        Number of threads to when for creating the multiprocessing pool.
+    pool : object
+        User defined multiprocessing pool that will be used when evaluating
+        the likelihood.
     """
 
     def __init__(
         self,
-        model,
-        output=os.getcwd(),
-        resume=True,
-        resume_file="nested_sampler_resume.pkl",
-        weights_file=None,
-        signal_handling=True,
-        exit_code=130,
-        pytorch_threads=1,
-        max_threads=None,
-        close_pool=True,
-        disable_vectorisation=False,
-        likelihood_chunksize=None,
-        allow_multi_valued_likelihood=None,
-        result_extension="hdf5",
-        **kwargs,
+        model: Model,
+        nlive: int,
+        output: str = None,
+        seed: int = None,
+        checkpointing: bool = True,
+        checkpoint_interval: int = 600,
+        checkpoint_on_iteration: bool = False,
+        logging_interval: int = None,
+        log_on_iteration: bool = True,
+        resume_file: str = None,
+        plot: bool = True,
+        n_pool: Optional[int] = None,
+        pool: Optional[Any] = None,
     ):
+        logger.info("Initialising nested sampler")
 
-        configure_threads(
-            max_threads=max_threads,
-            pytorch_threads=pytorch_threads,
-        )
-
-        self.exit_code = exit_code
-        self.close_pool = close_pool
-
-        self.result_extension = result_extension
-
-        if disable_vectorisation:
-            logger.warning(
-                "Overriding value of `allow_vectorised` in the model"
-            )
-            model.allow_vectorised = False
-
-        if likelihood_chunksize:
-            model.likelihood_chunksize = likelihood_chunksize
-
-        if allow_multi_valued_likelihood is not None:
-            model.allow_multi_valued_likelihood = allow_multi_valued_likelihood
-
-        self.output = os.path.join(output, "")
-        os.makedirs(self.output, exist_ok=True)
-        self.save_kwargs(kwargs)
+        self.info_enabled = logger.isEnabledFor(logging.INFO)
+        self.debug_enabled = logger.isEnabledFor(logging.DEBUG)
+        model.verify_model()
+        self.n_pool = n_pool
+        self.model = model
+        self.model.configure_pool(pool=pool, n_pool=n_pool)
+
+        self.nlive = nlive
+        self.plot = plot
+        self.checkpointing = checkpointing
+        self.checkpoint_interval = checkpoint_interval
+        self.checkpoint_on_iteration = checkpoint_on_iteration
+        if self.checkpoint_on_iteration:
+            self._last_checkpoint = 0
+        else:
+            self._last_checkpoint = datetime.datetime.now()
+        self.sampling_time = datetime.timedelta()
+        self.sampling_start_time = datetime.datetime.now()
+        self.iteration = 0
+        self.checkpoint_iterations = []
+        self.finalised = False
+        self.resumed = False
+
+        self.configure_random_seed(seed)
+        self.configure_output(output, resume_file=resume_file)
+        self.configure_periodic_logging(logging_interval, log_on_iteration)
 
-        model.configure_pool(
-            n_pool=kwargs.pop("n_pool", None), pool=kwargs.pop("pool", None)
-        )
+        self.live_points = None
 
-        if resume:
-            if not resume_file:
-                raise RuntimeError(
-                    "`resume_file` must be specified if resume=True. "
-                    f"Current value: {resume_file}"
-                )
-            if not any(
-                (
-                    os.path.exists(os.path.join(self.output, f))
-                    for f in [resume_file, resume_file + ".old"]
-                )
-            ):
-                logger.warning("No files to resume from, starting sampling")
-                self.ns = NestedSampler(
-                    model,
-                    output=self.output,
-                    resume_file=resume_file,
-                    close_pool=not self.close_pool,
-                    **kwargs,
-                )
-            else:
-                try:
-                    self.ns = NestedSampler.resume(
-                        os.path.join(self.output, resume_file),
-                        model,
-                        flow_config=kwargs.get("flow_config"),
-                        weights_file=weights_file,
-                    )
-                except (FileNotFoundError, RuntimeError) as e:
-                    logger.error(
-                        f"Could not load resume file from: {self.output} "
-                        f"with error {e}"
-                    )
-                    try:
-                        resume_file += ".old"
-                        self.ns = NestedSampler.resume(
-                            os.path.join(self.output, resume_file),
-                            model,
-                            flow_config=kwargs.get("flow_config"),
-                            weights_file=weights_file,
-                        )
-                    except RuntimeError as e:
-                        logger.error(
-                            "Could not load old resume "
-                            f"file from: {self.output}"
-                        )
-                        raise RuntimeError(
-                            "Could not resume sampler " f"with error: {e}"
-                        )
+    @property
+    def current_sampling_time(self):
+        if self.finalised:
+            return self.sampling_time
         else:
-            self.ns = NestedSampler(
-                model,
-                output=self.output,
-                resume_file=resume_file,
-                close_pool=not self.close_pool,
-                **kwargs,
+            return self.sampling_time + (
+                datetime.datetime.now() - self.sampling_start_time
             )
 
-        if signal_handling:
-            try:
-                signal.signal(signal.SIGTERM, self.safe_exit)
-                signal.signal(signal.SIGINT, self.safe_exit)
-                signal.signal(signal.SIGALRM, self.safe_exit)
-            except AttributeError:
-                logger.error("Cannot set signal attributes on this system")
-        else:
-            logger.warning(
-                "Signal handling is disabled. nessai will not automatically "
-                "checkpoint when exitted."
-            )
+    @property
+    def likelihood_evaluation_time(self):
+        """Current log-likelihood time"""
+        return self.model.likelihood_evaluation_time
 
     @property
-    def log_evidence(self):
-        """Return the most recent log evidence"""
-        return self.logZ
+    def total_likelihood_evaluations(self):
+        """Total number of likelihood evaluations"""
+        return self.model.likelihood_evaluations
+
+    likelihood_calls = total_likelihood_evaluations
+    """Alias for :code:`total_likelihood_evaluations`"""
 
     @property
-    def log_evidence_error(self):
-        """Return the most recent log evidence error"""
-        return self.logZ_error
+    @abstractmethod
+    def posterior_effective_sample_size(self):
+        """The effective sample size of the posterior distribution"""
+        raise NotImplementedError()
 
-    def run(
-        self,
-        plot=True,
-        plot_indices=True,
-        plot_posterior=True,
-        plot_logXlogL=True,
-        save=True,
-        posterior_sampling_method=None,
-        close_pool=None,
+    def configure_output(
+        self, output: Union[str, None], resume_file: Union[str, None] = None
     ):
-        """Run the nested sampler.
+        """Configure the output folder
 
         Parameters
         ----------
-        plot : bool
-            Toggle all plots produced once the sampler has converged.
-        plot_indices : bool
-            Toggle the insertion indices plot.
-        plot_posterior : bool
-            Toggle the posterior distribution plot.
-        plot_logXlogL : bool
-            Toggle the log-prior volume vs log-likelihood plot.
-        save : bool, optional
-            Toggle automatic saving of results
-        posterior_sampling_method : str, optional
-            Method used for drawing posterior samples. Defaults to rejection
-            sampling.
-        close_pool : bool, optional
-            Boolean to indicated if the pool should be closed at the end of the
-            run function. If False, the user must manually close the pool. If
-            specified, this value overrides the value passed when initialising
-            the FlowSampler class.
+        output : str
+            Directory where the results will be stored
+        resume_file : str, optional
+            Specific file to use for checkpointing. If not specified the
+            default is used (nested_sampler_resume.pkl)
         """
-        if close_pool is None:
-            close_pool = self.close_pool
-        if posterior_sampling_method is None:
-            posterior_sampling_method = "rejection_sampling"
-
-        self.ns.initialise()
-        self.logZ, self.nested_samples = self.ns.nested_sampling_loop()
-        self.logZ_error = self.ns.state.log_evidence_error
-        logger.info((f"Total sampling time: {self.ns.sampling_time}"))
-
-        logger.info("Starting post processing")
-        logger.info("Computing posterior samples")
-        self.posterior_samples = draw_posterior_samples(
-            self.nested_samples,
-            log_w=self.ns.state.log_posterior_weights,
-            method=posterior_sampling_method,
-        )
-        logger.info(
-            f"Returned {self.posterior_samples.size} " "posterior samples"
-        )
-
-        if save:
-            self.save_results(
-                os.path.join(self.output, "result"),
-                extension=self.result_extension,
-            )
+        if output is None:
+            output = os.getcwd()
+        if not os.path.exists(output):
+            os.makedirs(output, exist_ok=True)
 
-        if plot:
-            from nessai import plot
-
-            if plot_posterior:
-                plot.plot_live_points(
-                    self.posterior_samples,
-                    filename=os.path.join(
-                        self.output, "posterior_distribution.png"
-                    ),
-                )
-            if plot_indices:
-                plot.plot_indices(
-                    self.ns.insertion_indices,
-                    self.ns.nlive,
-                    filename=os.path.join(
-                        self.output, "insertion_indices.png"
-                    ),
-                )
+        if resume_file is None:
+            resume_file = os.path.join(output, "nested_sampler_resume.pkl")
+        else:
+            resume_file = os.path.join(output, resume_file)
 
-            if plot_logXlogL:
-                self.ns.state.plot(os.path.join(self.output, "logXlogL.png"))
+        self.output = output
+        self.resume_file = resume_file
 
-        if close_pool:
-            self.ns.close_pool()
+    def configure_random_seed(self, seed: Optional[int]):
+        """Initialise the random seed.
 
-    def save_kwargs(self, kwargs: dict) -> None:
+        Parameters
+        ----------
+        seed : Optional[int]
+            The random seed. If not specified, no seed is set.
         """
-        Save the dictionary of keyword arguments used.
+        self.seed = seed
+        if self.seed is not None:
+            logger.debug(f"Setting random seed to {seed}")
+            np.random.seed(seed=self.seed)
+            torch.manual_seed(self.seed)
 
-        Uses an encoder class to handle numpy arrays.
+    def configure_periodic_logging(self, logging_interval, log_on_iteration):
+        """Configure the periodic logging.
 
         Parameters
         ----------
-        kwargs : dict
-            Dictionary of kwargs to save.
+        logging_interval : int, optional
+            The interval in seconds used for periodic logging. If not
+            specified, then periodic logging is disabled.
+        log_on_iteration : bool
+            If true logging will occur based on the iteration. If false logging
+            will be periodic if `logging_interval` is set. In case where
+            neither logging is enabled, `log_on_iteration` will be set to true
+            with an interval of :code:`nlive`.
         """
-        save_to_json(kwargs.copy(), os.path.join(self.output, "config.json"))
+        self.logging_interval = logging_interval
+        self.log_on_iteration = log_on_iteration
+        if not self.logging_interval and not self.log_on_iteration:
+            logger.warning(
+                "All logging disabled. Enabling logging on iteration"
+            )
+            self.log_on_iteration = True
+        if self.log_on_iteration:
+            if self.logging_interval is None:
+                self.logging_interval = self.nlive
+            self._last_log = 0
+        else:
+            self._last_log = time.time()
 
-    def save_results(
-        self, filename: str, extension: Optional[str] = None
-    ) -> None:
+    @abstractmethod
+    def log_state(self):
+        raise NotImplementedError()
+
+    def periodically_log_state(self):
+        """Log the state of the sampler.
+
+        Calls :code:`log_state` if the elapsed interval in time (or iterations)
+        is more than the specified interval.
         """
-        Save the results from sampling to a specific results file.
+        if self.log_on_iteration:
+            if not (self.iteration - self._last_log) >= self.logging_interval:
+                return
+            else:
+                self._last_log = self.iteration
+        else:
+            now = time.time()
+            if not (now - self._last_log) >= self.logging_interval:
+                return
+            else:
+                self._last_log = now
+        self.log_state()
+
+    def checkpoint(
+        self,
+        periodic: bool = False,
+        force: bool = False,
+        save_existing: bool = True,
+    ):
+        """Checkpoint the classes internal state.
 
         Parameters
         ----------
-        filename : str
-            Name of file to save results to.
-        extension : Optional[str]
-            File extension to used. If not specified, it will be inferred from
-            the filename.
+        periodic : bool
+            Indicates if the checkpoint is regular periodic checkpointing
+            or forced by a signal. If forced by a signal, it will show up on
+            the state plot.
+        force : bool
+            Force the sampler to checkpoint.
+        save_existing : bool
+            If True, the previous checkpoint will be copied to `.old`.
+            If False, the new checkpoint will override the previous file.
         """
-        d = self.ns.get_result_dictionary()
-        d["posterior_samples"] = self.posterior_samples
-
-        ext = os.path.splitext(filename)[1].lstrip(".")
-        if extension is None:
-            if ext == "":
-                raise RuntimeError(
-                    "Must specify file extension if not present in filename!"
-                )
-            else:
-                extension = ext
-        elif ext == "":
-            filename = ".".join([filename, extension])
-
-        if extension == "json":
-            d["posterior_samples"] = live_points_to_dict(
-                d["posterior_samples"]
-            )
-            save_to_json(d, filename)
-        elif extension in ["hdf5", "h5"]:
-            save_dict_to_hdf5(d, filename)
+        now = datetime.datetime.now()
+        if not periodic:
+            self.checkpoint_iterations += [self.iteration]
+        elif force:
+            pass
         else:
-            raise RuntimeError(f"Unknown file extension: {extension}")
+            if self.checkpoint_on_iteration:
+                if (
+                    self.iteration - self._last_checkpoint
+                ) >= self.checkpoint_interval:
+                    self._last_checkpoint = self.iteration
+                else:
+                    return
+            else:
+                if (
+                    now - self._last_checkpoint
+                ).total_seconds() >= self.checkpoint_interval:
+                    self._last_checkpoint = now
+                else:
+                    return
+        self.sampling_time += now - self.sampling_start_time
+        logger.info("Checkpointing nested sampling")
+        safe_file_dump(
+            self, self.resume_file, pickle, save_existing=save_existing
+        )
+        self.sampling_start_time = datetime.datetime.now()
 
-    def terminate_run(self, code=None):
-        """Terminate a sampling run.
+    @classmethod
+    def resume(cls, filename: str, model: Model):
+        """Resumes the interrupted state from a checkpoint pickle file.
 
         Parameters
         ----------
-        code : int, optional
-            Code passed to :code:`close_pool`
+        filename : str
+            Pickle file to resume from
+        model : :obj:`nessai.model.Model`
+            User-defined model
+        Returns
+        -------
+        obj
+            Instance of BaseNestedSampler
         """
-        logger.warning("Terminating run")
-        self.ns.close_pool(code=code)
-        self.ns.checkpoint()
+        logger.info("Resuming NestedSampler from " + filename)
+        with open(filename, "rb") as f:
+            obj = pickle.load(f)
+        model.likelihood_evaluations += obj._previous_likelihood_evaluations
+        model.likelihood_evaluation_time += datetime.timedelta(
+            seconds=obj._previous_likelihood_evaluation_time
+        )
+        obj.model = model
+        obj.resumed = True
+        return obj
+
+    @abstractmethod
+    def nested_sampling_loop(self):
+        raise NotImplementedError()
+
+    def close_pool(self, code=None):
+        """Close the multiprocessing pool."""
+        self.model.close_pool(code=code)
 
-    def safe_exit(self, signum=None, frame=None):
-        """
-        Safely exit. This includes closing the multiprocessing pool.
+    def get_result_dictionary(self):
+        """Return a dictionary that contains results.
+
+        Only includes version, seed and sampling time. Child classes should
+        call this method and add to the dictionary.
         """
-        logger.warning(f"Trying to safely exit with code {signum}")
-        self.terminate_run(code=signum)
-        logger.warning(f"Exiting with code: {self.exit_code}")
-        sys.exit(self.exit_code)
+        d = dict()
+        d["version"] = version
+        d["glasflow_version"] = glasflow_version
+        d["seed"] = self.seed
+        d["sampling_time"] = self.sampling_time.total_seconds()
+        d["total_likelihood_evaluations"] = self.model.likelihood_evaluations
+        d[
+            "likelihood_evaluation_time"
+        ] = self.likelihood_evaluation_time.total_seconds()
+        if hasattr(self.model, "truth"):
+            d["truth"] = self.model.truth
+        return d
+
+    def __getstate__(self):
+        d = self.__dict__
+        exclude = {"model", "proposal"}
+        state = {k: d[k] for k in d.keys() - exclude}
+        state["_previous_likelihood_evaluations"] = d[
+            "model"
+        ].likelihood_evaluations
+        state["_previous_likelihood_evaluation_time"] = d[
+            "model"
+        ].likelihood_evaluation_time.total_seconds()
+        return state
```

### Comparing `nessai-0.8.1/nessai/gw/proposal.py` & `nessai-0.9.0/nessai/gw/proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/gw/reparameterisations.py` & `nessai-0.9.0/nessai/gw/reparameterisations.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/gw/utils.py` & `nessai-0.9.0/nessai/gw/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/livepoint.py` & `nessai-0.9.0/nessai/livepoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,34 +150,39 @@
             raise ValueError(
                 "Could not create empty structured array. Maybe the "
                 "non-sampling parameters are missing?"
             )
     return struct_array
 
 
-def live_points_to_array(live_points, names=None):
+def live_points_to_array(live_points, names=None, copy=False):
     """
     Converts live points to unstructured arrays for training.
 
     Parameters
     ----------
     live_points : structured_array
         Structured array of live points
     names : list of str or None
         If None all fields in the structured array are added to the dictionary
         else only those included in the list are added.
+    copy : bool
+        If true, returns a copy. If false, returns a view. See numpy
+        documentation for
+        :code:`numpy.lib.recfunctions.structured_to_unstructured` for more
+        details.
 
     Returns
     -------
     np.ndarray
         Unstructured numpy array
     """
     if names is None:
         names = list(live_points.dtype.names)
-    return rfn.structured_to_unstructured(live_points[names])
+    return rfn.structured_to_unstructured(live_points[names], copy=copy)
 
 
 def parameters_to_live_point(parameters, names, non_sampling_parameters=True):
     """
     Take a list or array of parameters for a single live point
     and converts them to a live point.
```

### Comparing `nessai-0.8.1/nessai/model.py` & `nessai-0.9.0/nessai/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,19 +179,22 @@
 
         This check can be prevented by setting
         :py:attr:`nessai.model.Model.allowed_vectorised` to ``False``.
         """
         if self._vectorised_likelihood is None:
             if self.allow_vectorised:
                 x = self.new_point(N=10)
-                target = np.fromiter(
-                    map(self.log_likelihood, x), config.livepoints.logl_dtype
+                target = np.array(
+                    [self.log_likelihood(xx) for xx in x],
+                    dtype=config.livepoints.logl_dtype,
                 )
                 try:
-                    batch = self.log_likelihood(x)
+                    batch = self.log_likelihood(x).astype(
+                        config.livepoints.logl_dtype
+                    )
                 except (TypeError, ValueError):
                     logger.debug(
                         "Evaluating a batch of points returned an error. "
                         "Assuming the likelihood is not vectorised."
                     )
                     self._vectorised_likelihood = False
                 else:
@@ -519,17 +522,17 @@
                                 ),
                             )
                         )
                     )
                 else:
                     log_likelihood = self.log_likelihood(x)
             else:
-                log_likelihood = np.fromiter(
-                    map(self.log_likelihood, x), config.livepoints.logl_dtype
-                )
+                log_likelihood = np.array(
+                    [self.log_likelihood(xx) for xx in x],
+                ).flatten()
         else:
             logger.debug("Using pool to evaluate likelihood")
             if self.allow_vectorised and self.vectorised_likelihood:
                 if self.likelihood_chunksize:
                     log_likelihood = np.concatenate(
                         self.pool.map(
                             log_likelihood_wrapper,
@@ -547,15 +550,15 @@
                     )
             else:
                 log_likelihood = np.array(
                     self.pool.map(log_likelihood_wrapper, x)
                 ).flatten()
         self.likelihood_evaluations += x.size
         self.likelihood_evaluation_time += datetime.datetime.now() - st
-        return log_likelihood
+        return log_likelihood.astype(config.livepoints.logl_dtype)
 
     def unstructured_view(self, x):
         """An unstructured view of point(s) x that only contains the \
             parameters in the model.
 
         This is quicker than converting to a unstructured array and does not
         create a copy of the array.
```

### Comparing `nessai-0.8.1/nessai/plot.py` & `nessai-0.9.0/nessai/plot.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/posterior.py` & `nessai-0.9.0/nessai/posterior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/priors.py` & `nessai-0.9.0/nessai/priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/proposal/analytic.py` & `nessai-0.9.0/nessai/proposal/analytic.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/proposal/augmented.py` & `nessai-0.9.0/nessai/proposal/augmented.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/proposal/base.py` & `nessai-0.9.0/nessai/proposal/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/proposal/flowproposal.py` & `nessai-0.9.0/nessai/proposal/flowproposal.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Main proposal object that includes normalising flows.
 """
 import copy
 import datetime
 from functools import partial
 import logging
 import os
+import re
 
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.lib.recfunctions as rfn
 import torch
 
 from .. import config
@@ -462,18 +463,25 @@
             )
             self.max_radius = False
 
     def configure_constant_volume(self):
         """Configure using constant volume latent contour."""
         if self.constant_volume_mode:
             logger.debug("Configuring constant volume latent contour")
-            if not self.latent_prior == "truncated_gaussian":
+            if self.latent_prior == "truncated_gaussian":
+                pass
+            elif self.latent_prior in ["uniform_nball", "uniform_nsphere"]:
+                logger.warning(
+                    "Constant volume mode with latent_prior="
+                    f"{self.latent_prior} is experimental!"
+                )
+            else:
                 raise RuntimeError(
-                    "Constant volume requires "
-                    "`latent_prior='truncated_gaussian'`"
+                    "Constant volume mode is not supported for latent_prior="
+                    f"{self.latent_prior}"
                 )
             self.fixed_radius = compute_radius(
                 self.rescaled_dims, self.volume_fraction
             )
             self.fuzz = 1.0
             if self.max_radius < self.fixed_radius:
                 logger.warning(
@@ -619,14 +627,34 @@
                         f"received instance of {type(cfg)}."
                     )
             else:
                 logger.debug(f"Assuming {k} is a reparameterisation")
                 try:
                     rc, default_config = self.get_reparameterisation(k)
                     default_config.update(cfg)
+                    parameters = default_config.get("parameters")
+
+                    if parameters is not None:
+                        if not isinstance(parameters, list):
+                            if isinstance(parameters, str):
+                                patterns = [parameters]
+                            else:
+                                patterns = list(parameters)
+                        else:
+                            patterns = parameters.copy()
+                        matches = []
+                        for pattern in patterns:
+                            r = re.compile(pattern)
+                            matches += list(filter(r.match, self.model.names))
+                        default_config["parameters"] = matches
+                    else:
+                        logger.warning(
+                            "Reparameterisation might be missing parameters!"
+                        )
+
                 except ValueError:
                     raise RuntimeError(
                         f"{k} is not a parameter in the model or a known "
                         "reparameterisation"
                     )
 
             if not default_config.get("parameters", False):
@@ -700,15 +728,15 @@
                     "settings."
                 )
 
         self._reparameterisation.check_order()
 
         self.names = self._reparameterisation.parameters
         self.rescaled_names = self._reparameterisation.prime_parameters
-        self.rescale_parameters = [
+        self.parameters_to_rescale = [
             p
             for p in self._reparameterisation.parameters
             if p not in self._reparameterisation.prime_parameters
         ]
 
     def set_rescaling(self):
         """
@@ -736,15 +764,15 @@
                     "detect_edges_kwargs": self.detect_edges_kwargs,
                 },
             }
 
         self.configure_reparameterisations(self.reparameterisations)
 
         logger.info(f"x space parameters: {self.names}")
-        logger.info(f"parameters to rescale: {self.rescale_parameters}")
+        logger.info(f"parameters to rescale: {self.parameters_to_rescale}")
         logger.info(f"x prime space parameters: {self.rescaled_names}")
         self.rescaling_set = True
 
     def verify_rescaling(self):
         """
         Verify the rescaling functions are invertible
         """
@@ -907,15 +935,15 @@
 
             plot_live_points(
                 x_gen,
                 c="logL",
                 filename=os.path.join(output, "x_generated.png"),
             )
 
-        if self.rescale_parameters:
+        if self.parameters_to_rescale:
             if self._plot_training == "all":
                 plot_live_points(
                     self.training_data_prime,
                     c="logL",
                     filename=os.path.join(output, "x_prime_samples.png"),
                 )
                 plot_live_points(
@@ -969,15 +997,17 @@
 
         x_prime, _ = self.rescale(x)
 
         self.training_data_prime = x_prime.copy()
 
         # Convert to numpy array for training and remove likelihoods and priors
         # Since the names of parameters may have changes, pull names from flows
-        x_prime_array = live_points_to_array(x_prime, self.rescaled_names)
+        x_prime_array = live_points_to_array(
+            x_prime, self.rescaled_names, copy=True
+        )
 
         self.flow.train(
             x_prime_array,
             output=block_output,
             plot=self._plot_training and plot,
         )
 
@@ -1044,15 +1074,15 @@
             jacobian)
         """
         log_J = 0
         if rescale:
             x, log_J_rescale = self.rescale(x, compute_radius=compute_radius)
             log_J += log_J_rescale
 
-        x = live_points_to_array(x, names=self.rescaled_names)
+        x = live_points_to_array(x, names=self.rescaled_names, copy=True)
 
         if x.ndim == 1:
             x = x[np.newaxis, :]
         z, log_prob = self.flow.forward_and_log_prob(x)
 
         return z, log_prob + log_J
```

### Comparing `nessai-0.8.1/nessai/proposal/rejection.py` & `nessai-0.9.0/nessai/proposal/rejection.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/proposal/utils.py` & `nessai-0.9.0/nessai/proposal/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/__init__.py` & `nessai-0.9.0/nessai/reparameterisations/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/angle.py` & `nessai-0.9.0/nessai/reparameterisations/angle.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/base.py` & `nessai-0.9.0/nessai/reparameterisations/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/combined.py` & `nessai-0.9.0/nessai/reparameterisations/combined.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/null.py` & `nessai-0.9.0/nessai/reparameterisations/null.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/rescale.py` & `nessai-0.9.0/nessai/reparameterisations/rescale.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/reparameterisations/utils.py` & `nessai-0.9.0/nessai/reparameterisations/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/samplers/nestedsampler.py` & `nessai-0.9.0/nessai/samplers/nestedsampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         checkpoint_on_iteration=False,
         checkpoint_on_training=False,
         logging_interval=None,
         log_on_iteration=True,
         resume_file=None,
         seed=None,
         pool=None,
-        close_pool=True,
+        close_pool=False,
         n_pool=None,
         plot=True,
         proposal_plots=False,
         prior_sampling=False,
         analytic_priors=False,
         maximum_uninformed=None,
         uninformed_proposal=None,
@@ -325,14 +325,19 @@
         Mean acceptance of the last nlive // 10 points
         """
         if self.acceptance_history:
             return np.mean(self.acceptance_history)
         else:
             return np.nan
 
+    @property
+    def posterior_effective_sample_size(self):
+        """The effective sample size of the posterior distribution"""
+        return self.state.effective_n_posterior_samples
+
     def configure_max_iteration(self, max_iteration):
         """Configure the maximum iteration.
 
         If None then no maximum is set.
 
         Parameters
         ----------
@@ -939,43 +944,34 @@
         Parameters
         ----------
         filename : str, optional
             If specified the figure will be saved, otherwise the figure is
             returned.
         """
 
-        fig, ax = plt.subplots(6, 1, sharex=True, figsize=(12, 12))
+        fig, ax = plt.subplots(7, 1, sharex=True, figsize=(12, 12))
         ax = ax.ravel()
         it = (np.arange(len(self.min_likelihood))) * (self.nlive // 10)
         it[-1] = self.iteration
 
-        for t in self.training_iterations:
-            for a in ax:
-                a.axvline(t, ls="-", color="lightgrey")
-
-        if not self.train_on_empty:
-            for p in self.population_iterations:
-                for a in ax:
-                    a.axvline(p, ls="-", color="tab:orange")
-
         for i in self.checkpoint_iterations:
             for a in ax:
                 a.axvline(i, ls=":", color="#66ccff")
 
         for a in ax:
             a.axvline(self.iteration, c="#ff9900", ls="-.")
 
-        ax[0].plot(it, self.min_likelihood, label="Min logL")
-        ax[0].plot(it, self.max_likelihood, label="Max logL")
-        ax[0].set_ylabel("logL")
+        ax[0].plot(it, self.min_likelihood, label="Min log L")
+        ax[0].plot(it, self.max_likelihood, label="Max log L")
+        ax[0].set_ylabel(r"$\log L$")
         ax[0].legend(frameon=False)
 
         logX_its = np.arange(len(self.state.log_vols))
         ax[1].plot(logX_its, self.state.log_vols, label="log X")
-        ax[1].set_ylabel("Log X")
+        ax[1].set_ylabel(r"$\log X$")
         ax[1].legend(frameon=False)
 
         if self.state.track_gradients:
             ax_logX_grad = plt.twinx(ax[1])
             # Use dotted linestyle (ls[2]) because dashed isn't clear
             ax_logX_grad.plot(
                 logX_its,
@@ -989,60 +985,72 @@
             handles, labels = ax[1].get_legend_handles_labels()
             handles_tw, labels_tw = ax_logX_grad.get_legend_handles_labels()
             ax[1].legend(
                 handles + handles_tw, labels + labels_tw, frameon=False
             )
 
         ax[2].plot(it, self.likelihood_evaluations, label="Evaluations")
-        ax[2].set_ylabel("logL evaluations")
+        ax[2].set_ylabel("Likelihood\n evaluations")
+        ax[2].set_yscale("log")
 
         ax[3].plot(it, self.logZ_history, label="logZ")
-        ax[3].set_ylabel("logZ")
+        ax[3].set_ylabel(r"$\log Z$")
         ax[3].legend(frameon=False)
 
         ax_dz = plt.twinx(ax[3])
         ax_dz.plot(
             it,
             self.dZ_history,
             label="dZ",
             c="C1",
             ls=config.plotting.line_styles[1],
         )
-        ax_dz.set_ylabel("dZ")
+        ax_dz.set_yscale("log")
+        ax_dz.set_ylabel(r"$dZ$")
         handles, labels = ax[3].get_legend_handles_labels()
         handles_dz, labels_dz = ax_dz.get_legend_handles_labels()
         ax[3].legend(handles + handles_dz, labels + labels_dz, frameon=False)
 
         ax[4].plot(it, self.mean_acceptance_history, label="Proposal")
         ax[4].plot(
             self.population_iterations,
             self.population_acceptance,
             label="Population",
         )
         ax[4].set_ylabel("Acceptance")
-        ax[4].set_ylim((-0.1, 1.1))
         handles, labels = ax[4].get_legend_handles_labels()
 
         ax_r = plt.twinx(ax[4])
         ax_r.plot(
             self.population_iterations,
             self.population_radii,
             label="Radius",
             color="C2",
             ls=config.plotting.line_styles[2],
         )
         ax_r.set_ylabel("Population radius")
         handles_r, labels_r = ax_r.get_legend_handles_labels()
         ax[4].legend(handles + handles_r, labels + labels_r, frameon=False)
+        ax[4].set_yscale("log")
+        ax[4].set_ylim(top=1.1)
+        dtrain = np.array(self.training_iterations[1:]) - np.array(
+            self.training_iterations[:-1]
+        )
+        ax[5].plot(self.training_iterations[1:], dtrain)
+        if self.training_iterations:
+            ax[5].axvline(
+                self.training_iterations[0], ls="-", color="lightgrey"
+            )
+        ax[5].set_ylabel(r"$\Delta$ train")
 
         if len(self.rolling_p):
             it = (np.arange(len(self.rolling_p)) + 1) * self.nlive
-            ax[5].plot(it, self.rolling_p, "o", label="p-value")
-        ax[5].set_ylabel("p-value")
-        ax[5].set_ylim([-0.1, 1.1])
+            ax[6].plot(it, self.rolling_p, "o", label="p-value")
+        ax[6].set_ylabel("p-value")
+        ax[6].set_ylim([-0.1, 1.1])
 
         ax[-1].set_xlabel("Iteration")
 
         fig.suptitle(
             f"Sampling time: {self.current_sampling_time}", fontsize=16
         )
 
@@ -1051,23 +1059,14 @@
                 [0],
                 [0],
                 color="#ff9900",
                 linestyle="-.",
                 label="Current iteration",
             ),
             Line2D(
-                [0],
-                [0],
-                color="lightgrey",
-                linestyle="-",
-                markersize=10,
-                markeredgewidth=1.5,
-                label="Training",
-            ),
-            Line2D(
                 [0], [0], color="#66ccff", linestyle=":", label="Checkpoint"
             ),
         ]
         fig.legend(handles=handles, frameon=False, ncol=3, loc=(0.6, 0.0))
 
         fig.tight_layout()
         fig.subplots_adjust(top=0.95)
@@ -1314,34 +1313,34 @@
         d["log_evidence_error"] = self.state.log_evidence_error
         d["information"] = self.information
         d["training_time"] = self.training_time.total_seconds()
         d["population_time"] = self.proposal_population_time.total_seconds()
         return d
 
     @classmethod
-    def resume(cls, filename, model, flow_config=None, weights_file=None):
+    def resume(cls, filename, model, flow_config=None, weights_path=None):
         """
         Resumes the interrupted state from a checkpoint pickle file.
 
         Parameters
         ----------
         filename : str
             Pickle pickle to resume from
         model : :obj:`nessai.model.Model`
             User-defined model
         flow_config : dict, optional
             Dictionary for configuring the flow
-        weights_file : str, optional
-            Weights files to use in place of the weights file stored in the
+        weights_path : str, optional
+            Weights file to use in place of the weights file stored in the
             pickle file.
 
         Returns
         -------
         obj
             Instance of NestedSampler
         """
         obj = super().resume(filename, model)
         obj._uninformed_proposal.resume(model)
         if flow_config is None:
             flow_config = {}
-        obj._flow_proposal.resume(model, flow_config, weights_file)
+        obj._flow_proposal.resume(model, flow_config, weights_path)
         return obj
```

### Comparing `nessai-0.8.1/nessai/utils/__init__.py` & `nessai-0.9.0/nessai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/distance.py` & `nessai-0.9.0/nessai/utils/distance.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/distributions.py` & `nessai-0.9.0/nessai/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/hist.py` & `nessai-0.9.0/nessai/utils/hist.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/indices.py` & `nessai-0.9.0/nessai/utils/indices.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/io.py` & `nessai-0.9.0/nessai/utils/io.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/logging.py` & `nessai-0.9.0/nessai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/multiprocessing.py` & `nessai-0.9.0/nessai/utils/multiprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,22 +35,23 @@
             )
     return n_pool
 
 
 def check_multiprocessing_start_method():
     """Check the multiprocessing start method.
 
-    Raise an error if the start method is not `fork`.
+    Print a warning if the start method is not `fork`.
     """
     start_method = multiprocessing.get_start_method()
     if start_method != "fork":
-        raise RuntimeError(
-            "nessai only supports multiprocessing using the 'fork' start "
-            f"method. Actual start method is: {start_method}. See the "
-            "multiprocessing documentation for more details."
+        logger.warning(
+            f"Using {start_method} start method for multiprocessing. "
+            "This may lead to high memory usage or errors. "
+            "Consider using the `fork` start method. "
+            "See the multiprocessing documentation for more details."
         )
 
 
 def initialise_pool_variables(model):
     """Prepare the model for use with a multiprocessing pool.
 
     Makes a global copy of the model. Should be called before initialising
```

### Comparing `nessai-0.8.1/nessai/utils/rescaling.py` & `nessai-0.9.0/nessai/utils/rescaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,16 +324,17 @@
     Returns
     -------
     float or ndarray
         Rescaled values.
     float or ndarray
         Log Jacobian determinant.
     """
-    x = np.divide(1, 1 + np.exp(-x))
-    log_j = np.log(x) + np.log1p(-x)
+    with np.errstate(over="ignore", divide="ignore"):
+        x = np.divide(1, 1 + np.exp(-x))
+        log_j = np.log(x) + np.log1p(-x)
     return x, log_j
 
 
 def logistic_function(x, x0=0.0, k=1.0):
     """Logistic function with configurable midpoint and gradient.
 
     Parameters
```

### Comparing `nessai-0.8.1/nessai/utils/sampling.py` & `nessai-0.9.0/nessai/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/sorting.py` & `nessai-0.9.0/nessai/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/structures.py` & `nessai-0.9.0/nessai/utils/structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,7 +93,15 @@
     -------
     list
         List of numpy arrays each with a maximum length given by the chunksize.
     """
     if chunksize < 1:
         raise ValueError("chunksize must be greater than 1")
     return np.array_split(x, range(chunksize, len(x), chunksize))
+
+
+def get_inverse_indices(n, indices):
+    """Return the indices that are not in input array given a size n"""
+    if indices.max() >= n:
+        raise ValueError("Indices contain values that are out of range for n")
+    inv = np.arange(n, dtype=int)
+    return inv[~np.in1d(inv, indices)]
```

### Comparing `nessai-0.8.1/nessai/utils/threading.py` & `nessai-0.9.0/nessai/utils/threading.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai/utils/torchutils.py` & `nessai-0.9.0/nessai/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/nessai.egg-info/PKG-INFO` & `nessai-0.9.0/nessai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nessai
-Version: 0.8.1
+Version: 0.9.0
 Summary: Nessai: Nested Sampling with Artificial Intelligence
 Home-page: https://github.com/mj-will/nessai
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 Project-URL: Documentation, https://nessai.readthedocs.io/
 Keywords: nested sampling,normalising flows,machine learning
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -30,15 +29,15 @@
 ![int-tests](https://github.com/mj-will/nessai/actions/workflows/integration-tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/mj-will/nessai/branch/main/graph/badge.svg?token=O7SN167SK6)](https://codecov.io/gh/mj-will/nessai)
 
 # nessai: Nested Sampling with Artificial Intelligence
 
 ``nessai`` (/ˈnɛsi/): Nested Sampling with Artificial Intelligence
 
-``nessai`` is a nested sampling algorithm for Bayesian Inference that incorporates normalisings flows. It is designed for applications where the Bayesian likelihood is computationally expensive.
+``nessai`` is a nested sampling algorithm for Bayesian Inference that incorporates normalising flows. It is designed for applications where the Bayesian likelihood is computationally expensive.
 
 ## Installation
 
 ``nessai`` can be installed using ``pip``:
 
 ```console
 pip install nessai
@@ -78,36 +77,47 @@
 
 Other code snippets that draw on existing code reference the source in their corresponding doc-strings.
 
 The authors also thank Christian Chapman-Bird, Laurence Datrier, Fergus Hayes, Jethro Linley and Simon Tait for their feedback and help finding bugs in ``nessai``.
 
 ## Citing
 
-If you find ``nessai`` useful in your work please cite the DOI for this code and our paper:
+If you find ``nessai`` useful in your work please cite the DOI for this code and our papers:
 
 ```bibtex
 @software{nessai,
   author       = {Michael J. Williams},
   title        = {nessai: Nested Sampling with Artificial Intelligence},
   month        = feb,
   year         = 2021,
   publisher    = {Zenodo},
   version      = {latest},
   doi          = {10.5281/zenodo.4550693},
   url          = {https://doi.org/10.5281/zenodo.4550693}
 }
 
-@article{PhysRevD.103.103006,
-  title = {Nested sampling with normalizing flows for gravitational-wave inference},
-  author = {Williams, Michael J. and Veitch, John and Messenger, Chris},
-  journal = {Phys. Rev. D},
-  volume = {103},
-  issue = {10},
-  pages = {103006},
-  numpages = {19},
-  year = {2021},
-  month = {May},
-  publisher = {American Physical Society},
-  doi = {10.1103/PhysRevD.103.103006},
-  url = {https://link.aps.org/doi/10.1103/PhysRevD.103.103006}
+@article{Williams:2021qyt,
+    author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+    title = "{Nested sampling with normalizing flows for gravitational-wave inference}",
+    eprint = "2102.11056",
+    archivePrefix = "arXiv",
+    primaryClass = "gr-qc",
+    doi = "10.1103/PhysRevD.103.103006",
+    journal = "Phys. Rev. D",
+    volume = "103",
+    number = "10",
+    pages = "103006",
+    year = "2021"
 }
+
+@article{Williams:2023ppp,
+    author = "Williams, Michael J. and Veitch, John and Messenger, Chris",
+    title = "{Importance nested sampling with normalising flows}",
+    eprint = "2302.08526",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    reportNumber = "LIGO-P2200283",
+    month = "2",
+    year = "2023"
+}
+
 ```
```

### Comparing `nessai-0.8.1/pyproject.toml` & `nessai-0.9.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
 ]
 
 [tool.black]
 line-length = 79
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
```

### Comparing `nessai-0.8.1/setup.cfg` & `nessai-0.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 long_description_content_type = text/markdown
 author = Michael J. Williams
 author_email = m.williams.4@research.gla.ac.uk
 url = https://github.com/mj-will/nessai
 project_urls = 
 	Documentation = https://nessai.readthedocs.io/
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 keywords = nested sampling, normalising flows, machine learning
 
 [options]
 packages = find:
-python requires = >=3.7
+python requires = >=3.8
 install_requires = 
 	numpy>=1.9
 	pandas
 	matplotlib>=2.0
 	seaborn
 	scipy>=0.16
 	torch>=1.11.0
@@ -35,15 +34,15 @@
 test = 
 	pytest
 	pytest-cov
 	pytest-timeout
 	pytest-rerunfailures
 	pytest-integration
 gw = 
-	lalsuite
+	lalsuite; sys_platform != 'win32'
 	bilby
 	astropy
 nflows = 
 	nflows
 dev = 
 	pre-commit
 	ray[default]
```

### Comparing `nessai-0.8.1/tests/conftest.py` & `nessai-0.9.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import numpy as np
 import pytest
 from scipy.stats import norm
 import time
 import torch
 import multiprocessing
 
+from nessai.livepoint import (
+    add_extra_parameters_to_live_points,
+    reset_extra_live_points_parameters,
+)
 from nessai.model import Model
+from nessai.utils.testing import IntegrationTestModel
 
 
 seed(170817)
 torch.manual_seed(170817)
 
 _requires_dependency_cache = dict()
 
@@ -33,18 +38,35 @@
 
         def log_likelihood(self, x):
             log_l = 0
             for pn in self.names:
                 log_l += norm.logpdf(x[pn])
             return log_l
 
+        def to_unit_hypercube(self, x):
+            x_out = x.copy()
+            for n in self.names:
+                x_out[n] = (x[n] - self.bounds[n][0]) / np.ptp(self.bounds[n])
+            return x_out
+
+        def from_unit_hypercube(self, x):
+            x_out = x.copy()
+            for n in self.names:
+                x_out[n] = np.ptp(self.bounds[n]) * x[n] + self.bounds[n][0]
+            return x_out
+
     return TestModel()
 
 
 @pytest.fixture()
+def integration_model():
+    return IntegrationTestModel()
+
+
+@pytest.fixture()
 def flow_config():
     d = dict(
         max_epochs=5,
         model_config=dict(
             n_blocks=2,
             n_neurons=2,
             n_layers=1,
@@ -64,34 +86,29 @@
 
     def func(*args, **kwargs):
         time.sleep(0.01)
 
     return func
 
 
-@pytest.fixture(params=["fork", "spawn"])
+@pytest.fixture(params=["fork", "forkserver", "spawn"])
 def mp_context(request):
     """Multiprocessing context to test"""
-    if request.param == "spawn":
-        pytest.skip(
-            "nessai does not currently support multiprocessing with the "
-            "'spawn' method."
-        )
-    if sys.platform == "win32":
-        pytest.skip("Windows does not support 'fork' method")
+    if sys.platform == "win32" and request.param != "spawn":
+        pytest.skip("Windows only supports the 'spawn' start method")
     return multiprocessing.get_context(request.param)
 
 
-def pytest_addoption(parser):
-    parser.addoption(
-        "--bilby-compatibility",
-        action="store_true",
-        default=False,
-        help="Run bilby compatibility tests",
-    )
+@pytest.fixture()
+def ins_parameters():
+    """Add (and remove) the standard INS parameters for the tests."""
+    # Before every test
+    add_extra_parameters_to_live_points(["logQ", "logW"])
+    yield
+    reset_extra_live_points_parameters()
 
 
 def pytest_configure(config):
     # register an additional marker
     config.addinivalue_line(
         "markers", "cuda: mark test to indicate it requires CUDA"
     )
@@ -108,14 +125,23 @@
     config.addinivalue_line(
         "markers",
         "bilby_compatibility: mark test as a bilby compatibility test, these "
         "tests will be skipped unless the command line option is specified.",
     )
 
 
+def pytest_addoption(parser):
+    parser.addoption(
+        "--bilby-compatibility",
+        action="store_true",
+        default=False,
+        help="Run bilby compatibility tests",
+    )
+
+
 def pytest_collection_modifyitems(config, items):
     if config.getoption("--bilby-compatibility"):
         return
     skip_bilby_compat = pytest.mark.skip(
         reason="Need --bilby-compatibility to run"
     )
     for item in items:
```

### Comparing `nessai-0.8.1/tests/test_bilby_compatibility.py` & `nessai-0.9.0/tests/test_bilby_compatibility.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_config.py` & `nessai-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_deprecation_warnings.py` & `nessai-0.9.0/tests/test_deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_evidence.py` & `nessai-0.9.0/tests/test_evidence/test_standard_evidence.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_flowmodel/test_flowmodel_base.py` & `nessai-0.9.0/tests/test_flowmodel/test_flowmodel_base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_flowmodel/test_flowmodel_utils.py` & `nessai-0.9.0/tests/test_flowmodel/test_flowmodel_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 Test the FlowModel utils.
 """
 import pytest
 from unittest.mock import patch
 
-from nessai.flowmodel import update_config
+from nessai.flowmodel.config import DEFAULT_MODEL_CONFIG
+from nessai.flowmodel.utils import update_config, update_model_config
+
+
+def test_update_config():
+    """Test with a basic config"""
+    model_config = dict(n_blocks=2)
+    config = dict(patience=1, model_config=model_config)
+    with patch(
+        "nessai.flowmodel.utils.update_model_config",
+        return_value=DEFAULT_MODEL_CONFIG.copy(),
+    ) as mock_update:
+        out = update_config(config)
+    mock_update.assert_called_once_with(model_config)
+    assert out["patience"] == 1
 
 
 def test_update_config_none():
     """Test update config for no input"""
-    config = update_config(None)
+    with patch(
+        "nessai.flowmodel.utils.update_model_config",
+        return_value=DEFAULT_MODEL_CONFIG.copy(),
+    ) as mock_update:
+        config = update_config(None)
+    mock_update.assert_called_once_with(None)
     assert "model_config" in config
 
 
 def test_update_config_invalid_type():
     """Test update config when an invalid argument is specified"""
     with pytest.raises(TypeError) as excinfo:
         update_config(False)
@@ -42,16 +61,28 @@
     """
     config = {"noise_type": "constant"}
     with pytest.raises(RuntimeError) as excinfo:
         update_config(config)
     assert "`noise_scale` must be specified" in str(excinfo.value)
 
 
-def test_update_config_n_neurons():
+def test_update_model_config_n_neurons():
     """Assert `get_n_neurons` is called"""
-    config = dict(model_config=dict(n_inputs=10))
+    config = dict(n_inputs=10)
     with patch(
         "nessai.flowmodel.utils.get_n_neurons", return_value=20
     ) as mock:
-        config = update_config(config)
+        config = update_model_config(config)
     mock.assert_called_once_with(n_neurons=None, n_inputs=10)
-    assert config["model_config"]["n_neurons"] == 20
+    assert config["n_neurons"] == 20
+
+
+def test_update_model_config_none():
+    """Assert the default is returned if the inputs is None"""
+    assert update_model_config(None) == DEFAULT_MODEL_CONFIG
+
+
+def test_update_model_config_type_error():
+    """Assert a type error is raised if the input is the wrong type"""
+    with pytest.raises(TypeError) as excinfo:
+        update_model_config(False)
+    assert "Must pass a dictionary" in str(excinfo.value)
```

### Comparing `nessai-0.8.1/tests/test_flows/test_base_flow.py` & `nessai-0.9.0/tests/test_flows/test_base_flow.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_flows/test_distributions.py` & `nessai-0.9.0/tests/test_flows/test_distributions/test_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_flows/test_flow_utils.py` & `nessai-0.9.0/tests/test_flows/test_flow_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,40 @@
 def test_get_base_distribution_error():
     """Assert an unknown dist raises an error."""
     with pytest.raises(ValueError) as excinfo:
         get_base_distribution(2, "not_a_distribution")
     assert "Unknown distribution: not_a_distribution" in str(excinfo.value)
 
 
+@pytest.mark.parametrize("name", ["lars", "resampled"])
+@pytest.mark.parametrize("n_layers", [None, 3])
+def test_get_base_distribution_lars(name, n_layers):
+    """Test using the LARS base distribution"""
+    kwargs = dict(test=False, net_kwargs=dict(dropout=0.1))
+    if n_layers:
+        kwargs["n_layers"] = n_layers
+    else:
+        n_layers = 2
+
+    mlp = object()
+
+    with patch("nessai.flows.utils.ResampledGaussian") as mock_dist, patch(
+        "nessai.flows.utils.MLP", return_value=mlp
+    ) as mock_mlp, patch(
+        "nessai.flows.utils.get_n_neurons", return_value=8
+    ) as mock_get_neurons:
+        get_base_distribution(2, name, **kwargs)
+
+    mock_get_neurons.assert_called_once_with(None, n_inputs=2)
+    mock_mlp.assert_called_once_with(
+        [2], [1], n_layers * [8], activate_output=torch.sigmoid, dropout=0.1
+    )
+    mock_dist.assert_called_once_with([2], mlp, test=False)
+
+
 @pytest.mark.parametrize(
     "n_neurons, n_inputs, expected",
     [
         (16, 2, 16),
         ("auto", 2, 4),
         ("double", 2, 4),
         (None, 2, 4),
```

### Comparing `nessai-0.8.1/tests/test_flows/test_included_flows.py` & `nessai-0.9.0/tests/test_flows/test_included_flows.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_flows/test_nets.py` & `nessai-0.9.0/tests/test_flows/test_nets.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_flows/test_specific_flows.py` & `nessai-0.9.0/tests/test_flows/test_specific_flows.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 @pytest.mark.parametrize(
     "kwargs",
     [
         dict(
             net="mlp", batch_norm_within_layers=True, dropout_probability=0.5
         ),
         dict(use_volume_preserving=True),
+        dict(actnorm=True),
         dict(linear_transform="permutation"),
         dict(linear_transform="svd"),
         dict(linear_transform="lu"),
         dict(linear_transform=None),
         dict(mask=np.array([[1, -1], [-1, 1]])),
         dict(mask=[1, -1]),
         dict(pre_transform="batch_norm"),
         dict(pre_transform="batch_norm", pre_transform_kwargs=dict(eps=1e-8)),
+        dict(scale_activation=lambda x: torch.sigmoid(x + 2) + 1e-3),
     ],
 )
 def test_with_realnvp_kwargs(kwargs):
     """Test RealNVP with specific kwargs"""
     flow = RealNVP(2, 2, 2, 2, **kwargs)
     x = torch.randn(10, 2)
     z, _ = flow.forward(x)
@@ -51,14 +53,24 @@
 def test_realnvp_value_errors(kwargs, string):
     """Assert incorrect values for some inputs raise an error"""
     with pytest.raises(ValueError) as excinfo:
         RealNVP(2, 2, 2, 2, **kwargs)
     assert string in str(excinfo.value)
 
 
+def test_realnvp_actnorm_batchnorm():
+    """
+    Assert an error is raised if actnorm and batchnorm are enabled at once.
+    """
+    with pytest.raises(
+        RuntimeError, match=r"Cannot enable actnorm and batchnorm .*"
+    ):
+        RealNVP(2, 2, 2, 2, actnorm=True, batch_norm_between_layers=True)
+
+
 @pytest.mark.parametrize(
     "kwargs",
     [
         dict(batch_norm_between_layers=True),
         dict(linear_transform="permutation"),
         dict(linear_transform="svd"),
         dict(linear_transform="lu"),
```

### Comparing `nessai-0.8.1/tests/test_flowsampler.py` & `nessai-0.9.0/tests/test_flowsampler.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 """
 import json
 import os
 import signal
 import sys
 import time
 from threading import Thread
-from unittest.mock import MagicMock, create_autospec, patch
+from unittest.mock import MagicMock, call, create_autospec, patch
 
 
 import h5py
 import pytest
+from nessai import config as nessai_config
 from nessai.evidence import _NSIntegralState
 from nessai.flowsampler import FlowSampler
 from nessai.livepoint import numpy_array_to_live_points
 import numpy as np
 
 
 @pytest.fixture()
 def flow_sampler():
-    return create_autospec(FlowSampler)
+    sampler = create_autospec(FlowSampler)
+    sampler.importance_nested_sampler = False
+    return sampler
 
 
 @pytest.fixture(autouse=True)
 def reset_handlers():
     """Reset signal handling after each test"""
     yield
     # Just in case the tests were ran on Windows
@@ -49,143 +52,168 @@
 
 @pytest.fixture()
 def nested_samples(names):
     return numpy_array_to_live_points(np.random.randn(20, len(names)), names)
 
 
 @pytest.mark.parametrize("resume", [False, True])
-def test_init_no_resume_file(flow_sampler, tmp_path, resume):
+@pytest.mark.parametrize("use_ins", [False, True])
+def test_init_no_resume_file(flow_sampler, tmp_path, resume, use_ins):
     """Test the init method when there is no run to resume from"""
 
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "init"
     output.mkdir()
     output = str(output)
     resume = resume
     exit_code = 131
     pytorch_threads = 2
     resume_file = "test.pkl"
     kwargs = dict(
         nlive=1000,
     )
     close_pool = True
 
+    sampler_class = "ImportanceNestedSampler" if use_ins else "NestedSampler"
+
     flow_sampler.save_kwargs = MagicMock()
 
     with patch(
-        "nessai.flowsampler.NestedSampler", return_value="ns"
+        f"nessai.flowsampler.{sampler_class}", return_value="ns"
     ) as mock, patch("nessai.flowsampler.configure_threads") as mock_threads:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             resume=resume,
             exit_code=exit_code,
             pytorch_threads=pytorch_threads,
             resume_file=resume_file,
             close_pool=close_pool,
+            importance_nested_sampler=use_ins,
             **kwargs,
         )
 
     mock_threads.assert_called_once_with(
         pytorch_threads=pytorch_threads,
         max_threads=None,
     )
 
     mock.assert_called_once_with(
-        model,
+        integration_model,
         output=os.path.join(output, ""),
         resume_file=resume_file,
         close_pool=False,
         **kwargs,
     )
 
     assert flow_sampler.ns == "ns"
 
     flow_sampler.save_kwargs.assert_called_once_with(kwargs)
 
 
+def test_init_eps(tmp_path):
+    initial_eps = nessai_config.general.eps
+
+    model = MagicMock()
+    output = tmp_path / "init"
+    output.mkdir()
+    output = str(output)
+    eps = 1e-4
+
+    flow_sampler.save_kwargs = MagicMock()
+
+    with patch("nessai.flowsampler.NestedSampler", return_value="ns"), patch(
+        "nessai.flowsampler.configure_threads"
+    ):
+        FlowSampler.__init__(flow_sampler, model, output=output, eps=eps)
+
+    assert nessai_config.general.eps == eps
+    assert nessai_config.general.eps != initial_eps
+    nessai_config.general.eps = initial_eps
+
+
 def test_disable_vectorisation(flow_sampler, tmp_path):
     """Assert vectorisation is disabled"""
     output = tmp_path / "test"
     output.mkdir()
 
-    model = MagicMock()
-    model.allow_vectorised = True
+    integration_model = MagicMock()
+    integration_model.allow_vectorised = True
 
     with patch("nessai.flowsampler.NestedSampler") as mock:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             disable_vectorisation=True,
         )
     mock.assert_called_once()
-    input_model = mock.call_args[0][0]
-    assert input_model.allow_vectorised is False
+    input_integration_model = mock.call_args[0][0]
+    assert input_integration_model.allow_vectorised is False
 
 
 def test_likelihood_chunksize(flow_sampler, tmp_path):
     """Assert the likelihood chunksize is set."""
     output = tmp_path / "test"
     output.mkdir()
 
-    model = MagicMock()
-    model.likelihood_chunksize = None
+    integration_model = MagicMock()
+    integration_model.likelihood_chunksize = None
 
     with patch("nessai.flowsampler.NestedSampler") as mock:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             likelihood_chunksize=100,
         )
     mock.assert_called_once()
-    input_model = mock.call_args[0][0]
-    assert input_model.likelihood_chunksize == 100
+    input_integration_model = mock.call_args[0][0]
+    assert input_integration_model.likelihood_chunksize == 100
 
 
 def test_allow_multi_valued_likelihood(flow_sampler, tmp_path):
     """Assert allow_multi_valued_likelihood is true"""
     output = tmp_path / "test"
     output.mkdir()
 
-    model = MagicMock()
-    model.allow_multi_value_likelihood = False
+    integration_model = MagicMock()
+    integration_model.allow_multi_value_likelihood = False
 
     with patch("nessai.flowsampler.NestedSampler") as mock:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             allow_multi_valued_likelihood=True,
         )
     mock.assert_called_once()
-    input_model = mock.call_args[0][0]
-    assert input_model.allow_multi_valued_likelihood is True
+    input_integration_model = mock.call_args[0][0]
+    assert input_integration_model.allow_multi_valued_likelihood is True
 
 
 @pytest.mark.parametrize(
     "test_old, error",
     [(False, None), (True, RuntimeError), (True, FileNotFoundError)],
 )
 def test_init_resume(flow_sampler, tmp_path, test_old, error):
     """Test the init method when the sampler should resume.
 
     Tests the case where the first file works and the case where the first
     file fails but the old method works.
     """
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "test"
     output.mkdir()
     resume = True
     exit_code = 131
     pytorch_threads = 2
     resume_file = "test.pkl"
-    weights_file = "model.pt"
+    weights_file = "integration_model.pt"
     flow_config = dict(lr=0.1)
 
     if test_old:
         expected_rf = output / (resume_file + ".old")
         side_effect = [error, "ns"]
     else:
         expected_rf = output / resume_file
@@ -205,15 +233,15 @@
     with patch(
         "nessai.flowsampler.NestedSampler.resume", side_effect=side_effect
     ) as mock_resume, patch(
         "nessai.flowsampler.configure_threads"
     ) as mock_threads:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             resume=resume,
             exit_code=exit_code,
             pytorch_threads=pytorch_threads,
             resume_file=resume_file,
             weights_file=weights_file,
             **kwargs,
@@ -222,27 +250,27 @@
     mock_threads.assert_called_once_with(
         pytorch_threads=pytorch_threads,
         max_threads=None,
     )
 
     mock_resume.assert_called_with(
         expected_rf,
-        model,
+        integration_model,
         flow_config=flow_config,
-        weights_file=weights_file,
+        weights_path=weights_file,
     )
 
     assert flow_sampler.ns == "ns"
 
     flow_sampler.save_kwargs.assert_called_once_with(kwargs)
 
 
 def test_init_resume_error_cannot_resume(flow_sampler, tmp_path):
     """Assert an error is raised if neither file loads"""
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "test"
     output.mkdir()
     resume = True
     resume_file = "test.pkl"
     expected_rf = output / (resume_file + ".old")
     expected_rf.write_text("contents")
     side_effect = [RuntimeError, RuntimeError]
@@ -254,83 +282,92 @@
     with patch(
         "nessai.flowsampler.NestedSampler.resume", side_effect=side_effect
     ), patch("nessai.flowsampler.configure_threads"), pytest.raises(
         RuntimeError
     ) as excinfo:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             resume=resume,
             resume_file=resume_file,
             flow_config=None,
         )
     assert "Could not resume sampler with error: " in str(excinfo.value)
 
 
 def test_init_resume_error_no_file(flow_sampler, tmp_path):
     """Assert an error is raised if resume=True and a resume_file is \
         not specified.
     """
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "test"
     output.mkdir()
     output = str(output)
 
     with patch("nessai.flowsampler.configure_threads"), pytest.raises(
         RuntimeError
     ) as excinfo:
         FlowSampler.__init__(
             flow_sampler,
-            model,
+            integration_model,
             output=output,
             resume=True,
             resume_file=None,
         )
     assert "`resume_file` must be specified" in str(excinfo.value)
 
 
 def test_init_signal_handling_enabled(flow_sampler, tmp_path):
     """Assert signal.signal is called when signal handling is enabled."""
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "test"
     output.mkdir()
     output = str(output)
 
     with patch("signal.signal") as mocked_fn:
         FlowSampler.__init__(
-            flow_sampler, model, output=output, signal_handling=True
+            flow_sampler,
+            integration_model,
+            output=output,
+            signal_handling=True,
         )
     mocked_fn.assert_called()
 
 
 def test_init_signal_handling_disabled(flow_sampler, tmp_path):
     """Assert signal handling is not configure when disabled"""
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "test"
     output.mkdir()
     output = str(output)
 
     with patch("signal.signal") as mocked_fn:
         FlowSampler.__init__(
-            flow_sampler, model, output=output, signal_handling=False
+            flow_sampler,
+            integration_model,
+            output=output,
+            signal_handling=False,
         )
     mocked_fn.assert_not_called()
 
 
 def test_init_signal_handling_error(flow_sampler, tmp_path, caplog):
     """Assert signal handling is skipped if an error is raised."""
-    model = MagicMock()
+    integration_model = MagicMock()
     output = tmp_path / "test"
     output.mkdir()
     output = str(output)
 
     with patch("signal.signal", side_effect=AttributeError):
         FlowSampler.__init__(
-            flow_sampler, model, output=output, signal_handling=True
+            flow_sampler,
+            integration_model,
+            output=output,
+            signal_handling=True,
         )
     assert "Cannot set signal attributes" in str(caplog.text)
 
 
 def test_log_evidence(flow_sampler):
     """Test log-evidence property"""
     out = 0.0
@@ -341,22 +378,44 @@
 def test_log_evidence_error(flow_sampler):
     """Test log-evidence property"""
     out = 0.1
     flow_sampler.logZ_error = out
     assert FlowSampler.log_evidence_error.__get__(flow_sampler) is out
 
 
+@pytest.mark.parametrize("use_ins", [False, True])
+def test_run(flow_sampler, use_ins):
+
+    flow_sampler.importance_nested_sampler = use_ins
+
+    kwargs = dict(
+        plot=False,
+        save=False,
+        posterior_sampling_method="test",
+        close_pool=True,
+        plot_posterior=True,
+    )
+    FlowSampler.run(flow_sampler, **kwargs)
+
+    if use_ins:
+        flow_sampler.run_importance_nested_sampler.assert_called_once_with(
+            **kwargs
+        )
+    else:
+        flow_sampler.run_standard_sampler.assert_called_once_with(**kwargs)
+
+
 @pytest.mark.parametrize("save", [False, True])
 @pytest.mark.parametrize("plot", [False, True])
 @patch(
     "nessai.flowsampler.draw_posterior_samples", return_value=np.array([0.1])
 )
 @patch("nessai.plot.plot_live_points")
 @patch("nessai.plot.plot_indices")
-def test_run(
+def test_run_standard(
     mock_plot_indices, mock_plot_post, mock_draw_post, flow_sampler, save, plot
 ):
     """Test the run method"""
     nlive = 10
     log_Z = -5.0
     nested_samples = [0.1, 1.0, 10.0]
     log_w = np.array([-0.1, -0.2, -0.3])
@@ -373,15 +432,15 @@
     flow_sampler.ns.state = MagicMock()
     flow_sampler.ns.state.log_posterior_weights = log_w
     flow_sampler.ns.state.plot_state = MagicMock()
     flow_sampler.save_results = MagicMock()
     flow_sampler.close_pool = True
     flow_sampler.result_extension = "hdf5"
 
-    FlowSampler.run(flow_sampler, save=save, plot=plot)
+    FlowSampler.run_standard_sampler(flow_sampler, save=save, plot=plot)
 
     flow_sampler.ns.initialise.assert_called_once()
     mock_draw_post.assert_called_once_with(
         nested_samples, log_w=log_w, method="rejection_sampling"
     )
     if save:
         flow_sampler.save_results.assert_called_once_with(
@@ -406,87 +465,168 @@
         )
     else:
         mock_plot_indices.assert_not_called()
         mock_plot_post.assert_not_called()
         flow_sampler.ns.state.plot.assert_not_called()
 
     assert flow_sampler.logZ == log_Z
-    assert flow_sampler.nested_samples == nested_samples
+    assert flow_sampler._nested_samples == nested_samples
     np.testing.assert_array_equal(
         flow_sampler.posterior_samples, np.array([0.1])
     )
 
 
 @pytest.mark.parametrize("close_pool", [True, False, None])
-def test_run_close_pool(flow_sampler, close_pool):
+def test_run_close_pool_standard(flow_sampler, close_pool):
     """Assert close pool is called following the intended logic"""
     flow_sampler.close_pool = True
     flow_sampler.ns = MagicMock()
     flow_sampler.ns.close_pool = MagicMock()
     flow_sampler.ns.nested_sampling_loop = MagicMock(return_value=("lZ", "ns"))
     with patch("nessai.flowsampler.draw_posterior_samples"):
-        FlowSampler.run(
+        FlowSampler.run_standard_sampler(
             flow_sampler, close_pool=close_pool, save=False, plot=False
         )
 
     # If True should be called
     # If None, should fallback to self.close_pool which is true
     if close_pool or close_pool is None:
         flow_sampler.ns.close_pool.assert_called_once()
     else:
         flow_sampler.ns.close_pool.assert_not_called()
 
 
 @pytest.mark.parametrize("method", (None, "multinomial_resampling"))
-def test_run_posterior_sampling_method(flow_sampler, method):
+def test_run_posterior_sampling_method_standard(flow_sampler, method):
     """Assert posterior sampling method is passed correctly"""
     log_w = np.random.rand(100)
     flow_sampler.ns = MagicMock()
     flow_sampler.ns.nested_sampling_loop = MagicMock(return_value=("lZ", "ns"))
     flow_sampler.ns.state = MagicMock(spec=_NSIntegralState)
     flow_sampler.ns.state.log_posterior_weights = log_w
     with patch("nessai.flowsampler.draw_posterior_samples") as mock:
-        FlowSampler.run(
+        FlowSampler.run_standard_sampler(
             flow_sampler,
             close_pool=False,
             save=False,
             plot=False,
             posterior_sampling_method=method,
         )
 
     if method is None:
         method = "rejection_sampling"
     mock.assert_called_once_with("ns", log_w=log_w, method=method)
 
 
-def test_run_plots_disabled(flow_sampler):
+def test_run_standard_plots_disabled(flow_sampler):
     """Assert individual plots can be disabled when plot=True"""
     flow_sampler.ns = MagicMock()
     flow_sampler.ns.nested_sampling_loop = MagicMock(return_value=("lZ", "ns"))
     flow_sampler.ns.nlive = 100
     flow_sampler.state = MagicMock()
     flow_sampler.state.plot = MagicMock()
 
     with patch("nessai.flowsampler.draw_posterior_samples"), patch(
         "nessai.plot.plot_indices"
     ) as mock_indices, patch("nessai.plot.plot_live_points") as mock_post:
-        FlowSampler.run(
+        FlowSampler.run_standard_sampler(
             flow_sampler,
             plot=True,
             save=False,
             close_pool=False,
             plot_indices=False,
             plot_posterior=False,
             plot_logXlogL=False,
         )
     mock_indices.assert_not_called()
     mock_post.assert_not_called()
     flow_sampler.state.plot.assert_not_called()
 
 
+def test_run_ins(flow_sampler):
+    """Test running the importance nested sampler"""
+    flow_sampler.importance_nested_sampler = True
+
+    flow_sampler.close_pool = False
+    logZ = 0.0
+    logZ_err = 0.1
+    nested_samples = np.array([1, 2, 3])
+    post = np.array([1, 2])
+    ns = MagicMock()
+    ns.nested_sampling_loop = MagicMock(return_value=(logZ, nested_samples))
+    ns.state.log_evidence_error = logZ_err
+    ns.draw_posterior_samples = MagicMock(return_value=post)
+    flow_sampler.ns = ns
+
+    FlowSampler.run_importance_nested_sampler(
+        flow_sampler, redraw_samples=False, save=False, plot=False
+    )
+
+    ns.draw_posterior_samples.assert_called_once_with(
+        sampling_method="importance_sampling",
+        use_final_samples=False,
+    )
+
+    assert flow_sampler.logZ is logZ
+    assert flow_sampler.logZ_error is logZ_err
+    assert flow_sampler.initial_posterior_samples is post
+    assert flow_sampler.posterior_samples is post
+
+
+def test_run_ins_redraw(flow_sampler):
+    """Test running the importance nested sampler and redrawing samples"""
+    flow_sampler.importance_nested_sampler = True
+    flow_sampler.close_pool = False
+    logZ = 0.0
+    logZ_err = 0.1
+    final_logZ = 0.01
+    final_logZ_err = 0.11
+    nested_samples = np.array([1, 2, 3])
+    final_samples = np.array([4, 5, 6])
+    post = np.array([1, 2])
+    final_post = np.array([4, 5])
+    ns = MagicMock()
+    ns.nested_sampling_loop = MagicMock(return_value=(logZ, nested_samples))
+    ns.state.log_evidence_error = logZ_err
+    ns.final_log_evidence_error = final_logZ_err
+    ns.draw_posterior_samples = MagicMock(
+        side_effect=[post, final_post],
+    )
+    ns.draw_final_samples = MagicMock(return_value=(final_logZ, final_samples))
+    flow_sampler.ns = ns
+
+    FlowSampler.run_importance_nested_sampler(
+        flow_sampler,
+        redraw_samples=True,
+        save=False,
+        plot=False,
+        compute_initial_posterior=True,
+    )
+
+    assert ns.draw_posterior_samples.has_calls(
+        [
+            call(
+                sampling_method="importance_sampling", use_final_samples=False
+            ),
+            call(
+                sampling_method="importance_sampling", use_final_samples=True
+            ),
+        ],
+        any_order=False,
+    )
+
+    assert flow_sampler.initial_logZ is logZ
+    assert flow_sampler.initial_logZ_error is logZ_err
+    assert flow_sampler.initial_posterior_samples is post
+
+    assert flow_sampler.logZ is final_logZ
+    assert flow_sampler.logZ_error is final_logZ_err
+    assert flow_sampler.posterior_samples is final_post
+
+
 @pytest.mark.parametrize("test_class", [False, True])
 def test_save_kwargs(flow_sampler, tmpdir, test_class):
     """Test the save kwargs method.
 
     If `test_class` is true, tests the case of the flow class being a class
     rather than a string.
     """
@@ -495,14 +635,17 @@
         from nessai.proposal import FlowProposal
 
         kwargs["flow_class"] = FlowProposal
     else:
         kwargs["flow_class"] = "flowproposal"
 
     flow_sampler.output = str(tmpdir.mkdir("test"))
+    flow_sampler.eps = 1e-8
+    flow_sampler.torch_dtype = "float32"
+    flow_sampler.importance_nested_sampler = False
 
     FlowSampler.save_kwargs(flow_sampler, kwargs)
 
     assert os.path.exists(os.path.join(flow_sampler.output, "config.json"))
 
 
 @pytest.mark.parametrize(
@@ -592,29 +735,31 @@
     flow_sampler.terminate_run.assert_called_once_with(code=2)
 
 
 @pytest.mark.parametrize("kwargs", [dict(n_pool=None), dict(n_pool=2)])
 @pytest.mark.slow_integration_test
 @pytest.mark.timeout(60)
 @pytest.mark.skip_on_windows
-def test_signal_handling(tmp_path, caplog, model, kwargs, mp_context):
+def test_signal_handling(
+    tmp_path, caplog, integration_model, kwargs, mp_context
+):
     """Test the signal handling in nessai.
 
     Test is based on a similar test in bilby which is in turn based on: \
         https://stackoverflow.com/a/49615525/18400311
     """
     output = tmp_path / "output"
     output.mkdir()
 
     with patch("multiprocessing.Pool", mp_context.Pool), patch(
         "nessai.utils.multiprocessing.multiprocessing.get_start_method",
         mp_context.get_start_method,
     ):
         fs = FlowSampler(
-            model,
+            integration_model,
             output=output,
             nlive=500,
             poolsize=1000,
             exit_code=5,
             signal_handling=True,
             **kwargs,
         )
@@ -641,25 +786,25 @@
         caplog.text
     )
 
 
 @pytest.mark.slow_integration_test
 @pytest.mark.timeout(60)
 @pytest.mark.skip_on_windows
-def test_signal_handling_disabled(tmp_path, caplog, model):
+def test_signal_handling_disabled(tmp_path, caplog, integration_model):
     """Assert signal handling is correctly disabled.
 
     Test is based on a similar test in bilby which is in turn based on: \
         https://stackoverflow.com/a/49615525/18400311
     """
     output = tmp_path / "output"
     output.mkdir()
 
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=500,
         poolsize=1000,
         exit_code=4,
         signal_handling=False,
     )
 
@@ -701,14 +846,15 @@
     d = dict(a=1)
 
     ns = MagicMock()
     ns.get_result_dictionary = MagicMock(return_value=d)
 
     flow_sampler.ns = ns
     flow_sampler.posterior_samples = posterior_samples
+    flow_sampler.initial_posterior_samples = posterior_samples.copy()
 
     FlowSampler.save_results(flow_sampler, filename)
 
     assert os.path.exists(filename)
     ns.get_result_dictionary.assert_called_once()
 
     if extension == "hdf5":
```

### Comparing `nessai-0.8.1/tests/test_gw/conftest.py` & `nessai-0.9.0/tests/test_gw/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_gw/test_distance_converters.py` & `nessai-0.9.0/tests/test_gw/test_distance_converters.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_gw/test_gw_proposal.py` & `nessai-0.9.0/tests/test_gw/test_gw_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_gw/test_gw_reparameterisations.py` & `nessai-0.9.0/tests/test_gw/test_gw_reparameterisations.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_gw/test_reparameterisation_integration.py` & `nessai-0.9.0/tests/test_gw/test_reparameterisation_integration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_livepoint.py` & `nessai-0.9.0/tests/test_livepoint.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_model.py` & `nessai-0.9.0/tests/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 import datetime
 import logging
 import numpy as np
 import pytest
 from scipy.stats import norm
 from unittest.mock import MagicMock, call, create_autospec, patch
 
+from nessai import config
 from nessai.livepoint import numpy_array_to_live_points
 from nessai.model import Model, OneDimensionalModelError
 from nessai.utils.multiprocessing import (
     initialise_pool_variables,
     log_likelihood_wrapper,
 )
-from nessai.utils.testing import assert_structured_arrays_equal
+from nessai.utils.testing import (
+    assert_structured_arrays_equal,
+)
 
 
 class EmptyModel(Model):
     def log_prior(self, x):
         return None
 
     def log_likelihood(self, x):
         return None
 
 
-class TestModel(Model):
+class BasicModel(Model):
     def __init__(self):
         self.bounds = {"x": [-5, 5], "y": [-5, 5]}
         self.names = ["x", "y"]
 
     def log_prior(self, x):
         log_p = np.log(self.in_bounds(x), dtype="float")
         for n in self.names:
@@ -40,36 +43,14 @@
     def log_likelihood(self, x):
         log_l = np.ones(x.size)
         for pn in self.names:
             log_l += norm.logpdf(x[pn])
         return log_l
 
 
-@pytest.fixture()
-def integration_model():
-    class IntegrationModel(Model):
-        def __init__(self):
-            self.bounds = {"x": [-5, 5], "y": [-5, 5]}
-            self.names = ["x", "y"]
-
-        def log_prior(self, x):
-            log_p = np.log(self.in_bounds(x), dtype="float")
-            for n in self.names:
-                log_p -= np.log(self.bounds[n][1] - self.bounds[n][0])
-            return log_p
-
-        def log_likelihood(self, x):
-            log_l = np.ones(x.size)
-            for pn in self.names:
-                log_l += norm.logpdf(x[pn])
-            return log_l
-
-    return IntegrationModel()
-
-
 @pytest.fixture
 def model():
     return create_autospec(Model, _pool_configured=False)
 
 
 @pytest.fixture
 def live_point(integration_model):
@@ -379,33 +360,33 @@
     Test the default method for generating a new point with the bounds.
 
     Uses the model defined in `conftest.py` with bounds [-5, 5] for
     x and y.
     """
     new_point = integration_model.new_point()
     log_q = integration_model.new_point_log_prob(new_point)
-    assert (new_point["x"] < 5) & (new_point["y"] > -5)
-    assert (new_point["y"] < 5) & (new_point["y"] > -5)
+    assert (new_point["x_0"] < 5) & (new_point["x_0"] > -5)
+    assert (new_point["x_1"] < 5) & (new_point["x_1"] > -5)
     assert log_q == 0
 
 
 @pytest.mark.integration_test
 def test_new_point_multiple_integration(integration_model):
     """
     Test drawing multiple new points from the model
 
     Uses the model defined in `conftest.py` with bounds [-5, 5] for
-    x and y.
+    x_0 and x_1.
     """
     new_points = integration_model.new_point(N=100)
     log_q = integration_model.new_point_log_prob(new_points)
     assert new_points.size == 100
     assert all(np.isnan(new_points["logP"]))
-    assert all(new_points["x"] < 5) & all(new_points["x"] > -5)
-    assert all(new_points["y"] < 5) & all(new_points["y"] > -5)
+    assert all(new_points["x_0"] < 5) & all(new_points["x_1"] > -5)
+    assert all(new_points["x_1"] < 5) & all(new_points["x_0"] > -5)
     assert (log_q == 0).all()
 
 
 def test_likelihood_evaluations(model, live_point):
     """
     Test `evaluate_log_likelihood` and ensure the counter increases.
     """
@@ -510,15 +491,15 @@
 
 def test_verify_new_point():
     """
     Test `Model.verify_model` and ensure a model with an ill-defined
     prior function raises the correct error
     """
 
-    class BrokenModel(TestModel):
+    class BrokenModel(BasicModel):
         def log_prior(self, x):
             return -np.inf
 
     model = BrokenModel()
 
     with pytest.raises(RuntimeError) as excinfo:
         model.verify_model()
@@ -529,15 +510,15 @@
 @pytest.mark.parametrize("log_p", [np.inf, -np.inf])
 def test_verify_log_prior_finite(log_p):
     """
     Test `Model.verify_model` and ensure a model with a log-prior that
     only returns inf function raises the correct error
     """
 
-    class BrokenModel(TestModel):
+    class BrokenModel(BasicModel):
         def log_prior(self, x):
             return log_p
 
     model = BrokenModel()
 
     with pytest.raises(RuntimeError):
         model.verify_model()
@@ -545,15 +526,15 @@
 
 def test_verify_log_prior_none():
     """
     Test `Model.verify_model` and ensure a model with a log-prior that
     only returns None raises an error.
     """
 
-    class BrokenModel(TestModel):
+    class BrokenModel(BasicModel):
         def log_prior(self, x):
             return None
 
     model = BrokenModel()
 
     with pytest.raises(RuntimeError) as excinfo:
         model.verify_model()
@@ -563,15 +544,15 @@
 
 def test_verify_log_likelihood_none():
     """
     Test `Model.verify_model` and ensure a model with a log-likelihood that
     only returns None raises an error.
     """
 
-    class BrokenModel(TestModel):
+    class BrokenModel(BasicModel):
         def log_likelihood(self, x):
             return None
 
     model = BrokenModel()
 
     with pytest.raises(RuntimeError) as excinfo:
         model.verify_model()
@@ -717,15 +698,15 @@
 @pytest.mark.parametrize("value", [np.log(True), np.float16(5.0)])
 def test_verify_float16(caplog, value):
     """
     Test `Model.verify_model` and ensure that a critical warning is raised
     if a float16 array is returned by the prior.
     """
 
-    class BrokenModel(TestModel):
+    class BrokenModel(BasicModel):
         def log_prior(self, x):
             return value
 
     model = BrokenModel()
 
     model.verify_model()
 
@@ -733,15 +714,15 @@
 
 
 def test_verify_no_float16(caplog):
     """
     Test `Model.verify_model` and ensure that a critical warning is not raised
     if array return by log_prior is not dtype float16.
     """
-    model = TestModel()
+    model = BasicModel()
     out = model.verify_model()
     assert out is True
     assert "float16 precision" not in caplog.text
 
 
 def test_unbounded_priors_wo_new_point():
     """Test `Model.verify_model` with unbounded priors"""
@@ -792,15 +773,15 @@
 
 
 def test_verify_model_likelihood_repeated_calls():
     """Assert that an error is raised if repeated calls with the likelihood
     return different values.
     """
 
-    class BrokenModel(TestModel):
+    class BrokenModel(BasicModel):
         count = 0
         allow_multi_valued_likelihood = False
 
         def log_likelihood(self, x):
             self.count += 1
             return self.count
 
@@ -812,15 +793,15 @@
 
 
 def test_verify_model_likelihood_repeated_calls_allowed(caplog):
     """Assert allow multi valued likelihood prevents an error from being
     raised.
     """
 
-    class MultiValuedModel(TestModel):
+    class MultiValuedModel(BasicModel):
         allow_multi_valued_likelihood = True
 
         def log_likelihood(self, x):
             return np.random.rand()
 
     model = MultiValuedModel()
     model.verify_model()
@@ -1113,36 +1094,65 @@
     model.pool = pool
     d = Model.__getstate__(model)
     assert d["pool"] is None
     assert model.pool is pool
 
 
 @pytest.mark.integration_test
-def test_pool(integration_model, mp_context):
+@pytest.mark.parametrize("pickleable", [False, True])
+@pytest.mark.parametrize("init", ["before", "after", "function"])
+def test_pool(integration_model, mp_context, pickleable, init):
     """Integration test for evaluating the likelihood with a pool"""
-    # Cannot pickle lambda functions
-    integration_model.fn = lambda x: x
-    initialise_pool_variables(integration_model)
-    pool = mp_context.Pool(1)
+    method = mp_context.get_start_method()
+
+    if not pickleable:
+        # Cannot pickle lambda functions
+        integration_model.fn = lambda x: x
+        if method != "fork":
+            pytest.xfail(f"start method {method} requires a pickleable model")
+
+    if init == "before":
+        if method != "fork":
+            pytest.xfail(f"Must use initializer in Pool with {method}")
+        initialise_pool_variables(integration_model)
+        pool = mp_context.Pool(1)
+    elif init == "function":
+        pool = mp_context.Pool(
+            1,
+            initializer=initialise_pool_variables,
+            initargs=(integration_model,),
+        )
+    elif init == "after":
+        if method != "fork":
+            pytest.xfail(f"Must use initializer in Pool with {method}")
+        pool = mp_context.Pool(1)
+        initialise_pool_variables(integration_model)
+    else:
+        raise ValueError(init)
+
     integration_model.configure_pool(pool=pool)
     assert integration_model.pool is pool
     x = integration_model.new_point(10)
     out = integration_model.batch_evaluate_log_likelihood(x)
 
-    target = np.fromiter(map(integration_model.log_likelihood, x), "float")
+    target = np.array(
+        [integration_model.log_likelihood(xx) for xx in x],
+        dtype=config.livepoints.logl_dtype,
+    ).flatten()
     np.testing.assert_array_equal(out, target)
     assert integration_model.likelihood_evaluations == 10
 
     integration_model.close_pool()
     assert integration_model.pool is None
 
 
 @pytest.mark.requires("ray")
 @pytest.mark.integration_test
 @pytest.mark.flaky(reruns=3)
+@pytest.mark.skip(reason="Skipping test with ray")
 def test_pool_ray(integration_model):
     """Integration test for evaluating the likelihood with a pool from ray.
 
     This will break if the class for integration_model is defined globally.
     """
     from ray.util.multiprocessing import Pool
 
@@ -1154,37 +1164,49 @@
         initargs=(integration_model,),
     )
     integration_model.configure_pool(pool=pool)
     assert integration_model.pool is pool
     x = integration_model.new_point(10)
     out = integration_model.batch_evaluate_log_likelihood(x)
 
-    target = np.fromiter(map(integration_model.log_likelihood, x), "float")
+    target = np.array(
+        [integration_model.log_likelihood(xx) for xx in x],
+        dtype=config.livepoints.logl_dtype,
+    ).flatten()
     np.testing.assert_array_equal(out, target)
     assert integration_model.likelihood_evaluations == 10
 
     integration_model.close_pool()
     assert integration_model.pool is None
 
 
 @pytest.mark.integration_test
-def test_n_pool(integration_model, mp_context):
+@pytest.mark.parametrize("pickleable", [False, True])
+def test_n_pool(integration_model, mp_context, pickleable):
     """Integration test for evaluating the likelihood with n_pool"""
-    # Cannot pickle lambda functions
-    integration_model.fn = lambda x: x
+    if not pickleable:
+        # Cannot pickle lambda functions
+        integration_model.fn = lambda x: x
+        method = mp_context.get_start_method()
+        if method != "fork":
+            pytest.xfail(f"start method {method} requires a pickleable model")
+
     with patch("multiprocessing.Pool", mp_context.Pool), patch(
         "nessai.utils.multiprocessing.multiprocessing.get_start_method",
         mp_context.get_start_method,
     ):
         integration_model.configure_pool(n_pool=1)
     assert integration_model.n_pool == 1
     x = integration_model.new_point(10)
     out = integration_model.batch_evaluate_log_likelihood(x)
 
-    target = np.fromiter(map(integration_model.log_likelihood, x), "float")
+    target = np.array(
+        [integration_model.log_likelihood(xx) for xx in x],
+        dtype=config.livepoints.logl_dtype,
+    ).flatten()
     np.testing.assert_array_equal(out, target)
     assert integration_model.likelihood_evaluations == 10
 
     integration_model.close_pool()
     assert integration_model.pool is None
```

### Comparing `nessai-0.8.1/tests/test_plot.py` & `nessai-0.9.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_posterior.py` & `nessai-0.9.0/tests/test_posterior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_priors.py` & `nessai-0.9.0/tests/test_priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_analytic.py` & `nessai-0.9.0/tests/test_proposal/test_analytic.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_augmented.py` & `nessai-0.9.0/tests/test_proposal/test_augmented.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_base_proposal.py` & `nessai-0.9.0/tests/test_proposal/test_base_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,24 @@
     """Make sure unknown latent priors raise an error"""
     proposal.latent_prior = "truncated"
     with pytest.raises(RuntimeError) as excinfo:
         FlowProposal.configure_latent_prior(proposal)
     assert "Unknown latent prior: truncated, " in str(excinfo.value)
 
 
-def test_configure_constant_volume(proposal):
+@pytest.mark.parametrize(
+    "latent_prior",
+    ["truncated_gaussian", "uniform_nball", "uniform_nsphere"],
+)
+def test_configure_constant_volume(proposal, latent_prior):
     """Test configuration for constant volume mode."""
     proposal.constant_volume_mode = True
     proposal.volume_fraction = 0.95
     proposal.rescaled_dims = 5
-    proposal.latent_prior = "truncated_gaussian"
+    proposal.latent_prior = latent_prior
     proposal.max_radius = 3.0
     proposal.min_radius = 5.0
     proposal.fuzz = 1.5
     with patch(
         "nessai.proposal.flowproposal.compute_radius", return_value=4.0
     ) as mock:
         FlowProposal.configure_constant_volume(proposal)
@@ -138,20 +142,19 @@
     mock.assert_not_called()
 
 
 def test_constant_volume_invalid_latent_prior(proposal):
     """Assert an error is raised if the latent prior is not a truncated \
         Gaussian
     """
-    err = "Constant volume requires `latent_prior='truncated_gaussian'`"
+    err = "Constant volume mode is not supported for latent_prior=gaussian"
     proposal.constant_volume_mode = True
     proposal.latent_prior = "gaussian"
-    with pytest.raises(RuntimeError) as excinfo:
+    with pytest.raises(RuntimeError, match=err):
         FlowProposal.configure_constant_volume(proposal)
-    assert str(excinfo.value) == err
 
 
 def test_update_flow_proposal(proposal):
     """Assert the number of inputs is updated"""
     proposal.flow_config = {"model_config": {}}
     proposal.rescaled_dims = 4
     FlowProposal.update_flow_config(proposal)
```

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     log_j = np.ones(data.shape[0])
 
     proposal.initialised = True
     proposal.training_count = 0
     proposal.populated = True
     proposal._plot_training = plot_training
     proposal.save_training_data = save
-    proposal.rescale_parameters = ["x"]
     proposal.rescaled_names = ["x_prime", "y_prime"]
     proposal.output = output
 
     proposal.check_state = MagicMock()
     proposal.rescale = MagicMock(return_value=(x_prime, log_j))
     proposal.flow = MagicMock()
     proposal.flow.train = MagicMock()
```

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
         expansion_fraction=None,
         rescale_parameters=False,
         max_radius=0.1,
         constant_volume_mode=False,
     )
 
     fp.initialise()
+    assert fp.rescale_parameters is False
+    assert fp.parameters_to_rescale == []
     worst = numpy_array_to_live_points(0.01 * np.ones(fp.dims), fp.names)
     fp.populate(worst, N=n_draw)
 
     assert fp.x.size == n_draw
 
 
 @pytest.mark.parametrize("plot", [False, True])
```

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         proposal.training_data_prime,
         x_gen,
         x_prime_gen,
     ]:
         array["logL"] = 0.0
 
     proposal.dims = 2
-    proposal.rescale_parameters = names
+    proposal.rescale_parameters = True
+    proposal.parameters_to_rescale = names
     proposal.rescaled_names = prime_names
 
     proposal.forward_pass = MagicMock(return_value=(z, None))
     proposal.backward_pass = MagicMock(return_value=(x_prime_gen, np.ones(10)))
     proposal.inverse_rescale = MagicMock(return_value=(x_gen, np.ones(10)))
     proposal.check_prior_bounds = lambda *args: args
     proposal.model = MagicMock()
```

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_population.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py` & `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = None
     FlowProposal.configure_reparameterisations(proposal, {"x": "default"})
 
     proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x_prime", "y"]
-    assert proposal.rescale_parameters == ["x"]
+    assert proposal.parameters_to_rescale == ["x"]
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == ["x_prime", "y"]
     assert mocked_class.called_once
 
 
 @patch("nessai.reparameterisations.CombinedReparameterisation")
 def test_configure_reparameterisations_dict_reparam(mocked_class, proposal):
@@ -242,33 +242,70 @@
     proposal.fallback_reparameterisation = None
     FlowProposal.configure_reparameterisations(
         proposal, {"default": {"parameters": ["x"]}}
     )
 
     proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x_prime", "y"]
-    assert proposal.rescale_parameters == ["x"]
+    assert proposal.parameters_to_rescale == ["x"]
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == ["x_prime", "y"]
     assert mocked_class.called_once
 
 
+@pytest.mark.parametrize(
+    "parameters",
+    [
+        "x.*",
+        [
+            "x.*",
+        ],
+        ("x.*",),
+    ],
+)
+@patch("nessai.reparameterisations.CombinedReparameterisation")
+def test_configure_reparameterisations_regex(
+    mocked_class, proposal, parameters
+):
+    """Test configuration for reparameterisations dictionary"""
+    proposal.add_default_reparameterisations = MagicMock()
+    proposal.get_reparameterisation = get_reparameterisation
+    proposal.model.names = ["x_0", "x_1", "y"]
+    proposal.model.bounds = {"x_0": [-1, 1], "x_1": [-1, 1], "y": [-1, 1]}
+    proposal.fallback_reparameterisation = None
+    FlowProposal.configure_reparameterisations(
+        proposal,
+        {"z-score": {"parameters": parameters}},
+    )
+
+    proposal.add_default_reparameterisations.assert_not_called()
+    assert proposal.rescaled_names == ["x_0_prime", "x_1_prime", "y"]
+    assert proposal.parameters_to_rescale == ["x_0", "x_1"]
+    assert proposal._reparameterisation.parameters == ["x_0", "x_1", "y"]
+    assert proposal._reparameterisation.prime_parameters == [
+        "x_0_prime",
+        "x_1_prime",
+        "y",
+    ]
+    assert mocked_class.called_once
+
+
 @patch("nessai.reparameterisations.CombinedReparameterisation")
 def test_configure_reparameterisations_none(mocked_class, proposal):
     """Test configuration when input is None"""
     proposal.add_default_reparameterisations = MagicMock()
     proposal.get_reparameterisation = get_reparameterisation
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = None
     FlowProposal.configure_reparameterisations(proposal, None)
     proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x", "y"]
 
-    assert proposal.rescale_parameters == []
+    assert proposal.parameters_to_rescale == []
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == ["x", "y"]
     assert all(
         [
             isinstance(r, NullReparameterisation)
             for r in proposal._reparameterisation.reparameterisations.values()
         ]
@@ -284,15 +321,15 @@
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = "default"
     FlowProposal.configure_reparameterisations(proposal, None)
     proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x_prime", "y_prime"]
 
-    assert proposal.rescale_parameters == ["x", "y"]
+    assert proposal.parameters_to_rescale == ["x", "y"]
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == [
         "x_prime",
         "y_prime",
     ]
     assert all(
         [
@@ -356,15 +393,15 @@
     Test setting the rescaling when the model contains reparmaeterisations.
     """
     proposal.model = model
     proposal.model.reparameterisations = {"x": "default"}
 
     def update(self):
         proposal.names = model.names
-        proposal.rescale_parameters = ["x"]
+        proposal.parameters_to_rescale = ["x"]
         proposal.rescaled_names = ["x_prime"]
 
     proposal.configure_reparameterisations = MagicMock()
     proposal.configure_reparameterisations.side_effect = update
 
     FlowProposal.set_rescaling(proposal)
 
@@ -381,15 +418,15 @@
     """
     proposal.model = model
     proposal.model.reparameterisations = None
     proposal.reparameterisations = {"x": "default"}
 
     def update(self):
         proposal.names = model.names
-        proposal.rescale_parameters = ["x"]
+        proposal.parameters_to_rescale = ["x"]
         proposal.rescaled_names = ["x_prime"]
 
     proposal.configure_reparameterisations = MagicMock()
     proposal.configure_reparameterisations.side_effect = update
 
     FlowProposal.set_rescaling(proposal)
 
@@ -414,15 +451,15 @@
 
     _rescale_parameters = (
         model.names if rescale_parameters is True else rescale_parameters
     )
 
     def update(self):
         proposal.names = model.names
-        proposal.rescale_parameters = _rescale_parameters
+        proposal.parameters_to_rescale = _rescale_parameters
         proposal.rescaled_names = rescaled_names
 
     proposal.model = model
     proposal.model.reparameterisations = None
     proposal.reparameterisations = None
     proposal.configure_reparameterisations = MagicMock()
     proposal.configure_reparameterisations.side_effect = update
@@ -448,14 +485,15 @@
             "detect_edges_kwargs": detect_edges_kwargs,
         },
     }
 
     proposal.configure_reparameterisations.assert_called_with(
         reparameterisations
     )
+    proposal.parameters_to_rescale == _rescale_parameters
 
 
 @pytest.mark.parametrize("n", [1, 10])
 def test_rescale(proposal, n):
     """Test rescaling when using reparameterisation dict"""
     x = numpy_array_to_live_points(np.random.randn(n, 2), ["x", "y"])
     x["logL"] = np.random.randn(n)
```

### Comparing `nessai-0.8.1/tests/test_proposal/test_rejection.py` & `nessai-0.9.0/tests/test_proposal/test_rejection.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_proposal/test_utils.py` & `nessai-0.9.0/tests/test_proposal/test_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/conftest.py` & `nessai-0.9.0/tests/test_reparameterisations/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_angle.py` & `nessai-0.9.0/tests/test_reparameterisations/test_angle.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_angle_pair.py` & `nessai-0.9.0/tests/test_reparameterisations/test_angle_pair.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_base_reparameterisation.py` & `nessai-0.9.0/tests/test_reparameterisations/test_base_reparameterisation.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_combined.py` & `nessai-0.9.0/tests/test_reparameterisations/test_combined.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_get_reparameterisation.py` & `nessai-0.9.0/tests/test_reparameterisations/test_get_reparameterisation.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_null.py` & `nessai-0.9.0/tests/test_reparameterisations/test_null.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_rescale_to_bounds.py` & `nessai-0.9.0/tests/test_reparameterisations/test_rescale_to_bounds.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_scale_and_shift.py` & `nessai-0.9.0/tests/test_reparameterisations/test_scale_and_shift.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_reparameterisations/test_to_cartesian.py` & `nessai-0.9.0/tests/test_reparameterisations/test_to_cartesian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_base_sampler.py` & `nessai-0.9.0/tests/test_samplers/test_base_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,20 @@
 def test_current_sampling_time_finalised(sampler):
     """Test the current sampling time if the sampling has been finalised"""
     sampler.finalised = True
     sampler.sampling_time = 10
     assert BaseNestedSampler.current_sampling_time.__get__(sampler) == 10
 
 
+def test_posterior_effective_sample_suze(sampler):
+    """Assert an error is raised"""
+    with pytest.raises(NotImplementedError):
+        BaseNestedSampler.posterior_effective_sample_size.__get__(sampler)
+
+
 @patch("numpy.random.seed")
 @patch("torch.manual_seed")
 def test_set_random_seed(mock1, mock2, sampler):
     """Test the correct functions are called when setting the random seed"""
     BaseNestedSampler.configure_random_seed(sampler, 150914)
     mock1.assert_called_once_with(150914)
     mock2.assert_called_once_with(seed=150914)
```

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_core_sampling.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_core_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_flow_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_general_config.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_general_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_live_points.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_live_points.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_manage_state.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_manage_state.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_ns_plotting.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_properties.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,7 +87,14 @@
     assert NestedSampler.mean_acceptance.__get__(sampler) == 2.0
 
 
 def test_mean_acceptance_empty(sampler):
     """Assert nan is returned if no points have been proposed"""
     sampler.acceptance_history = deque(maxlen=10)
     assert np.isnan(NestedSampler.mean_acceptance.__get__(sampler))
+
+
+def test_posterior_effective_sample_size(sampler):
+    """Assert the state property is called"""
+    sampler.state.effective_n_posterior_samples = 10
+    out = NestedSampler.posterior_effective_sample_size.__get__(sampler)
+    assert out == 10
```

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_proposal_config.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_proposal_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_resume.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_resume.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     with patch(
         "nessai.samplers.base.BaseNestedSampler.resume", return_value=obj
     ) as mock:
         out = NestedSampler.resume(
             "test.pkl",
             model,
             flow_config=flow_config,
-            weights_file=weights_file,
+            weights_path=weights_file,
         )
     assert out is obj
     mock.assert_called_once_with("test.pkl", model)
     obj._uninformed_proposal.resume.assert_called_once_with(
         model,
     )
     obj._flow_proposal.resume.assert_called_once_with(
```

### Comparing `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_yield_sample.py` & `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_yield_sample.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_sampling.py` & `nessai-0.9.0/tests/test_sampling/test_standard_sampling.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,47 +9,28 @@
 import pytest
 import numpy as np
 from unittest.mock import patch
 
 from nessai.flowsampler import FlowSampler
 from nessai.livepoint import numpy_array_to_live_points
 from nessai.model import Model
+from nessai.utils.testing import IntegrationTestModel
 
 
 torch.set_num_threads(1)
 
 
-class BaseModel(Model):
-    """Base model class for sampling tests"""
-
-    def __init__(self):
-        self.bounds = {"x": [-5, 5], "y": [-5, 5]}
-        self.names = ["x", "y"]
-
-    def log_prior(self, x):
-        log_p = np.log(self.in_bounds(x), dtype="float")
-        for n in self.names:
-            log_p -= self.bounds[n][1] - self.bounds[n][0]
-        return log_p
-
-    def log_likelihood(self, x):
-        log_l = np.zeros(x.size)
-        for pn in self.names:
-            log_l += norm.logpdf(x[pn])
-        return log_l
-
-
 @pytest.mark.slow_integration_test
-def test_sampling_with_rescale(model, flow_config, tmpdir):
+def test_sampling_with_rescale(integration_model, flow_config, tmpdir):
     """
     Test sampling with rescaling. Checks that flow is trained.
     """
     output = str(tmpdir.mkdir("w_rescale"))
     fp = FlowSampler(
-        model,
+        integration_model,
         output=output,
         resume=False,
         nlive=100,
         plot=False,
         flow_config=flow_config,
         training_frequency=10,
         maximum_uninformed=9,
@@ -60,21 +41,21 @@
     )
     fp.run()
     assert fp.ns.proposal.flow.weights_file is not None
     assert fp.ns.proposal.training_count == 1
 
 
 @pytest.mark.slow_integration_test
-def test_sampling_with_inversion(model, flow_config, tmpdir):
+def test_sampling_with_inversion(integration_model, flow_config, tmpdir):
     """
     Test sampling with inversion. Checks that flow is trained.
     """
     output = str(tmpdir.mkdir("w_rescale"))
     fp = FlowSampler(
-        model,
+        integration_model,
         output=output,
         resume=False,
         nlive=100,
         plot=False,
         flow_config=flow_config,
         training_frequency=10,
         maximum_uninformed=9,
@@ -84,28 +65,47 @@
         poolsize=10,
         boundary_inversion=True,
         update_bounds=True,
     )
     fp.run()
     reparams = list(fp.ns.proposal._reparameterisation.values())
     assert len(reparams) == 1
-    assert reparams[0].parameters == ["x", "y"]
-    assert list(reparams[0].boundary_inversion.keys()) == ["x", "y"]
+    assert reparams[0].parameters == ["x_0", "x_1"]
+    assert list(reparams[0].boundary_inversion.keys()) == ["x_0", "x_1"]
     assert fp.ns.proposal.flow.weights_file is not None
     assert fp.ns.proposal.training_count == 1
 
 
+def test_sampling_regex_reparams(model, flow_config, tmp_path):
+    """Test using regex to specify reparameterisations"""
+    model._names = ["x_0", "x_1"]
+    model._bounds = {"x_0": [-5, 5], "x_1": [-5, 5]}
+
+    fs = FlowSampler(
+        model,
+        nlive=100,
+        output=tmp_path / "test_regex",
+        flow_config=flow_config,
+        reparameterisations={"z-score": {"parameters": ["x.*"]}},
+        maximum_uninformed=50,
+        max_iteration=100,
+        plot=False,
+    )
+    fs.run()
+    assert fs.ns._flow_proposal.rescaled_names == ["x_0_prime", "x_1_prime"]
+
+
 @pytest.mark.slow_integration_test
-def test_sampling_without_rescale(model, flow_config, tmpdir):
+def test_sampling_without_rescale(integration_model, flow_config, tmpdir):
     """
     Test sampling without rescaling. Checks that flow is trained.
     """
     output = str(tmpdir.mkdir("wo_rescale"))
     fp = FlowSampler(
-        model,
+        integration_model,
         output=output,
         resume=False,
         nlive=100,
         plot=False,
         flow_config=flow_config,
         training_frequency=10,
         maximum_uninformed=9,
@@ -116,23 +116,23 @@
     )
     fp.run()
     assert fp.ns.proposal.flow.weights_file is not None
     assert fp.ns.proposal.training_count == 1
 
 
 @pytest.mark.slow_integration_test
-def test_sampling_with_maf(model, flow_config, tmpdir):
+def test_sampling_with_maf(integration_model, flow_config, tmpdir):
     """
     Test sampling with MAF. Checks that flow is trained but does not
     check convergence.
     """
     flow_config["model_config"]["ftype"] = "maf"
     output = str(tmpdir.mkdir("maf"))
     fp = FlowSampler(
-        model,
+        integration_model,
         output=output,
         resume=False,
         nlive=100,
         plot=False,
         flow_config=flow_config,
         training_frequency=10,
         maximum_uninformed=9,
@@ -144,21 +144,21 @@
     fp.run()
     assert fp.ns.proposal.flow.weights_file is not None
     assert fp.ns.proposal.training_count == 1
 
 
 @pytest.mark.slow_integration_test
 @pytest.mark.parametrize("analytic", [False, True])
-def test_sampling_uninformed(model, flow_config, tmpdir, analytic):
+def test_sampling_uninformed(integration_model, flow_config, tmpdir, analytic):
     """
     Test running the sampler with the two uninformed proposal methods.
     """
     output = str(tmpdir.mkdir("uninformed"))
     fp = FlowSampler(
-        model,
+        integration_model,
         output=output,
         resume=False,
         nlive=100,
         plot=False,
         flow_config=flow_config,
         training_frequency=None,
         maximum_uninformed=10,
@@ -168,25 +168,27 @@
         poolsize=10,
         analytic_priors=analytic,
     )
     fp.run()
 
 
 @pytest.mark.slow_integration_test
-def test_sampling_with_n_pool(model, flow_config, tmpdir, mp_context):
+def test_sampling_with_n_pool(
+    integration_model, flow_config, tmpdir, mp_context
+):
     """
     Test running the sampler with multiprocessing.
     """
     output = str(tmpdir.mkdir("pool"))
     with patch("multiprocessing.Pool", mp_context.Pool), patch(
         "nessai.utils.multiprocessing.multiprocessing.get_start_method",
         mp_context.get_start_method,
     ):
         fp = FlowSampler(
-            model,
+            integration_model,
             output=output,
             resume=False,
             nlive=100,
             plot=False,
             flow_config=flow_config,
             training_frequency=10,
             maximum_uninformed=9,
@@ -240,25 +242,27 @@
     assert fp.ns.iteration == 21
     assert os.path.exists(
         os.path.join(output, "nested_sampler_resume.pkl.old")
     )
 
 
 @pytest.mark.slow_integration_test
-def test_sampling_resume_w_pool(model, flow_config, tmpdir, mp_context):
+def test_sampling_resume_w_pool(
+    integration_model, flow_config, tmpdir, mp_context
+):
     """
     Test resuming the sampler with a pool.
     """
     output = str(tmpdir.mkdir("resume"))
     with patch("multiprocessing.Pool", mp_context.Pool), patch(
         "nessai.utils.multiprocessing.multiprocessing.get_start_method",
         mp_context.get_start_method,
     ):
         fp = FlowSampler(
-            model,
+            integration_model,
             output=output,
             resume=True,
             nlive=100,
             plot=False,
             flow_config=flow_config,
             training_frequency=10,
             maximum_uninformed=9,
@@ -270,22 +274,22 @@
             poolsize=10,
             n_pool=1,
         )
     assert fp.ns.model.n_pool == 1
     fp.run()
     assert os.path.exists(os.path.join(output, "nested_sampler_resume.pkl"))
     # Make sure the pool is already closed
-    model.close_pool()
+    integration_model.close_pool()
 
     with patch("multiprocessing.Pool", mp_context.Pool), patch(
         "nessai.utils.multiprocessing.multiprocessing.get_start_method",
         mp_context.get_start_method,
     ):
         fp = FlowSampler(
-            model,
+            integration_model,
             output=output,
             resume=True,
             flow_config=flow_config,
             n_pool=1,
         )
     assert fp.ns.model.n_pool == 1
     assert fp.ns.iteration == 11
@@ -294,25 +298,27 @@
     assert fp.ns.iteration == 21
     assert os.path.exists(
         os.path.join(output, "nested_sampler_resume.pkl.old")
     )
 
 
 @pytest.mark.slow_integration_test
-def test_sampling_resume_no_max_uninformed(model, flow_config, tmpdir):
+def test_sampling_resume_no_max_uninformed(
+    integration_model, flow_config, tmpdir
+):
     """
     Test resuming the sampler when there is no maximum iteration for
     the uinformed sampling.
 
     This test makes sure the correct proposal is loaded after resuming
     and re-initialising the sampler.
     """
     output = str(tmpdir.mkdir("resume"))
     fp = FlowSampler(
-        model,
+        integration_model,
         output=output,
         resume=True,
         nlive=100,
         plot=False,
         flow_config=flow_config,
         training_frequency=10,
         maximum_uninformed=9,
@@ -323,36 +329,87 @@
         checkpoint_interval=5,
         poolsize=10,
     )
     fp.run()
     assert os.path.exists(os.path.join(output, "nested_sampler_resume.pkl"))
 
     fp = FlowSampler(
-        model, output=output, resume=True, flow_config=flow_config
+        integration_model, output=output, resume=True, flow_config=flow_config
     )
     assert fp.ns.iteration == 11
     fp.ns.maximum_uninformed = np.inf
     fp.ns.initialise()
     assert fp.ns.proposal is fp.ns._flow_proposal
     fp.ns.max_iteration = 21
     fp.run()
     assert fp.ns.iteration == 21
     assert os.path.exists(
         os.path.join(output, "nested_sampler_resume.pkl.old")
     )
 
 
 @pytest.mark.slow_integration_test
+def test_resume_fallback_reparameterisation(tmpdir, model, flow_config):
+    """
+    Test resuming the sampler with the default reparameterisations disabled
+    and the fallback set.
+
+    This should load the same class after resuming.
+    """
+    from nessai.reparameterisations.rescale import ScaleAndShift
+
+    output = str(tmpdir.mkdir("resume"))
+    fp = FlowSampler(
+        model,
+        output=output,
+        resume=True,
+        nlive=100,
+        plot=False,
+        flow_config=flow_config,
+        training_frequency=10,
+        maximum_uninformed=9,
+        rescale_parameters=False,
+        use_default_reparameterisations=False,
+        fallback_reparameterisation="z-score",
+        checkpoint_on_iteration=True,
+        checkpoint_interval=5,
+        seed=1234,
+        max_iteration=11,
+        poolsize=10,
+    )
+    fp.run()
+
+    reparam = fp.ns._flow_proposal._reparameterisation
+    reparam = next(iter(fp.ns._flow_proposal._reparameterisation.values()))
+    assert isinstance(reparam, ScaleAndShift)
+    assert os.path.exists(os.path.join(output, "nested_sampler_resume.pkl"))
+
+    fp = FlowSampler(
+        model,
+        output=output,
+        resume=True,
+        flow_config=flow_config,
+    )
+    assert fp.ns.iteration == 11
+    fp.ns.max_iteration = 21
+    fp.run()
+    reparam = next(iter(fp.ns._flow_proposal._reparameterisation.values()))
+    assert isinstance(reparam, ScaleAndShift)
+    assert fp.ns.iteration == 21
+    assert os.path.exists(
+        os.path.join(output, "nested_sampler_resume.pkl.old")
+    )
+
+
+@pytest.mark.slow_integration_test
 def test_sampling_with_infinite_prior_bounds(tmpdir):
     """
     Make sure the sampler runs when sampling a parameter with infinite prior \
         bounds.
     """
-    from scipy.stats import norm
-
     output = str(tmpdir.mkdir("infinite_bounds"))
 
     class TestModel(Model):
 
         names = ["x", "y"]
         bounds = {"x": [0, 1], "y": [-np.inf, np.inf]}
         reparameterisations = {"x": "default", "y": None}
@@ -378,91 +435,91 @@
         TestModel(), output=output, nlive=500, plot=False, proposal_plots=False
     )
     fs.run(plot=False)
     assert fs.ns.condition <= 0.1
 
 
 @pytest.mark.slow_integration_test
-def test_constant_volume_mode(model, tmpdir):
+def test_constant_volume_mode(integration_model, tmpdir):
     """Test sampling in constant volume mode"""
     output = str(tmpdir.mkdir("test"))
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=500,
         plot=False,
         proposal_plots=False,
         constant_volume_mode=True,
     )
     fs.run(plot=False)
 
 
 @pytest.mark.slow_integration_test
-def test_prior_sampling(model, tmpdir):
+def test_prior_sampling(integration_model, tmpdir):
     """Test prior sampling"""
     output = str(tmpdir.mkdir("prior_sampling"))
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=100,
         plot=False,
         prior_sampling=True,
     )
     fs.run(plot=False)
 
     assert len(fs.nested_samples) == 100
     assert np.isfinite(fs.logZ)
 
 
 @pytest.mark.slow_integration_test
-def test_sampling_resume_finalised(model, tmp_path):
+def test_sampling_resume_finalised(integration_model, tmp_path):
     """Test resuming the sampler after it finishes sampling"""
     output = tmp_path / "output"
     output.mkdir()
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=100,
         plot=False,
     )
     fs.run(save=False, plot=False)
     assert os.path.exists(fs.ns.resume_file)
 
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=100,
         plot=False,
     )
 
     fs.run(save=False, plot=False)
 
 
 @pytest.mark.slow_integration_test
-def test_debug_log_level(model, tmpdir):
+def test_debug_log_level(integration_model, tmpdir):
     """Test running with debug log-level."""
     logger = logging.getLogger("nessai")
     original_level = logger.level
     logger.setLevel("DEBUG")
     output = str(tmpdir.mkdir("debug_logging"))
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=100,
         plot=False,
     )
     fs.run(plot=False)
     logger.setLevel(original_level)
 
 
 @pytest.mark.slow_integration_test
-def test_disable_vectorisation(model, tmp_path):
+def test_disable_vectorisation(tmp_path):
     """Assert vectorisation can be disabled"""
 
-    class TestModel(BaseModel):
+    class TestModel(IntegrationTestModel):
         def log_likelihood(self, x):
             # AssertionError won't be caught by nessai
             assert not (x.size > 1)
             return super().log_likelihood(x)
 
     output = tmp_path / "disable_vec"
     output.mkdir()
@@ -476,18 +533,18 @@
         disable_vectorisation=True,
         plot=False,
     )
     fs.run(plot=False)
 
 
 @pytest.mark.slow_integration_test
-def test_likelihood_chunksize(model, tmp_path):
+def test_likelihood_chunksize(tmp_path):
     """Assert likelihood chunksize limits number of samples in each call"""
 
-    class TestModel(BaseModel):
+    class TestModel(IntegrationTestModel):
         def log_likelihood(self, x):
             # AssertionError won't be caught by nessai
             assert not (x.size > self.likelihood_chunksize)
             return super().log_likelihood(x)
 
     output = tmp_path / "disable_vec"
     output.mkdir()
@@ -497,18 +554,18 @@
     fs = FlowSampler(
         model, output=output, nlive=100, plot=False, likelihood_chunksize=10
     )
     fs.run(plot=False, save=False)
 
 
 @pytest.mark.slow_integration_test
-def test_allow_multi_valued_likelihood(model, tmp_path):
+def test_allow_multi_valued_likelihood(tmp_path):
     """Assert a multi valued likelihood can be sampled from"""
 
-    class TestModel(BaseModel):
+    class TestModel(IntegrationTestModel):
         def log_likelihood(self, x):
             return super().log_likelihood(x) + 1e-10 * np.random.randn(x.size)
 
     output = tmp_path / "multi_value"
     output.mkdir()
 
     model = TestModel()
@@ -520,41 +577,41 @@
         plot=False,
         allow_multi_valued_likelihood=True,
     )
     fs.run(plot=False, save=False)
 
 
 @pytest.mark.integration_test
-def test_invalid_keyword_argument(model, tmp_path):
+def test_invalid_keyword_argument(integration_model, tmp_path):
     """Assert an error is raised if a keyword argument is unknown"""
 
     output = tmp_path / "kwargs_error"
     output.mkdir()
 
     with pytest.raises(
         RuntimeError,
         match="Unknown kwargs for FlowProposal: {'not_a_valid_kwarg'}.",
     ):
         FlowSampler(
-            model,
+            integration_model,
             output=output,
             nlive=100,
             plot=False,
             not_a_valid_kwarg=True,
         )
 
 
 @pytest.mark.parametrize("extension", ["hdf5", "h5", "json"])
 @pytest.mark.slow_integration_test
-def test_sampling_result_extension(model, tmp_path, extension):
+def test_sampling_result_extension(integration_model, tmp_path, extension):
     """Assert the correct extension is used"""
     output = tmp_path / "test"
     output.mkdir()
     fs = FlowSampler(
-        model,
+        integration_model,
         output=output,
         nlive=100,
         plot=False,
         proposal_plots=False,
         result_extension=extension,
     )
     fs.run(plot=False)
```

### Comparing `nessai-0.8.1/tests/test_utils/test_bilbyutils.py` & `nessai-0.9.0/tests/test_utils/test_bilbyutils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,71 @@
 # -*- coding: utf-8 -*-
 """
 Tests for bilbyutils
 """
 from unittest.mock import patch
+
+import pytest
 from nessai.flowsampler import FlowSampler
 from nessai.utils.bilbyutils import (
     get_all_kwargs,
     get_run_kwargs_list,
+    _get_importance_methods,
     _get_standard_methods,
 )
 
 
 def test_get_standard_methods():
     """Assert a list of methods is returned"""
     out = _get_standard_methods()
     assert len(out) == 5
 
 
-def test_get_all_kwargs():
+def test_get_importance_methods():
+    """Assert a list of methods is returned"""
+    out = _get_importance_methods()
+    assert len(out) == 4
+
+
+@pytest.mark.parametrize(
+    "ins, get_method",
+    [(False, "_get_standard_methods"), (True, "_get_importance_methods")],
+)
+def test_get_all_kwargs(ins, get_method):
     """Assert the correct dictionary is returned.
 
     Positional arguments should be ignored.
     """
 
     def func0(a, b, c=2, d=None):
         pass
 
     def func1(e, f, g=3, h=True):
         pass
 
     expected = dict(c=2, d=None, g=3, h=True)
 
     with patch(
-        "nessai.utils.bilbyutils._get_standard_methods",
+        f"nessai.utils.bilbyutils.{get_method}",
         return_value=[func0, func1],
     ):
-        out = get_all_kwargs()
+        out = get_all_kwargs(importance_nested_sampler=ins)
 
     assert out == expected
 
 
-def test_get_run_kwargs_list():
+@pytest.mark.parametrize(
+    "ins, run_method",
+    [(False, "run_standard_sampler"), (True, "run_importance_nested_sampler")],
+)
+def test_get_run_kwargs_list(ins, run_method):
     """Assert the correct list is returned"""
 
     def func(a, b=1, c=None):
         pass
 
     expected = ["b", "c"]
 
-    with patch.object(FlowSampler, "run", func):
-        out = get_run_kwargs_list()
+    with patch.object(FlowSampler, run_method, func):
+        out = get_run_kwargs_list(importance_nested_sampler=ins)
 
     assert out == expected
```

### Comparing `nessai-0.8.1/tests/test_utils/test_distance_utils.py` & `nessai-0.9.0/tests/test_utils/test_distance_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_distribution_utils.py` & `nessai-0.9.0/tests/test_utils/test_distribution_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_hist_utils.py` & `nessai-0.9.0/tests/test_utils/test_hist_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_indices_utils.py` & `nessai-0.9.0/tests/test_utils/test_indices_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_io_utils.py` & `nessai-0.9.0/tests/test_utils/test_io_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     m = mock_open()
     data = np.array([1, 2])
     with patch("builtins.open", m) as mo, patch("pickle.dump") as md, patch(
         "shutil.move"
     ) as msm:
         safe_file_dump(data, "test.pkl", pickle, save_existing=False)
     mo.assert_called_once_with("test.pkl.temp", "wb")
-    md.call_args_list[0][0] == data
+    np.testing.assert_array_equal(md.call_args_list[0][0][0], data)
     msm.assert_called_once_with("test.pkl.temp", "test.pkl")
 
 
 def test_safe_file_dump_save_existing():
     """Test safe file dump."""
     import pickle
 
@@ -132,15 +132,15 @@
     data = np.array([1, 2])
     with patch("os.path.exists", return_value=True) as mpe, patch(
         "builtins.open", m
     ) as mo, patch("pickle.dump") as md, patch("shutil.move") as msm:
         safe_file_dump(data, "test.pkl", pickle, save_existing=True)
     mpe.assert_called_once_with("test.pkl")
     mo.assert_called_once_with("test.pkl.temp", "wb")
-    md.call_args_list[0][0] == data
+    np.testing.assert_array_equal(md.call_args_list[0][0][0], data)
     msm.assert_has_calls(
         [
             call("test.pkl", "test.pkl.old"),
             call("test.pkl.temp", "test.pkl"),
         ]
     )
```

### Comparing `nessai-0.8.1/tests/test_utils/test_logging_utils.py` & `nessai-0.9.0/tests/test_utils/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_multiprocessing_utils.py` & `nessai-0.9.0/tests/test_utils/test_multiprocessing_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Tests for rescaling functions
 """
 import multiprocessing
 from multiprocessing.dummy import Pool
 import pytest
+import sys
 from unittest.mock import MagicMock, patch
 
 from nessai.utils.multiprocessing import (
     check_multiprocessing_start_method,
     initialise_pool_variables,
     get_n_pool,
     log_likelihood_wrapper,
@@ -26,48 +27,45 @@
     pool.terminate()
     assert out == [1, 2, 3]
 
     # Reset to the default value
     initialise_pool_variables(None)
 
 
-def test_check_multiprocessing_start_method():
-    """Test check multiprocessing start method passes for 'fork'"""
-    with patch("multiprocessing.get_start_method", return_value="fork"):
-        check_multiprocessing_start_method()
-
-
-@pytest.mark.parametrize("method", ["spawn", "forkserver"])
-def test_check_multiprocessing_start_method_error(method):
-    """Assert an error is raised if the start method is not fork."""
-    error_msg = r"nessai only supports multiprocessing using the 'fork' .*"
-    with patch(
-        "multiprocessing.get_start_method", return_value=method
-    ), pytest.raises(RuntimeError, match=error_msg):
+@pytest.mark.parametrize("method", ["fork", "forkserver", "spawn"])
+def test_check_multiprocessing_start_method(method, caplog):
+    """
+    Test check multiprocessing start method passes for all methods
+    """
+    with patch("multiprocessing.get_start_method", return_value=method):
         check_multiprocessing_start_method()
+    if method != "fork":
+        assert "This may lead to high memory usage or errors" in caplog.text
 
 
 @pytest.mark.integration_test
 @pytest.mark.skip_on_windows
 def test_check_multiprocessing_start_method_integration():
     """Integration test for checking the start method."""
     mp = multiprocessing.get_context("fork")
     with patch("multiprocessing.get_start_method", mp.get_start_method):
         check_multiprocessing_start_method()
 
 
+@pytest.mark.parametrize("method", ["fork", "forkserver", "spawn"])
 @pytest.mark.integration_test
-def test_check_multiprocessing_start_method_error_integration():
-    """Integration test for checking the start method raises an error."""
-    mp = multiprocessing.get_context("spawn")
-    error_msg = r"nessai only supports multiprocessing using the 'fork' .*"
-    with patch(
-        "multiprocessing.get_start_method", mp.get_start_method
-    ), pytest.raises(RuntimeError, match=error_msg):
+def test_check_multiprocessing_start_method_error_integration(method, caplog):
+    """Integration test for checking the start method prints a warning"""
+    if sys.platform == "win32" and method != "spawn":
+        pytest.skip("Windows only supports the 'spawn' start method")
+    mp = multiprocessing.get_context(method)
+    with patch("multiprocessing.get_start_method", mp.get_start_method):
         check_multiprocessing_start_method()
+    if method != "fork":
+        assert "This may lead to high memory usage or errors" in caplog.text
 
 
 def test_model_error():
     """Assert an error is raised in the global variables have not been \
         initialised
     """
     model = MagicMock()
```

### Comparing `nessai-0.8.1/tests/test_utils/test_rescaling_utils.py` & `nessai-0.9.0/tests/test_utils/test_rescaling_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_sampling_utils.py` & `nessai-0.9.0/tests/test_utils/test_sampling_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_sorting_utils.py` & `nessai-0.9.0/tests/test_utils/test_sorting_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_structures_utils.py` & `nessai-0.9.0/tests/test_utils/test_structures_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Tests for utilities related to python structures such as lists.
 """
 import numpy as np
 import pytest
 
 from nessai.utils.structures import (
     array_split_chunksize,
+    get_inverse_indices,
     get_subset_arrays,
     isfinite_struct,
     replace_in_list,
 )
 
 
 def test_replace_in_list():
@@ -131,7 +132,35 @@
     np.testing.assert_array_equal(out[0], a)
 
 
 def test_array_split_chunksize_invalid_chunksize():
     """Assert an error is returned if the chunksize is less than one"""
     with pytest.raises(ValueError, match="chunksize must be greater than 1"):
         array_split_chunksize(np.array([1, 2]), -1)
+
+
+def test_get_inverse_indices():
+    """Assert the correct indices are returned"""
+    indices = np.array([1, 2, 3])
+    n = 5
+    expected = np.array([0, 4])
+    out = get_inverse_indices(n, indices)
+    np.testing.assert_array_equal(out, expected)
+
+
+def test_get_inverse_indices_empty_inverse():
+    """Assert an empty array is returned in the indices are complete"""
+    indices = np.array([0, 1, 2, 3, 4])
+    n = 5
+    expected = np.array([])
+    out = get_inverse_indices(n, indices)
+    np.testing.assert_array_equal(out, expected)
+
+
+def test_get_inverse_indices_invalid_n():
+    """Assert"""
+    indices = np.array([0, 1, 4])
+    n = 4
+    with pytest.raises(
+        ValueError, match=r"Indices contain values that are out of range for n"
+    ):
+        get_inverse_indices(n, indices)
```

### Comparing `nessai-0.8.1/tests/test_utils/test_testing_utils.py` & `nessai-0.9.0/tests/test_utils/test_testing_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 """
 Test the testing utilities
 """
 import numpy as np
 import pytest
 
-from nessai.utils.testing import assert_structured_arrays_equal
+from nessai.utils.testing import (
+    IntegrationTestModel,
+    assert_structured_arrays_equal,
+)
+
+
+@pytest.mark.parametrize("n", [1, 10])
+@pytest.mark.parametrize("dims", [2, 4])
+def test_integration_test_model(n, dims):
+    """Assert the model is valid"""
+    model = IntegrationTestModel(dims)
+    model.verify_model()
+    x = model.new_point(n)
+    log_p = model.log_prior(x)
+    log_l = model.log_likelihood(x)
+    assert np.isfinite(log_p).all()
+    assert np.isfinite(log_l).all()
+    assert len(log_p) == len(x)
+    assert len(log_l) == len(x)
 
 
 def test_assert_struct_arrays_different_fields():
     """Assert an errors is raised if the arrays have different fields"""
     x = np.array((1, 2), dtype=[("x", "f8"), ("y", "f8")])
     y = np.array((1, 2), dtype=[("x", "f8"), ("y", "f4")])
     with pytest.raises(AssertionError):
```

### Comparing `nessai-0.8.1/tests/test_utils/test_threading_utils.py` & `nessai-0.9.0/tests/test_utils/test_threading_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_utils/test_torchtutils_utils.py` & `nessai-0.9.0/tests/test_utils/test_torchtutils_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.1/tests/test_version.py` & `nessai-0.9.0/tests/test_version.py`

 * *Files identical despite different names*

