# Comparing `tmp/python_kasa-0.5.1.tar.gz` & `tmp/python_kasa-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_kasa-0.5.1.tar", max compression
+gzip compressed data, was "python_kasa-0.5.2.tar", max compression
```

## Comparing `python_kasa-0.5.1.tar` & `python_kasa-0.5.2.tar`

### file list

```diff
@@ -1,106 +1,105 @@
--rw-r--r--   0        0        0    63551 2023-02-18 21:43:28.825349 python_kasa-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0    33218 2023-02-18 21:43:28.825349 python_kasa-0.5.1/LICENSE
--rw-r--r--   0        0        0     6400 2023-02-18 21:43:28.825349 python_kasa-0.5.1/README.md
--rwxr-xr-x   0        0        0     1304 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/__init__.py
--rwxr-xr-x   0        0        0    21242 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/cli.py
--rwxr-xr-x   0        0        0     8442 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/discover.py
--rw-r--r--   0        0        0     7476 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/effects.py
--rw-r--r--   0        0        0     2311 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/emeterstatus.py
--rw-r--r--   0        0        0      115 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/exceptions.py
--rw-r--r--   0        0        0      571 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/__init__.py
--rw-r--r--   0        0        0     1617 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/ambientlight.py
--rw-r--r--   0        0        0      234 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/antitheft.py
--rw-r--r--   0        0        0     1370 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/cloud.py
--rw-r--r--   0        0        0      158 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/countdown.py
--rw-r--r--   0        0        0     2947 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/emeter.py
--rw-r--r--   0        0        0     2351 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/module.py
--rw-r--r--   0        0        0     1791 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/motion.py
--rw-r--r--   0        0        0     1924 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/rulemodule.py
--rw-r--r--   0        0        0      150 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/schedule.py
--rw-r--r--   0        0        0     1417 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/time.py
--rw-r--r--   0        0        0     3476 2023-02-18 21:43:28.825349 python_kasa-0.5.1/kasa/modules/usage.py
--rwxr-xr-x   0        0        0     8375 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/protocol.py
--rw-r--r--   0        0        0        0 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/py.typed
--rw-r--r--   0        0        0    18426 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/smartbulb.py
--rwxr-xr-x   0        0        0    24020 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/smartdevice.py
--rw-r--r--   0        0        0     5503 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/smartdimmer.py
--rw-r--r--   0        0        0     4019 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/smartlightstrip.py
--rw-r--r--   0        0        0     2758 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/smartplug.py
--rwxr-xr-x   0        0        0    12649 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/smartstrip.py
--rw-r--r--   0        0        0        0 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/__init__.py
--rw-r--r--   0        0        0     6617 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/conftest.py
--rwxr-xr-x   0        0        0      974 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/EP10(US)_1.0_1.0.2.json
--rw-r--r--   0        0        0     1427 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/EP40(US)_1.0_1.0.2.json
--rw-r--r--   0        0        0     3677 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/ES20M(US)_1.0_1.0.8.json
--rw-r--r--   0        0        0     1382 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS100(US)_1.0.json
--rw-r--r--   0        0        0     1305 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS100(US)_1.0_real.json
--rw-r--r--   0        0        0     1422 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS100(US)_2.0_real.json
--rw-r--r--   0        0        0     1552 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS103(US)_1.0.json
--rw-r--r--   0        0        0     1356 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS103(US)_2.1.json
--rw-r--r--   0        0        0      938 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS103(US)_2.1_1.1.4.json
--rw-r--r--   0        0        0     1397 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS105(US)_1.0.json
--rw-r--r--   0        0        0     1425 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS105(US)_1.0_real.json
--rw-r--r--   0        0        0     1729 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS107(US)_1.0_real.json
--rw-r--r--   0        0        0     1477 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS110(EU)_1.0_real.json
--rw-r--r--   0        0        0     1503 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS110(EU)_2.0.json
--rw-r--r--   0        0        0     1480 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS110(US)_1.0.json
--rw-r--r--   0        0        0     1388 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS200(US)_1.0.json
--rw-r--r--   0        0        0     1442 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS200(US)_2.0_real.json
--rw-r--r--   0        0        0      946 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS200(US)_5.0_1.0.2.json
--rw-r--r--   0        0        0     1476 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS210(US)_1.0_real.json
--rw-r--r--   0        0        0     2175 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS220(US)_1.0.json
--rw-r--r--   0        0        0     2183 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS220(US)_1.0_real.json
--rw-r--r--   0        0        0     1845 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS220(US)_2.0.json
--rw-r--r--   0        0        0     3000 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS300(US)_1.0.json
--rw-r--r--   0        0        0     2964 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS300(US)_1.0_real.json
--rw-r--r--   0        0        0     2866 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/HS300(US)_2.0_1.0.3.json
--rw-r--r--   0        0        0     2664 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL110(US)_1.0_1.8.11.json
--rw-r--r--   0        0        0     2724 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL120(US)_1.0_real.json
--rw-r--r--   0        0        0     2627 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL125(US)_1.20_1.0.5.json
--rw-r--r--   0        0        0     2768 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL125(US)_2.0_1.0.7.json
--rw-r--r--   0        0        0     2537 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL130(EU)_1.0_1.8.8.json
--rw-r--r--   0        0        0     2736 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL130(US)_1.0.json
--rw-r--r--   0        0        0     2667 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL130(US)_1.0_1.8.11.json
--rw-r--r--   0        0        0     2649 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL135(US)_1.0_1.0.6.json
--rw-r--r--   0        0        0     1717 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.5.json
--rw-r--r--   0        0        0     1750 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.8.json
--rw-r--r--   0        0        0     1721 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL420L5(US)_1.0_1.0.2.json
--rw-r--r--   0        0        0     2757 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL430(UN)_2.0_1.0.8.json
--rw-r--r--   0        0        0     2065 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL430(US)_1.0.json
--rw-r--r--   0        0        0     1787 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL430(US)_2.0_1.0.8.json
--rw-r--r--   0        0        0     1757 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL430(US)_2.0_1.0.9.json
--rw-r--r--   0        0        0     2661 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL50(US)_1.0_1.1.13.json
--rw-r--r--   0        0        0     3007 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL60(UN)_1.0.json
--rw-r--r--   0        0        0     2668 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KL60(US)_1.0_1.1.13.json
--rw-r--r--   0        0        0      940 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP100(US)_3.0_1.0.1.json
--rw-r--r--   0        0        0      997 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP105(UK)_1.0_1.0.7.json
--rw-r--r--   0        0        0     1227 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP115(EU)_1.0_1.0.16.json
--rw-r--r--   0        0        0     1213 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP115(US)_1.0_1.0.17.json
--rw-r--r--   0        0        0     1230 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP125(US)_1.0_1.0.6.json
--rw-r--r--   0        0        0     2036 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP303(UK)_1.0.json
--rw-r--r--   0        0        0     1738 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP303(US)_2.0_1.0.3.json
--rw-r--r--   0        0        0     1843 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP400(US)_1.0.json
--rw-r--r--   0        0        0     1431 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP400(US)_2.0_1.0.6.json
--rw-r--r--   0        0        0      966 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KP401(US)_1.0_1.0.0.json
--rw-r--r--   0        0        0     2842 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KS200M(US)_1.0_1.0.8.json
--rw-r--r--   0        0        0     3684 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KS220M(US)_1.0_1.0.4.json
--rw-r--r--   0        0        0     1836 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/KS230(US)_1.0_1.0.14.json
--rw-r--r--   0        0        0     3062 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/LB100(US)_1.0.json
--rw-r--r--   0        0        0     2684 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/LB110(US)_1.0_1.8.11.json
--rw-r--r--   0        0        0     3067 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/LB120(US)_1.0.json
--rw-r--r--   0        0        0     3106 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/fixtures/LB130(US)_1.0.json
--rw-r--r--   0        0        0    16115 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/newfakes.py
--rw-r--r--   0        0        0     8110 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_bulb.py
--rw-r--r--   0        0        0     3538 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_cli.py
--rw-r--r--   0        0        0     3573 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_dimmer.py
--rw-r--r--   0        0        0     4391 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_discovery.py
--rw-r--r--   0        0        0     2997 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_emeter.py
--rw-r--r--   0        0        0     2142 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_lightstrip.py
--rw-r--r--   0        0        0      593 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_plug.py
--rw-r--r--   0        0        0     5789 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_protocol.py
--rw-r--r--   0        0        0     2753 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_readme_examples.py
--rw-r--r--   0        0        0     4014 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_smartdevice.py
--rw-r--r--   0        0        0     4056 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_strip.py
--rw-r--r--   0        0        0      576 2023-02-18 21:43:28.829349 python_kasa-0.5.1/kasa/tests/test_usage.py
--rw-r--r--   0        0        0     2278 2023-02-18 21:43:28.833349 python_kasa-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7700 1970-01-01 00:00:00.000000 python_kasa-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    66931 2023-07-02 14:29:08.870189 python_kasa-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0    33218 2023-07-02 14:29:08.870189 python_kasa-0.5.2/LICENSE
+-rw-r--r--   0        0        0     6690 2023-07-02 14:29:08.870189 python_kasa-0.5.2/README.md
+-rwxr-xr-x   0        0        0     1288 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/__init__.py
+-rwxr-xr-x   0        0        0    21335 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/cli.py
+-rwxr-xr-x   0        0        0     8514 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/discover.py
+-rw-r--r--   0        0        0     7476 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/effects.py
+-rw-r--r--   0        0        0     2311 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/emeterstatus.py
+-rw-r--r--   0        0        0      115 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/exceptions.py
+-rwxr-xr-x   0        0        0      262 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/json.py
+-rw-r--r--   0        0        0      571 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/__init__.py
+-rw-r--r--   0        0        0     1617 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/ambientlight.py
+-rw-r--r--   0        0        0      234 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/antitheft.py
+-rw-r--r--   0        0        0     1370 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/cloud.py
+-rw-r--r--   0        0        0      158 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/countdown.py
+-rw-r--r--   0        0        0     2947 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/emeter.py
+-rw-r--r--   0        0        0     2351 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/module.py
+-rw-r--r--   0        0        0     2294 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/motion.py
+-rw-r--r--   0        0        0     1924 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/rulemodule.py
+-rw-r--r--   0        0        0      150 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/schedule.py
+-rw-r--r--   0        0        0     1417 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/time.py
+-rw-r--r--   0        0        0     3476 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/modules/usage.py
+-rwxr-xr-x   0        0        0     8733 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:29:08.870189 python_kasa-0.5.2/kasa/py.typed
+-rw-r--r--   0        0        0    18768 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/smartbulb.py
+-rwxr-xr-x   0        0        0    24405 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/smartdevice.py
+-rw-r--r--   0        0        0     7217 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/smartdimmer.py
+-rw-r--r--   0        0        0     4019 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/smartlightstrip.py
+-rw-r--r--   0        0        0     2758 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/smartplug.py
+-rwxr-xr-x   0        0        0    12649 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/smartstrip.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/__init__.py
+-rw-r--r--   0        0        0     6626 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/conftest.py
+-rw-r--r--   0        0        0      974 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/EP10(US)_1.0_1.0.2.json
+-rw-r--r--   0        0        0     1427 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/EP40(US)_1.0_1.0.2.json
+-rw-r--r--   0        0        0     3677 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/ES20M(US)_1.0_1.0.8.json
+-rw-r--r--   0        0        0     1305 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS100(US)_1.0_1.2.5.json
+-rw-r--r--   0        0        0     1422 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS100(US)_2.0_1.5.6.json
+-rw-r--r--   0        0        0     1552 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS103(US)_1.0_1.5.7.json
+-rw-r--r--   0        0        0     1356 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS103(US)_2.1_1.1.2.json
+-rw-r--r--   0        0        0      938 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS103(US)_2.1_1.1.4.json
+-rw-r--r--   0        0        0     1425 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS105(US)_1.0_1.5.6.json
+-rw-r--r--   0        0        0     1397 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS105(US)_1.0_mocked.json
+-rw-r--r--   0        0        0     1729 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS107(US)_1.0_1.0.8.json
+-rw-r--r--   0        0        0     1477 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS110(EU)_1.0_1.2.5.json
+-rw-r--r--   0        0        0     1503 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS110(EU)_2.0_mocked.json
+-rw-r--r--   0        0        0     1480 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS110(US)_1.0_mocked.json
+-rw-r--r--   0        0        0     1388 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS200(US)_1.0_mocked.json
+-rw-r--r--   0        0        0     1442 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS200(US)_2.0_1.5.7.json
+-rw-r--r--   0        0        0      946 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS200(US)_5.0_1.0.2.json
+-rw-r--r--   0        0        0     1476 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS210(US)_1.0_1.5.8.json
+-rw-r--r--   0        0        0     2183 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS220(US)_1.0_1.5.7.json
+-rw-r--r--   0        0        0     2175 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS220(US)_1.0_mocked.json
+-rw-r--r--   0        0        0     1845 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS220(US)_2.0_1.0.3.json
+-rw-r--r--   0        0        0     2964 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS300(US)_1.0_1.0.10.json
+-rw-r--r--   0        0        0     2866 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/HS300(US)_2.0_1.0.3.json
+-rw-r--r--   0        0        0     2664 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL110(US)_1.0_1.8.11.json
+-rw-r--r--   0        0        0     2724 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL120(US)_1.0_1.8.6.json
+-rw-r--r--   0        0        0     2627 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL125(US)_1.20_1.0.5.json
+-rw-r--r--   0        0        0     2768 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL125(US)_2.0_1.0.7.json
+-rw-r--r--   0        0        0     2537 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL130(EU)_1.0_1.8.8.json
+-rw-r--r--   0        0        0     2667 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL130(US)_1.0_1.8.11.json
+-rw-r--r--   0        0        0     2649 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL135(US)_1.0_1.0.6.json
+-rw-r--r--   0        0        0     1717 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.5.json
+-rw-r--r--   0        0        0     1750 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.8.json
+-rw-r--r--   0        0        0     1721 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL420L5(US)_1.0_1.0.2.json
+-rw-r--r--   0        0        0     2757 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL430(UN)_2.0_1.0.8.json
+-rw-r--r--   0        0        0     2065 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL430(US)_1.0_1.0.10.json
+-rw-r--r--   0        0        0     1787 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL430(US)_2.0_1.0.8.json
+-rw-r--r--   0        0        0     1757 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL430(US)_2.0_1.0.9.json
+-rw-r--r--   0        0        0     2661 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL50(US)_1.0_1.1.13.json
+-rw-r--r--   0        0        0     3007 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL60(UN)_1.0_1.1.4.json
+-rw-r--r--   0        0        0     2668 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KL60(US)_1.0_1.1.13.json
+-rw-r--r--   0        0        0      940 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP100(US)_3.0_1.0.1.json
+-rw-r--r--   0        0        0      997 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP105(UK)_1.0_1.0.7.json
+-rw-r--r--   0        0        0     1227 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP115(EU)_1.0_1.0.16.json
+-rw-r--r--   0        0        0     1213 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP115(US)_1.0_1.0.17.json
+-rw-r--r--   0        0        0     1230 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP125(US)_1.0_1.0.6.json
+-rw-r--r--   0        0        0     2036 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP303(UK)_1.0_1.0.3.json
+-rw-r--r--   0        0        0     1738 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP303(US)_2.0_1.0.3.json
+-rw-r--r--   0        0        0     1843 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP400(US)_1.0_1.0.10.json
+-rw-r--r--   0        0        0     1431 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP400(US)_2.0_1.0.6.json
+-rw-r--r--   0        0        0      966 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP401(US)_1.0_1.0.0.json
+-rw-r--r--   0        0        0     1892 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KP405(US)_1.0_1.0.5.json
+-rw-r--r--   0        0        0     2842 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KS200M(US)_1.0_1.0.8.json
+-rw-r--r--   0        0        0     3684 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KS220M(US)_1.0_1.0.4.json
+-rw-r--r--   0        0        0     1836 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/KS230(US)_1.0_1.0.14.json
+-rw-r--r--   0        0        0     3062 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/LB100(US)_1.0_mocked.json
+-rw-r--r--   0        0        0     2684 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/LB110(US)_1.0_1.8.11.json
+-rw-r--r--   0        0        0     3067 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/LB120(US)_1.0_mocked.json
+-rw-r--r--   0        0        0     3106 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/fixtures/LB130(US)_1.0_mocked.json
+-rw-r--r--   0        0        0    16115 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/newfakes.py
+-rw-r--r--   0        0        0     8947 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_bulb.py
+-rw-r--r--   0        0        0     3210 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_cli.py
+-rw-r--r--   0        0        0     3573 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_dimmer.py
+-rw-r--r--   0        0        0     4241 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_discovery.py
+-rw-r--r--   0        0        0     2997 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_emeter.py
+-rw-r--r--   0        0        0     2142 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_lightstrip.py
+-rw-r--r--   0        0        0      593 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_plug.py
+-rw-r--r--   0        0        0     5611 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_protocol.py
+-rw-r--r--   0        0        0     2545 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_readme_examples.py
+-rw-r--r--   0        0        0     4014 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_smartdevice.py
+-rw-r--r--   0        0        0     4056 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_strip.py
+-rw-r--r--   0        0        0      576 2023-07-02 14:29:08.874189 python_kasa-0.5.2/kasa/tests/test_usage.py
+-rw-r--r--   0        0        0     2410 2023-07-02 14:29:08.874189 python_kasa-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8043 1970-01-01 00:00:00.000000 python_kasa-0.5.2/PKG-INFO
```

### Comparing `python_kasa-0.5.1/CHANGELOG.md` & `python_kasa-0.5.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 # Changelog
 
+## [0.5.2](https://github.com/python-kasa/python-kasa/tree/0.5.2) (2023-07-02)
+
+[Full Changelog](https://github.com/python-kasa/python-kasa/compare/0.5.1...0.5.2)
+
+Besides some small improvements, this release:
+* Adds optional dependency for for `orjson` and `kasa-crypt` to speed-up protocol handling by an order of magnitude.
+* Drops Python 3.7 support as it is no longer maintained.
+
+**Breaking changes:**
+
+- Drop python 3.7 support [\#455](https://github.com/python-kasa/python-kasa/pull/455) (@rytilahti)
+
+**Implemented enhancements:**
+
+- Use orjson when already installed or with speedups extra [\#466](https://github.com/python-kasa/python-kasa/pull/466) (@bdraco)
+- Add optional kasa-crypt dependency for speedups [\#464](https://github.com/python-kasa/python-kasa/pull/464) (@bdraco)
+- Add inactivity setting for the motion module [\#453](https://github.com/python-kasa/python-kasa/pull/453) (@rytilahti)
+- Add methods to configure dimmer settings [\#429](https://github.com/python-kasa/python-kasa/pull/429) (@rytilahti)
+
+**Fixed bugs:**
+
+- Request for KP405 Support - Dimmable Plug [\#469](https://github.com/python-kasa/python-kasa/issues/469)
+- Issue printing device in on\_discovered: pydantic.error\_wrappers.ValidationError: 3 validation errors for SmartBulbPreset [\#439](https://github.com/python-kasa/python-kasa/issues/439)
+- Possible firmware issue with KL125 \(1.0.7 Build 211009 Rel.172044\) [\#345](https://github.com/python-kasa/python-kasa/issues/345)
+- Exclude querying certain modules for KL125\(US\) which cause crashes  [\#451](https://github.com/python-kasa/python-kasa/pull/451) (@brianthedavis)
+- Return result objects for cli discover and implicit 'state' [\#446](https://github.com/python-kasa/python-kasa/pull/446) (@rytilahti)
+- Allow effect presets seen on light strips [\#440](https://github.com/python-kasa/python-kasa/pull/440) (@rytilahti)
+
+**Closed issues:**
+
+- Powershell version? [\#461](https://github.com/python-kasa/python-kasa/issues/461)
+- Add `set_cold_time` to Motion module [\#452](https://github.com/python-kasa/python-kasa/issues/452)
+- Discover.discover\(\) only returning ip adress on ep10 outlet [\#447](https://github.com/python-kasa/python-kasa/issues/447)
+- Query current wifi config? [\#445](https://github.com/python-kasa/python-kasa/issues/445)
+- bulb.turn\_off making device undiscoverable [\#444](https://github.com/python-kasa/python-kasa/issues/444)
+- best privacy practices for Kasa devices [\#438](https://github.com/python-kasa/python-kasa/issues/438)
+- Access device from different network [\#424](https://github.com/python-kasa/python-kasa/issues/424)
+- Lots of test failure with 0.5.0 [\#411](https://github.com/python-kasa/python-kasa/issues/411)
+
+**Merged pull requests:**
+
+- Add benchmarks for speedups [\#473](https://github.com/python-kasa/python-kasa/pull/473) (@bdraco)
+- Add fixture for KP405 Smart Dimmer Plug [\#470](https://github.com/python-kasa/python-kasa/pull/470) (@xinud190)
+- Remove importlib-metadata dependency [\#457](https://github.com/python-kasa/python-kasa/pull/457) (@rytilahti)
+- Update dependencies to fix CI [\#454](https://github.com/python-kasa/python-kasa/pull/454) (@rytilahti)
+- Cleanup fixture filenames [\#448](https://github.com/python-kasa/python-kasa/pull/448) (@rytilahti)
+
 ## [0.5.1](https://github.com/python-kasa/python-kasa/tree/0.5.1) (2023-02-18)
 
 [Full Changelog](https://github.com/python-kasa/python-kasa/compare/0.5.0...0.5.1)
 
 This minor release contains mostly small UX fine-tuning and documentation improvements alongside with bug fixes:
 * Improved console tool (JSON output, colorized output if rich is installed)
 * Pretty, colorized console output, if `rich` is installed
@@ -13,30 +60,30 @@
 
 **Breaking changes:**
 
 - Implement changing the bulb turn-on behavior [\#381](https://github.com/python-kasa/python-kasa/pull/381) (@rytilahti)
 
 **Implemented enhancements:**
 
-- Add support for json output [\#430](https://github.com/python-kasa/python-kasa/pull/430) (@rytilahti)
 - Pretty-print all exceptions from cli commands [\#428](https://github.com/python-kasa/python-kasa/pull/428) (@rytilahti)
 - Add transition parameter to lightstrip's set\_effect [\#416](https://github.com/python-kasa/python-kasa/pull/416) (@rytilahti)
 - Add brightness to lightstrip's set\_effect [\#415](https://github.com/python-kasa/python-kasa/pull/415) (@rytilahti)
 - Use rich for prettier output, if available [\#403](https://github.com/python-kasa/python-kasa/pull/403) (@rytilahti)
 - Adding cli command to delete a schedule rule [\#391](https://github.com/python-kasa/python-kasa/pull/391) (@aricforrest)
 - Add support for bulb presets [\#379](https://github.com/python-kasa/python-kasa/pull/379) (@rytilahti)
+- Add support for json output [\#430](https://github.com/python-kasa/python-kasa/pull/430) (@rytilahti)
 
 **Fixed bugs:**
 
 - cli.py usage year and month options do not output data as expected [\#373](https://github.com/python-kasa/python-kasa/issues/373)
 - cli.py usage --year command passes year argument incorrectly [\#371](https://github.com/python-kasa/python-kasa/issues/371)
 - KP303 reporting as device off [\#319](https://github.com/python-kasa/python-kasa/issues/319)
 - HS210 not updating the state correctly [\#193](https://github.com/python-kasa/python-kasa/issues/193)
-- Return usage.get\_{monthstat,daystat} in expected format  [\#394](https://github.com/python-kasa/python-kasa/pull/394) (@jules43)
 - Fix year emeter for cli by using kwarg for year parameter [\#372](https://github.com/python-kasa/python-kasa/pull/372) (@rytilahti)
+- Return usage.get\_{monthstat,daystat} in expected format  [\#394](https://github.com/python-kasa/python-kasa/pull/394) (@jules43)
 
 **Documentation updates:**
 
 - Update misleading docs about supported devices \(was: add support for EP25 plug\) [\#367](https://github.com/python-kasa/python-kasa/issues/367)
 - Minor fixes to smartbulb docs [\#431](https://github.com/python-kasa/python-kasa/pull/431) (@rytilahti)
 - Add a note that transition is not supported by all devices [\#398](https://github.com/python-kasa/python-kasa/pull/398) (@rytilahti)
 - fix more outdated CLI examples, remove EP40 from bulb list [\#383](https://github.com/python-kasa/python-kasa/pull/383) (@HankB)
@@ -72,14 +119,15 @@
 - Error using Kasa [\#346](https://github.com/python-kasa/python-kasa/issues/346)
 - KS220M\(US\) support [\#268](https://github.com/python-kasa/python-kasa/issues/268)
 - Add machine-readable output [\#209](https://github.com/python-kasa/python-kasa/issues/209)
 - Can we donate? [\#77](https://github.com/python-kasa/python-kasa/issues/77)
 
 **Merged pull requests:**
 
+- Prepare 0.5.1 [\#434](https://github.com/python-kasa/python-kasa/pull/434) (@rytilahti)
 - Some release preparation janitoring [\#432](https://github.com/python-kasa/python-kasa/pull/432) (@rytilahti)
 - Bump certifi from 2021.10.8 to 2022.12.7 [\#409](https://github.com/python-kasa/python-kasa/pull/409) (@dependabot[bot])
 - Add FUNDING.yml [\#402](https://github.com/python-kasa/python-kasa/pull/402) (@rytilahti)
 - Update pre-commit hooks [\#401](https://github.com/python-kasa/python-kasa/pull/401) (@rytilahti)
 - Update pre-commit url for flake8 [\#400](https://github.com/python-kasa/python-kasa/pull/400) (@rytilahti)
 - Added .gitattributes file to retain LF only EOL markers when checking out on Windows [\#399](https://github.com/python-kasa/python-kasa/pull/399) (@jules43)
 - Fix pytest warnings about asyncio [\#397](https://github.com/python-kasa/python-kasa/pull/397) (@jules43)
```

### Comparing `python_kasa-0.5.1/LICENSE` & `python_kasa-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/README.md` & `python_kasa-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 ## Getting started
 
 You can install the most recent release using pip:
 ```
 pip install python-kasa
 ```
 
+If you are using cpython, it is recommended to install with `[speedups]` to enable orjson (faster json support):
+```
+pip install python-kasa[speedups]
+```
+
+With `[speedups]`, the protocol overhead is roughly an order of magnitude lower (benchmarks available in devtools).
+
 Alternatively, you can clone this repository and use poetry to install the development version:
 ```
 git clone https://github.com/python-kasa/python-kasa.git
 cd python-kasa/
 poetry install
 ```
 
@@ -135,14 +142,15 @@
 
 ### Power Strips
 
 * EP40
 * HS300
 * KP303
 * KP400
+* KP405 (dimmer)
 
 ### Wall switches
 
 * ES20M
 * HS200
 * HS210
 * HS220
```

### Comparing `python_kasa-0.5.1/kasa/__init__.py` & `python_kasa-0.5.2/kasa/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 For device type specific actions `SmartBulb`, `SmartPlug`, or `SmartStrip`
  should be used instead.
 
 Module-specific errors are raised as `SmartDeviceException` and are expected
 to be handled by the user of the library.
 """
-from importlib_metadata import version  # type: ignore
+from importlib.metadata import version
 
 from kasa.discover import Discover
 from kasa.emeterstatus import EmeterStatus
 from kasa.exceptions import SmartDeviceException
 from kasa.protocol import TPLinkSmartHomeProtocol
 from kasa.smartbulb import SmartBulb, SmartBulbPreset, TurnOnBehavior, TurnOnBehaviors
 from kasa.smartdevice import DeviceType, SmartDevice
```

### Comparing `python_kasa-0.5.1/kasa/cli.py` & `python_kasa-0.5.2/kasa/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,28 +169,27 @@
             echo(f"Found hostname is {host}")
         else:
             echo(f"No device with name {alias} found")
             return
 
     if host is None:
         echo("No host name given, trying discovery..")
-        await ctx.invoke(discover)
-        return
+        return await ctx.invoke(discover)
 
     if type is not None:
         dev = TYPE_TO_CLASS[type](host)
     else:
         echo("No --type defined, discovering..")
         dev = await Discover.discover_single(host)
 
     await dev.update()
     ctx.obj = dev
 
     if ctx.invoked_subcommand is None:
-        await ctx.invoke(state)
+        return await ctx.invoke(state)
 
 
 @cli.group()
 @pass_dev
 def wifi(dev):
     """Commands to control wifi settings."""
 
@@ -228,26 +227,30 @@
 @click.option("--timeout", default=3, required=False)
 @click.pass_context
 async def discover(ctx, timeout):
     """Discover devices in the network."""
     target = ctx.parent.params["target"]
     echo(f"Discovering devices on {target} for {timeout} seconds")
     sem = asyncio.Semaphore()
+    discovered = dict()
 
     async def print_discovered(dev: SmartDevice):
         await dev.update()
         async with sem:
+            discovered[dev.host] = dev.internal_state
             ctx.obj = dev
             await ctx.invoke(state)
             echo()
 
-    return await Discover.discover(
+    await Discover.discover(
         target=target, timeout=timeout, on_discovered=print_discovered
     )
 
+    return discovered
+
 
 async def find_host_from_alias(alias, target="255.255.255.255", timeout=1, attempts=3):
     """Discover a device identified by its alias."""
     for attempt in range(1, attempts):
         found_devs = await Discover.discover(target=target, timeout=timeout)
         for ip, dev in found_devs.items():
             if dev.alias.lower() == alias.lower():
```

### Comparing `python_kasa-0.5.1/kasa/discover.py` & `python_kasa-0.5.2/kasa/discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Discovery module for TP-Link Smart Home devices."""
 import asyncio
-import json
 import logging
 import socket
 from typing import Awaitable, Callable, Dict, Optional, Type, cast
 
+from kasa.json import dumps as json_dumps
+from kasa.json import loads as json_loads
 from kasa.protocol import TPLinkSmartHomeProtocol
 from kasa.smartbulb import SmartBulb
 from kasa.smartdevice import SmartDevice, SmartDeviceException
 from kasa.smartdimmer import SmartDimmer
 from kasa.smartlightstrip import SmartLightStrip
 from kasa.smartplug import SmartPlug
 from kasa.smartstrip import SmartStrip
@@ -59,27 +60,27 @@
                 socket.SOL_SOCKET, socket.SO_BINDTODEVICE, self.interface.encode()
             )
 
         self.do_discover()
 
     def do_discover(self) -> None:
         """Send number of discovery datagrams."""
-        req = json.dumps(Discover.DISCOVERY_QUERY)
+        req = json_dumps(Discover.DISCOVERY_QUERY)
         _LOGGER.debug("[DISCOVERY] %s >> %s", self.target, Discover.DISCOVERY_QUERY)
         encrypted_req = TPLinkSmartHomeProtocol.encrypt(req)
         for i in range(self.discovery_packets):
             self.transport.sendto(encrypted_req[4:], self.target)  # type: ignore
 
     def datagram_received(self, data, addr) -> None:
         """Handle discovery responses."""
         ip, port = addr
         if ip in self.discovered_devices:
             return
 
-        info = json.loads(TPLinkSmartHomeProtocol.decrypt(data))
+        info = json_loads(TPLinkSmartHomeProtocol.decrypt(data))
         _LOGGER.debug("[DISCOVERY] %s << %s", ip, info)
 
         try:
             device_class = Discover._get_device_class(info)
         except SmartDeviceException as ex:
             _LOGGER.debug("Unable to find device type from %s: %s", info, ex)
             return
```

### Comparing `python_kasa-0.5.1/kasa/effects.py` & `python_kasa-0.5.2/kasa/effects.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/emeterstatus.py` & `python_kasa-0.5.2/kasa/emeterstatus.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/__init__.py` & `python_kasa-0.5.2/kasa/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/ambientlight.py` & `python_kasa-0.5.2/kasa/modules/ambientlight.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/cloud.py` & `python_kasa-0.5.2/kasa/modules/cloud.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/emeter.py` & `python_kasa-0.5.2/kasa/modules/emeter.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/module.py` & `python_kasa-0.5.2/kasa/modules/module.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/motion.py` & `python_kasa-0.5.2/kasa/modules/motion.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,7 +55,20 @@
             payload = {"index": range.value}
         else:
             raise SmartDeviceException(
                 "Either range or custom_range need to be defined"
             )
 
         return await self.call("set_trigger_sens", payload)
+
+    @property
+    def inactivity_timeout(self) -> int:
+        """Return inactivity timeout in milliseconds."""
+        return self.data["cold_time"]
+
+    async def set_inactivity_timeout(self, timeout: int):
+        """Set inactivity timeout in milliseconds.
+
+        Note, that you need to delete the default "Smart Control" rule in the app
+        to avoid reverting this back to 60 seconds after a period of time.
+        """
+        return await self.call("set_cold_time", {"cold_time": timeout})
```

### Comparing `python_kasa-0.5.1/kasa/modules/rulemodule.py` & `python_kasa-0.5.2/kasa/modules/rulemodule.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/time.py` & `python_kasa-0.5.2/kasa/modules/time.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/modules/usage.py` & `python_kasa-0.5.2/kasa/modules/usage.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/protocol.py` & `python_kasa-0.5.2/kasa/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 which are licensed under the Apache License, Version 2.0
 http://www.apache.org/licenses/LICENSE-2.0
 """
 import asyncio
 import contextlib
 import errno
-import json
 import logging
 import struct
 from pprint import pformat as pf
 from typing import Dict, Generator, Optional, Union
 
 from .exceptions import SmartDeviceException
+from .json import dumps as json_dumps
+from .json import loads as json_loads
 
 _LOGGER = logging.getLogger(__name__)
 _NO_RETRY_ERRORS = {errno.EHOSTDOWN, errno.EHOSTUNREACH, errno.ECONNREFUSED}
 
 
 class TPLinkSmartHomeProtocol:
     """Implementation of the TP-Link Smart Home protocol."""
@@ -60,15 +61,15 @@
         """
         self._detect_event_loop_change()
 
         if not self.query_lock:
             self.query_lock = asyncio.Lock()
 
         if isinstance(request, dict):
-            request = json.dumps(request)
+            request = json_dumps(request)
             assert isinstance(request, str)
 
         timeout = TPLinkSmartHomeProtocol.DEFAULT_TIMEOUT
 
         async with self.query_lock:
             return await self._query(request, retry_count, timeout)
 
@@ -92,15 +93,15 @@
         await self.writer.drain()
 
         packed_block_size = await self.reader.readexactly(self.BLOCK_SIZE)
         length = struct.unpack(">I", packed_block_size)[0]
 
         buffer = await self.reader.readexactly(length)
         response = TPLinkSmartHomeProtocol.decrypt(buffer)
-        json_payload = json.loads(response)
+        json_payload = json_loads(response)
         if debug_log:
             _LOGGER.debug("%s << %s", self.host, pf(json_payload))
 
         return json_payload
 
     async def close(self) -> None:
         """Close the connection."""
@@ -214,7 +215,17 @@
 
         :param ciphertext: encrypted response data
         :return: plaintext response
         """
         return bytes(
             TPLinkSmartHomeProtocol._xor_encrypted_payload(ciphertext)
         ).decode()
+
+
+# Try to load the kasa_crypt module and if it is available
+try:
+    from kasa_crypt import decrypt, encrypt
+
+    TPLinkSmartHomeProtocol.decrypt = decrypt  # type: ignore[method-assign]
+    TPLinkSmartHomeProtocol.encrypt = encrypt  # type: ignore[method-assign]
+except ImportError:
+    pass
```

### Comparing `python_kasa-0.5.1/kasa/smartbulb.py` & `python_kasa-0.5.2/kasa/smartbulb.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,24 @@
 
 
 class SmartBulbPreset(BaseModel):
     """Bulb configuration preset."""
 
     index: int
     brightness: int
-    hue: int
-    saturation: int
-    color_temp: int
+
+    # These are not available for effect mode presets on light strips
+    hue: Optional[int]
+    saturation: Optional[int]
+    color_temp: Optional[int]
+
+    # Variables for effect mode presets
+    custom: Optional[int]
+    id: Optional[str]
+    mode: Optional[int]
 
 
 class BehaviorMode(str, Enum):
     """Enum to present type of turn on behavior."""
 
     #: Return to the last state known state.
     Last = "last_status"
@@ -116,15 +123,15 @@
     and should be handled by the user of the library.
 
     Examples:
         >>> import asyncio
         >>> bulb = SmartBulb("127.0.0.1")
         >>> asyncio.run(bulb.update())
         >>> print(bulb.alias)
-        KL130 office bulb
+        Bulb2
 
         Bulbs, like any other supported devices, can be turned on and off:
 
         >>> asyncio.run(bulb.turn_off())
         >>> asyncio.run(bulb.turn_on())
         >>> asyncio.run(bulb.update())
         >>> print(bulb.is_on)
@@ -170,15 +177,15 @@
         The following changes the brightness over a period of 10 seconds:
 
         >>> asyncio.run(bulb.set_brightness(100, transition=10_000))
 
         Bulb configuration presets can be accessed using the :func:`presets` property:
 
         >>> bulb.presets
-        [SmartBulbPreset(index=0, brightness=50, hue=0, saturation=0, color_temp=2700), SmartBulbPreset(index=1, brightness=100, hue=0, saturation=75, color_temp=0), SmartBulbPreset(index=2, brightness=100, hue=120, saturation=75, color_temp=0), SmartBulbPreset(index=3, brightness=100, hue=240, saturation=75, color_temp=0)]
+        [SmartBulbPreset(index=0, brightness=50, hue=0, saturation=0, color_temp=2700, custom=None, id=None, mode=None), SmartBulbPreset(index=1, brightness=100, hue=0, saturation=75, color_temp=0, custom=None, id=None, mode=None), SmartBulbPreset(index=2, brightness=100, hue=120, saturation=75, color_temp=0, custom=None, id=None, mode=None), SmartBulbPreset(index=3, brightness=100, hue=240, saturation=75, color_temp=0, custom=None, id=None, mode=None)]
 
         To modify an existing preset, pass :class:`~kasa.smartbulb.SmartBulbPreset` instance to :func:`save_preset` method:
 
         >>> preset = bulb.presets[0]
         >>> preset.brightness
         50
         >>> preset.brightness = 100
@@ -510,19 +517,19 @@
     def presets(self) -> List[SmartBulbPreset]:
         """Return a list of available bulb setting presets."""
         return [SmartBulbPreset(**vals) for vals in self.sys_info["preferred_state"]]
 
     async def save_preset(self, preset: SmartBulbPreset):
         """Save a setting preset.
 
-        You can either construct a preset object manually, or pass an existing one obtained
+        You can either construct a preset object manually, or pass an existing one
         obtained using :func:`presets`.
         """
         if len(self.presets) == 0:
             raise SmartDeviceException("Device does not supported saving presets")
 
         if preset.index >= len(self.presets):
             raise SmartDeviceException("Invalid preset index")
 
         return await self._query_helper(
-            self.LIGHT_SERVICE, "set_preferred_state", preset.dict()
+            self.LIGHT_SERVICE, "set_preferred_state", preset.dict(exclude_none=True)
         )
```

### Comparing `python_kasa-0.5.1/kasa/smartdevice.py` & `python_kasa-0.5.2/kasa/smartdevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 from .emeterstatus import EmeterStatus
 from .exceptions import SmartDeviceException
 from .modules import Emeter, Module
 from .protocol import TPLinkSmartHomeProtocol
 
 _LOGGER = logging.getLogger(__name__)
 
+# Certain module queries will crash devices; this list skips those queries
+MODEL_MODULE_SKIPLIST = {"KL125(US)": ["cloud"]}  # Issue #345
+
 
 class DeviceType(Enum):
     """Device type enum."""
 
     Plug = auto()
     Bulb = auto()
     Strip = auto()
@@ -321,18 +324,23 @@
         """Execute an update query."""
         if self.has_emeter:
             _LOGGER.debug(
                 "The device has emeter, querying its information along sysinfo"
             )
             self.add_module("emeter", Emeter(self, self.emeter_type))
 
-        for module in self.modules.values():
+        for module_name, module in self.modules.items():
             if not module.is_supported:
                 _LOGGER.debug("Module %s not supported, skipping" % module)
                 continue
+            modules_to_skip = MODEL_MODULE_SKIPLIST.get(self.model, [])
+            if module_name in modules_to_skip:
+                _LOGGER.debug(f"Module {module} is excluded for {self.model}, skipping")
+                continue
+
             q = module.query()
             _LOGGER.debug("Adding query for %s: %s", module, q)
             req = merge(req, q)
 
         self._last_update = await self.protocol.query(req)
 
     def update_from_discover_info(self, info):
```

### Comparing `python_kasa-0.5.1/kasa/smartdimmer.py` & `python_kasa-0.5.2/kasa/smartdimmer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,39 @@
 """Module for dimmers (currently only HS220)."""
+from enum import Enum
 from typing import Any, Dict, Optional
 
 from kasa.modules import AmbientLight, Motion
 from kasa.smartdevice import DeviceType, SmartDeviceException, requires_update
 from kasa.smartplug import SmartPlug
 
 
+class ButtonAction(Enum):
+    """Button action."""
+
+    NoAction = "none"
+    Instant = "instant_on_off"
+    Gentle = "gentle_on_off"
+    Preset = "customize_preset"
+
+
+class ActionType(Enum):
+    """Button action."""
+
+    DoubleClick = "double_click_action"
+    LongPress = "long_press_action"
+
+
+class FadeType(Enum):
+    """Fade on/off setting."""
+
+    FadeOn = "fade_on"
+    FadeOff = "fade_off"
+
+
 class SmartDimmer(SmartPlug):
     r"""Representation of a TP-Link Smart Dimmer.
 
     Dimmers work similarly to plugs, but provide also support for
     adjusting the brightness. This class extends :class:`SmartPlug` interface.
 
     To initialize, you have to await :func:`update()` at least once.
@@ -136,14 +160,48 @@
 
         return await self._query_helper(
             self.DIMMER_SERVICE,
             "set_dimmer_transition",
             {"brightness": brightness, "duration": transition},
         )
 
+    @requires_update
+    async def get_behaviors(self):
+        """Return button behavior settings."""
+        behaviors = await self._query_helper(
+            self.DIMMER_SERVICE, "get_default_behavior", {}
+        )
+        return behaviors
+
+    @requires_update
+    async def set_button_action(
+        self, action_type: ActionType, action: ButtonAction, index: Optional[int] = None
+    ):
+        """Set action to perform on button click/hold.
+
+        :param action_type ActionType: whether to control double click or hold action.
+        :param action ButtonAction: what should the button do (nothing, instant, gentle, change preset)
+        :param index int: in case of preset change, the preset to select
+        """
+        action_type_setter = f"set_{action_type}"
+
+        payload: Dict[str, Any] = {"mode": str(action)}
+        if index is not None:
+            payload["index"] = index
+
+        await self._query_helper(self.DIMMER_SERVICE, action_type_setter, payload)
+
+    @requires_update
+    async def set_fade_time(self, fade_type: FadeType, time: int):
+        """Set time for fade in / fade out."""
+        fade_type_setter = f"set_{fade_type}_time"
+        payload = {"fadeTime": time}
+
+        await self._query_helper(self.DIMMER_SERVICE, fade_type_setter, payload)
+
     @property  # type: ignore
     @requires_update
     def is_dimmable(self) -> bool:
         """Whether the switch supports brightness changes."""
         sys_info = self.sys_info
         return "brightness" in sys_info
```

### Comparing `python_kasa-0.5.1/kasa/smartlightstrip.py` & `python_kasa-0.5.2/kasa/smartlightstrip.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/smartplug.py` & `python_kasa-0.5.2/kasa/smartplug.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/smartstrip.py` & `python_kasa-0.5.2/kasa/smartstrip.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/conftest.py` & `python_kasa-0.5.2/kasa/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "KP105",
     "KP115",
     "KP125",
     "KP401",
     "KS200M",
 }
 STRIPS = {"HS107", "HS300", "KP303", "KP400", "EP40"}
-DIMMERS = {"ES20M", "HS220", "KS220M", "KS230"}
+DIMMERS = {"ES20M", "HS220", "KS220M", "KS230", "KP405"}
 
 DIMMABLE = {*BULBS, *DIMMERS}
 WITH_EMETER = {"HS110", "HS300", "KP115", "KP125", *BULBS}
 
 ALL_DEVICES = BULBS.union(PLUGS).union(STRIPS).union(DIMMERS)
 
 IP_MODEL_CACHE: Dict[str, str] = {}
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/EP10(US)_1.0_1.0.2.json` & `python_kasa-0.5.2/kasa/tests/fixtures/EP10(US)_1.0_1.0.2.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/EP40(US)_1.0_1.0.2.json` & `python_kasa-0.5.2/kasa/tests/fixtures/EP40(US)_1.0_1.0.2.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/ES20M(US)_1.0_1.0.8.json` & `python_kasa-0.5.2/kasa/tests/fixtures/ES20M(US)_1.0_1.0.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS100(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS103(US)_1.0_1.5.7.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9810000000000001%*

 * *Differences: {"'system'": "{'get_sysinfo': {'alias': 'Night lite', 'dev_name': 'Smart Wi-Fi Plug Lite', "*

 * *             "'deviceId': '0000000000000000000000000000000000000000', 'hwId': "*

 * *             "'00000000000000000000000000000000', 'latitude_i': 0, 'longitude_i': 0, 'mac': "*

 * *             "'00:00:00:00:00:00', 'model': 'HS103(US)', 'oemId': "*

 * *             "'00000000000000000000000000000000', 'rssi': -43, 'sw_ver': '1.5.7 Build 191114 "*

 * *             "Rel.105922', 'fwId': '00000000000000000000000000000000', 'next_actio […]*

```diff
@@ -16,32 +16,37 @@
     "smartlife.iot.smartbulb.lightingservice": {
         "err_code": -1,
         "err_msg": "module not support"
     },
     "system": {
         "get_sysinfo": {
             "active_mode": "schedule",
-            "alias": "Mock hs100",
-            "dev_name": "Wi-Fi Smart Plug",
-            "deviceId": "048F069965D3230FD1382F0B78EAE68D42CAA2DE",
+            "alias": "Night lite",
+            "dev_name": "Smart Wi-Fi Plug Lite",
+            "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
             "feature": "TIM",
-            "hwId": "92688D028799C60F926049D1C9EFD9E8",
+            "fwId": "00000000000000000000000000000000",
+            "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
             "icon_hash": "",
-            "latitude": 63.5442,
-            "latitude_i": 63.5442,
+            "latitude_i": 0,
             "led_off": 0,
-            "longitude": -148.2817,
-            "longitude_i": -148.2817,
-            "mac": "50:c7:bf:a3:71:c0",
-            "model": "HS100(US)",
-            "oemId": "149C8A24AA3A1445DE84F00DFB210D60",
+            "longitude_i": 0,
+            "mac": "00:00:00:00:00:00",
+            "model": "HS103(US)",
+            "next_action": {
+                "action": 1,
+                "id": "F98589DFF09AEA1D5AC2BDB4A8867305",
+                "schd_sec": 75600,
+                "type": 1
+            },
+            "oemId": "00000000000000000000000000000000",
             "on_time": 0,
             "relay_state": 0,
-            "rssi": -65,
-            "sw_ver": "1.2.5 Build 171129 Rel.174814",
+            "rssi": -43,
+            "sw_ver": "1.5.7 Build 191114 Rel.105922",
             "type": "IOT.SMARTPLUGSWITCH",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS100(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS100(US)_1.0_1.2.5.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS100(US)_2.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS100(US)_2.0_1.5.6.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS103(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS210(US)_1.0_1.5.8.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.987125%*

 * *Differences: {"'system'": "{'get_sysinfo': {'active_mode': 'none', 'alias': 'Garage Light', 'dev_name': 'Smart "*

 * *             "Wi-Fi 3-Way Light Switch', 'model': 'HS210(US)', 'next_action': {'type': -1, delete: "*

 * *             "['action', 'id', 'schd_sec']}, 'rssi': -52, 'sw_ver': '1.5.8 Build 191118 "*

 * *             "Rel.135937', 'abnormal_detect': 1, 'mic_type': 'IOT.SMARTPLUGSWITCH', delete: "*

 * *             "['type']}}"}*

```diff
@@ -15,38 +15,36 @@
     },
     "smartlife.iot.smartbulb.lightingservice": {
         "err_code": -1,
         "err_msg": "module not support"
     },
     "system": {
         "get_sysinfo": {
-            "active_mode": "schedule",
-            "alias": "Night lite",
-            "dev_name": "Smart Wi-Fi Plug Lite",
+            "abnormal_detect": 1,
+            "active_mode": "none",
+            "alias": "Garage Light",
+            "dev_name": "Smart Wi-Fi 3-Way Light Switch",
             "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
             "feature": "TIM",
             "fwId": "00000000000000000000000000000000",
             "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
             "icon_hash": "",
             "latitude_i": 0,
             "led_off": 0,
             "longitude_i": 0,
             "mac": "00:00:00:00:00:00",
-            "model": "HS103(US)",
+            "mic_type": "IOT.SMARTPLUGSWITCH",
+            "model": "HS210(US)",
             "next_action": {
-                "action": 1,
-                "id": "F98589DFF09AEA1D5AC2BDB4A8867305",
-                "schd_sec": 75600,
-                "type": 1
+                "type": -1
             },
             "oemId": "00000000000000000000000000000000",
             "on_time": 0,
             "relay_state": 0,
-            "rssi": -43,
-            "sw_ver": "1.5.7 Build 191114 Rel.105922",
-            "type": "IOT.SMARTPLUGSWITCH",
+            "rssi": -52,
+            "sw_ver": "1.5.8 Build 191118 Rel.135937",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS103(US)_2.1.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS103(US)_2.1_1.1.2.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS103(US)_2.1_1.1.4.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS103(US)_2.1_1.1.4.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS105(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS105(US)_1.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS105(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS105(US)_1.0_1.5.6.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS107(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS107(US)_1.0_1.0.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS110(EU)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS110(EU)_1.0_1.2.5.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS110(EU)_2.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS110(EU)_2.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS110(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS110(US)_1.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS200(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS200(US)_1.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS200(US)_2.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS200(US)_2.0_1.5.7.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS200(US)_5.0_1.0.2.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS200(US)_5.0_1.0.2.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS210(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP125(US)_1.0_1.0.6.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3375%*

 * *Differences: {"'emeter'": "{'get_realtime': {'err_code': 0, 'current_ma': 978, 'power_mw': 100277, 'total_wh': "*

 * *             "12170, 'voltage_mv': 119425, delete: ['err_msg']}}",*

 * * "'system'": "{'get_sysinfo': {'alias': 'Test plug', 'dev_name': 'Smart Wi-Fi Plug Mini', "*

 * *             "'feature': 'TIM:ENE', 'model': 'KP125(US)', 'on_time': 301, 'relay_state': 1, "*

 * *             "'rssi': -41, 'sw_ver': '1.0.6 Build 210928 Rel.185924', 'ntc_state': 0, 'obd_src': "*

 * *             "'tplink', 'status': 'configured', delete: ['ab […]*

```diff
@@ -1,50 +1,42 @@
 {
     "emeter": {
         "get_realtime": {
-            "err_code": -1,
-            "err_msg": "module not support"
+            "current_ma": 978,
+            "err_code": 0,
+            "power_mw": 100277,
+            "total_wh": 12170,
+            "voltage_mv": 119425
         }
     },
-    "smartlife.iot.common.emeter": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
-    "smartlife.iot.dimmer": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
-    "smartlife.iot.smartbulb.lightingservice": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
     "system": {
         "get_sysinfo": {
-            "abnormal_detect": 1,
             "active_mode": "none",
-            "alias": "Garage Light",
-            "dev_name": "Smart Wi-Fi 3-Way Light Switch",
+            "alias": "Test plug",
+            "dev_name": "Smart Wi-Fi Plug Mini",
             "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
-            "feature": "TIM",
-            "fwId": "00000000000000000000000000000000",
+            "feature": "TIM:ENE",
             "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
             "icon_hash": "",
             "latitude_i": 0,
             "led_off": 0,
             "longitude_i": 0,
             "mac": "00:00:00:00:00:00",
             "mic_type": "IOT.SMARTPLUGSWITCH",
-            "model": "HS210(US)",
+            "model": "KP125(US)",
             "next_action": {
                 "type": -1
             },
+            "ntc_state": 0,
+            "obd_src": "tplink",
             "oemId": "00000000000000000000000000000000",
-            "on_time": 0,
-            "relay_state": 0,
-            "rssi": -52,
-            "sw_ver": "1.5.8 Build 191118 Rel.135937",
+            "on_time": 301,
+            "relay_state": 1,
+            "rssi": -41,
+            "status": "configured",
+            "sw_ver": "1.0.6 Build 210928 Rel.185924",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS220(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS220(US)_1.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS220(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS220(US)_1.0_1.5.7.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS220(US)_2.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS220(US)_2.0_1.0.3.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS300(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/LB130(US)_1.0_mocked.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6614285714285714%*

 * *Differences: {"'emeter'": "{replace: OrderedDict([('err_code', -1), ('err_msg', 'module not support')])}",*

 * * "'smartlife.iot.common.emeter'": "{replace: OrderedDict([('get_realtime', "*

 * *                                  "OrderedDict([('err_code', 0), ('power_mw', 10800)]))])}",*

 * * "'smartlife.iot.smartbulb.lightingservice'": "{replace: OrderedDict([('get_light_state', "*

 * *                                              "OrderedDict([('dft_on_state', "*

 * *                                              "OrderedDict([('brightness', 10 […]*

```diff
@@ -1,102 +1,104 @@
 {
     "emeter": {
+        "err_code": -1,
+        "err_msg": "module not support"
+    },
+    "smartlife.iot.common.emeter": {
         "get_realtime": {
-            "current_ma": 125,
             "err_code": 0,
-            "power_mw": 3140,
-            "total_wh": 51493,
-            "voltage_mv": 122049
+            "power_mw": 10800
         }
     },
-    "smartlife.iot.common.emeter": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
     "smartlife.iot.dimmer": {
         "err_code": -1,
         "err_msg": "module not support"
     },
     "smartlife.iot.smartbulb.lightingservice": {
-        "err_code": -1,
-        "err_msg": "module not support"
+        "get_light_state": {
+            "dft_on_state": {
+                "brightness": 100,
+                "color_temp": 2700,
+                "hue": 0,
+                "mode": "normal",
+                "saturation": 0
+            },
+            "err_code": 0,
+            "on_off": 0
+        }
     },
     "system": {
         "get_sysinfo": {
-            "alias": "Mock hs300",
-            "child_num": 6,
-            "children": [
-                {
-                    "alias": "Mock One",
-                    "id": "00",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 123,
-                    "state": 1
-                },
-                {
-                    "alias": "Mock Two",
-                    "id": "01",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 333,
-                    "state": 1
+            "INVALIDmac": "50:c7:bf:ac:f6:19",
+            "active_mode": "none",
+            "alias": "Mock lb130",
+            "ctrl_protocols": {
+                "name": "Linkie",
+                "version": "1.0"
+            },
+            "description": "Smart Wi-Fi LED Bulb with Color Changing",
+            "dev_state": "normal",
+            "deviceId": "50BE9E7B6F26CA75D495C13EAA459C491768F143",
+            "disco_ver": "1.0",
+            "err_code": 0,
+            "heapsize": 302452,
+            "hwId": "C8AD962B53417C2845CC10CE25C00BB1",
+            "hw_ver": "1.0",
+            "is_color": 1,
+            "is_dimmable": 1,
+            "is_factory": false,
+            "is_variable_color_temp": 1,
+            "latitude": 76.8649,
+            "latitude_i": 76.8649,
+            "light_state": {
+                "dft_on_state": {
+                    "brightness": 100,
+                    "color_temp": 2700,
+                    "hue": 0,
+                    "mode": "normal",
+                    "saturation": 0
                 },
-                {
-                    "alias": "Mock Three",
-                    "id": "02",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 0,
-                    "state": 0
+                "err_code": 0,
+                "on_off": 0
+            },
+            "longitude": -40.7284,
+            "longitude_i": -40.7284,
+            "mic_mac": "50C7BFACF619",
+            "mic_type": "IOT.SMARTBULB",
+            "model": "LB130(US)",
+            "oemId": "CF78964560AAB75A43F15D2E468B63EF",
+            "on_time": 0,
+            "preferred_state": [
+                {
+                    "brightness": 100,
+                    "color_temp": 2700,
+                    "hue": 0,
+                    "index": 0,
+                    "saturation": 0
                 },
                 {
-                    "alias": "Mock Four",
-                    "id": "03",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 0,
-                    "state": 0
+                    "brightness": 75,
+                    "color_temp": 2700,
+                    "hue": 0,
+                    "index": 1,
+                    "saturation": 0
                 },
                 {
-                    "alias": "Mock Five",
-                    "id": "04",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 0,
-                    "state": 0
+                    "brightness": 25,
+                    "color_temp": 2700,
+                    "hue": 0,
+                    "index": 2,
+                    "saturation": 0
                 },
                 {
-                    "alias": "Mock Six",
-                    "id": "05",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 0,
-                    "state": 0
+                    "brightness": 1,
+                    "color_temp": 2700,
+                    "hue": 0,
+                    "index": 3,
+                    "saturation": 0
                 }
             ],
-            "deviceId": "4BFC2F2C8678FE623700FD3737EC4E245196F3CF",
-            "err_code": 0,
-            "feature": "TIM:ENE",
-            "hwId": "1B63E5DF21B5AFB52F364DE66BFAAF8A",
-            "hw_ver": "1.0",
-            "latitude": -68.998,
-            "latitude_i": -68.998,
-            "led_off": 0,
-            "longitude": -109.44,
-            "longitude_i": -109.44,
-            "mac": "50:c7:bf:c2:75:88",
-            "mic_type": "IOT.SMARTPLUGSWITCH",
-            "model": "HS300(US)",
-            "oemId": "FC71DAAB004326F9369EDEF4353E4FE1",
-            "rssi": -68,
-            "sw_ver": "1.0.6 Build 180627 Rel.081000",
-            "updating": 0
+            "rssi": -65,
+            "sw_ver": "1.6.0 Build 170703 Rel.141938"
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS300(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS300(US)_1.0_1.0.10.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/HS300(US)_2.0_1.0.3.json` & `python_kasa-0.5.2/kasa/tests/fixtures/HS300(US)_2.0_1.0.3.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL110(US)_1.0_1.8.11.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL110(US)_1.0_1.8.11.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL120(US)_1.0_real.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL120(US)_1.0_1.8.6.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL125(US)_1.20_1.0.5.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL125(US)_1.20_1.0.5.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL125(US)_2.0_1.0.7.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL125(US)_2.0_1.0.7.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL130(EU)_1.0_1.8.8.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL130(EU)_1.0_1.8.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL130(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL130(US)_1.0_1.8.11.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5415178571428572%*

 * *Differences: {"'smartlife.iot.common.emeter'": "{'get_realtime': {'power_mw': 0}}",*

 * * "'smartlife.iot.smartbulb.lightingservice'": "{'get_light_state': {'on_off': 0, 'dft_on_state': "*

 * *                                              "OrderedDict([('brightness', 30), ('color_temp', 0), "*

 * *                                              "('hue', 240), ('mode', 'normal'), ('saturation', "*

 * *                                              "100)]), delete: ['brightness', 'color_temp', 'hue', "*

 * *                                           […]*

```diff
@@ -1,62 +1,58 @@
 {
-    "emeter": {
-        "err_code": -2001,
-        "err_msg": "Module not support"
-    },
     "smartlife.iot.common.emeter": {
         "get_realtime": {
             "err_code": 0,
-            "power_mw": 800
+            "power_mw": 0
         }
     },
-    "smartlife.iot.dimmer": {
-        "err_code": -2001,
-        "err_msg": "Module not support"
-    },
     "smartlife.iot.smartbulb.lightingservice": {
         "get_light_state": {
-            "brightness": 0,
-            "color_temp": 0,
+            "dft_on_state": {
+                "brightness": 30,
+                "color_temp": 0,
+                "hue": 240,
+                "mode": "normal",
+                "saturation": 100
+            },
             "err_code": 0,
-            "hue": 15,
-            "mode": "normal",
-            "on_off": 1,
-            "saturation": 100
+            "on_off": 0
         }
     },
     "system": {
         "get_sysinfo": {
             "active_mode": "none",
-            "alias": "KL130 office bulb",
+            "alias": "Bulb2",
             "ctrl_protocols": {
                 "name": "Linkie",
                 "version": "1.0"
             },
             "description": "Smart Wi-Fi LED Bulb with Color Changing",
             "dev_state": "normal",
             "deviceId": "0000000000000000000000000000000000000000",
             "disco_ver": "1.0",
             "err_code": 0,
-            "heapsize": 306332,
+            "heapsize": 305252,
             "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
             "is_color": 1,
             "is_dimmable": 1,
             "is_factory": false,
             "is_variable_color_temp": 1,
             "light_state": {
-                "brightness": 30,
-                "color_temp": 0,
-                "hue": 15,
-                "mode": "normal",
-                "on_off": 1,
-                "saturation": 100
+                "dft_on_state": {
+                    "brightness": 30,
+                    "color_temp": 0,
+                    "hue": 240,
+                    "mode": "normal",
+                    "saturation": 100
+                },
+                "on_off": 0
             },
-            "mic_mac": "1C3BF373CA4E",
+            "mic_mac": "000000000000",
             "mic_type": "IOT.SMARTBULB",
             "model": "KL130(US)",
             "oemId": "00000000000000000000000000000000",
             "preferred_state": [
                 {
                     "brightness": 50,
                     "color_temp": 2700,
@@ -82,12 +78,12 @@
                     "brightness": 100,
                     "color_temp": 0,
                     "hue": 240,
                     "index": 3,
                     "saturation": 75
                 }
             ],
-            "rssi": -62,
+            "rssi": -52,
             "sw_ver": "1.8.11 Build 191113 Rel.105336"
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL130(US)_1.0_1.8.11.json` & `python_kasa-0.5.2/kasa/tests/fixtures/LB110(US)_1.0_1.8.11.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9810386473429952%*

 * *Differences: {"'smartlife.iot.smartbulb.lightingservice'": "{'get_light_state': {'dft_on_state': {'brightness': "*

 * *                                              "100, 'color_temp': 2700, 'hue': 0, 'saturation': "*

 * *                                              '0}}}',*

 * * "'system'": "{'get_sysinfo': {'alias': 'TP-LINK_Smart Bulb_43EC', 'description': 'Smart Wi-Fi LED "*

 * *             "Bulb with Dimmable Light', 'heapsize': 290048, 'is_color': 0, "*

 * *             "'is_variable_color_temp': 0, 'light_state': {'dft_on_state': {'bri […]*

```diff
@@ -4,86 +4,86 @@
             "err_code": 0,
             "power_mw": 0
         }
     },
     "smartlife.iot.smartbulb.lightingservice": {
         "get_light_state": {
             "dft_on_state": {
-                "brightness": 30,
-                "color_temp": 0,
-                "hue": 240,
+                "brightness": 100,
+                "color_temp": 2700,
+                "hue": 0,
                 "mode": "normal",
-                "saturation": 100
+                "saturation": 0
             },
             "err_code": 0,
             "on_off": 0
         }
     },
     "system": {
         "get_sysinfo": {
             "active_mode": "none",
-            "alias": "Bulb2",
+            "alias": "TP-LINK_Smart Bulb_43EC",
             "ctrl_protocols": {
                 "name": "Linkie",
                 "version": "1.0"
             },
-            "description": "Smart Wi-Fi LED Bulb with Color Changing",
+            "description": "Smart Wi-Fi LED Bulb with Dimmable Light",
             "dev_state": "normal",
             "deviceId": "0000000000000000000000000000000000000000",
             "disco_ver": "1.0",
             "err_code": 0,
-            "heapsize": 305252,
+            "heapsize": 290048,
             "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
-            "is_color": 1,
+            "is_color": 0,
             "is_dimmable": 1,
             "is_factory": false,
-            "is_variable_color_temp": 1,
+            "is_variable_color_temp": 0,
             "light_state": {
                 "dft_on_state": {
-                    "brightness": 30,
-                    "color_temp": 0,
-                    "hue": 240,
+                    "brightness": 100,
+                    "color_temp": 2700,
+                    "hue": 0,
                     "mode": "normal",
-                    "saturation": 100
+                    "saturation": 0
                 },
                 "on_off": 0
             },
             "mic_mac": "000000000000",
             "mic_type": "IOT.SMARTBULB",
-            "model": "KL130(US)",
+            "model": "LB110(US)",
             "oemId": "00000000000000000000000000000000",
             "preferred_state": [
                 {
-                    "brightness": 50,
+                    "brightness": 100,
                     "color_temp": 2700,
                     "hue": 0,
                     "index": 0,
                     "saturation": 0
                 },
                 {
-                    "brightness": 100,
-                    "color_temp": 0,
+                    "brightness": 75,
+                    "color_temp": 2700,
                     "hue": 0,
                     "index": 1,
-                    "saturation": 75
+                    "saturation": 0
                 },
                 {
-                    "brightness": 100,
-                    "color_temp": 0,
-                    "hue": 120,
+                    "brightness": 25,
+                    "color_temp": 2700,
+                    "hue": 0,
                     "index": 2,
-                    "saturation": 75
+                    "saturation": 0
                 },
                 {
-                    "brightness": 100,
-                    "color_temp": 0,
-                    "hue": 240,
+                    "brightness": 1,
+                    "color_temp": 2700,
+                    "hue": 0,
                     "index": 3,
-                    "saturation": 75
+                    "saturation": 0
                 }
             ],
-            "rssi": -52,
+            "rssi": -59,
             "sw_ver": "1.8.11 Build 191113 Rel.105336"
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL135(US)_1.0_1.0.6.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL135(US)_1.0_1.0.6.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.5.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.5.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.8.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL400L5(US)_1.0_1.0.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL420L5(US)_1.0_1.0.2.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL420L5(US)_1.0_1.0.2.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL430(UN)_2.0_1.0.8.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL430(UN)_2.0_1.0.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL430(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL430(US)_1.0_1.0.10.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL430(US)_2.0_1.0.8.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL430(US)_2.0_1.0.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL430(US)_2.0_1.0.9.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL430(US)_2.0_1.0.9.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL50(US)_1.0_1.1.13.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL50(US)_1.0_1.1.13.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL60(UN)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL60(UN)_1.0_1.1.4.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KL60(US)_1.0_1.1.13.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KL60(US)_1.0_1.1.13.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP100(US)_3.0_1.0.1.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP100(US)_3.0_1.0.1.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP105(UK)_1.0_1.0.7.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP105(UK)_1.0_1.0.7.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP115(EU)_1.0_1.0.16.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP115(EU)_1.0_1.0.16.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP115(US)_1.0_1.0.17.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP115(US)_1.0_1.0.17.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP125(US)_1.0_1.0.6.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP303(US)_2.0_1.0.3.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.44212962962962965%*

 * *Differences: {"'system'": "{'get_sysinfo': {'alias': 'TP-LINK_Power Strip_BDF6', 'feature': 'TIM', 'hw_ver': "*

 * *             "'2.0', 'model': 'KP303(US)', 'rssi': -56, 'status': 'new', 'sw_ver': '1.0.3 Build "*

 * *             "201015 Rel.173920', 'child_num': 3, 'children': [OrderedDict([('alias', 'Plug 1'), "*

 * *             "('id', '800681855E0E9AEF096F4891B3DC88C71E59F42E00'), ('next_action', "*

 * *             "OrderedDict([('type', -1)])), ('on_time', 0), ('state', 0)]), OrderedDict([('alias', "*

 * *             "'Plug 2'), ('id' […]*

```diff
@@ -1,42 +1,54 @@
 {
-    "emeter": {
-        "get_realtime": {
-            "current_ma": 978,
-            "err_code": 0,
-            "power_mw": 100277,
-            "total_wh": 12170,
-            "voltage_mv": 119425
-        }
-    },
     "system": {
         "get_sysinfo": {
-            "active_mode": "none",
-            "alias": "Test plug",
-            "dev_name": "Smart Wi-Fi Plug Mini",
+            "alias": "TP-LINK_Power Strip_BDF6",
+            "child_num": 3,
+            "children": [
+                {
+                    "alias": "Plug 1",
+                    "id": "800681855E0E9AEF096F4891B3DC88C71E59F42E00",
+                    "next_action": {
+                        "type": -1
+                    },
+                    "on_time": 0,
+                    "state": 0
+                },
+                {
+                    "alias": "Plug 2",
+                    "id": "800681855E0E9AEF096F4891B3DC88C71E59F42E01",
+                    "next_action": {
+                        "type": -1
+                    },
+                    "on_time": 0,
+                    "state": 0
+                },
+                {
+                    "alias": "Plug 3",
+                    "id": "800681855E0E9AEF096F4891B3DC88C71E59F42E02",
+                    "next_action": {
+                        "type": -1
+                    },
+                    "on_time": 0,
+                    "state": 0
+                }
+            ],
             "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
-            "feature": "TIM:ENE",
+            "feature": "TIM",
             "hwId": "00000000000000000000000000000000",
-            "hw_ver": "1.0",
-            "icon_hash": "",
+            "hw_ver": "2.0",
             "latitude_i": 0,
             "led_off": 0,
             "longitude_i": 0,
             "mac": "00:00:00:00:00:00",
             "mic_type": "IOT.SMARTPLUGSWITCH",
-            "model": "KP125(US)",
-            "next_action": {
-                "type": -1
-            },
+            "model": "KP303(US)",
             "ntc_state": 0,
-            "obd_src": "tplink",
             "oemId": "00000000000000000000000000000000",
-            "on_time": 301,
-            "relay_state": 1,
-            "rssi": -41,
-            "status": "configured",
-            "sw_ver": "1.0.6 Build 210928 Rel.185924",
+            "rssi": -56,
+            "status": "new",
+            "sw_ver": "1.0.3 Build 201015 Rel.173920",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP303(UK)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP303(UK)_1.0_1.0.3.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP303(US)_2.0_1.0.3.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP400(US)_1.0_1.0.10.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.19192361111111111%*

 * *Differences: {"'emeter'": "OrderedDict([('err_code', -1), ('err_msg', 'module not support')])",*

 * * "'smartlife.iot.common.emeter'": "OrderedDict([('err_code', -1), ('err_msg', 'module not "*

 * *                                  "support')])",*

 * * "'smartlife.iot.dimmer'": "OrderedDict([('err_code', -1), ('err_msg', 'module not support')])",*

 * * "'smartlife.iot.smartbulb.lightingservice'": "OrderedDict([('err_code', -1), ('err_msg', 'module "*

 * *                                              "not support')])",*

 * * "'system'": "{'get_sysinf […]*

```diff
@@ -1,54 +1,63 @@
 {
+    "emeter": {
+        "err_code": -1,
+        "err_msg": "module not support"
+    },
+    "smartlife.iot.common.emeter": {
+        "err_code": -1,
+        "err_msg": "module not support"
+    },
+    "smartlife.iot.dimmer": {
+        "err_code": -1,
+        "err_msg": "module not support"
+    },
+    "smartlife.iot.smartbulb.lightingservice": {
+        "err_code": -1,
+        "err_msg": "module not support"
+    },
     "system": {
         "get_sysinfo": {
-            "alias": "TP-LINK_Power Strip_BDF6",
-            "child_num": 3,
+            "alias": "TP-LINK_Smart Plug_2ECE",
+            "child_num": 2,
             "children": [
                 {
-                    "alias": "Plug 1",
-                    "id": "800681855E0E9AEF096F4891B3DC88C71E59F42E00",
+                    "alias": "Rope",
+                    "id": "00",
                     "next_action": {
-                        "type": -1
+                        "action": 1,
+                        "schd_sec": 69240,
+                        "type": 1
                     },
                     "on_time": 0,
                     "state": 0
                 },
                 {
                     "alias": "Plug 2",
-                    "id": "800681855E0E9AEF096F4891B3DC88C71E59F42E01",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 0,
-                    "state": 0
-                },
-                {
-                    "alias": "Plug 3",
-                    "id": "800681855E0E9AEF096F4891B3DC88C71E59F42E02",
+                    "id": "01",
                     "next_action": {
                         "type": -1
                     },
                     "on_time": 0,
                     "state": 0
                 }
             ],
             "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
             "feature": "TIM",
             "hwId": "00000000000000000000000000000000",
-            "hw_ver": "2.0",
+            "hw_ver": "1.0",
             "latitude_i": 0,
             "led_off": 0,
             "longitude_i": 0,
             "mac": "00:00:00:00:00:00",
             "mic_type": "IOT.SMARTPLUGSWITCH",
-            "model": "KP303(US)",
+            "model": "KP400(US)",
             "ntc_state": 0,
             "oemId": "00000000000000000000000000000000",
-            "rssi": -56,
+            "rssi": -78,
             "status": "new",
-            "sw_ver": "1.0.3 Build 201015 Rel.173920",
+            "sw_ver": "1.0.10 Build 190716 Rel.095026",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP400(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KS230(US)_1.0_1.0.14.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2775862068965517%*

 * *Differences: {"'smartlife.iot.dimmer'": "{replace: OrderedDict([('get_dimmer_parameters', "*

 * *                           "OrderedDict([('bulb_type', 1), ('err_code', 0), ('fadeOffTime', 1000), "*

 * *                           "('fadeOnTime', 1000), ('gentleOffTime', 10000), ('gentleOnTime', "*

 * *                           "3000), ('minThreshold', 11), ('rampRate', 30)]))])}",*

 * * "'system'": "{'get_sysinfo': {'alias': 'Test KS230', 'model': 'KS230(US)', 'rssi': -52, 'sw_ver': "*

 * *             "'1.0.14 Build 220127 Rel.124555', 'activ […]*

```diff
@@ -1,63 +1,64 @@
 {
-    "emeter": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
-    "smartlife.iot.common.emeter": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
     "smartlife.iot.dimmer": {
-        "err_code": -1,
-        "err_msg": "module not support"
-    },
-    "smartlife.iot.smartbulb.lightingservice": {
-        "err_code": -1,
-        "err_msg": "module not support"
+        "get_dimmer_parameters": {
+            "bulb_type": 1,
+            "err_code": 0,
+            "fadeOffTime": 1000,
+            "fadeOnTime": 1000,
+            "gentleOffTime": 10000,
+            "gentleOnTime": 3000,
+            "minThreshold": 11,
+            "rampRate": 30
+        }
     },
     "system": {
         "get_sysinfo": {
-            "alias": "TP-LINK_Smart Plug_2ECE",
-            "child_num": 2,
-            "children": [
-                {
-                    "alias": "Rope",
-                    "id": "00",
-                    "next_action": {
-                        "action": 1,
-                        "schd_sec": 69240,
-                        "type": 1
-                    },
-                    "on_time": 0,
-                    "state": 0
-                },
-                {
-                    "alias": "Plug 2",
-                    "id": "01",
-                    "next_action": {
-                        "type": -1
-                    },
-                    "on_time": 0,
-                    "state": 0
-                }
-            ],
+            "active_mode": "none",
+            "alias": "Test KS230",
+            "brightness": 60,
+            "dc_state": 0,
+            "dev_name": "Wi-Fi Smart 3-Way Dimmer",
             "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
             "feature": "TIM",
             "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
+            "icon_hash": "",
             "latitude_i": 0,
             "led_off": 0,
             "longitude_i": 0,
             "mac": "00:00:00:00:00:00",
             "mic_type": "IOT.SMARTPLUGSWITCH",
-            "model": "KP400(US)",
+            "model": "KS230(US)",
+            "next_action": {
+                "type": -1
+            },
             "ntc_state": 0,
             "oemId": "00000000000000000000000000000000",
-            "rssi": -78,
+            "on_time": 0,
+            "preferred_state": [
+                {
+                    "brightness": 100,
+                    "index": 0
+                },
+                {
+                    "brightness": 75,
+                    "index": 1
+                },
+                {
+                    "brightness": 50,
+                    "index": 2
+                },
+                {
+                    "brightness": 25,
+                    "index": 3
+                }
+            ],
+            "relay_state": 0,
+            "rssi": -52,
             "status": "new",
-            "sw_ver": "1.0.10 Build 190716 Rel.095026",
+            "sw_ver": "1.0.14 Build 220127 Rel.124555",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP400(US)_2.0_1.0.6.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP400(US)_2.0_1.0.6.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KP401(US)_1.0_1.0.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP401(US)_1.0_1.0.0.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KS200M(US)_1.0_1.0.8.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KS200M(US)_1.0_1.0.8.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KS220M(US)_1.0_1.0.4.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KS220M(US)_1.0_1.0.4.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/KS230(US)_1.0_1.0.14.json` & `python_kasa-0.5.2/kasa/tests/fixtures/KP405(US)_1.0_1.0.5.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9546130952380953%*

 * *Differences: {"'smartlife.iot.dimmer'": "{'get_dimmer_parameters': {'minThreshold': 1, 'calibration_type': 0}}",*

 * * "'system'": "{'get_sysinfo': {'alias': 'Porch Lights', 'brightness': 50, 'dev_name': 'Kasa Smart "*

 * *             "Wi-Fi Outdoor Plug-In Dimmer', 'led_off': 1, 'model': 'KP405(US)', 'rssi': -64, "*

 * *             "'sw_ver': '1.0.5 Build 221108 Rel.181739', 'obd_src': 'tplink', delete: "*

 * *             "['dc_state']}}"}*

```diff
@@ -1,43 +1,44 @@
 {
     "smartlife.iot.dimmer": {
         "get_dimmer_parameters": {
             "bulb_type": 1,
+            "calibration_type": 0,
             "err_code": 0,
             "fadeOffTime": 1000,
             "fadeOnTime": 1000,
             "gentleOffTime": 10000,
             "gentleOnTime": 3000,
-            "minThreshold": 11,
+            "minThreshold": 1,
             "rampRate": 30
         }
     },
     "system": {
         "get_sysinfo": {
             "active_mode": "none",
-            "alias": "Test KS230",
-            "brightness": 60,
-            "dc_state": 0,
-            "dev_name": "Wi-Fi Smart 3-Way Dimmer",
+            "alias": "Porch Lights",
+            "brightness": 50,
+            "dev_name": "Kasa Smart Wi-Fi Outdoor Plug-In Dimmer",
             "deviceId": "0000000000000000000000000000000000000000",
             "err_code": 0,
             "feature": "TIM",
             "hwId": "00000000000000000000000000000000",
             "hw_ver": "1.0",
             "icon_hash": "",
             "latitude_i": 0,
-            "led_off": 0,
+            "led_off": 1,
             "longitude_i": 0,
             "mac": "00:00:00:00:00:00",
             "mic_type": "IOT.SMARTPLUGSWITCH",
-            "model": "KS230(US)",
+            "model": "KP405(US)",
             "next_action": {
                 "type": -1
             },
             "ntc_state": 0,
+            "obd_src": "tplink",
             "oemId": "00000000000000000000000000000000",
             "on_time": 0,
             "preferred_state": [
                 {
                     "brightness": 100,
                     "index": 0
                 },
@@ -51,14 +52,14 @@
                 },
                 {
                     "brightness": 25,
                     "index": 3
                 }
             ],
             "relay_state": 0,
-            "rssi": -52,
+            "rssi": -64,
             "status": "new",
-            "sw_ver": "1.0.14 Build 220127 Rel.124555",
+            "sw_ver": "1.0.5 Build 221108 Rel.181739",
             "updating": 0
         }
     }
 }
```

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/LB100(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/LB100(US)_1.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/fixtures/LB120(US)_1.0.json` & `python_kasa-0.5.2/kasa/tests/fixtures/LB120(US)_1.0_mocked.json`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/newfakes.py` & `python_kasa-0.5.2/kasa/tests/newfakes.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_bulb.py` & `python_kasa-0.5.2/kasa/tests/test_bulb.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         assert preset.brightness == raw["brightness"]
         assert preset.saturation == raw["saturation"]
         assert preset.color_temp == raw["color_temp"]
 
 
 @bulb
 async def test_modify_preset(dev: SmartBulb, mocker):
-    """Verify that modifying preset calls the  and exceptions are raised properly."""
+    """Verify that modifying preset calls the and exceptions are raised properly."""
     if not dev.presets:
         pytest.skip("Some strips do not support presets")
 
     data = {
         "index": 0,
         "brightness": 10,
         "hue": 0,
@@ -285,7 +285,31 @@
     await dev.save_preset(preset)
     assert dev.presets[0].brightness == 10
 
     with pytest.raises(SmartDeviceException):
         await dev.save_preset(
             SmartBulbPreset(index=5, hue=0, brightness=0, saturation=0, color_temp=0)
         )
+
+
+@bulb
+@pytest.mark.parametrize(
+    ("preset", "payload"),
+    [
+        (
+            SmartBulbPreset(index=0, hue=0, brightness=1, saturation=0),
+            {"index": 0, "hue": 0, "brightness": 1, "saturation": 0},
+        ),
+        (
+            SmartBulbPreset(index=0, brightness=1, id="testid", mode=2, custom=0),
+            {"index": 0, "brightness": 1, "id": "testid", "mode": 2, "custom": 0},
+        ),
+    ],
+)
+async def test_modify_preset_payloads(dev: SmartBulb, preset, payload, mocker):
+    """Test that modify preset payloads ignore none values."""
+    if not dev.presets:
+        pytest.skip("Some strips do not support presets")
+
+    query_helper = mocker.patch("kasa.SmartBulb._query_helper")
+    await dev.save_preset(preset)
+    query_helper.assert_called_with(dev.LIGHT_SERVICE, "set_preferred_state", payload)
```

### Comparing `python_kasa-0.5.1/kasa/tests/test_cli.py` & `python_kasa-0.5.2/kasa/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     assert dev.alias in res.output
 
     res = await runner.invoke(raw_command, obj=dev)
     assert res.exit_code != 0
     assert "Usage" in res.output
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="3.8 is first one with asyncmock")
 async def test_emeter(dev: SmartDevice, mocker):
     runner = CliRunner()
 
     res = await runner.invoke(emeter, obj=dev)
     if not dev.has_emeter:
         assert "Device has no emeter" in res.output
         return
@@ -99,17 +98,14 @@
     res = await runner.invoke(brightness, ["12"], obj=dev)
     assert "Setting brightness" in res.output
 
     res = await runner.invoke(brightness, obj=dev)
     assert "Brightness: 12" in res.output
 
 
-# Invoke fails when run on py3.7 with the following error:
-# E        +  where 1 = <Result TypeError("object list can't be used in 'await' expression")>.exit_code
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="fails on python3.7")
 async def test_json_output(dev: SmartDevice, mocker):
     """Test that the json output produces correct output."""
     mocker.patch("kasa.Discover.discover", return_value=[dev])
     runner = CliRunner()
     res = await runner.invoke(cli, ["--json", "state"], obj=dev)
     assert res.exit_code == 0
     assert json.loads(res.output) == dev.internal_state
```

### Comparing `python_kasa-0.5.1/kasa/tests/test_dimmer.py` & `python_kasa-0.5.2/kasa/tests/test_dimmer.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_discovery.py` & `python_kasa-0.5.2/kasa/tests/test_discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 async def test_type_unknown():
     invalid_info = {"system": {"get_sysinfo": {"type": "nosuchtype"}}}
     with pytest.raises(SmartDeviceException):
         Discover._get_device_class(invalid_info)
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="3.8 is first one with asyncmock")
 async def test_discover_single(discovery_data: dict, mocker):
     """Make sure that discover_single returns an initialized SmartDevice instance."""
     mocker.patch("kasa.TPLinkSmartHomeProtocol.query", return_value=discovery_data)
     x = await Discover.discover_single("127.0.0.1")
     assert issubclass(x.__class__, SmartDevice)
     assert x._sys_info is not None
 
@@ -67,15 +66,14 @@
         "Unable to find the device type field",
         {"system": {"get_sysinfo": {"missing_type": 1}}},
     ),
     ("Unknown device type: foo", {"system": {"get_sysinfo": {"type": "foo"}}}),
 ]
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="3.8 is first one with asyncmock")
 @pytest.mark.parametrize("msg, data", INVALIDS)
 async def test_discover_invalid_info(msg, data, mocker):
     """Make sure that invalid discovery information raises an exception."""
     mocker.patch("kasa.TPLinkSmartHomeProtocol.query", return_value=data)
     with pytest.raises(SmartDeviceException, match=msg):
         await Discover.discover_single("127.0.0.1")
 
@@ -89,15 +87,15 @@
     proto.do_discover()
     assert transport.sendto.call_count == proto.discovery_packets
 
 
 async def test_discover_datagram_received(mocker, discovery_data):
     """Verify that datagram received fills discovered_devices."""
     proto = _DiscoverProtocol()
-    mocker.patch("json.loads", return_value=discovery_data)
+    mocker.patch("kasa.discover.json_loads", return_value=discovery_data)
     mocker.patch.object(protocol.TPLinkSmartHomeProtocol, "encrypt")
     mocker.patch.object(protocol.TPLinkSmartHomeProtocol, "decrypt")
 
     addr = "127.0.0.1"
     proto.datagram_received("<placeholder data>", (addr, 1234))
 
     # Check that device in discovered_devices is initialized correctly
@@ -107,13 +105,13 @@
     assert dev.host == addr
 
 
 @pytest.mark.parametrize("msg, data", INVALIDS)
 async def test_discover_invalid_responses(msg, data, mocker):
     """Verify that we don't crash whole discovery if some devices in the network are sending unexpected data."""
     proto = _DiscoverProtocol()
-    mocker.patch("json.loads", return_value=data)
+    mocker.patch("kasa.discover.json_loads", return_value=data)
     mocker.patch.object(protocol.TPLinkSmartHomeProtocol, "encrypt")
     mocker.patch.object(protocol.TPLinkSmartHomeProtocol, "decrypt")
 
     proto.datagram_received(data, ("127.0.0.1", 1234))
     assert len(proto.discovered_devices) == 0
```

### Comparing `python_kasa-0.5.1/kasa/tests/test_emeter.py` & `python_kasa-0.5.2/kasa/tests/test_emeter.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_lightstrip.py` & `python_kasa-0.5.2/kasa/tests/test_lightstrip.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_plug.py` & `python_kasa-0.5.2/kasa/tests/test_plug.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_protocol.py` & `python_kasa-0.5.2/kasa/tests/test_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     )
     with pytest.raises(SmartDeviceException):
         await TPLinkSmartHomeProtocol("127.0.0.1").query({}, retry_count=5)
 
     assert conn.call_count == 6
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="3.8 is first one with asyncmock")
 @pytest.mark.parametrize("retry_count", [1, 3, 5])
 async def test_protocol_reconnect(mocker, retry_count):
     remaining = retry_count
     encrypted = TPLinkSmartHomeProtocol.encrypt('{"great":"success"}')[
         TPLinkSmartHomeProtocol.BLOCK_SIZE :
     ]
 
@@ -94,15 +93,14 @@
 
     protocol = TPLinkSmartHomeProtocol("127.0.0.1")
     mocker.patch("asyncio.open_connection", side_effect=aio_mock_writer)
     response = await protocol.query({}, retry_count=retry_count)
     assert response == {"great": "success"}
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="3.8 is first one with asyncmock")
 @pytest.mark.parametrize("log_level", [logging.WARNING, logging.DEBUG])
 async def test_protocol_logging(mocker, caplog, log_level):
     caplog.set_level(log_level)
     logging.getLogger("kasa").setLevel(log_level)
     encrypted = TPLinkSmartHomeProtocol.encrypt('{"great":"success"}')[
         TPLinkSmartHomeProtocol.BLOCK_SIZE :
     ]
```

### Comparing `python_kasa-0.5.1/kasa/tests/test_readme_examples.py` & `python_kasa-0.5.2/kasa/tests/test_readme_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,71 +5,66 @@
 import xdoctest
 
 from kasa.tests.conftest import get_device_for_file
 
 
 def test_bulb_examples(mocker):
     """Use KL130 (bulb with all features) to test the doctests."""
-    p = asyncio.run(get_device_for_file("KL130(US)_1.0.json"))
+    p = asyncio.run(get_device_for_file("KL130(US)_1.0_1.8.11.json"))
     mocker.patch("kasa.smartbulb.SmartBulb", return_value=p)
     mocker.patch("kasa.smartbulb.SmartBulb.update")
     res = xdoctest.doctest_module("kasa.smartbulb", "all")
     assert not res["failed"]
 
 
 def test_smartdevice_examples(mocker):
     """Use HS110 for emeter examples."""
-    p = asyncio.run(get_device_for_file("HS110(EU)_1.0_real.json"))
+    p = asyncio.run(get_device_for_file("HS110(EU)_1.0_1.2.5.json"))
     mocker.patch("kasa.smartdevice.SmartDevice", return_value=p)
     mocker.patch("kasa.smartdevice.SmartDevice.update")
     res = xdoctest.doctest_module("kasa.smartdevice", "all")
     assert not res["failed"]
 
 
 def test_plug_examples(mocker):
     """Test plug examples."""
-    p = asyncio.run(get_device_for_file("HS110(EU)_1.0_real.json"))
+    p = asyncio.run(get_device_for_file("HS110(EU)_1.0_1.2.5.json"))
     mocker.patch("kasa.smartplug.SmartPlug", return_value=p)
     mocker.patch("kasa.smartplug.SmartPlug.update")
     res = xdoctest.doctest_module("kasa.smartplug", "all")
     assert not res["failed"]
 
 
 def test_strip_examples(mocker):
     """Test strip examples."""
-    p = asyncio.run(get_device_for_file("KP303(UK)_1.0.json"))
+    p = asyncio.run(get_device_for_file("KP303(UK)_1.0_1.0.3.json"))
     mocker.patch("kasa.smartstrip.SmartStrip", return_value=p)
     mocker.patch("kasa.smartstrip.SmartStrip.update")
     res = xdoctest.doctest_module("kasa.smartstrip", "all")
     assert not res["failed"]
 
 
 def test_dimmer_examples(mocker):
     """Test dimmer examples."""
-    p = asyncio.run(get_device_for_file("HS220(US)_1.0_real.json"))
+    p = asyncio.run(get_device_for_file("HS220(US)_1.0_1.5.7.json"))
     mocker.patch("kasa.smartdimmer.SmartDimmer", return_value=p)
     mocker.patch("kasa.smartdimmer.SmartDimmer.update")
     res = xdoctest.doctest_module("kasa.smartdimmer", "all")
     assert not res["failed"]
 
 
 def test_lightstrip_examples(mocker):
     """Test lightstrip examples."""
-    p = asyncio.run(get_device_for_file("KL430(US)_1.0.json"))
+    p = asyncio.run(get_device_for_file("KL430(US)_1.0_1.0.10.json"))
     mocker.patch("kasa.smartlightstrip.SmartLightStrip", return_value=p)
     mocker.patch("kasa.smartlightstrip.SmartLightStrip.update")
     res = xdoctest.doctest_module("kasa.smartlightstrip", "all")
     assert not res["failed"]
 
 
-@pytest.mark.skipif(
-    sys.version_info < (3, 8), reason="3.7 handles asyncio.run differently"
-)
 def test_discovery_examples(mocker):
     """Test discovery examples."""
-    p = asyncio.run(get_device_for_file("KP303(UK)_1.0.json"))
+    p = asyncio.run(get_device_for_file("KP303(UK)_1.0_1.0.3.json"))
 
-    # This succeeds on python 3.8 but fails on 3.7
-    # ValueError: a coroutine was expected, got [<DeviceType.Strip model KP303(UK) ...
     mocker.patch("kasa.discover.Discover.discover", return_value=[p])
     res = xdoctest.doctest_module("kasa.discover", "all")
     assert not res["failed"]
```

### Comparing `python_kasa-0.5.1/kasa/tests/test_smartdevice.py` & `python_kasa-0.5.2/kasa/tests/test_smartdevice.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_strip.py` & `python_kasa-0.5.2/kasa/tests/test_strip.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/kasa/tests/test_usage.py` & `python_kasa-0.5.2/kasa/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `python_kasa-0.5.1/pyproject.toml` & `python_kasa-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-kasa"
-version = "0.5.1"
+version = "0.5.2"
 description = "Python API for TP-Link Kasa Smarthome devices"
 license = "GPL-3.0-or-later"
 authors = ["python-kasa developers"]
 repository = "https://github.com/python-kasa/python-kasa"
 readme = "README.md"
 packages = [
   { include = "kasa" }
@@ -15,20 +15,23 @@
 "Bug Tracker" = "https://github.com/python-kasa/python-kasa/issues"
 "Documentation" = "https://python-kasa.readthedocs.io"
 
 [tool.poetry.scripts]
 kasa = "kasa.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 anyio = "*"  # see https://github.com/python-trio/asyncclick/issues/18
-importlib-metadata = "*"
 asyncclick = ">=8"
 pydantic = "^1"
 
+# speed ups
+orjson = { "version" = ">=3.9.1", optional = true }
+kasa-crypt = { "version" = ">=0.2.0", optional = true }
+
 # required only for docs
 sphinx = { version = "^4", optional = true }
 sphinx_rtd_theme = { version = "^0", optional = true }
 sphinxcontrib-programoutput = { version = "^0", optional = true }
 myst-parser = { version = "*", optional = true }
 docutils = { version = ">=0.17", optional = true }
 
@@ -44,14 +47,15 @@
 pytest-mock = "*"
 codecov = "*"
 xdoctest = "*"
 coverage = {version = "*", extras = ["toml"]}
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx_rtd_theme", "sphinxcontrib-programoutput", "myst-parser", "docutils"]
+speedups = ["orjson", "kasa-crypt"]
 
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `python_kasa-0.5.1/PKG-INFO` & `python_kasa-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: python-kasa
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python API for TP-Link Kasa Smarthome devices
 Home-page: https://github.com/python-kasa/python-kasa
 License: GPL-3.0-or-later
 Author: python-kasa developers
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+Provides-Extra: speedups
 Requires-Dist: anyio
 Requires-Dist: asyncclick (>=8)
 Requires-Dist: docutils (>=0.17) ; extra == "docs"
-Requires-Dist: importlib-metadata
+Requires-Dist: kasa-crypt (>=0.2.0) ; extra == "speedups"
 Requires-Dist: myst-parser ; extra == "docs"
+Requires-Dist: orjson (>=3.9.1) ; extra == "speedups"
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: sphinx (>=4,<5) ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme (>=0,<1) ; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput (>=0,<1) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/python-kasa/python-kasa/issues
 Project-URL: Documentation, https://python-kasa.readthedocs.io
 Project-URL: Repository, https://github.com/python-kasa/python-kasa
@@ -44,14 +45,21 @@
 ## Getting started
 
 You can install the most recent release using pip:
 ```
 pip install python-kasa
 ```
 
+If you are using cpython, it is recommended to install with `[speedups]` to enable orjson (faster json support):
+```
+pip install python-kasa[speedups]
+```
+
+With `[speedups]`, the protocol overhead is roughly an order of magnitude lower (benchmarks available in devtools).
+
 Alternatively, you can clone this repository and use poetry to install the development version:
 ```
 git clone https://github.com/python-kasa/python-kasa.git
 cd python-kasa/
 poetry install
 ```
 
@@ -165,14 +173,15 @@
 
 ### Power Strips
 
 * EP40
 * HS300
 * KP303
 * KP400
+* KP405 (dimmer)
 
 ### Wall switches
 
 * ES20M
 * HS200
 * HS210
 * HS220
```

