# Comparing `tmp/i8-terminal-0.2.91.tar.gz` & `tmp/i8-terminal-0.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i8-terminal-0.2.91.tar", last modified: Sun Jun 25 17:46:51 2023, max compression
+gzip compressed data, was "i8-terminal-0.2.92.tar", last modified: Sat Jul  1 22:26:09 2023, max compression
```

## Comparing `i8-terminal-0.2.91.tar` & `i8-terminal-0.2.92.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/api/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/api/earnings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/app/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/app/plot_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/i8t_chart_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/i8t_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/company/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/company_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/company_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/compnay_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_recent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_upcoming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/financials/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/market/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/market/market_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_describe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_historical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/news/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/news/news_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/notebook/notebook_launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/price/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/price_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/price_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/price_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/screen/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_gainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_losers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/user/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/user_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/commands/watchlist/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/i8_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/service_result/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/column_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/columns_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/earning_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/service_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/services/earnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/i8_terminal/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/auto_complete_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/chart_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/fin_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/fin_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/fin_statement_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/i8_auto_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/i8_completer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/indicator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/market_indice_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/metric_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/metric_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/metric_view_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/output_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/period_type_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/price_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/screening_condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/screening_operator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/screening_value_field_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/sort_order_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/ticker_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/user_watchlist_tickers_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/user_watchlists_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/utils_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.046323 i8-terminal-0.2.92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-01 22:26:09.046323 i8-terminal-0.2.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.026323 i8-terminal-0.2.92/i8_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.026323 i8-terminal-0.2.92/i8_terminal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.026323 i8-terminal-0.2.92/i8_terminal/api/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/api/earnings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/app/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/app/plot_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/assets/i8t_chart_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/assets/i8t_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/assets/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/assets/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/commands/company/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/company/company_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/company/company_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/company/compnay_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/commands/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/earnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_upcoming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/commands/financials/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/financials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/financials/financials_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/financials/financials_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/financials/financials_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/financials/financials_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.030323 i8-terminal-0.2.92/i8_terminal/commands/market/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/market/market_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.034323 i8-terminal-0.2.92/i8_terminal/commands/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.034323 i8-terminal-0.2.92/i8_terminal/commands/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/news/news_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.034323 i8-terminal-0.2.92/i8_terminal/commands/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/notebook/notebook_launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.034323 i8-terminal-0.2.92/i8_terminal/commands/price/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/price/price_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/price/price_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/price/price_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.034323 i8-terminal-0.2.92/i8_terminal/commands/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/screen/screen_gainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/screen/screen_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/screen/screen_losers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/screen/screen_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.034323 i8-terminal-0.2.92/i8_terminal/commands/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/user/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/user/user_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/user/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.038323 i8-terminal-0.2.92/i8_terminal/commands/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.038323 i8-terminal-0.2.92/i8_terminal/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/i8_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.038323 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-01 22:26:08.000000 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-01 22:26:08.000000 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 22:26:08.000000 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 22:26:08.000000 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-01 22:26:08.000000 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 22:26:08.000000 i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.042323 i8-terminal-0.2.92/i8_terminal/service_result/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/service_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/service_result/column_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/service_result/columns_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/service_result/earning_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/service_result/service_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.042323 i8-terminal-0.2.92/i8_terminal/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/services/earnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:26:09.046323 i8-terminal-0.2.92/i8_terminal/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/auto_complete_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/chart_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/fin_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/fin_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/fin_statement_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/i8_auto_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/i8_completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/indicator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/market_indice_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/metric_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/metric_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/metric_view_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/output_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/period_type_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/price_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/screening_condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/screening_operator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/screening_value_field_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/sort_order_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/ticker_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/user_watchlist_tickers_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/types/user_watchlists_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/utils_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/i8_terminal/version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 22:26:09.046323 i8-terminal-0.2.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-01 22:24:51.000000 i8-terminal-0.2.92/setup.py
```

### Comparing `i8-terminal-0.2.91/LICENSE` & `i8-terminal-0.2.92/LICENSE`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/PKG-INFO` & `i8-terminal-0.2.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.91
+Version: 0.2.92
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.91/README.md` & `i8-terminal-0.2.92/README.md`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/app/layout.py` & `i8-terminal-0.2.92/i8_terminal/app/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/app/plot_server.py` & `i8-terminal-0.2.92/i8_terminal/app/plot_server.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/assets/favicon.ico` & `i8-terminal-0.2.92/i8_terminal/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/assets/i8t_chart_logo.png` & `i8-terminal-0.2.92/i8_terminal/assets/i8t_chart_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/assets/i8t_logo.png` & `i8-terminal-0.2.92/i8_terminal/assets/i8t_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/assets/loading.gif` & `i8-terminal-0.2.92/i8_terminal/assets/loading.gif`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/assets/styles.css` & `i8-terminal-0.2.92/i8_terminal/assets/styles.css`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/company/company_compare.py` & `i8-terminal-0.2.92/i8_terminal/commands/company/company_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/company/company_search.py` & `i8-terminal-0.2.92/i8_terminal/commands/company/company_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/company/compnay_details.py` & `i8-terminal-0.2.92/i8_terminal/commands/company/compnay_details.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_list.py` & `i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_plot.py` & `i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_recent.py` & `i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_recent.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_upcoming.py` & `i8-terminal-0.2.92/i8_terminal/commands/earnings/earnings_upcoming.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_compare.py` & `i8-terminal-0.2.92/i8_terminal/commands/financials/financials_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_coverage.py` & `i8-terminal-0.2.92/i8_terminal/commands/financials/financials_coverage.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_list.py` & `i8-terminal-0.2.92/i8_terminal/commands/financials/financials_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_plot.py` & `i8-terminal-0.2.92/i8_terminal/commands/financials/financials_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/market/market_summary.py` & `i8-terminal-0.2.92/i8_terminal/commands/market/market_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_current.py` & `i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_current.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_describe.py` & `i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_describe.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_historical.py` & `i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_historical.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_search.py` & `i8-terminal-0.2.92/i8_terminal/commands/metrics/metrics_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/news/news_list.py` & `i8-terminal-0.2.92/i8_terminal/commands/news/news_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/notebook/notebook_launch.py` & `i8-terminal-0.2.92/i8_terminal/commands/notebook/notebook_launch.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/price/price_compare.py` & `i8-terminal-0.2.92/i8_terminal/commands/price/price_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/price/price_list.py` & `i8-terminal-0.2.92/i8_terminal/commands/price/price_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/price/price_plot.py` & `i8-terminal-0.2.92/i8_terminal/commands/price/price_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/screen/screen_gainers.py` & `i8-terminal-0.2.92/i8_terminal/commands/screen/screen_gainers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/screen/screen_losers.py` & `i8-terminal-0.2.92/i8_terminal/commands/screen/screen_losers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/screen/screen_search.py` & `i8-terminal-0.2.92/i8_terminal/commands/screen/screen_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/user/user_login.py` & `i8-terminal-0.2.92/i8_terminal/commands/user/user_login.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/user/webserver.py` & `i8-terminal-0.2.92/i8_terminal/commands/user/webserver.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_add.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_add.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_create.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_create.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_export.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_export.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_financials.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_list.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_metrics.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_metrics.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_rm.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_rm.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_summary.py` & `i8-terminal-0.2.92/i8_terminal/commands/watchlist/watchlist_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/cli.py` & `i8-terminal-0.2.92/i8_terminal/common/cli.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/financials.py` & `i8-terminal-0.2.92/i8_terminal/common/financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/formatting.py` & `i8-terminal-0.2.92/i8_terminal/common/formatting.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/layout.py` & `i8-terminal-0.2.92/i8_terminal/common/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/metrics.py` & `i8-terminal-0.2.92/i8_terminal/common/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
+from ast import literal_eval
 from typing import Dict, List, Optional
 
 import arrow
 import investor8_sdk
 import numpy as np
 import pandas as pd
 from investor8_sdk import MetricsApi
 from pandas import DataFrame, read_csv
 
 from i8_terminal.common.layout import format_metrics_df
+from i8_terminal.common.stock_info import get_stocks_df
 from i8_terminal.common.utils import is_cached_file_expired, reverse_period, similarity
 from i8_terminal.config import APP_SETTINGS, SETTINGS_FOLDER
 
 
 def get_indicators_list(indicator: Optional[str] = None) -> List[str]:
     indicators_dict = {
         "Momentum": ["ma5", "ma12", "ma26", "ma52", "ema5", "ema12", "ema26", "ema52"],
@@ -114,16 +116,25 @@
         "3Y": arrow.now().shift(years=-3).datetime.strftime("%Y-%m-%d"),
         "5Y": arrow.now().shift(years=-5).datetime.strftime("%Y-%m-%d"),
     }
     return period_start_date[period]
 
 
 def get_current_metrics_df(tickers: str, metricsList: str) -> Optional[pd.DataFrame]:
+    stocks_peers = get_stocks_df()[["ticker", "peers"]].set_index("ticker").to_dict()["peers"]
+    tickers_list = []
+    for tk in tickers.split(","):
+        if "PEERS" in tk and stocks_peers.get(tk.split(".")[0]):
+            ticker_name = tk.split(".")[0]
+            tickers_list.append(ticker_name)
+            tickers_list.extend(literal_eval(stocks_peers.get(ticker_name)))
+        else:
+            tickers_list.append(tk)
     metrics = investor8_sdk.MetricsApi().get_current_metrics(
-        symbols=tickers,
+        symbols=",".join(tickers_list),
         metrics=metricsList,
     )
     if metrics.data is None:
         return None
     metrics_data_df = pd.DataFrame([m.to_dict() for m in metrics.data])
     metrics_data_df.rename(columns={"metric": "metric_name", "symbol": "Ticker"}, inplace=True)
     metrics_metadata_df = pd.DataFrame([m.to_dict() for m in metrics.metadata])
```

### Comparing `i8-terminal-0.2.91/i8_terminal/common/price.py` & `i8-terminal-0.2.92/i8_terminal/common/price.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/screen.py` & `i8-terminal-0.2.92/i8_terminal/common/screen.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/common/stock_info.py` & `i8-terminal-0.2.92/i8_terminal/common/stock_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,90 @@
 import os
 from typing import List, Optional, Tuple
 
 import click
 import investor8_sdk
+import numpy as np
 import pandas as pd
 
 from i8_terminal.common.utils import is_cached_file_expired
 from i8_terminal.config import SETTINGS_FOLDER
 
 
-def sort_stocks(df: pd.DataFrame) -> pd.DataFrame:
+def sort_stocks(df: pd.DataFrame, include_peers: bool = False) -> pd.DataFrame:
     df["default_rank"] = 11
-    default_rank = {
-        "A": 1,
-        "AAL": 2,
-        "AAP": 3,
-        "AAPL": 4,
-        "AABV": 5,
-        "ABC": 6,
-        "ABMD": 7,
-        "ABT": 8,
-        "ACN": 9,
-        "ADBE": 10,
-    }
+    default_rank = (
+        {
+            "A": 1,
+            "AAL": 2,
+            "AAP": 3,
+            "AAPL": 4,
+            "AABV": 5,
+            "ABC": 6,
+            "ABMD": 7,
+            "ABT": 8,
+            "ACN": 9,
+            "ADBE": 10,
+        }
+        if not include_peers
+        else {
+            "A": 1,
+            "A.peers": 2,
+            "AAL": 3,
+            "AAL.peers": 4,
+            "AAP": 5,
+            "AAP.peers": 6,
+            "AAPL": 7,
+            "AAPL.peers": 8,
+            "AABV": 9,
+            "AABV.peers": 10,
+        }
+    )
     df["default_rank"] = df["ticker"].apply(lambda x: default_rank.get(x, 11))
     df = df.sort_values("default_rank").reset_index(drop=True)
-    return df[["ticker", "name"]]
+    return df[["ticker", "name", "peers"]]
 
 
 def get_stocks_df() -> pd.DataFrame:
     companies_path = f"{SETTINGS_FOLDER}/companies.csv"
     if os.path.exists(companies_path) and not is_cached_file_expired(companies_path):
         stocks_df = pd.read_csv(companies_path, keep_default_na=False)
     else:
         results = investor8_sdk.StockInfoApi().get_all_active_companies()
-        stocks_df = pd.DataFrame([d.to_dict() for d in results])[["ticker", "name"]]
+        stocks_df = pd.DataFrame([d.to_dict() for d in results])[["ticker", "name", "peers"]]
         stocks_df = sort_stocks(stocks_df)
         stocks_df.to_csv(companies_path, index=False)
     return stocks_df
 
 
-def get_stocks() -> List[Tuple[str, str]]:
-    df = get_stocks_df()
-    return list(df.to_records(index=False))
+def get_stocks(include_peers: bool) -> List[Tuple[str, str]]:
+    columns_list = ["ticker", "name"]
+    df = get_stocks_df().replace("", np.nan)
+    if include_peers:
+        df_peers = df[~df["peers"].isna()].copy()
+        df_peers.loc[:, "ticker"] = df_peers["ticker"].apply(lambda x: x + ".PEERS")
+        df = sort_stocks(pd.concat([df, df_peers]), include_peers)
+    return list(df[columns_list].to_records(index=False))
 
 
 def validate_ticker(ctx: click.Context, param: str, value: str) -> Optional[str]:
     if not ctx.resilient_parsing:
         if value and len(value.replace(" ", "").split(",")) > 1:
             click.echo(click.style(f"`{value}` is not a valid ticker name.", fg="yellow"))
             ctx.exit()
         if value and value.replace(" ", "").upper() not in set(get_stocks_df()["ticker"]):
             click.echo(click.style(f"`{value}` is not a valid ticker name.", fg="yellow"))
             ctx.exit()
     return value
 
 
 def validate_tickers(ctx: click.Context, param: str, value: str) -> Optional[str]:
+    tickers = {d[0] for d in get_stocks(True)}
     if not ctx.resilient_parsing:
-        invalid_tickers = (
-            [*set(value.replace(" ", "").upper().split(",")) - set(get_stocks_df()["ticker"])] if value else []
-        )
+        invalid_tickers = [*set(value.replace(" ", "").upper().split(",")) - tickers] if value else []
         if value and invalid_tickers:
             msg = "are not valid ticker names." if len(invalid_tickers) > 1 else "is not a valid ticker name."
             click.echo(
                 click.style(
                     f"`{', '.join(invalid_tickers)}` {msg}",
                     fg="yellow",
                 )
```

### Comparing `i8-terminal-0.2.91/i8_terminal/common/utils.py` & `i8-terminal-0.2.92/i8_terminal/common/utils.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/config.py` & `i8-terminal-0.2.92/i8_terminal/config.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/config.yml` & `i8-terminal-0.2.92/i8_terminal/config.yml`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/PKG-INFO` & `i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.91
+Version: 0.2.92
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/SOURCES.txt` & `i8-terminal-0.2.92/i8_terminal/i8_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/main.py` & `i8-terminal-0.2.92/i8_terminal/main.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/service_result/column_info.py` & `i8-terminal-0.2.92/i8_terminal/service_result/column_info.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/service_result/columns_context.py` & `i8-terminal-0.2.92/i8_terminal/service_result/columns_context.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/service_result/earning_list_result.py` & `i8-terminal-0.2.92/i8_terminal/service_result/earning_list_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/service_result/service_result.py` & `i8-terminal-0.2.92/i8_terminal/service_result/service_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         style = get_table_style(style_profile)
         table = Table(**style)
         df = self._wide_df(format)
         ci_list = self._cols_context.get_col_infos()
         non_num_dts = ["str", "string", "datetime"]
 
         for ci in ci_list:
-            table.add_column(ci.display_name, justify="left" if ci.data_type in non_num_dts else "right")
+            table.add_column(
+                ci.display_name, justify="left" if ci.data_type in non_num_dts else "right"
+            )  # type: ignore
 
         def _process_value(raw: Union[int, float], formatted: str, ci: ColumnInfo) -> str:
             if raw is np.nan or raw is None:
                 return "-"
             value = raw if format == "raw" else formatted
             if ci.colorable and ci.data_type not in non_num_dts and raw != 0:
                 color = "green" if raw > 0 else "red"
```

### Comparing `i8-terminal-0.2.91/i8_terminal/services/earnings.py` & `i8-terminal-0.2.92/i8_terminal/services/earnings.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/auto_complete_choice.py` & `i8-terminal-0.2.92/i8_terminal/types/auto_complete_choice.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/chart_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/chart_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/command_parser.py` & `i8-terminal-0.2.92/i8_terminal/types/command_parser.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/condition_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/fin_identifier_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/fin_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/fin_period_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/fin_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/fin_statement_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/fin_statement_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/i8_auto_suggest.py` & `i8-terminal-0.2.92/i8_terminal/types/i8_auto_suggest.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/i8_completer.py` & `i8-terminal-0.2.92/i8_terminal/types/i8_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,22 @@
                     incomplete = parts[-1] if len(parts) > 0 else " "
                     for (ticker, name) in matched_param.type.get_suggestions(  # type: ignore
                         incomplete if incomplete else " ", True
                     ):
                         choices.append(Completion(text_type(ticker), -len(incomplete), display_meta=name))
                 elif type(matched_param.type) in [TickerParamType, UserWatchlistTickersParamType]:
                     filter_choices = False
+                    include_peers = matched_param.name != "ticker"
                     if matched_param.name == "ticker":
                         incomplete = ctx.incomplete
                     else:
                         parts = ctx.incomplete.split(",")
                         incomplete = parts[-1] if len(parts) > 0 else " "
                     for (ticker, name) in matched_param.type.get_suggestions(  # type: ignore
-                        incomplete if incomplete else " ", True
+                        incomplete if incomplete else " ", True, include_peers
                     ):
                         choices.append(Completion(text_type(ticker.upper()), -len(incomplete), display_meta=name))
                 elif type(matched_param.type) in [MetricParamType, IndicatorParamType]:
                     filter_choices = False
                     parts = ctx.incomplete.split(",")
                     incomplete = parts[-1] if len(parts) > 0 else " "
                     for (metric, name) in matched_param.type.get_suggestions(  # type: ignore
```

### Comparing `i8-terminal-0.2.91/i8_terminal/types/indicator_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/indicator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/market_indice_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/market_indice_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/metric_identifier_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/metric_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/metric_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/metric_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/metric_view_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/metric_view_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/output_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/output_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/period_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/period_type_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/period_type_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/price_period_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/price_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/screening_condition_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/screening_condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/screening_operator_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/screening_operator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/screening_value_field_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/screening_value_field_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/sort_order_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/sort_order_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/types/ticker_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/ticker_param_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from i8_terminal.common.stock_info import get_stocks
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
 
 
 class TickerParamType(AutoCompleteChoice):
     name = "ticker"
 
-    def get_suggestions(self, keyword: str, pre_populate: bool = False) -> List[Tuple[str, str]]:
+    def get_suggestions(
+        self, keyword: str, pre_populate: bool = False, include_peers: bool = False
+    ) -> List[Tuple[str, str]]:
         if not self.is_loaded:
-            self.set_choices(get_stocks())
+            self.set_choices(get_stocks(include_peers))
 
         if pre_populate and keyword.strip() == "":
             return self._choices[: self.size]
 
         return self.search_keyword(keyword)
 
     def __repr__(self) -> str:
```

### Comparing `i8-terminal-0.2.91/i8_terminal/types/user_watchlist_tickers_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/user_watchlist_tickers_param_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from i8_terminal.config import USER_SETTINGS
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
 
 
 def get_user_watchlist_tickers() -> List[Tuple[str, str]]:
     results = investor8_sdk.UserApi().get_watchlists_by_user(user_id=USER_SETTINGS.get("user_id"))
     tickers = set(ticker for wl in results.watchlists for ticker in wl.tickers)
-    stocks = get_stocks()
+    stocks = get_stocks(True)
     return [(tk, name) for (tk, name) in stocks if tk in tickers]
 
 
 class UserWatchlistTickersParamType(AutoCompleteChoice):
     name = "userwatchlisttickers"
 
     def get_suggestions(self, keyword: str, pre_populate: bool = False) -> List[Tuple[str, str]]:
```

### Comparing `i8-terminal-0.2.91/i8_terminal/types/user_watchlists_param_type.py` & `i8-terminal-0.2.92/i8_terminal/types/user_watchlists_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/i8_terminal/utils_setup.py` & `i8-terminal-0.2.92/i8_terminal/utils_setup.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.91/setup.py` & `i8-terminal-0.2.92/setup.py`

 * *Files identical despite different names*

