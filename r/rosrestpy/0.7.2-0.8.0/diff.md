# Comparing `tmp/rosrestpy-0.7.2.tar.gz` & `tmp/rosrestpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosrestpy-0.7.2.tar", max compression
+gzip compressed data, was "rosrestpy-0.8.0.tar", max compression
```

## Comparing `rosrestpy-0.7.2.tar` & `rosrestpy-0.8.0.tar`

### file list

```diff
@@ -1,85 +1,98 @@
--rw-r--r--   0        0        0    35149 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/LICENSE
--rw-r--r--   0        0        0     2269 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/README.md
--rw-r--r--   0        0        0     1222 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      553 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/__init__.py
--rw-r--r--   0        0        0     2675 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/_base.py
--rw-r--r--   0        0        0     4631 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/_literals.py
--rw-r--r--   0        0        0     1296 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/_utils.py
--rw-r--r--   0        0        0      301 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/error.py
--rw-r--r--   0        0        0     1617 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/inteface/__init__.py
--rw-r--r--   0        0        0     1002 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/__init__.py
--rw-r--r--   0        0        0      686 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/bridge.py
--rw-r--r--   0        0        0      262 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/msti.py
--rw-r--r--   0        0        0      763 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/port.py
--rw-r--r--   0        0        0      322 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/vlan.py
--rw-r--r--   0        0        0     1931 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/ethernet.py
--rw-r--r--   0        0        0      754 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/interface.py
--rw-r--r--   0        0        0      572 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/list/__init__.py
--rw-r--r--   0        0        0      244 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/list/list.py
--rw-r--r--   0        0        0      246 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/list/member.py
--rw-r--r--   0        0        0     2477 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/__init__.py
--rw-r--r--   0        0        0      392 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/address.py
--rw-r--r--   0        0        0      544 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/arp.py
--rw-r--r--   0        0        0      278 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/cloud.py
--rw-r--r--   0        0        0     1285 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_client.py
--rw-r--r--   0        0        0      470 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_relay.py
--rw-r--r--   0        0        0      771 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/__init__.py
--rw-r--r--   0        0        0      153 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/_literals.py
--rw-r--r--   0        0        0     1100 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/dhcp_server.py
--rw-r--r--   0        0        0     1050 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/lease.py
--rw-r--r--   0        0        0      423 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/network.py
--rw-r--r--   0        0        0     1032 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/__init__.py
--rw-r--r--   0        0        0      126 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/_literals.py
--rw-r--r--   0        0        0      195 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/cache.py
--rw-r--r--   0        0        0      626 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/static.py
--rw-r--r--   0        0        0     1472 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/__init__.py
--rw-r--r--   0        0        0      282 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/_literals.py
--rw-r--r--   0        0        0      748 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/connection.py
--rw-r--r--   0        0        0     2703 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/filter.py
--rw-r--r--   0        0        0     2978 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/mangle.py
--rw-r--r--   0        0        0     2381 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/nat.py
--rw-r--r--   0        0        0     1042 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/route.py
--rw-r--r--   0        0        0      565 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/setting.py
--rw-r--r--   0        0        0      181 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/log.py
--rw-r--r--   0        0        0      744 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/__init__.py
--rw-r--r--   0        0        0      220 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/_literals.py
--rw-r--r--   0        0        0      160 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/aaa.py
--rw-r--r--   0        0        0     1147 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/profile.py
--rw-r--r--   0        0        0      640 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/secret.py
--rw-r--r--   0        0        0      826 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/__init__.py
--rw-r--r--   0        0        0      153 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/interface.py
--rw-r--r--   0        0        0     2076 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/simple.py
--rw-r--r--   0        0        0      726 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/tree.py
--rw-r--r--   0        0        0     7146 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ros.py
--rw-r--r--   0        0        0      604 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/routing/__init__.py
--rw-r--r--   0        0        0      467 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/routing/rule.py
--rw-r--r--   0        0        0      334 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/routing/table.py
--rw-r--r--   0        0        0     2407 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/__init__.py
--rw-r--r--   0        0        0      123 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/health.py
--rw-r--r--   0        0        0      214 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/history.py
--rw-r--r--   0        0        0      126 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/identity.py
--rw-r--r--   0        0        0      122 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/license.py
--rw-r--r--   0        0        0      248 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/logging.py
--rw-r--r--   0        0        0      146 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/note.py
--rw-r--r--   0        0        0      580 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/__init__.py
--rw-r--r--   0        0        0      101 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/_literals.py
--rw-r--r--   0        0        0      297 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/package.py
--rw-r--r--   0        0        0      774 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/update.py
--rw-r--r--   0        0        0      460 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/resource.py
--rw-r--r--   0        0        0      232 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/routerboard.py
--rw-r--r--   0        0        0     6722 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/__init__.py
--rw-r--r--   0        0        0      223 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/bandwith_server.py
--rw-r--r--   0        0        0      546 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/bandwith_test.py
--rw-r--r--   0        0        0      158 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/ip_scan.py
--rw-r--r--   0        0        0     1042 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/netwatch.py
--rw-r--r--   0        0        0      236 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/ping.py
--rw-r--r--   0        0        0      416 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/torch.py
--rw-r--r--   0        0        0      290 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/traceroute.py
--rw-r--r--   0        0        0     1746 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/__init__.py
--rw-r--r--   0        0        0      168 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/aaa.py
--rw-r--r--   0        0        0      167 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/active.py
--rw-r--r--   0        0        0      188 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/group.py
--rw-r--r--   0        0        0      129 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/settings.py
--rw-r--r--   0        0        0      205 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/ssh_keys.py
--rw-r--r--   0        0        0      249 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/user.py
--rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 rosrestpy-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2543 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/README.md
+-rw-r--r--   0        0        0     1222 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/__init__.py
+-rw-r--r--   0        0        0     2659 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/_base.py
+-rw-r--r--   0        0        0     4631 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/_literals.py
+-rw-r--r--   0        0        0     1246 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/_utils.py
+-rw-r--r--   0        0        0      301 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/error.py
+-rw-r--r--   0        0        0     1851 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/bridge.py
+-rw-r--r--   0        0        0      262 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/msti.py
+-rw-r--r--   0        0        0      763 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/port.py
+-rw-r--r--   0        0        0      322 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/vlan.py
+-rw-r--r--   0        0        0     1008 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/eoip.py
+-rw-r--r--   0        0        0     1980 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/ethernet.py
+-rw-r--r--   0        0        0      754 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/interface.py
+-rw-r--r--   0        0        0      572 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/list/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/list/list.py
+-rw-r--r--   0        0        0      246 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/list/member.py
+-rw-r--r--   0        0        0     2758 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/__init__.py
+-rw-r--r--   0        0        0      392 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/address.py
+-rw-r--r--   0        0        0      544 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/arp.py
+-rw-r--r--   0        0        0      278 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/cloud.py
+-rw-r--r--   0        0        0     1285 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_client.py
+-rw-r--r--   0        0        0      470 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_relay.py
+-rw-r--r--   0        0        0      771 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/_literals.py
+-rw-r--r--   0        0        0     1100 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/dhcp_server.py
+-rw-r--r--   0        0        0     1050 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/lease.py
+-rw-r--r--   0        0        0      423 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/network.py
+-rw-r--r--   0        0        0     1032 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/_literals.py
+-rw-r--r--   0        0        0      195 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/cache.py
+-rw-r--r--   0        0        0      626 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/static.py
+-rw-r--r--   0        0        0     1472 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/_literals.py
+-rw-r--r--   0        0        0      748 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/connection.py
+-rw-r--r--   0        0        0     2703 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/filter.py
+-rw-r--r--   0        0        0     2978 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/mangle.py
+-rw-r--r--   0        0        0     2413 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/nat.py
+-rw-r--r--   0        0        0     3180 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/hotspot/__init__.py
+-rw-r--r--   0        0        0      454 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/active.py
+-rw-r--r--   0        0        0      214 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/cookie.py
+-rw-r--r--   0        0        0      625 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/host.py
+-rw-r--r--   0        0        0      529 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/hotspot.py
+-rw-r--r--   0        0        0      637 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/ip_binding.py
+-rw-r--r--   0        0        0     1325 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/profile.py
+-rw-r--r--   0        0        0      182 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/service_port.py
+-rw-r--r--   0        0        0     1236 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/user/__init__.py
+-rw-r--r--   0        0        0     1108 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/user/profile.py
+-rw-r--r--   0        0        0      998 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/walled_garden/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/walled_garden/ip.py
+-rw-r--r--   0        0        0     1042 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/route.py
+-rw-r--r--   0        0        0      565 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/setting.py
+-rw-r--r--   0        0        0      181 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/log.py
+-rw-r--r--   0        0        0      744 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/_literals.py
+-rw-r--r--   0        0        0      160 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/aaa.py
+-rw-r--r--   0        0        0     1147 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/profile.py
+-rw-r--r--   0        0        0      640 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/secret.py
+-rw-r--r--   0        0        0      826 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/interface.py
+-rw-r--r--   0        0        0     2076 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/simple.py
+-rw-r--r--   0        0        0      726 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/tree.py
+-rw-r--r--   0        0        0     7146 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ros.py
+-rw-r--r--   0        0        0      604 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/routing/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/routing/rule.py
+-rw-r--r--   0        0        0      334 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/routing/table.py
+-rw-r--r--   0        0        0     2407 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/__init__.py
+-rw-r--r--   0        0        0      123 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/health.py
+-rw-r--r--   0        0        0      214 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/history.py
+-rw-r--r--   0        0        0      126 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/identity.py
+-rw-r--r--   0        0        0      122 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/license.py
+-rw-r--r--   0        0        0      248 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/logging.py
+-rw-r--r--   0        0        0      146 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/note.py
+-rw-r--r--   0        0        0      580 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/__init__.py
+-rw-r--r--   0        0        0      101 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/_literals.py
+-rw-r--r--   0        0        0      297 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/package.py
+-rw-r--r--   0        0        0      774 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/update.py
+-rw-r--r--   0        0        0      460 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/resource.py
+-rw-r--r--   0        0        0      232 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/routerboard.py
+-rw-r--r--   0        0        0     6722 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/bandwith_server.py
+-rw-r--r--   0        0        0      546 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/bandwith_test.py
+-rw-r--r--   0        0        0      158 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/ip_scan.py
+-rw-r--r--   0        0        0     1042 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/netwatch.py
+-rw-r--r--   0        0        0      236 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/ping.py
+-rw-r--r--   0        0        0      416 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/torch.py
+-rw-r--r--   0        0        0      290 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/traceroute.py
+-rw-r--r--   0        0        0     1746 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/aaa.py
+-rw-r--r--   0        0        0      167 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/active.py
+-rw-r--r--   0        0        0      188 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/group.py
+-rw-r--r--   0        0        0      129 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/settings.py
+-rw-r--r--   0        0        0      205 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/ssh_keys.py
+-rw-r--r--   0        0        0      249 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/user.py
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 rosrestpy-0.8.0/PKG-INFO
```

### Comparing `rosrestpy-0.7.2/LICENSE` & `rosrestpy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/README.md` & `rosrestpy-0.8.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # RosRestPy
 
 [![PyPi Package Version](https://img.shields.io/pypi/v/rosrestpy)](https://pypi.org/project/rosrestpy/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/rosrestpy)](https://pypi.org/project/rosrestpy/)
 [![LICENSE](https://img.shields.io/github/license/hexatester/rosrestpy)](https://github.com/hexatester/rosrestpy/blob/main/LICENSE)
 
-RouterOS v7 REST API python module
+Mikrotik's RouterOS v7 REST API python module
 
 ## RouterOS v7 REST API Support
 
+[Check Here for API Support](https://github.com/hexatester/rosrestpy/blob/main/TODO.md).
+
 Not all types and methods of the RouterOS v7 REST API are supported, yet.
 Finding any bugs? Please [Create Issue](https://github.com/hexatester/rosrestpy/issues)
 
 ## Installing
 
 You can install or upgrade rosrestpy with:
 
@@ -44,14 +46,19 @@
 
 # Adding new /simple/queue
 from ros.queue import SimpleQueue
 new_queue = SimpleQueue(name="Test", target="192.168.88.0/24", max_limit="10M/10M", disabled=True)
 new_queue = ros.queue.simple.add(new_queue)
 print(new_queue)
 
+# Updating /simple/queue
+test_queue = ros.queue.simple(name="Test")[0]
+new_test_queue = ros.queue.simple.set(test_queue, {"comment": "Test comment"})
+print(new_test_queue)
+
 # Using /tool/bandwith-test
 bw_tests = ros.tool.bandwith_test("172.16.0.1", "3s", "admin", direction="both")
 result_bw_test = bw_tests[-1]
 print(f"Download {result_bw_test.rx_total_average}")
 print(f"Upload {result_bw_test.tx_total_average}")
 ```
```

### Comparing `rosrestpy-0.7.2/pyproject.toml` & `rosrestpy-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rosrestpy"
-version = "0.7.2"
+version = "0.8.0"
 description = "RouterOS v7 REST API python module"
 authors = ["hexatester <hexatester@protonmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/hexatester/rosrestpy"
 packages = [
     { include = "ros" },
```

### Comparing `rosrestpy-0.7.2/ros/__init__.py` & `rosrestpy-0.8.0/ros/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.2"
+__version__ = "0.8.0"
 from .inteface import InterfaceModule
 from .ip import IPModule
 from .ppp import PPPModule
 from .queue import QueueModule
 from .routing import RoutingModule
 from .system import SystemModule
 from .tool import ToolModule
```

### Comparing `rosrestpy-0.7.2/ros/_base.py` & `rosrestpy-0.8.0/ros/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def add(self, o: PR) -> PR:
         assert self._write and self._create, "Not writeable"
         data = unstructure(o)
         data = clean_before_put(data)
         return self.ros.put_as(self.filename, self.cl, data)
 
     def delete(self, o: PR):
-        assert self._write and self._delete, "Not writeable"
+        assert self._delete, "Not writeable"
         return self.remove(o)
 
     def _disabled(self, o: PR, s: bool) -> PR:
         assert self._write, "Not writeable"
         return self.ros.patch_as(
             self.filename + f"/{self._getid(o)}", self.cl, {"disabled": s}
         )
```

### Comparing `rosrestpy-0.7.2/ros/_literals.py` & `rosrestpy-0.8.0/ros/_literals.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/_utils.py` & `rosrestpy-0.8.0/ros/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,34 +21,26 @@
             if isinstance(val, dict):
                 data.append(clean_key(val))
             else:
                 data.append(val)
     return data
 
 
-def clean_filters(d: Dict[str, Any]) -> dict:
+def clean_filters(d: Dict[str, Any]) -> Dict[str, Any]:
     if not d:
         return d
-    nd = dict()
-    for k, v in d.items():
-        k = k.replace("_", "-")
-        nd[k] = v
-    return nd
+    translation_table = str.maketrans("_", "-")
+    return {k.translate(translation_table): v for k, v in d.items()}
 
 
 def clean_before_put(d: Dict[str, Any]) -> dict:
     if not d:
         return d
-    d.pop("id", None)
-    nd = dict()
-    for k, v in d.items():
-        if "_" in k:
-            k = k.replace("_", "-")
-        if v != None:
-            nd[k] = v
+    nd = {k.replace("_", "-"): v for k, v in d.items() if v is not None}
+    nd.pop("id", None)
     return nd
 
 
 def _union_str_int(v: str, t: Any) -> Union[str, int]:
     if v.isdigit():
         return int(v)
     return v
```

### Comparing `rosrestpy-0.7.2/ros/inteface/__init__.py` & `rosrestpy-0.8.0/ros/inteface/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import Any, List
 
 from ros._base import BaseModule, BaseProps
 
 from .bridge import BridgeModule, Bridge, BridgeMsti, BridgePort, BridgeVlan
+from .eoip import EoIP
 from .ethernet import InterfaceEthernet
 from .interface import Interface
 from .list import InterfaceList, InterfaceListMember, InterfaceListModule
 
 
 class InterfaceModule(BaseModule):
     _brigde: BridgeModule = None
+    _eoip: BaseProps[EoIP] = None
     _ethernet: BaseProps[InterfaceEthernet] = None
     _list: InterfaceListModule = None
 
     def __call__(self, **kwds: Any):
         return self.print(**kwds)
 
     @property
@@ -25,14 +27,20 @@
     @property
     def list(self) -> InterfaceListModule:
         if not self._list:
             self._list = InterfaceListModule(self.ros, "/interface/list", InterfaceList)
         return self._list
 
     @property
+    def eoip(self) -> BaseProps[EoIP]:
+        if not self._eoip:
+            self._eoip = BaseProps(self.ros, "/interface/eoip", EoIP)
+        return self._eoip
+
+    @property
     def ethernet(self) -> BaseProps[InterfaceEthernet]:
         if not self._ethernet:
             self._ethernet = BaseProps(
                 self.ros, "/interface/ethernet", InterfaceEthernet
             )
             self._ethernet._create = False
             self._ethernet._delete = False
```

### Comparing `rosrestpy-0.7.2/ros/inteface/bridge/__init__.py` & `rosrestpy-0.8.0/ros/inteface/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/inteface/bridge/bridge.py` & `rosrestpy-0.8.0/ros/inteface/bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/inteface/bridge/port.py` & `rosrestpy-0.8.0/ros/inteface/bridge/port.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/inteface/ethernet.py` & `rosrestpy-0.8.0/ros/inteface/ethernet.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     loop_protect_send_interval: str
     loop_protect_status: str
     mac_address: str
     mtu: int
     name: str
     orig_mac_address: str
     running: bool
-    rx_broadcast: int
     rx_bytes: int
     rx_fcs_error: int
     rx_flow_control: str
-    rx_fragment: int
-    rx_jabber: int
-    rx_multicast: int
     rx_pause: int
-    tx_broadcast: int
     tx_bytes: int
     tx_flow_control: str
-    tx_multicast: int
-    tx_pause: int
+    rx_broadcast: int = None
+    rx_fragment: int = None
+    rx_jabber: int = None
+    rx_multicast: int = None
+    tx_broadcast: int = None
+    tx_multicast: int = None
+    tx_pause: int = None
     advertise: str = None
     full_duplex: bool = None
     speed: str = None
     comment: str = None
     fec_mode: str = None
     rx_1024_1518: int = None
     rx_128_255: int = None
```

### Comparing `rosrestpy-0.7.2/ros/inteface/interface.py` & `rosrestpy-0.8.0/ros/inteface/interface.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/inteface/list/__init__.py` & `rosrestpy-0.8.0/ros/inteface/list/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/__init__.py` & `rosrestpy-0.8.0/ros/ip/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from .arp import ARP
 from .cloud import Cloud
 from .dhcp_client import DHCPClient
 from .dhcp_relay import DHCPRelay
 from .dhcp_server import DHCPServerModule, DHCPServer
 from .dns import DNS
 from .firewall import IPFirewallModule
+from .hotspot import HotspotModule, HotspotServer
 from .route import Route
 from .setting import Setting
 
 
 class IPModule(BaseModule):
     _dhcp_server: DHCPServerModule = None
     _firewall: IPFirewallModule = None
+    _hotspot: HotspotModule = None
 
     _address: BaseProps[Address] = None
     _arp: BaseProps[ARP] = None
     _dhcp_client: BaseProps[DHCPClient] = None
     _dhcp_relay: BaseProps[DHCPRelay] = None
     _route: BaseProps[Route] = None
 
@@ -67,14 +69,20 @@
     @property
     def firewall(self) -> IPFirewallModule:
         if not self._firewall:
             self._firewall = IPFirewallModule(self.ros, "/ip/firewall")
         return self._firewall
 
     @property
+    def hotspot(self) -> HotspotModule:
+        if not self._hotspot:
+            self._hotspot = HotspotModule(self.ros, "/ip/hotspot", HotspotServer)
+        return self._hotspot
+
+    @property
     def route(self) -> BaseProps[Route]:
         if not self._route:
             self._route = BaseProps(self.ros, "/ip/route", Route)
         return self._route
 
     @property
     def setting(self) -> Setting:
```

### Comparing `rosrestpy-0.7.2/ros/ip/arp.py` & `rosrestpy-0.8.0/ros/ip/arp.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/dhcp_client.py` & `rosrestpy-0.8.0/ros/ip/dhcp_client.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/dhcp_server/__init__.py` & `rosrestpy-0.8.0/ros/ip/dhcp_server/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/dhcp_server/dhcp_server.py` & `rosrestpy-0.8.0/ros/ip/dhcp_server/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/dhcp_server/lease.py` & `rosrestpy-0.8.0/ros/ip/dhcp_server/lease.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/dns/__init__.py` & `rosrestpy-0.8.0/ros/ip/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/dns/static.py` & `rosrestpy-0.8.0/ros/ip/dns/static.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/firewall/__init__.py` & `rosrestpy-0.8.0/ros/ip/firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/firewall/connection.py` & `rosrestpy-0.8.0/ros/ip/firewall/connection.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/firewall/filter.py` & `rosrestpy-0.8.0/ros/ip/firewall/filter.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/firewall/mangle.py` & `rosrestpy-0.8.0/ros/ip/firewall/mangle.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/firewall/nat.py` & `rosrestpy-0.8.0/ros/ip/firewall/nat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ._literals import IPv4Options
 
 Action = Literal[
     "accept",
     "add-dst-to-address-list",
     "add-src-to-address-list",
     "dst-nat",
+    "endpoint-independent-nat",
     "jump",
     "log",
     "masquerade",
     "netmap",
     "passthrough",
     "redirect",
     "return",
```

### Comparing `rosrestpy-0.7.2/ros/ip/route.py` & `rosrestpy-0.8.0/ros/ip/route.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ip/setting.py` & `rosrestpy-0.8.0/ros/ip/setting.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ppp/__init__.py` & `rosrestpy-0.8.0/ros/ppp/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ppp/profile.py` & `rosrestpy-0.8.0/ros/ppp/profile.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ppp/secret.py` & `rosrestpy-0.8.0/ros/ppp/secret.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/queue/__init__.py` & `rosrestpy-0.8.0/ros/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/queue/simple.py` & `rosrestpy-0.8.0/ros/queue/simple.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/queue/tree.py` & `rosrestpy-0.8.0/ros/queue/tree.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/ros.py` & `rosrestpy-0.8.0/ros/ros.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/routing/__init__.py` & `rosrestpy-0.8.0/ros/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/system/__init__.py` & `rosrestpy-0.8.0/ros/system/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/system/package/__init__.py` & `rosrestpy-0.8.0/ros/system/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/system/package/update.py` & `rosrestpy-0.8.0/ros/system/package/update.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/tool/__init__.py` & `rosrestpy-0.8.0/ros/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/tool/bandwith_test.py` & `rosrestpy-0.8.0/ros/tool/bandwith_test.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/tool/netwatch.py` & `rosrestpy-0.8.0/ros/tool/netwatch.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/ros/user/__init__.py` & `rosrestpy-0.8.0/ros/user/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.2/PKG-INFO` & `rosrestpy-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosrestpy
-Version: 0.7.2
+Version: 0.8.0
 Summary: RouterOS v7 REST API python module
 Home-page: https://github.com/hexatester/rosrestpy
 License: GPL-3.0-only
 Author: hexatester
 Author-email: hexatester@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -29,18 +29,20 @@
 
 # RosRestPy
 
 [![PyPi Package Version](https://img.shields.io/pypi/v/rosrestpy)](https://pypi.org/project/rosrestpy/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/rosrestpy)](https://pypi.org/project/rosrestpy/)
 [![LICENSE](https://img.shields.io/github/license/hexatester/rosrestpy)](https://github.com/hexatester/rosrestpy/blob/main/LICENSE)
 
-RouterOS v7 REST API python module
+Mikrotik's RouterOS v7 REST API python module
 
 ## RouterOS v7 REST API Support
 
+[Check Here for API Support](https://github.com/hexatester/rosrestpy/blob/main/TODO.md).
+
 Not all types and methods of the RouterOS v7 REST API are supported, yet.
 Finding any bugs? Please [Create Issue](https://github.com/hexatester/rosrestpy/issues)
 
 ## Installing
 
 You can install or upgrade rosrestpy with:
 
@@ -73,14 +75,19 @@
 
 # Adding new /simple/queue
 from ros.queue import SimpleQueue
 new_queue = SimpleQueue(name="Test", target="192.168.88.0/24", max_limit="10M/10M", disabled=True)
 new_queue = ros.queue.simple.add(new_queue)
 print(new_queue)
 
+# Updating /simple/queue
+test_queue = ros.queue.simple(name="Test")[0]
+new_test_queue = ros.queue.simple.set(test_queue, {"comment": "Test comment"})
+print(new_test_queue)
+
 # Using /tool/bandwith-test
 bw_tests = ros.tool.bandwith_test("172.16.0.1", "3s", "admin", direction="both")
 result_bw_test = bw_tests[-1]
 print(f"Download {result_bw_test.rx_total_average}")
 print(f"Upload {result_bw_test.tx_total_average}")
 ```
```

