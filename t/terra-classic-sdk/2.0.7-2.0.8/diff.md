# Comparing `tmp/terra_classic_sdk-2.0.7.tar.gz` & `tmp/terra_classic_sdk-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_classic_sdk-2.0.7.tar", max compression
+gzip compressed data, was "terra_classic_sdk-2.0.8.tar", max compression
```

## Comparing `terra_classic_sdk-2.0.7.tar` & `terra_classic_sdk-2.0.8.tar`

### file list

```diff
@@ -1,128 +1,243 @@
--rw-r--r--   0        0        0     1082 2023-04-11 08:50:13.847731 terra_classic_sdk-2.0.7/LICENSE
--rw-r--r--   0        0        0    12317 2023-04-15 09:35:43.011933 terra_classic_sdk-2.0.7/README.md
--rw-r--r--   0        0        0     1884 2023-04-15 10:14:27.538993 terra_classic_sdk-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.872423 terra_classic_sdk-2.0.7/terra_classic_sdk/.DS_Store
--rw-r--r--   0        0        0      161 2023-04-11 08:50:13.901954 terra_classic_sdk-2.0.7/terra_classic_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.904117 terra_classic_sdk-2.0.7/terra_classic_sdk/client/__init__.py
--rw-r--r--   0        0        0      216 2023-04-11 08:50:13.905477 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.907268 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/__init__.py
--rw-r--r--   0        0        0      812 2023-04-11 08:50:13.906398 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/_base.py
--rw-r--r--   0        0        0      982 2023-04-15 09:35:43.014907 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/auth.py
--rw-r--r--   0        0        0     1616 2023-04-15 09:35:43.014689 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/authz.py
--rw-r--r--   0        0        0     1618 2023-04-15 09:35:43.014832 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/bank.py
--rw-r--r--   0        0        0     3633 2023-04-15 09:35:43.014773 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/distribution.py
--rw-r--r--   0        0        0     2566 2023-04-15 09:35:43.014792 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/feegrant.py
--rw-r--r--   0        0        0    10292 2023-04-15 09:35:43.014622 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/gov.py
--rw-r--r--   0        0        0      587 2023-04-11 08:50:13.908029 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/ibc.py
--rw-r--r--   0        0        0      762 2023-04-11 08:50:13.909254 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/ibc_transfer.py
--rw-r--r--   0        0        0     2020 2023-04-15 09:35:43.014807 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/market.py
--rw-r--r--   0        0        0     1836 2023-04-15 09:35:43.014730 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/mint.py
--rw-r--r--   0        0        0     6371 2023-04-15 09:35:43.014757 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/oracle.py
--rw-r--r--   0        0        0     3519 2023-04-15 09:35:43.014854 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/slashing.py
--rw-r--r--   0        0        0    13208 2023-04-15 09:35:43.014885 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/staking.py
--rw-r--r--   0        0        0     2453 2023-04-11 08:50:13.907101 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/tendermint.py
--rw-r--r--   0        0        0     3770 2023-04-15 09:35:43.014638 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/treasury.py
--rw-r--r--   0        0        0    14753 2023-04-15 09:35:43.014662 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/tx.py
--rw-r--r--   0        0        0     3298 2023-04-15 09:35:43.014714 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/wasm.py
--rw-r--r--   0        0        0    12201 2023-04-15 09:35:43.014602 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/lcdclient.py
--rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.014571 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/lcdutils.py
--rw-r--r--   0        0        0     2394 2023-04-11 08:50:13.905004 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/params.py
--rw-r--r--   0        0        0     5207 2023-04-15 09:35:43.014541 terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/wallet.py
--rw-r--r--   0        0        0     3700 2023-04-15 09:35:43.014511 terra_classic_sdk-2.0.7/terra_classic_sdk/client/localterra.py
--rw-r--r--   0        0        0    10244 2023-04-11 08:50:13.877728 terra_classic_sdk-2.0.7/terra_classic_sdk/core/.DS_Store
--rw-r--r--   0        0        0      899 2023-04-11 08:50:13.884485 terra_classic_sdk-2.0.7/terra_classic_sdk/core/__init__.py
--rw-r--r--   0        0        0      249 2023-04-11 08:50:13.878407 terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/__init__.py
--rw-r--r--   0        0        0      403 2023-04-15 09:35:43.014285 terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/__init__.py
--rw-r--r--   0        0        0     1003 2023-04-15 09:35:43.014339 terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/account.py
--rw-r--r--   0        0        0     2824 2023-04-11 08:50:13.879294 terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/base_account.py
--rw-r--r--   0        0        0     3948 2023-04-15 09:35:43.014303 terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/base_vesting_account.py
--rw-r--r--   0        0        0     5915 2023-04-15 09:35:43.014323 terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py
--rw-r--r--   0        0        0      446 2023-04-11 08:50:13.894143 terra_classic_sdk-2.0.7/terra_classic_sdk/core/authz/__init__.py
--rw-r--r--   0        0        0     9483 2023-04-15 09:35:43.013660 terra_classic_sdk-2.0.7/terra_classic_sdk/core/authz/data.py
--rw-r--r--   0        0        0     6103 2023-04-15 09:35:43.013727 terra_classic_sdk-2.0.7/terra_classic_sdk/core/authz/msgs.py
--rw-r--r--   0        0        0      149 2023-04-11 08:50:13.880447 terra_classic_sdk-2.0.7/terra_classic_sdk/core/bank/__init__.py
--rw-r--r--   0        0        0     7220 2023-04-15 09:35:43.014366 terra_classic_sdk-2.0.7/terra_classic_sdk/core/bank/msgs.py
--rw-r--r--   0        0        0     4989 2023-04-11 08:50:13.876513 terra_classic_sdk-2.0.7/terra_classic_sdk/core/bech32.py
--rw-r--r--   0        0        0     1616 2023-04-11 08:50:13.894782 terra_classic_sdk-2.0.7/terra_classic_sdk/core/block.py
--rw-r--r--   0        0        0     2736 2023-04-15 09:35:43.012322 terra_classic_sdk-2.0.7/terra_classic_sdk/core/broadcast.py
--rw-r--r--   0        0        0     7757 2023-04-15 09:35:43.011986 terra_classic_sdk-2.0.7/terra_classic_sdk/core/coin.py
--rw-r--r--   0        0        0     8364 2023-04-15 09:35:43.013020 terra_classic_sdk-2.0.7/terra_classic_sdk/core/coins.py
--rw-r--r--   0        0        0     2866 2023-04-15 09:35:43.013363 terra_classic_sdk-2.0.7/terra_classic_sdk/core/compact_bit_array.py
--rw-r--r--   0        0        0       71 2023-04-11 08:50:13.884925 terra_classic_sdk-2.0.7/terra_classic_sdk/core/crisis/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-15 09:35:43.013412 terra_classic_sdk-2.0.7/terra_classic_sdk/core/crisis/msgs.py
--rw-r--r--   0        0        0     1095 2023-04-15 09:35:43.013455 terra_classic_sdk-2.0.7/terra_classic_sdk/core/deposit.py
--rw-r--r--   0        0        0      371 2023-04-11 08:50:13.883813 terra_classic_sdk-2.0.7/terra_classic_sdk/core/distribution/__init__.py
--rw-r--r--   0        0        0     6952 2023-04-15 09:35:43.014021 terra_classic_sdk-2.0.7/terra_classic_sdk/core/distribution/msgs.py
--rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.013993 terra_classic_sdk-2.0.7/terra_classic_sdk/core/distribution/proposals.py
--rw-r--r--   0        0        0     2024 2023-04-15 09:35:43.013238 terra_classic_sdk-2.0.7/terra_classic_sdk/core/fee.py
--rw-r--r--   0        0        0      297 2023-04-11 08:50:13.876956 terra_classic_sdk-2.0.7/terra_classic_sdk/core/feegrant/__init__.py
--rw-r--r--   0        0        0     7787 2023-04-15 09:35:43.014420 terra_classic_sdk-2.0.7/terra_classic_sdk/core/feegrant/data.py
--rw-r--r--   0        0        0     2895 2023-04-15 09:35:43.014435 terra_classic_sdk-2.0.7/terra_classic_sdk/core/feegrant/msgs.py
--rw-r--r--   0        0        0      410 2023-04-11 08:50:13.898057 terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/__init__.py
--rw-r--r--   0        0        0     6179 2023-04-15 09:35:43.013549 terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/data.py
--rw-r--r--   0        0        0     6540 2023-04-15 09:35:43.013517 terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/msgs.py
--rw-r--r--   0        0        0     1510 2023-04-15 09:35:43.017624 terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/proposals.py
--rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.885969 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/.DS_Store
--rw-r--r--   0        0        0       47 2023-04-11 08:50:13.886212 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/__init__.py
--rw-r--r--   0        0        0      492 2023-04-11 08:50:13.888431 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/__init__.py
--rw-r--r--   0        0        0     4813 2023-04-15 09:35:43.013917 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/channel.py
--rw-r--r--   0        0        0     5277 2023-04-15 09:35:43.013783 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/client.py
--rw-r--r--   0        0        0     1409 2023-04-15 09:35:43.013757 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/commitment.py
--rw-r--r--   0        0        0     1949 2023-04-15 09:35:43.013854 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/connection.py
--rw-r--r--   0        0        0      944 2023-04-11 08:50:13.887099 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/__init__.py
--rw-r--r--   0        0        0    14696 2023-04-15 09:35:43.013835 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/channel.py
--rw-r--r--   0        0        0     5949 2023-04-15 09:35:43.013805 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/client.py
--rw-r--r--   0        0        0    10008 2023-04-15 09:35:43.013690 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/connection.py
--rw-r--r--   0        0        0       79 2023-04-11 08:50:13.889087 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/proposals/__init__.py
--rw-r--r--   0        0        0     2146 2023-04-15 09:35:43.013944 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/proposals/proposals.py
--rw-r--r--   0        0        0      100 2023-04-11 08:50:13.881145 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc_transfer/__init__.py
--rw-r--r--   0        0        0      707 2023-04-15 09:35:43.014221 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc_transfer/data.py
--rw-r--r--   0        0        0     3385 2023-04-15 09:35:43.014192 terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc_transfer/msgs.py
--rw-r--r--   0        0        0       77 2023-04-11 08:50:13.893419 terra_classic_sdk-2.0.7/terra_classic_sdk/core/market/__init__.py
--rw-r--r--   0        0        0     3793 2023-04-15 09:35:43.013603 terra_classic_sdk-2.0.7/terra_classic_sdk/core/market/msgs.py
--rw-r--r--   0        0        0     3323 2023-04-15 09:35:43.013060 terra_classic_sdk-2.0.7/terra_classic_sdk/core/mode_info.py
--rw-r--r--   0        0        0      829 2023-04-15 09:35:43.012034 terra_classic_sdk-2.0.7/terra_classic_sdk/core/msg.py
--rw-r--r--   0        0        0     2430 2023-04-15 09:35:43.013203 terra_classic_sdk-2.0.7/terra_classic_sdk/core/multisig.py
--rw-r--r--   0        0        0    11374 2023-04-15 09:35:43.013157 terra_classic_sdk-2.0.7/terra_classic_sdk/core/numeric.py
--rw-r--r--   0        0        0      468 2023-04-11 08:50:13.882038 terra_classic_sdk-2.0.7/terra_classic_sdk/core/oracle/__init__.py
--rw-r--r--   0        0        0     3650 2023-04-15 09:35:43.014239 terra_classic_sdk-2.0.7/terra_classic_sdk/core/oracle/data.py
--rw-r--r--   0        0        0     7586 2023-04-15 09:35:43.014259 terra_classic_sdk-2.0.7/terra_classic_sdk/core/oracle/msgs.py
--rw-r--r--   0        0        0      114 2023-04-11 08:50:13.891484 terra_classic_sdk-2.0.7/terra_classic_sdk/core/params/__init__.py
--rw-r--r--   0        0        0     3317 2023-04-15 09:35:43.013970 terra_classic_sdk-2.0.7/terra_classic_sdk/core/params/proposals.py
--rw-r--r--   0        0        0    10239 2023-04-15 09:35:43.012359 terra_classic_sdk-2.0.7/terra_classic_sdk/core/public_key.py
--rw-r--r--   0        0        0     2637 2023-04-15 09:35:43.012272 terra_classic_sdk-2.0.7/terra_classic_sdk/core/sign_doc.py
--rw-r--r--   0        0        0     3546 2023-04-11 08:50:13.891997 terra_classic_sdk-2.0.7/terra_classic_sdk/core/signature_v2.py
--rw-r--r--   0        0        0       53 2023-04-11 08:50:13.896443 terra_classic_sdk-2.0.7/terra_classic_sdk/core/slashing/__init__.py
--rw-r--r--   0        0        0     1111 2023-04-15 09:35:43.013583 terra_classic_sdk-2.0.7/terra_classic_sdk/core/slashing/msgs.py
--rw-r--r--   0        0        0      661 2023-04-11 08:50:13.889757 terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/__init__.py
--rw-r--r--   0        0        0      429 2023-04-11 08:50:13.890702 terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/data/__init__.py
--rw-r--r--   0        0        0    11495 2023-04-15 09:35:43.013302 terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/data/delegation.py
--rw-r--r--   0        0        0     7943 2023-04-15 09:35:43.014165 terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/data/validator.py
--rw-r--r--   0        0        0    11049 2023-04-15 09:35:43.017202 terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/msgs.py
--rw-r--r--   0        0        0       69 2023-04-11 08:50:13.895436 terra_classic_sdk-2.0.7/terra_classic_sdk/core/treasury/__init__.py
--rw-r--r--   0        0        0     2276 2023-04-15 09:35:43.013629 terra_classic_sdk-2.0.7/terra_classic_sdk/core/treasury/data.py
--rw-r--r--   0        0        0    15356 2023-04-15 09:35:43.012406 terra_classic_sdk-2.0.7/terra_classic_sdk/core/tx.py
--rw-r--r--   0        0        0      176 2023-04-11 08:50:13.875622 terra_classic_sdk-2.0.7/terra_classic_sdk/core/upgrade/__init__.py
--rw-r--r--   0        0        0      149 2023-04-11 08:50:13.876081 terra_classic_sdk-2.0.7/terra_classic_sdk/core/upgrade/data/__init__.py
--rw-r--r--   0        0        0     3205 2023-04-15 09:35:43.014493 terra_classic_sdk-2.0.7/terra_classic_sdk/core/upgrade/data/proposal.py
--rw-r--r--   0        0        0     2103 2023-04-15 09:35:43.014461 terra_classic_sdk-2.0.7/terra_classic_sdk/core/upgrade/plan.py
--rw-r--r--   0        0        0      389 2023-04-11 08:50:13.883141 terra_classic_sdk-2.0.7/terra_classic_sdk/core/wasm/__init__.py
--rw-r--r--   0        0        0    12593 2023-04-15 09:35:43.014393 terra_classic_sdk-2.0.7/terra_classic_sdk/core/wasm/msgs.py
--rw-r--r--   0        0        0      427 2023-04-11 08:50:13.903381 terra_classic_sdk-2.0.7/terra_classic_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.902809 terra_classic_sdk-2.0.7/terra_classic_sdk/key/__init__.py
--rw-r--r--   0        0        0     7996 2023-04-15 09:35:43.015027 terra_classic_sdk-2.0.7/terra_classic_sdk/key/key.py
--rw-r--r--   0        0        0     2212 2023-04-11 08:50:13.903074 terra_classic_sdk-2.0.7/terra_classic_sdk/key/mnemonic.py
--rw-r--r--   0        0        0     1657 2023-04-11 08:50:13.902441 terra_classic_sdk-2.0.7/terra_classic_sdk/key/raw.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899834 terra_classic_sdk-2.0.7/terra_classic_sdk/util/__init__.py
--rw-r--r--   0        0        0     1678 2023-04-11 08:50:13.901675 terra_classic_sdk-2.0.7/terra_classic_sdk/util/base.py
--rw-r--r--   0        0        0     3286 2023-04-15 09:35:43.014980 terra_classic_sdk-2.0.7/terra_classic_sdk/util/contract.py
--rw-r--r--   0        0        0      199 2023-04-11 08:50:13.899684 terra_classic_sdk-2.0.7/terra_classic_sdk/util/converter.py
--rw-r--r--   0        0        0      211 2023-04-11 08:50:13.900086 terra_classic_sdk-2.0.7/terra_classic_sdk/util/hash.py
--rw-r--r--   0        0        0     1708 2023-04-15 09:35:43.014942 terra_classic_sdk-2.0.7/terra_classic_sdk/util/json.py
--rw-r--r--   0        0        0      969 2023-04-15 09:35:43.014928 terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_authorization.py
--rw-r--r--   0        0        0     2200 2023-04-15 09:35:43.014999 terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_content.py
--rw-r--r--   0        0        0     4247 2023-04-15 09:35:43.014959 terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_msg.py
--rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899175 terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_proto.py
--rw-r--r--   0        0        0      294 2023-04-11 08:50:13.899454 terra_classic_sdk-2.0.7/terra_classic_sdk/util/remove_none.py
--rw-r--r--   0        0        0      133 2023-04-11 08:50:13.900320 terra_classic_sdk-2.0.7/terra_classic_sdk/util/url.py
--rw-r--r--   0        0        0    14024 1970-01-01 00:00:00.000000 terra_classic_sdk-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-11 08:50:13.847731 terra_classic_sdk-2.0.8/LICENSE
+-rw-r--r--   0        0        0    12754 2023-06-28 02:29:46.017082 terra_classic_sdk-2.0.8/README.md
+-rw-r--r--   0        0        0     1884 2023-07-02 04:50:06.069721 terra_classic_sdk-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.872423 terra_classic_sdk-2.0.8/terra_classic_sdk/.DS_Store
+-rw-r--r--   0        0        0      161 2023-04-11 08:50:13.901954 terra_classic_sdk-2.0.8/terra_classic_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.904117 terra_classic_sdk-2.0.8/terra_classic_sdk/client/__init__.py
+-rw-r--r--   0        0        0      179 2023-06-26 08:32:24.148030 terra_classic_sdk-2.0.8/terra_classic_sdk/client/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3813 2023-06-26 08:32:24.148253 terra_classic_sdk-2.0.8/terra_classic_sdk/client/__pycache__/localterra.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-04-11 08:50:13.905477 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-26 08:32:24.148713 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9199 2023-06-26 08:32:24.149073 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/lcdclient.cpython-310.pyc
+-rw-r--r--   0        0        0     2853 2023-06-26 08:32:24.149298 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/lcdutils.cpython-310.pyc
+-rw-r--r--   0        0        0     2887 2023-06-26 08:32:24.149526 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/params.cpython-310.pyc
+-rw-r--r--   0        0        0     4733 2023-06-26 08:32:24.149761 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/__pycache__/wallet.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.907268 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-26 08:32:24.150055 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1407 2023-06-26 08:32:24.150263 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1489 2023-06-26 08:32:24.150491 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/auth.cpython-310.pyc
+-rw-r--r--   0        0        0     2127 2023-06-26 08:32:24.150892 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/authz.cpython-310.pyc
+-rw-r--r--   0        0        0     2200 2023-06-26 08:32:24.151103 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/bank.cpython-310.pyc
+-rw-r--r--   0        0        0     4304 2023-06-26 08:32:24.151436 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/distribution.cpython-310.pyc
+-rw-r--r--   0        0        0     2808 2023-06-26 08:32:24.151648 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/feegrant.cpython-310.pyc
+-rw-r--r--   0        0        0     9696 2023-06-26 08:32:24.151910 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/gov.cpython-310.pyc
+-rw-r--r--   0        0        0     1047 2023-06-26 08:32:24.152117 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/ibc.cpython-310.pyc
+-rw-r--r--   0        0        0     1203 2023-06-26 08:32:24.152347 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/ibc_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     2565 2023-06-26 08:32:24.152592 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/market.cpython-310.pyc
+-rw-r--r--   0        0        0     2255 2023-06-26 08:32:24.152796 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/mint.cpython-310.pyc
+-rw-r--r--   0        0        0     6379 2023-06-26 08:32:24.153054 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/oracle.cpython-310.pyc
+-rw-r--r--   0        0        0     3609 2023-06-26 08:32:24.153339 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/slashing.cpython-310.pyc
+-rw-r--r--   0        0        0    12230 2023-06-26 08:32:24.153836 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/staking.cpython-310.pyc
+-rw-r--r--   0        0        0     2940 2023-06-26 08:32:24.154072 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/tendermint.cpython-310.pyc
+-rw-r--r--   0        0        0     4270 2023-06-26 08:32:24.154331 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/treasury.cpython-310.pyc
+-rw-r--r--   0        0        0    15516 2023-06-26 08:32:24.154719 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/tx.cpython-310.pyc
+-rw-r--r--   0        0        0     3479 2023-06-26 08:32:24.154935 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/__pycache__/wasm.cpython-310.pyc
+-rw-r--r--   0        0        0      812 2023-04-11 08:50:13.906398 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/_base.py
+-rw-r--r--   0        0        0      982 2023-04-15 09:35:43.014907 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/auth.py
+-rw-r--r--   0        0        0     1616 2023-04-15 09:35:43.014689 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/authz.py
+-rw-r--r--   0        0        0     1618 2023-04-15 09:35:43.014832 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/bank.py
+-rw-r--r--   0        0        0     3633 2023-04-15 09:35:43.014773 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/distribution.py
+-rw-r--r--   0        0        0     2566 2023-04-15 09:35:43.014792 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/feegrant.py
+-rw-r--r--   0        0        0    10292 2023-04-15 09:35:43.014622 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/gov.py
+-rw-r--r--   0        0        0      587 2023-04-11 08:50:13.908029 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc.py
+-rw-r--r--   0        0        0      762 2023-04-11 08:50:13.909254 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc_transfer.py
+-rw-r--r--   0        0        0     2020 2023-04-15 09:35:43.014807 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/market.py
+-rw-r--r--   0        0        0     1836 2023-04-15 09:35:43.014730 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/mint.py
+-rw-r--r--   0        0        0     6371 2023-04-15 09:35:43.014757 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/oracle.py
+-rw-r--r--   0        0        0     3519 2023-04-15 09:35:43.014854 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/slashing.py
+-rw-r--r--   0        0        0    13208 2023-04-15 09:35:43.014885 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/staking.py
+-rw-r--r--   0        0        0     2453 2023-04-11 08:50:13.907101 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tendermint.py
+-rw-r--r--   0        0        0     3770 2023-04-15 09:35:43.014638 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/treasury.py
+-rw-r--r--   0        0        0    14753 2023-06-25 10:33:24.003762 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tx.py
+-rw-r--r--   0        0        0     3244 2023-06-26 08:46:22.680897 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/wasm.py
+-rw-r--r--   0        0        0    11889 2023-06-26 08:46:22.681285 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.014571 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdutils.py
+-rw-r--r--   0        0        0     2394 2023-04-11 08:50:13.905004 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/params.py
+-rw-r--r--   0        0        0     5207 2023-04-15 09:35:43.014541 terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/wallet.py
+-rw-r--r--   0        0        0     3700 2023-04-15 09:35:43.014511 terra_classic_sdk-2.0.8/terra_classic_sdk/client/localterra.py
+-rw-r--r--   0        0        0    10244 2023-04-11 08:50:13.877728 terra_classic_sdk-2.0.8/terra_classic_sdk/core/.DS_Store
+-rw-r--r--   0        0        0      899 2023-04-11 08:50:13.884485 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__init__.py
+-rw-r--r--   0        0        0      986 2023-06-26 08:32:24.156487 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4724 2023-06-26 08:32:24.156738 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/bech32.cpython-310.pyc
+-rw-r--r--   0        0        0     2816 2023-06-26 08:32:24.156950 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/broadcast.cpython-310.pyc
+-rw-r--r--   0        0        0     8676 2023-06-26 08:32:24.157185 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/coin.cpython-310.pyc
+-rw-r--r--   0        0        0    11636 2023-06-26 08:32:24.157554 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/coins.cpython-310.pyc
+-rw-r--r--   0        0        0     3585 2023-06-26 08:32:24.157869 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/compact_bit_array.cpython-310.pyc
+-rw-r--r--   0        0        0     1495 2023-06-26 08:32:24.158171 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/deposit.cpython-310.pyc
+-rw-r--r--   0        0        0     2546 2023-06-26 08:32:24.158381 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/fee.cpython-310.pyc
+-rw-r--r--   0        0        0     4434 2023-06-26 08:32:24.158599 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/mode_info.cpython-310.pyc
+-rw-r--r--   0        0        0     1452 2023-06-26 08:32:24.158795 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/msg.cpython-310.pyc
+-rw-r--r--   0        0        0     2716 2023-06-26 08:32:24.159109 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/multisig.cpython-310.pyc
+-rw-r--r--   0        0        0    12613 2023-06-26 08:32:24.159455 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/numeric.cpython-310.pyc
+-rw-r--r--   0        0        0    12790 2023-06-26 08:32:24.159784 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/public_key.cpython-310.pyc
+-rw-r--r--   0        0        0     2982 2023-06-26 08:32:24.159992 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/sign_doc.cpython-310.pyc
+-rw-r--r--   0        0        0     4309 2023-06-26 08:32:24.160229 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/signature_v2.cpython-310.pyc
+-rw-r--r--   0        0        0    16009 2023-06-26 08:32:24.160530 terra_classic_sdk-2.0.8/terra_classic_sdk/core/__pycache__/tx.cpython-310.pyc
+-rw-r--r--   0        0        0      249 2023-04-11 08:50:13.878407 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-26 08:32:24.160897 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      403 2023-04-15 09:35:43.014285 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__init__.py
+-rw-r--r--   0        0        0      574 2023-06-26 08:32:24.161152 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1501 2023-06-26 08:32:24.161384 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/account.cpython-310.pyc
+-rw-r--r--   0        0        0     3063 2023-06-26 08:32:24.161583 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/base_account.cpython-310.pyc
+-rw-r--r--   0        0        0     3463 2023-06-26 08:32:24.161782 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/base_vesting_account.cpython-310.pyc
+-rw-r--r--   0        0        0     7577 2023-06-26 08:32:24.162006 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/__pycache__/lazy_graded_vesting_account.cpython-310.pyc
+-rw-r--r--   0        0        0     1003 2023-04-15 09:35:43.014339 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/account.py
+-rw-r--r--   0        0        0     2824 2023-04-11 08:50:13.879294 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_account.py
+-rw-r--r--   0        0        0     3948 2023-04-15 09:35:43.014303 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_vesting_account.py
+-rw-r--r--   0        0        0     5915 2023-04-15 09:35:43.014323 terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py
+-rw-r--r--   0        0        0      446 2023-04-11 08:50:13.894143 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__init__.py
+-rw-r--r--   0        0        0      514 2023-06-26 08:32:24.162263 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10437 2023-06-26 08:32:24.162509 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     7364 2023-06-26 08:32:24.162724 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     9483 2023-04-15 09:35:43.013660 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/data.py
+-rw-r--r--   0        0        0     6103 2023-04-15 09:35:43.013727 terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/msgs.py
+-rw-r--r--   0        0        0      149 2023-04-11 08:50:13.880447 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-26 08:32:24.163067 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9156 2023-06-26 08:32:24.163318 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     7220 2023-04-15 09:35:43.014366 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/msgs.py
+-rw-r--r--   0        0        0     4989 2023-04-11 08:50:13.876513 terra_classic_sdk-2.0.8/terra_classic_sdk/core/bech32.py
+-rw-r--r--   0        0        0     1616 2023-04-11 08:50:13.894782 terra_classic_sdk-2.0.8/terra_classic_sdk/core/block.py
+-rw-r--r--   0        0        0     2736 2023-04-15 09:35:43.012322 terra_classic_sdk-2.0.8/terra_classic_sdk/core/broadcast.py
+-rw-r--r--   0        0        0     7757 2023-04-15 09:35:43.011986 terra_classic_sdk-2.0.8/terra_classic_sdk/core/coin.py
+-rw-r--r--   0        0        0     8364 2023-04-15 09:35:43.013020 terra_classic_sdk-2.0.8/terra_classic_sdk/core/coins.py
+-rw-r--r--   0        0        0     2866 2023-04-15 09:35:43.013363 terra_classic_sdk-2.0.8/terra_classic_sdk/core/compact_bit_array.py
+-rw-r--r--   0        0        0       71 2023-04-11 08:50:13.884925 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-26 08:32:24.163663 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2471 2023-06-26 08:32:24.163863 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     2075 2023-04-15 09:35:43.013412 terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/msgs.py
+-rw-r--r--   0        0        0     1095 2023-04-15 09:35:43.013455 terra_classic_sdk-2.0.8/terra_classic_sdk/core/deposit.py
+-rw-r--r--   0        0        0      371 2023-04-11 08:50:13.883813 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__init__.py
+-rw-r--r--   0        0        0      455 2023-06-26 08:32:24.164121 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6738 2023-06-26 08:32:24.164345 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     2895 2023-06-26 08:32:24.164546 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     6952 2023-04-15 09:35:43.014021 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/msgs.py
+-rw-r--r--   0        0        0     2633 2023-04-15 09:35:43.013993 terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/proposals.py
+-rw-r--r--   0        0        0     2024 2023-04-15 09:35:43.013238 terra_classic_sdk-2.0.8/terra_classic_sdk/core/fee.py
+-rw-r--r--   0        0        0      297 2023-04-11 08:50:13.876956 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__init__.py
+-rw-r--r--   0        0        0      433 2023-06-26 08:32:24.164784 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7469 2023-06-26 08:32:24.165025 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     3276 2023-06-26 08:32:24.165230 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     7787 2023-04-15 09:35:43.014420 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/data.py
+-rw-r--r--   0        0        0     2895 2023-04-15 09:35:43.014435 terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/msgs.py
+-rw-r--r--   0        0        0      410 2023-04-11 08:50:13.898057 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__init__.py
+-rw-r--r--   0        0        0      557 2023-06-26 08:32:24.165486 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5854 2023-06-26 08:32:24.165716 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     6013 2023-06-26 08:32:24.165948 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     2106 2023-06-26 08:32:24.166247 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     6179 2023-04-15 09:35:43.013549 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/data.py
+-rw-r--r--   0        0        0     6540 2023-04-15 09:35:43.013517 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/msgs.py
+-rw-r--r--   0        0        0     1510 2023-04-15 09:35:43.017624 terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/proposals.py
+-rw-r--r--   0        0        0     6148 2023-04-11 08:50:13.885969 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/.DS_Store
+-rw-r--r--   0        0        0       47 2023-04-11 08:50:13.886212 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/__init__.py
+-rw-r--r--   0        0        0      238 2023-06-26 08:32:24.166482 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      492 2023-04-11 08:50:13.888431 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-26 08:32:24.166737 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4765 2023-06-26 08:32:24.166961 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/channel.cpython-310.pyc
+-rw-r--r--   0        0        0     6419 2023-06-26 08:32:24.167185 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0     2225 2023-06-26 08:32:24.167393 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/commitment.cpython-310.pyc
+-rw-r--r--   0        0        0     2622 2023-06-26 08:32:24.167605 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0        0        0     4813 2023-04-15 09:35:43.013917 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/channel.py
+-rw-r--r--   0        0        0     5277 2023-04-15 09:35:43.013783 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/client.py
+-rw-r--r--   0        0        0     1409 2023-04-15 09:35:43.013757 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/commitment.py
+-rw-r--r--   0        0        0     1949 2023-04-15 09:35:43.013854 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/connection.py
+-rw-r--r--   0        0        0      944 2023-04-11 08:50:13.887099 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__init__.py
+-rw-r--r--   0        0        0      851 2023-06-26 08:32:24.167860 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13123 2023-06-26 08:32:24.168123 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/channel.cpython-310.pyc
+-rw-r--r--   0        0        0     5794 2023-06-26 08:32:24.168342 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0     8250 2023-06-26 08:32:24.168724 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0        0        0    14696 2023-04-15 09:35:43.013835 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/channel.py
+-rw-r--r--   0        0        0     5949 2023-04-15 09:35:43.013805 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/client.py
+-rw-r--r--   0        0        0    10008 2023-04-15 09:35:43.013690 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/connection.py
+-rw-r--r--   0        0        0       79 2023-04-11 08:50:13.889087 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-26 08:32:24.169026 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2246 2023-06-26 08:32:24.169247 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     2146 2023-04-15 09:35:43.013944 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/proposals.py
+-rw-r--r--   0        0        0      100 2023-04-11 08:50:13.881145 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-26 08:32:24.169635 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1271 2023-06-26 08:32:24.169857 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     3107 2023-06-26 08:32:24.170070 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0      707 2023-04-15 09:35:43.014221 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/data.py
+-rw-r--r--   0        0        0     3385 2023-04-15 09:35:43.014192 terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/msgs.py
+-rw-r--r--   0        0        0       77 2023-04-11 08:50:13.893419 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-26 08:32:24.170327 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3810 2023-06-26 08:32:24.170555 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     3793 2023-04-15 09:35:43.013603 terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/msgs.py
+-rw-r--r--   0        0        0     3323 2023-04-15 09:35:43.013060 terra_classic_sdk-2.0.8/terra_classic_sdk/core/mode_info.py
+-rw-r--r--   0        0        0      829 2023-04-15 09:35:43.012034 terra_classic_sdk-2.0.8/terra_classic_sdk/core/msg.py
+-rw-r--r--   0        0        0     2430 2023-04-15 09:35:43.013203 terra_classic_sdk-2.0.8/terra_classic_sdk/core/multisig.py
+-rw-r--r--   0        0        0    11374 2023-04-15 09:35:43.013157 terra_classic_sdk-2.0.8/terra_classic_sdk/core/numeric.py
+-rw-r--r--   0        0        0      468 2023-04-11 08:50:13.882038 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__init__.py
+-rw-r--r--   0        0        0      515 2023-06-26 08:32:24.170819 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4119 2023-06-26 08:32:24.171040 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     7738 2023-06-26 08:32:24.171385 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     3650 2023-04-15 09:35:43.014239 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/data.py
+-rw-r--r--   0        0        0     7586 2023-04-15 09:35:43.014259 terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/msgs.py
+-rw-r--r--   0        0        0      114 2023-04-11 08:50:13.891484 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-26 08:32:24.171825 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4444 2023-06-26 08:32:24.172048 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/__pycache__/proposals.cpython-310.pyc
+-rw-r--r--   0        0        0     3317 2023-04-15 09:35:43.013970 terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/proposals.py
+-rw-r--r--   0        0        0    10239 2023-04-15 09:35:43.012359 terra_classic_sdk-2.0.8/terra_classic_sdk/core/public_key.py
+-rw-r--r--   0        0        0     2637 2023-04-15 09:35:43.012272 terra_classic_sdk-2.0.8/terra_classic_sdk/core/sign_doc.py
+-rw-r--r--   0        0        0     3546 2023-04-11 08:50:13.891997 terra_classic_sdk-2.0.8/terra_classic_sdk/core/signature_v2.py
+-rw-r--r--   0        0        0       53 2023-04-11 08:50:13.896443 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-26 08:32:24.172292 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1757 2023-06-26 08:32:24.172492 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0     1111 2023-04-15 09:35:43.013583 terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/msgs.py
+-rw-r--r--   0        0        0      661 2023-04-11 08:50:13.889757 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__init__.py
+-rw-r--r--   0        0        0      669 2023-06-26 08:32:24.172749 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8990 2023-06-26 08:32:24.172986 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0      429 2023-04-11 08:50:13.890702 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-26 08:32:24.173240 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10270 2023-06-26 08:32:24.173485 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/delegation.cpython-310.pyc
+-rw-r--r--   0        0        0     6623 2023-06-26 08:32:24.173718 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/__pycache__/validator.cpython-310.pyc
+-rw-r--r--   0        0        0    11495 2023-04-15 09:35:43.013302 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/delegation.py
+-rw-r--r--   0        0        0     7943 2023-04-15 09:35:43.014165 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/validator.py
+-rw-r--r--   0        0        0    11049 2023-04-15 09:35:43.017202 terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/msgs.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:50:13.895436 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-26 08:32:24.174085 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2308 2023-06-26 08:32:24.174291 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     2276 2023-04-15 09:35:43.013629 terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/data.py
+-rw-r--r--   0        0        0    15356 2023-04-15 09:35:43.012406 terra_classic_sdk-2.0.8/terra_classic_sdk/core/tx.py
+-rw-r--r--   0        0        0      176 2023-04-11 08:50:13.875622 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-26 08:32:24.174643 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2323 2023-06-26 08:32:24.174849 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0        0        0      149 2023-04-11 08:50:13.876081 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-26 08:32:24.175082 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-06-26 08:32:24.175285 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/__pycache__/proposal.cpython-310.pyc
+-rw-r--r--   0        0        0     3205 2023-04-15 09:35:43.014493 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/proposal.py
+-rw-r--r--   0        0        0     2103 2023-04-15 09:35:43.014461 terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/plan.py
+-rw-r--r--   0        0        0      389 2023-04-11 08:50:13.883141 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-26 08:32:24.175533 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12249 2023-06-26 08:32:24.175785 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/__pycache__/msgs.cpython-310.pyc
+-rw-r--r--   0        0        0    12801 2023-06-26 08:46:22.681651 terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/msgs.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:50:13.903381 terra_classic_sdk-2.0.8/terra_classic_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.902809 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__init__.py
+-rw-r--r--   0        0        0      176 2023-06-26 08:32:24.176654 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6763 2023-06-26 08:32:24.176875 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/key.cpython-310.pyc
+-rw-r--r--   0        0        0     2269 2023-06-26 08:32:24.177060 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/mnemonic.cpython-310.pyc
+-rw-r--r--   0        0        0     2215 2023-06-26 08:32:24.177244 terra_classic_sdk-2.0.8/terra_classic_sdk/key/__pycache__/raw.cpython-310.pyc
+-rw-r--r--   0        0        0     8446 2023-06-28 03:21:35.643891 terra_classic_sdk-2.0.8/terra_classic_sdk/key/key.py
+-rw-r--r--   0        0        0     2623 2023-06-26 08:46:25.391063 terra_classic_sdk-2.0.8/terra_classic_sdk/key/mnemonic.py
+-rw-r--r--   0        0        0     1657 2023-04-11 08:50:13.902441 terra_classic_sdk-2.0.8/terra_classic_sdk/key/raw.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899834 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__init__.py
+-rw-r--r--   0        0        0      177 2023-06-26 08:32:24.177465 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3035 2023-06-26 08:32:24.177839 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      436 2023-06-26 08:32:24.178019 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/converter.cpython-310.pyc
+-rw-r--r--   0        0        0      474 2023-06-26 08:32:24.178200 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/hash.cpython-310.pyc
+-rw-r--r--   0        0        0     2581 2023-06-26 08:32:24.178409 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/json.cpython-310.pyc
+-rw-r--r--   0        0        0     1322 2023-06-26 08:32:24.178604 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/parse_content.cpython-310.pyc
+-rw-r--r--   0        0        0     3150 2023-06-26 08:32:24.178817 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/parse_msg.cpython-310.pyc
+-rw-r--r--   0        0        0      615 2023-06-26 08:32:24.178999 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/remove_none.cpython-310.pyc
+-rw-r--r--   0        0        0      397 2023-06-26 08:32:24.179170 terra_classic_sdk-2.0.8/terra_classic_sdk/util/__pycache__/url.cpython-310.pyc
+-rw-r--r--   0        0        0     1678 2023-04-11 08:50:13.901675 terra_classic_sdk-2.0.8/terra_classic_sdk/util/base.py
+-rw-r--r--   0        0        0     3286 2023-04-15 09:35:43.014980 terra_classic_sdk-2.0.8/terra_classic_sdk/util/contract.py
+-rw-r--r--   0        0        0      199 2023-04-11 08:50:13.899684 terra_classic_sdk-2.0.8/terra_classic_sdk/util/converter.py
+-rw-r--r--   0        0        0      211 2023-04-11 08:50:13.900086 terra_classic_sdk-2.0.8/terra_classic_sdk/util/hash.py
+-rw-r--r--   0        0        0     1708 2023-04-15 09:35:43.014942 terra_classic_sdk-2.0.8/terra_classic_sdk/util/json.py
+-rw-r--r--   0        0        0      969 2023-04-15 09:35:43.014928 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_authorization.py
+-rw-r--r--   0        0        0     2200 2023-04-15 09:35:43.014999 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_content.py
+-rw-r--r--   0        0        0     4247 2023-04-15 09:35:43.014959 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_msg.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:50:13.899175 terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_proto.py
+-rw-r--r--   0        0        0      294 2023-04-11 08:50:13.899454 terra_classic_sdk-2.0.8/terra_classic_sdk/util/remove_none.py
+-rw-r--r--   0        0        0      133 2023-04-11 08:50:13.900320 terra_classic_sdk-2.0.8/terra_classic_sdk/util/url.py
+-rw-r--r--   0        0        0    14212 1970-01-01 00:00:00.000000 terra_classic_sdk-2.0.8/PKG-INFO
```

### Comparing `terra_classic_sdk-2.0.7/LICENSE` & `terra_classic_sdk-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/README.md` & `terra_classic_sdk-2.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 <br/>
 <br/>
 
 <div  align="center"> <p > <img src="https://raw.githubusercontent.com/terra-money/terra-sdk-python/main/docs/img/logo.png" width=500 alt="py-sdk-logo"></p>
 
-The Python SDK for Terra
+The Python SDK for Terra Classic
 <br/>
 
 <p><sub>(Unfamiliar with Terra?  <a href="https://docs.terra.money/">Check out the Terra Docs</a>)</sub></p>
 
   <p > <img alt="GitHub" src="https://img.shields.io/github/license/terra-money/terra-sdk-python">
 <img alt="Python" src="https://img.shields.io/pypi/pyversions/terra-sdk">
   <img alt="pip" src="https://img.shields.io/pypi/v/terra-sdk"></p>
 <p>
   <a href="https://terra-money.github.io/terra.py/index.html"><strong>Explore the Docs »</strong></a>
 <br/>
-  <a href="https://pypi.org/project/terra-sdk/">PyPI Package</a>
+  <a href="https://pypi.org/project/terra-classic-sdk/">PyPI Package</a>
   ·
-  <a href="https://github.com/terra-money/terra.py">GitHub Repository</a>
+  <a href="https://github.com/geoffmunn/terra.py">GitHub Repository</a>
 </p></div>
 
-The Terra Software Development Kit (SDK) in Python is a simple library toolkit for building software that can interact with the Terra blockchain and provides simple abstractions over core data structures, serialization, key management, and API request generation.
+The Terra Classic Software Development Kit (SDK) in Python is a simple library toolkit for building software that can interact with the Terra Classic blockchain and provides simple abstractions over core data structures, serialization, key management, and API request generation.
 
 ## Features
 
 - Written in Python with extensive support libraries
 - Versatile support for key management solutions
-- Exposes the Terra API through LCDClient
+- Exposes the Terra Classic API through LCDClient
+- Supports non-Terra Classic addresses for transactions
+- IBC swaps between non-Terra Classic chains are partially supported (where IBC channels exist)
 
 <br/>
 
 # Table of Contents
 
 - [API Reference](#api-reference)
 - [Getting Started](#getting-started)
@@ -60,70 +62,70 @@
 
 # Getting Started
 
 A walk-through of the steps to get started with the Terra SDK alongside a few use case examples are provided below. Alternatively, a tutorial video is also available <a href="https://www.youtube.com/watch?v=GfasBlJHKIg">here</a> as reference.
 
 ## Requirements
 
-Terra SDK requires <a href="https://www.python.org/downloads/">Python v3.7+</a>.
+Terra Classic SDK requires <a href="https://www.python.org/downloads/">Python v3.7+</a>.
 
 ## Installation
 
 <sub>**NOTE:** _All code starting with a `$` is meant to run on your terminal (a bash prompt). All code starting with a `>>>` is meant to run in a python interpreter, like <a href="https://pypi.org/project/ipython/">ipython</a>._</sub>
 
 Terra SDK can be installed (preferably in a `virtual environment` from PyPI using `pip`) as follows:
 
 ```
 $ pip install -U terra_classic_sdk
 ```
 
-<sub>_You might have `pip3` installed instead of `pip`; proceed according to your own setup._<sub>
+<sub>_You might need to run pip via ```python -m pip install -U terra_classic_sdk```. Additionally, you might have `pip3` installed instead of `pip`; proceed according to your own setup._<sub>
 
 ## Dependencies
 
-Terra SDK uses <a href="https://python-poetry.org/">Poetry</a> to manage dependencies. To get set up with all the required dependencies, run:
+Terra Classic SDK uses <a href="https://python-poetry.org/">Poetry</a> to manage dependencies. To get set up with all the required dependencies, run:
 
 ```
 $ pip install poetry
 $ poetry install
 ```
 
 ## Tests
 
-Terra SDK provides extensive tests for data classes and functions. To run them, after the steps in [Dependencies](#dependencies):
+Terra Classic SDK provides extensive tests for data classes and functions. To run them, after the steps in [Dependencies](#dependencies):
 
 ```
 $ make test
 ```
 
 ## Code Quality
 
-Terra SDK uses <a href="https://black.readthedocs.io/en/stable/">Black</a>, <a href="https://isort.readthedocs.io/en/latest/">isort</a>, and <a href="https://mypy.readthedocs.io/en/stable/index.html">Mypy</a> for checking code quality and maintaining style. To reformat, after the steps in [Dependencies](#dependencies):
+Terra Classic SDK uses <a href="https://black.readthedocs.io/en/stable/">Black</a>, <a href="https://isort.readthedocs.io/en/latest/">isort</a>, and <a href="https://mypy.readthedocs.io/en/stable/index.html">Mypy</a> for checking code quality and maintaining style. To reformat, after the steps in [Dependencies](#dependencies):
 
 ```
 $ make qa && make format
 ```
 
 <br/>
 
 # Usage Examples
 
-Terra SDK can help you read block data, sign and send transactions, deploy and interact with contracts, and many more.
-The following examples are provided to help you get started. Use cases and functionalities of the Terra SDK are not limited to the following examples and can be found in full <a href="https://terra-money.github.io/terra.py/index.html">here</a>.
+Terra Classic SDK can help you read block data, sign and send transactions, deploy and interact with contracts, and many more.
+The following examples are provided to help you get started. Use cases and functionalities of the Terra Classic SDK are not limited to the following examples and can be found in full <a href="https://terra-money.github.io/terra.py/index.html">here</a>.
 
-In order to interact with the Terra blockchain, you'll need a connection to a Terra node. This can be done through setting up an LCDClient (The LCDClient is an object representing an HTTP connection to a Terra LCD node.):
+In order to interact with the Terra Classic blockchain, you'll need a connection to a Terra Classic node. This can be done through setting up an LCDClient (The LCDClient is an object representing an HTTP connection to a Terra Classic LCD node.):
 
 ```
 >>> from terra_classic_sdk.client.lcd import LCDClient
->>> terra = LCDClient(chain_id="columbus-5", url="https://lcd.terra.dev")
+>>> terra = LCDClient(chain_id="columbus-5", url="https://terra-classic-lcd.publicnode.com")
 ```
 
 ## Getting Blockchain Information
 
-Once properly configured, the `LCDClient` instance will allow you to interact with the Terra blockchain. Try getting the latest block height:
+Once properly configured, the `LCDClient` instance will allow you to interact with the Terra Classic blockchain. Try getting the latest block height:
 
 ```
 >>> terra.tendermint.block_info()['block']['header']['height']
 ```
 
 `'1687543'`
 
@@ -132,41 +134,41 @@
 If you want to make asynchronous, non-blocking LCD requests, you can use AsyncLCDClient. The interface is similar to LCDClient, except the module and wallet API functions must be awaited.
 
 <pre><code>
 >>> import asyncio 
 >>> from terra_classic_sdk.client.lcd import AsyncLCDClient
 
 >>> async def main():
-      <strong>terra = AsyncLCDClient("https://lcd.terra.dev", "columbus-5")</strong>
+      <strong>terra = AsyncLCDClient("https://terra-classic-lcd.publicnode.com", "columbus-5")</strong>
       total_supply = await terra.bank.total()
       print(total_supply)
       <strong>await terra.session.close # you must close the session</strong>
 
 >>> asyncio.get_event_loop().run_until_complete(main())
 </code></pre>
 
 ## Building and Signing Transactions
 
-If you wish to perform a state-changing operation on the Terra blockchain such as sending tokens, swapping assets, withdrawing rewards, or even invoking functions on smart contracts, you must create a **transaction** and broadcast it to the network.
-Terra SDK provides functions that help create StdTx objects.
+If you wish to perform a state-changing operation on the Terra Classic blockchain such as sending tokens, swapping assets, withdrawing rewards, or even invoking functions on smart contracts, you must create a **transaction** and broadcast it to the network.
+Terra Classic SDK provides functions that help create StdTx objects.
 
 ### Example Using a Wallet (_recommended_)
 
 A `Wallet` allows you to create and sign a transaction in a single step by automatically fetching the latest information from the blockchain (chain ID, account number, sequence).
 
 Use `LCDClient.wallet()` to create a Wallet from any Key instance. The Key provided should correspond to the account you intend to sign the transaction with.
   
 <sub>**NOTE:** *If you are using MacOS and got an exception 'bad key length' from MnemonicKey, please check your python implementation. if `python3 -c "import ssl; print(ssl.OPENSSL_VERSION)"` returns LibreSSL 2.8.3, you need to reinstall python via pyenv or homebrew.*</sub>
 
 ```
 >>> from terra_classic_sdk.client.lcd import LCDClient
 >>> from terra_classic_sdk.key.mnemonic import MnemonicKey
 
 >>> mk = MnemonicKey(mnemonic=MNEMONIC)
->>> terra = LCDClient("https://lcd.terra.dev", "columbus-5")
+>>> terra = LCDClient("https://terra-classic-lcd.publicnode.com", "columbus-5")
 >>> wallet = terra.wallet(mk)
 ```
 
 Once you have your Wallet, you can simply create a StdTx using `Wallet.create_and_sign_tx`.
 
 ```
 >>> from terra_classic_sdk.core.fee import Fee
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 
 
                                  [py-sdk-logo]
-                           The Python SDK for Terra
+                       The Python SDK for Terra Classic
                (Unfamiliar with Terra? Check_out_the_Terra_Docs)
                             [GitHub] [Python] [pip]
                              Explore_the_Docs_Â»
                        PyPI_Package Â· GitHub_Repository
-The Terra Software Development Kit (SDK) in Python is a simple library toolkit
-for building software that can interact with the Terra blockchain and provides
-simple abstractions over core data structures, serialization, key management,
-and API request generation. ## Features - Written in Python with extensive
-support libraries - Versatile support for key management solutions - Exposes
-the Terra API through LCDClient
+The Terra Classic Software Development Kit (SDK) in Python is a simple library
+toolkit for building software that can interact with the Terra Classic
+blockchain and provides simple abstractions over core data structures,
+serialization, key management, and API request generation. ## Features -
+Written in Python with extensive support libraries - Versatile support for key
+management solutions - Exposes the Terra Classic API through LCDClient -
+Supports non-Terra Classic addresses for transactions - IBC swaps between non-
+Terra Classic chains are partially supported (where IBC channels exist)
 # Table of Contents - [API Reference](#api-reference) - [Getting Started]
 (#getting-started) - [Requirements](#requirements) - [Installation]
 (#installation) - [Dependencies](#dependencies) - [Tests](#tests) - [Code
 Quality](#code-quality) - [Usage Examples](#usage-examples) - [Getting
 Blockchain Information](#getting-blockchain-information) - [Async Usage]
 (#async-usage) - [Building and Signing Transactions](#building-and-signing-
 transactions) - [Example Using a Wallet](#example-using-a-wallet-recommended) -
@@ -23,76 +25,82 @@
 [Requesting a Feature](#requesting-a-feature) - [Contributing Code]
 (#contributing-code) - [Documentation Contributions](#documentation-
 contributions) - [License](#license)
 # API Reference An intricate reference to the APIs on the Terra SDK can be
 found here.
 # Getting Started A walk-through of the steps to get started with the Terra SDK
 alongside a few use case examples are provided below. Alternatively, a tutorial
-video is also available here as reference. ## Requirements Terra SDK requires
-Python_v3.7+. ## Installation **NOTE:** _All code starting with a `$` is meant
-to run on your terminal (a bash prompt). All code starting with a `>>>` is
-meant to run in a python interpreter, like ipython._ Terra SDK can be installed
-(preferably in a `virtual environment` from PyPI using `pip`) as follows: ``` $
-pip install -U terra_classic_sdk ``` _You might have `pip3` installed instead
-of `pip`; proceed according to your own setup._## Dependencies Terra SDK uses
-Poetry to manage dependencies. To get set up with all the required
-dependencies, run: ``` $ pip install poetry $ poetry install ``` ## Tests Terra
-SDK provides extensive tests for data classes and functions. To run them, after
-the steps in [Dependencies](#dependencies): ``` $ make test ``` ## Code Quality
-Terra SDK uses Black, isort, and Mypy for checking code quality and maintaining
-style. To reformat, after the steps in [Dependencies](#dependencies): ``` $
-make qa && make format ```
-# Usage Examples Terra SDK can help you read block data, sign and send
+video is also available here as reference. ## Requirements Terra Classic SDK
+requires Python_v3.7+. ## Installation **NOTE:** _All code starting with a `$`
+is meant to run on your terminal (a bash prompt). All code starting with a
+`>>>` is meant to run in a python interpreter, like ipython._ Terra SDK can be
+installed (preferably in a `virtual environment` from PyPI using `pip`) as
+follows: ``` $ pip install -U terra_classic_sdk ``` _You might need to run pip
+via ```python -m pip install -U terra_classic_sdk```. Additionally, you might
+have `pip3` installed instead of `pip`; proceed according to your own setup._##
+Dependencies Terra Classic SDK uses Poetry to manage dependencies. To get set
+up with all the required dependencies, run: ``` $ pip install poetry $ poetry
+install ``` ## Tests Terra Classic SDK provides extensive tests for data
+classes and functions. To run them, after the steps in [Dependencies]
+(#dependencies): ``` $ make test ``` ## Code Quality Terra Classic SDK uses
+Black, isort, and Mypy for checking code quality and maintaining style. To
+reformat, after the steps in [Dependencies](#dependencies): ``` $ make qa &&
+make format ```
+# Usage Examples Terra Classic SDK can help you read block data, sign and send
 transactions, deploy and interact with contracts, and many more. The following
 examples are provided to help you get started. Use cases and functionalities of
-the Terra SDK are not limited to the following examples and can be found in
-full here. In order to interact with the Terra blockchain, you'll need a
-connection to a Terra node. This can be done through setting up an LCDClient
-(The LCDClient is an object representing an HTTP connection to a Terra LCD
-node.): ``` >>> from terra_classic_sdk.client.lcd import LCDClient >>> terra =
-LCDClient(chain_id="columbus-5", url="https://lcd.terra.dev") ``` ## Getting
-Blockchain Information Once properly configured, the `LCDClient` instance will
-allow you to interact with the Terra blockchain. Try getting the latest block
-height: ``` >>> terra.tendermint.block_info()['block']['header']['height'] ```
-`'1687543'` ### Async Usage If you want to make asynchronous, non-blocking LCD
-requests, you can use AsyncLCDClient. The interface is similar to LCDClient,
-except the module and wallet API functions must be awaited.
+the Terra Classic SDK are not limited to the following examples and can be
+found in full here. In order to interact with the Terra Classic blockchain,
+you'll need a connection to a Terra Classic node. This can be done through
+setting up an LCDClient (The LCDClient is an object representing an HTTP
+connection to a Terra Classic LCD node.): ``` >>> from
+terra_classic_sdk.client.lcd import LCDClient >>> terra = LCDClient
+(chain_id="columbus-5", url="https://terra-classic-lcd.publicnode.com") ``` ##
+Getting Blockchain Information Once properly configured, the `LCDClient`
+instance will allow you to interact with the Terra Classic blockchain. Try
+getting the latest block height: ``` >>> terra.tendermint.block_info()['block']
+['header']['height'] ``` `'1687543'` ### Async Usage If you want to make
+asynchronous, non-blocking LCD requests, you can use AsyncLCDClient. The
+interface is similar to LCDClient, except the module and wallet API functions
+must be awaited.
 
 >>> import asyncio
 >>> from terra_classic_sdk.client.lcd import AsyncLCDClient
 
 >>> async def main():
-      terra = AsyncLCDClient("https://lcd.terra.dev", "columbus-5")
+      terra = AsyncLCDClient("https://terra-classic-lcd.publicnode.com",
+"columbus-5")
       total_supply = await terra.bank.total()
       print(total_supply)
       await terra.session.close # you must close the session
 
 >>> asyncio.get_event_loop().run_until_complete(main())
 ## Building and Signing Transactions If you wish to perform a state-changing
-operation on the Terra blockchain such as sending tokens, swapping assets,
-withdrawing rewards, or even invoking functions on smart contracts, you must
-create a **transaction** and broadcast it to the network. Terra SDK provides
-functions that help create StdTx objects. ### Example Using a Wallet
-(_recommended_) A `Wallet` allows you to create and sign a transaction in a
-single step by automatically fetching the latest information from the
+operation on the Terra Classic blockchain such as sending tokens, swapping
+assets, withdrawing rewards, or even invoking functions on smart contracts, you
+must create a **transaction** and broadcast it to the network. Terra Classic
+SDK provides functions that help create StdTx objects. ### Example Using a
+Wallet (_recommended_) A `Wallet` allows you to create and sign a transaction
+in a single step by automatically fetching the latest information from the
 blockchain (chain ID, account number, sequence). Use `LCDClient.wallet()` to
 create a Wallet from any Key instance. The Key provided should correspond to
 the account you intend to sign the transaction with. **NOTE:** *If you are
 using MacOS and got an exception 'bad key length' from MnemonicKey, please
 check your python implementation. if `python3 -c "import ssl; print
 (ssl.OPENSSL_VERSION)"` returns LibreSSL 2.8.3, you need to reinstall python
 via pyenv or homebrew.* ``` >>> from terra_classic_sdk.client.lcd import
 LCDClient >>> from terra_classic_sdk.key.mnemonic import MnemonicKey >>> mk =
-MnemonicKey(mnemonic=MNEMONIC) >>> terra = LCDClient("https://lcd.terra.dev",
-"columbus-5") >>> wallet = terra.wallet(mk) ``` Once you have your Wallet, you
-can simply create a StdTx using `Wallet.create_and_sign_tx`. ``` >>> from
-terra_classic_sdk.core.fee import Fee >>> from terra_classic_sdk.core.bank
-import MsgSend >>> from terra_classic_sdk.client.lcd.api.tx import
-CreateTxOptions >>> tx = wallet.create_and_sign_tx(CreateTxOptions( msgs=
-[MsgSend( wallet.key.acc_address, RECIPIENT, "1000000uluna" # send 1 luna )],
+MnemonicKey(mnemonic=MNEMONIC) >>> terra = LCDClient("https://terra-classic-
+lcd.publicnode.com", "columbus-5") >>> wallet = terra.wallet(mk) ``` Once you
+have your Wallet, you can simply create a StdTx using
+`Wallet.create_and_sign_tx`. ``` >>> from terra_classic_sdk.core.fee import Fee
+>>> from terra_classic_sdk.core.bank import MsgSend >>> from
+terra_classic_sdk.client.lcd.api.tx import CreateTxOptions >>> tx =
+wallet.create_and_sign_tx(CreateTxOptions( msgs=[MsgSend
+( wallet.key.acc_address, RECIPIENT, "1000000uluna" # send 1 luna )],
 memo="test transaction!", fee=Fee(200000, "120000uluna") )) ``` You should now
 be able to broadcast your transaction to the network. ``` >>> result =
 terra.tx.broadcast(tx) >>> print(result) ```
 # Contributing Community contribution, whether it's a new feature, correction,
 bug report, additional documentation, or any other feedback is always welcome.
 Please read through this section to ensure that your contribution is in the
 most suitable format for us to effectively process.
```

### Comparing `terra_classic_sdk-2.0.7/pyproject.toml` & `terra_classic_sdk-2.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 documentation = "https://terra-money.github.io/terra.py/index.html"
 homepage = "https://github.com/geoffmunn/terra.py"
 keywords = ["jigu", "blockchain", "terra", "terra classic", "lunc", "defi", "crypto"]
 license = "MIT"
 packages = [{ include = "terra_classic_sdk" }]
 readme = "README.md"
 repository = "https://github.com/terra-money/terra.py"
-version = "2.0.7"
+version = "2.0.8"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.1"
 bech32 = "^1.2.0"
 bip32utils = "^0.3.post4"
-ecdsa = "^0.17.0"
+ecdsa = "^0.16.1"
 mnemonic = "^0.19"
 python = "^3.7"
 protobuf = "^3.19.1"
 betterproto = "2.0.0b4"
 furl = "^2.1.3"
 boltons = "^21.0.0"
-terra-proto = "^1.0.1"
+terra-proto = "^3.0.1"
 nest-asyncio = "^1.5.4"
-attrs = "^21.4.0"
+attrs = "^20.3.0"
 wrapt = "^1.13.3"
 
 [tool.poetry.dev-dependencies]
 aioresponses = "^0.7.2"
 asynctest = "^0.13.0"
 pytest-cov = "^3.0.0"
 pytest = "^7.0.1"
```

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/.DS_Store` & `terra_classic_sdk-2.0.8/terra_classic_sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/_base.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/_base.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/auth.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/auth.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/authz.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/authz.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/bank.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/bank.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/distribution.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/distribution.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/feegrant.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/feegrant.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/gov.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/gov.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/ibc.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/ibc_transfer.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/market.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/market.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/mint.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/mint.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/oracle.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/oracle.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/slashing.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/slashing.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/staking.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/staking.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/tendermint.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tendermint.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/treasury.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/treasury.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/tx.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/tx.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/api/wasm.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/api/wasm.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,24 +52,23 @@
         Args:
             contract_address (str): contract address
             query (dict): QueryMsg to run
 
         Returns:
             Any: results of query
         """
-        params = {
-            "query_msg": base64.b64encode(json.dumps(query).encode("utf-8")).decode(
-                "utf-8"
-            )
-        }
+        
+        params = base64.b64encode(json.dumps(query).encode("utf-8")).decode("utf-8")
+
         res = await self._c._get(
-            f"/terra/wasm/v1beta1/contracts/{contract_address}/store", params
+            f"/cosmwasm/wasm/v1/contract/{contract_address}/smart/{params}"
         )
-        return res.get("query_result")
-
+        
+        return res.get("data")
+    
     async def parameters(self) -> dict:
         """Fetches the Wasm module parameters.
 
         Returns:
             dict: Wasm module parameters
         """
         res = await self._c._get("/terra/wasm/v1beta1/params")
```

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/lcdclient.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,26 +31,14 @@
 from .api.treasury import AsyncTreasuryAPI, TreasuryAPI
 from .api.tx import AsyncTxAPI, TxAPI
 from .api.wasm import AsyncWasmAPI, WasmAPI
 from .lcdutils import AsyncLCDUtils, LCDUtils
 from .params import APIParams
 from .wallet import AsyncWallet, Wallet
 
-
-def get_default(chain_id: str) -> [Coins, Numeric]:
-    if chain_id == "columbus-5":
-        return [Coins.from_str("0.15uusd"), Numeric.parse(1.75)]
-    if chain_id == "bombay-12":
-        return [Coins.from_str("0.15uusd"), Numeric.parse(1.75)]
-    if chain_id == "localterra":
-        return [Coins.from_str("0.15uusd"), Numeric.parse(1.75)]
-
-    raise ValueError("chain_id is invalid")
-
-
 class AsyncLCDClient:
     def __init__(
         self,
         url: str,
         chain_id: Optional[str] = None,
         gas_prices: Optional[Coins.Input] = None,
         gas_adjustment: Optional[Numeric.Input] = None,
@@ -65,15 +53,17 @@
                 headers={"Accept": "application/json"}, loop=self.loop
             )
 
         self.chain_id = chain_id
         self.url = url
         self.last_request_height = None
 
-        default_price, default_adjustment = get_default(chain_id)
+        #default_price, default_adjustment = get_default(chain_id)
+        default_price = Coins.from_str('1uluna')
+        default_adjustment = 1
         self.gas_prices = Coins(gas_prices) if gas_prices else default_price
         self.gas_adjustment = gas_adjustment if gas_adjustment else default_adjustment
 
         self.auth = AsyncAuthAPI(self)
         self.bank = AsyncBankAPI(self)
         self.distribution = AsyncDistributionAPI(self)
         self.feegrant = AsyncFeeGrantAPI(self)
```

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/lcdutils.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/lcdutils.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/params.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/params.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/lcd/wallet.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/lcd/wallet.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/client/localterra.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/client/localterra.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/.DS_Store` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/__init__.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/account.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/base_account.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/base_vesting_account.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/base_vesting_account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/auth/data/lazy_graded_vesting_account.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/authz/data.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/authz/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/authz/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/bank/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/bank/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/bech32.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/bech32.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/block.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/block.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/broadcast.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/broadcast.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/coin.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/coin.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/coins.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/coins.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/compact_bit_array.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/compact_bit_array.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/crisis/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/crisis/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/deposit.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/deposit.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/distribution/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/distribution/proposals.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/distribution/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/fee.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/fee.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/feegrant/data.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/feegrant/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/feegrant/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/data.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/gov/proposals.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/gov/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/.DS_Store` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/.DS_Store`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/channel.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/channel.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/client.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/client.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/commitment.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/commitment.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/data/connection.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/data/connection.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/__init__.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/__init__.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/channel.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/channel.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/client.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/client.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/msgs/connection.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/msgs/connection.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc/proposals/proposals.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc/proposals/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc_transfer/data.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/ibc_transfer/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/ibc_transfer/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/market/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/market/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/mode_info.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/mode_info.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/msg.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/msg.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/multisig.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/multisig.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/numeric.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/numeric.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/oracle/data.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/oracle/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/oracle/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/params/proposals.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/params/proposals.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/public_key.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/public_key.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/sign_doc.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/sign_doc.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/signature_v2.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/signature_v2.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/slashing/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/slashing/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/__init__.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/__init__.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/data/delegation.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/delegation.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/data/validator.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/data/validator.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/staking/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/staking/msgs.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/treasury/data.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/treasury/data.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/tx.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/tx.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/upgrade/data/proposal.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/data/proposal.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/upgrade/plan.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/upgrade/plan.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/core/wasm/msgs.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/core/wasm/msgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,16 @@
         execute_msg (dict|str): ExecuteMsg to pass
         coins: coins to be sent, if needed by contract to execute.
             Defaults to empty ``Coins()``
     """
 
     type_amino = "wasm/MsgExecuteContract"
     """"""
-    type_url = "/terra.wasm.v1beta1.MsgExecuteContract"
+    #type_url = "/terra.wasm.v1beta1.MsgExecuteContract"
+    type_url = "/cosmwasm.wasm.v1.MsgExecuteContract"
     """"""
     prototype = MsgExecuteContract_pb
     """"""
 
     sender: AccAddress = attr.ib()
     contract: AccAddress = attr.ib()
     execute_msg: Union[dict, str] = attr.ib()
@@ -236,19 +237,24 @@
                 "execute_msg": remove_none(self.execute_msg),
                 "coins": self.coins.to_amino(),
             },
         }
 
     @classmethod
     def from_data(cls, data: dict) -> MsgExecuteContract:
+
+        asset      = data['msg']['swap']['offer_asset']
+        amount:str = str(asset['amount'])
+        denom:str  = asset['info']['native_token']['denom']
+
         return cls(
             sender=data["sender"],
             contract=data["contract"],
-            execute_msg=parse_msg(data["execute_msg"]),
-            coins=Coins.from_data(data["coins"]),
+            execute_msg=parse_msg(data["msg"]),
+            coins = Coins.from_str(amount + denom)
         )
 
     def to_proto(self) -> MsgExecuteContract_pb:
         return MsgExecuteContract_pb(
             sender=self.sender,
             contract=self.contract,
             execute_msg=bytes(json.dumps(self.execute_msg), "utf-8"),
```

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/key/key.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/key/key.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             ValueError: if Key was not initialized with proper public key
 
         Returns:
             AccAddress: account address
         """
         if not self.raw_address:
             raise ValueError("could not compute acc_address: missing raw_address")
-        return AccAddress(get_bech("terra", self.raw_address.hex()))
+        return AccAddress(get_bech(self.prefix, self.raw_address.hex()))
 
     @property
     def val_address(self) -> ValAddress:
         """Terra Bech32 validator operator address. Default derivation via :data:`public_key` is provided.
 
         Raises:
             ValueError: if Key was not initialized with proper public key
@@ -101,14 +101,29 @@
             ValAddress: validator operator address
         """
         if not self.raw_address:
             raise ValueError("could not compute val_address: missing raw_address")
         return ValAddress(get_bech("terravaloper", self.raw_address.hex()))
 
     @property
+    def prefix(self) -> str:
+        """The prefix of the address that was created.
+        It would normally be 'terra', but could be other cosmos-compatible addresses.
+
+        Raises:
+            ValueError: if Key was not initialized any kind of value
+
+        Returns:
+            string
+        """
+        if not self.address_prefix:
+            raise ValueError("No address prefix found")
+        return self.address_prefix
+
+    @property
     def acc_pubkey(self) -> AccPubKey:
         """Terra Bech32 account pubkey. Default derivation via :data:`public_key` is provided.
 
         Raises:
             ValueError: if Key was not initialized with proper public key
 
         Returns:
@@ -234,8 +249,8 @@
         signedTx.auth_info.signer_infos.append(
             SignerInfo(
                 public_key=signature.public_key,
                 sequence=signature.sequence,
                 mode_info=ModeInfo(single=ModeInfoSingle(mode=sigData.mode)),
             )
         )
-        return signedTx
+        return signedTx
```

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/key/mnemonic.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/key/mnemonic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 from __future__ import annotations
 
 from bip32utils import BIP32_HARDEN, BIP32Key
 from mnemonic import Mnemonic
 
 from .raw import RawKey
 
-__all__ = ["MnemonicKey", "LUNA_COIN_TYPE"]
-
-LUNA_COIN_TYPE = 330
+__all__ = ["MnemonicKey"]
 
+coin_types = {
+    'cosmos': 118,
+    'juno': 118,
+    'kava': 459,
+    'kujira': 118,
+    'osmo': 118,
+    'terra': 330,
+    'emoney': 118,
+    'sif': 118,
+    'inj': 60,     # Possibly wrong coin type
+    'axelar': 118,
+    'umee': 118,
+    'omniflix': 118,
+    'gravity': 118,
+    'somm': 118
+}
 
 class MnemonicKey(RawKey):
     """A MnemonicKey derives a private key using a BIP39 mnemonic seed phrase, and provides key-derivation options based on the BIP44 HD path standard.
 
     .. note:: You can change ``coin_type`` to 118 to derive the key for a legacy Terra
         wallet (shares ``coin_type`` with ATOM).
 
@@ -32,14 +46,17 @@
 
     index: int
     """HD path parameter: account index."""
 
     coin_type: int
     """HD path parameter: coin type"""
 
+    prefix: str
+    """The prefix of the address - usually 'terra'"""
+
     @property
     def hd_path(self) -> str:
         """Returns the BIP32 HD path for key-derivation:
 
         ``m/44'/COIN_TYPE'/ACCOUNT'/0/INDEX'``
 
         Returns:
@@ -48,16 +65,19 @@
         return f"m/44'/{self.coin_type}'/{self.account}'/0/{self.index}"
 
     def __init__(
         self,
         mnemonic: str = None,
         account: int = 0,
         index: int = 0,
-        coin_type: int = LUNA_COIN_TYPE,
+        prefix:str = 'terra'
     ):
+        
+        coin_type = coin_types[prefix]
+        
         if mnemonic is None:
             mnemonic = Mnemonic("english").generate(256)
         seed = Mnemonic("english").to_seed(mnemonic)
         root = BIP32Key.fromEntropy(seed)
         # derive from hdpath
         child = (
             root.ChildKey(44 + BIP32_HARDEN)
@@ -68,7 +88,8 @@
         )
 
         super().__init__(child.PrivateKey())
         self.mnemonic = mnemonic
         self.coin_type = coin_type
         self.account = account
         self.index = index
+        self.address_prefix = prefix
```

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/key/raw.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/key/raw.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/util/base.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/util/base.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/util/contract.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/util/contract.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/util/json.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/util/json.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_authorization.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_authorization.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_content.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_content.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/terra_classic_sdk/util/parse_msg.py` & `terra_classic_sdk-2.0.8/terra_classic_sdk/util/parse_msg.py`

 * *Files identical despite different names*

### Comparing `terra_classic_sdk-2.0.7/PKG-INFO` & `terra_classic_sdk-2.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terra-classic-sdk
-Version: 2.0.7
+Version: 2.0.8
 Summary: The Python SDK for Terra Classic
 Home-page: https://github.com/geoffmunn/terra.py
 License: MIT
 Keywords: jigu,blockchain,terra,terra classic,lunc,defi,crypto
 Author: Geoff Munn
 Author-email: geoff@zimoobo.com
 Requires-Python: >=3.7,<4.0
@@ -13,64 +13,61 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: attrs (>=21.4.0,<22.0.0)
+Requires-Dist: attrs (>=20.3.0,<21.0.0)
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
 Requires-Dist: betterproto (==2.0.0b4)
 Requires-Dist: bip32utils (>=0.3.post4,<0.4)
 Requires-Dist: boltons (>=21.0.0,<22.0.0)
-Requires-Dist: ecdsa (>=0.17.0,<0.18.0)
+Requires-Dist: ecdsa (>=0.16.1,<0.17.0)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: mnemonic (>=0.19,<0.20)
 Requires-Dist: nest-asyncio (>=1.5.4,<2.0.0)
 Requires-Dist: protobuf (>=3.19.1,<4.0.0)
-Requires-Dist: terra-proto (>=1.0.1,<2.0.0)
+Requires-Dist: terra-proto (>=3.0.1,<4.0.0)
 Requires-Dist: wrapt (>=1.13.3,<2.0.0)
 Project-URL: Documentation, https://terra-money.github.io/terra.py/index.html
 Project-URL: Repository, https://github.com/terra-money/terra.py
 Description-Content-Type: text/markdown
 
 <br/>
 <br/>
 
 <div  align="center"> <p > <img src="https://raw.githubusercontent.com/terra-money/terra-sdk-python/main/docs/img/logo.png" width=500 alt="py-sdk-logo"></p>
 
-The Python SDK for Terra
+The Python SDK for Terra Classic
 <br/>
 
 <p><sub>(Unfamiliar with Terra?  <a href="https://docs.terra.money/">Check out the Terra Docs</a>)</sub></p>
 
   <p > <img alt="GitHub" src="https://img.shields.io/github/license/terra-money/terra-sdk-python">
 <img alt="Python" src="https://img.shields.io/pypi/pyversions/terra-sdk">
   <img alt="pip" src="https://img.shields.io/pypi/v/terra-sdk"></p>
 <p>
   <a href="https://terra-money.github.io/terra.py/index.html"><strong>Explore the Docs »</strong></a>
 <br/>
-  <a href="https://pypi.org/project/terra-sdk/">PyPI Package</a>
+  <a href="https://pypi.org/project/terra-classic-sdk/">PyPI Package</a>
   ·
-  <a href="https://github.com/terra-money/terra.py">GitHub Repository</a>
+  <a href="https://github.com/geoffmunn/terra.py">GitHub Repository</a>
 </p></div>
 
-The Terra Software Development Kit (SDK) in Python is a simple library toolkit for building software that can interact with the Terra blockchain and provides simple abstractions over core data structures, serialization, key management, and API request generation.
+The Terra Classic Software Development Kit (SDK) in Python is a simple library toolkit for building software that can interact with the Terra Classic blockchain and provides simple abstractions over core data structures, serialization, key management, and API request generation.
 
 ## Features
 
 - Written in Python with extensive support libraries
 - Versatile support for key management solutions
-- Exposes the Terra API through LCDClient
+- Exposes the Terra Classic API through LCDClient
+- Supports non-Terra Classic addresses for transactions
+- IBC swaps between non-Terra Classic chains are partially supported (where IBC channels exist)
 
 <br/>
 
 # Table of Contents
 
 - [API Reference](#api-reference)
 - [Getting Started](#getting-started)
@@ -101,70 +98,70 @@
 
 # Getting Started
 
 A walk-through of the steps to get started with the Terra SDK alongside a few use case examples are provided below. Alternatively, a tutorial video is also available <a href="https://www.youtube.com/watch?v=GfasBlJHKIg">here</a> as reference.
 
 ## Requirements
 
-Terra SDK requires <a href="https://www.python.org/downloads/">Python v3.7+</a>.
+Terra Classic SDK requires <a href="https://www.python.org/downloads/">Python v3.7+</a>.
 
 ## Installation
 
 <sub>**NOTE:** _All code starting with a `$` is meant to run on your terminal (a bash prompt). All code starting with a `>>>` is meant to run in a python interpreter, like <a href="https://pypi.org/project/ipython/">ipython</a>._</sub>
 
 Terra SDK can be installed (preferably in a `virtual environment` from PyPI using `pip`) as follows:
 
 ```
 $ pip install -U terra_classic_sdk
 ```
 
-<sub>_You might have `pip3` installed instead of `pip`; proceed according to your own setup._<sub>
+<sub>_You might need to run pip via ```python -m pip install -U terra_classic_sdk```. Additionally, you might have `pip3` installed instead of `pip`; proceed according to your own setup._<sub>
 
 ## Dependencies
 
-Terra SDK uses <a href="https://python-poetry.org/">Poetry</a> to manage dependencies. To get set up with all the required dependencies, run:
+Terra Classic SDK uses <a href="https://python-poetry.org/">Poetry</a> to manage dependencies. To get set up with all the required dependencies, run:
 
 ```
 $ pip install poetry
 $ poetry install
 ```
 
 ## Tests
 
-Terra SDK provides extensive tests for data classes and functions. To run them, after the steps in [Dependencies](#dependencies):
+Terra Classic SDK provides extensive tests for data classes and functions. To run them, after the steps in [Dependencies](#dependencies):
 
 ```
 $ make test
 ```
 
 ## Code Quality
 
-Terra SDK uses <a href="https://black.readthedocs.io/en/stable/">Black</a>, <a href="https://isort.readthedocs.io/en/latest/">isort</a>, and <a href="https://mypy.readthedocs.io/en/stable/index.html">Mypy</a> for checking code quality and maintaining style. To reformat, after the steps in [Dependencies](#dependencies):
+Terra Classic SDK uses <a href="https://black.readthedocs.io/en/stable/">Black</a>, <a href="https://isort.readthedocs.io/en/latest/">isort</a>, and <a href="https://mypy.readthedocs.io/en/stable/index.html">Mypy</a> for checking code quality and maintaining style. To reformat, after the steps in [Dependencies](#dependencies):
 
 ```
 $ make qa && make format
 ```
 
 <br/>
 
 # Usage Examples
 
-Terra SDK can help you read block data, sign and send transactions, deploy and interact with contracts, and many more.
-The following examples are provided to help you get started. Use cases and functionalities of the Terra SDK are not limited to the following examples and can be found in full <a href="https://terra-money.github.io/terra.py/index.html">here</a>.
+Terra Classic SDK can help you read block data, sign and send transactions, deploy and interact with contracts, and many more.
+The following examples are provided to help you get started. Use cases and functionalities of the Terra Classic SDK are not limited to the following examples and can be found in full <a href="https://terra-money.github.io/terra.py/index.html">here</a>.
 
-In order to interact with the Terra blockchain, you'll need a connection to a Terra node. This can be done through setting up an LCDClient (The LCDClient is an object representing an HTTP connection to a Terra LCD node.):
+In order to interact with the Terra Classic blockchain, you'll need a connection to a Terra Classic node. This can be done through setting up an LCDClient (The LCDClient is an object representing an HTTP connection to a Terra Classic LCD node.):
 
 ```
 >>> from terra_classic_sdk.client.lcd import LCDClient
->>> terra = LCDClient(chain_id="columbus-5", url="https://lcd.terra.dev")
+>>> terra = LCDClient(chain_id="columbus-5", url="https://terra-classic-lcd.publicnode.com")
 ```
 
 ## Getting Blockchain Information
 
-Once properly configured, the `LCDClient` instance will allow you to interact with the Terra blockchain. Try getting the latest block height:
+Once properly configured, the `LCDClient` instance will allow you to interact with the Terra Classic blockchain. Try getting the latest block height:
 
 ```
 >>> terra.tendermint.block_info()['block']['header']['height']
 ```
 
 `'1687543'`
 
@@ -173,41 +170,41 @@
 If you want to make asynchronous, non-blocking LCD requests, you can use AsyncLCDClient. The interface is similar to LCDClient, except the module and wallet API functions must be awaited.
 
 <pre><code>
 >>> import asyncio 
 >>> from terra_classic_sdk.client.lcd import AsyncLCDClient
 
 >>> async def main():
-      <strong>terra = AsyncLCDClient("https://lcd.terra.dev", "columbus-5")</strong>
+      <strong>terra = AsyncLCDClient("https://terra-classic-lcd.publicnode.com", "columbus-5")</strong>
       total_supply = await terra.bank.total()
       print(total_supply)
       <strong>await terra.session.close # you must close the session</strong>
 
 >>> asyncio.get_event_loop().run_until_complete(main())
 </code></pre>
 
 ## Building and Signing Transactions
 
-If you wish to perform a state-changing operation on the Terra blockchain such as sending tokens, swapping assets, withdrawing rewards, or even invoking functions on smart contracts, you must create a **transaction** and broadcast it to the network.
-Terra SDK provides functions that help create StdTx objects.
+If you wish to perform a state-changing operation on the Terra Classic blockchain such as sending tokens, swapping assets, withdrawing rewards, or even invoking functions on smart contracts, you must create a **transaction** and broadcast it to the network.
+Terra Classic SDK provides functions that help create StdTx objects.
 
 ### Example Using a Wallet (_recommended_)
 
 A `Wallet` allows you to create and sign a transaction in a single step by automatically fetching the latest information from the blockchain (chain ID, account number, sequence).
 
 Use `LCDClient.wallet()` to create a Wallet from any Key instance. The Key provided should correspond to the account you intend to sign the transaction with.
   
 <sub>**NOTE:** *If you are using MacOS and got an exception 'bad key length' from MnemonicKey, please check your python implementation. if `python3 -c "import ssl; print(ssl.OPENSSL_VERSION)"` returns LibreSSL 2.8.3, you need to reinstall python via pyenv or homebrew.*</sub>
 
 ```
 >>> from terra_classic_sdk.client.lcd import LCDClient
 >>> from terra_classic_sdk.key.mnemonic import MnemonicKey
 
 >>> mk = MnemonicKey(mnemonic=MNEMONIC)
->>> terra = LCDClient("https://lcd.terra.dev", "columbus-5")
+>>> terra = LCDClient("https://terra-classic-lcd.publicnode.com", "columbus-5")
 >>> wallet = terra.wallet(mk)
 ```
 
 Once you have your Wallet, you can simply create a StdTx using `Wallet.create_and_sign_tx`.
 
 ```
 >>> from terra_classic_sdk.core.fee import Fee
```

#### html2text {}

```diff
@@ -1,43 +1,42 @@
-Metadata-Version: 2.1 Name: terra-classic-sdk Version: 2.0.7 Summary: The
+Metadata-Version: 2.1 Name: terra-classic-sdk Version: 2.0.8 Summary: The
 Python SDK for Terra Classic Home-page: https://github.com/geoffmunn/terra.py
 License: MIT Keywords: jigu,blockchain,terra,terra classic,lunc,defi,crypto
 Author: Geoff Munn Author-email: geoff@zimoobo.com Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0)
-Requires-Dist: bech32 (>=1.2.0,<2.0.0) Requires-Dist: betterproto (==2.0.0b4)
-Requires-Dist: bip32utils (>=0.3.post4,<0.4) Requires-Dist: boltons
-(>=21.0.0,<22.0.0) Requires-Dist: ecdsa (>=0.17.0,<0.18.0) Requires-Dist: furl
-(>=2.1.3,<3.0.0) Requires-Dist: mnemonic (>=0.19,<0.20) Requires-Dist: nest-
-asyncio (>=1.5.4,<2.0.0) Requires-Dist: protobuf (>=3.19.1,<4.0.0) Requires-
-Dist: terra-proto (>=1.0.1,<2.0.0) Requires-Dist: wrapt (>=1.13.3,<2.0.0)
-Project-URL: Documentation, https://terra-money.github.io/terra.py/index.html
-Project-URL: Repository, https://github.com/terra-money/terra.py Description-
-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
+(>=3.8.1,<4.0.0) Requires-Dist: attrs (>=20.3.0,<21.0.0) Requires-Dist: bech32
+(>=1.2.0,<2.0.0) Requires-Dist: betterproto (==2.0.0b4) Requires-Dist:
+bip32utils (>=0.3.post4,<0.4) Requires-Dist: boltons (>=21.0.0,<22.0.0)
+Requires-Dist: ecdsa (>=0.16.1,<0.17.0) Requires-Dist: furl (>=2.1.3,<3.0.0)
+Requires-Dist: mnemonic (>=0.19,<0.20) Requires-Dist: nest-asyncio
+(>=1.5.4,<2.0.0) Requires-Dist: protobuf (>=3.19.1,<4.0.0) Requires-Dist:
+terra-proto (>=3.0.1,<4.0.0) Requires-Dist: wrapt (>=1.13.3,<2.0.0) Project-
+URL: Documentation, https://terra-money.github.io/terra.py/index.html Project-
+URL: Repository, https://github.com/terra-money/terra.py Description-Content-
+Type: text/markdown
 
                                  [py-sdk-logo]
-                           The Python SDK for Terra
+                       The Python SDK for Terra Classic
                (Unfamiliar with Terra? Check_out_the_Terra_Docs)
                             [GitHub] [Python] [pip]
                              Explore_the_Docs_Â»
                        PyPI_Package Â· GitHub_Repository
-The Terra Software Development Kit (SDK) in Python is a simple library toolkit
-for building software that can interact with the Terra blockchain and provides
-simple abstractions over core data structures, serialization, key management,
-and API request generation. ## Features - Written in Python with extensive
-support libraries - Versatile support for key management solutions - Exposes
-the Terra API through LCDClient
+The Terra Classic Software Development Kit (SDK) in Python is a simple library
+toolkit for building software that can interact with the Terra Classic
+blockchain and provides simple abstractions over core data structures,
+serialization, key management, and API request generation. ## Features -
+Written in Python with extensive support libraries - Versatile support for key
+management solutions - Exposes the Terra Classic API through LCDClient -
+Supports non-Terra Classic addresses for transactions - IBC swaps between non-
+Terra Classic chains are partially supported (where IBC channels exist)
 # Table of Contents - [API Reference](#api-reference) - [Getting Started]
 (#getting-started) - [Requirements](#requirements) - [Installation]
 (#installation) - [Dependencies](#dependencies) - [Tests](#tests) - [Code
 Quality](#code-quality) - [Usage Examples](#usage-examples) - [Getting
 Blockchain Information](#getting-blockchain-information) - [Async Usage]
 (#async-usage) - [Building and Signing Transactions](#building-and-signing-
 transactions) - [Example Using a Wallet](#example-using-a-wallet-recommended) -
@@ -45,76 +44,82 @@
 [Requesting a Feature](#requesting-a-feature) - [Contributing Code]
 (#contributing-code) - [Documentation Contributions](#documentation-
 contributions) - [License](#license)
 # API Reference An intricate reference to the APIs on the Terra SDK can be
 found here.
 # Getting Started A walk-through of the steps to get started with the Terra SDK
 alongside a few use case examples are provided below. Alternatively, a tutorial
-video is also available here as reference. ## Requirements Terra SDK requires
-Python_v3.7+. ## Installation **NOTE:** _All code starting with a `$` is meant
-to run on your terminal (a bash prompt). All code starting with a `>>>` is
-meant to run in a python interpreter, like ipython._ Terra SDK can be installed
-(preferably in a `virtual environment` from PyPI using `pip`) as follows: ``` $
-pip install -U terra_classic_sdk ``` _You might have `pip3` installed instead
-of `pip`; proceed according to your own setup._## Dependencies Terra SDK uses
-Poetry to manage dependencies. To get set up with all the required
-dependencies, run: ``` $ pip install poetry $ poetry install ``` ## Tests Terra
-SDK provides extensive tests for data classes and functions. To run them, after
-the steps in [Dependencies](#dependencies): ``` $ make test ``` ## Code Quality
-Terra SDK uses Black, isort, and Mypy for checking code quality and maintaining
-style. To reformat, after the steps in [Dependencies](#dependencies): ``` $
-make qa && make format ```
-# Usage Examples Terra SDK can help you read block data, sign and send
+video is also available here as reference. ## Requirements Terra Classic SDK
+requires Python_v3.7+. ## Installation **NOTE:** _All code starting with a `$`
+is meant to run on your terminal (a bash prompt). All code starting with a
+`>>>` is meant to run in a python interpreter, like ipython._ Terra SDK can be
+installed (preferably in a `virtual environment` from PyPI using `pip`) as
+follows: ``` $ pip install -U terra_classic_sdk ``` _You might need to run pip
+via ```python -m pip install -U terra_classic_sdk```. Additionally, you might
+have `pip3` installed instead of `pip`; proceed according to your own setup._##
+Dependencies Terra Classic SDK uses Poetry to manage dependencies. To get set
+up with all the required dependencies, run: ``` $ pip install poetry $ poetry
+install ``` ## Tests Terra Classic SDK provides extensive tests for data
+classes and functions. To run them, after the steps in [Dependencies]
+(#dependencies): ``` $ make test ``` ## Code Quality Terra Classic SDK uses
+Black, isort, and Mypy for checking code quality and maintaining style. To
+reformat, after the steps in [Dependencies](#dependencies): ``` $ make qa &&
+make format ```
+# Usage Examples Terra Classic SDK can help you read block data, sign and send
 transactions, deploy and interact with contracts, and many more. The following
 examples are provided to help you get started. Use cases and functionalities of
-the Terra SDK are not limited to the following examples and can be found in
-full here. In order to interact with the Terra blockchain, you'll need a
-connection to a Terra node. This can be done through setting up an LCDClient
-(The LCDClient is an object representing an HTTP connection to a Terra LCD
-node.): ``` >>> from terra_classic_sdk.client.lcd import LCDClient >>> terra =
-LCDClient(chain_id="columbus-5", url="https://lcd.terra.dev") ``` ## Getting
-Blockchain Information Once properly configured, the `LCDClient` instance will
-allow you to interact with the Terra blockchain. Try getting the latest block
-height: ``` >>> terra.tendermint.block_info()['block']['header']['height'] ```
-`'1687543'` ### Async Usage If you want to make asynchronous, non-blocking LCD
-requests, you can use AsyncLCDClient. The interface is similar to LCDClient,
-except the module and wallet API functions must be awaited.
+the Terra Classic SDK are not limited to the following examples and can be
+found in full here. In order to interact with the Terra Classic blockchain,
+you'll need a connection to a Terra Classic node. This can be done through
+setting up an LCDClient (The LCDClient is an object representing an HTTP
+connection to a Terra Classic LCD node.): ``` >>> from
+terra_classic_sdk.client.lcd import LCDClient >>> terra = LCDClient
+(chain_id="columbus-5", url="https://terra-classic-lcd.publicnode.com") ``` ##
+Getting Blockchain Information Once properly configured, the `LCDClient`
+instance will allow you to interact with the Terra Classic blockchain. Try
+getting the latest block height: ``` >>> terra.tendermint.block_info()['block']
+['header']['height'] ``` `'1687543'` ### Async Usage If you want to make
+asynchronous, non-blocking LCD requests, you can use AsyncLCDClient. The
+interface is similar to LCDClient, except the module and wallet API functions
+must be awaited.
 
 >>> import asyncio
 >>> from terra_classic_sdk.client.lcd import AsyncLCDClient
 
 >>> async def main():
-      terra = AsyncLCDClient("https://lcd.terra.dev", "columbus-5")
+      terra = AsyncLCDClient("https://terra-classic-lcd.publicnode.com",
+"columbus-5")
       total_supply = await terra.bank.total()
       print(total_supply)
       await terra.session.close # you must close the session
 
 >>> asyncio.get_event_loop().run_until_complete(main())
 ## Building and Signing Transactions If you wish to perform a state-changing
-operation on the Terra blockchain such as sending tokens, swapping assets,
-withdrawing rewards, or even invoking functions on smart contracts, you must
-create a **transaction** and broadcast it to the network. Terra SDK provides
-functions that help create StdTx objects. ### Example Using a Wallet
-(_recommended_) A `Wallet` allows you to create and sign a transaction in a
-single step by automatically fetching the latest information from the
+operation on the Terra Classic blockchain such as sending tokens, swapping
+assets, withdrawing rewards, or even invoking functions on smart contracts, you
+must create a **transaction** and broadcast it to the network. Terra Classic
+SDK provides functions that help create StdTx objects. ### Example Using a
+Wallet (_recommended_) A `Wallet` allows you to create and sign a transaction
+in a single step by automatically fetching the latest information from the
 blockchain (chain ID, account number, sequence). Use `LCDClient.wallet()` to
 create a Wallet from any Key instance. The Key provided should correspond to
 the account you intend to sign the transaction with. **NOTE:** *If you are
 using MacOS and got an exception 'bad key length' from MnemonicKey, please
 check your python implementation. if `python3 -c "import ssl; print
 (ssl.OPENSSL_VERSION)"` returns LibreSSL 2.8.3, you need to reinstall python
 via pyenv or homebrew.* ``` >>> from terra_classic_sdk.client.lcd import
 LCDClient >>> from terra_classic_sdk.key.mnemonic import MnemonicKey >>> mk =
-MnemonicKey(mnemonic=MNEMONIC) >>> terra = LCDClient("https://lcd.terra.dev",
-"columbus-5") >>> wallet = terra.wallet(mk) ``` Once you have your Wallet, you
-can simply create a StdTx using `Wallet.create_and_sign_tx`. ``` >>> from
-terra_classic_sdk.core.fee import Fee >>> from terra_classic_sdk.core.bank
-import MsgSend >>> from terra_classic_sdk.client.lcd.api.tx import
-CreateTxOptions >>> tx = wallet.create_and_sign_tx(CreateTxOptions( msgs=
-[MsgSend( wallet.key.acc_address, RECIPIENT, "1000000uluna" # send 1 luna )],
+MnemonicKey(mnemonic=MNEMONIC) >>> terra = LCDClient("https://terra-classic-
+lcd.publicnode.com", "columbus-5") >>> wallet = terra.wallet(mk) ``` Once you
+have your Wallet, you can simply create a StdTx using
+`Wallet.create_and_sign_tx`. ``` >>> from terra_classic_sdk.core.fee import Fee
+>>> from terra_classic_sdk.core.bank import MsgSend >>> from
+terra_classic_sdk.client.lcd.api.tx import CreateTxOptions >>> tx =
+wallet.create_and_sign_tx(CreateTxOptions( msgs=[MsgSend
+( wallet.key.acc_address, RECIPIENT, "1000000uluna" # send 1 luna )],
 memo="test transaction!", fee=Fee(200000, "120000uluna") )) ``` You should now
 be able to broadcast your transaction to the network. ``` >>> result =
 terra.tx.broadcast(tx) >>> print(result) ```
 # Contributing Community contribution, whether it's a new feature, correction,
 bug report, additional documentation, or any other feedback is always welcome.
 Please read through this section to ensure that your contribution is in the
 most suitable format for us to effectively process.
```

