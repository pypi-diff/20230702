# Comparing `tmp/mqt.bench-0.4.4.tar.gz` & `tmp/mqt.bench-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.bench-0.4.4.tar", last modified: Tue May 16 10:22:33 2023, max compression
+gzip compressed data, was "mqt.bench-1.0.0.tar", last modified: Sun Jul  2 15:00:45 2023, max compression
```

## Comparing `mqt.bench-0.4.4.tar` & `mqt.bench-1.0.0.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.347708 mqt.bench-0.4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/img/
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/arch.png
--rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_4.png
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/mqt_light.png
--rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/mqtbench.png
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.347708 mqt.bench-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.347708 mqt.bench-0.4.4/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/src/mqt/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmark_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/dj.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/graphstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/hhl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qft.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qftentangled.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_ml/qgan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_nature/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeinexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qwalk.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/realamprandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/shor.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/su2random.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/twolocalrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/wstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation_visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/pie.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/qubit_dist.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/violins.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/qiskit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/tket_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/MQTBench_all.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/qasm_output/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/qasm_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/tum_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/benchmark_description.html
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/description.html
--rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/legal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/src/mqt.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26017 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/tests/test_benchviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.353476 mqt.bench-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.353476 mqt.bench-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.357476 mqt.bench-1.0.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/arch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/mqtbench.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.349476 mqt.bench-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.349476 mqt.bench-1.0.0/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.361476 mqt.bench-1.0.0/src/mqt/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmark_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/graphstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qftentangled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_nature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeinexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qwalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/realamprandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/shor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/su2random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/twolocalrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/wstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.385477 mqt.bench-1.0.0/src/mqt/bench/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123) 15925096 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.385477 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/pie.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/qubit_dist.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/violins.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/qiskit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/tket_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/MQTBench_all.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/qasm_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/qasm_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/tum_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/benchmark_description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28232 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/legal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.357476 mqt.bench-1.0.0/src/mqt.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27066 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/tests/test_benchviewer.py
```

### Comparing `mqt.bench-0.4.4/.github/dependabot.yml` & `mqt.bench-1.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/.github/release-drafter.yml` & `mqt.bench-1.0.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/.github/workflows/codeql.yml` & `mqt.bench-1.0.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/.github/workflows/coverage.yml` & `mqt.bench-1.0.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/.github/workflows/deploy.yml` & `mqt.bench-1.0.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/.gitignore` & `mqt.bench-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/.pre-commit-config.yaml` & `mqt.bench-1.0.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -39,42 +39,42 @@
   - repo: https://github.com/psf/black
     rev: "23.3.0" # Keep in sync with blacken-docs
     hooks:
       - id: black-jupyter
 
   # Also run Black on examples in the documentation
   - repo: https://github.com/asottile/blacken-docs
-    rev: "1.13.0"
+    rev: "1.14.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==23.3.0 # keep in sync with black hook
 
   # Clean jupyter notebooks
   - repo: https://github.com/srstevenson/nb-clean
     rev: "2.4.0"
     hooks:
       - id: nb-clean
   # Check for spelling
   - repo: https://github.com/codespell-project/codespell
-    rev: "v2.2.4"
+    rev: "v2.2.5"
     hooks:
       - id: codespell
         args: ["-L", "wille,linz"]
         exclude: "mqt/benchviewer/templates/legal.html"
 
   # Format configuration files with prettier
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+    rev: v0.0.272
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
```

### Comparing `mqt.bench-0.4.4/LICENSE` & `mqt.bench-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/PKG-INFO` & `mqt.bench-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 0.4.4
+Version: 1.0.0
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)](https://pypi.org/project/mqt.bench/)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/coverage.yml?branch=main&style=flat-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/actions/workflows/coverage.yml)
 [![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/workflows/deploy.yml)
-[![codecov](https://img.shields.io/codecov/c/github/cda-tum/MQTBench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/MQTBench)
+[![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-bench)
 
 <p align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqtbench/main/img/mqt_light.png" width="60%">
   <img src="https://raw.githubusercontent.com/cda-tum/mqtbench/main/img/mqt_dark.png" width="60%">
 </picture>
 </p>
@@ -137,26 +137,26 @@
 - Amplitude Estimation
 - Deutsch-Jozsa
 - GHZ State
 - Graph State
 - Ground State
 - Grover's (no ancilla)
 - Grover's (v-chain)
-- HHL
 - Portfolio Optimization with QAOA
 - Portfolio Optimization with VQE
 - Pricing Call Option
 - Pricing Put Option
 - Quantum Fourier Transformation (QFT)
 - QFT Entangled
-- Quantum Generative Adversarial Network (QGAN)
+- Quantum Neural Network (QNN)
 - Quantum Phase Estimation (QPE) Exact
 - Quantum Phase Estimation (QPE) Inexact
 - Quantum Walk (no ancilla)
 - Quantum Walk (-chain)
+- Random Circuit
 - Routing
 - Shor's
 - Travelling Salesman
 - Variational Quantum Eigensolver (VQE)
 - VQE-ansätze with random values:
   - Efficient SU2 ansatz with Random Parameters
   - Real Amplitudes ansatz with Random Parameters
@@ -176,24 +176,27 @@
 
 So far, MQT Bench supports the following native gate-sets:
 
 1. IBMQ gate-set: _\['rz', 'sx', 'x', 'cx', 'measure'\]_
 2. Rigetti gate-set: _\['rx', 'rz', 'cz', 'measure'\]_
 3. IonQ gate-set: _\['rxx', 'rz', 'ry', 'rx', 'measure'\]_
 4. OQC gate-set: _\['rz', 'sx', 'x', 'ecr', 'measure'\]_
+5. Quantinuum gate-set: _\['rzz', 'rz', 'ry', 'rx', 'measure'\]_
 
 ## Device Support
 
 So far, MQT Bench supports the following devices:
 
 1. IBMQ Washington with 127 qubits
 2. IBMQ Montreal with 27 qubits
 3. Rigetti Aspen-M2 with 80 qubits
-4. IonQ with 11 qubits
-5. OQC Lucy with 8 qubits
+4. IonQ Harmony with 11 qubits
+5. IonQ Aria 1 with 25 qubits
+6. OQC Lucy with 8 qubits
+7. Quantinuum H2 with 32 qubits
 
 # Repository Structure
 
 - src/mqt/: main source directory
   - bench: Directory for the MQT Bench package
   - bench/benchmarks: Directory for the benchmarks
   - benchviewer: Directory for the webpage (which can be started locally and is also hosted at
@@ -232,17 +235,17 @@
     device_name: str = "ibm_washington",
 ):
 ```
 
 The available parameters are:
 
 - `benchmark_name`: `"ae"`, `"dj"`, `"grover-noancilla"`, `"grover-v-chain"`, `"ghz"`, `"graphstate"`, `"portfolioqaoa"`,
-  `"portfoliovqe"`, `"qaoa"`, `"qft"`, `"qftentangled"`, `"qgan"`, `"qpeexact"`, `"qpeinexact"`,
-  `"qwalk-noancilla"`, `"qwalk-v-chain"`, `"realamprandom"`, `"su2random"`, `"twolocalrandom"`, `"vqe"`,
-  `"wstate"`, `"shor"`, `"hhl"`, `"pricingcall"`, `"pricingput"`, `"groundstate"`, `"routing"`,
+  `"portfoliovqe"`, `"qaoa"`, `"qft"`, `"qftentangled"`, `"qnn"`, `"qpeexact"`, `"qpeinexact"`,
+  `"qwalk-noancilla"`, `"qwalk-v-chain"`, `"random"`, `"realamprandom"`, `"su2random"`, `"twolocalrandom"`, `"vqe"`,
+  `"wstate"`, `"shor"`, `"pricingcall"`, `"pricingput"`, `"groundstate"`, `"routing"`,
   `"tsp"`
 - `level`: `0` or `"alg"`, `1` or `"indep"`, `2` or `"nativegates"`, `3` or `"mapped"`
 - `circuit_size`: for most of the cases this is equal to number of qubits
   (all scalable benchmarks except `"qwalk-v-chain"` and `"grover-v-chain"`) while for all other the qubit number is higher
 - `compiler`: `"qiskit"` or `"tket"`
 - `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
 
@@ -251,16 +254,16 @@
 
 compiler_settings = CompilerSettings(
     qiskit={"optimization_level": 1},
     tket={"placement": "lineplacement"},
 )
 ```
 
-- `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, or `"oqc"`
-- `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"aspen_m1"`, `"ionq11"`, `"lucy"`
+- `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, `"oqc"`, or `"quantinuum"`
+- `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"rigetti_aspen_m2"`, `"ionq_harmony"`, `"ionq_aria1"`, `"oqc_lucy"`, or `"quantinuum_h2"`
 
 Hereby, the mappings between shortened `benchmark_name` and actual benchmarks are:
 
 | `benchmark_name`     | Actual Benchmark                                    |
 | -------------------- | --------------------------------------------------- |
 | `"ae"`               | Amplitude Estimation (AE)                           |
 | `"dj"`               | Deutsch-Jozsa                                       |
@@ -269,26 +272,26 @@
 | `"ghz"`              | GHZ State                                           |
 | `"graphstate"`       | Graph State                                         |
 | `"portfolioqaoa"`    | Portfolio Optimization with QAOA                    |
 | `"portfoliovqe"`     | Portfolio Optimization with VQE                     |
 | `"qaoa"`             | Quantum Approximation Optimization Algorithm (QAOA) |
 | `"qft"`              | Quantum Fourier Transformation (QFT)                |
 | `"qftentangled"`     | QFT Entangled                                       |
-| `"qgan"`             | Quantum Generative Adversarial Network              |
+| `"qnn"`              | Quantum Neural Network (QNN)                        |
 | `"qpeexact"`         | Quantum Phase Estimation (QPE) exact                |
 | `"qpeinexact"`       | Quantum Phase Estimation (QPE) inexact              |
 | `"qwalk-noancilla"`  | Quantum Walk (no ancilla)                           |
 | `"qwalk-v-chain"`    | Quantum Walk (v-chain)                              |
+| `"random"`           | Random Quantum Circuit                              |
 | `"realamprandom"`    | Real Amplitudes ansatz with Random Parameters       |
 | `"su2random"`        | Efficient SU2 ansatz with Random Parameters         |
 | `"twolocalrandom"`   | Two Local ansatz with Random Parameters             |
 | `"vqe"`              | Variational Quantum Eigensolver (VQE)               |
 | `"wstate"`           | W-State                                             |
 | `"shor"`             | Shor's                                              |
-| `"hhl"`              | HHL                                                 |
 | `"pricingcall"`      | Pricing Call Option                                 |
 | `"pricingput"`       | Pricing Put Option                                  |
 | `"groundstate"`      | Ground State                                        |
 | `"routing"`          | Routing                                             |
 | `"tsp"`              | Travelling Salesman                                 |
 
 For example, in order to obtain the _5_-qubit Deutsch-Josza benchmark on algorithm level, use the following:
```

### Comparing `mqt.bench-0.4.4/README.md` & `mqt.bench-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)](https://pypi.org/project/mqt.bench/)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/coverage.yml?branch=main&style=flat-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/actions/workflows/coverage.yml)
 [![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/workflows/deploy.yml)
-[![codecov](https://img.shields.io/codecov/c/github/cda-tum/MQTBench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/MQTBench)
+[![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-bench)
 
 <p align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqtbench/main/img/mqt_light.png" width="60%">
   <img src="https://raw.githubusercontent.com/cda-tum/mqtbench/main/img/mqt_dark.png" width="60%">
 </picture>
 </p>
@@ -85,26 +85,26 @@
 - Amplitude Estimation
 - Deutsch-Jozsa
 - GHZ State
 - Graph State
 - Ground State
 - Grover's (no ancilla)
 - Grover's (v-chain)
-- HHL
 - Portfolio Optimization with QAOA
 - Portfolio Optimization with VQE
 - Pricing Call Option
 - Pricing Put Option
 - Quantum Fourier Transformation (QFT)
 - QFT Entangled
-- Quantum Generative Adversarial Network (QGAN)
+- Quantum Neural Network (QNN)
 - Quantum Phase Estimation (QPE) Exact
 - Quantum Phase Estimation (QPE) Inexact
 - Quantum Walk (no ancilla)
 - Quantum Walk (-chain)
+- Random Circuit
 - Routing
 - Shor's
 - Travelling Salesman
 - Variational Quantum Eigensolver (VQE)
 - VQE-ansätze with random values:
   - Efficient SU2 ansatz with Random Parameters
   - Real Amplitudes ansatz with Random Parameters
@@ -124,24 +124,27 @@
 
 So far, MQT Bench supports the following native gate-sets:
 
 1. IBMQ gate-set: _\['rz', 'sx', 'x', 'cx', 'measure'\]_
 2. Rigetti gate-set: _\['rx', 'rz', 'cz', 'measure'\]_
 3. IonQ gate-set: _\['rxx', 'rz', 'ry', 'rx', 'measure'\]_
 4. OQC gate-set: _\['rz', 'sx', 'x', 'ecr', 'measure'\]_
+5. Quantinuum gate-set: _\['rzz', 'rz', 'ry', 'rx', 'measure'\]_
 
 ## Device Support
 
 So far, MQT Bench supports the following devices:
 
 1. IBMQ Washington with 127 qubits
 2. IBMQ Montreal with 27 qubits
 3. Rigetti Aspen-M2 with 80 qubits
-4. IonQ with 11 qubits
-5. OQC Lucy with 8 qubits
+4. IonQ Harmony with 11 qubits
+5. IonQ Aria 1 with 25 qubits
+6. OQC Lucy with 8 qubits
+7. Quantinuum H2 with 32 qubits
 
 # Repository Structure
 
 - src/mqt/: main source directory
   - bench: Directory for the MQT Bench package
   - bench/benchmarks: Directory for the benchmarks
   - benchviewer: Directory for the webpage (which can be started locally and is also hosted at
@@ -180,17 +183,17 @@
     device_name: str = "ibm_washington",
 ):
 ```
 
 The available parameters are:
 
 - `benchmark_name`: `"ae"`, `"dj"`, `"grover-noancilla"`, `"grover-v-chain"`, `"ghz"`, `"graphstate"`, `"portfolioqaoa"`,
-  `"portfoliovqe"`, `"qaoa"`, `"qft"`, `"qftentangled"`, `"qgan"`, `"qpeexact"`, `"qpeinexact"`,
-  `"qwalk-noancilla"`, `"qwalk-v-chain"`, `"realamprandom"`, `"su2random"`, `"twolocalrandom"`, `"vqe"`,
-  `"wstate"`, `"shor"`, `"hhl"`, `"pricingcall"`, `"pricingput"`, `"groundstate"`, `"routing"`,
+  `"portfoliovqe"`, `"qaoa"`, `"qft"`, `"qftentangled"`, `"qnn"`, `"qpeexact"`, `"qpeinexact"`,
+  `"qwalk-noancilla"`, `"qwalk-v-chain"`, `"random"`, `"realamprandom"`, `"su2random"`, `"twolocalrandom"`, `"vqe"`,
+  `"wstate"`, `"shor"`, `"pricingcall"`, `"pricingput"`, `"groundstate"`, `"routing"`,
   `"tsp"`
 - `level`: `0` or `"alg"`, `1` or `"indep"`, `2` or `"nativegates"`, `3` or `"mapped"`
 - `circuit_size`: for most of the cases this is equal to number of qubits
   (all scalable benchmarks except `"qwalk-v-chain"` and `"grover-v-chain"`) while for all other the qubit number is higher
 - `compiler`: `"qiskit"` or `"tket"`
 - `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
 
@@ -199,16 +202,16 @@
 
 compiler_settings = CompilerSettings(
     qiskit={"optimization_level": 1},
     tket={"placement": "lineplacement"},
 )
 ```
 
-- `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, or `"oqc"`
-- `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"aspen_m1"`, `"ionq11"`, `"lucy"`
+- `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, `"oqc"`, or `"quantinuum"`
+- `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"rigetti_aspen_m2"`, `"ionq_harmony"`, `"ionq_aria1"`, `"oqc_lucy"`, or `"quantinuum_h2"`
 
 Hereby, the mappings between shortened `benchmark_name` and actual benchmarks are:
 
 | `benchmark_name`     | Actual Benchmark                                    |
 | -------------------- | --------------------------------------------------- |
 | `"ae"`               | Amplitude Estimation (AE)                           |
 | `"dj"`               | Deutsch-Jozsa                                       |
@@ -217,26 +220,26 @@
 | `"ghz"`              | GHZ State                                           |
 | `"graphstate"`       | Graph State                                         |
 | `"portfolioqaoa"`    | Portfolio Optimization with QAOA                    |
 | `"portfoliovqe"`     | Portfolio Optimization with VQE                     |
 | `"qaoa"`             | Quantum Approximation Optimization Algorithm (QAOA) |
 | `"qft"`              | Quantum Fourier Transformation (QFT)                |
 | `"qftentangled"`     | QFT Entangled                                       |
-| `"qgan"`             | Quantum Generative Adversarial Network              |
+| `"qnn"`              | Quantum Neural Network (QNN)                        |
 | `"qpeexact"`         | Quantum Phase Estimation (QPE) exact                |
 | `"qpeinexact"`       | Quantum Phase Estimation (QPE) inexact              |
 | `"qwalk-noancilla"`  | Quantum Walk (no ancilla)                           |
 | `"qwalk-v-chain"`    | Quantum Walk (v-chain)                              |
+| `"random"`           | Random Quantum Circuit                              |
 | `"realamprandom"`    | Real Amplitudes ansatz with Random Parameters       |
 | `"su2random"`        | Efficient SU2 ansatz with Random Parameters         |
 | `"twolocalrandom"`   | Two Local ansatz with Random Parameters             |
 | `"vqe"`              | Variational Quantum Eigensolver (VQE)               |
 | `"wstate"`           | W-State                                             |
 | `"shor"`             | Shor's                                              |
-| `"hhl"`              | HHL                                                 |
 | `"pricingcall"`      | Pricing Call Option                                 |
 | `"pricingput"`       | Pricing Put Option                                  |
 | `"groundstate"`      | Ground State                                        |
 | `"routing"`          | Routing                                             |
 | `"tsp"`              | Travelling Salesman                                 |
 
 For example, in order to obtain the _5_-qubit Deutsch-Josza benchmark on algorithm level, use the following:
```

### Comparing `mqt.bench-0.4.4/config.json` & `mqt.bench-1.0.0/config.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7111193783068783%*

 * *Differences: {"'benchmarks'": "{0: {'max_qubits': 131}, 1: {'max_qubits': 131}, 2: {'max_qubits': 131}, 3: "*

 * *                 "{'max_qubits': 131}, 4: {'instances': {insert: [(2, 'large')]}}, 5: "*

 * *                 "{'max_qubits': 131}, 6: {'max_qubits': 131}, 7: {'max_qubits': 131}, 8: "*

 * *                 "{'max_uncertainty': 131}, 9: {'max_uncertainty': 131}, 10: {'max_qubits': 131}, "*

 * *                 "11: {'max_qubits': 131}, 12: {'max_qubits': 131}, 13: {'name': 'qnn', "*

 * *                 "'max_qubits': 131, 'precheck […]*

```diff
@@ -1,219 +1,222 @@
 {
     "benchmarks": [
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "ae",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "dj",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "ghz",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 3,
             "name": "graphstate",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
             "instances": [
                 "small",
-                "medium"
+                "medium",
+                "large"
             ],
             "name": "groundstate",
             "precheck_possible": false
         },
         {
             "ancillary_mode": [
                 "noancilla",
                 "v-chain"
             ],
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "grover",
             "precheck_possible": false,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_index": 10,
-            "min_index": 1,
-            "name": "hhl",
-            "precheck_possible": false
-        },
-        {
-            "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 3,
             "name": "portfolioqaoa",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 3,
             "name": "portfoliovqe",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_uncertainty": 130,
+            "max_uncertainty": 131,
             "min_uncertainty": 2,
             "name": "pricingcall",
             "precheck_possible": false
         },
         {
             "include": true,
-            "max_uncertainty": 130,
+            "max_uncertainty": 131,
             "min_uncertainty": 2,
             "name": "pricingput",
             "precheck_possible": false
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 3,
             "name": "qaoa",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "qft",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "qftentangled",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
-            "name": "qgan",
-            "precheck_possible": false,
+            "name": "qnn",
+            "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "qpeexact",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "qpeinexact",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "ancillary_mode": [
                 "noancilla",
                 "v-chain"
             ],
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 3,
             "name": "qwalk",
             "precheck_possible": false,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
+            "min_qubits": 2,
+            "name": "random",
+            "precheck_possible": true,
+            "stepsize": 1
+        },
+        {
+            "include": true,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "realamprandom",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_nodes": 130,
+            "max_nodes": 131,
             "min_nodes": 2,
             "name": "routing",
             "precheck_possible": false
         },
         {
             "include": true,
             "instances": [
                 "xsmall",
                 "small",
-                "medium"
+                "medium",
+                "large"
             ],
             "name": "shor",
             "precheck_possible": false
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "su2random",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_nodes": 10,
+            "max_nodes": 131,
             "min_nodes": 2,
             "name": "tsp",
             "precheck_possible": false
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "twolocalrandom",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 3,
             "name": "vqe",
             "precheck_possible": true,
             "stepsize": 1
         },
         {
             "include": true,
-            "max_qubits": 130,
+            "max_qubits": 131,
             "min_qubits": 2,
             "name": "wstate",
             "precheck_possible": true,
             "stepsize": 1
         }
     ],
-    "timeout": 120
+    "timeout": 65
 }
```

### Comparing `mqt.bench-0.4.4/img/arch.png` & `mqt.bench-1.0.0/img/arch.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/level_1.png` & `mqt.bench-1.0.0/img/level_1.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/level_2.png` & `mqt.bench-1.0.0/img/level_2.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/level_3.png` & `mqt.bench-1.0.0/img/level_3.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/level_4.png` & `mqt.bench-1.0.0/img/level_4.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/mqt_dark.png` & `mqt.bench-1.0.0/img/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/mqt_light.png` & `mqt.bench-1.0.0/img/mqt_light.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/img/mqtbench.png` & `mqt.bench-1.0.0/img/mqtbench.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/pyproject.toml` & `mqt.bench-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 ]
 keywords = ["MQT",  "quantum computing", "benchmarking", "performance", "testing"]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["version"]
 
 dependencies = [
-    "pytket-qiskit>=0.34.0,<0.40.0",  #  manages the dependencies for qiskit and tket in a combined fashion
+    "pytket-qiskit>=0.40.0,<0.41.0",  #  manages the dependencies for qiskit and tket in a combined fashion
     "qiskit[all]",  # this is merely to get the [all] dependencies. The versioning is covered by pytket-qiskit
     "pandas>=1.0.0",
     "flask>=2.0.0",
     "networkx>=2.0.0",
+    "scipy<1.11.0",
     "pyscf>=2.1.0",
     "packaging>=21.0",
     "tqdm>=4.0.0",
     "importlib_metadata>=3.6; python_version < '3.10'",
     "importlib_resources>=5.9; python_version < '3.10'",
 ]
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmark_generator.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmark_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import TYPE_CHECKING, Any, Callable, TypedDict
 
 from joblib import Parallel, delayed
 from mqt.bench import qiskit_helper, tket_helper, utils
 from qiskit import QuantumCircuit
 
 if TYPE_CHECKING:  # pragma: no cover
+    from types import ModuleType
+
     from pytket.circuit import Circuit
 
 if TYPE_CHECKING or sys.version_info >= (3, 10, 0):  # pragma: no cover
     from importlib import resources
 else:
     import importlib_resources as resources
 
@@ -64,209 +66,191 @@
         if qasm_output_path is None:
             self.qasm_output_path = str(resources.files("mqt.benchviewer") / "static" / "files" / "qasm_output")
         else:
             self.qasm_output_path = qasm_output_path
 
         Path(self.qasm_output_path).mkdir(exist_ok=True, parents=True)
 
-    def create_benchmarks_from_config(self, num_jobs: int = -1) -> bool:
+    def create_benchmarks_from_config(self, num_jobs: int) -> bool:
         benchmarks = [Benchmark(benchmark) for benchmark in self.cfg["benchmarks"]]  # type: ignore[misc]
-        Parallel(n_jobs=num_jobs, verbose=100)(delayed(self.generate_benchmark)(benchmark) for benchmark in benchmarks)
+        Parallel(n_jobs=num_jobs, verbose=100)(
+            delayed(self.define_benchmark_instances)(benchmark) for benchmark in benchmarks
+        )
         return True
 
-    def generate_benchmark(self, benchmark: Benchmark) -> None:  # noqa: PLR0912
+    def define_benchmark_instances(self, benchmark: Benchmark) -> None:
         lib = utils.get_module_for_benchmark(benchmark["name"])
         file_precheck = benchmark["precheck_possible"]
+        instances: list[tuple[int, str]] | list[int] | list[str] | range
         if benchmark["include"]:
             if benchmark["name"] == "grover" or benchmark["name"] == "qwalk":
-                for anc_mode in benchmark["ancillary_mode"]:
-                    for n in range(
-                        benchmark["min_qubits"],
-                        benchmark["max_qubits"],
-                        benchmark["stepsize"],
-                    ):
-                        success_flag = self.start_benchmark_generation(lib.create_circuit, [n, anc_mode], file_precheck)
-                        if not success_flag:
-                            break
+                instances_without_anc_mode = range(
+                    benchmark["min_qubits"],
+                    benchmark["max_qubits"],
+                    benchmark["stepsize"],
+                )
+                instances = [
+                    (instance, anc_mode)
+                    for instance in instances_without_anc_mode
+                    for anc_mode in benchmark["ancillary_mode"]
+                ]
 
             elif benchmark["name"] == "shor":
-                for choice in benchmark["instances"]:
-                    to_be_factored_number, a_value = lib.get_instance(choice)
-                    success_flag = self.start_benchmark_generation(
-                        lib.create_circuit, [to_be_factored_number, a_value], file_precheck
-                    )
-                    if not success_flag:
-                        break
-
-            elif benchmark["name"] == "hhl":
-                for i in range(benchmark["min_index"], benchmark["max_index"]):
-                    success_flag = self.start_benchmark_generation(lib.create_circuit, [i], file_precheck)
-                    if not success_flag:
-                        break
+                instances = [lib.get_instance(choice) for choice in benchmark["instances"]]
 
-            elif benchmark["name"] == "routing":
-                for nodes in range(benchmark["min_nodes"], benchmark["max_nodes"]):
-                    success_flag = self.start_benchmark_generation(lib.create_circuit, [nodes, 2], file_precheck)
-                    if not success_flag:
-                        break
-
-            elif benchmark["name"] == "tsp":
-                for nodes in range(benchmark["min_nodes"], benchmark["max_nodes"]):
-                    success_flag = self.start_benchmark_generation(lib.create_circuit, [nodes], file_precheck)
-                    if not success_flag:
-                        break
+            elif benchmark["name"] == "routing" or benchmark["name"] == "tsp":
+                instances = range(benchmark["min_nodes"], benchmark["max_nodes"])
 
             elif benchmark["name"] == "groundstate":
-                for choice in benchmark["instances"]:
-                    success_flag = self.start_benchmark_generation(lib.create_circuit, [choice], file_precheck)
-                    if not success_flag:
-                        break
+                instances = benchmark["instances"]
 
             elif benchmark["name"] == "pricingcall" or benchmark["name"] == "pricingput":
-                for nodes in range(benchmark["min_uncertainty"], benchmark["max_uncertainty"]):
-                    success_flag = self.start_benchmark_generation(lib.create_circuit, [nodes], file_precheck)
-                    if not success_flag:
-                        break
-            else:
-                for n in range(
-                    benchmark["min_qubits"],
-                    benchmark["max_qubits"],
-                    benchmark["stepsize"],
-                ):
-                    success_flag = self.start_benchmark_generation(lib.create_circuit, [n], file_precheck)
-                    if not success_flag:
-                        break
-
-    def generate_circuits_on_all_levels(self, qc: QuantumCircuit, num_qubits: int, file_precheck: bool) -> bool:
-        success_generated_circuits_t_indep = self.generate_target_indep_level_circuit(qc, num_qubits, file_precheck)
+                instances = range(benchmark["min_uncertainty"], benchmark["max_uncertainty"])
 
-        if not success_generated_circuits_t_indep:
-            return False
+            else:
+                instances = range(benchmark["min_qubits"], benchmark["max_qubits"], benchmark["stepsize"])
 
-        self.generate_target_dep_level_circuit(qc, num_qubits, file_precheck)
-        return True
+            self.generate_all_benchmarks(lib, instances, file_precheck)
 
-    def generate_target_indep_level_circuit(self, qc: QuantumCircuit, num_qubits: int, file_precheck: bool) -> bool:
-        num_generated_circuits = 0
-        res_indep_qiskit = timeout_watcher(
-            qiskit_helper.get_indep_level,
-            self.timeout,
-            [qc, num_qubits, file_precheck, False, self.qasm_output_path],
-        )
-        if res_indep_qiskit:
-            num_generated_circuits += 1
+    def generate_all_benchmarks(
+        self,
+        lib: ModuleType,
+        parameter_space: list[tuple[int, str]] | list[int] | list[str] | range,
+        file_precheck: bool,
+    ) -> None:
+        self.generate_indep_levels(file_precheck, lib, parameter_space)
+        self.generate_native_gates_levels(file_precheck, lib, parameter_space)
+        self.generate_mapped_levels(file_precheck, lib, parameter_space)
+
+    def generate_mapped_levels(  # noqa: PLR0912
+        self,
+        file_precheck: bool,
+        lib: ModuleType,
+        parameter_space: list[tuple[int, str]] | list[int] | list[str] | range,
+    ) -> None:
+        for gate_set_name, devices in utils.get_compilation_paths():
+            for device_name, max_qubits in devices:
+                for opt_level in range(4):
+                    for parameter_instance in parameter_space:
+                        qc = timeout_watcher(lib.create_circuit, self.timeout, parameter_instance)
+                        if not qc:
+                            break
+                        assert isinstance(qc, QuantumCircuit)
+                        if qc.num_qubits <= max_qubits:
+                            res = timeout_watcher(
+                                qiskit_helper.get_mapped_level,
+                                self.timeout,
+                                [
+                                    qc,
+                                    gate_set_name,
+                                    qc.num_qubits,
+                                    device_name,
+                                    opt_level,
+                                    file_precheck,
+                                    False,
+                                    self.qasm_output_path,
+                                ],
+                            )
+                            if not res:
+                                break
+                        else:
+                            break
 
-        res_indep_tket = timeout_watcher(
-            tket_helper.get_indep_level,
-            self.timeout,
-            [qc, num_qubits, file_precheck, False, self.qasm_output_path],
-        )
-        if res_indep_tket:
-            num_generated_circuits += 1
+                for lineplacement in (False, True):
+                    for parameter_instance in parameter_space:
+                        qc = timeout_watcher(lib.create_circuit, self.timeout, parameter_instance)
+                        if not qc:
+                            break
+                        assert isinstance(qc, QuantumCircuit)
+                        if qc.num_qubits <= max_qubits:
+                            res = timeout_watcher(
+                                tket_helper.get_mapped_level,
+                                self.timeout,
+                                [
+                                    qc,
+                                    gate_set_name,
+                                    qc.num_qubits,
+                                    device_name,
+                                    lineplacement,
+                                    file_precheck,
+                                    False,
+                                    self.qasm_output_path,
+                                ],
+                            )
+                            if not res:
+                                break
+                        else:
+                            break
 
-        return num_generated_circuits != 0
+    def generate_native_gates_levels(
+        self,
+        file_precheck: bool,
+        lib: ModuleType,
+        parameter_space: list[tuple[int, str]] | list[int] | list[str] | range,
+    ) -> None:
+        for gate_set in utils.get_supported_gatesets():
+            for opt_level in [0, 1, 2, 3]:
+                for parameter_instance in parameter_space:
+                    qc = timeout_watcher(lib.create_circuit, self.timeout, parameter_instance)
+                    if not qc:
+                        break
+                    assert isinstance(qc, QuantumCircuit)
+                    res = timeout_watcher(
+                        qiskit_helper.get_native_gates_level,
+                        self.timeout,
+                        [
+                            qc,
+                            gate_set,
+                            qc.num_qubits,
+                            opt_level,
+                            file_precheck,
+                            False,
+                            self.qasm_output_path,
+                        ],
+                    )
+                    if not res:
+                        break
 
-    def generate_target_dep_level_circuit(self, qc: QuantumCircuit, num_qubits: int, file_precheck: bool) -> bool:
-        compilation_paths: list[tuple[str, list[tuple[str, int]]]] = [
-            ("ibm", [("ibm_washington", 127), ("ibm_montreal", 27)]),
-            ("rigetti", [("rigetti_aspen_m2", 80)]),
-            ("ionq", [("ionq11", 11)]),
-            ("oqc", [("oqc_lucy", 8)]),
-        ]
-        num_generated_benchmarks = 0
-        for gate_set_name, devices in compilation_paths:
-            # Creating the circuit on both target-dependent levels for qiskit
-            for opt_level in range(4):
+            for parameter_instance in parameter_space:
+                qc = timeout_watcher(lib.create_circuit, self.timeout, parameter_instance)
+                if not qc:
+                    break
+                assert isinstance(qc, QuantumCircuit)
                 res = timeout_watcher(
-                    qiskit_helper.get_native_gates_level,
+                    tket_helper.get_native_gates_level,
                     self.timeout,
                     [
                         qc,
-                        gate_set_name,
-                        num_qubits,
-                        opt_level,
+                        gate_set,
+                        qc.num_qubits,
                         file_precheck,
                         False,
                         self.qasm_output_path,
                     ],
                 )
                 if not res:
                     break
-                num_generated_benchmarks += 1
 
-            for device_name, max_qubits in devices:
-                for opt_level in range(4):
-                    # Creating the circuit on target-dependent: mapped level qiskit
-                    if max_qubits >= qc.num_qubits:
-                        res = timeout_watcher(
-                            qiskit_helper.get_mapped_level,
-                            self.timeout,
-                            [
-                                qc,
-                                gate_set_name,
-                                qc.num_qubits,
-                                device_name,
-                                opt_level,
-                                file_precheck,
-                                self.qasm_output_path,
-                            ],
-                        )
-                        if not res:
-                            break
-                        num_generated_benchmarks += 1
-
-            # Creating the circuit on both target-dependent levels for tket
-
-            res = timeout_watcher(
-                tket_helper.get_native_gates_level,
-                self.timeout,
-                [
-                    qc,
-                    gate_set_name,
-                    num_qubits,
-                    file_precheck,
-                    False,
-                    self.qasm_output_path,
-                ],
-            )
-            if not res:
-                continue
-            num_generated_benchmarks += 1
-
-            for device_name, max_qubits in devices:
-                if max_qubits >= qc.num_qubits:
-                    for lineplacement in (False, True):
-                        # Creating the circuit on target-dependent: mapped level tket
-                        res = timeout_watcher(
-                            tket_helper.get_mapped_level,
-                            self.timeout,
-                            [
-                                qc,
-                                gate_set_name,
-                                qc.num_qubits,
-                                device_name,
-                                lineplacement,
-                                file_precheck,
-                                False,
-                                self.qasm_output_path,
-                            ],
-                        )
-                        if not res:
-                            continue
-                        num_generated_benchmarks += 1
-        return num_generated_benchmarks != 0
-
-    def start_benchmark_generation(
-        self, create_circuit_function: Callable[..., QuantumCircuit], parameters: list[int | str], file_precheck: bool
-    ) -> bool:
-        res_qc_creation = timeout_watcher(create_circuit_function, self.timeout, parameters)
-        if not res_qc_creation:
-            return False
-        assert isinstance(res_qc_creation, QuantumCircuit)
-        return self.generate_circuits_on_all_levels(res_qc_creation, res_qc_creation.num_qubits, file_precheck)
+    def generate_indep_levels(
+        self,
+        file_precheck: bool,
+        lib: ModuleType,
+        parameter_space: list[tuple[int, str]] | list[int] | list[str] | range,
+    ) -> None:
+        for function in [qiskit_helper.get_indep_level, tket_helper.get_indep_level]:
+            for parameter_instance in parameter_space:
+                qc = timeout_watcher(lib.create_circuit, self.timeout, parameter_instance)
+                if not qc:
+                    break
+                assert isinstance(qc, QuantumCircuit)
+                res = timeout_watcher(
+                    function, self.timeout, [qc, qc.num_qubits, file_precheck, False, self.qasm_output_path]
+                )
+                if not res:
+                    break
 
 
 def get_benchmark(  # noqa: PLR0911, PLR0912, PLR0915
     benchmark_name: str,
     level: str | int,
     circuit_size: int | None = None,
     benchmark_instance_name: str | None = None,
@@ -279,16 +263,16 @@
     Keyword arguments:
     benchmark_name -- name of the to be generated benchmark
     level -- Choice of level, either as a string ("alg", "indep", "nativegates" or "mapped") or as a number between 0-3 where 0 corresponds to "alg" level and 3 to "mapped" level
     circuit_size -- Input for the benchmark creation, in most cases this is equal to the qubit number
     benchmark_instance_name -- Input selection for some benchmarks, namely "groundstate" and "shor"
     compiler -- "qiskit" or "tket"
     CompilerSettings -- Data class containing the respective compiler settings for the specified compiler (e.g., optimization level for Qiskit or placement for TKET)
-    gate_set_name -- "ibm", "rigetti", "ionq", or "oqc"
-    device_name -- "ibm_washington", "ibm_montreal", "rigetti_aspen_m2", "ionq11", ""oqc_lucy""
+    gate_set_name -- "ibm", "rigetti", "ionq", "oqc", or "quantinuum"
+    device_name -- "ibm_washington", "ibm_montreal", "rigetti_aspen_m2", "ionq_harmony", "ionq_aria1", ""oqc_lucy"", ""quantinuum_h2"",
     Return values:
     Quantum Circuit Object -- Representing the benchmark with the selected options, either as Qiskit::QuantumCircuit or Pytket::Circuit object (depending on the chosen compiler---while the algorithm level is always provided using Qiskit)
     """
 
     if benchmark_name not in utils.get_supported_benchmarks():
         msg = f"Selected benchmark is not supported. Valid benchmarks are {utils.get_supported_benchmarks()}."
         raise ValueError(msg)
@@ -420,44 +404,45 @@
     parser.add_argument("--file-name", type=str, help="optional filename", default="./config.json")
     args = parser.parse_args()
     benchmark_generator = BenchmarkGenerator(args.file_name)
     benchmark_generator.create_benchmarks_from_config(num_jobs)
 
 
 def timeout_watcher(
-    func: Callable[..., bool | QuantumCircuit], timeout: int, args: list[Any]
+    func: Callable[..., bool | QuantumCircuit], timeout: int, args: list[Any] | int | tuple[int, str] | str
 ) -> bool | QuantumCircuit | Circuit:
     class TimeoutException(Exception):  # Custom exception class
         pass
 
     def timeout_handler(_signum: Any, _frame: Any) -> None:  # Custom signal handler
         raise TimeoutException()
 
     # Change the behavior of SIGALRM
     signal.signal(signal.SIGALRM, timeout_handler)
     signal.alarm(timeout)
     try:
-        res = func(*args)
+        res = func(*args) if isinstance(args, (tuple, list)) else func(args)
     except TimeoutException:
         print(
             "Calculation/Generation exceeded timeout limit for ",
             func.__name__,
             func.__module__.split(".")[-1],
-            args[0].name,
-            args[1:],
         )
+        if isinstance(args, list) and isinstance(args[0], QuantumCircuit):
+            print(args[0].name, args[1:])
+        else:
+            print(args)
         return False
     except Exception as e:
         print(
             "Exception: ",
             e,
             func.__name__,
             func.__module__.split(".")[-1],
-            args[0],
-            args[1:],
+            args,
         )
         return False
     else:
         # Reset the alarm
         signal.alarm(0)
 
     return res
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/ae.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/ae.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/dj.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/dj.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/ghz.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/ghz.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/graphstate.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/graphstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/grover.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/grover.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/hhl.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qaoa.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Code based on https://qiskit.org/textbook/ch-applications/hhl_tutorial.html
+# Code from https://github.com/qiskit-community/qiskit-application-modules-demo-sessions/blob/main/qiskit-optimization/qiskit-optimization-demo.ipynb
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import numpy as np
-from qiskit.algorithms.linear_solvers.hhl import HHL
-from qiskit.algorithms.linear_solvers.matrices.tridiagonal_toeplitz import (
-    TridiagonalToeplitz,
-)
+from mqt.bench.utils import get_examplary_max_cut_qp
+from qiskit.algorithms.minimum_eigensolvers import QAOA
+from qiskit.algorithms.optimizers import SLSQP
+from qiskit.primitives import Sampler
+from qiskit_optimization import QuadraticProgram
 
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
-    """Returns a quantum circuit implementing the HHL algorithm for a specific example matrix.
+    """Returns a quantum circuit implementing the Quantum Approximation Optimization Algorithm for a specific max-cut
+     example.
 
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
 
-    a = 1
-    b = -1 / 3
+    qp = get_examplary_max_cut_qp(num_qubits)
+    assert isinstance(qp, QuadraticProgram)
 
-    vector = np.array([1] + [0] * (2**num_qubits - 1))
-    tridi_matrix = TridiagonalToeplitz(num_qubits, a, b)
-    qc = HHL().solve(tridi_matrix, vector).state
+    qaoa = QAOA(sampler=Sampler(), reps=2, optimizer=SLSQP(maxiter=25))
+    qaoa_result = qaoa.compute_minimum_eigenvalue(qp.to_ising()[0])
+    qc = qaoa.ansatz.bind_parameters(qaoa_result.optimal_point)
 
-    qc.name = "hhl"
-    qc.measure_all()
+    qc.name = "qaoa"
 
     return qc
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qaoa.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/vqe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-# Code from https://github.com/qiskit-community/qiskit-application-modules-demo-sessions/blob/main/qiskit-optimization/qiskit-optimization-demo.ipynb
+# Code based on https://github.com/qiskit-community/qiskit-application-modules-demo-sessions/blob/main/qiskit-optimization/qiskit-optimization-demo.ipynb
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mqt.bench.utils import get_examplary_max_cut_qp
-from qiskit.algorithms.minimum_eigensolvers import QAOA
+from qiskit.algorithms.minimum_eigensolvers import VQE
 from qiskit.algorithms.optimizers import SLSQP
-from qiskit.primitives import Sampler
+from qiskit.circuit.library import RealAmplitudes
+from qiskit.primitives import Estimator
 from qiskit_optimization import QuadraticProgram
 
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
-    """Returns a quantum circuit implementing the Quantum Approximation Optimization Algorithm for a specific max-cut
+    """Returns a quantum circuit implementing the Variational Quantum Eigensolver Algorithm for a specific max-cut
      example.
 
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
 
     qp = get_examplary_max_cut_qp(num_qubits)
     assert isinstance(qp, QuadraticProgram)
 
-    qaoa = QAOA(sampler=Sampler(), reps=2, optimizer=SLSQP(maxiter=25))
-    qaoa_result = qaoa.compute_minimum_eigenvalue(qp.to_ising()[0])
-    qc = qaoa.ansatz.bind_parameters(qaoa_result.optimal_point)
+    ansatz = RealAmplitudes(num_qubits, reps=2)
+    vqe = VQE(ansatz=ansatz, optimizer=SLSQP(maxiter=25), estimator=Estimator())
+    vqe_result = vqe.compute_minimum_eigenvalue(qp.to_ising()[0])
+    qc = vqe.ansatz.bind_parameters(vqe_result.optimal_point)
 
-    qc.name = "qaoa"
+    qc.measure_all()
+    qc.name = "vqe"
 
     return qc
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qft.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qft.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qftentangled.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qftentangled.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeexact.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeinexact.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeinexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qwalk.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qwalk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 from qiskit import AncillaRegister, QuantumCircuit, QuantumRegister
 
 
 def create_circuit(
     n: int,
+    ancillary_mode: str = "noancilla",
     depth: int = 3,
     coin_state_preparation: QuantumCircuit = None,
-    ancillary_mode: str = "noancilla",
 ) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Walk algorithm.
 
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     depth -- number of quantum steps
     coin_state_preparation -- optional quantum circuit for state preparation
     ancillary_mode -- defining the decomposition scheme
     """
-
     n = n - 1  # because one qubit is needed for the coin
     coin = QuantumRegister(1, "coin")
     node = QuantumRegister(n, "node")
 
     n_anc = 0
     ancillary_cutoff_recursion = 3
     if ancillary_mode == "recursion" and n > ancillary_cutoff_recursion:
@@ -87,9 +86,10 @@
                     ancilla_qubits=anc[:],
                 )
             qc.cx(coin, node[n - 1])
             qc.x(node[1:])
             qc.x(coin)
 
     qc.measure_all()
+    qc.name = qc.name + "-" + ancillary_mode
 
     return qc
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/realamprandom.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/su2random.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
-from qiskit.circuit.library import RealAmplitudes
+from qiskit.circuit.library import EfficientSU2
 
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
-    """Returns a quantum circuit implementing the RealAmplitudes ansatz with random parameter
+    """Returns a quantum circuit implementing EfficientSU2 ansatz with random parameter
     values.
 
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
 
     np.random.seed(10)
-    qc = RealAmplitudes(num_qubits, entanglement="full", reps=3)
+    qc = EfficientSU2(num_qubits, entanglement="full", reps=3)
     num_params = qc.num_parameters
-    qc = qc.bind_parameters(np.random.rand(num_params))
+    qc = qc.bind_parameters(2 * np.pi * np.random.rand(num_params))
     qc.measure_all()
-    qc.name = "realamprandom"
+    qc.name = "su2random"
 
     return qc
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/su2random.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/realamprandom.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
-from qiskit.circuit.library import EfficientSU2
+from qiskit.circuit.library import RealAmplitudes
 
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
-    """Returns a quantum circuit implementing EfficientSU2 ansatz with random parameter
+    """Returns a quantum circuit implementing the RealAmplitudes ansatz with random parameter
     values.
 
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
 
     np.random.seed(10)
-    qc = EfficientSU2(num_qubits, entanglement="full", reps=3)
+    qc = RealAmplitudes(num_qubits, entanglement="full", reps=3)
     num_params = qc.num_parameters
-    qc = qc.bind_parameters(np.random.rand(num_params))
+    qc = qc.bind_parameters(2 * np.pi * np.random.rand(num_params))
     qc.measure_all()
-    qc.name = "su2random"
+    qc.name = "realamprandom"
 
     return qc
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/twolocalrandom.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/twolocalrandom.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
 
     np.random.seed(10)
     qc = TwoLocal(num_qubits, "ry", "cx", entanglement="full", reps=3)
     num_params = qc.num_parameters
-    qc = qc.bind_parameters(np.random.rand(num_params))
+    qc = qc.bind_parameters(2 * np.pi * np.random.rand(num_params))
     qc.measure_all()
     qc.name = "twolocalrandom"
 
     return qc
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/benchmarks/wstate.py` & `mqt.bench-1.0.0/src/mqt/bench/benchmarks/wstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation.py` & `mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,28 @@
     num_qubits: int
     depth: int
     num_gates: int
     num_multiple_qubit_gates: int
     supermarq_features: utils.SupermarqFeatures
 
 
-def evaluate_qasm_file(filename: str) -> EvaluationResult:
-    qc = QuantumCircuit.from_qasm_file(filename)
+def evaluate_qasm_file(filename: str) -> EvaluationResult | None:
+    try:
+        qc = QuantumCircuit.from_qasm_file(filename)
+    except Exception as e:
+        print(f"Failed for {filename}: {e}")
+        return EvaluationResult(
+            filename=filename,
+            num_qubits=-1,
+            depth=-1,
+            num_gates=-1,
+            num_multiple_qubit_gates=-1,
+            supermarq_features=utils.SupermarqFeatures(-1, -1, -1, -1, -1),
+        )
+
     return EvaluationResult(
         filename=filename,
         num_qubits=int(str(filename).split("_")[-1].split(".")[0]),
         depth=qc.depth(),
         num_gates=sum(qc.count_ops().values()),
         num_multiple_qubit_gates=qc.num_nonlocal_gates(),
         supermarq_features=utils.calc_supermarq_features(qc),
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation_visualization.ipynb` & `mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_visualization.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9819242185510568%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(9, \'font = {"size": 16}\\n\')], delete: [9]}}, 1: '*

 * *            "{'id': '03f145b0'}, 2: {'source': {insert: [(0, 'with "*

 * *            'Path("evaluation_data.pkl").open("rb") as f:\\n\')], delete: [0]}}, 6: {\'source\': '*

 * *            "{insert: [(5, 'mapped_quantinuum_count = evaluation.count_occurrences(benchmarks, "*

 * *            '"mapped_quantinuum")\\n\'), (6, \'mapped_ionq_aria1_count = '*

 * *            'evaluation.count_occurrences(benchmarks, "mapped_ionq_aria1")\\n\ […]*

```diff
@@ -12,36 +12,36 @@
                 "import matplotlib.pyplot as plt\n",
                 "import matplotlib\n",
                 "import seaborn as sns\n",
                 "import pandas as pd\n",
                 "from pathlib import Path\n",
                 "from mqt.bench.evaluation import evaluation\n",
                 "\n",
-                "font = {\"size\": 12}\n",
+                "font = {\"size\": 16}\n",
                 "matplotlib.rc(\"font\", **font)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5e7e54e4",
+            "id": "03f145b0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "evaluation.create_statistics()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "062813f4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with Path(\"./evaluation_data.pkl\").open(\"rb\") as f:\n",
+                "with Path(\"evaluation_data.pkl\").open(\"rb\") as f:\n",
                 "    eval_data = pickle.load(f)\n",
                 "df = pd.DataFrame(eval_data)\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
@@ -90,15 +90,17 @@
             "outputs": [],
             "source": [
                 "overall_count_mapped = evaluation.count_occurrences(benchmarks, \"mapped\")\n",
                 "mapped_ibm_montreal_count = evaluation.count_occurrences(benchmarks, \"mapped_ibm_montreal\")\n",
                 "mapped_ibm_washington_count = evaluation.count_occurrences(benchmarks, \"mapped_ibm_washington\")\n",
                 "mapped_oqc_lucy_count = evaluation.count_occurrences(benchmarks, \"mapped_oqc_lucy\")\n",
                 "mapped_rigetti_count = evaluation.count_occurrences(benchmarks, \"mapped_rigetti\")\n",
-                "mapped_ionq_count = evaluation.count_occurrences(benchmarks, \"mapped_ionq\")\n",
+                "mapped_quantinuum_count = evaluation.count_occurrences(benchmarks, \"mapped_quantinuum\")\n",
+                "mapped_ionq_aria1_count = evaluation.count_occurrences(benchmarks, \"mapped_ionq_aria1\")\n",
+                "mapped_ionq_harmony_count = evaluation.count_occurrences(benchmarks, \"mapped_ionq_harmony\")\n",
                 "\n",
                 "qiskit_qubit_numbers = evaluation.count_qubit_numbers_per_compiler(benchmarks, \"qiskit\")\n",
                 "tket_qubit_numbers = evaluation.count_qubit_numbers_per_compiler(benchmarks, \"tket\")"
             ]
         },
         {
             "cell_type": "code",
@@ -107,30 +109,42 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "perc_montreal = mapped_ibm_montreal_count / overall_count_mapped\n",
                 "perc_washington = mapped_ibm_washington_count / overall_count_mapped\n",
                 "perc_oqc = mapped_oqc_lucy_count / overall_count_mapped\n",
                 "perc_rigetti = mapped_rigetti_count / overall_count_mapped\n",
-                "perc_ionq = mapped_ionq_count / overall_count_mapped"
+                "perc_quantinuum = mapped_quantinuum_count / overall_count_mapped\n",
+                "perc_ionq_aria1 = mapped_ionq_aria1_count / overall_count_mapped\n",
+                "perc_ionq_harmony = mapped_ionq_harmony_count / overall_count_mapped"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "089acc25",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = [perc_washington, perc_rigetti, perc_montreal, perc_ionq, perc_oqc]\n",
-                "colors = [\"#B7E6A5\", \"#7CCBA2\", \"#46AEA0\", \"#089099\", \"#00718B\"]\n",
-                "labels = [\"IBMQ Washington (127)\", \"Rigetti Aspen M2 (80)\", \"IBMQ Montreal (27)\", \"IonQ Harmony (11)\", \"OQC Lucy (8)\"]\n",
+                "font = {\"size\": 12}\n",
+                "matplotlib.rc(\"font\", **font)\n",
+                "data = [perc_washington, perc_rigetti, perc_montreal, perc_quantinuum, perc_ionq_aria1, perc_ionq_harmony, perc_oqc]\n",
+                "colors = [\"#B7E6A5\", \"#7CCBA2\", \"#46AEA0\", \"#089099\", \"#02818B\", \"#026688\", \"#025582\"]\n",
+                "labels = [\n",
+                "    \"IBMQ Washington (127)\",\n",
+                "    \"Rigetti Aspen M2 (80)\",\n",
+                "    \"Quantinuum H2 (32)\",\n",
+                "    \"IBMQ Montreal (27)\",\n",
+                "    \"IonQ Aria 1 (25)\",\n",
+                "    \"IonQ Harmony (11)\",\n",
+                "    \"OQC Lucy (8)\",\n",
+                "]\n",
                 "pies = plt.pie(data, labels=labels, autopct=\"%1.1f%%\", colors=colors)\n",
                 "for pie in pies[0]:\n",
-                "    pie.set_alpha(0.6)\n",
+                "    pie.set_alpha(0.7)\n",
                 "plt.savefig(\"results/pie.pdf\", format=\"pdf\", bbox_inches=\"tight\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1fc0ca44",
@@ -142,31 +156,33 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fd1cc85d",
             "metadata": {},
             "outputs": [],
             "source": [
+                "font = {\"size\": 16}\n",
+                "matplotlib.rc(\"font\", **font)\n",
                 "qiskit_qubit_numbers = evaluation.count_qubit_numbers_per_compiler(benchmarks, \"qiskit\")\n",
                 "tket_qubit_numbers = evaluation.count_qubit_numbers_per_compiler(benchmarks, \"tket\")\n",
                 "\n",
                 "# colors = ['#7CCBA2', '#46AEA0', '#089099', \"#00718B\", \"#045275\", \"#003147\"]\n",
                 "# colors = ['#089099', '#003147']\n",
-                "plt.figure(figsize=(10, 5))\n",
+                "plt.figure(figsize=(8, 5))\n",
                 "plot = sns.histplot(\n",
-                "    data=[qiskit_qubit_numbers, tket_qubit_numbers],\n",
-                "    bins=128,\n",
+                "    data=[tket_qubit_numbers, qiskit_qubit_numbers],\n",
+                "    bins=129,\n",
                 "    stat=\"density\",\n",
                 "    alpha=0.3,\n",
                 "    kde=True,\n",
                 "    edgecolor=\"white\",\n",
                 "    linewidth=0.5,\n",
-                "    palette=sns.color_palette(\"viridis\", 2),\n",
+                "    palette=sns.color_palette(\"viridis\", 2)[::-1],\n",
                 ")\n",
-                "plt.legend([\"TKET\", \"Qiskit\"])\n",
+                "plt.legend([\"Qiskit\", \"TKET\"])\n",
                 "plt.ylabel(\"Relative Frequency\")\n",
                 "plt.xlabel(\"Number of Qubits\")\n",
                 "plt.savefig(\"results/qubit_dist.pdf\", format=\"pdf\", bbox_inches=\"tight\")\n",
                 "plt.show()"
             ]
         },
         {
@@ -194,15 +210,15 @@
                 "]\n",
                 "labels = [\n",
                 "    \"Program Communication\",\n",
                 "    \"Critical Depth\",\n",
                 "    \"Entanglement Ratio\",\n",
                 "    \"Liveness\",\n",
                 "    \"Parallelism\",\n",
-                "    \"Percentage Multi-Qubit Gates\",\n",
+                "    \"Percentage \\nMulti-Qubit Gates\",\n",
                 "]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "54ac24f3",
@@ -218,30 +234,14 @@
                 "    pc.set_facecolor(color)\n",
                 "\n",
                 "ax.set_xticks(pos)\n",
                 "plt.xticks(rotation=0)\n",
                 "ax.set_xticklabels(labels)\n",
                 "plt.savefig(\"results/violins.pdf\", format=\"pdf\", bbox_inches=\"tight\")"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a03c6674",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "b29d06c6",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/evaluation/results/pie.pdf` & `mqt.bench-1.0.0/src/mqt/bench/evaluation/results/pie.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,16 +1,23 @@
 IBMQ Washington (127)
-42.6%
-
-31.5%
 Rigetti Aspen M2 (80)
 
-4.6%
-6.6%
-14.7%
+32.8%
+24.3%
+11.4%
+
+Quantinuum H2 (32)
+
+12.5%
+
+IBMQ Montreal (27)
+
+3.6%
+5.2%
+10.3%
 
 OQC Lucy (8)
 IonQ Harmony (11)
 
-IBMQ Montreal (27)
+IonQ Aria 1 (25)
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/evaluation/results/qubit_dist.pdf` & `mqt.bench-1.0.0/src/mqt/bench/evaluation/results/qubit_dist.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### pdftotext {} -

```diff
@@ -16,15 +16,13 @@
 0
 
 20
 
 40
 
 60
-80
+80 100
 Number of Qubits
 
-100
-
 120
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/evaluation/results/violins.pdf` & `mqt.bench-1.0.0/src/mqt/bench/evaluation/results/violins.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,20 +1,18 @@
 1.0
 0.8
 0.6
 0.4
 0.2
 0.0
-
-Program Communication
-
-Critical Depth
+Program Communication Critical Depth
 
 Entanglement Ratio
 
 Liveness
 
 Parallelism
 
-Percentage Multi-Qubit Gates
+Percentage
+Multi-Qubit Gates
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/qiskit_helper.py` & `mqt.bench-1.0.0/src/mqt/bench/qiskit_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         return get_ionq_native_gates()
     if gate_set_name == "oqc":
         return get_oqc_native_gates()
     if gate_set_name == "ibm":
         return get_ibm_native_gates()
     if gate_set_name == "rigetti":
         return get_rigetti_native_gates()
+    if gate_set_name == "quantinuum":
+        return get_quantinuum_native_gates()
     raise ValueError("Unknown gate set name: " + gate_set_name)
 
 
 def get_ibm_native_gates() -> list[str]:
     return ["rz", "sx", "x", "cx", "measure"]
 
 
@@ -34,14 +36,18 @@
     return ["rxx", "rz", "ry", "rx", "measure"]
 
 
 def get_oqc_native_gates() -> list[str]:
     return ["rz", "sx", "x", "ecr", "measure"]
 
 
+def get_quantinuum_native_gates() -> list[str]:
+    return ["rzz", "rz", "ry", "rx", "measure"]
+
+
 @overload
 def get_indep_level(
     qc: QuantumCircuit,
     num_qubits: int | None,
     file_precheck: bool,
     return_qc: Literal[True],
     target_directory: str = "./",
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/tket_helper.py` & `mqt.bench-1.0.0/src/mqt/bench/tket_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from typing import TYPE_CHECKING, Literal, overload
 
 from mqt.bench import utils
 from pytket import OpType
 from pytket.architecture import Architecture  # type: ignore[attr-defined]
 from pytket.extensions.qiskit import qiskit_to_tk
 from pytket.passes import (  # type: ignore[attr-defined]
-    CliffordSimp,
     CXMappingPass,
     FullPeepholeOptimise,
-    KAKDecomposition,
+    PeepholeOptimise2Q,
     PlacementPass,
     RoutingPass,
     SynthesiseTket,
     auto_rebase_pass,
 )
 from pytket.placement import GraphPlacement, LinePlacement  # type: ignore[attr-defined]
 from pytket.qasm import circuit_to_qasm_str
@@ -31,23 +30,31 @@
         return get_ionq_rebase(get_gatenames)
     if gate_set_name == "oqc":
         return get_oqc_rebase(get_gatenames)
     if gate_set_name == "ibm":
         return get_ibm_rebase(get_gatenames)
     if gate_set_name == "rigetti":
         return get_rigetti_rebase(get_gatenames)
+    if gate_set_name == "quantinuum":
+        return get_quantinuum_rebase(get_gatenames)
     raise ValueError("Unknown gate set name: " + gate_set_name)
 
 
 def get_ionq_rebase(get_gatenames: bool = False) -> RebaseCustom:
     if get_gatenames:
         return ["rz", "ry", "rx", "rxx", "measure"]
     return auto_rebase_pass({OpType.Rz, OpType.Ry, OpType.Rx, OpType.XXPhase, OpType.Measure})
 
 
+def get_quantinuum_rebase(get_gatenames: bool = False) -> RebaseCustom:
+    if get_gatenames:
+        return ["rz", "ry", "rx", "rzz", "measure"]
+    return auto_rebase_pass({OpType.Rz, OpType.Ry, OpType.Rx, OpType.ZZPhase, OpType.Measure})
+
+
 def get_oqc_rebase(get_gatenames: bool = False) -> RebaseCustom:
     if get_gatenames:
         return ["rz", "sx", "x", "ecr", "measure"]
     return auto_rebase_pass({OpType.Rz, OpType.SX, OpType.X, OpType.ECR, OpType.Measure})
 
 
 def get_rigetti_rebase(get_gatenames: bool = False) -> RebaseCustom:
@@ -319,17 +326,15 @@
     qc_tket.add_blank_wires(diff)
 
     native_gate_set_rebase.apply(qc_tket)
     FullPeepholeOptimise(target_2qb_gate=OpType.TK2).apply(qc_tket)
     placer = LinePlacement(arch) if lineplacement else GraphPlacement(arch)
     PlacementPass(placer).apply(qc_tket)
     RoutingPass(arch).apply(qc_tket)
-    SynthesiseTket().apply(qc_tket)
-    KAKDecomposition(allow_swaps=False).apply(qc_tket)
-    CliffordSimp(allow_swaps=False).apply(qc_tket)
+    PeepholeOptimise2Q(allow_swaps=False).apply(qc_tket)
     SynthesiseTket().apply(qc_tket)
     if not qc_tket.valid_connectivity(arch, directed=True):
         CXMappingPass(arc=arch, placer=placer, directed_cx=True, delay_measures=False).apply(qc_tket)
     native_gate_set_rebase.apply(qc_tket)
 
     if return_qc:
         return qc_tket
```

### Comparing `mqt.bench-0.4.4/src/mqt/bench/utils.py` & `mqt.bench-1.0.0/src/mqt/bench/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         "ghz",
         "graphstate",
         "portfolioqaoa",
         "portfoliovqe",
         "qaoa",
         "qft",
         "qftentangled",
-        "qgan",
+        "qnn",
         "qpeexact",
         "qpeinexact",
         "qwalk-noancilla",
         "qwalk-v-chain",
+        "random",
         "realamprandom",
         "su2random",
         "twolocalrandom",
         "vqe",
         "wstate",
         "shor",
-        "hhl",
         "pricingcall",
         "pricingput",
         "groundstate",
         "routing",
         "tsp",
     ]
 
@@ -81,19 +81,15 @@
 
 
 def get_supported_compilers() -> list[str]:
     return ["qiskit", "tket"]
 
 
 def get_supported_gatesets() -> list[str]:
-    return ["ibm", "rigetti", "ionq", "oqc"]
-
-
-def get_supported_devices() -> list[str]:
-    return ["ibm_washington", "ibm_montreal", "rigetti_aspen_m2", "ionq11", "oqc_lucy"]
+    return ["ibm", "rigetti", "ionq", "oqc", "quantinuum"]
 
 
 def get_default_qasm_output_path() -> str:
     """Returns the path where all .qasm files are stored."""
     return str(resources.files("mqt.benchviewer") / "static" / "files" / "qasm_output")
 
 
@@ -146,21 +142,21 @@
 
     inverted = [[item[1], item[0]] for item in c_map_rigetti]
     c_map_rigetti = c_map_rigetti + inverted
 
     return c_map_rigetti
 
 
-def get_ionq11_c_map() -> list[list[int]]:
-    ionq11_c_map = []
-    for i in range(0, 11):
-        for j in range(0, 11):
+def get_fully_connected_cmap(num_qubits: int) -> list[list[int]]:
+    c_map = []
+    for i in range(0, num_qubits):
+        for j in range(0, num_qubits):
             if i != j:
-                ionq11_c_map.append([i, j])
-    return ionq11_c_map
+                c_map.append([i, j])
+    return c_map
 
 
 def get_openqasm_gates() -> list[str]:
     """Returns a list of all quantum gates within the openQASM 2.0 standard header."""
     # according to https://github.com/Qiskit/qiskit-terra/blob/main/qiskit/qasm/libs/qelib1.inc
     return [
         "u3",
@@ -264,24 +260,36 @@
     # source: https://github.com/aws/amazon-braket-examples/blob/main/examples/braket_features/Verbatim_Compilation.ipynb
 
     # Connections are NOT bidirectional, this is not an accident
     return [[0, 1], [0, 7], [1, 2], [2, 3], [7, 6], [6, 5], [4, 3], [4, 5]]
 
 
 def get_cmap_from_devicename(device: str) -> list[list[int]]:
-    if device == "ibm_washington":
-        return cast(list[list[int]], FakeWashington().configuration().coupling_map)
-    if device == "ibm_montreal":
-        return cast(list[list[int]], FakeMontreal().configuration().coupling_map)
-    if device == "rigetti_aspen_m2":
-        return get_rigetti_aspen_m2_map()
-    if device == "oqc_lucy":
-        return get_cmap_oqc_lucy()
-    if device == "ionq11":
-        return get_ionq11_c_map()
+    c_map_functions = {
+        "ibm_washington": FakeWashington,
+        "ibm_montreal": FakeMontreal,
+        "rigetti_aspen_m2": get_rigetti_aspen_m2_map,
+        "oqc_lucy": get_cmap_oqc_lucy,
+        "ionq_harmony": get_fully_connected_cmap,
+        "ionq_aria1": get_fully_connected_cmap,
+        "quantinuum_h2": get_fully_connected_cmap,
+    }
+
+    if device in c_map_functions:
+        if device == "ibm_washington" or device == "ibm_montreal":
+            cmap = c_map_functions[device]().configuration().coupling_map
+        elif device == "ionq_harmony":
+            cmap = c_map_functions[device](11)
+        elif device == "ionq_aria1":
+            cmap = c_map_functions[device](25)
+        elif device == "quantinuum_h2":
+            cmap = c_map_functions[device](32)
+        else:
+            cmap = c_map_functions[device]()
+        return cast(list[list[int]], cmap)
     error_msg = f"Device {device} is not supported."
     raise ValueError(error_msg)
 
 
 def postprocess_single_oqc_file(filename: str) -> None:
     with Path(filename).open() as f:
         lines = f.readlines()
@@ -332,15 +340,20 @@
             connectivity_collection[int(qubit_index)].extend(to_be_added_entries)
 
     connectivity: list[int] = []
     for i in range(qc.num_qubits):
         connectivity.append(len(set(connectivity_collection[i])))
 
     count_ops = qc.count_ops()
-    num_gates = sum(count_ops.values()) - count_ops.get("measure") - count_ops.get("barrier")
+    num_gates = sum(count_ops.values())
+    # before subtracting the measure and barrier gates, check whether it is in the dict
+    if "measure" in count_ops:
+        num_gates -= count_ops.get("measure")
+    if "barrier" in count_ops:
+        num_gates -= count_ops.get("barrier")
     num_multiple_qubit_gates = qc.num_nonlocal_gates()
     depth = qc.depth(lambda x: x[0].name != "barrier" and x[0].name != "measure")
     program_communication = np.sum(connectivity) / (qc.num_qubits * (qc.num_qubits - 1))
 
     if num_multiple_qubit_gates == 0:
         critical_depth = 0.0
     else:
@@ -369,16 +382,38 @@
         liveness,
     )
 
 
 def get_module_for_benchmark(benchmark_name: str) -> ModuleType:
     if benchmark_name in ["portfolioqaoa", "portfoliovqe", "pricingcall", "pricingput"]:
         return import_module("mqt.bench.benchmarks.qiskit_application_finance." + benchmark_name)
-    if benchmark_name == "qgan":
-        return import_module("mqt.bench.benchmarks.qiskit_application_ml.qgan")
+    if benchmark_name == "qnn":
+        return import_module("mqt.bench.benchmarks.qiskit_application_ml.qnn")
     if benchmark_name == "groundstate":
         return import_module("mqt.bench.benchmarks.qiskit_application_nature.groundstate")
     if benchmark_name == "routing":
         return import_module("mqt.bench.benchmarks.qiskit_application_optimization.routing")
     if benchmark_name == "tsp":
         return import_module("mqt.bench.benchmarks.qiskit_application_optimization.tsp")
     return import_module("mqt.bench.benchmarks." + benchmark_name)
+
+
+def get_compilation_paths() -> list[tuple[str, list[tuple[str, int]]]]:
+    return [
+        ("ibm", [("ibm_washington", 127), ("ibm_montreal", 27)]),
+        ("rigetti", [("rigetti_aspen_m2", 80)]),
+        ("ionq", [("ionq_harmony", 11), ("ionq_aria1", 25)]),
+        ("oqc", [("oqc_lucy", 8)]),
+        ("quantinuum", [("quantinuum_h2", 32)]),
+    ]
+
+
+def get_supported_devices() -> list[str]:
+    return [
+        "ibm_washington",
+        "ibm_montreal",
+        "rigetti_aspen_m2",
+        "ionq_harmony",
+        "ionq_aria1",
+        "oqc_lucy",
+        "quantinuum_h2",
+    ]
```

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/backend.py` & `mqt.bench-1.0.0/src/mqt/benchviewer/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,49 +74,49 @@
             {
                 "name": "Quantum Approximation Optimization Algorithm (QAOA)",
                 "id": "9",
                 "filename": "qaoa",
             },
             {"name": "Quantum Fourier Transformation (QFT)", "id": "10", "filename": "qft"},
             {"name": "QFT Entangled", "id": "11", "filename": "qftentangled"},
-            {"name": "Quantum Generative Adversarial Network", "id": "12", "filename": "qgan"},
+            {"name": "Quantum Neural Network (QNN)", "id": "12", "filename": "qnn"},
             {
                 "name": "Quantum Phase Estimation (QPE) exact",
                 "id": "13",
                 "filename": "qpeexact",
             },
             {
                 "name": "Quantum Phase Estimation (QPE) inexact",
                 "id": "14",
                 "filename": "qpeinexact",
             },
             {"name": "Quantum Walk (no ancilla)", "id": "15", "filename": "qwalk-noancilla"},
             {"name": "Quantum Walk (v-chain)", "id": "16", "filename": "qwalk-v-chain"},
-            {"name": "Variational Quantum Eigensolver (VQE)", "id": "17", "filename": "vqe"},
+            {"name": "Random Circuit", "id": "17", "filename": "random"},
+            {"name": "Variational Quantum Eigensolver (VQE)", "id": "18", "filename": "vqe"},
             {
                 "name": "Efficient SU2 ansatz with Random Parameters",
-                "id": "18",
+                "id": "19",
                 "filename": "su2random",
             },
             {
                 "name": "Real Amplitudes ansatz with Random Parameters",
-                "id": "19",
+                "id": "20",
                 "filename": "realamprandom",
             },
             {
                 "name": "Two Local ansatz with Random Parameters",
-                "id": "20",
+                "id": "21",
                 "filename": "twolocalrandom",
             },
-            {"name": "W-State", "id": "21", "filename": "wstate"},
+            {"name": "W-State", "id": "22", "filename": "wstate"},
         ]
 
         self.nonscalable_benchmarks = [
-            {"name": "Ground State", "id": "22", "filename": "groundstate"},
-            {"name": "HHL", "id": "23", "filename": "hhl"},
+            {"name": "Ground State", "id": "23", "filename": "groundstate"},
             {"name": "Pricing Call Option", "id": "24", "filename": "pricingcall"},
             {"name": "Pricing Put Option", "id": "25", "filename": "pricingput"},
             {"name": "Routing", "id": "26", "filename": "routing"},
             {"name": "Shor's", "id": "27", "filename": "shor"},
             {"name": "Travelling Salesman", "id": "28", "filename": "tsp"},
         ]
 
@@ -317,28 +317,31 @@
             native_qiskit_opt_lvls.append(1) if "nativegates_qiskit_compiler_opt1" in k else None
             native_qiskit_opt_lvls.append(2) if "nativegates_qiskit_compiler_opt2" in k else None
             native_qiskit_opt_lvls.append(3) if "nativegates_qiskit_compiler_opt3" in k else None
             native_gatesets.append("ibm") if "nativegates_ibm" in k else None
             native_gatesets.append("rigetti") if "nativegates_rigetti" in k else None
             native_gatesets.append("oqc") if "nativegates_oqc" in k else None
             native_gatesets.append("ionq") if "nativegates_ionq" in k else None
+            native_gatesets.append("quantinuum") if "nativegates_quantinuum" in k else None
 
             mapped_qiskit_compiler = "mapped_qiskit_compiler" in k or mapped_qiskit_compiler
             mapped_tket_compiler = "mapped_tket_compiler" in k or mapped_tket_compiler
             mapped_qiskit_opt_lvls.append(0) if "mapped_qiskit_compiler_opt0" in k else None
             mapped_qiskit_opt_lvls.append(1) if "mapped_qiskit_compiler_opt1" in k else None
             mapped_qiskit_opt_lvls.append(2) if "mapped_qiskit_compiler_opt2" in k else None
             mapped_qiskit_opt_lvls.append(3) if "mapped_qiskit_compiler_opt3" in k else None
             mapped_tket_placements.append("graph") if "mapped_tket_compiler_graph" in k else None
             mapped_tket_placements.append("line") if "mapped_tket_compiler_line" in k else None
             mapped_devices.append("ibm_montreal") if "device_ibm_montreal" in k else None
             mapped_devices.append("ibm_washington") if "device_ibm_washington" in k else None
-            mapped_devices.append("rigetti_aspen") if "device_rigetti_aspen" in k else None
+            mapped_devices.append("rigetti_aspen_m2") if "device_rigetti_aspen_m2" in k else None
             mapped_devices.append("oqc_lucy") if "device_oqc_lucy" in k else None
-            mapped_devices.append("ionq11") if "device_ionq_ionq11" in k else None
+            mapped_devices.append("ionq_harmony") if "device_ionq_harmony" in k else None
+            mapped_devices.append("ionq_aria1") if "device_ionq_aria1" in k else None
+            mapped_devices.append("quantinuum_h2") if "device_quantinuum_h2" in k else None
 
         return BenchmarkConfiguration(
             min_qubits=min_qubits,
             max_qubits=max_qubits,
             indices_benchmarks=indices_benchmarks,
             indep_qiskit_compiler=indep_qiskit_compiler,
             indep_tket_compiler=indep_tket_compiler,
@@ -564,28 +567,41 @@
         return "oqc"
     if "ionq" in filename:
         return "ionq"
     if "ibm" in filename:
         return "ibm"
     if "rigetti" in filename:
         return "rigetti"
+    if "quantinuum" in filename:
+        return "quantinuum"
     raise ValueError("Unknown gate set: " + filename)
 
 
 def get_target_device(filename: str) -> str:
-    if "ibm_washington" in filename:
-        return "ibm_washington"
-    if "ibm_montreal" in filename:
-        return "ibm_montreal"
-    if "rigetti_aspen" in filename:
-        return "rigetti_aspen"
+    devices = [
+        "ibm_washington",
+        "ibm_montreal",
+        "rigetti_aspen_m2",
+        "ionq_harmony",
+        "ionq_aria1",
+        "oqc_lucy",
+        "quantinuum_h2",
+    ]
     if "ionq11" in filename:
-        return "ionq11"
-    if "oqc_lucy" in filename:
-        return "oqc_lucy"
+        import warnings
+
+        warnings.warn(
+            "You are using a deprecated MQTBench version. Please re-install MQTBench or remove the MQTBench_all.zip file located at mqt/benchviewer/static/files/MQTBench_all.zip and re-start the server to download the latest benchmarks",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return "ionq_harmony"
+    for device in devices:
+        if device in filename:
+            return device
     raise ValueError("Unknown target device: " + filename)
 
 
 def get_compiler_and_settings(filename: str) -> tuple[str, str | int | None]:
     if "qiskit" in filename:
         return "qiskit", get_opt_level(filename)
     if "tket" in filename:
```

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/main.py` & `mqt.bench-1.0.0/src/mqt/benchviewer/main.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/static/favicon.ico` & `mqt.bench-1.0.0/src/mqt/benchviewer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/static/mqt_dark.png` & `mqt.bench-1.0.0/src/mqt/benchviewer/static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/static/tum_logo.svg` & `mqt.bench-1.0.0/src/mqt/benchviewer/static/tum_logo.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/templates/benchmark_description.html` & `mqt.bench-1.0.0/src/mqt/benchviewer/templates/benchmark_description.html`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,14 @@
             <td style="vertical-align: top">Grover's (v-chain)</td>
             <td style="vertical-align: top">
               Similar to the algorithm above with the difference, that the
               ancillary mode is a v-chain in this algorithm.
             </td>
           </tr>
           <tr>
-            <td style="vertical-align: top">HHL</td>
-            <td style="vertical-align: top">
-              The Harrow-Hassadim-Lloyd algorithm is used to solve linear system
-              of equations. Here, we use a specific system of equations.
-            </td>
-          </tr>
-          <tr>
             <td style="vertical-align: top">
               Portfolio Optimization with QAOA
             </td>
             <td style="vertical-align: top">
               This algorithms solves the mean-variance portfolio optimization
               problem for different assets. In this case, a QAOA algorithm
               instance is used. The source code for the algorithmic level
@@ -231,23 +224,20 @@
             <td style="vertical-align: top">Entangled QFT</td>
             <td style="vertical-align: top">
               Applies regular QFT to entangled qubits.
             </td>
           </tr>
 
           <tr>
+            <td style="vertical-align: top">Quantum Neural Network (QNN)</td>
             <td style="vertical-align: top">
-              Quantum Generative Adversarial Network (QGAN)
-            </td>
-            <td style="vertical-align: top">
-              This algorithm class is the quantum equivalent to classical GAN
-              and learns the underlying distribution of input data. The source
-              code for the algorithmic level originates from
+              This algorithm class is the quantum equivalent to classical Neural
+              Network. The source code for the algorithmic level originates from
               <a
-                href="https://qiskit.org/documentation/machine-learning/tutorials/04_qgans_for_loading_random_distributions.html"
+                href="https://qiskit.org/ecosystem/machine-learning/stubs/qiskit_machine_learning.neural_networks.EstimatorQNN.html"
                 target="_blank"
                 >this page</a
               >.
             </td>
           </tr>
           <tr>
             <td style="vertical-align: top">
@@ -281,14 +271,21 @@
             <td style="vertical-align: top">Quantum Walk (v-chain)</td>
             <td style="vertical-align: top">
               Similar to the algorithm above with the difference, that the
               ancillary mode is a v-chain in this algorithm.
             </td>
           </tr>
           <tr>
+            <td style="vertical-align: top">Random Circuit</td>
+            <td style="vertical-align: top">
+              This benchmark represents a random circuit which is twice as deep
+              as wide. It considers random quantum gates with up to four qubits.
+            </td>
+          </tr>
+          <tr>
             <td style="vertical-align: top">Routing</td>
             <td style="vertical-align: top">
               This problem is similar to the travelling salesman problem with
               the difference, that more than one vehicle may be used to travel
               between those to be visited points, such that each point is
               visited at least once. The source code for the algorithmic level
               originates from
```

#### html2text {}

```diff
@@ -40,18 +40,14 @@
                                         multi-controlled Toffoli gate over all
                                         input qubits. In this no ancilla
                                         version, no ancilla qubits are used
                                         during its realization.
                                         Similar to the algorithm above with the
 Grover's (v-chain)                      difference, that the ancillary mode is
                                         a v-chain in this algorithm.
-                                        The Harrow-Hassadim-Lloyd algorithm is
-HHL                                     used to solve linear system of
-                                        equations. Here, we use a specific
-                                        system of equations.
                                         This algorithms solves the mean-
                                         variance portfolio optimization problem
 Portfolio Optimization with QAOA        for different assets. In this case, a
                                         QAOA algorithm instance is used. The
                                         source code for the algorithmic level
                                         originates from this_page.
                                         This algorithm estimates the fair price
@@ -73,19 +69,17 @@
                                         QFT embodies the quantum equivalent of
 Quantum Fourier Transformation (QFT)    the discrete Fourier transform and is a
                                         very important building block in many
                                         quantum algorithms.
 Entangled QFT                           Applies regular QFT to entangled
                                         qubits.
                                         This algorithm class is the quantum
-                                        equivalent to classical GAN and learns
-Quantum Generative Adversarial Network  the underlying distribution of input
-(QGAN)                                  data. The source code for the
-                                        algorithmic level originates from this
-                                        page.
+Quantum Neural Network (QNN)            equivalent to classical Neural Network.
+                                        The source code for the algorithmic
+                                        level originates from this_page.
                                         QPE estimates the phase of a quantum
                                         operation and is a very important
 Quantum Phase Estimation (QPE) exact    building block in many quantum
                                         algorithms. In the exact case, the
                                         applied phase is exactly representable
                                         by the number of qubits.
                                         Similar to QPE exact with the
@@ -95,14 +89,18 @@
                                         Quantum walks are the quantum
 Quantum Walk (no ancilla)               equivalent to classical random walks.
                                         In this no ancilla version, no ancilla
                                         qubits are used during its realization.
                                         Similar to the algorithm above with the
 Quantum Walk (v-chain)                  difference, that the ancillary mode is
                                         a v-chain in this algorithm.
+                                        This benchmark represents a random
+Random Circuit                          circuit which is twice as deep as wide.
+                                        It considers random quantum gates with
+                                        up to four qubits.
                                         This problem is similar to the
                                         travelling salesman problem with the
                                         difference, that more than one vehicle
 Routing                                 may be used to travel between those to
                                         be visited points, such that each point
                                         is visited at least once. The source
                                         code for the algorithmic level
```

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/templates/description.html` & `mqt.bench-1.0.0/src/mqt/benchviewer/templates/description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/templates/index.html` & `mqt.bench-1.0.0/src/mqt/benchviewer/templates/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         benchmarks in order for new software tools or design automation methods
         to be empirically evaluated and compared to the current state of the
         art. Since these tools and methods operate on and across different
         levels of abstraction, it is beneficial having benchmarks consistently
         available across those levels. The MQT Benchmark Library (MQT Bench)
         provides a single benchmark suite which offers the same benchmark
         algorithms on different levels of abstractions. At the moment, MQT Bench
-        comprises around 50,000 benchmark circuits ranging from 2 up to 130
+        comprises around 70,000 benchmark circuits ranging from 2 up to 130
         qubits on four abstraction levels.
       </p>
 
       <p>
         In order to create a benchmark set according to your needs, simply fill
         out the form below.
       </p>
@@ -272,46 +272,64 @@
             <h6>Target-dependent Native Gates Level</h6>
 
             <p class="text-justify" style="margin: 0px">
               Select targeted native gate-set:
             </p>
             <div class="row">
               <div class="col-md-12 align-items-center">
-                <input
-                  class="form-check-input"
-                  type="checkbox"
-                  value="true"
-                  id="nativegates_ibm"
-                  name="nativegates_ibm"
-                />
-                <label for="nativegates_ibm">IBM</label>
-                <input
-                  class="form-check-input"
-                  type="checkbox"
-                  value="true"
-                  id="nativegates_rigetti"
-                  name="nativegates_rigetti"
-                />
-                <label for="nativegates_rigetti">Rigetti</label>
-                <input
-                  class="form-check-input"
-                  type="checkbox"
-                  value="true"
-                  id="nativegates_oqc"
-                  name="nativegates_oqc"
-                />
-                <label for="nativegates_oqc">OQC</label>
-                <input
-                  class="form-check-input"
-                  type="checkbox"
-                  value="true"
-                  id="nativegates_ionq"
-                  name="nativegates_ionq"
-                />
-                <label for="nativegates_ionq">IonQ</label>
+                <div class="form-group">
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    value="true"
+                    id="nativegates_ibm"
+                    name="nativegates_ibm"
+                  />
+                  <label for="nativegates_ibm">IBM</label>
+                </div>
+                <div class="form-group">
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    value="true"
+                    id="nativegates_rigetti"
+                    name="nativegates_rigetti"
+                  />
+                  <label for="nativegates_rigetti">Rigetti</label>
+                </div>
+                <div class="form-group">
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    value="true"
+                    id="nativegates_oqc"
+                    name="nativegates_oqc"
+                  />
+                  <label for="nativegates_oqc">OQC</label>
+                </div>
+                <div class="form-group">
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    value="true"
+                    id="nativegates_ionq"
+                    name="nativegates_ionq"
+                  />
+                  <label for="nativegates_ionq">IonQ</label>
+                </div>
+                <div class="form-group">
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    value="true"
+                    id="nativegates_quantinuum"
+                    name="nativegates_quantinuum"
+                  />
+                  <label for="nativegates_quantinuum">Quantinuum</label>
+                </div>
               </div>
             </div>
             <p class="text-justify" style="margin: 0px; margin-top: 15px">
               Select the used compiler:
             </p>
 
             <div class="d-flex">
@@ -438,22 +456,46 @@
                   />
                   <label for="device_oqc_lucy">OQC Lucy (8 Qubits) </label>
                 </div>
                 <div>
                   <input
                     class="form-check-input"
                     type="checkbox"
-                    id="device_ionq_ionq11"
+                    id="device_ionq_harmony"
                     value="true"
-                    name="device_ionq_ionq11"
+                    name="device_ionq_harmony"
                   />
-                  <label for="device_ionq_ionq11"
+                  <label for="device_ionq_harmony"
                     >IonQ Harmony (11 Qubits)
                   </label>
                 </div>
+                <div>
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    id="device_ionq_aria1"
+                    value="true"
+                    name="device_ionq_aria1"
+                  />
+                  <label for="device_ionq_aria1"
+                    >IonQ Aria 1 (25 Qubits)
+                  </label>
+                </div>
+                <div>
+                  <input
+                    class="form-check-input"
+                    type="checkbox"
+                    id="device_quantinuum_h2"
+                    value="true"
+                    name="device_quantinuum_h2"
+                  />
+                  <label for="device_quantinuum_h2"
+                    >Quantinuum H2 (32 Qubits)
+                  </label>
+                </div>
               </div>
             </div>
             <p class="text-justify" style="margin: 0px; margin-top: 15px">
               Select the used compiler:
             </p>
             <div class="d-flex">
               <div class="col-md-6 align-items-center">
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 quantum applications. This requires practical and relevant benchmarks in order
 for new software tools or design automation methods to be empirically evaluated
 and compared to the current state of the art. Since these tools and methods
 operate on and across different levels of abstraction, it is beneficial having
 benchmarks consistently available across those levels. The MQT Benchmark
 Library (MQT Bench) provides a single benchmark suite which offers the same
 benchmark algorithms on different levels of abstractions. At the moment, MQT
-Bench comprises around 50,000 benchmark circuits ranging from 2 up to 130
+Bench comprises around 70,000 benchmark circuits ranging from 2 up to 130
 qubits on four abstraction levels.
 In order to create a benchmark set according to your needs, simply fill out the
 form below.
 *** Benchmark Selection ***
 Please select the desired benchmarks from the set of all available ones or
 select all (⁰). For details, see the benchmark_description.
 * Scalable Benchmarks: *
@@ -48,27 +48,33 @@
 GitHub_page.
 * Target-independent Level *
 Select the used compiler:
 ⁰ Qiskit
 ⁰ TKET
 * Target-dependent Native Gates Level *
 Select targeted native gate-set:
-⁰ IBM ⁰ Rigetti ⁰ OQC ⁰ IonQ
+⁰ IBM
+⁰ Rigetti
+⁰ OQC
+⁰ IonQ
+⁰ Quantinuum
 Select the used compiler:
 ⁰ Qiskit
 ⁰ TKET
 If Qiskit is selected, select its optimization level:
 ⁰ Opt. 0 ⁰ Opt. 1 ⁰ Opt. 2 ⁰ Opt. 3
 * Target-dependent Mapped Level *
 Select a targeted device:
 ⁰ IBM Washington (127 Qubits)
 ⁰ IBM Montreal (27 Qubits)
 ⁰ Rigetti Aspen-M2 (80 Qubits)
 ⁰ OQC Lucy (8 Qubits)
 ⁰ IonQ Harmony (11 Qubits)
+⁰ IonQ Aria 1 (25 Qubits)
+⁰ Quantinuum H2 (32 Qubits)
 Select the used compiler:
 ⁰ Qiskit
 ⁰ TKET
 If Qiskit is selected, select its optimization level:
 ⁰ Opt. 0 ⁰ Opt. 1 ⁰ Opt. 2 ⁰ Opt. 3
 If TKET is selected, select its placement settings:
 ⁰ Graph Placement  ⁰ Line Placement
```

### Comparing `mqt.bench-0.4.4/src/mqt/benchviewer/templates/legal.html` & `mqt.bench-1.0.0/src/mqt/benchviewer/templates/legal.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.4/src/mqt.bench.egg-info/PKG-INFO` & `mqt.bench-1.0.0/src/mqt.bench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 0.4.4
+Version: 1.0.0
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)](https://pypi.org/project/mqt.bench/)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/coverage.yml?branch=main&style=flat-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/actions/workflows/coverage.yml)
 [![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/workflows/deploy.yml)
-[![codecov](https://img.shields.io/codecov/c/github/cda-tum/MQTBench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/MQTBench)
+[![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-bench)
 
 <p align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqtbench/main/img/mqt_light.png" width="60%">
   <img src="https://raw.githubusercontent.com/cda-tum/mqtbench/main/img/mqt_dark.png" width="60%">
 </picture>
 </p>
@@ -137,26 +137,26 @@
 - Amplitude Estimation
 - Deutsch-Jozsa
 - GHZ State
 - Graph State
 - Ground State
 - Grover's (no ancilla)
 - Grover's (v-chain)
-- HHL
 - Portfolio Optimization with QAOA
 - Portfolio Optimization with VQE
 - Pricing Call Option
 - Pricing Put Option
 - Quantum Fourier Transformation (QFT)
 - QFT Entangled
-- Quantum Generative Adversarial Network (QGAN)
+- Quantum Neural Network (QNN)
 - Quantum Phase Estimation (QPE) Exact
 - Quantum Phase Estimation (QPE) Inexact
 - Quantum Walk (no ancilla)
 - Quantum Walk (-chain)
+- Random Circuit
 - Routing
 - Shor's
 - Travelling Salesman
 - Variational Quantum Eigensolver (VQE)
 - VQE-ansätze with random values:
   - Efficient SU2 ansatz with Random Parameters
   - Real Amplitudes ansatz with Random Parameters
@@ -176,24 +176,27 @@
 
 So far, MQT Bench supports the following native gate-sets:
 
 1. IBMQ gate-set: _\['rz', 'sx', 'x', 'cx', 'measure'\]_
 2. Rigetti gate-set: _\['rx', 'rz', 'cz', 'measure'\]_
 3. IonQ gate-set: _\['rxx', 'rz', 'ry', 'rx', 'measure'\]_
 4. OQC gate-set: _\['rz', 'sx', 'x', 'ecr', 'measure'\]_
+5. Quantinuum gate-set: _\['rzz', 'rz', 'ry', 'rx', 'measure'\]_
 
 ## Device Support
 
 So far, MQT Bench supports the following devices:
 
 1. IBMQ Washington with 127 qubits
 2. IBMQ Montreal with 27 qubits
 3. Rigetti Aspen-M2 with 80 qubits
-4. IonQ with 11 qubits
-5. OQC Lucy with 8 qubits
+4. IonQ Harmony with 11 qubits
+5. IonQ Aria 1 with 25 qubits
+6. OQC Lucy with 8 qubits
+7. Quantinuum H2 with 32 qubits
 
 # Repository Structure
 
 - src/mqt/: main source directory
   - bench: Directory for the MQT Bench package
   - bench/benchmarks: Directory for the benchmarks
   - benchviewer: Directory for the webpage (which can be started locally and is also hosted at
@@ -232,17 +235,17 @@
     device_name: str = "ibm_washington",
 ):
 ```
 
 The available parameters are:
 
 - `benchmark_name`: `"ae"`, `"dj"`, `"grover-noancilla"`, `"grover-v-chain"`, `"ghz"`, `"graphstate"`, `"portfolioqaoa"`,
-  `"portfoliovqe"`, `"qaoa"`, `"qft"`, `"qftentangled"`, `"qgan"`, `"qpeexact"`, `"qpeinexact"`,
-  `"qwalk-noancilla"`, `"qwalk-v-chain"`, `"realamprandom"`, `"su2random"`, `"twolocalrandom"`, `"vqe"`,
-  `"wstate"`, `"shor"`, `"hhl"`, `"pricingcall"`, `"pricingput"`, `"groundstate"`, `"routing"`,
+  `"portfoliovqe"`, `"qaoa"`, `"qft"`, `"qftentangled"`, `"qnn"`, `"qpeexact"`, `"qpeinexact"`,
+  `"qwalk-noancilla"`, `"qwalk-v-chain"`, `"random"`, `"realamprandom"`, `"su2random"`, `"twolocalrandom"`, `"vqe"`,
+  `"wstate"`, `"shor"`, `"pricingcall"`, `"pricingput"`, `"groundstate"`, `"routing"`,
   `"tsp"`
 - `level`: `0` or `"alg"`, `1` or `"indep"`, `2` or `"nativegates"`, `3` or `"mapped"`
 - `circuit_size`: for most of the cases this is equal to number of qubits
   (all scalable benchmarks except `"qwalk-v-chain"` and `"grover-v-chain"`) while for all other the qubit number is higher
 - `compiler`: `"qiskit"` or `"tket"`
 - `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
 
@@ -251,16 +254,16 @@
 
 compiler_settings = CompilerSettings(
     qiskit={"optimization_level": 1},
     tket={"placement": "lineplacement"},
 )
 ```
 
-- `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, or `"oqc"`
-- `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"aspen_m1"`, `"ionq11"`, `"lucy"`
+- `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, `"oqc"`, or `"quantinuum"`
+- `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"rigetti_aspen_m2"`, `"ionq_harmony"`, `"ionq_aria1"`, `"oqc_lucy"`, or `"quantinuum_h2"`
 
 Hereby, the mappings between shortened `benchmark_name` and actual benchmarks are:
 
 | `benchmark_name`     | Actual Benchmark                                    |
 | -------------------- | --------------------------------------------------- |
 | `"ae"`               | Amplitude Estimation (AE)                           |
 | `"dj"`               | Deutsch-Jozsa                                       |
@@ -269,26 +272,26 @@
 | `"ghz"`              | GHZ State                                           |
 | `"graphstate"`       | Graph State                                         |
 | `"portfolioqaoa"`    | Portfolio Optimization with QAOA                    |
 | `"portfoliovqe"`     | Portfolio Optimization with VQE                     |
 | `"qaoa"`             | Quantum Approximation Optimization Algorithm (QAOA) |
 | `"qft"`              | Quantum Fourier Transformation (QFT)                |
 | `"qftentangled"`     | QFT Entangled                                       |
-| `"qgan"`             | Quantum Generative Adversarial Network              |
+| `"qnn"`              | Quantum Neural Network (QNN)                        |
 | `"qpeexact"`         | Quantum Phase Estimation (QPE) exact                |
 | `"qpeinexact"`       | Quantum Phase Estimation (QPE) inexact              |
 | `"qwalk-noancilla"`  | Quantum Walk (no ancilla)                           |
 | `"qwalk-v-chain"`    | Quantum Walk (v-chain)                              |
+| `"random"`           | Random Quantum Circuit                              |
 | `"realamprandom"`    | Real Amplitudes ansatz with Random Parameters       |
 | `"su2random"`        | Efficient SU2 ansatz with Random Parameters         |
 | `"twolocalrandom"`   | Two Local ansatz with Random Parameters             |
 | `"vqe"`              | Variational Quantum Eigensolver (VQE)               |
 | `"wstate"`           | W-State                                             |
 | `"shor"`             | Shor's                                              |
-| `"hhl"`              | HHL                                                 |
 | `"pricingcall"`      | Pricing Call Option                                 |
 | `"pricingput"`       | Pricing Put Option                                  |
 | `"groundstate"`      | Ground State                                        |
 | `"routing"`          | Routing                                             |
 | `"tsp"`              | Travelling Salesman                                 |
 
 For example, in order to obtain the _5_-qubit Deutsch-Josza benchmark on algorithm level, use the following:
```

### Comparing `mqt.bench-0.4.4/src/mqt.bench.egg-info/SOURCES.txt` & `mqt.bench-1.0.0/src/mqt.bench.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,37 +38,38 @@
 src/mqt/bench/utils.py
 src/mqt/bench/benchmarks/__init__.py
 src/mqt/bench/benchmarks/ae.py
 src/mqt/bench/benchmarks/dj.py
 src/mqt/bench/benchmarks/ghz.py
 src/mqt/bench/benchmarks/graphstate.py
 src/mqt/bench/benchmarks/grover.py
-src/mqt/bench/benchmarks/hhl.py
 src/mqt/bench/benchmarks/qaoa.py
 src/mqt/bench/benchmarks/qft.py
 src/mqt/bench/benchmarks/qftentangled.py
 src/mqt/bench/benchmarks/qpeexact.py
 src/mqt/bench/benchmarks/qpeinexact.py
 src/mqt/bench/benchmarks/qwalk.py
+src/mqt/bench/benchmarks/random.py
 src/mqt/bench/benchmarks/realamprandom.py
 src/mqt/bench/benchmarks/shor.py
 src/mqt/bench/benchmarks/su2random.py
 src/mqt/bench/benchmarks/twolocalrandom.py
 src/mqt/bench/benchmarks/vqe.py
 src/mqt/bench/benchmarks/wstate.py
 src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
 src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
 src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
 src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-src/mqt/bench/benchmarks/qiskit_application_ml/qgan.py
+src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
 src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
 src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
 src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
 src/mqt/bench/evaluation/__init__.py
 src/mqt/bench/evaluation/evaluation.py
+src/mqt/bench/evaluation/evaluation_data.pkl
 src/mqt/bench/evaluation/evaluation_visualization.ipynb
 src/mqt/bench/evaluation/results/pie.pdf
 src/mqt/bench/evaluation/results/qubit_dist.pdf
 src/mqt/bench/evaluation/results/violins.pdf
 src/mqt/benchviewer/__init__.py
 src/mqt/benchviewer/backend.py
 src/mqt/benchviewer/main.py
```

### Comparing `mqt.bench-0.4.4/tests/test_bench.py` & `mqt.bench-1.0.0/tests/test_bench.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 from mqt.bench.benchmarks import (
     ae,
     dj,
     ghz,
     graphstate,
     groundstate,
     grover,
-    hhl,
     portfolioqaoa,
     portfoliovqe,
     pricingcall,
     pricingput,
     qaoa,
     qft,
     qftentangled,
-    qgan,
+    qnn,
     qpeexact,
     qpeinexact,
     qwalk,
+    random,
     realamprandom,
     routing,
     shor,
     su2random,
     tsp,
     twolocalrandom,
     vqe,
@@ -67,46 +67,48 @@
         "ae_indep_tket_93.qasm",
         "wstate_nativegates_rigetti_qiskit_opt0_79.qasm",
         "ae_mapped_ibm_montreal_qiskit_opt1_9.qasm",
         "ae_mapped_ibm_washington_qiskit_opt0_38.qasm",
         "ae_mapped_oqc_lucy_qiskit_opt0_5.qasm",
         "ae_mapped_rigetti_aspen_m2_qiskit_opt1_61.qasm",
         "ae_mapped_ibm_washington_qiskit_opt2_88.qasm",
-        "qgan_mapped_ionq11_qiskit_opt3_3.qasm",
-        "qgan_mapped_oqc_lucy_tket_line_2.qasm",
+        "qnn_mapped_ionq_harmony_qiskit_opt3_3.qasm",
+        "qnn_mapped_oqc_lucy_tket_line_2.qasm",
+        "qaoa_mapped_quantinuum_h2_tket_graph_2.qasm",
+        "dj_mapped_quantinuum_h2_qiskit_opt3_23.qasm",
     ]
 
 
 @pytest.mark.parametrize(
     ("benchmark", "input_value", "scalable"),
     [
         (ae, 8, True),
         (ghz, 5, True),
         (dj, 3, True),
         (graphstate, 8, True),
         (grover, 5, False),
-        (hhl, 2, False),
         (qaoa, 5, True),
         (qft, 8, True),
         (qftentangled, 8, True),
+        (qnn, 8, True),
         (qpeexact, 8, True),
         (qpeinexact, 8, True),
         (tsp, 3, False),
         (qwalk, 5, False),
         (vqe, 5, True),
+        (random, 9, True),
         (realamprandom, 9, True),
         (su2random, 7, True),
         (twolocalrandom, 8, True),
         (wstate, 8, True),
         (portfolioqaoa, 5, True),
         (shor, 9, False),
         (portfoliovqe, 5, True),
         (pricingcall, 5, False),
         (pricingput, 5, False),
-        (qgan, 5, True),
     ],
 )
 def test_quantumcircuit_indep_level(
     benchmark: types.ModuleType, input_value: int, scalable: bool, output_path: str
 ) -> None:
     if benchmark in (grover, qwalk):
         qc = benchmark.create_circuit(input_value, ancillary_mode="noancilla")
@@ -157,46 +159,43 @@
         (ghz, 5, True),
         (dj, 3, True),
         (graphstate, 8, True),
         (grover, 5, False),
         (qaoa, 5, True),
         (qft, 8, True),
         (qftentangled, 8, True),
+        (qnn, 5, True),
         (qpeexact, 8, True),
         (qpeinexact, 8, True),
         (tsp, 3, False),
         (qwalk, 5, False),
         (vqe, 5, True),
+        (random, 9, True),
         (realamprandom, 3, True),
         (su2random, 7, True),
         (twolocalrandom, 5, True),
         (wstate, 8, True),
         (portfolioqaoa, 5, True),
         (portfoliovqe, 5, True),
         (pricingcall, 5, False),
         (pricingput, 5, False),
-        (qgan, 5, True),
     ],
 )
 def test_quantumcircuit_native_and_mapped_levels(
     benchmark: types.ModuleType, input_value: int, scalable: bool, output_path: str
 ) -> None:
     if benchmark in (grover, qwalk):
         qc = benchmark.create_circuit(input_value, ancillary_mode="noancilla")
     else:
         qc = benchmark.create_circuit(input_value)
     if scalable:
         assert qc.num_qubits == input_value
 
-    compilation_paths = [
-        ("ibm", [("ibm_washington", 127), ("ibm_montreal", 27)]),
-        ("rigetti", [("rigetti_aspen_m2", 80)]),
-        ("ionq", [("ionq11", 11)]),
-        ("oqc", [("oqc_lucy", 8)]),
-    ]
+    compilation_paths = utils.get_compilation_paths()
+
     for gate_set_name, devices in compilation_paths:
         opt_level = 1
         res = qiskit_helper.get_native_gates_level(
             qc,
             gate_set_name,
             qc.num_qubits,
             opt_level,
@@ -211,40 +210,40 @@
             qc.num_qubits,
             opt_level,
             file_precheck=True,
             return_qc=False,
             target_directory=output_path,
         )
         assert res
-        if gate_set_name != "ionq":
-            for device_name, max_qubits in devices:
-                # Creating the circuit on target-dependent: mapped level qiskit
-                if max_qubits >= qc.num_qubits:
-                    res = qiskit_helper.get_mapped_level(
-                        qc,
-                        gate_set_name,
-                        qc.num_qubits,
-                        device_name,
-                        opt_level,
-                        file_precheck=False,
-                        return_qc=False,
-                        target_directory=output_path,
-                    )
-                    assert res
-                    res = qiskit_helper.get_mapped_level(
-                        qc,
-                        gate_set_name,
-                        qc.num_qubits,
-                        device_name,
-                        opt_level,
-                        file_precheck=True,
-                        return_qc=False,
-                        target_directory=output_path,
-                    )
-                    assert res
+
+        for device_name, max_qubits in devices:
+            # Creating the circuit on target-dependent: mapped level qiskit
+            if max_qubits >= qc.num_qubits:
+                res = qiskit_helper.get_mapped_level(
+                    qc,
+                    gate_set_name,
+                    qc.num_qubits,
+                    device_name,
+                    opt_level,
+                    file_precheck=False,
+                    return_qc=False,
+                    target_directory=output_path,
+                )
+                assert res
+                res = qiskit_helper.get_mapped_level(
+                    qc,
+                    gate_set_name,
+                    qc.num_qubits,
+                    device_name,
+                    opt_level,
+                    file_precheck=True,
+                    return_qc=False,
+                    target_directory=output_path,
+                )
+                assert res
 
     for gate_set_name, devices in compilation_paths:
         res = tket_helper.get_native_gates_level(
             qc,
             gate_set_name,
             qc.num_qubits,
             file_precheck=False,
@@ -257,40 +256,39 @@
             gate_set_name,
             qc.num_qubits,
             file_precheck=True,
             return_qc=False,
             target_directory=output_path,
         )
         assert res
-        if gate_set_name != "ionq":
-            for device_name, max_qubits in devices:
-                # Creating the circuit on target-dependent: mapped level qiskit
-                if max_qubits >= qc.num_qubits:
-                    res = tket_helper.get_mapped_level(
-                        qc,
-                        gate_set_name,
-                        qc.num_qubits,
-                        device_name,
-                        True,
-                        file_precheck=False,
-                        return_qc=False,
-                        target_directory=output_path,
-                    )
-                    assert res
-                    res = tket_helper.get_mapped_level(
-                        qc,
-                        gate_set_name,
-                        qc.num_qubits,
-                        device_name,
-                        False,
-                        file_precheck=True,
-                        return_qc=False,
-                        target_directory=output_path,
-                    )
-                    assert res
+        for device_name, max_qubits in devices:
+            # Creating the circuit on target-dependent: mapped level qiskit
+            if max_qubits >= qc.num_qubits:
+                res = tket_helper.get_mapped_level(
+                    qc,
+                    gate_set_name,
+                    qc.num_qubits,
+                    device_name,
+                    True,
+                    file_precheck=False,
+                    return_qc=False,
+                    target_directory=output_path,
+                )
+                assert res
+                res = tket_helper.get_mapped_level(
+                    qc,
+                    gate_set_name,
+                    qc.num_qubits,
+                    device_name,
+                    False,
+                    file_precheck=True,
+                    return_qc=False,
+                    target_directory=output_path,
+                )
+                assert res
 
 
 def test_openqasm_gates() -> None:
     openqasm_gates = utils.get_openqasm_gates()
     num_openqasm_gates = 42
     assert len(openqasm_gates) == num_openqasm_gates
 
@@ -517,15 +515,35 @@
             "qpeexact",
             "mapped",
             5,
             None,
             "qiskit",
             CompilerSettings(qiskit=QiskitSettings(optimization_level=1)),
             "ionq",
-            "ionq11",
+            "ionq_harmony",
+        ),
+        (
+            "qpeexact",
+            "mapped",
+            5,
+            None,
+            "qiskit",
+            CompilerSettings(qiskit=QiskitSettings(optimization_level=1)),
+            "ionq",
+            "ionq_aria1",
+        ),
+        (
+            "qpeexact",
+            "mapped",
+            5,
+            None,
+            "qiskit",
+            CompilerSettings(qiskit=QiskitSettings(optimization_level=2)),
+            "ionq",
+            "ionq_aria1",
         ),
         (
             "qpeexact",
             "mapped",
             5,
             None,
             "qiskit",
@@ -609,14 +627,34 @@
             4,
             None,
             "tket",
             CompilerSettings(tket=TKETSettings(placement="graphplacement")),
             "oqc",
             "oqc_lucy",
         ),
+        (
+            "qpeinexact",
+            3,
+            4,
+            None,
+            "tket",
+            CompilerSettings(tket=TKETSettings(placement="graphplacement")),
+            "quantinuum",
+            "quantinuum_h2",
+        ),
+        (
+            "qpeinexact",
+            3,
+            4,
+            None,
+            "qiskit",
+            CompilerSettings(qiskit=QiskitSettings(optimization_level=2)),
+            "quantinuum",
+            "quantinuum_h2",
+        ),
     ],
 )
 def test_get_benchmark(
     benchmark_name: str,
     level: str | int,
     circuit_size: int,
     benchmark_instance_name: str | None,
@@ -831,55 +869,64 @@
         "oqc",
         qc.num_qubits,
         file_precheck=False,
         return_qc=False,
         target_directory=directory,
         target_filename=filename,
     )
+
     assert QuantumCircuit.from_qasm_file(str(path))
     path.unlink()
 
+    directory = "."
+    filename = "ghz_oqc2"
+    path = Path(directory) / Path(filename).with_suffix(".qasm")
     tket_helper.get_mapped_level(
         qc,
         "oqc",
         qc.num_qubits,
         "oqc_lucy",
         lineplacement=False,
         file_precheck=False,
         return_qc=False,
         target_directory=directory,
         target_filename=filename,
     )
     assert QuantumCircuit.from_qasm_file(str(path))
     path.unlink()
-
+    directory = "."
+    filename = "ghz_oqc3"
+    path = Path(directory) / Path(filename).with_suffix(".qasm")
     qiskit_helper.get_native_gates_level(
         qc,
         "oqc",
         qc.num_qubits,
         opt_level=1,
         file_precheck=False,
         return_qc=False,
         target_directory=directory,
         target_filename=filename,
     )
     assert QuantumCircuit.from_qasm_file(str(path))
     path.unlink()
-
+    directory = "."
+    filename = "ghz_oqc4"
+    path = Path(directory) / Path(filename).with_suffix(".qasm")
     qiskit_helper.get_mapped_level(
         qc,
         "oqc",
         qc.num_qubits,
         "oqc_lucy",
         opt_level=1,
         file_precheck=False,
         return_qc=False,
         target_directory=directory,
         target_filename=filename,
     )
+
     assert QuantumCircuit.from_qasm_file(str(path))
     path.unlink()
 
 
 def test_evaluate_qasm_file() -> None:
     qc = get_benchmark("dj", 1, 5)
     filename = "test_5.qasm"
@@ -890,35 +937,35 @@
 
     path.unlink()
 
 
 @pytest.mark.parametrize(
     ("search_str", "expected_val"),
     [
-        ("qiskit", 9),
-        ("tket", 2),
+        ("qiskit", 10),
+        ("tket", 3),
         ("nativegates", 2),
         ("indep", 2),
-        ("mapped", 7),
+        ("mapped", 9),
         ("mapped_ibm_washington", 2),
         ("mapped_ibm_montreal", 1),
         ("mapped_oqc_lucy", 2),
         ("mapped_rigetti_aspen_m2", 1),
-        ("mapped_ionq11", 1),
+        ("mapped_ionq_harmony", 1),
     ],
 )
 def test_count_occurrences(search_str: str, expected_val: int, sample_filenames: list[str]) -> None:
     assert evaluation.count_occurrences(sample_filenames, search_str) == expected_val
 
 
 @pytest.mark.parametrize(
     ("compiler", "expected_val"),
     [
-        ("qiskit", [10, 54, 79, 9, 38, 5, 61, 88, 3]),
-        ("tket", [93, 2]),
+        ("qiskit", [10, 54, 79, 9, 38, 5, 61, 88, 3, 23]),
+        ("tket", [93, 2, 2]),
     ],
 )
 def test_count_qubit_numbers_per_compiler(compiler: str, expected_val: list[int], sample_filenames: list[str]) -> None:
     assert evaluation.count_qubit_numbers_per_compiler(sample_filenames, compiler) == expected_val
 
 
 def test_calc_supermarq_features() -> None:
@@ -931,29 +978,29 @@
     generator = BenchmarkGenerator(qasm_output_path="test")
     assert generator.qasm_output_path == "test"
     assert generator.timeout > 0
     assert generator.cfg is not None
 
 
 # This function is used to test the timeout watchers and needs two parameters since those values are logged when a timeout occurs.
-def endless_loop(arg1: TestObject, run_forever: bool) -> bool:  # noqa: ARG001
+def endless_loop(arg1: SampleObject, run_forever: bool) -> bool:  # noqa: ARG001
     while run_forever:
         pass
     return True
 
 
-class TestObject:
+class SampleObject:
     def __init__(self, name: str):
         self.name = name
 
 
 def test_timeout_watchers() -> None:
     timeout = 1
-    assert not timeout_watcher(endless_loop, timeout, [TestObject("test"), True])
-    assert timeout_watcher(endless_loop, timeout, [TestObject("test"), False])
+    assert not timeout_watcher(endless_loop, timeout, [SampleObject("test"), True])
+    assert timeout_watcher(endless_loop, timeout, [SampleObject("test"), False])
 
 
 def test_get_module_for_benchmark() -> None:
     for benchmark in utils.get_supported_benchmarks():
         assert utils.get_module_for_benchmark(benchmark.split("-")[0]) is not None
```

### Comparing `mqt.bench-0.4.4/tests/test_benchviewer.py` & `mqt.bench-1.0.0/tests/test_benchviewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 @pytest.mark.parametrize(
     ("filename", "expected_res"),
     [
         ("shor_15_4_nativegates_rigetti_qiskit_opt0_18.qasm", 0),
         ("dj_mapped_ibm_washington_qiskit_opt3_103.qasm", 3),
         ("graphstate_nativegates_ibm_qiskit_opt2_15.qasm", 2),
         ("grover-noancilla_nativegates_ibm_qiskit_opt1_8.qasm", 1),
-        ("HHL_indep_5.qasm", -1),
+        ("random_indep_5.qasm", -1),
     ],
 )
 def test_get_opt_level(filename: str, expected_res: int) -> None:
     assert int(backend.get_opt_level(filename)) == expected_res
 
 
 @pytest.mark.parametrize(
     ("filename", "expected_res"),
     [
         ("shor_15_4_nativegates_rigetti_qiskit_opt0_18.qasm", 18),
         ("dj_mapped_ibm_washington_qiskit_opt3_103.qasm", 103),
         ("graphstate_nativegates_ibm_qiskit_opt2_15.qasm", 15),
         ("grover-noancilla_nativegates_ibm_qiskit_opt1_8.qasm", 8),
-        ("HHL_indep_5.qasm", 5),
+        ("random_indep_5.qasm", 5),
     ],
 )
 def test_get_num_qubits(filename: str, expected_res: int) -> None:
     assert int(backend.get_num_qubits(filename)) == expected_res
 
 
 @pytest.mark.parametrize(
@@ -101,26 +101,26 @@
                 compiler_settings=1,
                 gate_set="ionq",
                 target_device=None,
                 filename="portfoliovqe_nativegates_ionq_qiskit_opt1_3.qasm",
             ),
         ),
         (
-            "HHL_indep_qiskit_5.qasm",
+            "random_indep_qiskit_5.qasm",
             backend.ParsedBenchmarkName(
-                benchmark="hhl",
+                benchmark="random",
                 num_qubits=5,
                 indep_flag=True,
                 nativegates_flag=False,
                 mapped_flag=False,
                 compiler="qiskit",
                 compiler_settings=-1,
                 gate_set=None,
                 target_device=None,
-                filename="HHL_indep_qiskit_5.qasm",
+                filename="random_indep_qiskit_5.qasm",
             ),
         ),
     ],
 )
 def test_parse_data(filename: str, expected_res: backend.ParsedBenchmarkName) -> None:
     assert backend.parse_data(filename) == expected_res
 
@@ -137,26 +137,26 @@
         "selectBench_5": "Grover's (no ancilla)",
         "selectBench_6": "Grover's (v-chain)",
         "selectBench_7": "Portfolio Optimization with QAOA",
         "selectBench_8": "Portfolio Optimization with VQE",
         "selectBench_9": "Quantum Approximation Optimization Algorithm (QAOA)",
         "selectBench_10": "Quantum Fourier Transformation (QFT)",
         "selectBench_11": "QFT Entangled",
-        "selectBench_12": "Quantum Generative Adversarial Network",
+        "selectBench_12": "Quantum Neural Network (QNN)",
         "selectBench_13": "Quantum Phase Estimation (QPE) exact",
         "selectBench_14": "Quantum Phase Estimation (QPE) inexact",
         "selectBench_15": "Quantum Walk (no ancilla)",
         "selectBench_16": "Quantum Walk (v-chain)",
-        "selectBench_17": "Variational Quantum Eigensolver (VQE)",
-        "selectBench_18": "Efficient SU2 ansatz with Random Parameters",
-        "selectBench_19": "Real Amplitudes ansatz with Random Parameters",
-        "selectBench_20": "Two Local ansatz with Random Parameters",
-        "selectBench_21": "W-State",
-        "selectBench_22": "Ground State",
-        "selectBench_23": "HHL",
+        "selectBench_17": "Random Circuit",
+        "selectBench_18": "Variational Quantum Eigensolver (VQE)",
+        "selectBench_19": "Efficient SU2 ansatz with Random Parameters",
+        "selectBench_20": "Real Amplitudes ansatz with Random Parameters",
+        "selectBench_21": "Two Local ansatz with Random Parameters",
+        "selectBench_22": "W-State",
+        "selectBench_23": "Ground State",
         "selectBench_24": "Pricing Call Option",
         "selectBench_25": "Pricing Put Option",
         "selectBench_26": "Routing",
         "selectBench_27": "Shor's",
         "selectBench_28": "Travelling Salesman",
         "indep_qiskit_compiler": "true",
         "indep_tket_compiler": "true",
@@ -166,44 +166,55 @@
         "nativegates_qiskit_compiler_opt2": "true",
         "nativegates_qiskit_compiler_opt3": "true",
         "nativegates_tket_compiler value=": "on",
         "nativegates_ibm": "true",
         "nativegates_rigetti": "true",
         "nativegates_oqc": "true",
         "nativegates_ionq": "true",
+        "nativegates_quantinuum": "true",
         "mapped_qiskit_compiler": "true",
         "mapped_qiskit_compiler_opt0": "true",
         "mapped_qiskit_compiler_opt1": "true",
         "mapped_qiskit_compiler_opt2": "true",
         "mapped_qiskit_compiler_opt3": "true",
         "mapped_tket_compiler": "true",
         "mapped_tket_compiler_graph": "true",
         "mapped_tket_compiler_line": "true",
         "device_ibm_washington": "true",
         "device_ibm_montreal": "true",
         "device_rigetti_aspen_m2": "true",
         "device_oqc_lucy": "true",
-        "device_ionq_ionq11": "true",
+        "device_ionq_harmony": "true",
+        "device_ionq_aria1": "true",
+        "device_quantinuum_h2": "true",
     }
 
     expected_res = BenchmarkConfiguration(
         min_qubits=75,
         max_qubits=110,
         indices_benchmarks=list(range(1, 29)),
         indep_qiskit_compiler=True,
         indep_tket_compiler=True,
         nativegates_qiskit_compiler=True,
         native_qiskit_opt_lvls=[0, 1, 2, 3],
         nativegates_tket_compiler=True,
-        native_gatesets=["ibm", "rigetti", "oqc", "ionq"],
+        native_gatesets=["ibm", "rigetti", "oqc", "ionq", "quantinuum"],
         mapped_qiskit_compiler=True,
         mapped_qiskit_opt_lvls=[0, 1, 2, 3],
         mapped_tket_compiler=True,
         mapped_tket_placements=["graph", "line"],
-        mapped_devices=["ibm_washington", "ibm_montreal", "rigetti_aspen", "oqc_lucy", "ionq11"],
+        mapped_devices=[
+            "ibm_washington",
+            "ibm_montreal",
+            "rigetti_aspen_m2",
+            "oqc_lucy",
+            "ionq_harmony",
+            "ionq_aria1",
+            "quantinuum_h2",
+        ],
     )
     backend = Backend()
     assert backend.prepare_form_input(form_data) == expected_res
 
     form_data = {
         "all_benchmarks": "true",
         "minQubits": "75",
@@ -216,43 +227,54 @@
         "nativegates_qiskit_compiler_opt2": "true",
         "nativegates_qiskit_compiler_opt3": "true",
         "nativegates_tket_compiler value=": "on",
         "nativegates_ibm": "true",
         "nativegates_rigetti": "true",
         "nativegates_oqc": "true",
         "nativegates_ionq": "true",
+        "nativegates_quantinuum": "true",
         "mapped_qiskit_compiler": "true",
         "mapped_qiskit_compiler_opt0": "true",
         "mapped_qiskit_compiler_opt1": "true",
         "mapped_qiskit_compiler_opt2": "true",
         "mapped_qiskit_compiler_opt3": "true",
         "mapped_tket_compiler": "true",
         "mapped_tket_compiler_graph": "true",
         "mapped_tket_compiler_line": "true",
         "device_ibm_washington": "true",
         "device_ibm_montreal": "true",
         "device_rigetti_aspen_m2": "true",
         "device_oqc_lucy": "true",
-        "device_ionq_ionq11": "true",
+        "device_ionq_harmony": "true",
+        "device_ionq_aria1": "true",
+        "device_quantinuum_h2": "true",
     }
     expected_res = BenchmarkConfiguration(
         min_qubits=75,
         max_qubits=110,
         indices_benchmarks=[],
         indep_qiskit_compiler=True,
         indep_tket_compiler=True,
         nativegates_qiskit_compiler=True,
         native_qiskit_opt_lvls=[0, 1, 2, 3],
         nativegates_tket_compiler=True,
-        native_gatesets=["ibm", "rigetti", "oqc", "ionq"],
+        native_gatesets=["ibm", "rigetti", "oqc", "ionq", "quantinuum"],
         mapped_qiskit_compiler=True,
         mapped_qiskit_opt_lvls=[0, 1, 2, 3],
         mapped_tket_compiler=True,
         mapped_tket_placements=["graph", "line"],
-        mapped_devices=["ibm_washington", "ibm_montreal", "rigetti_aspen", "oqc_lucy", "ionq11"],
+        mapped_devices=[
+            "ibm_washington",
+            "ibm_montreal",
+            "rigetti_aspen_m2",
+            "oqc_lucy",
+            "ionq_harmony",
+            "ionq_aria1",
+            "quantinuum_h2",
+        ],
     )
     backend = Backend()
     assert backend.prepare_form_input(form_data) == expected_res
 
 
 benchviewer = resources.files("mqt.benchviewer")
 
@@ -331,16 +353,16 @@
         indices_benchmarks=[23],
         indep_qiskit_compiler=True,
         indep_tket_compiler=True,
         nativegates_qiskit_compiler=True,
         nativegates_tket_compiler=False,
         mapped_qiskit_compiler=True,
         mapped_tket_compiler=True,
-        native_gatesets=["rigetti", "ionq", "oqc", "ibm"],
-        mapped_devices=["ibm_montreal", "rigetti_aspen", "ionq11", "ocq_lucy"],
+        native_gatesets=["rigetti", "ionq", "oqc", "ibm", "quantinuum"],
+        mapped_devices=["ibm_montreal", "rigetti_aspen_m2", "ionq_harmony", "ionq_aria1", "ocq_lucy", "quantinuum_h2"],
         mapped_tket_placements=["graph", "line"],
         native_qiskit_opt_lvls=[0, 3],
         mapped_qiskit_opt_lvls=[0, 3],
     )
     res = backend.get_selected_file_paths(input_data)
     assert isinstance(res, list)
     assert len(res) > 20
```

