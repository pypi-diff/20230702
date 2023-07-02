# Comparing `tmp/terra_classic_sdk-2.0.8.tar.gz` & `tmp/terra_classic_sdk-2.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_classic_sdk-2.0.8.tar", max compression
+gzip compressed data, was "terra_classic_sdk-2.0.8.1.tar", max compression
```

## Comparing `terra_classic_sdk-2.0.8.tar` & `terra_classic_sdk-2.0.8.1.tar`

### file list

```diff
@@ -1,243 +1,243 @@
--rw-r--r--   0        0        0     1082 2023-04-11 08:50:13.847731 terra_classic_sdk-2.0.8/LICENSE
--rw-r--r--   0        0        0    12754 2023-06-28 02:29:46.017082 terra_classic_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     1884 2023-07-02 04:50:06.069721 terra_classic_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.872423 terra_classic_sdk-2.0.8/terra_classic_sdk/.DS_Store
--rw-r--r--   0        0        0      161 2023-04-11 08:50:13.901954 terra_classic_sdk-2.0.8/terra_classic_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.904117 terra_classic_sdk-2.0.8/terra_classic_sdk/client/__init__.py
--rw-r--r--   0        0        0      179 2023-06-26 08:32:24.148030 terra_classic_sdk-2.0.8/terra_classic_sdk/client/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3813 2023-06-26 08:32:24.148253 terra_classic_sdk-2.0.8/terra_classic_sdk/client/__pycache__/localterra.cpython-310.pyc
--rw-r--r--   0        0        0      216 2023-04-11 08:50:13.905477 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__init__.py
--rw-r--r--   0        0        0      404 2023-06-26 08:32:24.148713 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9199 2023-06-26 08:32:24.149073 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/lcdclient.cpython-310.pyc
--rw-r--r--   0        0        0     2853 2023-06-26 08:32:24.149298 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/lcdutils.cpython-310.pyc
--rw-r--r--   0        0        0     2887 2023-06-26 08:32:24.149526 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/params.cpython-310.pyc
--rw-r--r--   0        0        0     4733 2023-06-26 08:32:24.149761 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/wallet.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.907268 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__init__.py
--rw-r--r--   0        0        0      187 2023-06-26 08:32:24.150055 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1407 2023-06-26 08:32:24.150263 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/_base.cpython-310.pyc
--rw-r--r--   0        0        0     1489 2023-06-26 08:32:24.150491 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/auth.cpython-310.pyc
--rw-r--r--   0        0        0     2127 2023-06-26 08:32:24.150892 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/authz.cpython-310.pyc
--rw-r--r--   0        0        0     2200 2023-06-26 08:32:24.151103 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/bank.cpython-310.pyc
--rw-r--r--   0        0        0     4304 2023-06-26 08:32:24.151436 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/distribution.cpython-310.pyc
--rw-r--r--   0        0        0     2808 2023-06-26 08:32:24.151648 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/feegrant.cpython-310.pyc
--rw-r--r--   0        0        0     9696 2023-06-26 08:32:24.151910 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/gov.cpython-310.pyc
--rw-r--r--   0        0        0     1047 2023-06-26 08:32:24.152117 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/ibc.cpython-310.pyc
--rw-r--r--   0        0        0     1203 2023-06-26 08:32:24.152347 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/ibc_transfer.cpython-310.pyc
--rw-r--r--   0        0        0     2565 2023-06-26 08:32:24.152592 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/market.cpython-310.pyc
--rw-r--r--   0        0        0     2255 2023-06-26 08:32:24.152796 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/mint.cpython-310.pyc
--rw-r--r--   0        0        0     6379 2023-06-26 08:32:24.153054 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/oracle.cpython-310.pyc
--rw-r--r--   0        0        0     3609 2023-06-26 08:32:24.153339 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/slashing.cpython-310.pyc
--rw-r--r--   0        0        0    12230 2023-06-26 08:32:24.153836 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/staking.cpython-310.pyc
--rw-r--r--   0        0        0     2940 2023-06-26 08:32:24.154072 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/tendermint.cpython-310.pyc
--rw-r--r--   0        0        0     4270 2023-06-26 08:32:24.154331 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/treasury.cpython-310.pyc
--rw-r--r--   0        0        0    15516 2023-06-26 08:32:24.154719 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/tx.cpython-310.pyc
--rw-r--r--   0        0        0     3479 2023-06-26 08:32:24.154935 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/wasm.cpython-310.pyc
--rw-r--r--   0        0        0      812 2023-04-11 08:50:13.906398 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/_base.py
--rw-r--r--   0        0        0      982 2023-04-15 09:35:43.014907 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/auth.py
--rw-r--r--   0        0        0     1616 2023-04-15 09:35:43.014689 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/authz.py
--rw-r--r--   0        0        0     1618 2023-04-15 09:35:43.014832 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/bank.py
--rw-r--r--   0        0        0     3633 2023-04-15 09:35:43.014773 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/distribution.py
--rw-r--r--   0        0        0     2566 2023-04-15 09:35:43.014792 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/feegrant.py
--rw-r--r--   0        0        0    10292 2023-04-15 09:35:43.014622 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/gov.py
--rw-r--r--   0        0        0      587 2023-04-11 08:50:13.908029 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc.py
--rw-r--r--   0        0        0      762 2023-04-11 08:50:13.909254 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc_transfer.py
--rw-r--r--   0        0        0     2020 2023-04-15 09:35:43.014807 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/market.py
--rw-r--r--   0        0        0     1836 2023-04-15 09:35:43.014730 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/mint.py
--rw-r--r--   0        0        0     6371 2023-04-15 09:35:43.014757 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/oracle.py
--rw-r--r--   0        0        0     3519 2023-04-15 09:35:43.014854 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/slashing.py
--rw-r--r--   0        0        0    13208 2023-04-15 09:35:43.014885 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/staking.py
--rw-r--r--   0        0        0     2453 2023-04-11 08:50:13.907101 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tendermint.py
--rw-r--r--   0        0        0     3770 2023-04-15 09:35:43.014638 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/treasury.py
--rw-r--r--   0        0        0    14753 2023-06-25 10:33:24.003762 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tx.py
--rw-r--r--   0        0        0     3244 2023-06-26 08:46:22.680897 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/wasm.py
--rw-r--r--   0        0        0    11889 2023-06-26 08:46:22.681285 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdclient.py
--rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.014571 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdutils.py
--rw-r--r--   0        0        0     2394 2023-04-11 08:50:13.905004 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/params.py
--rw-r--r--   0        0        0     5207 2023-04-15 09:35:43.014541 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/wallet.py
--rw-r--r--   0        0        0     3700 2023-04-15 09:35:43.014511 terra_classic_sdk-2.0.8/terra_classic_sdk/client/localterra.py
--rw-r--r--   0        0        0    10244 2023-04-11 08:50:13.877728 terra_classic_sdk-2.0.8/terra_classic_sdk/core/.DS_Store
--rw-r--r--   0        0        0      899 2023-04-11 08:50:13.884485 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__init__.py
--rw-r--r--   0        0        0      986 2023-06-26 08:32:24.156487 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4724 2023-06-26 08:32:24.156738 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/bech32.cpython-310.pyc
--rw-r--r--   0        0        0     2816 2023-06-26 08:32:24.156950 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/broadcast.cpython-310.pyc
--rw-r--r--   0        0        0     8676 2023-06-26 08:32:24.157185 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/coin.cpython-310.pyc
--rw-r--r--   0        0        0    11636 2023-06-26 08:32:24.157554 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/coins.cpython-310.pyc
--rw-r--r--   0        0        0     3585 2023-06-26 08:32:24.157869 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/compact_bit_array.cpython-310.pyc
--rw-r--r--   0        0        0     1495 2023-06-26 08:32:24.158171 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/deposit.cpython-310.pyc
--rw-r--r--   0        0        0     2546 2023-06-26 08:32:24.158381 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/fee.cpython-310.pyc
--rw-r--r--   0        0        0     4434 2023-06-26 08:32:24.158599 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/mode_info.cpython-310.pyc
--rw-r--r--   0        0        0     1452 2023-06-26 08:32:24.158795 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/msg.cpython-310.pyc
--rw-r--r--   0        0        0     2716 2023-06-26 08:32:24.159109 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/multisig.cpython-310.pyc
--rw-r--r--   0        0        0    12613 2023-06-26 08:32:24.159455 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/numeric.cpython-310.pyc
--rw-r--r--   0        0        0    12790 2023-06-26 08:32:24.159784 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/public_key.cpython-310.pyc
--rw-r--r--   0        0        0     2982 2023-06-26 08:32:24.159992 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/sign_doc.cpython-310.pyc
--rw-r--r--   0        0        0     4309 2023-06-26 08:32:24.160229 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/signature_v2.cpython-310.pyc
--rw-r--r--   0        0        0    16009 2023-06-26 08:32:24.160530 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/tx.cpython-310.pyc
--rw-r--r--   0        0        0      249 2023-04-11 08:50:13.878407 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/__init__.py
--rw-r--r--   0        0        0      381 2023-06-26 08:32:24.160897 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      403 2023-04-15 09:35:43.014285 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__init__.py
--rw-r--r--   0        0        0      574 2023-06-26 08:32:24.161152 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1501 2023-06-26 08:32:24.161384 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/account.cpython-310.pyc
--rw-r--r--   0        0        0     3063 2023-06-26 08:32:24.161583 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/base_account.cpython-310.pyc
--rw-r--r--   0        0        0     3463 2023-06-26 08:32:24.161782 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/base_vesting_account.cpython-310.pyc
--rw-r--r--   0        0        0     7577 2023-06-26 08:32:24.162006 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/lazy_graded_vesting_account.cpython-310.pyc
--rw-r--r--   0        0        0     1003 2023-04-15 09:35:43.014339 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/account.py
--rw-r--r--   0        0        0     2824 2023-04-11 08:50:13.879294 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_account.py
--rw-r--r--   0        0        0     3948 2023-04-15 09:35:43.014303 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_vesting_account.py
--rw-r--r--   0        0        0     5915 2023-04-15 09:35:43.014323 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py
--rw-r--r--   0        0        0      446 2023-04-11 08:50:13.894143 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__init__.py
--rw-r--r--   0        0        0      514 2023-06-26 08:32:24.162263 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10437 2023-06-26 08:32:24.162509 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     7364 2023-06-26 08:32:24.162724 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     9483 2023-04-15 09:35:43.013660 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/data.py
--rw-r--r--   0        0        0     6103 2023-04-15 09:35:43.013727 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/msgs.py
--rw-r--r--   0        0        0      149 2023-04-11 08:50:13.880447 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__init__.py
--rw-r--r--   0        0        0      333 2023-06-26 08:32:24.163067 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9156 2023-06-26 08:32:24.163318 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     7220 2023-04-15 09:35:43.014366 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/msgs.py
--rw-r--r--   0        0        0     4989 2023-04-11 08:50:13.876513 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bech32.py
--rw-r--r--   0        0        0     1616 2023-04-11 08:50:13.894782 terra_classic_sdk-2.0.8/terra_classic_sdk/core/block.py
--rw-r--r--   0        0        0     2736 2023-04-15 09:35:43.012322 terra_classic_sdk-2.0.8/terra_classic_sdk/core/broadcast.py
--rw-r--r--   0        0        0     7757 2023-04-15 09:35:43.011986 terra_classic_sdk-2.0.8/terra_classic_sdk/core/coin.py
--rw-r--r--   0        0        0     8364 2023-04-15 09:35:43.013020 terra_classic_sdk-2.0.8/terra_classic_sdk/core/coins.py
--rw-r--r--   0        0        0     2866 2023-04-15 09:35:43.013363 terra_classic_sdk-2.0.8/terra_classic_sdk/core/compact_bit_array.py
--rw-r--r--   0        0        0       71 2023-04-11 08:50:13.884925 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__init__.py
--rw-r--r--   0        0        0      253 2023-06-26 08:32:24.163663 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2471 2023-06-26 08:32:24.163863 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     2075 2023-04-15 09:35:43.013412 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/msgs.py
--rw-r--r--   0        0        0     1095 2023-04-15 09:35:43.013455 terra_classic_sdk-2.0.8/terra_classic_sdk/core/deposit.py
--rw-r--r--   0        0        0      371 2023-04-11 08:50:13.883813 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__init__.py
--rw-r--r--   0        0        0      455 2023-06-26 08:32:24.164121 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6738 2023-06-26 08:32:24.164345 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     2895 2023-06-26 08:32:24.164546 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/proposals.cpython-310.pyc
--rw-r--r--   0        0        0     6952 2023-04-15 09:35:43.014021 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/msgs.py
--rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.013993 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/proposals.py
--rw-r--r--   0        0        0     2024 2023-04-15 09:35:43.013238 terra_classic_sdk-2.0.8/terra_classic_sdk/core/fee.py
--rw-r--r--   0        0        0      297 2023-04-11 08:50:13.876956 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__init__.py
--rw-r--r--   0        0        0      433 2023-06-26 08:32:24.164784 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7469 2023-06-26 08:32:24.165025 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     3276 2023-06-26 08:32:24.165230 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     7787 2023-04-15 09:35:43.014420 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/data.py
--rw-r--r--   0        0        0     2895 2023-04-15 09:35:43.014435 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/msgs.py
--rw-r--r--   0        0        0      410 2023-04-11 08:50:13.898057 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__init__.py
--rw-r--r--   0        0        0      557 2023-06-26 08:32:24.165486 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5854 2023-06-26 08:32:24.165716 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     6013 2023-06-26 08:32:24.165948 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     2106 2023-06-26 08:32:24.166247 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/proposals.cpython-310.pyc
--rw-r--r--   0        0        0     6179 2023-04-15 09:35:43.013549 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/data.py
--rw-r--r--   0        0        0     6540 2023-04-15 09:35:43.013517 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/msgs.py
--rw-r--r--   0        0        0     1510 2023-04-15 09:35:43.017624 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/proposals.py
--rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.885969 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/.DS_Store
--rw-r--r--   0        0        0       47 2023-04-11 08:50:13.886212 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/__init__.py
--rw-r--r--   0        0        0      238 2023-06-26 08:32:24.166482 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      492 2023-04-11 08:50:13.888431 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__init__.py
--rw-r--r--   0        0        0      599 2023-06-26 08:32:24.166737 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4765 2023-06-26 08:32:24.166961 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/channel.cpython-310.pyc
--rw-r--r--   0        0        0     6419 2023-06-26 08:32:24.167185 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0     2225 2023-06-26 08:32:24.167393 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/commitment.cpython-310.pyc
--rw-r--r--   0        0        0     2622 2023-06-26 08:32:24.167605 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/connection.cpython-310.pyc
--rw-r--r--   0        0        0     4813 2023-04-15 09:35:43.013917 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/channel.py
--rw-r--r--   0        0        0     5277 2023-04-15 09:35:43.013783 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/client.py
--rw-r--r--   0        0        0     1409 2023-04-15 09:35:43.013757 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/commitment.py
--rw-r--r--   0        0        0     1949 2023-04-15 09:35:43.013854 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/connection.py
--rw-r--r--   0        0        0      944 2023-04-11 08:50:13.887099 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__init__.py
--rw-r--r--   0        0        0      851 2023-06-26 08:32:24.167860 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    13123 2023-06-26 08:32:24.168123 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/channel.cpython-310.pyc
--rw-r--r--   0        0        0     5794 2023-06-26 08:32:24.168342 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0     8250 2023-06-26 08:32:24.168724 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/connection.cpython-310.pyc
--rw-r--r--   0        0        0    14696 2023-04-15 09:35:43.013835 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/channel.py
--rw-r--r--   0        0        0     5949 2023-04-15 09:35:43.013805 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/client.py
--rw-r--r--   0        0        0    10008 2023-04-15 09:35:43.013690 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/connection.py
--rw-r--r--   0        0        0       79 2023-04-11 08:50:13.889087 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__init__.py
--rw-r--r--   0        0        0      267 2023-06-26 08:32:24.169026 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2246 2023-06-26 08:32:24.169247 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__pycache__/proposals.cpython-310.pyc
--rw-r--r--   0        0        0     2146 2023-04-15 09:35:43.013944 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/proposals.py
--rw-r--r--   0        0        0      100 2023-04-11 08:50:13.881145 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__init__.py
--rw-r--r--   0        0        0      298 2023-06-26 08:32:24.169635 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1271 2023-06-26 08:32:24.169857 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     3107 2023-06-26 08:32:24.170070 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0      707 2023-04-15 09:35:43.014221 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/data.py
--rw-r--r--   0        0        0     3385 2023-04-15 09:35:43.014192 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/msgs.py
--rw-r--r--   0        0        0       77 2023-04-11 08:50:13.893419 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__init__.py
--rw-r--r--   0        0        0      271 2023-06-26 08:32:24.170327 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3810 2023-06-26 08:32:24.170555 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     3793 2023-04-15 09:35:43.013603 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/msgs.py
--rw-r--r--   0        0        0     3323 2023-04-15 09:35:43.013060 terra_classic_sdk-2.0.8/terra_classic_sdk/core/mode_info.py
--rw-r--r--   0        0        0      829 2023-04-15 09:35:43.012034 terra_classic_sdk-2.0.8/terra_classic_sdk/core/msg.py
--rw-r--r--   0        0        0     2430 2023-04-15 09:35:43.013203 terra_classic_sdk-2.0.8/terra_classic_sdk/core/multisig.py
--rw-r--r--   0        0        0    11374 2023-04-15 09:35:43.013157 terra_classic_sdk-2.0.8/terra_classic_sdk/core/numeric.py
--rw-r--r--   0        0        0      468 2023-04-11 08:50:13.882038 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__init__.py
--rw-r--r--   0        0        0      515 2023-06-26 08:32:24.170819 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4119 2023-06-26 08:32:24.171040 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     7738 2023-06-26 08:32:24.171385 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     3650 2023-04-15 09:35:43.014239 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/data.py
--rw-r--r--   0        0        0     7586 2023-04-15 09:35:43.014259 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/msgs.py
--rw-r--r--   0        0        0      114 2023-04-11 08:50:13.891484 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__init__.py
--rw-r--r--   0        0        0      292 2023-06-26 08:32:24.171825 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4444 2023-06-26 08:32:24.172048 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__pycache__/proposals.cpython-310.pyc
--rw-r--r--   0        0        0     3317 2023-04-15 09:35:43.013970 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/proposals.py
--rw-r--r--   0        0        0    10239 2023-04-15 09:35:43.012359 terra_classic_sdk-2.0.8/terra_classic_sdk/core/public_key.py
--rw-r--r--   0        0        0     2637 2023-04-15 09:35:43.012272 terra_classic_sdk-2.0.8/terra_classic_sdk/core/sign_doc.py
--rw-r--r--   0        0        0     3546 2023-04-11 08:50:13.891997 terra_classic_sdk-2.0.8/terra_classic_sdk/core/signature_v2.py
--rw-r--r--   0        0        0       53 2023-04-11 08:50:13.896443 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__init__.py
--rw-r--r--   0        0        0      246 2023-06-26 08:32:24.172292 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1757 2023-06-26 08:32:24.172492 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0     1111 2023-04-15 09:35:43.013583 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/msgs.py
--rw-r--r--   0        0        0      661 2023-04-11 08:50:13.889757 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__init__.py
--rw-r--r--   0        0        0      669 2023-06-26 08:32:24.172749 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8990 2023-06-26 08:32:24.172986 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0      429 2023-04-11 08:50:13.890702 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__init__.py
--rw-r--r--   0        0        0      529 2023-06-26 08:32:24.173240 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10270 2023-06-26 08:32:24.173485 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/delegation.cpython-310.pyc
--rw-r--r--   0        0        0     6623 2023-06-26 08:32:24.173718 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/validator.cpython-310.pyc
--rw-r--r--   0        0        0    11495 2023-04-15 09:35:43.013302 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/delegation.py
--rw-r--r--   0        0        0     7943 2023-04-15 09:35:43.014165 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/validator.py
--rw-r--r--   0        0        0    11049 2023-04-15 09:35:43.017202 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/msgs.py
--rw-r--r--   0        0        0       69 2023-04-11 08:50:13.895436 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__init__.py
--rw-r--r--   0        0        0      254 2023-06-26 08:32:24.174085 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2308 2023-06-26 08:32:24.174291 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     2276 2023-04-15 09:35:43.013629 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/data.py
--rw-r--r--   0        0        0    15356 2023-04-15 09:35:43.012406 terra_classic_sdk-2.0.8/terra_classic_sdk/core/tx.py
--rw-r--r--   0        0        0      176 2023-04-11 08:50:13.875622 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__init__.py
--rw-r--r--   0        0        0      346 2023-06-26 08:32:24.174643 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2323 2023-06-26 08:32:24.174849 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0        0        0      149 2023-04-11 08:50:13.876081 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__init__.py
--rw-r--r--   0        0        0      315 2023-06-26 08:32:24.175082 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-06-26 08:32:24.175285 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__pycache__/proposal.cpython-310.pyc
--rw-r--r--   0        0        0     3205 2023-04-15 09:35:43.014493 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/proposal.py
--rw-r--r--   0        0        0     2103 2023-04-15 09:35:43.014461 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/plan.py
--rw-r--r--   0        0        0      389 2023-04-11 08:50:13.883141 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__init__.py
--rw-r--r--   0        0        0      460 2023-06-26 08:32:24.175533 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12249 2023-06-26 08:32:24.175785 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__pycache__/msgs.cpython-310.pyc
--rw-r--r--   0        0        0    12801 2023-06-26 08:46:22.681651 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/msgs.py
--rw-r--r--   0        0        0      427 2023-04-11 08:50:13.903381 terra_classic_sdk-2.0.8/terra_classic_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.902809 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__init__.py
--rw-r--r--   0        0        0      176 2023-06-26 08:32:24.176654 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6763 2023-06-26 08:32:24.176875 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/key.cpython-310.pyc
--rw-r--r--   0        0        0     2269 2023-06-26 08:32:24.177060 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/mnemonic.cpython-310.pyc
--rw-r--r--   0        0        0     2215 2023-06-26 08:32:24.177244 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/raw.cpython-310.pyc
--rw-r--r--   0        0        0     8446 2023-06-28 03:21:35.643891 terra_classic_sdk-2.0.8/terra_classic_sdk/key/key.py
--rw-r--r--   0        0        0     2623 2023-06-26 08:46:25.391063 terra_classic_sdk-2.0.8/terra_classic_sdk/key/mnemonic.py
--rw-r--r--   0        0        0     1657 2023-04-11 08:50:13.902441 terra_classic_sdk-2.0.8/terra_classic_sdk/key/raw.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899834 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__init__.py
--rw-r--r--   0        0        0      177 2023-06-26 08:32:24.177465 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3035 2023-06-26 08:32:24.177839 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      436 2023-06-26 08:32:24.178019 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/converter.cpython-310.pyc
--rw-r--r--   0        0        0      474 2023-06-26 08:32:24.178200 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/hash.cpython-310.pyc
--rw-r--r--   0        0        0     2581 2023-06-26 08:32:24.178409 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/json.cpython-310.pyc
--rw-r--r--   0        0        0     1322 2023-06-26 08:32:24.178604 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/parse_content.cpython-310.pyc
--rw-r--r--   0        0        0     3150 2023-06-26 08:32:24.178817 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/parse_msg.cpython-310.pyc
--rw-r--r--   0        0        0      615 2023-06-26 08:32:24.178999 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/remove_none.cpython-310.pyc
--rw-r--r--   0        0        0      397 2023-06-26 08:32:24.179170 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/url.cpython-310.pyc
--rw-r--r--   0        0        0     1678 2023-04-11 08:50:13.901675 terra_classic_sdk-2.0.8/terra_classic_sdk/util/base.py
--rw-r--r--   0        0        0     3286 2023-04-15 09:35:43.014980 terra_classic_sdk-2.0.8/terra_classic_sdk/util/contract.py
--rw-r--r--   0        0        0      199 2023-04-11 08:50:13.899684 terra_classic_sdk-2.0.8/terra_classic_sdk/util/converter.py
--rw-r--r--   0        0        0      211 2023-04-11 08:50:13.900086 terra_classic_sdk-2.0.8/terra_classic_sdk/util/hash.py
--rw-r--r--   0        0        0     1708 2023-04-15 09:35:43.014942 terra_classic_sdk-2.0.8/terra_classic_sdk/util/json.py
--rw-r--r--   0        0        0      969 2023-04-15 09:35:43.014928 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_authorization.py
--rw-r--r--   0        0        0     2200 2023-04-15 09:35:43.014999 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_content.py
--rw-r--r--   0        0        0     4247 2023-04-15 09:35:43.014959 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_msg.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899175 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_proto.py
--rw-r--r--   0        0        0      294 2023-04-11 08:50:13.899454 terra_classic_sdk-2.0.8/terra_classic_sdk/util/remove_none.py
--rw-r--r--   0        0        0      133 2023-04-11 08:50:13.900320 terra_classic_sdk-2.0.8/terra_classic_sdk/util/url.py
--rw-r--r--   0        0        0    14212 1970-01-01 00:00:00.000000 terra_classic_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-11 08:50:13.847731 terra_classic_sdk-2.0.8.1/LICENSE
+-rw-r--r--   0        0        0    12754 2023-06-28 02:29:46.017082 terra_classic_sdk-2.0.8.1/README.md
+-rw-r--r--   0        0        0     1886 2023-07-02 05:01:38.708953 terra_classic_sdk-2.0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.872423 terra_classic_sdk-2.0.8.1/terra_classic_sdk/.DS_Store
+-rw-r--r--   0        0        0      161 2023-04-11 08:50:13.901954 terra_classic_sdk-2.0.8.1/terra_classic_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.904117 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/__init__.py
+-rw-r--r--   0        0        0      179 2023-06-26 08:32:24.148030 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3813 2023-06-26 08:32:24.148253 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/__pycache__/localterra.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-04-11 08:50:13.905477 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-26 08:32:24.148713 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9199 2023-06-26 08:32:24.149073 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/lcdclient.cpython-310.pyc
+-rw-r--r--   0        0        0     2853 2023-06-26 08:32:24.149298 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/lcdutils.cpython-310.pyc
+-rw-r--r--   0        0        0     2887 2023-06-26 08:32:24.149526 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/params.cpython-310.pyc
+-rw-r--r--   0        0        0     4733 2023-06-26 08:32:24.149761 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/wallet.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.907268 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-26 08:32:24.150055 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1407 2023-06-26 08:32:24.150263 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1489 2023-06-26 08:32:24.150491 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/auth.cpython-310.pyc
+-rw-r--r--   0        0        0     2127 2023-06-26 08:32:24.150892 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/authz.cpython-310.pyc
+-rw-r--r--   0        0        0     2200 2023-06-26 08:32:24.151103 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/bank.cpython-310.pyc
+-rw-r--r--   0        0        0     4304 2023-06-26 08:32:24.151436 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/distribution.cpython-310.pyc
+-rw-r--r--   0        0        0     2808 2023-06-26 08:32:24.151648 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/feegrant.cpython-310.pyc
+-rw-r--r--   0        0        0     9696 2023-06-26 08:32:24.151910 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/gov.cpython-310.pyc
+-rw-r--r--   0        0        0     1047 2023-06-26 08:32:24.152117 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/ibc.cpython-310.pyc
+-rw-r--r--   0        0        0     1203 2023-06-26 08:32:24.152347 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/ibc_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     2565 2023-06-26 08:32:24.152592 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/market.cpython-310.pyc
+-rw-r--r--   0        0        0     2255 2023-06-26 08:32:24.152796 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/mint.cpython-310.pyc
+-rw-r--r--   0        0        0     6379 2023-06-26 08:32:24.153054 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/oracle.cpython-310.pyc
+-rw-r--r--   0        0        0     3609 2023-06-26 08:32:24.153339 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/slashing.cpython-310.pyc
+-rw-r--r--   0        0        0    12230 2023-06-26 08:32:24.153836 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/staking.cpython-310.pyc
+-rw-r--r--   0        0        0     2940 2023-06-26 08:32:24.154072 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/tendermint.cpython-310.pyc
+-rw-r--r--   0        0        0     4270 2023-06-26 08:32:24.154331 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/treasury.cpython-310.pyc
+-rw-r--r--   0        0        0    15516 2023-06-26 08:32:24.154719 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/tx.cpython-310.pyc
+-rw-r--r--   0        0        0     3479 2023-06-26 08:32:24.154935 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/wasm.cpython-310.pyc
+-rw-r--r--   0        0        0      812 2023-04-11 08:50:13.906398 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/_base.py
+-rw-r--r--   0        0        0      982 2023-04-15 09:35:43.014907 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/auth.py
+-rw-r--r--   0        0        0     1616 2023-04-15 09:35:43.014689 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/authz.py
+-rw-r--r--   0        0        0     1618 2023-04-15 09:35:43.014832 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/bank.py
+-rw-r--r--   0        0        0     3633 2023-04-15 09:35:43.014773 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/distribution.py
+-rw-r--r--   0        0        0     2566 2023-04-15 09:35:43.014792 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/feegrant.py
+-rw-r--r--   0        0        0    10292 2023-04-15 09:35:43.014622 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/gov.py
+-rw-r--r--   0        0        0      587 2023-04-11 08:50:13.908029 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/ibc.py
+-rw-r--r--   0        0        0      762 2023-04-11 08:50:13.909254 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/ibc_transfer.py
+-rw-r--r--   0        0        0     2020 2023-04-15 09:35:43.014807 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/market.py
+-rw-r--r--   0        0        0     1836 2023-04-15 09:35:43.014730 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/mint.py
+-rw-r--r--   0        0        0     6371 2023-04-15 09:35:43.014757 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/oracle.py
+-rw-r--r--   0        0        0     3519 2023-04-15 09:35:43.014854 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/slashing.py
+-rw-r--r--   0        0        0    13208 2023-04-15 09:35:43.014885 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/staking.py
+-rw-r--r--   0        0        0     2453 2023-04-11 08:50:13.907101 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/tendermint.py
+-rw-r--r--   0        0        0     3770 2023-04-15 09:35:43.014638 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/treasury.py
+-rw-r--r--   0        0        0    14753 2023-06-25 10:33:24.003762 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/tx.py
+-rw-r--r--   0        0        0     3244 2023-06-26 08:46:22.680897 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/wasm.py
+-rw-r--r--   0        0        0    11889 2023-06-26 08:46:22.681285 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.014571 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/lcdutils.py
+-rw-r--r--   0        0        0     2394 2023-04-11 08:50:13.905004 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/params.py
+-rw-r--r--   0        0        0     5207 2023-04-15 09:35:43.014541 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/wallet.py
+-rw-r--r--   0        0        0     3700 2023-04-15 09:35:43.014511 terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/localterra.py
+-rw-r--r--   0        0        0    10244 2023-04-11 08:50:13.877728 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/.DS_Store
+-rw-r--r--   0        0        0      899 2023-04-11 08:50:13.884485 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__init__.py
+-rw-r--r--   0        0        0      986 2023-06-26 08:32:24.156487 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4724 2023-06-26 08:32:24.156738 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/bech32.cpython-310.pyc
+-rw-r--r--   0        0        0     2816 2023-06-26 08:32:24.156950 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/broadcast.cpython-310.pyc
+-rw-r--r--   0        0        0     8676 2023-06-26 08:32:24.157185 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/coin.cpython-310.pyc
+-rw-r--r--   0        0        0    11636 2023-06-26 08:32:24.157554 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/coins.cpython-310.pyc
+-rw-r--r--   0        0        0     3585 2023-06-26 08:32:24.157869 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/compact_bit_array.cpython-310.pyc
+-rw-r--r--   0        0        0     1495 2023-06-26 08:32:24.158171 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/deposit.cpython-310.pyc
+-rw-r--r--   0        0        0     2546 2023-06-26 08:32:24.158381 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/fee.cpython-310.pyc
+-rw-r--r--   0        0        0     4434 2023-06-26 08:32:24.158599 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/mode_info.cpython-310.pyc
+-rw-r--r--   0        0        0     1452 2023-06-26 08:32:24.158795 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/msg.cpython-310.pyc
+-rw-r--r--   0        0        0     2716 2023-06-26 08:32:24.159109 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/multisig.cpython-310.pyc
+-rw-r--r--   0        0        0    12613 2023-06-26 08:32:24.159455 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/numeric.cpython-310.pyc
+-rw-r--r--   0        0        0    12790 2023-06-26 08:32:24.159784 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/public_key.cpython-310.pyc
+-rw-r--r--   0        0        0     2982 2023-06-26 08:32:24.159992 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/sign_doc.cpython-310.pyc
+-rw-r--r--   0        0        0     4309 2023-06-26 08:32:24.160229 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/signature_v2.cpython-310.pyc
+-rw-r--r--   0        0        0    16009 2023-06-26 08:32:24.160530 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/tx.cpython-310.pyc
+-rw-r--r--   0        0        0      249 2023-04-11 08:50:13.878407 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-26 08:32:24.160897 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      403 2023-04-15 09:35:43.014285 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__init__.py
+-rw-r--r--   0        0        0      574 2023-06-26 08:32:24.161152 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1501 2023-06-26 08:32:24.161384 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/account.cpython-310.pyc
+-rw-r--r--   0        0        0     3063 2023-06-26 08:32:24.161583 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/base_account.cpython-310.pyc
+-rw-r--r--   0        0        0     3463 2023-06-26 08:32:24.161782 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/base_vesting_account.cpython-310.pyc
+-rw-r--r--   0        0        0     7577 2023-06-26 08:32:24.162006 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/lazy_graded_vesting_account.cpython-310.pyc
+-rw-r--r--   0        0        0     1003 2023-04-15 09:35:43.014339 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/account.py
+-rw-r--r--   0        0        0     2824 2023-04-11 08:50:13.879294 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/base_account.py
+-rw-r--r--   0        0        0     3948 2023-04-15 09:35:43.014303 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/base_vesting_account.py
+-rw-r--r--   0        0        0     5915 2023-04-15 09:35:43.014323 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py
+-rw-r--r--   0        0        0      446 2023-04-11 08:50:13.894143 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__init__.py
+-rw-r--r--   0        0        0      514 2023-06-26 08:32:24.162263 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10437 2023-06-26 08:32:24.162509 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     7364 2023-06-26 08:32:24.162724 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     9483 2023-04-15 09:35:43.013660 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/data.py
+-rw-r--r--   0        0        0     6103 2023-04-15 09:35:43.013727 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/msgs.py
+-rw-r--r--   0        0        0      149 2023-04-11 08:50:13.880447 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bank/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-26 08:32:24.163067 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bank/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9156 2023-06-26 08:32:24.163318 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bank/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     7220 2023-04-15 09:35:43.014366 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bank/msgs.py
+-rw-r--r--   0        0        0     4989 2023-04-11 08:50:13.876513 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bech32.py
+-rw-r--r--   0        0        0     1616 2023-04-11 08:50:13.894782 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/block.py
+-rw-r--r--   0        0        0     2736 2023-04-15 09:35:43.012322 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/broadcast.py
+-rw-r--r--   0        0        0     7757 2023-04-15 09:35:43.011986 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/coin.py
+-rw-r--r--   0        0        0     8364 2023-04-15 09:35:43.013020 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/coins.py
+-rw-r--r--   0        0        0     2866 2023-04-15 09:35:43.013363 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/compact_bit_array.py
+-rw-r--r--   0        0        0       71 2023-04-11 08:50:13.884925 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/crisis/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-26 08:32:24.163663 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/crisis/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2471 2023-06-26 08:32:24.163863 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/crisis/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     2075 2023-04-15 09:35:43.013412 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/crisis/msgs.py
+-rw-r--r--   0        0        0     1095 2023-04-15 09:35:43.013455 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/deposit.py
+-rw-r--r--   0        0        0      371 2023-04-11 08:50:13.883813 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/__init__.py
+-rw-r--r--   0        0        0      455 2023-06-26 08:32:24.164121 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6738 2023-06-26 08:32:24.164345 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     2895 2023-06-26 08:32:24.164546 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     6952 2023-04-15 09:35:43.014021 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/msgs.py
+-rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.013993 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/proposals.py
+-rw-r--r--   0        0        0     2024 2023-04-15 09:35:43.013238 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/fee.py
+-rw-r--r--   0        0        0      297 2023-04-11 08:50:13.876956 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/__init__.py
+-rw-r--r--   0        0        0      433 2023-06-26 08:32:24.164784 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7469 2023-06-26 08:32:24.165025 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     3276 2023-06-26 08:32:24.165230 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     7787 2023-04-15 09:35:43.014420 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/data.py
+-rw-r--r--   0        0        0     2895 2023-04-15 09:35:43.014435 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/msgs.py
+-rw-r--r--   0        0        0      410 2023-04-11 08:50:13.898057 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__init__.py
+-rw-r--r--   0        0        0      557 2023-06-26 08:32:24.165486 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5854 2023-06-26 08:32:24.165716 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     6013 2023-06-26 08:32:24.165948 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     2106 2023-06-26 08:32:24.166247 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     6179 2023-04-15 09:35:43.013549 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/data.py
+-rw-r--r--   0        0        0     6540 2023-04-15 09:35:43.013517 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/msgs.py
+-rw-r--r--   0        0        0     1510 2023-04-15 09:35:43.017624 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/proposals.py
+-rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.885969 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/.DS_Store
+-rw-r--r--   0        0        0       47 2023-04-11 08:50:13.886212 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/__init__.py
+-rw-r--r--   0        0        0      238 2023-06-26 08:32:24.166482 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      492 2023-04-11 08:50:13.888431 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-26 08:32:24.166737 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4765 2023-06-26 08:32:24.166961 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/channel.cpython-310.pyc
+-rw-r--r--   0        0        0     6419 2023-06-26 08:32:24.167185 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0     2225 2023-06-26 08:32:24.167393 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/commitment.cpython-310.pyc
+-rw-r--r--   0        0        0     2622 2023-06-26 08:32:24.167605 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0        0        0     4813 2023-04-15 09:35:43.013917 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/channel.py
+-rw-r--r--   0        0        0     5277 2023-04-15 09:35:43.013783 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/client.py
+-rw-r--r--   0        0        0     1409 2023-04-15 09:35:43.013757 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/commitment.py
+-rw-r--r--   0        0        0     1949 2023-04-15 09:35:43.013854 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/connection.py
+-rw-r--r--   0        0        0      944 2023-04-11 08:50:13.887099 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__init__.py
+-rw-r--r--   0        0        0      851 2023-06-26 08:32:24.167860 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13123 2023-06-26 08:32:24.168123 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/channel.cpython-310.pyc
+-rw-r--r--   0        0        0     5794 2023-06-26 08:32:24.168342 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0     8250 2023-06-26 08:32:24.168724 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0        0        0    14696 2023-04-15 09:35:43.013835 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/channel.py
+-rw-r--r--   0        0        0     5949 2023-04-15 09:35:43.013805 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/client.py
+-rw-r--r--   0        0        0    10008 2023-04-15 09:35:43.013690 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/connection.py
+-rw-r--r--   0        0        0       79 2023-04-11 08:50:13.889087 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/proposals/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-26 08:32:24.169026 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/proposals/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2246 2023-06-26 08:32:24.169247 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/proposals/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     2146 2023-04-15 09:35:43.013944 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/proposals/proposals.py
+-rw-r--r--   0        0        0      100 2023-04-11 08:50:13.881145 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-26 08:32:24.169635 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1271 2023-06-26 08:32:24.169857 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     3107 2023-06-26 08:32:24.170070 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0      707 2023-04-15 09:35:43.014221 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/data.py
+-rw-r--r--   0        0        0     3385 2023-04-15 09:35:43.014192 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/msgs.py
+-rw-r--r--   0        0        0       77 2023-04-11 08:50:13.893419 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/market/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-26 08:32:24.170327 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/market/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3810 2023-06-26 08:32:24.170555 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/market/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     3793 2023-04-15 09:35:43.013603 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/market/msgs.py
+-rw-r--r--   0        0        0     3323 2023-04-15 09:35:43.013060 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/mode_info.py
+-rw-r--r--   0        0        0      829 2023-04-15 09:35:43.012034 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/msg.py
+-rw-r--r--   0        0        0     2430 2023-04-15 09:35:43.013203 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/multisig.py
+-rw-r--r--   0        0        0    11374 2023-04-15 09:35:43.013157 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/numeric.py
+-rw-r--r--   0        0        0      468 2023-04-11 08:50:13.882038 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__init__.py
+-rw-r--r--   0        0        0      515 2023-06-26 08:32:24.170819 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4119 2023-06-26 08:32:24.171040 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     7738 2023-06-26 08:32:24.171385 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     3650 2023-04-15 09:35:43.014239 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/data.py
+-rw-r--r--   0        0        0     7586 2023-04-15 09:35:43.014259 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/msgs.py
+-rw-r--r--   0        0        0      114 2023-04-11 08:50:13.891484 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/params/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-26 08:32:24.171825 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/params/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4444 2023-06-26 08:32:24.172048 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/params/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     3317 2023-04-15 09:35:43.013970 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/params/proposals.py
+-rw-r--r--   0        0        0    10239 2023-04-15 09:35:43.012359 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/public_key.py
+-rw-r--r--   0        0        0     2637 2023-04-15 09:35:43.012272 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/sign_doc.py
+-rw-r--r--   0        0        0     3546 2023-04-11 08:50:13.891997 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/signature_v2.py
+-rw-r--r--   0        0        0       53 2023-04-11 08:50:13.896443 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/slashing/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-26 08:32:24.172292 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/slashing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1757 2023-06-26 08:32:24.172492 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/slashing/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     1111 2023-04-15 09:35:43.013583 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/slashing/msgs.py
+-rw-r--r--   0        0        0      661 2023-04-11 08:50:13.889757 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/__init__.py
+-rw-r--r--   0        0        0      669 2023-06-26 08:32:24.172749 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8990 2023-06-26 08:32:24.172986 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0      429 2023-04-11 08:50:13.890702 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-26 08:32:24.173240 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10270 2023-06-26 08:32:24.173485 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__pycache__/delegation.cpython-310.pyc
+-rw-r--r--   0        0        0     6623 2023-06-26 08:32:24.173718 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__pycache__/validator.cpython-310.pyc
+-rw-r--r--   0        0        0    11495 2023-04-15 09:35:43.013302 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/delegation.py
+-rw-r--r--   0        0        0     7943 2023-04-15 09:35:43.014165 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/validator.py
+-rw-r--r--   0        0        0    11049 2023-04-15 09:35:43.017202 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/msgs.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:50:13.895436 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/treasury/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-26 08:32:24.174085 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/treasury/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2308 2023-06-26 08:32:24.174291 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/treasury/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     2276 2023-04-15 09:35:43.013629 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/treasury/data.py
+-rw-r--r--   0        0        0    15356 2023-04-15 09:35:43.012406 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/tx.py
+-rw-r--r--   0        0        0      176 2023-04-11 08:50:13.875622 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-26 08:32:24.174643 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2323 2023-06-26 08:32:24.174849 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0        0        0      149 2023-04-11 08:50:13.876081 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/data/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-26 08:32:24.175082 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-06-26 08:32:24.175285 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/data/__pycache__/proposal.cpython-310.pyc
+-rw-r--r--   0        0        0     3205 2023-04-15 09:35:43.014493 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/data/proposal.py
+-rw-r--r--   0        0        0     2103 2023-04-15 09:35:43.014461 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/plan.py
+-rw-r--r--   0        0        0      389 2023-04-11 08:50:13.883141 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/wasm/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-26 08:32:24.175533 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/wasm/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12249 2023-06-26 08:32:24.175785 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/wasm/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0    12801 2023-06-26 08:46:22.681651 terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/wasm/msgs.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:50:13.903381 terra_classic_sdk-2.0.8.1/terra_classic_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.902809 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__init__.py
+-rw-r--r--   0        0        0      176 2023-06-26 08:32:24.176654 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6763 2023-06-26 08:32:24.176875 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/key.cpython-310.pyc
+-rw-r--r--   0        0        0     2269 2023-06-26 08:32:24.177060 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/mnemonic.cpython-310.pyc
+-rw-r--r--   0        0        0     2215 2023-06-26 08:32:24.177244 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/raw.cpython-310.pyc
+-rw-r--r--   0        0        0     8446 2023-06-28 03:21:35.643891 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/key.py
+-rw-r--r--   0        0        0     2623 2023-06-26 08:46:25.391063 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/mnemonic.py
+-rw-r--r--   0        0        0     1657 2023-04-11 08:50:13.902441 terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/raw.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899834 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__init__.py
+-rw-r--r--   0        0        0      177 2023-06-26 08:32:24.177465 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3035 2023-06-26 08:32:24.177839 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      436 2023-06-26 08:32:24.178019 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/converter.cpython-310.pyc
+-rw-r--r--   0        0        0      474 2023-06-26 08:32:24.178200 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/hash.cpython-310.pyc
+-rw-r--r--   0        0        0     2581 2023-06-26 08:32:24.178409 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/json.cpython-310.pyc
+-rw-r--r--   0        0        0     1322 2023-06-26 08:32:24.178604 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/parse_content.cpython-310.pyc
+-rw-r--r--   0        0        0     3150 2023-06-26 08:32:24.178817 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/parse_msg.cpython-310.pyc
+-rw-r--r--   0        0        0      615 2023-06-26 08:32:24.178999 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/remove_none.cpython-310.pyc
+-rw-r--r--   0        0        0      397 2023-06-26 08:32:24.179170 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/url.cpython-310.pyc
+-rw-r--r--   0        0        0     1678 2023-04-11 08:50:13.901675 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/base.py
+-rw-r--r--   0        0        0     3286 2023-04-15 09:35:43.014980 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/contract.py
+-rw-r--r--   0        0        0      199 2023-04-11 08:50:13.899684 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/converter.py
+-rw-r--r--   0        0        0      211 2023-04-11 08:50:13.900086 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/hash.py
+-rw-r--r--   0        0        0     1708 2023-04-15 09:35:43.014942 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/json.py
+-rw-r--r--   0        0        0      969 2023-04-15 09:35:43.014928 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_authorization.py
+-rw-r--r--   0        0        0     2200 2023-04-15 09:35:43.014999 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_content.py
+-rw-r--r--   0        0        0     4247 2023-04-15 09:35:43.014959 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_msg.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899175 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_proto.py
+-rw-r--r--   0        0        0      294 2023-04-11 08:50:13.899454 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/remove_none.py
+-rw-r--r--   0        0        0      133 2023-04-11 08:50:13.900320 terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/url.py
+-rw-r--r--   0        0        0    14214 1970-01-01 00:00:00.000000 terra_classic_sdk-2.0.8.1/PKG-INFO
```

### Comparing `terra_classic_sdk-2.0.8/LICENSE` & `terra_classic_sdk-2.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/README.md` & `terra_classic_sdk-2.0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/pyproject.toml` & `terra_classic_sdk-2.0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 documentation = "https://terra-money.github.io/terra.py/index.html"
 homepage = "https://github.com/geoffmunn/terra.py"
 keywords = ["jigu", "blockchain", "terra", "terra classic", "lunc", "defi", "crypto"]
 license = "MIT"
 packages = [{ include = "terra_classic_sdk" }]
 readme = "README.md"
 repository = "https://github.com/terra-money/terra.py"
-version = "2.0.8"
+version = "2.0.8.1"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.1"
 bech32 = "^1.2.0"
 bip32utils = "^0.3.post4"
 ecdsa = "^0.16.1"
 mnemonic = "^0.19"
```

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/.DS_Store` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/__pycache__/localterra.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/__pycache__/localterra.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/lcdclient.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/lcdclient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/lcdutils.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/lcdutils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/params.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/wallet.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/__pycache__/wallet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/_base.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/auth.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/authz.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/authz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/bank.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/bank.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/distribution.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/distribution.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/feegrant.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/feegrant.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/gov.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/gov.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/ibc.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/ibc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/ibc_transfer.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/ibc_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/market.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/market.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/mint.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/mint.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/oracle.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/oracle.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/slashing.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/slashing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/staking.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/staking.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/tendermint.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/tendermint.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/treasury.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/tx.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/tx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/wasm.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/__pycache__/wasm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/_base.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/_base.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/auth.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/auth.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/authz.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/authz.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/bank.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/bank.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/distribution.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/distribution.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/feegrant.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/feegrant.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/gov.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/gov.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/ibc.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc_transfer.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/market.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/market.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/mint.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/mint.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/oracle.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/oracle.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/slashing.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/slashing.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/staking.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/staking.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tendermint.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/tendermint.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/treasury.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/treasury.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tx.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/tx.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/wasm.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/api/wasm.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdclient.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/lcdclient.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdutils.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/lcdutils.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/params.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/params.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/wallet.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/lcd/wallet.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/client/localterra.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/client/localterra.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/.DS_Store` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__init__.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/bech32.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/bech32.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/broadcast.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/broadcast.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/coin.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/coin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/coins.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/coins.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/compact_bit_array.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/compact_bit_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/deposit.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/deposit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/fee.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/fee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/mode_info.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/mode_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/msg.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/msg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/multisig.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/multisig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/numeric.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/numeric.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/public_key.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/public_key.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/sign_doc.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/sign_doc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/signature_v2.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/signature_v2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/tx.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/__pycache__/tx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/account.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/account.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/base_account.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/base_account.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/base_vesting_account.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/base_vesting_account.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/lazy_graded_vesting_account.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/__pycache__/lazy_graded_vesting_account.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/account.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_account.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/base_account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_vesting_account.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/base_vesting_account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/data.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/data.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/authz/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bank/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bank/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/bech32.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/bech32.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/block.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/block.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/broadcast.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/broadcast.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/coin.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/coin.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/coins.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/coins.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/compact_bit_array.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/compact_bit_array.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/crisis/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/crisis/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/deposit.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/deposit.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/proposals.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/__pycache__/proposals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/proposals.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/distribution/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/fee.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/fee.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/data.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/data.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/feegrant/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/data.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/proposals.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/__pycache__/proposals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/data.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/proposals.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/gov/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/.DS_Store` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/.DS_Store`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/channel.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/channel.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/client.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/commitment.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/commitment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/connection.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/__pycache__/connection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/channel.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/channel.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/client.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/client.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/commitment.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/commitment.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/connection.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/data/connection.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__init__.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__init__.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/channel.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/channel.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/client.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/connection.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/__pycache__/connection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/channel.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/channel.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/client.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/client.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/connection.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/msgs/connection.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__pycache__/proposals.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/proposals/__pycache__/proposals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/proposals.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc/proposals/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/data.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/data.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/ibc_transfer/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/market/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/market/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/mode_info.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/mode_info.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/msg.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/msg.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/multisig.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/multisig.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/numeric.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/numeric.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/data.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/data.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/oracle/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__pycache__/proposals.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/params/__pycache__/proposals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/proposals.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/params/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/public_key.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/public_key.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/sign_doc.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/sign_doc.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/signature_v2.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/signature_v2.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/slashing/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/slashing/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__init__.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/__init__.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/__init__.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/delegation.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__pycache__/delegation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/validator.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/__pycache__/validator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/delegation.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/delegation.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/validator.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/data/validator.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/staking/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__pycache__/data.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/treasury/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/data.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/treasury/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/tx.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/tx.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__pycache__/plan.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/__pycache__/plan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__pycache__/proposal.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/data/__pycache__/proposal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/proposal.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/data/proposal.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/plan.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/upgrade/plan.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__pycache__/msgs.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/wasm/__pycache__/msgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/msgs.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/core/wasm/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/key.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/key.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/mnemonic.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/mnemonic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/raw.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/__pycache__/raw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/key/key.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/key.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/key/mnemonic.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/mnemonic.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/key/raw.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/key/raw.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/base.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/json.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/json.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/parse_content.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/parse_content.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/parse_msg.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/parse_msg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/remove_none.cpython-310.pyc` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/__pycache__/remove_none.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/base.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/base.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/contract.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/contract.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/json.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/json.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_authorization.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_authorization.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_content.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_content.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_msg.py` & `terra_classic_sdk-2.0.8.1/terra_classic_sdk/util/parse_msg.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.8/PKG-INFO` & `terra_classic_sdk-2.0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terra-classic-sdk
-Version: 2.0.8
+Version: 2.0.8.1
 Summary: The Python SDK for Terra Classic
 Home-page: https://github.com/geoffmunn/terra.py
 License: MIT
 Keywords: jigu,blockchain,terra,terra classic,lunc,defi,crypto
 Author: Geoff Munn
 Author-email: geoff@zimoobo.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: terra-classic-sdk Version: 2.0.8 Summary: The
+Metadata-Version: 2.1 Name: terra-classic-sdk Version: 2.0.8.1 Summary: The
 Python SDK for Terra Classic Home-page: https://github.com/geoffmunn/terra.py
 License: MIT Keywords: jigu,blockchain,terra,terra classic,lunc,defi,crypto
 Author: Geoff Munn Author-email: geoff@zimoobo.com Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

