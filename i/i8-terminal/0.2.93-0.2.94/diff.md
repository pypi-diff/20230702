# Comparing `tmp/i8-terminal-0.2.93.tar.gz` & `tmp/i8-terminal-0.2.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i8-terminal-0.2.93.tar", last modified: Sun Jul  2 20:42:41 2023, max compression
+gzip compressed data, was "i8-terminal-0.2.94.tar", last modified: Sun Jul  2 20:44:17 2023, max compression
```

## Comparing `i8-terminal-0.2.93.tar` & `i8-terminal-0.2.94.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.552555 i8-terminal-0.2.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-02 20:42:41.548555 i8-terminal-0.2.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/api/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/api/earnings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/app/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/app/plot_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/assets/i8t_chart_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/assets/i8t_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/assets/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/assets/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/commands/company/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/company/company_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/company/company_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/company/compnay_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/commands/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/earnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_recent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_upcoming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/commands/financials/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/financials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/financials/financials_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/financials/financials_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/financials/financials_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/financials/financials_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.540555 i8-terminal-0.2.93/i8_terminal/commands/market/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/market/market_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_describe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_historical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/news/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/news/news_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/notebook/notebook_launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/price/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/price/price_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/price/price_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/price/price_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/screen/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/screen/screen_gainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/screen/screen_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/screen/screen_losers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/screen/screen_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/user/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/user/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/user/user_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/user/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/commands/watchlist/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.544555 i8-terminal-0.2.93/i8_terminal/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/i8_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.548555 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-02 20:42:41.000000 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-02 20:42:41.000000 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:42:41.000000 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 20:42:41.000000 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 20:42:41.000000 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 20:42:41.000000 i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.548555 i8-terminal-0.2.93/i8_terminal/service_result/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/service_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/service_result/column_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/service_result/columns_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/service_result/earning_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/service_result/service_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.548555 i8-terminal-0.2.93/i8_terminal/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/services/earnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:42:41.548555 i8-terminal-0.2.93/i8_terminal/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/auto_complete_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/chart_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/fin_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/fin_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/fin_statement_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/i8_auto_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/i8_completer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/indicator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/market_indice_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/metric_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/metric_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/metric_view_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/output_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/period_type_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/price_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/screening_condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/screening_operator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/screening_value_field_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/sort_order_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/ticker_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/user_watchlist_tickers_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/types/user_watchlists_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/utils_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/i8_terminal/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 20:42:41.552555 i8-terminal-0.2.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-02 20:41:44.000000 i8-terminal-0.2.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/api/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/api/earnings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/app/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/app/plot_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/assets/i8t_chart_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/assets/i8t_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/assets/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/assets/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/commands/company/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/company/company_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/company/company_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/company/compnay_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/commands/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/earnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_upcoming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.024142 i8-terminal-0.2.94/i8_terminal/commands/financials/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/financials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/financials/financials_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/financials/financials_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/financials/financials_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/financials/financials_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/market/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/market/market_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/news/news_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/notebook/notebook_launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/price/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/price/price_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/price/price_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/price/price_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/screen/screen_gainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/screen/screen_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/screen/screen_losers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/screen/screen_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/user/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/user/user_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/user/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/commands/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.028142 i8-terminal-0.2.94/i8_terminal/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/i8_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-02 20:44:16.000000 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-02 20:44:16.000000 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:44:16.000000 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 20:44:16.000000 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 20:44:16.000000 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 20:44:16.000000 i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/i8_terminal/service_result/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/service_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/service_result/column_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/service_result/columns_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/service_result/earning_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/service_result/service_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/i8_terminal/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/services/earnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/i8_terminal/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/auto_complete_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/chart_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/fin_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/fin_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/fin_statement_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/i8_auto_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/i8_completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/indicator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/market_indice_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/metric_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/metric_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/metric_view_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/output_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/period_type_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/price_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/screening_condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/screening_operator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/screening_value_field_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/sort_order_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/ticker_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/user_watchlist_tickers_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/types/user_watchlists_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/utils_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/i8_terminal/version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 20:44:17.032142 i8-terminal-0.2.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-02 20:43:16.000000 i8-terminal-0.2.94/setup.py
```

### Comparing `i8-terminal-0.2.93/LICENSE` & `i8-terminal-0.2.94/LICENSE`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/PKG-INFO` & `i8-terminal-0.2.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.93
+Version: 0.2.94
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.93/README.md` & `i8-terminal-0.2.94/README.md`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/app/layout.py` & `i8-terminal-0.2.94/i8_terminal/app/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/app/plot_server.py` & `i8-terminal-0.2.94/i8_terminal/app/plot_server.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/assets/favicon.ico` & `i8-terminal-0.2.94/i8_terminal/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/assets/i8t_chart_logo.png` & `i8-terminal-0.2.94/i8_terminal/assets/i8t_chart_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/assets/i8t_logo.png` & `i8-terminal-0.2.94/i8_terminal/assets/i8t_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/assets/loading.gif` & `i8-terminal-0.2.94/i8_terminal/assets/loading.gif`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/assets/styles.css` & `i8-terminal-0.2.94/i8_terminal/assets/styles.css`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/company/company_compare.py` & `i8-terminal-0.2.94/i8_terminal/commands/company/company_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/company/company_search.py` & `i8-terminal-0.2.94/i8_terminal/commands/company/company_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/company/compnay_details.py` & `i8-terminal-0.2.94/i8_terminal/commands/company/compnay_details.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_list.py` & `i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_plot.py` & `i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_recent.py` & `i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_recent.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/earnings/earnings_upcoming.py` & `i8-terminal-0.2.94/i8_terminal/commands/earnings/earnings_upcoming.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/financials/financials_compare.py` & `i8-terminal-0.2.94/i8_terminal/commands/financials/financials_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/financials/financials_coverage.py` & `i8-terminal-0.2.94/i8_terminal/commands/financials/financials_coverage.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/financials/financials_list.py` & `i8-terminal-0.2.94/i8_terminal/commands/financials/financials_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/financials/financials_plot.py` & `i8-terminal-0.2.94/i8_terminal/commands/financials/financials_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/market/market_summary.py` & `i8-terminal-0.2.94/i8_terminal/commands/market/market_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_current.py` & `i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_current.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_describe.py` & `i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_describe.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_historical.py` & `i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_historical.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/metrics/metrics_search.py` & `i8-terminal-0.2.94/i8_terminal/commands/metrics/metrics_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/news/news_list.py` & `i8-terminal-0.2.94/i8_terminal/commands/news/news_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/notebook/notebook_launch.py` & `i8-terminal-0.2.94/i8_terminal/commands/notebook/notebook_launch.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/price/price_compare.py` & `i8-terminal-0.2.94/i8_terminal/commands/price/price_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/price/price_list.py` & `i8-terminal-0.2.94/i8_terminal/commands/price/price_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/price/price_plot.py` & `i8-terminal-0.2.94/i8_terminal/commands/price/price_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/screen/screen_gainers.py` & `i8-terminal-0.2.94/i8_terminal/commands/screen/screen_gainers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/screen/screen_losers.py` & `i8-terminal-0.2.94/i8_terminal/commands/screen/screen_losers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/screen/screen_search.py` & `i8-terminal-0.2.94/i8_terminal/commands/screen/screen_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/user/user_login.py` & `i8-terminal-0.2.94/i8_terminal/commands/user/user_login.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/user/webserver.py` & `i8-terminal-0.2.94/i8_terminal/commands/user/webserver.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_add.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_add.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_create.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_create.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_export.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_export.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_financials.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_list.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_metrics.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_metrics.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_rm.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_rm.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/commands/watchlist/watchlist_summary.py` & `i8-terminal-0.2.94/i8_terminal/commands/watchlist/watchlist_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/cli.py` & `i8-terminal-0.2.94/i8_terminal/common/cli.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/financials.py` & `i8-terminal-0.2.94/i8_terminal/common/financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/formatting.py` & `i8-terminal-0.2.94/i8_terminal/common/formatting.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/layout.py` & `i8-terminal-0.2.94/i8_terminal/common/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/metrics.py` & `i8-terminal-0.2.94/i8_terminal/common/metrics.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/price.py` & `i8-terminal-0.2.94/i8_terminal/common/price.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/screen.py` & `i8-terminal-0.2.94/i8_terminal/common/screen.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/stock_info.py` & `i8-terminal-0.2.94/i8_terminal/common/stock_info.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/common/utils.py` & `i8-terminal-0.2.94/i8_terminal/common/utils.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/config.py` & `i8-terminal-0.2.94/i8_terminal/config.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/config.yml` & `i8-terminal-0.2.94/i8_terminal/config.yml`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/PKG-INFO` & `i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.93
+Version: 0.2.94
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.93/i8_terminal/i8_terminal.egg-info/SOURCES.txt` & `i8-terminal-0.2.94/i8_terminal/i8_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/main.py` & `i8-terminal-0.2.94/i8_terminal/main.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/service_result/column_info.py` & `i8-terminal-0.2.94/i8_terminal/service_result/column_info.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/service_result/columns_context.py` & `i8-terminal-0.2.94/i8_terminal/service_result/columns_context.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/service_result/earning_list_result.py` & `i8-terminal-0.2.94/i8_terminal/service_result/earning_list_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/service_result/service_result.py` & `i8-terminal-0.2.94/i8_terminal/service_result/service_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/services/earnings.py` & `i8-terminal-0.2.94/i8_terminal/services/earnings.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/auto_complete_choice.py` & `i8-terminal-0.2.94/i8_terminal/types/auto_complete_choice.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/chart_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/chart_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/command_parser.py` & `i8-terminal-0.2.94/i8_terminal/types/command_parser.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/condition_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/fin_identifier_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/fin_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/fin_period_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/fin_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/fin_statement_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/fin_statement_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/i8_auto_suggest.py` & `i8-terminal-0.2.94/i8_terminal/types/i8_auto_suggest.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/i8_completer.py` & `i8-terminal-0.2.94/i8_terminal/types/i8_completer.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/indicator_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/indicator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/market_indice_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/market_indice_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/metric_identifier_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/metric_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/metric_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/metric_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/metric_view_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/metric_view_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/output_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/output_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/period_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/period_type_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/period_type_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/price_period_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/price_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/screening_condition_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/screening_condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/screening_operator_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/screening_operator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/screening_value_field_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/screening_value_field_param_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 def get_value_fields() -> List[Tuple[str, str]]:
     return [
         ("value_numeric", "Absolute Value Numeric"),
         ("value", "Absolute Value"),
         ("overall_rank", "Overall Rank"),
         ("spx_rank", "Spx Rank"),
         ("dow_rank", "Dow Rank"),
+        ("nasdaq_rank", "Nasdaq Rank"),
         ("sector_rank", "Sector Rank"),
         ("industry_rank", "Industry Rank"),
         ("overall_percentile", "Overall Percentile"),
         ("spx_percentile", "Spx Percentile"),
         ("nasdaq_percentile", "Nasdaq Percentile"),
         ("dow_percentile", "Dow Percentile"),
         ("sector_percentile", "Sector Percentile"),
```

### Comparing `i8-terminal-0.2.93/i8_terminal/types/sort_order_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/sort_order_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/ticker_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/ticker_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/user_watchlist_tickers_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/user_watchlist_tickers_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/types/user_watchlists_param_type.py` & `i8-terminal-0.2.94/i8_terminal/types/user_watchlists_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/i8_terminal/utils_setup.py` & `i8-terminal-0.2.94/i8_terminal/utils_setup.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.93/setup.py` & `i8-terminal-0.2.94/setup.py`

 * *Files identical despite different names*

