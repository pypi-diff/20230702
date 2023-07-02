# Comparing `tmp/cca_zoo-2.0.8.tar.gz` & `tmp/cca_zoo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cca_zoo-2.0.8.tar", max compression
+gzip compressed data, was "cca_zoo-2.1.0.tar", max compression
```

## Comparing `cca_zoo-2.0.8.tar` & `cca_zoo-2.1.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1069 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/LICENSE
--rw-r--r--   0        0        0     3999 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/README.md
--rw-r--r--   0        0        0      323 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/__init__.py
--rw-r--r--   0        0        0      127 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/data/__init__.py
--rw-r--r--   0        0        0     3176 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/data/deep.py
--rw-r--r--   0        0        0     7074 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/data/simulated.py
--rw-r--r--   0        0        0      598 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/__init__.py
--rw-r--r--   0        0        0     5356 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_base.py
--rw-r--r--   0        0        0      276 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0        0        0     1831 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0        0        0     2342 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0        0        0     2401 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0        0        0     1275 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0        0        0     2240 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0        0        0     2539 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0        0        0     1681 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0        0        0      676 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0        0        0      784 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dtcca.py
--rw-r--r--   0        0        0       82 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0        0        0     1449 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0        0        0     2481 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0        0        0     5339 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0        0        0     2051 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0        0        0     9528 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/architectures.py
--rw-r--r--   0        0        0      337 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/callbacks.py
--rw-r--r--   0        0        0     1931 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/metrics.py
--rw-r--r--   0        0        0     8808 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/deep/objectives.py
--rw-r--r--   0        0        0     1385 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/__init__.py
--rw-r--r--   0        0        0     7492 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_base.py
--rw-r--r--   0        0        0     1584 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_dummy.py
--rw-r--r--   0        0        0     3332 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gcca.py
--rw-r--r--   0        0        0      133 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/__init__.py
--rw-r--r--   0        0        0     8646 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_ey.py
--rw-r--r--   0        0        0     2223 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gh.py
--rw-r--r--   0        0        0     1757 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gradient.py
--rw-r--r--   0        0        0     1713 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_stochasticpls.py
--rw-r--r--   0        0        0     1738 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_gradient/_svd.py
--rw-r--r--   0        0        0     6599 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_grcca.py
--rw-r--r--   0        0        0      451 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/__init__.py
--rw-r--r--   0        0        0     7048 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_altmaxvar.py
--rw-r--r--   0        0        0    10968 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_base.py
--rw-r--r--   0        0        0     2459 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_deflation.py
--rw-r--r--   0        0        0    13982 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_elasticnet.py
--rw-r--r--   0        0        0     3789 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_incrementalpls.py
--rw-r--r--   0        0        0     3246 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_pls_als.py
--rw-r--r--   0        0        0     6728 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_admm.py
--rw-r--r--   0        0        0     4089 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_parkhomenko.py
--rw-r--r--   0        0        0     7166 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_pmd.py
--rw-r--r--   0        0        0     4460 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_span.py
--rw-r--r--   0        0        0     3813 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_iterative/_swcca.py
--rw-r--r--   0        0        0    10289 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_mcca.py
--rw-r--r--   0        0        0     3087 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_partialcca.py
--rw-r--r--   0        0        0     1621 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_pcacca.py
--rw-r--r--   0        0        0    11203 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_pls.py
--rw-r--r--   0        0        0     4214 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_prcca.py
--rw-r--r--   0        0        0     2341 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_search.py
--rw-r--r--   0        0        0     4710 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/linear/_tcca.py
--rw-r--r--   0        0        0      330 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/model_selection/__init__.py
--rw-r--r--   0        0        0    11669 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/model_selection/_search.py
--rw-r--r--   0        0        0    18413 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/model_selection/_validation.py
--rw-r--r--   0        0        0       62 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/nonparametric/__init__.py
--rw-r--r--   0        0        0     5066 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/nonparametric/_gradkcca.py
--rw-r--r--   0        0        0    12589 2023-06-30 02:09:47.786475 cca_zoo-2.0.8/cca_zoo/nonparametric/_kcca.py
--rw-r--r--   0        0        0     6385 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/nonparametric/_ncca.py
--rw-r--r--   0        0        0     6280 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/nonparametric/_scca_hsic.py
--rw-r--r--   0        0        0       80 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0        0        0     4502 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/probabilistic/_probabilisticcca.py
--rw-r--r--   0        0        0      129 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/utils/__init__.py
--rw-r--r--   0        0        0     1581 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/utils/check_values.py
--rw-r--r--   0        0        0      163 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/visualisation/__init__.py
--rw-r--r--   0        0        0     2292 2023-06-30 02:09:47.790475 cca_zoo-2.0.8/cca_zoo/visualisation/plotting.py
--rw-r--r--   0        0        0     1158 2023-06-30 02:09:48.110476 cca_zoo-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     5233 1970-01-01 00:00:00.000000 cca_zoo-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3999 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/README.md
+-rw-r--r--   0        0        0      325 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/__init__.py
+-rw-r--r--   0        0        0     7517 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/_base/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/data/__init__.py
+-rw-r--r--   0        0        0     3176 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/data/deep.py
+-rw-r--r--   0        0        0     7074 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/data/simulated.py
+-rw-r--r--   0        0        0      598 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/__init__.py
+-rw-r--r--   0        0        0     5270 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_base.py
+-rw-r--r--   0        0        0      426 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0        0        0     1777 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0        0        0     2342 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0        0        0     2401 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0        0        0     1275 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0        0        0     2240 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0        0        0     2539 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0        0        0     1681 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0        0        0      676 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0        0        0      784 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dtcca.py
+-rw-r--r--   0        0        0      123 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0        0        0     1449 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0        0        0     2481 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0        0        0     5339 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0        0        0     2051 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0        0        0     9528 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/architectures.py
+-rw-r--r--   0        0        0      337 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/callbacks.py
+-rw-r--r--   0        0        0     1931 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/metrics.py
+-rw-r--r--   0        0        0     8808 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/objectives.py
+-rw-r--r--   0        0        0      816 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/__init__.py
+-rw-r--r--   0        0        0     1577 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_dummy.py
+-rw-r--r--   0        0        0     3093 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gcca.py
+-rw-r--r--   0        0        0      241 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/__init__.py
+-rw-r--r--   0        0        0     8646 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_ey.py
+-rw-r--r--   0        0        0     2223 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gh.py
+-rw-r--r--   0        0        0     1757 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gradient.py
+-rw-r--r--   0        0        0     1713 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_stochasticpls.py
+-rw-r--r--   0        0        0     1738 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_svd.py
+-rw-r--r--   0        0        0     6599 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_grcca.py
+-rw-r--r--   0        0        0      364 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/__init__.py
+-rw-r--r--   0        0        0     7635 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_altmaxvar.py
+-rw-r--r--   0        0        0    12323 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_base.py
+-rw-r--r--   0        0        0     2459 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_deflation.py
+-rw-r--r--   0        0        0    13319 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_elasticnet.py
+-rw-r--r--   0        0        0     3789 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_incrementalpls.py
+-rw-r--r--   0        0        0     3261 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_pls_als.py
+-rw-r--r--   0        0        0     6728 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_admm.py
+-rw-r--r--   0        0        0     4181 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0        0        0     7258 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_pmd.py
+-rw-r--r--   0        0        0     4461 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_span.py
+-rw-r--r--   0        0        0     3813 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_swcca.py
+-rw-r--r--   0        0        0    10291 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_mcca.py
+-rw-r--r--   0        0        0     3086 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_partialcca.py
+-rw-r--r--   0        0        0     1621 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_pcacca.py
+-rw-r--r--   0        0        0    11322 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_pls.py
+-rw-r--r--   0        0        0     4216 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_prcca.py
+-rw-r--r--   0        0        0     2722 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_search.py
+-rw-r--r--   0        0        0     4716 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_tcca.py
+-rw-r--r--   0        0        0      269 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0        0        0    11669 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/model_selection/_search.py
+-rw-r--r--   0        0        0    18413 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/model_selection/_validation.py
+-rw-r--r--   0        0        0      108 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/__init__.py
+-rw-r--r--   0        0        0     5066 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_gradkcca.py
+-rw-r--r--   0        0        0    12301 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_kcca.py
+-rw-r--r--   0        0        0     6378 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_ncca.py
+-rw-r--r--   0        0        0     6280 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_scca_hsic.py
+-rw-r--r--   0        0        0       80 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0        0        0     4561 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/probabilistic/_probabilisticcca.py
+-rw-r--r--   0        0        0      129 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/utils/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/utils/check_values.py
+-rw-r--r--   0        0        0       52 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0        0        0    15027 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/visualisation/plotter.py
+-rw-r--r--   0        0        0     1167 2023-07-02 02:30:33.022161 cca_zoo-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 cca_zoo-2.1.0/PKG-INFO
```

### Comparing `cca_zoo-2.0.8/LICENSE` & `cca_zoo-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/README.md` & `cca_zoo-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/data/deep.py` & `cca_zoo-2.1.0/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/data/simulated.py` & `cca_zoo-2.1.0/cca_zoo/data/simulated.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/__init__.py` & `cca_zoo-2.1.0/cca_zoo/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_base.py` & `cca_zoo-2.1.0/cca_zoo/deep/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from torch.optim.lr_scheduler import CosineAnnealingLR, MultiStepLR
 
+from cca_zoo._base import BaseModel
 
-class BaseDeep(pl.LightningModule):
+
+class BaseDeep(pl.LightningModule, BaseModel):
     """A base class for deep learning linear using PyTorch Lightning."""
 
     def __init__(
         self,
         latent_dimensions: int,
         optimizer: str = "adam",
         scheduler: Optional[str] = None,
@@ -139,11 +141,7 @@
         pass
 
     @staticmethod
     def detach_all(z: List[torch.Tensor]) -> List[torch.Tensor]:
         """Detaches all tensors in a list from the computation graph."""
         # Use list comprehension instead of for loop
         return [z_.detach() for z_ in z]
-
-    def _more_tags(self) -> Dict[str, bool]:
-        """Returns additional tags for the model."""
-        return {"multiview": True}
```

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import torch
 
 from cca_zoo.deep import objectives
 from cca_zoo.deep._base import BaseDeep
 from cca_zoo.deep.metrics import MCCA
-from cca_zoo.linear._base import BaseModel
 
 
-class DCCA(BaseDeep, BaseModel):
+class DCCA(BaseDeep):
     """
     A class used to fit a DCCA model.
 
     References
     ----------
     Andrew, Galen, et al. "Deep canonical correlation analysis." International conference on machine learning. PMLR, 2013.
```

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_discriminative/_dtcca.py` & `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.1.0/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.1.0/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.1.0/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.1.0/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/architectures.py` & `cca_zoo-2.1.0/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/metrics.py` & `cca_zoo-2.1.0/cca_zoo/deep/metrics.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/deep/objectives.py` & `cca_zoo-2.1.0/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_base.py` & `cca_zoo-2.1.0/cca_zoo/_base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import itertools
 from abc import abstractmethod
-from typing import Iterable, Union
+from typing import Union, Iterable
 
 import numpy as np
 from sklearn.base import BaseEstimator, MultiOutputMixin, RegressorMixin
-from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted, check_random_state
+from sklearn.utils import check_random_state
+from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted
 
 
 class BaseModel(BaseEstimator, MultiOutputMixin, RegressorMixin):
     """
     A base class for multivariate latent variable linear.
 
     This class implements common methods and attributes for fitting and transforming
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_dummy.py` & `cca_zoo-2.1.0/cca_zoo/linear/_dummy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable
 
 import numpy as np
 
-from cca_zoo.linear._base import BaseModel
+from cca_zoo._base import BaseModel
 
 
 class DummyCCA(BaseModel):
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_gcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_gcca.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,30 +57,20 @@
             c=c,
             eps=eps,
             pca=False,
         )
         self.view_weights = view_weights
 
     def fit(self, views: Iterable[np.ndarray], y=None, K=None, **kwargs):
-        """
-        Parameters
-        ----------
-        views : Iterable[np.ndarray]
-            Views to fit the model with.
-        y : None
-            Not used in this model.
-        K : None
-            Observation matrix
-        """
         return super().fit(views, y=y, K=K, **kwargs)
 
     def _check_params(self):
         self.c = _process_parameter("c", self.c, 0, self.n_views_)
 
-    def C(self, views, K=None):
+    def _C(self, views, K=None):
         if K is None:
             # just use identity when all rows are observed in all views.
             K = np.ones((len(views), views[0].shape[0]))
         Q = []
         self.view_weights = _process_parameter(
             "view_weights", self.view_weights, 1, self.n_views_
         )
@@ -95,15 +85,15 @@
         Q = (
             np.diag(np.sqrt(np.sum(K, axis=0)))
             @ Q
             @ np.diag(np.sqrt(np.sum(K, axis=0)))
         )
         return Q
 
-    def D(self, views, **kwargs):
+    def _D(self, views, **kwargs):
         return None
 
     def _weights(self, eigvals, eigvecs, views, **kwargs):
         self.weights = [
             np.linalg.pinv(view) @ eigvecs[:, : self.latent_dimensions]
             for view in views
         ]
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_ey.py` & `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gh.py` & `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_gradient.py` & `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gradient.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_stochasticpls.py` & `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_stochasticpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_gradient/_svd.py` & `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_grcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_altmaxvar.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_altmaxvar.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,19 @@
         latent_dimensions=1,
         copy_data=True,
         random_state=None,
         epochs=100,
         tol=1e-3,
         proximal="L1",
         positive=False,
+        initialization="uniform",
         tau: Union[Iterable[float], float] = None,
         proximal_params: Iterable[dict] = None,
         gamma=0.1,
-        learning_rate=0.1,
+        learning_rate=1e-2,
         T=100,
         trainer_kwargs=None,
         convergence_checking=None,
         track=None,
         verbose=False,
     ):
         super().__init__(
@@ -33,14 +34,15 @@
             random_state=random_state,
             tol=tol,
             epochs=epochs,
             convergence_checking=convergence_checking,
             track=track,
             verbose=verbose,
             trainer_kwargs=trainer_kwargs,
+            initialization=initialization,
         )
         self.tau = tau
         self.proximal = proximal
         self.proximal_params = proximal_params
         self.gamma = gamma
         self.learning_rate = learning_rate
         self.T = T
@@ -91,15 +93,15 @@
     def __init__(
         self,
         weights,
         k=None,
         gamma=0.1,
         T=100,
         proximal_operators=None,
-        learning_rate=0.1,
+        learning_rate=1e-3,
         convergence_checking=None,
         track=None,
     ):
         super().__init__(
             weights=weights,
             k=k,
             convergence_checking=convergence_checking,
@@ -118,59 +120,63 @@
     def _get_target(self, scores):
         if hasattr(self, "G"):
             R = self.gamma * scores.mean(axis=0) + (1 - self.gamma) * self.G
         else:
             R = scores.mean(axis=0)
         U, S, Vt = np.linalg.svd(R, full_matrices=False)
         G = U @ Vt
-        return G
+        return G / np.sqrt(np.diag(np.atleast_1d(np.cov(G, rowvar=False))))
 
     def objective(self, views, scores, weights) -> int:
         least_squares = (np.linalg.norm(scores - self.G, axis=(1, 2)) ** 2).sum()
         regularization = np.array(
-            [
-                self.proximal_operators[view](weights[view])
-                for view in range(self.n_views)
-            ]
+            [self.proximal_operators[view](weights[view]) for view in range(len(views))]
         ).sum()
         return least_squares + regularization
 
     def training_step(self, batch, batch_idx):
         scores = np.stack(self(batch["views"]))
         self.G = self._get_target(scores)
-        converged = False
+        old_weights = self.weights.copy()
         for i, view in enumerate(batch["views"]):
             view = view.detach().numpy()
             t = 0
-            # initialize the previous weights to None
             prev_weights = None
+            converged = False
             while t < self.T and not converged:
+                grad = view.T @ (view @ self.weights[i] - self.G) / view.shape[0]
                 # update the weights using the gradient descent and proximal operator
-                self.weights[i] -= self.learning_rate * (
-                    view.T @ (view @ self.weights[i] - self.G)
-                )
+                self.weights[i] -= self.learning_rate * grad
                 self.weights[i] = self.proximal_operators[i].prox(
                     self.weights[i], self.learning_rate
                 )
                 # check if the weights have changed significantly from the previous iteration
                 if prev_weights is not None and np.allclose(
                     self.weights[i], prev_weights
                 ):
                     # if yes, set converged to True and break the loop
                     converged = True
-                    break
                 # update the previous weights for the next iteration
-                prev_weights = self.weights[i]
+                prev_weights = self.weights[i].copy()
                 t += 1
 
         # if track or convergence_checking is enabled, compute the objective function
         if self.tracking or self.convergence_checking:
-            objective = self.objective(batch["views"])
-
-            return {"loss": torch.tensor(objective)}
+            objective = self.objective(batch["views"], scores, self.weights)
+            # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
+            weights_change = torch.tensor(
+                np.max(
+                    [
+                        np.max(np.abs(old_weights[i] - self.weights[i]))
+                        / np.max(np.abs(self.weights[i]))
+                        for i in range(len(self.weights))
+                    ]
+                )
+            )
+            return {"loss": torch.tensor(objective), "weights_change": weights_change}
 
 
 from pyproximal import (
     L0,
     L0Ball,
     L1,
     L1Ball,
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_base.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 from abc import abstractmethod
 from typing import Iterable, List, Optional, Union, Any
 
 import numpy as np
 import pytorch_lightning as pl
+from lightning_fabric.utilities.warnings import PossibleUserWarning
 from pytorch_lightning.callbacks import Callback, EarlyStopping
 from torch.utils import data
 from torch.utils.data import DataLoader
 
 from cca_zoo.data.deep import NumpyDataset
-from cca_zoo.linear import MCCA, rCCA
-from cca_zoo.linear._base import BaseModel
-from cca_zoo.linear._dummy import DummyCCA
+from cca_zoo.linear._pls import MPLS
+from cca_zoo.linear._mcca import MCCA
+
+from cca_zoo._base import BaseModel
+from cca_zoo.linear._dummy import DummyCCA, DummyPLS
 import torch
 
+# filter warnings from pytorch_lightning
+import warnings
+
+warnings.filterwarnings("ignore", category=UserWarning)
+warnings.filterwarnings("ignore", category=PossibleUserWarning)
+
+
+def supress_device_warnings():
+    import logging
+
+    rank_zero_logger = logging.getLogger("pytorch_lightning.utilities.rank_zero")
+    rank_zero_logger.disabled = True
+
+
 # Default Trainer kwargs
 DEFAULT_TRAINER_KWARGS = dict(
     enable_checkpointing=False,
     logger=False,
     enable_model_summary=False,
     enable_progress_bar=True,
 )
@@ -65,17 +82,17 @@
         self.learning_rate = learning_rate
         # validate the deflation method
         if deflation not in ["cca", "pls"]:
             raise ValueError("Deflation method must be one of ['cca','pls']")
         else:
             self.deflation = deflation
         # validate the initialization method
-        if initialization not in ["random", "uniform", "pls", "cca"]:
+        if initialization not in ["random", "uniform", "unregularized", "pls"]:
             raise ValueError(
-                "Initialization method must be one of ['random', 'uniform', 'pls', 'cca']"
+                "Initialization method must be one of ['random', 'uniform', 'unregularized', 'pls']"
             )
         else:
             self.initialization = initialization
         # validate the callbacks
         self.verbose = verbose
         self.patience = patience
         self.callbacks = callbacks or []
@@ -179,21 +196,26 @@
         """Initialize the CCA weights using the initialization method or function.
 
         Parameters
         ----------
         views : Iterable[np.ndarray]
             The input views to initialize the CCA weights from
         """
+        pls = self._get_tags().get("pls", False)
         initializer = _default_initializer(
-            self.initialization, self.random_state, self.latent_dimensions
+            self.initialization, self.random_state, self.latent_dimensions, pls
         )
         # Fit the initializer on the input views and get the weights as numpy arrays
         self.weights = initializer.fit(views).weights
         self.weights = [weights.astype(np.float32) for weights in self.weights]
 
+    def _more_tags(self):
+        # Indicate that this class is for multiview data
+        return {"iterative": True}
+
 
 class BaseLoop(pl.LightningModule):
     def __init__(
         self,
         weights=None,
         k=None,
         tracking=False,
@@ -214,27 +236,43 @@
     def objective(self, *args, **kwargs) -> float:
         raise NotImplementedError
 
     def forward(self, views: list) -> list:
         return [view @ weight for view, weight in zip(views, self.weights)]
 
 
-def _default_initializer(initialization, random_state, latent_dims):
-    if initialization == "random":
-        initializer = DummyCCA(latent_dims, random_state=random_state, uniform=False)
-    elif initialization == "uniform":
-        initializer = DummyCCA(latent_dims, random_state=random_state, uniform=True)
-    elif initialization == "pls":
-        initializer = rCCA(latent_dims, random_state=random_state, c=1)
-    elif initialization == "cca":
-        initializer = MCCA(latent_dims)
+def _default_initializer(initialization, random_state, latent_dims, pls):
+    if pls:
+        if initialization == "random":
+            initializer = DummyPLS(
+                latent_dims, random_state=random_state, uniform=False
+            )
+        elif initialization == "uniform":
+            initializer = DummyPLS(latent_dims, random_state=random_state, uniform=True)
+        elif initialization == "unregularized":
+            initializer = MPLS(latent_dims, random_state=random_state)
+        else:
+            raise ValueError(
+                "Initialization {type} not supported. Pass a generator implementing this method"
+            )
     else:
-        raise ValueError(
-            "Initialization {type} not supported. Pass a generator implementing this method"
-        )
+        if initialization == "random":
+            initializer = DummyCCA(
+                latent_dims, random_state=random_state, uniform=False
+            )
+        elif initialization == "uniform":
+            initializer = DummyCCA(latent_dims, random_state=random_state, uniform=True)
+        elif initialization == "unregularized":
+            initializer = MCCA(latent_dims, random_state=random_state)
+        elif initialization == "pls":
+            initializer = MPLS(latent_dims, random_state=random_state)
+        else:
+            raise ValueError(
+                "Initialization {type} not supported. Pass a generator implementing this method"
+            )
     return initializer
 
 
 class ConvergenceCallback(EarlyStopping):
     def __init__(
         self,
         monitor: str = "loss",
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_deflation.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_deflation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_elasticnet.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_elasticnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import warnings
 from typing import Iterable, Union
 
 import numpy as np
 import torch
 from sklearn.linear_model import ElasticNet, Lasso, Ridge, SGDRegressor
 
-from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._base import (
+    BaseLoop,
+    BaseIterative,
+    supress_device_warnings,
+)
 from cca_zoo.linear._iterative._deflation import DeflationMixin
 from cca_zoo.utils import _process_parameter
 
+supress_device_warnings()
+
 
 class ElasticCCA(DeflationMixin, BaseIterative):
     r"""
     A class used to fit an elastic CCA model for two or more views of data.
 
     This model finds the linear projections of multiple views that maximize their pairwise correlations while enforcing L1 and L2 penalties on the projection vectors.
 
@@ -66,15 +72,15 @@
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         epochs: int = 100,
         deflation="cca",
-        initialization: Union[str, callable] = "pls",
+        initialization: Union[str, callable] = "uniform",
         tol: float = 1e-3,
         alpha: Union[Iterable[float], float] = None,
         l1_ratio: Union[Iterable[float], float] = None,
         stochastic=False,
         positive: Union[Iterable[bool], bool] = None,
         trainer_kwargs=None,
         convergence_checking=None,
@@ -164,30 +170,21 @@
             tol,
             random_state,
         )
         for view_index, weight in enumerate(weights):
             self.regressors[view_index].coef_ = weight[:, 0]
             self.regressors[view_index].intercept_ = 0
 
-    def forward(self, views: list) -> list:
-        scores = []
-        for view_index, view in enumerate(views):
-            scores.append(self.regressors[view_index].predict(view))
-        return scores
-
     def training_step(self, batch, batch_idx):
         scores = np.stack(self(batch["views"]))
+        target = np.sum(scores, axis=0)
+        target /= np.sqrt(np.cov(target))
         old_weights = self.weights.copy()
         # Update each view using loop update function
         for view_index, view in enumerate(batch["views"]):
-            # create a mask that is True for elements not equal to k along dim k
-            mask = np.arange(scores.shape[0]) != view_index
-            # apply the mask to scores and sum along dim k
-            target = np.sum(scores[mask], axis=0)
-            target /= np.linalg.norm(target) / np.sqrt(self.n_samples_)
             # Solve the elastic regression
             self.regressors[view_index] = self.regressors[view_index].fit(
                 batch["views"][view_index], target
             )
             self.weights[view_index] = self.regressors[view_index].coef_
         # if tracking or convergence_checking is enabled, compute the objective function
         if self.tracking or self.convergence_checking:
@@ -205,25 +202,22 @@
             return {"loss": torch.tensor(objective), "weights_change": weights_change}
 
     def on_fit_end(self) -> None:
         self.weights = [regressor.coef_ for regressor in self.regressors]
 
     def objective(self, views):
         scores = np.stack(self(views))
+        target = np.sum(scores, axis=0)
+        target /= np.sqrt(np.cov(target))
         objective = 0
         for view_index, view in enumerate(views):
-            # create a mask that is True for elements not equal to k along dim k
-            mask = np.arange(scores.shape[0]) != view_index
-            # apply the mask to scores and sum along dim k
-            target = np.sum(scores[mask], axis=0)
-            target /= np.linalg.norm(target) / np.sqrt(self.n_samples_)
             objective += elastic_objective(
-                view,
-                self.regressors[view_index].coef_,
+                scores[view_index],
                 target,
+                self.regressors[view_index].coef_,
                 self.alpha[view_index],
                 self.l1_ratio[view_index],
             )
         return objective
 
 
 class SCCA_IPLS(ElasticCCA):
@@ -257,73 +251,72 @@
             k=k,
             alpha=self.alpha,
             l1_ratio=self.l1_ratio,
             stochastic=self.stochastic,
             positive=self.positive,
             tol=self.tol,
             random_state=self.random_state,
+            tracking=self.track,
+            convergence_checking=self.convergence_checking,
         )
 
 
 class IPLSLoop(ElasticLoop):
     def training_step(self, batch, batch_idx):
-        scores = np.stack(self(batch["views"]))
         old_weights = self.weights.copy()
         # Update each view using loop update function
         for view_index, view in enumerate(batch["views"]):
+            scores = np.stack(self(batch["views"]))
             # create a mask that is True for elements not equal to k along dim k
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
             target = np.sum(scores[mask], axis=0)
             # Solve the elastic regression
             self.regressors[view_index] = self.regressors[view_index].fit(
                 batch["views"][view_index], target
             )
-            self.regressors[view_index].coef_ /= np.linalg.norm(
-                view @ self.regressors[view_index].coef_
-            ) / np.sqrt(self.n_samples_)
+            self.regressors[view_index].coef_ /= np.sqrt(
+                np.cov(view @ self.regressors[view_index].coef_)
+            )
             self.weights[view_index] = self.regressors[view_index].coef_
             # if tracking or convergence_checking is enabled, compute the objective function
-            if self.tracking or self.convergence_checking:
-                objective = self.objective(batch["views"])
-                # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
-                weights_change = torch.tensor(
-                    np.max(
-                        [
-                            np.max(np.abs(old_weights[i] - self.weights[i]))
-                            / np.max(np.abs(self.weights[i]))
-                            for i in range(len(self.weights))
-                        ]
-                    )
+        if self.tracking or self.convergence_checking:
+            objective = self.objective(batch["views"])
+            # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
+            weights_change = torch.tensor(
+                np.max(
+                    [
+                        np.max(np.abs(old_weights[i] - self.weights[i]))
+                        / np.max(np.abs(self.weights[i]))
+                        for i in range(len(self.weights))
+                    ]
                 )
-                return {"loss": objective, "weights_change": weights_change}
+            )
+            return {"loss": torch.tensor(objective), "weights_change": weights_change}
 
     def objective(self, views):
         scores = np.stack(self(views))
-
         objective = 0
         for view_index, view in enumerate(views):
             # create a mask that is True for elements not equal to k along dim k
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
             target = np.sum(scores[mask], axis=0)
-            target /= np.linalg.norm(target) / np.sqrt(self.n_samples_)
             objective += elastic_objective(
-                view,
-                self.regressors[view_index].coef_,
+                scores[view_index],
                 target,
+                self.regressors[view_index].coef_,
                 self.alpha[view_index],
                 self.l1_ratio[view_index],
             )
-        return {"loss": torch.tensor(objective)}
+        return objective
 
 
-def elastic_objective(x, w, y, alpha, l1_ratio):
+def elastic_objective(z, y, w, alpha, l1_ratio):
     n = len(y)
-    z = x @ w
     objective = np.linalg.norm(z - y) ** 2 / (2 * n)
     l1_pen = alpha * l1_ratio * np.linalg.norm(w, ord=1)
     l2_pen = alpha * (1 - l1_ratio) * np.linalg.norm(w, ord=2)
     return objective + l1_pen + l2_pen
 
 
 def initialize_regressors(alpha, l1_ratio, positive, stochastic, tol, random_state):
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_incrementalpls.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_incrementalpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_pls_als.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_pls_als.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,24 +74,24 @@
             learning_rate=learning_rate,
             initialization=initialization,
             callbacks=callbacks,
             trainer_kwargs={"accelerator": "cpu"},
         )
 
     def _get_module(self, weights=None, k=None):
-        return PlsAlsLoop(
+        return PLS_ALSLoop(
             weights=weights,
             k=k,
         )
 
     def _more_tags(self):
-        return {"multiview": True}
+        return {"multiview": True, "pls": True}
 
 
-class PlsAlsLoop(BaseLoop):
+class PLS_ALSLoop(BaseLoop):
     def training_step(self, batch, batch_idx):
         scores = np.stack(self(batch["views"]))
         # Update each view using loop update function
         for view_index, view in enumerate(batch["views"]):
             # create a mask that is True for elements not equal to k along dim k
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_admm.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_admm.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from typing import Iterable, Union
 import numpy as np
-from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._base import (
+    BaseLoop,
+    BaseIterative,
+    supress_device_warnings,
+)
 from cca_zoo.linear._iterative._deflation import DeflationMixin
 from cca_zoo.linear._pls import PLSMixin
 from cca_zoo.utils import _process_parameter
 
+supress_device_warnings()
+
 
 class SCCA_Parkhomenko(DeflationMixin, PLSMixin, BaseIterative):
     r"""
     A class used to fit a sparse CCA (penalized CCA) model for two or more views.
 
     This model finds the linear projections of multiple views that maximize their pairwise correlations while enforcing sparsity constraints on the projection vectors.
 
@@ -43,15 +49,15 @@
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         deflation="cca",
         tau: Union[Iterable[float], float] = None,
-        initialization: Union[str, callable] = "pls",
+        initialization: Union[str, callable] = "unregularized",
         tol: float = 1e-3,
         convergence_checking=False,
         patience=10,
         track=False,
         verbose=False,
     ):
         self.tau = tau
@@ -81,15 +87,15 @@
             weights=weights,
             k=k,
             tau=self.tau,
             tol=self.tol,
         )
 
     def _more_tags(self):
-        return {"multiview": True}
+        return {"multiview": True, "pls": True}
 
 
 class ParkhomenkoLoop(BaseLoop):
     def __init__(self, weights, k=None, tau=None, tol=1e-3):
         super().__init__(weights=weights, k=k)
         self.tau = tau
         self.tol = tol
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_pmd.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_pmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import itertools
 import warnings
 
 import numpy as np
 import torch
 
-from cca_zoo.linear._iterative._base import BaseLoop, BaseIterative
+from cca_zoo.linear._iterative._base import (
+    BaseLoop,
+    BaseIterative,
+    supress_device_warnings,
+)
 from cca_zoo.linear._iterative._deflation import DeflationMixin
 from cca_zoo.linear._pls import PLSMixin
 from cca_zoo.linear._search import _delta_search
 from cca_zoo.utils import _process_parameter
 
+supress_device_warnings()
+
 
 class SCCA_PMD(DeflationMixin, PLSMixin, BaseIterative):
     r"""
     A class used to fit a sparse CCA model by penalized matrix decomposition (PMD).
 
     This model finds the linear projections of two views that maximize their correlation while enforcing sparsity constraints on the projection vectors.
 
@@ -64,15 +70,15 @@
     def __init__(
         self,
         latent_dimensions=1,
         copy_data=True,
         random_state=None,
         epochs=100,
         deflation="cca",
-        initialization="pls",
+        initialization="unregularized",
         tol=1e-3,
         positive=False,
         tau=None,
         trainer_kwargs=None,
         convergence_checking=None,
         track=None,
         verbose=None,
@@ -118,15 +124,15 @@
             tau=self.tau,
             tol=self.tol,
             tracking=self.track,
             convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
-        return {"multiview": True}
+        return {"multiview": True, "pls": True}
 
 
 class PMDLoop(BaseLoop):
     def __init__(
         self,
         weights,
         k=None,
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_scca_span.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_span.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             self.update = support_threshold
         elif self.regularisation == "l1":
             self.update = _delta_search
         self.rank = rank
         self.random_state = random_state
 
     def training_step(self, batch, batch_idx):
-        # if P, D, Q not initialised, initialise them
+        # if P, _D, Q not initialised, initialise them
         if getattr(self, "P", None) is None:
             self._initialize(batch["views"])
         c = self.random_state.randn(self.rank)
         c /= np.linalg.norm(c)
         a = self.P @ np.diag(self.D) @ c
         u = self.update(a, self.tau[0])
         u /= np.linalg.norm(u)
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_iterative/_swcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_swcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_mcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_mcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, Union
 
 import numpy as np
 from scipy.linalg import block_diag
 from scipy.linalg import eigh
 from sklearn.decomposition import PCA
 
-from cca_zoo.linear._base import BaseModel
+from cca_zoo._base import BaseModel
 from cca_zoo.utils import _process_parameter
 
 
 class MCCA(BaseModel):
     r"""
     A class used to fit Regularised CCA (canonical ridge) model. This model adds a regularization term to the CCA objective function to avoid overfitting and improve stability. It uses PCA to perform the optimization efficiently for high dimensional data.
 
@@ -39,15 +39,15 @@
         Regularisation parameter, by default None
     accept_sparse : Union[bool, str], optional
         Whether to accept sparse data, by default None
 
 
     References
     --------
-    Vinod, Hrishikesh D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
+    Vinod, Hrishikesh _D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
     """
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
@@ -92,19 +92,19 @@
     def _process_data(self, views, **kwargs):
         if self.pca:
             views = self._apply_pca(views)
         return views
 
     def _solve_gevp(self, views: Iterable[np.ndarray], y=None, **kwargs):
         # Setup the eigenvalue problem
-        C = self.C(views, **kwargs)
-        D = self.D(views, **kwargs)
+        C = self._C(views, **kwargs)
+        D = self._D(views, **kwargs)
         self.splits = np.cumsum([view.shape[1] for view in views])
         # Solve the eigenvalue problem
-        # Get the dimension of C
+        # Get the dimension of _C
         p = C.shape[0]
         # Solve the generalized eigenvalue problem Cx=lambda Dx using a subset of eigenvalues and eigenvectors
         [eigvals, eigvecs] = eigh(
             C,
             D,
             subset_by_index=[p - self.latent_dimensions, p - 1],
         )
@@ -127,21 +127,21 @@
         """
         Do data driven PCA on each view
         """
         self.pca_models = [PCA() for _ in views]
         # Fit PCA on each view
         return [self.pca_models[i].fit_transform(view) for i, view in enumerate(views)]
 
-    def C(self, views, **kwargs):
+    def _C(self, views, **kwargs):
         all_views = np.hstack(views)
         C = np.cov(all_views, rowvar=False)
         C -= block_diag(*[np.cov(view, rowvar=False) for view in views])
         return C / len(views)
 
-    def D(self, views, **kwargs):
+    def _D(self, views, **kwargs):
         if self.pca:
             # Can regularise by adding to diagonal
             D = block_diag(
                 *[
                     np.diag((1 - self.c[i]) * pc.explained_variance_ + self.c[i])
                     for i, pc in enumerate(self.pca_models)
                 ]
@@ -179,18 +179,18 @@
 
         (1-c_2)w_2^TX_2^TX_2w_2+c_2w_2^Tw_2=n
 
     where :math:`c_i` are the regularization parameters for each view.
 
     References
     --------
-    Vinod, Hrishikesh D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
+    Vinod, Hrishikesh _D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
     """
 
-    def C(self, views, **kwargs):
+    def _C(self, views, **kwargs):
         if len(views) != 2:
             raise ValueError(
                 f"Model can only be used with two views, but {len(views)} were given. Use MCCA or GCCA instead."
             )
         # Compute the B matrices for each view
         B = [
             (1 - self.c[i]) * pc.explained_variance_ + self.c[i]
@@ -203,15 +203,15 @@
         if views[0].shape[1] <= views[1].shape[1]:
             self.primary_view = 0
             return C @ C.T
         else:
             self.primary_view = 1
             return C.T @ C
 
-    def D(self, views, **kwargs):
+    def _D(self, views, **kwargs):
         return None
 
     def _weights(self, eigvals, eigvecs, views):
         B = [
             (1 - self.c[i]) * pc.singular_values_**2 / self.n_samples_ + self.c[i]
             for i, pc in enumerate(self.pca_models)
         ]
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_partialcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_partialcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Iterable, Union
+from typing import Iterable
 
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.linear import MCCA
+from cca_zoo.linear._mcca import MCCA
 
 
 class PartialCCA(MCCA):
     r"""
     A class used to fit a partial CCA model. This model extends CCA to account for confounding variables that may affect the correlation between views.
 
     .. math::
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_pcacca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_pcacca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_pls.py` & `cca_zoo-2.1.0/cca_zoo/linear/_pls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cca_zoo.linear import rCCA, MCCA
+from cca_zoo.linear._mcca import rCCA, MCCA
 from typing import Iterable
 
 import numpy as np
 
 
 def reduce_dims(x):
     U, S, _ = np.linalg.svd(x, full_matrices=False)
@@ -258,14 +258,18 @@
         total_correlation_captured : float
 
         """
         transformed_views = self.transform(views, **kwargs)
         total_correlation_captured = self.total_correlation_(transformed_views)
         return total_correlation_captured
 
+    def _more_tags(self):
+        # Indicate that this class is for multiview data
+        return {"pls": True}
+
 
 class PLS(rCCA, PLSMixin):
     r"""
     A class used to fit a simple PLS model. This model finds the linear projections of two views that maximize their covariance.
 
     Implements PLS by inheriting regularised CCA with maximal regularisation. This is equivalent to solving the following optimization problem:
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_prcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_prcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,21 @@
         self.p = [X_i.shape[1] for X_i in X_1]
         X_2 = [np.delete(view, idx, axis=1) for view, idx in zip(views, idxs)]
         self.B = [np.linalg.pinv(X_2) @ X_1 for X_1, X_2 in zip(X_1, X_2)]
         X_1 = [X_1 - X_2 @ B for X_1, X_2, B in zip(X_1, X_2, self.B)]
         views = [np.hstack((X_1, X_2)) for X_1, X_2 in zip(X_1, X_2)]
         return views
 
-    def C(self, views, **kwargs):
+    def _C(self, views, **kwargs):
         all_views = np.concatenate(views, axis=1)
         C = np.cov(all_views, rowvar=False)
         C -= block_diag(*[np.cov(view, rowvar=False) for view in views])
         return C
 
-    def D(self, views: Iterable[np.ndarray], idxs=None, **kwargs):
+    def _D(self, views: Iterable[np.ndarray], idxs=None, **kwargs):
         penalties = [np.zeros((view.shape[1])) for view in views]
         for i, idx in enumerate(idxs):
             penalties[i][idx] = self.c[i]
         D = block_diag(
             *[
                 (1 - self.c[i]) * np.cov(view, rowvar=False) + np.diag(penalties[i])
                 for i, view in enumerate(views)
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_search.py` & `cca_zoo-2.1.0/cca_zoo/linear/_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,15 +38,23 @@
         # Return the square of the difference between the 1-norm of coefficients and the threshold c
         return (np.sum(np.abs(coef)) - c) ** 2
 
     # Find the minimum of f using scipy minimization function
     # You can specify the method or let the function choose the best one for you
     # You can also pass other parameters like tol, maxiter, etc.
     # bound x to be between 0 and 1
-    result = minimize(f, x0=0, bounds=[(0, 1)])
+
+    # try some different methods until one gets result.success == True
+    result = minimize(f, x0=0, bounds=[(0, 1)], method="L-BFGS-B")
+    if not result.success:
+        result = minimize(f, x0=0, bounds=[(0, 1)], method="TNC")
+    if not result.success:
+        result = minimize(f, x0=0, bounds=[(0, 1)], method="SLSQP")
+    if not result.success:
+        result = minimize(f, x0=0, bounds=[(0, 1)], method="trust-constr")
 
     # Check if the solution is valid and converged
     if result.success:
         # Get the optimal delta from the result object
         delta = result.x
 
         # Apply soft thresholding to the weights with optimal delta
```

### Comparing `cca_zoo-2.0.8/cca_zoo/linear/_tcca.py` & `cca_zoo-2.1.0/cca_zoo/linear/_tcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable
 
 import numpy as np
 import tensorly as tl
 from scipy.linalg import sqrtm
 from tensorly.decomposition import parafac
 
-from cca_zoo.linear import MCCA
+from cca_zoo.linear._mcca import MCCA
 
 
 class TCCA(MCCA):
     r"""
     A class used to fit TCCA model. This model extends MCCA to higher order correlations by using tensor products of the views.
 
     The objective function of TCCA is:
```

### Comparing `cca_zoo-2.0.8/cca_zoo/model_selection/_search.py` & `cca_zoo-2.1.0/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.1.0/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/nonparametric/_gradkcca.py` & `cca_zoo-2.1.0/cca_zoo/nonparametric/_gradkcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/nonparametric/_kcca.py` & `cca_zoo-2.1.0/cca_zoo/nonparametric/_kcca.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,18 @@
         return transformed_views
 
     @property
     def alphas(self):
         check_is_fitted(self, attributes=["weights"])
         return self.weights
 
+    def _more_tags(self):
+        # Indicate that this class is for multiview data
+        return {"kernel": True}
+
 
 class KCCA(KernelMixin, MCCA):
     r"""
     A class used to fit KCCA model. This model extends MCCA to nonlinear relationships by using kernel functions on each view.
 
     The objective function of KCCA is:
 
@@ -141,29 +145,25 @@
         # Store the kernel parameters
         self.kernel_params = kernel_params
         self.gamma = gamma
         self.coef0 = coef0
         self.kernel = kernel
         self.degree = degree
 
-    def D(self, views, **kwargs):
+    def _D(self, views, **kwargs):
         D = block_diag(
             *[
                 (1 - self.c[i]) * np.cov(view, rowvar=False) + self.c[i] * view
                 for i, view in enumerate(views)
             ]
         )
         D_smallest_eig = min(0, np.linalg.eigvalsh(D).min()) - self.eps
         D = D - D_smallest_eig * np.eye(D.shape[0])
         return D / len(views)
 
-    def _more_tags(self):
-        # Indicate that this class is for multiview data
-        return {"multiview": True, "kernel": True}
-
 
 class KGCCA(KernelMixin, GCCA):
     r"""
     A class used to fit KGCCA model. This model extends GCCA to nonlinear relationships by using kernel functions on each view.
 
     The objective function of KGCCA is:
 
@@ -259,18 +259,14 @@
             for i, view in enumerate(self.train_views)
         ]
         self.weights = [
             np.linalg.pinv(kernel) @ eigvecs[:, : self.latent_dimensions]
             for kernel in kernels
         ]
 
-    def _more_tags(self):
-        # Indicate that this class is for multiview data
-        return {"multiview": True, "kernel": True}
-
 
 class KTCCA(KernelMixin, TCCA):
     r"""
     A class used to fit KTCCA model. This model extends TCCA to nonlinear relationships by using kernel functions on each view.
 
     The objective function of KTCCA is:
 
@@ -337,11 +333,7 @@
                 coef0=self.coef0[i],
                 filter_params=True,
                 **self.kernel_params[i]
             )
             for i, view in enumerate(self.train_views)
         ]
         return super()._setup_tensor(kernels)
-
-    def _more_tags(self):
-        # Indicate that this class is for multiview data
-        return {"multiview": True, "kernel": True}
```

### Comparing `cca_zoo-2.0.8/cca_zoo/nonparametric/_ncca.py` & `cca_zoo-2.1.0/cca_zoo/nonparametric/_ncca.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable, Union
 
 import numpy as np
 from sklearn.metrics import pairwise_kernels
 from sklearn.neighbors import NearestNeighbors
 
-from cca_zoo.linear._base import BaseModel
+from cca_zoo._base import BaseModel
 from cca_zoo.utils.check_values import _process_parameter
 
 
 class NCCA(BaseModel):
     """
     A class used to fit nonparametric (NCCA) model. This model extends CCA to nonlinear relationships by using local linear projections based on nearest neighbors.
```

### Comparing `cca_zoo-2.0.8/cca_zoo/nonparametric/_scca_hsic.py` & `cca_zoo-2.1.0/cca_zoo/nonparametric/_scca_hsic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.1.0/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import numpyro
 import numpyro.distributions as dist
 from jax.random import PRNGKey
 from numpyro.infer import MCMC, NUTS, Predictive
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.linear._base import BaseModel
+from cca_zoo._base import BaseModel
 
 
 class ProbabilisticCCA(BaseModel):
     """
     A class used to fit a Probabilistic CCA. Not quite the same due to using VI methods rather than EM
 
     Parameters
@@ -118,7 +118,10 @@
                     dist.MultivariateNormal((z @ W_) + mu_, scale_tril=psi_),
                     obs=X_,
                 )
                 for i, (X_, psi_, mu_, W_) in enumerate(
                     zip(views, psi, mu, self.weights_list)
                 )
             ]
+
+    def _more_tags(self):
+        return {"probabilistic": True}
```

### Comparing `cca_zoo-2.0.8/cca_zoo/utils/check_values.py` & `cca_zoo-2.1.0/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.8/pyproject.toml` & `cca_zoo-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "cca-zoo"
-version = "2.0.8"
+version = "2.1.0"
 description = "Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework"
 authors = ["jameschapman <james.chapman.19@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jameschapman19/cca_zoo"
 keywords = ["cca"]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<4.0.0"
 numpy = "*"
 scipy = "*"
-scikit-learn = "*"
-matplotlib = "*"
+scikit-learn = "^1.2.2"
+matplotlib = "^3.7.1"
 pandas = "*"
 seaborn = "*"
 tensorly = "*"
 joblib = "*"
 mvlearn = "*"
 tqdm = "*"
 torch = [
      {version = "^2.0.1", platform = "darwin"},
      {version = "^2.0.1", platform = "linux", source = "torch"},
      {version = "^2.0.1", platform = "win32", source = "torch"}, ]
-pytorch-lightning = "*"
+lightning = "*"
 pyproximal = "*"
 
 [[tool.poetry.source]]
  name = "torch"
  url = "https://download.pytorch.org/whl/cpu"
  priority = "explicit"
```

### Comparing `cca_zoo-2.0.8/PKG-INFO` & `cca_zoo-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.0.8
+Version: 2.1.0
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 License: MIT
 Keywords: cca
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: probabilistic
 Requires-Dist: joblib
-Requires-Dist: matplotlib
+Requires-Dist: lightning
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mvlearn
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyproximal
-Requires-Dist: pytorch-lightning
-Requires-Dist: scikit-learn
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: tensorly
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; sys_platform == "darwin"
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; sys_platform == "linux"
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; sys_platform == "win32"
 Requires-Dist: tqdm
```

